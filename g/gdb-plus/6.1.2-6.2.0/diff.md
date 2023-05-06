# Comparing `tmp/gdb_plus-6.1.2.tar.gz` & `tmp/gdb_plus-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdb_plus-6.1.2.tar", last modified: Thu May  4 11:33:59 2023, max compression
+gzip compressed data, was "gdb_plus-6.2.0.tar", last modified: Sat May  6 10:25:50 2023, max compression
```

## Comparing `gdb_plus-6.1.2.tar` & `gdb_plus-6.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-04 11:33:59.265838 gdb_plus-6.1.2/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.1.2/LICENSE
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11532 2023-05-04 11:33:59.264915 gdb_plus-6.1.2/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11293 2023-05-04 10:56:05.000000 gdb_plus-6.1.2/README.md
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-04 11:33:59.243924 gdb_plus-6.1.2/gdb_plus/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11017 2023-05-04 10:40:58.000000 gdb_plus-6.1.2/gdb_plus/Inner_Debugger.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-05-04 10:40:57.000000 gdb_plus-6.1.2/gdb_plus/__init__.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)    76260 2023-05-04 10:49:43.000000 gdb_plus-6.1.2/gdb_plus/gdb_plus.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)     4775 2023-05-04 10:40:58.000000 gdb_plus-6.1.2/gdb_plus/utils.py
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-04 11:33:59.259086 gdb_plus-6.1.2/gdb_plus.egg-info/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11532 2023-05-04 11:33:59.000000 gdb_plus-6.1.2/gdb_plus.egg-info/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)      292 2023-05-04 11:33:59.000000 gdb_plus-6.1.2/gdb_plus.egg-info/SOURCES.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-05-04 11:33:59.000000 gdb_plus-6.1.2/gdb_plus.egg-info/dependency_links.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-05-04 11:33:59.000000 gdb_plus-6.1.2/gdb_plus.egg-info/requires.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-05-04 11:33:59.000000 gdb_plus-6.1.2/gdb_plus.egg-info/top_level.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)      656 2023-05-04 11:30:52.000000 gdb_plus-6.1.2/pyproject.toml
--rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-05-04 11:33:59.266155 gdb_plus-6.1.2/setup.cfg
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-04 11:33:59.261759 gdb_plus-6.1.2/tests/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    17663 2023-05-04 11:33:14.000000 gdb_plus-6.1.2/tests/test.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-06 10:25:50.876994 gdb_plus-6.2.0/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.2.0/LICENSE
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    12629 2023-05-06 10:25:50.875850 gdb_plus-6.2.0/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    12410 2023-05-06 08:12:37.000000 gdb_plus-6.2.0/README.md
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-06 10:25:50.833814 gdb_plus-6.2.0/gdb_plus/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    11259 2023-05-06 01:40:48.000000 gdb_plus-6.2.0/gdb_plus/Inner_Debugger.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-05-05 17:49:09.000000 gdb_plus-6.2.0/gdb_plus/__init__.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    84636 2023-05-06 08:12:37.000000 gdb_plus-6.2.0/gdb_plus/gdb_plus.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    74194 2023-05-06 08:12:30.000000 gdb_plus-6.2.0/gdb_plus/gdb_plus_dev_libdebug.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)     5031 2023-05-06 01:38:11.000000 gdb_plus-6.2.0/gdb_plus/utils.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-06 10:25:50.863436 gdb_plus-6.2.0/gdb_plus.egg-info/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    12629 2023-05-06 10:25:50.000000 gdb_plus-6.2.0/gdb_plus.egg-info/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      326 2023-05-06 10:25:50.000000 gdb_plus-6.2.0/gdb_plus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-05-06 10:25:50.000000 gdb_plus-6.2.0/gdb_plus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-05-06 10:25:50.000000 gdb_plus-6.2.0/gdb_plus.egg-info/requires.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-05-06 10:25:50.000000 gdb_plus-6.2.0/gdb_plus.egg-info/top_level.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      656 2023-05-06 01:40:57.000000 gdb_plus-6.2.0/pyproject.toml
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-05-06 10:25:50.877347 gdb_plus-6.2.0/setup.cfg
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-06 10:25:50.865858 gdb_plus-6.2.0/tests/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    17513 2023-05-06 01:38:11.000000 gdb_plus-6.2.0/tests/test.py
```

### Comparing `gdb_plus-6.1.2/LICENSE` & `gdb_plus-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.1.2/PKG-INFO` & `gdb_plus-6.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb_plus
-Version: 6.1.2
+Version: 6.2.0
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
@@ -84,32 +84,45 @@
 Debugger can also take as parameter a dictionary for the environment variables. You CAN use it to preload libraries, but if you want to do it for the libc I would advise to **patch the rpath** of the binary instead (if you don't know how take a look at [spwn](https://github.com/MarcoMarce) or [pwninit](https://github.com/io12/pwninit). This will prevent problems when running `system("/bin/sh")` that will fail due to LD_PRELOAD and may hide other problems in your exploit.
 
 **Warning**  
 Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped
 
 ## Control Flow
 
-The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require calling `dbg.wait()`.
+The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require you to call `dbg.wait()`.
 
 ```py
+dbg.jump() # set instruction pointer to specific address
 dbg.step() # Single instruction (will enter function calls)
 dbg.next() # Next instruction (will jump over function calls)
 dbg.cont() # Continue execution
+dbg.continue_until() # Continue until you reach a specific location
 dbg.finish() # Finish current function
 dbg.interrupt() # Stop the execution of your process
 dbg.wait() # Wait until you have control of gdb
 ```
 
-**Note**
-* dbg.cont(until=ADDRESS) allows you to block your script until you reach a specific address (or symbol). This means that you can debug manually with gdb while your script is waiting without problems
+In the cases where you have to interact with the process before reaching the address you want or if you would like to put some more breakpoints on the way to play manually with gdb you can use wait=False
+
+```py
+...
+dbg.breakpoint("main+0x12", temporary=True)
+dbg.breakpoint(0x23, temporary=True)
+done = dbg.continue_until("main+0x43", wait=False)
+dbg.p.recvline()
+dbg.p.sendline(b"4")
+done.wait()
+# Here the script will wait until you reach the offset 0x43 from main while gdb will break at offset 0x12 and 0x23 to let you look at the process
+...
+```
 
 **Warning**  
 * `finish` can only work if the stack frame hasn't been corrupted
-* you should specify if you want continue to wait or not with `dbg.cont(wait=True/False)`. We aren't sure about what should be the default behaviour and may set it to `wait=True` in a future version
 * Try avoiding `interrupt` as much as possible. 
+* You may be tempted to do `dbg.instruction_pointer = dbg.parse_address(location)`, but a bug in gdb may cause an unexpected behaviour if you do so. Use `dbg.jump(location)` instead
 
 If the function modifies itself you may find yourself unable to set breakpoints where you want. To analyse these function we can run them step by step
 
 ```py
 def MyCallback(dbg):
     if dbg.next_inst.mnemonic == "int3":
         dbg.step()
@@ -208,37 +221,41 @@
 We can also use capstone to know what is the next instruction that will be executed
 ```py
 print(dbg.next_inst.toString()) # "mov rax, r12"
 print(dbg.next_inst.mnemonic)   # "mov"
 ```
 
 ## Fork
-You can set the debugger to spwn a new instance of gdb every time the process calls fork with `dbg.set_split_on_fork()`.
+You can set the debugger to spwn a new instance of gdb every time the process calls fork with `dbg.set_split_on_fork()`. The child will stop as soon as the process is created by fork, but will wait for the debugger to stop before creating the new object
 
 ```py
 dbg = Debugger("http_server").set_split_on_fork()
-dbg.cont(wait=False)
+done = dbg.continue_until(0x40233)
 dbg.p.sendline("input")
+done.wait()
+# Now that the process stopped at address 0x40233 a new debugger will attach to the child
 pid_child = dbg.wait_split()
 
-# all children are saved in dbg.children and can be accessed by the pid
+# all children have their debugger saved in dbg.children and can be accessed by the pid
 child = dbg.children[pid_child]
 ```
 
 If the program traces its child to make sure you aren't debugging it or to unpack a region of code, you should be able to emulate the calls to ptrace. 
 
 ```py
 child.emulate_ptrace_slave(dbg)
 dbg.emulate_ptrace_master(child)
 ```
 
-This will interrupt the process at every call to waitpid for the master and SIGSTOP or INT3 for the child. You have to handle yourself when to let each one of them continue while you debug them.
+This will interrupt the process at every call to waitpid for the master and SIGSTOP or INT3 for the child. You have to handle yourself when to let each one of them continue while you debug them. To help you a bit we print "Slave can continue" every time the tracer tries to send a continue to the tracee
 
 **Warning**
-pwndbg can not handle multi-process applications and this section is only possible in native gdb or with GEF
+* If the tracee stopped with a SIGSTOP gdb may bug a bit and you may need `force=True` to make it continue correctly
+* pwndbg can not handle multi-process applications and this section is only possible in native gdb or with GEF
+* Handleling multiple processes in the same debugger instead of splitting them may cause problems whith the waits
 
 ## Call functions
 
 If you want to test the effects of a specific function you can directly call it with the parameters you want
 
 ```py
 pointer = dbg.alloc(100)
@@ -262,8 +279,9 @@
 # TODO
 
 * Add option to use libdebug instead of gdb
 * Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
+    * register waitpid return value
 * Maybe nop split_on_fork&co while debugging is False
```

### Comparing `gdb_plus-6.1.2/README.md` & `gdb_plus-6.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,32 +70,45 @@
 Debugger can also take as parameter a dictionary for the environment variables. You CAN use it to preload libraries, but if you want to do it for the libc I would advise to **patch the rpath** of the binary instead (if you don't know how take a look at [spwn](https://github.com/MarcoMarce) or [pwninit](https://github.com/io12/pwninit). This will prevent problems when running `system("/bin/sh")` that will fail due to LD_PRELOAD and may hide other problems in your exploit.
 
 **Warning**  
 Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped
 
 ## Control Flow
 
-The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require calling `dbg.wait()`.
+The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require you to call `dbg.wait()`.
 
 ```py
+dbg.jump() # set instruction pointer to specific address
 dbg.step() # Single instruction (will enter function calls)
 dbg.next() # Next instruction (will jump over function calls)
 dbg.cont() # Continue execution
+dbg.continue_until() # Continue until you reach a specific location
 dbg.finish() # Finish current function
 dbg.interrupt() # Stop the execution of your process
 dbg.wait() # Wait until you have control of gdb
 ```
 
-**Note**
-* dbg.cont(until=ADDRESS) allows you to block your script until you reach a specific address (or symbol). This means that you can debug manually with gdb while your script is waiting without problems
+In the cases where you have to interact with the process before reaching the address you want or if you would like to put some more breakpoints on the way to play manually with gdb you can use wait=False
+
+```py
+...
+dbg.breakpoint("main+0x12", temporary=True)
+dbg.breakpoint(0x23, temporary=True)
+done = dbg.continue_until("main+0x43", wait=False)
+dbg.p.recvline()
+dbg.p.sendline(b"4")
+done.wait()
+# Here the script will wait until you reach the offset 0x43 from main while gdb will break at offset 0x12 and 0x23 to let you look at the process
+...
+```
 
 **Warning**  
 * `finish` can only work if the stack frame hasn't been corrupted
-* you should specify if you want continue to wait or not with `dbg.cont(wait=True/False)`. We aren't sure about what should be the default behaviour and may set it to `wait=True` in a future version
 * Try avoiding `interrupt` as much as possible. 
+* You may be tempted to do `dbg.instruction_pointer = dbg.parse_address(location)`, but a bug in gdb may cause an unexpected behaviour if you do so. Use `dbg.jump(location)` instead
 
 If the function modifies itself you may find yourself unable to set breakpoints where you want. To analyse these function we can run them step by step
 
 ```py
 def MyCallback(dbg):
     if dbg.next_inst.mnemonic == "int3":
         dbg.step()
@@ -194,37 +207,41 @@
 We can also use capstone to know what is the next instruction that will be executed
 ```py
 print(dbg.next_inst.toString()) # "mov rax, r12"
 print(dbg.next_inst.mnemonic)   # "mov"
 ```
 
 ## Fork
-You can set the debugger to spwn a new instance of gdb every time the process calls fork with `dbg.set_split_on_fork()`.
+You can set the debugger to spwn a new instance of gdb every time the process calls fork with `dbg.set_split_on_fork()`. The child will stop as soon as the process is created by fork, but will wait for the debugger to stop before creating the new object
 
 ```py
 dbg = Debugger("http_server").set_split_on_fork()
-dbg.cont(wait=False)
+done = dbg.continue_until(0x40233)
 dbg.p.sendline("input")
+done.wait()
+# Now that the process stopped at address 0x40233 a new debugger will attach to the child
 pid_child = dbg.wait_split()
 
-# all children are saved in dbg.children and can be accessed by the pid
+# all children have their debugger saved in dbg.children and can be accessed by the pid
 child = dbg.children[pid_child]
 ```
 
 If the program traces its child to make sure you aren't debugging it or to unpack a region of code, you should be able to emulate the calls to ptrace. 
 
 ```py
 child.emulate_ptrace_slave(dbg)
 dbg.emulate_ptrace_master(child)
 ```
 
-This will interrupt the process at every call to waitpid for the master and SIGSTOP or INT3 for the child. You have to handle yourself when to let each one of them continue while you debug them.
+This will interrupt the process at every call to waitpid for the master and SIGSTOP or INT3 for the child. You have to handle yourself when to let each one of them continue while you debug them. To help you a bit we print "Slave can continue" every time the tracer tries to send a continue to the tracee
 
 **Warning**
-pwndbg can not handle multi-process applications and this section is only possible in native gdb or with GEF
+* If the tracee stopped with a SIGSTOP gdb may bug a bit and you may need `force=True` to make it continue correctly
+* pwndbg can not handle multi-process applications and this section is only possible in native gdb or with GEF
+* Handleling multiple processes in the same debugger instead of splitting them may cause problems whith the waits
 
 ## Call functions
 
 If you want to test the effects of a specific function you can directly call it with the parameters you want
 
 ```py
 pointer = dbg.alloc(100)
@@ -248,8 +265,9 @@
 # TODO
 
 * Add option to use libdebug instead of gdb
 * Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
-* Maybe nop split_on_fork&co while debugging is False
+    * register waitpid return value
+* Maybe nop split_on_fork&co while debugging is False
```

### Comparing `gdb_plus-6.1.2/gdb_plus/Inner_Debugger.py` & `gdb_plus-6.2.0/gdb_plus/Inner_Debugger.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,28 +89,33 @@
     def _cont(self, wait = False):
         self.dbg.call("ptrace", [constants.PTRACE_CONT, self.pid, 0, 0])
         if wait:
             self.wait()
 
     # Please, never ever put two breakpoints next to each others as a user (using next is fine) [03/03/23]
     def cont(self, *, wait=False, until=None) -> None:
-        ip = self.instruction_pointer
         if until is not None:
-            address = self.dbg.parse_address(until)
-            self.b(address, temporary=True)
-            wait = True
-        # Attento a non fare riferimenti ciclici
-        if ip in self.breakpoints:
-            self.step()
-        self._cont(wait)
-        if until is not None and address != self.instruction_pointer:
-            log.critical(f"couldn't reach address {hex(address)}. Stopped at address {hex(self.instruction_pointer)} instead")
+            log.warn_once("dbg.cont(until=ADDRESS) is deprecated, use dbg.continue_until(ADDRESS) instead!")  
+            self.continue_until(until)  
+        self.step()
+        if self.instruction_pointer not in self.breakpoints:    
+            self._cont(wait)
 
     c = cont
 
+    def continue_until(self, location):
+        ip = self.instruction_pointer
+        address = self.dbg.parse_address(location)
+        self.b(address, temporary=True)
+        self.cont(wait=True)
+        if address != self.instruction_pointer:
+            log.critical(f"couldn't reach address {hex(address)}. Stopped at address {hex(self.instruction_pointer)} instead")
+
+    until = continue_until
+
     def interrupt(self) -> None:
         # PTRACE_INTERRUPT may not work
         #self.dbg.call(self.dbg.symbols["ptrace"], [constants.PTRACE_INTERRUPT.real, self.pid, 0, 0])
         kill(self.pid, signal.SIGINT)
         self.wait() # Necessario ? [03/03/23]
 
     def _set_breakpoint(self, address, temporary=False):
@@ -139,47 +144,48 @@
             self.write_memory(address, breakpoint.byte)
 
     def _enable_breakpoints(self):
         for address, breakpoint in self.breakpoints.items():
             byte = self.read_memory(address, 1)
             if byte != INT3:
                 breakpoint.byte = byte
-    # No need to emulate jumps. Ptrace can do it
+
     def step(self):
         constants.PTRACE_SINGLESTEP = 0x9
         ip = self.instruction_pointer
         self._disable_breakpoint(ip)
         self.dbg.call("ptrace", [constants.PTRACE_SINGLESTEP, self.pid, 0, 0])
         self.wait()
         self._restore_breakpoint(ip)
 
     def next(self):
         ip = self.instruction_pointer
         inst = self.next_inst
         if inst.mnemonic == "call":
             self._disable_breakpoint(ip)
-            self.cont(until=ip + inst.size)
+            self.until(ip + inst.size)
             self._restore_breakpoint(ip)
         else:
             self.step()
 
     def wait(self):
         status_pointer = self.dbg.alloc(4)
         self.dbg.call("waitpid", [self.pid, status_pointer, 0x40000000, 0])
-        # be carefull that INT3 is executed as an instruction! You have to back down
         
         log.debug(f"wait finished with status: {hex(u32(self.dbg.read(status_pointer, 4)))}")
         self.dbg.dealloc(status_pointer)
         
+        # be carefull that INT3 is executed as an instruction! You have to back down if you did hit a breakpoint
         ip = self.instruction_pointer - 1
         breakpoint = self.breakpoints.get(ip)
         
         if breakpoint is None:
             return
 
+        # What happens if I step over a breakpoint on an instruction of size 1 ?
         self.instruction_pointer = ip
 
         if breakpoint.temporary:
             self._disable_breakpoint(ip)
             del self.breakpoints[ip]
 
     def detach(self):
```

### Comparing `gdb_plus-6.1.2/gdb_plus/gdb_plus.py` & `gdb_plus-6.2.0/gdb_plus/gdb_plus_dev_libdebug.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from os import kill
 from time import sleep
 from functools import partial
 from capstone import Cs, CS_ARCH_X86
 from threading import Thread, Event
 from queue import Queue
 from gdb_plus.utils import Arguments, user_regs_struct, context, MyEvent, Breakpoint
+from libdebug import Debugger as lib_Debugger
 
 RET = b"\xc3"
-DEBUG_OFF = "Debug is off, commands won't be executed"
 
 class Debugger:
     # If possible patch the rpath (spwn and pwninit do it automatically) instead of using env to load the correct libc. This will let you get a shell not having problems trying to preload bash too
     def __init__(self, target: [int, process, str, list], env={}, aslr:bool=True, script:str="", from_start:bool=True, binary:str=None, debug_from: int=None, timeout: int=0.5):
         log.debug(f"debugging {target if binary is None else binary} using arch: {context.arch} [{context.bits}bits]")
 
         self._capstone = None #To decompile assembly for next_inst
@@ -55,16 +55,15 @@
             _, self.gdb = gdb.attach(target, gdbscript=script, api=True)
 
         elif args.REMOTE:
             self.elf = ELF(target, checksec=False) if binary is None else ELF(binary, checksec=False)
 
         elif context.noptrace:
             self.p = process(target, env=env, aslr=aslr)
-            self.elf = self.p.elf if binary is None else ELF(binary, checksec=False)
-
+            
         elif from_start:
             self.p = gdb.debug(target, env=env, aslr=aslr, gdbscript=script, api=True)
             self.gdb = self.p.gdb
 
         else:
             self.p = process(target, env=env, aslr=aslr)
             _, self.gdb = gdb.attach(self.p, gdbscript=script, api=True)
@@ -96,88 +95,78 @@
                 while True:  
                     self.detach()
                     sleep(timeout)
                     # what happens if there is a continue in script ? It should break the script, but usually it's the last instruction so who cares ? Just warn them in the docs [06/04/23]
                     _, self.gdb = gdb.attach(self.pid, gdbscript=script, api=True) # P is gdbserver...
                     if self.instruction_pointer - address_debug_from in range(0, len(backup)): # I'm in the sleep shellcode
                         self.write(address_debug_from, backup)
-                        # To allow call to wait inside the jump
-                        self.gdb.myStopped = self.gdb.stopped
-                        self.gdb.myStopped.priority = 0
-                        # should maybe rename priority_wait into wait and avoid this line [17/04/23]
-                        self.gdb.myStopped.priority_wait = lambda: self.gdb.myStopped.wait()
-                        self.jump(address_debug_from)
+                        self.instruction_pointer = address_debug_from
                         break
                     else:
                         log.warn(f"{timeout}s timeout isn't enought to reach the code... Retrying...")
 
-            self.__setup_gdb()
+        if libdebug:
+            self.migrate(libdebug=True)
 
-    # We stopped using gdb's implementation of temporary breakpoints so that we can differentiate an interruption caused by my debugger and cause by the manual use of gdb 
     def __stop_handler(self):
         """
         Actions that the debugger performs every time the process is interrupted
         Handle temporary breakpoints and callbacks
         """
         self.restore_arch()
-        ip = self.parse_address(self.instruction_pointer) # same as self.instruction_pointer right now, but let's stay safe in case we change something later [17/04/23]
+        ip = self.parse_address(self.instruction_pointer)
         bp = self.breakpoints.get(ip)
         if bp is None:
-            if self.stepped or self.interrupted or self._stop_reason in ["SIGSTOP", "SIGTRAP"]: # SIGTRAP to handle known int3 in the code
-                self.stepped == False
-                self.interrupted == False
-                self.__set_stop()
-            return
+            if not self.stepped and not self.interrupted:
+                raise Exception("How is it possible that libdebug stopped ?")
         
         if bp.temporary:
             self.delete_breakpoint(ip)
 
-        # TODO, it may be interesting to have the option to put an array of breakpoints for recursive functions [21/03/23]
-        # something like
-        #if type(self.real_callbacks[self.instruction_pointer]) is list:
-        #   callback =  self.real_callbacks[ip].pop()
-        #   if len(self.real_callbacks[ip]) == 0:
-        #       del self.real_callbacks[ip]
-        #else:
-                        
-        # This should let us keep control of the debugger even if we use gdb manually while emulating ptrace
-        # Doesn't handle the case where we use ni and hit the breakpoint though... [17/04/23] TODO!
-        # Doesn't even handle the case where I step, but I'm waiting in continue until
-        if bp.callback is not None and bp.callback(self) == False and self._stop_reason != "SINGLE STEP":
+        if bp.callback is not None and bp.callback(self) == False and not self.stepped:
             self.execute("c")
         else:
             self.__set_stop()
 
+        self.stepped = False
+        self.interrupted = False
         
-        
-    def __setup_gdb(self):
+    def __setup_debugger(self):
         """
         setup of gdb's events
         """
-        # MyEvent allows calls to wait in parallel
-        self.gdb.myStopped = MyEvent()
-        self.gdb.myStopped.set() # we call __setup_gdb after an attach so the process isn't running. Make just sure this doesn't cause troubles [17/04/23]
+        # Move in __init__ ? [28/04/23]
+        # Keep it here and put MyEvent(originalEvent) ? [28/04/23]
+        self.myStopped = MyEvent()
+        self.myStopped.set()
 
-        self.gdb.events.stop.connect(lambda event: Thread(target=self.__stop_handler).start())
+        self.libdebug.handle_stop = lambda dbg: Thread(target=self.__stop_handler).start()
         
         def exit_handler(event):
             log.debug("setting stop because process exited")
-            self.gdb.myStopped.set()
+            self.myStopped.set()
             self.closed.set()
 
-        self.gdb.events.exited.connect(exit_handler)
-
-        # Manually set by split_child
-        self.gdb.split = Queue()
+        self.libdebug.handle_exit = exit_handler
 
-        # Ptrace_cont
-        self.gdb.master_wants_you_to_continue = Event()
-        self.gdb.slave_has_stopped = Event()    
+    def migrate(self, *, gdb=False, libdebug=False):
+        self.migrated.clear()
+        backup = self.inject_sleep(address)
+        self.detach()
+        if gdb:
+            self.libdebug = None
+            self.gdb = pwn.gdb.attach(self.pid, api=True)
+        else:
+            self.gdb = None
+            self.libdebug = lib_Debugger()
+            self.libdebug.attach(self.pid)
+        self.write(address, backup)
+        self.instruction_pointer = address
+        self.__setup_debugger()
 
-    # Because pwntools isn't perfect
     def restore_arch(self):
         """
         check that the context used by pwntools is correct
         """
         if self.elf is not None and context.arch != self.elf.arch:
             log.debug("wrong context ! Updating...")
         context.arch = self.elf.arch
@@ -189,87 +178,78 @@
         wait dbg.debug_from_done to know when to continue
 
         event: optional event to signal that you have finished the actions you needed to perform. Otherwise a timeout of 0.5s will be used
         """
         address = self.parse_address(location)
 
         if self.debugging:
+            if self.libdebug is not None:
+                raise Exception("Migrate to libdebug after reaching your destination")
             def action():
                 backup = self.inject_sleep(address)
                 while True:  
                     self.detach()
                     if event is not None:
                         event.wait()
                         log.debug("user finished interaction. Proceeding with debug_from")
+                    log.warn("you haven't set an event to let me know when you finished interactiong with the process. I will give you half a second.")
                     sleep(timeout)
-                    # Maybe the process is being traced and I can't attach to it yet
                     try:
-                        # what happens if there is a continue in script ? It should break the script, but usually it's the last instruction so who cares ? Just warn them in the docs [06/04/23]
-                        _, self.gdb = gdb.attach(self.p.pid, gdbscript=self.gdbscript, api=True) # P is gdbserver...
+                        self.libdebug.attach(self.pid)
                     except Exception as e:
                         log.debug(f"can't attach in debug_from because of {e}... Retrying...")
                         continue
-                    self.__setup_gdb()
+                    self.__setup_debugger()
                     if self.instruction_pointer - address in range(0, len(backup)): # I'm in the sleep shellcode
                         self.write(address, backup)
                         self.jump(address)
                         self.debug_from_done.set()
                         break
                     else:
                         log.warn(f"{timeout}s timeout isn't enought to reach the code... Retrying...")
 
             Thread(target=action).start()
         else:
-            log.warn_once(DEBUG_OFF)
             self.debug_from_done.set()
         return self
 
-    # Use as : dbg = Debugger("file").remote(IP, PORT)
     def remote(self, host: str, port: int):
         """
         Define the connection to use when the script is called with argument REMOTE
         """
         if args.REMOTE:
             self.p = remote(host, port)
         return self
 
-    def detach(self, quit = True):
-        try:
-            self.execute("detach")
-        except:
-            log.debug("process already stopped")
-        try:
-            self.execute("quit") # Doesn't always work if after interacting manually
-        except EOFError:
-            log.debug("GDB successfully closed")
+    def detach(self):
+        if self.libdebug is not None:
+            self.libdebug.detach()
 
-    def close(self):
-        self.detach()
-        # Can't close the process if I just attached to the pid
-        if self.p:
-            self.p.close()
-
-    # Now we may have problems if the user try calling it...
-    # should warn to use execute_action and wait if they are doing something that will let the process run
-    def execute(self, code: str):
-        """ 
-        Execute a command that does NOT require a wait later
-        """
-        if self.debugging:
-            return self.gdb.execute(code, to_string=True)
         else:
-            log.warn_once(DEBUG_OFF)
+            try:
+                self.execute("detach")
+            except:
+                log.debug("process already stopped")
+            try:
+                self.execute("quit") # Doesn't always work if after interacting manually
+            except EOFError:
+                log.debug("GDB successfully closed")
 
-    # I want a function to restart the process without closing and opening a new one
-    # Not working properly
-    def reset(self, argv=None, reload_elf=False):
-        ...
+    def close(self):
+        if self.libdebug is not None:
+            # Is this what I should do ?
+            self.libdebug.close()
 
-    # Since reset doesn't work
-    # Could be expanded with memory regions
+        else:
+            self.detach()
+            # Can't close the process if I just attached to the pid
+            if self.p:
+                self.p.close()
+
+    # with libdebug we could do ptrace.getregs...
     def backup(self) -> list:
         """
         Save the state of all registers
         """
         values = []
         for register in self.special_registers + self.registers[:-1]: # exclude ip
             values.append(getattr(self, register))
@@ -321,35 +301,40 @@
         dbg.args[5] = 1 # Valid
         a, b = dbg.args[:2] # Not valid!
         """
         if self._args is None:
             self._args = Arguments(self)
         return self._args 
 
-    # Taken from GEF to handle slave interruption
+    # How do I parse it ?
     @property
     def _stop_reason(self) -> str:
-        res = self.gdb.execute("info program", to_string=True).splitlines()
-        if not res:
-            return "NOT RUNNING"
+        if self.libdebug is not None:
+            res = self.libdebug.__stop_status
+            ...
 
-        for line in res:
-            line = line.strip()
-            if line.startswith("It stopped with signal "):
-                return line.replace("It stopped with signal ", "").split(",", 1)[0]
-            if line == "The program being debugged is not being run.":
+        else:
+            res = self.gdb.execute("info program", to_string=True).splitlines()
+            if not res:
                 return "NOT RUNNING"
-            if line == "It stopped at a breakpoint that has since been deleted.":
-                return "TEMPORARY BREAKPOINT"
-            if line.startswith("It stopped at breakpoint "):
-                return "BREAKPOINT"
-            if line == "It stopped after being stepped.":
-                return "SINGLE STEP"
 
-        return "STOPPED"
+            for line in res:
+                line = line.strip()
+                if line.startswith("It stopped with signal "):
+                    return line.replace("It stopped with signal ", "").split(",", 1)[0]
+                if line == "The program being debugged is not being run.":
+                    return "NOT RUNNING"
+                if line == "It stopped at a breakpoint that has since been deleted.":
+                    return "TEMPORARY BREAKPOINT"
+                if line.startswith("It stopped at breakpoint "):
+                    return "BREAKPOINT"
+                if line == "It stopped after being stepped.":
+                    return "SINGLE STEP"
+
+            return "STOPPED"
 
     @property
     def _details_breakpoint_stopped(self) -> str:
         """
         If the program stopped at a breakpoint, return the id of that breakpoint
         This can be used to identify caught syscall
         """
@@ -365,21 +350,18 @@
    ########################## CONTROL FLOW ##########################
 
     # For commands that will make the process run and should handle priority
     def execute_action(self, command, sender=None):
         """
         Wrapper around execute to handle commands that will require a wait
         """
-        if self.debugging:
-            self.priority += 1
-            self.__clear_stop(sender if sender is not None else command)
-            self.execute(command)
-        else:
-            log.warn_once(DEBUG_OFF)
-            
+        self.priority += 1
+        self.__clear_stop(sender if sender is not None else command)
+        self.execute(command)
+
     # TODO make the option to have "until" be non blocking with an event when we reach the address [28/04/23] In other words migrate wait=False to wait=Event()
     def c(self, wait=False, force = False, until = None):
         """
         Continue execution of the process
 
         Arguments:
             wait: Should block your script until the next interruption ?
@@ -412,99 +394,92 @@
 
     def wait(self, timeout=None, legacy=False):
         """
         Wait for the process to stop after an action.
         Won't return until all future actions have been handled so that you can use it at the same time in your script and in a breakpoint
         """
         if legacy:
-            self.gdb.myStopped.wait(timeout)
+            self.myStopped.wait(timeout)
         else:
             self.priority_wait()
 
     # This should only be used under the hood, but how do we let the other one to the user without generating problems ? [14/04/23]
     def priority_wait(self):
-        if self.debugging:
-            self.gdb.myStopped.priority_wait()
-        else:
-            log.warn_once(DEBUG_OFF)
+        self.myStopped.priority_wait()
 
     # problems when I haven't executed anything
     @property
     def running(self):
-        return not self.gdb.myStopped.is_set()
+        return not self.myStopped.is_set()
 
     @property
     def priority(self):
-        return self.gdb.myStopped.priority
+        return self.myStopped.priority
 
     @priority.setter
     def priority(self, value):
-        self.gdb.myStopped.priority = value
+        self.myStopped.priority = value
 
     def __clear_stop(self, name="someone", /):
         log.debug(f"stopped has been cleared by {name}")
-        self.gdb.myStopped.clear()
+        self.myStopped.clear()
 
     def __set_stop(self):
         log.debug(f"setting stopped in {hex(self.instruction_pointer)}")
         # handle case where no action are performed after the end of a callback with high priority 
         self.__clear_stop("__set_stop")
-        self.gdb.myStopped.set()
-
-    #def wait_fork(self):
-    #    self.gdb.forked.wait()
-    #    self.gdb.forked.clear()
+        self.myStopped.set()
 
     def wait_split(self):
         """
         Wait for the process to fork
         set_split_on_fork() must be set before the call to fork
 
         Return:
             pid: pid of the child process
         """
-        pid = self.gdb.split.get()
+        pid = self.libdebug.split.get()
         return pid
 
     def advanced_continue_and_wait_split(self):
         log.warn("advanced_continue_and_wait_split is deprecated. Use cont(until=\"fork\"); finish(); wait_split() instead")
         self.c(until="fork")
         self.finish()
         return self.wait_split()
 
     # For now is handled by simple wait [06/03/23]
     def wait_exit(self):
         ...
 
     def wait_master(self):
-        self.gdb.master_wants_you_to_continue.wait()
-        self.gdb.master_wants_you_to_continue.clear()
+        self.libdebug.master_wants_you_to_continue.wait()
+        self.libdebug.master_wants_you_to_continue.clear()
 
     # Should handle multiple slaves ?
     def wait_slave(self):
-        self.gdb.slave_has_stopped.wait()
-        self.gdb.slave_has_stopped.clear()
+        self.libdebug.slave_has_stopped.wait()
+        self.libdebug.slave_has_stopped.clear()
 
     # temporarily interrupt the execution of our process to get back control of gdb (equivalent of a manual ctrl+C)
     # don't worry about the "kill"
     # May cause problem with the priority [26/04/23]
     def interrupt(self):
         """
         Stop the process as you would with ctrl+C in gdb
 
         Warning: can not YET be put inside a callback
         """
         if not self.debugging:
-            log.warn_once(DEBUG_OFF)
+            #log.warn_once(FEATURE_SKIPPED)
             return
         
         # TODO check that self.running is valid and then use execute_action and priority_wait
         if self.running == self.running:
             self.interrupted = True
-            self.gdb.myStopped.clear()
+            self.myStopped.clear()
             kill(self.inferiors[self._inferior].pid, signal.SIGINT)
             self.wait(legacy=True, timeout=0.1)
 
     manual = interrupt
 
 
     # Next may break again on the same address, but not step
@@ -635,22 +610,19 @@
     def jump(self, location: [int, str], stop = True):
         """
         Jump to specified location
         """
         if not stop:
             log.warn_once("jump(stop = False) is deprecated. Use jump(); c() instead")
         address = self.parse_address(location)
-        log.debug(f"breaking destination at {hex(address)}")
-        self.b(address, temporary=True)
-        self.execute_action(f"jump *{hex(address)}", sender="jump")
-        log.debug("Waiting for jump to conclude")
-        self.priority_wait()
+        self.instruction_pointer = address
 
     # Now can return from anywhere in the function
     # Works only for standard functions (push rbp; mov rbp, rsp; ...; leave; ret;). May crash if used in the libc
+    # Can't I use __saved_ip now ? [28/04/23]
     def ret(self, value: int = None):
         """
         Exit from current function without executing it. 
 
         Warning: Experimental and depends on the stack frame
         """
         log.warn_once(f"ret is still at an experimental stage and may not work properly")
@@ -677,15 +649,15 @@
                 # GEF prints logs as base 16, but pwndbg as base 10
                 return int(ans, 16) if "0x" in ans else int(ans)
             except Exception: #gdb.error: The program being debugged was signalled while in a function called from GDB.
                 log.debug(f"gdb got int3 executing {function}. Retrying...")
                 self.finish()
                 # For some reason I just get 0x0
                 #return self.return_value()
-                return self.gdb_call(function, args) # Should work this time
+                return self.libdebug_call(function, args) # Should work this time
         
         elif function in self.symbols:
             return self.call(self.symbols[function], args)
             
         else:
             raise Exception(f"I don't know how to handle this function! {function} not in symbols")
 
@@ -916,29 +888,29 @@
         address = self.parse_address(location)
 
         log.debug(f"putting breakpoint in {hex(address)}")
         
         # Still needed for hidden breakpoint with return False when you want to also use gdb manually [17/04/23]
         if legacy_callback is not None:
             log.warn_once("if your callbacks crash you may not notice it and you have to scroll a bit to find the error messages hidden in the gdb terminal")
-            # I don't know yet how to handle the conn if I don't go through self.gdb.Breakpoint so I create the class here :(
-            class MyBreakpoint(self.gdb.Breakpoint):
+            # I don't know yet how to handle the conn if I don't go through self.libdebug.Breakpoint so I create the class here :(
+            class MyBreakpoint(self.libdebug.Breakpoint):
                 def __init__(_self, address, callback):
                     super().__init__(address)
                     _self.callback = legacy_callback
                 # WARNING IF A TEMPORARY BREAKPOINT DOESN'T STOP IT WON'T COUNT AS HIT AND STAY ACTIVE. May cause problems with the callback if you pass multiple times [26/02/23]
                 def stop(_self, *args):
                     _break = _self.callback(self) 
                     if _break is None:
                         return True
                     return _break
             res = MyBreakpoint(f"*{hex(address)}", callback)
 
         else:
-            res = self.gdb.Breakpoint(f"*{hex(address)}")
+            res = self.libdebug.Breakpoint(f"*{hex(address)}")
         
         self.breakpoints[address] = Breakpoint(res.server_breakpoint, callback, temporary)
         return res
         
     breakpoint = b
 
     def delete_breakpoint(self, location: [int, str]) -> bool:
@@ -1008,15 +980,15 @@
 
         if inferior == None:
             inferior = self._inferior
         
         if heap:
             old_inferior = self.switch_inferior(inferior)
             
-            res = self.gdb_call("malloc", [n])
+            res = self.libdebug_call("malloc", [n])
 
             self.switch_inferior(old_inferior)
 
             return res
 
         else:
             if self._free_bss is None:
@@ -1029,15 +1001,15 @@
         if inferior == None:
             inferior = self._inferior
         
         if heap:
             
             old_inferior = self.switch_inferior(inferior)
 
-            self.gdb_call("free", [pointer], cast="void")
+            self.libdebug_call("free", [pointer], cast="void")
 
             self.switch_inferior(old_inferior)
 
         else:
             # MMMMMMM, not perfect for different inferiors
             self._free_bss -= len
             #I know it's not perfect, but damn I don't want to implement a heap logic for the bss ahahah
@@ -1264,15 +1236,15 @@
             self.rbp = value
 
     # Prevent null pointers
     @property
     def instruction_pointer(self):
         ans = 0
         while ans == 0:
-            # what about self.gdb.newest_frame().pc() ? [28/04/23]
+            # what about self.libdebug.newest_frame().pc() ? [28/04/23]
             if context.bits == 32:
                 ans = self.eip
             else:
                 ans = self.rip
             # log
             if ans == 0:
                 log.debug("null pointer in ip ! retrying...")
@@ -1283,15 +1255,15 @@
         if context.bits == 32:
             self.eip = value
         else:
             self.rip = value
 
     @property
     def __saved_ip(self):
-        return self.gdb.newest_frame().older().pc()
+        return self.libdebug.newest_frame().older().pc()
 
         ## rip = 0x7ffff7fe45b8 in _dl_start_final (./elf/rtld.c:507); saved rip = 0x7ffff7fe32b8
         #data = self.execute("info frame 0").split("\n")
         #print(data)
         #for line in data:
         #    if " saved " in line and "ip = " in line:
         #        ip = line.split("saved ")[-1].split("= ")[-1]
@@ -1342,15 +1314,15 @@
         child.write(ip, backup)
         log.debug("shellcode patched")
         child.jump(ip)
         # 3 -> exit arch_fork, __GI__Fork, and __libc_fork
         #child.finish(repeat=3)
         #while child.instruction_pointer > self.libs()[self.libc.path]:
         #    child.finish()
-        self.gdb.split.put(pid)
+        self.libdebug.split.put(pid)
         return child
     
     # entrambi dovrebbero essere interrotti, il parent alla fine di fork, il child a metà
     # Ho deciso di lasciare correre il parent. Te la gestisci te se vuoi mettere un breakpoint mettilo dopo
     # I just discovered "gdb.events.new_inferior"... I can take the pid from event.inferior.pid, but can I do more ?
     def set_split_on_fork(self, off=False, c=False, keep_breakpoints=False):
         """
@@ -1363,30 +1335,30 @@
         if off:
             self.execute("set detach-on-fork on")
             #if self.symbols["fork"] in self.breakpoints:
             #    self.breakpoints["fork"].enabled = False
             #    del self.breakpoints["fork"]
 
             # Will break if not set on before
-            self.gdb.events.new_inferior.disconnect(self.inferior_handler)
+            self.libdebug.events.new_inferior.disconnect(self.inferior_handler)
                 
         else:
             self.execute("set detach-on-fork off")
 
             def fork_handler(event):
                 inferior = event.inferior
                 pid = inferior.pid
                 def split(inferior):
                     print(f"splitting child {inferior}")
                     self.interrupt()
                     self.children[pid] = self.split_child(inferior=inferior)
                 # Non puoi eseguire azioni dentro ad un handler degli eventi quindi lancio in un thread a parte
                 context.Thread(target=split, args = (inferior,)).start()
 
-            self.gdb.events.new_inferior.connect(fork_handler)
+            self.libdebug.events.new_inferior.connect(fork_handler)
 
             #def finish(dbg):
             #    log.debug("process forked")
             #    next_ip = unpack(self.read(self.stack_pointer, context.bytes))
             #    #
             #    def split(dbg):
             #        child = dbg.split_child()
@@ -1399,15 +1371,15 @@
             #self.b(self.symbols["fork"], callback=finish)
             
             return self
 
     # Taken from GEF to handle slave interuption
     @property
     def _stop_reason(self) -> str:
-        res = self.gdb.execute("info program", to_string=True).splitlines()
+        res = self.libdebug.execute("info program", to_string=True).splitlines()
         if not res:
             return "NOT RUNNING"
 
         for line in res:
             line = line.strip()
             if line.startswith("It stopped with signal "):
                 return line.replace("It stopped with signal ", "").split(",", 1)[0]
@@ -1568,15 +1540,15 @@
 
     ########################## PTRACE EMULATION ##########################
     def PTRACE_ATTACH(self, _, __, *, slave):
         log.debug(f"pretending to attach to process {slave.pid}")
         slave.master = self
         # I don't think it is needed to stop the child
         #slave.interrupt() ?
-        self.gdb.slave_has_stopped.set()
+        self.libdebug.slave_has_stopped.set()
         self.return_value = 0
 
 
         # set slave. ?
 
     # Only function called by the slave
     def PTRACE_TRACEME(self):
@@ -1750,21 +1722,21 @@
     def __getattr__(self, name):
     #    log.debug(f"looking for attr {name}")
     #    #getattr is only called when an attribute is NOT found in the instance's dictionary
     #    #I may wan't to use this instead of the 300 lines of registers, but have to check how to handle the setter
         if name in ["p", "elf", "gdb"]: #If __getattr__ is called with p it means I haven't finished initializing the class so I shouldn't call self.registers in __setattr__
             return False
         if name in self.special_registers + self.registers + self.minor_registers:
-            res = int(self.gdb.parse_and_eval(f"${name}")) % 2**context.bits
+            res = int(self.libdebug.parse_and_eval(f"${name}")) % 2**context.bits
             return res
         elif self.p and hasattr(self.p, name):
             return getattr(self.p, name)
         # May want to also expose in case you want to access something like inferiors() 
-        elif self.gdb and hasattr(self.gdb, name):
-            return getattr(self.gdb, name)
+        elif self.libdebug and hasattr(self.libdebug, name):
+            return getattr(self.libdebug, name)
         else:
             # Get better errors when can't resolve properties
             self.__getattribute__(name)
 
     def __setattr__(self, name, value):
         if self.elf and name in self.special_registers + self.registers + self.minor_registers:
             self.restore_arch()
```

### Comparing `gdb_plus-6.1.2/gdb_plus/utils.py` & `gdb_plus-6.2.0/gdb_plus/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,31 +67,35 @@
             pointer = self.dbg.stack_pointer + (index + 1) * context.bytes
         elif self.dbg.next_inst.toString() in ["mov rbp, rsp", "mov ebp, esp"]:
             pointer = self.dbg.stack_pointer + (index + 2) * context.bytes
         else:
             pointer = self.dbg.base_pointer + (index + 2) * context.bytes
         return self.dbg.write(pointer, pack(value))
 
+# Warning. Calling wait() before clear() returns immediatly!
 class MyEvent(Event):
     def __init__(self):
         super().__init__()
         self.cleared = Event()
         #self.secret = Event()
         self.priority = 0
+        self.pid = 0
 
     # I still need a standard wait for actions not initiated by dbg.cont and dbg.next
     def priority_wait(self):
         priority = self.priority
         log.debug(f"waiting with priority {priority}")
         while True:
-            #super().wait()
-            self.wait()
+            super().wait()
+            #self.wait()
             if priority == self.priority:
-                log.debug(f"priority {priority} met")
+                log.debug(f"priority {priority} met for {self.pid}")
                 self.priority -= 1
+                if self.priority < 0:
+                    log.warn(f"I think there is something wrong with the wait! We reached priority {self.priority}")
                 break
             # If I call wait again while the event is set it won't block ! [04/04/23]
             self.cleared.wait()
 
     
     def clear(self):
         #self.secret.clear()
```

### Comparing `gdb_plus-6.1.2/gdb_plus.egg-info/PKG-INFO` & `gdb_plus-6.2.0/gdb_plus.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb-plus
-Version: 6.1.2
+Version: 6.2.0
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
@@ -84,32 +84,45 @@
 Debugger can also take as parameter a dictionary for the environment variables. You CAN use it to preload libraries, but if you want to do it for the libc I would advise to **patch the rpath** of the binary instead (if you don't know how take a look at [spwn](https://github.com/MarcoMarce) or [pwninit](https://github.com/io12/pwninit). This will prevent problems when running `system("/bin/sh")` that will fail due to LD_PRELOAD and may hide other problems in your exploit.
 
 **Warning**  
 Old versions of gdbserver (< 11.0.50) have problems launching 32bit binaries. If you see a crash trying to find the canary use `from_start=False` as parameter for the debugger. This will launch the process and then attach to it once the memory has been correctly mapped
 
 ## Control Flow
 
-The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require calling `dbg.wait()`.
+The main actions for gdb are already wrapped in individual methods. For all commands not present you can reconstruct them by calling `dbg.execute(<command>)` as if you where using gdb. Just make sure to use `dbg.execute_action(<command>)` if your command will require you to call `dbg.wait()`.
 
 ```py
+dbg.jump() # set instruction pointer to specific address
 dbg.step() # Single instruction (will enter function calls)
 dbg.next() # Next instruction (will jump over function calls)
 dbg.cont() # Continue execution
+dbg.continue_until() # Continue until you reach a specific location
 dbg.finish() # Finish current function
 dbg.interrupt() # Stop the execution of your process
 dbg.wait() # Wait until you have control of gdb
 ```
 
-**Note**
-* dbg.cont(until=ADDRESS) allows you to block your script until you reach a specific address (or symbol). This means that you can debug manually with gdb while your script is waiting without problems
+In the cases where you have to interact with the process before reaching the address you want or if you would like to put some more breakpoints on the way to play manually with gdb you can use wait=False
+
+```py
+...
+dbg.breakpoint("main+0x12", temporary=True)
+dbg.breakpoint(0x23, temporary=True)
+done = dbg.continue_until("main+0x43", wait=False)
+dbg.p.recvline()
+dbg.p.sendline(b"4")
+done.wait()
+# Here the script will wait until you reach the offset 0x43 from main while gdb will break at offset 0x12 and 0x23 to let you look at the process
+...
+```
 
 **Warning**  
 * `finish` can only work if the stack frame hasn't been corrupted
-* you should specify if you want continue to wait or not with `dbg.cont(wait=True/False)`. We aren't sure about what should be the default behaviour and may set it to `wait=True` in a future version
 * Try avoiding `interrupt` as much as possible. 
+* You may be tempted to do `dbg.instruction_pointer = dbg.parse_address(location)`, but a bug in gdb may cause an unexpected behaviour if you do so. Use `dbg.jump(location)` instead
 
 If the function modifies itself you may find yourself unable to set breakpoints where you want. To analyse these function we can run them step by step
 
 ```py
 def MyCallback(dbg):
     if dbg.next_inst.mnemonic == "int3":
         dbg.step()
@@ -208,37 +221,41 @@
 We can also use capstone to know what is the next instruction that will be executed
 ```py
 print(dbg.next_inst.toString()) # "mov rax, r12"
 print(dbg.next_inst.mnemonic)   # "mov"
 ```
 
 ## Fork
-You can set the debugger to spwn a new instance of gdb every time the process calls fork with `dbg.set_split_on_fork()`.
+You can set the debugger to spwn a new instance of gdb every time the process calls fork with `dbg.set_split_on_fork()`. The child will stop as soon as the process is created by fork, but will wait for the debugger to stop before creating the new object
 
 ```py
 dbg = Debugger("http_server").set_split_on_fork()
-dbg.cont(wait=False)
+done = dbg.continue_until(0x40233)
 dbg.p.sendline("input")
+done.wait()
+# Now that the process stopped at address 0x40233 a new debugger will attach to the child
 pid_child = dbg.wait_split()
 
-# all children are saved in dbg.children and can be accessed by the pid
+# all children have their debugger saved in dbg.children and can be accessed by the pid
 child = dbg.children[pid_child]
 ```
 
 If the program traces its child to make sure you aren't debugging it or to unpack a region of code, you should be able to emulate the calls to ptrace. 
 
 ```py
 child.emulate_ptrace_slave(dbg)
 dbg.emulate_ptrace_master(child)
 ```
 
-This will interrupt the process at every call to waitpid for the master and SIGSTOP or INT3 for the child. You have to handle yourself when to let each one of them continue while you debug them.
+This will interrupt the process at every call to waitpid for the master and SIGSTOP or INT3 for the child. You have to handle yourself when to let each one of them continue while you debug them. To help you a bit we print "Slave can continue" every time the tracer tries to send a continue to the tracee
 
 **Warning**
-pwndbg can not handle multi-process applications and this section is only possible in native gdb or with GEF
+* If the tracee stopped with a SIGSTOP gdb may bug a bit and you may need `force=True` to make it continue correctly
+* pwndbg can not handle multi-process applications and this section is only possible in native gdb or with GEF
+* Handleling multiple processes in the same debugger instead of splitting them may cause problems whith the waits
 
 ## Call functions
 
 If you want to test the effects of a specific function you can directly call it with the parameters you want
 
 ```py
 pointer = dbg.alloc(100)
@@ -262,8 +279,9 @@
 # TODO
 
 * Add option to use libdebug instead of gdb
 * Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
+    * register waitpid return value
 * Maybe nop split_on_fork&co while debugging is False
```

### Comparing `gdb_plus-6.1.2/pyproject.toml` & `gdb_plus-6.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools",
     "wheel",
 ]
 
 [project]
 name = "gdb_plus"
 description = "Python library to automate gdb debugging"
-version = "6.1.2"
+version = "6.2.0"
 authors = [{name = "Edoardo"}]
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "pwntools>=4.5.0",
     "capstone"
 ]
```

### Comparing `gdb_plus-6.1.2/tests/test.py` & `gdb_plus-6.2.0/tests/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,53 +3,51 @@
 import warnings
 
 gdbinit = """
 handle SIGALRM nopass
 source ~/.gdbinit-gef.py
 """
 
-#@unittest.skip
+@unittest.skip
 class Debugger_process(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		self.debuggers = []
 
 	def tearDown(self):
 		for dbg in self.debuggers:
 			try:
 				dbg.close()
 			except:
 				pass
 		pass
 
-	@unittest.skip
+	#@unittest.skip
 	def test_file_standard(self):
 		print("\ntest_file_standard: ", end="")
 		with context.local(arch="i386", bits=32):
 			dbg = Debugger("./start").remote("chall.pwnable.tw", 10000)
 			self.debuggers.append(dbg)
-			dbg.c()
+			dbg.c(wait=False)
 			self.assertEqual(dbg.recv(), b"Let's start the CTF:")
 			dbg.interrupt()
 			self.assertEqual(dbg.instruction_pointer - dbg.elf.address, 0x99)
 			dbg.close()
 	
 	#@unittest.skip
 	def test_noptrace(self):
 		print("\ntest_noptrace: ", end="")
 		with context.local(noptrace = True, arch="i386", bits=32):
 			dbg = Debugger("./start").remote("chall.pwnable.tw", 10000)
 			self.debuggers.append(dbg)
 			self.assertEqual(dbg.recv(), b"Let's start the CTF:")
-			dbg.c(wait=False)
-			dbg.c(wait=True)
 			self.assertFalse(dbg.gdb) 
 			dbg.close()
 
-	@unittest.skip
+	#@unittest.skip
 	def test_remote(self):
 		print("\ntest_remote: ", end="")
 		with context.local(arch="i386", bits=32):
 			args.REMOTE = True
 			dbg = Debugger("./start").remote("chall.pwnable.tw", 10000)
 			self.debuggers.append(dbg)
 			shellcode = b"\x6a\x0b\x58\x68\x2f\x73\x68\x00\x68\x2f\x62\x69\x6e\x89\xe3\x31\xC9\x31\xD2\xcd\x80"
@@ -62,46 +60,46 @@
 			dbg.p.recv()
 			dbg.p.send(shellcode.ljust(0x2c, b'\x90') + p32(stack))
 			dbg.p.sendline(b"cat /home/start/flag")
 			self.assertEqual(dbg.p.recv().strip(), b"FLAG{Pwn4bl3_tW_1s_y0ur_st4rt}")
 			dbg.close()
 			args.REMOTE = ""
 
-	@unittest.skip
+	#@unittest.skip
 	def test_process(self):
 		print("\ntest_process: ", end="")
 		with context.local(arch="i386", bits=32):
 			p = process("./start")
 			dbg = Debugger(p)
 			self.debuggers.append(dbg)
 			self.assertEqual(dbg.p.recv(), b"Let's start the CTF:")
 			dbg.close()
 			p.close()
 
-	@unittest.skip
+	#@unittest.skip
 	def test_pid(self):
 		print("\ntest_pid: ", end="")
 		with context.local(arch="i386", bits=32):
 			p = process("./start")
 			self.assertEqual(type(p.pid), int)
 			dbg = Debugger(p.pid, binary="./start")
 			self.debuggers.append(dbg)
 			dbg.close()
 			p.close()
 
-	@unittest.skip
+	#@unittest.skip
 	def test_debug_from(self):
 		print("\ntest_debug_from: ", end="")
 		with context.local(arch="amd64", bits=64):
 			dbg = Debugger("./traps_withSymbols", aslr=False, debug_from=0x0401590, timeout=0.4)
 			self.debuggers.append(dbg)
 			self.assertEqual(dbg.rip, 0x0401590)
 			dbg.close()
 
-	@unittest.skip
+	#@unittest.skip
 	def test_nonblocking_debug_from(self):
 		print("\ntest_nonblocking_debug_from: ", end="")
 
 		with context.local(arch="i386", bits=32):
 			interaction_finished = Event()
 			dbg = Debugger("./start", aslr=False).debug_from(0x804809d, event=interaction_finished, timeout=0.01)
 			dbg.p.sendline(b"ciao")
@@ -116,32 +114,40 @@
 		with context.local(arch="amd64", bits=64):
 			self.dbg = Debugger("./insaaaaaaane")
 
 	def tearDown(self):
 		self.dbg.close()
 
 	# Fail, ho fatto next a mano e ho perso il controllo
-	@unittest.skip
+	#@unittest.skip
 	def test_continue_until(self):
 		print("\ntest_continue_until: ", end="")
 		self.dbg.b(0x403ad7, temporary=True)
 		print("\nPlay with gdb once we hit address 0x403ad7 and then send continue")
 		self.dbg.c(until=0x403adb)
 		self.assertEqual(self.dbg.instruction_pointer, 0x403adb)
 
+	#@unittest.skip
+	def test_nonblocking_continue_until(self):
+		print("\ntest_nonblocking_continue_until: ", end="")
+		done = self.dbg.continue_until(0x4038c2, wait=False)
+		self.p.sendline(b"ciao")
+		done.wait()
+		self.assertEqual(self.dbg.instruction_pointer, 0x4038c2)
+
 @unittest.skip
 class Debugger_callbacks(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		self.dbg = Debugger("./insaaaaaaane")
 
 	def tearDown(self):
 		self.dbg.close()
 
-	@unittest.skip
+	#@unittest.skip
 	def test_read_memory(self):
 		print("\ntest_read_memory: ", end="")
 		
 		data = []
 
 		def callback(dbg):
 			dbg.push(dbg.rsi)
@@ -150,15 +156,15 @@
 			return True
 			
 		self.dbg.b(0x400786, callback=callback, temporary=True)
 		self.dbg.c(wait=True)
 
 		self.assertFalse(sum(data))
 
-	@unittest.skip
+	#@unittest.skip
 	def test_no_stop(self):
 		print("\ntest_no_stop: ", end="")
 		def callback(dbg):
 			dbg.b(0x403ad9, temporary=True)
 			return False
 
 		self.dbg.b(0x403ad0, callback=callback, temporary=True)
@@ -167,15 +173,15 @@
 		#self.dbg.b(0x403ad9, temporary=True)
 
 		self.dbg.c(wait=True)
 		#self.dbg.interactive()
 		self.assertEqual(self.dbg.rip, 0x403ad9)
 		self.assertFalse(len(self.dbg.breakpoints))
 
-	@unittest.skip
+	#@unittest.skip
 	def test_step(self):
 		print("\ntest_step: ", end="")
 
 		def callback(dbg):
 			dbg.step()
 			return True
 
@@ -223,15 +229,15 @@
 		self.dbg.dealloc(pointer)
 		pointer = self.dbg.alloc(16, heap=False)
 		self.dbg.write(pointer, p64(0xdeadbeeffafa90be))
 		self.dbg.dealloc(pointer, len=16, heap=False)
 		# remember dealloc in the bss will only delete the last chunk... 
 		self.dbg.close()
 		
-@unittest.skip
+#@unittest.skip
 class Debbuger_fork(unittest.TestCase):
 	from base64 import b64encode
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		warnings.simplefilter("ignore", ImportWarning)
 
 	def tearDown(self):
@@ -256,26 +262,21 @@
 		gdbscript = """
 		set detach-on-fork off
 		set follow-fork-mode child
 		"""
 		self.dbg = Debugger("./httpd", aslr=False, script=gdbscript)
 		CALL_TO_B64DECODE = 0x26d5
 		self.dbg.b(CALL_TO_B64DECODE)
-		self.dbg.c()
+		self.dbg.c(wait=False)
 		self.dbg.p.sendline(self.http_request(keepAlive=True))
 		self.dbg.wait()
 		self.assertEqual(self.dbg.rip, 0x5555555566d5)
-		self.dbg.c() # Don't forget to switch only after the child has continued
-		# do what you want and go back to the parent once you are done (you can also do it after the children death)
-		#print("\nthe first child is dead")
-		#self.dbg.wait(timeout=2) # Non riceve mai il segnale che è finito...
-		##sleep(2) # TODO find an alternative than waiting for the child to die
-		self.dbg.wait() # Ora dovrei ricevere l'output
+		self.dbg.c(wait=True)
 		self.dbg.execute("inferior 1") # We can't go back while the child is running
-		self.dbg.c()
+		self.dbg.c(wait=False)
 		self.dbg.p.sendline(self.http_request(keepAlive=True))
 		self.dbg.wait()
 		self.assertEqual(self.dbg.rip, 0x5555555566d5)
 		self.dbg.close()
 	
 	@unittest.skip
 	def test_split(self):
@@ -286,61 +287,58 @@
 			set detach-on-fork off
 			continue
 			"""
 			dbg = Debugger("./httpd", aslr=False, script=gdbscript)
 			sleep(1) # wait for the child to spwn. The parrent will continue while the child is stopped at fork
 			dbg.interrupt()
 			dbg.b(CALL_TO_B64DECODE)
-			child = dbg.split_child(2)
+			child = dbg.split_child(n=2)
 			dbg.p.sendline(self.http_request(keepAlive=True))
 			child.b(CALL_TO_B64DECODE)
 			#child.c()
 			#child.wait()
 			child.c(wait=True)
 			self.assertEqual(child.rip, 0x5555555566d5)
 			child.c()
 			dbg.execute("set follow-fork-mode child")
 			dbg.p.sendline(self.http_request(keepAlive=True))
-			#dbg.c()
+			#dbg.c(wait=False)
 			#dbg.wait()
 			dbg.c(wait=True)
 			self.assertEqual(dbg.rip, 0x5555555566d5)
 			dbg.close()
 			child.close()
 
 	@unittest.skip
 	def test_my_split(self):
 		print("\ntest_my_split: ", end="")
 		with context.local(arch = 'amd64'):
-			SYSCALL_RET = 0x04133f6
-			dbg = Debugger("./traps_withSymbols", aslr=False).set_split_on_fork()
-			dbg.elf.symbols["_syscall"] = SYSCALL_RET
-			dbg.c()
-			#dbg.c(wait=True) # wait for the fork
+			dbg = Debugger("./traps_withSymbols", script="", aslr=False).set_split_on_fork(interrupt=True)
+			dbg.c(wait=False)
 			pid = dbg.wait_split() # and then for the child to split out
 			child = dbg.children[pid]
 			self.assertEqual(dbg.instruction_pointer, 0x4327a7) # Will continue without interuptions. Get's there waiting for the PTRACE from the child
 			self.assertEqual(child.instruction_pointer, 0x432d37)
 			dbg.close()
 			child.close()
 
-	@unittest.skip
+	# This one fails 1/4 times
+	#@unittest.skip
 	def test_ptrace_emulation(self):
 		print("\ntest_ptrace_emulation: ", end="")
 		with context.local(arch = 'amd64'):
-			SYSCALL_RET = 0x04133f6
 			ANTI_DEBUG_TEST_FINISHED = 0x0401590
 			RWX_SECTION = 0x7ffff7ff8000
 			END_UNPACK  = RWX_SECTION + 0x80
 			SYSCALL_TRAP_PTRACE = RWX_SECTION + 0x9e
-			dbg = Debugger("./traps_withSymbols", script=gdbinit, aslr=False, debug_from=ANTI_DEBUG_TEST_FINISHED, timeout=1).set_split_on_fork()
-			dbg.elf.symbols["_syscall"] = SYSCALL_RET
+			dbg = Debugger("./traps_withSymbols", script=gdbinit, aslr=False, debug_from=ANTI_DEBUG_TEST_FINISHED).set_split_on_fork()
 			
-			pid = dbg.advanced_continue_and_wait_split()
-			dbg.step(force=True)
+			dbg.continue_until("fork")
+			dbg.finish()
+			pid = dbg.wait_split()
 			
 			second_child = dbg.children[pid]
 			second_child.emulate_ptrace_slave(dbg)
 			dbg.emulate_ptrace_master(second_child)
 			# Continue after fork
 			dbg.c(wait=True)
 			second_child.c(wait=True)
@@ -445,15 +443,15 @@
 #			else:
 #				output.append(ni.toString())
 #		self.dbg.step_until_ret(callback)
 #		with open("dump_ExceptionalChecking") as fp:
 #			self.assertEqual(output, fp.read().split("\n"))
 	
 	# Commented out to not slow down too much the tests
-	@unittest.skip
+	#@unittest.skip
 	def test_signal_handler(self):
 		print("\ntest_signal_handler: ", end="")
 		from queue import Queue
 		HANDLER_RET = 0x04011ff
 		CHECK_CALL = 0x0401341
 		self.dbg.p.sendline(b"serial_a_caso")
 		self.dbg.cont(until=CHECK_CALL)
@@ -481,15 +479,15 @@
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 
 	def tearDown(self):
 		if hasattr(self, "dbg"):
 			self.dbg.close()
 
-	@unittest.skip
+	#@unittest.skip
 	def test_call(self):
 		print("\ntest_call: ", end="")
 		out = []
 		self.dbg = Debugger("./cube", from_start=False, aslr=False) # You must wait for the libc to be loaded to call malloc
 		for mossa in [0x00003175, 0x00003e74, 0x000038d9, 0x00001885]:
 			# Create blank cube
 			pointer = self.dbg.alloc(54*8)
@@ -501,14 +499,15 @@
 			for i in range(54):
 				out.append(f"{i}: {u64(self.dbg.read(pointer+i*8, 8))}")
 		#print("\n\n".join(out)) 
 		with open("./dump_Cube") as fd:
 			self.assertEqual(out, fd.read().split("\n"))
 		self.dbg.close()
 
+	#@unittest.skip
 	def test_syscall_64bit(self):
 		path = "./data.txt"
 		with context.local(arch="amd64", bits=64):
 			with open(path, "wb") as file:
 				file.write(b"")
 			self.dbg = Debugger("./insaaaaaaane", from_start=False) # You must wait for the libc to be loaded to call malloc
 			fd = self.dbg.syscall(constants.SYS_open, [path, constants.O_WRONLY, 0x0])
@@ -526,27 +525,30 @@
 #		pass
 #
 #	def test_pwndbg(self):
 #		gdbinit = """
 #		source ~/.gdbinit-pwndbg
 #		"""
 #		self.dbg = Debugger("./httpd", script=gdbinit, from_start=False)
-#		self.dbg.c()
+#		self.dbg.c(wait=False)
 #		sleep(1)
 #		self.dbg.interrupt() # Non è questo ad ucciderlo anche se printa SIGINT
 #		pointer = self.dbg.alloc(16, heap=False)
 #		self.dbg.write(pointer, p64(0xdeadbeeffafa90be))
 #		pointer = self.dbg.alloc(16)
 #		self.dbg.write(pointer, p64(0xdeadbeeffafa90be))
 #		self.dbg.close()
 #		gdbinit = """
 #		source ~/.gdbinit-gef.py
 #		"""
 #		self.dbg = Debugger("./httpd", script=gdbinit, from_start=False)
 #		pointer = self.dbg.alloc(16)
 #		self.dbg.write(pointer, p64(0xdeadbeeffafa90be))
 #		self.dbg.close()
-#
+
+@unittest.skip
+class Debugger_no_wait(unittest.TestCase):
+	pass	
 
 if __name__ == "__main__":
 	with context.quiet:
 		unittest.main()
```

