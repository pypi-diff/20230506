# Comparing `tmp/meta-package-manager-5.8.0.tar.gz` & `tmp/meta_package_manager-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta-package-manager-5.8.0.tar", max compression
+gzip compressed data, was "meta_package_manager-5.9.0.tar", max compression
```

## Comparing `meta-package-manager-5.8.0.tar` & `meta_package_manager-5.9.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1302 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/__init__.py
--rw-r--r--   0        0        0     1451 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/__main__.py
--rw-r--r--   0        0        0     1462 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/bar_plugin/__init__.py
--rwxr-xr-x   0        0        0    14099 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/bar_plugin/meta_package_manager.7h.py
--rw-r--r--   0        0        0    32058 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/base.py
--rw-r--r--   0        0        0     2962 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/capabilities.py
--rw-r--r--   0        0        0    41104 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/cli.py
--rw-r--r--   0        0        0     3607 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/inventory.py
--rw-r--r--   0        0        0     2873 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/labels.py
--rw-r--r--   0        0        0      793 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/__init__.py
--rw-r--r--   0        0        0    16332 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/apm.py
--rw-r--r--   0        0        0    12100 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/apt.py
--rw-r--r--   0        0        0     5559 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/cargo.py
--rw-r--r--   0        0        0     5989 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/chocolatey.py
--rw-r--r--   0        0        0     7716 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/composer.py
--rw-r--r--   0        0        0     6637 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/dnf.py
--rw-r--r--   0        0        0    11160 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/emerge.py
--rw-r--r--   0        0        0     6917 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/flatpak.py
--rw-r--r--   0        0        0     8921 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/gem.py
--rw-r--r--   0        0        0    21044 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/homebrew.py
--rw-r--r--   0        0        0     5671 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/mas.py
--rw-r--r--   0        0        0    11033 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/npm.py
--rw-r--r--   0        0        0     5664 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/opkg.py
--rw-r--r--   0        0        0     7507 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/pacman.py
--rw-r--r--   0        0        0    10807 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/pip.py
--rw-r--r--   0        0        0     6661 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/pipx.py
--rw-r--r--   0        0        0     9200 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/scoop.py
--rw-r--r--   0        0        0     5519 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/snap.py
--rw-r--r--   0        0        0     2920 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/steamcmd.py
--rw-r--r--   0        0        0     2487 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/vscode.py
--rw-r--r--   0        0        0    13220 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/yarn.py
--rw-r--r--   0        0        0    10851 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/managers/zypper.py
--rw-r--r--   0        0        0    17890 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/output.py
--rw-r--r--   0        0        0     7834 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/pool.py
--rw-r--r--   0        0        0        0 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/py.typed
--rw-r--r--   0        0        0    11634 2022-10-05 13:00:03.918668 meta-package-manager-5.8.0/meta_package_manager/specifier.py
--rw-r--r--   0        0        0      793 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/__init__.py
--rw-r--r--   0        0        0     1523 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/conftest.py
--rw-r--r--   0        0        0     9677 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_bar_plugin.py
--rw-r--r--   0        0        0    13211 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli.py
--rw-r--r--   0        0        0     2131 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_backup.py
--rw-r--r--   0        0        0     1295 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_cleanup.py
--rw-r--r--   0        0        0     4066 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_install_remove.py
--rw-r--r--   0        0        0     2524 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_installed.py
--rw-r--r--   0        0        0     3375 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_managers.py
--rw-r--r--   0        0        0     2843 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_outdated.py
--rw-r--r--   0        0        0     4566 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_restore.py
--rw-r--r--   0        0        0     7002 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_search.py
--rw-r--r--   0        0        0     1289 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_sync.py
--rw-r--r--   0        0        0     2981 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_upgrade.py
--rw-r--r--   0        0        0     7031 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_docs.py
--rw-r--r--   0        0        0     5754 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_manager_homebrew.py
--rw-r--r--   0        0        0    12492 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_managers.py
--rw-r--r--   0        0        0     4706 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_pool.py
--rw-r--r--   0        0        0     8328 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_specifier.py
--rw-r--r--   0        0        0     8550 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/tests/test_version.py
--rw-r--r--   0        0        0    10662 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/meta_package_manager/version.py
--rw-r--r--   0        0        0     4819 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/pyproject.toml
--rw-r--r--   0        0        0    20365 2022-10-05 13:00:03.922668 meta-package-manager-5.8.0/readme.md
--rw-r--r--   0        0        0    21862 1970-01-01 00:00:00.000000 meta-package-manager-5.8.0/setup.py
--rw-r--r--   0        0        0    22994 1970-01-01 00:00:00.000000 meta-package-manager-5.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1302 2022-11-20 18:00:11.274708 meta_package_manager-5.9.0/meta_package_manager/__init__.py
+-rw-r--r--   0        0        0     1451 2022-11-20 18:00:11.274708 meta_package_manager-5.9.0/meta_package_manager/__main__.py
+-rw-r--r--   0        0        0     1462 2022-11-20 18:00:11.274708 meta_package_manager-5.9.0/meta_package_manager/bar_plugin/__init__.py
+-rwxr-xr-x   0        0        0    14099 2022-11-20 18:00:11.274708 meta_package_manager-5.9.0/meta_package_manager/bar_plugin/meta_package_manager.7h.py
+-rw-r--r--   0        0        0    33012 2022-11-20 18:00:11.274708 meta_package_manager-5.9.0/meta_package_manager/base.py
+-rw-r--r--   0        0        0     2962 2022-11-20 18:00:11.274708 meta_package_manager-5.9.0/meta_package_manager/capabilities.py
+-rw-r--r--   0        0        0    42014 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/cli.py
+-rw-r--r--   0        0        0     3607 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/inventory.py
+-rw-r--r--   0        0        0     2883 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/labels.py
+-rw-r--r--   0        0        0      793 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/__init__.py
+-rw-r--r--   0        0        0    16777 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/apm.py
+-rw-r--r--   0        0        0    12100 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/apt.py
+-rw-r--r--   0        0        0     5559 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/cargo.py
+-rw-r--r--   0        0        0     5989 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/chocolatey.py
+-rw-r--r--   0        0        0     7716 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/composer.py
+-rw-r--r--   0        0        0     6637 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/dnf.py
+-rw-r--r--   0        0        0    11160 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/emerge.py
+-rw-r--r--   0        0        0     6917 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/flatpak.py
+-rw-r--r--   0        0        0     8921 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/gem.py
+-rw-r--r--   0        0        0    21044 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/homebrew.py
+-rw-r--r--   0        0        0     5671 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/mas.py
+-rw-r--r--   0        0        0    11033 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/npm.py
+-rw-r--r--   0        0        0     5664 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/opkg.py
+-rw-r--r--   0        0        0     7877 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/pacman.py
+-rw-r--r--   0        0        0    10807 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/pip.py
+-rw-r--r--   0        0        0     6661 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/pipx.py
+-rw-r--r--   0        0        0     9200 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/scoop.py
+-rw-r--r--   0        0        0     5519 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/snap.py
+-rw-r--r--   0        0        0     2920 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/steamcmd.py
+-rw-r--r--   0        0        0     2487 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/vscode.py
+-rw-r--r--   0        0        0    13220 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/yarn.py
+-rw-r--r--   0        0        0    10851 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/managers/zypper.py
+-rw-r--r--   0        0        0    16840 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/output.py
+-rw-r--r--   0        0        0     8558 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/pool.py
+-rw-r--r--   0        0        0        0 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/py.typed
+-rw-r--r--   0        0        0    11634 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/specifier.py
+-rw-r--r--   0        0        0      793 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/__init__.py
+-rw-r--r--   0        0        0     1523 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/conftest.py
+-rw-r--r--   0        0        0     9677 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_bar_plugin.py
+-rw-r--r--   0        0        0    13179 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli.py
+-rw-r--r--   0        0        0     2131 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_backup.py
+-rw-r--r--   0        0        0     1295 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_cleanup.py
+-rw-r--r--   0        0        0     4101 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_install_remove.py
+-rw-r--r--   0        0        0     2524 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_installed.py
+-rw-r--r--   0        0        0     3375 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_managers.py
+-rw-r--r--   0        0        0     2843 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_outdated.py
+-rw-r--r--   0        0        0     4566 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_restore.py
+-rw-r--r--   0        0        0     7002 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_search.py
+-rw-r--r--   0        0        0     1289 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_sync.py
+-rw-r--r--   0        0        0     2981 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_upgrade.py
+-rw-r--r--   0        0        0     7031 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_docs.py
+-rw-r--r--   0        0        0     5909 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_manager_homebrew.py
+-rw-r--r--   0        0        0    13563 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_managers.py
+-rw-r--r--   0        0        0     6099 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_pool.py
+-rw-r--r--   0        0        0     8328 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_specifier.py
+-rw-r--r--   0        0        0     8550 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/tests/test_version.py
+-rw-r--r--   0        0        0    10662 2022-11-20 18:00:11.278708 meta_package_manager-5.9.0/meta_package_manager/version.py
+-rw-r--r--   0        0        0     4832 2022-11-20 18:00:11.282708 meta_package_manager-5.9.0/pyproject.toml
+-rw-r--r--   0        0        0    20618 2022-11-20 18:00:11.282708 meta_package_manager-5.9.0/readme.md
+-rw-r--r--   0        0        0    22117 1970-01-01 00:00:00.000000 meta_package_manager-5.9.0/setup.py
+-rw-r--r--   0        0        0    23306 1970-01-01 00:00:00.000000 meta_package_manager-5.9.0/PKG-INFO
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/__init__.py` & `meta_package_manager-5.9.0/meta_package_manager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 """Expose package-wide elements."""
 
-__version__ = "5.8.0"
+__version__ = "5.9.0"
 """ Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = '1.2.3.dev1'   # Development release 1
     __version__ = '1.2.3a1'      # Alpha Release 1
     __version__ = '1.2.3b1'      # Beta Release 1
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/__main__.py` & `meta_package_manager-5.9.0/meta_package_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/bar_plugin/__init__.py` & `meta_package_manager-5.9.0/meta_package_manager/bar_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/bar_plugin/meta_package_manager.7h.py` & `meta_package_manager-5.9.0/meta_package_manager/bar_plugin/meta_package_manager.7h.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # <xbar.title>Meta Package Manager</xbar.title>
-# <xbar.version>v5.8.0</xbar.version>
+# <xbar.version>v5.9.0</xbar.version>
 # <xbar.author>Kevin Deldycke</xbar.author>
 # <xbar.author.github>kdeldycke</xbar.author.github>
 # <xbar.desc>List outdated packages and manage upgrades.</xbar.desc>
 # <xbar.dependencies>python,mpm</xbar.dependencies>
 # <xbar.image>https://i.imgur.com/B5wdxIc.png</xbar.image>
 # <xbar.abouturl>https://github.com/kdeldycke/meta-package-manager</xbar.abouturl>
 # <xbar.var>boolean(VAR_SUBMENU_LAYOUT=false): Group packages into a sub-menu for each manager.</xbar.var>
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/base.py` & `meta_package_manager-5.9.0/meta_package_manager/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,31 @@
             cls.virtual = name == "PackageManager" or not cls.cli_names
 
 
 class PackageManager(metaclass=MetaPackageManager):
 
     """Base class from which all package manager definitions inherits."""
 
+    deprecated: bool = False
+    """A manager marked as deprecated will be hidden from all package selection by default.
+
+    You can still use it but need to explicitly call for it on the command line.
+
+    Implementation of a deprecated manager will be kept within mpm source code, but some of its
+    features or total implementation are allowed to be scraped in the face of
+    maintenance pain and adversity.
+
+    Integration tests and unittests for deprecated managers can be removed. We do not care if
+    a deprecated manager is not 100% reliable. A flakky deprecated manager should not block a
+    release due to flakky tests.
+    """
+
+    deprecation_url: str | None = None
+    """Announcement from the official project or evidence of abandonment of maintainance."""
+
     id: str
     """Package manager's ID.
 
     Derived by defaults from the lower-cased class name in which underscores ``_`` are replaced
     by dashes ``-``.
 
     This ID must be unique among all package manager definitions and lower-case, as
@@ -449,15 +466,17 @@
 
         1. is :py:attr:`supported on the current platform <meta_package_manager.base.PackageManager.supported>`,
         2. was :py:attr:`found on the system <meta_package_manager.base.PackageManager.cli_path>`,
         3. is :py:attr:`executable <meta_package_manager.base.PackageManager.executable>`, and
         4. :py:attr:`match the version requirement <meta_package_manager.base.PackageManager.fresh>`.
         """
         logger.debug(
-            f"{self.id} is supported: {self.supported}; "
+            f"{self.id} "
+            f"is deprecated: {self.deprecated}; "
+            f"is supported: {self.supported}; "
             f"found at: {self.cli_path}; "
             f"is executable: {self.executable}; "
             f"is fresh: {self.fresh}."
         )
         return bool(self.supported and self.cli_path and self.executable and self.fresh)
 
     def run(self, *args: Arg | NestedArgs, extra_env: EnvVars | None = None) -> str:
@@ -574,37 +593,37 @@
                 raise NotImplementedError("sudo only supported on Linux.")
             if override_pre_cmds:
                 raise ValueError("Pre-commands not allowed if sudo is requested.")
             if auto_pre_cmds:
                 auto_pre_cmds = False
             params.append("sudo")
         elif override_pre_cmds:
-            params.extend(override_pre_cmds)
+            params.extend(override_pre_cmds)  # type: ignore[arg-type]
         elif auto_pre_cmds:
             params.extend(self.pre_cmds)
 
         if override_cli_path:
             params.append(override_cli_path)
         else:
             params.append(self.cli_path)
 
         if override_pre_args:
-            params.extend(override_pre_args)
+            params.extend(override_pre_args)  # type: ignore[arg-type]
         elif auto_pre_args:
             params.extend(self.pre_args)
 
         if args:
             params.extend(args)
 
         if override_post_args:
-            params.extend(override_post_args)
+            params.extend(override_post_args)  # type: ignore[arg-type]
         elif auto_post_args:
             params.extend(self.post_args)
 
-        return args_cleanup(params)  # type: ignore
+        return args_cleanup(params)  # type: ignore[arg-type]
 
     def run_cli(
         self,
         *args: Arg | NestedArgs,
         auto_extra_env: bool = True,
         auto_pre_cmds: bool = True,
         auto_pre_args: bool = True,
@@ -814,12 +833,12 @@
         """Refresh package metadata from remote repositories.
 
         Optional. Will be simply skipped by :program:`mpm` if not implemented.
         """
         raise NotImplementedError
 
     def cleanup(self) -> None:
-        """Removes left-overs, orphaned dependencies,
+        """Prune left-overs, remove orphaned dependencies and clear caches.
 
         Optional. Will be simply skipped by :program:`mpm` if not implemented.
         """
         raise NotImplementedError
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/capabilities.py` & `meta_package_manager-5.9.0/meta_package_manager/capabilities.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/cli.py` & `meta_package_manager-5.9.0/meta_package_manager/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,22 @@
 from cloup import Section
 
 from . import __version__, bar_plugin, logger
 from .base import CLIError, Operations, PackageManager, packages_asdict
 from .output import (
     SORTABLE_FIELDS,
     BarPluginRenderer,
-    TabularOutputFormatter,
     colored_diff,
+    output_formats,
     print_json,
     print_stats,
     print_table,
 )
 from .pool import pool
