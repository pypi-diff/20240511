# Comparing `tmp/operagents-0.0.8.tar.gz` & `tmp/operagents-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operagents-0.0.8.tar", max compression
+gzip compressed data, was "operagents-0.0.9.tar", max compression
```

## Comparing `operagents-0.0.8.tar` & `operagents-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11338 2024-03-22 04:08:33.245904 operagents-0.0.8/LICENSE
--rw-r--r--   0        0        0     5585 2024-03-22 04:08:33.245904 operagents-0.0.8/README.md
--rw-r--r--   0        0        0       91 2024-03-22 04:08:33.245904 operagents-0.0.8/operagents/__init__.py
--rw-r--r--   0        0        0       30 2024-03-22 04:08:33.245904 operagents-0.0.8/operagents/__main__.py
--rw-r--r--   0        0        0     7796 2024-03-22 04:08:33.245904 operagents-0.0.8/operagents/agent/__init__.py
--rw-r--r--   0        0        0     3321 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/agent/memory.py
--rw-r--r--   0        0        0      858 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/backend/__init__.py
--rw-r--r--   0        0        0     2261 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/backend/_base.py
--rw-r--r--   0        0        0     4571 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/backend/openai.py
--rw-r--r--   0        0        0      851 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/backend/user.py
--rw-r--r--   0        0        0     1548 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/character/__init__.py
--rw-r--r--   0        0        0     1604 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/cli/__init__.py
--rw-r--r--   0        0        0     8575 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/config/__init__.py
--rw-r--r--   0        0        0      740 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/config/const.py
--rw-r--r--   0        0        0      682 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/director/__init__.py
--rw-r--r--   0        0        0      717 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/director/_base.py
--rw-r--r--   0        0        0     2770 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/director/model.py
--rw-r--r--   0        0        0      659 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/director/never.py
--rw-r--r--   0        0        0     1186 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/director/user.py
--rw-r--r--   0        0        0      797 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/exception.py
--rw-r--r--   0        0        0      604 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/flow/__init__.py
--rw-r--r--   0        0        0      871 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/flow/_base.py
--rw-r--r--   0        0        0     3486 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/flow/model.py
--rw-r--r--   0        0        0     1397 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/flow/order.py
--rw-r--r--   0        0        0     1458 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/flow/user.py
--rw-r--r--   0        0        0     1275 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/log.py
--rw-r--r--   0        0        0     1278 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/opera/__init__.py
--rw-r--r--   0        0        0      532 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/prop/__init__.py
--rw-r--r--   0        0        0     2033 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/prop/_base.py
--rw-r--r--   0        0        0     1818 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/prop/function.py
--rw-r--r--   0        0        0     1681 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/scene/__init__.py
--rw-r--r--   0        0        0      720 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/scene/prepare/__init__.py
--rw-r--r--   0        0        0      710 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/scene/prepare/_base.py
--rw-r--r--   0        0        0      820 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/scene/prepare/function.py
--rw-r--r--   0        0        0     1126 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/scene/prepare/preface.py
--rw-r--r--   0        0        0     5530 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/timeline/__init__.py
--rw-r--r--   0        0        0      476 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/timeline/event.py
--rw-r--r--   0        0        0     1621 2024-03-22 04:08:33.249904 operagents-0.0.8/operagents/utils.py
--rw-r--r--   0        0        0     1953 2024-03-22 04:08:33.249904 operagents-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6460 1970-01-01 00:00:00.000000 operagents-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-03-24 06:47:17.191728 operagents-0.0.9/LICENSE
+-rw-r--r--   0        0        0    13342 2024-03-24 06:47:17.191728 operagents-0.0.9/README.md
+-rw-r--r--   0        0        0       91 2024-03-24 06:47:17.191728 operagents-0.0.9/operagents/__init__.py
+-rw-r--r--   0        0        0       30 2024-03-24 06:47:17.191728 operagents-0.0.9/operagents/__main__.py
+-rw-r--r--   0        0        0     8241 2024-03-24 06:47:17.191728 operagents-0.0.9/operagents/agent/__init__.py
+-rw-r--r--   0        0        0     3327 2024-03-24 06:47:17.191728 operagents-0.0.9/operagents/agent/memory.py
+-rw-r--r--   0        0        0      858 2024-03-24 06:47:17.191728 operagents-0.0.9/operagents/backend/__init__.py
+-rw-r--r--   0        0        0     2261 2024-03-24 06:47:17.191728 operagents-0.0.9/operagents/backend/_base.py
+-rw-r--r--   0        0        0     4829 2024-03-24 06:47:17.191728 operagents-0.0.9/operagents/backend/openai.py
+-rw-r--r--   0        0        0      851 2024-03-24 06:47:17.191728 operagents-0.0.9/operagents/backend/user.py
+-rw-r--r--   0        0        0     1548 2024-03-24 06:47:17.191728 operagents-0.0.9/operagents/character/__init__.py
+-rw-r--r--   0        0        0     1604 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/cli/__init__.py
+-rw-r--r--   0        0        0     8638 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/config/__init__.py
+-rw-r--r--   0        0        0      740 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/config/const.py
+-rw-r--r--   0        0        0      682 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/director/__init__.py
+-rw-r--r--   0        0        0      717 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/director/_base.py
+-rw-r--r--   0        0        0     2770 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/director/model.py
+-rw-r--r--   0        0        0      659 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/director/never.py
+-rw-r--r--   0        0        0     1186 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/director/user.py
+-rw-r--r--   0        0        0      797 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/exception.py
+-rw-r--r--   0        0        0      604 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/flow/__init__.py
+-rw-r--r--   0        0        0      871 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/flow/_base.py
+-rw-r--r--   0        0        0     3486 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/flow/model.py
+-rw-r--r--   0        0        0     1397 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/flow/order.py
+-rw-r--r--   0        0        0     1458 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/flow/user.py
+-rw-r--r--   0        0        0     1275 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/log.py
+-rw-r--r--   0        0        0     1835 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/opera/__init__.py
+-rw-r--r--   0        0        0      532 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/prop/__init__.py
+-rw-r--r--   0        0        0     2033 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/prop/_base.py
+-rw-r--r--   0        0        0     1838 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/prop/function.py
+-rw-r--r--   0        0        0     1681 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/scene/__init__.py
+-rw-r--r--   0        0        0      720 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/scene/prepare/__init__.py
+-rw-r--r--   0        0        0      710 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/scene/prepare/_base.py
+-rw-r--r--   0        0        0      820 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/scene/prepare/function.py
+-rw-r--r--   0        0        0     1126 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/scene/prepare/preface.py
+-rw-r--r--   0        0        0     5997 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/timeline/__init__.py
+-rw-r--r--   0        0        0      476 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/timeline/event.py
+-rw-r--r--   0        0        0     1621 2024-03-24 06:47:17.195729 operagents-0.0.9/operagents/utils.py
+-rw-r--r--   0        0        0     1953 2024-03-24 06:47:17.195729 operagents-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    14217 1970-01-01 00:00:00.000000 operagents-0.0.9/PKG-INFO
```

### Comparing `operagents-0.0.8/LICENSE` & `operagents-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/agent/__init__.py` & `operagents-0.0.9/operagents/agent/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
+from types import TracebackType
 from typing import TYPE_CHECKING
 from typing_extensions import Self
 from dataclasses import field, dataclass
 
 from operagents import backend
 from operagents.log import logger
 from operagents.utils import get_template_renderer
