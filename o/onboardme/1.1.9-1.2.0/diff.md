# Comparing `tmp/onboardme-1.1.9.tar.gz` & `tmp/onboardme-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.1.9.tar", max compression
+gzip compressed data, was "onboardme-1.2.0.tar", max compression
```

## Comparing `onboardme-1.1.9.tar` & `onboardme-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.9/LICENSE.txt
--rw-r--r--   0        0        0    15257 2023-05-21 10:41:32.239098 onboardme-1.1.9/README.md
--rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.9/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.9/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.9/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.1.9/onboardme/console_logging.py
--rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.1.9/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.9/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.9/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.9/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.9/onboardme/help_text.py
--rw-r--r--   0        0        0     3085 2023-05-21 10:34:53.575751 onboardme-1.1.9/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.9/onboardme/misc.py
--rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.9/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.9/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.9/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.9/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.9/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1919 2023-05-21 10:43:46.741149 onboardme-1.1.9/pyproject.toml
--rw-r--r--   0        0        0    16638 1970-01-01 00:00:00.000000 onboardme-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0    15245 2023-05-21 11:22:02.167263 onboardme-1.2.0/README.md
+-rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.2.0/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.2.0/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.2.0/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.2.0/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.2.0/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.2.0/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.2.0/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.2.0/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5790 2023-05-21 15:49:30.802500 onboardme-1.2.0/onboardme/help_text.py
+-rw-r--r--   0        0        0     3085 2023-05-21 11:22:02.171439 onboardme-1.2.0/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.2.0/onboardme/misc.py
+-rwxr-xr-x   0        0        0     9362 2023-05-21 15:32:16.703438 onboardme-1.2.0/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.2.0/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.2.0/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.2.0/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.2.0/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1919 2023-05-21 15:32:43.314470 onboardme-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16626 1970-01-01 00:00:00.000000 onboardme-1.2.0/PKG-INFO
```

### Comparing `onboardme-1.1.9/LICENSE.txt` & `onboardme-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/README.md` & `onboardme-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,16 @@
 <img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/python_virtual_env_example.png' alt='screenshot of using bat and python virtual env in powerline'>
 </p>
 
 </details>
 
 # Quick Start
 
-### Prereq Installs
+### Install Locally
+
 You'll need `curl`, `brew`, `git`, and Python 3.11 to get started. We have a setup script to install those (except `curl`) and help you get your environment to the XDG spec under <b>Locally</b> or you can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).
 
 <details>
   <summary>Local prereq install script</summary>
 
 
 <details>
@@ -173,17 +174,15 @@
 chsh -s /usr/local/bin/bash $(whoami)
 ```
 
 After that, you can also set the shell directly in your terminal app via the settings.
 
 </details>
 
-#### Install
-
-If you've already got brew and Python3.11 on your machine, you can just do:
+If you've already got all the above prereq on your machine, you can just do:
 ```bash
 # should also work with pipx, if you'd like to use that instead
 pip install --user --upgrade onboardme
 ```
 
 ### Using the Docker image
```

#### html2text {}

```diff
@@ -42,15 +42,15 @@
                 [screenshot_of_full_output_of_onboardme_--help]
   Examples of the terminal after onboardme runs
 ### neovim [screenshot of neovim with colors] ### Powerline and ls [screenshot
  of powerline and lsd] ### Powerline with git [screenshot of powerline and git
   colors] ### Image and colors [screenshot of color samples and image of dog
   using a computer using sixel] ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
- # Quick Start ### Prereq Installs You'll need `curl`, `brew`, `git`, and
+ # Quick Start ### Install Locally You'll need `curl`, `brew`, `git`, and
 Python 3.11 to get started. We have a setup script to install those (except
 `curl`) and help you get your environment to the XDG spec under Locally or you
 can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/
 jessebot/onboardme).  Local prereq install script  curl, a pre-prereq ```bash #
 First, make sure you have curl, but it *should* be there already be on macOS. #
 if this doesn't return anything, you need to install curl which curl # Debian/
 Ubuntu may not have curl installed depending on where you are sudo apt install
@@ -65,26 +65,26 @@
 MacOS source your updated `.bash_profile`: ```bash bash source ~/.bash_profile
 ``` You will still have to set your default shell to BASH to if you want to
 take advantage of the default dot files for onboardme. You can do that like
 this: ```bash brew install bash sudo -i # if you're on an M1 or newer: echo "/
 opt/homebrew/bin/bash" >> /etc/shells && exit chsh -s /opt/homebrew/bin/bash $
 (whoami) # if you're on a mac earlier than the M1: echo "/usr/local/bin/bash"
 >> /etc/shells && exit chsh -s /usr/local/bin/bash $(whoami) ``` After that,
