# Comparing `tmp/onboardme-1.1.8.tar.gz` & `tmp/onboardme-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.1.8.tar", max compression
+gzip compressed data, was "onboardme-1.1.9.tar", max compression
```

## Comparing `onboardme-1.1.8.tar` & `onboardme-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.8/LICENSE.txt
--rw-r--r--   0        0        0    14730 2023-05-20 19:55:38.998380 onboardme-1.1.8/README.md
--rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.8/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.8/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.8/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.1.8/onboardme/console_logging.py
--rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.1.8/onboardme/constants.py
--rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.8/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.8/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.8/onboardme/firewall.py
--rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.8/onboardme/help_text.py
--rw-r--r--   0        0        0     3081 2023-05-20 20:09:43.362905 onboardme-1.1.8/onboardme/ide_setup.py
--rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.8/onboardme/misc.py
--rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.8/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.8/onboardme/scripts/get_apt_list.sh
--rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.8/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.8/onboardme/subproc.py
--rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.8/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1919 2023-05-20 20:05:50.789968 onboardme-1.1.8/pyproject.toml
--rw-r--r--   0        0        0    16111 1970-01-01 00:00:00.000000 onboardme-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-11-01 08:47:49.234908 onboardme-1.1.9/LICENSE.txt
+-rw-r--r--   0        0        0    15257 2023-05-21 10:41:32.239098 onboardme-1.1.9/README.md
+-rwxr-xr-x   0        0        0     6786 2023-05-20 12:14:51.142576 onboardme-1.1.9/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2022-11-01 08:47:49.282424 onboardme-1.1.9/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2022-11-04 13:33:39.466645 onboardme-1.1.9/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2023-05-20 12:40:29.736539 onboardme-1.1.9/onboardme/console_logging.py
+-rw-r--r--   0        0        0     1793 2023-05-20 13:11:53.818575 onboardme-1.1.9/onboardme/constants.py
+-rw-r--r--   0        0        0     4935 2023-03-18 10:20:53.858756 onboardme-1.1.9/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     5606 2023-03-18 21:01:43.624191 onboardme-1.1.9/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2023-01-12 13:30:47.874910 onboardme-1.1.9/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     5790 2023-05-20 10:57:17.511316 onboardme-1.1.9/onboardme/help_text.py
+-rw-r--r--   0        0        0     3085 2023-05-21 10:34:53.575751 onboardme-1.1.9/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      933 2022-11-16 14:22:47.478337 onboardme-1.1.9/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8773 2023-05-20 10:53:13.449514 onboardme-1.1.9/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0       97 2022-12-04 19:57:47.905273 onboardme-1.1.9/onboardme/scripts/get_apt_list.sh
+-rwxr-xr-x   0        0        0      233 2022-11-25 16:03:39.303327 onboardme-1.1.9/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2023-01-12 13:30:47.881539 onboardme-1.1.9/onboardme/subproc.py
+-rw-r--r--   0        0        0     1789 2022-11-18 16:13:55.306804 onboardme-1.1.9/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1919 2023-05-21 10:43:46.741149 onboardme-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0    16638 1970-01-01 00:00:00.000000 onboardme-1.1.9/PKG-INFO
```

### Comparing `onboardme-1.1.8/LICENSE.txt` & `onboardme-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/README.md` & `onboardme-1.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -109,19 +109,37 @@
 </p>
 
 </details>
 
 # Quick Start
 
 ### Prereq Installs
-You'll need `brew`, `git`, and Python 3.11 to get started. We have a setup script to install those and help you get your environment to the XDG spec under <b>Locally</b> or you can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).
+You'll need `curl`, `brew`, `git`, and Python 3.11 to get started. We have a setup script to install those (except `curl`) and help you get your environment to the XDG spec under <b>Locally</b> or you can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).
 
 <details>
   <summary>Local prereq install script</summary>
 
+
+<details>
+  <summary><code>curl</code>, a pre-prereq</summary>
+
+  ```bash
+  # First, make sure you have curl, but it *should* be there already be on macOS.
+  # if this doesn't return anything, you need to install curl
+  which curl
+
+  # Debian/Ubuntu may not have curl installed depending on where you are
+  sudo apt install -y curl
+  ```
+
+  If it's not there on Linux, you can install it with `apt` or use any default package manager like yum, or whatever people who use gentoo use.
+
+</details>
+
+Make sure you have sudo access, otherwise we won't be able to install certain things.
 The quickest way to get started on a fresh macOS or distro of Debian (including Ubuntu) is:
 ```bash
 # this will download setup.sh to your current directory and run it
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)"
 ```
 
 #### Linux
