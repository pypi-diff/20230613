# Comparing `tmp/revolt.py-0.1.8.tar.gz` & `tmp/revolt.py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revolt.py-0.1.8.tar", max compression
+gzip compressed data, was "revolt.py-0.1.9.tar", max compression
```

## Comparing `revolt.py-0.1.8.tar` & `revolt.py-0.1.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rwxr-xr-x   0        0        0     1060 2021-08-17 23:20:51.907694 revolt.py-0.1.8/LICENSE
--rwxr-xr-x   0        0        0     1011 2022-03-23 22:01:12.138959 revolt.py-0.1.8/README.md
--rwxr-xr-x   0        0        0     1471 2022-06-23 01:09:44.789470 revolt.py-0.1.8/pyproject.toml
--rwxr-xr-x   0        0        0      423 2022-06-23 01:09:54.190405 revolt.py-0.1.8/revolt/__init__.py
--rwxr-xr-x   0        0        0     3615 2022-04-25 12:40:59.362547 revolt.py-0.1.8/revolt/asset.py
--rwxr-xr-x   0        0        0      954 2021-11-13 23:58:47.525700 revolt.py-0.1.8/revolt/category.py
--rwxr-xr-x   0        0        0    10785 2022-05-31 00:46:44.723699 revolt.py-0.1.8/revolt/channel.py
--rwxr-xr-x   0        0        0    10584 2022-04-25 12:41:14.561495 revolt.py-0.1.8/revolt/client.py
--rwxr-xr-x   0        0        0     3210 2022-04-25 12:40:10.550593 revolt.py-0.1.8/revolt/embed.py
--rwxr-xr-x   0        0        0     1198 2022-03-23 22:46:24.794731 revolt.py-0.1.8/revolt/enums.py
--rwxr-xr-x   0        0        0      477 2022-04-25 12:31:38.788467 revolt.py-0.1.8/revolt/errors.py
--rwxr-xr-x   0        0        0        0 2021-10-17 00:52:49.549872 revolt.py-0.1.8/revolt/ext/__init__.py
--rwxr-xr-x   0        0        0      198 2022-04-25 12:40:10.640318 revolt.py-0.1.8/revolt/ext/commands/__init__.py
--rwxr-xr-x   0        0        0     1632 2022-02-10 06:38:18.162889 revolt.py-0.1.8/revolt/ext/commands/checks.py
--rwxr-xr-x   0        0        0    10086 2022-04-25 12:40:10.616440 revolt.py-0.1.8/revolt/ext/commands/client.py
--rwxr-xr-x   0        0        0     1673 2022-04-25 12:40:10.618645 revolt.py-0.1.8/revolt/ext/commands/cog.py
--rwxr-xr-x   0        0        0     8785 2022-04-25 12:40:10.621931 revolt.py-0.1.8/revolt/ext/commands/command.py
--rwxr-xr-x   0        0        0     3311 2022-03-30 17:27:30.223137 revolt.py-0.1.8/revolt/ext/commands/context.py
--rwxr-xr-x   0        0        0     2744 2022-01-21 23:47:55.013058 revolt.py-0.1.8/revolt/ext/commands/converters.py
--rwxr-xr-x   0        0        0     2497 2022-02-14 05:54:30.771351 revolt.py-0.1.8/revolt/ext/commands/errors.py
--rwxr-xr-x   0        0        0     4263 2022-04-25 12:40:10.631478 revolt.py-0.1.8/revolt/ext/commands/group.py
--rwxr-xr-x   0        0        0     6959 2022-04-25 12:40:10.635258 revolt.py-0.1.8/revolt/ext/commands/help.py
--rwxr-xr-x   0        0        0      533 2022-04-25 12:40:10.636783 revolt.py-0.1.8/revolt/ext/commands/utils.py
--rwxr-xr-x   0        0        0     1254 2022-03-23 21:47:17.015355 revolt.py-0.1.8/revolt/ext/commands/view.py
--rwxr-xr-x   0        0        0     1201 2022-04-25 12:41:25.751978 revolt.py-0.1.8/revolt/file.py
--rwxr-xr-x   0        0        0     4201 2022-05-08 22:20:07.704844 revolt.py-0.1.8/revolt/flags.py
--rwxr-xr-x   0        0        0    14248 2022-05-13 18:29:20.204448 revolt.py-0.1.8/revolt/http.py
--rwxr-xr-x   0        0        0     2054 2022-01-21 21:19:56.554850 revolt.py-0.1.8/revolt/invite.py
--rwxr-xr-x   0        0        0     3028 2022-04-25 12:41:35.246157 revolt.py-0.1.8/revolt/member.py
--rwxr-xr-x   0        0        0     6271 2022-04-25 12:40:10.574695 revolt.py-0.1.8/revolt/message.py
--rwxr-xr-x   0        0        0     5036 2022-02-10 02:34:01.746647 revolt.py-0.1.8/revolt/messageable.py
--rwxr-xr-x   0        0        0     4919 2022-05-31 00:48:37.099378 revolt.py-0.1.8/revolt/permissions.py
--rwxr-xr-x   0        0        0        0 2021-10-29 08:12:41.387687 revolt.py-0.1.8/revolt/py.typed
--rwxr-xr-x   0        0        0     2910 2022-05-13 18:28:51.579487 revolt.py-0.1.8/revolt/role.py
--rwxr-xr-x   0        0        0    11749 2022-05-13 18:57:37.931132 revolt.py-0.1.8/revolt/server.py
--rwxr-xr-x   0        0        0     2941 2022-03-28 01:55:26.257490 revolt.py-0.1.8/revolt/state.py
--rwxr-xr-x   0        0        0      295 2022-05-31 00:37:24.976742 revolt.py-0.1.8/revolt/types/__init__.py
--rwxr-xr-x   0        0        0      201 2021-10-28 02:14:11.366205 revolt.py-0.1.8/revolt/types/category.py
--rwxr-xr-x   0        0        0     1613 2022-05-13 16:48:09.168897 revolt.py-0.1.8/revolt/types/channel.py
--rwxr-xr-x   0        0        0     2242 2022-04-25 12:40:10.652053 revolt.py-0.1.8/revolt/types/embed.py
--rwxr-xr-x   0        0        0      478 2021-09-03 21:35:21.413212 revolt.py-0.1.8/revolt/types/file.py
--rwxr-xr-x   0        0        0     4797 2022-05-31 00:35:49.056958 revolt.py-0.1.8/revolt/types/gateway.py
--rwxr-xr-x   0        0        0      913 2022-04-02 17:42:15.080571 revolt.py-0.1.8/revolt/types/http.py
--rwxr-xr-x   0        0        0      638 2022-02-14 04:26:21.238471 revolt.py-0.1.8/revolt/types/invite.py
--rwxr-xr-x   0        0        0      390 2022-04-25 12:40:10.662354 revolt.py-0.1.8/revolt/types/member.py
--rwxr-xr-x   0        0        0     1513 2022-04-25 12:40:10.664577 revolt.py-0.1.8/revolt/types/message.py
--rwxr-xr-x   0        0        0      116 2022-05-08 21:06:45.374322 revolt.py-0.1.8/revolt/types/permissions.py
--rwxr-xr-x   0        0        0      344 2022-05-13 16:40:49.463811 revolt.py-0.1.8/revolt/types/role.py
--rwxr-xr-x   0        0        0     1202 2022-05-13 18:18:45.677387 revolt.py-0.1.8/revolt/types/server.py
--rwxr-xr-x   0        0        0     1011 2022-04-25 12:40:10.670419 revolt.py-0.1.8/revolt/types/user.py
--rwxr-xr-x   0        0        0     6278 2022-04-25 12:41:53.317340 revolt.py-0.1.8/revolt/user.py
--rwxr-xr-x   0        0        0     2859 2022-04-25 12:40:10.595904 revolt.py-0.1.8/revolt/utils.py
--rwxr-xr-x   0        0        0    11219 2022-04-25 12:40:10.602744 revolt.py-0.1.8/revolt/websocket.py
--rw-r--r--   0        0        0     2015 2022-06-23 01:12:32.375649 revolt.py-0.1.8/setup.py
--rw-r--r--   0        0        0     2337 2022-06-23 01:12:32.376002 revolt.py-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1060 2021-08-17 23:20:51.907694 revolt.py-0.1.9/LICENSE
+-rwxr-xr-x   0        0        0     1011 2022-03-23 22:01:12.138959 revolt.py-0.1.9/README.md
+-rwxr-xr-x   0        0        0     1471 2022-08-08 18:25:13.673734 revolt.py-0.1.9/pyproject.toml
+-rwxr-xr-x   0        0        0      423 2022-08-08 18:25:37.688215 revolt.py-0.1.9/revolt/__init__.py
+-rwxr-xr-x   0        0        0     3615 2022-04-25 12:40:59.362547 revolt.py-0.1.9/revolt/asset.py
+-rwxr-xr-x   0        0        0      954 2021-11-13 23:58:47.525700 revolt.py-0.1.9/revolt/category.py
+-rwxr-xr-x   0        0        0    12761 2022-07-15 22:24:00.524322 revolt.py-0.1.9/revolt/channel.py
+-rwxr-xr-x   0        0        0    10584 2022-07-15 21:38:17.237984 revolt.py-0.1.9/revolt/client.py
+-rwxr-xr-x   0        0        0     3210 2022-04-25 12:40:10.550593 revolt.py-0.1.9/revolt/embed.py
+-rwxr-xr-x   0        0        0     1198 2022-03-23 22:46:24.794731 revolt.py-0.1.9/revolt/enums.py
+-rwxr-xr-x   0        0        0      477 2022-04-25 12:31:38.788467 revolt.py-0.1.9/revolt/errors.py
+-rwxr-xr-x   0        0        0        0 2021-10-17 00:52:49.549872 revolt.py-0.1.9/revolt/ext/__init__.py
+-rwxr-xr-x   0        0        0      198 2022-04-25 12:40:10.640318 revolt.py-0.1.9/revolt/ext/commands/__init__.py
+-rwxr-xr-x   0        0        0     1632 2022-02-10 06:38:18.162889 revolt.py-0.1.9/revolt/ext/commands/checks.py
+-rwxr-xr-x   0        0        0    10086 2022-04-25 12:40:10.616440 revolt.py-0.1.9/revolt/ext/commands/client.py
+-rwxr-xr-x   0        0        0     1673 2022-04-25 12:40:10.618645 revolt.py-0.1.9/revolt/ext/commands/cog.py
+-rwxr-xr-x   0        0        0     8785 2022-04-25 12:40:10.621931 revolt.py-0.1.9/revolt/ext/commands/command.py
+-rwxr-xr-x   0        0        0     3311 2022-03-30 17:27:30.223137 revolt.py-0.1.9/revolt/ext/commands/context.py
+-rwxr-xr-x   0        0        0     2744 2022-01-21 23:47:55.013058 revolt.py-0.1.9/revolt/ext/commands/converters.py
+-rwxr-xr-x   0        0        0     2497 2022-02-14 05:54:30.771351 revolt.py-0.1.9/revolt/ext/commands/errors.py
+-rwxr-xr-x   0        0        0     4263 2022-04-25 12:40:10.631478 revolt.py-0.1.9/revolt/ext/commands/group.py
+-rwxr-xr-x   0        0        0     6959 2022-04-25 12:40:10.635258 revolt.py-0.1.9/revolt/ext/commands/help.py
+-rwxr-xr-x   0        0        0      533 2022-04-25 12:40:10.636783 revolt.py-0.1.9/revolt/ext/commands/utils.py
+-rwxr-xr-x   0        0        0     1254 2022-03-23 21:47:17.015355 revolt.py-0.1.9/revolt/ext/commands/view.py
+-rwxr-xr-x   0        0        0     1201 2022-04-25 12:41:25.751978 revolt.py-0.1.9/revolt/file.py
+-rwxr-xr-x   0        0        0     4201 2022-05-08 22:20:07.704844 revolt.py-0.1.9/revolt/flags.py
+-rwxr-xr-x   0        0        0    14200 2022-07-15 22:37:02.975195 revolt.py-0.1.9/revolt/http.py
+-rwxr-xr-x   0        0        0     2054 2022-01-21 21:19:56.554850 revolt.py-0.1.9/revolt/invite.py
+-rwxr-xr-x   0        0        0     3207 2022-08-08 17:16:25.557556 revolt.py-0.1.9/revolt/member.py
+-rwxr-xr-x   0        0        0     6530 2022-08-08 18:22:19.489883 revolt.py-0.1.9/revolt/message.py
+-rwxr-xr-x   0        0        0     5036 2022-02-10 02:34:01.746647 revolt.py-0.1.9/revolt/messageable.py
+-rwxr-xr-x   0        0        0     4919 2022-05-31 00:48:37.099378 revolt.py-0.1.9/revolt/permissions.py
+-rwxr-xr-x   0        0        0        0 2021-10-29 08:12:41.387687 revolt.py-0.1.9/revolt/py.typed
+-rwxr-xr-x   0        0        0     2910 2022-07-15 21:38:17.240140 revolt.py-0.1.9/revolt/role.py
+-rwxr-xr-x   0        0        0    12177 2022-07-15 21:38:17.240989 revolt.py-0.1.9/revolt/server.py
+-rwxr-xr-x   0        0        0     3283 2022-08-08 17:30:43.600227 revolt.py-0.1.9/revolt/state.py
+-rwxr-xr-x   0        0        0      295 2022-05-31 00:37:24.976742 revolt.py-0.1.9/revolt/types/__init__.py
+-rwxr-xr-x   0        0        0      201 2021-10-28 02:14:11.366205 revolt.py-0.1.9/revolt/types/category.py
+-rwxr-xr-x   0        0        0     1750 2022-07-15 21:38:52.256173 revolt.py-0.1.9/revolt/types/channel.py
+-rwxr-xr-x   0        0        0     2242 2022-04-25 12:40:10.652053 revolt.py-0.1.9/revolt/types/embed.py
+-rwxr-xr-x   0        0        0      478 2021-09-03 21:35:21.413212 revolt.py-0.1.9/revolt/types/file.py
+-rwxr-xr-x   0        0        0     4934 2022-08-06 23:23:37.582094 revolt.py-0.1.9/revolt/types/gateway.py
+-rwxr-xr-x   0        0        0      913 2022-04-02 17:42:15.080571 revolt.py-0.1.9/revolt/types/http.py
+-rwxr-xr-x   0        0        0      638 2022-02-14 04:26:21.238471 revolt.py-0.1.9/revolt/types/invite.py
+-rwxr-xr-x   0        0        0      390 2022-04-25 12:40:10.662354 revolt.py-0.1.9/revolt/types/member.py
+-rwxr-xr-x   0        0        0     1529 2022-07-15 21:40:47.236552 revolt.py-0.1.9/revolt/types/message.py
+-rwxr-xr-x   0        0        0      116 2022-05-08 21:06:45.374322 revolt.py-0.1.9/revolt/types/permissions.py
+-rwxr-xr-x   0        0        0      344 2022-05-13 16:40:49.463811 revolt.py-0.1.9/revolt/types/role.py
+-rwxr-xr-x   0        0        0     1202 2022-05-13 18:18:45.677387 revolt.py-0.1.9/revolt/types/server.py
+-rwxr-xr-x   0        0        0     1011 2022-04-25 12:40:10.670419 revolt.py-0.1.9/revolt/types/user.py
+-rwxr-xr-x   0        0        0     6714 2022-08-08 17:21:07.603726 revolt.py-0.1.9/revolt/user.py
+-rwxr-xr-x   0        0        0     2859 2022-04-25 12:40:10.595904 revolt.py-0.1.9/revolt/utils.py
+-rwxr-xr-x   0        0        0    13286 2022-08-08 18:21:25.933788 revolt.py-0.1.9/revolt/websocket.py
+-rw-r--r--   0        0        0     2015 2022-08-08 18:32:04.653631 revolt.py-0.1.9/setup.py
+-rw-r--r--   0        0        0     2337 2022-08-08 18:32:04.653975 revolt.py-0.1.9/PKG-INFO
```

### Comparing `revolt.py-0.1.8/LICENSE` & `revolt.py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/README.md` & `revolt.py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/pyproject.toml` & `revolt.py-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "revolt.py"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python wrapper for the revolt.chat API"
 authors = ["Zomatee <me@zomatree.live>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/revoltchat/revolt.py"
 documentation = "https://revoltpy.readthedocs.io/en/latest/"
 classifiers = [
```

### Comparing `revolt.py-0.1.8/revolt/asset.py` & `revolt.py-0.1.9/revolt/asset.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/category.py` & `revolt.py-0.1.9/revolt/category.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/channel.py` & `revolt.py-0.1.9/revolt/channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,21 +30,45 @@
 class EditableChannel:
     __slots__ = ()
 
     state: State
     id: str
 
     async def edit(self, **kwargs):
+        """Edits the channel
+
+        Passing ``None`` to the parameters that accept it will remove them.
+
+        Parameters
+        -----------
+        name: str
+            The new name for the channel
+        description: Optional[str]
+            The new description for the channel
+        owner: User
+            The new owner for the group dm channel
+        icon: Optional[File]
+            The new icon for the channel
+        nsfw: bool
+            Sets whether the channel is nsfw or not
+        """
         if kwargs.get("icon", Missing) == None:
             remove = "Icon"
         elif kwargs.get("description", Missing) == None:
             remove = "Description"
         else:
             remove = None
 
+        if icon := kwargs.get("icon"):
+            asset = await self.state.http.upload_file(icon, "icons")
+            kwargs["icon"] = asset["id"]
+
+        if owner := kwargs.get("owner"):
+            kwargs["owner"] = owner.id
+
         await self.state.http.edit_channel(self.id, remove, kwargs)
 
 class Channel:
     """Base class for all channels
 
     Attributes
     -----------
@@ -89,17 +113,41 @@
 
 class SavedMessageChannel(Channel, Messageable):
     """The Saved Message Channel"""
     def __init__(self, data: SavedMessagesPayload, state: State):
         super().__init__(data, state)
 
 class DMChannel(Channel, Messageable):
-    """A DM channel"""
+    """A DM channel
+
+    Attributes
+    -----------
+    last_message_id: Optional[:class:`str`]
+        The id of the last message in this channel, if any
+    """
+
+    __slots__ = ("last_message_id",)
+
     def __init__(self, data: DMChannelPayload, state: State):
         super().__init__(data, state)
+        self.last_message_id = data.get("last_message_id")
+
+    @property
+    def last_message(self) -> Message:
+        """Gets the last message from the channel, shorthand for `client.get_message(channel.last_message_id)`
+
+        Returns
+        --------
+        :class:`Message` the last message in the channel
+        """
+
+        if not self.last_message_id:
+            raise LookupError
+
+        return self.state.get_message(self.last_message_id)
 
 class GroupDMChannel(Channel, Messageable, EditableChannel):
     """A group DM channel
 
     Attributes
     -----------
     recipients: list[:class:`User`]
@@ -110,24 +158,27 @@
         The user who created the group dm channel
     icon: Optional[:class:`Asset`]
         The icon of the group dm channel
     permissions: :class:`ChannelPermissions`
         The permissions of the users inside the group dm channel
     description: Optional[:class:`str`]
         The description of the channel, if any
+    last_message_id: Optional[:class:`str`]
+        The id of the last message in this channel, if any
     """
 
-    __slots__ = ("recipients", "name", "owner", "permissions", "icon", "description")
+    __slots__ = ("recipients", "name", "owner", "permissions", "icon", "description", "last_message_id")
 
     def __init__(self, data: GroupDMChannelPayload, state: State):
         super().__init__(data, state)
         self.recipients = [state.get_user(user_id) for user_id in data["recipients"]]
         self.name = data["name"]
         self.owner = state.get_user(data["owner"])
         self.description: Optional[str] = data.get("description")
+        self.last_message_id = data.get("last_message_id")
 
         if icon := data.get("icon"):
             self.icon = Asset(icon, state)
         else:
             self.icon = None
 
         self.permissions = Permissions(data.get("permissions", 0))
@@ -147,22 +198,37 @@
         Parameters
         -----------
         permissions: :class:`ChannelPermissions`
             The new default group permissions
         """
         await self.state.http.set_group_channel_default_permissions(self.id, permissions.value)
 
+    @property
+    def last_message(self) -> Message:
+        """Gets the last message from the channel, shorthand for `client.get_message(channel.last_message_id)`
+
+        Returns
+        --------
+        :class:`Message` the last message in the channel
+        """
+
+        if not self.last_message_id:
+            raise LookupError
+
+        return self.state.get_message(self.last_message_id)
+
 class GuildChannel(Channel):
     def __init__(self, data: GuildChannelPayload, state: State):
         super().__init__(data, state)
 
         self.server_id = data["server"]
         self.name = data["name"]
         self.description: Optional[str] = data.get("description")
-
+        self.nsfw = data.get("nsfw", False)
+        self.active = False
         self.default_permissions = PermissionsOverwrite._from_overwrite(data.get("default_permissions", {"a": 0, "d": 0}))
 
         permissions: dict[str, PermissionsOverwrite] = {}
 
         for role_name, overwrite_data in data.get("role_permissions", {}).items():
             overwrite = PermissionsOverwrite._from_overwrite(overwrite_data)
             permissions[role_name] = overwrite
@@ -219,16 +285,14 @@
 
             self.permissions = permissions
 
         if default_permissions is not None:
             self.default_permissions = default_permissions
 
 class TextChannel(GuildChannel, Messageable, EditableChannel):
-    __slots__ = ("name", "description", "last_message_id", "server_id", "default_permissions", "icon", "overwrites")
-
     """A text channel
 
     Attributes
     -----------
     name: :class:`str`
         The name of the text channel
     server_id: :class:`str`
@@ -240,19 +304,21 @@
     role_permissions: dict[:class:`str`, :class:`ChannelPermissions`]
         A dictionary of role id's to the permissions of that role in the text channel
     icon: Optional[:class:`Asset`]
         The icon of the text channel, if any
     description: Optional[:class:`str`]
         The description of the channel, if any
     """
+
+    __slots__ = ("name", "description", "last_message_id", "default_permissions", "icon", "overwrites")
+
     def __init__(self, data: TextChannelPayload, state: State):
         super().__init__(data, state)
 
-        last_message_id = data.get("last_message")
-        self.last_message_id = last_message_id
+        self.last_message_id = data.get("last_message_id")
 
     async def _get_channel_id(self) -> str:
         return self.id
 
     @property
     def last_message(self) -> Message:
         """Gets the last message from the channel, shorthand for `client.get_message(channel.last_message_id)`
```

### Comparing `revolt.py-0.1.8/revolt/client.py` & `revolt.py-0.1.9/revolt/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         """Edits the client's own user
 
         Parameters
         -----------
         avatar: Optional[:class:`File`]
             The avatar to change to, passing in ``None`` will remove the avatar
         """
-        if kwargs.get("avatar", Missing) == None:
+        if kwargs.get("avatar", Missing) is None:
             del kwargs["avatar"]
             remove = "Avatar"
         else:
             remove = None
 
         await self.state.http.edit_self(remove, kwargs)
 
@@ -314,15 +314,15 @@
         Parameters
         -----------
         presence: :class:`PresenceType`
             The presence to change to
         text: Optional[:class:`str`]
             The text to change the status to, passing in ``None`` will remove the status
         """
-        if kwargs.get("text", Missing) == None:
+        if kwargs.get("text", Missing) is None:
             del kwargs["text"]
             remove = "StatusText"
         else:
             remove = None
 
         if presence := kwargs.get("presence"):
             kwargs["presence"] = presence.value
@@ -335,17 +335,17 @@
         Parameters
         -----------
         content: Optional[:class:`str`]
             The new content for the profile, passing in ``None`` will remove the profile content
         background: Optional[:class:`File`]
             The new background for the profile, passing in ``None`` will remove the profile background
         """
-        if kwargs.get("content", Missing) == None:
+        if kwargs.get("content", Missing) is None:
             del kwargs["content"]
             remove = "ProfileContent"
-        elif kwargs.get("background", Missing) == None:
+        elif kwargs.get("background", Missing) is None:
             del kwargs["background"]
             remove = "ProfileBackground"
         else:
             remove = None
 
         await self.state.http.edit_self(remove, {"profile": kwargs})
```

### Comparing `revolt.py-0.1.8/revolt/embed.py` & `revolt.py-0.1.9/revolt/embed.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/enums.py` & `revolt.py-0.1.9/revolt/enums.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/checks.py` & `revolt.py-0.1.9/revolt/ext/commands/checks.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/client.py` & `revolt.py-0.1.9/revolt/ext/commands/client.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/cog.py` & `revolt.py-0.1.9/revolt/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/command.py` & `revolt.py-0.1.9/revolt/ext/commands/command.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/context.py` & `revolt.py-0.1.9/revolt/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/converters.py` & `revolt.py-0.1.9/revolt/ext/commands/converters.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/errors.py` & `revolt.py-0.1.9/revolt/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/group.py` & `revolt.py-0.1.9/revolt/ext/commands/group.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/help.py` & `revolt.py-0.1.9/revolt/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/utils.py` & `revolt.py-0.1.9/revolt/ext/commands/utils.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/ext/commands/view.py` & `revolt.py-0.1.9/revolt/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/file.py` & `revolt.py-0.1.9/revolt/file.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/flags.py` & `revolt.py-0.1.9/revolt/flags.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/http.py` & `revolt.py-0.1.9/revolt/http.py`

 * *Files 12% similar despite different names*

```diff
@@ -151,52 +151,52 @@
         return self.request("PATCH", f"/channels/{channel}/messages/{message}", json=json)
 
     def delete_message(self, channel: str, message: str) -> Request[None]:
         return self.request("DELETE", f"/channels/{channel}/messages/{message}")
 
     def fetch_message(self, channel: str, message: str) -> Request[MessagePayload]:
         return self.request("GET", f"/channels/{channel}/messages/{message}")
-    
+
     @overload
     def fetch_messages(
-        self, 
-        channel: str, 
+        self,
+        channel: str,
         sort: SortType,
-        *, 
-        limit: Optional[int] = ..., 
-        before: Optional[str] = ..., 
-        after: Optional[str] = ..., 
-        nearby: Optional[str] = ..., 
+        *,
+        limit: Optional[int] = ...,
+        before: Optional[str] = ...,
+        after: Optional[str] = ...,
+        nearby: Optional[str] = ...,
         include_users: Literal[False] = ...
     ) -> Request[list[MessagePayload]]:
         ...
-    
+
     @overload
     def fetch_messages(
-        self, 
-        channel: str, 
+        self,
+        channel: str,
         sort: SortType,
-        *, 
-        limit: Optional[int] = ..., 
-        before: Optional[str] = ..., 
-        after: Optional[str] = ..., 
-        nearby: Optional[str] = ..., 
+        *,
+        limit: Optional[int] = ...,
+        before: Optional[str] = ...,
+        after: Optional[str] = ...,
+        nearby: Optional[str] = ...,
         include_users: Literal[True] = ...
     ) -> Request[MessageWithUserData]:
         ...
 
     def fetch_messages(
-        self, 
-        channel: str, 
+        self,
+        channel: str,
         sort: SortType,
-        *, 
-        limit: Optional[int] = None, 
-        before: Optional[str] = None, 
-        after: Optional[str] = None, 
-        nearby: Optional[str] = None, 
+        *,
+        limit: Optional[int] = None,
+        before: Optional[str] = None,
+        after: Optional[str] = None,
+        nearby: Optional[str] = None,
         include_users: bool = False
     ) -> Request[Union[list[MessagePayload], MessageWithUserData]]:
 
         json = {"sort": sort.value, "include_users": str(include_users)}
 
         if limit:
             json["limit"] = limit
@@ -210,47 +210,47 @@
         if nearby:
             json["nearby"] = nearby
 
         return self.request("GET", f"/channels/{channel}/messages", params=json)
 
     @overload
     def search_messages(
-        self, 
-        channel: str, 
+        self,
+        channel: str,
         query: str,
-        *, 
-        limit: Optional[int] = ..., 
-        before: Optional[str] = ..., 
+        *,
+        limit: Optional[int] = ...,
+        before: Optional[str] = ...,
         after: Optional[str] = ...,
         sort: Optional[SortType] = ...,
         include_users: Literal[False] = ...
     ) -> Request[list[MessagePayload]]:
         ...
 
     @overload
     def search_messages(
-        self, 
-        channel: str, 
+        self,
+        channel: str,
         query: str,
-        *, 
-        limit: Optional[int] = ..., 
-        before: Optional[str] = ..., 
+        *,
+        limit: Optional[int] = ...,
+        before: Optional[str] = ...,
         after: Optional[str] = ...,
         sort: Optional[SortType] = ...,
         include_users: Literal[True] = ...
     ) -> Request[MessageWithUserData]:
         ...
 
     def search_messages(
-        self, 
-        channel: str, 
+        self,
+        channel: str,
         query: str,
-        *, 
-        limit: Optional[int] = None, 
-        before: Optional[str] = None, 
+        *,
+        limit: Optional[int] = None,
+        before: Optional[str] = None,
         after: Optional[str] = None,
         sort: Optional[SortType] = None,
         include_users: bool = False
     ) -> Request[Union[list[MessagePayload], MessageWithUserData]]:
 
         json = {"query": query, "include_users": include_users}
 
@@ -276,15 +276,15 @@
         return self.request("GET", f"/users/{user_id}")
 
     def fetch_profile(self, user_id: str) -> Request[UserProfile]:
         return self.request("GET", f"/users/{user_id}/profile")
 
     def fetch_default_avatar(self, user_id: str) -> Request[bytes]:
         return self.request_file(f"{self.api_url}/users/{user_id}/default_avatar")
-    
+
     def fetch_dm_channels(self) -> Request[list[Union[DMChannel, GroupDMChannel]]]:
         return self.request("GET", "/users/dms")
 
     def open_dm(self, user_id: str) -> Request[DMChannel]:
         return self.request("GET", f"/users/{user_id}/dm")
 
     def fetch_channel(self, channel_id: str) -> Request[Channel]:
```

### Comparing `revolt.py-0.1.8/revolt/invite.py` & `revolt.py-0.1.9/revolt/invite.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/member.py` & `revolt.py-0.1.9/revolt/member.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,28 +31,32 @@
     guild_avatar: Optional[:class:`Asset`]
         The member's guild avatar if any
     """
     __slots__ = ("_state", "nickname", "roles", "server", "guild_avatar")
 
     def __init__(self, data: MemberPayload, server: Server, state: State):
         user = state.get_user(data["_id"]["user"])
+
+        # due to not having a user payload and only a user object we have to manually add all the attributes instead of calling User.__init__
+
         flattern_user(self, user)
+        user._members.append(self)
 
         self._state = state
-        self.nickname = data.get("nickname")
 
         if avatar := data.get("avatar"):
             self.guild_avatar = Asset(avatar, state)
         else:
             self.guild_avatar = None
 
         roles = [server.get_role(role_id) for role_id in data.get("roles", [])]
         self.roles = sorted(roles, key=lambda role: role.rank, reverse=True)
 
         self.server = server
+        self.nickname = data.get("nickname")
 
     @property
     def avatar(self) -> Optional[Asset]:
         """Optional[:class:`Asset`] The avatar the member is displaying, this includes guild avatars and masqueraded avatar"""
         return self.masquerade_avatar or self.guild_avatar or self.original_avatar
 
     @property
```

### Comparing `revolt.py-0.1.8/revolt/message.py` & `revolt.py-0.1.9/revolt/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 if TYPE_CHECKING:
     from .state import State
     from .types import Embed as EmbedPayload
     from .types import Masquerade as MasqueradePayload
     from .types import Message as MessagePayload
     from .types import MessageReplyPayload
-
+    from .server import Server
 
 __all__ = (
     "Message",
     "MessageReply",
     "Masquerade"
 )
 
@@ -32,45 +32,41 @@
         The content of the message, this will not include system message's content
     attachments: list[:class:`Asset`]
         The attachments of the message
     embeds: list[Union[:class:`WebsiteEmbed`, :class:`ImageEmbed`, :class:`TextEmbed`, :class:`NoneEmbed`]]
         The embeds of the message
     channel: :class:`Messageable`
         The channel the message was sent in
-    server: :class:`Server`
-        The server the message was sent in
     author: Union[:class:`Member`, :class:`User`]
         The author of the message, will be :class:`User` in DMs
     edited_at: Optional[:class:`datetime.datetime`]
         The time at which the message was edited, will be None if the message has not been edited
     mentions: list[Union[:class:`Member`, :class:`User`]]
         The users or members that where mentioned in the message
     replies: list[:class:`Message`]
         The message's this message has replied to, this may not contain all the messages if they are outside the cache
     reply_ids: list[:class:`str`]
         The message's ids this message has replies to
     """
-    __slots__ = ("state", "id", "content", "attachments", "embeds", "channel", "server", "author", "edited_at", "mentions", "replies", "reply_ids")
+    __slots__ = ("state", "id", "content", "attachments", "embeds", "channel", "author", "edited_at", "mentions", "replies", "reply_ids")
 
     def __init__(self, data: MessagePayload, state: State):
         self.state = state
 
         self.id = data["_id"]
         self.content = data["content"]
         self.attachments = [Asset(attachment, state) for attachment in data.get("attachments", [])]
         self.embeds = [to_embed(embed, state) for embed in data.get("embeds", [])]
 
         channel = state.get_channel(data["channel"])
         assert isinstance(channel, Messageable)
         self.channel = channel
 
-        self.server = self.channel and self.channel.server
-
-        if self.server:
-            author = state.get_member(self.server.id, data["author"])
+        if server_id := self.channel.server_id:
+            author = state.get_member(server_id, data["author"])
         else:
             author = state.get_user(data["author"])
 
         self.author = author
 
         if masquerade := data.get("masquerade"):
             if name := masquerade.get("name"):
@@ -131,14 +127,19 @@
         .. code-block:: python
 
             await channel.send(..., replies=[MessageReply(message, mention)])
 
         """
         return self.channel.send(*args, **kwargs, replies=[MessageReply(self, mention)])
 
+    @property
+    def server(self) -> Server:
+        """:class:`Server` The server this voice channel belongs too"""
+        return self.channel.server
+
 class MessageReply(NamedTuple):
     """A namedtuple which represents a reply to a message.
 
     Parameters
     -----------
     message: :class:`Message`
         The message being replied to.
@@ -156,21 +157,27 @@
 
     Parameters
     -----------
     name: Optional[:class:`str`]
         The name to display for the message
     avatar: Optional[:class:`str`]
         The avatar's url to display for the message
+    colour: Optional[:class:`str`]
+        The colour of the name, similar to role colours
     """
     name: Optional[str] = None
     avatar: Optional[str] = None
+    colour: Optional[str] = None
 
     def to_dict(self) -> MasqueradePayload:
         output: MasqueradePayload = {}
 
         if name := self.name:
             output["name"] = name
 
         if avatar := self.avatar:
             output["avatar"] = avatar
 
+        if colour := self.colour:
+            output["colour"] = colour
+
         return output
```

### Comparing `revolt.py-0.1.8/revolt/messageable.py` & `revolt.py-0.1.9/revolt/messageable.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/permissions.py` & `revolt.py-0.1.9/revolt/permissions.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/role.py` & `revolt.py-0.1.9/revolt/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,13 +82,13 @@
 
     async def edit(self, **kwargs):
         """Edits the role
 
         Parameters
         -----------
         """
-        if kwargs.get("colour", Missing) == None:
+        if kwargs.get("colour", Missing) is None:
             remove = "Colour"
         else:
             remove = None
 
         await self.state.http.edit_role(self.server.id, self.id, remove, kwargs)
```

### Comparing `revolt.py-0.1.8/revolt/server.py` & `revolt.py-0.1.9/revolt/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             self.banner  = None
 
         self._members: dict[str, Member] = {}
         self._roles: dict[str, Role] = {role_id: Role(role, role_id, self, state) for role_id, role in data.get("roles", {}).items()}
 
         self._channels: dict[str, Channel] = {channel_id: state.get_channel(channel_id) for channel_id in data.get("channels", [])}
 
-    def _update(self, *, owner: Optional[str] = None, name: Optional[str] = None, description: Optional[str] = None, icon: Optional[FilePayload] = None, banner: Optional[FilePayload] = None, default_permissions: Optional[int] = None, nsfw: Optional[bool] = None, system_messages: Optional[SystemMessagesConfig] = None, categories: Optional[list[CategoryPayload]] = None):
+    def _update(self, *, owner: Optional[str] = None, name: Optional[str] = None, description: Optional[str] = None, icon: Optional[FilePayload] = None, banner: Optional[FilePayload] = None, default_permissions: Optional[int] = None, nsfw: Optional[bool] = None, system_messages: Optional[SystemMessagesConfig] = None, categories: Optional[list[CategoryPayload]] = None, channels: Optional[list[str]] = None):
         if owner:
             self.owner_id = owner
         if name:
             self.name = name
         if description is not None:
             self.description = description or None
         if icon:
@@ -133,14 +133,16 @@
             self.default_permissions = Permissions(default_permissions)
         if nsfw is not None:
             self.nsfw = nsfw
         if system_messages is not None:
             self.system_messages = SystemMessages(system_messages, self.state)
         if categories is not None:
             self._categories = {data["id"]: Category(data, self.state) for data in categories}
+        if channels is not None:
+            self._channels = {channel_id: self.state.get_channel(channel_id) for channel_id in channels}
 
     @property
     def roles(self) -> list[Role]:
         """list[:class:`Role`] Gets all roles in the server in decending order"""
         return list(self._roles.values())
 
     @property
@@ -182,45 +184,54 @@
             The id of the member
 
         Returns
         --------
         :class:`Member`
             The member
         """
-        return self._members[member_id]
+        try:
+            return self._members[member_id]
+        except KeyError as e:
+            raise LookupError from e
 
     def get_channel(self, channel_id: str) -> Channel:
         """Gets a channel from the cache
 
         Parameters
         -----------
         id: :class:`str`
             The id of the channel
 
         Returns
         --------
         :class:`Channel`
             The channel
         """
-        return self._channels[channel_id]
+        try:
+            return self._channels[channel_id]
+        except KeyError as e:
+            raise LookupError from e
 
     def get_category(self, category_id: str) -> Category:
         """Gets a category from the cache
 
         Parameters
         -----------
         id: :class:`str`
             The id of the category
 
         Returns
         --------
         :class:`Category`
             The category
         """
-        return self._categories[category_id]
+        try:
+            return self._categories[category_id]
+        except KeyError as e:
+            raise LookupError from e
 
     @property
     def owner(self) -> Member:
         """:class:`Member` The owner of the server"""
         return self.get_member(self.owner_id)
 
     async def set_default_permissions(self, permissions: Permissions) -> None:
```

### Comparing `revolt.py-0.1.8/revolt/state.py` & `revolt.py-0.1.9/revolt/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,25 +31,34 @@
 
         self.users: dict[str, User] = {}
         self.channels: dict[str, Channel] = {}
         self.servers: dict[str, Server] = {}
         self.messages: deque[Message] = deque()
 
     def get_user(self, id: str) -> User:
-        return self.users[id]
+        try:
+            return self.users[id]
+        except KeyError as e:
+            raise LookupError from e
 
     def get_member(self, server_id: str, member_id: str) -> Member:
         server = self.servers[server_id]
         return server.get_member(member_id)
 
     def get_channel(self, id: str) -> Channel:
-        return self.channels[id]
+        try:
+            return self.channels[id]
+        except KeyError as e:
+            raise LookupError from e
 
     def get_server(self, id: str) -> Server:
-        return self.servers[id]
+        try:
+            return self.servers[id]
+        except KeyError as e:
+            raise LookupError from e
 
     def add_user(self, payload: UserPayload) -> User:
         user = User(payload, self)
         self.users[user.id] = user
         return user
 
     def add_member(self, server_id: str, payload: MemberPayload) -> Member:
@@ -78,18 +87,21 @@
         return message
 
     def get_message(self, message_id: str) -> Message:
         for msg in self.messages:
             if msg.id == message_id:
                 return msg
 
-        raise KeyError
+        raise LookupError
 
-    async def fetch_all_server_members(self):
-        for server_id in self.servers.keys():
-            data = await self.http.fetch_members(server_id)
+    async def fetch_server_members(self, server_id: str):
+        data = await self.http.fetch_members(server_id)
+
+        for user in data["users"]:
+            self.add_user(user)
 
-            for user in data["users"]:
-                self.add_user(user)
+        for member in data["members"]:
+            self.add_member(server_id, member)
 
-            for member in data["members"]:
-                self.add_member(server_id, member)
+    async def fetch_all_server_members(self):
+        for server_id in self.servers:
+            await self.fetch_server_members(server_id)
```

### Comparing `revolt.py-0.1.8/revolt/types/channel.py` & `revolt.py-0.1.9/revolt/types/channel.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,40 +26,44 @@
 class SavedMessages(BaseChannel):
     user: str
     channel_type: Literal["SavedMessages"]
 
 class DMChannel(BaseChannel):
     active: bool
     recipients: list[str]
-    last_message: Message
+    last_message_id: NotRequired[str]
     channel_type: Literal["DirectMessage"]
 
 class GroupDMChannel(BaseChannel):
     recipients: list[str]
     name: str
     owner: str
     channel_type: Literal["Group"]
     icon: NotRequired[File]
     permissions: NotRequired[int]
     description: NotRequired[str]
+    nsfw: NotRequired[bool]
+    last_message_id: NotRequired[str]
 
 class TextChannel(BaseChannel):
     server: str
     name: str
     description: str
     channel_type: Literal["TextChannel"]
     icon: NotRequired[File]
     default_permissions: NotRequired[Overwrite]
     role_permissions: NotRequired[dict[str, Overwrite]]
-    last_message: NotRequired[str]
+    nsfw: NotRequired[bool]
+    last_message_id: NotRequired[str]
 
 class VoiceChannel(BaseChannel):
     server: str
     name: str
     description: str
     channel_type: Literal["VoiceChannel"]
     icon: NotRequired[File]
     default_permissions: NotRequired[Overwrite]
     role_permissions: NotRequired[dict[str, Overwrite]]
+    nsfw: NotRequired[bool]
 
 GuildChannel = Union[TextChannel, VoiceChannel]
 Channel = Union[SavedMessages, DMChannel, GroupDMChannel, TextChannel, VoiceChannel]
```

### Comparing `revolt.py-0.1.8/revolt/types/embed.py` & `revolt.py-0.1.9/revolt/types/embed.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/types/gateway.py` & `revolt.py-0.1.9/revolt/types/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     "ServerDeleteEventPayload",
     "ServerMemberUpdateEventPayload",
     "ServerMemberJoinEventPayload",
     "ServerMemberLeaveEventPayload",
     "ServerRoleUpdateEventPayload",
     "ServerRoleDeleteEventPayload",
     "UserUpdateEventPayload",
-    "UserRelationshipEventPayload"
+    "UserRelationshipEventPayload",
+    "ServerCreateEventPayload"
 )
 
 class BasePayload(TypedDict):
     type: str
 
 class AuthenticatePayload(BasePayload):
     token: str
@@ -126,14 +127,19 @@
     id: str
     data: ServerUpdateEventPayloadData
     clear: Literal["Icon", "Banner", "Description"]
 
 class ServerDeleteEventPayload(BasePayload):
     id: str
 
+class ServerCreateEventPayload(BasePayload):
+    id: str
+    server: Server
+    channels: list[Channel]
+
 class ServerMemberUpdateEventPayloadData(TypedDict, total=False):
     nickname: str
     avatar: File
     roles: list[str]
 
 class ServerMemberUpdateEventPayload(BasePayload):
     id: MemberID
```

### Comparing `revolt.py-0.1.8/revolt/types/http.py` & `revolt.py-0.1.9/revolt/types/http.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/types/invite.py` & `revolt.py-0.1.9/revolt/types/invite.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/types/message.py` & `revolt.py-0.1.9/revolt/types/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     by: str
 
 MessageEdited = TypedDict("MessageEdited", {"$date": str})
 
 class Masquerade(TypedDict, total=False):
     name: str
     avatar: str
+    colour: str
 
 class Message(TypedDict):
     _id: str
     channel: str
     author: str
     content: Union[str, UserAddContent, UserRemoveContent, UserJoinedContent, UserLeftContent, UserKickedContent, UserBannedContent, ChannelRenameContent, ChannelDescriptionChangeContent, ChannelIconChangeContent]
     attachments: NotRequired[list[File]]
```

### Comparing `revolt.py-0.1.8/revolt/types/server.py` & `revolt.py-0.1.9/revolt/types/server.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/types/user.py` & `revolt.py-0.1.9/revolt/types/user.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/user.py` & `revolt.py-0.1.9/revolt/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, NamedTuple, Optional, Union
+from typing import TYPE_CHECKING, Literal, NamedTuple, Optional, Union
 
 from .asset import Asset, PartialAsset
 from .channel import DMChannel
 from .enums import PresenceType, RelationshipType
 from .flags import UserBadges
 from .messageable import Messageable
 
 if TYPE_CHECKING:
     from .state import State
     from .types import File
     from .types import Status as StatusPayload
     from .types import User as UserPayload
-
+    from .member import Member
 
 __all__ = ("User", "Status", "Relation", "UserProfile")
 
 class Relation(NamedTuple):
     """A namedtuple representing a relation between the bot and a user"""
     type: RelationshipType
     user: User
@@ -55,18 +55,19 @@
         The relationship between the user and the bot
     status: Optional[:class:`Status`]
         The users status
     dm_channel: Optional[:class:`DMChannel`]
         The dm channel between the client and the user, this will only be set if the client has dm'ed the user or :meth:`User.open_dm` was run
     """
     __flattern_attributes__ = ("id", "bot", "owner_id", "badges", "online", "flags", "relations", "relationship", "status", "masquerade_avatar", "masquerade_name", "original_name", "original_avatar", "profile", "dm_channel")
-    __slots__ = (*__flattern_attributes__, "state")
+    __slots__ = (*__flattern_attributes__, "state", "_members")
 
     def __init__(self, data: UserPayload, state: State):
         self.state = state
+        self._members: list[Member] = []  # we store all member versions of this user to avoid having to check every guild when needing to update.
         self.id = data["_id"]
         self.original_name = data["username"]
         self.dm_channel = None
 
         bot = data.get("bot")
         if bot:
             self.bot = True
@@ -149,14 +150,19 @@
 
         if avatar:
             self.original_avatar = Asset(avatar, self.state)
 
         if online:
             self.online = online
 
+        # update user infomation for all members
+
+        for member in self._members:
+            User._update(member, status=status, profile_content=profile_content, profile_background=profile_background, avatar=avatar, online=online)
+
     async def default_avatar(self) -> bytes:
         """Returns the default avatar for this user
 
         Returns
         --------
         :class:`bytes`
             The bytes of the image
```

### Comparing `revolt.py-0.1.8/revolt/utils.py` & `revolt.py-0.1.9/revolt/utils.py`

 * *Files identical despite different names*

### Comparing `revolt.py-0.1.8/revolt/websocket.py` & `revolt.py-0.1.9/revolt/websocket.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .types import (ChannelCreateEventPayload, ChannelDeleteEventPayload,
                     ChannelDeleteTypingEventPayload,
                     ChannelStartTypingEventPayload, ChannelUpdateEventPayload)
 from .types import Message as MessagePayload
 from .types import (MessageDeleteEventPayload, MessageUpdateEventPayload,
                     ServerDeleteEventPayload, ServerMemberJoinEventPayload,
                     ServerMemberLeaveEventPayload,
+                    ServerCreateEventPayload,
                     ServerMemberUpdateEventPayload,
                     ServerRoleDeleteEventPayload, ServerRoleUpdateEventPayload,
                     ServerUpdateEventPayload, UserRelationshipEventPayload,
                     UserUpdateEventPayload)
 from .user import Status, UserProfile
 
 try:
@@ -42,26 +43,31 @@
 
 
 __all__ = ("WebsocketHandler",)
 
 logger = logging.getLogger("revolt")
 
 class WebsocketHandler:
-    __slots__ = ("session", "token", "ws_url", "dispatch", "state", "websocket", "loop", "user", "ready")
+    __slots__ = ("session", "token", "ws_url", "dispatch", "state", "websocket", "loop", "user", "ready", "server_events")
 
     def __init__(self, session: aiohttp.ClientSession, token: str, ws_url: str, dispatch: Callable[..., None], state: State):
         self.session = session
         self.token = token
         self.ws_url = ws_url
         self.dispatch = dispatch
         self.state = state
         self.websocket: aiohttp.ClientWebSocketResponse
         self.loop = asyncio.get_running_loop()
         self.user = None
         self.ready = asyncio.Event()
+        self.server_events: dict[str, asyncio.Event] = {}
+
+    async def _wait_for_server_ready(self, server_id: str):
+        if event := self.server_events.get(server_id):
+            await event.wait()
 
     async def send_payload(self, payload: BasePayload):
         if use_msgpack:
             await self.websocket.send_bytes(msgpack.packb(payload))  # type: ignore
         else:
             await self.websocket.send_str(json.dumps(payload))
 
@@ -83,15 +89,15 @@
         event_type = payload["type"].lower()
         logger.debug("Recieved event %s %s", event_type, payload)
         try:
             if event_type != "ready":
                 await self.ready.wait()
 
             func = getattr(self, f"handle_{event_type}")
-        except:
+        except AttributeError:
             logger.debug("Unknown event '%s'", event_type)
             return
 
         await func(payload)
 
     async def handle_authenticated(self, _):
         logger.info("Successfully authenticated")
@@ -116,14 +122,18 @@
         await self.state.fetch_all_server_members()
 
         self.ready.set()
         self.dispatch("ready")
 
     async def handle_message(self, payload: MessageEventPayload):
         message = self.state.add_message(cast(MessagePayload, payload))
+
+        if server := message.server:
+            await self._wait_for_server_ready(server.id)
+
         self.dispatch("message", message)
 
     async def handle_messageupdate(self, payload: MessageUpdateEventPayload):
         self.dispatch("raw_message_update", payload)
 
         message = self.state.get_message(payload["id"])
 
@@ -136,30 +146,40 @@
         kwargs["edited_at"] = data["edited"]["$date"]
 
         if embeds := data.get("embeds"):
             kwargs["embeds"] = embeds
 
         message._update(**kwargs)
 
+        if server := message.server:
+            await self._wait_for_server_ready(server.id)
+
         self.dispatch("message_update", message)
 
     async def handle_messagedelete(self, payload: MessageDeleteEventPayload):
         self.dispatch("raw_message_delete", payload)
 
         try:
             message = self.state.get_message(payload["id"])
-        except:
+        except KeyError:
             return
 
         self.state.messages.remove(message)
+
+        if server := message.server:
+            await self._wait_for_server_ready(server.id)
+
         self.dispatch("message_delete", message)
 
     async def handle_channelcreate(self, payload: ChannelCreateEventPayload):
         channel = self.state.add_channel(payload)
 
+        if server := channel.server:
+            await self._wait_for_server_ready(server.id)
+
         self.dispatch("channel_create", channel)
 
     async def handle_channelupdate(self, payload: ChannelUpdateEventPayload):
         channel = self.state.get_channel(payload["id"])
 
         old_channel = copy(channel)
 
@@ -170,31 +190,43 @@
                 if isinstance(channel, (TextChannel, VoiceChannel, GroupDMChannel)):
                     channel.icon = None
 
             elif clear == "Description":
                 if isinstance(channel, (TextChannel, VoiceChannel, GroupDMChannel)):
                     channel.description = None
 
+        if server := channel.server:
+            await self._wait_for_server_ready(server.id)
+
         self.dispatch("channel_update", old_channel, channel)
 
     async def handle_channeldelete(self, payload: ChannelDeleteEventPayload):
         channel = self.state.channels.pop(payload["id"])
 
+        if server := channel.server:
+            await self._wait_for_server_ready(server.id)
+
         self.dispatch("channel_delete", channel)
 
     async def handle_channelstarttyping(self, payload: ChannelStartTypingEventPayload):
         channel = self.state.get_channel(payload["id"])
         user = self.state.get_user(payload["user"])
 
+        if server := channel.server:
+            await self._wait_for_server_ready(server.id)
+
         self.dispatch("typing_start", channel, user)
 
     async def handle_channelstoptyping(self, payload: ChannelDeleteTypingEventPayload):
         channel = self.state.get_channel(payload["id"])
         user = self.state.get_user(payload["user"])
 
+        if server := channel.server:
+            await self._wait_for_server_ready(server.id)
+
         self.dispatch("typing_stop", channel, user)
 
     async def handle_serverupdate(self, payload: ServerUpdateEventPayload):
         server = self.state.get_server(payload["id"])
 
         old_server = copy(server)
 
@@ -206,25 +238,44 @@
 
             elif clear == "Banner":
                 server.banner = None
 
             elif clear == "Description":
                 server.description = None
 
+        await self._wait_for_server_ready(server.id)
+
         self.dispatch("server_update", old_server, server)
 
     async def handle_serverdelete(self, payload: ServerDeleteEventPayload):
         server = self.state.servers.pop(payload["id"])
 
         for channel in server.channels:
             del self.state.channels[channel.id]
 
+        await self._wait_for_server_ready(server.id)
+
         self.dispatch("server_delete", server)
 
+    async def handle_servercreate(self, payload: ServerCreateEventPayload):
+        for channel in payload["channels"]:
+            self.state.add_channel(channel)
+
+        server = self.state.add_server(payload["server"])
+
+        # lock all server events until we fetch all the members, otherwise the cache will be incomplete
+        self.server_events[server.id] = asyncio.Event()
+        await self.state.fetch_server_members(server.id)
+        self.server_events.pop(server.id).set()
+
+        self.dispatch("server_create", server)
+
     async def handle_servermemberupdate(self, payload: ServerMemberUpdateEventPayload):
+        await self._wait_for_server_ready(payload["id"]["server"])
+
         member = self.state.get_member(payload["id"]["server"], payload["id"]["user"])
         old_member = copy(member)
 
         if clear := payload.get("clear"):
             if clear == "Nickname":
                 member.nickname = None
             elif clear == "Avatar":
@@ -235,36 +286,47 @@
         self.dispatch("member_update", old_member, member)
 
     async def handle_servermemberjoin(self, payload: ServerMemberJoinEventPayload):
         member = self.state.add_member(payload["id"], {"_id": {"server": payload["id"], "user": payload["user"]}})
         self.dispatch("member_join", member)
 
     async def handle_memberleave(self, payload: ServerMemberLeaveEventPayload):
+        await self._wait_for_server_ready(payload["id"])
+
         server = self.state.get_server(payload["id"])
         member = server._members.pop(payload["user"])
 
+        # remove the member from the user
+
+        user = self.state.get_user(payload["user"])
+        user._members.remove(member)
+
         self.dispatch("member_leave", member)
 
     async def handle_serveroleupdate(self, payload: ServerRoleUpdateEventPayload):
         server = self.state.get_server(payload["id"])
         role = server.get_role(payload["role_id"])
         old_role = copy(role)
 
         if clear := payload.get("clear"):
             if clear == "Colour":
                 role.colour = None
 
         role._update(**payload["data"])
 
+        await self._wait_for_server_ready(server.id)
+
         self.dispatch("role_update", old_role, role)
 
     async def handle_serverroledelete(self, payload: ServerRoleDeleteEventPayload):
         server = self.state.get_server(payload["id"])
         role = server._roles.pop(payload["role_id"])
 
+        await self._wait_for_server_ready(server.id)
+
         self.dispatch("role_delete", role)
 
     async def handle_userupdate(self, payload: UserUpdateEventPayload):
         user = self.state.get_user(payload["id"])
         old_user = copy(user)
 
         if clear := payload.get("clear"):
```

### Comparing `revolt.py-0.1.8/setup.py` & `revolt.py-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'docs': ['Sphinx==4.3.2',
           'sphinx-nameko-theme==0.0.3',
           'sphinx-toolbox==2.15.2'],
  'speedups': ['ujson==5.1.0', 'msgpack']}
 
 setup_kwargs = {
     'name': 'revolt.py',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Python wrapper for the revolt.chat API',
     'long_description': '# Revolt.py\n\nAn async library to interact with the https://revolt.chat API.\n\nYou can join the support server [here](https://rvlt.gg/FDXER6hr) and find the library\'s documentation [here](https://revoltpy.readthedocs.io/en/latest/).\n\n## Installing\n\nYou can use `pip` to install revolt.py. It differs slightly depending on what OS/Distro you use.\n\nOn Windows\n```\npy -m pip install -U revolt.py # -U to update\n```\n\nOn macOS and Linux\n```\npython3 -m pip install -U revolt.py\n```\n\n## Example\n\nMore examples can be found in the [examples folder](https://github.com/revoltchat/revolt.py/blob/master/examples).\n\n```py\nimport revolt\nimport asyncio\nimport aiohttp\n\nclass Client(revolt.Client):\n    async def on_message(self, message: revolt.Message):\n        if message.content == "hello":\n            await message.channel.send("hi how are you")\n\nasync def main():\n    async with aiohttp.ClientSession() as session:\n        client = Client(session, "BOT TOKEN HERE")\n        await client.start()\n\nasyncio.run(main())\n```\n',
     'author': 'Zomatee',
     'author_email': 'me@zomatree.live',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/revoltchat/revolt.py',
```

### Comparing `revolt.py-0.1.8/PKG-INFO` & `revolt.py-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revolt.py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python wrapper for the revolt.chat API
 Home-page: https://github.com/revoltchat/revolt.py
 License: MIT
 Keywords: wrapper,async,api,websockets,http
 Author: Zomatee
 Author-email: me@zomatree.live
 Requires-Python: >=3.9,<4.0
```

