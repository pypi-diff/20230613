# Comparing `tmp/z3c.saconfig-0.9.1.tar.gz` & `tmp/z3c.saconfig-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.saconfig-0.9.1.tar", last modified: Fri Aug 14 14:47:46 2009, max compression, from Unix
+gzip compressed data, was "z3c.saconfig-1.0.tar", last modified: Tue Jun 13 06:08:13 2023, max compression
```

## Comparing `z3c.saconfig-0.9.1.tar` & `z3c.saconfig-1.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 faassen   (1000) faassen   (1000)        0 2009-08-14 14:47:46.000000 z3c.saconfig-0.9.1/
-drwxr-xr-x   0 faassen   (1000) faassen   (1000)        0 2009-08-14 14:47:46.000000 z3c.saconfig-0.9.1/src/
-drwxr-xr-x   0 faassen   (1000) faassen   (1000)        0 2009-08-14 14:47:46.000000 z3c.saconfig-0.9.1/src/z3c/
-drwxr-xr-x   0 faassen   (1000) faassen   (1000)        0 2009-08-14 14:47:46.000000 z3c.saconfig-0.9.1/src/z3c/saconfig/
--rw-r--r--   0 faassen   (1000) faassen   (1000)    11807 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/src/z3c/saconfig/README.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)      165 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/src/z3c/saconfig/__init__.py
--rw-r--r--   0 faassen   (1000) faassen   (1000)     2189 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/src/z3c/saconfig/interfaces.py
--rw-r--r--   0 faassen   (1000) faassen   (1000)      549 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/src/z3c/saconfig/meta.zcml
--rw-r--r--   0 faassen   (1000) faassen   (1000)     1103 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/src/z3c/saconfig/scopedsession.py
--rw-r--r--   0 faassen   (1000) faassen   (1000)     3334 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/src/z3c/saconfig/tests.py
--rw-r--r--   0 faassen   (1000) faassen   (1000)     5912 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/src/z3c/saconfig/utility.py
--rw-r--r--   0 faassen   (1000) faassen   (1000)     3397 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/src/z3c/saconfig/zcml.py
--rw-r--r--   0 faassen   (1000) faassen   (1000)      244 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/src/z3c/__init__.py
-drwxr-xr-x   0 faassen   (1000) faassen   (1000)        0 2009-08-14 14:47:46.000000 z3c.saconfig-0.9.1/src/z3c.saconfig.egg-info/
--rw-r--r--   0 faassen   (1000) faassen   (1000)    15245 2009-08-14 14:47:45.000000 z3c.saconfig-0.9.1/src/z3c.saconfig.egg-info/PKG-INFO
--rw-r--r--   0 faassen   (1000) faassen   (1000)      659 2009-08-14 14:47:45.000000 z3c.saconfig-0.9.1/src/z3c.saconfig.egg-info/SOURCES.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)        1 2009-08-14 14:47:45.000000 z3c.saconfig-0.9.1/src/z3c.saconfig.egg-info/dependency_links.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)       37 2009-08-14 14:47:45.000000 z3c.saconfig-0.9.1/src/z3c.saconfig.egg-info/entry_points.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)        4 2009-08-14 14:47:45.000000 z3c.saconfig-0.9.1/src/z3c.saconfig.egg-info/namespace_packages.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)        1 2009-08-14 14:47:44.000000 z3c.saconfig-0.9.1/src/z3c.saconfig.egg-info/not-zip-safe
--rw-r--r--   0 faassen   (1000) faassen   (1000)      146 2009-08-14 14:47:45.000000 z3c.saconfig-0.9.1/src/z3c.saconfig.egg-info/requires.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)        4 2009-08-14 14:47:45.000000 z3c.saconfig-0.9.1/src/z3c.saconfig.egg-info/top_level.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)      192 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/CHANGES.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)      252 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/CREDITS.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)     1262 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/INSTALL.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)      128 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/README.txt
--rw-r--r--   0 faassen   (1000) faassen   (1000)     1783 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/bootstrap.py
--rw-r--r--   0 faassen   (1000) faassen   (1000)      190 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/buildout.cfg
--rw-r--r--   0 faassen   (1000) faassen   (1000)     1517 2009-08-14 14:47:43.000000 z3c.saconfig-0.9.1/setup.py
--rw-r--r--   0 faassen   (1000) faassen   (1000)    15245 2009-08-14 14:47:46.000000 z3c.saconfig-0.9.1/PKG-INFO
--rw-r--r--   0 faassen   (1000) faassen   (1000)       59 2009-08-14 14:47:46.000000 z3c.saconfig-0.9.1/setup.cfg
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-13 06:08:13.831157 z3c.saconfig-1.0/
+-rw-r--r--   0 mac        (513) staff       (20)     2243 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/COPYRIGHT.rst
+-rw-r--r--   0 mac        (513) staff       (20)      252 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/CREDITS.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1297 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/INSTALL.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/LICENSE.rst
+-rw-r--r--   0 mac        (513) staff       (20)      253 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    15971 2023-06-13 06:08:13.831347 z3c.saconfig-1.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      139 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      417 2023-06-13 06:08:13.832357 z3c.saconfig-1.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2135 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-13 06:08:13.817471 z3c.saconfig-1.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-13 06:08:13.824154 z3c.saconfig-1.0/src/z3c/
+-rw-r--r--   0 mac        (513) staff       (20)       76 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/src/z3c/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-13 06:08:13.830742 z3c.saconfig-1.0/src/z3c/saconfig/
+-rw-r--r--   0 mac        (513) staff       (20)    12609 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/src/z3c/saconfig/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      394 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/src/z3c/saconfig/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     2572 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/src/z3c/saconfig/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)      549 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/src/z3c/saconfig/meta.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     1094 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/src/z3c/saconfig/scopedsession.py
+-rw-r--r--   0 mac        (513) staff       (20)     3303 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/src/z3c/saconfig/tests.py
+-rw-r--r--   0 mac        (513) staff       (20)     5721 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/src/z3c/saconfig/utility.py
+-rw-r--r--   0 mac        (513) staff       (20)     5541 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/src/z3c/saconfig/zcml.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-13 06:08:13.827267 z3c.saconfig-1.0/src/z3c.saconfig.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    15971 2023-06-13 06:08:13.000000 z3c.saconfig-1.0/src/z3c.saconfig.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      662 2023-06-13 06:08:13.000000 z3c.saconfig-1.0/src/z3c.saconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-13 06:08:13.000000 z3c.saconfig-1.0/src/z3c.saconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        4 2023-06-13 06:08:13.000000 z3c.saconfig-1.0/src/z3c.saconfig.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-13 06:08:13.000000 z3c.saconfig-1.0/src/z3c.saconfig.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      141 2023-06-13 06:08:13.000000 z3c.saconfig-1.0/src/z3c.saconfig.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        4 2023-06-13 06:08:13.000000 z3c.saconfig-1.0/src/z3c.saconfig.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1421 2023-06-13 06:08:12.000000 z3c.saconfig-1.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `z3c.saconfig-0.9.1/src/z3c/saconfig/README.txt` & `z3c.saconfig-1.0/src/z3c/saconfig/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 instance. Multiple applications will all share this session. The
 engine is set up with a global utility.
 
 We use the SQLAlchemy ``sqlalchemy.ext.declarative`` extension to
 define some tables and classes::
 
   >>> from sqlalchemy import *
-  >>> from sqlalchemy.ext.declarative import declarative_base
-  >>> from sqlalchemy.orm import relation
+  >>> from sqlalchemy.orm import declarative_base
+  >>> from sqlalchemy.orm import relationship
 
   >>> Base = declarative_base()
   >>> class User(Base):
   ...     __tablename__ = 'test_users'
   ...     id = Column('id', Integer, primary_key=True)
   ...     name = Column('name', String(50))
-  ...     addresses = relation("Address", backref="user")
+  ...     addresses = relationship("Address", backref="user")
   >>> class Address(Base):
   ...     __tablename__ = 'test_addresses'
   ...     id = Column('id', Integer, primary_key=True)
   ...     email = Column('email', String(50))
   ...     user_id = Column('user_id', Integer, ForeignKey('test_users.id'))
 
 So far this doesn't differ from the ``zope.sqlalchemy`` example. We
@@ -48,15 +48,15 @@
 directly, we can set up the engine factory as a (global) utility. This
 utility makes sure an engine is created and cached for us.
 
   >>> from z3c.saconfig import EngineFactory
   >>> engine_factory = EngineFactory(TEST_DSN)
 
 You can pass the parameters you'd normally pass to
-``sqlalchemy.create_engine`` to ``EngineFactory``. 
+``sqlalchemy.create_engine`` to ``EngineFactory``.
 
 We now register the engine factory as a global utility using
 ``zope.component``. Normally you'd use either ZCML or Grok to do this
 confirmation, but we'll do it manually here::::
 
   >>> from zope import component
   >>> from z3c.saconfig.interfaces import IEngineFactory
@@ -89,22 +89,22 @@
 if you don't supply your own ``bind``
 argument. ``GloballyScopedSession`` also automatically sets up the
 ``autocommit``, ``autoflush`` and ``extension`` parameters to be the
 right ones for Zope integration, so normally you wouldn't need to
 supply these, but you could pass in your own if you do need it.
 
 We now register this as an ``IScopedSession`` utility::
-  
+
   >>> from z3c.saconfig.interfaces import IScopedSession
   >>> component.provideUtility(utility, provides=IScopedSession)
- 
+
 We are done with configuration now. As you have seen it involves
 setting up two utilities, ``IEngineFactory`` and ``IScopedSession``,
 where only the latter is really needed in this globally shared session
-use case. 
+use case.
 
 After the ``IScopedSession`` utility is registered, one can import the
 ``Session`` class from z3c.saconfig.  This ``Session`` class is like
 the one you'd produce with ``sessionmaker`` from
 SQLAlchemy. `z3c.saconfig.Session`` is intended to be the only
 ``Session`` class you'll ever need, as all configuration and Zope
 integration is done automatically for you by ``z3c.saconfig``,