@@ -155,41 +173,37 @@
 chsh -s /usr/local/bin/bash $(whoami)
 ```
 
 After that, you can also set the shell directly in your terminal app via the settings.
 
 </details>
 
+#### Install
 
-<details>
-  <summary><code>jessebot/onboardme</code> docker image</summary>
+If you've already got brew and Python3.11 on your machine, you can just do:
+```bash
+# should also work with pipx, if you'd like to use that instead
+pip install --user --upgrade onboardme
+```
+
+### Using the Docker image
 
 To run the image locally with onboardme installed and already run using default settings:
 
 ```bash
 # this image is built daily and has already run onboardme with the default settings
-docker run jessebot/onboardme:latest /bin/bash
+docker run jessebot/onboardme:latest
 ```
 
 To run the image locally with onbaordme installed but _not_ run:
 
 ```bash
 # best if you have your own dot files, or need a smaller initial docker image to pull
 # no packages outside of the required pre-reqs for onboardme have been installed
-docker run jessebot/onboardme:no-install /bin/bash
-```
-
-</details>
-
-## Install
-
-If you've already got brew and Python3.11 on your machine, you can just do:
-```bash
-# should also work with pipx, if you'd like to use that instead
-pip install --user --upgrade onboardme
+docker run jessebot/onboardme:no-install
 ```
 
 ## Running commands
 
 _Now_ you can run `onboardme` 🎉 
 ```bash
 # this will display the help text for onboardme
```

#### html2text {}

```diff
@@ -42,92 +42,98 @@
                 [screenshot_of_full_output_of_onboardme_--help]
   Examples of the terminal after onboardme runs
 ### neovim [screenshot of neovim with colors] ### Powerline and ls [screenshot
  of powerline and lsd] ### Powerline with git [screenshot of powerline and git
   colors] ### Image and colors [screenshot of color samples and image of dog
   using a computer using sixel] ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
- # Quick Start ### Prereq Installs You'll need `brew`, `git`, and Python 3.11
-to get started. We have a setup script to install those and help you get your
-environment to the XDG spec under Locally or you can just use our docker image,
-[jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).  Local
-prereq install script The quickest way to get started on a fresh macOS or
-distro of Debian (including Ubuntu) is: ```bash # this will download setup.sh
-to your current directory and run it /bin/bash -c "$(curl -fsSL https://
+ # Quick Start ### Prereq Installs You'll need `curl`, `brew`, `git`, and
+Python 3.11 to get started. We have a setup script to install those (except
+`curl`) and help you get your environment to the XDG spec under Locally or you
+can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/
+jessebot/onboardme).  Local prereq install script  curl, a pre-prereq ```bash #
+First, make sure you have curl, but it *should* be there already be on macOS. #
+if this doesn't return anything, you need to install curl which curl # Debian/
+Ubuntu may not have curl installed depending on where you are sudo apt install
+-y curl ``` If it's not there on Linux, you can install it with `apt` or use
+any default package manager like yum, or whatever people who use gentoo use.
+Make sure you have sudo access, otherwise we won't be able to install certain
+things. The quickest way to get started on a fresh macOS or distro of Debian
+(including Ubuntu) is: ```bash # this will download setup.sh to your current
+directory and run it /bin/bash -c "$(curl -fsSL https://
 raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)" ``` #### Linux
 Source your updated `.bashrc`: ```bash # for linux source ~/.bashrc ``` ####
 MacOS source your updated `.bash_profile`: ```bash bash source ~/.bash_profile
 ``` You will still have to set your default shell to BASH to if you want to
 take advantage of the default dot files for onboardme. You can do that like
 this: ```bash brew install bash sudo -i # if you're on an M1 or newer: echo "/
 opt/homebrew/bin/bash" >> /etc/shells && exit chsh -s /opt/homebrew/bin/bash $
 (whoami) # if you're on a mac earlier than the M1: echo "/usr/local/bin/bash"
 >> /etc/shells && exit chsh -s /usr/local/bin/bash $(whoami) ``` After that,
 you can also set the shell directly in your terminal app via the settings.
