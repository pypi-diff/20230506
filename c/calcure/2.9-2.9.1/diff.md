# Comparing `tmp/calcure-2.9.tar.gz` & `tmp/calcure-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcure-2.9.tar", last modified: Thu May  4 11:42:08 2023, max compression
+gzip compressed data, was "calcure-2.9.1.tar", last modified: Sat May  6 06:51:01 2023, max compression
```

## Comparing `calcure-2.9.tar` & `calcure-2.9.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-04 11:42:08.356486 calcure-2.9/
--rw-r--r--   0 r         (1000) r         (1000)     1071 2023-03-01 08:49:55.000000 calcure-2.9/LICENSE
--rw-r--r--   0 r         (1000) r         (1000)     3906 2023-05-04 11:42:08.356486 calcure-2.9/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     3145 2023-03-02 07:55:45.000000 calcure-2.9/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-04 11:42:08.356486 calcure-2.9/calcure/
--rw-r--r--   0 r         (1000) r         (1000)    41137 2023-05-04 11:06:59.000000 calcure-2.9/calcure/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     2551 2023-03-02 07:54:07.000000 calcure-2.9/calcure/calendars.py
--rw-r--r--   0 r         (1000) r         (1000)     4162 2023-03-04 12:39:25.000000 calcure-2.9/calcure/colors.py
--rw-r--r--   0 r         (1000) r         (1000)    20290 2023-05-04 10:23:28.000000 calcure-2.9/calcure/configuration.py
--rw-r--r--   0 r         (1000) r         (1000)    25533 2023-05-04 11:25:37.000000 calcure-2.9/calcure/controls.py
--rw-r--r--   0 r         (1000) r         (1000)    13499 2023-05-04 11:25:39.000000 calcure-2.9/calcure/data.py
--rw-r--r--   0 r         (1000) r         (1000)     3564 2023-05-03 20:15:00.000000 calcure-2.9/calcure/dialogues.py
--rw-r--r--   0 r         (1000) r         (1000)     1071 2023-05-03 19:07:50.000000 calcure-2.9/calcure/errors.py
--rw-r--r--   0 r         (1000) r         (1000)     3689 2023-05-03 19:07:39.000000 calcure-2.9/calcure/importers.py
--rw-r--r--   0 r         (1000) r         (1000)    14637 2023-05-04 10:09:19.000000 calcure-2.9/calcure/loaders.py
--rw-r--r--   0 r         (1000) r         (1000)     2550 2023-03-01 08:49:55.000000 calcure-2.9/calcure/savers.py
--rw-r--r--   0 r         (1000) r         (1000)     4725 2023-05-03 18:19:49.000000 calcure-2.9/calcure/screen.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-04 11:42:08.356486 calcure-2.9/calcure/translations/
--rw-r--r--   0 r         (1000) r         (1000)     5793 2023-05-04 11:34:28.000000 calcure-2.9/calcure/translations/br.py
--rw-r--r--   0 r         (1000) r         (1000)     5289 2023-05-04 11:33:46.000000 calcure-2.9/calcure/translations/en.py
--rw-r--r--   0 r         (1000) r         (1000)     6251 2023-05-04 11:37:01.000000 calcure-2.9/calcure/translations/fr.py
--rw-r--r--   0 r         (1000) r         (1000)     6283 2023-05-04 11:34:29.000000 calcure-2.9/calcure/translations/it.py
--rw-r--r--   0 r         (1000) r         (1000)     8277 2023-05-04 11:34:30.000000 calcure-2.9/calcure/translations/ru.py
--rw-r--r--   0 r         (1000) r         (1000)     6134 2023-05-04 11:34:30.000000 calcure-2.9/calcure/translations/tr.py
--rw-r--r--   0 r         (1000) r         (1000)     5433 2023-05-04 11:36:18.000000 calcure-2.9/calcure/translations/zh.py
--rw-r--r--   0 r         (1000) r         (1000)      905 2023-03-01 08:49:55.000000 calcure-2.9/calcure/weather.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-04 11:42:08.356486 calcure-2.9/calcure.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     3906 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      672 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       49 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       23 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)        8 2023-05-04 11:42:08.000000 calcure-2.9/calcure.egg-info/top_level.txt
--rw-r--r--   0 r         (1000) r         (1000)       91 2023-03-01 08:49:55.000000 calcure-2.9/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-04 11:42:08.356486 calcure-2.9/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1427 2023-03-01 08:49:55.000000 calcure-2.9/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-06 06:51:01.751570 calcure-2.9.1/
+-rw-r--r--   0 r         (1000) r         (1000)     1071 2023-03-01 08:49:55.000000 calcure-2.9.1/LICENSE
+-rw-r--r--   0 r         (1000) r         (1000)     3908 2023-05-06 06:51:01.751570 calcure-2.9.1/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     3145 2023-03-02 07:55:45.000000 calcure-2.9.1/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-06 06:51:01.751570 calcure-2.9.1/calcure/
+-rw-r--r--   0 r         (1000) r         (1000)    41704 2023-05-06 06:48:22.000000 calcure-2.9.1/calcure/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     2551 2023-03-02 07:54:07.000000 calcure-2.9.1/calcure/calendars.py
+-rw-r--r--   0 r         (1000) r         (1000)     4162 2023-03-04 12:39:25.000000 calcure-2.9.1/calcure/colors.py
+-rw-r--r--   0 r         (1000) r         (1000)    20458 2023-05-06 06:48:33.000000 calcure-2.9.1/calcure/configuration.py
+-rw-r--r--   0 r         (1000) r         (1000)    25533 2023-05-04 11:25:37.000000 calcure-2.9.1/calcure/controls.py
+-rw-r--r--   0 r         (1000) r         (1000)    13499 2023-05-04 11:25:39.000000 calcure-2.9.1/calcure/data.py
+-rw-r--r--   0 r         (1000) r         (1000)     3564 2023-05-03 20:15:00.000000 calcure-2.9.1/calcure/dialogues.py
+-rw-r--r--   0 r         (1000) r         (1000)     1071 2023-05-04 12:44:35.000000 calcure-2.9.1/calcure/errors.py
+-rw-r--r--   0 r         (1000) r         (1000)     3689 2023-05-03 19:07:39.000000 calcure-2.9.1/calcure/importers.py
+-rw-r--r--   0 r         (1000) r         (1000)    14637 2023-05-04 10:09:19.000000 calcure-2.9.1/calcure/loaders.py
+-rw-r--r--   0 r         (1000) r         (1000)     2550 2023-03-01 08:49:55.000000 calcure-2.9.1/calcure/savers.py
+-rw-r--r--   0 r         (1000) r         (1000)     4725 2023-05-06 06:48:16.000000 calcure-2.9.1/calcure/screen.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-06 06:51:01.751570 calcure-2.9.1/calcure/translations/
+-rw-r--r--   0 r         (1000) r         (1000)     5793 2023-05-04 11:34:28.000000 calcure-2.9.1/calcure/translations/br.py
+-rw-r--r--   0 r         (1000) r         (1000)     5289 2023-05-04 11:33:46.000000 calcure-2.9.1/calcure/translations/en.py
+-rw-r--r--   0 r         (1000) r         (1000)     6251 2023-05-04 11:37:01.000000 calcure-2.9.1/calcure/translations/fr.py
+-rw-r--r--   0 r         (1000) r         (1000)     6283 2023-05-04 11:34:29.000000 calcure-2.9.1/calcure/translations/it.py
+-rw-r--r--   0 r         (1000) r         (1000)     8277 2023-05-04 11:34:30.000000 calcure-2.9.1/calcure/translations/ru.py
+-rw-r--r--   0 r         (1000) r         (1000)     6134 2023-05-04 11:34:30.000000 calcure-2.9.1/calcure/translations/tr.py
+-rw-r--r--   0 r         (1000) r         (1000)     5433 2023-05-04 11:36:18.000000 calcure-2.9.1/calcure/translations/zh.py
+-rw-r--r--   0 r         (1000) r         (1000)      989 2023-05-06 06:48:14.000000 calcure-2.9.1/calcure/weather.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-06 06:51:01.751570 calcure-2.9.1/calcure.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     3908 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      672 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       49 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       23 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)        8 2023-05-06 06:51:01.000000 calcure-2.9.1/calcure.egg-info/top_level.txt
+-rw-r--r--   0 r         (1000) r         (1000)       91 2023-03-01 08:49:55.000000 calcure-2.9.1/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-06 06:51:01.751570 calcure-2.9.1/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1427 2023-03-01 08:49:55.000000 calcure-2.9.1/setup.py
```

### Comparing `calcure-2.9/LICENSE` & `calcure-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calcure-2.9/PKG-INFO` & `calcure-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcure
-Version: 2.9
+Version: 2.9.1
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/anufrievroman/calcure
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calcure-2.9/README.md` & `calcure-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/__main__.py` & `calcure-2.9.1/calcure/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     from calcure.translations.tr import *
 elif cf.LANG == "zh":
     from calcure.translations.zh import *
 else:
     from calcure.translations.en import *
 
 