@@ -118,46 +118,50 @@
   >>> from z3c.saconfig import Session
   >>> session = Session()
 
 Now things go the usual ``zope.sqlalchemy`` way, which is like
 ``SQLAlchemy`` except you can use Zope's ``transaction`` module::
 
   >>> session.query(User).all()
-  []    
+  []
   >>> import transaction
   >>> session.add(User(name='bob'))
   >>> transaction.commit()
 
   >>> session = Session()
   >>> bob = session.query(User).all()[0]
-  >>> bob.name
-  u'bob'
+  >>> bob.name == 'bob'
+  True
   >>> bob.addresses
   []
 
 Events
 ======
 
 When a new engine is created by an ``EngineFactory``, an
 ``IEngineCreatedEvent`` is fired. This event has an attribute
 ``engine`` that contains the engine that was just created::
 
   >>> from z3c.saconfig.interfaces import IEngineCreatedEvent
   >>> @component.adapter(IEngineCreatedEvent)
   ... def createdHandler(event):
-  ...     print "created engine"
+  ...     print("created engine")
+  ...     print("args: {0}".format(event.engine_args))
+  ...     print("kw: {0}".format(event.engine_kw))
   >>> component.provideHandler(createdHandler)
   >>> event_engine_factory = EngineFactory(TEST_DSN1)
   >>> engine = event_engine_factory()
   created engine
