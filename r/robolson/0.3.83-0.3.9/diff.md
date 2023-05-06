# Comparing `tmp/robolson-0.3.83.tar.gz` & `tmp/robolson-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robolson-0.3.83.tar", max compression
+gzip compressed data, was "robolson-0.3.9.tar", max compression
```

## Comparing `robolson-0.3.83.tar` & `robolson-0.3.9.tar`

### file list

```diff
@@ -1,50 +1,10 @@
--rw-r--r--   0        0        0      123 2022-07-23 00:18:58.660549 robolson-0.3.83/.autoenv
--rw-r--r--   0        0        0       56 2023-01-12 07:11:08.976913 robolson-0.3.83/.justfile
--rw-r--r--   0        0        0       24 2022-03-21 20:13:02.294495 robolson-0.3.83/__init__.py
--rw-r--r--   0        0        0       66 2022-03-21 23:26:56.141915 robolson-0.3.83/__main__.py
--rw-r--r--   0        0        0      829 2023-02-17 21:22:04.657577 robolson-0.3.83/anagram.py
--rw-r--r--   0        0        0    24615 2023-04-01 13:05:00.492511 robolson-0.3.83/clean.py
--rw-r--r--   0        0        0      103 2022-03-21 21:21:02.284735 robolson-0.3.83/config/.autoenv
--rw-r--r--   0        0        0     1006 2023-01-18 09:41:39.545792 robolson-0.3.83/config/clean.toml
--rw-r--r--   0        0        0   816591 2023-02-17 19:54:50.219010 robolson-0.3.83/data/word_list.txt
--rw-r--r--   0        0        0     5166 2023-01-21 00:44:10.045520 robolson-0.3.83/email.py
--rw-r--r--   0        0        0    10015 2023-03-23 10:24:04.360312 robolson-0.3.83/ffmpeg.py
--rw-r--r--   0        0        0     1043 2022-07-04 02:09:47.244686 robolson-0.3.83/help.py
--rw-r--r--   0        0        0    20235 2022-05-02 00:50:16.538685 robolson-0.3.83/hierarchy.py
--rw-r--r--   0        0        0        0 2022-05-21 03:18:54.857385 robolson-0.3.83/loggers/__init__.py
--rw-r--r--   0        0        0     1021 2022-07-14 03:10:34.224571 robolson-0.3.83/loggers/tick_logger.py
--rw-r--r--   0        0        0      228 2023-02-09 11:55:19.637586 robolson-0.3.83/New Text Document.reg
--rw-r--r--   0        0        0     1509 2023-05-06 17:13:02.774072 robolson-0.3.83/night.py
--rw-r--r--   0        0        0    22080 2023-01-24 18:58:55.889318 robolson-0.3.83/old_clean.py
--rw-r--r--   0        0        0        0 2022-05-21 03:18:36.761960 robolson-0.3.83/parser/__init__.py
--rw-r--r--   0        0        0     1119 2023-01-14 21:30:02.931167 robolson-0.3.83/parser/clean_parser.py
--rw-r--r--   0        0        0     1220 2022-07-08 10:11:15.790934 robolson-0.3.83/parser/email_parser.py
--rw-r--r--   0        0        0     1770 2022-04-08 02:11:14.941735 robolson-0.3.83/parser/ffmpeg_parser.py
--rw-r--r--   0        0        0     1509 2023-02-06 13:43:39.345746 robolson-0.3.83/parser/reddit_parser.py
--rw-r--r--   0        0        0      909 2022-07-04 01:50:11.624597 robolson-0.3.83/parser/tick_parser.py
--rw-r--r--   0        0        0   133656 2023-05-06 21:04:54.397024 robolson-0.3.83/poetry.lock
--rw-r--r--   0        0        0     1056 2023-05-06 21:06:24.124198 robolson-0.3.83/pyproject.toml
--rw-r--r--   0        0        0     8401 2023-02-06 13:44:14.394052 robolson-0.3.83/reddit_archive.py
--rw-r--r--   0        0        0     4153 2023-02-27 21:47:08.721554 robolson-0.3.83/robai.py
--rw-r--r--   0        0        0     5978 2023-02-08 17:22:46.858389 robolson-0.3.83/tick.py
--rw-r--r--   0        0        0        0 2022-04-07 19:21:12.560000 robolson-0.3.83/ticktick/__init__.py
--rw-r--r--   0        0        0    24751 2022-05-09 07:55:23.045790 robolson-0.3.83/ticktick/api.py
--rw-r--r--   0        0        0     1473 2022-05-02 00:50:17.516634 robolson-0.3.83/ticktick/cache.py
--rw-r--r--   0        0        0        0 2022-04-07 19:21:12.670000 robolson-0.3.83/ticktick/helpers/__init__.py
--rw-r--r--   0        0        0       68 2022-04-07 19:21:12.699905 robolson-0.3.83/ticktick/helpers/constants.py
--rw-r--r--   0        0        0     1184 2022-05-02 00:50:17.590600 robolson-0.3.83/ticktick/helpers/hex_color.py
--rw-r--r--   0        0        0     2787 2022-05-09 07:49:04.451389 robolson-0.3.83/ticktick/helpers/time_methods.py
--rw-r--r--   0        0        0     8805 2022-04-08 04:12:37.380147 robolson-0.3.83/ticktick/helpers/timezones.txt
--rw-r--r--   0        0        0        0 2022-04-07 19:21:12.804000 robolson-0.3.83/ticktick/managers/__init__.py
--rw-r--r--   0        0        0      444 2022-05-02 00:50:18.497442 robolson-0.3.83/ticktick/managers/check_logged_in.py
--rw-r--r--   0        0        0      408 2022-05-02 00:50:18.510446 robolson-0.3.83/ticktick/managers/focus.py
--rw-r--r--   0        0        0     4956 2022-05-02 00:50:18.524792 robolson-0.3.83/ticktick/managers/habits.py
--rw-r--r--   0        0        0      334 2022-05-02 00:50:18.547793 robolson-0.3.83/ticktick/managers/pomo.py
--rw-r--r--   0        0        0    43862 2022-06-11 04:09:26.134840 robolson-0.3.83/ticktick/managers/projects.py
--rw-r--r--   0        0        0      429 2022-05-02 00:50:18.617905 robolson-0.3.83/ticktick/managers/settings.py
--rw-r--r--   0        0        0    46804 2022-06-11 04:10:45.717520 robolson-0.3.83/ticktick/managers/tags.py
--rw-r--r--   0        0        0    54311 2022-06-11 04:08:26.998571 robolson-0.3.83/ticktick/managers/tasks.py
--rw-r--r--   0        0        0    13289 2022-05-09 07:54:06.826880 robolson-0.3.83/ticktick/oauth2.py
--rw-r--r--   0        0        0       24 2022-04-19 17:39:25.252880 robolson-0.3.83/tox.ini
--rw-r--r--   0        0        0     1342 2023-05-06 21:06:34.716930 robolson-0.3.83/setup.py
--rw-r--r--   0        0        0      888 2023-05-06 21:06:34.717934 robolson-0.3.83/PKG-INFO
+-rw-r--r--   0        0        0      800 2022-03-01 07:48:26.175730 robolson-0.3.9/config/clean.toml
+-rw-r--r--   0        0        0      517 2022-03-03 22:36:47.590940 robolson-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1370 2022-03-03 22:20:19.066408 robolson-0.3.9/rob/__init__.py
+-rw-r--r--   0        0        0     9461 2022-03-03 22:20:57.643345 robolson-0.3.9/rob/clean.py
+-rw-r--r--   0        0        0     3371 2022-02-18 20:11:06.384003 robolson-0.3.9/rob/ffmpeg_concat.py
+-rw-r--r--   0        0        0    19816 2021-10-05 21:28:44.953483 robolson-0.3.9/rob/hierarchy.py
+-rw-r--r--   0        0        0     7590 2022-02-27 00:03:52.749759 robolson-0.3.9/rob/reddit_archive.py
+-rw-r--r--   0        0        0     3922 2022-01-01 00:08:23.770615 robolson-0.3.9/rob/robai.py
+-rw-r--r--   0        0        0      712 2022-03-03 22:37:01.742591 robolson-0.3.9/setup.py
+-rw-r--r--   0        0        0      471 2022-03-03 22:37:01.742591 robolson-0.3.9/PKG-INFO
```

### Comparing `robolson-0.3.83/hierarchy.py` & `robolson-0.3.9/rob/hierarchy.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 #   list_depth(...) <-- returns the depth of nesting as an integer
 #
 #
 #Rob O.
 #Last Updated: 8/25/2014
 
 import weakref