-__version__ = "2.9"
+__version__ = "2.9.1"
 
 
 def read_items_from_user_arguments(screen, user_tasks, user_events, task_saver_csv, event_saver_csv):
     """Read --task and --event flags from user arguments to create new tasks or events"""
     try:
         opts, _ = getopt.getopt(sys.argv[1:], "pjhvi", ["folder=", "config=", "task=", "event="])
         for opt, arg in opts:
@@ -257,35 +257,44 @@
         """Select the right icon for the event"""
         return cf.EVENT_ICON
 
     @property
     def color(self):
         """Assign color depending on the status or calendar number if it's from .ics file"""
         if self.event.calendar_number is None:
-
             if self.event.status == Status.DONE:
                 return Color.DONE
             if self.event.status == Status.IMPORTANT:
                 return Color.IMPORTANT
             if self.event.status == Status.UNIMPORTANT:
                 return Color.UNIMPORTANT
             return Color.EVENTS
         else:
             for color in Color:
                 if color.value == Color.ICS_CALENDARS0.value + self.event.calendar_number:
                     return color
             return Color.EVENTS
 
+    def decorate_info(self):
+        """Icon and name of the event, which is decorated if needed"""
+        if self.event.status == Status.DONE and cf.STRIKETHROUGH_DONE_TASKS:
+            strike = "\u0336"
+            self.info = f'{self.icon} {strike}{strike.join(self.event.name)}{strike}'
+
     def obfuscate_info(self):
         """Obfuscate the info if privacy mode is on"""