-from .specifier import Solver, Specifier
+from .specifier import VERSION_SEP, Solver, Specifier
 
 # Subcommand sections.
 EXPLORE = Section("Explore subcommands")
 MAINTENANCE = Section("Maintenance subcommands")
 SNAPSHOTS = Section("Package snapshots subcommands")
 
 
@@ -84,19 +84,23 @@
         manager_id = param.name.replace("_", "-")
         ctx.obj["single_manager_selector"].append(manager_id)
 
 
 def single_manager_selectors():
     """Dynamiccaly creates a dedicated flag selector alias for each manager."""
     for manager_id in pool.all_manager_ids:
+        manager = pool.get(manager_id)
+        # Parameters do not have a deprecated flag.
+        # See: https://github.com/pallets/click/issues/2263
+        deprecated_msg = " (deprecated)" if manager.deprecated else ""
         yield option(
             f"--{manager_id}",
             is_flag=True,
             default=False,
-            help=f"Alias to --manager {manager_id}.",
+            help=f"Alias to --manager {manager_id}{deprecated_msg}.",
             expose_value=False,
             callback=add_manager_to_selection,
         )
 
 
 def bar_plugin_path(ctx, param, value):
     """Print the location of the :doc:`Xbar/SwiftBar plugin <bar-plugin>`.
@@ -151,17 +155,17 @@
         help="Exclude a manager. Repeat to exclude multiple managers.",
     ),
     option(
         "-a",
         "--all-managers",
         is_flag=True,
         default=False,
-        help="Force evaluation of all manager recognized by mpm, even those "
-        "not supported by the current platform. Still applies filtering by --manager "
-        "and --exclude options before calling the subcommand.",
+        help="Force evaluation of all managers recognized by mpm, including those "
+        "not supported by the current platform or deprecated. Still applies filtering "
+        "by --manager and --exclude options before calling the subcommand.",
     ),
     option(
         "-x",
         "--xkcd",
         is_flag=True,
         default=False,
         help="Preset manager selection as defined by XKCD #1654. Equivalent to: "
@@ -191,17 +195,15 @@
     ),
 )
 @option_group(
     "Output options",
     table_format_option(
         "-o",
         "--output-format",
-        type=Choice(
-            sorted(TabularOutputFormatter._output_formats), case_sensitive=False
-        ),
+        type=Choice(output_formats, case_sensitive=False),
         help="Rendering mode of the output.",
     ),
     option(
         "--description",
         is_flag=True,
         default=False,
         help="Show package description in results.",
@@ -241,30 +243,47 @@
     dry_run,
     description,
     sort_by,
     stats,
 ):
     """Common CLI options for subcommands."""
 
-    # Update the list of selected managers with single selectors.
-    if ctx.obj:
-        manager = list(manager) + ctx.obj.get("single_manager_selector", [])
-
     # Silence all log message for JSON rendering unless in debug mode.
     level = logger.level
     level_name = logging._levelToName.get(level, level)
-    if ctx.find_root().table_formatter.format_name == "json" and level_name != "DEBUG":
+    if ctx.find_root().table_format == "json" and level_name != "DEBUG":
         logger.setLevel(logging.CRITICAL * 2)
 
+    # Merge all manager selectors to form the initial population enforced by the
+    # user.
+    initial_managers = list(manager)
+    # Update with single selectors.
+    if ctx.obj:
+        initial_managers.extend(ctx.obj.get("single_manager_selector", []))
+    # Update the list of managers with the XKCD preset.
+    if xkcd:
+        initial_managers.extend(XKCD_MANAGER_ORDER)
+    # Normalize to None if no manager selectors have been used. This prevent the
+    # pool.select_managers() method to iterate over an empty population of managers to
+    # choose from.
+    if not initial_managers:
+        initial_managers = None
+        logger.debug(f"No initial population of managers selected by user.")
+    else:
+        logger.debug(
+            "Initial population of user-selected managers: "
+            f"{' > '.join(map(theme.invoked_command, initial_managers))}"
+        )
+
     # Select the subset of manager to target, and apply manager-level options.
     selected_managers = partial(
         pool.select_managers,
-        keep=manager if not xkcd else XKCD_MANAGER_ORDER,
+        keep=initial_managers,
         drop=exclude,
-        keep_unsupported=all_managers,
+        keep_deprecated=all_managers,
         # Should we include auto-update packages or not?
         ignore_auto_updates=ignore_auto_updates,
         # Does the manager should raise on error or not.
         stop_on_error=stop_on_error,
         dry_run=dry_run,
     )
 
@@ -296,15 +315,15 @@
     select_params = {
         # Do not drop inactive managers. Keep them to show off how mpm is reacting
         # to the local platform.
         "drop_inactive": False,
     }
 
     # Machine-friendly data rendering.
-    if ctx.find_root().table_formatter.format_name == "json":
+    if ctx.find_root().table_format == "json":
         manager_data = {}
         # Build up the data structure of manager metadata.
         fields = (
             "name",
             "id",
             "supported",
             "cli_path",
@@ -329,14 +348,16 @@
 
         # Build up the OS column content.
         os_infos = OK if manager.supported else KO
         if not manager.supported:
             os_infos += " {} only".format(
                 ", ".join(sorted(os_label(os_id) for os_id in manager.platforms))
             )
+        if manager.deprecated:
+            os_infos += f" {theme.warning('(deprecated)')}"
 
         # Build up the CLI path column content.
         cli_infos = "{} {}".format(
             OK if manager.cli_path else KO,
             # TODO: highlight cli_name found in manager.cli_path. I.e, the "choco" string in:
             #    ✓ C:\ProgramData\chocolatey\bin\choco.EXE
             manager.cli_path
@@ -434,15 +455,15 @@
                 p
                 for p in installed_data[manager_id]["packages"]
                 if p["id"] in duplicates_ids
             )
             installed_data[manager_id]["packages"] = duplicate_packages
 
     # Machine-friendly data rendering.
-    if ctx.find_root().table_formatter.format_name == "json":
+    if ctx.find_root().table_format == "json":
         print_json(installed_data)
         ctx.exit()
 
     # Human-friendly content rendering.
     table = []
     for manager_id, installed_pkg in installed_data.items():
         table += [
@@ -509,15 +530,15 @@
 
         # Serialize errors at the last minute to gather all we encountered.
         outdated_data[manager.id]["errors"] = list(
             {expt.error for expt in manager.cli_errors}
         )
 
     # Machine-friendly data rendering.
-    if ctx.find_root().table_formatter.format_name == "json":
+    if ctx.find_root().table_format == "json":
         print_json(outdated_data)
         ctx.exit()
 
     # Xbar/SwiftBar-friendly plugin rendering.
     if plugin_output:
         BarPluginRenderer().print(outdated_data)
         ctx.exit()
@@ -619,15 +640,15 @@
 
         # Serialize errors at the last minute to gather all we encountered.
         matches[manager.id]["errors"] = list(
             {expt.error for expt in manager.cli_errors}
         )
 
     # Machine-friendly data rendering.
-    if ctx.find_root().table_formatter.format_name == "json":
+    if ctx.find_root().table_format == "json":
         print_json(matches)
         ctx.exit()
 
     # Prepare highlighting helpers.
     query_parts = {query}.union(PackageManager.query_parts(query))
     highlight_query = cached(LRI(max_size=1000))(
         partial(
@@ -1156,15 +1177,16 @@
             if manager.id not in doc:
                 logger.warning(
                     f"No [{theme.invoked_command(manager.id)}] section found."
                 )
                 continue
             logger.info(f"Restore {theme.invoked_command(manager.id)} packages...")
             for package_id, version in doc[manager.id].items():
-                spec = Specifier(package_id=package_id, version=version)
-                # Let the command fail if the manager doesn't implement the
-                # install operation.
-                logger.info(
-                    f"Install {spec} package with {theme.invoked_command(manager.id)}..."
+                spec = Specifier(
+                    raw_spec=f"pkg:{manager.id}:/{package_id}{VERSION_SEP}{package_id}",
+                    package_id=package_id,
+                    manager_id=manager.id,
+                    version=version,
                 )
+                logger.info(f"Install {spec}...")
                 output = manager.install(spec.package_id, version=spec.version)
                 echo(output)
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/inventory.py` & `meta_package_manager-5.9.0/meta_package_manager/inventory.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/labels.py` & `meta_package_manager-5.9.0/meta_package_manager/labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 """ Maps all manager IDs to their labels. """
 
 
 MANAGER_GROUPS = {
     "dnf-based": {"dnf", "yum"},
     "dpkg-based": {"dpkg", "apt", "apt-mint", "opkg"},
     "npm-based": {"npm", "yarn"},
-    "pacman-based": {"pacman", "paru", "yay"},
+    "pacman-based": {"pacman", "pacaur", "paru", "yay"},
     "pip-based": {"pip", "pipx"},
 }
 """Managers sharing some roots or implementation will be grouped together."""
 
 
 PLATFORM_PREFIX = "🖥 platform: "
 """Default platform label prefix."""
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/__init__.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/apm.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/apm.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,24 @@
 
 from ..base import Package, PackageManager
 from ..capabilities import search_capabilities, version_not_implemented
 
 
 class APM(PackageManager):
 
+    deprecated = True
+    deprecation_url = "https://github.blog/2022-06-08-sunsetting-atom/"
+    """GitHub announced the end of the project for December 15, 2022.
+    Source: https://github.blog/2022-06-08-sunsetting-atom/
+
+    There is a tentative community fork being discussed. See: https://github.com/atom-community/apm
+
+    In the mean time, as long as no apm alternative is useable, it is safe to tag this manager as deprecated.
+    """
+
     name = "Atom's apm"
 
     homepage_url = "https://atom.io/packages"
 
     platforms = frozenset({LINUX, MACOS, WINDOWS})
 
     requirement = "1.0.0"
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/apt.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/apt.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/cargo.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/cargo.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/chocolatey.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/chocolatey.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/composer.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/composer.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/dnf.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/dnf.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/emerge.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/emerge.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/flatpak.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/flatpak.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/gem.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/gem.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/homebrew.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/homebrew.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/mas.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/mas.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/npm.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/npm.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/opkg.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/opkg.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/pacman.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/pacman.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,14 +197,31 @@
         .. code-block:: shell-session
 
             ► sudo pacman --noconfirm --sync --clean --clean
         """
         self.run_cli("--sync", "--clean", "--clean", sudo=True)
 
 
+class Pacaur(Pacman):
+    """``Pacaur`` wraps ``pacman`` and shadows its options."""
+
+    homepage_url = "https://github.com/E5ten/pacaur"
+
+    requirement = "4.0.0"
+
+    version_regex = r"pacaur\s+(?P<version>\S+)"
+    r"""Search version right after the ``pacaur`` string.
+
+    .. code-block:: shell-session
+
+        ► pacaur --version
+        pacaur 4.8.6
+    """
+
+
 class Paru(Pacman):
     """``paru`` wraps ``pacman`` and shadows its options."""
 
     homepage_url = "https://github.com/Morganamilo/paru"
 
     # v1.9.3 is the first version implementing the --sysupgrade option.
     requirement = "1.9.3"
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/pip.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/pip.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/pipx.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/pipx.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/scoop.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/scoop.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/snap.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/snap.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/steamcmd.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/steamcmd.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/vscode.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/vscode.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/yarn.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/yarn.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/managers/zypper.py` & `meta_package_manager-5.9.0/meta_package_manager/managers/zypper.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/output.py` & `meta_package_manager-5.9.0/meta_package_manager/output.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 else:
     from boltons.cacheutils import cachedproperty as cached_property
 
 from boltons.iterutils import flatten
 from boltons.strutils import strip_ansi
 from click_extra import echo, get_current_context, style
 from click_extra.colorize import default_theme as theme
-from click_extra.tabulate import TabularOutputFormatter
+from click_extra.tabulate import output_formats
 from tabulate import DataRow, TableFormat, tabulate
 
 from . import logger
 from .bar_plugin import MPMPlugin  # type: ignore
 from .pool import pool
 from .version import TokenizedString
 
@@ -94,33 +94,15 @@
         colored_a += style_a(a[common_size:])
     if b:
         colored_b += style_b(b[common_size:])
 
     return colored_a, colored_b
 
 
-def not_implemented_json_handler(data, headers, **kwargs):
-    """Dummy `TabularOutputFormatter <https://cli-helpers.readthedocs.io/en/latest/api.h
-    tml#cli_helpers.tabular_output.TabularOutputFormatter>`_ renderer.
-
-    Raises a :py:exc:`NotImplementedError` exception as this handler is not designed to
-    be used as-is by `tabulate module <https://github.com/astanin/python-tabulate>`_.
-    Its only purpose is to serve as a signal to detect leaks in our custom JSON
-    rendering code path.
-    """
-    raise NotImplementedError(
-        "JSON rendering is not generic and need specific subcommand implementation."
-    )
-
-
-TabularOutputFormatter.register_new_formatter("json", not_implemented_json_handler)
-"""Register our custom JSON rendering option to `TabularOutputFormatter <https://cli-helpers.readthedocs.io/en/latest/api.html#cli_helpers.tabular_output.TabularOutputFormatter>`_.
-
-Link it to the dummy :function:`not_implemented_json_handler` renderer as we plan to intercept the JSON option before the tabular renderer has a chance to call it.
-"""
+output_formats = sorted(output_formats + ["json"])
 
 
 def print_json(data):
     """Pretty-print Python data to JSON and output results to ``<stdout>``.
 
     Serialize :py:class:`pathlib.Path` and :py:class:`meta_package_manager.version.TokenizedString` objects.
     """
@@ -140,15 +122,15 @@
         ),
         # Do not pollute output with ANSI codes.
         color=False,
     )
 
 
 def print_table(header_defs, rows, sort_key=None):
-    """Print a table.
+    """Print a sorted table.
 
     ``header_defs`` parameter is an ordered list of tuple whose first item is the column's label and the second the column's ID. Example:
 
     .. code-block:: python
 
         [("Column 1", "column1"), ("User's name", "name"), ("Package manager", "manager_id"), ...]
 