-jessebot/onboardme docker image To run the image locally with onboardme
-installed and already run using default settings: ```bash # this image is built
-daily and has already run onboardme with the default settings docker run
-jessebot/onboardme:latest /bin/bash ``` To run the image locally with onbaordme
-installed but _not_ run: ```bash # best if you have your own dot files, or need
-a smaller initial docker image to pull # no packages outside of the required
-pre-reqs for onboardme have been installed docker run jessebot/onboardme:no-
-install /bin/bash ```  ## Install If you've already got brew and Python3.11 on
-your machine, you can just do: ```bash # should also work with pipx, if you'd
-like to use that instead pip install --user --upgrade onboardme ``` ## Running
-commands _Now_ you can run `onboardme` ð ```bash # this will display the
-help text for onboardme onboardme --help # Running this won't overwrite any
-existing dot files, but it may add new ones. onboardme ``` From here, if you
-want to *completely wipe your existing dot files* for a fresh start with with
-`onboardme`, you can run: ```bash # WARNING: This will overwrite your local
-dotfiles, including your .bashrc and .bash_profile # can also be done with:
-onboardme -O onboardme --overwrite ``` You can read more in depth at the
-[Getting Started Docs] ð! There's also more [docs] on basically every
-program that onboardme touches. ### Upgrades If you're on python 3.11, you
-should be able to do: ```bash pip3.11 install --upgrade onboardme ``` ###
-Configuration onboardme has lots of CLI options, but you can also use config
-files. You have to create these files for the time being. Config files are in
-`$XDG_CONFIG_HOME/onboardme/`, or `~/.config/onboardme/` if `$XDG_CONFIG_HOME`
-is not defined. | Config File | Description | |:-------------------------------
------------|:----------------------------------------------------| |
-`$XDG_CONFIG_HOME/onboardme/config.yml` | For step configuration to run either
-all steps, or just a subset. | | `$XDG_CONFIG_HOME/onboardme/packages.yml` |
-For adding packages with different package managers | Examples:  ~/.config/
-onboardme/config.yml ```yaml log: # Full path to a file you'd like to log to.
-Creates file if it doesn't exist file: "" # what level of logs to output
-(DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific function
-in the list of functions we run steps: # these are mac specific steps Darwin: #
-clones dot files into home dir/git fetches updates for dot files - dot_files #
-install packages - packages # adds nerdfonts - font_setup # runs :Lazy sync to
-install all your plugins - neovim_setup # sets up touchID for sudo - sudo_setup
-# these are linux specific steps Linux: - dot_files - packages - font_setup -
-neovim_setup # add your user to the docker group - group_setup dot_files: #
-personal git repo URL for your dot files, defaults to jessebot/dot_files
-git_url: "https://github.com/jessebot/dot_files.git" # the branch to use for
-the git repo above, defaults to main git_branch: "main" # !CAREFUL: runs a `git
-reset --hard`, which will overwite/delete local files in ~ that # conflict with
-the above defined git repo url and branch. You should run # `onboardme -
-s dot_files` to get the files that would be overwritten overwrite: false #
-basic package config package: # Remove any of the below pkg managers to only
-run the remaining pkg managers managers: # these are macOS specific steps
-Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
-pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
-install groups: - default # uncomment these to add them as default installed
-package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
-tested for these operating systems: [![Tested on Ventura 13.4 with a 13-inch M1
-Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro]
-(https://img.shields.io/badge/mac%20os-000000?style=for-the-
-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
-[Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/
-badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
-www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
-badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
-ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
-(https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
-badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
-(https://img.shields.io/badge/Python-FFD43B?style=for-the-
+#### Install If you've already got brew and Python3.11 on your machine, you can
+just do: ```bash # should also work with pipx, if you'd like to use that
+instead pip install --user --upgrade onboardme ``` ### Using the Docker image
+To run the image locally with onboardme installed and already run using default
+settings: ```bash # this image is built daily and has already run onboardme
+with the default settings docker run jessebot/onboardme:latest ``` To run the
+image locally with onbaordme installed but _not_ run: ```bash # best if you
+have your own dot files, or need a smaller initial docker image to pull # no
+packages outside of the required pre-reqs for onboardme have been installed
+docker run jessebot/onboardme:no-install ``` ## Running commands _Now_ you can
+run `onboardme` ð ```bash # this will display the help text for onboardme
+onboardme --help # Running this won't overwrite any existing dot files, but it
+may add new ones. onboardme ``` From here, if you want to *completely wipe your
+existing dot files* for a fresh start with with `onboardme`, you can run:
+```bash # WARNING: This will overwrite your local dotfiles, including your
+.bashrc and .bash_profile # can also be done with: onboardme -O onboardme --
+overwrite ``` You can read more in depth at the [Getting Started Docs] ð!
+There's also more [docs] on basically every program that onboardme touches. ###
+Upgrades If you're on python 3.11, you should be able to do: ```bash pip3.11
+install --upgrade onboardme ``` ### Configuration onboardme has lots of CLI
+options, but you can also use config files. You have to create these files for
+the time being. Config files are in `$XDG_CONFIG_HOME/onboardme/`, or
+`~/.config/onboardme/` if `$XDG_CONFIG_HOME` is not defined. | Config File |
+Description | |:------------------------------------------|:-------------------
+---------------------------------| | `$XDG_CONFIG_HOME/onboardme/config.yml` |
+For step configuration to run either all steps, or just a subset. | |
+`$XDG_CONFIG_HOME/onboardme/packages.yml` | For adding packages with different
+package managers | Examples:  ~/.config/onboardme/config.yml ```yaml log: #
+Full path to a file you'd like to log to. Creates file if it doesn't exist
+file: "" # what level of logs to output (DEBUG, INFO, WARN, ERROR) level:
+"INFO" # steps refer to a specific function in the list of functions we run
+steps: # these are mac specific steps Darwin: # clones dot files into home dir/
+git fetches updates for dot files - dot_files # install packages - packages #
+adds nerdfonts - font_setup # runs :Lazy sync to install all your plugins -
+neovim_setup # sets up touchID for sudo - sudo_setup # these are linux specific
+steps Linux: - dot_files - packages - font_setup - neovim_setup # add your user
+to the docker group - group_setup dot_files: # personal git repo URL for your
+dot files, defaults to jessebot/dot_files git_url: "https://github.com/
+jessebot/dot_files.git" # the branch to use for the git repo above, defaults to
+main git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will
+overwite/delete local files in ~ that # conflict with the above defined git
+repo url and branch. You should run # `onboardme -s dot_files` to get the files
+that would be overwritten overwrite: false # basic package config package: #
+Remove any of the below pkg managers to only run the remaining pkg managers
+managers: # these are macOS specific steps Darwin: - brew - pip3.11 # these are
+linux specific steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of
+extra existing packages groups to install groups: - default # uncomment these
+to add them as default installed package groups # - gui # - gaming # - devops
+```  ## Under the Hood Made and tested for these operating systems: [![Tested
+on Ventura 13.4 with a 13-inch M1 Macbook pro and a 13-inch AMD 1,4 GHz Quad-
+Core Intel Core i5 2020 Macbook Pro](https://img.shields.io/badge/mac%20os-
+000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/
+wiki/MacOS?lang=en) [![Tested only on Debian Bookworm (debian:bookworm)](https:
+//img.shields.io/badge/Debian-A81D33?style=for-the-
+badge&logo=debian&logoColor=white)](https://www.debian.org/) [![Tested only on
+ubuntu servers](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-
+badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/) And optomized for the
+following programs: [![made-with-neovim](https://img.shields.io/badge/NeoVim-
+0f191f?style=for-the-badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/)
+[![made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
 (https://img.shields.io/badge/GNU%20Bash-000000?style=for-the-
 badge&logo=GNU%20Bash&logoColor=#5c983b)](https://www.gnu.org/software/bash/)
 [![made-with-powerline](https://img.shields.io/badge/powerline-
 000000?style=for-the-badge&logo=powerline&logoColor=#5c983b)](https://
 powerline.readthedocs.io/en/master/overview.html) #### Built using these great
 tools: [[rich python library logo with with yellow snake]](https://github.com/
```