-import deal
 
 
 class HierarchyError(Exception):
     """Indicates an exception emanating from the Hierarchy class."""
 
 class Hierarchy(object):
     """Initializer is an element name, or a hierarchically nested list.
@@ -43,15 +42,15 @@
     used by Sub-Classes (the base class ignores the remaining elements).
 * Remaining list elements are recursively parsed following the above criteria.
 
 NOTE: The parser is flexible enough to handle any nested list, although the
       result may need tweaking if the original list was not properly structured.
       The hier_out(...) function will give you a visual indication of how the
       Hierarchy class will interpret any given nested list.
-
+      
 EXAMPLES:
 
 >>> print Hierarchy('A hierarchical singleton')
 +------------------------+
 |A hierarchical singleton|
 +------------------------+
 >>> h = Hierarchy('root')
@@ -70,15 +69,14 @@
 ||   child 1   ||child 2||
 ||+-----------+|+-------+|
 |||grand-child||         |
 ||+-----------+|         |
 |+-------------+         |
 +------------------------+
 """
-    @deal.pure
     def __init__(self, initializer='root', parent=None, *args): #Remove *args?
 
 
         self.name = None
         self._sisters = []
         self._daughters = []
         self._parent = None
@@ -88,41 +86,39 @@
         if isinstance(initializer, (list, tuple, dict)):
 
             #this recursive function does all the work
             temp = self._parse_list(initializer)
 
             if temp._parent == self:
                 temp._parent = None