@@ -191,40 +173,38 @@
                 key = None
             else:
                 key = TokenizedString(strip_ansi(cell))
             sorting_key.append(key)
         return tuple(sorting_key)
 
     ctx = get_current_context()
-    ctx.find_root().print_table(
-        sorted(rows, key=sort_method), header_labels, disable_numparse=True
-    )
+    ctx.find_root().print_table(sorted(rows, key=sort_method), header_labels)
 
 
 def print_stats(manager_stats: Counter) -> None:
-    """Prints statistics to ``<stdout>``: total packages and a break down by package
+    """Prints statistics to ``<stderr>``: total packages and a break down by package
     manager.
 
     Prints something like:
 
     .. code-block:: text
 
-        16 packages total (brew: 2, pip: 2, apm: 2, gem: 2, cask: 2, mas: 2, vscode: 2, npm: 2, composer: 0).
+        16 packages total (brew: 2, pip: 2, gem: 2, cask: 2, mas: 2, vscode: 2, npm: 2, composer: 0).
     """
     per_manager_totals = ""
     if manager_stats:
         per_manager_totals = (
             f" ({', '.join(f'{k}: {v}' for k, v in manager_stats.most_common())})"
         )
     if sys.version_info >= (3, 10):
         total = manager_stats.total()
     else:
         total = sum(manager_stats.values())
     plural = "s" if total > 1 else ""
-    echo(f"{total} package{plural} total{per_manager_totals}.")
+    echo(f"{total} package{plural} total{per_manager_totals}.", err=True)
 
 
 class BarPluginRenderer(MPMPlugin):
     """All utilities used to render output compatible with both Xbar and SwiftBar plugin
     dialect.
 
     The minimal code to locate ``mpm``, then call it and print its output resides in the plugin itself at
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/pool.py` & `meta_package_manager-5.9.0/meta_package_manager/pool.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,75 +120,94 @@
 
         Returns a list of sorted items to provide consistency across all UI, and
         reproducibility in the order package managers are evaluated.
         """
         return tuple(sorted(self.register))
 
     @cached_property
+    def maintained_manager_ids(self) -> tuple[str, ...]:
+        """All manager IDs which are not deprecated."""
+        return tuple(
+            mid for mid in self.all_manager_ids if not self.register.get(mid).deprecated
+        )
+
+    @cached_property
     def default_manager_ids(self) -> tuple[str, ...]:
-        """All manager IDs supported on the current platform.
+        """All manager IDs supported on the current platform and not deprecated.
 
         Must keep the same order defined by :py:prop:`meta_package_manager.pool.ManagerPool.all_manager_ids`.
         """
         return tuple(
-            mid for mid in self.all_manager_ids if self.register.get(mid).supported
+            mid
+            for mid in self.maintained_manager_ids
+            if self.register.get(mid).supported
         )
 
     @cached_property
     def unsupported_manager_ids(self) -> tuple[str, ...]:
-        """All manager IDs unsupported on the current platform.
+        """All manager IDs unsupported on the current platform but still maintained.
 
         Order is not important here as this list will be used to discard managers from
         selection sets.
         """
         return tuple(
-            mid for mid in self.all_manager_ids if mid not in self.default_manager_ids
+            mid
+            for mid in self.maintained_manager_ids
+            if mid not in self.default_manager_ids
         )
 
     def select_managers(
         self,
-        keep: Iterable | None = None,
-        drop: Iterable | None = None,
+        keep: Iterable[str] | None = None,
+        drop: Iterable[str] | None = None,
+        keep_deprecated: bool = False,
         keep_unsupported: bool = False,
         drop_inactive: bool = True,
         implements_operation: Operations | None = None,
         **extra_options: bool,
     ) -> Iterator[PackageManager]:
         """Utility method to extract a subset of the manager pool based on selection
         list (``keep`` parameter) and exclusion list (``drop`` parameter) criterion.
 
         By default, only the managers supported by the current platform are selected. Unless
         ``keep_unsupported`` is set to ``True``, in which case all managers implemented by ``mpm``
         are selected, regardless of their supported platform.
 
+        Deprecated managers are also excluded by default, unless ``keep_deprecated`` is ``True``.
+
         ``drop_inactive`` filters out managers that where not found on the system.
 
         ``implements_operation`` filters out managers which do not implements the provided operation.
 
         Finally, ``extra_options`` parameters are fed to manager objects to set some additional options.
 
         Returns a generator producing a manager instance one after the other.
         """
-        if not keep:
-            keep = (
-                self.all_manager_ids if keep_unsupported else self.default_manager_ids
-            )
-        if not drop:
+        # Produce the default set of managers to consider if none have been
+        # provided by the ``keep`` parameter.
+        if keep is None:
+            if keep_deprecated:
+                keep = self.all_manager_ids
+            elif keep_unsupported:
+                keep = self.maintained_manager_ids
+            else:
+                keep = self.default_manager_ids
+        if drop is None:
             drop = set()
-        assert set(self.all_manager_ids).issuperset(keep)  # type: ignore
+        assert set(self.all_manager_ids).issuperset(keep)
         assert set(self.all_manager_ids).issuperset(drop)
 
         assert self.ALLOWED_EXTRA_OPTION.issuperset(extra_options)
 
-        # Only keeps the subset selected by the user.
-        selected_ids = keep
+        # Reduce the set to the user's constraints.
+        selected_ids = (mid for mid in unique(keep) if mid not in drop)
 
         # Deduplicate managers IDs while preserving order, then remove excluded
         # managers.
-        for manager_id in (mid for mid in unique(selected_ids) if mid not in drop):
+        for manager_id in selected_ids:
             manager = self.register.get(manager_id)
 
             # Check if operation is not implemented before calling `.available`. It saves one
             # call to the package manager CLI.
             if implements_operation and not manager.implements(implements_operation):
                 logger.warning(
                     f"{theme.invoked_command(manager_id)} does not implement {implements_operation}."
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/specifier.py` & `meta_package_manager-5.9.0/meta_package_manager/specifier.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/__init__.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/conftest.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_bar_plugin.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_bar_plugin.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import json
 import re
 import subprocess
 
 import pytest
 from boltons.strutils import strip_ansi
-from click_extra.tabulate import TabularOutputFormatter
+from click_extra.tabulate import output_formats
 
 from .. import __version__
 from ..bar_plugin import MPMPlugin  # type: ignore
 from ..base import Operations
 from ..pool import pool
 
 """ Common tests for all CLI basic features and templates for subcommands. """
@@ -168,15 +168,15 @@
                     re.search(
                         rf"warning: {mid} does not implement "
                         rf"Operations\.({'|'.join(Operations.__members__.keys())}).",
                         stderr,
                     )
                 ),
                 # Stats line at the end of output.
-                f"{mid}: " in stdout.splitlines()[-1] if stdout else "",
+                f"{mid}: " in stderr.splitlines()[-1] if stderr else "",
                 # Match output of managers command.
                 bool(
                     re.search(
                         rf"│\s+{mid}\s+│.+│\s+(✓|✘).+│\s+(✓|✘)",
                         stdout,
                     )
                 ),
@@ -337,15 +337,15 @@
 class CLITableTests:
 
     """Test subcommands whose output is a configurable table.
 
     A table output is also allowed to be rendered as JSON.
     """
 
-    @pytest.mark.parametrize("mode", TabularOutputFormatter._output_formats)
+    @pytest.mark.parametrize("mode", output_formats)
     def test_all_table_rendering(self, invoke, subcmd, mode):
         result = invoke("--output-format", mode, subcmd)
         assert result.exit_code == 0
 
     def test_json_output(self, invoke, subcmd):
         """JSON output is expected to be parseable if read from <stdout>.
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_backup.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_backup.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_cleanup.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_cleanup.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_install_remove.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_install_remove.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         "dnf": "usd",
         "emerge": "dev-vcs/git",
         "flatpak": "org.gnome.Dictionary",
         "gem": "markdown",
         "mas": "747648890",  # Telegram
         "npm": "raven",
         "opkg": "enigma2-hotplug",
+        "pacaur": "manjaro-hello",
         "pacman": "manjaro-hello",
         # https://aur.archlinux.org/packages/meta-package-manager
         "paru": "meta-package-manager",
         # https://pypi.org/project/meta-package-manager
         "pip": "meta-package-manager",
         # https://pypi.org/project/meta-package-manager
         "pipx": "meta-package-manager",
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_installed.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_installed.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_managers.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_managers.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_outdated.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_outdated.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_restore.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_restore.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_search.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_search.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_sync.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_cli_upgrade.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_cli_upgrade.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_docs.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_manager_homebrew.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_manager_homebrew.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,19 @@
         process = subprocess.run(
             ("brew", "cleanup", "-s", "--prune=all"),
             env=env_copy({"HOMEBREW_NO_AUTO_UPDATE": "1"}),
         )
         assert not process.stderr
         assert process.returncode == 0
 
+    def brew_uninstall(package_id):
+        process = subprocess.run(("brew", "uninstall", "--cask", "--force", package_id))
+        assert not process.stderr
+        assert process.returncode == 0
+
     def _install_cask(package_id, commit):
         packages.add(package_id)
 
         # Fetch locally the old version of the Cask's formula.
         git_checkout(package_id, commit)
         brew_cleanup()
 
@@ -99,15 +104,15 @@
         assert process.returncode == 0
         return process.stdout
 
     yield _install_cask
 
     # Remove all installed packages.
     for package_id in packages:
-        subprocess.run(("brew", "uninstall", "--cask", "--force", package_id))
+        brew_uninstall(package_id)
 
 
 @destructive
 @unless_macos
 class TestCask:
     @pytest.mark.xdist_group(name="avoid_concurrent_git_tweaks")
     def test_autoupdate_unicode_name(self, invoke, install_cask):
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_managers.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_managers.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,51 +20,65 @@
 import ast
 import inspect
 import re
 import types
 from operator import attrgetter
 from pathlib import Path, PurePath
 from string import ascii_letters, ascii_lowercase, digits
-from types import MethodType
 
 import pytest
 from boltons.iterutils import unique
 from boltons.urlutils import URL
 from click_extra.platform import OS_DEFINITIONS
+from click_extra.tests.conftest import destructive
 
 from ..base import Operations, Package, PackageManager
 from ..cli import XKCD_MANAGER_ORDER
 from ..pool import pool
 from ..version import TokenizedString
 
 """ Test the structure, data and types returned by all package managers.
 
 This test suite try to automate most of the basic reviewing work for the addition of
 new package manager definitions.
 """
 
 # Parametrization decorators.
 all_managers = pytest.mark.parametrize("manager", pool.values(), ids=attrgetter("id"))
+available_managers = pytest.mark.parametrize(
+    "manager", tuple(m for m in pool.values() if m.available), ids=attrgetter("id")
+)
+
+
+def test_xkcd_set():
+    assert len(unique(XKCD_MANAGER_ORDER)) == len(XKCD_MANAGER_ORDER)
+    assert set(pool.all_manager_ids).issuperset(XKCD_MANAGER_ORDER)
+
+
+@all_managers
+def test_deprecated(manager):
+    assert isinstance(manager.deprecated, bool)
+    if manager.deprecation_url is not None:
+        assert isinstance(manager.deprecation_url, str)
+        location = URL(manager.deprecation_url)
+        assert location
+        assert location.scheme.lower() in ("http", "https")
+        assert manager.deprecated is True
 
 
 @pytest.mark.parametrize("manager_id,manager", pool.items())
 def test_ascii_id(manager_id, manager):
     """All package manager IDs should be short ASCII strings."""
     assert manager_id
     assert isinstance(manager_id, str)
     assert manager_id.isascii()
     assert set(manager_id).issubset(ascii_lowercase + digits + "-")
     assert manager_id == manager.id
 
 
-def test_xkcd_set():
-    assert len(unique(XKCD_MANAGER_ORDER)) == len(XKCD_MANAGER_ORDER)
-    assert set(pool.all_manager_ids).issuperset(XKCD_MANAGER_ORDER)
-
-
 @all_managers
 def test_name(manager):
     """Check all managers have a name."""
     assert manager.name
     assert isinstance(manager.name, str)
     assert set(manager.name).issubset(ascii_letters + digits + "' ")
 
@@ -108,14 +122,20 @@
     for name in manager.cli_names:
         assert isinstance(name, str)
         assert name.isalnum()
         assert PurePath(name).name == name
 
 
 @all_managers
+def test_virtual(manager):
+    """Check the manager as a defined virtual property."""
+    assert isinstance(manager.virtual, bool)
+
+
+@all_managers
 def test_cli_search_path(manager):
     assert isinstance(manager.cli_search_path, tuple)
     assert len(set(manager.cli_search_path)) == len(manager.cli_search_path)
     for search_path in manager.cli_search_path:
         assert isinstance(search_path, str)
         path_obj = Path(search_path).resolve()
         assert path_obj.is_absolute()
