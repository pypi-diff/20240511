# Comparing `tmp/cyberiadaml_py-0.1.1.tar.gz` & `tmp/cyberiadaml_py-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberiadaml_py-0.1.1.tar", max compression
+gzip compressed data, was "cyberiadaml_py-1.0.tar", max compression
```

## Comparing `cyberiadaml_py-0.1.1.tar` & `cyberiadaml_py-1.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     7652 2024-03-07 13:29:23.021427 cyberiadaml_py-0.1.1/LICENSE
--rw-r--r--   0        0        0      528 2024-03-22 07:21:14.906906 cyberiadaml_py-0.1.1/README.md
--rw-r--r--   0        0        0       60 2024-03-07 13:29:03.825033 cyberiadaml_py-0.1.1/cyberiadaml_py/__init__.py
--rw-r--r--   0        0        0     9511 2024-03-22 07:11:56.037177 cyberiadaml_py-0.1.1/cyberiadaml_py/cyberiadaml_builder.py
--rw-r--r--   0        0        0    14779 2024-03-22 07:11:56.073176 cyberiadaml_py-0.1.1/cyberiadaml_py/cyberiadaml_parser.py
--rw-r--r--   0        0        0     2285 2024-03-22 07:11:56.089176 cyberiadaml_py-0.1.1/cyberiadaml_py/types/cgml_scheme.py
--rw-r--r--   0        0        0      382 2024-03-07 13:29:03.825033 cyberiadaml_py-0.1.1/cyberiadaml_py/types/common.py
--rw-r--r--   0        0        0     4144 2024-03-22 07:11:56.089176 cyberiadaml_py-0.1.1/cyberiadaml_py/types/elements.py
--rw-r--r--   0        0        0      710 2024-03-22 07:22:34.355150 cyberiadaml_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 cyberiadaml_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-03-07 13:29:23.021427 cyberiadaml_py-1.0/LICENSE
+-rw-r--r--   0        0        0      528 2024-04-27 07:05:27.455114 cyberiadaml_py-1.0/README.md
+-rw-r--r--   0        0        0       60 2024-03-07 13:29:03.825033 cyberiadaml_py-1.0/cyberiadaml_py/__init__.py
+-rw-r--r--   0        0        0    13273 2024-05-11 07:50:31.145555 cyberiadaml_py-1.0/cyberiadaml_py/cyberiadaml_builder.py
+-rw-r--r--   0        0        0    18064 2024-05-11 07:50:31.157550 cyberiadaml_py-1.0/cyberiadaml_py/cyberiadaml_parser.py
+-rw-r--r--   0        0        0     2596 2024-05-11 07:50:31.173543 cyberiadaml_py-1.0/cyberiadaml_py/types/cgml_scheme.py
+-rw-r--r--   0        0        0      338 2024-05-11 07:50:31.185538 cyberiadaml_py-1.0/cyberiadaml_py/types/common.py
+-rw-r--r--   0        0        0     5869 2024-05-11 07:50:31.185538 cyberiadaml_py-1.0/cyberiadaml_py/types/elements.py
+-rw-r--r--   0        0        0      354 2024-05-11 07:50:31.201532 cyberiadaml_py-1.0/cyberiadaml_py/utils.py
+-rw-r--r--   0        0        0      708 2024-05-11 07:51:08.714505 cyberiadaml_py-1.0/pyproject.toml
+-rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 cyberiadaml_py-1.0/PKG-INFO
```

### Comparing `cyberiadaml_py-0.1.1/LICENSE` & `cyberiadaml_py-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberiadaml_py-0.1.1/README.md` & `cyberiadaml_py-1.0/README.md`

 * *Files identical despite different names*

### Comparing `cyberiadaml_py-0.1.1/cyberiadaml_py/cyberiadaml_builder.py` & `cyberiadaml_py-1.0/cyberiadaml_py/cyberiadaml_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,214 +1,295 @@
 """Module implements building CyberiadaML schemes."""
-from typing import Dict, Iterable, List
+from typing import Dict, Iterable, List, Mapping
+from copy import deepcopy
+from itertools import chain
 
 from xmltodict import unparse
 from pydantic import RootModel
-
-try:
-    from cyberiadaml_py.types.cgml_scheme import (
-        CGML,
-        CGMLDataNode,
-        CGMLEdge,
-        CGMLGraph,
-        CGMLGraphml,
-        CGMLKeyNode,
-        CGMLNode
-    )
-    from cyberiadaml_py.types.common import Point, Rectangle
-    from cyberiadaml_py.types.elements import (
-        AwailableKeys,
-        CGMLComponent,
-        CGMLElements,
-        CGMLInitialState,
-        CGMLNote,
-        CGMLState,
-        CGMLTransition
-    )
-except ImportError:
-    from .types.cgml_scheme import (
-        CGML,
-        CGMLDataNode,
-        CGMLEdge,
-        CGMLGraph,
-        CGMLGraphml,
-        CGMLKeyNode,
-        CGMLNode
-    )
-    from .types.common import Point, Rectangle
-    from .types.elements import (
-        AwailableKeys,
-        CGMLComponent,
-        CGMLElements,
-        CGMLInitialState,
-        CGMLNote,
-        CGMLState,
-        CGMLTransition
-    )
+from cyberiadaml_py.types.cgml_scheme import (
+    CGMLNode,
+    CGMLPointNode,
+    CGMLRectNode,
+    CGML,
+    CGMLDataNode,
+    CGMLEdge,
+    CGMLGraph,
+    CGMLGraphml,
+    CGMLKeyNode,
+)
+from cyberiadaml_py.types.elements import (
+    CGMLBaseVertex,
+    CGMLInitialState,
+    CGMLMeta,
+    CGMLNoteType,
+    CGMLVertexType,
+    AvailableKeys,
+    CGMLComponent,
+    CGMLElements,
+    CGMLNote,
+    CGMLState,
+    CGMLTransition,
+    Vertex
+)
+from cyberiadaml_py.types.common import Point, Rectangle
+from cyberiadaml_py.utils import to_list
 
 
 class CGMLBuilderException(Exception):
     """Logical errors during building CGML scheme."""
 
     ...
 
 
 class CGMLBuilder:
     """Contains functions to build CGML scheme."""
 
     def __init__(self) -> None:
-        self.scheme: CGML = CGMLBuilder.createEmptyscheme()
+        self.scheme: CGML = CGMLBuilder.create_empty_scheme()
 
     @staticmethod
-    def createEmptyscheme() -> CGML:
+    def create_empty_scheme() -> CGML:
         """Create empty CyberiadaML scheme."""
         return CGML(graphml=CGMLGraphml(
             [],
             'http://graphml.graphdrawing.org/xmlns',
         ))
 
+    def _get_state_machine_datanode(self) -> CGMLDataNode:
+        return CGMLDataNode('dStateMachine')
+
     def build(self, elements: CGMLElements) -> str:
         """Build CGML scheme from elements."""
-        self.scheme.graphml.key = self._getKeys(elements.keys)
-        self.scheme.graphml.data = self._getFormatNode(elements.format)
         self.scheme.graphml.graph = CGMLGraph(
             'directed',
             'G',
+            data=self._get_state_machine_datanode()
+        )
+        cgml_states: Dict[str, CGMLNode] = self._get_state_nodes(
+            elements.states)
+        initials: List[CGMLNode] = self._get_vertex_nodes(
+            elements.initial_states, 'initial')
+        finals: List[CGMLNode] = self._get_vertex_nodes(
+            elements.finals, 'final')
+        terminates: List[CGMLNode] = self._get_vertex_nodes(
+            elements.terminates, 'terminate')
+        choices: List[CGMLNode] = self._get_vertex_nodes(
+            elements.choices, 'choice'
         )