-
+                
             for k in temp.__dict__.keys():
                 setattr(self, k, getattr(temp, k))
 
         #construct a hierarchical singleton
         #which can be subsequently attached to an existing hierarchy
         else:
             self.name = initializer
 
             if parent:
                 self.parent = parent
-
-    @deal.has()
-    @deal.raises(HierarchyError, ValueError)
+        
     def __getitem__(self, name):
         """Experimenting with special syntax...
 A string index with the '=' symbol will be broken into two parts.
 Example:
 'name=super man' will return the first element with self.name == 'super man'.
 'ID=99701' will return the first element with self.ID == 99701.
 
 NOTE: Nested attributes are not allowed.  Only primitives and built-ins should
       be used in this way."""
 
         if isinstance(name, int):
             return self._daughters[name]
-
+        
         if name.count("=") > 1:
             raise HierarchyError("'=' can appear only once per index specifier.")
 
         if '=' in name:
             attribute, value = name.split('=')
             attribute  = attribute.strip()
             value = value.strip()
@@ -134,219 +130,199 @@
             #the commented out return statement will return the first matching
             #element from ANYWHERE IN THE TREE...(the above return statment too)
             #As is, self.__get__item(...) only searches daughters of self.
             #return self._traverse(self.origin, value, attribute)
             return self._traverse(self, name)
         raise ValueError("{} not found in hierarchy.".format(name))
 
-    @deal.has()
-    @deal.raises(HierarchyError, ValueError)
     def __setitem__(self, name, value):
 
         if "ID={}".format(value.ID) in self:
             raise HierarchyError("Cannot assign objects already in the hierarchy.")