@@ -164,20 +184,14 @@
     """
     assert isinstance(manager.version_regex, str)
     regex = re.compile(manager.version_regex)
     assert "version" in regex.groupindex
 
 
 @all_managers
-def test_virtual(manager):
-    """Check the manager as a defined virtual property."""
-    assert isinstance(manager.virtual, bool)
-
-
-@all_managers
 def test_cli_path(manager):
     if manager.cli_path is not None:
         assert isinstance(manager.cli_path, Path)
         assert manager.cli_path.is_absolute()
         assert not manager.cli_path.is_reserved()
         assert manager.cli_path.is_file()
 
@@ -204,41 +218,39 @@
 
 
 @all_managers
 def test_available(manager):
     assert isinstance(manager.available, bool)
 
 
-@all_managers
+@available_managers
 def test_installed_type(manager):
     """All installed operations are either not implemented or returns a dict of
     dicts."""
-    if manager.available:
-        try:
-            result = manager.installed
-        except Exception as ex:
-            assert isinstance(ex, NotImplementedError)
-        else:
-            assert isinstance(result, types.GeneratorType)
-            for pkg in result:
-                assert isinstance(pkg, Package)
+    try:
+        result = manager.installed
+    except Exception as ex:
+        assert isinstance(ex, NotImplementedError)
+    else:
+        assert isinstance(result, types.GeneratorType)
+        for pkg in result:
+            assert isinstance(pkg, Package)
 
 
-@all_managers
+@available_managers
 def test_outdated_type(manager):
     """All outdated operations are either not implemented or returns a dict of dicts."""
-    if manager.available:
-        try:
-            result = manager.outdated
-        except Exception as ex:
-            assert isinstance(ex, NotImplementedError)
-        else:
-            assert isinstance(result, types.GeneratorType)
-            for pkg in result:
-                assert isinstance(pkg, Package)
+    try:
+        result = manager.outdated
+    except Exception as ex:
+        assert isinstance(ex, NotImplementedError)
+    else:
+        assert isinstance(result, types.GeneratorType)
+        for pkg in result:
+            assert isinstance(pkg, Package)
 
 
 @pytest.mark.parametrize(
     "query,query_parts",
     (
         ("cli-l-cli", {"cli", "l"}),
         ("ab12--cd34", {"ab12", "cd34"}),
@@ -246,80 +258,111 @@
         ("AB ab", {"AB", "ab"}),
     ),
 )
 def test_query_parts(query, query_parts):
     assert PackageManager.query_parts(query) == query_parts
 
 
-@all_managers
+@available_managers
 def test_search_type(manager):
     """All search operations are either not implemented or returns a generator of
     dicts."""
-    assert isinstance(manager.search, MethodType)
-    if manager.available:
-        try:
-            matches = manager.search("python", extended=True, exact=False)
-        except Exception as ex:
-            assert isinstance(ex, NotImplementedError)
-        else:
-            assert isinstance(matches, types.GeneratorType)
-            for pkg in matches:
-                assert isinstance(pkg, Package)
+    try:
+        matches = manager.search("python", extended=True, exact=False)
+    except Exception as ex:
+        assert isinstance(ex, NotImplementedError)
+    else:
+        assert isinstance(matches, types.GeneratorType)
+        for pkg in matches:
+            assert isinstance(pkg, Package)
 
 
-@all_managers
-def test_upgrade_one_cli_type(manager):
-    """All methods returning an upgrade CLI are either not implemented or returns a
-    tuple."""
-    assert isinstance(manager.upgrade_one_cli, MethodType)
+@destructive
+@available_managers
+def test_install_type(manager):
+    """All methods installing packages are either not implemented or returns a
+    string."""
     try:
-        result = manager.upgrade_one_cli("dummy_package_id")
+        result = manager.install("dummy_package_id")
     except Exception as ex:
         assert isinstance(ex, NotImplementedError)
     else:
-        assert isinstance(result, tuple)
+        assert isinstance(result, str)
 
 
-@all_managers
+@destructive
+@available_managers
 def test_upgrade_all_cli_type(manager):
     """All methods returning an upgrade-all CLI are either not implemented or returns a
     tuple."""
-    assert isinstance(manager.upgrade_all_cli, MethodType)
     try:
         result = manager.upgrade_all_cli()
     except Exception as ex:
         assert isinstance(ex, NotImplementedError)
     else:
         assert isinstance(result, tuple)
 
 
-@all_managers
+@destructive
+@available_managers
+def test_upgrade_one_cli_type(manager):
+    """All methods returning an upgrade CLI are either not implemented or returns a
+    tuple."""
+    try:
+        result = manager.upgrade_one_cli("dummy_package_id")
+    except Exception as ex:
+        assert isinstance(ex, NotImplementedError)
+    else:
+        assert isinstance(result, tuple)
+
+
+@destructive
+@available_managers
+def test_upgrade_type(manager):
+    """All methods upgrading packages are either not implemented or returns a string."""
+    try:
+        result = manager.upgrade()
+    except Exception as ex:
+        assert isinstance(ex, NotImplementedError)
+    else:
+        assert isinstance(result, str)
+
+
+@destructive
+@available_managers
+def test_remove_type(manager):
+    """All methods removing packages are either not implemented or returns a string."""
+    try:
+        result = manager.remove("dummy_package_id")
+    except Exception as ex:
+        assert isinstance(ex, NotImplementedError)
+    else:
+        assert isinstance(result, str)
+
+
+@available_managers
 def test_sync_type(manager):
     """Sync operations are either not implemented or returns nothing."""
-    assert isinstance(manager.sync, MethodType)
-    if manager.available:
-        try:
-            result = manager.sync()
-        except Exception as ex:
-            assert isinstance(ex, NotImplementedError)
-        else:
-            assert result is None
+    try:
+        result = manager.sync()
+    except Exception as ex:
+        assert isinstance(ex, NotImplementedError)
+    else:
+        assert result is None
 
 
-@all_managers
+@available_managers
 def test_cleanup_type(manager):
     """Cleanup operations are either not implemented or returns nothing."""
-    assert isinstance(manager.cleanup, MethodType)
-    if manager.available:
-        try:
-            result = manager.cleanup()
-        except Exception as ex:
-            assert isinstance(ex, NotImplementedError)
-        else:
-            assert result is None
+    try:
+        result = manager.cleanup()
+    except Exception as ex:
+        assert isinstance(ex, NotImplementedError)
+    else:
+        assert result is None
 
 
 def collect_props_ref():
     """Build the canonical reference from the base class.
 
     We need to parse the AST so we can collect both attributes and naked type
     annotations.
```

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_specifier.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_specifier.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/tests/test_version.py` & `meta_package_manager-5.9.0/meta_package_manager/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/meta_package_manager/version.py` & `meta_package_manager-5.9.0/meta_package_manager/version.py`

 * *Files identical despite different names*

### Comparing `meta-package-manager-5.8.0/pyproject.toml` & `meta_package_manager-5.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "meta-package-manager"
-version = "5.8.0"
+version = "5.9.0"
 description = "🎁 wraps all package managers with an unifying CLI"
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/meta-package-manager'
 repository = 'https://github.com/kdeldycke/meta-package-manager'
 documentation = 'https://kdeldycke.github.io/meta-package-manager'
@@ -29,14 +29,15 @@
     'mac app store',
     'macos',
     'mas',
     'node',
     'npm',
     'opkg',
     'package',
+    'pacaur',
     'pacman',
     'paru',
     'php composer',
     'pip',
     'pipx',
     'plugin',
     'portage',
@@ -83,43 +84,43 @@
 
 [tool.poetry.dependencies]
 # List of python versions and their support status:
 # https://en.wikipedia.org/wiki/History_of_Python#Support
 python = "^3.7"
 boltons = "^21.0.0"
 click = "^8.1.2"
-click-extra = "^3.2.5"
+click-extra = "^3.3.1"
 packageurl-python = "^0.10.3"
-tabulate = { extras = ["widechars"], version = "^0.8.9" }
+tabulate = { extras = ["widechars"], version = "^0.9.0" }
 tomli = { version = "^2.0.1", python = "< 3.11" }
 tomli_w = "^1.0.0"
 typing-extensions = { version = "^4.3.0", python = "< 3.10" }
 xmltodict = "^0.13.0"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
 coverage = { extras = ["toml"], version = "^6.5" }
 furo = "^2022.9.29"
-mypy = "^0.982"
+mypy = "^0.991"
 myst-parser = "^0.18.0"
-pytest = "^7.1.3"
+pytest = "^7.2.0"
 # More pytest plugins at: https://docs.pytest.org/en/latest/reference/plugin_list.html
 pytest-cov = "^4.0.0"
 pytest-randomly = "^3.12.0"
-pytest-xdist = { extras = ["psutil"], version = "^2.5.0" }
+pytest-xdist = { extras = ["psutil"], version = "^3.0.2" }
 pyyaml = "^6.0"
-sphinx = "^5.2.3"
+sphinx = "^5.3.0"
 sphinx-autodoc-typehints = "^1.19.4,"
 sphinx-click = "^4.3.0"
-sphinx-copybutton = "^0.5.0"
+sphinx-copybutton = "^0.5.1"
 sphinx-design = "^0.3.0"
 sphinx-issues = "^3.0.1"
-sphinxext-opengraph = "^0.6.3"
+sphinxext-opengraph = "^0.7.2"
 types-PyYAML = "^6.0.12"
-types-tabulate = "^0.8.11"
+types-tabulate = "^0.9.0"
 types-xmltodict = "^0.13.0"
 
 [tool.poetry.scripts]
 mpm = 'meta_package_manager.cli:mpm'
 
 [tool.pylint.MASTER]
 # http://pylint.pycqa.org/en/latest/technical_reference/features.html