-        nodes: List[CGMLNode] = [*self._getStateNodes(elements.states),
-                                 *self._getNoteNodes(
-                                     list(elements.notes.values())),
-                                 self._getMetaNode(
-                                     elements.meta, elements.platform),
-                                 *self._getComponentsNodes(elements.components)
-                                 ]
-        edges: List[CGMLEdge] = [
-            *self._getEdges(elements.transitions),
-            *self._getComponentsEdges(elements.components)
+        vertexes: Dict[str, Vertex] = (
+            elements.finals |
+            elements.choices |
+            elements.initial_states |
+            elements.terminates |
+            elements.unknown_vertexes
+        )
+        vertexes_nodes: List[CGMLNode] = list(
+            chain(initials, finals, terminates, choices))
+        states_with_vertexes, independent_vertexes = (
+            self._add_vertexes_to_states(
+                vertexes_nodes, vertexes, cgml_states)
+        )
+        nodes: List[CGMLNode] = [
+            *independent_vertexes,
+            *states_with_vertexes.values(),
+            self._get_meta_node(
+                elements.meta,
+                elements.platform,
+                elements.standard_version
+            ),
+            *self._get_components_nodes(elements.components),
+            *self._get_note_nodes(elements.notes)
         ]
-        if elements.initial_state is not None:
-            nodes.append(
-                self._getInitialNode(elements.initial_state))
-            edges.append(self._getInitialEdge(
-                elements.initial_state.transitionId,
-                elements.initial_state.id,
-                elements.initial_state.target))
+        edges: List[CGMLEdge] = self._get_edges(elements.transitions)
+        self.scheme.graphml.data = self._get_format_node(elements.format)
+        self.scheme.graphml.key = self._get_keys(elements.keys)
         self.scheme.graphml.graph.node = nodes
         self.scheme.graphml.graph.edge = edges
         scheme: CGML = RootModel[CGML](self.scheme).model_dump(
             by_alias=True, exclude_defaults=True)
         # У model_dump неправильный возвращаемый тип (CGML),
         # поэтому приходится явно показывать линтеру, что это dict
         if isinstance(scheme, dict):
             return unparse(scheme, pretty=True)
         else:
             raise CGMLBuilderException('Internal error: scheme is not dict')
 
-    def _getComponentsEdges(self,
-                            components: List[CGMLComponent]) -> List[CGMLEdge]:
-        edges: List[CGMLEdge] = []
-        for component in components:
-            edges.append(CGMLEdge(f'edge_{component.id}', '', component.id))
-        return edges
-
-    def _getComponentsNodes(self,
-                            components: List[CGMLComponent]) -> List[CGMLNode]:
+    def _get_vertex_nodes(self, vertexes: Mapping[str, Vertex],
+                          vertex_type: CGMLVertexType) -> List[CGMLNode]:
+        vertex_nodes: List[CGMLNode] = []
+        for vertex_id, vertex in vertexes.items():
+            vertex_node: CGMLNode = CGMLNode(vertex_id)
+            data: List[CGMLDataNode] = []
+            data.append(self._get_vertex_datanode(vertex_type))
+            if isinstance(vertex.position, Point):
+                data.append(self._point_to_data(vertex.position))
+            elif isinstance(vertex.position, Rectangle):
+                data.append(self._bounds_to_data(vertex.position))
+            vertex_node.data = data
+            vertex_nodes.append(vertex_node)
+        return vertex_nodes
+
+    def _add_vertexes_to_states(
+        self,
+        vertex_nodes: List[CGMLNode],
+        vertexes: Dict[str, Vertex],
+        cgml_states: Dict[str, CGMLNode]
+    ) -> tuple[Dict[str, CGMLNode], List[CGMLNode]]:
+        new_states = deepcopy(cgml_states)
+        independent_vertexes: List[CGMLNode] = []
+        for node in vertex_nodes:
+            vertex: CGMLBaseVertex = vertexes[node.id]
+            if vertex.parent is None:
+                independent_vertexes.append(node)
+                continue
+            parent_node: CGMLNode = new_states[vertex.parent]
+            if parent_node.graph is None:
+                parent_node.graph = CGMLGraph(
+                    f'g{parent_node.id}', node=[node])
+                continue
+            if isinstance(parent_node.graph, CGMLGraph):
+                graph_nodes = to_list(parent_node.graph.node)
+                graph_nodes.append(node)
+                parent_node.graph.node = graph_nodes
+            new_states[vertex.parent] = parent_node
+        return new_states, independent_vertexes
+
+    def _get_components_nodes(self,
+                              components: Dict[str, CGMLComponent]
+                              ) -> List[CGMLNode]:
         nodes: List[CGMLNode] = []
-        for component in components:
-            node: CGMLNode = CGMLNode(component.id)
+        for component_id, component in components.items():
+            node: CGMLNode = CGMLNode(component_id)
             data: List[CGMLDataNode] = []
-            data.append(self._nameToData(component.id))
-            data.append(self._actionsToData(component.parameters))
+            data.append(self._get_note_datanode('formal'))
+            data.append(self._name_to_data('CGML_COMPONENT'))
+            str_parameters = self._get_actions_string(
+                component.parameters | {'id': component.id,
+                                        'type': component.type
+                                        }
+            )
+            data.append(self._actions_to_data(str_parameters))
             node.data = data
             nodes.append(node)
         return nodes
 
-    def _getInitialEdge(self, transitionId: str,
-                        initId: str, target: str) -> CGMLEdge:
-        return CGMLEdge(
-            transitionId,
-            initId,
-            target
-        )
-
-    def _getEdges(self,
-                  transitions: Dict[str, CGMLTransition]) -> List[CGMLEdge]:
+    def _get_edges(self,
+                   transitions: Dict[str, CGMLTransition]) -> List[CGMLEdge]:
         edges: List[CGMLEdge] = []
         for transition in list(transitions.values()):
             edge: CGMLEdge = CGMLEdge(
                 transition.id, transition.source, transition.target)
             data: List[CGMLDataNode] = []
-            data.append(self._actionsToData(transition.actions))
+            data.append(self._actions_to_data(transition.actions))
             if transition.color is not None:
                 data.append(self._colorToData(transition.color))
-            if transition.position is not None:
-                data.append(self._pointToData(transition.position))
-            data.extend(transition.unknownDatanodes)
+            if isinstance(transition.position, Point):
+                data.append(self._point_to_data(transition.position))
+            if isinstance(transition.label_position, Point):
+                data.append(self._point_label(transition.label_position))
+            data.extend(transition.unknown_datanodes)
             edge.data = data
             edges.append(edge)
         return edges
 
-    def _getInitialNode(self, initialState: CGMLInitialState) -> CGMLNode:
-        initialNode: CGMLNode = CGMLNode(initialState.id)
+    def _get_vertex_datanode(
+            self,
+            vertex_type: CGMLVertexType
+    ) -> CGMLDataNode:
+        return CGMLDataNode('dVertex', vertex_type)
+
+    def _get_initial_nodes(
+            self,
+            initial_states: Dict[str, CGMLInitialState]
+    ) -> List[CGMLNode]:
+        initial_nodes: List[CGMLNode] = []
+        for initial_id, initial_state in initial_states.items():
+            initial_node: CGMLNode = CGMLNode(initial_id)
+            data: List[CGMLDataNode] = []
+            data.append(self._get_vertex_datanode('initial'))
+            if isinstance(initial_state.position, Point):
+                data.append(self._point_to_data(initial_state.position))
+            elif isinstance(initial_state.position, Rectangle):
+                data.append(self._bounds_to_data(initial_state.position))
+            initial_node.data = data
+            initial_nodes.append(initial_node)
+        return initial_nodes
+
+    def _get_actions_string(self, values: Dict[str, str]) -> str:
+        parameters = ''
+        for name, value in values.items():
+            parameters += f'{name}/{value}\n\n'
+        return parameters
+
+    def _get_note_datanode(self, note_type: CGMLNoteType) -> CGMLDataNode:
+        return CGMLDataNode('dNote', note_type)
+
+    def _get_meta_node(
+        self,
+        meta: CGMLMeta,
+        platform: str,
+        standard_version: str
+    ) -> CGMLNode:
+        meta_node: CGMLNode = CGMLNode(meta.id)
         data: List[CGMLDataNode] = []
-        if initialState.position is not None:
-            data.append(self._pointToData(initialState.position))
-        data.append(self._getInitialDataNode())
-        initialNode.data = data
-        return initialNode
-
-    def _getInitialDataNode(self) -> CGMLDataNode:
-        return CGMLDataNode(
-            'dInitial'
+        meta_parameters: str = self._get_actions_string(
+            meta.values | {
+                'platform': platform,
+                'standardVersion': standard_version
+            }
         )
+        data.append(self._get_note_datanode('formal'))
+        data.append(self._name_to_data('CGML_META'))
+        data.append(self._actions_to_data(meta_parameters))
+        meta_node.data = data
+        return meta_node
 
-    def _getMetaNode(self, meta: str, platform: str) -> CGMLNode:
-        metaNode: CGMLNode = CGMLNode('')
-        data: List[CGMLDataNode] = []
-        data.append(self._nameToData(platform))
-        data.append(self._actionsToData(meta))
-        metaNode.data = data
-        return metaNode
-
-    def _getNoteNodes(self, notes: List[CGMLNote]) -> List[CGMLNode]:
+    def _get_note_nodes(self, notes: Dict[str, CGMLNote]) -> List[CGMLNode]:
         nodes: List[CGMLNode] = []
-        for note in notes:
+        for note_id, note in notes.items():
             data: List[CGMLDataNode] = []
-            data.append(self._noteToData(note.text))
-            data.append(self._pointToData(note.position))
-            data.extend(note.unknownDatanodes)
+            data.append(self._get_note_datanode('informal'))
+            data.append(self._actions_to_data(note.text))
+            if isinstance(note.position, Point):
+                data.append(self._point_to_data(note.position))
+            else:
+                data.append(self._bounds_to_data(note.position))
+            data.extend(note.unknown_datanodes)
             nodes.append(CGMLNode(
-                note.id,
+                note_id,
                 data=data
             ))
         return nodes
 
-    def _pointToData(self, point: Point) -> CGMLDataNode:
+    def _point_label(self, point: Point) -> CGMLDataNode:
         return CGMLDataNode(
-            'dGeometry', None, str(point.x), str(point.y)
-        )
+            'dLabelGeometry', None, None, CGMLPointNode(point.x, point.y))
 
-    def _noteToData(self, note_information: str) -> CGMLDataNode:
-        return CGMLDataNode('dNote', note_information)
+    def _point_to_data(self, point: Point) -> CGMLDataNode:
+        return CGMLDataNode(
+            'dGeometry', None, None, CGMLPointNode(point.x, point.y))
 
-    def _getStateNodes(self, states: Dict[str, CGMLState]) -> List[CGMLNode]:
+    def _get_state_nodes(self,
+                         states: Dict[str, CGMLState]) -> Dict[str, CGMLNode]:
         def _getCGMLNode(nodes: Dict[str, CGMLNode],
                          state: CGMLState, stateId: str) -> CGMLNode:
             if nodes.get(stateId) is not None:
                 return nodes[stateId]
             else:
                 node = CGMLNode(stateId)
                 data: List[CGMLDataNode] = []
-                if state.bounds is not None:
-                    data.append(self._boundsToData(state.bounds))
+                if isinstance(state.bounds, Rectangle):
+                    data.append(self._bounds_to_data(state.bounds))
+                elif isinstance(state.bounds, Point):
+                    data.append(self._point_to_data(state.bounds))
                 if state.color is not None:
                     data.append(self._colorToData(state.color))
-                data.append(self._actionsToData(state.actions))
-                data.append(self._nameToData(state.name))
-                data.extend(state.unknownDatanodes)
+                data.append(self._actions_to_data(state.actions))
+                data.append(self._name_to_data(state.name))
+                data.extend(state.unknown_datanodes)
                 node.data = data
                 return node
 
         nodes: Dict[str, CGMLNode] = {}
         for stateId in list(states.keys()):
             state: CGMLState = states[stateId]
             node: CGMLNode = _getCGMLNode(nodes, state, stateId)
@@ -225,37 +306,41 @@
                             isinstance(parent.graph.node, Iterable)):
                         parent.graph.node.append(node)
                     else:
                         parent.graph.node = [node]
                 nodes[state.parent] = parent
             else:
                 nodes[stateId] = node