-you can also set the shell directly in your terminal app via the settings.
-#### Install If you've already got brew and Python3.11 on your machine, you can
-just do: ```bash # should also work with pipx, if you'd like to use that
-instead pip install --user --upgrade onboardme ``` ### Using the Docker image
-To run the image locally with onboardme installed and already run using default
-settings: ```bash # this image is built daily and has already run onboardme
-with the default settings docker run jessebot/onboardme:latest ``` To run the
-image locally with onbaordme installed but _not_ run: ```bash # best if you
-have your own dot files, or need a smaller initial docker image to pull # no
-packages outside of the required pre-reqs for onboardme have been installed
-docker run jessebot/onboardme:no-install ``` ## Running commands _Now_ you can
-run `onboardme` ð ```bash # this will display the help text for onboardme
+you can also set the shell directly in your terminal app via the settings.  If
+you've already got all the above prereq on your machine, you can just do:
+```bash # should also work with pipx, if you'd like to use that instead pip
+install --user --upgrade onboardme ``` ### Using the Docker image To run the
+image locally with onboardme installed and already run using default settings:
+```bash # this image is built daily and has already run onboardme with the
+default settings docker run jessebot/onboardme:latest ``` To run the image
+locally with onbaordme installed but _not_ run: ```bash # best if you have your
+own dot files, or need a smaller initial docker image to pull # no packages
+outside of the required pre-reqs for onboardme have been installed docker run
+jessebot/onboardme:no-install ``` ## Running commands _Now_ you can run
+`onboardme` ð ```bash # this will display the help text for onboardme
 onboardme --help # Running this won't overwrite any existing dot files, but it
 may add new ones. onboardme ``` From here, if you want to *completely wipe your
 existing dot files* for a fresh start with with `onboardme`, you can run:
 ```bash # WARNING: This will overwrite your local dotfiles, including your
 .bashrc and .bash_profile # can also be done with: onboardme -O onboardme --
 overwrite ``` You can read more in depth at the [Getting Started Docs] ð!
 There's also more [docs] on basically every program that onboardme touches. ###
```

### Comparing `onboardme-1.1.9/onboardme/__init__.py` & `onboardme-1.2.0/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/config/firewall/iptables.sh` & `onboardme-1.2.0/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/console_logging.py` & `onboardme-1.2.0/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/constants.py` & `onboardme-1.2.0/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/dot_files.py` & `onboardme-1.2.0/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/env_config.py` & `onboardme-1.2.0/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/firewall.py` & `onboardme-1.2.0/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/help_text.py` & `onboardme-1.2.0/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/ide_setup.py` & `onboardme-1.2.0/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/misc.py` & `onboardme-1.2.0/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/pkg_management.py` & `onboardme-1.2.0/onboardme/pkg_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,14 +105,17 @@
             pkg_emoji = pkg_mngr_dict['emoji']
             msg = f'{pkg_emoji} [grn][b]{pkg_mngr}[/b][/grn] app management'
             print_header(msg)
 
             # commands for listing, installing, updating, upgrading, & cleanup
             pkg_cmds = pkg_mngr_dict['commands']
 
+            # make sure we use any required env vars during installs
+            install_env_vars = pkg_mngr_dict.get('env_vars', None)
+
             if pkg_mngr == 'snap' and not shutil.which('snap'):
                 log.warn("snap is either not installed, or you need to log out"
                          "and back in (or reboot) for it to be available. "
                          "https://snapcraft.io/docs/installing-snap-on-debian")
                 # continues onto the next package manager
                 continue
 
@@ -137,31 +140,38 @@
             else:
                 installed_pkgs = []
 
             # iterate through package groups for a given package manager
             for pkg_group in pkg_groups:
                 # if package group is in the packages.yaml file
                 if pkg_group in available_pkg_groups:
