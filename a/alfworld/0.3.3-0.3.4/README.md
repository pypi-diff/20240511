# Comparing `tmp/alfworld-0.3.3.tar.gz` & `tmp/alfworld-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfworld-0.3.3.tar", last modified: Sat Mar  2 12:00:11 2024, max compression
+gzip compressed data, was "alfworld-0.3.4.tar", last modified: Sat May 11 14:26:31 2024, max compression
```

## Comparing `alfworld-0.3.3.tar` & `alfworld-0.3.4.tar`

### file list

```diff
@@ -1,479 +1,479 @@
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.114192 alfworld-0.3.3/
--rw-rw-r--   0 macote    (1000) macote    (1000)     1082 2023-11-23 02:08:40.000000 alfworld-0.3.3/LICENSE
--rw-rw-r--   0 macote    (1000) macote    (1000)      233 2023-12-18 16:44:08.000000 alfworld-0.3.3/MANIFEST.in
--rw-r--r--   0 macote    (1000) macote    (1000)     2178 2024-03-02 12:00:11.114192 alfworld-0.3.3/PKG-INFO
--rw-rw-r--   0 macote    (1000) macote    (1000)     8177 2024-02-23 14:23:25.000000 alfworld-0.3.3/README.md
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.070192 alfworld-0.3.3/alfworld/
--rw-rw-r--   0 macote    (1000) macote    (1000)       28 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/__init__.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.070192 alfworld-0.3.3/alfworld/agents/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/__init__.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.070192 alfworld-0.3.3/alfworld/agents/agent/
--rw-rw-r--   0 macote    (1000) macote    (1000)      256 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/agent/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    23278 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/agent/base_agent.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    19881 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/agent/text_dagger_agent.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    56477 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/agent/text_dqn_agent.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    16924 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/agent/vision_dagger_agent.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.070192 alfworld-0.3.3/alfworld/agents/config/
--rw-rw-r--   0 macote    (1000) macote    (1000)     1405 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/config/rewards.json
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.070192 alfworld-0.3.3/alfworld/agents/controller/
--rw-rw-r--   0 macote    (1000) macote    (1000)      255 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/controller/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     8696 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/controller/base.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    26384 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/controller/mrcnn.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     2442 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/controller/mrcnn_astar.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    18696 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/controller/oracle.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     2153 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/controller/oracle_astar.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/agents/detector/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/detector/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    12009 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/detector/coco_eval.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     8757 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/detector/coco_utils.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     3830 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/detector/engine.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     6926 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/detector/group_by_aspect_ratio.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     1788 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/detector/mrcnn.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     7109 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/detector/train.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     1534 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/detector/transforms.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     9491 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/detector/utils.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/agents/environment/
--rw-rw-r--   0 macote    (1000) macote    (1000)      202 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/environment/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     1873 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/environment/alfred_hybrid.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    15742 2024-03-02 11:59:47.000000 alfworld-0.3.3/alfworld/agents/environment/alfred_thor_env.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    10662 2024-03-02 11:59:47.000000 alfworld-0.3.3/alfworld/agents/environment/alfred_tw_env.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/agents/eval/
--rw-rw-r--   0 macote    (1000) macote    (1000)      202 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/eval/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     8925 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/eval/evaluate_dagger.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     7399 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/eval/evaluate_dqn.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     6778 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/eval/evaluate_vision_dagger.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/agents/expert/
--rw-rw-r--   0 macote    (1000) macote    (1000)      243 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/expert/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    26144 2023-12-18 16:44:08.000000 alfworld-0.3.3/alfworld/agents/expert/handcoded_expert.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     9554 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/expert/handcoded_expert_thor.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     8153 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/expert/handcoded_expert_tw.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/agents/modules/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/modules/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     8881 2024-02-29 03:35:36.000000 alfworld-0.3.3/alfworld/agents/modules/generic.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    67031 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/modules/layers.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    15643 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/modules/memory.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    13871 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/modules/model.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     5245 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/modules/segment_tree.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/agents/utils/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/agents/utils/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    11289 2024-03-02 11:59:47.000000 alfworld-0.3.3/alfworld/agents/utils/misc.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/data/
--rw-rw-r--   0 macote    (1000) macote    (1000)    17067 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/data/alfred.pddl
--rw-rw-r--   0 macote    (1000) macote    (1000)    12154 2023-11-24 03:09:38.000000 alfworld-0.3.3/alfworld/data/alfred.twl2
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/env/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/env/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    10191 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/env/reward.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    16131 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/env/tasks.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    25941 2024-02-23 14:54:10.000000 alfworld-0.3.3/alfworld/env/thor_env.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/gen/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/__init__.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/gen/agents/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/agents/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     2111 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/agents/agent_base.py
--rw-rw-r--   0 macote    (1000) macote    (1000)      962 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/agents/deterministic_planner_agent.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     4414 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/agents/plan_agent.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     3017 2024-02-23 14:24:15.000000 alfworld-0.3.3/alfworld/gen/agents/semantic_map_planner_agent.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    31309 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/constants.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/gen/game_states/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/game_states/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    48340 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/game_states/game_state_base.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    21532 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/game_states/planned_game_state.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    18855 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/game_states/task_game_state.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    23385 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/game_states/task_game_state_full_knowledge.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    22677 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/goal_library.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.074192 alfworld-0.3.3/alfworld/gen/graph/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/graph/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    19588 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/graph/graph_obj.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.114192 alfworld-0.3.3/alfworld/gen/layouts/
--rw-rw-r--   0 macote    (1000) macote    (1000)     2192 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan1-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      714 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan1-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2344 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan1-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3376 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan10-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      687 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan10-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1541 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan10-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1200 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan11-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      609 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan11-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2136 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan11-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1392 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan12-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      554 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan12-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2413 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan12-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2944 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan13-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      611 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan13-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2988 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan13-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2016 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan14-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      553 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan14-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      876 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan14-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1664 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan15-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      619 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan15-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1651 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan15-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3296 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan16-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      663 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan16-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3754 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan16-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1248 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan17-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      660 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan17-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1655 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan17-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3680 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan18-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      653 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan18-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2505 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan18-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1248 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan19-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      559 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan19-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1874 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan19-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1968 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan2-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      598 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan2-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2240 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan2-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1408 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan20-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      617 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan20-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1856 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan20-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3152 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan201-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      504 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan201-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1066 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan201-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2416 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan202-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      350 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan202-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      584 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan202-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     8096 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan203-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      500 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan203-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1149 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan203-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3552 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan204-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      435 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan204-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1709 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan204-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     4096 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan205-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      415 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan205-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1150 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan205-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1968 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan206-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      329 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan206-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1823 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan206-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2448 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan207-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      330 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan207-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1331 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan207-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3536 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan208-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      362 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan208-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1539 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan208-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     4992 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan209-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      421 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan209-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      987 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan209-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1808 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan21-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      618 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan21-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1281 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan21-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     4416 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan210-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      415 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan210-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1446 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan210-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2128 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan211-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      395 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan211-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1050 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan211-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1792 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan212-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      427 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan212-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1144 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan212-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     4800 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan213-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      380 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan213-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2021 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan213-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3104 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan214-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      396 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan214-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      679 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan214-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     6160 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan215-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      407 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan215-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1242 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan215-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2528 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan216-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      396 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan216-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1053 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan216-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2576 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan217-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      411 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan217-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1454 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan217-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     6848 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan218-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      437 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan218-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1056 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan218-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3536 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan219-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      418 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan219-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2452 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan219-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2304 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan22-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      586 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan22-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2738 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan22-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3920 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan220-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      414 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan220-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1438 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan220-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2016 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan221-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      376 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan221-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      688 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan221-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1824 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan222-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      369 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan222-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1437 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan222-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3632 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan223-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      382 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan223-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      782 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan223-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     4496 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan224-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      425 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan224-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2583 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan224-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2592 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan225-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      424 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan225-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1241 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan225-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1392 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan226-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      352 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan226-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1060 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan226-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3312 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan227-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      393 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan227-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3333 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan227-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2688 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan228-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      379 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan228-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      782 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan228-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3456 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan229-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      439 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan229-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1067 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan229-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1664 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan23-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      649 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan23-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1182 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan23-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     5872 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan230-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      439 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan230-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      788 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan230-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1104 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan24-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      595 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan24-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3006 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan24-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      560 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan25-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      567 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan25-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1654 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan25-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1344 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan26-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      560 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan26-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1480 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan26-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      816 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan27-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      606 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan27-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1826 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan27-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1744 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan28-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      591 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan28-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1762 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan28-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1168 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan29-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      540 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan29-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1078 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan29-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1792 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan3-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      624 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan3-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1545 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan3-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1072 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan30-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      636 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan30-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     4499 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan30-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1520 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan301-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      447 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan301-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1516 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan301-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      848 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan302-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      416 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan302-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      954 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan302-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1424 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan303-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      436 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan303-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1637 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan303-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1872 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan304-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      415 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan304-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      281 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan304-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1488 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan305-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      449 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan305-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      655 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan305-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1616 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan306-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      383 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan306-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      858 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan306-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1552 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan307-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      480 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan307-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      770 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan307-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1696 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan308-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      421 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan308-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1236 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan308-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     5920 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan309-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      481 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan309-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1060 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan309-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1200 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan310-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      414 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan310-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1058 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan310-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3728 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan311-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      483 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan311-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      871 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan311-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1616 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan312-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      321 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan312-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1233 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan312-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      912 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan313-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      446 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan313-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1046 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan313-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1408 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan314-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      351 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan314-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      756 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan314-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1744 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan315-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      366 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan315-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1647 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan315-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1056 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan316-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      381 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan316-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      476 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan316-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2160 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan317-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      422 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan317-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1541 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan317-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1536 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan318-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      395 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan318-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1704 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan318-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1536 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan319-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      388 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan319-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1896 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan319-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1088 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan320-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      347 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan320-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      755 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan320-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1440 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan321-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      360 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan321-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      683 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan321-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1696 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan322-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      386 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan322-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1242 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan322-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3152 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan323-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      375 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan323-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1713 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan323-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1616 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan324-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      360 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan324-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1520 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan324-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3104 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan325-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      350 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan325-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2300 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan325-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1744 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan326-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      461 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan326-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1900 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan326-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1360 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan327-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      381 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan327-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1426 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan327-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1120 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan328-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      404 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan328-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      675 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan328-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1536 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan329-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      355 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan329-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      486 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan329-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2304 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan330-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      408 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan330-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2016 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan330-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1232 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan4-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      591 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan4-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1467 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan4-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1696 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan401-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      491 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan401-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      779 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan401-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1632 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan402-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      505 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan402-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1498 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan402-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1152 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan403-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      510 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan403-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      885 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan403-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      928 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan404-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      424 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan404-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      586 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan404-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      560 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan405-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      427 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan405-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      898 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan405-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1696 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan406-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      420 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan406-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      699 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan406-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      656 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan407-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      478 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan407-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1008 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan407-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      720 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan408-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      427 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan408-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      991 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan408-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      752 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan409-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      407 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan409-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      970 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan409-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1408 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan410-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      441 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan410-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      996 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan410-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1200 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan411-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      456 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan411-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      891 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan411-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      912 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan412-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      443 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan412-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      704 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan412-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1232 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan413-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      485 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan413-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1100 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan413-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      928 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan414-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      474 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan414-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1384 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan414-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1040 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan415-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      472 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan415-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1092 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan415-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1248 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan416-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      402 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan416-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      696 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan416-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1056 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan417-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      443 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan417-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      802 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan417-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      896 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan418-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      422 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan418-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      493 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan418-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      624 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan419-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      442 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan419-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      317 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan419-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      576 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan420-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      437 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan420-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      506 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan420-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      624 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan421-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      443 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan421-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1065 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan421-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      768 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan422-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      485 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan422-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1088 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan422-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1024 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan423-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      495 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan423-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1280 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan423-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      736 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan424-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      408 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan424-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      784 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan424-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      528 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan425-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      457 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan425-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      590 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan425-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      928 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan426-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      457 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan426-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1181 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan426-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      944 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan427-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      483 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan427-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1079 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan427-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1008 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan428-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      423 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan428-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      791 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan428-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1136 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan429-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      438 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan429-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      398 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan429-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1824 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan430-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      551 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan430-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)      983 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan430-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1712 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan5-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      646 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan5-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3116 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan5-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2272 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan6-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      590 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan6-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2639 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan6-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     4416 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan7-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      674 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan7-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2434 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan7-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     2880 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan8-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      648 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan8-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     3203 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan8-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     1344 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan9-layout.npy
--rw-rw-r--   0 macote    (1000) macote    (1000)      587 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan9-objects.json
--rw-rw-r--   0 macote    (1000) macote    (1000)     4498 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/FloorPlan9-openable.json
--rw-rw-r--   0 macote    (1000) macote    (1000)    20040 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/layouts/precompute_layout_locations.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.114192 alfworld-0.3.3/alfworld/gen/planner/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/planner/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     9905 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/planner/ff_planner_handler.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.114192 alfworld-0.3.3/alfworld/gen/utils/
--rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/utils/__init__.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     4977 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/utils/bb_util.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     3198 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/utils/dataset_management_util.py
--rw-rw-r--   0 macote    (1000) macote    (1000)    14817 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/utils/game_util.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     1753 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/utils/image_util.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     2304 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/utils/py_util.py
--rw-rw-r--   0 macote    (1000) macote    (1000)     2145 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/utils/replay_json.py
--rw-rw-r--   0 macote    (1000) macote    (1000)      419 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/gen/utils/video_util.py
--rw-rw-r--   0 macote    (1000) macote    (1000)      522 2024-03-02 11:59:47.000000 alfworld-0.3.3/alfworld/info.py
--rw-rw-r--   0 macote    (1000) macote    (1000)      413 2023-11-23 02:08:40.000000 alfworld-0.3.3/alfworld/utils.py
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.114192 alfworld-0.3.3/alfworld.egg-info/
--rw-r--r--   0 macote    (1000) macote    (1000)     2178 2024-03-02 12:00:11.000000 alfworld-0.3.3/alfworld.egg-info/PKG-INFO
--rwxr-xr-x   0 macote    (1000) macote    (1000)    19860 2024-03-02 12:00:11.000000 alfworld-0.3.3/alfworld.egg-info/SOURCES.txt
--rwxr-xr-x   0 macote    (1000) macote    (1000)        1 2024-03-02 12:00:11.000000 alfworld-0.3.3/alfworld.egg-info/dependency_links.txt
--rwxr-xr-x   0 macote    (1000) macote    (1000)        1 2020-12-14 19:17:21.000000 alfworld-0.3.3/alfworld.egg-info/not-zip-safe
--rwxr-xr-x   0 macote    (1000) macote    (1000)      241 2024-03-02 12:00:11.000000 alfworld-0.3.3/alfworld.egg-info/requires.txt
--rwxr-xr-x   0 macote    (1000) macote    (1000)        9 2024-03-02 12:00:11.000000 alfworld-0.3.3/alfworld.egg-info/top_level.txt
--rw-rw-r--   0 macote    (1000) macote    (1000)       88 2023-12-18 16:44:08.000000 alfworld-0.3.3/pyproject.toml
--rw-rw-r--   0 macote    (1000) macote    (1000)      136 2024-02-23 14:23:25.000000 alfworld-0.3.3/requirements-full.txt
--rw-rw-r--   0 macote    (1000) macote    (1000)       97 2024-01-05 20:41:03.000000 alfworld-0.3.3/requirements.txt
-drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-03-02 12:00:11.114192 alfworld-0.3.3/scripts/
--rwxrwxr-x   0 macote    (1000) macote    (1000)     6025 2023-11-23 02:16:19.000000 alfworld-0.3.3/scripts/alfworld-download
--rwxrwxr-x   0 macote    (1000) macote    (1000)     8517 2024-03-02 11:59:47.000000 alfworld-0.3.3/scripts/alfworld-generate
--rwxrwxr-x   0 macote    (1000) macote    (1000)     3977 2024-02-23 14:54:10.000000 alfworld-0.3.3/scripts/alfworld-play-thor
--rwxrwxr-x   0 macote    (1000) macote    (1000)     3318 2024-03-02 11:59:47.000000 alfworld-0.3.3/scripts/alfworld-play-tw
--rw-rw-r--   0 macote    (1000) macote    (1000)       38 2024-03-02 12:00:11.114192 alfworld-0.3.3/setup.cfg
--rw-rw-r--   0 macote    (1000) macote    (1000)      855 2024-03-02 11:59:47.000000 alfworld-0.3.3/setup.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:31.042873 alfworld-0.3.4/
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1082 2023-11-23 02:08:40.000000 alfworld-0.3.4/LICENSE
+-rw-rw-r--   0 macote    (1000) macote    (1000)      233 2023-12-18 16:44:08.000000 alfworld-0.3.4/MANIFEST.in
+-rw-r--r--   0 macote    (1000) macote    (1000)     2178 2024-05-11 14:26:31.042873 alfworld-0.3.4/PKG-INFO
+-rw-rw-r--   0 macote    (1000) macote    (1000)     8177 2024-02-23 14:23:25.000000 alfworld-0.3.4/README.md
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.978872 alfworld-0.3.4/alfworld/
+-rw-rw-r--   0 macote    (1000) macote    (1000)       28 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/__init__.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.978872 alfworld-0.3.4/alfworld/agents/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/__init__.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.978872 alfworld-0.3.4/alfworld/agents/agent/
+-rw-rw-r--   0 macote    (1000) macote    (1000)      256 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/agent/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    23278 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/agent/base_agent.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    19881 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/agent/text_dagger_agent.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    56477 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/agent/text_dqn_agent.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    16924 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/agent/vision_dagger_agent.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.978872 alfworld-0.3.4/alfworld/agents/config/
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1405 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/config/rewards.json
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.978872 alfworld-0.3.4/alfworld/agents/controller/
+-rw-rw-r--   0 macote    (1000) macote    (1000)      255 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/controller/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     8696 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/controller/base.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    26384 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/controller/mrcnn.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2442 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/controller/mrcnn_astar.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    18696 2024-05-11 12:51:48.000000 alfworld-0.3.4/alfworld/agents/controller/oracle.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2153 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/controller/oracle_astar.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.982872 alfworld-0.3.4/alfworld/agents/detector/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/detector/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    12009 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/detector/coco_eval.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     8757 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/detector/coco_utils.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3830 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/detector/engine.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     6926 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/detector/group_by_aspect_ratio.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1788 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/detector/mrcnn.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     7109 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/detector/train.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1534 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/detector/transforms.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     9491 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/detector/utils.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.982872 alfworld-0.3.4/alfworld/agents/environment/
+-rw-rw-r--   0 macote    (1000) macote    (1000)      202 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/environment/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1873 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/environment/alfred_hybrid.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    15742 2024-03-12 13:39:05.000000 alfworld-0.3.4/alfworld/agents/environment/alfred_thor_env.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    10728 2024-05-11 13:58:09.000000 alfworld-0.3.4/alfworld/agents/environment/alfred_tw_env.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.982872 alfworld-0.3.4/alfworld/agents/eval/
+-rw-rw-r--   0 macote    (1000) macote    (1000)      202 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/eval/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     8925 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/eval/evaluate_dagger.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     7399 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/eval/evaluate_dqn.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     6778 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/eval/evaluate_vision_dagger.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.982872 alfworld-0.3.4/alfworld/agents/expert/
+-rw-rw-r--   0 macote    (1000) macote    (1000)      243 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/expert/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    26144 2023-12-18 16:44:08.000000 alfworld-0.3.4/alfworld/agents/expert/handcoded_expert.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     9554 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/expert/handcoded_expert_thor.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     8153 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/expert/handcoded_expert_tw.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.982872 alfworld-0.3.4/alfworld/agents/modules/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/modules/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     8881 2024-03-13 12:18:00.000000 alfworld-0.3.4/alfworld/agents/modules/generic.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    67031 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/modules/layers.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    15643 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/modules/memory.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    13871 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/modules/model.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     5245 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/modules/segment_tree.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.982872 alfworld-0.3.4/alfworld/agents/utils/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/agents/utils/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    11289 2024-03-12 13:39:05.000000 alfworld-0.3.4/alfworld/agents/utils/misc.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.982872 alfworld-0.3.4/alfworld/data/
+-rw-rw-r--   0 macote    (1000) macote    (1000)    17067 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/data/alfred.pddl
+-rw-rw-r--   0 macote    (1000) macote    (1000)    12154 2023-11-24 03:09:38.000000 alfworld-0.3.4/alfworld/data/alfred.twl2
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.982872 alfworld-0.3.4/alfworld/env/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/env/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    10191 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/env/reward.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    16131 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/env/tasks.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    25941 2024-03-13 12:18:00.000000 alfworld-0.3.4/alfworld/env/thor_env.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.982872 alfworld-0.3.4/alfworld/gen/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/__init__.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.986872 alfworld-0.3.4/alfworld/gen/agents/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/agents/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2111 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/agents/agent_base.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)      962 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/agents/deterministic_planner_agent.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     4414 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/agents/plan_agent.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3017 2024-02-23 14:24:15.000000 alfworld-0.3.4/alfworld/gen/agents/semantic_map_planner_agent.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    31309 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/constants.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.986872 alfworld-0.3.4/alfworld/gen/game_states/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/game_states/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    48340 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/game_states/game_state_base.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    21532 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/game_states/planned_game_state.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    18855 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/game_states/task_game_state.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    23385 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/game_states/task_game_state_full_knowledge.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    22677 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/goal_library.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:30.986872 alfworld-0.3.4/alfworld/gen/graph/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/graph/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    19588 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/graph/graph_obj.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:31.038872 alfworld-0.3.4/alfworld/gen/layouts/
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2192 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan1-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      714 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan1-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2344 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan1-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3376 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan10-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      687 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan10-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1541 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan10-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1200 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan11-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      609 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan11-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2136 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan11-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1392 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan12-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      554 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan12-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2413 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan12-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2944 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan13-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      611 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan13-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2988 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan13-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2016 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan14-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      553 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan14-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      876 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan14-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1664 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan15-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      619 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan15-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1651 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan15-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3296 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan16-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      663 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan16-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3754 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan16-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1248 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan17-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      660 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan17-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1655 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan17-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3680 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan18-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      653 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan18-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2505 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan18-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1248 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan19-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      559 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan19-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1874 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan19-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1968 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan2-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      598 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan2-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2240 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan2-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1408 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan20-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      617 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan20-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1856 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan20-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3152 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan201-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      504 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan201-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1066 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan201-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2416 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan202-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      350 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan202-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      584 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan202-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     8096 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan203-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      500 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan203-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1149 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan203-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3552 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan204-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      435 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan204-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1709 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan204-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     4096 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan205-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      415 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan205-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1150 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan205-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1968 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan206-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      329 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan206-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1823 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan206-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2448 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan207-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      330 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan207-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1331 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan207-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3536 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan208-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      362 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan208-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1539 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan208-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     4992 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan209-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      421 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan209-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      987 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan209-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1808 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan21-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      618 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan21-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1281 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan21-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     4416 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan210-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      415 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan210-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1446 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan210-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2128 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan211-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      395 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan211-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1050 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan211-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1792 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan212-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      427 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan212-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1144 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan212-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     4800 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan213-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      380 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan213-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2021 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan213-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3104 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan214-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      396 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan214-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      679 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan214-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     6160 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan215-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      407 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan215-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1242 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan215-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2528 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan216-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      396 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan216-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1053 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan216-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2576 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan217-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      411 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan217-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1454 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan217-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     6848 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan218-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      437 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan218-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1056 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan218-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3536 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan219-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      418 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan219-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2452 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan219-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2304 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan22-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      586 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan22-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2738 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan22-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3920 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan220-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      414 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan220-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1438 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan220-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2016 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan221-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      376 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan221-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      688 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan221-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1824 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan222-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      369 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan222-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1437 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan222-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3632 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan223-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      382 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan223-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      782 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan223-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     4496 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan224-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      425 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan224-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2583 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan224-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2592 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan225-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      424 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan225-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1241 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan225-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1392 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan226-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      352 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan226-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1060 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan226-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3312 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan227-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      393 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan227-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3333 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan227-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2688 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan228-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      379 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan228-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      782 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan228-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3456 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan229-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      439 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan229-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1067 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan229-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1664 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan23-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      649 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan23-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1182 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan23-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     5872 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan230-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      439 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan230-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      788 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan230-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1104 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan24-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      595 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan24-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3006 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan24-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      560 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan25-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      567 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan25-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1654 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan25-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1344 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan26-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      560 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan26-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1480 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan26-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      816 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan27-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      606 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan27-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1826 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan27-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1744 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan28-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      591 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan28-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1762 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan28-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1168 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan29-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      540 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan29-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1078 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan29-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1792 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan3-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      624 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan3-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1545 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan3-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1072 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan30-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      636 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan30-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     4499 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan30-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1520 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan301-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      447 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan301-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1516 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan301-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      848 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan302-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      416 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan302-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      954 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan302-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1424 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan303-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      436 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan303-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1637 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan303-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1872 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan304-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      415 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan304-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      281 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan304-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1488 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan305-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      449 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan305-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      655 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan305-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1616 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan306-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      383 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan306-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      858 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan306-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1552 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan307-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      480 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan307-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      770 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan307-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1696 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan308-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      421 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan308-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1236 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan308-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     5920 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan309-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      481 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan309-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1060 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan309-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1200 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan310-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      414 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan310-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1058 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan310-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3728 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan311-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      483 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan311-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      871 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan311-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1616 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan312-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      321 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan312-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1233 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan312-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      912 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan313-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      446 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan313-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1046 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan313-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1408 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan314-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      351 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan314-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      756 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan314-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1744 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan315-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      366 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan315-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1647 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan315-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1056 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan316-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      381 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan316-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      476 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan316-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2160 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan317-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      422 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan317-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1541 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan317-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1536 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan318-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      395 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan318-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1704 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan318-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1536 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan319-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      388 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan319-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1896 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan319-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1088 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan320-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      347 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan320-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      755 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan320-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1440 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan321-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      360 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan321-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      683 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan321-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1696 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan322-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      386 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan322-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1242 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan322-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3152 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan323-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      375 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan323-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1713 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan323-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1616 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan324-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      360 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan324-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1520 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan324-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3104 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan325-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      350 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan325-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2300 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan325-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1744 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan326-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      461 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan326-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1900 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan326-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1360 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan327-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      381 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan327-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1426 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan327-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1120 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan328-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      404 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan328-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      675 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan328-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1536 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan329-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      355 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan329-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      486 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan329-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2304 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan330-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      408 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan330-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2016 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan330-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1232 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan4-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      591 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan4-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1467 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan4-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1696 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan401-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      491 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan401-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      779 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan401-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1632 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan402-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      505 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan402-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1498 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan402-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1152 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan403-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      510 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan403-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      885 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan403-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      928 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan404-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      424 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan404-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      586 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan404-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      560 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan405-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      427 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan405-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      898 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan405-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1696 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan406-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      420 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan406-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      699 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan406-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      656 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan407-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      478 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan407-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1008 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan407-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      720 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan408-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      427 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan408-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      991 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan408-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      752 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan409-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      407 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan409-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      970 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan409-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1408 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan410-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      441 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan410-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      996 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan410-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1200 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan411-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      456 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan411-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      891 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan411-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      912 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan412-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      443 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan412-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      704 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan412-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1232 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan413-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      485 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan413-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1100 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan413-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      928 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan414-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      474 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan414-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1384 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan414-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1040 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan415-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      472 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan415-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1092 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan415-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1248 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan416-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      402 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan416-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      696 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan416-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1056 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan417-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      443 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan417-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      802 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan417-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      896 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan418-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      422 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan418-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      493 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan418-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      624 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan419-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      442 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan419-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      317 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan419-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      576 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan420-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      437 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan420-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      506 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan420-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      624 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan421-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      443 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan421-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1065 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan421-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      768 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan422-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      485 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan422-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1088 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan422-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1024 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan423-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      495 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan423-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1280 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan423-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      736 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan424-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      408 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan424-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      784 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan424-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      528 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan425-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      457 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan425-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      590 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan425-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      928 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan426-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      457 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan426-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1181 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan426-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      944 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan427-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      483 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan427-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1079 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan427-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1008 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan428-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      423 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan428-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      791 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan428-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1136 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan429-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      438 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan429-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      398 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan429-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1824 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan430-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      551 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan430-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)      983 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan430-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1712 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan5-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      646 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan5-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3116 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan5-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2272 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan6-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      590 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan6-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2639 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan6-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     4416 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan7-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      674 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan7-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2434 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan7-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2880 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan8-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      648 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan8-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3203 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan8-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1344 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan9-layout.npy
+-rw-rw-r--   0 macote    (1000) macote    (1000)      587 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan9-objects.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)     4498 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/FloorPlan9-openable.json
+-rw-rw-r--   0 macote    (1000) macote    (1000)    20040 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/layouts/precompute_layout_locations.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:31.038872 alfworld-0.3.4/alfworld/gen/planner/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/planner/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     9905 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/planner/ff_planner_handler.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:31.038872 alfworld-0.3.4/alfworld/gen/utils/
+-rw-rw-r--   0 macote    (1000) macote    (1000)        0 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/utils/__init__.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     4977 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/utils/bb_util.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     3198 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/utils/dataset_management_util.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)    14817 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/utils/game_util.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     1753 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/utils/image_util.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2304 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/utils/py_util.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)     2145 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/utils/replay_json.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)      419 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/gen/utils/video_util.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)      522 2024-05-11 14:06:30.000000 alfworld-0.3.4/alfworld/info.py
+-rw-rw-r--   0 macote    (1000) macote    (1000)      413 2023-11-23 02:08:40.000000 alfworld-0.3.4/alfworld/utils.py
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:31.038872 alfworld-0.3.4/alfworld.egg-info/
+-rw-r--r--   0 macote    (1000) macote    (1000)     2178 2024-05-11 14:26:30.000000 alfworld-0.3.4/alfworld.egg-info/PKG-INFO
+-rwxr-xr-x   0 macote    (1000) macote    (1000)    19860 2024-05-11 14:26:30.000000 alfworld-0.3.4/alfworld.egg-info/SOURCES.txt
+-rwxr-xr-x   0 macote    (1000) macote    (1000)        1 2024-05-11 14:26:30.000000 alfworld-0.3.4/alfworld.egg-info/dependency_links.txt
+-rwxr-xr-x   0 macote    (1000) macote    (1000)        1 2020-12-14 19:17:21.000000 alfworld-0.3.4/alfworld.egg-info/not-zip-safe
+-rwxr-xr-x   0 macote    (1000) macote    (1000)      241 2024-05-11 14:26:30.000000 alfworld-0.3.4/alfworld.egg-info/requires.txt
+-rwxr-xr-x   0 macote    (1000) macote    (1000)        9 2024-05-11 14:26:30.000000 alfworld-0.3.4/alfworld.egg-info/top_level.txt
+-rw-rw-r--   0 macote    (1000) macote    (1000)       88 2023-12-18 16:44:08.000000 alfworld-0.3.4/pyproject.toml
+-rw-rw-r--   0 macote    (1000) macote    (1000)      136 2024-02-23 14:23:25.000000 alfworld-0.3.4/requirements-full.txt
+-rw-rw-r--   0 macote    (1000) macote    (1000)       97 2024-01-05 20:41:03.000000 alfworld-0.3.4/requirements.txt
+drwxrwxr-x   0 macote    (1000) macote    (1000)        0 2024-05-11 14:26:31.038872 alfworld-0.3.4/scripts/
+-rwxrwxr-x   0 macote    (1000) macote    (1000)     6025 2023-11-23 02:16:19.000000 alfworld-0.3.4/scripts/alfworld-download
+-rwxrwxr-x   0 macote    (1000) macote    (1000)     8517 2024-03-12 13:39:05.000000 alfworld-0.3.4/scripts/alfworld-generate
+-rwxrwxr-x   0 macote    (1000) macote    (1000)     3977 2024-05-11 12:51:48.000000 alfworld-0.3.4/scripts/alfworld-play-thor
+-rwxrwxr-x   0 macote    (1000) macote    (1000)     3318 2024-05-11 14:04:37.000000 alfworld-0.3.4/scripts/alfworld-play-tw
+-rw-rw-r--   0 macote    (1000) macote    (1000)       38 2024-05-11 14:26:31.042873 alfworld-0.3.4/setup.cfg
+-rw-rw-r--   0 macote    (1000) macote    (1000)      855 2024-03-12 13:39:05.000000 alfworld-0.3.4/setup.py
```

### Comparing `alfworld-0.3.3/LICENSE` & `alfworld-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/PKG-INFO` & `alfworld-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfworld
-Version: 0.3.3
+Version: 0.3.4
 Summary: ALFWorld - Aligning Text and Embodied Environments for Interactive Learning.
 License: MIT License
         
         Copyright (c) 2020 Mohit Shridhar and others
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `alfworld-0.3.3/README.md` & `alfworld-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/agent/base_agent.py` & `alfworld-0.3.4/alfworld/agents/agent/base_agent.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/agent/text_dagger_agent.py` & `alfworld-0.3.4/alfworld/agents/agent/text_dagger_agent.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/agent/text_dqn_agent.py` & `alfworld-0.3.4/alfworld/agents/agent/text_dqn_agent.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/agent/vision_dagger_agent.py` & `alfworld-0.3.4/alfworld/agents/agent/vision_dagger_agent.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/config/rewards.json` & `alfworld-0.3.4/alfworld/agents/config/rewards.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/controller/base.py` & `alfworld-0.3.4/alfworld/agents/controller/base.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/controller/mrcnn.py` & `alfworld-0.3.4/alfworld/agents/controller/mrcnn.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/controller/mrcnn_astar.py` & `alfworld-0.3.4/alfworld/agents/controller/mrcnn_astar.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/controller/oracle.py` & `alfworld-0.3.4/alfworld/agents/controller/oracle.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/controller/oracle_astar.py` & `alfworld-0.3.4/alfworld/agents/controller/oracle_astar.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/detector/coco_eval.py` & `alfworld-0.3.4/alfworld/agents/detector/coco_eval.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/detector/coco_utils.py` & `alfworld-0.3.4/alfworld/agents/detector/coco_utils.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/detector/engine.py` & `alfworld-0.3.4/alfworld/agents/detector/engine.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/detector/group_by_aspect_ratio.py` & `alfworld-0.3.4/alfworld/agents/detector/group_by_aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/detector/mrcnn.py` & `alfworld-0.3.4/alfworld/agents/detector/mrcnn.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/detector/train.py` & `alfworld-0.3.4/alfworld/agents/detector/train.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/detector/transforms.py` & `alfworld-0.3.4/alfworld/agents/detector/transforms.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/detector/utils.py` & `alfworld-0.3.4/alfworld/agents/detector/utils.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/environment/alfred_hybrid.py` & `alfworld-0.3.4/alfworld/agents/environment/alfred_hybrid.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/environment/alfred_thor_env.py` & `alfworld-0.3.4/alfworld/agents/environment/alfred_thor_env.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/environment/alfred_tw_env.py` & `alfworld-0.3.4/alfworld/agents/environment/alfred_tw_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
             self.state["extra.expert_plan"] = self.state["policy_commands"]
         else:
             raise NotImplementedError("Unknown type of AlfredExpert: {}.".format(self.expert_type))
 
     def load(self, gamefile):
         super().load(gamefile)
         self.gamefile = gamefile
-        self.request_infos.policy_commands = (self.expert_type == AlfredExpertType.PLANNER)
-        self.request_infos.facts = (self.expert_type == AlfredExpertType.HANDCODED)
+        self.request_infos.policy_commands = self.request_infos.policy_commands or (self.expert_type == AlfredExpertType.PLANNER)
+        self.request_infos.facts = self.request_infos.facts or (self.expert_type == AlfredExpertType.HANDCODED)
         self._handcoded_expert = HandCodedTWAgent(max_steps=200)
 
     def step(self, command):
         self.state, reward, done = super().step(command)
         self.prev_command = str(command)
         self._gather_infos()
         return self.state, reward, done
```