-
+        
         if isinstance(value, Hierarchy):
-
+            
             if self[name]:
-
+                
                 if value._parent:
                     vp = value._parent
                     vp._daughters.remove(value)
                     for daughter in vp._daughters:
                         daughter._sisters.remove(value)
-
+                        
                 target = self[name]
                 tp = target._parent
                 tp._daughters.remove(target)
                 for daughter in tp._daughters:
                     daughter._sisters.remove(target)
-
+                
                 value.parent = tp
-
-
+                
+                
             else:
                 raise ValueError("'{}' was not found.".format(name))
         else:
             raise HierarchyError("{} must be a hierarchical type.".format(value))
 
-    @deal.pure
     def __len__(self):
         if self._daughters:
             return sum([len(daughter) for daughter in self._daughters])+1
         else:
             return 1
 
-    @deal.pure
     def __repr__(self):
         class_Name = str(self.__class__)
         dot_Index = class_Name.rindex('.')
         class_Name = class_Name[dot_Index+1:-2]
         #class_Name = re.search(r"\.([A-Za-z_]+)'>$", class_Name)[0]
-
+        
         return "{}('{}')".format(class_Name,self.name)
 
-    @deal.pure
     def __str__(self):
         return self.render()
 
-    @deal.pure
     def __contains__(self, value):
         try:
             self[value]
             return True
         except ValueError:
             return False
 
-    @property  # type: ignore[misc]
-    @deal.pure
+    @property
     def ID(self):
         """Read only."""
         return hash(self)
 
-    @property  # type: ignore[misc]
-    @deal.pure
+    @property
     def sisters(self):
         """Read only."""
         return self._sisters
-
-    @property  # type: ignore[misc]
-    @deal.pure
+    
+    @property
     def daughters(self):
         """Read only."""
         return self._daughters
-    @property  # type: ignore[misc]
-    @deal.pure
+    @property
     def origin(self):
         """Read only."""
         return self._origin
-
-    @property  # type: ignore[misc]
-    @deal.pure
+    
+    @property
     def parent(self):
         return self._parent
 
-    @deal.pure
     @parent.setter
     def parent(self, target):
         """Removes self from current parent and makes target self's new parent.
 Also cleans up secondary references, lateral references, etc."""
-
+        
         try:
             self._traverse(self, target.ID, 'ID')
             raise HierarchyError("Cannot make a child element a parent.")
         except ValueError:
             pass
 
         if self._parent:
             old_Parent = self._parent
             old_Parent._daughters.remove(self)
             for daughter in old_Parent._daughters:
                 daughter._sisters.remove(self)
 
         self._sisters = target._daughters[:]
-
+        
         if target._daughters:
             for daughter in target._daughters:
                 daughter._sisters.append(self)
-
+        
 
         target._daughters.append(self)
 
         self._parent = target
         self._propagate(self, "_origin", target.origin)
 
-    @deal.pure
     def _copy(self, depth = -1):
         """The recursive part of the self.copy() method."""
         temp = self.__class__(self.name)
 
         temp.__dict__ = self.__dict__.copy()
-
+        
         if depth == 0:
             temp._daughters = []
-
+            
         if depth > 0 or depth == -1:
-
+            
             if depth > 0:
                 depth -= 1
 
             #daughters are cached and the list is emptied so that copies
             #can be re-inserted individually using copy.parent assignment
             temp_daughters = [daughter.copy(depth) for daughter in temp._daughters]
             temp._daughters = []
             for daughter in temp_daughters:
                 daughter._sisters = temp_daughters[:].remove(daughter)
                 daughter.parent = temp
 
-        return temp
+        return temp 
 
-    @deal.pure
     def _propagate(self, root, attribute, value):
         """Assign value to root.attribute and all of root's daughter.attribute."""
 
         setattr(root, attribute, value)
 
         for daughter in root._daughters:
             self._propagate(daughter, attribute, value)
 