+from operagents.exception import TimelineNotStarted
 from operagents.timeline.event import TimelineEventAct
 from operagents.config import AgentConfig, TemplateConfig
 
-from .memory import (
-    AgentEvent,
-    AgentMemory,
-    AgentEventAct,
-    AgentEventObserve,
-    AgentEventSummary,
-)
+from .memory import AgentEvent as AgentEvent
+from .memory import AgentMemory, AgentEventAct, AgentEventObserve, AgentEventSummary
 
 if TYPE_CHECKING:
     from operagents.timeline import Timeline
     from operagents.backend import Backend, Message
     from operagents.timeline.event import TimelineEvent
 
 
@@ -36,18 +33,15 @@
     """The user template to use for generating text."""
 
     scene_summary_system_template: TemplateConfig = field(kw_only=True)
     """The scene summary system template to use for generating summary."""
     scene_summary_user_template: TemplateConfig = field(kw_only=True)
     """The scene summary user template to use for generating summary."""
 
-    # chat_history: list["Message"] = field(default_factory=list, kw_only=True)
-    # """The history of the agent self's chat messages."""
-    memory: AgentMemory = field(default_factory=AgentMemory, kw_only=True)
-    """The memory of the agent."""
+    _memory: AgentMemory | None = field(default=None, init=False)
 
     def __post_init__(self):
         self.logger = logger.bind(agent=self)
         self.system_renderer = get_template_renderer(self.system_template)
         self.user_renderer = get_template_renderer(self.user_template)
         self.scene_summary_system_renderer = get_template_renderer(
             self.scene_summary_system_template
@@ -64,14 +58,21 @@
             backend=backend.from_config(config.backend),
             system_template=config.system_template,
             user_template=config.user_template,
             scene_summary_system_template=config.scene_summary_system_template,
             scene_summary_user_template=config.scene_summary_user_template,
         )
 