### Comparing `alfworld-0.3.3/alfworld/agents/eval/evaluate_dagger.py` & `alfworld-0.3.4/alfworld/agents/eval/evaluate_dagger.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/eval/evaluate_dqn.py` & `alfworld-0.3.4/alfworld/agents/eval/evaluate_dqn.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/eval/evaluate_vision_dagger.py` & `alfworld-0.3.4/alfworld/agents/eval/evaluate_vision_dagger.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/expert/handcoded_expert.py` & `alfworld-0.3.4/alfworld/agents/expert/handcoded_expert.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/expert/handcoded_expert_thor.py` & `alfworld-0.3.4/alfworld/agents/expert/handcoded_expert_thor.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/expert/handcoded_expert_tw.py` & `alfworld-0.3.4/alfworld/agents/expert/handcoded_expert_tw.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/modules/generic.py` & `alfworld-0.3.4/alfworld/agents/modules/generic.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/modules/layers.py` & `alfworld-0.3.4/alfworld/agents/modules/layers.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/modules/memory.py` & `alfworld-0.3.4/alfworld/agents/modules/memory.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/modules/model.py` & `alfworld-0.3.4/alfworld/agents/modules/model.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/modules/segment_tree.py` & `alfworld-0.3.4/alfworld/agents/modules/segment_tree.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/agents/utils/misc.py` & `alfworld-0.3.4/alfworld/agents/utils/misc.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/data/alfred.pddl` & `alfworld-0.3.4/alfworld/data/alfred.pddl`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/data/alfred.twl2` & `alfworld-0.3.4/alfworld/data/alfred.twl2`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/env/reward.py` & `alfworld-0.3.4/alfworld/env/reward.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/env/tasks.py` & `alfworld-0.3.4/alfworld/env/tasks.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/env/thor_env.py` & `alfworld-0.3.4/alfworld/env/thor_env.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/agents/agent_base.py` & `alfworld-0.3.4/alfworld/gen/agents/agent_base.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/agents/deterministic_planner_agent.py` & `alfworld-0.3.4/alfworld/gen/agents/deterministic_planner_agent.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/agents/plan_agent.py` & `alfworld-0.3.4/alfworld/gen/agents/plan_agent.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/agents/semantic_map_planner_agent.py` & `alfworld-0.3.4/alfworld/gen/agents/semantic_map_planner_agent.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/constants.py` & `alfworld-0.3.4/alfworld/gen/constants.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/game_states/game_state_base.py` & `alfworld-0.3.4/alfworld/gen/game_states/game_state_base.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/game_states/planned_game_state.py` & `alfworld-0.3.4/alfworld/gen/game_states/planned_game_state.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/game_states/task_game_state.py` & `alfworld-0.3.4/alfworld/gen/game_states/task_game_state.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/game_states/task_game_state_full_knowledge.py` & `alfworld-0.3.4/alfworld/gen/game_states/task_game_state_full_knowledge.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/goal_library.py` & `alfworld-0.3.4/alfworld/gen/goal_library.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/graph/graph_obj.py` & `alfworld-0.3.4/alfworld/gen/graph/graph_obj.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan1-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan1-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan1-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan1-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan1-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan1-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan10-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan10-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan10-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan10-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan10-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan10-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan11-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan11-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan11-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan11-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan11-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan11-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan12-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan12-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan12-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan12-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan12-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan12-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan13-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan13-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan13-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan13-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan13-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan13-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan14-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan14-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan14-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan14-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan14-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan14-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan15-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan15-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan15-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan15-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan15-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan15-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan16-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan16-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan16-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan16-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan16-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan16-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan17-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan17-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan17-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan17-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan17-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan17-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan18-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan18-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan18-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan18-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan18-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan18-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan19-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan19-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan19-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan19-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan19-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan19-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan2-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan2-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan2-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan2-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan2-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan2-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan20-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan20-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan20-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan20-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan20-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan20-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan201-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan201-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan201-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan201-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan202-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan202-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan202-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan202-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan203-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan203-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan203-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan203-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan204-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan204-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan204-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan204-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan205-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan205-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan205-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan205-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan206-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan206-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan206-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan206-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan207-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan207-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan207-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan207-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan208-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan208-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan208-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan208-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan209-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan209-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan209-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan209-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan21-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan21-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan21-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan21-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan21-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan21-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan210-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan210-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan210-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan210-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan211-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan211-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan211-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan211-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan212-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan212-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan212-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan212-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan213-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan213-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan213-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan213-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan214-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan214-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan214-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan214-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan215-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan215-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan215-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan215-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan216-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan216-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan216-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan216-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan217-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan217-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan217-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan217-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan218-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan218-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan218-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan218-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan219-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan219-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan219-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan219-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan22-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan22-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan22-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan22-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan22-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan22-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan220-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan220-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan220-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan220-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan221-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan221-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan221-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan221-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan222-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan222-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan222-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan222-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan223-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan223-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan223-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan223-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan224-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan224-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan224-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan224-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan225-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan225-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan225-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan225-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan226-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan226-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan226-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan226-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan227-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan227-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan227-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan227-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan228-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan228-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan228-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan228-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan229-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan229-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan229-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan229-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan23-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan23-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan23-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan23-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan23-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan23-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan230-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan230-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan230-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan230-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan24-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan24-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan24-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan24-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan24-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan24-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan25-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan25-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan25-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan25-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan25-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan25-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan26-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan26-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan26-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan26-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan26-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan26-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan27-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan27-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan27-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan27-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan27-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan27-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan28-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan28-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan28-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan28-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan28-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan28-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan29-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan29-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan29-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan29-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan29-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan29-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan3-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan3-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan3-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan3-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan3-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan3-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan30-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan30-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan30-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan30-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan30-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan30-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan301-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan301-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan301-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan301-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan302-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan302-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan302-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan302-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan303-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan303-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan303-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan303-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan304-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan304-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan305-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan305-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan305-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan305-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan306-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan306-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan306-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan306-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan307-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan307-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan307-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan307-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan308-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan308-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan308-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan308-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan309-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan309-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan309-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan309-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan310-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan310-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan310-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan310-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan311-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan311-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan311-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan311-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan312-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan312-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan312-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan312-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan313-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan313-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan313-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan313-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan314-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan314-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan314-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan314-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan315-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan315-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan315-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan315-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan316-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan316-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan317-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan317-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan317-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan317-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan318-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan318-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan318-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan318-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan319-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan319-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan319-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan319-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan320-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan320-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan320-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan320-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan321-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan321-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan321-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan321-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan322-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan322-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan322-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan322-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan323-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan323-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan323-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan323-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan324-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan324-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan324-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan324-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan325-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan325-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan325-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan325-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan326-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan326-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan326-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan326-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan327-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan327-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan327-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan327-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan328-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan328-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan328-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan328-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan329-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan329-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan330-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan330-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan330-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan330-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan4-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan4-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan4-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan4-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan4-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan4-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan401-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan401-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan401-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan401-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan402-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan402-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan402-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan402-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan403-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan403-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan403-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan403-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan404-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan404-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan404-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan404-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan405-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan405-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan405-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan405-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan406-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan406-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan406-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan406-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan407-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan407-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan407-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan407-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan408-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan408-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan408-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan408-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan409-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan409-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan409-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan409-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan410-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan410-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan410-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan410-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan411-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan411-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan411-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan411-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan412-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan412-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan412-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan412-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan413-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan413-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan413-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan413-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan414-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan414-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan414-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan414-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan415-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan415-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan415-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan415-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan416-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan416-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan416-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan416-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan417-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan417-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan417-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan417-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan418-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan418-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan419-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan419-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan420-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan420-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan421-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan421-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan421-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan421-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan422-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan422-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan422-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan422-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan423-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan423-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan423-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan423-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan424-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan424-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan424-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan424-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan425-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan425-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan425-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan425-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan426-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan426-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan426-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan426-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan427-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan427-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan427-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan427-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan428-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan428-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan428-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan428-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan429-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan429-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan430-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan430-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan430-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan430-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan430-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan430-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan5-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan5-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan5-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan5-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan5-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan5-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan6-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan6-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan6-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan6-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan6-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan6-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan7-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan7-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan7-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan7-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan7-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan7-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan8-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan8-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan8-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan8-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan8-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan8-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan9-layout.npy` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan9-layout.npy`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan9-objects.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan9-objects.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/FloorPlan9-openable.json` & `alfworld-0.3.4/alfworld/gen/layouts/FloorPlan9-openable.json`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/layouts/precompute_layout_locations.py` & `alfworld-0.3.4/alfworld/gen/layouts/precompute_layout_locations.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/planner/ff_planner_handler.py` & `alfworld-0.3.4/alfworld/gen/planner/ff_planner_handler.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/utils/bb_util.py` & `alfworld-0.3.4/alfworld/gen/utils/bb_util.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/utils/dataset_management_util.py` & `alfworld-0.3.4/alfworld/gen/utils/dataset_management_util.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/utils/game_util.py` & `alfworld-0.3.4/alfworld/gen/utils/game_util.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/utils/image_util.py` & `alfworld-0.3.4/alfworld/gen/utils/image_util.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/utils/py_util.py` & `alfworld-0.3.4/alfworld/gen/utils/py_util.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/gen/utils/replay_json.py` & `alfworld-0.3.4/alfworld/gen/utils/replay_json.py`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/alfworld/info.py` & `alfworld-0.3.4/alfworld/info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 
 import os
 from os.path import join as pjoin
 
 from alfworld.utils import mkdirs
```

### Comparing `alfworld-0.3.3/alfworld.egg-info/PKG-INFO` & `alfworld-0.3.4/alfworld.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfworld
-Version: 0.3.3
+Version: 0.3.4
 Summary: ALFWorld - Aligning Text and Embodied Environments for Interactive Learning.
 License: MIT License
         
         Copyright (c) 2020 Mohit Shridhar and others
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `alfworld-0.3.3/alfworld.egg-info/SOURCES.txt` & `alfworld-0.3.4/alfworld.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/scripts/alfworld-download` & `alfworld-0.3.4/scripts/alfworld-download`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/scripts/alfworld-generate` & `alfworld-0.3.4/scripts/alfworld-generate`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/scripts/alfworld-play-thor` & `alfworld-0.3.4/scripts/alfworld-play-thor`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/scripts/alfworld-play-tw` & `alfworld-0.3.4/scripts/alfworld-play-tw`

 * *Files identical despite different names*

### Comparing `alfworld-0.3.3/setup.py` & `alfworld-0.3.4/setup.py`

 * *Files identical despite different names*

