# Comparing `tmp/st_ant_carousel-0.0.1-py3-none-any.whl.zip` & `tmp/st_ant_carousel-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 653680 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat     5866 b- defN 23-May-06 10:56 st_ant_carousel/__init__.py
+Zip file size: 653858 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat     6207 b- defN 23-May-06 16:48 st_ant_carousel/__init__.py
 -rw-rw-rw-  2.0 fat      859 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/asset-manifest.json
 -rw-rw-rw-  2.0 fat   206960 b- defN 23-May-01 13:22 st_ant_carousel/frontend/build/bootstrap.min.css
 -rw-rw-rw-  2.0 fat     2075 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/index.html
 -rw-rw-rw-  2.0 fat      564 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/precache-manifest.2607c490f9520a6a70a96334da952fb8.js
 -rw-rw-rw-  2.0 fat     1183 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/service-worker.js
 -rw-rw-rw-  2.0 fat   693699 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/static/js/2.6435dd4a.chunk.js
 -rw-rw-rw-  2.0 fat     1925 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/static/js/2.6435dd4a.chunk.js.LICENSE.txt
 -rw-rw-rw-  2.0 fat  1999238 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/static/js/2.6435dd4a.chunk.js.map
 -rw-rw-rw-  2.0 fat     1754 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/static/js/main.a2df1366.chunk.js
 -rw-rw-rw-  2.0 fat     5650 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/static/js/main.a2df1366.chunk.js.map
 -rw-rw-rw-  2.0 fat     1572 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/static/js/runtime-main.502c8693.js
 -rw-rw-rw-  2.0 fat     8291 b- defN 23-May-06 10:46 st_ant_carousel/frontend/build/static/js/runtime-main.502c8693.js.map
--rw-rw-rw-  2.0 fat     1084 b- defN 23-May-06 10:56 st_ant_carousel-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4895 b- defN 23-May-06 10:56 st_ant_carousel-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 10:56 st_ant_carousel-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-May-06 10:56 st_ant_carousel-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1930 b- defN 23-May-06 10:56 st_ant_carousel-0.0.1.dist-info/RECORD
-18 files, 2937653 bytes uncompressed, 650376 bytes compressed:  77.9%
+-rw-rw-rw-  2.0 fat     1084 b- defN 23-May-06 16:48 st_ant_carousel-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5055 b- defN 23-May-06 16:48 st_ant_carousel-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 16:48 st_ant_carousel-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-May-06 16:48 st_ant_carousel-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1930 b- defN 23-May-06 16:48 st_ant_carousel-0.0.2.dist-info/RECORD
+18 files, 2938154 bytes uncompressed, 650554 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: st_ant_carousel/frontend/build/static/js/runtime-main.502c8693.js
 Comment: 
 
 Filename: st_ant_carousel/frontend/build/static/js/runtime-main.502c8693.js.map
 Comment: 
 
-Filename: st_ant_carousel-0.0.1.dist-info/LICENSE
+Filename: st_ant_carousel-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: st_ant_carousel-0.0.1.dist-info/METADATA
+Filename: st_ant_carousel-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: st_ant_carousel-0.0.1.dist-info/WHEEL
+Filename: st_ant_carousel-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: st_ant_carousel-0.0.1.dist-info/top_level.txt
+Filename: st_ant_carousel-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: st_ant_carousel-0.0.1.dist-info/RECORD
+Filename: st_ant_carousel-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## st_ant_carousel/__init__.py

```diff
@@ -23,15 +23,15 @@
     # replace the `url` param with `path`, and point it to to the component's
     # build directory:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component("st_ant_carousel", path=build_dir)
 
 def st_ant_carousel(content:list, carousel_style:dict = None, autoplay:bool = False, autoplaySpeed:int = 3000, dotPosition:str = "bottom", dots:bool = True,  waitForAnimate:bool = True, easing:str = "linear", effect:str = "scrollx",
-                    pauseOnDotsHover: bool = False, pauseOnHover:bool = True, animationSpeed:int = 500, vertical:bool=False, adaptiveHeight:bool = False, height:int = 200,key:str = "first_carousel") -> int:
+                    pauseOnDotsHover: bool = False, pauseOnHover:bool = True, animationSpeed:int = 500, vertical:bool=False, adaptiveHeight:bool = False, height:int = 200,key:str = "first_carousel", return_value = False) -> int:
     """
 
     Parameters
     ----------
     content: list, example: [{"style": {"font-color":"red", "font-size": "20px"}, "content": "<b>1. Entry<b>"},{"style": {"font-color":"blue", "font-size": "20px"}, "content": "<b><h1>2. Entry<b></h1>"}]
 
     carousel_style: dict, default None - The style of the carousel e.g. {"background-color": "black"}
@@ -47,18 +47,19 @@
     pauseOnHover: bool, default True - Whether to pause when hovering over the carousel
     animationSpeed: int, default 500 - Transition animation duration, in milliseconds
     vertical: bool, default False - Whether to scroll vertically
     adaptiveHeight: bool, default False - Whether to adapt to the height of the current slide
 
     key: str, default "first_carousel" - The key used to save the state of the widget
 
+    return_value: bool, default False - Whether to return the value of the widget - When True the widget will return the selected option, however this will leed to streamlit reloading the page. 
     
     Returns
     -------
-    The selected options as a list of strings.
+    The selected options as a list of strings. (only if return_value is True)
 
     """
     #  dropdownStyle={{ maxHeight: max_height, overflow: 'auto', width: width_dropdown }}
 
     #        style={{ width: width_dropdown, marginTop: "10px" }}
 
     if dotPosition not in ["top", "bottom", "left", "right"]:
@@ -119,10 +120,12 @@
             "padding": "30px",
 
         }
             
        
     component_value = _component_func(content=content,key = key, autoplay=autoplay, dotPosition=dotPosition, dots=dots,  waitForAnimate=waitForAnimate, easing=easing, effect=effect,autoplaySpeed=autoplaySpeed,
                                       pauseOnDotsHover=pauseOnDotsHover, pauseOnHover=pauseOnHover, animationSpeed=animationSpeed, vertical=vertical, adaptiveHeight=adaptiveHeight,height=height,carousel_style=carousel_style,
+                                      returnValue = return_value
                                       )
 
-    return component_value
+    if return_value:
+        return component_value
```