-        self.info = f'{cf.EVENT_ICON} {cf.PRIVACY_ICON * len(self.event.name)}'
+        if self.screen.privacy or self.event.privacy:
+            self.info = f'{cf.EVENT_ICON} {cf.PRIVACY_ICON * len(self.event.name)}'
 
     def cut_info(self):
         """Cut the name to fit into the cell of the calendar"""
-        self.info = self.info[:self.screen.x_max - self.x]
+        avaliable_space = self.screen.x_max - self.x
+        number_of_special = self.info[:avaliable_space].count('\u0336')
+        number_of_special += 2 if number_of_special > 2 else 0
+        self.info = self.info[:self.screen.x_max - self.x + number_of_special]
         x_cell = self.screen.x_max // 7
         if (cf.CUT_TITLES or cf.SHOW_CALENDAR_BOARDERS) and self.screen.calendar_state == CalState.MONTHLY:
             self.info = self.info[:(x_cell - 1)]
 
     def minimize_info(self):
         """Reduce the info to just icon if not much space if available"""
         x_cell = self.screen.x_max // 7
@@ -312,16 +321,16 @@
                     icon = cf.ICONS[keyword]
         if self.screen.privacy or self.event.privacy:
             icon = cf.PRIVACY_ICON
         return icon
 
     def render(self):
         """Render this view on the screen"""
