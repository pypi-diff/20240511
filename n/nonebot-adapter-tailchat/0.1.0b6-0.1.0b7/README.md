# Comparing `tmp/nonebot_adapter_tailchat-0.1.0b6.tar.gz` & `tmp/nonebot_adapter_tailchat-0.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b6.tar", max compression
+gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b7.tar", max compression
```

## Comparing `nonebot_adapter_tailchat-0.1.0b6.tar` & `nonebot_adapter_tailchat-0.1.0b7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11335 2024-05-09 12:01:17.177909 nonebot_adapter_tailchat-0.1.0b6/LICENSE
--rw-r--r--   0        0        0     1488 2024-05-09 12:01:17.177909 nonebot_adapter_tailchat-0.1.0b6/README.md
--rw-r--r--   0        0        0      260 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/__init__.py
--rw-r--r--   0        0        0     7316 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/adapter.py
--rw-r--r--   0        0        0    24311 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/api.py
--rw-r--r--   0        0        0     8081 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/bbcode.py
--rw-r--r--   0        0        0     4454 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/bot.py
--rw-r--r--   0        0        0      675 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/config.py
--rw-r--r--   0        0        0      158 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/const.py
--rw-r--r--   0        0        0    10816 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/event.py
--rw-r--r--   0        0        0     1497 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/exception.py
--rw-r--r--   0        0        0    11198 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/message.py
--rw-r--r--   0        0        0     5817 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/model.py
--rw-r--r--   0        0        0      374 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/permission.py
--rw-r--r--   0        0        0      456 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/rule.py
--rw-r--r--   0        0        0     2103 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/util.py
--rw-r--r--   0        0        0     1232 2024-05-09 12:01:17.181909 nonebot_adapter_tailchat-0.1.0b6/pyproject.toml
--rw-r--r--   0        0        0     2272 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b6/PKG-INFO
+-rw-r--r--   0        0        0    11335 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/LICENSE
+-rw-r--r--   0        0        0     1488 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/README.md
+-rw-r--r--   0        0        0      260 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/__init__.py
+-rw-r--r--   0        0        0     7316 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/adapter.py
+-rw-r--r--   0        0        0    24554 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/api.py
+-rw-r--r--   0        0        0     8081 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/bbcode.py
+-rw-r--r--   0        0        0     5415 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/bot.py
+-rw-r--r--   0        0        0      675 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/config.py
+-rw-r--r--   0        0        0      158 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/const.py
+-rw-r--r--   0        0        0    11139 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/event.py
+-rw-r--r--   0        0        0     1517 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/exception.py
+-rw-r--r--   0        0        0    11160 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/message.py
+-rw-r--r--   0        0        0     5976 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/model.py
+-rw-r--r--   0        0        0      374 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/permission.py
+-rw-r--r--   0        0        0      456 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/rule.py
+-rw-r--r--   0        0        0     2103 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/util.py
+-rw-r--r--   0        0        0     1407 2024-05-11 08:27:36.450628 nonebot_adapter_tailchat-0.1.0b7/pyproject.toml
+-rw-r--r--   0        0        0     2493 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b7/PKG-INFO
```

### Comparing `nonebot_adapter_tailchat-0.1.0b6/LICENSE` & `nonebot_adapter_tailchat-0.1.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b6/README.md` & `nonebot_adapter_tailchat-0.1.0b7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/adapter.py` & `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/api.py` & `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from abc import ABC
 from typing import Any, Literal, Union
 
 from nonebot.adapters import Bot as BaseBot
 from pydantic import TypeAdapter
 
 from .const import Optional, Undefined
-from .message import Message
 from .model import (
     Ack,
     AddFriendRequestRet,
     BaseGroupInfo,
     ClientConfig,
     ConverseInfo,
     FileInfo,
@@ -25,15 +24,15 @@
     TokenInfo,
     UserInfo,
     Whoami,
 )
 
 
 class API(BaseBot, ABC):
