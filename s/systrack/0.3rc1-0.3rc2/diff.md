# Comparing `tmp/systrack-0.3rc1.tar.gz` & `tmp/systrack-0.3rc2.tar.gz`

## Comparing `systrack-0.3rc1.tar` & `systrack-0.3rc2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 systrack-0.3rc1/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/__init__.py
--rw-r--r--   0        0        0    11563 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/__main__.py
--rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/elf.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/kconfig.py
--rw-r--r--   0        0        0    26227 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/kconfig_options.py
--rw-r--r--   0        0        0    21459 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/kernel.py
--rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/location.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/output.py
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/signature.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/syscall.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/type_hints.py
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/utils.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/version.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/all.py
--rw-r--r--   0        0        0    10269 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/arch_base.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/arm.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/arm64.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/mips.py
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/powerpc.py
--rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/arch/x86.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/templates/syscall_table.css
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/templates/syscall_table.html
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 systrack-0.3rc1/src/systrack/templates/syscall_table.js
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 systrack-0.3rc1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 systrack-0.3rc1/LICENSE
--rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 systrack-0.3rc1/README.md
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 systrack-0.3rc1/pyproject.toml
--rw-r--r--   0        0        0    47672 2020-02-02 00:00:00.000000 systrack-0.3rc1/PKG-INFO
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 systrack-0.3rc2/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/__init__.py
+-rw-r--r--   0        0        0    11563 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/__main__.py
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/elf.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/kconfig.py
+-rw-r--r--   0        0        0    26320 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/kconfig_options.py
+-rw-r--r--   0        0        0    21459 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/kernel.py
+-rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/location.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/output.py
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/signature.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/syscall.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/type_hints.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/utils.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/version.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/all.py
+-rw-r--r--   0        0        0    10299 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/arch_base.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/arm.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/arm64.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/mips.py
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/powerpc.py
+-rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/x86.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/templates/syscall_table.css
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/templates/syscall_table.html
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/templates/syscall_table.js
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 systrack-0.3rc2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 systrack-0.3rc2/LICENSE
+-rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 systrack-0.3rc2/README.md
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 systrack-0.3rc2/pyproject.toml
+-rw-r--r--   0        0        0    47672 2020-02-02 00:00:00.000000 systrack-0.3rc2/PKG-INFO
```

### Comparing `systrack-0.3rc1/CHANGELOG.md` & `systrack-0.3rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/__main__.py` & `systrack-0.3rc2/src/systrack/__main__.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/elf.py` & `systrack-0.3rc2/src/systrack/elf.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/kconfig.py` & `systrack-0.3rc2/src/systrack/kconfig.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/kconfig_options.py` & `systrack-0.3rc2/src/systrack/kconfig_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,14 +261,15 @@
 	(VERSION_ZERO, VERSION_INF, 'send'                   , 'NET'                             ),
 	(VERSION_ZERO, VERSION_INF, 'sendmmsg'               , 'NET'                             ),
 	(VERSION_ZERO, VERSION_INF, 'sendmsg'                , 'NET'                             ),
 	(VERSION_ZERO, VERSION_INF, 'sendto'                 , 'NET'                             ),
 	(VERSION_ZERO, VERSION_INF, 'setsockopt'             , 'NET'                             ),
 	(VERSION_ZERO, VERSION_INF, 'shutdown'               , 'NET'                             ),
 	(VERSION_ZERO, VERSION_INF, 'socket'                 , 'NET'                             ),
+	(VERSION_ZERO, VERSION_INF, 'socketcall'             , 'NET'                             ),
 	(VERSION_ZERO, VERSION_INF, 'socketpair'             , 'NET'                             ),
 	(VERSION_ZERO, (3, 1)     , 'nfsservctl'             , 'NFSD'                            ), # dead
 	(VERSION_ZERO, VERSION_INF, 'mbind'                  , 'NUMA'                            ),
 	(VERSION_ZERO, VERSION_INF, 'migrate_pages'          , 'MIGRATION'                       ),
 	(VERSION_ZERO, VERSION_INF, 'move_pages'             , 'MIGRATION'                       ),
 	(VERSION_ZERO, VERSION_INF, 'get_mempolicy'          , 'NUMA'                            ),
 	(VERSION_ZERO, VERSION_INF, 'set_mempolicy'          , 'NUMA'                            ),
