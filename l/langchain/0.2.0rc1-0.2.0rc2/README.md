# Comparing `tmp/langchain-0.2.0rc1.tar.gz` & `tmp/langchain-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-0.2.0rc1.tar", max compression
+gzip compressed data, was "langchain-0.2.0rc2.tar", max compression
```

## Comparing `langchain-0.2.0rc1.tar` & `langchain-0.2.0rc2.tar`

### file list

```diff
@@ -1,1338 +1,1339 @@
--rw-r--r--   0        0        0     1067 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/LICENSE
--rw-r--r--   0        0        0     5778 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/README.md
--rw-r--r--   0        0        0    13708 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/__init__.py
--rw-r--r--   0        0        0      733 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/_api/__init__.py
--rw-r--r--   0        0        0      471 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/_api/deprecation.py
--rw-r--r--   0        0        0      139 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/_api/interactive_env.py
--rw-r--r--   0        0        0     6746 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/_api/module_import.py
--rw-r--r--   0        0        0      122 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/_api/path.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/adapters/__init__.py
--rw-r--r--   0        0        0     1996 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/adapters/openai.py
--rw-r--r--   0        0        0     6293 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/__init__.py
--rw-r--r--   0        0        0    56623 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent.py
--rw-r--r--   0        0        0    15135 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_iterator.py
--rw-r--r--   0        0        0     7364 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       25 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/ainetwork/__init__.py
--rw-r--r--   0        0        0      685 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/ainetwork/toolkit.py
--rw-r--r--   0        0        0      668 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/amadeus/toolkit.py
--rw-r--r--   0        0        0      771 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/azure_cognitive_services.py
--rw-r--r--   0        0        0       72 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/base.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/clickup/__init__.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/clickup/toolkit.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0     3235 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
--rw-r--r--   0        0        0       97 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/conversational_retrieval/tool.py
--rw-r--r--   0        0        0     1091 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0      782 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/file_management/__init__.py
--rw-r--r--   0        0        0      745 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/file_management/toolkit.py
--rw-r--r--   0        0        0       22 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/github/__init__.py
--rw-r--r--   0        0        0     2244 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/github/toolkit.py
--rw-r--r--   0        0        0       22 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/gitlab/__init__.py
--rw-r--r--   0        0        0      670 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/gitlab/toolkit.py
--rw-r--r--   0        0        0       21 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/gmail/__init__.py
--rw-r--r--   0        0        0      659 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/gmail/toolkit.py
--rw-r--r--   0        0        0       20 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/jira/__init__.py
--rw-r--r--   0        0        0      654 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/jira/toolkit.py
--rw-r--r--   0        0        0       18 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/json/__init__.py
--rw-r--r--   0        0        0      672 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/json/base.py
--rw-r--r--   0        0        0      749 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/json/prompt.py
--rw-r--r--   0        0        0      654 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/json/toolkit.py
--rw-r--r--   0        0        0       23 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/multion/__init__.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/multion/toolkit.py
--rw-r--r--   0        0        0       19 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/nasa/__init__.py
--rw-r--r--   0        0        0      654 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/nasa/toolkit.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/nla/__init__.py
--rw-r--r--   0        0        0      634 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/nla/tool.py
--rw-r--r--   0        0        0      649 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/nla/toolkit.py
--rw-r--r--   0        0        0       25 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/office365/__init__.py
--rw-r--r--   0        0        0      670 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/office365/toolkit.py
--rw-r--r--   0        0        0       26 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/__init__.py
--rw-r--r--   0        0        0      687 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/base.py
--rw-r--r--   0        0        0     1599 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/planner.py
--rw-r--r--   0        0        0     3526 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/planner_prompt.py
--rw-r--r--   0        0        0      909 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/prompt.py
--rw-r--r--   0        0        0      833 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/spec.py
--rw-r--r--   0        0        0      818 2024-05-08 04:43:20.138225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/toolkit.py
--rw-r--r--   0        0        0     1104 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/pandas/__init__.py
--rw-r--r--   0        0        0      762 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/playwright/__init__.py
--rw-r--r--   0        0        0      728 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/playwright/toolkit.py
--rw-r--r--   0        0        0       22 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/powerbi/__init__.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/powerbi/base.py
--rw-r--r--   0        0        0      717 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/powerbi/chat_base.py
--rw-r--r--   0        0        0     1084 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/powerbi/prompt.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/powerbi/toolkit.py
--rw-r--r--   0        0        0     1094 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/python/__init__.py
--rw-r--r--   0        0        0       21 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/slack/__init__.py
--rw-r--r--   0        0        0      659 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/slack/toolkit.py
--rw-r--r--   0        0        0     1103 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/spark/__init__.py
--rw-r--r--   0        0        0       23 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/spark_sql/__init__.py
--rw-r--r--   0        0        0      697 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/spark_sql/base.py
--rw-r--r--   0        0        0      783 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/spark_sql/prompt.py
--rw-r--r--   0        0        0      682 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/spark_sql/toolkit.py
--rw-r--r--   0        0        0       17 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/sql/__init__.py
--rw-r--r--   0        0        0      661 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/sql/base.py
--rw-r--r--   0        0        0      896 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/sql/prompt.py
--rw-r--r--   0        0        0      679 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/sql/toolkit.py
--rw-r--r--   0        0        0       21 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/steam/__init__.py
--rw-r--r--   0        0        0      659 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/steam/toolkit.py
--rw-r--r--   0        0        0       56 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/vectorstore/__init__.py
--rw-r--r--   0        0        0     4216 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/vectorstore/base.py
--rw-r--r--   0        0        0      834 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/vectorstore/prompt.py
--rw-r--r--   0        0        0     3289 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/vectorstore/toolkit.py
--rw-r--r--   0        0        0     1095 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0       22 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/zapier/__init__.py
--rw-r--r--   0        0        0      670 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_toolkits/zapier/toolkit.py
--rw-r--r--   0        0        0     1948 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/agent_types.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/chat/__init__.py
--rw-r--r--   0        0        0     5110 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/chat/base.py
--rw-r--r--   0        0        0     1977 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/chat/output_parser.py
--rw-r--r--   0        0        0     1158 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/chat/prompt.py
--rw-r--r--   0        0        0       75 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/conversational/__init__.py
--rw-r--r--   0        0        0     4979 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/conversational/base.py
--rw-r--r--   0        0        0     1383 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/conversational/output_parser.py
--rw-r--r--   0        0        0     1859 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/conversational/prompt.py
--rw-r--r--   0        0        0       75 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/conversational_chat/__init__.py
--rw-r--r--   0        0        0     5244 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/conversational_chat/base.py
--rw-r--r--   0        0        0     2394 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/conversational_chat/output_parser.py
--rw-r--r--   0        0        0     2763 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/conversational_chat/prompt.py
--rw-r--r--   0        0        0      955 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/format_scratchpad/__init__.py
--rw-r--r--   0        0        0      528 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/format_scratchpad/log.py
--rw-r--r--   0        0        0      721 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/format_scratchpad/log_to_messages.py
--rw-r--r--   0        0        0     2203 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/format_scratchpad/openai_functions.py
--rw-r--r--   0        0        0      166 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/format_scratchpad/openai_tools.py
--rw-r--r--   0        0        0     1853 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/format_scratchpad/tools.py
--rw-r--r--   0        0        0      578 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/format_scratchpad/xml.py
--rw-r--r--   0        0        0     3244 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/initialize.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/json_chat/__init__.py
--rw-r--r--   0        0        0     7743 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/json_chat/base.py
--rw-r--r--   0        0        0      551 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/json_chat/prompt.py
--rw-r--r--   0        0        0      286 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/load_tools.py
--rw-r--r--   0        0        0     4634 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/loading.py
--rw-r--r--   0        0        0       86 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/mrkl/__init__.py
--rw-r--r--   0        0        0     6064 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/mrkl/base.py
--rw-r--r--   0        0        0     3407 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/mrkl/output_parser.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/mrkl/prompt.py
--rw-r--r--   0        0        0      114 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/openai_assistant/__init__.py
--rw-r--r--   0        0        0    27654 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/openai_assistant/base.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/openai_functions_agent/__init__.py
--rw-r--r--   0        0        0     2761 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py
--rw-r--r--   0        0        0    11633 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/openai_functions_agent/base.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/openai_functions_multi_agent/__init__.py
--rw-r--r--   0        0        0    12006 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/openai_functions_multi_agent/base.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/openai_tools/__init__.py
--rw-r--r--   0        0        0     3435 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/openai_tools/base.py
--rw-r--r--   0        0        0     1373 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/output_parsers/__init__.py
--rw-r--r--   0        0        0     1846 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/output_parsers/json.py
--rw-r--r--   0        0        0     3467 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/output_parsers/openai_functions.py
--rw-r--r--   0        0        0     2317 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/output_parsers/openai_tools.py
--rw-r--r--   0        0        0     2455 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/output_parsers/react_json_single_input.py
--rw-r--r--   0        0        0     3218 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/output_parsers/react_single_input.py
--rw-r--r--   0        0        0     1545 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/output_parsers/self_ask.py
--rw-r--r--   0        0        0     3753 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/output_parsers/tools.py
--rw-r--r--   0        0        0     1658 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/output_parsers/xml.py
--rw-r--r--   0        0        0       76 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/react/__init__.py
--rw-r--r--   0        0        0     4975 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/react/agent.py
--rw-r--r--   0        0        0     5798 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/react/base.py
--rw-r--r--   0        0        0     1231 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/react/output_parser.py
--rw-r--r--   0        0        0     1906 2024-05-08 04:43:20.142225 langchain-0.2.0rc1/langchain/agents/react/textworld_prompt.py
--rw-r--r--   0        0        0     6127 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/react/wiki_prompt.py
--rw-r--r--   0        0        0     1175 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/schema.py
--rw-r--r--   0        0        0      106 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/self_ask_with_search/__init__.py
--rw-r--r--   0        0        0     8228 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/self_ask_with_search/base.py
--rw-r--r--   0        0        0      138 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/self_ask_with_search/output_parser.py
--rw-r--r--   0        0        0     1926 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/self_ask_with_search/prompt.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/structured_chat/__init__.py
--rw-r--r--   0        0        0    10812 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/structured_chat/base.py
--rw-r--r--   0        0        0     3799 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/structured_chat/output_parser.py
--rw-r--r--   0        0        0      992 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/structured_chat/prompt.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/tool_calling_agent/__init__.py
--rw-r--r--   0        0        0     3465 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/tool_calling_agent/base.py
--rw-r--r--   0        0        0     1409 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/tools.py
--rw-r--r--   0        0        0     1475 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/types.py
--rw-r--r--   0        0        0      384 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/utils.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/xml/__init__.py
--rw-r--r--   0        0        0     8103 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/xml/base.py
--rw-r--r--   0        0        0      767 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/agents/xml/prompt.py
--rw-r--r--   0        0        0      217 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/base_language.py
--rw-r--r--   0        0        0     2155 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/cache.py
--rw-r--r--   0        0        0     5960 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      941 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/aim_callback.py
--rw-r--r--   0        0        0      688 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/argilla_callback.py
--rw-r--r--   0        0        0      678 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/arize_callback.py
--rw-r--r--   0        0        0      683 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/arthur_callback.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/base.py
--rw-r--r--   0        0        0      688 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/clearml_callback.py
--rw-r--r--   0        0        0      684 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/comet_ml_callback.py
--rw-r--r--   0        0        0      695 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/confident_callback.py
--rw-r--r--   0        0        0      688 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/context_callback.py
--rw-r--r--   0        0        0       97 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/file.py
--rw-r--r--   0        0        0      678 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/flyte_callback.py
--rw-r--r--   0        0        0      997 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/human.py
--rw-r--r--   0        0        0      683 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/infino_callback.py
--rw-r--r--   0        0        0     1006 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/labelstudio_callback.py
--rw-r--r--   0        0        0      715 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/llmonitor_callback.py
--rw-r--r--   0        0        0     2410 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/manager.py
--rw-r--r--   0        0        0     1137 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/mlflow_callback.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/openai_info.py
--rw-r--r--   0        0        0      725 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/promptlayer_callback.py
--rw-r--r--   0        0        0      715 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/sagemaker_callback.py
--rw-r--r--   0        0        0      103 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/stdout.py
--rw-r--r--   0        0        0     2399 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/streaming_aiter.py
--rw-r--r--   0        0        0     3371 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/streaming_aiter_final_only.py
--rw-r--r--   0        0        0      173 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0     3357 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/streaming_stdout_final_only.py
--rw-r--r--   0        0        0     3407 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/streamlit/__init__.py
--rw-r--r--   0        0        0      937 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/streamlit/mutable_expander.py
--rw-r--r--   0        0        0     1372 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/streamlit/streamlit_callback_handler.py
--rw-r--r--   0        0        0     1140 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0      154 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/base.py
--rw-r--r--   0        0        0      800 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/comet.py
--rw-r--r--   0        0        0      233 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/evaluation.py
--rw-r--r--   0        0        0      218 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/langchain.py
--rw-r--r--   0        0        0       99 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/langchain_v1.py
--rw-r--r--   0        0        0      226 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/log_stream.py
--rw-r--r--   0        0        0     1384 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/logging.py
--rw-r--r--   0        0        0      105 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/root_listeners.py
--rw-r--r--   0        0        0      120 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/run_collector.py
--rw-r--r--   0        0        0      470 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/schemas.py
--rw-r--r--   0        0        0      168 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/stdout.py
--rw-r--r--   0        0        0      885 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/tracers/wandb.py
--rw-r--r--   0        0        0      693 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/trubrics_callback.py
--rw-r--r--   0        0        0     1409 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/utils.py
--rw-r--r--   0        0        0      678 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/wandb_callback.py
--rw-r--r--   0        0        0      688 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/callbacks/whylabs_callback.py
--rw-r--r--   0        0        0     4885 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/__init__.py
--rw-r--r--   0        0        0       84 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/__init__.py
--rw-r--r--   0        0        0    10003 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/base.py
--rw-r--r--   0        0        0     2452 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/news_docs.py
--rw-r--r--   0        0        0     3399 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/open_meteo_docs.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/openapi/__init__.py
--rw-r--r--   0        0        0      667 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/openapi/chain.py
--rw-r--r--   0        0        0      795 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/openapi/prompts.py
--rw-r--r--   0        0        0      963 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/openapi/requests_chain.py
--rw-r--r--   0        0        0      966 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/openapi/response_chain.py
--rw-r--r--   0        0        0     1920 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/podcast_docs.py
--rw-r--r--   0        0        0     1031 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/prompt.py
--rw-r--r--   0        0        0     1537 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/api/tmdb_docs.py
--rw-r--r--   0        0        0    30553 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/base.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/chat_vector_db/__init__.py
--rw-r--r--   0        0        0      694 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/chat_vector_db/prompts.py
--rw-r--r--   0        0        0      367 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/combine_documents/__init__.py
--rw-r--r--   0        0        0     8006 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/combine_documents/base.py
--rw-r--r--   0        0        0    11781 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/combine_documents/map_reduce.py
--rw-r--r--   0        0        0     8991 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/combine_documents/map_rerank.py
--rw-r--r--   0        0        0    13894 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/combine_documents/reduce.py
--rw-r--r--   0        0        0     9113 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/combine_documents/refine.py
--rw-r--r--   0        0        0    10958 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/combine_documents/stuff.py
--rw-r--r--   0        0        0      107 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/constitutional_ai/__init__.py
--rw-r--r--   0        0        0     6341 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/constitutional_ai/base.py
--rw-r--r--   0        0        0      283 2024-05-08 04:43:20.146225 langchain-0.2.0rc1/langchain/chains/constitutional_ai/models.py
--rw-r--r--   0        0        0    21738 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/constitutional_ai/principles.py
--rw-r--r--   0        0        0     8666 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/constitutional_ai/prompts.py
--rw-r--r--   0        0        0       71 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/conversation/__init__.py
--rw-r--r--   0        0        0     2366 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/conversation/base.py
--rw-r--r--   0        0        0     1396 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/conversation/memory.py
--rw-r--r--   0        0        0      913 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/conversation/prompt.py
--rw-r--r--   0        0        0       49 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0    20995 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/conversational_retrieval/base.py
--rw-r--r--   0        0        0      720 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/conversational_retrieval/prompts.py
--rw-r--r--   0        0        0      126 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/elasticsearch_database/__init__.py
--rw-r--r--   0        0        0     8287 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/elasticsearch_database/base.py
--rw-r--r--   0        0        0     1425 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/elasticsearch_database/prompts.py
--rw-r--r--   0        0        0     1514 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/ernie_functions/__init__.py
--rw-r--r--   0        0        0     1730 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/ernie_functions/base.py
--rw-r--r--   0        0        0      741 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/example_generator.py
--rw-r--r--   0        0        0       51 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/flare/__init__.py
--rw-r--r--   0        0        0     9081 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/flare/base.py
--rw-r--r--   0        0        0     1471 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/flare/prompts.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/__init__.py
--rw-r--r--   0        0        0      669 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/arangodb.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/base.py
--rw-r--r--   0        0        0     1205 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/cypher.py
--rw-r--r--   0        0        0      792 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/cypher_utils.py
--rw-r--r--   0        0        0      925 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/falkordb.py
--rw-r--r--   0        0        0     1090 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/gremlin.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/hugegraph.py
--rw-r--r--   0        0        0      870 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/kuzu.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/nebulagraph.py
--rw-r--r--   0        0        0     1232 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/neptune_cypher.py
--rw-r--r--   0        0        0     1137 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/neptune_sparql.py
--rw-r--r--   0        0        0      714 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/ontotext_graphdb.py
--rw-r--r--   0        0        0     3934 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/prompts.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/graph_qa/sparql.py
--rw-r--r--   0        0        0     2662 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/history_aware_retriever.py
--rw-r--r--   0        0        0       75 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/hyde/__init__.py
--rw-r--r--   0        0        0     3341 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/hyde/base.py
--rw-r--r--   0        0        0     1913 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/hyde/prompts.py
--rw-r--r--   0        0        0    15470 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm.py
--rw-r--r--   0        0        0      453 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_bash/__init__.py
--rw-r--r--   0        0        0      139 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_checker/__init__.py
--rw-r--r--   0        0        0     6190 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_checker/base.py
--rw-r--r--   0        0        0     1125 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_checker/prompt.py
--rw-r--r--   0        0        0      143 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_math/__init__.py
--rw-r--r--   0        0        0     6709 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_math/base.py
--rw-r--r--   0        0        0      868 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_math/prompt.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_requests.py
--rw-r--r--   0        0        0      352 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_summarization_checker/__init__.py
--rw-r--r--   0        0        0     6582 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_summarization_checker/base.py
--rw-r--r--   0        0        0      654 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
--rw-r--r--   0        0        0      377 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_summarization_checker/prompts/check_facts.txt
--rw-r--r--   0        0        0      128 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_summarization_checker/prompts/create_facts.txt
--rw-r--r--   0        0        0      416 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt
--rw-r--r--   0        0        0      470 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/llm_symbolic_math/__init__.py
--rw-r--r--   0        0        0    28297 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/loading.py
--rw-r--r--   0        0        0     3733 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/mapreduce.py
--rw-r--r--   0        0        0     3086 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/moderation.py
--rw-r--r--   0        0        0       96 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/natbot/__init__.py
--rw-r--r--   0        0        0     4778 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/natbot/base.py
--rw-r--r--   0        0        0    16050 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/natbot/crawler.py
--rw-r--r--   0        0        0     4989 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/natbot/prompt.py
--rw-r--r--   0        0        0     1403 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/openai_functions/__init__.py
--rw-r--r--   0        0        0    10172 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/openai_functions/base.py
--rw-r--r--   0        0        0     3558 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/openai_functions/citation_fuzzy_match.py
--rw-r--r--   0        0        0     7337 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/openai_functions/extraction.py
--rw-r--r--   0        0        0    11911 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/openai_functions/openapi.py
--rw-r--r--   0        0        0     3959 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/openai_functions/qa_with_structure.py
--rw-r--r--   0        0        0     2663 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/openai_functions/tagging.py
--rw-r--r--   0        0        0     1255 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/openai_functions/utils.py
--rw-r--r--   0        0        0      134 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/openai_tools/__init__.py
--rw-r--r--   0        0        0     3446 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/openai_tools/extraction.py
--rw-r--r--   0        0        0     2015 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/prompt_selector.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/qa_generation/__init__.py
--rw-r--r--   0        0        0     2465 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/qa_generation/base.py
--rw-r--r--   0        0        0     1875 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/qa_generation/prompt.py
--rw-r--r--   0        0        0      173 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/qa_with_sources/__init__.py
--rw-r--r--   0        0        0     7998 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/qa_with_sources/base.py
--rw-r--r--   0        0        0     7079 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/qa_with_sources/loading.py
--rw-r--r--   0        0        0     6971 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/qa_with_sources/map_reduce_prompt.py
--rw-r--r--   0        0        0     1318 2024-05-08 04:43:20.150225 langchain-0.2.0rc1/langchain/chains/qa_with_sources/refine_prompts.py
--rw-r--r--   0        0        0     2451 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/qa_with_sources/retrieval.py
--rw-r--r--   0        0        0     6581 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/qa_with_sources/stuff_prompt.py
--rw-r--r--   0        0        0     2770 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/qa_with_sources/vector_db.py
--rw-r--r--   0        0        0      131 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/query_constructor/__init__.py
--rw-r--r--   0        0        0    13680 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/query_constructor/base.py
--rw-r--r--   0        0        0      393 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/query_constructor/ir.py
--rw-r--r--   0        0        0     5694 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/query_constructor/parser.py
--rw-r--r--   0        0        0     6880 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/query_constructor/prompt.py
--rw-r--r--   0        0        0      321 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/query_constructor/schema.py
--rw-r--r--   0        0        0     8811 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/question_answering/__init__.py
--rw-r--r--   0        0        0     8013 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/question_answering/map_reduce_prompt.py
--rw-r--r--   0        0        0     1622 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/question_answering/map_rerank_prompt.py
--rw-r--r--   0        0        0     2378 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/question_answering/refine_prompts.py
--rw-r--r--   0        0        0     1146 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/question_answering/stuff_prompt.py
--rw-r--r--   0        0        0     2742 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/retrieval.py
--rw-r--r--   0        0        0       62 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/retrieval_qa/__init__.py
--rw-r--r--   0        0        0    11243 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/retrieval_qa/base.py
--rw-r--r--   0        0        0      399 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/retrieval_qa/prompt.py
--rw-r--r--   0        0        0      407 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/router/__init__.py
--rw-r--r--   0        0        0     4571 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/router/base.py
--rw-r--r--   0        0        0     3124 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/router/embedding_router.py
--rw-r--r--   0        0        0     4345 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/router/llm_router.py
--rw-r--r--   0        0        0     2245 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/router/multi_prompt.py
--rw-r--r--   0        0        0     1156 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/router/multi_prompt_prompt.py
--rw-r--r--   0        0        0     1079 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/router/multi_retrieval_prompt.py
--rw-r--r--   0        0        0     4227 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/router/multi_retrieval_qa.py
--rw-r--r--   0        0        0     7510 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/sequential.py
--rw-r--r--   0        0        0       47 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/sql_database/__init__.py
--rw-r--r--   0        0        0    15458 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/sql_database/prompt.py
--rw-r--r--   0        0        0     5367 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/sql_database/query.py
--rw-r--r--   0        0        0      204 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/structured_output/__init__.py
--rw-r--r--   0        0        0    25550 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/structured_output/base.py
--rw-r--r--   0        0        0      151 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/summarize/__init__.py
--rw-r--r--   0        0        0     6192 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/summarize/chain.py
--rw-r--r--   0        0        0      238 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/summarize/map_reduce_prompt.py
--rw-r--r--   0        0        0      677 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/summarize/refine_prompts.py
--rw-r--r--   0        0        0      238 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/summarize/stuff_prompt.py
--rw-r--r--   0        0        0     2369 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chains/transform.py
--rw-r--r--   0        0        0      452 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_loaders/__init__.py
--rw-r--r--   0        0        0       85 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_loaders/base.py
--rw-r--r--   0        0        0      884 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_loaders/facebook_messenger.py
--rw-r--r--   0        0        0      636 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_loaders/gmail.py
--rw-r--r--   0        0        0      663 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_loaders/imessage.py
--rw-r--r--   0        0        0      851 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_loaders/langsmith.py
--rw-r--r--   0        0        0      648 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_loaders/slack.py
--rw-r--r--   0        0        0      663 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_loaders/telegram.py
--rw-r--r--   0        0        0     1077 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_loaders/utils.py
--rw-r--r--   0        0        0      663 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_loaders/whatsapp.py
--rw-r--r--   0        0        0     1978 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/__init__.py
--rw-r--r--   0        0        0      851 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/anthropic.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/anyscale.py
--rw-r--r--   0        0        0      660 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/azure_openai.py
--rw-r--r--   0        0        0      863 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/azureml_endpoint.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/baichuan.py
--rw-r--r--   0        0        0      715 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0      268 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/base.py
--rw-r--r--   0        0        0      757 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/bedrock.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/cohere.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/databricks.py
--rw-r--r--   0        0        0      637 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/ernie.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/everlyai.py
--rw-r--r--   0        0        0      815 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/fake.py
--rw-r--r--   0        0        0      648 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/fireworks.py
--rw-r--r--   0        0        0      631 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/gigachat.py
--rw-r--r--   0        0        0      809 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/google_palm.py
--rw-r--r--   0        0        0      658 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/human.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/hunyuan.py
--rw-r--r--   0        0        0      821 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/javelin_ai_gateway.py
--rw-r--r--   0        0        0      631 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/jinachat.py
--rw-r--r--   0        0        0      628 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/konko.py
--rw-r--r--   0        0        0      791 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/litellm.py
--rw-r--r--   0        0        0      701 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/meta.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/minimax.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/mlflow.py
--rw-r--r--   0        0        0      815 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/mlflow_ai_gateway.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/ollama.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/openai.py
--rw-r--r--   0        0        0      683 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/pai_eas_endpoint.py
--rw-r--r--   0        0        0      696 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/promptlayer_openai.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/tongyi.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/vertexai.py
--rw-r--r--   0        0        0      845 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/volcengine_maas.py
--rw-r--r--   0        0        0      642 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/chat_models/yandex.py
--rw-r--r--   0        0        0     1245 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/docstore/__init__.py
--rw-r--r--   0        0        0      639 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/docstore/arbitrary_fn.py
--rw-r--r--   0        0        0      715 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/docstore/base.py
--rw-r--r--   0        0        0       70 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/docstore/document.py
--rw-r--r--   0        0        0      651 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/docstore/in_memory.py
--rw-r--r--   0        0        0      630 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/docstore/wikipedia.py
--rw-r--r--   0        0        0    20699 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/document_loaders/acreom.py
--rw-r--r--   0        0        0     1574 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/document_loaders/airbyte.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/document_loaders/airbyte_json.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/document_loaders/airtable.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/document_loaders/apify_dataset.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.154225 langchain-0.2.0rc1/langchain/document_loaders/arcgis_loader.py
--rw-r--r--   0        0        0      632 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/arxiv.py
--rw-r--r--   0        0        0      879 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/assemblyai.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/async_html.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/azlyrics.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/azure_ai_data.py
--rw-r--r--   0        0        0      698 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/azure_blob_storage_container.py
--rw-r--r--   0        0        0      683 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/azure_blob_storage_file.py
--rw-r--r--   0        0        0      758 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/baiducloud_bos_directory.py
--rw-r--r--   0        0        0      716 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/baiducloud_bos_file.py
--rw-r--r--   0        0        0      115 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/base.py
--rw-r--r--   0        0        0      661 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/base_o365.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/bibtex.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/bigquery.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/bilibili.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/blackboard.py
--rw-r--r--   0        0        0     1005 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/blob_loaders/__init__.py
--rw-r--r--   0        0        0      659 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/blob_loaders/file_system.py
--rw-r--r--   0        0        0      707 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/blob_loaders/schema.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/blob_loaders/youtube_audio.py
--rw-r--r--   0        0        0      852 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/blockchain.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/brave_search.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/browserless.py
--rw-r--r--   0        0        0      819 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/chatgpt.py
--rw-r--r--   0        0        0      656 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/chromium.py
--rw-r--r--   0        0        0      680 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/college_confidential.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/concurrent.py
--rw-r--r--   0        0        0      825 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/confluence.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/conllu.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/couchbase.py
--rw-r--r--   0        0        0      754 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/csv_loader.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/cube_semantic.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/datadog_logs.py
--rw-r--r--   0        0        0      838 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/dataframe.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/diffbot.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/directory.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/discord.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/docusaurus.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/dropbox.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/duckdb_loader.py
--rw-r--r--   0        0        0      818 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/email.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/epub.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/etherscan.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/evernote.py
--rw-r--r--   0        0        0      668 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/excel.py
--rw-r--r--   0        0        0      846 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/facebook_chat.py
--rw-r--r--   0        0        0      632 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/fauna.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/figma.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/gcs_directory.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/gcs_file.py
--rw-r--r--   0        0        0      654 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/generic.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/geodataframe.py
--rw-r--r--   0        0        0      626 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/git.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/gitbook.py
--rw-r--r--   0        0        0      832 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/github.py
--rw-r--r--   0        0        0      671 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/google_speech_to_text.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/googledrive.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/gutenberg.py
--rw-r--r--   0        0        0      812 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/helpers.py
--rw-r--r--   0        0        0      623 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/hn.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/html.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/html_bs.py
--rw-r--r--   0        0        0      671 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/hugging_face_dataset.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/ifixit.py
--rw-r--r--   0        0        0      668 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/image.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/image_captions.py
--rw-r--r--   0        0        0      632 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/imsdb.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/iugu.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/joplin.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/json_loader.py
--rw-r--r--   0        0        0      964 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/lakefs.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/larksuite.py
--rw-r--r--   0        0        0      683 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/markdown.py
--rw-r--r--   0        0        0      656 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/mastodon.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/max_compute.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/mediawikidump.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/merge.py
--rw-r--r--   0        0        0      632 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/mhtml.py
--rw-r--r--   0        0        0      659 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/modern_treasury.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/mongodb.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/news.py
--rw-r--r--   0        0        0      964 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/notebook.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/notion.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/notiondb.py
--rw-r--r--   0        0        0      649 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/nuclia.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/obs_directory.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/obs_file.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/obsidian.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/odt.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/onedrive.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/onedrive_file.py
--rw-r--r--   0        0        0      654 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/onenote.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/open_city_data.py
--rw-r--r--   0        0        0      680 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/org_mode.py
--rw-r--r--   0        0        0     2142 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/__init__.py
--rw-r--r--   0        0        0      985 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/audio.py
--rw-r--r--   0        0        0      821 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/docai.py
--rw-r--r--   0        0        0      694 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/generic.py
--rw-r--r--   0        0        0      848 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/grobid.py
--rw-r--r--   0        0        0      678 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/html/__init__.py
--rw-r--r--   0        0        0      678 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/html/bs4.py
--rw-r--r--   0        0        0      747 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/language/__init__.py
--rw-r--r--   0        0        0      710 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/language/cobol.py
--rw-r--r--   0        0        0      742 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/language/code_segmenter.py
--rw-r--r--   0        0        0      752 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/language/javascript.py
--rw-r--r--   0        0        0      747 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/language/language_parser.py
--rw-r--r--   0        0        0      715 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/language/python.py
--rw-r--r--   0        0        0      671 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/msword.py
--rw-r--r--   0        0        0     1662 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/pdf.py
--rw-r--r--   0        0        0      669 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/registry.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/parsers/txt.py
--rw-r--r--   0        0        0     2181 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/pdf.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/polars_dataframe.py
--rw-r--r--   0        0        0      689 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/powerpoint.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/psychic.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/pubmed.py
--rw-r--r--   0        0        0      718 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/pyspark_dataframe.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.158225 langchain-0.2.0rc1/langchain/document_loaders/python.py
--rw-r--r--   0        0        0      639 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/quip.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/readthedocs.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/recursive_url_loader.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/reddit.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/roam.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/rocksetdb.py
--rw-r--r--   0        0        0      649 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/rspace.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/rss.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/rst.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/rtf.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/s3_directory.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/s3_file.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/sharepoint.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/sitemap.py
--rw-r--r--   0        0        0      659 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/slack_directory.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/snowflake_loader.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/spreedly.py
--rw-r--r--   0        0        0      626 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/srt.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/stripe.py
--rw-r--r--   0        0        0     1122 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/telegram.py
--rw-r--r--   0        0        0      680 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/tencent_cos_directory.py
--rw-r--r--   0        0        0      659 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/tencent_cos_file.py
--rw-r--r--   0        0        0      668 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/tensorflow_datasets.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/text.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/tomarkdown.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/toml.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/trello.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/tsv.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/twitter.py
--rw-r--r--   0        0        0     1855 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/unstructured.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/url.py
--rw-r--r--   0        0        0     1033 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/url_playwright.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/url_selenium.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/weather.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/web_base.py
--rw-r--r--   0        0        0      846 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/whatsapp_chat.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/wikipedia.py
--rw-r--r--   0        0        0      821 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/word_document.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/xml.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/xorbits.py
--rw-r--r--   0        0        0      905 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_loaders/youtube.py
--rw-r--r--   0        0        0     2573 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/__init__.py
--rw-r--r--   0        0        0      687 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/beautiful_soup_transformer.py
--rw-r--r--   0        0        0      687 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/doctran_text_extract.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/doctran_text_qa.py
--rw-r--r--   0        0        0      678 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/doctran_text_translate.py
--rw-r--r--   0        0        0     1667 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/embeddings_redundant_filter.py
--rw-r--r--   0        0        0      693 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/google_translate.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/html2text.py
--rw-r--r--   0        0        0      663 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/long_context_reorder.py
--rw-r--r--   0        0        0      678 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/nuclia_text_transform.py
--rw-r--r--   0        0        0      929 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/openai_functions.py
--rw-r--r--   0        0        0     6033 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/document_transformers/xsl/html_chunks_with_headers.xslt
--rw-r--r--   0        0        0     8314 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/__init__.py
--rw-r--r--   0        0        0      890 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/aleph_alpha.py
--rw-r--r--   0        0        0      626 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/awa.py
--rw-r--r--   0        0        0      650 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/azure_openai.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0      113 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/base.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/bedrock.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/bookend.py
--rw-r--r--   0        0        0     8862 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/cache.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/clarifai.py
--rw-r--r--   0        0        0      756 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/cloudflare_workersai.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/cohere.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/dashscope.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/databricks.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/deepinfra.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/edenai.py
--rw-r--r--   0        0        0      656 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/elasticsearch.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/embaas.py
--rw-r--r--   0        0        0      632 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/ernie.py
--rw-r--r--   0        0        0      791 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/fake.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/fastembed.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/google_palm.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/gpt4all.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/gradient_ai.py
--rw-r--r--   0        0        0     1112 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/huggingface.py
--rw-r--r--   0        0        0      659 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/huggingface_hub.py
--rw-r--r--   0        0        0      895 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/infinity.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/javelin_ai_gateway.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/jina.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/johnsnowlabs.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/llamacpp.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/llm_rails.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/localai.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/minimax.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/mlflow.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/mlflow_gateway.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/modelscope_hub.py
--rw-r--r--   0        0        0      671 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/mosaicml.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/nlpcloud.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/octoai_embeddings.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/ollama.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/openai.py
--rw-r--r--   0        0        0      900 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/sagemaker_endpoint.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/self_hosted.py
--rw-r--r--   0        0        0      881 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/self_hosted_hugging_face.py
--rw-r--r--   0        0        0      667 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0      632 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/spacy_embeddings.py
--rw-r--r--   0        0        0      656 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/tensorflow_hub.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/vertexai.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/voyageai.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/embeddings/xinference.py
--rw-r--r--   0        0        0      476 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/env.py
--rw-r--r--   0        0        0     5803 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/evaluation/__init__.py
--rw-r--r--   0        0        0      165 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/evaluation/agents/__init__.py
--rw-r--r--   0        0        0    13915 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/evaluation/agents/trajectory_eval_chain.py
--rw-r--r--   0        0        0     5938 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/evaluation/agents/trajectory_eval_prompt.py
--rw-r--r--   0        0        0     1400 2024-05-08 04:43:20.162225 langchain-0.2.0rc1/langchain/evaluation/comparison/__init__.py
--rw-r--r--   0        0        0    15934 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/comparison/eval_chain.py
--rw-r--r--   0        0        0     2358 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/comparison/prompt.py
--rw-r--r--   0        0        0     1647 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/criteria/__init__.py
--rw-r--r--   0        0        0    21304 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/criteria/eval_chain.py
--rw-r--r--   0        0        0     1756 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/criteria/prompt.py
--rw-r--r--   0        0        0      323 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/embedding_distance/__init__.py
--rw-r--r--   0        0        0    17095 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/embedding_distance/base.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/exact_match/__init__.py
--rw-r--r--   0        0        0     2751 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/exact_match/base.py
--rw-r--r--   0        0        0     7327 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/loading.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/parsing/__init__.py
--rw-r--r--   0        0        0     5241 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/parsing/base.py
--rw-r--r--   0        0        0     3662 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/parsing/json_distance.py
--rw-r--r--   0        0        0     3180 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/parsing/json_schema.py
--rw-r--r--   0        0        0      344 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/qa/__init__.py
--rw-r--r--   0        0        0    10891 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/qa/eval_chain.py
--rw-r--r--   0        0        0     3911 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/qa/eval_prompt.py
--rw-r--r--   0        0        0     1052 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/qa/generate_chain.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/qa/generate_prompt.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/regex_match/__init__.py
--rw-r--r--   0        0        0     2407 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/regex_match/base.py
--rw-r--r--   0        0        0    18197 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/schema.py
--rw-r--r--   0        0        0     1112 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/scoring/__init__.py
--rw-r--r--   0        0        0    15476 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/scoring/eval_chain.py
--rw-r--r--   0        0        0     2129 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/scoring/prompt.py
--rw-r--r--   0        0        0      285 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/string_distance/__init__.py
--rw-r--r--   0        0        0    14019 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/evaluation/string_distance/base.py
--rw-r--r--   0        0        0      141 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/example_generator.py
--rw-r--r--   0        0        0      167 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/formatting.py
--rw-r--r--   0        0        0     7435 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/globals/__init__.py
--rw-r--r--   0        0        0     1527 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/__init__.py
--rw-r--r--   0        0        0      796 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/arangodb_graph.py
--rw-r--r--   0        0        0      618 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/falkordb_graph.py
--rw-r--r--   0        0        0      862 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/graph_document.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/graph_store.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/hugegraph.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/kuzu_graph.py
--rw-r--r--   0        0        0      618 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/memgraph_graph.py
--rw-r--r--   0        0        0      612 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/nebula_graph.py
--rw-r--r--   0        0        0      609 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/neo4j_graph.py
--rw-r--r--   0        0        0      615 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/neptune_graph.py
--rw-r--r--   0        0        0     1042 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/networkx_graph.py
--rw-r--r--   0        0        0      603 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/graphs/rdf_graph.py
--rw-r--r--   0        0        0     3462 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/hub.py
--rw-r--r--   0        0        0     1480 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/indexes/__init__.py
--rw-r--r--   0        0        0      252 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/indexes/_api.py
--rw-r--r--   0        0        0    20640 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/indexes/_sql_record_manager.py
--rw-r--r--   0        0        0      906 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/indexes/graph.py
--rw-r--r--   0        0        0      357 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/indexes/prompts/__init__.py
--rw-r--r--   0        0        0     1952 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/indexes/prompts/entity_extraction.py
--rw-r--r--   0        0        0     1157 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/indexes/prompts/entity_summarization.py
--rw-r--r--   0        0        0     1554 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/indexes/prompts/knowledge_triplet_extraction.py
--rw-r--r--   0        0        0     7067 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/indexes/vectorstore.py
--rw-r--r--   0        0        0      282 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/input.py
--rw-r--r--   0        0        0    17100 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/__init__.py
--rw-r--r--   0        0        0      735 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/ai21.py
--rw-r--r--   0        0        0      605 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/aleph_alpha.py
--rw-r--r--   0        0        0      623 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/amazon_api_gateway.py
--rw-r--r--   0        0        0      602 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/anthropic.py
--rw-r--r--   0        0        0      599 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/anyscale.py
--rw-r--r--   0        0        0      590 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/arcee.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/aviary.py
--rw-r--r--   0        0        0     1649 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/azureml_endpoint.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/bananadev.py
--rw-r--r--   0        0        0      228 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/base.py
--rw-r--r--   0        0        0      596 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/baseten.py
--rw-r--r--   0        0        0      587 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/beam.py
--rw-r--r--   0        0        0      738 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/bedrock.py
--rw-r--r--   0        0        0      617 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/bittensor.py
--rw-r--r--   0        0        0      608 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/cerebriumai.py
--rw-r--r--   0        0        0      596 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/chatglm.py
--rw-r--r--   0        0        0      599 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/clarifai.py
--rw-r--r--   0        0        0      680 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/cloudflare_workersai.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/cohere.py
--rw-r--r--   0        0        0      614 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/ctransformers.py
--rw-r--r--   0        0        0      608 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/ctranslate2.py
--rw-r--r--   0        0        0      605 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/databricks.py
--rw-r--r--   0        0        0      602 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/deepinfra.py
--rw-r--r--   0        0        0      605 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/deepsparse.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/edenai.py
--rw-r--r--   0        0        0      777 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/fake.py
--rw-r--r--   0        0        0      602 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/fireworks.py
--rw-r--r--   0        0        0      608 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/forefrontai.py
--rw-r--r--   0        0        0      599 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/gigachat.py
--rw-r--r--   0        0        0      605 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/google_palm.py
--rw-r--r--   0        0        0      596 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/gooseai.py
--rw-r--r--   0        0        0      596 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/gpt4all.py
--rw-r--r--   0        0        0      758 2024-05-08 04:43:20.166225 langchain-0.2.0rc1/langchain/llms/gradient_ai.py
--rw-r--r--   0        0        0      664 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/grammars/json.gbnf
--rw-r--r--   0        0        0      167 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/grammars/list.gbnf
--rw-r--r--   0        0        0      632 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/huggingface_endpoint.py
--rw-r--r--   0        0        0      617 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/huggingface_hub.py
--rw-r--r--   0        0        0      632 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/huggingface_pipeline.py
--rw-r--r--   0        0        0      656 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/huggingface_text_gen_inference.py
--rw-r--r--   0        0        0      614 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/human.py
--rw-r--r--   0        0        0      772 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/javelin_ai_gateway.py
--rw-r--r--   0        0        0      611 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/koboldai.py
--rw-r--r--   0        0        0      599 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/llamacpp.py
--rw-r--r--   0        0        0      736 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/loading.py
--rw-r--r--   0        0        0      620 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/manifest.py
--rw-r--r--   0        0        0      596 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/minimax.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/mlflow.py
--rw-r--r--   0        0        0      620 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/mlflow_ai_gateway.py
--rw-r--r--   0        0        0      590 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/modal.py
--rw-r--r--   0        0        0      599 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/mosaicml.py
--rw-r--r--   0        0        0      599 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/nlpcloud.py
--rw-r--r--   0        0        0      617 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/octoai_endpoint.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/ollama.py
--rw-r--r--   0        0        0      614 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/opaqueprompts.py
--rw-r--r--   0        0        0      885 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/openai.py
--rw-r--r--   0        0        0      596 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/openllm.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/openlm.py
--rw-r--r--   0        0        0      617 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/pai_eas_endpoint.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/petals.py
--rw-r--r--   0        0        0      605 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/pipelineai.py
--rw-r--r--   0        0        0      602 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/predibase.py
--rw-r--r--   0        0        0      620 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/predictionguard.py
--rw-r--r--   0        0        0      742 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/promptlayer_openai.py
--rw-r--r--   0        0        0      602 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/replicate.py
--rw-r--r--   0        0        0      587 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/rwkv.py
--rw-r--r--   0        0        0      808 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/self_hosted.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/self_hosted_hugging_face.py
--rw-r--r--   0        0        0      611 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/stochasticai.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/symblai_nebula.py
--rw-r--r--   0        0        0      596 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/textgen.py
--rw-r--r--   0        0        0      611 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/titan_takeoff.py
--rw-r--r--   0        0        0      620 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/titan_takeoff_pro.py
--rw-r--r--   0        0        0      599 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/together.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/tongyi.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/utils.py
--rw-r--r--   0        0        0      709 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/vertexai.py
--rw-r--r--   0        0        0      670 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/vllm.py
--rw-r--r--   0        0        0      805 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/volcengine_maas.py
--rw-r--r--   0        0        0      605 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/watsonxllm.py
--rw-r--r--   0        0        0      593 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/writer.py
--rw-r--r--   0        0        0      605 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/xinference.py
--rw-r--r--   0        0        0      602 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/llms/yandex.py
--rw-r--r--   0        0        0      206 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/load/__init__.py
--rw-r--r--   0        0        0      100 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/load/dump.py
--rw-r--r--   0        0        0       98 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/load/load.py
--rw-r--r--   0        0        0      412 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/load/serializable.py
--rw-r--r--   0        0        0     5389 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/__init__.py
--rw-r--r--   0        0        0     4861 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/buffer.py
--rw-r--r--   0        0        0     1616 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/buffer_window.py
--rw-r--r--   0        0        0     2795 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_memory.py
--rw-r--r--   0        0        0     3506 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/__init__.py
--rw-r--r--   0        0        0      692 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/astradb.py
--rw-r--r--   0        0        0      698 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/cassandra.py
--rw-r--r--   0        0        0      695 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/cosmos_db.py
--rw-r--r--   0        0        0      695 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/dynamodb.py
--rw-r--r--   0        0        0      727 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/elasticsearch.py
--rw-r--r--   0        0        0      683 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/file.py
--rw-r--r--   0        0        0      698 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/firestore.py
--rw-r--r--   0        0        0      130 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/in_memory.py
--rw-r--r--   0        0        0      692 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/momento.py
--rw-r--r--   0        0        0      692 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/mongodb.py
--rw-r--r--   0        0        0      686 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/neo4j.py
--rw-r--r--   0        0        0      695 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/postgres.py
--rw-r--r--   0        0        0      686 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/redis.py
--rw-r--r--   0        0        0      692 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/rocksetdb.py
--rw-r--r--   0        0        0      727 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/singlestoredb.py
--rw-r--r--   0        0        0     1033 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/sql.py
--rw-r--r--   0        0        0      698 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/streamlit.py
--rw-r--r--   0        0        0      724 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/upstash_redis.py
--rw-r--r--   0        0        0      683 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/xata.py
--rw-r--r--   0        0        0      680 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/chat_message_histories/zep.py
--rw-r--r--   0        0        0     2912 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/combined.py
--rw-r--r--   0        0        0    15936 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/entity.py
--rw-r--r--   0        0        0      645 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/kg.py
--rw-r--r--   0        0        0      658 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/motorhead_memory.py
--rw-r--r--   0        0        0     8181 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/prompt.py
--rw-r--r--   0        0        0      792 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/readonly.py
--rw-r--r--   0        0        0      761 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/simple.py
--rw-r--r--   0        0        0     3389 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/summary.py
--rw-r--r--   0        0        0     2949 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/summary_buffer.py
--rw-r--r--   0        0        0     2144 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/token_buffer.py
--rw-r--r--   0        0        0      617 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/utils.py
--rw-r--r--   0        0        0     3875 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/vectorstore.py
--rw-r--r--   0        0        0      628 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/memory/zep_memory.py
--rw-r--r--   0        0        0     3278 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/model_laboratory.py
--rw-r--r--   0        0        0     2719 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     1689 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/boolean.py
--rw-r--r--   0        0        0     1799 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/combining.py
--rw-r--r--   0        0        0     1974 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1205 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/enum.py
--rw-r--r--   0        0        0     1427 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/ernie_functions.py
--rw-r--r--   0        0        0     3150 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/fix.py
--rw-r--r--   0        0        0     3958 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/format_instructions.py
--rw-r--r--   0        0        0      340 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/json.py
--rw-r--r--   0        0        0      310 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/list.py
--rw-r--r--   0        0        0      702 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/loading.py
--rw-r--r--   0        0        0      364 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/openai_functions.py
--rw-r--r--   0        0        0      229 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/openai_tools.py
--rw-r--r--   0        0        0     6548 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/pandas_dataframe.py
--rw-r--r--   0        0        0      508 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/prompts.py
--rw-r--r--   0        0        0       99 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/pydantic.py
--rw-r--r--   0        0        0      691 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/rail_parser.py
--rw-r--r--   0        0        0     1214 2024-05-08 04:43:20.170225 langchain-0.2.0rc1/langchain/output_parsers/regex.py
--rw-r--r--   0        0        0     1709 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/output_parsers/regex_dict.py
--rw-r--r--   0        0        0     7786 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/output_parsers/retry.py
--rw-r--r--   0        0        0     3132 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/output_parsers/structured.py
--rw-r--r--   0        0        0       93 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/output_parsers/xml.py
--rw-r--r--   0        0        0     2181 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/output_parsers/yaml.py
--rw-r--r--   0        0        0     3152 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/__init__.py
--rw-r--r--   0        0        0      565 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/base.py
--rw-r--r--   0        0        0     1045 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/chat.py
--rw-r--r--   0        0        0     1152 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/example_selector/__init__.py
--rw-r--r--   0        0        0      105 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/example_selector/base.py
--rw-r--r--   0        0        0      136 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/example_selector/length_based.py
--rw-r--r--   0        0        0      877 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/example_selector/ngram_overlap.py
--rw-r--r--   0        0        0      288 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/example_selector/semantic_similarity.py
--rw-r--r--   0        0        0      265 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/few_shot.py
--rw-r--r--   0        0        0      128 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/few_shot_with_templates.py
--rw-r--r--   0        0        0      530 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/loading.py
--rw-r--r--   0        0        0      133 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/pipeline.py
--rw-r--r--   0        0        0      153 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/prompts/prompt.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/py.typed
--rw-r--r--   0        0        0      897 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      134 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      120 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/pydantic_v1/main.py
--rw-r--r--   0        0        0      462 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/python.py
--rw-r--r--   0        0        0      905 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/requests.py
--rw-r--r--   0        0        0     6660 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/__init__.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/arcee.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/arxiv.py
--rw-r--r--   0        0        0      824 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/azure_ai_search.py
--rw-r--r--   0        0        0      979 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/bedrock.py
--rw-r--r--   0        0        0      819 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/bm25.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/chaindesk.py
--rw-r--r--   0        0        0      653 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/chatgpt_plugin_retriever.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/cohere_rag_retriever.py
--rw-r--r--   0        0        0     2290 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/contextual_compression.py
--rw-r--r--   0        0        0      661 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/databerry.py
--rw-r--r--   0        0        0      791 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/docarray.py
--rw-r--r--   0        0        0      834 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/__init__.py
--rw-r--r--   0        0        0     2942 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/base.py
--rw-r--r--   0        0        0     4012 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/chain_extract.py
--rw-r--r--   0        0        0      366 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/chain_extract_prompt.py
--rw-r--r--   0        0        0     2762 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/chain_filter.py
--rw-r--r--   0        0        0      231 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/chain_filter_prompt.py
--rw-r--r--   0        0        0     4542 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/cohere_rerank.py
--rw-r--r--   0        0        0      393 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/cross_encoder.py
--rw-r--r--   0        0        0     1597 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/cross_encoder_rerank.py
--rw-r--r--   0        0        0     3614 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/embeddings_filter.py
--rw-r--r--   0        0        0     2503 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/document_compressors/flashrank_rerank.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/elastic_search_bm25.py
--rw-r--r--   0        0        0      644 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/embedchain.py
--rw-r--r--   0        0        0     9991 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/ensemble.py
--rw-r--r--   0        0        0      695 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/google_cloud_documentai_warehouse.py
--rw-r--r--   0        0        0     1040 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/google_vertex_ai_search.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/kay.py
--rw-r--r--   0        0        0     2235 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/kendra.py
--rw-r--r--   0        0        0      623 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/knn.py
--rw-r--r--   0        0        0      800 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/llama_index.py
--rw-r--r--   0        0        0     3601 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/merger_retriever.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/metal.py
--rw-r--r--   0        0        0      796 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/milvus.py
--rw-r--r--   0        0        0     6760 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/multi_query.py
--rw-r--r--   0        0        0     3920 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/multi_vector.py
--rw-r--r--   0        0        0      635 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/outline.py
--rw-r--r--   0        0        0     5198 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/parent_document_retriever.py
--rw-r--r--   0        0        0      674 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/pinecone_hybrid_search.py
--rw-r--r--   0        0        0      632 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/pubmed.py
--rw-r--r--   0        0        0      632 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/pupmed.py
--rw-r--r--   0        0        0     2654 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/re_phraser.py
--rw-r--r--   0        0        0      659 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/remote_retriever.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/__init__.py
--rw-r--r--   0        0        0      670 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/astradb.py
--rw-r--r--   0        0        0    12134 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/base.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/chroma.py
--rw-r--r--   0        0        0      685 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/dashvector.py
--rw-r--r--   0        0        0      782 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/databricks_vector_search.py
--rw-r--r--   0        0        0      816 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/deeplake.py
--rw-r--r--   0        0        0      666 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/dingo.py
--rw-r--r--   0        0        0      717 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/elasticsearch.py
--rw-r--r--   0        0        0      792 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/milvus.py
--rw-r--r--   0        0        0      714 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/mongodb_atlas.py
--rw-r--r--   0        0        0      670 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/myscale.py
--rw-r--r--   0        0        0      685 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/opensearch.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/pgvector.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/pinecone.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/qdrant.py
--rw-r--r--   0        0        0      660 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/redis.py
--rw-r--r--   0        0        0      693 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/supabase.py
--rw-r--r--   0        0        0      743 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/tencentvectordb.py
--rw-r--r--   0        0        0      743 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/timescalevector.py
--rw-r--r--   0        0        0      798 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/vectara.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/self_query/weaviate.py
--rw-r--r--   0        0        0      623 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/svm.py
--rw-r--r--   0        0        0      833 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/tavily_search_api.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/tfidf.py
--rw-r--r--   0        0        0     7665 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/time_weighted_retriever.py
--rw-r--r--   0        0        0      629 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/vespa_retriever.py
--rw-r--r--   0        0        0      674 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/weaviate_hybrid_search.py
--rw-r--r--   0        0        0      939 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/web_research.py
--rw-r--r--   0        0        0      641 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/wikipedia.py
--rw-r--r--   0        0        0      623 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/you.py
--rw-r--r--   0        0        0      855 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/zep.py
--rw-r--r--   0        0        0      796 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/retrievers/zilliz.py
--rw-r--r--   0        0        0      693 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/runnables/__init__.py
--rw-r--r--   0        0        0      809 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/runnables/hub.py
--rw-r--r--   0        0        0     1525 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/runnables/openai_functions.py
--rw-r--r--   0        0        0     2065 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/schema/__init__.py
--rw-r--r--   0        0        0      149 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/schema/agent.py
--rw-r--r--   0        0        0      105 2024-05-08 04:43:20.174225 langchain-0.2.0rc1/langchain/schema/cache.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/__init__.py
--rw-r--r--   0        0        0      511 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/base.py
--rw-r--r--   0        0        0     1511 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/manager.py
--rw-r--r--   0        0        0      103 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/stdout.py
--rw-r--r--   0        0        0      131 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0      113 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/tracers/base.py
--rw-r--r--   0        0        0      176 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/tracers/evaluation.py
--rw-r--r--   0        0        0      219 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/tracers/langchain.py
--rw-r--r--   0        0        0      127 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/tracers/langchain_v1.py
--rw-r--r--   0        0        0      226 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/tracers/log_stream.py
--rw-r--r--   0        0        0      105 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/tracers/root_listeners.py
--rw-r--r--   0        0        0      120 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/tracers/run_collector.py
--rw-r--r--   0        0        0      470 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/tracers/schemas.py
--rw-r--r--   0        0        0      257 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/callbacks/tracers/stdout.py
--rw-r--r--   0        0        0       80 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/chat.py
--rw-r--r--   0        0        0      101 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/chat_history.py
--rw-r--r--   0        0        0      122 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/document.py
--rw-r--r--   0        0        0       75 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/embeddings.py
--rw-r--r--   0        0        0       91 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/exceptions.py
--rw-r--r--   0        0        0      367 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/language_model.py
--rw-r--r--   0        0        0       71 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/memory.py
--rw-r--r--   0        0        0     1048 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/messages.py
--rw-r--r--   0        0        0      320 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/output.py
--rw-r--r--   0        0        0      651 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/output_parser.py
--rw-r--r--   0        0        0       80 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/prompt.py
--rw-r--r--   0        0        0      124 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/prompt_template.py
--rw-r--r--   0        0        0       81 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/retriever.py
--rw-r--r--   0        0        0     1796 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/__init__.py
--rw-r--r--   0        0        0      781 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/base.py
--rw-r--r--   0        0        0       89 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/branch.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/config.py
--rw-r--r--   0        0        0      333 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/configurable.py
--rw-r--r--   0        0        0      106 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/fallbacks.py
--rw-r--r--   0        0        0      260 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/history.py
--rw-r--r--   0        0        0      205 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/passthrough.py
--rw-r--r--   0        0        0       94 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/retry.py
--rw-r--r--   0        0        0      117 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/router.py
--rw-r--r--   0        0        0     1118 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/runnable/utils.py
--rw-r--r--   0        0        0       85 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/storage.py
--rw-r--r--   0        0        0      137 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/schema/vectorstore.py
--rw-r--r--   0        0        0      662 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/serpapi.py
--rw-r--r--   0        0        0     3544 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/smith/__init__.py
--rw-r--r--   0        0        0     2199 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/smith/evaluation/__init__.py
--rw-r--r--   0        0        0    13429 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/smith/evaluation/config.py
--rw-r--r--   0        0        0     9936 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/smith/evaluation/name_generation.py
--rw-r--r--   0        0        0     3310 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/smith/evaluation/progress.py
--rw-r--r--   0        0        0    54230 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/smith/evaluation/runner_utils.py
--rw-r--r--   0        0        0    17112 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/smith/evaluation/string_run_evaluator.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/smith/evaluation/utils.py
--rw-r--r--   0        0        0      663 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/sql_database.py
--rw-r--r--   0        0        0     1584 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/storage/__init__.py
--rw-r--r--   0        0        0     2517 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/storage/_lc_store.py
--rw-r--r--   0        0        0     4333 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/storage/encoder_backed.py
--rw-r--r--   0        0        0       89 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/storage/exceptions.py
--rw-r--r--   0        0        0     5516 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/storage/file_system.py
--rw-r--r--   0        0        0      368 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/storage/in_memory.py
--rw-r--r--   0        0        0      611 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/storage/redis.py
--rw-r--r--   0        0        0      751 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/storage/upstash_redis.py
--rw-r--r--   0        0        0     1553 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/text_splitter.py
--rw-r--r--   0        0        0     5662 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/ainetwork/__init__.py
--rw-r--r--   0        0        0      863 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/ainetwork/app.py
--rw-r--r--   0        0        0      748 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/ainetwork/base.py
--rw-r--r--   0        0        0      767 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/ainetwork/owner.py
--rw-r--r--   0        0        0      762 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/ainetwork/rule.py
--rw-r--r--   0        0        0      785 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/ainetwork/transfer.py
--rw-r--r--   0        0        0      770 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/ainetwork/value.py
--rw-r--r--   0        0        0      905 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/amadeus/__init__.py
--rw-r--r--   0        0        0      648 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/amadeus/base.py
--rw-r--r--   0        0        0      851 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/amadeus/closest_airport.py
--rw-r--r--   0        0        0      833 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/amadeus/flight_search.py
--rw-r--r--   0        0        0       25 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/arxiv/__init__.py
--rw-r--r--   0        0        0      763 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/arxiv/tool.py
--rw-r--r--   0        0        0     1258 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/__init__.py
--rw-r--r--   0        0        0      658 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/form_recognizer.py
--rw-r--r--   0        0        0      655 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/image_analysis.py
--rw-r--r--   0        0        0      649 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/speech2text.py
--rw-r--r--   0        0        0      649 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/text2speech.py
--rw-r--r--   0        0        0      673 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/text_analytics_health.py
--rw-r--r--   0        0        0      332 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/base.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/bearly/__init__.py
--rw-r--r--   0        0        0      957 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/bearly/tool.py
--rw-r--r--   0        0        0      752 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/bing_search/__init__.py
--rw-r--r--   0        0        0      721 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/bing_search/tool.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/brave_search/__init__.py
--rw-r--r--   0        0        0      610 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/brave_search/tool.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/clickup/__init__.py
--rw-r--r--   0        0        0      642 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/clickup/tool.py
--rw-r--r--   0        0        0      157 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/convert_to_openai.py
--rw-r--r--   0        0        0      927 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/dataforseo_api_search/__init__.py
--rw-r--r--   0        0        0      897 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/dataforseo_api_search/tool.py
--rw-r--r--   0        0        0      671 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/ddg_search/__init__.py
--rw-r--r--   0        0        0     1024 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/ddg_search/tool.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.178225 langchain-0.2.0rc1/langchain/tools/e2b_data_analysis/__init__.py
--rw-r--r--   0        0        0      990 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/e2b_data_analysis/tool.py
--rw-r--r--   0        0        0     1513 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/edenai/__init__.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/edenai/audio_speech_to_text.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/edenai/audio_text_to_speech.py
--rw-r--r--   0        0        0      607 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/edenai/edenai_base_tool.py
--rw-r--r--   0        0        0      646 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/edenai/image_explicitcontent.py
--rw-r--r--   0        0        0      652 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/edenai/image_objectdetection.py
--rw-r--r--   0        0        0      634 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/edenai/ocr_identityparser.py
--rw-r--r--   0        0        0      649 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/edenai/ocr_invoiceparser.py
--rw-r--r--   0        0        0      649 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/edenai/text_moderation.py
--rw-r--r--   0        0        0      686 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/eleven_labs/__init__.py
--rw-r--r--   0        0        0      660 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/eleven_labs/models.py
--rw-r--r--   0        0        0      652 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/eleven_labs/text2speech.py
--rw-r--r--   0        0        0     1242 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/file_management/__init__.py
--rw-r--r--   0        0        0      789 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/file_management/copy.py
--rw-r--r--   0        0        0      805 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/file_management/delete.py
--rw-r--r--   0        0        0      815 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/file_management/file_search.py
--rw-r--r--   0        0        0      836 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/file_management/list_dir.py
--rw-r--r--   0        0        0      789 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/file_management/move.py
--rw-r--r--   0        0        0      789 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/file_management/read.py
--rw-r--r--   0        0        0      797 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/file_management/write.py
--rw-r--r--   0        0        0       20 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/github/__init__.py
--rw-r--r--   0        0        0      637 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/github/tool.py
--rw-r--r--   0        0        0       20 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/gitlab/__init__.py
--rw-r--r--   0        0        0      637 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/gitlab/tool.py
--rw-r--r--   0        0        0     1056 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/gmail/__init__.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/gmail/base.py
--rw-r--r--   0        0        0      809 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/gmail/create_draft.py
--rw-r--r--   0        0        0      801 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/gmail/get_message.py
--rw-r--r--   0        0        0      793 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/gmail/get_thread.py
--rw-r--r--   0        0        0      863 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/gmail/search.py
--rw-r--r--   0        0        0      809 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/gmail/send_message.py
--rw-r--r--   0        0        0      681 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/golden_query/__init__.py
--rw-r--r--   0        0        0      655 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/golden_query/tool.py
--rw-r--r--   0        0        0      684 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_cloud/__init__.py
--rw-r--r--   0        0        0      658 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_cloud/texttospeech.py
--rw-r--r--   0        0        0      720 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_finance/__init__.py
--rw-r--r--   0        0        0      686 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_finance/tool.py
--rw-r--r--   0        0        0      696 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_jobs/__init__.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_jobs/tool.py
--rw-r--r--   0        0        0      696 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_lens/__init__.py
--rw-r--r--   0        0        0      665 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_lens/tool.py
--rw-r--r--   0        0        0      658 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_places/__init__.py
--rw-r--r--   0        0        0      812 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_places/tool.py
--rw-r--r--   0        0        0      720 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_scholar/__init__.py
--rw-r--r--   0        0        0      686 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_scholar/tool.py
--rw-r--r--   0        0        0      766 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_search/__init__.py
--rw-r--r--   0        0        0      733 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_search/tool.py
--rw-r--r--   0        0        0      815 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_serper/__init__.py
--rw-r--r--   0        0        0      733 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_serper/tool.py
--rw-r--r--   0        0        0      714 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_trends/__init__.py
--rw-r--r--   0        0        0      681 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/google_trends/tool.py
--rw-r--r--   0        0        0       47 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/graphql/__init__.py
--rw-r--r--   0        0        0      622 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/graphql/tool.py
--rw-r--r--   0        0        0      655 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/human/__init__.py
--rw-r--r--   0        0        0      616 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/human/tool.py
--rw-r--r--   0        0        0      613 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/ifttt.py
--rw-r--r--   0        0        0       43 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/interaction/__init__.py
--rw-r--r--   0        0        0      625 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/interaction/tool.py
--rw-r--r--   0        0        0       17 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/jira/__init__.py
--rw-r--r--   0        0        0      607 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/jira/tool.py
--rw-r--r--   0        0        0       46 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/json/__init__.py
--rw-r--r--   0        0        0      859 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/json/tool.py
--rw-r--r--   0        0        0      677 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/memorize/__init__.py
--rw-r--r--   0        0        0      733 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/memorize/tool.py
--rw-r--r--   0        0        0       35 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/merriam_webster/__init__.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/merriam_webster/tool.py
--rw-r--r--   0        0        0      675 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/metaphor_search/__init__.py
--rw-r--r--   0        0        0      640 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/metaphor_search/tool.py
--rw-r--r--   0        0        0     1105 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/multion/__init__.py
--rw-r--r--   0        0        0      833 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/multion/close_session.py
--rw-r--r--   0        0        0      842 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/multion/create_session.py
--rw-r--r--   0        0        0      842 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/multion/update_session.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/nasa/__init__.py
--rw-r--r--   0        0        0      607 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/nasa/tool.py
--rw-r--r--   0        0        0      667 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/nuclia/__init__.py
--rw-r--r--   0        0        0      760 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/nuclia/tool.py
--rw-r--r--   0        0        0     1085 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/office365/__init__.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/office365/base.py
--rw-r--r--   0        0        0      905 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/office365/create_draft_message.py
--rw-r--r--   0        0        0      819 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/office365/events_search.py
--rw-r--r--   0        0        0      823 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/office365/messages_search.py
--rw-r--r--   0        0        0      798 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/office365/send_event.py
--rw-r--r--   0        0        0      814 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/office365/send_message.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/openapi/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/openapi/utils/__init__.py
--rw-r--r--   0        0        0     1859 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/openapi/utils/api_models.py
--rw-r--r--   0        0        0      833 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/openapi/utils/openapi_utils.py
--rw-r--r--   0        0        0      677 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/openweathermap/__init__.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/openweathermap/tool.py
--rw-r--r--   0        0        0     1282 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/playwright/__init__.py
--rw-r--r--   0        0        0      654 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/playwright/base.py
--rw-r--r--   0        0        0      775 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/playwright/click.py
--rw-r--r--   0        0        0      631 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/playwright/current_page.py
--rw-r--r--   0        0        0      906 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/playwright/extract_hyperlinks.py
--rw-r--r--   0        0        0      622 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/playwright/extract_text.py
--rw-r--r--   0        0        0      825 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/playwright/get_elements.py
--rw-r--r--   0        0        0      799 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/playwright/navigate.py
--rw-r--r--   0        0        0      625 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/playwright/navigate_back.py
--rw-r--r--   0        0        0      935 2024-05-08 04:43:20.182225 langchain-0.2.0rc1/langchain/tools/plugin.py
--rw-r--r--   0        0        0       52 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/powerbi/__init__.py
--rw-r--r--   0        0        0      849 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/powerbi/tool.py
--rw-r--r--   0        0        0       26 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/pubmed/__init__.py
--rw-r--r--   0        0        0      619 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/pubmed/tool.py
--rw-r--r--   0        0        0      515 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/python/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/reddit_search/__init__.py
--rw-r--r--   0        0        0      730 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/reddit_search/tool.py
--rw-r--r--   0        0        0      705 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/render.py
--rw-r--r--   0        0        0       52 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/requests/__init__.py
--rw-r--r--   0        0        0     1167 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/requests/tool.py
--rw-r--r--   0        0        0      328 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/retriever.py
--rw-r--r--   0        0        0       31 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/scenexplain/__init__.py
--rw-r--r--   0        0        0      799 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/scenexplain/tool.py
--rw-r--r--   0        0        0      797 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/searchapi/__init__.py
--rw-r--r--   0        0        0      715 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/searchapi/tool.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/searx_search/__init__.py
--rw-r--r--   0        0        0      727 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/searx_search/tool.py
--rw-r--r--   0        0        0      622 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/shell/__init__.py
--rw-r--r--   0        0        0      751 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/shell/tool.py
--rw-r--r--   0        0        0      983 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/slack/__init__.py
--rw-r--r--   0        0        0      638 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/slack/base.py
--rw-r--r--   0        0        0      622 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/slack/get_channel.py
--rw-r--r--   0        0        0      816 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/slack/get_message.py
--rw-r--r--   0        0        0      841 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/slack/schedule_message.py
--rw-r--r--   0        0        0      809 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/slack/send_message.py
--rw-r--r--   0        0        0       18 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/sleep/__init__.py
--rw-r--r--   0        0        0      751 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/sleep/tool.py
--rw-r--r--   0        0        0       44 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/spark_sql/__init__.py
--rw-r--r--   0        0        0     1064 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/spark_sql/tool.py
--rw-r--r--   0        0        0       49 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/sql_database/__init__.py
--rw-r--r--   0        0        0      504 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/sql_database/prompt.py
--rw-r--r--   0        0        0     1109 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/sql_database/tool.py
--rw-r--r--   0        0        0       33 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/stackexchange/__init__.py
--rw-r--r--   0        0        0      628 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/stackexchange/tool.py
--rw-r--r--   0        0        0       24 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/steam/__init__.py
--rw-r--r--   0        0        0      634 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/steam/tool.py
--rw-r--r--   0        0        0      694 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/steamship_image_generation/__init__.py
--rw-r--r--   0        0        0      847 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/steamship_image_generation/tool.py
--rw-r--r--   0        0        0      839 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/tavily_search/__init__.py
--rw-r--r--   0        0        0      913 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/tavily_search/tool.py
--rw-r--r--   0        0        0       51 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/vectorstore/__init__.py
--rw-r--r--   0        0        0      791 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/vectorstore/tool.py
--rw-r--r--   0        0        0       29 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/wikipedia/__init__.py
--rw-r--r--   0        0        0      628 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/wikipedia/tool.py
--rw-r--r--   0        0        0      670 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/wolfram_alpha/__init__.py
--rw-r--r--   0        0        0      637 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/wolfram_alpha/tool.py
--rw-r--r--   0        0        0      637 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/yahoo_finance_news.py
--rw-r--r--   0        0        0        0 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/youtube/__init__.py
--rw-r--r--   0        0        0      628 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/youtube/search.py
--rw-r--r--   0        0        0      764 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/zapier/__init__.py
--rw-r--r--   0        0        0      745 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/tools/zapier/tool.py
--rw-r--r--   0        0        0     5891 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/__init__.py
--rw-r--r--   0        0        0      651 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/alpha_vantage.py
--rw-r--r--   0        0        0      839 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/anthropic.py
--rw-r--r--   0        0        0      621 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/apify.py
--rw-r--r--   0        0        0     1336 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/arcee.py
--rw-r--r--   0        0        0      630 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/arxiv.py
--rw-r--r--   0        0        0      274 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/asyncio.py
--rw-r--r--   0        0        0      624 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/awslambda.py
--rw-r--r--   0        0        0      642 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/bibtex.py
--rw-r--r--   0        0        0      645 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/bing_search.py
--rw-r--r--   0        0        0      639 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/brave_search.py
--rw-r--r--   0        0        0     1180 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/clickup.py
--rw-r--r--   0        0        0      680 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/dalle_image_generator.py
--rw-r--r--   0        0        0      695 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/dataforseo_api_search.py
--rw-r--r--   0        0        0      663 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/duckduckgo_search.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/github.py
--rw-r--r--   0        0        0      647 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/gitlab.py
--rw-r--r--   0        0        0      648 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/golden_query.py
--rw-r--r--   0        0        0      654 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/google_finance.py
--rw-r--r--   0        0        0      645 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/google_jobs.py
--rw-r--r--   0        0        0      645 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/google_lens.py
--rw-r--r--   0        0        0      651 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/google_places_api.py
--rw-r--r--   0        0        0      654 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/google_scholar.py
--rw-r--r--   0        0        0      651 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/google_search.py
--rw-r--r--   0        0        0      651 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/google_serper.py
--rw-r--r--   0        0        0      651 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/google_trends.py
--rw-r--r--   0        0        0      636 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/graphql.py
--rw-r--r--   0        0        0      627 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/jira.py
--rw-r--r--   0        0        0      122 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/loading.py
--rw-r--r--   0        0        0      645 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/max_compute.py
--rw-r--r--   0        0        0      657 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/merriam_webster.py
--rw-r--r--   0        0        0      657 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/metaphor_search.py
--rw-r--r--   0        0        0      627 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/nasa.py
--rw-r--r--   0        0        0      739 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/opaqueprompts.py
--rw-r--r--   0        0        0      753 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/openapi.py
--rw-r--r--   0        0        0      657 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/openweathermap.py
--rw-r--r--   0        0        0      636 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/outline.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/portkey.py
--rw-r--r--   0        0        0      627 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/powerbi.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/pubmed.py
--rw-r--r--   0        0        0      462 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/python.py
--rw-r--r--   0        0        0      685 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/reddit_search.py
--rw-r--r--   0        0        0      889 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/redis.py
--rw-r--r--   0        0        0      712 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/requests.py
--rw-r--r--   0        0        0      648 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/scenexplain.py
--rw-r--r--   0        0        0      642 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/searchapi.py
--rw-r--r--   0        0        0      804 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/searx_search.py
--rw-r--r--   0        0        0      782 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/serpapi.py
--rw-r--r--   0        0        0      609 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/spark_sql.py
--rw-r--r--   0        0        0      786 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/sql_database.py
--rw-r--r--   0        0        0      654 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/stackexchange.py
--rw-r--r--   0        0        0      639 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/steam.py
--rw-r--r--   0        0        0      685 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/tavily_search.py
--rw-r--r--   0        0        0      639 2024-05-08 04:43:20.186225 langchain-0.2.0rc1/langchain/utilities/tensorflow_datasets.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utilities/twilio.py
--rw-r--r--   0        0        0     1056 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utilities/vertexai.py
--rw-r--r--   0        0        0      642 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utilities/wikipedia.py
--rw-r--r--   0        0        0      651 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utilities/wolfram_alpha.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utilities/zapier.py
--rw-r--r--   0        0        0     1846 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/__init__.py
--rw-r--r--   0        0        0      102 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/aiter.py
--rw-r--r--   0        0        0      124 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/env.py
--rw-r--r--   0        0        0     1140 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/ernie_functions.py
--rw-r--r--   0        0        0       91 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/formatting.py
--rw-r--r--   0        0        0      421 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/html.py
--rw-r--r--   0        0        0      211 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/input.py
--rw-r--r--   0        0        0      133 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/iter.py
--rw-r--r--   0        0        0      258 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/json_schema.py
--rw-r--r--   0        0        0       92 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/loading.py
--rw-r--r--   0        0        0      918 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/math.py
--rw-r--r--   0        0        0      627 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/openai.py
--rw-r--r--   0        0        0      325 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/openai_functions.py
--rw-r--r--   0        0        0      111 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/pydantic.py
--rw-r--r--   0        0        0      148 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/strings.py
--rw-r--r--   0        0        0      446 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/utils/utils.py
--rw-r--r--   0        0        0     7933 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/__init__.py
--rw-r--r--   0        0        0      833 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/alibabacloud_opensearch.py
--rw-r--r--   0        0        0      621 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/analyticdb.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/annoy.py
--rw-r--r--   0        0        0      612 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/astradb.py
--rw-r--r--   0        0        0      612 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/atlas.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/awadb.py
--rw-r--r--   0        0        0      873 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/azure_cosmos_db.py
--rw-r--r--   0        0        0      867 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/azuresearch.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/bageldb.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/baiducloud_vector_search.py
--rw-r--r--   0        0        0      125 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/base.py
--rw-r--r--   0        0        0      618 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/cassandra.py
--rw-r--r--   0        0        0      609 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/chroma.py
--rw-r--r--   0        0        0      615 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/clarifai.py
--rw-r--r--   0        0        0      736 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/clickhouse.py
--rw-r--r--   0        0        0      621 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/dashvector.py
--rw-r--r--   0        0        0      657 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/databricks_vector_search.py
--rw-r--r--   0        0        0      615 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/deeplake.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/dingo.py
--rw-r--r--   0        0        0      797 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/docarray/__init__.py
--rw-r--r--   0        0        0      658 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/docarray/base.py
--rw-r--r--   0        0        0      645 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/docarray/hnsw.py
--rw-r--r--   0        0        0      657 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/docarray/in_memory.py
--rw-r--r--   0        0        0      757 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/elastic_vector_search.py
--rw-r--r--   0        0        0     1294 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/elasticsearch.py
--rw-r--r--   0        0        0      612 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/epsilla.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/faiss.py
--rw-r--r--   0        0        0      618 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/hippo.py
--rw-r--r--   0        0        0      615 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/hologres.py
--rw-r--r--   0        0        0      612 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/lancedb.py
--rw-r--r--   0        0        0      795 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/llm_rails.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/marqo.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/matching_engine.py
--rw-r--r--   0        0        0      624 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/meilisearch.py
--rw-r--r--   0        0        0      609 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/milvus.py
--rw-r--r--   0        0        0      645 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/momento_vector_index.py
--rw-r--r--   0        0        0      663 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/mongodb_atlas.py
--rw-r--r--   0        0        0      890 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/myscale.py
--rw-r--r--   0        0        0      789 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/neo4j_vector.py
--rw-r--r--   0        0        0      633 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/nucliadb.py
--rw-r--r--   0        0        0      657 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/opensearch_vector_search.py
--rw-r--r--   0        0        0     1042 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/pgembedding.py
--rw-r--r--   0        0        0      643 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/pgvecto_rs.py
--rw-r--r--   0        0        0      790 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/pgvector.py
--rw-r--r--   0        0        0      615 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/pinecone.py
--rw-r--r--   0        0        0      777 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/qdrant.py
--rw-r--r--   0        0        0     1295 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/redis/__init__.py
--rw-r--r--   0        0        0      956 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/redis/base.py
--rw-r--r--   0        0        0     1514 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/redis/filters.py
--rw-r--r--   0        0        0     1745 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/redis/schema.py
--rw-r--r--   0        0        0      612 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/rocksetdb.py
--rw-r--r--   0        0        0      606 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/scann.py
--rw-r--r--   0        0        0      609 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/semadb.py
--rw-r--r--   0        0        0      630 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/singlestoredb.py
--rw-r--r--   0        0        0     1325 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/sklearn.py
--rw-r--r--   0        0        0      618 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/sqlitevss.py
--rw-r--r--   0        0        0      798 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/starrocks.py
--rw-r--r--   0        0        0      648 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/supabase.py
--rw-r--r--   0        0        0      603 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/tair.py
--rw-r--r--   0        0        0      953 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/tencentvectordb.py
--rw-r--r--   0        0        0      609 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/tigris.py
--rw-r--r--   0        0        0      609 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/tiledb.py
--rw-r--r--   0        0        0      636 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/timescalevector.py
--rw-r--r--   0        0        0      618 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/typesense.py
--rw-r--r--   0        0        0      612 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/usearch.py
--rw-r--r--   0        0        0      958 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/utils.py
--rw-r--r--   0        0        0      603 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/vald.py
--rw-r--r--   0        0        0      609 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/vearch.py
--rw-r--r--   0        0        0      785 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/vectara.py
--rw-r--r--   0        0        0      621 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/vespa.py
--rw-r--r--   0        0        0      615 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/weaviate.py
--rw-r--r--   0        0        0      646 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/xata.py
--rw-r--r--   0        0        0      624 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/yellowbrick.py
--rw-r--r--   0        0        0      798 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/zep.py
--rw-r--r--   0        0        0      609 2024-05-08 04:43:20.190225 langchain-0.2.0rc1/langchain/vectorstores/zilliz.py
--rw-r--r--   0        0        0    11798 2024-05-08 04:43:20.194225 langchain-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0    13746 1970-01-01 00:00:00.000000 langchain-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/LICENSE
+-rw-r--r--   0        0        0     5778 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/README.md
+-rw-r--r--   0        0        0    13708 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/_api/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/_api/deprecation.py
+-rw-r--r--   0        0        0      139 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/_api/interactive_env.py
+-rw-r--r--   0        0        0     6746 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/_api/module_import.py
+-rw-r--r--   0        0        0      122 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/_api/path.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/adapters/__init__.py
+-rw-r--r--   0        0        0     1996 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/adapters/openai.py
+-rw-r--r--   0        0        0     6293 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/__init__.py
+-rw-r--r--   0        0        0    56686 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent.py
+-rw-r--r--   0        0        0    15302 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_iterator.py
+-rw-r--r--   0        0        0     7364 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       25 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/ainetwork/__init__.py
+-rw-r--r--   0        0        0      685 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/ainetwork/toolkit.py
+-rw-r--r--   0        0        0      668 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/amadeus/toolkit.py
+-rw-r--r--   0        0        0      771 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/azure_cognitive_services.py
+-rw-r--r--   0        0        0       72 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/base.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/clickup/__init__.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/clickup/toolkit.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0     3235 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
+-rw-r--r--   0        0        0       97 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/conversational_retrieval/tool.py
+-rw-r--r--   0        0        0     1091 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0      782 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/file_management/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/file_management/toolkit.py
+-rw-r--r--   0        0        0       22 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/github/__init__.py
+-rw-r--r--   0        0        0     2244 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/github/toolkit.py
+-rw-r--r--   0        0        0       22 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/gitlab/__init__.py
+-rw-r--r--   0        0        0      670 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/gitlab/toolkit.py
+-rw-r--r--   0        0        0       21 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/gmail/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/gmail/toolkit.py
+-rw-r--r--   0        0        0       20 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/jira/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/jira/toolkit.py
+-rw-r--r--   0        0        0       18 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/json/__init__.py
+-rw-r--r--   0        0        0      672 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/json/base.py
+-rw-r--r--   0        0        0      749 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/json/prompt.py
+-rw-r--r--   0        0        0      654 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/json/toolkit.py
+-rw-r--r--   0        0        0       23 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/multion/__init__.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/multion/toolkit.py
+-rw-r--r--   0        0        0       19 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/nasa/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/nasa/toolkit.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/nla/__init__.py
+-rw-r--r--   0        0        0      634 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/nla/tool.py
+-rw-r--r--   0        0        0      649 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/nla/toolkit.py
+-rw-r--r--   0        0        0       25 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/office365/__init__.py
+-rw-r--r--   0        0        0      670 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/office365/toolkit.py
+-rw-r--r--   0        0        0       26 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/__init__.py
+-rw-r--r--   0        0        0      687 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/base.py
+-rw-r--r--   0        0        0     1599 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/planner.py
+-rw-r--r--   0        0        0     3526 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/planner_prompt.py
+-rw-r--r--   0        0        0      909 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/prompt.py
+-rw-r--r--   0        0        0      833 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/spec.py
+-rw-r--r--   0        0        0      818 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/toolkit.py
+-rw-r--r--   0        0        0     1104 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/pandas/__init__.py
+-rw-r--r--   0        0        0      762 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/playwright/__init__.py
+-rw-r--r--   0        0        0      728 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/playwright/toolkit.py
+-rw-r--r--   0        0        0       22 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/powerbi/__init__.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/powerbi/base.py
+-rw-r--r--   0        0        0      717 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/powerbi/chat_base.py
+-rw-r--r--   0        0        0     1084 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/powerbi/prompt.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/powerbi/toolkit.py
+-rw-r--r--   0        0        0     1094 2024-05-09 20:46:47.218468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/python/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/slack/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/slack/toolkit.py
+-rw-r--r--   0        0        0     1103 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/spark/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/spark_sql/__init__.py
+-rw-r--r--   0        0        0      697 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/spark_sql/base.py
+-rw-r--r--   0        0        0      783 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/spark_sql/prompt.py
+-rw-r--r--   0        0        0      682 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/spark_sql/toolkit.py
+-rw-r--r--   0        0        0       17 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/sql/__init__.py
+-rw-r--r--   0        0        0      661 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/sql/base.py
+-rw-r--r--   0        0        0      896 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/sql/prompt.py
+-rw-r--r--   0        0        0      679 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/sql/toolkit.py
+-rw-r--r--   0        0        0       21 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/steam/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/steam/toolkit.py
+-rw-r--r--   0        0        0       56 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/vectorstore/__init__.py
+-rw-r--r--   0        0        0     4216 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/vectorstore/base.py
+-rw-r--r--   0        0        0      834 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/vectorstore/prompt.py
+-rw-r--r--   0        0        0     3289 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/vectorstore/toolkit.py
+-rw-r--r--   0        0        0     1095 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/zapier/__init__.py
+-rw-r--r--   0        0        0      670 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_toolkits/zapier/toolkit.py
+-rw-r--r--   0        0        0     1948 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/agent_types.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/chat/__init__.py
+-rw-r--r--   0        0        0     5110 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/chat/base.py
+-rw-r--r--   0        0        0     1977 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/chat/output_parser.py
+-rw-r--r--   0        0        0     1158 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/chat/prompt.py
+-rw-r--r--   0        0        0       75 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/conversational/__init__.py
+-rw-r--r--   0        0        0     4979 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/conversational/base.py
+-rw-r--r--   0        0        0     1383 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/conversational/output_parser.py
+-rw-r--r--   0        0        0     1859 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/conversational/prompt.py
+-rw-r--r--   0        0        0       75 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/conversational_chat/__init__.py
+-rw-r--r--   0        0        0     5244 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/conversational_chat/base.py
+-rw-r--r--   0        0        0     2394 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/conversational_chat/output_parser.py
+-rw-r--r--   0        0        0     2763 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/conversational_chat/prompt.py
+-rw-r--r--   0        0        0      955 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/format_scratchpad/__init__.py
+-rw-r--r--   0        0        0      528 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/format_scratchpad/log.py
+-rw-r--r--   0        0        0      721 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/format_scratchpad/log_to_messages.py
+-rw-r--r--   0        0        0     2203 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/format_scratchpad/openai_functions.py
+-rw-r--r--   0        0        0      166 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/format_scratchpad/openai_tools.py
+-rw-r--r--   0        0        0     1853 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/format_scratchpad/tools.py
+-rw-r--r--   0        0        0      578 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/format_scratchpad/xml.py
+-rw-r--r--   0        0        0     3244 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/initialize.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/json_chat/__init__.py
+-rw-r--r--   0        0        0     7743 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/json_chat/base.py
+-rw-r--r--   0        0        0      551 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/json_chat/prompt.py
+-rw-r--r--   0        0        0      286 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/load_tools.py
+-rw-r--r--   0        0        0     4634 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/loading.py
+-rw-r--r--   0        0        0       86 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/mrkl/__init__.py
+-rw-r--r--   0        0        0     6064 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/mrkl/base.py
+-rw-r--r--   0        0        0     3407 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/mrkl/output_parser.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/mrkl/prompt.py
+-rw-r--r--   0        0        0      114 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/openai_assistant/__init__.py
+-rw-r--r--   0        0        0    27657 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/openai_assistant/base.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/openai_functions_agent/__init__.py
+-rw-r--r--   0        0        0     2761 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py
+-rw-r--r--   0        0        0    11633 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/openai_functions_agent/base.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/openai_functions_multi_agent/__init__.py
+-rw-r--r--   0        0        0    12006 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/openai_functions_multi_agent/base.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/openai_tools/__init__.py
+-rw-r--r--   0        0        0     3435 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/openai_tools/base.py
+-rw-r--r--   0        0        0     1373 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1846 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/output_parsers/json.py
+-rw-r--r--   0        0        0     3467 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/output_parsers/openai_functions.py
+-rw-r--r--   0        0        0     2317 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/output_parsers/openai_tools.py
+-rw-r--r--   0        0        0     2455 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/output_parsers/react_json_single_input.py
+-rw-r--r--   0        0        0     3218 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/output_parsers/react_single_input.py
+-rw-r--r--   0        0        0     1545 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/output_parsers/self_ask.py
+-rw-r--r--   0        0        0     3753 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/output_parsers/tools.py
+-rw-r--r--   0        0        0     1658 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/output_parsers/xml.py
+-rw-r--r--   0        0        0       76 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/react/__init__.py
+-rw-r--r--   0        0        0     4975 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/react/agent.py
+-rw-r--r--   0        0        0     5798 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/react/base.py
+-rw-r--r--   0        0        0     1231 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/react/output_parser.py
+-rw-r--r--   0        0        0     1906 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/react/textworld_prompt.py
+-rw-r--r--   0        0        0     6127 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/react/wiki_prompt.py
+-rw-r--r--   0        0        0     1175 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/schema.py
+-rw-r--r--   0        0        0      106 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/self_ask_with_search/__init__.py
+-rw-r--r--   0        0        0     8228 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/self_ask_with_search/base.py
+-rw-r--r--   0        0        0      138 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/self_ask_with_search/output_parser.py
+-rw-r--r--   0        0        0     1926 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/self_ask_with_search/prompt.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/structured_chat/__init__.py
+-rw-r--r--   0        0        0    10812 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/structured_chat/base.py
+-rw-r--r--   0        0        0     3799 2024-05-09 20:46:47.222468 langchain-0.2.0rc2/langchain/agents/structured_chat/output_parser.py
+-rw-r--r--   0        0        0      992 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/agents/structured_chat/prompt.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/agents/tool_calling_agent/__init__.py
+-rw-r--r--   0        0        0     3465 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/agents/tool_calling_agent/base.py
+-rw-r--r--   0        0        0     1409 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/agents/tools.py
+-rw-r--r--   0        0        0     1475 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/agents/types.py
+-rw-r--r--   0        0        0      384 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/agents/utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/agents/xml/__init__.py
+-rw-r--r--   0        0        0     8103 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/agents/xml/base.py
+-rw-r--r--   0        0        0      767 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/agents/xml/prompt.py
+-rw-r--r--   0        0        0      217 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/base_language.py
+-rw-r--r--   0        0        0     2155 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/cache.py
+-rw-r--r--   0        0        0     5960 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      941 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/aim_callback.py
+-rw-r--r--   0        0        0      688 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/argilla_callback.py
+-rw-r--r--   0        0        0      678 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/arize_callback.py
+-rw-r--r--   0        0        0      683 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/arthur_callback.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/base.py
+-rw-r--r--   0        0        0      688 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/clearml_callback.py
+-rw-r--r--   0        0        0      684 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/comet_ml_callback.py
+-rw-r--r--   0        0        0      695 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/confident_callback.py
+-rw-r--r--   0        0        0      688 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/context_callback.py
+-rw-r--r--   0        0        0       97 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/file.py
+-rw-r--r--   0        0        0      678 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/flyte_callback.py
+-rw-r--r--   0        0        0      997 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/human.py
+-rw-r--r--   0        0        0      683 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/infino_callback.py
+-rw-r--r--   0        0        0     1006 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/labelstudio_callback.py
+-rw-r--r--   0        0        0      715 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/llmonitor_callback.py
+-rw-r--r--   0        0        0     2410 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/manager.py
+-rw-r--r--   0        0        0     1137 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/mlflow_callback.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/openai_info.py
+-rw-r--r--   0        0        0      725 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/promptlayer_callback.py
+-rw-r--r--   0        0        0      715 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/sagemaker_callback.py
+-rw-r--r--   0        0        0      103 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/stdout.py
+-rw-r--r--   0        0        0     2399 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/streaming_aiter.py
+-rw-r--r--   0        0        0     3371 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/streaming_aiter_final_only.py
+-rw-r--r--   0        0        0      173 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0     3357 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/streaming_stdout_final_only.py
+-rw-r--r--   0        0        0     3407 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/streamlit/__init__.py
+-rw-r--r--   0        0        0      937 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/streamlit/mutable_expander.py
+-rw-r--r--   0        0        0     1372 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/streamlit/streamlit_callback_handler.py
+-rw-r--r--   0        0        0     1140 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0      154 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/base.py
+-rw-r--r--   0        0        0      800 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/comet.py
+-rw-r--r--   0        0        0      233 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/evaluation.py
+-rw-r--r--   0        0        0      218 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/langchain.py
+-rw-r--r--   0        0        0       99 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/langchain_v1.py
+-rw-r--r--   0        0        0      226 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/log_stream.py
+-rw-r--r--   0        0        0     1384 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/logging.py
+-rw-r--r--   0        0        0      105 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/root_listeners.py
+-rw-r--r--   0        0        0      120 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/run_collector.py
+-rw-r--r--   0        0        0      470 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/schemas.py
+-rw-r--r--   0        0        0      168 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/stdout.py
+-rw-r--r--   0        0        0      885 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/tracers/wandb.py
+-rw-r--r--   0        0        0      693 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/trubrics_callback.py
+-rw-r--r--   0        0        0     1409 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/utils.py
+-rw-r--r--   0        0        0      678 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0      688 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/callbacks/whylabs_callback.py
+-rw-r--r--   0        0        0     4885 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/__init__.py
+-rw-r--r--   0        0        0       84 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/__init__.py
+-rw-r--r--   0        0        0    10003 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/base.py
+-rw-r--r--   0        0        0     2452 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/news_docs.py
+-rw-r--r--   0        0        0     3399 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/open_meteo_docs.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/openapi/__init__.py
+-rw-r--r--   0        0        0      667 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/openapi/chain.py
+-rw-r--r--   0        0        0      795 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/openapi/prompts.py
+-rw-r--r--   0        0        0      963 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/openapi/requests_chain.py
+-rw-r--r--   0        0        0      966 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/openapi/response_chain.py
+-rw-r--r--   0        0        0     1920 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/podcast_docs.py
+-rw-r--r--   0        0        0     1031 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/prompt.py
+-rw-r--r--   0        0        0     1537 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/api/tmdb_docs.py
+-rw-r--r--   0        0        0    30670 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/base.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/chat_vector_db/__init__.py
+-rw-r--r--   0        0        0      694 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/chat_vector_db/prompts.py
+-rw-r--r--   0        0        0      367 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/combine_documents/__init__.py
+-rw-r--r--   0        0        0     8006 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/combine_documents/base.py
+-rw-r--r--   0        0        0    11781 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/combine_documents/map_reduce.py
+-rw-r--r--   0        0        0     8991 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/combine_documents/map_rerank.py
+-rw-r--r--   0        0        0    13894 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/combine_documents/reduce.py
+-rw-r--r--   0        0        0     9113 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/combine_documents/refine.py
+-rw-r--r--   0        0        0    10958 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/combine_documents/stuff.py
+-rw-r--r--   0        0        0      107 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/constitutional_ai/__init__.py
+-rw-r--r--   0        0        0     6341 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/constitutional_ai/base.py
+-rw-r--r--   0        0        0      283 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/constitutional_ai/models.py
+-rw-r--r--   0        0        0    21738 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/constitutional_ai/principles.py
+-rw-r--r--   0        0        0     8666 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/constitutional_ai/prompts.py
+-rw-r--r--   0        0        0       71 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/conversation/__init__.py
+-rw-r--r--   0        0        0     2366 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/conversation/base.py
+-rw-r--r--   0        0        0     1396 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/conversation/memory.py
+-rw-r--r--   0        0        0      913 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/conversation/prompt.py
+-rw-r--r--   0        0        0       49 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0    20995 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/conversational_retrieval/base.py
+-rw-r--r--   0        0        0      720 2024-05-09 20:46:47.226468 langchain-0.2.0rc2/langchain/chains/conversational_retrieval/prompts.py
+-rw-r--r--   0        0        0      126 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/elasticsearch_database/__init__.py
+-rw-r--r--   0        0        0     8287 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/elasticsearch_database/base.py
+-rw-r--r--   0        0        0     1425 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/elasticsearch_database/prompts.py
+-rw-r--r--   0        0        0     1514 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/ernie_functions/__init__.py
+-rw-r--r--   0        0        0     1730 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/ernie_functions/base.py
+-rw-r--r--   0        0        0      741 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/example_generator.py
+-rw-r--r--   0        0        0       51 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/flare/__init__.py
+-rw-r--r--   0        0        0     9081 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/flare/base.py
+-rw-r--r--   0        0        0     1471 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/flare/prompts.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/arangodb.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/base.py
+-rw-r--r--   0        0        0     1205 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/cypher.py
+-rw-r--r--   0        0        0      792 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/cypher_utils.py
+-rw-r--r--   0        0        0      925 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/falkordb.py
+-rw-r--r--   0        0        0     1090 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/gremlin.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/hugegraph.py
+-rw-r--r--   0        0        0      870 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/kuzu.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/nebulagraph.py
+-rw-r--r--   0        0        0     1232 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/neptune_cypher.py
+-rw-r--r--   0        0        0     1137 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/neptune_sparql.py
+-rw-r--r--   0        0        0      714 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/ontotext_graphdb.py
+-rw-r--r--   0        0        0     3934 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/prompts.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/graph_qa/sparql.py
+-rw-r--r--   0        0        0     2662 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/history_aware_retriever.py
+-rw-r--r--   0        0        0       75 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/hyde/__init__.py
+-rw-r--r--   0        0        0     3341 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/hyde/base.py
+-rw-r--r--   0        0        0     1913 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/hyde/prompts.py
+-rw-r--r--   0        0        0    15470 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm.py
+-rw-r--r--   0        0        0      453 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_bash/__init__.py
+-rw-r--r--   0        0        0      139 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_checker/__init__.py
+-rw-r--r--   0        0        0     6190 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_checker/base.py
+-rw-r--r--   0        0        0     1125 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_checker/prompt.py
+-rw-r--r--   0        0        0      143 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_math/__init__.py
+-rw-r--r--   0        0        0     6709 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_math/base.py
+-rw-r--r--   0        0        0      868 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_math/prompt.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_requests.py
+-rw-r--r--   0        0        0      352 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_summarization_checker/__init__.py
+-rw-r--r--   0        0        0     6582 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_summarization_checker/base.py
+-rw-r--r--   0        0        0      654 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
+-rw-r--r--   0        0        0      377 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_summarization_checker/prompts/check_facts.txt
+-rw-r--r--   0        0        0      128 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_summarization_checker/prompts/create_facts.txt
+-rw-r--r--   0        0        0      416 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt
+-rw-r--r--   0        0        0      470 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/llm_symbolic_math/__init__.py
+-rw-r--r--   0        0        0    28297 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/loading.py
+-rw-r--r--   0        0        0     3733 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/mapreduce.py
+-rw-r--r--   0        0        0     3086 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/moderation.py
+-rw-r--r--   0        0        0       96 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/natbot/__init__.py
+-rw-r--r--   0        0        0     4778 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/natbot/base.py
+-rw-r--r--   0        0        0    16050 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/natbot/crawler.py
+-rw-r--r--   0        0        0     4989 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/natbot/prompt.py
+-rw-r--r--   0        0        0     1403 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/openai_functions/__init__.py
+-rw-r--r--   0        0        0    10172 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/openai_functions/base.py
+-rw-r--r--   0        0        0     3558 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/openai_functions/citation_fuzzy_match.py
+-rw-r--r--   0        0        0     7301 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/openai_functions/extraction.py
+-rw-r--r--   0        0        0    11911 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/openai_functions/openapi.py
+-rw-r--r--   0        0        0     3959 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/openai_functions/qa_with_structure.py
+-rw-r--r--   0        0        0     2663 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/openai_functions/tagging.py
+-rw-r--r--   0        0        0     1255 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/openai_functions/utils.py
+-rw-r--r--   0        0        0      134 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/openai_tools/__init__.py
+-rw-r--r--   0        0        0     3428 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/openai_tools/extraction.py
+-rw-r--r--   0        0        0     2015 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/prompt_selector.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_generation/__init__.py
+-rw-r--r--   0        0        0     2465 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_generation/base.py
+-rw-r--r--   0        0        0     1875 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_generation/prompt.py
+-rw-r--r--   0        0        0      173 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_with_sources/__init__.py
+-rw-r--r--   0        0        0     7998 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_with_sources/base.py
+-rw-r--r--   0        0        0     7079 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_with_sources/loading.py
+-rw-r--r--   0        0        0     6971 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_with_sources/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1318 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_with_sources/refine_prompts.py
+-rw-r--r--   0        0        0     2451 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_with_sources/retrieval.py
+-rw-r--r--   0        0        0     6581 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_with_sources/stuff_prompt.py
+-rw-r--r--   0        0        0     2770 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/qa_with_sources/vector_db.py
+-rw-r--r--   0        0        0      131 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/query_constructor/__init__.py
+-rw-r--r--   0        0        0    13680 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/query_constructor/base.py
+-rw-r--r--   0        0        0      393 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/query_constructor/ir.py
+-rw-r--r--   0        0        0     5694 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/query_constructor/parser.py
+-rw-r--r--   0        0        0     6880 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/query_constructor/prompt.py
+-rw-r--r--   0        0        0      321 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/query_constructor/schema.py
+-rw-r--r--   0        0        0      144 2024-05-09 20:46:47.230468 langchain-0.2.0rc2/langchain/chains/question_answering/__init__.py
+-rw-r--r--   0        0        0     8811 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/question_answering/chain.py
+-rw-r--r--   0        0        0     8013 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/question_answering/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1622 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/question_answering/map_rerank_prompt.py
+-rw-r--r--   0        0        0     2378 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/question_answering/refine_prompts.py
+-rw-r--r--   0        0        0     1146 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/question_answering/stuff_prompt.py
+-rw-r--r--   0        0        0     2742 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/retrieval.py
+-rw-r--r--   0        0        0       62 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/retrieval_qa/__init__.py
+-rw-r--r--   0        0        0    11243 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/retrieval_qa/base.py
+-rw-r--r--   0        0        0      399 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/retrieval_qa/prompt.py
+-rw-r--r--   0        0        0      407 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/router/__init__.py
+-rw-r--r--   0        0        0     4571 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/router/base.py
+-rw-r--r--   0        0        0     3124 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/router/embedding_router.py
+-rw-r--r--   0        0        0     4345 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/router/llm_router.py
+-rw-r--r--   0        0        0     2245 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/router/multi_prompt.py
+-rw-r--r--   0        0        0     1156 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/router/multi_prompt_prompt.py
+-rw-r--r--   0        0        0     1079 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/router/multi_retrieval_prompt.py
+-rw-r--r--   0        0        0     4227 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/router/multi_retrieval_qa.py
+-rw-r--r--   0        0        0     7510 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/sequential.py
+-rw-r--r--   0        0        0       47 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/sql_database/__init__.py
+-rw-r--r--   0        0        0    15458 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/sql_database/prompt.py
+-rw-r--r--   0        0        0     5367 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/sql_database/query.py
+-rw-r--r--   0        0        0      204 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/structured_output/__init__.py
+-rw-r--r--   0        0        0    25514 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/structured_output/base.py
+-rw-r--r--   0        0        0      151 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/summarize/__init__.py
+-rw-r--r--   0        0        0     6192 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/summarize/chain.py
+-rw-r--r--   0        0        0      238 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/summarize/map_reduce_prompt.py
+-rw-r--r--   0        0        0      677 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/summarize/refine_prompts.py
+-rw-r--r--   0        0        0      238 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/summarize/stuff_prompt.py
+-rw-r--r--   0        0        0     2369 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chains/transform.py
+-rw-r--r--   0        0        0      452 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_loaders/__init__.py
+-rw-r--r--   0        0        0       85 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_loaders/base.py
+-rw-r--r--   0        0        0      884 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_loaders/facebook_messenger.py
+-rw-r--r--   0        0        0      636 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_loaders/gmail.py
+-rw-r--r--   0        0        0      663 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_loaders/imessage.py
+-rw-r--r--   0        0        0      851 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_loaders/langsmith.py
+-rw-r--r--   0        0        0      648 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_loaders/slack.py
+-rw-r--r--   0        0        0      663 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_loaders/telegram.py
+-rw-r--r--   0        0        0     1077 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_loaders/utils.py
+-rw-r--r--   0        0        0      663 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_loaders/whatsapp.py
+-rw-r--r--   0        0        0     1978 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/__init__.py
+-rw-r--r--   0        0        0      851 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/anthropic.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/anyscale.py
+-rw-r--r--   0        0        0      660 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/azure_openai.py
+-rw-r--r--   0        0        0      863 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/azureml_endpoint.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/baichuan.py
+-rw-r--r--   0        0        0      715 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0      268 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/base.py
+-rw-r--r--   0        0        0      757 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/bedrock.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/cohere.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/databricks.py
+-rw-r--r--   0        0        0      637 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/ernie.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/everlyai.py
+-rw-r--r--   0        0        0      815 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/fake.py
+-rw-r--r--   0        0        0      648 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/fireworks.py
+-rw-r--r--   0        0        0      631 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/gigachat.py
+-rw-r--r--   0        0        0      809 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/google_palm.py
+-rw-r--r--   0        0        0      658 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/human.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/hunyuan.py
+-rw-r--r--   0        0        0      821 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/javelin_ai_gateway.py
+-rw-r--r--   0        0        0      631 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/jinachat.py
+-rw-r--r--   0        0        0      628 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/konko.py
+-rw-r--r--   0        0        0      791 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/litellm.py
+-rw-r--r--   0        0        0      701 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/meta.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/minimax.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/mlflow.py
+-rw-r--r--   0        0        0      815 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/ollama.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/openai.py
+-rw-r--r--   0        0        0      683 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/pai_eas_endpoint.py
+-rw-r--r--   0        0        0      696 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/promptlayer_openai.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/tongyi.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/vertexai.py
+-rw-r--r--   0        0        0      845 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/volcengine_maas.py
+-rw-r--r--   0        0        0      642 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/chat_models/yandex.py
+-rw-r--r--   0        0        0     1245 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/docstore/__init__.py
+-rw-r--r--   0        0        0      639 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/docstore/arbitrary_fn.py
+-rw-r--r--   0        0        0      715 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/docstore/base.py
+-rw-r--r--   0        0        0       70 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/docstore/document.py
+-rw-r--r--   0        0        0      651 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/docstore/in_memory.py
+-rw-r--r--   0        0        0      630 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/docstore/wikipedia.py
+-rw-r--r--   0        0        0    20699 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/acreom.py
+-rw-r--r--   0        0        0     1574 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/airbyte.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/airbyte_json.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/airtable.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/apify_dataset.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/arcgis_loader.py
+-rw-r--r--   0        0        0      632 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/arxiv.py
+-rw-r--r--   0        0        0      879 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/assemblyai.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/async_html.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/azlyrics.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/azure_ai_data.py
+-rw-r--r--   0        0        0      698 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/azure_blob_storage_container.py
+-rw-r--r--   0        0        0      683 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/azure_blob_storage_file.py
+-rw-r--r--   0        0        0      758 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/baiducloud_bos_directory.py
+-rw-r--r--   0        0        0      716 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/baiducloud_bos_file.py
+-rw-r--r--   0        0        0      115 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/base.py
+-rw-r--r--   0        0        0      661 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/base_o365.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/bibtex.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/bigquery.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/bilibili.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/blackboard.py
+-rw-r--r--   0        0        0     1005 2024-05-09 20:46:47.234468 langchain-0.2.0rc2/langchain/document_loaders/blob_loaders/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/blob_loaders/file_system.py
+-rw-r--r--   0        0        0      707 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/blob_loaders/schema.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/blob_loaders/youtube_audio.py
+-rw-r--r--   0        0        0      852 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/blockchain.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/brave_search.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/browserless.py
+-rw-r--r--   0        0        0      819 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/chatgpt.py
+-rw-r--r--   0        0        0      656 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/chromium.py
+-rw-r--r--   0        0        0      680 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/college_confidential.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/concurrent.py
+-rw-r--r--   0        0        0      825 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/confluence.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/conllu.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/couchbase.py
+-rw-r--r--   0        0        0      754 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/csv_loader.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/cube_semantic.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/datadog_logs.py
+-rw-r--r--   0        0        0      838 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/dataframe.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/diffbot.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/directory.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/discord.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/docusaurus.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/dropbox.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/duckdb_loader.py
+-rw-r--r--   0        0        0      818 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/email.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/epub.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/etherscan.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/evernote.py
+-rw-r--r--   0        0        0      668 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/excel.py
+-rw-r--r--   0        0        0      846 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/facebook_chat.py
+-rw-r--r--   0        0        0      632 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/fauna.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/figma.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/gcs_directory.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/gcs_file.py
+-rw-r--r--   0        0        0      654 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/generic.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/geodataframe.py
+-rw-r--r--   0        0        0      626 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/git.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/gitbook.py
+-rw-r--r--   0        0        0      832 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/github.py
+-rw-r--r--   0        0        0      671 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/google_speech_to_text.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/googledrive.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/gutenberg.py
+-rw-r--r--   0        0        0      812 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/helpers.py
+-rw-r--r--   0        0        0      623 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/hn.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/html.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/html_bs.py
+-rw-r--r--   0        0        0      671 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/hugging_face_dataset.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/ifixit.py
+-rw-r--r--   0        0        0      668 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/image.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/image_captions.py
+-rw-r--r--   0        0        0      632 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/imsdb.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/iugu.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/joplin.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/json_loader.py
+-rw-r--r--   0        0        0      964 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/lakefs.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/larksuite.py
+-rw-r--r--   0        0        0      683 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/markdown.py
+-rw-r--r--   0        0        0      656 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/mastodon.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/max_compute.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/mediawikidump.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/merge.py
+-rw-r--r--   0        0        0      632 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/mhtml.py
+-rw-r--r--   0        0        0      659 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/modern_treasury.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/mongodb.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/news.py
+-rw-r--r--   0        0        0      964 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/notebook.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/notion.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/notiondb.py
+-rw-r--r--   0        0        0      649 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/nuclia.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/obs_directory.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/obs_file.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/obsidian.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/odt.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/onedrive.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/onedrive_file.py
+-rw-r--r--   0        0        0      654 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/onenote.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/open_city_data.py
+-rw-r--r--   0        0        0      680 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/org_mode.py
+-rw-r--r--   0        0        0     2142 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/audio.py
+-rw-r--r--   0        0        0      821 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/docai.py
+-rw-r--r--   0        0        0      694 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/generic.py
+-rw-r--r--   0        0        0      848 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/grobid.py
+-rw-r--r--   0        0        0      678 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/html/__init__.py
+-rw-r--r--   0        0        0      678 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/html/bs4.py
+-rw-r--r--   0        0        0      747 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/language/__init__.py
+-rw-r--r--   0        0        0      710 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/language/cobol.py
+-rw-r--r--   0        0        0      742 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/language/code_segmenter.py
+-rw-r--r--   0        0        0      752 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/language/javascript.py
+-rw-r--r--   0        0        0      747 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/language/language_parser.py
+-rw-r--r--   0        0        0      715 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/language/python.py
+-rw-r--r--   0        0        0      671 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/msword.py
+-rw-r--r--   0        0        0     1662 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/pdf.py
+-rw-r--r--   0        0        0      669 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/registry.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/parsers/txt.py
+-rw-r--r--   0        0        0     2181 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/pdf.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/polars_dataframe.py
+-rw-r--r--   0        0        0      689 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/powerpoint.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/psychic.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/pubmed.py
+-rw-r--r--   0        0        0      718 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/pyspark_dataframe.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/python.py
+-rw-r--r--   0        0        0      639 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/quip.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/readthedocs.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/recursive_url_loader.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/reddit.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/roam.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/rocksetdb.py
+-rw-r--r--   0        0        0      649 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/rspace.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/rss.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/rst.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/rtf.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/s3_directory.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/s3_file.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/sharepoint.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/sitemap.py
+-rw-r--r--   0        0        0      659 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/slack_directory.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/snowflake_loader.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/spreedly.py
+-rw-r--r--   0        0        0      626 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/srt.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.238468 langchain-0.2.0rc2/langchain/document_loaders/stripe.py
+-rw-r--r--   0        0        0     1122 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/telegram.py
+-rw-r--r--   0        0        0      680 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/tencent_cos_directory.py
+-rw-r--r--   0        0        0      659 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/tencent_cos_file.py
+-rw-r--r--   0        0        0      668 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/tensorflow_datasets.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/text.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/tomarkdown.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/toml.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/trello.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/tsv.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/twitter.py
+-rw-r--r--   0        0        0     1855 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/unstructured.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/url.py
+-rw-r--r--   0        0        0     1033 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/url_playwright.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/url_selenium.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/weather.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/web_base.py
+-rw-r--r--   0        0        0      846 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/whatsapp_chat.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/wikipedia.py
+-rw-r--r--   0        0        0      821 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/word_document.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/xml.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/xorbits.py
+-rw-r--r--   0        0        0      905 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_loaders/youtube.py
+-rw-r--r--   0        0        0     2573 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/__init__.py
+-rw-r--r--   0        0        0      687 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/beautiful_soup_transformer.py
+-rw-r--r--   0        0        0      687 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/doctran_text_extract.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/doctran_text_qa.py
+-rw-r--r--   0        0        0      678 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/doctran_text_translate.py
+-rw-r--r--   0        0        0     1667 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/embeddings_redundant_filter.py
+-rw-r--r--   0        0        0      693 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/google_translate.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/html2text.py
+-rw-r--r--   0        0        0      663 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/long_context_reorder.py
+-rw-r--r--   0        0        0      678 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/nuclia_text_transform.py
+-rw-r--r--   0        0        0      929 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/openai_functions.py
+-rw-r--r--   0        0        0     6033 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/document_transformers/xsl/html_chunks_with_headers.xslt
+-rw-r--r--   0        0        0     8314 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/aleph_alpha.py
+-rw-r--r--   0        0        0      626 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/awa.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/azure_openai.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0      113 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/base.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/bedrock.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/bookend.py
+-rw-r--r--   0        0        0     8862 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/cache.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/clarifai.py
+-rw-r--r--   0        0        0      756 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/cloudflare_workersai.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/cohere.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/dashscope.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/databricks.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/deepinfra.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/edenai.py
+-rw-r--r--   0        0        0      656 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/elasticsearch.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/embaas.py
+-rw-r--r--   0        0        0      632 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/ernie.py
+-rw-r--r--   0        0        0      791 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/fake.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/fastembed.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/google_palm.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/gpt4all.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/gradient_ai.py
+-rw-r--r--   0        0        0     1112 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/huggingface.py
+-rw-r--r--   0        0        0      659 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/huggingface_hub.py
+-rw-r--r--   0        0        0      895 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/infinity.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/javelin_ai_gateway.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/jina.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/johnsnowlabs.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/llamacpp.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/llm_rails.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/localai.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/minimax.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/mlflow.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/mlflow_gateway.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/modelscope_hub.py
+-rw-r--r--   0        0        0      671 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/mosaicml.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/nlpcloud.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/octoai_embeddings.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/ollama.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/openai.py
+-rw-r--r--   0        0        0      900 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/sagemaker_endpoint.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/self_hosted.py
+-rw-r--r--   0        0        0      881 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      667 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0      632 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/spacy_embeddings.py
+-rw-r--r--   0        0        0      656 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/tensorflow_hub.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/vertexai.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/voyageai.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/embeddings/xinference.py
+-rw-r--r--   0        0        0      476 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/env.py
+-rw-r--r--   0        0        0     5803 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/__init__.py
+-rw-r--r--   0        0        0      165 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/agents/__init__.py
+-rw-r--r--   0        0        0    13915 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/agents/trajectory_eval_chain.py
+-rw-r--r--   0        0        0     5938 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/agents/trajectory_eval_prompt.py
+-rw-r--r--   0        0        0     1400 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/comparison/__init__.py
+-rw-r--r--   0        0        0    15934 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/comparison/eval_chain.py
+-rw-r--r--   0        0        0     2358 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/comparison/prompt.py
+-rw-r--r--   0        0        0     1647 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/criteria/__init__.py
+-rw-r--r--   0        0        0    21304 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/criteria/eval_chain.py
+-rw-r--r--   0        0        0     1756 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/criteria/prompt.py
+-rw-r--r--   0        0        0      323 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/embedding_distance/__init__.py
+-rw-r--r--   0        0        0    17095 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/embedding_distance/base.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/exact_match/__init__.py
+-rw-r--r--   0        0        0     2751 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/exact_match/base.py
+-rw-r--r--   0        0        0     7327 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/loading.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/parsing/__init__.py
+-rw-r--r--   0        0        0     5241 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/parsing/base.py
+-rw-r--r--   0        0        0     3662 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/parsing/json_distance.py
+-rw-r--r--   0        0        0     3180 2024-05-09 20:46:47.242467 langchain-0.2.0rc2/langchain/evaluation/parsing/json_schema.py
+-rw-r--r--   0        0        0      344 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/qa/__init__.py
+-rw-r--r--   0        0        0    10891 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/qa/eval_chain.py
+-rw-r--r--   0        0        0     3911 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/qa/eval_prompt.py
+-rw-r--r--   0        0        0     1052 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/qa/generate_chain.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/qa/generate_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/regex_match/__init__.py
+-rw-r--r--   0        0        0     2407 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/regex_match/base.py
+-rw-r--r--   0        0        0    18197 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/schema.py
+-rw-r--r--   0        0        0     1112 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/scoring/__init__.py
+-rw-r--r--   0        0        0    15476 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/scoring/eval_chain.py
+-rw-r--r--   0        0        0     2129 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/scoring/prompt.py
+-rw-r--r--   0        0        0      285 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/string_distance/__init__.py
+-rw-r--r--   0        0        0    14019 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/evaluation/string_distance/base.py
+-rw-r--r--   0        0        0      141 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/example_generator.py
+-rw-r--r--   0        0        0      167 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/formatting.py
+-rw-r--r--   0        0        0     7435 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/globals/__init__.py
+-rw-r--r--   0        0        0     1527 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/__init__.py
+-rw-r--r--   0        0        0      796 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/arangodb_graph.py
+-rw-r--r--   0        0        0      618 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/falkordb_graph.py
+-rw-r--r--   0        0        0      862 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/graph_document.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/graph_store.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/hugegraph.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/kuzu_graph.py
+-rw-r--r--   0        0        0      618 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/memgraph_graph.py
+-rw-r--r--   0        0        0      612 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/nebula_graph.py
+-rw-r--r--   0        0        0      609 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/neo4j_graph.py
+-rw-r--r--   0        0        0      615 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/neptune_graph.py
+-rw-r--r--   0        0        0     1042 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/networkx_graph.py
+-rw-r--r--   0        0        0      603 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/graphs/rdf_graph.py
+-rw-r--r--   0        0        0     3462 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/hub.py
+-rw-r--r--   0        0        0     1480 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/indexes/__init__.py
+-rw-r--r--   0        0        0      252 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/indexes/_api.py
+-rw-r--r--   0        0        0    20640 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/indexes/_sql_record_manager.py
+-rw-r--r--   0        0        0      906 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/indexes/graph.py
+-rw-r--r--   0        0        0      357 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/indexes/prompts/__init__.py
+-rw-r--r--   0        0        0     1952 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/indexes/prompts/entity_extraction.py
+-rw-r--r--   0        0        0     1157 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/indexes/prompts/entity_summarization.py
+-rw-r--r--   0        0        0     1554 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/indexes/prompts/knowledge_triplet_extraction.py
+-rw-r--r--   0        0        0     7067 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/indexes/vectorstore.py
+-rw-r--r--   0        0        0      282 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/input.py
+-rw-r--r--   0        0        0    17100 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/ai21.py
+-rw-r--r--   0        0        0      605 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/aleph_alpha.py
+-rw-r--r--   0        0        0      623 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/amazon_api_gateway.py
+-rw-r--r--   0        0        0      602 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/anthropic.py
+-rw-r--r--   0        0        0      599 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/anyscale.py
+-rw-r--r--   0        0        0      590 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/arcee.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/aviary.py
+-rw-r--r--   0        0        0     1649 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/azureml_endpoint.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/bananadev.py
+-rw-r--r--   0        0        0      228 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/base.py
+-rw-r--r--   0        0        0      596 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/baseten.py
+-rw-r--r--   0        0        0      587 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/beam.py
+-rw-r--r--   0        0        0      738 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/bedrock.py
+-rw-r--r--   0        0        0      617 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/bittensor.py
+-rw-r--r--   0        0        0      608 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/cerebriumai.py
+-rw-r--r--   0        0        0      596 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/chatglm.py
+-rw-r--r--   0        0        0      599 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/clarifai.py
+-rw-r--r--   0        0        0      680 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/cloudflare_workersai.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/cohere.py
+-rw-r--r--   0        0        0      614 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/ctransformers.py
+-rw-r--r--   0        0        0      608 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/ctranslate2.py
+-rw-r--r--   0        0        0      605 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/databricks.py
+-rw-r--r--   0        0        0      602 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/deepinfra.py
+-rw-r--r--   0        0        0      605 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/deepsparse.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/edenai.py
+-rw-r--r--   0        0        0      777 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/fake.py
+-rw-r--r--   0        0        0      602 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/fireworks.py
+-rw-r--r--   0        0        0      608 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/forefrontai.py
+-rw-r--r--   0        0        0      599 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/gigachat.py
+-rw-r--r--   0        0        0      605 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/google_palm.py
+-rw-r--r--   0        0        0      596 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/gooseai.py
+-rw-r--r--   0        0        0      596 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/gpt4all.py
+-rw-r--r--   0        0        0      758 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/gradient_ai.py
+-rw-r--r--   0        0        0      664 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/grammars/json.gbnf
+-rw-r--r--   0        0        0      167 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/grammars/list.gbnf
+-rw-r--r--   0        0        0      632 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/huggingface_endpoint.py
+-rw-r--r--   0        0        0      617 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/huggingface_hub.py
+-rw-r--r--   0        0        0      632 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/huggingface_pipeline.py
+-rw-r--r--   0        0        0      656 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/huggingface_text_gen_inference.py
+-rw-r--r--   0        0        0      614 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/human.py
+-rw-r--r--   0        0        0      772 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/javelin_ai_gateway.py
+-rw-r--r--   0        0        0      611 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/koboldai.py
+-rw-r--r--   0        0        0      599 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/llamacpp.py
+-rw-r--r--   0        0        0      736 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/loading.py
+-rw-r--r--   0        0        0      620 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/manifest.py
+-rw-r--r--   0        0        0      596 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/minimax.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/mlflow.py
+-rw-r--r--   0        0        0      620 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0      590 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/modal.py
+-rw-r--r--   0        0        0      599 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/mosaicml.py
+-rw-r--r--   0        0        0      599 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/nlpcloud.py
+-rw-r--r--   0        0        0      617 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/octoai_endpoint.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/ollama.py
+-rw-r--r--   0        0        0      614 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/opaqueprompts.py
+-rw-r--r--   0        0        0      885 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/openai.py
+-rw-r--r--   0        0        0      596 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/openllm.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.246467 langchain-0.2.0rc2/langchain/llms/openlm.py
+-rw-r--r--   0        0        0      617 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/pai_eas_endpoint.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/petals.py
+-rw-r--r--   0        0        0      605 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/pipelineai.py
+-rw-r--r--   0        0        0      602 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/predibase.py
+-rw-r--r--   0        0        0      620 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/predictionguard.py
+-rw-r--r--   0        0        0      742 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/promptlayer_openai.py
+-rw-r--r--   0        0        0      602 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/replicate.py
+-rw-r--r--   0        0        0      587 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/rwkv.py
+-rw-r--r--   0        0        0      808 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/self_hosted.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      611 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/stochasticai.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/symblai_nebula.py
+-rw-r--r--   0        0        0      596 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/textgen.py
+-rw-r--r--   0        0        0      611 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/titan_takeoff.py
+-rw-r--r--   0        0        0      620 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/titan_takeoff_pro.py
+-rw-r--r--   0        0        0      599 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/together.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/tongyi.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/utils.py
+-rw-r--r--   0        0        0      709 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/vertexai.py
+-rw-r--r--   0        0        0      670 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/vllm.py
+-rw-r--r--   0        0        0      805 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/volcengine_maas.py
+-rw-r--r--   0        0        0      605 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/watsonxllm.py
+-rw-r--r--   0        0        0      593 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/writer.py
+-rw-r--r--   0        0        0      605 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/xinference.py
+-rw-r--r--   0        0        0      602 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/llms/yandex.py
+-rw-r--r--   0        0        0      206 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/load/__init__.py
+-rw-r--r--   0        0        0      100 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/load/dump.py
+-rw-r--r--   0        0        0       98 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/load/load.py
+-rw-r--r--   0        0        0      412 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/load/serializable.py
+-rw-r--r--   0        0        0     5389 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/__init__.py
+-rw-r--r--   0        0        0     4861 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/buffer.py
+-rw-r--r--   0        0        0     1616 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/buffer_window.py
+-rw-r--r--   0        0        0     2795 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_memory.py
+-rw-r--r--   0        0        0     3506 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/__init__.py
+-rw-r--r--   0        0        0      692 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/astradb.py
+-rw-r--r--   0        0        0      698 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/cassandra.py
+-rw-r--r--   0        0        0      695 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/cosmos_db.py
+-rw-r--r--   0        0        0      695 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/dynamodb.py
+-rw-r--r--   0        0        0      727 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/elasticsearch.py
+-rw-r--r--   0        0        0      683 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/file.py
+-rw-r--r--   0        0        0      698 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/firestore.py
+-rw-r--r--   0        0        0      130 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/in_memory.py
+-rw-r--r--   0        0        0      692 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/momento.py
+-rw-r--r--   0        0        0      692 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/mongodb.py
+-rw-r--r--   0        0        0      686 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/neo4j.py
+-rw-r--r--   0        0        0      695 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/postgres.py
+-rw-r--r--   0        0        0      686 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/redis.py
+-rw-r--r--   0        0        0      692 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/rocksetdb.py
+-rw-r--r--   0        0        0      727 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/singlestoredb.py
+-rw-r--r--   0        0        0     1033 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/sql.py
+-rw-r--r--   0        0        0      698 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/streamlit.py
+-rw-r--r--   0        0        0      724 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/upstash_redis.py
+-rw-r--r--   0        0        0      683 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/xata.py
+-rw-r--r--   0        0        0      680 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/chat_message_histories/zep.py
+-rw-r--r--   0        0        0     2912 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/combined.py
+-rw-r--r--   0        0        0    15936 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/entity.py
+-rw-r--r--   0        0        0      645 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/kg.py
+-rw-r--r--   0        0        0      658 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/motorhead_memory.py
+-rw-r--r--   0        0        0     8181 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/prompt.py
+-rw-r--r--   0        0        0      792 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/readonly.py
+-rw-r--r--   0        0        0      761 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/simple.py
+-rw-r--r--   0        0        0     3389 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/summary.py
+-rw-r--r--   0        0        0     3043 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/summary_buffer.py
+-rw-r--r--   0        0        0     2144 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/token_buffer.py
+-rw-r--r--   0        0        0      617 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/utils.py
+-rw-r--r--   0        0        0     3875 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/vectorstore.py
+-rw-r--r--   0        0        0      628 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/memory/zep_memory.py
+-rw-r--r--   0        0        0     3278 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/model_laboratory.py
+-rw-r--r--   0        0        0     2719 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1689 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/boolean.py
+-rw-r--r--   0        0        0     1799 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/combining.py
+-rw-r--r--   0        0        0     1974 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1205 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/enum.py
+-rw-r--r--   0        0        0     1427 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/ernie_functions.py
+-rw-r--r--   0        0        0     3150 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/fix.py
+-rw-r--r--   0        0        0     3958 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/format_instructions.py
+-rw-r--r--   0        0        0      340 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/json.py
+-rw-r--r--   0        0        0      310 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/list.py
+-rw-r--r--   0        0        0      702 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/loading.py
+-rw-r--r--   0        0        0      364 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/openai_functions.py
+-rw-r--r--   0        0        0      229 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/openai_tools.py
+-rw-r--r--   0        0        0     6548 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/pandas_dataframe.py
+-rw-r--r--   0        0        0      508 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/prompts.py
+-rw-r--r--   0        0        0       99 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/pydantic.py
+-rw-r--r--   0        0        0      691 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/rail_parser.py
+-rw-r--r--   0        0        0     1214 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/regex.py
+-rw-r--r--   0        0        0     1709 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/regex_dict.py
+-rw-r--r--   0        0        0     7786 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/retry.py
+-rw-r--r--   0        0        0     3132 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/structured.py
+-rw-r--r--   0        0        0       93 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/xml.py
+-rw-r--r--   0        0        0     2181 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/output_parsers/yaml.py
+-rw-r--r--   0        0        0     3152 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/__init__.py
+-rw-r--r--   0        0        0      565 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/base.py
+-rw-r--r--   0        0        0     1045 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/chat.py
+-rw-r--r--   0        0        0     1152 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/example_selector/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/example_selector/base.py
+-rw-r--r--   0        0        0      136 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/example_selector/length_based.py
+-rw-r--r--   0        0        0      877 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/example_selector/ngram_overlap.py
+-rw-r--r--   0        0        0      288 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/example_selector/semantic_similarity.py
+-rw-r--r--   0        0        0      265 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/few_shot.py
+-rw-r--r--   0        0        0      128 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/few_shot_with_templates.py
+-rw-r--r--   0        0        0      530 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/loading.py
+-rw-r--r--   0        0        0      133 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/pipeline.py
+-rw-r--r--   0        0        0      153 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/prompts/prompt.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/py.typed
+-rw-r--r--   0        0        0      897 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      134 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      120 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/pydantic_v1/main.py
+-rw-r--r--   0        0        0      462 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/python.py
+-rw-r--r--   0        0        0      905 2024-05-09 20:46:47.250467 langchain-0.2.0rc2/langchain/requests.py
+-rw-r--r--   0        0        0     6660 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/arcee.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/arxiv.py
+-rw-r--r--   0        0        0      824 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/azure_ai_search.py
+-rw-r--r--   0        0        0      979 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/bedrock.py
+-rw-r--r--   0        0        0      819 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/bm25.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/chaindesk.py
+-rw-r--r--   0        0        0      653 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/chatgpt_plugin_retriever.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/cohere_rag_retriever.py
+-rw-r--r--   0        0        0     2290 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/contextual_compression.py
+-rw-r--r--   0        0        0      661 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/databerry.py
+-rw-r--r--   0        0        0      791 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/docarray.py
+-rw-r--r--   0        0        0      834 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/__init__.py
+-rw-r--r--   0        0        0     2942 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/base.py
+-rw-r--r--   0        0        0     4215 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/chain_extract.py
+-rw-r--r--   0        0        0      366 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/chain_extract_prompt.py
+-rw-r--r--   0        0        0     2935 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/chain_filter.py
+-rw-r--r--   0        0        0      231 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/chain_filter_prompt.py
+-rw-r--r--   0        0        0     4542 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/cohere_rerank.py
+-rw-r--r--   0        0        0      393 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/cross_encoder.py
+-rw-r--r--   0        0        0     1597 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/cross_encoder_rerank.py
+-rw-r--r--   0        0        0     3614 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/embeddings_filter.py
+-rw-r--r--   0        0        0     2503 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/document_compressors/flashrank_rerank.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/elastic_search_bm25.py
+-rw-r--r--   0        0        0      644 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/embedchain.py
+-rw-r--r--   0        0        0     9991 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/ensemble.py
+-rw-r--r--   0        0        0      695 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/google_cloud_documentai_warehouse.py
+-rw-r--r--   0        0        0     1040 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/google_vertex_ai_search.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/kay.py
+-rw-r--r--   0        0        0     2235 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/kendra.py
+-rw-r--r--   0        0        0      623 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/knn.py
+-rw-r--r--   0        0        0      800 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/llama_index.py
+-rw-r--r--   0        0        0     3601 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/merger_retriever.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/metal.py
+-rw-r--r--   0        0        0      796 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/milvus.py
+-rw-r--r--   0        0        0     6760 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/multi_query.py
+-rw-r--r--   0        0        0     3920 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/multi_vector.py
+-rw-r--r--   0        0        0      635 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/outline.py
+-rw-r--r--   0        0        0     5198 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/parent_document_retriever.py
+-rw-r--r--   0        0        0      674 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/pinecone_hybrid_search.py
+-rw-r--r--   0        0        0      632 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/pubmed.py
+-rw-r--r--   0        0        0      632 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/pupmed.py
+-rw-r--r--   0        0        0     2654 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/re_phraser.py
+-rw-r--r--   0        0        0      659 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/remote_retriever.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/__init__.py
+-rw-r--r--   0        0        0      670 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/astradb.py
+-rw-r--r--   0        0        0    12134 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/base.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/chroma.py
+-rw-r--r--   0        0        0      685 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/dashvector.py
+-rw-r--r--   0        0        0      782 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/databricks_vector_search.py
+-rw-r--r--   0        0        0      816 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/deeplake.py
+-rw-r--r--   0        0        0      666 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/dingo.py
+-rw-r--r--   0        0        0      717 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/elasticsearch.py
+-rw-r--r--   0        0        0      792 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/milvus.py
+-rw-r--r--   0        0        0      714 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/mongodb_atlas.py
+-rw-r--r--   0        0        0      670 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/myscale.py
+-rw-r--r--   0        0        0      685 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/opensearch.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/pgvector.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/pinecone.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/qdrant.py
+-rw-r--r--   0        0        0      660 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/redis.py
+-rw-r--r--   0        0        0      693 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/supabase.py
+-rw-r--r--   0        0        0      743 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/tencentvectordb.py
+-rw-r--r--   0        0        0      743 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/timescalevector.py
+-rw-r--r--   0        0        0      798 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/vectara.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/self_query/weaviate.py
+-rw-r--r--   0        0        0      623 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/svm.py
+-rw-r--r--   0        0        0      833 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/tavily_search_api.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/tfidf.py
+-rw-r--r--   0        0        0     7665 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/time_weighted_retriever.py
+-rw-r--r--   0        0        0      629 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/vespa_retriever.py
+-rw-r--r--   0        0        0      674 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/weaviate_hybrid_search.py
+-rw-r--r--   0        0        0      939 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/web_research.py
+-rw-r--r--   0        0        0      641 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/wikipedia.py
+-rw-r--r--   0        0        0      623 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/you.py
+-rw-r--r--   0        0        0      855 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/zep.py
+-rw-r--r--   0        0        0      796 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/retrievers/zilliz.py
+-rw-r--r--   0        0        0      693 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/runnables/__init__.py
+-rw-r--r--   0        0        0      809 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/runnables/hub.py
+-rw-r--r--   0        0        0     1525 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/runnables/openai_functions.py
+-rw-r--r--   0        0        0     2065 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/__init__.py
+-rw-r--r--   0        0        0      149 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/agent.py
+-rw-r--r--   0        0        0      105 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/cache.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/__init__.py
+-rw-r--r--   0        0        0      511 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/base.py
+-rw-r--r--   0        0        0     1511 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/manager.py
+-rw-r--r--   0        0        0      103 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/stdout.py
+-rw-r--r--   0        0        0      131 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/tracers/base.py
+-rw-r--r--   0        0        0      176 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/tracers/evaluation.py
+-rw-r--r--   0        0        0      219 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/tracers/langchain.py
+-rw-r--r--   0        0        0      127 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/tracers/langchain_v1.py
+-rw-r--r--   0        0        0      226 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/tracers/log_stream.py
+-rw-r--r--   0        0        0      105 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/tracers/root_listeners.py
+-rw-r--r--   0        0        0      120 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/tracers/run_collector.py
+-rw-r--r--   0        0        0      470 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/tracers/schemas.py
+-rw-r--r--   0        0        0      257 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/callbacks/tracers/stdout.py
+-rw-r--r--   0        0        0       80 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/chat.py
+-rw-r--r--   0        0        0      101 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/chat_history.py
+-rw-r--r--   0        0        0      122 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/document.py
+-rw-r--r--   0        0        0       75 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/embeddings.py
+-rw-r--r--   0        0        0       91 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/exceptions.py
+-rw-r--r--   0        0        0      367 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/language_model.py
+-rw-r--r--   0        0        0       71 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/memory.py
+-rw-r--r--   0        0        0     1048 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/messages.py
+-rw-r--r--   0        0        0      320 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/output.py
+-rw-r--r--   0        0        0      651 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/output_parser.py
+-rw-r--r--   0        0        0       80 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/prompt.py
+-rw-r--r--   0        0        0      124 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/prompt_template.py
+-rw-r--r--   0        0        0       81 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/retriever.py
+-rw-r--r--   0        0        0     1796 2024-05-09 20:46:47.254468 langchain-0.2.0rc2/langchain/schema/runnable/__init__.py
+-rw-r--r--   0        0        0      781 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/runnable/base.py
+-rw-r--r--   0        0        0       89 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/runnable/branch.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/runnable/config.py
+-rw-r--r--   0        0        0      333 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/runnable/configurable.py
+-rw-r--r--   0        0        0      106 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/runnable/fallbacks.py
+-rw-r--r--   0        0        0      260 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/runnable/history.py
+-rw-r--r--   0        0        0      205 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/runnable/passthrough.py
+-rw-r--r--   0        0        0       94 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/runnable/retry.py
+-rw-r--r--   0        0        0      117 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/runnable/router.py
+-rw-r--r--   0        0        0     1118 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/runnable/utils.py
+-rw-r--r--   0        0        0       85 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/storage.py
+-rw-r--r--   0        0        0      137 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/schema/vectorstore.py
+-rw-r--r--   0        0        0      662 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/serpapi.py
+-rw-r--r--   0        0        0     3544 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/smith/__init__.py
+-rw-r--r--   0        0        0     2199 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/smith/evaluation/__init__.py
+-rw-r--r--   0        0        0    13429 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/smith/evaluation/config.py
+-rw-r--r--   0        0        0     9936 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/smith/evaluation/name_generation.py
+-rw-r--r--   0        0        0     3310 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/smith/evaluation/progress.py
+-rw-r--r--   0        0        0    54230 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/smith/evaluation/runner_utils.py
+-rw-r--r--   0        0        0    17112 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/smith/evaluation/string_run_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/smith/evaluation/utils.py
+-rw-r--r--   0        0        0      663 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/sql_database.py
+-rw-r--r--   0        0        0     1584 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/storage/__init__.py
+-rw-r--r--   0        0        0     2517 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/storage/_lc_store.py
+-rw-r--r--   0        0        0     4333 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/storage/encoder_backed.py
+-rw-r--r--   0        0        0       89 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/storage/exceptions.py
+-rw-r--r--   0        0        0     6107 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/storage/file_system.py
+-rw-r--r--   0        0        0      368 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/storage/in_memory.py
+-rw-r--r--   0        0        0      611 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/storage/redis.py
+-rw-r--r--   0        0        0      751 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/storage/upstash_redis.py
+-rw-r--r--   0        0        0     1553 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/text_splitter.py
+-rw-r--r--   0        0        0     5662 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/ainetwork/__init__.py
+-rw-r--r--   0        0        0      863 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/ainetwork/app.py
+-rw-r--r--   0        0        0      748 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/ainetwork/base.py
+-rw-r--r--   0        0        0      767 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/ainetwork/owner.py
+-rw-r--r--   0        0        0      762 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/ainetwork/rule.py
+-rw-r--r--   0        0        0      785 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/ainetwork/transfer.py
+-rw-r--r--   0        0        0      770 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/ainetwork/value.py
+-rw-r--r--   0        0        0      905 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/amadeus/__init__.py
+-rw-r--r--   0        0        0      648 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/amadeus/base.py
+-rw-r--r--   0        0        0      851 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/amadeus/closest_airport.py
+-rw-r--r--   0        0        0      833 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/amadeus/flight_search.py
+-rw-r--r--   0        0        0       25 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/arxiv/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/arxiv/tool.py
+-rw-r--r--   0        0        0     1258 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/__init__.py
+-rw-r--r--   0        0        0      658 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/form_recognizer.py
+-rw-r--r--   0        0        0      655 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/image_analysis.py
+-rw-r--r--   0        0        0      649 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/speech2text.py
+-rw-r--r--   0        0        0      649 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/text2speech.py
+-rw-r--r--   0        0        0      673 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/text_analytics_health.py
+-rw-r--r--   0        0        0      332 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/base.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/bearly/__init__.py
+-rw-r--r--   0        0        0      957 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/bearly/tool.py
+-rw-r--r--   0        0        0      752 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/bing_search/__init__.py
+-rw-r--r--   0        0        0      721 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/bing_search/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/brave_search/__init__.py
+-rw-r--r--   0        0        0      610 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/brave_search/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/clickup/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/clickup/tool.py
+-rw-r--r--   0        0        0      157 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/convert_to_openai.py
+-rw-r--r--   0        0        0      927 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/dataforseo_api_search/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/dataforseo_api_search/tool.py
+-rw-r--r--   0        0        0      671 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/ddg_search/__init__.py
+-rw-r--r--   0        0        0     1024 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/ddg_search/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/e2b_data_analysis/__init__.py
+-rw-r--r--   0        0        0      990 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/e2b_data_analysis/tool.py
+-rw-r--r--   0        0        0     1513 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/edenai/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/edenai/audio_speech_to_text.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/edenai/audio_text_to_speech.py
+-rw-r--r--   0        0        0      607 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/edenai/edenai_base_tool.py
+-rw-r--r--   0        0        0      646 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/edenai/image_explicitcontent.py
+-rw-r--r--   0        0        0      652 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/edenai/image_objectdetection.py
+-rw-r--r--   0        0        0      634 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/edenai/ocr_identityparser.py
+-rw-r--r--   0        0        0      649 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/edenai/ocr_invoiceparser.py
+-rw-r--r--   0        0        0      649 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/edenai/text_moderation.py
+-rw-r--r--   0        0        0      686 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/eleven_labs/__init__.py
+-rw-r--r--   0        0        0      660 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/eleven_labs/models.py
+-rw-r--r--   0        0        0      652 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/eleven_labs/text2speech.py
+-rw-r--r--   0        0        0     1242 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/file_management/__init__.py
+-rw-r--r--   0        0        0      789 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/file_management/copy.py
+-rw-r--r--   0        0        0      805 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/file_management/delete.py
+-rw-r--r--   0        0        0      815 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/file_management/file_search.py
+-rw-r--r--   0        0        0      836 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/file_management/list_dir.py
+-rw-r--r--   0        0        0      789 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/file_management/move.py
+-rw-r--r--   0        0        0      789 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/file_management/read.py
+-rw-r--r--   0        0        0      797 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/file_management/write.py
+-rw-r--r--   0        0        0       20 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/github/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/github/tool.py
+-rw-r--r--   0        0        0       20 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/gitlab/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-09 20:46:47.258468 langchain-0.2.0rc2/langchain/tools/gitlab/tool.py
+-rw-r--r--   0        0        0     1056 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/gmail/__init__.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/gmail/base.py
+-rw-r--r--   0        0        0      809 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/gmail/create_draft.py
+-rw-r--r--   0        0        0      801 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/gmail/get_message.py
+-rw-r--r--   0        0        0      793 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/gmail/get_thread.py
+-rw-r--r--   0        0        0      863 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/gmail/search.py
+-rw-r--r--   0        0        0      809 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/gmail/send_message.py
+-rw-r--r--   0        0        0      681 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/golden_query/__init__.py
+-rw-r--r--   0        0        0      655 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/golden_query/tool.py
+-rw-r--r--   0        0        0      684 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_cloud/__init__.py
+-rw-r--r--   0        0        0      658 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_cloud/texttospeech.py
+-rw-r--r--   0        0        0      720 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_finance/__init__.py
+-rw-r--r--   0        0        0      686 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_finance/tool.py
+-rw-r--r--   0        0        0      696 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_jobs/__init__.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_jobs/tool.py
+-rw-r--r--   0        0        0      696 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_lens/__init__.py
+-rw-r--r--   0        0        0      665 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_lens/tool.py
+-rw-r--r--   0        0        0      658 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_places/__init__.py
+-rw-r--r--   0        0        0      812 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_places/tool.py
+-rw-r--r--   0        0        0      720 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_scholar/__init__.py
+-rw-r--r--   0        0        0      686 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_scholar/tool.py
+-rw-r--r--   0        0        0      766 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_search/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_search/tool.py
+-rw-r--r--   0        0        0      815 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_serper/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_serper/tool.py
+-rw-r--r--   0        0        0      714 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_trends/__init__.py
+-rw-r--r--   0        0        0      681 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/google_trends/tool.py
+-rw-r--r--   0        0        0       47 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/graphql/__init__.py
+-rw-r--r--   0        0        0      622 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/graphql/tool.py
+-rw-r--r--   0        0        0      655 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/human/__init__.py
+-rw-r--r--   0        0        0      616 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/human/tool.py
+-rw-r--r--   0        0        0      613 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/ifttt.py
+-rw-r--r--   0        0        0       43 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/interaction/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/interaction/tool.py
+-rw-r--r--   0        0        0       17 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/jira/__init__.py
+-rw-r--r--   0        0        0      607 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/jira/tool.py
+-rw-r--r--   0        0        0       46 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/json/__init__.py
+-rw-r--r--   0        0        0      859 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/json/tool.py
+-rw-r--r--   0        0        0      677 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/memorize/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/memorize/tool.py
+-rw-r--r--   0        0        0       35 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/merriam_webster/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/merriam_webster/tool.py
+-rw-r--r--   0        0        0      675 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/metaphor_search/__init__.py
+-rw-r--r--   0        0        0      640 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/metaphor_search/tool.py
+-rw-r--r--   0        0        0     1105 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/multion/__init__.py
+-rw-r--r--   0        0        0      833 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/multion/close_session.py
+-rw-r--r--   0        0        0      842 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/multion/create_session.py
+-rw-r--r--   0        0        0      842 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/multion/update_session.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/nasa/__init__.py
+-rw-r--r--   0        0        0      607 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/nasa/tool.py
+-rw-r--r--   0        0        0      667 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/nuclia/__init__.py
+-rw-r--r--   0        0        0      760 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/nuclia/tool.py
+-rw-r--r--   0        0        0     1085 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/office365/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/office365/base.py
+-rw-r--r--   0        0        0      905 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/office365/create_draft_message.py
+-rw-r--r--   0        0        0      819 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/office365/events_search.py
+-rw-r--r--   0        0        0      823 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/office365/messages_search.py
+-rw-r--r--   0        0        0      798 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/office365/send_event.py
+-rw-r--r--   0        0        0      814 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/office365/send_message.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/openapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/openapi/utils/__init__.py
+-rw-r--r--   0        0        0     1859 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/openapi/utils/api_models.py
+-rw-r--r--   0        0        0      833 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/openapi/utils/openapi_utils.py
+-rw-r--r--   0        0        0      677 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/openweathermap/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/openweathermap/tool.py
+-rw-r--r--   0        0        0     1282 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/playwright/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/playwright/base.py
+-rw-r--r--   0        0        0      775 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/playwright/click.py
+-rw-r--r--   0        0        0      631 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/playwright/current_page.py
+-rw-r--r--   0        0        0      906 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/playwright/extract_hyperlinks.py
+-rw-r--r--   0        0        0      622 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/playwright/extract_text.py
+-rw-r--r--   0        0        0      825 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/playwright/get_elements.py
+-rw-r--r--   0        0        0      799 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/playwright/navigate.py
+-rw-r--r--   0        0        0      625 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/playwright/navigate_back.py
+-rw-r--r--   0        0        0      935 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/plugin.py
+-rw-r--r--   0        0        0       52 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/powerbi/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/powerbi/tool.py
+-rw-r--r--   0        0        0       26 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/pubmed/__init__.py
+-rw-r--r--   0        0        0      619 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/pubmed/tool.py
+-rw-r--r--   0        0        0      515 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/python/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/reddit_search/__init__.py
+-rw-r--r--   0        0        0      730 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/reddit_search/tool.py
+-rw-r--r--   0        0        0      705 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/render.py
+-rw-r--r--   0        0        0       52 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/requests/__init__.py
+-rw-r--r--   0        0        0     1167 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/requests/tool.py
+-rw-r--r--   0        0        0      328 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/retriever.py
+-rw-r--r--   0        0        0       31 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/scenexplain/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/scenexplain/tool.py
+-rw-r--r--   0        0        0      797 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/searchapi/__init__.py
+-rw-r--r--   0        0        0      715 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/searchapi/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/searx_search/__init__.py
+-rw-r--r--   0        0        0      727 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/searx_search/tool.py
+-rw-r--r--   0        0        0      622 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/shell/__init__.py
+-rw-r--r--   0        0        0      751 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/shell/tool.py
+-rw-r--r--   0        0        0      983 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/slack/__init__.py
+-rw-r--r--   0        0        0      638 2024-05-09 20:46:47.262467 langchain-0.2.0rc2/langchain/tools/slack/base.py
+-rw-r--r--   0        0        0      622 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/slack/get_channel.py
+-rw-r--r--   0        0        0      816 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/slack/get_message.py
+-rw-r--r--   0        0        0      841 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/slack/schedule_message.py
+-rw-r--r--   0        0        0      809 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/slack/send_message.py
+-rw-r--r--   0        0        0       18 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/sleep/__init__.py
+-rw-r--r--   0        0        0      751 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/sleep/tool.py
+-rw-r--r--   0        0        0       44 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/spark_sql/__init__.py
+-rw-r--r--   0        0        0     1064 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/spark_sql/tool.py
+-rw-r--r--   0        0        0       49 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/sql_database/__init__.py
+-rw-r--r--   0        0        0      504 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/sql_database/prompt.py
+-rw-r--r--   0        0        0     1109 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/sql_database/tool.py
+-rw-r--r--   0        0        0       33 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/stackexchange/__init__.py
+-rw-r--r--   0        0        0      628 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/stackexchange/tool.py
+-rw-r--r--   0        0        0       24 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/steam/__init__.py
+-rw-r--r--   0        0        0      634 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/steam/tool.py
+-rw-r--r--   0        0        0      694 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/steamship_image_generation/__init__.py
+-rw-r--r--   0        0        0      847 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/steamship_image_generation/tool.py
+-rw-r--r--   0        0        0      839 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/tavily_search/__init__.py
+-rw-r--r--   0        0        0      913 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/tavily_search/tool.py
+-rw-r--r--   0        0        0       51 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/vectorstore/__init__.py
+-rw-r--r--   0        0        0      791 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/vectorstore/tool.py
+-rw-r--r--   0        0        0       29 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/wikipedia/__init__.py
+-rw-r--r--   0        0        0      628 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/wikipedia/tool.py
+-rw-r--r--   0        0        0      670 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/wolfram_alpha/tool.py
+-rw-r--r--   0        0        0      637 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/yahoo_finance_news.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/youtube/__init__.py
+-rw-r--r--   0        0        0      628 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/youtube/search.py
+-rw-r--r--   0        0        0      764 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/zapier/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/tools/zapier/tool.py
+-rw-r--r--   0        0        0     5891 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/__init__.py
+-rw-r--r--   0        0        0      651 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/alpha_vantage.py
+-rw-r--r--   0        0        0      839 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/anthropic.py
+-rw-r--r--   0        0        0      621 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/apify.py
+-rw-r--r--   0        0        0     1336 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/arcee.py
+-rw-r--r--   0        0        0      630 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/arxiv.py
+-rw-r--r--   0        0        0      274 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/asyncio.py
+-rw-r--r--   0        0        0      624 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/awslambda.py
+-rw-r--r--   0        0        0      642 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/bibtex.py
+-rw-r--r--   0        0        0      645 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/bing_search.py
+-rw-r--r--   0        0        0      639 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/brave_search.py
+-rw-r--r--   0        0        0     1180 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/clickup.py
+-rw-r--r--   0        0        0      680 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/dalle_image_generator.py
+-rw-r--r--   0        0        0      695 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/dataforseo_api_search.py
+-rw-r--r--   0        0        0      663 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/duckduckgo_search.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/github.py
+-rw-r--r--   0        0        0      647 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/gitlab.py
+-rw-r--r--   0        0        0      648 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/golden_query.py
+-rw-r--r--   0        0        0      654 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/google_finance.py
+-rw-r--r--   0        0        0      645 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/google_jobs.py
+-rw-r--r--   0        0        0      645 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/google_lens.py
+-rw-r--r--   0        0        0      651 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/google_places_api.py
+-rw-r--r--   0        0        0      654 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/google_scholar.py
+-rw-r--r--   0        0        0      651 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/google_search.py
+-rw-r--r--   0        0        0      651 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/google_serper.py
+-rw-r--r--   0        0        0      651 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/google_trends.py
+-rw-r--r--   0        0        0      636 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/graphql.py
+-rw-r--r--   0        0        0      627 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/jira.py
+-rw-r--r--   0        0        0      122 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/loading.py
+-rw-r--r--   0        0        0      645 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/max_compute.py
+-rw-r--r--   0        0        0      657 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/merriam_webster.py
+-rw-r--r--   0        0        0      657 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/metaphor_search.py
+-rw-r--r--   0        0        0      627 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/nasa.py
+-rw-r--r--   0        0        0      739 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/opaqueprompts.py
+-rw-r--r--   0        0        0      753 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/openapi.py
+-rw-r--r--   0        0        0      657 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/openweathermap.py
+-rw-r--r--   0        0        0      636 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/outline.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/portkey.py
+-rw-r--r--   0        0        0      627 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/powerbi.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/pubmed.py
+-rw-r--r--   0        0        0      462 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/python.py
+-rw-r--r--   0        0        0      685 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/reddit_search.py
+-rw-r--r--   0        0        0      889 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/redis.py
+-rw-r--r--   0        0        0      712 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/requests.py
+-rw-r--r--   0        0        0      648 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/scenexplain.py
+-rw-r--r--   0        0        0      642 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/searchapi.py
+-rw-r--r--   0        0        0      804 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/searx_search.py
+-rw-r--r--   0        0        0      782 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/serpapi.py
+-rw-r--r--   0        0        0      609 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/spark_sql.py
+-rw-r--r--   0        0        0      786 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/sql_database.py
+-rw-r--r--   0        0        0      654 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/stackexchange.py
+-rw-r--r--   0        0        0      639 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/steam.py
+-rw-r--r--   0        0        0      685 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/tavily_search.py
+-rw-r--r--   0        0        0      639 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/tensorflow_datasets.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/twilio.py
+-rw-r--r--   0        0        0     1056 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/vertexai.py
+-rw-r--r--   0        0        0      642 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/wikipedia.py
+-rw-r--r--   0        0        0      651 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/wolfram_alpha.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utilities/zapier.py
+-rw-r--r--   0        0        0     1846 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/__init__.py
+-rw-r--r--   0        0        0      102 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/aiter.py
+-rw-r--r--   0        0        0      124 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/env.py
+-rw-r--r--   0        0        0     1140 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/ernie_functions.py
+-rw-r--r--   0        0        0       91 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/formatting.py
+-rw-r--r--   0        0        0      421 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/html.py
+-rw-r--r--   0        0        0      211 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/input.py
+-rw-r--r--   0        0        0      133 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/iter.py
+-rw-r--r--   0        0        0      258 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/json_schema.py
+-rw-r--r--   0        0        0       92 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/loading.py
+-rw-r--r--   0        0        0      918 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/math.py
+-rw-r--r--   0        0        0      627 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/openai.py
+-rw-r--r--   0        0        0      325 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/openai_functions.py
+-rw-r--r--   0        0        0      111 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/pydantic.py
+-rw-r--r--   0        0        0      148 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/strings.py
+-rw-r--r--   0        0        0      446 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/utils/utils.py
+-rw-r--r--   0        0        0     8070 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/vectorstores/__init__.py
+-rw-r--r--   0        0        0      833 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/vectorstores/alibabacloud_opensearch.py
+-rw-r--r--   0        0        0      621 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/vectorstores/analyticdb.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/vectorstores/annoy.py
+-rw-r--r--   0        0        0      612 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/vectorstores/astradb.py
+-rw-r--r--   0        0        0      612 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/vectorstores/atlas.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/vectorstores/awadb.py
+-rw-r--r--   0        0        0      873 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/vectorstores/azure_cosmos_db.py
+-rw-r--r--   0        0        0      867 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/vectorstores/azuresearch.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.266467 langchain-0.2.0rc2/langchain/vectorstores/bageldb.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/baiducloud_vector_search.py
+-rw-r--r--   0        0        0      125 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/base.py
+-rw-r--r--   0        0        0      618 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/cassandra.py
+-rw-r--r--   0        0        0      609 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/chroma.py
+-rw-r--r--   0        0        0      615 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/clarifai.py
+-rw-r--r--   0        0        0      736 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/clickhouse.py
+-rw-r--r--   0        0        0      621 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/dashvector.py
+-rw-r--r--   0        0        0      657 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/databricks_vector_search.py
+-rw-r--r--   0        0        0      615 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/deeplake.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/dingo.py
+-rw-r--r--   0        0        0      797 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/docarray/__init__.py
+-rw-r--r--   0        0        0      658 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/docarray/base.py
+-rw-r--r--   0        0        0      645 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/docarray/hnsw.py
+-rw-r--r--   0        0        0      657 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/docarray/in_memory.py
+-rw-r--r--   0        0        0      757 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/elastic_vector_search.py
+-rw-r--r--   0        0        0     1294 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/elasticsearch.py
+-rw-r--r--   0        0        0      612 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/epsilla.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/faiss.py
+-rw-r--r--   0        0        0      618 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/hippo.py
+-rw-r--r--   0        0        0      615 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/hologres.py
+-rw-r--r--   0        0        0      612 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/lancedb.py
+-rw-r--r--   0        0        0      795 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/llm_rails.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/marqo.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/matching_engine.py
+-rw-r--r--   0        0        0      624 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/meilisearch.py
+-rw-r--r--   0        0        0      609 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/milvus.py
+-rw-r--r--   0        0        0      645 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/momento_vector_index.py
+-rw-r--r--   0        0        0      663 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/mongodb_atlas.py
+-rw-r--r--   0        0        0      890 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/myscale.py
+-rw-r--r--   0        0        0      789 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/neo4j_vector.py
+-rw-r--r--   0        0        0      633 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/nucliadb.py
+-rw-r--r--   0        0        0      657 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/opensearch_vector_search.py
+-rw-r--r--   0        0        0     1042 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/pgembedding.py
+-rw-r--r--   0        0        0      643 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/pgvecto_rs.py
+-rw-r--r--   0        0        0      790 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/pgvector.py
+-rw-r--r--   0        0        0      615 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/pinecone.py
+-rw-r--r--   0        0        0      777 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/qdrant.py
+-rw-r--r--   0        0        0     1295 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/redis/__init__.py
+-rw-r--r--   0        0        0      956 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/redis/base.py
+-rw-r--r--   0        0        0     1514 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/redis/filters.py
+-rw-r--r--   0        0        0     1745 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/redis/schema.py
+-rw-r--r--   0        0        0      612 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/rocksetdb.py
+-rw-r--r--   0        0        0      606 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/scann.py
+-rw-r--r--   0        0        0      609 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/semadb.py
+-rw-r--r--   0        0        0      630 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/singlestoredb.py
+-rw-r--r--   0        0        0     1325 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/sklearn.py
+-rw-r--r--   0        0        0      618 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/sqlitevss.py
+-rw-r--r--   0        0        0      798 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/starrocks.py
+-rw-r--r--   0        0        0      648 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/supabase.py
+-rw-r--r--   0        0        0      603 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/tair.py
+-rw-r--r--   0        0        0      953 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/tencentvectordb.py
+-rw-r--r--   0        0        0      609 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/tigris.py
+-rw-r--r--   0        0        0      609 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/tiledb.py
+-rw-r--r--   0        0        0      636 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/timescalevector.py
+-rw-r--r--   0        0        0      618 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/typesense.py
+-rw-r--r--   0        0        0      612 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/usearch.py
+-rw-r--r--   0        0        0      958 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/utils.py
+-rw-r--r--   0        0        0      603 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/vald.py
+-rw-r--r--   0        0        0      609 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/vearch.py
+-rw-r--r--   0        0        0      785 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/vectara.py
+-rw-r--r--   0        0        0      621 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/vespa.py
+-rw-r--r--   0        0        0      615 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/weaviate.py
+-rw-r--r--   0        0        0      646 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/xata.py
+-rw-r--r--   0        0        0      624 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/yellowbrick.py
+-rw-r--r--   0        0        0      798 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/zep.py
+-rw-r--r--   0        0        0      609 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/langchain/vectorstores/zilliz.py
+-rw-r--r--   0        0        0    11803 2024-05-09 20:46:47.270467 langchain-0.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    13751 1970-01-01 00:00:00.000000 langchain-0.2.0rc2/PKG-INFO
```

### Comparing `langchain-0.2.0rc1/LICENSE` & `langchain-0.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/README.md` & `langchain-0.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/__init__.py` & `langchain-0.2.0rc2/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/_api/__init__.py` & `langchain-0.2.0rc2/langchain/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/_api/module_import.py` & `langchain-0.2.0rc2/langchain/_api/module_import.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/adapters/openai.py` & `langchain-0.2.0rc2/langchain/adapters/openai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/__init__.py` & `langchain-0.2.0rc2/langchain/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent.py` & `langchain-0.2.0rc2/langchain/agents/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Chain that takes in an input and produces an action and action input."""
+
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import time
 from abc import abstractmethod
@@ -342,19 +343,19 @@
     """Agent powered by runnables."""
 
     runnable: Runnable[dict, Union[AgentAction, AgentFinish]]
     """Runnable to call to get agent action."""
     input_keys_arg: List[str] = []
     return_keys_arg: List[str] = []
     stream_runnable: bool = True
-    """Whether to stream from the runnable or not. 
+    """Whether to stream from the runnable or not.
 
-    If True then underlying LLM is invoked in a streaming fashion to make it possible 
-        to get access to the individual LLM tokens when using stream_log with the Agent 
-        Executor. If False then LLM is invoked in a non-streaming fashion and 
+    If True then underlying LLM is invoked in a streaming fashion to make it possible
+        to get access to the individual LLM tokens when using stream_log with the Agent
+        Executor. If False then LLM is invoked in a non-streaming fashion and
         individual LLM tokens will not be available in stream_log.
     """
 
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
@@ -451,19 +452,19 @@
     """Agent powered by runnables."""
 
     runnable: Runnable[dict, Union[List[AgentAction], AgentFinish]]
     """Runnable to call to get agent actions."""
     input_keys_arg: List[str] = []
     return_keys_arg: List[str] = []
     stream_runnable: bool = True