-    @deal.has()
-    @deal.raises(ValueError)
     def _traverse(self, root, target, attribute = "name"):
         """Search the hierarchy from root->leaves for an element with target attribute."""
         prop = getattr(root, attribute, None)
         if prop:
             if prop == prop.__class__(target):
                 return root
             else:
                 for daughter in root._daughters:
                     temp = self._traverse(daughter, target, attribute)
                     if temp:
                         return temp
-
+                    
         if root==self:
             raise ValueError("{} not found in the hierarchy.".format(target))
-
-    @deal.pure
+    
     def _parse_list(self, nested_List):
         """Recursively turn a nested list/dictionary into a tree of Hierarchy objects."""
 
         # Handle the empty edge case
         if not nested_List:
             nested_list = ["root"]
         # Convert dictionary into a (str, list) tuple corresponding to (key, value)
         elif isinstance(nested_List, dict):
             nested_list = ["dict"]+[[str(k)+":->", (v if isinstance(v, (list, dict)) else [v])] for k, v in nested_List.items()]
         else:
             nested_list = nested_List[:]
 
-
+        
         sub_Lists = [elem for elem in nested_list if isinstance(elem, (list, tuple, dict))]
         extra_Args = [elem for elem in nested_list if not isinstance(elem, (list, tuple, dict))]
 
         temp = self.__class__(", ".join([str(elem) for elem in extra_Args]), self, *extra_Args)
-
+        
         daughters = [temp._parse_list(daughter) for daughter in sub_Lists]
-
+        
         temp._daughters = daughters
 
         for daughter in daughters:
             daughter._parent = temp
-
+        
         return temp
 
-    @deal.pure
     def _list_depth(self, root):
         if root._daughters:
             return max([self._list_depth(elem) for elem in root.daughters])+1
         else:
             return 1
 
-    @deal.has('import')
-    @deal.safe
     def _frame_down(self, root, attributes=[]):
         from textframe import frame, parallelize
         contents = ""
         for attr in attributes:
             line = "{}.{}: {}".format(root.name,
                                       attr,
                                       getattr(root, attr, "Error"))
@@ -361,86 +337,81 @@
         if root._daughters:
             daughter_boxes = [self._frame_down(elem, attributes=attributes) for elem in root._daughters]
             return frame(contents+("\n" if contents else "")+\
                          parallelize(daughter_boxes), hJust="c")
         else:
             return frame(contents, hJust='c')
 
-    @deal.has('import')
-    @deal.safe
     def _stringify(self, attributes=[], depth = 0):
         """Recursively lay self out along one line for each level of nesting.
 TODO: Make indent and grouper variables to customize output style."""
-
+        
         from text import parallelize
-
+        
         if 'name' in attributes:
             attributes.remove('name')
 
         head = "\n"*depth + self.name
         attrs = ", ".join([repr(getattr(self, attr, "Error")) for attr in attributes])
         if attrs:
             head += "({})".format(attrs)
-
+            
         foot = "\n"*depth + ">"
-
+        
         if self._daughters:
             head += "<"
-
+            
             canvas = [head]
             for daughter in self._daughters:
                 canvas.append(daughter._stringify(attributes = attributes,
                                                   depth = depth+1))
-
+                
                 if self._daughters.index(daughter) != len(self._daughters)-1:
                     canvas.append("\n"*(depth+1) + ", ")
             canvas.append(foot)
 
             return parallelize(canvas)
-
+        
         else:
             return head
-
-    @deal.pure
+            
     def _verticalize(self, attributes = [], depth = 0):
         """Recursively lay self out on lines.
 TODO: Make indent and grouper variables to customize output style."""
 
         if 'name' in attributes:
             attributes.remove('name')
 
         attrs = ", ".join([repr(getattr(self, attr, "Error")) for attr in attributes])
         if attrs:
             attrs = "({})".format(attrs)