+    @property
+    def memory(self) -> AgentMemory:
+        """The memory of the agent."""
+        if self._memory is None:
+            raise TimelineNotStarted("The timeline has not been started.")
+        return self._memory
+
     async def _act_precheck(self, timeline: "Timeline") -> None:
         """Check if the agent needs to summarize the scene before acting."""
         if (
             scene := self.memory.last_remembered_scene()
         ) and scene.name != timeline.current_scene.name:
             await self.summary(timeline)
 
@@ -214,7 +215,19 @@
             )
             response = await self.backend.generate(messages)
             self.logger.debug("Summary: {response}", scene=scene, response=response)
 
             self.memory.remember(
                 AgentEventSummary(scene=scene, content=summary_message)
             )
+
+    async def __aenter__(self) -> Self:
+        self._memory = AgentMemory()
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        traceback: TracebackType | None,
+    ) -> None:
+        self._memory = None
```

### Comparing `operagents-0.0.8/operagents/agent/memory.py` & `operagents-0.0.9/operagents/agent/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,56 +52,56 @@
 AgentEvent: TypeAlias = Annotated[
     AgentEventObserve | AgentEventSummary | AgentEventAct, Field(discriminator="type_")
 ]
 
 
 class AgentMemory:
     def __init__(self) -> None:
-        self.memory: list[AgentEvent] = []
-        """The memory of the agent."""
+        self.events: list[AgentEvent] = []
+        """Memorized events of the agent."""
 
     def last_remembered_scene(self) -> "Scene | None":
         """Get the last remembered scene."""
-        return self.memory[-1].scene if self.memory else None
+        return self.events[-1].scene if self.events else None
 
     def need_summary_scenes(self) -> list["Scene"]:
         """Get the scenes that need a summary."""
         result: dict[str, "Scene"] = {}
-        for event in self.memory:
+        for event in self.events:
             if event.type_ == "observe" or event.type_ == "act":
                 result[event.scene.name] = event.scene
             elif event.type_ == "scene_summary":
                 result.pop(event.scene.name, None)
         return list(result.values())
 
     def summarized(self, scene: "Scene") -> bool:
         return any(
             event.type_ == "scene_summary" and event.scene.name == scene.name
-            for event in self.memory
+            for event in self.events
         )
 
     def remember(self, event: AgentEvent) -> None:
         """Remember an agent event."""
         if (event.type_ == "observe" or event.type_ == "act") and self.summarized(
             event.scene
         ):
             raise SceneFinished()
-        self.memory.append(event)
+        self.events.append(event)
 
     def get_memory(self, timeline: "Timeline") -> list[AgentEvent]:
         """Get the agent memory for acting in the current scene."""
 
         result: list[AgentEvent] = []
-        for event in self.memory:
+        for event in self.events:
             if event.type_ == "observe" or event.type_ == "act":
                 if event.scene.name != timeline.current_scene.name:
                     # if the event is from past scene,
                     # ignore it and use the summary instead
                     continue
                 result.append(event)
             elif event.type_ == "scene_summary":
                 result.append(event)
         return result
 
     def get_memory_for_scene(self, scene: "Scene") -> list[AgentEvent]:
         """Get the agent memory for acting in the given scene."""
-        return [event for event in self.memory if event.scene.name == scene.name]
+        return [event for event in self.events if event.scene.name == scene.name]
```

### Comparing `operagents-0.0.8/operagents/backend/__init__.py` & `operagents-0.0.9/operagents/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/backend/_base.py` & `operagents-0.0.9/operagents/backend/_base.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/backend/openai.py` & `operagents-0.0.9/operagents/backend/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,27 +23,39 @@
         ChatCompletionAssistantMessageParam,
     )
 
 
 class OpenAIBackend(Backend):
     type_ = "openai"
 