-    async def ackAll(self) -> list[Ack]:
+    async def allAck(self) -> list[Ack]:
         """获取所有会话的最后一条消息的ID"""
         return TypeAdapter(list[Ack]).validate_python(await self.call_api("chat.ack.all"))
 
     async def allApp(self):
         """获取当前账号全部openapi app信息"""
         return await self.call_api("openapi.app.all")
 
@@ -49,17 +48,17 @@
         """获取文件url (但是参数不知道填啥)"""
         return await self.call_api("file.get", objectName=objectName)
 
     async def ackInbox(self, *, inboxItemIds: list[str]):
         """标记消息为已读"""
         return await self.call_api("chat.inbox.ack", inboxItemIds=inboxItemIds)
 
-    async def allInbox(self) -> Message:
+    async def allInbox(self) -> MessageRet:
         """获取用户收件箱中所有内容"""
-        return TypeAdapter(Message).validate_python(await self.call_api("chat.inbox.all"))
+        return TypeAdapter(MessageRet).validate_python(await self.call_api("chat.inbox.all"))
 
     async def isMember(self, *, groupId: str):
         """是否为指定群的成员"""
         return await self.call_api("group.isMember", groupId=groupId)
 
     async def register(
         self,
@@ -242,33 +241,35 @@
         [{'id': '***'}]"""
         return await self.call_api("friend.getAllFriends")
 
     async def getUserGroups(self) -> list[GroupInfo]:
         """获取用户的群组"""
         return TypeAdapter(list[GroupInfo]).validate_python(await self.call_api("group.getUserGroups"))
 
-    async def recallMessage(self, *, messageId: str) -> Message:
+    async def recallMessage(self, *, messageId: str) -> MessageRet:
         """撤回消息, 大于15分钟的消息无法撤回, 会报错"""
-        return TypeAdapter(Message).validate_python(
+        return TypeAdapter(MessageRet).validate_python(
             await self.call_api("chat.message.recallMessage", messageId=messageId)
         )
 
     async def resetPassword(self, *, otp: str, email: str, password: str):
         return await self.call_api("user.resetPassword", otp=otp, email=email, password=password)
 
     async def saveGroupData(self, *, data: str, name: str, groupId: str):
         return await self.call_api("group.extra.saveGroupData", data=data, name=name, groupId=groupId)
 
     async def savePanelData(self, *, data: str, name: str, groupId: str, panelId: str):
         """保存面板数据"""
         return await self.call_api("group.extra.savePanelData", data=data, name=name, groupId=groupId, panelId=panelId)
 
-    async def searchMessage(self, *, text: str, converseId: str, groupId: Optional[str] = Undefined) -> list[Message]:
+    async def searchMessage(
+        self, *, text: str, converseId: str, groupId: Optional[str] = Undefined
+    ) -> list[MessageRet]:
         """搜索消息"""
-        return TypeAdapter(list[Message]).validate_python(
+        return TypeAdapter(list[MessageRet]).validate_python(
             await self.call_api("chat.message.searchMessage", text=text, groupId=groupId, converseId=converseId)
         )
 
     async def setAppBotInfo(self, *, appId: str, fieldName: str, fieldValue: Any):
         return await self.call_api("openapi.app.setAppBotInfo", appId=appId, fieldName=fieldName, fieldValue=fieldValue)
 
     async def forgetPassword(self, *, email: str):
@@ -363,27 +364,29 @@
             await self.call_api("chat.converse.createDMConverse", memberIds=memberIds)
         )
 
     async def createGroupPanel(
         self,
         *,
         name: str,
-        meta: dict,
         type_: int,
         groupId: str,
+        meta: Optional[dict] = Undefined,
+        parentId: Optional[str] = Undefined,
         provider: Optional[str] = Undefined,
         pluginPanelName: Optional[str] = Undefined,
     ):
         """创建群组面板"""
         return await self.call_api(
             "group.createGroupPanel",
-            meta=meta,
             name=name,
+            meta=meta,
             type=type_,
             groupId=groupId,
+            parentId=parentId,
             provider=provider,
             pluginPanelName=pluginPanelName,
         )
 
     async def deleteGroupPanel(self, *, groupId: str, panelId: str) -> GroupInfo:
         """删除群组面板"""
         return TypeAdapter(GroupInfo).validate_python(
@@ -482,19 +485,21 @@
             email=email,
             userId=userId,
             emailOTP=emailOTP,
             password=password,
             username=username,
         )
 
-    async def fetchNearbyMessage(self, *, groupId: str, messageId: str, converseId: str) -> list[Message]:
+    async def fetchNearbyMessage(
+        self, *, messageId: str, converseId: str, num: Optional[int] = Undefined, groupId: Optional[str] = Undefined
+    ) -> list[MessageRet]:
         """获取指定消息的上下文"""
-        return TypeAdapter(list[Message]).validate_python(
+        return TypeAdapter(list[MessageRet]).validate_python(
             await self.call_api(
-                "chat.message.fetchNearbyMessage", groupId=groupId, messageId=messageId, converseId=converseId
+                "chat.message.fetchNearbyMessage", num=num, groupId=groupId, messageId=messageId, converseId=converseId
             )
         )
 
     async def verifyEmailWithOTP(self, *, emailOTP: str):
         """验证邮箱"""
         return await self.call_api("user.verifyEmailWithOTP", emailOTP=emailOTP)
 
@@ -510,18 +515,18 @@
 
     async def updateGroupRoleName(self, *, roleId: str, groupId: str, roleName: str) -> GroupInfo:
         """更新群用户组名称"""
         return TypeAdapter(GroupInfo).validate_python(
             await self.call_api("group.updateGroupRoleName", roleId=roleId, groupId=groupId, roleName=roleName)
         )
 
-    async def fetchConverseMessage(self, *, converseId: str) -> list[Message]:
+    async def fetchConverseMessage(self, *, converseId: str, startId: Optional[str] = Undefined) -> list[MessageRet]:
         """获取会话消息"""
-        return TypeAdapter(list[Message]).validate_python(
-            await self.call_api("chat.message.fetchConverseMessage", converseId=converseId)
+        return TypeAdapter(list[MessageRet]).validate_python(
+            await self.call_api("chat.message.fetchConverseMessage", startId=startId, converseId=converseId)
         )
 
     async def getAllGroupInviteCode(self, *, groupId: str) -> list[InviteCodeInfo]:
         """获取所有群组邀请码"""
         return TypeAdapter(list[InviteCodeInfo]).validate_python(
             await self.call_api("group.invite.getAllGroupInviteCode", groupId=groupId)
         )
```

### Comparing `nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/bbcode.py` & `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/bbcode.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/bot.py` & `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/bot.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 from pydantic import TypeAdapter
 from socketio import AsyncClient as AsyncSocketClient
 from typing_extensions import override
 
 from .api import API
 from .config import BotInfo
 from .event import Event, MessageEvent
-from .message import Message, MessageSegment
+from .message import At, Message, MessageSegment
 from .model import (
     BaseBotInfo,
     JwtPayload,
     MessageRet,
     TokenInfo,
 )
+from .util import log
 
 if TYPE_CHECKING:
     from .adapter import Adapter
 
 
 def _with_update_info(func):
     @wraps(func)
@@ -42,15 +43,39 @@
     async def connect(self):
         return await self.sio.connect(
             url=self.url,
             auth={"token": self.base_info.jwt},
             transports=["websocket"],
         )
 
+    async def _check_is_to_me(self, event: Event):
+        try:
+            message: Message = event.get_message()
+            # at
+            seg: MessageSegment = message[0]
+            if seg.type == At.__name__.lower():
+                if seg.get_tag(At).main == event.self_id:
+                    event._isToMe = True
+                    message.pop(0)
+                return
+            # nickname
+            if seg.type == "text":
+                text = seg.get_text().strip()
+                for i in self.config.nickname:
+                    if text.startswith(i):
+                        event._isToMe = True
+                        if len(text) == len(i):
+                            message.pop(0)
+                        else:
+                            seg.data["text"] = text[len(i) :]
+        except Exception as e:
+            log.debug(f"Bot._check_is_to_me error: {e}")
+
     async def handle_event(self, event: Event) -> None:
+        await self._check_is_to_me(event)
         await handle_event(self, event)
 
     @staticmethod
     def md5(text: str) -> str:
         return md5(text.encode()).hexdigest()
 
     @staticmethod
```

### Comparing `nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/config.py` & `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/event.py` & `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,29 +27,31 @@
 
 class Event(BaseEvent, ABC):
     event_name: str
     event_type: str
 
     self_id: ObjectId
 
+    _isToMe: bool = False
+
     @override
     def get_type(self) -> str:
         return self.event_type
 
     @override
     def get_event_name(self) -> str:
         return self.event_name
 
     @override
     def get_event_description(self) -> str:
         return str(model_dump(self))
 
     @override
     def is_tome(self) -> bool:
-        return not self.is_self() and self._is_tome
+        return not self.is_self() and (self._isToMe or self._is_tome)
 
     @property
     @abstractmethod
     def _is_tome(self) -> bool:
         return True
 
     def is_self(self) -> bool:
@@ -116,15 +118,17 @@
         raise ValueError("Unknown event has no context!")
 
     def get_session_id(self) -> str:
         raise ValueError("Unknown event has no context!")
 
     def get_message(self) -> "Message":
         if hasattr(self, "content"):
-            return Message(self.content)
+            if not isinstance(self.content, Message):
+                setattr(self, "content", Message(self.content))
+            return self.content
         raise ValueError("Unknown event has no message content")
 
 
 EVENT_CLASSES: dict[str, type[Event]] = {}
 
 E = TypeVar("E", bound=Event)
 
@@ -225,15 +229,15 @@
 
 @register_event_class
 class RemoveGroupEvent(GroupInfoEvent):
     """机器人退群事件"""
 
     event_name: Literal["notify:group.remove"]
 
-    groupId: str
+    groupId: ObjectId
 
     @property
     def _is_tome(self) -> bool:
         return True
 
     def get_user_id(self) -> str:
         return self.self_id
@@ -274,51 +278,56 @@
 
 @register_event_class
 class ReactionRemoveEvent(ReactionEvent):
     event_name: Literal["notify:chat.message.removeReaction"]
 
 
 class DefaultMessageEvent(MessageEvent):
-    def get_message_id(self) -> str:
-        return self.id
-
-    def get_converse_id(self) -> str:
-        return self.converseId
-
-    def get_group_id(self) -> Optional[str]:
-        return self.groupId
-
     id: ObjectId = Field(alias="_id")
     author: ObjectId
     hasRecall: bool
     converseId: ObjectId
     meta: Optional[MessageMeta] = Field(default=None)
 
     content: Message
     raw_content: str = Field(alias="content")
     reactions: list[Reaction]
     createdAt: datetime
     updatedAt: datetime
 
-    groupId: Optional[str] = Field(default=None)
+    groupId: Optional[ObjectId] = Field(default=None)
+
+    def get_message_id(self) -> str:
+        return self.id
+
+    def get_converse_id(self) -> str:
+        return self.converseId
+
+    def get_group_id(self) -> Optional[str]:
+        return self.groupId
 
     @property
     def replay(self) -> Optional[Replay]:
         return self.meta.replay if self.meta else None
 
     @override
     def get_message(self) -> Message:
         return self.content
 
     @override
     def get_user_id(self) -> str:
         return self.author
 
     def _is_tome(self) -> bool:
-        return not self.is_group() or (self.meta and self.self_id in self.meta.mentions)
+        # 私聊/提及/回复
+        return (
+            not self.is_group()
+            or (self.meta and self.self_id in self.meta.mentions)
+            or (self.meta and self.meta.replay and self.self_id == self.meta.replay.author)
+        )
 
     @override
     def get_event_description(self) -> str:
         return (
             f"Message {self.id} from {self.author}"
             + (f"@[群:{self.groupId}]" if self.groupId else "")
             + f" {self.content.show()}"
```

### Comparing `nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/exception.py` & `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,26 +25,26 @@
     def __init__(self, *, name: Optional[str], code: Optional[int] = None, message: Optional[str] = None):
         super(TailchatAdapterException).__init__()
         self.name = name
         self.code = code
         self.message = message
 
     def __repr__(self) -> str:
-        return f"{self.__name__}(name={self.name!r}, code={self.code!r}, message={self.message!r})"
+        return f"{self.__class__.__name__}(name={self.name!r}, code={self.code!r}, message={self.message!r})"
 
 
 class DisconnectException(TailchatAdapterException): ...
 
 
 class ConnectionException(TailchatAdapterException):
     def __init__(self, message: str):
         self.message = message
 
     def __repr__(self) -> str:
-        return f"{self.__name__}(message={self.message!r})"
+        return f"{self.__class__.__name__}(message={self.message!r})"
 
 
 class Error(ActionFailed):
     """通用错误"""
 
 
 class DataNotFoundError(ActionFailed):
```

### Comparing `nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/message.py` & `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,18 @@
     MessageSegment as BaseMessageSegment,
 )
 from typing_extensions import Self, override
 
 from .bbcode import Parser
 
 B = TypeVar("B", bound="BBCode")
-TEXTS: set[str] = set()
 BBCODES: dict[str, type[B]] = {}
 RELATION: dict[int, list[B]] = defaultdict(list)
 
 
-def _register_text(bbcode: type[B]) -> type[B]:
-    TEXTS.update(bbcode.tags)
-    return bbcode
-
-
 def _register_bbcode(code: Union[int, type[B]]):
     if isinstance(code, int):
 
         def _(bbcode: type[B]) -> type[B]:
             bbcode.relation = code
             for tag in bbcode.tags:
                 BBCODES[tag] = bbcode
@@ -133,33 +127,29 @@
 
 
 @_register_bbcode
 class Emoji(BBCode):
     tags = {"emoji"}
 
 
-@_register_text
 @_register_bbcode(0)
 class Bold(BBCode):
     tags = {"b"}
 
 
-@_register_text
 @_register_bbcode(0)
 class Italic(BBCode):
     tags = {"i"}
 
 
-@_register_text
 @_register_bbcode(0)
 class Underline(BBCode):
     tags = {"u"}
 
 
-@_register_text
 @_register_bbcode(0)
 class Strikeout(BBCode):
     tags = {"s"}
 
 
 @_register_bbcode
 class At(BBCode):
@@ -213,15 +203,15 @@
         return self.data["text"]
 
     def set_text(self, text: str):
         self.data["text"] = text
 
     @override
     def is_text(self) -> bool:
-        return not any(not (_.tags & TEXTS) for _ in self.data["tags"])
+        return self.type == "text"
 
     @classmethod
     def card(cls, *, text: str, type_: str, data: str) -> Self:
         return cls.build(text, [Card], {"type": type_, "data": data})
 
     @classmethod
     def at(cls, *, uid: str, nickname: Optional[str] = None) -> Self:
@@ -271,15 +261,25 @@
     def md(cls, text: str) -> Self:
         return cls.build(text, [Markdown])
 
     @classmethod
     def build(cls, text: str, tags: list[type[B]], extra: Optional[dict[str, str]] = None) -> Self:
         if extra is None:
             extra = {}
-        _ = cls("rich" if len(tags) > 0 else "text", {"text": text, "extra": extra, "tags": []})
+        if (length := len(tags)) == 0:
+            type_ = "text"
+        elif length == 1:
+            type_ = tags[0].__name__.lower()
+        else:
+            type_ = "rich"
+
+        _ = cls(
+            type_,
+            {"text": text, "extra": extra, "tags": []},
+        )
         for tag in tags:
             _.data["tags"].append(tag(box=_.data))
         return _
 
     def tag_relation(self) -> set[int]:
         return {_.relation for _ in self.data["tags"]}
 
@@ -292,14 +292,20 @@
         新消息段的 text = self.text or seg.text
         :param seg: 要合并的消息段
         :param strict: 严格模式
         :return: 新消息段
         """
         if strict and (relations := self.tag_relation()) and any(_.relation not in relations for _ in seg.data["tags"]):
             raise ValueError("Tag relation not match")
+
+        if self.type == "text":
+            self.type = seg.type
+        elif self.type != "rich":
+            self.type = "rich"
+
         self.data["extra"].update(seg.data["extra"])
         for idx, tag in enumerate(seg.data["tags"]):
             seg.data["tags"][idx] = tag.__class__(box=self.data)
         self.data["tags"].extend(seg.data["tags"])
         self.set_text(self.get_text() or seg.get_text())
         return self
 
@@ -317,15 +323,15 @@
         if bbcode is type[B]:
             bbcode: B = self.get_tag(bbcode)
         self.data["text"] = str(bbcode)
         return self.remove(bbcode)
 
     def get_tag(self, bbcode: type[B]) -> Optional[B]:
         for _ in self.data["tags"]:
-            if _ is bbcode:
+            if isinstance(_, bbcode):
                 return _
         return None
 
     def get_tags(self) -> list[B]:
         return self.data["tags"]
 
     def decode(self) -> str:
@@ -384,19 +390,14 @@
         cls.parser = Parser(MessageSegment, BBCODES)
 
     @classmethod
     def register_bbcode(cls, code: Union[int, type[B]]):
         _register_bbcode(code)
         cls.update_parser()
 
-    @staticmethod
-    def register_text(bbcode: type[B]) -> type[B]:
-        """注册文本类型"""
-        return _register_text(bbcode)
-
     @override
     def __contains__(  # pyright: ignore[reportIncompatibleMethodOverride]
         self, value: Union[MessageSegment, str, type[B]]
     ) -> bool:
         if issubclass(value, BBCode):
             return value.tag_in(self)
         return super().__contains__(value)
```

### Comparing `nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/model.py` & `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     discriminator: Optional[str] = None
 
 
 TemporaryUserInfo = TokenInfo
 
 
 class MessageRet(RawModel):
-    _id: str
+    id: str = Field(alias="_id")
     content: str
     author: str
     converseId: str
     hasRecall: bool
     reactions: list[Reaction]
     createdAt: datetime
     updatedAt: datetime
@@ -194,15 +194,15 @@
     language: str
     user: BaseUserInfo
     token: str
     userId: str
 
 
 class ConverseInfo(RawModel):
-    _id: str
+    id: str = Field(alias="_id")
     type: str
     members: list[str]
     createdAt: datetime
     updatedAt: datetime
 
     v: int = Field(alias="__v")
 
@@ -256,15 +256,15 @@
 class FileInfo(RawModel):
     etag: str
     path: str
     url: str
 
 
 class InviteCodeInfo(RawModel):
-    _id: str
+    id: str = Field(alias="_id")
     code: str
     creator: str
     groupId: str
     usage: int
     createdAt: datetime
     updatedAt: datetime
 
@@ -274,21 +274,27 @@
 class BaseGroupInfo(RawModel):
     name: str
     owner: str
     description: str
     memberCount: int
 
 
+class Role(RawModel):
+    id: str = Field(alias="_id")
+    name: str
+    permissions: list[str]
+
+
 class GroupInfo(RawModel):
     id: str = Field(alias="_id")
     name: str
     owner: str
     members: list[MemberInfo]
     panels: list[Panel]
-    roles: list[str]
+    roles: list[Role]
     fallbackPermissions: list[str]
     createdAt: datetime
     updatedAt: datetime
 
     v: int = Field(alias="__v")
 
     config: Optional[dict] = None
```

### Comparing `nonebot_adapter_tailchat-0.1.0b6/nonebot_adapter_tailchat/util.py` & `nonebot_adapter_tailchat-0.1.0b7/nonebot_adapter_tailchat/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b6/pyproject.toml` & `nonebot_adapter_tailchat-0.1.0b7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 [tool.poetry]
 name = "nonebot-adapter-tailchat"
-version = "0.1.0b6"
+version = "0.1.0b7"
 description = "NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2"
 authors = ["eya46 <61458340+eya46@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "nonebot_adapter_tailchat" }]
+keywords = ["bot", "tailchat", "nonebot2"]
+repository = "https://github.com/eya46/nonebot-adapter-tailchat"
+
+
+[tool.poetry.urls]
+"Tailchat" = "https://tailchat.msgbyte.com/"
+
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = ">=2.3.0"
 pydantic = ">=2.0.0"
 python-socketio = { extras = ["asyncio-client"], version = "^5.11.2" }
 msgpack = "^1.0.8"
```

### Comparing `nonebot_adapter_tailchat-0.1.0b6/PKG-INFO` & `nonebot_adapter_tailchat-0.1.0b7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-tailchat
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2
+Home-page: https://github.com/eya46/nonebot-adapter-tailchat
 License: Apache-2.0
+Keywords: bot,tailchat,nonebot2
 Author: eya46
 Author-email: 61458340+eya46@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: msgpack (>=1.0.8,<2.0.0)
 Requires-Dist: nonebot2 (>=2.3.0)
 Requires-Dist: pydantic (>=2.0.0)
 Requires-Dist: python-socketio[asyncio-client] (>=5.11.2,<6.0.0)
+Project-URL: Repository, https://github.com/eya46/nonebot-adapter-tailchat
+Project-URL: Tailchat, https://tailchat.msgbyte.com/
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://nonebot.dev/"><img src="https://nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b6 Summary:
-NoneBot2 Tailchat ééå¨ / Tailchat adapter for nonebot2 License: Apache-2.0
-Author: eya46 Author-email: 61458340+eya46@users.noreply.github.com Requires-
-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: msgpack (>=1.0.8,<2.0.0) Requires-
-Dist: nonebot2 (>=2.3.0) Requires-Dist: pydantic (>=2.0.0) Requires-Dist:
-python-socketio[asyncio-client] (>=5.11.2,<6.0.0) Description-Content-Type:
-text/markdown
+Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b7 Summary:
+NoneBot2 Tailchat ééå¨ / Tailchat adapter for nonebot2 Home-page: https://
+github.com/eya46/nonebot-adapter-tailchat License: Apache-2.0 Keywords:
+bot,tailchat,nonebot2 Author: eya46 Author-email:
+61458340+eya46@users.noreply.github.com Requires-Python: >=3.9,<4.0 Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: msgpack (>=1.0.8,<2.0.0) Requires-Dist: nonebot2 (>=2.3.0)
+Requires-Dist: pydantic (>=2.0.0) Requires-Dist: python-socketio[asyncio-
+client] (>=5.11.2,<6.0.0) Project-URL: Repository, https://github.com/eya46/
+nonebot-adapter-tailchat Project-URL: Tailchat, https://tailchat.msgbyte.com/
+Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
      # Nonebot Adapter Tailchat ## Tailchat ééå¨ ![License](https://
 img.shields.io/github/license/eya46/nonebot-adapter-tailchat) ![Python](https:/
 /img.shields.io/badge/python-3.9+-blue.svg) ![NoneBot](https://img.shields.io/
                          badge/nonebot-2.3.0+-red.svg)
 ## ç¯å¢è¦æ± - Python 3.9+ - NoneBot 2.3.0+ - pydantic >= 2.0.0 -
 HTTPClienté©±å¨å¨ - > é»è®¤éè¦,é¤é `useHttp=False`, ä¸éç½®äº `jwt`
```