-
+            
         if self._daughters:
             base_String = "  "*depth + str(self.name)+ attrs +"\n"+ "  "*depth + "<\n"
             for daughter in self._daughters:
                 base_String += daughter._verticalize(attributes= attributes,
                                                      depth = depth+1) + "\n"
 
             base_String += "  "*depth + ">"
 
             return base_String
 
         else:
             return "  "*depth+str(self.name)+attrs
 
-    @deal.has('import')
-    @deal.safe
     def render(self, attributes=[], mode = "frames"):
         """Display the hierarchy visually.  Attributes is a list of attributes.
 
 3 supported rendering modes:
 MODE       - VALID STRING CODES
 ----------------------
 frames     - 'frames', 'f'
 vertical   - 'vertical', 'v'
 horizontal - 'horizontal', 'h'"""
-
+        
         try:
             from text import frame, parallelize
         except ImportError:
             mode = "v"
 
         #if my text module is available, use it to frame the hierarchy
         if mode in ("frames", "f"):
@@ -451,99 +422,90 @@
             return self._stringify(attributes = attributes, depth = 0)
 
         #this is a simple fall-back representation
         elif mode in ("vertical", "v"):
             return self._verticalize(attributes = attributes, depth=0)
 
         return self._frame_down(self, attributes = attributes)
-
-    @deal.pure
+    
     def insert(self, *args):
         """If first argument is hierarchical, it is simply added as a child of self.
 Otherwise, arguments are taken and passed to self.__init__(...) to generate
     a hierarchical object, which is added as a child of self."""
 
         if isinstance(args[0], Hierarchy):
             args[0].parent = self
         else:
             temp = self.__class__(*args)
             temp.parent = self
 
-    @deal.pure
     def copy(self, depth=-1):
         """Return a copy of self including all children up to depth.
 If depth == -1, copying is exhaustive.
 If depth == 0, no children are copied (only self).
 NOTE: Element ID's are based on location in memory.  (The copy will have a
 different self.ID value than the original.)"""
-
+        
         temp = self._copy(depth)
         temp._parent = None
         temp._propagate(temp, "_origin", temp)
         return temp
-
-    @deal.has()
-    @deal.raises(AttributeError)
+        
     def set_precedence(self, index):
         """Move this element to the index'th position among its siblings."""
         if self._parent:
             self._parent._daughters.remove(self)
             self._parent._daughters.insert(index,self)
 
         else:
             raise AttributeError("Root element has no index.")
 
-    @deal.has()
-    @deal.raises(HierarchyError)
     def permute_daughters(self, permutation):
         """Change the order of self's daughters to match that of permutation.
 Examples:
 The [0, 1, 2] permutation is the identity permutation.
 The [2, 1, 0] permutation is equivalent to using reversed.
 The [0,2,4,...,1,3,5,...] permutation organizes daughters by parity."""
-
+        
         if len(permutation) != len(self._daughters):
             raise HierarchyError("Permutation must have exactly 1 distinct index for each daughter.")
 
         if sorted(permutation)!=range(len(permutation)):
             raise HierarchyError("Permutation indeces must range from 0 to n in increments of 1.")
 
         #This code allows greater flexibility in the permutation argument
         #Any iterable with a distinct ordering will work
         #But that seemed like a good hiding place for bugs, so its out for now.
         #permutation = [permutation.index(elem) for elem in sorted(permutation)]
 
         for elem, index in zip(self._daughters[:], permutation):
             elem.set_precedence(index)
 
-    @deal.pure
     def transfer(self):
         pass
-
-
-@deal.pure
+        
+        
 def list_depth(nestedList):
     """A non-list object has 0 depth.  A simple list has a depth of 1.  Etc."""
 
     if isinstance(nestedList, (list, tuple)):
         return max([list_depth(elem) for elem in nestedList])+1
     else:
         return 0
 