-    """Whether to stream from the runnable or not. 
-    
-    If True then underlying LLM is invoked in a streaming fashion to make it possible 
-        to get access to the individual LLM tokens when using stream_log with the Agent 
-        Executor. If False then LLM is invoked in a non-streaming fashion and 
+    """Whether to stream from the runnable or not.
+
+    If True then underlying LLM is invoked in a streaming fashion to make it possible
+        to get access to the individual LLM tokens when using stream_log with the Agent
+        Executor. If False then LLM is invoked in a non-streaming fashion and
         individual LLM tokens will not be available in stream_log.
     """
 
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
@@ -922,27 +923,27 @@
     """The valid tools the agent can call."""
     return_intermediate_steps: bool = False
     """Whether to return the agent's trajectory of intermediate steps
     at the end in addition to the final output."""
     max_iterations: Optional[int] = 15
     """The maximum number of steps to take before ending the execution
     loop.
-    
+
     Setting to 'None' could lead to an infinite loop."""
     max_execution_time: Optional[float] = None
     """The maximum amount of wall clock time to spend in the execution
     loop.
     """
     early_stopping_method: str = "force"
     """The method to use for early stopping if the agent never
     returns `AgentFinish`. Either 'force' or 'generate'.
 
     `"force"` returns a string saying that it stopped because it met a
         time or iteration limit.