```

### Comparing `systrack-0.3rc1/src/systrack/kernel.py` & `systrack-0.3rc2/src/systrack/kernel.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/location.py` & `systrack-0.3rc2/src/systrack/location.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/output.py` & `systrack-0.3rc2/src/systrack/output.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/signature.py` & `systrack-0.3rc2/src/systrack/signature.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/syscall.py` & `systrack-0.3rc2/src/systrack/syscall.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/utils.py` & `systrack-0.3rc2/src/systrack/utils.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/arch/__init__.py` & `systrack-0.3rc2/src/systrack/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/arch/arch_base.py` & `systrack-0.3rc2/src/systrack/arch/arch_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,16 @@
 		to be able to correctly identify a syscall. Overriding this shouldn't be
 		needed in most cases.
 
 		This default implementation just removes prefixes/suffixes that are not
 		common enough to be indentified as common prefixes and stripped
 		automatically.
 		'''
-		return noprefix(sym_name, 'ptregs_sys_', 'ptregs_compat_sys_', '__se_sys_', '__sys_')
+		return noprefix(sym_name, 'ptregs_sys_', 'ptregs_compat_sys_',
+			'__se_compat_sys_', '__se_sys_', '__sys_', 'compat_sys_')
 
 	def normalize_syscall_name(self, name: str) -> str:
 		'''Normalize a syscall name removing unneeded prefixes and suffixes.
 		These are prefixes/suffixes that are ACTUALLY PRESENT IN THE SOURCE,
 		and not just in the symbol name.
 
 		This generic method oly handles common prefixes/suffixes. Arch-specific