-    def __init__(self, model: str, temperature: float | None = None) -> None:
+    def __init__(
+        self,
+        model: str,
+        temperature: float | None = None,
+        *,
+        api_key: str | None = None,
+        base_url: str | None = None,
+    ) -> None:
         super().__init__()
 
-        self.client = openai.AsyncOpenAI()
+        self.client = openai.AsyncOpenAI(api_key=api_key, base_url=base_url)
         self.model: str = model
         self.temperature: float | None = temperature
 
     @classmethod
     @override
     def from_config(  # pyright: ignore[reportIncompatibleMethodOverride]
         cls, config: OpenaiBackendConfig
     ) -> Self:
-        return cls(model=config.model, temperature=config.temperature)
+        return cls(
+            model=config.model,
+            temperature=config.temperature,
+            api_key=config.api_key,
+            base_url=config.base_url,
+        )
 
     async def _use_prop(self, prop: Prop, args: str) -> str:
         if prop.params is None:
             param = None
         else:
             try:
                 param = prop.params.model_validate_json(args)
```

### Comparing `operagents-0.0.8/operagents/backend/user.py` & `operagents-0.0.9/operagents/backend/user.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/character/__init__.py` & `operagents-0.0.9/operagents/character/__init__.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/cli/__init__.py` & `operagents-0.0.9/operagents/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/config/__init__.py` & `operagents-0.0.9/operagents/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 class OpenaiBackendConfig(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     type_: Literal["openai"] = Field(alias="type")
     model: str
     temperature: float | None = None
+    api_key: str | None = None
+    base_url: str | None = None
 
 
 class UserBackendConfig(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     type_: Literal["user"] = Field(alias="type")
```

### Comparing `operagents-0.0.8/operagents/config/const.py` & `operagents-0.0.9/operagents/config/const.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/director/__init__.py` & `operagents-0.0.9/operagents/director/__init__.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/director/_base.py` & `operagents-0.0.9/operagents/director/_base.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/director/model.py` & `operagents-0.0.9/operagents/director/model.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/director/never.py` & `operagents-0.0.9/operagents/director/never.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/director/user.py` & `operagents-0.0.9/operagents/director/user.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/exception.py` & `operagents-0.0.9/operagents/exception.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/flow/__init__.py` & `operagents-0.0.9/operagents/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/flow/_base.py` & `operagents-0.0.9/operagents/flow/_base.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/flow/model.py` & `operagents-0.0.9/operagents/flow/model.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/flow/order.py` & `operagents-0.0.9/operagents/flow/order.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/flow/user.py` & `operagents-0.0.9/operagents/flow/user.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/log.py` & `operagents-0.0.9/operagents/log.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/opera/__init__.py` & `operagents-0.0.9/operagents/opera/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+from typing import TypedDict
 from dataclasses import dataclass
 from typing_extensions import Self
 
 from operagents.log import logger
-from operagents.agent import Agent
 from operagents.scene import Scene
-from operagents.timeline import Timeline
+from operagents.agent import Agent, AgentEvent
 from operagents.config import OperagentsConfig
 from operagents.exception import OperaFinished
+from operagents.timeline import Timeline, TimelineEvent
+
+
+class OperaResult(TypedDict):
+    timeline_events: list[TimelineEvent]
+    agent_memories: dict[str, list[AgentEvent]]
 
 
 @dataclass(eq=False)
 class Opera:
     agents: dict[str, Agent]
     scenes: dict[str, Scene]
     opening_scene: str
@@ -28,16 +34,25 @@
             scenes={
                 name: Scene.from_config(name, scene_config)
                 for name, scene_config in config.scenes.items()
             },
             opening_scene=config.opening_scene,
         )
 
-    async def run(self):
+    async def run(self) -> OperaResult:
         logger.info("Starting opera...")
         async with self.timeline:
-            while True:
-                try:
-                    await self.timeline.next_time()
-                except OperaFinished:
-                    break
+            try:
+                while True:
+                    try:
+                        await self.timeline.next_time()
+                    except OperaFinished:
+                        break
+            finally:
+                timeline_events = self.timeline.events
+                agent_memories = {
+                    agent.name: agent.memory.events for agent in self.agents.values()
+                }
         logger.info("Opera finished.")
+        return OperaResult(
+            timeline_events=timeline_events, agent_memories=agent_memories
+        )
```

### Comparing `operagents-0.0.8/operagents/prop/__init__.py` & `operagents-0.0.9/operagents/prop/__init__.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/prop/_base.py` & `operagents-0.0.9/operagents/prop/_base.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/prop/function.py` & `operagents-0.0.9/operagents/prop/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 P = TypeVar("P", bound=BaseModel, default=BaseModel)
 R = TypeVar("R", default=Any)
 FunctionNoParams = Callable[[], Awaitable[R]]
 FunctionWithParams = Callable[[P], Awaitable[R]]
 
 
 class FunctionProp(Prop[P, R]):
-    """Call custom functions."""
+    """Call custom functions with pydantic model."""
 
     type_ = "function"
 
     def __init__(
         self, function: FunctionNoParams[R] | FunctionWithParams[P, R]
     ) -> None:
         super().__init__()
```

### Comparing `operagents-0.0.8/operagents/scene/__init__.py` & `operagents-0.0.9/operagents/scene/__init__.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/scene/prepare/__init__.py` & `operagents-0.0.9/operagents/scene/prepare/__init__.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/scene/prepare/_base.py` & `operagents-0.0.9/operagents/scene/prepare/_base.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/scene/prepare/function.py` & `operagents-0.0.9/operagents/scene/prepare/function.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/scene/prepare/preface.py` & `operagents-0.0.9/operagents/scene/prepare/preface.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/operagents/timeline/__init__.py` & `operagents-0.0.9/operagents/timeline/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import weakref
 from types import TracebackType
 from typing import TYPE_CHECKING
+from typing_extensions import Self
+from contextlib import AsyncExitStack
 
 from operagents.log import logger
 from operagents.exception import TimelineNotStarted
 
-from .event import TimelineEvent
+from .event import TimelineEvent as TimelineEvent
 
 if TYPE_CHECKING:
     from operagents.agent import Agent
     from operagents.opera import Opera
     from operagents.scene import Scene
     from operagents.character import Character
 
@@ -18,14 +20,15 @@
 
     def __init__(self, opera: "Opera") -> None:
         self._opera_ref = weakref.ref(opera)
 
         self._events: list[TimelineEvent] | None = None
         self._current_scene: "Scene | None" = None
         self._current_character: "Character | None" = None
+        self._exit_stack: AsyncExitStack | None = None
 
     @property
     def opera(self) -> "Opera":
         """The opera this timeline belongs to."""
         opera = self._opera_ref()
         if opera is None:
             raise RuntimeError("The opera this timeline belongs to has been destroyed.")
@@ -126,16 +129,20 @@
             self._current_character = await self.next_character()
             logger.debug(
                 "Next character: {next_character.name}",
                 scene=self.current_scene,
                 next_character=self.current_character,
             )
 
-    async def __aenter__(self) -> "Timeline":
+    async def __aenter__(self) -> Self:
         self._events = []
+        self._exit_stack = AsyncExitStack()
+
+        for agent in self.opera.agents.values():
+            await self._exit_stack.enter_async_context(agent)
 
         self._current_scene = self.opera.scenes[self.opera.opening_scene]
         logger.debug(
             "Timeline starts with opening scene {opening_scene.name}.",
             opening_scene=self.current_scene,
         )
         await self.prepare_scene()
@@ -146,10 +153,16 @@
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_value: BaseException | None,
         traceback: TracebackType | None,
     ) -> None:
         logger.debug("Timeline ends.")
-        self._events = None
-        self._current_scene = None
-        self._current_character = None
+
+        try:
+            if self._exit_stack is not None:
+                await self._exit_stack.aclose()
+        finally:
+            self._events = None
+            self._exit_stack = None
+            self._current_scene = None
+            self._current_character = None
```

### Comparing `operagents-0.0.8/operagents/utils.py` & `operagents-0.0.9/operagents/utils.py`

 * *Files identical despite different names*

### Comparing `operagents-0.0.8/pyproject.toml` & `operagents-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "operagents"
-version = "0.0.8"
+version = "0.0.9"
 description = "Dynamic, highly customizable language agents framework"
 authors = ["yanyongyu <yyy@yyydl.top>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["agent", "llm", "langchain", "sop", "langgraph"]
 
 [tool.poetry.dependencies]
```