-        return list(nodes.values())
+        return nodes
 
-    def _nameToData(self, name: str) -> CGMLDataNode:
+    def _name_to_data(self, name: str) -> CGMLDataNode:
         return CGMLDataNode('dName', name)
 
     def _colorToData(self, color: str) -> CGMLDataNode:
         return CGMLDataNode('dColor', color)
 
-    def _actionsToData(self, actions: str) -> CGMLDataNode:
+    def _actions_to_data(self, actions: str) -> CGMLDataNode:
         return CGMLDataNode(
             'dData', actions
         )
 
-    def _boundsToData(self, bounds: Rectangle) -> CGMLDataNode:
-        return CGMLDataNode('dGeometry',
-                            None,
-                            str(bounds.x),
-                            str(bounds.y),
-                            str(bounds.width),
-                            str(bounds.height))
+    def _bounds_to_data(self, bounds: Rectangle) -> CGMLDataNode:
+        return CGMLDataNode(
+            'dGeometry',
+            None,
+            CGMLRectNode(
+                bounds.x,
+                bounds.y,
+                bounds.width,
+                bounds.height
+            )
+        )
 
-    def _getFormatNode(self, format: str) -> CGMLDataNode:
+    def _get_format_node(self, format: str) -> CGMLDataNode:
         return CGMLDataNode('gFormat', format)
 
-    def _getKeys(self, awaialaibleKeys: AwailableKeys) -> List[CGMLKeyNode]:
+    def _get_keys(self, awaialaibleKeys: AvailableKeys) -> List[CGMLKeyNode]:
         keyNodes: List[CGMLKeyNode] = []
         for key in list(awaialaibleKeys.keys()):
             keyNodes.extend(awaialaibleKeys[key])
 
         return keyNodes
```

### Comparing `cyberiadaml_py-0.1.1/cyberiadaml_py/cyberiadaml_parser.py` & `cyberiadaml_py-1.0/cyberiadaml_py/cyberiadaml_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 """The module implements parsing CyberiadaML schemes."""
 from collections import defaultdict
 from collections.abc import Iterable
-from typing import Any, Dict, List, Optional
+from typing import (
+    DefaultDict,
+    Dict,
+    List,
+    Optional,
+    get_args,
+    TypeGuard,
+    TypeVar
+)
 
 from xmltodict import parse
+from cyberiadaml_py.utils import to_list
+from cyberiadaml_py.types.cgml_scheme import (
+    CGMLDataNode,
+    CGMLKeyNode,
+    CGMLPointNode,
+    CGML,
+    CGMLEdge,
+    CGMLGraph,
+    CGMLNode
+)
+from cyberiadaml_py.types.elements import (
+    CGMLBaseVertex,
+    CGMLChoice,
+    CGMLFinal,
+    CGMLMeta,
+    CGMLNoteType,
+    CGMLTerminate,
+    CGMLVertexType,
+    CGMLComponent,
+    CGMLElements,
+    AvailableKeys,
+    CGMLInitialState,
+    CGMLNote,
+    CGMLState,
+    CGMLTransition
+)
+from cyberiadaml_py.types.common import Point, Rectangle
 
-try:
-    from .types.common import Point, Rectangle
-    from .types.cgml_scheme import (
-        CGML,
-        CGMLDataNode,
-        CGMLEdge,
-        CGMLGraph,
-        CGMLNode
-    )
-    from .types.elements import (
-        CGMLComponent,
-        CGMLElements,
-        AwailableKeys,
-        CGMLInitialState,
-        CGMLNote,
-        CGMLState,
-        CGMLTransition
-    )
-except ImportError:
-    from cyberiadaml_py.types.cgml_scheme import (
-        CGML,
-        CGMLDataNode,
-        CGMLEdge,
-        CGMLGraph,
-        CGMLNode
-    )
-    from cyberiadaml_py.types.common import Point, Rectangle
-    from cyberiadaml_py.types.elements import (
-        CGMLComponent,
-        CGMLElements,
-        AwailableKeys,
-        CGMLInitialState,
-        CGMLNote,
-        CGMLState,
-        CGMLTransition
-    )
+ListType = TypeVar('ListType')
 
 
 class CGMLParserException(Exception):
     """Logical errors during parsing CGML scheme."""
 
     ...
 
@@ -57,315 +57,406 @@
 
     @staticmethod
     def createEmptyElements() -> CGMLElements:
         """Create CGMLElements with empty fields."""
         return CGMLElements(
             states={},
             transitions={},
-            components=[],
+            finals={},
+            choices={},
+            terminates={},
+            initial_states={},
+            standard_version='',
+            components={},
             platform='',
             format='',
-            meta='',
+            meta=CGMLMeta(
+                id='',
+                values={},
+            ),
             keys=defaultdict(),
-            notes={}
+            notes={},
+            unknown_vertexes={}
         )
 