-    
+
     `"generate"` calls the agent's LLM Chain one final time to generate
         a final answer based on the previous steps.
     """
     handle_parsing_errors: Union[
         bool, str, Callable[[OutputParserException], str]
     ] = False
     """How to handle errors raised by the agent's output parser.
@@ -1561,14 +1562,15 @@
         iterator = AgentExecutorIterator(
             self,
             input,
             config.get("callbacks"),
             tags=config.get("tags"),
             metadata=config.get("metadata"),
             run_name=config.get("run_name"),
+            run_id=config.get("run_id"),
             yield_actions=True,
             **kwargs,
         )
         for step in iterator:
             yield step
 
     async def astream(
@@ -1582,12 +1584,13 @@
         iterator = AgentExecutorIterator(
             self,
             input,
             config.get("callbacks"),
             tags=config.get("tags"),
             metadata=config.get("metadata"),
             run_name=config.get("run_name"),
+            run_id=config.get("run_id"),
             yield_actions=True,
             **kwargs,
         )
         async for step in iterator:
             yield step
```

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_iterator.py` & `langchain-0.2.0rc2/langchain/agents/agent_iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Dict,
     Iterator,
     List,
     Optional,
     Tuple,
     Union,
 )
+from uuid import UUID
 
 from langchain_core.agents import (
     AgentAction,
     AgentFinish,
     AgentStep,
 )
 from langchain_core.callbacks import (
@@ -50,36 +51,39 @@
         agent_executor: AgentExecutor,
         inputs: Any,
         callbacks: Callbacks = None,
         *,
         tags: Optional[list[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         run_name: Optional[str] = None,
+        run_id: Optional[UUID] = None,
         include_run_info: bool = False,
         yield_actions: bool = False,
     ):
         """
         Initialize the AgentExecutorIterator with the given AgentExecutor,
         inputs, and optional callbacks.
         """
         self._agent_executor = agent_executor
         self.inputs = inputs
         self.callbacks = callbacks
         self.tags = tags
         self.metadata = metadata
         self.run_name = run_name
+        self.run_id = run_id
         self.include_run_info = include_run_info
         self.yield_actions = yield_actions
         self.reset()
 
     _inputs: Dict[str, str]
     callbacks: Callbacks
     tags: Optional[list[str]]
     metadata: Optional[Dict[str, Any]]
     run_name: Optional[str]
+    run_id: Optional[UUID]
     include_run_info: bool
     yield_actions: bool
 
     @property
     def inputs(self) -> Dict[str, str]:
         return self._inputs
 
@@ -158,14 +162,15 @@
             self.agent_executor.tags,
             self.metadata,
             self.agent_executor.metadata,
         )
         run_manager = callback_manager.on_chain_start(
             dumpd(self.agent_executor),
             self.inputs,
+            self.run_id,
             name=self.run_name,
         )
         try:
             while self.agent_executor._should_continue(
                 self.iterations, self.time_elapsed
             ):
                 # take the next step: this plans next action, executes it,
@@ -223,14 +228,15 @@
             self.agent_executor.tags,
             self.metadata,
             self.agent_executor.metadata,
         )
         run_manager = await callback_manager.on_chain_start(
             dumpd(self.agent_executor),
             self.inputs,
+            self.run_id,
             name=self.run_name,
         )
         try:
             async with asyncio_timeout(self.agent_executor.max_execution_time):
                 while self.agent_executor._should_continue(
                     self.iterations, self.time_elapsed
                 ):
```

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/__init__.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/ainetwork/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/ainetwork/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/amadeus/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/amadeus/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/azure_cognitive_services.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/azure_cognitive_services.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/clickup/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/clickup/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/csv/__init__.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/file_management/__init__.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/file_management/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/file_management/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/github/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/github/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/gitlab/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/gitlab/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/gmail/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/gmail/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/jira/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/jira/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/json/base.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/json/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/json/prompt.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/json/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/json/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/json/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/multion/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/multion/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/nasa/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/nasa/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/nla/tool.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/nla/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/nla/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/nla/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/office365/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/office365/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/base.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/planner.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/planner.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/planner_prompt.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/planner_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/prompt.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/spec.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/spec.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/openapi/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/openapi/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/pandas/__init__.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/playwright/__init__.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/playwright/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/playwright/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/powerbi/base.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/powerbi/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/powerbi/chat_base.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/powerbi/chat_base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/powerbi/prompt.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/powerbi/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/powerbi/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/python/__init__.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/slack/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/slack/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/spark/__init__.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/spark_sql/base.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/spark_sql/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/spark_sql/prompt.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/spark_sql/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/spark_sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/sql/base.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/sql/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/sql/prompt.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/sql/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/steam/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/steam/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/vectorstore/base.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/vectorstore/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/vectorstore/prompt.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/vectorstore/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/vectorstore/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/vectorstore/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/xorbits/__init__.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/xorbits/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_toolkits/zapier/toolkit.py` & `langchain-0.2.0rc2/langchain/agents/agent_toolkits/zapier/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/agent_types.py` & `langchain-0.2.0rc2/langchain/agents/agent_types.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/chat/base.py` & `langchain-0.2.0rc2/langchain/agents/chat/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/chat/output_parser.py` & `langchain-0.2.0rc2/langchain/agents/chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/chat/prompt.py` & `langchain-0.2.0rc2/langchain/agents/chat/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/conversational/base.py` & `langchain-0.2.0rc2/langchain/agents/conversational/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/conversational/output_parser.py` & `langchain-0.2.0rc2/langchain/agents/conversational/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/conversational/prompt.py` & `langchain-0.2.0rc2/langchain/agents/conversational/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/conversational_chat/base.py` & `langchain-0.2.0rc2/langchain/agents/conversational_chat/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/conversational_chat/output_parser.py` & `langchain-0.2.0rc2/langchain/agents/conversational_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/conversational_chat/prompt.py` & `langchain-0.2.0rc2/langchain/agents/conversational_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/format_scratchpad/__init__.py` & `langchain-0.2.0rc2/langchain/agents/format_scratchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/format_scratchpad/log.py` & `langchain-0.2.0rc2/langchain/agents/format_scratchpad/log.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/format_scratchpad/log_to_messages.py` & `langchain-0.2.0rc2/langchain/agents/format_scratchpad/log_to_messages.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/format_scratchpad/openai_functions.py` & `langchain-0.2.0rc2/langchain/agents/format_scratchpad/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/format_scratchpad/tools.py` & `langchain-0.2.0rc2/langchain/agents/format_scratchpad/tools.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/format_scratchpad/xml.py` & `langchain-0.2.0rc2/langchain/agents/format_scratchpad/xml.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/initialize.py` & `langchain-0.2.0rc2/langchain/agents/initialize.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/json_chat/base.py` & `langchain-0.2.0rc2/langchain/agents/json_chat/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/json_chat/prompt.py` & `langchain-0.2.0rc2/langchain/agents/json_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/loading.py` & `langchain-0.2.0rc2/langchain/agents/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/mrkl/base.py` & `langchain-0.2.0rc2/langchain/agents/mrkl/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/mrkl/output_parser.py` & `langchain-0.2.0rc2/langchain/agents/mrkl/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/mrkl/prompt.py` & `langchain-0.2.0rc2/langchain/agents/mrkl/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/openai_assistant/base.py` & `langchain-0.2.0rc2/langchain/agents/openai_assistant/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,32 +430,32 @@
                             "content": input["content"],
                             "file_ids": input.get("file_ids", []),
                             "metadata": input.get("message_metadata"),
                         }
                     ],
                     "metadata": input.get("thread_metadata"),
                 }