## Comparing `st_ant_carousel-0.0.1.dist-info/LICENSE` & `st_ant_carousel-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `st_ant_carousel-0.0.1.dist-info/METADATA` & `st_ant_carousel-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: st-ant-carousel
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit Component for ANT Carousel
 Author: 
 Author-email: 
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit (>=0.63)
 
 # st_ant_carousel
 
 A Streamlit custom component that displays a modern and customizable carousel using the Ant Design library.
 
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://flucas96-st-ant-carousel-example-app-9er76d.streamlit.app/)
+
+
 ## Installation
 
 You can install the st_ant_carousel component using pip:
 
 ```
 pip install st_ant_carousel
 ```
```

## Comparing `st_ant_carousel-0.0.1.dist-info/RECORD` & `st_ant_carousel-0.0.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-st_ant_carousel/__init__.py,sha256=sn-uUofFgcieV1BniMT5cgDwZXtApOdgXRIXu4uvmZY,5866
+st_ant_carousel/__init__.py,sha256=27qWy03CEGfiPgYXwfsbkFlRruHBuz9tmN_PrJ-L4CI,6207
 st_ant_carousel/frontend/build/asset-manifest.json,sha256=qLUK0lmFIaja0kcdPOAVdQIfKPEfMafWlh48Tptg684,859
 st_ant_carousel/frontend/build/bootstrap.min.css,sha256=X9ITP3t3djkRs4SffIkA1Q2WMy-oYl6au5HFYTVShe0,206960
 st_ant_carousel/frontend/build/index.html,sha256=FyR7pkO2mQ4Q4FG44K4jb4fSkDKLB4MeCCi44CJTTfI,2075
 st_ant_carousel/frontend/build/precache-manifest.2607c490f9520a6a70a96334da952fb8.js,sha256=pjAhVD31_pdMZFg0BlOeYUmwOddc0ngX_8ykWY3GOc4,564
 st_ant_carousel/frontend/build/service-worker.js,sha256=RQDVkwU8E2guAw-QCMqFqjGxC70AEHIePyUfxkJF-tY,1183
 st_ant_carousel/frontend/build/static/js/2.6435dd4a.chunk.js,sha256=s-S7TkWQyfg41yVqu4-CbgdYD04QGhNIFILzNiX9ILA,693699
 st_ant_carousel/frontend/build/static/js/2.6435dd4a.chunk.js.LICENSE.txt,sha256=uLktg5ueuL2SEYT1W5lpqqgmyG7YWw5pNowP6_cIHw8,1925
 st_ant_carousel/frontend/build/static/js/2.6435dd4a.chunk.js.map,sha256=ygn-xuCpgMGlD-fsD_jMeSgUeD7JV4QDF8QwnFDcJ2Q,1999238
 st_ant_carousel/frontend/build/static/js/main.a2df1366.chunk.js,sha256=NORfIgAfxjWZaTT0R5aQ4NIxgquCiKHPUNdhA2hvJRk,1754
 st_ant_carousel/frontend/build/static/js/main.a2df1366.chunk.js.map,sha256=XJ2WPw9gKlocyI6djmhvufAe4FiUMDOBQnujIu98fhQ,5650
 st_ant_carousel/frontend/build/static/js/runtime-main.502c8693.js,sha256=xr1UCWnVJHD-4X35euxCvVvsh5rX6m6OErjerkpepFo,1572
 st_ant_carousel/frontend/build/static/js/runtime-main.502c8693.js.map,sha256=FkgabUfZVsIiDu-syl6_U8PiWAlWX7AWjiKLpCfzTmA,8291
-st_ant_carousel-0.0.1.dist-info/LICENSE,sha256=Rf0bFykiS2fprQb8Gknfmwp4h9J2AkaE_fMrKC6vd0g,1084
-st_ant_carousel-0.0.1.dist-info/METADATA,sha256=RE7Itt_ZSRSSnKEuDyKzVSMZEhgnMvXjdh02fL12b-Q,4895
-st_ant_carousel-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-st_ant_carousel-0.0.1.dist-info/top_level.txt,sha256=s8xOu6B_B4gKciRmCx-SBPmnQqYLeLVokqO3r1h_9uM,16
-st_ant_carousel-0.0.1.dist-info/RECORD,,
+st_ant_carousel-0.0.2.dist-info/LICENSE,sha256=Rf0bFykiS2fprQb8Gknfmwp4h9J2AkaE_fMrKC6vd0g,1084
+st_ant_carousel-0.0.2.dist-info/METADATA,sha256=nxX01aVcylBRX3R6lKvwR1dX0pGrJklTegQarNloDZw,5055
+st_ant_carousel-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+st_ant_carousel-0.0.2.dist-info/top_level.txt,sha256=s8xOu6B_B4gKciRmCx-SBPmnQqYLeLVokqO3r1h_9uM,16
+st_ant_carousel-0.0.2.dist-info/RECORD,,
```