-                    if pkg_group == "macOS":
-                        # zathura needs some help on macOS
-                        check_zathura()
+                    # used to be for zathura, a document viewer, might delete
+                    # if pkg_group == "macOS":
+                    #     # zathura needs some help on macOS
+                    #     check_zathura()
 
                     install_pkg_group(pkg_cmds['install'],
                                       available_pkg_groups[pkg_group],
-                                      installed_pkgs)
+                                      installed_pkgs,
+                                      install_env_vars,
+                                      no_upgrade)
                     sub_header(f'{pkg_group.title()} packages installed.')
 
             # run final cleanup commands, if any
             if 'cleanup' in pkg_cmds:
                 subproc([pkg_cmds['cleanup']])
                 sub_header("[b]Cleanup[/b] step Completed.")
 
 
-def install_pkg_group(install_cmd: str, pkgs_to_install: list,
-                      installed_pkgs: list) -> None:
+def install_pkg_group(install_cmd: str, 
+                      pkgs_to_install: list,
+                      installed_pkgs: list, 
+                      install_env_vars: dict,
+                      no_upgrade: bool
+                      ) -> None:
     """
     Installs packages if they are not already installed.
     provided install command string.
     Returns True.
     """
     log.debug(f"Currently installed packages: {installed_pkgs}")
     log.info(f"Packages to install are: {pkgs_to_install}")
@@ -179,24 +189,24 @@
 
             # this covers things like "--cask iterm2" for brew
             if "--cask" in pkg:
                 pkg_short_name = pkg.split(' ')[1]
 
             log.debug(f"Checking if {pkg_short_name} is installed...")
             if pkg_short_name in installed_pkgs:
-                if 'upgrade' not in install_cmd:
+                if no_upgrade or 'upgrade' not in install_cmd:
                     log.info(f"{pkg} already installed. Moving on.")
                     # continues to the next pkg in the pkgs_to_install list
                     continue
                 # if the install command has upgrade in it, we always run it
                 else:
                     log.info(f"Upgrading {pkg} now...")
 
         # Actual installation
-        subproc([install_cmd + pkg], quiet=True)
+        subproc([install_cmd + pkg], quiet=True, env=install_env_vars)
 
 
 def install_brew_taps(taps: list) -> None:
     """
     Checks current brew taps, and then runs brew tap {tap} on any taps that are
     in a list of git repos from packages.yaml, and aren't already tapped
     """
@@ -216,19 +226,20 @@
         # only brew tap if they don't already exist
         if tap not in current_taps:
             subproc(["brew tap " + tap])
         else:
             log.info(f"{tap} already installed. Moving on.")
 
 
-def check_zathura() -> None:
-    """
-    make sure zathura is installed on macos
-    installs via brew if it's not installed
-    always returns True if everything was successful
-    """
-    if not shutil.which("zathura"):
-        zathura_pdf = "$(brew --prefix zathura-pdf-mupdf)"
-        cmds = ["mkdir -p $(brew --prefix zathura)/lib/zathura",
-                f"ln -s {zathura_pdf}/libpdf-mupdf.dylib" +
-                f"{zathura_pdf}/lib/zathura/libpdf-mupdf.dylib"]
-        subproc(cmds, quiet=True)
+# not currently using zathura on macOS, so removing as it's untested
+# def check_zathura() -> None:
+#     """
+#     make sure zathura is installed on macos
+#     installs via brew if it's not installed
+#     always returns True if everything was successful
+#     """
+#     if not shutil.which("zathura"):
+#         zathura_pdf = "$(brew --prefix zathura-pdf-mupdf)"
+#         cmds = ["mkdir -p $(brew --prefix zathura)/lib/zathura",
+#                 f"ln -s {zathura_pdf}/libpdf-mupdf.dylib" +
+#                 f"{zathura_pdf}/lib/zathura/libpdf-mupdf.dylib"]
+#         subproc(cmds, quiet=True)
```

### Comparing `onboardme-1.1.9/onboardme/subproc.py` & `onboardme-1.2.0/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/onboardme/sudo_setup.py` & `onboardme-1.2.0/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.9/pyproject.toml` & `onboardme-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.1.9"
+version       = "1.2.0"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.1.9/PKG-INFO` & `onboardme-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.1.9
+Version: 1.2.0
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
@@ -138,15 +138,16 @@
 <img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/python_virtual_env_example.png' alt='screenshot of using bat and python virtual env in powerline'>
 </p>
 
 </details>
 
 # Quick Start
 
-### Prereq Installs
+### Install Locally
+
 You'll need `curl`, `brew`, `git`, and Python 3.11 to get started. We have a setup script to install those (except `curl`) and help you get your environment to the XDG spec under <b>Locally</b> or you can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).
 
 <details>
   <summary>Local prereq install script</summary>
 
 
 <details>