-@deal.pure
 def join_contiguous(theList, depth = -1):
     """Joins 2 or more consecutive containers in theList, up to specified depth.
 If depth == -1, ALL levels of nesting are affected.
 If depth == 0, the function does nothing.
 If depth == 1, once-nested lists are affected.
 If depth == 2, twice-nested lists are also affected.
 ...etc..."""
 
     if depth > 0 or depth == -1:
-
+        
         i = 0
         #This loop cycles through the outer-most list, looking for 2 consecutive
         #list or tuple elements.  Those 2 elements are replaced by the union.
         #The union is, itself, a list so that if there is a 3rd consecutive
         #list or tuple, it will be caught during the loop's, next iteration, etc
         while i + 1 < len(theList):
             if isinstance(theList[i], (tuple, list)):
@@ -564,15 +526,14 @@
         for subList in theList[:]:
             if isinstance(subList, (list, tuple)):
                 n = theList.index(subList)
                 theList.remove(subList)
                 theList.insert(n, join_contiguous(subList, depth-1))
     return theList
 
-@deal.pure
 def hier_out(hierarchical_Object, mode = 'f'):
     """Returns a string representation of the passed object.
 
 EXAMPLES:
 >>> print hier_out(['parent',['child']])
 +-------+
 |parent |
@@ -586,24 +547,24 @@
   child
   <
     grand-child
   >
 >
 >>> print hier_out(['root',['1',['a'],['b']],['2',['i'],['ii']]], mode = 'h')
 root<                 >
-     1<    >, 2<     >
-       a, b     i, ii
+     1<    >, 2<     > 
+       a, b     i, ii  
 """
     try:
         return hierarchical_Object.render(mode= mode)
     except AttributeError:
         return Hierarchy(hierarchical_Object).render(mode= mode)
 
 if __name__ == "__main__":
     import unittest, doctest
     from testhierarchy import *
 
     #A simple instance for debugging purposes
     h = Hierarchy(['r',['t'],['b']])
-
-    doctest.testmod()
+    
+    doctest.testmod()    
     unittest.main()
```

### Comparing `robolson-0.3.83/robai.py` & `robolson-0.3.9/rob/robai.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import argparse
-import datetime
 import os
-import re
-import shelve
+import openai
 import sys
+import shelve
+import datetime
+import argparse
+import re
+
 from pathlib import Path
 
-import openai
 import rich
 
 NOW = datetime.datetime.today()
 openai.api_key = os.getenv("OPENAI_API_KEY")
 
 USER = "Stranger"
 FILE = Path(sys.argv[0])
@@ -49,21 +50,14 @@
 my_parser.add_argument(
     "-c",
     "--clear",
     action="store_true",
     help="Clear user's database of convos.",
 )
 