-                run = await self._create_thread_and_run(input, thread)
+                run = await self._acreate_thread_and_run(input, thread)
             # Starting a new run in an existing thread.
             elif "run_id" not in input:
                 _ = await self.async_client.beta.threads.messages.create(
                     input["thread_id"],
                     content=input["content"],
                     role="user",
                     file_ids=input.get("file_ids", []),
                     metadata=input.get("message_metadata"),
                 )
-                run = await self._create_run(input)
+                run = await self._acreate_run(input)
             # Submitting tool outputs to an existing run, outside the AgentExecutor
             # framework.
             else:
                 run = await self.async_client.beta.threads.runs.submit_tool_outputs(
                     **input
                 )
-            run = await self._wait_for_run(run.id, run.thread_id)
+            run = await self._await_for_run(run.id, run.thread_id)
         except BaseException as e:
             run_manager.on_chain_error(e)
             raise e
         try:
             response = self._get_response(run)
         except BaseException as e:
             run_manager.on_chain_error(e, metadata=run.dict())
```

### Comparing `langchain-0.2.0rc1/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py` & `langchain-0.2.0rc2/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/openai_functions_agent/base.py` & `langchain-0.2.0rc2/langchain/agents/openai_functions_agent/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/openai_functions_multi_agent/base.py` & `langchain-0.2.0rc2/langchain/agents/openai_functions_multi_agent/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/openai_tools/base.py` & `langchain-0.2.0rc2/langchain/agents/openai_tools/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/output_parsers/__init__.py` & `langchain-0.2.0rc2/langchain/agents/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/output_parsers/json.py` & `langchain-0.2.0rc2/langchain/agents/output_parsers/json.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/output_parsers/openai_functions.py` & `langchain-0.2.0rc2/langchain/agents/output_parsers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/output_parsers/openai_tools.py` & `langchain-0.2.0rc2/langchain/agents/output_parsers/openai_tools.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/output_parsers/react_json_single_input.py` & `langchain-0.2.0rc2/langchain/agents/output_parsers/react_json_single_input.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/output_parsers/react_single_input.py` & `langchain-0.2.0rc2/langchain/agents/output_parsers/react_single_input.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/output_parsers/self_ask.py` & `langchain-0.2.0rc2/langchain/agents/output_parsers/self_ask.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/output_parsers/tools.py` & `langchain-0.2.0rc2/langchain/agents/output_parsers/tools.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/output_parsers/xml.py` & `langchain-0.2.0rc2/langchain/agents/output_parsers/xml.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/react/agent.py` & `langchain-0.2.0rc2/langchain/agents/react/agent.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/react/base.py` & `langchain-0.2.0rc2/langchain/agents/react/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/react/output_parser.py` & `langchain-0.2.0rc2/langchain/agents/react/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/react/textworld_prompt.py` & `langchain-0.2.0rc2/langchain/agents/react/textworld_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/react/wiki_prompt.py` & `langchain-0.2.0rc2/langchain/agents/react/wiki_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/schema.py` & `langchain-0.2.0rc2/langchain/agents/schema.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/self_ask_with_search/base.py` & `langchain-0.2.0rc2/langchain/agents/self_ask_with_search/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/self_ask_with_search/prompt.py` & `langchain-0.2.0rc2/langchain/agents/self_ask_with_search/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/structured_chat/base.py` & `langchain-0.2.0rc2/langchain/agents/structured_chat/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/structured_chat/output_parser.py` & `langchain-0.2.0rc2/langchain/agents/structured_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/structured_chat/prompt.py` & `langchain-0.2.0rc2/langchain/agents/structured_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/tool_calling_agent/base.py` & `langchain-0.2.0rc2/langchain/agents/tool_calling_agent/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/tools.py` & `langchain-0.2.0rc2/langchain/agents/tools.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/types.py` & `langchain-0.2.0rc2/langchain/agents/types.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/xml/base.py` & `langchain-0.2.0rc2/langchain/agents/xml/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/agents/xml/prompt.py` & `langchain-0.2.0rc2/langchain/agents/xml/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/cache.py` & `langchain-0.2.0rc2/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/__init__.py` & `langchain-0.2.0rc2/langchain/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/aim_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/aim_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/argilla_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/argilla_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/arize_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/arize_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/arthur_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/arthur_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/base.py` & `langchain-0.2.0rc2/langchain/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/clearml_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/clearml_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/comet_ml_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/comet_ml_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/confident_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/confident_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/context_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/context_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/flyte_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/flyte_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/human.py` & `langchain-0.2.0rc2/langchain/callbacks/human.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/infino_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/infino_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/labelstudio_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/labelstudio_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/llmonitor_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/llmonitor_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/manager.py` & `langchain-0.2.0rc2/langchain/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/mlflow_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/mlflow_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/openai_info.py` & `langchain-0.2.0rc2/langchain/callbacks/openai_info.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/promptlayer_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/promptlayer_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/sagemaker_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/sagemaker_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/streaming_aiter.py` & `langchain-0.2.0rc2/langchain/callbacks/streaming_aiter.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/streaming_aiter_final_only.py` & `langchain-0.2.0rc2/langchain/callbacks/streaming_aiter_final_only.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/streaming_stdout_final_only.py` & `langchain-0.2.0rc2/langchain/callbacks/streaming_stdout_final_only.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/streamlit/__init__.py` & `langchain-0.2.0rc2/langchain/callbacks/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/streamlit/mutable_expander.py` & `langchain-0.2.0rc2/langchain/callbacks/streamlit/mutable_expander.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/streamlit/streamlit_callback_handler.py` & `langchain-0.2.0rc2/langchain/callbacks/streamlit/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/tracers/__init__.py` & `langchain-0.2.0rc2/langchain/callbacks/tracers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/tracers/comet.py` & `langchain-0.2.0rc2/langchain/callbacks/tracers/comet.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/tracers/logging.py` & `langchain-0.2.0rc2/langchain/callbacks/tracers/logging.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/tracers/wandb.py` & `langchain-0.2.0rc2/langchain/callbacks/tracers/wandb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/trubrics_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/trubrics_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/utils.py` & `langchain-0.2.0rc2/langchain/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/wandb_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/callbacks/whylabs_callback.py` & `langchain-0.2.0rc2/langchain/callbacks/whylabs_callback.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/__init__.py` & `langchain-0.2.0rc2/langchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/api/base.py` & `langchain-0.2.0rc2/langchain/chains/api/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/api/news_docs.py` & `langchain-0.2.0rc2/langchain/chains/api/news_docs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/api/open_meteo_docs.py` & `langchain-0.2.0rc2/langchain/chains/api/open_meteo_docs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/api/openapi/chain.py` & `langchain-0.2.0rc2/langchain/chains/api/openapi/chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/api/openapi/prompts.py` & `langchain-0.2.0rc2/langchain/chains/api/openapi/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/api/openapi/requests_chain.py` & `langchain-0.2.0rc2/langchain/chains/api/openapi/requests_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/api/openapi/response_chain.py` & `langchain-0.2.0rc2/langchain/chains/api/openapi/response_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/api/podcast_docs.py` & `langchain-0.2.0rc2/langchain/chains/api/podcast_docs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/api/prompt.py` & `langchain-0.2.0rc2/langchain/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/api/tmdb_docs.py` & `langchain-0.2.0rc2/langchain/chains/api/tmdb_docs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/base.py` & `langchain-0.2.0rc2/langchain/chains/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base interface that all chains should implement."""
+
 import inspect
 import json
 import logging
 import warnings
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Type, Union, cast
@@ -123,14 +124,15 @@
         **kwargs: Any,
     ) -> Dict[str, Any]:
         config = ensure_config(config)
         callbacks = config.get("callbacks")
         tags = config.get("tags")
         metadata = config.get("metadata")
         run_name = config.get("run_name") or self.get_name()
+        run_id = config.get("run_id")
         include_run_info = kwargs.get("include_run_info", False)
         return_only_outputs = kwargs.get("return_only_outputs", False)
 
         inputs = self.prep_inputs(input)
         callback_manager = CallbackManager.configure(
             callbacks,
             self.callbacks,
@@ -141,14 +143,15 @@
             self.metadata,
         )
         new_arg_supported = inspect.signature(self._call).parameters.get("run_manager")
 
         run_manager = callback_manager.on_chain_start(
             dumpd(self),
             inputs,
+            run_id,
             name=run_name,
         )
         try:
             self._validate_inputs(inputs)
             outputs = (
                 self._call(inputs, run_manager=run_manager)
                 if new_arg_supported
@@ -174,14 +177,15 @@
         **kwargs: Any,
     ) -> Dict[str, Any]:
         config = ensure_config(config)
         callbacks = config.get("callbacks")
         tags = config.get("tags")
         metadata = config.get("metadata")
         run_name = config.get("run_name") or self.get_name()
+        run_id = config.get("run_id")
         include_run_info = kwargs.get("include_run_info", False)
         return_only_outputs = kwargs.get("return_only_outputs", False)
 
         inputs = await self.aprep_inputs(input)
         callback_manager = AsyncCallbackManager.configure(
             callbacks,
             self.callbacks,
@@ -191,14 +195,15 @@
             metadata,
             self.metadata,
         )
         new_arg_supported = inspect.signature(self._acall).parameters.get("run_manager")
         run_manager = await callback_manager.on_chain_start(
             dumpd(self),
             inputs,
+            run_id,
             name=run_name,
         )
         try:
             self._validate_inputs(inputs)
             outputs = (
                 await self._acall(inputs, run_manager=run_manager)
                 if new_arg_supported
```

### Comparing `langchain-0.2.0rc1/langchain/chains/chat_vector_db/prompts.py` & `langchain-0.2.0rc2/langchain/chains/chat_vector_db/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/combine_documents/base.py` & `langchain-0.2.0rc2/langchain/chains/combine_documents/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/combine_documents/map_reduce.py` & `langchain-0.2.0rc2/langchain/chains/combine_documents/map_reduce.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/combine_documents/map_rerank.py` & `langchain-0.2.0rc2/langchain/chains/combine_documents/map_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/combine_documents/reduce.py` & `langchain-0.2.0rc2/langchain/chains/combine_documents/reduce.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/combine_documents/refine.py` & `langchain-0.2.0rc2/langchain/chains/combine_documents/refine.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/combine_documents/stuff.py` & `langchain-0.2.0rc2/langchain/chains/combine_documents/stuff.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/constitutional_ai/base.py` & `langchain-0.2.0rc2/langchain/chains/constitutional_ai/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/constitutional_ai/principles.py` & `langchain-0.2.0rc2/langchain/chains/constitutional_ai/principles.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/constitutional_ai/prompts.py` & `langchain-0.2.0rc2/langchain/chains/constitutional_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/conversation/base.py` & `langchain-0.2.0rc2/langchain/chains/conversation/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/conversation/memory.py` & `langchain-0.2.0rc2/langchain/chains/conversation/memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/conversation/prompt.py` & `langchain-0.2.0rc2/langchain/chains/conversation/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/conversational_retrieval/base.py` & `langchain-0.2.0rc2/langchain/chains/conversational_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/conversational_retrieval/prompts.py` & `langchain-0.2.0rc2/langchain/chains/conversational_retrieval/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/elasticsearch_database/base.py` & `langchain-0.2.0rc2/langchain/chains/elasticsearch_database/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/elasticsearch_database/prompts.py` & `langchain-0.2.0rc2/langchain/chains/elasticsearch_database/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/ernie_functions/__init__.py` & `langchain-0.2.0rc2/langchain/chains/ernie_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/ernie_functions/base.py` & `langchain-0.2.0rc2/langchain/chains/ernie_functions/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/example_generator.py` & `langchain-0.2.0rc2/langchain/chains/example_generator.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/flare/base.py` & `langchain-0.2.0rc2/langchain/chains/flare/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/flare/prompts.py` & `langchain-0.2.0rc2/langchain/chains/flare/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/arangodb.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/arangodb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/base.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/cypher.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/cypher.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/cypher_utils.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/cypher_utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/falkordb.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/falkordb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/gremlin.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/gremlin.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/hugegraph.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/hugegraph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/kuzu.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/kuzu.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/nebulagraph.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/nebulagraph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/neptune_cypher.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/neptune_cypher.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/neptune_sparql.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/neptune_sparql.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/ontotext_graphdb.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/ontotext_graphdb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/prompts.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/graph_qa/sparql.py` & `langchain-0.2.0rc2/langchain/chains/graph_qa/sparql.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/history_aware_retriever.py` & `langchain-0.2.0rc2/langchain/chains/history_aware_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/hyde/base.py` & `langchain-0.2.0rc2/langchain/chains/hyde/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/hyde/prompts.py` & `langchain-0.2.0rc2/langchain/chains/hyde/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/llm.py` & `langchain-0.2.0rc2/langchain/chains/llm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/llm_checker/base.py` & `langchain-0.2.0rc2/langchain/chains/llm_checker/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/llm_checker/prompt.py` & `langchain-0.2.0rc2/langchain/chains/llm_checker/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/llm_math/base.py` & `langchain-0.2.0rc2/langchain/chains/llm_math/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/llm_math/prompt.py` & `langchain-0.2.0rc2/langchain/chains/llm_math/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/llm_requests.py` & `langchain-0.2.0rc2/langchain/chains/llm_requests.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/llm_summarization_checker/base.py` & `langchain-0.2.0rc2/langchain/chains/llm_summarization_checker/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt` & `langchain-0.2.0rc2/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/loading.py` & `langchain-0.2.0rc2/langchain/chains/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/mapreduce.py` & `langchain-0.2.0rc2/langchain/chains/mapreduce.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/moderation.py` & `langchain-0.2.0rc2/langchain/chains/moderation.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/natbot/base.py` & `langchain-0.2.0rc2/langchain/chains/natbot/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/natbot/crawler.py` & `langchain-0.2.0rc2/langchain/chains/natbot/crawler.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/natbot/prompt.py` & `langchain-0.2.0rc2/langchain/chains/natbot/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/openai_functions/__init__.py` & `langchain-0.2.0rc2/langchain/chains/openai_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/openai_functions/base.py` & `langchain-0.2.0rc2/langchain/chains/openai_functions/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/openai_functions/citation_fuzzy_match.py` & `langchain-0.2.0rc2/langchain/chains/openai_functions/citation_fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/openai_functions/extraction.py` & `langchain-0.2.0rc2/langchain/chains/openai_functions/extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         "on how to do information extraction with LLMs."
         "https://python.langchain.com/docs/use_cases/extraction/."
         "If you notice other issues, please provide "
         "feedback here:"
         "https://github.com/langchain-ai/langchain/discussions/18154"
     ),
     removal="0.3.0",
-    pending=True,
     alternative=(
         """
             from langchain_core.pydantic_v1 import BaseModel, Field
             from langchain_anthropic import ChatAnthropic
     
             class Joke(BaseModel):
                 setup: str = Field(description="The setup of the joke")