@@ -241,15 +242,15 @@
 		should only override ._dummy_syscall_code().
 		'''
 		code = self._dummy_syscall_code(sc, vmlinux)
 		if code is None:
 			return False
 
 		logging.info('Syscall %s (%s) is not really implemented (dummy '
-			'implementation). Machine code: %s.', sc.name, sc.symbol.name, code.hex())
+			'implementation), code: %s.', sc.name, sc.symbol.name, code.hex())
 		return True
 
 	def adjust_syscall_number(self, number: int) -> int:
 		'''Adjust the number for the given syscall according to any
 		arch-specific quirk there might be (e.g. PowerPC with its interleaved
 		syscall numbers).
 		'''
```

### Comparing `systrack-0.3rc1/src/systrack/arch/arm.py` & `systrack-0.3rc2/src/systrack/arch/arm.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/arch/arm64.py` & `systrack-0.3rc2/src/systrack/arch/arm64.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/arch/mips.py` & `systrack-0.3rc2/src/systrack/arch/mips.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/arch/powerpc.py` & `systrack-0.3rc2/src/systrack/arch/powerpc.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/arch/x86.py` & `systrack-0.3rc2/src/systrack/arch/x86.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Tuple, List, Type, Optional
-
+import logging
 from ..syscall import Syscall
 from ..elf import Symbol, ELF, E_MACHINE
 from ..utils import VersionedDict, noprefix
 from ..type_hints import KernelVersion
 from ..kconfig_options import VERSION_ZERO, VERSION_INF
 
 from .arch_base import Arch
@@ -169,14 +169,20 @@
 
 		# vm86 and vm86old are only available in 32-bit kernels, but might still
 		# be implemented as simple wrappers that print a warning to dmesg and
 		# return -ENOSYS in 64-bit kernels, so ignore them
 		if self.abi == 'ia32' and not self.bits32 and sc.number in (113, 166):
 			return True
 
+		# pkey_{alloc,free,mprotect} can exist for compat 32-bit mode on 64-bit
+		# kernels (interesting), but definitely do not exist for 32-bit kernels,
+		# so avoid wasting time with these
+		if self.abi == 'ia32' and self.bits32 and sc.number in (380, 381, 382):
+			return True
+
 		return False
 
 	def translate_syscall_symbol_name(self, sym_name: str) -> str:
 		sym_name = super().translate_syscall_symbol_name(sym_name)
 		# For whatever reason some syscalls are wrapped in assembly at the entry
 		# point e.g. in v4.0 stub_execve in arch/x86/kernel/entry_64.S or
 		# stub32_execve in arch/x86/ia32/ia32entry.S. These stubs with prefix
@@ -197,32 +203,41 @@
 	def normalize_syscall_name(self, name: str) -> str:
 		name = super().normalize_syscall_name(name)
 		# E.g. v5.18 COMPAT_SYSCALL_DEFINE1(ia32_mmap, ...)
 		return noprefix(name, 'ia32_', 'x86_', 'x32_')
 
 	def _dummy_syscall_code(self, sc: Syscall, vmlinux: ELF) -> Optional[bytes]:
 		# Check if the code of the syscall only consists of
-		# `MOV rax/eax, -ENOSYS/-EINVAL` followed by a RET or relative JMP, e.g.
-		# lookup_dcookie in v5.19:
+		# `MOV rax/eax, -ENOSYS/-EINVAL` followed by a RET or relative JMP and
+		# optionally preceded by an ENDBR64/32. E.G., lookup_dcookie in v6.3:
 		#
-		#     48 c7 c0 da ff ff ff     mov    rax,  0xffffffffffffffda
-		#     e9 84 ca f6 00           jmp    0xf6ca90
+		# <__x64_sys_lookup_dcookie>:
+		#        f3 0f 1e fa             endbr64
+		#        48 c7 c0 da ff ff ff    mov    rax,0xffffffffffffffda
+		#        e9 74 8d 90 00          jmp    ffffffff819b8b84 <__x86_return_thunk>
 		#
+		# TODO: relies on the symbol having a valid size (!= 0), improve?
 		sz = sc.symbol.size
-		if sz < 6 or sz > 12:
+		if sz < 6 or sz > 16:
 			return None
 
-		code = vmlinux.read_symbol(sc.symbol)
+		orig = code = vmlinux.read_symbol(sc.symbol)
 		bad_imm = (b'\xda\xff\xff\xff', b'\xea\xff\xff\xff')
 
-		if self.abi == 'ia32':
-			if code[:1] == b'\xb8' and code[1:5] in bad_imm: # mov eax, -ENOSYS/-EINVAL
-				if sz == 6  and code[5] == 0xc3: return code # ret
-				if sz == 7  and code[5] == 0xeb: return code # jmp rel8
-				if sz == 10 and code[5] == 0xe9: return code # jmp rel32
-			return None
+		# endbr64/endbr32
+		if code.startswith(b'\xf3\x0f\x1e\xfa') or code.startswith(b'\xf3\x0f\x1e\xfb'):
+			code = code[4:]
+			sz -= 4
+
+		# 32-bit kernel
+		if code[:1] == b'\xb8' and code[1:5] in bad_imm: # mov eax, -ENOSYS/-EINVAL
+			if sz == 6  and code[5] == 0xc3: return orig # ret
+			if sz == 7  and code[5] == 0xeb: return orig # jmp rel8
+			if sz == 10 and code[5] == 0xe9: return orig # jmp rel32
 
+		# 64-bit kernel
 		if code[:3] == b'\x48\xc7\xc0' and code[3:7] in bad_imm: # mov rax, -ENOSYS/-EINVAL
-			if sz == 8  and code[7] == 0xc3: return code # ret
-			if sz == 9  and code[7] == 0xeb: return code # jmp rel8
-			if sz == 12 and code[7] == 0xe9: return code # jmp rel32
+			if sz == 8  and code[7] == 0xc3: return orig # ret
+			if sz == 9  and code[7] == 0xeb: return orig # jmp rel8
+			if sz == 12 and code[7] == 0xe9: return orig # jmp rel32
+
 		return None
```

### Comparing `systrack-0.3rc1/src/systrack/templates/syscall_table.css` & `systrack-0.3rc2/src/systrack/templates/syscall_table.css`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/templates/syscall_table.html` & `systrack-0.3rc2/src/systrack/templates/syscall_table.html`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/src/systrack/templates/syscall_table.js` & `systrack-0.3rc2/src/systrack/templates/syscall_table.js`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/LICENSE` & `systrack-0.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/README.md` & `systrack-0.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/pyproject.toml` & `systrack-0.3rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc1/PKG-INFO` & `systrack-0.3rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systrack
-Version: 0.3rc1
+Version: 0.3rc2
 Summary: Linux kernel syscall implementation tracker
 Project-URL: homepage, https://github.com/mebeim/systrack
 Project-URL: repository, https://github.com/mebeim/systrack.git
 Author-email: Marco Bonelli <marco@mebeim.net>
 Maintainer-email: Marco Bonelli <marco@mebeim.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