```

### Comparing `meta-package-manager-5.8.0/readme.md` & `meta_package_manager-5.9.0/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 [![DOI](https://zenodo.org/badge/65922807.svg)](https://zenodo.org/badge/latestdoi/65922807)
 
 **What is Meta Package Manager?**
 
 - provides the `mpm` CLI, a wrapper around all package managers
 - `mpm` is like [`yt-dlp`](https://github.com/yt-dlp/yt-dlp), but for package
   managers instead of videos
-- `mpm` solves [XKCD #1654: Universal Install Script](https://xkcd.com/1654/)
+- `mpm` solves [XKCD #1654 - *Universal Install Script*](https://xkcd.com/1654/)
 
 ______________________________________________________________________
 
 ## Features
 
 <img align="right" width="30%" height="30%" src="https://raw.githubusercontent.com/kdeldycke/meta-package-manager/main/docs/images/mpm-outdated-cli.png"/>
 
@@ -68,14 +68,15 @@
 | [`dnf`](https://github.com/rpm-software-management/dnf)                   | 4.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |
 | [`emerge`](https://wiki.gentoo.org/wiki/Portage#emerge)                   | 3.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |
 | [`flatpak`](https://flatpak.org)                                          | 1.2.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |     ✓     |
 | [`gem`](https://rubygems.org)                                             | 2.5.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |        |     ✓     |
 | [`mas`](https://github.com/argon/mas)                                     | 1.6.1        |       |   🍎   |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |
 | [`npm`](https://www.npmjs.com)                                            | 4.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |        |           |
 | [`opkg`](https://git.yoctoproject.org/cgit/cgit.cgi/opkg/)                | 0.2.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |           |
+| [`pacaur`](https://github.com/E5ten/pacaur)                               | 4.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |
 | [`pacman`](https://wiki.archlinux.org/title/pacman)                       | 5.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |
 | [`paru`](https://github.com/Morganamilo/paru)                             | 1.9.3        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |
 | [`pip`](https://pip.pypa.io)                                              | 10.0.0       |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |          |     ✓     |     ✓     |       ✓       |    ✓     |        |           |
 | [`pipx`](https://pypa.github.io/pipx/)                                    | 1.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |          |     ✓     |     ✓     |       ✓       |    ✓     |        |           |
 | [`scoop`](https://scoop.sh)                                               | 0.2.4        |       |       |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |
 | [`snap`](https://snapcraft.io)                                            | 2.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |
 | [`steamcmd`](https://developer.valvesoftware.com/wiki/SteamCMD)           | None         |   🐧   |   🍎   |    🪟    |             |            |          |     ✓     |           |               |          |        |           |
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 [![Documentation status](https://github.com/kdeldycke/meta-package-manager/
 actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/
 kdeldycke/meta-package-manager/actions/workflows/docs.yaml?query=branch%3Amain)
 [![DOI](https://zenodo.org/badge/65922807.svg)](https://zenodo.org/badge/
 latestdoi/65922807) **What is Meta Package Manager?** - provides the `mpm` CLI,
 a wrapper around all package managers - `mpm` is like [`yt-dlp`](https://
 github.com/yt-dlp/yt-dlp), but for package managers instead of videos - `mpm`
-solves [XKCD #1654: Universal Install Script](https://xkcd.com/1654/
+solves [XKCD #1654 - *Universal Install Script*](https://xkcd.com/1654/
 ) ______________________________________________________________________ ##
 Features [https://raw.githubusercontent.com/kdeldycke/meta-package-manager/
 main/docs/images/mpm-outdated-cli.png] [https://raw.githubusercontent.com/
 kdeldycke/meta-package-manager/main/docs/images/mpm-managers-cli.png] -
 Inventory and list all package managers available on the system. - Supports
 macOS, Linux and Windows. - List installed packages. - Search for packages. -
 Install a package. - Remove a package. - List outdated packages. - Sync local
@@ -58,38 +58,40 @@
 | â | â | | â | â | | [`flatpak`](https://flatpak.org) | 1.2.0 | ð§ |
 | | â | â | â | â | â | â | | | â | | [`gem`](https://
 rubygems.org) | 2.5.0 | ð§ | ð | ðª | â | â | â | â | â | â
 | â | | â | | [`mas`](https://github.com/argon/mas) | 1.6.1 | | ð | |
 â | â | â | â | â | â | | | | | [`npm`](https://www.npmjs.com) |
 4.0.0 | ð§ | ð | ðª | â | â | â | â | â | â | â | | | |
 [`opkg`](https://git.yoctoproject.org/cgit/cgit.cgi/opkg/) | 0.2.0 | ð§ | | |
-â | â | â | â | â | â | | â | | | [`pacman`](https://
-wiki.archlinux.org/title/pacman) | 5.0.0 | ð§ | | | â | â | â | â |
-â | â | â | â | â | | [`paru`](https://github.com/Morganamilo/paru) |
-1.9.3 | ð§ | | | â | â | â | â | â | â | â | â | â | |
-[`pip`](https://pip.pypa.io) | 10.0.0 | ð§ | ð | ðª | â | â | | â
-| â | â | â | | | | [`pipx`](https://pypa.github.io/pipx/) | 1.0.0 | ð§
-| ð | ðª | â | â | | â | â | â | â | | | | [`scoop`](https://
-scoop.sh) | 0.2.4 | | | ðª | â | â | â | â | â | â | â | â |
-â | | [`snap`](https://snapcraft.io) | 2.0.0 | ð§ | | | â | â | â |
-â | â | â | | | | | [`steamcmd`](https://developer.valvesoftware.com/
-wiki/SteamCMD) | None | ð§ | ð | ðª | | | | â | | | | | | | [`vscode`]
-(https://code.visualstudio.com) | 1.60.0 | ð§ | ð | ðª | â | | | â |
-| | | | | | [`yarn`](https://yarnpkg.com) | 1.20.0 | ð§ | ð | ðª | â |
-â | â | â | â | â | â | | â | | [`yay`](https://github.com/Jguer/
-yay) | 11.0.0 | ð§ | | | â | â | â | â | â | â | â | â | â
-| | [`yum`](http://yum.baseurl.org) | 4.0.0 | ð§ | | | â | â | â | â
-| â | â | | â | â | | [`zypper`](https://en.opensuse.org/Portal:Zypper)
-| 1.14.0 | ð§ | | | â | â | â | â | â | â | | â | â | ##
-Quickstart Easiest way is to install `mpm` with [`pipx`](https://
-pypa.github.io/pipx/): ```shell-session $ pipx install meta-package-manager ```
-Other [alternatives installation methods](https://kdeldycke.github.io/meta-
-package-manager/install.html) are available in the documentation. ## List
-managers List all supported package managers and their status on current system
-(macOS in this case): ```shell-session $ mpm --all-managers managers
+â | â | â | â | â | â | | â | | | [`pacaur`](https://github.com/
+E5ten/pacaur) | 4.0.0 | ð§ | | | â | â | â | â | â | â | â |
+â | â | | [`pacman`](https://wiki.archlinux.org/title/pacman) | 5.0.0 |
+ð§ | | | â | â | â | â | â | â | â | â | â | | [`paru`]
+(https://github.com/Morganamilo/paru) | 1.9.3 | ð§ | | | â | â | â |
+â | â | â | â | â | â | | [`pip`](https://pip.pypa.io) | 10.0.0 |
+ð§ | ð | ðª | â | â | | â | â | â | â | | | | [`pipx`]
+(https://pypa.github.io/pipx/) | 1.0.0 | ð§ | ð | ðª | â | â | | â
+| â | â | â | | | | [`scoop`](https://scoop.sh) | 0.2.4 | | | ðª | â
+| â | â | â | â | â | â | â | â | | [`snap`](https://
+snapcraft.io) | 2.0.0 | ð§ | | | â | â | â | â | â | â | | | | |
+[`steamcmd`](https://developer.valvesoftware.com/wiki/SteamCMD) | None | ð§ |
+ð | ðª | | | | â | | | | | | | [`vscode`](https://code.visualstudio.com)
+| 1.60.0 | ð§ | ð | ðª | â | | | â | | | | | | | [`yarn`](https://
+yarnpkg.com) | 1.20.0 | ð§ | ð | ðª | â | â | â | â | â | â
+| â | | â | | [`yay`](https://github.com/Jguer/yay) | 11.0.0 | ð§ | | |
+â | â | â | â | â | â | â | â | â | | [`yum`](http://
+yum.baseurl.org) | 4.0.0 | ð§ | | | â | â | â | â | â | â | | â
+| â | | [`zypper`](https://en.opensuse.org/Portal:Zypper) | 1.14.0 | ð§ | |
+| â | â | â | â | â | â | | â | â | ## Quickstart Easiest way
+is to install `mpm` with [`pipx`](https://pypa.github.io/pipx/): ```shell-
+session $ pipx install meta-package-manager ``` Other [alternatives
+installation methods](https://kdeldycke.github.io/meta-package-manager/
+install.html) are available in the documentation. ## List managers List all
+supported package managers and their status on current system (macOS in this
+case): ```shell-session $ mpm --all-managers managers
 â­âââââââââââââ¬âââââââââââââââââââââ¬âââââââââââââââââ¬âââââââââââââââââââââââââââââââ¬âââââââââââââ¬ââââââââââââ®
 â Manager ID â Name â Supported â CLI â Executable â Version â
 ââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââââ¼âââââââââââââââââââââââââââââââ¼âââââââââââââ¼ââââââââââââ¤
 â apm â Atom's apm â â â â apm not found â â â â apt â
 APT â â Linux only â â /usr/bin/apt â â â â â â apt-mint
 â Linux Mint's apt â â Linux only â â /usr/bin/apt â â â â
 â â brew â Homebrew Formulae â â â â /opt/homebrew/bin/brew â
```

### Comparing `meta-package-manager-5.8.0/setup.py` & `meta_package_manager-5.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,33 +8,33 @@
  'meta_package_manager.tests']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['boltons>=21.0.0,<22.0.0',
- 'click-extra>=3.2.5,<4.0.0',
+ 'click-extra>=3.3.1,<4.0.0',
  'click>=8.1.2,<9.0.0',
  'packageurl-python>=0.10.3,<0.11.0',
- 'tabulate[widechars]>=0.8.9,<0.9.0',
+ 'tabulate[widechars]>=0.9.0,<0.10.0',
  'tomli_w>=1.0.0,<2.0.0',
  'xmltodict>=0.13.0,<0.14.0']
 
 extras_require = \
 {':python_version < "3.10"': ['typing-extensions>=4.3.0,<5.0.0'],
  ':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['mpm = meta_package_manager.cli:mpm']}
 
 setup_kwargs = {
     'name': 'meta-package-manager',
-    'version': '5.8.0',
+    'version': '5.9.0',
     'description': '🎁 wraps all package managers with an unifying CLI',
-    'long_description': '<p align="center">\n  <a href="https://github.com/kdeldycke/meta-package-manager/">\n    <img src="https://raw.githubusercontent.com/kdeldycke/meta-package-manager/main/docs/images/logo-banner.svg" alt="Meta Package Manager">\n  </a>\n</p>\n\n<a href="https://xkcd.com/1654/" alt="XKCD #1654: Universal Install Script">\n<img align="right" width="20%" height="20%" src="http://imgs.xkcd.com/comics/universal_install_script.png"/>\n</a>\n\n[![Last release](https://img.shields.io/pypi/v/meta-package-manager.svg)](https://pypi.python.org/pypi/meta-package-manager)\n[![Python versions](https://img.shields.io/pypi/pyversions/meta-package-manager.svg)](https://pypi.python.org/pypi/meta-package-manager)\n[![Type checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Unittests status](https://github.com/kdeldycke/meta-package-manager/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/meta-package-manager/actions/workflows/tests.yaml?query=branch%3Amain)\n[![Coverage status](https://codecov.io/gh/kdeldycke/meta-package-manager/branch/main/graph/badge.svg)](https://codecov.io/gh/kdeldycke/meta-package-manager/branch/main)\n[![Documentation status](https://github.com/kdeldycke/meta-package-manager/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/meta-package-manager/actions/workflows/docs.yaml?query=branch%3Amain)\n[![DOI](https://zenodo.org/badge/65922807.svg)](https://zenodo.org/badge/latestdoi/65922807)\n\n**What is Meta Package Manager?**\n\n- provides the `mpm` CLI, a wrapper around all package managers\n- `mpm` is like [`yt-dlp`](https://github.com/yt-dlp/yt-dlp), but for package\n  managers instead of videos\n- `mpm` solves [XKCD #1654: Universal Install Script](https://xkcd.com/1654/)\n\n______________________________________________________________________\n\n## Features\n\n<img align="right" width="30%" height="30%" src="https://raw.githubusercontent.com/kdeldycke/meta-package-manager/main/docs/images/mpm-outdated-cli.png"/>\n\n<img align="right" width="30%" height="30%" src="https://raw.githubusercontent.com/kdeldycke/meta-package-manager/main/docs/images/mpm-managers-cli.png"/>\n\n- Inventory and list all package managers available on the system.\n- Supports macOS, Linux and Windows.\n- List installed packages.\n- Search for packages.\n- Install a package.\n- Remove a package.\n- List outdated packages.\n- Sync local package infos.\n- Upgrade all outdated packages.\n- Backup list of installed packages to TOML file.\n- Restore/install list of packages from TOML files.\n- Pin-point commands to a subset of package managers (include/exclude\n  selectors).\n- Support plain, versionned and [purl](https://github.com/package-url/purl-spec) package specifiers.\n- Export output to JSON or print user-friendly tables.\n- Shell auto-completion for Bash, Zsh and Fish.\n- Provides a\n  [Xbar/SwiftBar plugin](https://kdeldycke.github.io/meta-package-manager/bar-plugin.html) for\n  friendly macOS integration.\n- Because `mpm` try to wrap all other package managers, it became another\n  pathological case of [XKCD #927: Standards](https://xkcd.com/927/)\n\n## Supported package managers and operations\n\n| Package manager                                                           | Min. version | Linux | macOS | Windows | `installed` | `outdated` | `search` | `install` | `upgrade` | `upgrade_all` | `remove` | `sync` | `cleanup` |\n| ------------------------------------------------------------------------- | ------------ | :---: | :---: | :-----: | :---------: | :--------: | :------: | :-------: | :-------: | :-----------: | :------: | :----: | :-------: |\n| [`apm`](https://atom.io/packages)                                         | 1.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |\n| [`apt`](https://wiki.debian.org/AptCLI)                                   | 1.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n| [`apt-mint`](https://github.com/kdeldycke/meta-package-manager/issues/52) | 1.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n| [`brew`](https://brew.sh)                                                 | 2.7.0        |   🐧   |   🍎   |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`cargo`](https://doc.rust-lang.org/cargo/)                               | 1.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |            |    ✓     |     ✓     |           |               |    ✓     |        |           |\n| [`cask`](https://caskroom.github.io)                                      | 2.7.0        |       |   🍎   |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`choco`](https://chocolatey.org)                                         | 0.10.4       |       |       |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |\n| [`composer`](https://getcomposer.org)                                     | 1.4.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |     ✓     |\n| [`dnf`](https://github.com/rpm-software-management/dnf)                   | 4.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n| [`emerge`](https://wiki.gentoo.org/wiki/Portage#emerge)                   | 3.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n| [`flatpak`](https://flatpak.org)                                          | 1.2.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |     ✓     |\n| [`gem`](https://rubygems.org)                                             | 2.5.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |        |     ✓     |\n| [`mas`](https://github.com/argon/mas)                                     | 1.6.1        |       |   🍎   |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |\n| [`npm`](https://www.npmjs.com)                                            | 4.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |        |           |\n| [`opkg`](https://git.yoctoproject.org/cgit/cgit.cgi/opkg/)                | 0.2.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |           |\n| [`pacman`](https://wiki.archlinux.org/title/pacman)                       | 5.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`paru`](https://github.com/Morganamilo/paru)                             | 1.9.3        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`pip`](https://pip.pypa.io)                                              | 10.0.0       |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |          |     ✓     |     ✓     |       ✓       |    ✓     |        |           |\n| [`pipx`](https://pypa.github.io/pipx/)                                    | 1.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |          |     ✓     |     ✓     |       ✓       |    ✓     |        |           |\n| [`scoop`](https://scoop.sh)                                               | 0.2.4        |       |       |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`snap`](https://snapcraft.io)                                            | 2.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |\n| [`steamcmd`](https://developer.valvesoftware.com/wiki/SteamCMD)           | None         |   🐧   |   🍎   |    🪟    |             |            |          |     ✓     |           |               |          |        |           |\n| [`vscode`](https://code.visualstudio.com)                                 | 1.60.0       |   🐧   |   🍎   |    🪟    |      ✓      |            |          |     ✓     |           |               |          |        |           |\n| [`yarn`](https://yarnpkg.com)                                             | 1.20.0       |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |        |     ✓     |\n| [`yay`](https://github.com/Jguer/yay)                                     | 11.0.0       |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`yum`](http://yum.baseurl.org)                                           | 4.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n| [`zypper`](https://en.opensuse.org/Portal:Zypper)                         | 1.14.0       |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n\n## Quickstart\n\nEasiest way is to install `mpm` with [`pipx`](https://pypa.github.io/pipx/):\n\n```shell-session\n$ pipx install meta-package-manager\n```\n\nOther\n[alternatives installation methods](https://kdeldycke.github.io/meta-package-manager/install.html)\nare available in the documentation.\n\n## List managers\n\nList all supported package managers and their status on current system (macOS\nin this case):\n\n```shell-session\n$ mpm --all-managers managers\n╭────────────┬────────────────────┬────────────────┬──────────────────────────────┬────────────┬───────────╮\n│ Manager ID │ Name               │ Supported      │ CLI                          │ Executable │ Version   │\n├────────────┼────────────────────┼────────────────┼──────────────────────────────┼────────────┼───────────┤\n│ apm        │ Atom\'s apm         │ ✓              │ ✘ apm not found              │            │           │\n│ apt        │ APT                │ ✘ Linux only   │ ✓ /usr/bin/apt               │ ✓          │ ✘         │\n│ apt-mint   │ Linux Mint\'s apt   │ ✘ Linux only   │ ✓ /usr/bin/apt               │ ✓          │ ✘         │\n│ brew       │ Homebrew Formulae  │ ✓              │ ✓ /opt/homebrew/bin/brew     │ ✓          │ ✓ 3.6.3   │\n│ cargo      │ Rust\'s cargo       │ ✓              │ ✓ /opt/homebrew/bin/cargo    │ ✓          │ ✓ 1.64.0  │\n│ cask       │ Homebrew Cask      │ ✓              │ ✓ /opt/homebrew/bin/brew     │ ✓          │ ✓ 3.6.3   │\n│ choco      │ Chocolatey         │ ✘ Windows only │ ✘ choco not found            │            │           │\n│ composer   │ PHP\'s Composer     │ ✓              │ ✓ /opt/homebrew/bin/composer │ ✓          │ ✓ 2.4.2   │\n│ dnf        │ DNF                │ ✘ Linux only   │ ✘ dnf not found              │            │           │\n│ emerge     │ Emerge             │ ✘ Linux only   │ ✘ emerge not found           │            │           │\n│ flatpak    │ Flatpak            │ ✘ Linux only   │ ✘ flatpak not found          │            │           │\n│ gem        │ Ruby Gems          │ ✓              │ ✓ /usr/bin/gem               │ ✓          │ ✓ 3.0.3.1 │\n│ mas        │ Mac AppStore       │ ✓              │ ✓ /opt/homebrew/bin/mas      │ ✓          │ ✓ 1.8.6   │\n│ npm        │ Node\'s npm         │ ✓              │ ✓ /opt/homebrew/bin/npm      │ ✓          │ ✓ 8.19.2  │\n│ opkg       │ OPKG               │ ✘ Linux only   │ ✘ opkg not found             │            │           │\n│ pacman     │ Pacman             │ ✘ Linux only   │ ✘ pacman not found           │            │           │\n│ paru       │ Paru               │ ✘ Linux only   │ ✘ paru not found             │            │           │\n│ pip        │ Pip                │ ✓              │ ✓ ~/.pyenv/shims/python3     │ ✓          │ ✓ 22.2.2  │\n│ pipx       │ Pipx               │ ✓              │ ✓ /opt/homebrew/bin/pipx     │ ✓          │ ✓ 1.1.0   │\n│ scoop      │ Scoop              │ ✘ Windows only │ ✘ scoop not found            │            │           │\n│ snap       │ Snap               │ ✘ Linux only   │ ✘ snap not found             │            │           │\n│ steamcmd   │ Valve Steam        │ ✓              │ ✘ steamcmd not found         │            │           │\n│ vscode     │ Visual Studio Code │ ✓              │ ✓ /opt/homebrew/bin/code     │ ✓          │ ✓ 1.71.2  │\n│ yarn       │ Node\'s yarn        │ ✓              │ ✓ /opt/homebrew/bin/yarn     │ ✓          │ ✓ 1.22.19 │\n│ yay        │ Yay                │ ✘ Linux only   │ ✘ yay not found              │            │           │\n│ yum        │ YUM                │ ✘ Linux only   │ ✘ yum not found              │            │           │\n│ zypper     │ Zypper             │ ✘ Linux only   │ ✘ zypper not found           │            │           │\n╰────────────┴────────────────────┴────────────────┴──────────────────────────────┴────────────┴───────────╯\n```\n\nIf your favorite manager is not supported yet, you can help! See the [contibution guide](https://kdeldycke.github.io/meta-package-manager/contributing.html).\n\n## List installed packages\n\nList all packages installed on current system:\n\n```shell-session\n$ mpm installed\n╭─────────────────────────────┬─────────────────────────────┬─────────┬────────────────────╮\n│ Package name                │ ID                          │ Manager │ Installed version  │\n├─────────────────────────────┼─────────────────────────────┼─────────┼────────────────────┤\n│ github                      │ github                      │ apm     │ 0.36.9             │\n│ update-package-dependencies │ update-package-dependencies │ apm     │ 0.13.1             │\n│ rust                        │ rust                        │ brew    │ 1.55.0             │\n│ x264                        │ x264                        │ brew    │ r3060              │\n│ atom                        │ atom                        │ cask    │ 1.58.0             │\n│ visual-studio-code          │ visual-studio-code          │ cask    │ 1.52.0             │\n│ nokogiri                    │ nokogiri                    │ gem     │ x86_64-darwin      │\n│ rake                        │ rake                        │ gem     │ 13.0.3             │\n│ iMovie                      │ 408981434                   │ mas     │ 10.2.5             │\n│ Telegram                    │ 747648890                   │ mas     │ 8.1                │\n│ npm                         │ npm                         │ npm     │ 7.24.0             │\n│ raven                       │ raven                       │ npm     │ 2.6.4              │\n│ jupyterlab                  │ jupyterlab                  │ pip     │ 3.1.14             │\n│ Sphinx                      │ Sphinx                      │ pip     │ 4.2.0              │\n│ ms-python.python            │ ms-python.python            │ vscode  │ 2021.10.1317843341 │\n│ ms-toolsai.jupyter          │ ms-toolsai.jupyter          │ vscode  │ 2021.9.1001312534  │\n╰─────────────────────────────┴─────────────────────────────┴─────────┴────────────────────╯\n16 packages total (brew: 2, pip: 2, apm: 2, gem: 2, cask: 2, mas: 2, vscode: 2, npm: 2, composer: 0).\n```\n\n## List outdated packages\n\nList all packages installed for which an upgrade is available:\n\n```shell-session\n$ mpm outdated\n╭──────────────┬─────────────┬─────────┬───────────────────┬────────────────╮\n│ Package name │ ID          │ Manager │ Installed version │ Latest version │\n├──────────────┼─────────────┼─────────┼───────────────────┼────────────────┤\n│ curl         │ curl        │ brew    │ 7.79.1            │ 7.79.1_1       │\n│ git          │ git         │ brew    │ 2.33.0            │ 2.33.0_1       │\n│ openssl@1.1  │ openssl@1.1 │ brew    │ 1.1.1l            │ 1.1.1l_1       │\n│ rake         │ rake        │ gem     │ 13.0.3            │ 13.0.6         │\n│ Telegram     │ 747648890   │ mas     │ 8.1               │ 8.1.3          │\n│ npm          │ npm@8.0.0   │ npm     │ 7.24.0            │ 8.0.0          │\n│ pip          │ pip         │ pip     │ 21.2.4            │ 21.3           │\n│ regex        │ regex       │ pip     │ 2021.9.30         │ 2021.10.8      │\n╰──────────────┴─────────────┴─────────┴───────────────────┴────────────────╯\n8 packages total (brew: 3, pip: 2, gem: 1, mas: 1, npm: 1, apm: 0, cask: 0, composer: 0).\n```\n\n## Usage\n\nMore documentation is available in:\n\n- the\n  [detailed help screens](https://kdeldycke.github.io/meta-package-manager/cli-help.html)\n- the\n  [list of use-cases](https://kdeldycke.github.io/meta-package-manager/usecase.html)\n  where you’ll find inspiration on how to leverage `mpm` power\n',
+    'long_description': '<p align="center">\n  <a href="https://github.com/kdeldycke/meta-package-manager/">\n    <img src="https://raw.githubusercontent.com/kdeldycke/meta-package-manager/main/docs/images/logo-banner.svg" alt="Meta Package Manager">\n  </a>\n</p>\n\n<a href="https://xkcd.com/1654/" alt="XKCD #1654: Universal Install Script">\n<img align="right" width="20%" height="20%" src="http://imgs.xkcd.com/comics/universal_install_script.png"/>\n</a>\n\n[![Last release](https://img.shields.io/pypi/v/meta-package-manager.svg)](https://pypi.python.org/pypi/meta-package-manager)\n[![Python versions](https://img.shields.io/pypi/pyversions/meta-package-manager.svg)](https://pypi.python.org/pypi/meta-package-manager)\n[![Type checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Unittests status](https://github.com/kdeldycke/meta-package-manager/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/meta-package-manager/actions/workflows/tests.yaml?query=branch%3Amain)\n[![Coverage status](https://codecov.io/gh/kdeldycke/meta-package-manager/branch/main/graph/badge.svg)](https://codecov.io/gh/kdeldycke/meta-package-manager/branch/main)\n[![Documentation status](https://github.com/kdeldycke/meta-package-manager/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/meta-package-manager/actions/workflows/docs.yaml?query=branch%3Amain)\n[![DOI](https://zenodo.org/badge/65922807.svg)](https://zenodo.org/badge/latestdoi/65922807)\n\n**What is Meta Package Manager?**\n\n- provides the `mpm` CLI, a wrapper around all package managers\n- `mpm` is like [`yt-dlp`](https://github.com/yt-dlp/yt-dlp), but for package\n  managers instead of videos\n- `mpm` solves [XKCD #1654 - *Universal Install Script*](https://xkcd.com/1654/)\n\n______________________________________________________________________\n\n## Features\n\n<img align="right" width="30%" height="30%" src="https://raw.githubusercontent.com/kdeldycke/meta-package-manager/main/docs/images/mpm-outdated-cli.png"/>\n\n<img align="right" width="30%" height="30%" src="https://raw.githubusercontent.com/kdeldycke/meta-package-manager/main/docs/images/mpm-managers-cli.png"/>\n\n- Inventory and list all package managers available on the system.\n- Supports macOS, Linux and Windows.\n- List installed packages.\n- Search for packages.\n- Install a package.\n- Remove a package.\n- List outdated packages.\n- Sync local package infos.\n- Upgrade all outdated packages.\n- Backup list of installed packages to TOML file.\n- Restore/install list of packages from TOML files.\n- Pin-point commands to a subset of package managers (include/exclude\n  selectors).\n- Support plain, versionned and [purl](https://github.com/package-url/purl-spec) package specifiers.\n- Export output to JSON or print user-friendly tables.\n- Shell auto-completion for Bash, Zsh and Fish.\n- Provides a\n  [Xbar/SwiftBar plugin](https://kdeldycke.github.io/meta-package-manager/bar-plugin.html) for\n  friendly macOS integration.\n- Because `mpm` try to wrap all other package managers, it became another\n  pathological case of [XKCD #927: Standards](https://xkcd.com/927/)\n\n## Supported package managers and operations\n\n| Package manager                                                           | Min. version | Linux | macOS | Windows | `installed` | `outdated` | `search` | `install` | `upgrade` | `upgrade_all` | `remove` | `sync` | `cleanup` |\n| ------------------------------------------------------------------------- | ------------ | :---: | :---: | :-----: | :---------: | :--------: | :------: | :-------: | :-------: | :-----------: | :------: | :----: | :-------: |\n| [`apm`](https://atom.io/packages)                                         | 1.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |\n| [`apt`](https://wiki.debian.org/AptCLI)                                   | 1.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n| [`apt-mint`](https://github.com/kdeldycke/meta-package-manager/issues/52) | 1.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n| [`brew`](https://brew.sh)                                                 | 2.7.0        |   🐧   |   🍎   |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`cargo`](https://doc.rust-lang.org/cargo/)                               | 1.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |            |    ✓     |     ✓     |           |               |    ✓     |        |           |\n| [`cask`](https://caskroom.github.io)                                      | 2.7.0        |       |   🍎   |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`choco`](https://chocolatey.org)                                         | 0.10.4       |       |       |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |\n| [`composer`](https://getcomposer.org)                                     | 1.4.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |     ✓     |\n| [`dnf`](https://github.com/rpm-software-management/dnf)                   | 4.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n| [`emerge`](https://wiki.gentoo.org/wiki/Portage#emerge)                   | 3.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n| [`flatpak`](https://flatpak.org)                                          | 1.2.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |     ✓     |\n| [`gem`](https://rubygems.org)                                             | 2.5.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |        |     ✓     |\n| [`mas`](https://github.com/argon/mas)                                     | 1.6.1        |       |   🍎   |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |\n| [`npm`](https://www.npmjs.com)                                            | 4.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |        |           |\n| [`opkg`](https://git.yoctoproject.org/cgit/cgit.cgi/opkg/)                | 0.2.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |           |\n| [`pacaur`](https://github.com/E5ten/pacaur)                               | 4.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`pacman`](https://wiki.archlinux.org/title/pacman)                       | 5.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`paru`](https://github.com/Morganamilo/paru)                             | 1.9.3        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`pip`](https://pip.pypa.io)                                              | 10.0.0       |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |          |     ✓     |     ✓     |       ✓       |    ✓     |        |           |\n| [`pipx`](https://pypa.github.io/pipx/)                                    | 1.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |          |     ✓     |     ✓     |       ✓       |    ✓     |        |           |\n| [`scoop`](https://scoop.sh)                                               | 0.2.4        |       |       |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`snap`](https://snapcraft.io)                                            | 2.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |\n| [`steamcmd`](https://developer.valvesoftware.com/wiki/SteamCMD)           | None         |   🐧   |   🍎   |    🪟    |             |            |          |     ✓     |           |               |          |        |           |\n| [`vscode`](https://code.visualstudio.com)                                 | 1.60.0       |   🐧   |   🍎   |    🪟    |      ✓      |            |          |     ✓     |           |               |          |        |           |\n| [`yarn`](https://yarnpkg.com)                                             | 1.20.0       |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |        |     ✓     |\n| [`yay`](https://github.com/Jguer/yay)                                     | 11.0.0       |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |\n| [`yum`](http://yum.baseurl.org)                                           | 4.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n| [`zypper`](https://en.opensuse.org/Portal:Zypper)                         | 1.14.0       |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |\n\n## Quickstart\n\nEasiest way is to install `mpm` with [`pipx`](https://pypa.github.io/pipx/):\n\n```shell-session\n$ pipx install meta-package-manager\n```\n\nOther\n[alternatives installation methods](https://kdeldycke.github.io/meta-package-manager/install.html)\nare available in the documentation.\n\n## List managers\n\nList all supported package managers and their status on current system (macOS\nin this case):\n\n```shell-session\n$ mpm --all-managers managers\n╭────────────┬────────────────────┬────────────────┬──────────────────────────────┬────────────┬───────────╮\n│ Manager ID │ Name               │ Supported      │ CLI                          │ Executable │ Version   │\n├────────────┼────────────────────┼────────────────┼──────────────────────────────┼────────────┼───────────┤\n│ apm        │ Atom\'s apm         │ ✓              │ ✘ apm not found              │            │           │\n│ apt        │ APT                │ ✘ Linux only   │ ✓ /usr/bin/apt               │ ✓          │ ✘         │\n│ apt-mint   │ Linux Mint\'s apt   │ ✘ Linux only   │ ✓ /usr/bin/apt               │ ✓          │ ✘         │\n│ brew       │ Homebrew Formulae  │ ✓              │ ✓ /opt/homebrew/bin/brew     │ ✓          │ ✓ 3.6.3   │\n│ cargo      │ Rust\'s cargo       │ ✓              │ ✓ /opt/homebrew/bin/cargo    │ ✓          │ ✓ 1.64.0  │\n│ cask       │ Homebrew Cask      │ ✓              │ ✓ /opt/homebrew/bin/brew     │ ✓          │ ✓ 3.6.3   │\n│ choco      │ Chocolatey         │ ✘ Windows only │ ✘ choco not found            │            │           │\n│ composer   │ PHP\'s Composer     │ ✓              │ ✓ /opt/homebrew/bin/composer │ ✓          │ ✓ 2.4.2   │\n│ dnf        │ DNF                │ ✘ Linux only   │ ✘ dnf not found              │            │           │\n│ emerge     │ Emerge             │ ✘ Linux only   │ ✘ emerge not found           │            │           │\n│ flatpak    │ Flatpak            │ ✘ Linux only   │ ✘ flatpak not found          │            │           │\n│ gem        │ Ruby Gems          │ ✓              │ ✓ /usr/bin/gem               │ ✓          │ ✓ 3.0.3.1 │\n│ mas        │ Mac AppStore       │ ✓              │ ✓ /opt/homebrew/bin/mas      │ ✓          │ ✓ 1.8.6   │\n│ npm        │ Node\'s npm         │ ✓              │ ✓ /opt/homebrew/bin/npm      │ ✓          │ ✓ 8.19.2  │\n│ opkg       │ OPKG               │ ✘ Linux only   │ ✘ opkg not found             │            │           │\n│ pacman     │ Pacman             │ ✘ Linux only   │ ✘ pacman not found           │            │           │\n│ paru       │ Paru               │ ✘ Linux only   │ ✘ paru not found             │            │           │\n│ pip        │ Pip                │ ✓              │ ✓ ~/.pyenv/shims/python3     │ ✓          │ ✓ 22.2.2  │\n│ pipx       │ Pipx               │ ✓              │ ✓ /opt/homebrew/bin/pipx     │ ✓          │ ✓ 1.1.0   │\n│ scoop      │ Scoop              │ ✘ Windows only │ ✘ scoop not found            │            │           │\n│ snap       │ Snap               │ ✘ Linux only   │ ✘ snap not found             │            │           │\n│ steamcmd   │ Valve Steam        │ ✓              │ ✘ steamcmd not found         │            │           │\n│ vscode     │ Visual Studio Code │ ✓              │ ✓ /opt/homebrew/bin/code     │ ✓          │ ✓ 1.71.2  │\n│ yarn       │ Node\'s yarn        │ ✓              │ ✓ /opt/homebrew/bin/yarn     │ ✓          │ ✓ 1.22.19 │\n│ yay        │ Yay                │ ✘ Linux only   │ ✘ yay not found              │            │           │\n│ yum        │ YUM                │ ✘ Linux only   │ ✘ yum not found              │            │           │\n│ zypper     │ Zypper             │ ✘ Linux only   │ ✘ zypper not found           │            │           │\n╰────────────┴────────────────────┴────────────────┴──────────────────────────────┴────────────┴───────────╯\n```\n\nIf your favorite manager is not supported yet, you can help! See the [contibution guide](https://kdeldycke.github.io/meta-package-manager/contributing.html).\n\n## List installed packages\n\nList all packages installed on current system:\n\n```shell-session\n$ mpm installed\n╭─────────────────────────────┬─────────────────────────────┬─────────┬────────────────────╮\n│ Package name                │ ID                          │ Manager │ Installed version  │\n├─────────────────────────────┼─────────────────────────────┼─────────┼────────────────────┤\n│ github                      │ github                      │ apm     │ 0.36.9             │\n│ update-package-dependencies │ update-package-dependencies │ apm     │ 0.13.1             │\n│ rust                        │ rust                        │ brew    │ 1.55.0             │\n│ x264                        │ x264                        │ brew    │ r3060              │\n│ atom                        │ atom                        │ cask    │ 1.58.0             │\n│ visual-studio-code          │ visual-studio-code          │ cask    │ 1.52.0             │\n│ nokogiri                    │ nokogiri                    │ gem     │ x86_64-darwin      │\n│ rake                        │ rake                        │ gem     │ 13.0.3             │\n│ iMovie                      │ 408981434                   │ mas     │ 10.2.5             │\n│ Telegram                    │ 747648890                   │ mas     │ 8.1                │\n│ npm                         │ npm                         │ npm     │ 7.24.0             │\n│ raven                       │ raven                       │ npm     │ 2.6.4              │\n│ jupyterlab                  │ jupyterlab                  │ pip     │ 3.1.14             │\n│ Sphinx                      │ Sphinx                      │ pip     │ 4.2.0              │\n│ ms-python.python            │ ms-python.python            │ vscode  │ 2021.10.1317843341 │\n│ ms-toolsai.jupyter          │ ms-toolsai.jupyter          │ vscode  │ 2021.9.1001312534  │\n╰─────────────────────────────┴─────────────────────────────┴─────────┴────────────────────╯\n16 packages total (brew: 2, pip: 2, apm: 2, gem: 2, cask: 2, mas: 2, vscode: 2, npm: 2, composer: 0).\n```\n\n## List outdated packages\n\nList all packages installed for which an upgrade is available:\n\n```shell-session\n$ mpm outdated\n╭──────────────┬─────────────┬─────────┬───────────────────┬────────────────╮\n│ Package name │ ID          │ Manager │ Installed version │ Latest version │\n├──────────────┼─────────────┼─────────┼───────────────────┼────────────────┤\n│ curl         │ curl        │ brew    │ 7.79.1            │ 7.79.1_1       │\n│ git          │ git         │ brew    │ 2.33.0            │ 2.33.0_1       │\n│ openssl@1.1  │ openssl@1.1 │ brew    │ 1.1.1l            │ 1.1.1l_1       │\n│ rake         │ rake        │ gem     │ 13.0.3            │ 13.0.6         │\n│ Telegram     │ 747648890   │ mas     │ 8.1               │ 8.1.3          │\n│ npm          │ npm@8.0.0   │ npm     │ 7.24.0            │ 8.0.0          │\n│ pip          │ pip         │ pip     │ 21.2.4            │ 21.3           │\n│ regex        │ regex       │ pip     │ 2021.9.30         │ 2021.10.8      │\n╰──────────────┴─────────────┴─────────┴───────────────────┴────────────────╯\n8 packages total (brew: 3, pip: 2, gem: 1, mas: 1, npm: 1, apm: 0, cask: 0, composer: 0).\n```\n\n## Usage\n\nMore documentation is available in:\n\n- the\n  [detailed help screens](https://kdeldycke.github.io/meta-package-manager/cli-help.html)\n- the\n  [list of use-cases](https://kdeldycke.github.io/meta-package-manager/usecase.html)\n  where you’ll find inspiration on how to leverage `mpm` power\n',
     'author': 'Kevin Deldycke',
     'author_email': 'kevin@deldycke.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kdeldycke/meta-package-manager',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['meta_package_manager', 'meta_package_manager.bar_plugin',
 'meta_package_manager.managers', 'meta_package_manager.tests'] package_data = \
 {'': ['*']} install_requires = \ ['boltons>=21.0.0,<22.0.0', 'click-
-extra>=3.2.5,<4.0.0', 'click>=8.1.2,<9.0.0', 'packageurl-
-python>=0.10.3,<0.11.0', 'tabulate[widechars]>=0.8.9,<0.9.0',
+extra>=3.3.1,<4.0.0', 'click>=8.1.2,<9.0.0', 'packageurl-
+python>=0.10.3,<0.11.0', 'tabulate[widechars]>=0.9.0,<0.10.0',
 'tomli_w>=1.0.0,<2.0.0', 'xmltodict>=0.13.0,<0.14.0'] extras_require = \ {':
 python_version < "3.10"': ['typing-extensions>=4.3.0,<5.0.0'], ':python_version
 < "3.11"': ['tomli>=2.0.1,<3.0.0']} entry_points = \ {'console_scripts': ['mpm
 = meta_package_manager.cli:mpm']} setup_kwargs = { 'name': 'meta-package-
-manager', 'version': '5.8.0', 'description': 'ð wraps all package managers
+manager', 'version': '5.9.0', 'description': 'ð wraps all package managers
 with an unifying CLI', 'long_description': '
                        \n \n_[Meta_Package_Manager]\n\n
 \n\n\n[http://imgs.xkcd.com/comics/universal_install_script.png]\n\n\n[![Last
 release](https://img.shields.io/pypi/v/meta-package-manager.svg)](https://
 pypi.python.org/pypi/meta-package-manager)\n[![Python versions](https://
 img.shields.io/pypi/pyversions/meta-package-manager.svg)](https://
 pypi.python.org/pypi/meta-package-manager)\n[![Type checked with mypy](http://
@@ -25,16 +25,16 @@
 [![Documentation status](https://github.com/kdeldycke/meta-package-manager/
 actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/
 kdeldycke/meta-package-manager/actions/workflows/
 docs.yaml?query=branch%3Amain)\n[![DOI](https://zenodo.org/badge/65922807.svg)]
 (https://zenodo.org/badge/latestdoi/65922807)\n\n**What is Meta Package
 Manager?**\n\n- provides the `mpm` CLI, a wrapper around all package
 managers\n- `mpm` is like [`yt-dlp`](https://github.com/yt-dlp/yt-dlp), but for
-package\n managers instead of videos\n- `mpm` solves [XKCD #1654: Universal
-Install Script](https://xkcd.com/1654/
+package\n managers instead of videos\n- `mpm` solves [XKCD #1654 - *Universal
+Install Script*](https://xkcd.com/1654/
 )\n\n______________________________________________________________________\n\n##
 Features\n\n[https://raw.githubusercontent.com/kdeldycke/meta-package-manager/
 main/docs/images/mpm-outdated-cli.png]\n\n[https://raw.githubusercontent.com/
 kdeldycke/meta-package-manager/main/docs/images/mpm-managers-cli.png]\n\n-
 Inventory and list all package managers available on the system.\n- Supports
 macOS, Linux and Windows.\n- List installed packages.\n- Search for
 packages.\n- Install a package.\n- Remove a package.\n- List outdated
@@ -72,39 +72,40 @@
 [`flatpak`](https://flatpak.org) | 1.2.0 | ð§ | | | â | â | â | â |
 â | â | | | â |\n| [`gem`](https://rubygems.org) | 2.5.0 | ð§ | ð |
 ðª | â | â | â | â | â | â | â | | â |\n| [`mas`](https://
 github.com/argon/mas) | 1.6.1 | | ð | | â | â | â | â | â | â |
 | | |\n| [`npm`](https://www.npmjs.com) | 4.0.0 | ð§ | ð | ðª | â |
 â | â | â | â | â | â | | |\n| [`opkg`](https://
 git.yoctoproject.org/cgit/cgit.cgi/opkg/) | 0.2.0 | ð§ | | | â | â | â
-| â | â | â | | â | |\n| [`pacman`](https://wiki.archlinux.org/title/
-pacman) | 5.0.0 | ð§ | | | â | â | â | â | â | â | â | â |
-â |\n| [`paru`](https://github.com/Morganamilo/paru) | 1.9.3 | ð§ | | | â
-| â | â | â | â | â | â | â | â |\n| [`pip`](https://
-pip.pypa.io) | 10.0.0 | ð§ | ð | ðª | â | â | | â | â | â |
-â | | |\n| [`pipx`](https://pypa.github.io/pipx/) | 1.0.0 | ð§ | ð |
-ðª | â | â | | â | â | â | â | | |\n| [`scoop`](https://scoop.sh)
-| 0.2.4 | | | ðª | â | â | â | â | â | â | â | â | â |\n|
-[`snap`](https://snapcraft.io) | 2.0.0 | ð§ | | | â | â | â | â | â
-| â | | | |\n| [`steamcmd`](https://developer.valvesoftware.com/wiki/
-SteamCMD) | None | ð§ | ð | ðª | | | | â | | | | | |\n| [`vscode`]
-(https://code.visualstudio.com) | 1.60.0 | ð§ | ð | ðª | â | | | â |
-| | | | |\n| [`yarn`](https://yarnpkg.com) | 1.20.0 | ð§ | ð | ðª | â
-| â | â | â | â | â | â | | â |\n| [`yay`](https://github.com/
-Jguer/yay) | 11.0.0 | ð§ | | | â | â | â | â | â | â | â | â
-| â |\n| [`yum`](http://yum.baseurl.org) | 4.0.0 | ð§ | | | â | â | â
-| â | â | â | | â | â |\n| [`zypper`](https://en.opensuse.org/Portal:
-Zypper) | 1.14.0 | ð§ | | | â | â | â | â | â | â | | â | â
-|\n\n## Quickstart\n\nEasiest way is to install `mpm` with [`pipx`](https://
-pypa.github.io/pipx/):\n\n```shell-session\n$ pipx install meta-package-
-manager\n```\n\nOther\n[alternatives installation methods](https://
-kdeldycke.github.io/meta-package-manager/install.html)\nare available in the
-documentation.\n\n## List managers\n\nList all supported package managers and
-their status on current system (macOS\nin this case):\n\n```shell-session\n$
-mpm --all-managers
+| â | â | â | | â | |\n| [`pacaur`](https://github.com/E5ten/pacaur) |
+4.0.0 | ð§ | | | â | â | â | â | â | â | â | â | â |\n|
+[`pacman`](https://wiki.archlinux.org/title/pacman) | 5.0.0 | ð§ | | | â |
+â | â | â | â | â | â | â | â |\n| [`paru`](https://github.com/
+Morganamilo/paru) | 1.9.3 | ð§ | | | â | â | â | â | â | â | â
+| â | â |\n| [`pip`](https://pip.pypa.io) | 10.0.0 | ð§ | ð | ðª |
+â | â | | â | â | â | â | | |\n| [`pipx`](https://pypa.github.io/
+pipx/) | 1.0.0 | ð§ | ð | ðª | â | â | | â | â | â | â | |
+|\n| [`scoop`](https://scoop.sh) | 0.2.4 | | | ðª | â | â | â | â |
+â | â | â | â | â |\n| [`snap`](https://snapcraft.io) | 2.0.0 | ð§
+| | | â | â | â | â | â | â | | | |\n| [`steamcmd`](https://
+developer.valvesoftware.com/wiki/SteamCMD) | None | ð§ | ð | ðª | | | |
+â | | | | | |\n| [`vscode`](https://code.visualstudio.com) | 1.60.0 | ð§ |
+ð | ðª | â | | | â | | | | | |\n| [`yarn`](https://yarnpkg.com) |
+1.20.0 | ð§ | ð | ðª | â | â | â | â | â | â | â | | â
+|\n| [`yay`](https://github.com/Jguer/yay) | 11.0.0 | ð§ | | | â | â |
+â | â | â | â | â | â | â |\n| [`yum`](http://yum.baseurl.org) |
+4.0.0 | ð§ | | | â | â | â | â | â | â | | â | â |\n|
+[`zypper`](https://en.opensuse.org/Portal:Zypper) | 1.14.0 | ð§ | | | â |
+â | â | â | â | â | | â | â |\n\n## Quickstart\n\nEasiest way is
+to install `mpm` with [`pipx`](https://pypa.github.io/pipx/):\n\n```shell-
+session\n$ pipx install meta-package-manager\n```\n\nOther\n[alternatives
+installation methods](https://kdeldycke.github.io/meta-package-manager/
+install.html)\nare available in the documentation.\n\n## List managers\n\nList
+all supported package managers and their status on current system (macOS\nin
+this case):\n\n```shell-session\n$ mpm --all-managers
 managers\nâ­âââââââââââââ¬âââââââââââââââââââââ¬âââââââââââââââââ¬âââââââââââââââââââââââââââââââ¬âââââââââââââ¬ââââââââââââ®\nâ
 Manager ID â Name â Supported â CLI â Executable â Version
 â\nââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââââ¼âââââââââââââââââââââââââââââââ¼âââââââââââââ¼ââââââââââââ¤\nâ
 apm â Atom\'s apm â â â â apm not found â â â\nâ apt â APT
 â â Linux only â â /usr/bin/apt â â â â â\nâ apt-mint â
 Linux Mint\'s apt â â Linux only â â /usr/bin/apt â â â â
 â\nâ brew â Homebrew Formulae â â â â /opt/homebrew/bin/brew â
```

### Comparing `meta-package-manager-5.8.0/PKG-INFO` & `meta_package_manager-5.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: meta-package-manager
-Version: 5.8.0
+Version: 5.9.0
 Summary: 🎁 wraps all package managers with an unifying CLI
 Home-page: https://github.com/kdeldycke/meta-package-manager
 License: GPL-2.0-or-later
-Keywords: CLI,apm,apt,apt-mint,atom,brew,cargo,cask,choco,chocotaley,composer,dnf,emerge,flatpak,gem,homebrew,mac app store,macos,mas,node,npm,opkg,package,pacman,paru,php composer,pip,pipx,plugin,portage,purl,ruby,rust,scoop,snap,steamcmd,visual studio code,vscode,xbar,swiftbar,yarn,yay,yum,zypper
+Keywords: CLI,apm,apt,apt-mint,atom,brew,cargo,cask,choco,chocotaley,composer,dnf,emerge,flatpak,gem,homebrew,mac app store,macos,mas,node,npm,opkg,package,pacaur,pacman,paru,php composer,pip,pipx,plugin,portage,purl,ruby,rust,scoop,snap,steamcmd,visual studio code,vscode,xbar,swiftbar,yarn,yay,yum,zypper
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Plugins
@@ -20,26 +20,27 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: boltons (>=21.0.0,<22.0.0)
 Requires-Dist: click (>=8.1.2,<9.0.0)
-Requires-Dist: click-extra (>=3.2.5,<4.0.0)
+Requires-Dist: click-extra (>=3.3.1,<4.0.0)
 Requires-Dist: packageurl-python (>=0.10.3,<0.11.0)
-Requires-Dist: tabulate[widechars] (>=0.8.9,<0.9.0)
+Requires-Dist: tabulate[widechars] (>=0.9.0,<0.10.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0); python_version < "3.11"
 Requires-Dist: tomli_w (>=1.0.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0); python_version < "3.10"
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Changelog, https://kdeldycke.github.io/meta-package-manager/changelog.html
 Project-URL: Documentation, https://kdeldycke.github.io/meta-package-manager
 Project-URL: Funding, https://github.com/sponsors/kdeldycke
@@ -66,15 +67,15 @@
 [![DOI](https://zenodo.org/badge/65922807.svg)](https://zenodo.org/badge/latestdoi/65922807)
 
 **What is Meta Package Manager?**
 
 - provides the `mpm` CLI, a wrapper around all package managers
 - `mpm` is like [`yt-dlp`](https://github.com/yt-dlp/yt-dlp), but for package
   managers instead of videos
-- `mpm` solves [XKCD #1654: Universal Install Script](https://xkcd.com/1654/)
+- `mpm` solves [XKCD #1654 - *Universal Install Script*](https://xkcd.com/1654/)
 
 ______________________________________________________________________
 
 ## Features
 
 <img align="right" width="30%" height="30%" src="https://raw.githubusercontent.com/kdeldycke/meta-package-manager/main/docs/images/mpm-outdated-cli.png"/>
 
@@ -117,14 +118,15 @@
 | [`dnf`](https://github.com/rpm-software-management/dnf)                   | 4.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |
 | [`emerge`](https://wiki.gentoo.org/wiki/Portage#emerge)                   | 3.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |     ✓     |
 | [`flatpak`](https://flatpak.org)                                          | 1.2.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |     ✓     |
 | [`gem`](https://rubygems.org)                                             | 2.5.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |        |     ✓     |
 | [`mas`](https://github.com/argon/mas)                                     | 1.6.1        |       |   🍎   |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |
 | [`npm`](https://www.npmjs.com)                                            | 4.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |        |           |
 | [`opkg`](https://git.yoctoproject.org/cgit/cgit.cgi/opkg/)                | 0.2.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |   ✓    |           |
+| [`pacaur`](https://github.com/E5ten/pacaur)                               | 4.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |
 | [`pacman`](https://wiki.archlinux.org/title/pacman)                       | 5.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |
 | [`paru`](https://github.com/Morganamilo/paru)                             | 1.9.3        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |
 | [`pip`](https://pip.pypa.io)                                              | 10.0.0       |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |          |     ✓     |     ✓     |       ✓       |    ✓     |        |           |
 | [`pipx`](https://pypa.github.io/pipx/)                                    | 1.0.0        |   🐧   |   🍎   |    🪟    |      ✓      |     ✓      |          |     ✓     |     ✓     |       ✓       |    ✓     |        |           |
 | [`scoop`](https://scoop.sh)                                               | 0.2.4        |       |       |    🪟    |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |    ✓     |   ✓    |     ✓     |
 | [`snap`](https://snapcraft.io)                                            | 2.0.0        |   🐧   |       |         |      ✓      |     ✓      |    ✓     |     ✓     |     ✓     |       ✓       |          |        |           |
 | [`steamcmd`](https://developer.valvesoftware.com/wiki/SteamCMD)           | None         |   🐧   |   🍎   |    🪟    |             |            |          |     ✓     |           |               |          |        |           |
```

#### html2text {}

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1 Name: meta-package-manager Version: 5.8.0 Summary: ð
+Metadata-Version: 2.1 Name: meta-package-manager Version: 5.9.0 Summary: ð
 wraps all package managers with an unifying CLI Home-page: https://github.com/
 kdeldycke/meta-package-manager License: GPL-2.0-or-later Keywords:
 CLI,apm,apt,apt-
 mint,atom,brew,cargo,cask,choco,chocotaley,composer,dnf,emerge,flatpak,gem,homebrew,mac
-app store,macos,mas,node,npm,opkg,package,pacman,paru,php
+app store,macos,mas,node,npm,opkg,package,pacaur,pacman,paru,php
 composer,pip,pipx,plugin,portage,purl,ruby,rust,scoop,snap,steamcmd,visual
 studio code,vscode,xbar,swiftbar,yarn,yay,yum,zypper Author: Kevin Deldycke
 Author-email: kevin@deldycke.com Requires-Python: >=3.7,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: MacOS X Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later
 (GPLv2+) Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
-Implementation :: CPython Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: System :: Archiving ::
-Packaging Classifier: Topic :: System :: Installation/Setup Classifier: Topic
-:: System :: Software Distribution Classifier: Topic :: Utilities Classifier:
-Typing :: Typed Requires-Dist: boltons (>=21.0.0,<22.0.0) Requires-Dist: click
-(>=8.1.2,<9.0.0) Requires-Dist: click-extra (>=3.2.5,<4.0.0) Requires-Dist:
-packageurl-python (>=0.10.3,<0.11.0) Requires-Dist: tabulate[widechars]
-(>=0.8.9,<0.9.0) Requires-Dist: tomli (>=2.0.1,<3.0.0); python_version < "3.11"
-Requires-Dist: tomli_w (>=1.0.0,<2.0.0) Requires-Dist: typing-extensions
-(>=4.3.0,<5.0.0); python_version < "3.10" Requires-Dist: xmltodict
-(>=0.13.0,<0.14.0) Project-URL: Changelog, https://kdeldycke.github.io/meta-
-package-manager/changelog.html Project-URL: Documentation, https://
-kdeldycke.github.io/meta-package-manager Project-URL: Funding, https://
-github.com/sponsors/kdeldycke Project-URL: Issues, https://github.com/
-kdeldycke/meta-package-manager/issues Project-URL: Repository, https://
-github.com/kdeldycke/meta-package-manager Description-Content-Type: text/
-markdown
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Archiving :: Packaging Classifier: Topic ::
+System :: Installation/Setup Classifier: Topic :: System :: Software
+Distribution Classifier: Topic :: Utilities Classifier: Typing :: Typed
+Requires-Dist: boltons (>=21.0.0,<22.0.0) Requires-Dist: click (>=8.1.2,<9.0.0)
+Requires-Dist: click-extra (>=3.3.1,<4.0.0) Requires-Dist: packageurl-python
+(>=0.10.3,<0.11.0) Requires-Dist: tabulate[widechars] (>=0.9.0,<0.10.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0); python_version < "3.11" Requires-Dist:
+tomli_w (>=1.0.0,<2.0.0) Requires-Dist: typing-extensions (>=4.3.0,<5.0.0);
+python_version < "3.10" Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-
+URL: Changelog, https://kdeldycke.github.io/meta-package-manager/changelog.html
+Project-URL: Documentation, https://kdeldycke.github.io/meta-package-manager
+Project-URL: Funding, https://github.com/sponsors/kdeldycke Project-URL:
+Issues, https://github.com/kdeldycke/meta-package-manager/issues Project-URL:
+Repository, https://github.com/kdeldycke/meta-package-manager Description-
+Content-Type: text/markdown
                             [Meta_Package_Manager]
 [http://imgs.xkcd.com/comics/universal_install_script.png] [![Last release]
 (https://img.shields.io/pypi/v/meta-package-manager.svg)](https://
 pypi.python.org/pypi/meta-package-manager) [![Python versions](https://
 img.shields.io/pypi/pyversions/meta-package-manager.svg)](https://
 pypi.python.org/pypi/meta-package-manager) [![Type checked with mypy](http://
 www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![Unittests
@@ -50,15 +50,15 @@
 [![Documentation status](https://github.com/kdeldycke/meta-package-manager/
 actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/
 kdeldycke/meta-package-manager/actions/workflows/docs.yaml?query=branch%3Amain)
 [![DOI](https://zenodo.org/badge/65922807.svg)](https://zenodo.org/badge/
 latestdoi/65922807) **What is Meta Package Manager?** - provides the `mpm` CLI,
 a wrapper around all package managers - `mpm` is like [`yt-dlp`](https://
 github.com/yt-dlp/yt-dlp), but for package managers instead of videos - `mpm`
-solves [XKCD #1654: Universal Install Script](https://xkcd.com/1654/
+solves [XKCD #1654 - *Universal Install Script*](https://xkcd.com/1654/
 ) ______________________________________________________________________ ##
 Features [https://raw.githubusercontent.com/kdeldycke/meta-package-manager/
 main/docs/images/mpm-outdated-cli.png] [https://raw.githubusercontent.com/
 kdeldycke/meta-package-manager/main/docs/images/mpm-managers-cli.png] -
 Inventory and list all package managers available on the system. - Supports
 macOS, Linux and Windows. - List installed packages. - Search for packages. -
 Install a package. - Remove a package. - List outdated packages. - Sync local
@@ -95,38 +95,40 @@
 | â | â | | â | â | | [`flatpak`](https://flatpak.org) | 1.2.0 | ð§ |
 | | â | â | â | â | â | â | | | â | | [`gem`](https://
 rubygems.org) | 2.5.0 | ð§ | ð | ðª | â | â | â | â | â | â
 | â | | â | | [`mas`](https://github.com/argon/mas) | 1.6.1 | | ð | |
 â | â | â | â | â | â | | | | | [`npm`](https://www.npmjs.com) |
 4.0.0 | ð§ | ð | ðª | â | â | â | â | â | â | â | | | |
 [`opkg`](https://git.yoctoproject.org/cgit/cgit.cgi/opkg/) | 0.2.0 | ð§ | | |
-â | â | â | â | â | â | | â | | | [`pacman`](https://
-wiki.archlinux.org/title/pacman) | 5.0.0 | ð§ | | | â | â | â | â |
-â | â | â | â | â | | [`paru`](https://github.com/Morganamilo/paru) |
-1.9.3 | ð§ | | | â | â | â | â | â | â | â | â | â | |
-[`pip`](https://pip.pypa.io) | 10.0.0 | ð§ | ð | ðª | â | â | | â
-| â | â | â | | | | [`pipx`](https://pypa.github.io/pipx/) | 1.0.0 | ð§
-| ð | ðª | â | â | | â | â | â | â | | | | [`scoop`](https://
-scoop.sh) | 0.2.4 | | | ðª | â | â | â | â | â | â | â | â |
-â | | [`snap`](https://snapcraft.io) | 2.0.0 | ð§ | | | â | â | â |
-â | â | â | | | | | [`steamcmd`](https://developer.valvesoftware.com/
-wiki/SteamCMD) | None | ð§ | ð | ðª | | | | â | | | | | | | [`vscode`]
-(https://code.visualstudio.com) | 1.60.0 | ð§ | ð | ðª | â | | | â |
-| | | | | | [`yarn`](https://yarnpkg.com) | 1.20.0 | ð§ | ð | ðª | â |
-â | â | â | â | â | â | | â | | [`yay`](https://github.com/Jguer/
-yay) | 11.0.0 | ð§ | | | â | â | â | â | â | â | â | â | â
-| | [`yum`](http://yum.baseurl.org) | 4.0.0 | ð§ | | | â | â | â | â
-| â | â | | â | â | | [`zypper`](https://en.opensuse.org/Portal:Zypper)
-| 1.14.0 | ð§ | | | â | â | â | â | â | â | | â | â | ##
-Quickstart Easiest way is to install `mpm` with [`pipx`](https://
-pypa.github.io/pipx/): ```shell-session $ pipx install meta-package-manager ```
-Other [alternatives installation methods](https://kdeldycke.github.io/meta-
-package-manager/install.html) are available in the documentation. ## List
-managers List all supported package managers and their status on current system
-(macOS in this case): ```shell-session $ mpm --all-managers managers
+â | â | â | â | â | â | | â | | | [`pacaur`](https://github.com/
+E5ten/pacaur) | 4.0.0 | ð§ | | | â | â | â | â | â | â | â |
+â | â | | [`pacman`](https://wiki.archlinux.org/title/pacman) | 5.0.0 |
+ð§ | | | â | â | â | â | â | â | â | â | â | | [`paru`]
+(https://github.com/Morganamilo/paru) | 1.9.3 | ð§ | | | â | â | â |
+â | â | â | â | â | â | | [`pip`](https://pip.pypa.io) | 10.0.0 |
+ð§ | ð | ðª | â | â | | â | â | â | â | | | | [`pipx`]
+(https://pypa.github.io/pipx/) | 1.0.0 | ð§ | ð | ðª | â | â | | â
+| â | â | â | | | | [`scoop`](https://scoop.sh) | 0.2.4 | | | ðª | â
+| â | â | â | â | â | â | â | â | | [`snap`](https://
+snapcraft.io) | 2.0.0 | ð§ | | | â | â | â | â | â | â | | | | |
+[`steamcmd`](https://developer.valvesoftware.com/wiki/SteamCMD) | None | ð§ |
+ð | ðª | | | | â | | | | | | | [`vscode`](https://code.visualstudio.com)
+| 1.60.0 | ð§ | ð | ðª | â | | | â | | | | | | | [`yarn`](https://
+yarnpkg.com) | 1.20.0 | ð§ | ð | ðª | â | â | â | â | â | â
+| â | | â | | [`yay`](https://github.com/Jguer/yay) | 11.0.0 | ð§ | | |
+â | â | â | â | â | â | â | â | â | | [`yum`](http://
+yum.baseurl.org) | 4.0.0 | ð§ | | | â | â | â | â | â | â | | â
+| â | | [`zypper`](https://en.opensuse.org/Portal:Zypper) | 1.14.0 | ð§ | |
+| â | â | â | â | â | â | | â | â | ## Quickstart Easiest way
+is to install `mpm` with [`pipx`](https://pypa.github.io/pipx/): ```shell-
+session $ pipx install meta-package-manager ``` Other [alternatives
+installation methods](https://kdeldycke.github.io/meta-package-manager/
+install.html) are available in the documentation. ## List managers List all
+supported package managers and their status on current system (macOS in this
+case): ```shell-session $ mpm --all-managers managers
 â­âââââââââââââ¬âââââââââââââââââââââ¬âââââââââââââââââ¬âââââââââââââââââââââââââââââââ¬âââââââââââââ¬ââââââââââââ®
 â Manager ID â Name â Supported â CLI â Executable â Version â
 ââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââââ¼âââââââââââââââââââââââââââââââ¼âââââââââââââ¼ââââââââââââ¤
 â apm â Atom's apm â â â â apm not found â â â â apt â
 APT â â Linux only â â /usr/bin/apt â â â â â â apt-mint
 â Linux Mint's apt â â Linux only â â /usr/bin/apt â â â â
 â â brew â Homebrew Formulae â â â â /opt/homebrew/bin/brew â
```