+  args: ('sqlite:///:memory:',)
+  kw: {}
 
 Let's get rid of the event handler again::
 
   >>> sm = component.getSiteManager()
-  >>> sm.unregisterHandler(None, 
+  >>> sm.unregisterHandler(None,
   ...   required=[IEngineCreatedEvent])
   True
 
 SiteScopedSession (one database per site)
 =========================================
 
 In the example above we have set up SQLAlchemy with Zope using
@@ -222,84 +226,84 @@
   >>> component.getUtility(IEngineFactory) is engine_factory2
   True
 
 We can look up our global utility even if we're in a site::
 
   >>> component.getUtility(IScopedSession) is utility
   True
-  
+
 Phew. That was a lot of set up, but basically this is actually just
 straightforward utility setup code; you should use the APIs or Grok's
 ``grok.local_utility`` directive to set up local utilities. Now all
 that is out of the way, we can create a session for ``site1``::
 
   >>> setSite(site1)
   >>> session = Session()
 
 The database is still empty::
 
-  >>> session.query(User).all() 
+  >>> session.query(User).all()
   []
 
 We'll add something to this database now::
 
   >>> session.add(User(name='bob'))
   >>> transaction.commit()
 
 ``bob`` is now there::
 
   >>> session = Session()
-  >>> session.query(User).all()[0].name
-  u'bob'
+  >>> session.query(User).all()[0].name == 'bob'
+  True
 
 Now we'll switch to ``site2``::
 
   >>> setSite(site2)
-  
+
 If we create a new session now, we should now be working with a
 different database, which should still be empty::
 
   >>> session = Session()
-  >>> session.query(User).all() 
+  >>> session.query(User).all()
   []
-  
+
 We'll add ``fred`` to this database::
 
   >>> session.add(User(name='fred'))
   >>> transaction.commit()
 
 Now ``fred`` is indeed there::
- 
+
   >>> session = Session()
   >>> users = session.query(User).all()
   >>> len(users)
   1
-  >>> users[0].name
-  u'fred'
+  >>> users[0].name == 'fred'
+  True
 
 And ``bob`` is still in ``site1``::
 
   >>> setSite(site1)
   >>> session = Session()
   >>> users = session.query(User).all()
   >>> len(users)
   1
-  >>> users[0].name
-  u'bob'
+  >>> users[0].name == 'bob'
+  True
 
 Engines and Threading
 =====================
 
   >>> engine = None
   >>> def setEngine():
   ...     global engine
   ...     engine = engine_factory1()
 
 Engine factories must produce the same engine:
- 
+
   >>> setEngine()
   >>> engine is engine_factory1()
   True
 
 Even if you call it in a different thread:
 
   >>> import threading
@@ -308,15 +312,15 @@
   >>> t.start()
   >>> t.join()
 
   >>> engine is engine_factory1()
   True
 
 Unless they are reset:
-  
+
   >>> engine_factory1.reset()
   >>> engine is engine_factory1()
   False
 
 Even engine factories with the same parameters created at (almost) the same
 time should produce different engines:
 
@@ -325,41 +329,60 @@
 
 Configuration using ZCML
 ========================
 
 A configuration directive is provided to register a database engine
 factory using ZCML.
 
-  >>> from cStringIO import StringIO
+  >>> from io import BytesIO
   >>> from zope.configuration import xmlconfig
   >>> import z3c.saconfig
   >>> xmlconfig.XMLConfig('meta.zcml', z3c.saconfig)()
 
 Let's try registering the directory again.
 
-  >>> xmlconfig.xmlconfig(StringIO("""
+  >>> xmlconfig.xmlconfig(BytesIO(b"""
   ... <configure xmlns="http://namespaces.zope.org/db">
   ...   <engine name="dummy" url="sqlite:///:memory:" />
   ... </configure>"""))
 
   >>> component.getUtility(IEngineFactory, name="dummy")
   <z3c.saconfig.utility.EngineFactory object at ...>
 
 This time with a setup call.
 
-  >>> xmlconfig.xmlconfig(StringIO("""
+  >>> xmlconfig.xmlconfig(BytesIO(b"""
   ... <configure xmlns="http://namespaces.zope.org/db">
   ...   <engine name="dummy2" url="sqlite:///:memory:"
   ...           setup="z3c.saconfig.tests.engine_subscriber" />
   ... </configure>"""))
   got: Engine(sqlite:///:memory:)
 
+It's also possible to specify connection pooling options:
+
+  >>> xmlconfig.xmlconfig(BytesIO(b"""
+  ... <configure xmlns="http://namespaces.zope.org/db">
+  ...   <engine name="dummy" url="sqlite:///:memory:"
+  ...       pool_size="1"
+  ...       max_overflow="2"
+  ...       pool_recycle="3"
+  ...       pool_timeout="4"
+  ...       />
+  ... </configure>"""))
+
+  >>> engineFactory = component.getUtility(IEngineFactory, name="dummy")
+  >>> engineFactory._kw == {'echo': None, 'pool_size': 1, 'max_overflow': 2, 'pool_recycle': 3, 'pool_timeout': 4}
+  True
+
+(See the SQLAlchemy documentation on connection pooling for details on how
+these arguments are used.)
+
 The session directive is provided to register a scoped session utility:
 
-  >>> xmlconfig.xmlconfig(StringIO("""
+  >>> xmlconfig.xmlconfig(BytesIO(b"""
   ... <configure xmlns="http://namespaces.zope.org/db">
   ...   <session name="dummy" engine="dummy2" />
   ... </configure>"""))
 
   >>> component.getUtility(IScopedSession, name="dummy")
   <z3c.saconfig.utility.GloballyScopedSession object at ...>
```

### Comparing `z3c.saconfig-0.9.1/src/z3c/saconfig/interfaces.py` & `z3c.saconfig-1.0/src/z3c/saconfig/interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from zope.interface import Interface, implements, Attribute
+from zope.interface import Attribute
+from zope.interface import Interface
+from zope.interface import implementer
+
 
 class IScopedSession(Interface):
     """A utility that plugs into SQLAlchemy's scoped session machinery.
 
     The idea is that you'd either register a IScopedSession utility globally,
     for simple configurations, or locally, if you want to have the ability
     to transparently use a different engine and session configuration per
@@ -19,21 +22,23 @@
         """Determine the scope of the session.
 
         This can be used to scope the session per thread, per Zope 3 site,
         or otherwise. Return an immutable value to scope the session,
         like a thread id, or a tuple with thread id and application id.
         """
 
+
 class ISiteScopedSession(IScopedSession):
     """A utility that makes sessions be scoped by site.
     """
     def siteScopeFunc():
         """Returns a unique id per site.
         """
 
+
 class IEngineFactory(Interface):
     """A utility that maintains an SQLAlchemy engine.
 
     If the engine isn't created yet, it will create it. Otherwise the
     engine will be cached.
     """
 
@@ -53,20 +58,30 @@
 
     def reset():
         """Reset the cached engine (if any).
 
         This causes the engine to be recreated on next use.
         """
 
+
 class IEngineCreatedEvent(Interface):
     """An SQLAlchemy engine has been created.
 
     Hook into this event to do setup that can only be performed with
     an active engine.
     """
     engine = Attribute("The engine that was just created.")
-    
-class EngineCreatedEvent(object):
-    implements(IEngineCreatedEvent)
 
-    def __init__(self, engine):
+    engine_args = Attribute("List of arguments given to SQLAlchemy "
+                            "create_engine")
+
+    engine_kw = Attribute("Dictionary of keyword attributes given to "
+                          "SQLAlchemy create_engine")
+
+
+@implementer(IEngineCreatedEvent)
+class EngineCreatedEvent:
+
+    def __init__(self, engine, engine_args, engine_kw):
         self.engine = engine
+        self.engine_args = engine_args
+        self.engine_kw = engine_kw
```

### Comparing `z3c.saconfig-0.9.1/src/z3c/saconfig/meta.zcml` & `z3c.saconfig-1.0/src/z3c/saconfig/meta.zcml`

 * *Files identical despite different names*

### Comparing `z3c.saconfig-0.9.1/src/z3c/saconfig/scopedsession.py` & `z3c.saconfig-1.0/src/z3c/saconfig/scopedsession.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,41 @@
-from z3c.saconfig.interfaces import IScopedSession
-
 from sqlalchemy.orm import scoped_session
 from zope import component
 
-def session_factory(name=u''):
+from z3c.saconfig.interfaces import IScopedSession
+
+
+def session_factory(name=''):
     """This is used by scoped session to create a new Session object.
 
     It delegates to a IScopedSession utility.
     """
     utility = component.getUtility(IScopedSession, name)
     return utility.sessionFactory()
 
-def scopefunc(name=u''):
+
+def scopefunc(name=''):
     """This is used by scoped session to distinguish between sessions.
 
     It delegates to a IScopedSession utility.
     """
     utility = component.getUtility(IScopedSession, name)
     return utility.scopeFunc()
 
 # this is framework central configuration. Use a IScopedSession utility
 # to define behavior.
+
+
 Session = scoped_session(session_factory, scopefunc)
 
-_named_scoped_sessions = {u'': Session}
+_named_scoped_sessions = {'': Session}
+
 
 def named_scoped_session(name):
     try:
         return _named_scoped_sessions[name]
     except KeyError:
-        return _named_scoped_sessions.setdefault(name,
-                            scoped_session(lambda:session_factory(name),
-                                           lambda:scopefunc(name)))
+        return _named_scoped_sessions.setdefault(
+            name,
+            scoped_session(
+                lambda: session_factory(name),
+                lambda: scopefunc(name)))
```

### Comparing `z3c.saconfig-0.9.1/src/z3c/saconfig/tests.py` & `z3c.saconfig-1.0/src/z3c/saconfig/tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,117 +3,131 @@
 #
 # export TEST_DSN=postgres://plone:plone@localhost/test
 # export TEST_DSN=mssql://plone:plone@/test?dsn=mydsn
 
 # Since the test exercise what happens with two different DSNs
 # locally, you need to also set up a different TEST_DSN2.
 
-# To test in twophase commit mode export TEST_TWOPHASE=True 
-#
-# NOTE: The sqlite that ships with Mac OS X 10.4 is buggy.
-# Install a newer version (3.5.6) and rebuild pysqlite2 against it.
-
-
-import unittest
 import doctest
 import os
+import unittest
 
+import zope.component.eventtesting
+# To test in twophase commit mode export TEST_TWOPHASE=True
+#
+# NOTE: The sqlite that ships with Mac OS X 10.4 is buggy.
+# Install a newer version (3.5.6) and rebuild pysqlite2 against it.
+from zope import component
+from zope.interface import registry
 from zope.testing import cleanup
 from zope.testing.cleanup import addCleanUp
 
-from zope import component
-from zope.component import registry
-import zope.component.eventtesting
 
 TEST_TWOPHASE = bool(os.environ.get('TEST_TWOPHASE'))
 TEST_DSN = os.environ.get('TEST_DSN', 'sqlite:///:memory:')
 TEST_DSN1 = TEST_DSN
 # this can reuse TEST_DSN1 in the default case, as we can open another
 # in-memory database. You can't do this for other databases however.
 TEST_DSN2 = os.environ.get('TEST_DSN', TEST_DSN1)
 
+
 def setUpReadMe(test):
     # set up special local component architecture
     setHooks()
     # set up event handling
     zope.component.eventtesting.setUp(test)
 
+
 def tearDownReadMe(test):
     # clean up Zope
     cleanup.cleanUp()
 
     # clean up SQLAlchemy
     Base = test.globs['Base']
     engine = test.globs['engine']
     Base.metadata.drop_all(engine)
 
 # a very simple implementation of setSite and getSite so we don't have
 # to rely on zope.app.component just for our tests
+
+
 _site = None
 
-class DummySite(object):
+
+class DummySite:
     def __init__(self, id):
         self.id = id
         self._sm = SiteManager()
-        
+
     def getSiteManager(self):
         return self._sm
 
+
 class SiteManager(registry.Components):
     def __init__(self):
-        super(SiteManager, self).__init__()
+        super().__init__()
         self.__bases__ = (component.getGlobalSiteManager(),)
 
+
 def setSite(site=None):
     global _site
     _site = site
 
+
 def getSite():
     return _site
 
+
 def adapter_hook(interface, object, name='', default=None):
     try:
         return getSiteManager().adapters.adapter_hook(
             interface, object, name, default)
     except component.interfaces.ComponentLookupError:
         return default
 
+
 def getSiteManager(context=None):
     if _site is not None:
         return _site.getSiteManager()
     return component.getGlobalSiteManager()
 
+
 def setHooks():
     component.adapter_hook.sethook(adapter_hook)
     component.getSiteManager.sethook(getSiteManager)
 
+
 def resetHooks():
     component.adapter_hook.reset()
     component.getSiteManager.reset()
 
 # make sure hooks get cleaned up after tests are run
+
+
 addCleanUp(resetHooks)
 
+
 def engine_subscriber(engine):
-    print "got: %s " % engine
+    print(f'got: {engine!s} ')
+
 
 def test_suite():
     optionflags = doctest.NORMALIZE_WHITESPACE | doctest.ELLIPSIS
     globs = {
         'DummySite': DummySite,
         'setSite': setSite,
         'getSite': getSite,
         'TEST_DSN': TEST_DSN,
         'TEST_DSN1': TEST_DSN1,
         'TEST_DSN2': TEST_DSN2,
         'TEST_TWOPHASE': TEST_TWOPHASE,
-        }
-    
+    }
+
     suite = unittest.TestSuite()
-    
+
     suite.addTest(doctest.DocFileSuite(
-        'README.txt',
+        'README.rst',
         optionflags=optionflags,
         setUp=setUpReadMe,
         tearDown=tearDownReadMe,
         globs=globs))
     return suite
```

### Comparing `z3c.saconfig-0.9.1/src/z3c/saconfig/utility.py` & `z3c.saconfig-1.0/src/z3c/saconfig/utility.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 """
 Some reusable, standard implementations of IScopedSession.
 """
-
-import time
-import thread
 import threading
-import sqlalchemy
+import time
+from threading import get_ident
 
-from zope.interface import implements
+import sqlalchemy
 from zope import component
-from zope.sqlalchemy import ZopeTransactionExtension
 from zope.event import notify
+from zope.interface import implementer
+from zope.sqlalchemy import register
 
-from z3c.saconfig.interfaces import (IScopedSession, ISiteScopedSession,
-                                     IEngineFactory, EngineCreatedEvent)
+from z3c.saconfig.interfaces import EngineCreatedEvent
+from z3c.saconfig.interfaces import IEngineFactory
+from z3c.saconfig.interfaces import IScopedSession
+from z3c.saconfig.interfaces import ISiteScopedSession
 
-SA_0_5 = sqlalchemy.__version__ == 'svn' or sqlalchemy.__version__.split('.')[:2] == ['0', '5']
 
-if SA_0_5:
-    SESSION_DEFAULTS = dict(
-        autocommit=False,
-        autoflush=True,
-        extension=ZopeTransactionExtension())
-else:
-    SESSION_DEFAULTS = dict(
-        autoflush=True,
-        transactional=True,
-        extension=ZopeTransactionExtension())
+SESSION_DEFAULTS = dict(
+    autocommit=False,
+    autoflush=True,
+)
 
-class GloballyScopedSession(object):
+
+@implementer(IScopedSession)
+class GloballyScopedSession:
     """A globally scoped session.
 
     Register this as a global utility to have just one kind of session
     per Zope instance. All applications in this instance will share the
     same session.
 
     To register as a global utility you may need to register it with
     a custom factory, or alternatively subclass it and override __init__
     to pass the right arguments to the superclasses __init__.
     """
-    implements(IScopedSession)
-    
-    def __init__(self, engine=u'', **kw):
+
+    def __init__(self, engine='', **kw):
         """Pass keywords arguments for sqlalchemy.orm.create_session.
 
         The `engine` argument is the name of a utility implementing
         IEngineFactory.
-        
+
         Note that GloballyScopedSesssion does have different defaults than
         ``create_session`` for various parameters where it makes sense
         for Zope integration, namely:
 
         autocommit = False
         autoflush = True
         extension = ZopeTransactionExtension()
@@ -63,109 +58,118 @@
 
     def sessionFactory(self):
         kw = self.kw.copy()
         if 'bind' not in kw:
             engine_factory = component.getUtility(IEngineFactory,
                                                   name=self.engine)
             kw['bind'] = engine_factory()
-        return sqlalchemy.orm.create_session(**kw)
-    
+        session = sqlalchemy.orm.create_session(**kw)
+        register(session)
+        return session
+
     def scopeFunc(self):
-        return thread.get_ident()
+        return get_ident()
+
 
 def _zope_session_defaults(kw):
     """Adjust keyword parameters with proper defaults for Zope.
     """
 
     d = SESSION_DEFAULTS.copy()
     d.update(kw)
 
     return d
 
-class SiteScopedSession(object):
+
+@implementer(ISiteScopedSession)
+class SiteScopedSession:
     """A session that is scoped per site.
 
     Even though this makes the sessions scoped per site,
     the utility can be registered globally to make this work.
-    
+
     Creation arguments as for GloballyScopedSession, except that no ``bind``
     parameter should be passed. This means it is possible to create
     a SiteScopedSession utility without passing parameters to its constructor.
     """
-    implements(ISiteScopedSession)
-    
-    def __init__(self, engine=u'', **kw):
+
+    def __init__(self, engine='', **kw):
         assert 'bind' not in kw
         self.engine = engine
         self.kw = _zope_session_defaults(kw)
-        
+
     def sessionFactory(self):
         engine_factory = component.getUtility(IEngineFactory,
                                               name=self.engine)
         kw = self.kw.copy()
         kw['bind'] = engine_factory()
-        return sqlalchemy.orm.create_session(**kw)
+        session = sqlalchemy.orm.create_session(**kw)
+        register(session)
+        return session
 
     def scopeFunc(self):
-        return (thread.get_ident(), self.siteScopeFunc())
+        return (get_ident(), self.siteScopeFunc())
 
     def siteScopeFunc(self):
         raise NotImplementedError
 
 # Credits: This method of storing engines lifted from zope.app.cache.ram
+
+
 _COUNTER = 0
 _COUNTER_LOCK = threading.Lock()
 
 _ENGINES = {}
 _ENGINES_LOCK = threading.Lock()
 
-class EngineFactory(object):
+
+@implementer(IEngineFactory)
+class EngineFactory:
     """An engine factory.
 
     If you need engine connection parameters to be different per site,
     EngineFactory should be registered as a local utility in that
     site.
 
     If you want this utility to be persistent, you should subclass it
     and mixin Persistent. You could then manage the parameters
     differently than is done in this __init__, for instance as
     attributes, which is nicer if you are using Persistent (or Zope 3
     schema). In this case you need to override the configuration method.
     """
-    implements(IEngineFactory)
 
     def __init__(self, *args, **kw):
         self._args = args
         self._kw = kw
         self._key = self._getKey()
 
     def _getKey(self):
         """Get a unique key"""
         global _COUNTER
         _COUNTER_LOCK.acquire()
         try:
             _COUNTER += 1
-            return  "%s_%f_%d" % (id(self), time.time(), _COUNTER)
+            return "%s_%f_%d" % (id(self), time.time(), _COUNTER)
         finally:
             _COUNTER_LOCK.release()
-    
+
     def __call__(self):
         # optimistically try get without lock
         engine = _ENGINES.get(self._key, None)
         if engine is not None:
             return engine
         # no engine, lock and redo
         _ENGINES_LOCK.acquire()
         try:
             # need to check, another thread may have got there first
             if self._key not in _ENGINES:
                 args, kw = self.configuration()
                 _ENGINES[self._key] = engine = sqlalchemy.create_engine(
                     *args, **kw)
-                notify(EngineCreatedEvent(engine))
+                notify(EngineCreatedEvent(engine, args, kw))
             return _ENGINES[self._key]
         finally:
             _ENGINES_LOCK.release()
 
     def configuration(self):
         """Returns engine parameters.
```

### Comparing `z3c.saconfig-0.9.1/src/z3c/saconfig/zcml.py` & `z3c.saconfig-1.0/src/z3c/saconfig/zcml.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,104 +1,169 @@
+import warnings
+
+import zope.component.zcml
 import zope.interface
 import zope.schema
-import zope.component.zcml
+from zope.component.security import PublicPermission
 from zope.configuration.name import resolve
 
-import utility
-import interfaces
+from .interfaces import IEngineFactory
+from .interfaces import IScopedSession
+from .utility import EngineFactory
+
 
 class IEngineDirective(zope.interface.Interface):
     """Registers a database engine factory."""
 
     url = zope.schema.URI(
-        title=u"Database URL",
-        description=u"e.g. 'sqlite:///:memory:'.",
+        title='Database URL',
+        description="e.g. 'sqlite:///:memory:'.",
         required=True)
 
     name = zope.schema.Text(
-        title=u"Engine name",
-        description=u"Empty if this is the default engine.",
+        title="Engine name",
+        description="Empty if this is the default engine.",
         required=False,
-        default=u"")
+        default='')
 
     convert_unicode = zope.schema.Bool(
-        title=u'Convert all string columns to unicode',
-        description=u'This setting makes the SQLAlchemy String column type '
-                    u'equivalent to UnicodeString. Do not use this unless '
-                    u'there is a good reason not to use standard '
-                    u'UnicodeString columns',
+        title='Convert all string columns to unicode',
+        description='This setting makes the SQLAlchemy String column type '
+                    'equivalent to UnicodeString. Do not use this unless '
+                    'there is a good reason not to use standard '
+                    'UnicodeString columns',
         required=False,
         default=False)
-    
+
     echo = zope.schema.Bool(
-        title=u'Echo SQL statements',
-        description=u'Enable logging statements for debugging.',
+        title='Echo SQL statements',
+        description='Enable logging statements for debugging.',
         required=False,
-        default=False)
-    
+        default=None)
+
     setup = zope.schema.BytesLine(
-        title=u'After engine creation hook',
-        description=u'Callback for creating mappers etc. One argument is passed, the engine',
+        title='After engine creation hook',
+        description='Callback for creating mappers etc. '
+                    'One argument is passed, the engine',
         required=False,
         default=None)
-    
+
+    # Connection pooling options - probably only works on SQLAlchemy 0.5 and up
+
+    pool_size = zope.schema.Int(
+        title="The size of the pool to be maintained",
+        description="Defaults to 5 in SQLAlchemy.",
+        required=False)
+
+    max_overflow = zope.schema.Int(
+        title="The maximum overflow size of the pool.",
+        description="When the number of checked-out connections "
+                    "reaches the size set in pool_size, additional "
+                    "connections will be returned up to this limit. "
+                    "Defaults to 10 in SQLAlchemy",
+        required=False)
+
+    pool_recycle = zope.schema.Int(
+        title="Number of seconds between connection recycling",
+        description="Upon checkout, if this timeout is "
+                    "surpassed the connection will be closed and "
+                    "replaced with a newly opened connection",
+        required=False)
+
+    pool_timeout = zope.schema.Int(
+        title="The number of seconds to wait before giving up on "
+              "returning a connection.",
+        description="Defaults to 30 in SQLAlchemy if not set",
+        required=False)
+
 
 class ISessionDirective(zope.interface.Interface):
     """Registers a database scoped session"""
 
     name = zope.schema.Text(
-        title=u"Scoped session name",
-        description=u"Empty if this is the default session.",
+        title="Scoped session name",
+        description="Empty if this is the default session.",
         required=False,
-        default=u"")
+        default="")
 
     twophase = zope.schema.Bool(
-        title=u'Use two-phase commit',
-        description=u'Session should use two-phase commit',
+        title='Use two-phase commit',
+        description='Session should use two-phase commit',
         required=False,
         default=False)
 
     engine = zope.schema.Text(
-        title=u"Engine name",
-        description=u"Empty if this is to use the default engine.",
+        title="Engine name",
+        description="Empty if this is to use the default engine.",
         required=False,
-        default=u"")
+        default="")
 
     factory = zope.schema.DottedName(
-        title=u'Scoped Session utility factory',
-        description=u'GloballyScopedSession by default',
+        title='Scoped Session utility factory',
+        description='GloballyScopedSession by default',
         required=False,
         default="z3c.saconfig.utility.GloballyScopedSession")
 
 
-def engine(_context, url, name=u"", convert_unicode=False, echo=False, setup=None, twophase=False):
-    factory = utility.EngineFactory(
-        url, echo=echo, convert_unicode=convert_unicode)
-    
+def engine(_context, url, name="", convert_unicode=False,
+           echo=None, setup=None, twophase=False,
+           pool_size=None, max_overflow=None, pool_recycle=None,
+           pool_timeout=None):
+
+    if convert_unicode:  # pragma: no cover
+        warnings.warn(
+            '`convert_unicode` is no longer suported by SQLAlchemy, so it is'
+            ' ignored here.', DeprecationWarning)
+
+    kwargs = {
+        'echo': echo,
+    }
+
+    # Only add these if they're actually set, since we want to let SQLAlchemy
+    # control the defaults
+    if pool_size is not None:
+        kwargs['pool_size'] = pool_size
+    if max_overflow is not None:
+        kwargs['max_overflow'] = max_overflow
+    if pool_recycle is not None:
+        kwargs['pool_recycle'] = pool_recycle
+    if pool_timeout is not None:
+        kwargs['pool_timeout'] = pool_timeout
+
+    factory = EngineFactory(url, **kwargs)
+
     zope.component.zcml.utility(
         _context,
-        provides=interfaces.IEngineFactory,
+        provides=IEngineFactory,
         component=factory,
-        permission=zope.component.zcml.PublicPermission,
+        permission=PublicPermission,
         name=name)
-    
+
     if setup:
+        if isinstance(setup, bytes):
+            setup = setup.decode()
+
         if _context.package is None:
             callback = resolve(setup)
         else:
             callback = resolve(setup, package=_context.package.__name__)
-        callback(factory())
+        _context.action(
+            discriminator=(IEngineFactory, name),
+            callable=callback,
+            args=(factory(), ),
+            order=9999)
+
 
-def session(_context, name=u"", engine=u"", twophase=False,
+def session(_context, name="", engine="", twophase=False,
             factory="z3c.saconfig.utility.GloballyScopedSession"):
     if _context.package is None:
         ScopedSession = resolve(factory)
     else:
         ScopedSession = resolve(factory, package=_context.package.__name__)
     scoped_session = ScopedSession(engine=engine, twophase=twophase)
 
     zope.component.zcml.utility(
         _context,
-        provides=interfaces.IScopedSession,
+        provides=IScopedSession,
         component=scoped_session,
-        permission=zope.component.zcml.PublicPermission,
+        permission=PublicPermission,
         name=name)
```

### Comparing `z3c.saconfig-0.9.1/INSTALL.txt` & `z3c.saconfig-1.0/INSTALL.rst`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 Normally this code would be set up an as egg. If you want help with
 development, you can install it as a buildout.
 
 Installation
 ============
 
 This package can be checked out from
-svn://svn.zope.org/repos/main/z3c.saconfig/trunk. You can then execute
+https://github.com/zopefoundation/z3c.saconfig. You can then execute
 the buildout to download and install the requirements and install the
 test runner. Using your desired python run::
 
-  $ python bootstrap.py
+  $ python3 -m venv .
+  $ bin/pip install -r requirements.txt
 
 If installation configuration changes later, you need to run::
 
   $ bin/buildout
 
 Running the tests
 =================
@@ -30,15 +31,15 @@
 
 By default, the tests are run against an in-memory SQLite database.
 
 To enable testing with your own database set the ``TEST_DSN`` and
 ``TEST_DSN2`` environment variables to your sqlalchemy database dsn::
 
   $ export TEST_DSN=postgres://test:test@localhost/test
- 
+
 Since the tests also need access to a second, independent database,
 you also need to define a TEST_DSN2 that points to a different
 database::
 
   $ export TEST_DSN2=postgres://test:test@localhost/test2
 
 Two-phase commit behaviour may be tested by setting the TEST_TWOPHASE
```