@@ -126,15 +125,14 @@
         "on how to do information extraction with LLMs."
         "https://python.langchain.com/docs/use_cases/extraction/."
         "If you notice other issues, please provide "
         "feedback here:"
         "https://github.com/langchain-ai/langchain/discussions/18154"
     ),
     removal="0.3.0",
-    pending=True,
     alternative=(
         """
             from langchain_core.pydantic_v1 import BaseModel, Field
             from langchain_anthropic import ChatAnthropic
     
             class Joke(BaseModel):
                 setup: str = Field(description="The setup of the joke")
```

### Comparing `langchain-0.2.0rc1/langchain/chains/openai_functions/openapi.py` & `langchain-0.2.0rc2/langchain/chains/openai_functions/openapi.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/openai_functions/qa_with_structure.py` & `langchain-0.2.0rc2/langchain/chains/openai_functions/qa_with_structure.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/openai_functions/tagging.py` & `langchain-0.2.0rc2/langchain/chains/openai_functions/tagging.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/openai_functions/utils.py` & `langchain-0.2.0rc2/langchain/chains/openai_functions/utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/openai_tools/extraction.py` & `langchain-0.2.0rc2/langchain/chains/openai_tools/extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         "https://python.langchain.com/docs/use_cases/extraction/."
         "with_structured_output does not currently support a list of pydantic schemas. "
         "If this is a blocker or if you notice other issues, please provide "
         "feedback here:"
         "https://github.com/langchain-ai/langchain/discussions/18154"
     ),
     removal="0.3.0",
-    pending=True,
     alternative=(
         """
             from langchain_core.pydantic_v1 import BaseModel, Field
             from langchain_anthropic import ChatAnthropic
     
             class Joke(BaseModel):
                 setup: str = Field(description="The setup of the joke")
```

### Comparing `langchain-0.2.0rc1/langchain/chains/prompt_selector.py` & `langchain-0.2.0rc2/langchain/chains/prompt_selector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/qa_generation/base.py` & `langchain-0.2.0rc2/langchain/chains/qa_generation/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/qa_generation/prompt.py` & `langchain-0.2.0rc2/langchain/chains/qa_generation/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/qa_with_sources/base.py` & `langchain-0.2.0rc2/langchain/chains/qa_with_sources/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/qa_with_sources/loading.py` & `langchain-0.2.0rc2/langchain/chains/qa_with_sources/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/qa_with_sources/map_reduce_prompt.py` & `langchain-0.2.0rc2/langchain/chains/qa_with_sources/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/qa_with_sources/refine_prompts.py` & `langchain-0.2.0rc2/langchain/chains/qa_with_sources/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/qa_with_sources/retrieval.py` & `langchain-0.2.0rc2/langchain/chains/qa_with_sources/retrieval.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/qa_with_sources/stuff_prompt.py` & `langchain-0.2.0rc2/langchain/chains/qa_with_sources/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/qa_with_sources/vector_db.py` & `langchain-0.2.0rc2/langchain/chains/qa_with_sources/vector_db.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/query_constructor/base.py` & `langchain-0.2.0rc2/langchain/chains/query_constructor/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/query_constructor/parser.py` & `langchain-0.2.0rc2/langchain/chains/query_constructor/parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/query_constructor/prompt.py` & `langchain-0.2.0rc2/langchain/chains/query_constructor/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/question_answering/__init__.py` & `langchain-0.2.0rc2/langchain/chains/question_answering/chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/question_answering/map_reduce_prompt.py` & `langchain-0.2.0rc2/langchain/chains/question_answering/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/question_answering/map_rerank_prompt.py` & `langchain-0.2.0rc2/langchain/chains/question_answering/map_rerank_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/question_answering/refine_prompts.py` & `langchain-0.2.0rc2/langchain/chains/question_answering/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/question_answering/stuff_prompt.py` & `langchain-0.2.0rc2/langchain/chains/question_answering/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/retrieval.py` & `langchain-0.2.0rc2/langchain/chains/retrieval.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/retrieval_qa/base.py` & `langchain-0.2.0rc2/langchain/chains/retrieval_qa/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/router/base.py` & `langchain-0.2.0rc2/langchain/chains/router/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/router/embedding_router.py` & `langchain-0.2.0rc2/langchain/chains/router/embedding_router.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/router/llm_router.py` & `langchain-0.2.0rc2/langchain/chains/router/llm_router.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/router/multi_prompt.py` & `langchain-0.2.0rc2/langchain/chains/router/multi_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/router/multi_prompt_prompt.py` & `langchain-0.2.0rc2/langchain/chains/router/multi_prompt_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/router/multi_retrieval_prompt.py` & `langchain-0.2.0rc2/langchain/chains/router/multi_retrieval_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/router/multi_retrieval_qa.py` & `langchain-0.2.0rc2/langchain/chains/router/multi_retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/sequential.py` & `langchain-0.2.0rc2/langchain/chains/sequential.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/sql_database/prompt.py` & `langchain-0.2.0rc2/langchain/chains/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/sql_database/query.py` & `langchain-0.2.0rc2/langchain/chains/sql_database/query.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/structured_output/base.py` & `langchain-0.2.0rc2/langchain/chains/structured_output/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         "on how to do information extraction with LLMs. "
         "https://python.langchain.com/docs/use_cases/extraction/. "
         "If you notice other issues, please provide "
         "feedback here: "
         "https://github.com/langchain-ai/langchain/discussions/18154"
     ),
     removal="0.3.0",