-    def parseCGML(self, graphml: str) -> CGMLElements:
+    def parse_cgml(self, graphml: str) -> CGMLElements:
         """
         Parse CyberiadaGraphml scheme.
 
         Args:
             graphml (str): CyberiadaML scheme.
 
         Returns:
             CGMLElements: notes, states, transitions,\
                 initial state and components
         Raises:
             CGMLParserException('Data node with key "gFormat" is empty'):\
                 content of <data key='gFormat'> is None
             CGMLParserException('Data node with key "gFormat" is missing'):\
-                <data key='gFormat'> doesn't exist in graphml->data.s
+                <data key='gFormat'> doesn't exist in graphml->data
             CGMLParserException('No position for note!):\
                 <node>, that contains <data key='dNote'>, graphml
-                    doesn't contains <data key='dGeometry' x='...' y='...'>
-            CGMLParserException('Unknown key "key" for "node-type",\
-                                    did you forgot ...'):\
-                                        using an undeclarated key
-            CGMLParserException('<node-type> with key\
-                dGeometry doesnt have x, y properties'): \
-                    <data key='dGeometry'> must contain at least x and y\
-                        properties (width and height are additional)
+                    doesn't contains <data key='dGeometry'>
             ValidationError(...): pydatinc's validation error, occurs when\
                 the scheme doesn't match the format.
         """
         self.elements = CGMLParser.createEmptyElements()
         cgml = CGML(**parse(graphml))
-        self.elements.format = self._getFormat(cgml)
-        if self.elements.format != 'Cyberiada-GraphML':
-            raise CGMLParserException(
-                ('Format must be '
-                 f'Cyberiada-GraphML, but got {self.elements.format}'))
-        self.elements.keys = self._getAwaialbleKeys(cgml)
-        graphs: List[CGMLGraph] = self._toList(cgml.graphml.graph)
+        format: str = self._get_format(cgml)
+        keys: DefaultDict[str, List[CGMLKeyNode]
+                          ] = self._get_available_keys(cgml)
+        platform = ''
+        standard_version = ''
+        graphs: List[CGMLGraph] = to_list(cgml.graphml.graph)
         states: Dict[str, CGMLState] = {}
         transitions: Dict[str, CGMLTransition] = {}
         notes: Dict[str, CGMLNote] = {}
+        terminates: Dict[str, CGMLTerminate] = {}
+        finals: Dict[str, CGMLFinal] = {}
+        choices: Dict[str, CGMLChoice] = {}
+        initials: Dict[str, CGMLInitialState] = {}
+        unknown_vertexes: Dict[str, CGMLBaseVertex] = {}
+        meta: CGMLMeta = CGMLMeta(
+            id='',
+            values={}
+        )
+        components: Dict[str, CGMLComponent] = {}
+        vertex_dicts: Dict[CGMLVertexType,
+                           tuple[Dict[str, CGMLInitialState], type] |
+                           tuple[Dict[str, CGMLFinal], type] |
+                           tuple[Dict[str, CGMLChoice], type] |
+                           tuple[Dict[str, CGMLTerminate], type]] = {
+            'initial': (initials, CGMLInitialState),
+            'choice': (choices, CGMLChoice),
+            'final': (finals, CGMLFinal),
+            'terminate': (terminates, CGMLTerminate)
+        }
         for graph in graphs:
-            states = states | self._parseGraphNodes(graph)
-            transitions = transitions | self._parseGraphEdges(graph)
-        try:
-            self.elements.platform, self.elements.meta = self._getMeta(
-                states[''])
-            del states['']
-        except KeyError:
-            raise CGMLParserException('Meta node is missing')
-        for stateId in list(states.keys()):
-            state, isInit = self._processStateData(states[stateId], stateId)
+            states = states | self._parse_graph_nodes(graph)
+            transitions = transitions | self._parse_graph_edges(graph)
+        for state_id in list(states.keys()):
+            state = self._process_state_data(states[state_id])
             if isinstance(state, CGMLNote):
-                notes[state.id] = state
-                del states[stateId]
+                note = state
+                del states[state_id]
+                if note.type == 'informal':
+                    notes[state_id] = state
+                    continue
+
+                match note.name:
+                    case 'CGML_META':
+                        meta.id = state_id
+                        meta.values = self._parse_meta(note.text)
+                        try:
+                            platform = meta.values['platform']
+                            standard_version = meta.values['standardVersion']
+                        except KeyError:
+                            raise CGMLParserException(
+                                'No platform or standardVersion.')
+                    case 'CGML_COMPONENT':
+                        component_parameters: Dict[str, str] = (
+                            self._parse_meta(
+                                note.text
+                            )
+                        )
+                        try:
+                            component_id = component_parameters['id'].strip()
+                            component_type = (
+                                component_parameters['type'].strip())
+                            del component_parameters['id']
+                            del component_parameters['type']
+                        except KeyError:
+                            raise CGMLParserException(
+                                "Component doesn't have type or id.")
+                        components[state_id] = CGMLComponent(
+                            id=component_id,
+                            type=component_type,
+                            parameters=component_parameters
+                        )
             elif isinstance(state, CGMLState):
-                if isInit:
-                    if self.elements.initial_state is not None:
-                        raise CGMLParserException('Double init states')
-                    position: Point | None = None
-                    if state.bounds is not None:
-                        position = Point(state.bounds.x, state.bounds.y)
-                    self.elements.initial_state = CGMLInitialState(
-                        transitionId='', id=stateId,
-                        target='', position=position)
-                    del states[stateId]
+                states[state_id] = state
+            elif isinstance(state, CGMLBaseVertex):
+                vertex = state
+                del states[state_id]
+                if self.__is_vertex_type(vertex.type):
+                    vertex_dict, vertex_type = vertex_dicts[vertex.type]
+                    vertex_dict[state_id] = vertex_type(
+                        type=vertex.type,
+                        data=vertex.data,
+                        position=vertex.position,
+                        parent=vertex.parent
+                    )
                 else:
-                    states[stateId] = state
+                    unknown_vertexes[state_id] = CGMLBaseVertex(
+                        vertex.type,
+                        vertex.data,
+                        vertex.position,
+                        vertex.parent
+                    )
             else:
                 raise CGMLParserException(
                     'Internal error: Unknown type of node')