-        if self.screen.privacy or self.event.privacy:
-            self.obfuscate_info()
+        self.decorate_info()
+        self.obfuscate_info()
         self.fill_remaining_space()
         self.cut_info()
         self.minimize_info()
         self.display_line(self.y, self.x, self.info, self.color)
 
 
 class BirthdayView(EventView):
@@ -523,15 +532,15 @@
         """Render this view on the screen"""
         _, x_max = self.stdscr.getmaxyx()
 
         # Show title:
         title_view = TitleView(self.stdscr, 0, self.screen.x_min, self.title, self.screen)
         title_view.render()
 
-        if self.screen.state == AppState.JOURNAL and self.screen.split:
+        if self.screen.currently_drawn == AppState.JOURNAL and self.screen.split:
             return
 
         # Show weather is space allows and it is loaded:
         size_allows = len(self.weather.forcast) < self.screen.x_max - len(self.title)
         if cf.SHOW_WEATHER and size_allows:
             self.display_line(0, self.screen.x_max - len(self.weather.forcast) - 1, self.weather.forcast, Color.WEATHER)
 
@@ -919,15 +928,15 @@
         self.display_line(d_y + 5, d_x, MSG_SITE, Color.TITLE)
 
 
 def main(stdscr) -> None:
     """Main function that runs and switches screens"""
 
     # Load the data:
-    weather = Weather(cf.WEATHER_CITY)
+    weather = Weather(cf.WEATHER_CITY, cf.WEATHER_METRIC_UNITS)
     if cf.SHOW_WEATHER:
         sys.stdout.write(f"\r{MSG_WEATHER}")
         weather.load_from_wttr()
     screen = Screen(stdscr, cf)
 
     # Initialise loaders:
     event_loader_csv = EventLoaderCSV(cf)
```

### Comparing `calcure-2.9/calcure/calendars.py` & `calcure-2.9.1/calcure/calendars.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/colors.py` & `calcure-2.9.1/calcure/colors.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/configuration.py` & `calcure-2.9.1/calcure/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
                 "default_view":              "calendar",
                 "default_calendar_view":     "monthly",
                 "birthdays_from_abook":      "Yes",
                 "show_keybindings":          "Yes",
                 "privacy_mode":              "No",
                 "show_weather":              "No",
                 "weather_city":              "",
+                "weather_metric_units":      "Yes",
                 "minimal_today_indicator":   "Yes",
                 "minimal_days_indicator":    "Yes",
                 "minimal_weekend_indicator": "Yes",
                 "show_calendar_boarders":    "No",
                 "cut_titles_by_cell_length": "No",
                 "ask_confirmations":         "Yes",
                 "use_unicode_icons":         "Yes",
@@ -202,14 +203,15 @@
             self.USE_PERSIAN_CALENDAR      = conf.getboolean("Parameters", "use_persian_calendar", fallback=False)
             self.LANG                      = conf.get("Parameters", "language", fallback="en")
             self.START_WEEK_DAY            = int(conf.get("Parameters", "start_week_day", fallback=1))
             self.WEEKEND_DAYS              = conf.get("Parameters", "weekend_days", fallback="6,7")
             self.WEEKEND_DAYS              = [int(i) for i in self.WEEKEND_DAYS.split(",")]
             self.HOLIDAY_COUNTRY           = conf.get("Parameters", "holiday_country", fallback="UnitedStates")
             self.WEATHER_CITY              = conf.get("Parameters", "weather_city", fallback="")