-    pending=True,
     alternative=(
         """
             from langchain_core.pydantic_v1 import BaseModel, Field
             from langchain_anthropic import ChatAnthropic
     
             class Joke(BaseModel):
                 setup: str = Field(description="The setup of the joke")
@@ -156,15 +155,14 @@
         "on how to do information extraction with LLMs. "
         "https://python.langchain.com/docs/use_cases/extraction/. "
         "If you notice other issues, please provide "
         "feedback here: "
         "https://github.com/langchain-ai/langchain/discussions/18154"
     ),
     removal="0.3.0",
-    pending=True,
     alternative=(
         """
             from langchain_core.pydantic_v1 import BaseModel, Field
             from langchain_anthropic import ChatAnthropic
 
             class Joke(BaseModel):
                 setup: str = Field(description="The setup of the joke")
```

### Comparing `langchain-0.2.0rc1/langchain/chains/summarize/chain.py` & `langchain-0.2.0rc2/langchain/chains/summarize/chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/summarize/refine_prompts.py` & `langchain-0.2.0rc2/langchain/chains/summarize/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chains/transform.py` & `langchain-0.2.0rc2/langchain/chains/transform.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_loaders/facebook_messenger.py` & `langchain-0.2.0rc2/langchain/chat_loaders/facebook_messenger.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_loaders/gmail.py` & `langchain-0.2.0rc2/langchain/chat_loaders/gmail.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_loaders/imessage.py` & `langchain-0.2.0rc2/langchain/chat_loaders/imessage.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_loaders/langsmith.py` & `langchain-0.2.0rc2/langchain/chat_loaders/langsmith.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_loaders/slack.py` & `langchain-0.2.0rc2/langchain/chat_loaders/slack.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_loaders/telegram.py` & `langchain-0.2.0rc2/langchain/chat_loaders/telegram.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_loaders/utils.py` & `langchain-0.2.0rc2/langchain/chat_loaders/utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_loaders/whatsapp.py` & `langchain-0.2.0rc2/langchain/chat_loaders/whatsapp.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/__init__.py` & `langchain-0.2.0rc2/langchain/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/anthropic.py` & `langchain-0.2.0rc2/langchain/chat_models/anthropic.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/anyscale.py` & `langchain-0.2.0rc2/langchain/chat_models/anyscale.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/azure_openai.py` & `langchain-0.2.0rc2/langchain/chat_models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/azureml_endpoint.py` & `langchain-0.2.0rc2/langchain/chat_models/azureml_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/baichuan.py` & `langchain-0.2.0rc2/langchain/chat_models/baichuan.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/baidu_qianfan_endpoint.py` & `langchain-0.2.0rc2/langchain/chat_models/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/bedrock.py` & `langchain-0.2.0rc2/langchain/chat_models/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/cohere.py` & `langchain-0.2.0rc2/langchain/chat_models/cohere.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/databricks.py` & `langchain-0.2.0rc2/langchain/chat_models/databricks.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/ernie.py` & `langchain-0.2.0rc2/langchain/chat_models/ernie.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/everlyai.py` & `langchain-0.2.0rc2/langchain/chat_models/everlyai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/fake.py` & `langchain-0.2.0rc2/langchain/chat_models/fake.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/fireworks.py` & `langchain-0.2.0rc2/langchain/chat_models/fireworks.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/gigachat.py` & `langchain-0.2.0rc2/langchain/chat_models/gigachat.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/google_palm.py` & `langchain-0.2.0rc2/langchain/chat_models/google_palm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/human.py` & `langchain-0.2.0rc2/langchain/chat_models/human.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/hunyuan.py` & `langchain-0.2.0rc2/langchain/chat_models/hunyuan.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/javelin_ai_gateway.py` & `langchain-0.2.0rc2/langchain/chat_models/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/jinachat.py` & `langchain-0.2.0rc2/langchain/chat_models/jinachat.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/konko.py` & `langchain-0.2.0rc2/langchain/chat_models/konko.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/litellm.py` & `langchain-0.2.0rc2/langchain/chat_models/litellm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/meta.py` & `langchain-0.2.0rc2/langchain/chat_models/meta.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/minimax.py` & `langchain-0.2.0rc2/langchain/chat_models/minimax.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/mlflow.py` & `langchain-0.2.0rc2/langchain/chat_models/mlflow.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/mlflow_ai_gateway.py` & `langchain-0.2.0rc2/langchain/chat_models/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/ollama.py` & `langchain-0.2.0rc2/langchain/chat_models/ollama.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/openai.py` & `langchain-0.2.0rc2/langchain/chat_models/openai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/pai_eas_endpoint.py` & `langchain-0.2.0rc2/langchain/chat_models/pai_eas_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/promptlayer_openai.py` & `langchain-0.2.0rc2/langchain/chat_models/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/tongyi.py` & `langchain-0.2.0rc2/langchain/chat_models/tongyi.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/vertexai.py` & `langchain-0.2.0rc2/langchain/chat_models/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/volcengine_maas.py` & `langchain-0.2.0rc2/langchain/chat_models/volcengine_maas.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/chat_models/yandex.py` & `langchain-0.2.0rc2/langchain/chat_models/yandex.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/docstore/__init__.py` & `langchain-0.2.0rc2/langchain/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/docstore/arbitrary_fn.py` & `langchain-0.2.0rc2/langchain/docstore/arbitrary_fn.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/docstore/base.py` & `langchain-0.2.0rc2/langchain/docstore/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/docstore/in_memory.py` & `langchain-0.2.0rc2/langchain/docstore/in_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/docstore/wikipedia.py` & `langchain-0.2.0rc2/langchain/docstore/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/__init__.py` & `langchain-0.2.0rc2/langchain/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/acreom.py` & `langchain-0.2.0rc2/langchain/document_loaders/acreom.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/airbyte.py` & `langchain-0.2.0rc2/langchain/document_loaders/airbyte.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/airbyte_json.py` & `langchain-0.2.0rc2/langchain/document_loaders/airbyte_json.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/airtable.py` & `langchain-0.2.0rc2/langchain/document_loaders/airtable.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/apify_dataset.py` & `langchain-0.2.0rc2/langchain/document_loaders/apify_dataset.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/arcgis_loader.py` & `langchain-0.2.0rc2/langchain/document_loaders/arcgis_loader.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/arxiv.py` & `langchain-0.2.0rc2/langchain/document_loaders/arxiv.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/assemblyai.py` & `langchain-0.2.0rc2/langchain/document_loaders/assemblyai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/async_html.py` & `langchain-0.2.0rc2/langchain/document_loaders/async_html.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/azlyrics.py` & `langchain-0.2.0rc2/langchain/document_loaders/azlyrics.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/azure_ai_data.py` & `langchain-0.2.0rc2/langchain/document_loaders/azure_ai_data.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/azure_blob_storage_container.py` & `langchain-0.2.0rc2/langchain/document_loaders/azure_blob_storage_container.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/azure_blob_storage_file.py` & `langchain-0.2.0rc2/langchain/document_loaders/azure_blob_storage_file.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/baiducloud_bos_directory.py` & `langchain-0.2.0rc2/langchain/document_loaders/baiducloud_bos_directory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/baiducloud_bos_file.py` & `langchain-0.2.0rc2/langchain/document_loaders/baiducloud_bos_file.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/base_o365.py` & `langchain-0.2.0rc2/langchain/document_loaders/base_o365.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/bibtex.py` & `langchain-0.2.0rc2/langchain/document_loaders/bibtex.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/bigquery.py` & `langchain-0.2.0rc2/langchain/document_loaders/bigquery.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/bilibili.py` & `langchain-0.2.0rc2/langchain/document_loaders/bilibili.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/blackboard.py` & `langchain-0.2.0rc2/langchain/document_loaders/blackboard.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/blob_loaders/__init__.py` & `langchain-0.2.0rc2/langchain/document_loaders/blob_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/blob_loaders/file_system.py` & `langchain-0.2.0rc2/langchain/document_loaders/blob_loaders/file_system.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/blob_loaders/schema.py` & `langchain-0.2.0rc2/langchain/document_loaders/blob_loaders/schema.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/blob_loaders/youtube_audio.py` & `langchain-0.2.0rc2/langchain/document_loaders/blob_loaders/youtube_audio.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/blockchain.py` & `langchain-0.2.0rc2/langchain/document_loaders/blockchain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/brave_search.py` & `langchain-0.2.0rc2/langchain/document_loaders/brave_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/browserless.py` & `langchain-0.2.0rc2/langchain/document_loaders/browserless.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/chatgpt.py` & `langchain-0.2.0rc2/langchain/document_loaders/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/chromium.py` & `langchain-0.2.0rc2/langchain/document_loaders/chromium.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/college_confidential.py` & `langchain-0.2.0rc2/langchain/document_loaders/college_confidential.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/concurrent.py` & `langchain-0.2.0rc2/langchain/document_loaders/concurrent.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/confluence.py` & `langchain-0.2.0rc2/langchain/document_loaders/confluence.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/conllu.py` & `langchain-0.2.0rc2/langchain/document_loaders/conllu.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/couchbase.py` & `langchain-0.2.0rc2/langchain/document_loaders/couchbase.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/csv_loader.py` & `langchain-0.2.0rc2/langchain/document_loaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/cube_semantic.py` & `langchain-0.2.0rc2/langchain/document_loaders/cube_semantic.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/datadog_logs.py` & `langchain-0.2.0rc2/langchain/document_loaders/datadog_logs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/dataframe.py` & `langchain-0.2.0rc2/langchain/document_loaders/dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/diffbot.py` & `langchain-0.2.0rc2/langchain/document_loaders/diffbot.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/directory.py` & `langchain-0.2.0rc2/langchain/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/discord.py` & `langchain-0.2.0rc2/langchain/document_loaders/discord.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/docugami.py` & `langchain-0.2.0rc2/langchain/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/docusaurus.py` & `langchain-0.2.0rc2/langchain/document_loaders/docusaurus.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/dropbox.py` & `langchain-0.2.0rc2/langchain/document_loaders/dropbox.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/duckdb_loader.py` & `langchain-0.2.0rc2/langchain/document_loaders/duckdb_loader.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/email.py` & `langchain-0.2.0rc2/langchain/document_loaders/email.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/epub.py` & `langchain-0.2.0rc2/langchain/document_loaders/epub.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/etherscan.py` & `langchain-0.2.0rc2/langchain/document_loaders/etherscan.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/evernote.py` & `langchain-0.2.0rc2/langchain/document_loaders/evernote.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/excel.py` & `langchain-0.2.0rc2/langchain/document_loaders/excel.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/facebook_chat.py` & `langchain-0.2.0rc2/langchain/document_loaders/facebook_chat.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/fauna.py` & `langchain-0.2.0rc2/langchain/document_loaders/fauna.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/figma.py` & `langchain-0.2.0rc2/langchain/document_loaders/figma.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/gcs_directory.py` & `langchain-0.2.0rc2/langchain/document_loaders/gcs_directory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/gcs_file.py` & `langchain-0.2.0rc2/langchain/document_loaders/gcs_file.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/generic.py` & `langchain-0.2.0rc2/langchain/document_loaders/generic.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/geodataframe.py` & `langchain-0.2.0rc2/langchain/document_loaders/geodataframe.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/git.py` & `langchain-0.2.0rc2/langchain/document_loaders/git.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/gitbook.py` & `langchain-0.2.0rc2/langchain/document_loaders/gitbook.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/github.py` & `langchain-0.2.0rc2/langchain/document_loaders/github.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/google_speech_to_text.py` & `langchain-0.2.0rc2/langchain/document_loaders/google_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/googledrive.py` & `langchain-0.2.0rc2/langchain/document_loaders/googledrive.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/gutenberg.py` & `langchain-0.2.0rc2/langchain/document_loaders/gutenberg.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/helpers.py` & `langchain-0.2.0rc2/langchain/document_loaders/helpers.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/hn.py` & `langchain-0.2.0rc2/langchain/document_loaders/hn.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/html.py` & `langchain-0.2.0rc2/langchain/document_loaders/html.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/html_bs.py` & `langchain-0.2.0rc2/langchain/document_loaders/html_bs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/hugging_face_dataset.py` & `langchain-0.2.0rc2/langchain/document_loaders/hugging_face_dataset.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/ifixit.py` & `langchain-0.2.0rc2/langchain/document_loaders/ifixit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/image.py` & `langchain-0.2.0rc2/langchain/document_loaders/image.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/image_captions.py` & `langchain-0.2.0rc2/langchain/document_loaders/image_captions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/imsdb.py` & `langchain-0.2.0rc2/langchain/document_loaders/imsdb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/iugu.py` & `langchain-0.2.0rc2/langchain/document_loaders/iugu.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/joplin.py` & `langchain-0.2.0rc2/langchain/document_loaders/joplin.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/json_loader.py` & `langchain-0.2.0rc2/langchain/document_loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/lakefs.py` & `langchain-0.2.0rc2/langchain/document_loaders/lakefs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/larksuite.py` & `langchain-0.2.0rc2/langchain/document_loaders/larksuite.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/markdown.py` & `langchain-0.2.0rc2/langchain/document_loaders/markdown.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/mastodon.py` & `langchain-0.2.0rc2/langchain/document_loaders/mastodon.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/max_compute.py` & `langchain-0.2.0rc2/langchain/document_loaders/max_compute.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/mediawikidump.py` & `langchain-0.2.0rc2/langchain/document_loaders/mediawikidump.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/merge.py` & `langchain-0.2.0rc2/langchain/document_loaders/merge.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/mhtml.py` & `langchain-0.2.0rc2/langchain/document_loaders/mhtml.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/modern_treasury.py` & `langchain-0.2.0rc2/langchain/document_loaders/modern_treasury.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/mongodb.py` & `langchain-0.2.0rc2/langchain/document_loaders/mongodb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/news.py` & `langchain-0.2.0rc2/langchain/document_loaders/news.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/notebook.py` & `langchain-0.2.0rc2/langchain/document_loaders/notebook.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/notion.py` & `langchain-0.2.0rc2/langchain/document_loaders/notion.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/notiondb.py` & `langchain-0.2.0rc2/langchain/document_loaders/notiondb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/nuclia.py` & `langchain-0.2.0rc2/langchain/document_loaders/nuclia.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/obs_directory.py` & `langchain-0.2.0rc2/langchain/document_loaders/obs_directory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/obs_file.py` & `langchain-0.2.0rc2/langchain/document_loaders/obs_file.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/obsidian.py` & `langchain-0.2.0rc2/langchain/document_loaders/obsidian.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/odt.py` & `langchain-0.2.0rc2/langchain/document_loaders/odt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/onedrive.py` & `langchain-0.2.0rc2/langchain/document_loaders/onedrive.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/onedrive_file.py` & `langchain-0.2.0rc2/langchain/document_loaders/onedrive_file.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/onenote.py` & `langchain-0.2.0rc2/langchain/document_loaders/onenote.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/open_city_data.py` & `langchain-0.2.0rc2/langchain/document_loaders/open_city_data.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/org_mode.py` & `langchain-0.2.0rc2/langchain/document_loaders/org_mode.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/__init__.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/audio.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/docai.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/docai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/generic.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/grobid.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/grobid.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/html/__init__.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/html/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/html/bs4.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/html/bs4.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/language/__init__.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/language/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/language/cobol.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/language/cobol.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/language/code_segmenter.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/language/code_segmenter.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/language/javascript.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/language/javascript.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/language/language_parser.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/language/language_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/language/python.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/language/python.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/msword.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/msword.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/pdf.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/pdf.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/registry.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/registry.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/parsers/txt.py` & `langchain-0.2.0rc2/langchain/document_loaders/parsers/txt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/pdf.py` & `langchain-0.2.0rc2/langchain/document_loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/polars_dataframe.py` & `langchain-0.2.0rc2/langchain/document_loaders/polars_dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/powerpoint.py` & `langchain-0.2.0rc2/langchain/document_loaders/powerpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/psychic.py` & `langchain-0.2.0rc2/langchain/document_loaders/psychic.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/pubmed.py` & `langchain-0.2.0rc2/langchain/document_loaders/pubmed.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/pyspark_dataframe.py` & `langchain-0.2.0rc2/langchain/document_loaders/pyspark_dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/python.py` & `langchain-0.2.0rc2/langchain/document_loaders/python.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/quip.py` & `langchain-0.2.0rc2/langchain/document_loaders/quip.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/readthedocs.py` & `langchain-0.2.0rc2/langchain/document_loaders/readthedocs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/recursive_url_loader.py` & `langchain-0.2.0rc2/langchain/document_loaders/recursive_url_loader.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/reddit.py` & `langchain-0.2.0rc2/langchain/document_loaders/reddit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/roam.py` & `langchain-0.2.0rc2/langchain/document_loaders/roam.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/rocksetdb.py` & `langchain-0.2.0rc2/langchain/document_loaders/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/rspace.py` & `langchain-0.2.0rc2/langchain/document_loaders/rspace.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/rss.py` & `langchain-0.2.0rc2/langchain/document_loaders/rss.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/rst.py` & `langchain-0.2.0rc2/langchain/document_loaders/rst.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/rtf.py` & `langchain-0.2.0rc2/langchain/document_loaders/rtf.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/s3_directory.py` & `langchain-0.2.0rc2/langchain/document_loaders/s3_directory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/s3_file.py` & `langchain-0.2.0rc2/langchain/document_loaders/s3_file.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/sharepoint.py` & `langchain-0.2.0rc2/langchain/document_loaders/sharepoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/sitemap.py` & `langchain-0.2.0rc2/langchain/document_loaders/sitemap.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/slack_directory.py` & `langchain-0.2.0rc2/langchain/document_loaders/slack_directory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/snowflake_loader.py` & `langchain-0.2.0rc2/langchain/document_loaders/snowflake_loader.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/spreedly.py` & `langchain-0.2.0rc2/langchain/document_loaders/spreedly.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/srt.py` & `langchain-0.2.0rc2/langchain/document_loaders/srt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/stripe.py` & `langchain-0.2.0rc2/langchain/document_loaders/stripe.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/telegram.py` & `langchain-0.2.0rc2/langchain/document_loaders/telegram.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/tencent_cos_directory.py` & `langchain-0.2.0rc2/langchain/document_loaders/tencent_cos_directory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/tencent_cos_file.py` & `langchain-0.2.0rc2/langchain/document_loaders/tencent_cos_file.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/tensorflow_datasets.py` & `langchain-0.2.0rc2/langchain/document_loaders/tensorflow_datasets.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/text.py` & `langchain-0.2.0rc2/langchain/document_loaders/text.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/tomarkdown.py` & `langchain-0.2.0rc2/langchain/document_loaders/tomarkdown.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/toml.py` & `langchain-0.2.0rc2/langchain/document_loaders/toml.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/trello.py` & `langchain-0.2.0rc2/langchain/document_loaders/trello.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/tsv.py` & `langchain-0.2.0rc2/langchain/document_loaders/tsv.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/twitter.py` & `langchain-0.2.0rc2/langchain/document_loaders/twitter.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/unstructured.py` & `langchain-0.2.0rc2/langchain/document_loaders/unstructured.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/url.py` & `langchain-0.2.0rc2/langchain/document_loaders/url.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/url_playwright.py` & `langchain-0.2.0rc2/langchain/document_loaders/url_playwright.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/url_selenium.py` & `langchain-0.2.0rc2/langchain/document_loaders/url_selenium.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/weather.py` & `langchain-0.2.0rc2/langchain/document_loaders/weather.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/web_base.py` & `langchain-0.2.0rc2/langchain/document_loaders/web_base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/whatsapp_chat.py` & `langchain-0.2.0rc2/langchain/document_loaders/whatsapp_chat.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/wikipedia.py` & `langchain-0.2.0rc2/langchain/document_loaders/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/word_document.py` & `langchain-0.2.0rc2/langchain/document_loaders/word_document.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/xml.py` & `langchain-0.2.0rc2/langchain/document_loaders/xml.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/xorbits.py` & `langchain-0.2.0rc2/langchain/document_loaders/xorbits.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_loaders/youtube.py` & `langchain-0.2.0rc2/langchain/document_loaders/youtube.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/__init__.py` & `langchain-0.2.0rc2/langchain/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/beautiful_soup_transformer.py` & `langchain-0.2.0rc2/langchain/document_transformers/beautiful_soup_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/doctran_text_extract.py` & `langchain-0.2.0rc2/langchain/document_transformers/doctran_text_extract.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/doctran_text_qa.py` & `langchain-0.2.0rc2/langchain/document_transformers/doctran_text_qa.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/doctran_text_translate.py` & `langchain-0.2.0rc2/langchain/document_transformers/doctran_text_translate.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/embeddings_redundant_filter.py` & `langchain-0.2.0rc2/langchain/document_transformers/embeddings_redundant_filter.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/google_translate.py` & `langchain-0.2.0rc2/langchain/document_transformers/google_translate.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/html2text.py` & `langchain-0.2.0rc2/langchain/document_transformers/html2text.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/long_context_reorder.py` & `langchain-0.2.0rc2/langchain/document_transformers/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/nuclia_text_transform.py` & `langchain-0.2.0rc2/langchain/document_transformers/nuclia_text_transform.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/openai_functions.py` & `langchain-0.2.0rc2/langchain/document_transformers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/document_transformers/xsl/html_chunks_with_headers.xslt` & `langchain-0.2.0rc2/langchain/document_transformers/xsl/html_chunks_with_headers.xslt`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/__init__.py` & `langchain-0.2.0rc2/langchain/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/aleph_alpha.py` & `langchain-0.2.0rc2/langchain/embeddings/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/awa.py` & `langchain-0.2.0rc2/langchain/embeddings/awa.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/azure_openai.py` & `langchain-0.2.0rc2/langchain/embeddings/azure_openai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/baidu_qianfan_endpoint.py` & `langchain-0.2.0rc2/langchain/embeddings/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/bedrock.py` & `langchain-0.2.0rc2/langchain/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/bookend.py` & `langchain-0.2.0rc2/langchain/embeddings/bookend.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/cache.py` & `langchain-0.2.0rc2/langchain/embeddings/cache.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/clarifai.py` & `langchain-0.2.0rc2/langchain/embeddings/clarifai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/cloudflare_workersai.py` & `langchain-0.2.0rc2/langchain/embeddings/cloudflare_workersai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/cohere.py` & `langchain-0.2.0rc2/langchain/embeddings/cohere.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/dashscope.py` & `langchain-0.2.0rc2/langchain/embeddings/dashscope.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/databricks.py` & `langchain-0.2.0rc2/langchain/embeddings/databricks.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/deepinfra.py` & `langchain-0.2.0rc2/langchain/embeddings/deepinfra.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/edenai.py` & `langchain-0.2.0rc2/langchain/embeddings/edenai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/elasticsearch.py` & `langchain-0.2.0rc2/langchain/embeddings/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/embaas.py` & `langchain-0.2.0rc2/langchain/embeddings/embaas.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/ernie.py` & `langchain-0.2.0rc2/langchain/embeddings/ernie.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/fake.py` & `langchain-0.2.0rc2/langchain/embeddings/fake.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/fastembed.py` & `langchain-0.2.0rc2/langchain/embeddings/fastembed.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/google_palm.py` & `langchain-0.2.0rc2/langchain/embeddings/google_palm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/gpt4all.py` & `langchain-0.2.0rc2/langchain/embeddings/gpt4all.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/gradient_ai.py` & `langchain-0.2.0rc2/langchain/embeddings/gradient_ai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/huggingface.py` & `langchain-0.2.0rc2/langchain/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/huggingface_hub.py` & `langchain-0.2.0rc2/langchain/embeddings/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/infinity.py` & `langchain-0.2.0rc2/langchain/embeddings/infinity.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/javelin_ai_gateway.py` & `langchain-0.2.0rc2/langchain/embeddings/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/jina.py` & `langchain-0.2.0rc2/langchain/embeddings/jina.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/johnsnowlabs.py` & `langchain-0.2.0rc2/langchain/embeddings/johnsnowlabs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/llamacpp.py` & `langchain-0.2.0rc2/langchain/embeddings/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/llm_rails.py` & `langchain-0.2.0rc2/langchain/embeddings/llm_rails.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/localai.py` & `langchain-0.2.0rc2/langchain/embeddings/localai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/minimax.py` & `langchain-0.2.0rc2/langchain/embeddings/minimax.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/mlflow.py` & `langchain-0.2.0rc2/langchain/embeddings/mlflow.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/mlflow_gateway.py` & `langchain-0.2.0rc2/langchain/embeddings/mlflow_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/modelscope_hub.py` & `langchain-0.2.0rc2/langchain/embeddings/modelscope_hub.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/mosaicml.py` & `langchain-0.2.0rc2/langchain/embeddings/mosaicml.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/nlpcloud.py` & `langchain-0.2.0rc2/langchain/embeddings/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/octoai_embeddings.py` & `langchain-0.2.0rc2/langchain/embeddings/octoai_embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/ollama.py` & `langchain-0.2.0rc2/langchain/embeddings/ollama.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/openai.py` & `langchain-0.2.0rc2/langchain/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/sagemaker_endpoint.py` & `langchain-0.2.0rc2/langchain/embeddings/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/self_hosted.py` & `langchain-0.2.0rc2/langchain/embeddings/self_hosted.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/self_hosted_hugging_face.py` & `langchain-0.2.0rc2/langchain/embeddings/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/sentence_transformer.py` & `langchain-0.2.0rc2/langchain/embeddings/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/spacy_embeddings.py` & `langchain-0.2.0rc2/langchain/embeddings/spacy_embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/tensorflow_hub.py` & `langchain-0.2.0rc2/langchain/embeddings/tensorflow_hub.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/vertexai.py` & `langchain-0.2.0rc2/langchain/embeddings/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/voyageai.py` & `langchain-0.2.0rc2/langchain/embeddings/voyageai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/embeddings/xinference.py` & `langchain-0.2.0rc2/langchain/embeddings/xinference.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/__init__.py` & `langchain-0.2.0rc2/langchain/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/agents/trajectory_eval_chain.py` & `langchain-0.2.0rc2/langchain/evaluation/agents/trajectory_eval_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/agents/trajectory_eval_prompt.py` & `langchain-0.2.0rc2/langchain/evaluation/agents/trajectory_eval_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/comparison/__init__.py` & `langchain-0.2.0rc2/langchain/evaluation/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/comparison/eval_chain.py` & `langchain-0.2.0rc2/langchain/evaluation/comparison/eval_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/comparison/prompt.py` & `langchain-0.2.0rc2/langchain/evaluation/comparison/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/criteria/__init__.py` & `langchain-0.2.0rc2/langchain/evaluation/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/criteria/eval_chain.py` & `langchain-0.2.0rc2/langchain/evaluation/criteria/eval_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/criteria/prompt.py` & `langchain-0.2.0rc2/langchain/evaluation/criteria/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/embedding_distance/base.py` & `langchain-0.2.0rc2/langchain/evaluation/embedding_distance/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/exact_match/base.py` & `langchain-0.2.0rc2/langchain/evaluation/exact_match/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/loading.py` & `langchain-0.2.0rc2/langchain/evaluation/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/parsing/base.py` & `langchain-0.2.0rc2/langchain/evaluation/parsing/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/parsing/json_distance.py` & `langchain-0.2.0rc2/langchain/evaluation/parsing/json_distance.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/parsing/json_schema.py` & `langchain-0.2.0rc2/langchain/evaluation/parsing/json_schema.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/qa/eval_chain.py` & `langchain-0.2.0rc2/langchain/evaluation/qa/eval_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/qa/eval_prompt.py` & `langchain-0.2.0rc2/langchain/evaluation/qa/eval_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/qa/generate_chain.py` & `langchain-0.2.0rc2/langchain/evaluation/qa/generate_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/qa/generate_prompt.py` & `langchain-0.2.0rc2/langchain/evaluation/qa/generate_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/regex_match/base.py` & `langchain-0.2.0rc2/langchain/evaluation/regex_match/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/schema.py` & `langchain-0.2.0rc2/langchain/evaluation/schema.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/scoring/__init__.py` & `langchain-0.2.0rc2/langchain/evaluation/scoring/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/scoring/eval_chain.py` & `langchain-0.2.0rc2/langchain/evaluation/scoring/eval_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/scoring/prompt.py` & `langchain-0.2.0rc2/langchain/evaluation/scoring/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/evaluation/string_distance/base.py` & `langchain-0.2.0rc2/langchain/evaluation/string_distance/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/globals/__init__.py` & `langchain-0.2.0rc2/langchain/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/__init__.py` & `langchain-0.2.0rc2/langchain/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/arangodb_graph.py` & `langchain-0.2.0rc2/langchain/graphs/arangodb_graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/falkordb_graph.py` & `langchain-0.2.0rc2/langchain/graphs/falkordb_graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/graph_document.py` & `langchain-0.2.0rc2/langchain/graphs/graph_document.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/graph_store.py` & `langchain-0.2.0rc2/langchain/graphs/graph_store.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/hugegraph.py` & `langchain-0.2.0rc2/langchain/graphs/hugegraph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/kuzu_graph.py` & `langchain-0.2.0rc2/langchain/graphs/kuzu_graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/memgraph_graph.py` & `langchain-0.2.0rc2/langchain/graphs/memgraph_graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/nebula_graph.py` & `langchain-0.2.0rc2/langchain/graphs/nebula_graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/neo4j_graph.py` & `langchain-0.2.0rc2/langchain/graphs/neo4j_graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/neptune_graph.py` & `langchain-0.2.0rc2/langchain/graphs/neptune_graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/networkx_graph.py` & `langchain-0.2.0rc2/langchain/graphs/networkx_graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/graphs/rdf_graph.py` & `langchain-0.2.0rc2/langchain/graphs/rdf_graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/hub.py` & `langchain-0.2.0rc2/langchain/hub.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/indexes/__init__.py` & `langchain-0.2.0rc2/langchain/indexes/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/indexes/_sql_record_manager.py` & `langchain-0.2.0rc2/langchain/indexes/_sql_record_manager.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/indexes/graph.py` & `langchain-0.2.0rc2/langchain/indexes/graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/indexes/prompts/entity_extraction.py` & `langchain-0.2.0rc2/langchain/indexes/prompts/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/indexes/prompts/entity_summarization.py` & `langchain-0.2.0rc2/langchain/indexes/prompts/entity_summarization.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/indexes/prompts/knowledge_triplet_extraction.py` & `langchain-0.2.0rc2/langchain/indexes/prompts/knowledge_triplet_extraction.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/indexes/vectorstore.py` & `langchain-0.2.0rc2/langchain/indexes/vectorstore.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/__init__.py` & `langchain-0.2.0rc2/langchain/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/ai21.py` & `langchain-0.2.0rc2/langchain/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/aleph_alpha.py` & `langchain-0.2.0rc2/langchain/llms/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/amazon_api_gateway.py` & `langchain-0.2.0rc2/langchain/llms/amazon_api_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/anthropic.py` & `langchain-0.2.0rc2/langchain/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/anyscale.py` & `langchain-0.2.0rc2/langchain/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/arcee.py` & `langchain-0.2.0rc2/langchain/llms/arcee.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/aviary.py` & `langchain-0.2.0rc2/langchain/llms/aviary.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/azureml_endpoint.py` & `langchain-0.2.0rc2/langchain/llms/azureml_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/baidu_qianfan_endpoint.py` & `langchain-0.2.0rc2/langchain/llms/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/bananadev.py` & `langchain-0.2.0rc2/langchain/llms/bananadev.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/baseten.py` & `langchain-0.2.0rc2/langchain/llms/baseten.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/beam.py` & `langchain-0.2.0rc2/langchain/llms/beam.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/bedrock.py` & `langchain-0.2.0rc2/langchain/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/bittensor.py` & `langchain-0.2.0rc2/langchain/llms/bittensor.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/cerebriumai.py` & `langchain-0.2.0rc2/langchain/llms/cerebriumai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/chatglm.py` & `langchain-0.2.0rc2/langchain/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/clarifai.py` & `langchain-0.2.0rc2/langchain/llms/clarifai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/cloudflare_workersai.py` & `langchain-0.2.0rc2/langchain/llms/cloudflare_workersai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/cohere.py` & `langchain-0.2.0rc2/langchain/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/ctransformers.py` & `langchain-0.2.0rc2/langchain/llms/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/ctranslate2.py` & `langchain-0.2.0rc2/langchain/llms/ctranslate2.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/databricks.py` & `langchain-0.2.0rc2/langchain/llms/databricks.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/deepinfra.py` & `langchain-0.2.0rc2/langchain/llms/deepinfra.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/deepsparse.py` & `langchain-0.2.0rc2/langchain/llms/deepsparse.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/edenai.py` & `langchain-0.2.0rc2/langchain/llms/edenai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/fake.py` & `langchain-0.2.0rc2/langchain/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/fireworks.py` & `langchain-0.2.0rc2/langchain/llms/fireworks.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/forefrontai.py` & `langchain-0.2.0rc2/langchain/llms/forefrontai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/gigachat.py` & `langchain-0.2.0rc2/langchain/llms/gigachat.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/google_palm.py` & `langchain-0.2.0rc2/langchain/llms/google_palm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/gooseai.py` & `langchain-0.2.0rc2/langchain/llms/gooseai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/gpt4all.py` & `langchain-0.2.0rc2/langchain/llms/gpt4all.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/gradient_ai.py` & `langchain-0.2.0rc2/langchain/llms/gradient_ai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/grammars/json.gbnf` & `langchain-0.2.0rc2/langchain/llms/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/huggingface_endpoint.py` & `langchain-0.2.0rc2/langchain/llms/huggingface_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/huggingface_hub.py` & `langchain-0.2.0rc2/langchain/llms/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/huggingface_pipeline.py` & `langchain-0.2.0rc2/langchain/llms/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/huggingface_text_gen_inference.py` & `langchain-0.2.0rc2/langchain/llms/huggingface_text_gen_inference.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/human.py` & `langchain-0.2.0rc2/langchain/llms/human.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/javelin_ai_gateway.py` & `langchain-0.2.0rc2/langchain/llms/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/koboldai.py` & `langchain-0.2.0rc2/langchain/llms/koboldai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/llamacpp.py` & `langchain-0.2.0rc2/langchain/llms/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/loading.py` & `langchain-0.2.0rc2/langchain/llms/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/manifest.py` & `langchain-0.2.0rc2/langchain/llms/manifest.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/minimax.py` & `langchain-0.2.0rc2/langchain/llms/minimax.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/mlflow.py` & `langchain-0.2.0rc2/langchain/llms/mlflow.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/mlflow_ai_gateway.py` & `langchain-0.2.0rc2/langchain/llms/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/modal.py` & `langchain-0.2.0rc2/langchain/llms/modal.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/mosaicml.py` & `langchain-0.2.0rc2/langchain/llms/mosaicml.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/nlpcloud.py` & `langchain-0.2.0rc2/langchain/llms/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/octoai_endpoint.py` & `langchain-0.2.0rc2/langchain/llms/octoai_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/ollama.py` & `langchain-0.2.0rc2/langchain/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/opaqueprompts.py` & `langchain-0.2.0rc2/langchain/llms/opaqueprompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/openai.py` & `langchain-0.2.0rc2/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/openllm.py` & `langchain-0.2.0rc2/langchain/llms/openllm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/openlm.py` & `langchain-0.2.0rc2/langchain/llms/openlm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/pai_eas_endpoint.py` & `langchain-0.2.0rc2/langchain/llms/pai_eas_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/petals.py` & `langchain-0.2.0rc2/langchain/llms/petals.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/pipelineai.py` & `langchain-0.2.0rc2/langchain/llms/pipelineai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/predibase.py` & `langchain-0.2.0rc2/langchain/llms/predibase.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/predictionguard.py` & `langchain-0.2.0rc2/langchain/llms/predictionguard.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/promptlayer_openai.py` & `langchain-0.2.0rc2/langchain/llms/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/replicate.py` & `langchain-0.2.0rc2/langchain/llms/replicate.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/rwkv.py` & `langchain-0.2.0rc2/langchain/llms/rwkv.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/sagemaker_endpoint.py` & `langchain-0.2.0rc2/langchain/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/self_hosted.py` & `langchain-0.2.0rc2/langchain/llms/self_hosted.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/self_hosted_hugging_face.py` & `langchain-0.2.0rc2/langchain/llms/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/stochasticai.py` & `langchain-0.2.0rc2/langchain/llms/stochasticai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/symblai_nebula.py` & `langchain-0.2.0rc2/langchain/llms/symblai_nebula.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/textgen.py` & `langchain-0.2.0rc2/langchain/llms/textgen.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/titan_takeoff.py` & `langchain-0.2.0rc2/langchain/llms/titan_takeoff.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/titan_takeoff_pro.py` & `langchain-0.2.0rc2/langchain/llms/titan_takeoff_pro.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/together.py` & `langchain-0.2.0rc2/langchain/llms/together.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/tongyi.py` & `langchain-0.2.0rc2/langchain/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/utils.py` & `langchain-0.2.0rc2/langchain/llms/utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/vertexai.py` & `langchain-0.2.0rc2/langchain/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/vllm.py` & `langchain-0.2.0rc2/langchain/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/volcengine_maas.py` & `langchain-0.2.0rc2/langchain/llms/volcengine_maas.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/watsonxllm.py` & `langchain-0.2.0rc2/langchain/llms/watsonxllm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/writer.py` & `langchain-0.2.0rc2/langchain/llms/writer.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/xinference.py` & `langchain-0.2.0rc2/langchain/llms/xinference.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/llms/yandex.py` & `langchain-0.2.0rc2/langchain/llms/yandex.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/__init__.py` & `langchain-0.2.0rc2/langchain/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/buffer.py` & `langchain-0.2.0rc2/langchain/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/buffer_window.py` & `langchain-0.2.0rc2/langchain/memory/buffer_window.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_memory.py` & `langchain-0.2.0rc2/langchain/memory/chat_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/__init__.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/astradb.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/cassandra.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/cassandra.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/cosmos_db.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/dynamodb.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/dynamodb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/elasticsearch.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/file.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/file.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/firestore.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/firestore.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/momento.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/momento.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/mongodb.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/mongodb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/neo4j.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/neo4j.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/postgres.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/postgres.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/redis.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/redis.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/rocksetdb.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/singlestoredb.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/sql.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/sql.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/streamlit.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/streamlit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/upstash_redis.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/upstash_redis.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/xata.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/xata.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/chat_message_histories/zep.py` & `langchain-0.2.0rc2/langchain/memory/chat_message_histories/zep.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/combined.py` & `langchain-0.2.0rc2/langchain/memory/combined.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/entity.py` & `langchain-0.2.0rc2/langchain/memory/entity.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/kg.py` & `langchain-0.2.0rc2/langchain/memory/kg.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/motorhead_memory.py` & `langchain-0.2.0rc2/langchain/memory/motorhead_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/prompt.py` & `langchain-0.2.0rc2/langchain/memory/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/readonly.py` & `langchain-0.2.0rc2/langchain/memory/readonly.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/simple.py` & `langchain-0.2.0rc2/langchain/memory/simple.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/summary.py` & `langchain-0.2.0rc2/langchain/memory/summary.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/summary_buffer.py` & `langchain-0.2.0rc2/langchain/memory/summary_buffer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Union
 
 from langchain_core.messages import BaseMessage, get_buffer_string
 from langchain_core.pydantic_v1 import root_validator
 
 from langchain.memory.chat_memory import BaseChatMemory
 from langchain.memory.summary import SummarizerMixin
 
@@ -11,28 +11,29 @@
     """Buffer with summarizer for storing conversation memory."""
 
     max_token_limit: int = 2000
     moving_summary_buffer: str = ""
     memory_key: str = "history"
 
     @property
-    def buffer(self) -> List[BaseMessage]:
-        return self.chat_memory.messages
+    def buffer(self) -> Union[str, List[BaseMessage]]:
+        """String buffer of memory."""
+        return self.load_memory_variables({})[self.memory_key]
 
     @property
     def memory_variables(self) -> List[str]:
         """Will always return list of memory variables.
 
         :meta private:
         """
         return [self.memory_key]
 
     def load_memory_variables(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         """Return history buffer."""
-        buffer = self.buffer
+        buffer = self.chat_memory.messages
         if self.moving_summary_buffer != "":
             first_messages: List[BaseMessage] = [
                 self.summary_message_cls(content=self.moving_summary_buffer)
             ]
             buffer = first_messages + buffer
         if self.return_messages:
             final_buffer: Any = buffer
```

### Comparing `langchain-0.2.0rc1/langchain/memory/token_buffer.py` & `langchain-0.2.0rc2/langchain/memory/token_buffer.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/utils.py` & `langchain-0.2.0rc2/langchain/memory/utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/vectorstore.py` & `langchain-0.2.0rc2/langchain/memory/vectorstore.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/memory/zep_memory.py` & `langchain-0.2.0rc2/langchain/memory/zep_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/model_laboratory.py` & `langchain-0.2.0rc2/langchain/model_laboratory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/__init__.py` & `langchain-0.2.0rc2/langchain/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/boolean.py` & `langchain-0.2.0rc2/langchain/output_parsers/boolean.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/combining.py` & `langchain-0.2.0rc2/langchain/output_parsers/combining.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/datetime.py` & `langchain-0.2.0rc2/langchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/enum.py` & `langchain-0.2.0rc2/langchain/output_parsers/enum.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/ernie_functions.py` & `langchain-0.2.0rc2/langchain/output_parsers/ernie_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/fix.py` & `langchain-0.2.0rc2/langchain/output_parsers/fix.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/format_instructions.py` & `langchain-0.2.0rc2/langchain/output_parsers/format_instructions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/loading.py` & `langchain-0.2.0rc2/langchain/output_parsers/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/pandas_dataframe.py` & `langchain-0.2.0rc2/langchain/output_parsers/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/rail_parser.py` & `langchain-0.2.0rc2/langchain/output_parsers/rail_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/regex.py` & `langchain-0.2.0rc2/langchain/output_parsers/regex.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/regex_dict.py` & `langchain-0.2.0rc2/langchain/output_parsers/regex_dict.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/retry.py` & `langchain-0.2.0rc2/langchain/output_parsers/retry.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/structured.py` & `langchain-0.2.0rc2/langchain/output_parsers/structured.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/output_parsers/yaml.py` & `langchain-0.2.0rc2/langchain/output_parsers/yaml.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/prompts/__init__.py` & `langchain-0.2.0rc2/langchain/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/prompts/base.py` & `langchain-0.2.0rc2/langchain/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/prompts/chat.py` & `langchain-0.2.0rc2/langchain/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/prompts/example_selector/__init__.py` & `langchain-0.2.0rc2/langchain/prompts/example_selector/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/prompts/example_selector/ngram_overlap.py` & `langchain-0.2.0rc2/langchain/prompts/example_selector/ngram_overlap.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/prompts/loading.py` & `langchain-0.2.0rc2/langchain/prompts/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/pydantic_v1/__init__.py` & `langchain-0.2.0rc2/langchain/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/requests.py` & `langchain-0.2.0rc2/langchain/requests.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/__init__.py` & `langchain-0.2.0rc2/langchain/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/arcee.py` & `langchain-0.2.0rc2/langchain/retrievers/arcee.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/arxiv.py` & `langchain-0.2.0rc2/langchain/retrievers/arxiv.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/azure_ai_search.py` & `langchain-0.2.0rc2/langchain/retrievers/azure_ai_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/bedrock.py` & `langchain-0.2.0rc2/langchain/retrievers/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/bm25.py` & `langchain-0.2.0rc2/langchain/retrievers/bm25.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/chaindesk.py` & `langchain-0.2.0rc2/langchain/retrievers/chaindesk.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/chatgpt_plugin_retriever.py` & `langchain-0.2.0rc2/langchain/retrievers/chatgpt_plugin_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/cohere_rag_retriever.py` & `langchain-0.2.0rc2/langchain/retrievers/cohere_rag_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/contextual_compression.py` & `langchain-0.2.0rc2/langchain/retrievers/contextual_compression.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/databerry.py` & `langchain-0.2.0rc2/langchain/retrievers/databerry.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/docarray.py` & `langchain-0.2.0rc2/langchain/retrievers/docarray.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/document_compressors/__init__.py` & `langchain-0.2.0rc2/langchain/retrievers/document_compressors/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/document_compressors/base.py` & `langchain-0.2.0rc2/langchain/retrievers/document_compressors/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/document_compressors/chain_extract.py` & `langchain-0.2.0rc2/langchain/retrievers/document_compressors/chain_extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,15 +60,18 @@
         query: str,
         callbacks: Optional[Callbacks] = None,
     ) -> Sequence[Document]:
         """Compress page content of raw documents."""
         compressed_docs = []
         for doc in documents:
             _input = self.get_input(query, doc)