@@ -203,17 +204,15 @@
 chsh -s /usr/local/bin/bash $(whoami)
 ```
 
 After that, you can also set the shell directly in your terminal app via the settings.
 
 </details>
 
-#### Install
-
-If you've already got brew and Python3.11 on your machine, you can just do:
+If you've already got all the above prereq on your machine, you can just do:
 ```bash
 # should also work with pipx, if you'd like to use that instead
 pip install --user --upgrade onboardme
 ```
 
 ### Using the Docker image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.1.9 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.2.0 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
@@ -61,15 +61,15 @@
                 [screenshot_of_full_output_of_onboardme_--help]
   Examples of the terminal after onboardme runs
 ### neovim [screenshot of neovim with colors] ### Powerline and ls [screenshot
  of powerline and lsd] ### Powerline with git [screenshot of powerline and git
   colors] ### Image and colors [screenshot of color samples and image of dog
   using a computer using sixel] ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
- # Quick Start ### Prereq Installs You'll need `curl`, `brew`, `git`, and
+ # Quick Start ### Install Locally You'll need `curl`, `brew`, `git`, and
 Python 3.11 to get started. We have a setup script to install those (except
 `curl`) and help you get your environment to the XDG spec under Locally or you
 can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/
 jessebot/onboardme).  Local prereq install script  curl, a pre-prereq ```bash #
 First, make sure you have curl, but it *should* be there already be on macOS. #
 if this doesn't return anything, you need to install curl which curl # Debian/
 Ubuntu may not have curl installed depending on where you are sudo apt install
@@ -84,26 +84,26 @@
 MacOS source your updated `.bash_profile`: ```bash bash source ~/.bash_profile
 ``` You will still have to set your default shell to BASH to if you want to
 take advantage of the default dot files for onboardme. You can do that like
 this: ```bash brew install bash sudo -i # if you're on an M1 or newer: echo "/
 opt/homebrew/bin/bash" >> /etc/shells && exit chsh -s /opt/homebrew/bin/bash $
 (whoami) # if you're on a mac earlier than the M1: echo "/usr/local/bin/bash"
 >> /etc/shells && exit chsh -s /usr/local/bin/bash $(whoami) ``` After that,
-you can also set the shell directly in your terminal app via the settings.
-#### Install If you've already got brew and Python3.11 on your machine, you can
-just do: ```bash # should also work with pipx, if you'd like to use that
-instead pip install --user --upgrade onboardme ``` ### Using the Docker image
-To run the image locally with onboardme installed and already run using default
-settings: ```bash # this image is built daily and has already run onboardme
-with the default settings docker run jessebot/onboardme:latest ``` To run the
-image locally with onbaordme installed but _not_ run: ```bash # best if you
-have your own dot files, or need a smaller initial docker image to pull # no
-packages outside of the required pre-reqs for onboardme have been installed
-docker run jessebot/onboardme:no-install ``` ## Running commands _Now_ you can
-run `onboardme` ð ```bash # this will display the help text for onboardme
+you can also set the shell directly in your terminal app via the settings.  If
+you've already got all the above prereq on your machine, you can just do:
+```bash # should also work with pipx, if you'd like to use that instead pip
+install --user --upgrade onboardme ``` ### Using the Docker image To run the
+image locally with onboardme installed and already run using default settings:
+```bash # this image is built daily and has already run onboardme with the
+default settings docker run jessebot/onboardme:latest ``` To run the image
+locally with onbaordme installed but _not_ run: ```bash # best if you have your
+own dot files, or need a smaller initial docker image to pull # no packages
+outside of the required pre-reqs for onboardme have been installed docker run
+jessebot/onboardme:no-install ``` ## Running commands _Now_ you can run
+`onboardme` ð ```bash # this will display the help text for onboardme
 onboardme --help # Running this won't overwrite any existing dot files, but it
 may add new ones. onboardme ``` From here, if you want to *completely wipe your
 existing dot files* for a fresh start with with `onboardme`, you can run:
 ```bash # WARNING: This will overwrite your local dotfiles, including your
 .bashrc and .bash_profile # can also be done with: onboardme -O onboardme --
 overwrite ``` You can read more in depth at the [Getting Started Docs] ð!
 There's also more [docs] on basically every program that onboardme touches. ###
```