### Comparing `onboardme-1.1.8/onboardme/__init__.py` & `onboardme-1.1.9/onboardme/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/config/firewall/iptables.sh` & `onboardme-1.1.9/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/console_logging.py` & `onboardme-1.1.9/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/constants.py` & `onboardme-1.1.9/onboardme/constants.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/dot_files.py` & `onboardme-1.1.9/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/env_config.py` & `onboardme-1.1.9/onboardme/env_config.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/firewall.py` & `onboardme-1.1.9/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/help_text.py` & `onboardme-1.1.9/onboardme/help_text.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/ide_setup.py` & `onboardme-1.1.9/onboardme/ide_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,10 +75,10 @@
     Runs this command that works via the cli:
         nvim --headless "+Lazy! sync" +qa
     """
     print_header('[green][i]NeoVim[/i][/green] plugins installation '
                  '[dim]and[/dim] upgrades via [green]lazy.nvim[/green]')
 
     subproc(['nvim --headless ":Lazy sync" +qa',
-             'nvim --headless ":TSUpdate" +qa'])
+             'nvim --headless ":TSUpdateSync" +qa'])
 
     print_sub_header('NeoVim Plugins installed.')
```

### Comparing `onboardme-1.1.8/onboardme/misc.py` & `onboardme-1.1.9/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/pkg_management.py` & `onboardme-1.1.9/onboardme/pkg_management.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/subproc.py` & `onboardme-1.1.9/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/onboardme/sudo_setup.py` & `onboardme-1.1.9/onboardme/sudo_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.1.8/pyproject.toml` & `onboardme-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.1.8"
+version       = "1.1.9"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
```

### Comparing `onboardme-1.1.8/PKG-INFO` & `onboardme-1.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.1.8
+Version: 1.1.9
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<4.0
@@ -139,19 +139,37 @@
 </p>
 
 </details>
 
 # Quick Start
 
 ### Prereq Installs
-You'll need `brew`, `git`, and Python 3.11 to get started. We have a setup script to install those and help you get your environment to the XDG spec under <b>Locally</b> or you can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).
+You'll need `curl`, `brew`, `git`, and Python 3.11 to get started. We have a setup script to install those (except `curl`) and help you get your environment to the XDG spec under <b>Locally</b> or you can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).
 
 <details>
   <summary>Local prereq install script</summary>
 
+
+<details>
+  <summary><code>curl</code>, a pre-prereq</summary>
+
+  ```bash
+  # First, make sure you have curl, but it *should* be there already be on macOS.
+  # if this doesn't return anything, you need to install curl
+  which curl
+
+  # Debian/Ubuntu may not have curl installed depending on where you are
+  sudo apt install -y curl
+  ```
+
+  If it's not there on Linux, you can install it with `apt` or use any default package manager like yum, or whatever people who use gentoo use.
+
+</details>
+
+Make sure you have sudo access, otherwise we won't be able to install certain things.
 The quickest way to get started on a fresh macOS or distro of Debian (including Ubuntu) is:
 ```bash
 # this will download setup.sh to your current directory and run it
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)"
 ```
 
 #### Linux
@@ -185,41 +203,37 @@
 chsh -s /usr/local/bin/bash $(whoami)
 ```
 
 After that, you can also set the shell directly in your terminal app via the settings.
 
 </details>
 
+#### Install
 
-<details>
-  <summary><code>jessebot/onboardme</code> docker image</summary>
+If you've already got brew and Python3.11 on your machine, you can just do:
+```bash
+# should also work with pipx, if you'd like to use that instead
+pip install --user --upgrade onboardme
+```
+
+### Using the Docker image
 
 To run the image locally with onboardme installed and already run using default settings:
 
 ```bash
 # this image is built daily and has already run onboardme with the default settings
-docker run jessebot/onboardme:latest /bin/bash
+docker run jessebot/onboardme:latest
 ```
 
 To run the image locally with onbaordme installed but _not_ run:
 
 ```bash
 # best if you have your own dot files, or need a smaller initial docker image to pull
 # no packages outside of the required pre-reqs for onboardme have been installed
-docker run jessebot/onboardme:no-install /bin/bash
-```
-
-</details>
-
-## Install
-
-If you've already got brew and Python3.11 on your machine, you can just do:
-```bash
-# should also work with pipx, if you'd like to use that instead
-pip install --user --upgrade onboardme
+docker run jessebot/onboardme:no-install
 ```
 
 ## Running commands
 
 _Now_ you can run `onboardme` 🎉 
 ```bash
 # this will display the help text for onboardme
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onboardme Version: 1.1.8 Summary: Install dot files
+Metadata-Version: 2.1 Name: onboardme Version: 1.1.9 Summary: Install dot files
 and packages, including a base mode with sensible defaults to run on most
 computers running Debian based distros or macOS. Home-page: http://github.com/
 jessebot/onboardme License: AGPL-3.0-or-later Keywords:
 onboardme,onboarding,desktop-setup,development-environment Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
@@ -61,92 +61,98 @@
                 [screenshot_of_full_output_of_onboardme_--help]
   Examples of the terminal after onboardme runs
 ### neovim [screenshot of neovim with colors] ### Powerline and ls [screenshot
  of powerline and lsd] ### Powerline with git [screenshot of powerline and git
   colors] ### Image and colors [screenshot of color samples and image of dog
   using a computer using sixel] ### Python virtual env in powerline and cat
          [screenshot of using bat and python virtual env in powerline]
- # Quick Start ### Prereq Installs You'll need `brew`, `git`, and Python 3.11
-to get started. We have a setup script to install those and help you get your
-environment to the XDG spec under Locally or you can just use our docker image,
-[jessebot/onboardme](https://hub.docker.com/r/jessebot/onboardme).  Local
-prereq install script The quickest way to get started on a fresh macOS or
-distro of Debian (including Ubuntu) is: ```bash # this will download setup.sh
-to your current directory and run it /bin/bash -c "$(curl -fsSL https://
+ # Quick Start ### Prereq Installs You'll need `curl`, `brew`, `git`, and
+Python 3.11 to get started. We have a setup script to install those (except
+`curl`) and help you get your environment to the XDG spec under Locally or you
+can just use our docker image, [jessebot/onboardme](https://hub.docker.com/r/
+jessebot/onboardme).  Local prereq install script  curl, a pre-prereq ```bash #
+First, make sure you have curl, but it *should* be there already be on macOS. #
+if this doesn't return anything, you need to install curl which curl # Debian/
+Ubuntu may not have curl installed depending on where you are sudo apt install
+-y curl ``` If it's not there on Linux, you can install it with `apt` or use
+any default package manager like yum, or whatever people who use gentoo use.
+Make sure you have sudo access, otherwise we won't be able to install certain
+things. The quickest way to get started on a fresh macOS or distro of Debian
+(including Ubuntu) is: ```bash # this will download setup.sh to your current
+directory and run it /bin/bash -c "$(curl -fsSL https://
 raw.githubusercontent.com/jessebot/onboardme/main/setup.sh)" ``` #### Linux
 Source your updated `.bashrc`: ```bash # for linux source ~/.bashrc ``` ####
 MacOS source your updated `.bash_profile`: ```bash bash source ~/.bash_profile
 ``` You will still have to set your default shell to BASH to if you want to
 take advantage of the default dot files for onboardme. You can do that like
 this: ```bash brew install bash sudo -i # if you're on an M1 or newer: echo "/
 opt/homebrew/bin/bash" >> /etc/shells && exit chsh -s /opt/homebrew/bin/bash $
 (whoami) # if you're on a mac earlier than the M1: echo "/usr/local/bin/bash"
 >> /etc/shells && exit chsh -s /usr/local/bin/bash $(whoami) ``` After that,
 you can also set the shell directly in your terminal app via the settings.
-jessebot/onboardme docker image To run the image locally with onboardme
-installed and already run using default settings: ```bash # this image is built
-daily and has already run onboardme with the default settings docker run
-jessebot/onboardme:latest /bin/bash ``` To run the image locally with onbaordme
-installed but _not_ run: ```bash # best if you have your own dot files, or need
-a smaller initial docker image to pull # no packages outside of the required
-pre-reqs for onboardme have been installed docker run jessebot/onboardme:no-
-install /bin/bash ```  ## Install If you've already got brew and Python3.11 on
-your machine, you can just do: ```bash # should also work with pipx, if you'd
-like to use that instead pip install --user --upgrade onboardme ``` ## Running
-commands _Now_ you can run `onboardme` ð ```bash # this will display the
-help text for onboardme onboardme --help # Running this won't overwrite any
-existing dot files, but it may add new ones. onboardme ``` From here, if you
-want to *completely wipe your existing dot files* for a fresh start with with
-`onboardme`, you can run: ```bash # WARNING: This will overwrite your local
-dotfiles, including your .bashrc and .bash_profile # can also be done with:
-onboardme -O onboardme --overwrite ``` You can read more in depth at the
-[Getting Started Docs] ð! There's also more [docs] on basically every
-program that onboardme touches. ### Upgrades If you're on python 3.11, you
-should be able to do: ```bash pip3.11 install --upgrade onboardme ``` ###
-Configuration onboardme has lots of CLI options, but you can also use config
-files. You have to create these files for the time being. Config files are in
-`$XDG_CONFIG_HOME/onboardme/`, or `~/.config/onboardme/` if `$XDG_CONFIG_HOME`
-is not defined. | Config File | Description | |:-------------------------------
------------|:----------------------------------------------------| |
-`$XDG_CONFIG_HOME/onboardme/config.yml` | For step configuration to run either
-all steps, or just a subset. | | `$XDG_CONFIG_HOME/onboardme/packages.yml` |
-For adding packages with different package managers | Examples:  ~/.config/
-onboardme/config.yml ```yaml log: # Full path to a file you'd like to log to.
-Creates file if it doesn't exist file: "" # what level of logs to output
-(DEBUG, INFO, WARN, ERROR) level: "INFO" # steps refer to a specific function
-in the list of functions we run steps: # these are mac specific steps Darwin: #
-clones dot files into home dir/git fetches updates for dot files - dot_files #
-install packages - packages # adds nerdfonts - font_setup # runs :Lazy sync to
-install all your plugins - neovim_setup # sets up touchID for sudo - sudo_setup
-# these are linux specific steps Linux: - dot_files - packages - font_setup -
-neovim_setup # add your user to the docker group - group_setup dot_files: #
-personal git repo URL for your dot files, defaults to jessebot/dot_files
-git_url: "https://github.com/jessebot/dot_files.git" # the branch to use for
-the git repo above, defaults to main git_branch: "main" # !CAREFUL: runs a `git
-reset --hard`, which will overwite/delete local files in ~ that # conflict with
-the above defined git repo url and branch. You should run # `onboardme -
-s dot_files` to get the files that would be overwritten overwrite: false #
-basic package config package: # Remove any of the below pkg managers to only
-run the remaining pkg managers managers: # these are macOS specific steps
-Darwin: - brew - pip3.11 # these are linux specific steps Linux: - brew -
-pip3.11 - apt - snap - flatpak # list of extra existing packages groups to
-install groups: - default # uncomment these to add them as default installed
-package groups # - gui # - gaming # - devops ```  ## Under the Hood Made and
-tested for these operating systems: [![Tested on Ventura 13.4 with a 13-inch M1
-Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro]
-(https://img.shields.io/badge/mac%20os-000000?style=for-the-
-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en) [!
-[Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/
-badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://
-www.debian.org/) [![Tested only on ubuntu servers](https://img.shields.io/
-badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://
-ubuntu.com/) And optomized for the following programs: [![made-with-neovim]
-(https://img.shields.io/badge/NeoVim-0f191f?style=for-the-
-badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/) [![made-with-python]
-(https://img.shields.io/badge/Python-FFD43B?style=for-the-
+#### Install If you've already got brew and Python3.11 on your machine, you can
+just do: ```bash # should also work with pipx, if you'd like to use that
+instead pip install --user --upgrade onboardme ``` ### Using the Docker image
+To run the image locally with onboardme installed and already run using default
+settings: ```bash # this image is built daily and has already run onboardme
+with the default settings docker run jessebot/onboardme:latest ``` To run the
+image locally with onbaordme installed but _not_ run: ```bash # best if you
+have your own dot files, or need a smaller initial docker image to pull # no
+packages outside of the required pre-reqs for onboardme have been installed
+docker run jessebot/onboardme:no-install ``` ## Running commands _Now_ you can
+run `onboardme` ð ```bash # this will display the help text for onboardme
+onboardme --help # Running this won't overwrite any existing dot files, but it
+may add new ones. onboardme ``` From here, if you want to *completely wipe your
+existing dot files* for a fresh start with with `onboardme`, you can run:
+```bash # WARNING: This will overwrite your local dotfiles, including your
+.bashrc and .bash_profile # can also be done with: onboardme -O onboardme --
+overwrite ``` You can read more in depth at the [Getting Started Docs] ð!
+There's also more [docs] on basically every program that onboardme touches. ###
+Upgrades If you're on python 3.11, you should be able to do: ```bash pip3.11
+install --upgrade onboardme ``` ### Configuration onboardme has lots of CLI
+options, but you can also use config files. You have to create these files for
+the time being. Config files are in `$XDG_CONFIG_HOME/onboardme/`, or
+`~/.config/onboardme/` if `$XDG_CONFIG_HOME` is not defined. | Config File |
+Description | |:------------------------------------------|:-------------------
+---------------------------------| | `$XDG_CONFIG_HOME/onboardme/config.yml` |
+For step configuration to run either all steps, or just a subset. | |
+`$XDG_CONFIG_HOME/onboardme/packages.yml` | For adding packages with different
+package managers | Examples:  ~/.config/onboardme/config.yml ```yaml log: #
+Full path to a file you'd like to log to. Creates file if it doesn't exist
+file: "" # what level of logs to output (DEBUG, INFO, WARN, ERROR) level:
+"INFO" # steps refer to a specific function in the list of functions we run
+steps: # these are mac specific steps Darwin: # clones dot files into home dir/
+git fetches updates for dot files - dot_files # install packages - packages #
+adds nerdfonts - font_setup # runs :Lazy sync to install all your plugins -
+neovim_setup # sets up touchID for sudo - sudo_setup # these are linux specific
+steps Linux: - dot_files - packages - font_setup - neovim_setup # add your user
+to the docker group - group_setup dot_files: # personal git repo URL for your
+dot files, defaults to jessebot/dot_files git_url: "https://github.com/
+jessebot/dot_files.git" # the branch to use for the git repo above, defaults to
+main git_branch: "main" # !CAREFUL: runs a `git reset --hard`, which will
+overwite/delete local files in ~ that # conflict with the above defined git
+repo url and branch. You should run # `onboardme -s dot_files` to get the files
+that would be overwritten overwrite: false # basic package config package: #
+Remove any of the below pkg managers to only run the remaining pkg managers
+managers: # these are macOS specific steps Darwin: - brew - pip3.11 # these are
+linux specific steps Linux: - brew - pip3.11 - apt - snap - flatpak # list of
+extra existing packages groups to install groups: - default # uncomment these
+to add them as default installed package groups # - gui # - gaming # - devops
+```  ## Under the Hood Made and tested for these operating systems: [![Tested
+on Ventura 13.4 with a 13-inch M1 Macbook pro and a 13-inch AMD 1,4 GHz Quad-
+Core Intel Core i5 2020 Macbook Pro](https://img.shields.io/badge/mac%20os-
+000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/
+wiki/MacOS?lang=en) [![Tested only on Debian Bookworm (debian:bookworm)](https:
+//img.shields.io/badge/Debian-A81D33?style=for-the-
+badge&logo=debian&logoColor=white)](https://www.debian.org/) [![Tested only on
+ubuntu servers](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-
+badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/) And optomized for the
+following programs: [![made-with-neovim](https://img.shields.io/badge/NeoVim-
+0f191f?style=for-the-badge&logo=neovim&logoColor=#5c983b)](https://neovim.io/)
+[![made-with-python](https://img.shields.io/badge/Python-FFD43B?style=for-the-
 badge&logo=python&logoColor=blue)](https://www.python.org/) [![made-with-bash]
 (https://img.shields.io/badge/GNU%20Bash-000000?style=for-the-
 badge&logo=GNU%20Bash&logoColor=#5c983b)](https://www.gnu.org/software/bash/)
 [![made-with-powerline](https://img.shields.io/badge/powerline-
 000000?style=for-the-badge&logo=powerline&logoColor=#5c983b)](https://
 powerline.readthedocs.io/en/master/overview.html) #### Built using these great
 tools: [[rich python library logo with with yellow snake]](https://github.com/
```