-            output = self.llm_chain.predict_and_parse(**_input, callbacks=callbacks)
+            output_dict = self.llm_chain.invoke(_input, config={"callbacks": callbacks})
+            output = output_dict[self.llm_chain.output_key]
+            if self.llm_chain.prompt.output_parser is not None:
+                output = self.llm_chain.prompt.output_parser.parse(output)
             if len(output) == 0:
                 continue
             compressed_docs.append(
                 Document(page_content=cast(str, output), metadata=doc.metadata)
             )
         return compressed_docs
```

### Comparing `langchain-0.2.0rc1/langchain/retrievers/document_compressors/chain_filter.py` & `langchain-0.2.0rc2/langchain/retrievers/document_compressors/chain_filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,17 +43,18 @@
         query: str,
         callbacks: Optional[Callbacks] = None,
     ) -> Sequence[Document]:
         """Filter down documents based on their relevance to the query."""
         filtered_docs = []
         for doc in documents:
             _input = self.get_input(query, doc)
-            include_doc = self.llm_chain.predict_and_parse(
-                **_input, callbacks=callbacks
-            )
+            output_dict = self.llm_chain.invoke(_input, config={"callbacks": callbacks})
+            output = output_dict[self.llm_chain.output_key]
+            if self.llm_chain.prompt.output_parser is not None:
+                include_doc = self.llm_chain.prompt.output_parser.parse(output)
             if include_doc:
                 filtered_docs.append(doc)
         return filtered_docs
 
     @classmethod
     def from_llm(
         cls,
```

### Comparing `langchain-0.2.0rc1/langchain/retrievers/document_compressors/cohere_rerank.py` & `langchain-0.2.0rc2/langchain/retrievers/document_compressors/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/document_compressors/cross_encoder_rerank.py` & `langchain-0.2.0rc2/langchain/retrievers/document_compressors/cross_encoder_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/document_compressors/embeddings_filter.py` & `langchain-0.2.0rc2/langchain/retrievers/document_compressors/embeddings_filter.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/document_compressors/flashrank_rerank.py` & `langchain-0.2.0rc2/langchain/retrievers/document_compressors/flashrank_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/elastic_search_bm25.py` & `langchain-0.2.0rc2/langchain/retrievers/elastic_search_bm25.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/embedchain.py` & `langchain-0.2.0rc2/langchain/retrievers/embedchain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/ensemble.py` & `langchain-0.2.0rc2/langchain/retrievers/ensemble.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/google_cloud_documentai_warehouse.py` & `langchain-0.2.0rc2/langchain/retrievers/google_cloud_documentai_warehouse.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/google_vertex_ai_search.py` & `langchain-0.2.0rc2/langchain/retrievers/google_vertex_ai_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/kay.py` & `langchain-0.2.0rc2/langchain/retrievers/kay.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/kendra.py` & `langchain-0.2.0rc2/langchain/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/knn.py` & `langchain-0.2.0rc2/langchain/retrievers/knn.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/llama_index.py` & `langchain-0.2.0rc2/langchain/retrievers/llama_index.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/merger_retriever.py` & `langchain-0.2.0rc2/langchain/retrievers/merger_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/metal.py` & `langchain-0.2.0rc2/langchain/retrievers/metal.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/milvus.py` & `langchain-0.2.0rc2/langchain/retrievers/milvus.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/multi_query.py` & `langchain-0.2.0rc2/langchain/retrievers/multi_query.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/multi_vector.py` & `langchain-0.2.0rc2/langchain/retrievers/multi_vector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/outline.py` & `langchain-0.2.0rc2/langchain/retrievers/outline.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/parent_document_retriever.py` & `langchain-0.2.0rc2/langchain/retrievers/parent_document_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/pinecone_hybrid_search.py` & `langchain-0.2.0rc2/langchain/retrievers/pinecone_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/pubmed.py` & `langchain-0.2.0rc2/langchain/retrievers/pubmed.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/pupmed.py` & `langchain-0.2.0rc2/langchain/retrievers/pupmed.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/re_phraser.py` & `langchain-0.2.0rc2/langchain/retrievers/re_phraser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/remote_retriever.py` & `langchain-0.2.0rc2/langchain/retrievers/remote_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/astradb.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/base.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/chroma.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/chroma.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/dashvector.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/dashvector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/databricks_vector_search.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/databricks_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/deeplake.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/deeplake.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/dingo.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/dingo.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/elasticsearch.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/milvus.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/milvus.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/mongodb_atlas.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/myscale.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/myscale.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/opensearch.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/opensearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/pgvector.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/pgvector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/pinecone.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/pinecone.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/qdrant.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/qdrant.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/redis.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/redis.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/supabase.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/supabase.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/tencentvectordb.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/tencentvectordb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/timescalevector.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/timescalevector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/vectara.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/vectara.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/self_query/weaviate.py` & `langchain-0.2.0rc2/langchain/retrievers/self_query/weaviate.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/svm.py` & `langchain-0.2.0rc2/langchain/retrievers/svm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/tavily_search_api.py` & `langchain-0.2.0rc2/langchain/retrievers/tavily_search_api.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/tfidf.py` & `langchain-0.2.0rc2/langchain/retrievers/tfidf.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/time_weighted_retriever.py` & `langchain-0.2.0rc2/langchain/retrievers/time_weighted_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/vespa_retriever.py` & `langchain-0.2.0rc2/langchain/retrievers/vespa_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/weaviate_hybrid_search.py` & `langchain-0.2.0rc2/langchain/retrievers/weaviate_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/web_research.py` & `langchain-0.2.0rc2/langchain/retrievers/web_research.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/wikipedia.py` & `langchain-0.2.0rc2/langchain/retrievers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/you.py` & `langchain-0.2.0rc2/langchain/retrievers/you.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/zep.py` & `langchain-0.2.0rc2/langchain/retrievers/zep.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/retrievers/zilliz.py` & `langchain-0.2.0rc2/langchain/retrievers/zilliz.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/runnables/__init__.py` & `langchain-0.2.0rc2/langchain/runnables/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/runnables/hub.py` & `langchain-0.2.0rc2/langchain/runnables/hub.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/runnables/openai_functions.py` & `langchain-0.2.0rc2/langchain/runnables/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/schema/__init__.py` & `langchain-0.2.0rc2/langchain/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/schema/callbacks/manager.py` & `langchain-0.2.0rc2/langchain/schema/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/schema/messages.py` & `langchain-0.2.0rc2/langchain/schema/messages.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/schema/output_parser.py` & `langchain-0.2.0rc2/langchain/schema/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/schema/runnable/__init__.py` & `langchain-0.2.0rc2/langchain/schema/runnable/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/schema/runnable/base.py` & `langchain-0.2.0rc2/langchain/schema/runnable/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/schema/runnable/config.py` & `langchain-0.2.0rc2/langchain/schema/runnable/config.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/schema/runnable/utils.py` & `langchain-0.2.0rc2/langchain/schema/runnable/utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/serpapi.py` & `langchain-0.2.0rc2/langchain/serpapi.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/smith/__init__.py` & `langchain-0.2.0rc2/langchain/smith/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/smith/evaluation/__init__.py` & `langchain-0.2.0rc2/langchain/smith/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/smith/evaluation/config.py` & `langchain-0.2.0rc2/langchain/smith/evaluation/config.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/smith/evaluation/name_generation.py` & `langchain-0.2.0rc2/langchain/smith/evaluation/name_generation.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/smith/evaluation/progress.py` & `langchain-0.2.0rc2/langchain/smith/evaluation/progress.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/smith/evaluation/runner_utils.py` & `langchain-0.2.0rc2/langchain/smith/evaluation/runner_utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/smith/evaluation/string_run_evaluator.py` & `langchain-0.2.0rc2/langchain/smith/evaluation/string_run_evaluator.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/sql_database.py` & `langchain-0.2.0rc2/langchain/sql_database.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/storage/__init__.py` & `langchain-0.2.0rc2/langchain/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/storage/_lc_store.py` & `langchain-0.2.0rc2/langchain/storage/_lc_store.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/storage/encoder_backed.py` & `langchain-0.2.0rc2/langchain/storage/encoder_backed.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/storage/file_system.py` & `langchain-0.2.0rc2/langchain/storage/file_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import time
 from pathlib import Path
 from typing import Iterator, List, Optional, Sequence, Tuple, Union
 
 from langchain_core.stores import ByteStore
 
 from langchain.storage.exceptions import InvalidKeyException
 
@@ -38,28 +39,34 @@
 
     def __init__(
         self,
         root_path: Union[str, Path],
         *,
         chmod_file: Optional[int] = None,
         chmod_dir: Optional[int] = None,
+        update_atime: bool = False,
     ) -> None:
         """Implement the BaseStore interface for the local file system.
 
         Args:
             root_path (Union[str, Path]): The root path of the file store. All keys are
                 interpreted as paths relative to this root.
             chmod_file: (optional, defaults to `None`) If specified, sets permissions
                 for newly created files, overriding the current `umask` if needed.
             chmod_dir: (optional, defaults to `None`) If specified, sets permissions
                 for newly created dirs, overriding the current `umask` if needed.
+            update_atime: (optional, defaults to `False`) If `True`, updates the
+                filesystem access time (but not the modified time) when a file is read.
+                This allows MRU/LRU cache policies to be implemented for filesystems
+                where access time updates are disabled.
         """
         self.root_path = Path(root_path).absolute()
         self.chmod_file = chmod_file
         self.chmod_dir = chmod_dir
+        self.update_atime = update_atime
 
     def _get_full_path(self, key: str) -> Path:
         """Get the full path for a given key relative to the root path.
 
         Args:
             key (str): The key relative to the root path.
 
@@ -108,14 +115,17 @@
         """
         values: List[Optional[bytes]] = []
         for key in keys:
             full_path = self._get_full_path(key)
             if full_path.exists():
                 value = full_path.read_bytes()
                 values.append(value)
+                if self.update_atime:
+                    # update access time only; preserve modified time
+                    os.utime(full_path, (time.time(), os.stat(full_path).st_mtime))
             else:
                 values.append(None)
         return values
 
     def mset(self, key_value_pairs: Sequence[Tuple[str, bytes]]) -> None:
         """Set the values for the given keys.
```

### Comparing `langchain-0.2.0rc1/langchain/storage/redis.py` & `langchain-0.2.0rc2/langchain/storage/redis.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/storage/upstash_redis.py` & `langchain-0.2.0rc2/langchain/storage/upstash_redis.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/text_splitter.py` & `langchain-0.2.0rc2/langchain/text_splitter.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/__init__.py` & `langchain-0.2.0rc2/langchain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/ainetwork/app.py` & `langchain-0.2.0rc2/langchain/tools/ainetwork/app.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/ainetwork/base.py` & `langchain-0.2.0rc2/langchain/tools/ainetwork/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/ainetwork/owner.py` & `langchain-0.2.0rc2/langchain/tools/ainetwork/owner.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/ainetwork/rule.py` & `langchain-0.2.0rc2/langchain/tools/ainetwork/rule.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/ainetwork/transfer.py` & `langchain-0.2.0rc2/langchain/tools/ainetwork/transfer.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/ainetwork/value.py` & `langchain-0.2.0rc2/langchain/tools/ainetwork/value.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/amadeus/__init__.py` & `langchain-0.2.0rc2/langchain/tools/amadeus/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/amadeus/base.py` & `langchain-0.2.0rc2/langchain/tools/amadeus/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/amadeus/closest_airport.py` & `langchain-0.2.0rc2/langchain/tools/amadeus/closest_airport.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/amadeus/flight_search.py` & `langchain-0.2.0rc2/langchain/tools/amadeus/flight_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/arxiv/tool.py` & `langchain-0.2.0rc2/langchain/tools/arxiv/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/__init__.py` & `langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/form_recognizer.py` & `langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/form_recognizer.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/image_analysis.py` & `langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/image_analysis.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/speech2text.py` & `langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/speech2text.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/text2speech.py` & `langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/text2speech.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/azure_cognitive_services/text_analytics_health.py` & `langchain-0.2.0rc2/langchain/tools/azure_cognitive_services/text_analytics_health.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/bearly/tool.py` & `langchain-0.2.0rc2/langchain/tools/bearly/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/bing_search/__init__.py` & `langchain-0.2.0rc2/langchain/tools/bing_search/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/bing_search/tool.py` & `langchain-0.2.0rc2/langchain/tools/bing_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/brave_search/tool.py` & `langchain-0.2.0rc2/langchain/tools/brave_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/clickup/tool.py` & `langchain-0.2.0rc2/langchain/tools/clickup/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/dataforseo_api_search/__init__.py` & `langchain-0.2.0rc2/langchain/tools/dataforseo_api_search/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/dataforseo_api_search/tool.py` & `langchain-0.2.0rc2/langchain/tools/dataforseo_api_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/ddg_search/__init__.py` & `langchain-0.2.0rc2/langchain/tools/ddg_search/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/ddg_search/tool.py` & `langchain-0.2.0rc2/langchain/tools/ddg_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/e2b_data_analysis/tool.py` & `langchain-0.2.0rc2/langchain/tools/e2b_data_analysis/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/edenai/__init__.py` & `langchain-0.2.0rc2/langchain/tools/edenai/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/edenai/audio_speech_to_text.py` & `langchain-0.2.0rc2/langchain/tools/edenai/audio_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/edenai/audio_text_to_speech.py` & `langchain-0.2.0rc2/langchain/tools/edenai/audio_text_to_speech.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/edenai/edenai_base_tool.py` & `langchain-0.2.0rc2/langchain/tools/edenai/edenai_base_tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/edenai/image_explicitcontent.py` & `langchain-0.2.0rc2/langchain/tools/edenai/image_explicitcontent.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/edenai/image_objectdetection.py` & `langchain-0.2.0rc2/langchain/tools/edenai/image_objectdetection.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/edenai/ocr_identityparser.py` & `langchain-0.2.0rc2/langchain/tools/edenai/ocr_identityparser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/edenai/ocr_invoiceparser.py` & `langchain-0.2.0rc2/langchain/tools/edenai/ocr_invoiceparser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/edenai/text_moderation.py` & `langchain-0.2.0rc2/langchain/tools/edenai/text_moderation.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/eleven_labs/__init__.py` & `langchain-0.2.0rc2/langchain/tools/eleven_labs/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/eleven_labs/models.py` & `langchain-0.2.0rc2/langchain/tools/eleven_labs/models.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/eleven_labs/text2speech.py` & `langchain-0.2.0rc2/langchain/tools/eleven_labs/text2speech.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/file_management/__init__.py` & `langchain-0.2.0rc2/langchain/tools/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/file_management/copy.py` & `langchain-0.2.0rc2/langchain/tools/file_management/copy.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/file_management/delete.py` & `langchain-0.2.0rc2/langchain/tools/file_management/delete.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/file_management/file_search.py` & `langchain-0.2.0rc2/langchain/tools/file_management/file_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/file_management/list_dir.py` & `langchain-0.2.0rc2/langchain/tools/file_management/list_dir.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/file_management/move.py` & `langchain-0.2.0rc2/langchain/tools/file_management/move.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/file_management/read.py` & `langchain-0.2.0rc2/langchain/tools/file_management/read.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/file_management/write.py` & `langchain-0.2.0rc2/langchain/tools/file_management/write.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/github/tool.py` & `langchain-0.2.0rc2/langchain/tools/github/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/gitlab/tool.py` & `langchain-0.2.0rc2/langchain/tools/gitlab/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/gmail/__init__.py` & `langchain-0.2.0rc2/langchain/tools/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/gmail/base.py` & `langchain-0.2.0rc2/langchain/tools/gmail/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/gmail/create_draft.py` & `langchain-0.2.0rc2/langchain/tools/gmail/create_draft.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/gmail/get_message.py` & `langchain-0.2.0rc2/langchain/tools/gmail/get_message.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/gmail/get_thread.py` & `langchain-0.2.0rc2/langchain/tools/gmail/get_thread.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/gmail/search.py` & `langchain-0.2.0rc2/langchain/tools/gmail/search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/gmail/send_message.py` & `langchain-0.2.0rc2/langchain/tools/gmail/send_message.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/golden_query/__init__.py` & `langchain-0.2.0rc2/langchain/tools/golden_query/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/golden_query/tool.py` & `langchain-0.2.0rc2/langchain/tools/golden_query/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_cloud/__init__.py` & `langchain-0.2.0rc2/langchain/tools/google_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_cloud/texttospeech.py` & `langchain-0.2.0rc2/langchain/tools/google_cloud/texttospeech.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_finance/__init__.py` & `langchain-0.2.0rc2/langchain/tools/google_finance/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_finance/tool.py` & `langchain-0.2.0rc2/langchain/tools/google_finance/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_jobs/__init__.py` & `langchain-0.2.0rc2/langchain/tools/google_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_jobs/tool.py` & `langchain-0.2.0rc2/langchain/tools/google_jobs/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_lens/__init__.py` & `langchain-0.2.0rc2/langchain/tools/google_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_lens/tool.py` & `langchain-0.2.0rc2/langchain/tools/google_lens/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_places/__init__.py` & `langchain-0.2.0rc2/langchain/tools/google_places/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_places/tool.py` & `langchain-0.2.0rc2/langchain/tools/google_places/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_scholar/__init__.py` & `langchain-0.2.0rc2/langchain/tools/google_scholar/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_scholar/tool.py` & `langchain-0.2.0rc2/langchain/tools/google_scholar/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_search/__init__.py` & `langchain-0.2.0rc2/langchain/tools/google_search/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_search/tool.py` & `langchain-0.2.0rc2/langchain/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_serper/__init__.py` & `langchain-0.2.0rc2/langchain/tools/google_serper/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_serper/tool.py` & `langchain-0.2.0rc2/langchain/tools/google_serper/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_trends/__init__.py` & `langchain-0.2.0rc2/langchain/tools/google_trends/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/google_trends/tool.py` & `langchain-0.2.0rc2/langchain/tools/google_trends/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/graphql/tool.py` & `langchain-0.2.0rc2/langchain/tools/graphql/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/human/__init__.py` & `langchain-0.2.0rc2/langchain/tools/human/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/human/tool.py` & `langchain-0.2.0rc2/langchain/tools/human/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/ifttt.py` & `langchain-0.2.0rc2/langchain/tools/ifttt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/interaction/tool.py` & `langchain-0.2.0rc2/langchain/tools/interaction/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/jira/tool.py` & `langchain-0.2.0rc2/langchain/tools/jira/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/json/tool.py` & `langchain-0.2.0rc2/langchain/tools/json/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/memorize/__init__.py` & `langchain-0.2.0rc2/langchain/tools/memorize/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/memorize/tool.py` & `langchain-0.2.0rc2/langchain/tools/memorize/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/merriam_webster/tool.py` & `langchain-0.2.0rc2/langchain/tools/merriam_webster/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/metaphor_search/__init__.py` & `langchain-0.2.0rc2/langchain/tools/metaphor_search/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/metaphor_search/tool.py` & `langchain-0.2.0rc2/langchain/tools/metaphor_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/multion/__init__.py` & `langchain-0.2.0rc2/langchain/tools/multion/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/multion/close_session.py` & `langchain-0.2.0rc2/langchain/tools/multion/close_session.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/multion/create_session.py` & `langchain-0.2.0rc2/langchain/tools/multion/create_session.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/multion/update_session.py` & `langchain-0.2.0rc2/langchain/tools/multion/update_session.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/nasa/tool.py` & `langchain-0.2.0rc2/langchain/tools/nasa/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/nuclia/__init__.py` & `langchain-0.2.0rc2/langchain/tools/nuclia/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/nuclia/tool.py` & `langchain-0.2.0rc2/langchain/tools/nuclia/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/office365/__init__.py` & `langchain-0.2.0rc2/langchain/tools/office365/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/office365/base.py` & `langchain-0.2.0rc2/langchain/tools/office365/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/office365/create_draft_message.py` & `langchain-0.2.0rc2/langchain/tools/office365/create_draft_message.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/office365/events_search.py` & `langchain-0.2.0rc2/langchain/tools/office365/events_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/office365/messages_search.py` & `langchain-0.2.0rc2/langchain/tools/office365/messages_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/office365/send_event.py` & `langchain-0.2.0rc2/langchain/tools/office365/send_event.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/office365/send_message.py` & `langchain-0.2.0rc2/langchain/tools/office365/send_message.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/openapi/utils/api_models.py` & `langchain-0.2.0rc2/langchain/tools/openapi/utils/api_models.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/openapi/utils/openapi_utils.py` & `langchain-0.2.0rc2/langchain/tools/openapi/utils/openapi_utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/openweathermap/__init__.py` & `langchain-0.2.0rc2/langchain/tools/openweathermap/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/openweathermap/tool.py` & `langchain-0.2.0rc2/langchain/tools/openweathermap/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/playwright/__init__.py` & `langchain-0.2.0rc2/langchain/tools/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/playwright/base.py` & `langchain-0.2.0rc2/langchain/tools/playwright/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/playwright/click.py` & `langchain-0.2.0rc2/langchain/tools/playwright/click.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/playwright/current_page.py` & `langchain-0.2.0rc2/langchain/tools/playwright/current_page.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/playwright/extract_hyperlinks.py` & `langchain-0.2.0rc2/langchain/tools/playwright/extract_hyperlinks.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/playwright/extract_text.py` & `langchain-0.2.0rc2/langchain/tools/playwright/extract_text.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/playwright/get_elements.py` & `langchain-0.2.0rc2/langchain/tools/playwright/get_elements.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/playwright/navigate.py` & `langchain-0.2.0rc2/langchain/tools/playwright/navigate.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/playwright/navigate_back.py` & `langchain-0.2.0rc2/langchain/tools/playwright/navigate_back.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/plugin.py` & `langchain-0.2.0rc2/langchain/tools/plugin.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/powerbi/tool.py` & `langchain-0.2.0rc2/langchain/tools/powerbi/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/pubmed/tool.py` & `langchain-0.2.0rc2/langchain/tools/pubmed/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/python/__init__.py` & `langchain-0.2.0rc2/langchain/tools/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/reddit_search/tool.py` & `langchain-0.2.0rc2/langchain/tools/reddit_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/render.py` & `langchain-0.2.0rc2/langchain/tools/render.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/requests/tool.py` & `langchain-0.2.0rc2/langchain/tools/requests/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/scenexplain/tool.py` & `langchain-0.2.0rc2/langchain/tools/scenexplain/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/searchapi/__init__.py` & `langchain-0.2.0rc2/langchain/tools/searchapi/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/searchapi/tool.py` & `langchain-0.2.0rc2/langchain/tools/searchapi/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/searx_search/tool.py` & `langchain-0.2.0rc2/langchain/tools/searx_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/shell/__init__.py` & `langchain-0.2.0rc2/langchain/tools/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/shell/tool.py` & `langchain-0.2.0rc2/langchain/tools/shell/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/slack/__init__.py` & `langchain-0.2.0rc2/langchain/tools/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/slack/base.py` & `langchain-0.2.0rc2/langchain/tools/slack/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/slack/get_channel.py` & `langchain-0.2.0rc2/langchain/tools/slack/get_channel.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/slack/get_message.py` & `langchain-0.2.0rc2/langchain/tools/slack/get_message.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/slack/schedule_message.py` & `langchain-0.2.0rc2/langchain/tools/slack/schedule_message.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/slack/send_message.py` & `langchain-0.2.0rc2/langchain/tools/slack/send_message.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/sleep/tool.py` & `langchain-0.2.0rc2/langchain/tools/sleep/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/spark_sql/tool.py` & `langchain-0.2.0rc2/langchain/tools/spark_sql/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/sql_database/tool.py` & `langchain-0.2.0rc2/langchain/tools/sql_database/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/stackexchange/tool.py` & `langchain-0.2.0rc2/langchain/tools/stackexchange/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/steam/tool.py` & `langchain-0.2.0rc2/langchain/tools/steam/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/steamship_image_generation/__init__.py` & `langchain-0.2.0rc2/langchain/tools/steamship_image_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/steamship_image_generation/tool.py` & `langchain-0.2.0rc2/langchain/tools/steamship_image_generation/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/tavily_search/__init__.py` & `langchain-0.2.0rc2/langchain/tools/tavily_search/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/tavily_search/tool.py` & `langchain-0.2.0rc2/langchain/tools/tavily_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/vectorstore/tool.py` & `langchain-0.2.0rc2/langchain/tools/vectorstore/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/wikipedia/tool.py` & `langchain-0.2.0rc2/langchain/tools/wikipedia/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/wolfram_alpha/__init__.py` & `langchain-0.2.0rc2/langchain/tools/wolfram_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/wolfram_alpha/tool.py` & `langchain-0.2.0rc2/langchain/tools/wolfram_alpha/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/yahoo_finance_news.py` & `langchain-0.2.0rc2/langchain/tools/yahoo_finance_news.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/youtube/search.py` & `langchain-0.2.0rc2/langchain/tools/youtube/search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/zapier/__init__.py` & `langchain-0.2.0rc2/langchain/tools/zapier/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/tools/zapier/tool.py` & `langchain-0.2.0rc2/langchain/tools/zapier/tool.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/__init__.py` & `langchain-0.2.0rc2/langchain/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/alpha_vantage.py` & `langchain-0.2.0rc2/langchain/utilities/alpha_vantage.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/anthropic.py` & `langchain-0.2.0rc2/langchain/utilities/anthropic.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/apify.py` & `langchain-0.2.0rc2/langchain/utilities/apify.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/arcee.py` & `langchain-0.2.0rc2/langchain/utilities/arcee.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/arxiv.py` & `langchain-0.2.0rc2/langchain/utilities/arxiv.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/awslambda.py` & `langchain-0.2.0rc2/langchain/utilities/awslambda.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/bibtex.py` & `langchain-0.2.0rc2/langchain/utilities/bibtex.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/bing_search.py` & `langchain-0.2.0rc2/langchain/utilities/bing_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/brave_search.py` & `langchain-0.2.0rc2/langchain/utilities/brave_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/clickup.py` & `langchain-0.2.0rc2/langchain/utilities/clickup.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/dalle_image_generator.py` & `langchain-0.2.0rc2/langchain/utilities/dalle_image_generator.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/dataforseo_api_search.py` & `langchain-0.2.0rc2/langchain/utilities/dataforseo_api_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/duckduckgo_search.py` & `langchain-0.2.0rc2/langchain/utilities/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/github.py` & `langchain-0.2.0rc2/langchain/utilities/github.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/gitlab.py` & `langchain-0.2.0rc2/langchain/utilities/gitlab.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/golden_query.py` & `langchain-0.2.0rc2/langchain/utilities/golden_query.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/google_finance.py` & `langchain-0.2.0rc2/langchain/utilities/google_finance.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/google_jobs.py` & `langchain-0.2.0rc2/langchain/utilities/google_jobs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/google_lens.py` & `langchain-0.2.0rc2/langchain/utilities/google_lens.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/google_places_api.py` & `langchain-0.2.0rc2/langchain/utilities/google_places_api.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/google_scholar.py` & `langchain-0.2.0rc2/langchain/utilities/google_scholar.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/google_search.py` & `langchain-0.2.0rc2/langchain/utilities/google_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/google_serper.py` & `langchain-0.2.0rc2/langchain/utilities/google_serper.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/google_trends.py` & `langchain-0.2.0rc2/langchain/utilities/google_trends.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/graphql.py` & `langchain-0.2.0rc2/langchain/utilities/graphql.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/jira.py` & `langchain-0.2.0rc2/langchain/utilities/jira.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/max_compute.py` & `langchain-0.2.0rc2/langchain/utilities/max_compute.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/merriam_webster.py` & `langchain-0.2.0rc2/langchain/utilities/merriam_webster.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/metaphor_search.py` & `langchain-0.2.0rc2/langchain/utilities/metaphor_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/nasa.py` & `langchain-0.2.0rc2/langchain/utilities/nasa.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/opaqueprompts.py` & `langchain-0.2.0rc2/langchain/utilities/opaqueprompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/openapi.py` & `langchain-0.2.0rc2/langchain/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/openweathermap.py` & `langchain-0.2.0rc2/langchain/utilities/openweathermap.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/outline.py` & `langchain-0.2.0rc2/langchain/utilities/outline.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/portkey.py` & `langchain-0.2.0rc2/langchain/utilities/portkey.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/powerbi.py` & `langchain-0.2.0rc2/langchain/utilities/powerbi.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/pubmed.py` & `langchain-0.2.0rc2/langchain/utilities/pubmed.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/reddit_search.py` & `langchain-0.2.0rc2/langchain/utilities/reddit_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/redis.py` & `langchain-0.2.0rc2/langchain/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/requests.py` & `langchain-0.2.0rc2/langchain/utilities/requests.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/scenexplain.py` & `langchain-0.2.0rc2/langchain/utilities/scenexplain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/searchapi.py` & `langchain-0.2.0rc2/langchain/utilities/searchapi.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/searx_search.py` & `langchain-0.2.0rc2/langchain/utilities/searx_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/serpapi.py` & `langchain-0.2.0rc2/langchain/utilities/serpapi.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/spark_sql.py` & `langchain-0.2.0rc2/langchain/utilities/spark_sql.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/sql_database.py` & `langchain-0.2.0rc2/langchain/utilities/sql_database.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/stackexchange.py` & `langchain-0.2.0rc2/langchain/utilities/stackexchange.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/steam.py` & `langchain-0.2.0rc2/langchain/utilities/steam.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/tavily_search.py` & `langchain-0.2.0rc2/langchain/utilities/tavily_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/tensorflow_datasets.py` & `langchain-0.2.0rc2/langchain/utilities/tensorflow_datasets.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/twilio.py` & `langchain-0.2.0rc2/langchain/utilities/twilio.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/vertexai.py` & `langchain-0.2.0rc2/langchain/utilities/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/wikipedia.py` & `langchain-0.2.0rc2/langchain/utilities/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/wolfram_alpha.py` & `langchain-0.2.0rc2/langchain/utilities/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utilities/zapier.py` & `langchain-0.2.0rc2/langchain/utilities/zapier.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utils/__init__.py` & `langchain-0.2.0rc2/langchain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utils/ernie_functions.py` & `langchain-0.2.0rc2/langchain/utils/ernie_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utils/math.py` & `langchain-0.2.0rc2/langchain/utils/math.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/utils/openai.py` & `langchain-0.2.0rc2/langchain/utils/openai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/__init__.py` & `langchain-0.2.0rc2/langchain/vectorstores/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         Meilisearch,
         Milvus,
         MomentoVectorIndex,
         MongoDBAtlasVectorSearch,
         MyScale,
         MyScaleSettings,
         Neo4jVector,
+        NeuralDBClientVectorStore,
         NeuralDBVectorStore,
         OpenSearchVectorSearch,
         PGEmbedding,
         PGVector,
         Pinecone,
         Qdrant,
         Redis,
@@ -138,14 +139,15 @@
     "Meilisearch": "langchain_community.vectorstores",
     "Milvus": "langchain_community.vectorstores",
     "MomentoVectorIndex": "langchain_community.vectorstores",
     "MongoDBAtlasVectorSearch": "langchain_community.vectorstores",
     "MyScale": "langchain_community.vectorstores",
     "MyScaleSettings": "langchain_community.vectorstores",
     "Neo4jVector": "langchain_community.vectorstores",
+    "NeuralDBClientVectorStore": "langchain_community.vectorstores",
     "NeuralDBVectorStore": "langchain_community.vectorstores",
     "NEuralDBVectorStore": "langchain_community.vectorstores",
     "OpenSearchVectorSearch": "langchain_community.vectorstores",
     "PGEmbedding": "langchain_community.vectorstores",
     "PGVector": "langchain_community.vectorstores",
     "Pinecone": "langchain_community.vectorstores",
     "Qdrant": "langchain_community.vectorstores",
@@ -220,14 +222,15 @@
     "Meilisearch",
     "Milvus",
     "MomentoVectorIndex",
     "MongoDBAtlasVectorSearch",
     "MyScale",
     "MyScaleSettings",
     "Neo4jVector",
+    "NeuralDBClientVectorStore",
     "NeuralDBVectorStore",
     "OpenSearchVectorSearch",
     "PGEmbedding",
     "PGVector",
     "Pinecone",
     "Qdrant",
     "Redis",
```

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/alibabacloud_opensearch.py` & `langchain-0.2.0rc2/langchain/vectorstores/alibabacloud_opensearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/analyticdb.py` & `langchain-0.2.0rc2/langchain/vectorstores/analyticdb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/annoy.py` & `langchain-0.2.0rc2/langchain/vectorstores/annoy.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/astradb.py` & `langchain-0.2.0rc2/langchain/vectorstores/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/atlas.py` & `langchain-0.2.0rc2/langchain/vectorstores/atlas.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/awadb.py` & `langchain-0.2.0rc2/langchain/vectorstores/awadb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/azure_cosmos_db.py` & `langchain-0.2.0rc2/langchain/vectorstores/azure_cosmos_db.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/azuresearch.py` & `langchain-0.2.0rc2/langchain/vectorstores/azuresearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/bageldb.py` & `langchain-0.2.0rc2/langchain/vectorstores/bageldb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/baiducloud_vector_search.py` & `langchain-0.2.0rc2/langchain/vectorstores/baiducloud_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/cassandra.py` & `langchain-0.2.0rc2/langchain/vectorstores/cassandra.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/chroma.py` & `langchain-0.2.0rc2/langchain/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/clarifai.py` & `langchain-0.2.0rc2/langchain/vectorstores/clarifai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/clickhouse.py` & `langchain-0.2.0rc2/langchain/vectorstores/clickhouse.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/dashvector.py` & `langchain-0.2.0rc2/langchain/vectorstores/dashvector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/databricks_vector_search.py` & `langchain-0.2.0rc2/langchain/vectorstores/databricks_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/deeplake.py` & `langchain-0.2.0rc2/langchain/vectorstores/deeplake.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/dingo.py` & `langchain-0.2.0rc2/langchain/vectorstores/dingo.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/docarray/__init__.py` & `langchain-0.2.0rc2/langchain/vectorstores/docarray/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/docarray/base.py` & `langchain-0.2.0rc2/langchain/vectorstores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/docarray/hnsw.py` & `langchain-0.2.0rc2/langchain/vectorstores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/docarray/in_memory.py` & `langchain-0.2.0rc2/langchain/vectorstores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/elastic_vector_search.py` & `langchain-0.2.0rc2/langchain/vectorstores/elastic_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/elasticsearch.py` & `langchain-0.2.0rc2/langchain/vectorstores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/epsilla.py` & `langchain-0.2.0rc2/langchain/vectorstores/epsilla.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/faiss.py` & `langchain-0.2.0rc2/langchain/vectorstores/faiss.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/hippo.py` & `langchain-0.2.0rc2/langchain/vectorstores/hippo.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/hologres.py` & `langchain-0.2.0rc2/langchain/vectorstores/hologres.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/lancedb.py` & `langchain-0.2.0rc2/langchain/vectorstores/lancedb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/llm_rails.py` & `langchain-0.2.0rc2/langchain/vectorstores/llm_rails.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/marqo.py` & `langchain-0.2.0rc2/langchain/vectorstores/marqo.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/matching_engine.py` & `langchain-0.2.0rc2/langchain/vectorstores/matching_engine.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/meilisearch.py` & `langchain-0.2.0rc2/langchain/vectorstores/meilisearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/milvus.py` & `langchain-0.2.0rc2/langchain/vectorstores/milvus.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/momento_vector_index.py` & `langchain-0.2.0rc2/langchain/vectorstores/momento_vector_index.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/mongodb_atlas.py` & `langchain-0.2.0rc2/langchain/vectorstores/mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/myscale.py` & `langchain-0.2.0rc2/langchain/vectorstores/myscale.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/neo4j_vector.py` & `langchain-0.2.0rc2/langchain/vectorstores/neo4j_vector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/nucliadb.py` & `langchain-0.2.0rc2/langchain/vectorstores/nucliadb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/opensearch_vector_search.py` & `langchain-0.2.0rc2/langchain/vectorstores/opensearch_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/pgembedding.py` & `langchain-0.2.0rc2/langchain/vectorstores/pgembedding.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/pgvecto_rs.py` & `langchain-0.2.0rc2/langchain/vectorstores/pgvecto_rs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/pgvector.py` & `langchain-0.2.0rc2/langchain/vectorstores/pgvector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/pinecone.py` & `langchain-0.2.0rc2/langchain/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/qdrant.py` & `langchain-0.2.0rc2/langchain/vectorstores/qdrant.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/redis/__init__.py` & `langchain-0.2.0rc2/langchain/vectorstores/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/redis/base.py` & `langchain-0.2.0rc2/langchain/vectorstores/redis/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/redis/filters.py` & `langchain-0.2.0rc2/langchain/vectorstores/redis/filters.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/redis/schema.py` & `langchain-0.2.0rc2/langchain/vectorstores/redis/schema.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/rocksetdb.py` & `langchain-0.2.0rc2/langchain/vectorstores/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/scann.py` & `langchain-0.2.0rc2/langchain/vectorstores/scann.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/semadb.py` & `langchain-0.2.0rc2/langchain/vectorstores/semadb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/singlestoredb.py` & `langchain-0.2.0rc2/langchain/vectorstores/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/sklearn.py` & `langchain-0.2.0rc2/langchain/vectorstores/sklearn.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/sqlitevss.py` & `langchain-0.2.0rc2/langchain/vectorstores/sqlitevss.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/starrocks.py` & `langchain-0.2.0rc2/langchain/vectorstores/starrocks.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/supabase.py` & `langchain-0.2.0rc2/langchain/vectorstores/supabase.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/tair.py` & `langchain-0.2.0rc2/langchain/vectorstores/tair.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/tencentvectordb.py` & `langchain-0.2.0rc2/langchain/vectorstores/tencentvectordb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/tigris.py` & `langchain-0.2.0rc2/langchain/vectorstores/tigris.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/tiledb.py` & `langchain-0.2.0rc2/langchain/vectorstores/tiledb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/timescalevector.py` & `langchain-0.2.0rc2/langchain/vectorstores/timescalevector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/typesense.py` & `langchain-0.2.0rc2/langchain/vectorstores/typesense.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/usearch.py` & `langchain-0.2.0rc2/langchain/vectorstores/usearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/utils.py` & `langchain-0.2.0rc2/langchain/vectorstores/utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/vald.py` & `langchain-0.2.0rc2/langchain/vectorstores/vald.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/vearch.py` & `langchain-0.2.0rc2/langchain/vectorstores/vearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/vectara.py` & `langchain-0.2.0rc2/langchain/vectorstores/vectara.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/vespa.py` & `langchain-0.2.0rc2/langchain/vectorstores/vespa.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/weaviate.py` & `langchain-0.2.0rc2/langchain/vectorstores/weaviate.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/xata.py` & `langchain-0.2.0rc2/langchain/vectorstores/xata.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/yellowbrick.py` & `langchain-0.2.0rc2/langchain/vectorstores/yellowbrick.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/zep.py` & `langchain-0.2.0rc2/langchain/vectorstores/zep.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/langchain/vectorstores/zilliz.py` & `langchain-0.2.0rc2/langchain/vectorstores/zilliz.py`

 * *Files identical despite different names*

### Comparing `langchain-0.2.0rc1/pyproject.toml` & `langchain-0.2.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "langchain"
-version = "0.2.0rc1"
+version = "0.2.0rc2"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 
 [tool.poetry.scripts]
 langchain-server = "langchain.server:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.48"
+langchain-core = "^0.1.52"
 langchain-text-splitters = ">=0.0.1,<0.1"
 langsmith = "^0.1.17"
 pydantic = ">=1,<3"
-SQLAlchemy = ">=1.4,<3"
+SQLAlchemy = ">=1.4,<2.0.29"
 requests = "^2"
 PyYAML = ">=5.3"
 numpy = "^1"
 aiohttp = "^3.8.3"
 tenacity = "^8.1.0"
 azure-core = {version = "^1.26.4", optional=true}
 tqdm = {version = ">=4.48.0", optional = true}
```

### Comparing `langchain-0.2.0rc1/PKG-INFO` & `langchain-0.2.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: Building applications with LLMs through composability
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -21,15 +21,15 @@
 Provides-Extra: extended-testing
 Provides-Extra: javascript
 Provides-Extra: llms
 Provides-Extra: openai
 Provides-Extra: qdrant
 Provides-Extra: text-helpers
 Requires-Dist: PyYAML (>=5.3)
-Requires-Dist: SQLAlchemy (>=1.4,<3)
+Requires-Dist: SQLAlchemy (>=1.4,<2.0.29)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0) ; extra == "extended-testing"
 Requires-Dist: aleph-alpha-client (>=2.15.0,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: anthropic (>=0.3.11,<0.4.0) ; extra == "extended-testing"
 Requires-Dist: arxiv (>=1.4,<2.0) ; extra == "extended-testing"
 Requires-Dist: assemblyai (>=0.17.0,<0.18.0) ; extra == "extended-testing"
 Requires-Dist: async-timeout (>=4.0.0,<5.0.0) ; python_version < "3.11"
@@ -65,15 +65,15 @@
 Requires-Dist: hologres-vector (>=0.0.6,<0.0.7) ; extra == "extended-testing"
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0) ; extra == "extended-testing"
 Requires-Dist: huggingface_hub (>=0,<1) ; extra == "llms"
 Requires-Dist: javelin-sdk (>=0.1.8,<0.2.0) ; extra == "extended-testing"
 Requires-Dist: jinja2 (>=3,<4) ; extra == "extended-testing"
 Requires-Dist: jq (>=1.4.1,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: jsonschema (>1) ; extra == "extended-testing"
-Requires-Dist: langchain-core (>=0.1.48,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.52,<0.2.0)
 Requires-Dist: langchain-openai (>=0.0.2,<0.1) ; extra == "extended-testing"
 Requires-Dist: langchain-text-splitters (>=0.0.1,<0.1)
 Requires-Dist: langsmith (>=0.1.17,<0.2.0)
 Requires-Dist: lxml (>=4.9.3,<6.0) ; extra == "extended-testing"
 Requires-Dist: manifest-ml (>=0.0.1,<0.0.2) ; extra == "llms"
 Requires-Dist: markdownify (>=0.11.6,<0.12.0) ; extra == "extended-testing"
 Requires-Dist: motor (>=3.3.1,<4.0.0) ; extra == "extended-testing"
```