-my_parser.add_argument(
-    "-i",
-    "--inspect",
-    action="store_true",
-    help="Clear user's database of convos.",
-)
-
 # Execute the parse_args() method
 args = my_parser.parse_args()
 
 if args.clear and args.user:
     if input("Are you sure you want to clear the conversation database? [y/n]\n") in [
         "y",
         "yes",
@@ -78,78 +72,78 @@
     USER = args.user
 
 PRE_PROMPT = f"""
 Robert is a charming man who loves his friends and family.  {USER} is texting him.  His texts are short.
 """
 
 if "?" in args.Prompt:
-    TEMPERATURE = 0.2
+    TEMPERATURE = 0.1
 else:
-    TEMPERATURE = 0.2
+    TEMPERATURE = 0.9
 
 NEW_PROMPT = f"""
 {USER}: {args.Prompt}"""
 ROB = """
 Robert:"""
 
 CLEAN_PROMPT = f"Robert is a charming man who loves his friends and family.  {USER} is texting him.  His texts are short.  Reduce his following response to ONE sentence.  Make it short and clear.\n"
 
-if args.inspect:
-    breakpoint()
-
 with shelve.open(f"{FILE.parent}/db/{args.user}_convo.db") as db:
     for date in sorted(db.keys()):
         if (NOW - datetime.datetime.fromisoformat(date)).total_seconds() < 3600 * 4:
             PRE_PROMPT += db[date]
-        # else:
-        #     break
+        else:
+            break
 
         if len(PRE_PROMPT) > 1000:
             break
     try:
-        # r1 = openai.Completion.create(
-        r1 = openai.Edit.create(
-            # model="curie:ft-user-lxdklb8ngeneatsn8iouxynt-2021-12-09-06-55-36",
-            model="text-davinci-edit-001",
-            input=PRE_PROMPT + NEW_PROMPT + ROB,
-            # prompt=PRE_PROMPT + NEW_PROMPT + ROB,
-            instruction="Complete Robert's response.",
-            # max_tokens=60,
+        r1 = openai.Completion.create(
+            model="curie:ft-user-lxdklb8ngeneatsn8iouxynt-2021-12-09-06-55-36",
+            prompt=PRE_PROMPT + NEW_PROMPT + ROB,
+            max_tokens=60,
             n=1,
             temperature=TEMPERATURE,
         )
 
     # If the model isn't spun up then this error might happen
     except openai.error.RateLimitError:
         r1 = openai.Completion.create(
-            # model="curie:ft-user-lxdklb8ngeneatsn8iouxynt-2021-12-09-06-55-36",
-            model="text-davinci-001",
-            # prompt=PRE_PROMPT + NEW_PROMPT + ROB,
-            input=PRE_PROMPT + NEW_PROMPT + ROB,
-            instruction="Complete Robert's response.",
+            model="curie:ft-user-lxdklb8ngeneatsn8iouxynt-2021-12-09-06-55-36",
+            prompt=PRE_PROMPT + NEW_PROMPT + ROB,
             max_tokens=60,
             n=1,
             temperature=TEMPERATURE,
         )
 
-    # response = r1.choices[0].text
-    # patt = re.compile(r"[^\.!?:,]+")
-    # reg = patt.findall(response)
-
-    # if reg:
-    #     response = ""
-    #     for sentence in reg:
-    #         response += sentence
-    #         if len(response) > 55:
-    #             if response[-1] == ",":
-    #                 response = response[:-1]
-    #             break
-
-    # repeat_patt = re.compile(r"(.{7,}?)\1+")
-    # reg = repeat_patt.match(response)
-    # if reg:
-    #     response = reg.groups(0)[0]
-
-    response = r1.choices[0].text.split("\n")[-2]
-
-    rich.print(f"{PRE_PROMPT}{NEW_PROMPT}\n[black on red]{response}[/black on red]")
-    db[str(NOW)] = f"{NEW_PROMPT}\n{response}\n\n###\n"
+    response = r1.choices[0].text
+    patt = re.compile(r"[^\.!?:,]+")
+    reg = patt.findall(response)
+
+    if reg:
+        response = ""
+        for sentence in reg:
+            response += sentence
+            if len(response) > 55:
+                if response[-1] == ",":
+                    response = response[:-1]
+                break
+
+    repeat_patt = re.compile(r"(.{7,}?)\1+")
+    reg = repeat_patt.match(response)
+    if reg:
+        response = reg.groups(0)[0]
+    # r2 = openai.Completion.create(
+    #     engine="davinci-instruct-beta-v3",
+    #     prompt=f'{CLEAN_PROMPT}\n\n{response}',
+    #     max_tokens=35,
+    #     n=1,
+    #     temperature=0.2
+    # )
+    # response2=r2.choices[0].text
+
+    # rich.print(f"FIRST PASS\n[black on yellow]{response}\n[/black on  yellow]")
+
+    rich.print(
+        f"{PRE_PROMPT}{NEW_PROMPT}\nRobert:[black on red]{response}[/black on red]"
+    )
+    db[str(NOW)] = f"{NEW_PROMPT}\nRobert:{response}\n\n###\n"
```