-        # TODO Вынести в отдельные функции
-        componentIds: List[str] = []
+
+        component_ids: List[str] = []
         for transition in list(transitions.values()):
-            processedTransition: CGMLTransition = self._processEdgeData(
+            processedTransition: CGMLTransition = self._process_edge_data(
                 transition)
-            if (self.elements.initial_state is not None and
-                    (processedTransition.source ==
-                        self.elements.initial_state.id)):
-                self.elements.initial_state.target = processedTransition.target
-                self.elements.initial_state\
-                    .transitionId = processedTransition.id
-            elif transition.source == '':
-                componentIds.append(transition.target)
+            if transition.source == meta.id:
+                component_ids.append(transition.id)
             else:
-                self.elements.transitions[transition.id] = processedTransition
-        for componentId in componentIds:
-            componentState: CGMLState | None = states.get(componentId)
-            if componentState is None:
-                raise CGMLParserException('Unknown component node')
-            self.elements.components.append(CGMLComponent(
-                id=componentId,
-                parameters=componentState.actions
-            ))  # TODO: raise exception if smth else
-            del states[componentId]
+                transitions[transition.id] = processedTransition
+
+        for component_id in component_ids:
+            del transitions[component_id]
+        self.elements.meta = meta
         self.elements.states = states
         self.elements.notes = notes
+        self.elements.choices = choices
+        self.elements.finals = finals
+        self.elements.initial_states = initials
+        self.elements.keys = keys
+        self.elements.transitions = transitions
+        self.elements.components = components
+        self.elements.format = format
+        self.elements.platform = platform
+        self.elements.standard_version = standard_version
         return self.elements
 
-    def _getDataContent(self, dataNode: CGMLDataNode) -> str:
-        return dataNode.content if dataNode.content is not None else ''
-
-    def _processEdgeData(self, transition: CGMLTransition) -> CGMLTransition:
-        newTransition = CGMLTransition(
+    def _parse_meta(self, meta: str) -> Dict[str, str]:
+        splited_parameters: List[str] = meta.split('\n\n')
+        parameters: Dict[str, str] = {}
+        for parameter in splited_parameters:
+            parameter_name, parameter_value = parameter.split('/')
+            parameters[parameter_name.strip()] = parameter_value.strip()
+        return parameters
+
+    def _get_data_content(self, data_node: CGMLDataNode) -> str:
+        return data_node.content if data_node.content is not None else ''
+
+    def _process_edge_data(self, transition: CGMLTransition) -> CGMLTransition:
+        new_transition = CGMLTransition(
+            position=[],
             id=transition.id,
             source=transition.source,
             target=transition.target,
             actions=transition.actions,
-            unknownDatanodes=[]
+            unknown_datanodes=[]
         )
-        for dataNode in transition.unknownDatanodes:
-            for keyNode in self.elements.keys['edge']:
-                if dataNode.key == keyNode.id:
-                    break
-            else:
-                raise CGMLParserException(
-                    (f'Unknown key {dataNode.key} for edge, did you forgot: '
-                     f'"<key id="{dataNode.key}" for="edge"/>"?'))
-            match dataNode.key:
+        for data_node in transition.unknown_datanodes:
+            match data_node.key:
                 case 'dData':
-                    newTransition.actions = self._getDataContent(dataNode)
+                    new_transition.actions = self._get_data_content(data_node)
                 case 'dGeometry':
-                    if dataNode.x is None or dataNode.y is None:
+                    if data_node.point is None:
                         raise CGMLParserException(
                             'Edge with key dGeometry\
-                                doesnt have x, y properties')
-                    newTransition.position = Point(
-                        float(dataNode.x), float(dataNode.y))
+                                doesnt have <point> node.')
+                    points: List[CGMLPointNode] = (
+                        to_list(data_node.point)
+                    )
+                    for point in points:
+                        new_transition.position.append(Point(
+                            x=point.x, y=point.y))
                 case 'dColor':
-                    newTransition.color = self._getDataContent(dataNode)
+                    new_transition.color = self._get_data_content(data_node)
+                case 'dLabelGeometry':
+                    if data_node.point is None:
+                        raise CGMLParserException(
+                            'Edge with key dGeometry\
+                                doesnt have <point> node.')
+                    if isinstance(data_node.point, list):
+                        raise CGMLParserException(
+                            'dLabelGeometry with several points!')
+                    point = data_node.point
+                    new_transition.label_position = Point(
+                        x=point.x, y=point.y)
                 case _:
-                    newTransition.unknownDatanodes.append(dataNode)
-        return newTransition
+                    new_transition.unknown_datanodes.append(data_node)
+        return new_transition
+
+    def __is_note_type(self, value: str) -> TypeGuard[CGMLNoteType]:
+        return value in get_args(CGMLNoteType)
 
-    def _processStateData(self,
-                          state: CGMLState,
-                          stateId: str) -> tuple[CGMLState | CGMLNote, bool]:
+    def _get_note_type(self, value: str) -> CGMLNoteType:
+        if self.__is_note_type(value):
+            return value
+        raise CGMLParserException(
+            f'Unknown type of note! Expect {get_args(CGMLNoteType)}.')
+
+    def __is_vertex_type(self, value: str) -> TypeGuard[CGMLVertexType]:
+        return value in get_args(CGMLVertexType)
+
+    def _process_state_data(self,
+                            state: CGMLState
+                            ) -> CGMLState | CGMLNote | CGMLBaseVertex:
         """Return tuple[CGMLState | CGMLNote, isInit]."""
         # no mutations? B^)
-        newState = CGMLState(
+        new_state = CGMLState(
             name=state.name,
             actions=state.actions,
-            unknownDatanodes=[],
+            unknown_datanodes=[],
             bounds=state.bounds,
             parent=state.parent
         )
-        isNote: bool = False
-        isInit: bool = False
-        for dataNode in state.unknownDatanodes:
-            match dataNode.key:
+        note_type: Optional[CGMLNoteType] = None
+        vertex_type: Optional[str] = None
+        is_note = False
+        is_vertex = False
+        for data_node in state.unknown_datanodes:
+            match data_node.key:
                 case 'dName':
-                    newState.name = self._getDataContent(dataNode)
+                    new_state.name = self._get_data_content(data_node)
                 case 'dGeometry':
-                    if dataNode.x is None or dataNode.y is None:
+                    if data_node.rect is None and data_node.point is None:
                         raise CGMLParserException(
                             'Node with key dGeometry\
-                                doesnt have x, y properties')
-                    x: float = float(dataNode.x)
-                    y: float = float(dataNode.y)
-
-                    if (dataNode.width is not None and
-                            dataNode.height is not None):
-                        newState.bounds = Rectangle(
-                            x=x,
-                            y=y,
-                            width=float(dataNode.width),
-                            height=float(dataNode.height)
-                        )
-                    else:
-                        newState.bounds = Rectangle(
-                            x=x,
-                            y=y
+                                doesnt have rect or point child')
+                    if data_node.point is not None:
+                        if isinstance(data_node.point, list):
+                            raise CGMLParserException(
+                                "State doesn't support several points.")
+                        new_state.bounds = Point(x=data_node.point.x,
+                                                 y=data_node.point.y)
+                        continue
+
+                    if (data_node.rect is not None):
+                        new_state.bounds = Rectangle(
+                            x=data_node.rect.x,
+                            y=data_node.rect.y,
+                            width=data_node.rect.width,
+                            height=data_node.rect.height
                         )
+                case 'dVertex':
+                    is_vertex = True
+                    vertex_type = self._get_data_content(data_node)
                 case 'dData':
-                    newState.actions = self._getDataContent(dataNode)
+                    new_state.actions = self._get_data_content(data_node)
                 case 'dNote':
-                    isNote = True
-                    newState.actions = self._getDataContent(dataNode)
-                case 'dInitial':
-                    isInit = True
-                    if isNote:
-                        raise CGMLParserException('dInit in dNote')
+                    is_note = True
+                    if data_node.content is None:
+                        note_type = 'informal'
+                    else:
+                        note_type = self._get_note_type(
+                            self._get_data_content(data_node))
                 case 'dColor':
-                    newState.color = self._getDataContent(dataNode)
+                    new_state.color = self._get_data_content(data_node)
                 case _:
-                    newState.unknownDatanodes.append(dataNode)
-        if isNote:
-            bounds: Rectangle | None = newState.bounds
+                    new_state.unknown_datanodes.append(data_node)
+        if is_note and note_type is not None:
+            bounds: Optional[Rectangle | Point] = new_state.bounds
+            x = 0.
+            y = 0.
             if bounds is None:
-                raise CGMLParserException('No position for note!')
+                if note_type == 'informal':
+                    raise CGMLParserException('No position for note!')
             else:
-                return (CGMLNote(
-                    id=stateId,
-                    position=Point(
-                        x=bounds.x,
-                        y=bounds.y,
-                    ),
-                    text=newState.actions,
-                    unknownDatanodes=newState.unknownDatanodes
-                ), False)
-        return (newState, isInit)
+                x = bounds.x
+                y = bounds.y
+            return CGMLNote(
+                parent=new_state.parent,
+                name=new_state.name,
+                position=Point(
+                    x=x,
+                    y=y,
+                ),
+                type=note_type,
+                text=new_state.actions,
+                unknown_datanodes=new_state.unknown_datanodes
+            )
+        if is_vertex and vertex_type is not None:
+            return CGMLBaseVertex(
+                type=vertex_type,
+                position=new_state.bounds,
+                parent=new_state.parent
+            )
+        return new_state
 
-    def _getMeta(self, metaNode: CGMLState) -> tuple[str, str]:
+    def _get_meta(self, metaNode: CGMLState) -> tuple[str, str]:
         """Return tuple[platfrom, meta]."""
-        dataNodes: List[CGMLDataNode] = self._toList(metaNode.unknownDatanodes)
+        dataNodes: List[CGMLDataNode] = to_list(
+            metaNode.unknown_datanodes)
         platform: str = ''
         meta: str = ''
-        for dataNode in dataNodes:
-            match dataNode.key:
+        for data_node in dataNodes:
+            match data_node.key:
                 case 'dName':
-                    platform = self._getDataContent(dataNode)
+                    platform = self._get_data_content(data_node)
                 case 'dData':
-                    meta = self._getDataContent(dataNode)
+                    meta = self._get_data_content(data_node)
         return platform, meta
 
-    def _toList(self, nodes: List | None | Any) -> List:
-        if nodes is None:
-            return []
-        if isinstance(nodes, list):
-            return nodes
-        else:
-            return [nodes]
-
-    def _parseGraphEdges(self, root: CGMLGraph) -> Dict[str, CGMLTransition]:
+    def _parse_graph_edges(self, root: CGMLGraph) -> Dict[str, CGMLTransition]:
         def _parseEdge(edge: CGMLEdge,
                        cgmlTransitions: Dict[str, CGMLTransition]) -> None:
             cgmlTransitions[edge.id] = CGMLTransition(
                 id=edge.id,
                 source=edge.source,
                 target=edge.target,
                 actions='',
-                unknownDatanodes=self._toList(
+                unknown_datanodes=to_list(
                         edge.data),
             )
 
         cgmlTransitions: Dict[str, CGMLTransition] = {}
         if root.edge is not None:
             if isinstance(root.edge, Iterable):
                 for edge in root.edge:
                     _parseEdge(edge, cgmlTransitions)
             else:
                 _parseEdge(root.edge, cgmlTransitions)
         return cgmlTransitions
 
-    def _parseGraphNodes(self,
-                         root: CGMLGraph,
-                         parent: Optional[str] = None) -> Dict[str, CGMLState]:
+    def _parse_graph_nodes(
+        self,
+        root: CGMLGraph,
+        parent: Optional[str] = None
+    ) -> Dict[str, CGMLState]:
         def parseNode(node: CGMLNode) -> Dict[str, CGMLState]:
             cgmlStates: Dict[str, CGMLState] = {}
             cgmlStates[node.id] = CGMLState(
                 name='',
                 actions='',
-                unknownDatanodes=self._toList(node.data),
+                unknown_datanodes=to_list(node.data),
             )
             if parent is not None:
                 cgmlStates[node.id].parent = parent
-            graphs: List[CGMLGraph] = self._toList(node.graph)
+            graphs: List[CGMLGraph] = to_list(node.graph)
             for graph in graphs:
-                cgmlStates = cgmlStates | self._parseGraphNodes(
+                cgmlStates = cgmlStates | self._parse_graph_nodes(
                     graph, node.id)
 
             return cgmlStates
 
         cgmlStates: Dict[str, CGMLState] = {}
         if root.node is not None:
             if isinstance(root.node, Iterable):
                 for node in root.node:
                     cgmlStates = cgmlStates | parseNode(node)
             else:
                 cgmlStates = cgmlStates | parseNode(root.node)
         return cgmlStates
 
-    def _checkDataNodeKey(self, node_name: str, key: str,
-                          awaialableKeys: AwailableKeys) -> bool:
-        return key in awaialableKeys[node_name]
-
     # key nodes to comfortable dict
-    def _getAwaialbleKeys(self, cgml: CGML) -> AwailableKeys:
-        keyNodeDict: AwailableKeys = defaultdict(lambda: [])
+    def _get_available_keys(self, cgml: CGML) -> AvailableKeys:
+        keyNodeDict: AvailableKeys = defaultdict(lambda: [])
         if cgml.graphml.key is not None:
             if isinstance(cgml.graphml.key, Iterable):
                 for keyNode in cgml.graphml.key:
                     keyNodeDict[keyNode.for_].append(keyNode)
             else:
                 keyNodeDict[cgml.graphml.key.for_].append(cgml.graphml.key)
         return keyNodeDict
 
-    def _getFormat(self, cgml: CGML) -> str:
+    def _get_format(self, cgml: CGML) -> str:
         # TODO: DRY
         if isinstance(cgml.graphml.data, Iterable):
-            for dataNode in cgml.graphml.data:
-                if dataNode.key == 'gFormat':
-                    if dataNode.content is not None:
-                        return dataNode.content
+            for data_node in cgml.graphml.data:
+                if data_node.key == 'gFormat':
+                    if data_node.content is not None:
+                        return data_node.content
                     raise CGMLParserException(
                         'Data node with key "gFormat" is empty')
         else:
             if cgml.graphml.data.key == 'gFormat':
                 if cgml.graphml.data.content is not None:
                     return cgml.graphml.data.content
                 raise CGMLParserException(
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cyberiadaml_py-0.1.1/cyberiadaml_py/types/cgml_scheme.py` & `cyberiadaml_py-1.0/cyberiadaml_py/types/cgml_scheme.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,68 +2,85 @@
 
 from typing import List, Optional
 
 from pydantic.dataclasses import dataclass
 from pydantic import Field, ConfigDict
 
 
+@dataclass
+class CGMLRectNode:
+    """The type represents <rect> node."""
+
+    x: float = Field(alias='@x')
+    y: float = Field(alias='@y')
+    width: float = Field(alias='@width')
+    height: float = Field(alias='@height')
+
+
+@dataclass
+class CGMLPointNode:
+    """The type represents <point> node."""
+
+    x: float = Field(alias='@x')
+    y: float = Field(alias='@y')
+
+
 @dataclass(config=ConfigDict(extra='forbid'))
 class CGMLDataNode:
-    """Type representing <data> node."""
+    """The type represents <data> node."""
 
     key: str = Field(alias='@key')
     content: Optional[str] = Field(default=None, alias='#text')
-    x: Optional[str] = Field(default=None, alias='@x')
-    y: Optional[str] = Field(default=None, alias='@y')
-    width: Optional[str] = Field(default=None, alias='@width')
-    height: Optional[str] = Field(default=None, alias='@height')
+    rect: Optional[CGMLRectNode] = None
+    point: Optional[CGMLPointNode | List[CGMLPointNode]] = None
 
 
 @dataclass(config=ConfigDict(extra='allow'))
 class CGMLKeyNode:
-    """Type representing <key> node."""
+    """The type represents <key> node."""
 
     id: str = Field(alias='@id')
     for_: str = Field(alias='@for')
     attr_name: Optional[str] = Field(default=None, alias='@attr.name')
     attr_type: Optional[str] = Field(default=None, alias='@attr.type')
 
 
 @dataclass(config=ConfigDict(extra='forbid'))
 class CGMLEdge:
-    """Type representing <edge> node."""
+    """The type represents <edge> node."""
 
     id: str = Field(alias='@id')
     source: str = Field(alias='@source')
     target: str = Field(alias='@target')
     data: Optional[List[CGMLDataNode] | CGMLDataNode] = None
 
 
 @dataclass(config=ConfigDict(extra='forbid'))
 class CGMLGraph:
-    """Type representing <graph> node."""
+    """The type represents <graph> node."""
 
     edgedefault: Optional[str] = Field(alias='@edgedefault', default=None)
     id: Optional[str] = Field(alias='@id', default=None)
     node: Optional[List['CGMLNode'] | 'CGMLNode'] = None
     edge: Optional[List[CGMLEdge] | CGMLEdge] = None
+    data: Optional[List[CGMLDataNode] | CGMLDataNode] = None
 
 
 @dataclass(config=ConfigDict(extra='forbid'))
 class CGMLNode:
-    """Type representing <node> node."""
+    """The type represents <node> node."""
 
     id: str = Field(alias='@id')
     graph: Optional[CGMLGraph | List[CGMLGraph]] = None
     data: List[CGMLDataNode] | CGMLDataNode | None = None
 
 
 @dataclass(config=ConfigDict(extra='forbid'))
 class CGMLGraphml:
-    """Type representing <graphml> node."""
+    """The type represents <graphml> node."""
 
     data: CGMLDataNode | List[CGMLDataNode]
     xmlns: str = Field(alias='@xmlns')
     key: Optional[List[CGMLKeyNode] | CGMLKeyNode] = None
     graph: Optional[List[CGMLGraph] | CGMLGraph] = None
```

### Comparing `cyberiadaml_py-0.1.1/pyproject.toml` & `cyberiadaml_py-1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyberiadaml-py"
-version = "0.1.1"
+version = "1.0"
 description = "The Python 3 library for processing the CyberiadaML state machine graphs"
 authors = ["L140-beep <kartoshka0302@mail.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.10"
 xmltodict = "^0.13.0"
```

### Comparing `cyberiadaml_py-0.1.1/PKG-INFO` & `cyberiadaml_py-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberiadaml-py
-Version: 0.1.1
+Version: 1.0
 Summary: The Python 3 library for processing the CyberiadaML state machine graphs
 Author: L140-beep
 Author-email: kartoshka0302@mail.ru
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
```