+            self.WEATHER_METRIC_UNITS      = conf.getboolean("Parameters", "weather_metric_units", fallback=True)
             self.DEFAULT_CALENDAR_VIEW     = conf.get("Parameters", "default_calendar_view", fallback="monthly")
 
             # Journal settings:
             self.CALCURSE_TODO_FILE    = conf.get("Parameters", "calcurse_todo_file", fallback=self.calcurse_todo_file)
             self.CALCURSE_EVENTS_FILE  = conf.get("Parameters", "calcurse_events_file", fallback=self.calcurse_events_file)
             self.TASKWARRIOR_FOLDER    = conf.get("Parameters", "taskwarrior_folder", fallback=self.taskwarrior_folder)
             self.JOURNAL_HEADER        = conf.get("Parameters", "journal_header", fallback="JOURNAL")
@@ -332,15 +334,15 @@
                     self.DEFAULT_VIEW = AppState.JOURNAL
                 elif opt == '-d':
                     self.DEFAULT_VIEW = AppState.JOURNAL
                 elif opt in ('-h'):
                     self.DEFAULT_VIEW = AppState.HELP
                 elif opt in ('-v'):
                     self.DEFAULT_VIEW = AppState.EXIT
-                    print ('Calcure - version 2.9')
+                    print ('Calcure - version 2.9.1')
                 elif opt in ('-i'):
                     self.USE_PERSIAN_CALENDAR = True
         except getopt.GetoptError as e_message:
             logging.error("Invalid user arguments. %s", e_message)
             pass
```

### Comparing `calcure-2.9/calcure/controls.py` & `calcure-2.9.1/calcure/controls.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/data.py` & `calcure-2.9.1/calcure/data.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/dialogues.py` & `calcure-2.9.1/calcure/dialogues.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/errors.py` & `calcure-2.9.1/calcure/errors.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/importers.py` & `calcure-2.9.1/calcure/importers.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/loaders.py` & `calcure-2.9.1/calcure/loaders.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/savers.py` & `calcure-2.9.1/calcure/savers.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/screen.py` & `calcure-2.9.1/calcure/screen.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/translations/br.py` & `calcure-2.9.1/calcure/translations/br.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/translations/en.py` & `calcure-2.9.1/calcure/translations/en.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/translations/fr.py` & `calcure-2.9.1/calcure/translations/fr.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/translations/it.py` & `calcure-2.9.1/calcure/translations/it.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/translations/ru.py` & `calcure-2.9.1/calcure/translations/ru.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/translations/tr.py` & `calcure-2.9.1/calcure/translations/tr.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/translations/zh.py` & `calcure-2.9.1/calcure/translations/zh.py`

 * *Files identical despite different names*

### Comparing `calcure-2.9/calcure/weather.py` & `calcure-2.9.1/calcure/weather.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 import subprocess
 import logging
 
 
 class Weather:
     """Information about the weather today"""
 
-    def __init__(self, city):
+    def __init__(self, city, is_metric_units):
         self.city = city
         self.forcast = ""
         self.max_load_time = 2  # seconds
+        self.units = "?m" if is_metric_units else "?u"
 
     def load_from_wttr(self):
         """Load the weather info from wttr.in"""
         try:
-            request_url = f"wttr.in/{self.city}?format=3"
+            request_url = f"wttr.in/{self.city}{self.units}&format=3"
             self.forcast = str(subprocess.check_output(["curl", "-s", request_url],
                                                         timeout=self.max_load_time,
                                                         encoding='utf-8'))[:-1]
             self.forcast = self.forcast.split(':')[1]
         except (subprocess.TimeoutExpired, subprocess.CalledProcessError, IndexError):
             logging.warning("Weather failed to load.")
             self.forcast = ""
```

### Comparing `calcure-2.9/calcure.egg-info/PKG-INFO` & `calcure-2.9.1/calcure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcure
-Version: 2.9
+Version: 2.9.1
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/anufrievroman/calcure
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calcure-2.9/calcure.egg-info/SOURCES.txt` & `calcure-2.9.1/calcure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calcure-2.9/setup.py` & `calcure-2.9.1/setup.py`

 * *Files identical despite different names*

