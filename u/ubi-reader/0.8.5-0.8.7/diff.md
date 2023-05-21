# Comparing `tmp/ubi_reader-0.8.5.tar.gz` & `tmp/ubi_reader-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubi_reader-0.8.5.tar", last modified: Sun Dec  4 04:29:57 2022, max compression
+gzip compressed data, was "ubi_reader-0.8.7.tar", max compression
```

## Comparing `ubi_reader-0.8.5.tar` & `ubi_reader-0.8.7.tar`

### file list

```diff
@@ -1,44 +1,33 @@
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2022-12-04 04:29:57.324583 ubi_reader-0.8.5/
--rw-rw-r--   0 jason     (1000) jason     (1000)    35117 2017-02-13 21:08:59.000000 ubi_reader-0.8.5/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)      396 2022-12-04 04:29:57.324583 ubi_reader-0.8.5/PKG-INFO
--rwxr-xr-x   0 jason     (1000) jason     (1000)     5702 2022-12-04 04:07:48.000000 ubi_reader-0.8.5/README.md
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2022-12-04 04:29:57.320583 ubi_reader-0.8.5/scripts/
--rwxr-xr-x   0 jason     (1000) jason     (1000)     7401 2022-12-04 04:15:17.000000 ubi_reader-0.8.5/scripts/ubireader_display_blocks
--rwxr-xr-x   0 jason     (1000) jason     (1000)     7252 2022-12-04 04:15:17.000000 ubi_reader-0.8.5/scripts/ubireader_display_info
--rwxr-xr-x   0 jason     (1000) jason     (1000)     7530 2022-12-04 04:15:17.000000 ubi_reader-0.8.5/scripts/ubireader_extract_files
--rwxr-xr-x   0 jason     (1000) jason     (1000)     6549 2022-12-04 04:15:17.000000 ubi_reader-0.8.5/scripts/ubireader_extract_images
--rwxr-xr-x   0 jason     (1000) jason     (1000)     6690 2022-12-04 04:15:17.000000 ubi_reader-0.8.5/scripts/ubireader_list_files
--rwxr-xr-x   0 jason     (1000) jason     (1000)    13769 2022-12-04 04:15:17.000000 ubi_reader-0.8.5/scripts/ubireader_utils_info
--rw-r--r--   0 jason     (1000) jason     (1000)       38 2022-12-04 04:29:57.324583 ubi_reader-0.8.5/setup.cfg
--rwxr-xr-x   0 jason     (1000) jason     (1000)      875 2022-12-04 04:15:53.000000 ubi_reader-0.8.5/setup.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2022-12-04 04:29:57.320583 ubi_reader-0.8.5/ubi_reader.egg-info/
--rw-r--r--   0 jason     (1000) jason     (1000)      396 2022-12-04 04:29:57.000000 ubi_reader-0.8.5/ubi_reader.egg-info/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)      894 2022-12-04 04:29:57.000000 ubi_reader-0.8.5/ubi_reader.egg-info/SOURCES.txt
--rw-r--r--   0 jason     (1000) jason     (1000)        1 2022-12-04 04:29:57.000000 ubi_reader-0.8.5/ubi_reader.egg-info/dependency_links.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       10 2022-12-04 04:29:57.000000 ubi_reader-0.8.5/ubi_reader.egg-info/top_level.txt
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2022-12-04 04:29:57.320583 ubi_reader-0.8.5/ubireader/
--rwxrwxr-x   0 jason     (1000) jason     (1000)        0 2017-02-13 21:08:59.000000 ubi_reader-0.8.5/ubireader/__init__.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     1892 2022-12-03 21:54:47.000000 ubi_reader-0.8.5/ubireader/debug.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     1575 2022-12-04 00:38:02.000000 ubi_reader-0.8.5/ubireader/settings.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2022-12-04 04:29:57.320583 ubi_reader-0.8.5/ubireader/ubi/
--rwxr-xr-x   0 jason     (1000) jason     (1000)     6725 2022-12-04 02:35:53.000000 ubi_reader-0.8.5/ubireader/ubi/__init__.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2022-12-04 04:29:57.324583 ubi_reader-0.8.5/ubireader/ubi/block/
--rwxr-xr-x   0 jason     (1000) jason     (1000)     8700 2022-12-04 00:33:05.000000 ubi_reader-0.8.5/ubireader/ubi/block/__init__.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     2181 2022-12-04 01:29:03.000000 ubi_reader-0.8.5/ubireader/ubi/block/layout.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4043 2022-12-04 00:43:17.000000 ubi_reader-0.8.5/ubireader/ubi/block/sort.py
--rw-r--r--   0 jason     (1000) jason     (1000)     4867 2019-05-09 06:33:26.000000 ubi_reader-0.8.5/ubireader/ubi/defines.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     5443 2019-05-09 06:33:26.000000 ubi_reader-0.8.5/ubireader/ubi/display.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     3683 2022-12-01 19:21:47.000000 ubi_reader-0.8.5/ubireader/ubi/headers.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     2132 2022-12-02 02:39:40.000000 ubi_reader-0.8.5/ubireader/ubi/image.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     3923 2022-12-04 00:43:14.000000 ubi_reader-0.8.5/ubireader/ubi/volume.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     7684 2022-12-04 00:40:15.000000 ubi_reader-0.8.5/ubireader/ubi_io.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2022-12-04 04:29:57.324583 ubi_reader-0.8.5/ubireader/ubifs/
--rwxr-xr-x   0 jason     (1000) jason     (1000)     5161 2022-12-04 00:39:09.000000 ubi_reader-0.8.5/ubireader/ubifs/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)    19399 2021-03-26 00:46:48.000000 ubi_reader-0.8.5/ubireader/ubifs/defines.py
--rw-r--r--   0 jason     (1000) jason     (1000)     5071 2022-12-04 00:40:23.000000 ubi_reader-0.8.5/ubireader/ubifs/display.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     5672 2022-12-04 02:35:53.000000 ubi_reader-0.8.5/ubireader/ubifs/list.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     2421 2022-12-04 00:40:41.000000 ubi_reader-0.8.5/ubireader/ubifs/misc.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     7982 2022-09-06 07:32:41.000000 ubi_reader-0.8.5/ubireader/ubifs/nodes.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     7759 2022-12-04 02:38:14.000000 ubi_reader-0.8.5/ubireader/ubifs/output.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     5990 2022-12-01 19:21:47.000000 ubi_reader-0.8.5/ubireader/ubifs/walk.py
--rwxr-xr-x   0 jason     (1000) jason     (1000)     5342 2022-12-04 02:40:21.000000 ubi_reader-0.8.5/ubireader/utils.py
+-rw-r--r--   0        0        0    35117 2023-05-21 19:46:21.693206 ubi_reader-0.8.7/LICENSE
+-rwxr-xr-x   0        0        0     5551 2023-05-21 19:46:21.693206 ubi_reader-0.8.7/README.md
+-rw-r--r--   0        0        0     1179 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/__init__.py
+-rwxr-xr-x   0        0        0     1892 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/debug.py
+-rw-r--r--   0        0        0        1 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/scripts/__init__.py
+-rwxr-xr-x   0        0        0     7425 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/scripts/ubireader_display_blocks.py
+-rwxr-xr-x   0        0        0     7275 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/scripts/ubireader_display_info.py
+-rwxr-xr-x   0        0        0     7554 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/scripts/ubireader_extract_files.py
+-rwxr-xr-x   0        0        0     6572 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/scripts/ubireader_extract_images.py
+-rwxr-xr-x   0        0        0     6714 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/scripts/ubireader_list_files.py
+-rwxr-xr-x   0        0        0    13792 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/scripts/ubireader_utils_info.py
+-rwxr-xr-x   0        0        0     1575 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/settings.py
+-rwxr-xr-x   0        0        0     6725 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubi/__init__.py
+-rwxr-xr-x   0        0        0     8700 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubi/block/__init__.py
+-rwxr-xr-x   0        0        0     2181 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubi/block/layout.py
+-rw-r--r--   0        0        0     4043 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubi/block/sort.py
+-rw-r--r--   0        0        0     4867 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubi/defines.py
+-rwxr-xr-x   0        0        0     5443 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubi/display.py
+-rwxr-xr-x   0        0        0     3683 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubi/headers.py
+-rwxr-xr-x   0        0        0     2132 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubi/image.py
+-rwxr-xr-x   0        0        0     3923 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubi/volume.py
+-rwxr-xr-x   0        0        0     7684 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubi_io.py
+-rwxr-xr-x   0        0        0     5161 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubifs/__init__.py
+-rw-r--r--   0        0        0    19399 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubifs/defines.py
+-rw-r--r--   0        0        0     5071 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubifs/display.py
+-rwxr-xr-x   0        0        0     5672 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubifs/list.py
+-rwxr-xr-x   0        0        0     2465 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubifs/misc.py
+-rwxr-xr-x   0        0        0     7982 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubifs/nodes.py
+-rwxr-xr-x   0        0        0     7759 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubifs/output.py
+-rwxr-xr-x   0        0        0     5990 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/ubifs/walk.py
+-rwxr-xr-x   0        0        0     5342 2023-05-21 19:46:21.697206 ubi_reader-0.8.7/ubireader/utils.py
+-rw-r--r--   0        0        0     6132 1970-01-01 00:00:00.000000 ubi_reader-0.8.7/PKG-INFO
```

### Comparing `ubi_reader-0.8.5/LICENSE` & `ubi_reader-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/README.md` & `ubi_reader-0.8.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,33 +18,25 @@
 The testing branch includes a tools/ directory, that has scripts to help when trying to extract data from broken images. These also serve as examples of how to use parts of ubi_reader in custom scripts.
 
 An override system is also included, for manually setting certain parameters that may be reported wrong by the UBI/FS data.
 
 This branch will probably remain seperate, as it is meant to be customized to aid in extracting data from problematic images. You can install it with 'python setup.py develop' to make it easier to modify ubi_reader as needed.
 
 
-## Dependencies:
-
-Python 2.7 or 3 with the following packages:
-
-    $ sudo apt-get install liblzo2-dev
-    $ sudo pip install python-lzo
-
-
 ## Installation:
 
 Latest Version
 
     $ git clone https://github.com/jrspruitt/ubi_reader
     $ cd ubi_reader
-    $ sudo python setup.py install
+    $ poetry install
 
 Or
 
-    $ sudo pip install ubi_reader
+    $ pip install --user ubi_reader
 
 
 ## Usage:
 For basic usage, the scripts need no options and if applicable will save output
 to ./ubifs-root/. More advanced usage can set start and end offset, specify
 an output directory, or for debugging can print out what it is doing to the
 terminal.
```

### Comparing `ubi_reader-0.8.5/scripts/ubireader_display_blocks` & `ubi_reader-0.8.7/ubireader/scripts/ubireader_display_blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from ubireader.ubi import ubi_base
 from ubireader.ubi_io import ubi_file
 from ubireader import settings
 from ubireader.ubi.defines import UBI_EC_HDR_MAGIC
 from ubireader.ubifs.defines import UBIFS_NODE_MAGIC
 from ubireader.utils import guess_filetype, guess_start_offset, guess_leb_size, guess_peb_size
 
-if __name__=='__main__':
 
+def main():
     description = 'Search for specified blocks and display information.'
     usage = """
     ubireader_display_blocks "{'block.attr': value,...}" path/to/image
         Search for blocks by given parameters and display information about them.
         This is block only, no volume or image information is created, which can
         be used to debug file and image extraction.
     Example:
@@ -184,7 +184,10 @@
         if match:                
             blocks.append(ubi_obj.blocks[block])
 
     print('\nBlock matches: %s' % len(blocks))
 
     for block in blocks:
         print(block.display())
+
+if __name__=='__main__':
+    main()
```

### Comparing `ubi_reader-0.8.5/scripts/ubireader_display_info` & `ubi_reader-0.8.7/ubireader/scripts/ubireader_display_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 from ubireader.ubi import ubi
 from ubireader.ubi.defines import UBI_EC_HDR_MAGIC
 from ubireader.ubifs import ubifs
 from ubireader.ubifs.defines import UBIFS_NODE_MAGIC
 from ubireader.utils import guess_filetype, guess_start_offset, guess_leb_size, guess_peb_size
 from ubireader.ubi_io import ubi_file, leb_virtual_file
 
-
-if __name__=='__main__':
+def main():
     start = time.time()
     description = 'Show information about UBI or UBIFS image.'
     usage = 'ubireader_display_info [options] filepath'
     parser = argparse.ArgumentParser(usage=usage, description=description)
 
     parser.add_argument('-l', '--log', action='store_true', dest='log',
                       help='Print extraction information to screen.')
@@ -181,7 +180,10 @@
         try:
             print(ubifs_obj.master_node2.display('\t'))
         except:
             print('Master Node Error only one valid node.')
 
     else:
         print('Something went wrong to get here.')
+
+if __name__=='__main__':
+    main()
```

### Comparing `ubi_reader-0.8.5/scripts/ubireader_extract_files` & `ubi_reader-0.8.7/ubireader/scripts/ubireader_extract_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,15 @@
     else:
         try:
             os.makedirs(outpath)
             log(create_output_dir, 'Created output path: %s' % outpath)
         except Exception as e:
             error(create_output_dir, 'Fatal', '%s' % e)
 
-
-if __name__=='__main__':
+def main():
     start = time.time()
     description = 'Extract contents of a UBI or UBIFS image.'
     usage = 'ubireader_extract_files [options] filepath'
     parser = argparse.ArgumentParser(usage=usage, description=description)
 
     parser.add_argument('-k', '--keep-permissions', action='store_true', dest='permissions',
                       help='Maintain file permissions, requires running as root. (default: False)')
@@ -194,7 +193,11 @@
 
         # Extract files from UBIFS image.
         print('Extracting files to: %s' % outpath)
         extract_files(ubifs_obj, outpath, perms)
 
     else:
         print('Something went wrong to get here.')
+
+
+if __name__=='__main__':
+    main()
```

### Comparing `ubi_reader-0.8.5/scripts/ubireader_extract_images` & `ubi_reader-0.8.7/ubireader/scripts/ubireader_extract_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     if not os.path.exists(outpath):
         try:
             os.makedirs(outpath)
             log(create_output_dir, 'Created output path: %s' % outpath)
         except Exception as e:
             error(create_output_dir, 'Fatal', '%s' % e)
 
-
-if __name__=='__main__':
+def main():
     start = time.time()
     description = 'Extract UBI or UBIFS images from file containing UBI data in it.'
     usage = 'ubireader_extract_images [options] filepath'
     parser = argparse.ArgumentParser(usage=usage, description=description)
 
     parser.add_argument('-l', '--log', action='store_true', dest='log',
                       help='Print extraction information to screen.')
@@ -163,7 +162,10 @@
                 vol_outpath = os.path.join(outpath, 'img-%s_vol-%s.ubifs' % (image.image_seq, volume))
                 create_output_dir(outpath)
                 f = open(vol_outpath, 'wb')
 
                 # Loop through and write volume block data (LEB) to file.
                 for block in image.volumes[volume].reader(ubi_obj):
                     f.write(block)
+
+if __name__=='__main__':
+    main()
```

### Comparing `ubi_reader-0.8.5/scripts/ubireader_list_files` & `ubi_reader-0.8.7/ubireader/scripts/ubireader_list_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from ubireader.ubifs import ubifs
 from ubireader.ubifs.list import list_files, copy_file
 from ubireader.ubifs.defines import UBIFS_NODE_MAGIC
 from ubireader.ubi_io import ubi_file, leb_virtual_file
 from ubireader.debug import error, log
 from ubireader.utils import guess_filetype, guess_start_offset, guess_leb_size, guess_peb_size
 
-if __name__=='__main__':
+def main():
     start = time.time()
     description = 'List and Extract files of a UBI or UBIFS image.'
     usage = 'ubireader_list_files [options] filepath'
     parser = argparse.ArgumentParser(usage=usage, description=description)
 
     parser.add_argument('-l', '--log', action='store_true', dest='log',
                       help='Print extraction information to screen.')
@@ -168,7 +168,10 @@
         if args.listpath:
             list_files(ubifs_obj, args.listpath)
         if args.copyfile and args.copyfiledest:
             copy_file(ubifs_obj, args.copyfile, args.copyfiledest)
 
     else:
         print('Something went wrong to get here.')
+
+if __name__=='__main__':
+    main()
```

### Comparing `ubi_reader-0.8.5/scripts/ubireader_utils_info` & `ubi_reader-0.8.7/ubireader/scripts/ubireader_utils_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
             for flag in ubinize_flags:
                 argstr += ' %s %s' % (ubi_flags[flag], ubi_args[flag])
 
             buf += '/usr/sbin/ubinize%s -o %s %s\n' % (argstr, ubi_file, ini_file)
             fscr.write(buf)
         os.chmod(script_path, 0o755)
 
-if __name__=='__main__':
+def main():
     start = time.time()
     description = 'Determine settings for recreating UBI image.'
     usage = 'ubireader_utils_info [options] filepath'
     parser = argparse.ArgumentParser(usage=usage, description=description)
 
     parser.add_argument('-r', '--show-only', action='store_true', dest='show_only',
                       help='Print parameters to screen only. (default: false)')
@@ -339,7 +339,9 @@
     print_ubi_params(ubi_obj)
 
     if not args.show_only:
         create_output_dir(outpath)
         # Create build scripts.
         make_files(ubi_obj, outpath)
 
+if __name__=='__main__':
+    main()
```

### Comparing `ubi_reader-0.8.5/ubireader/debug.py` & `ubi_reader-0.8.7/ubireader/debug.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/settings.py` & `ubi_reader-0.8.7/ubireader/settings.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubi/__init__.py` & `ubi_reader-0.8.7/ubireader/ubi/__init__.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubi/block/__init__.py` & `ubi_reader-0.8.7/ubireader/ubi/block/__init__.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubi/block/layout.py` & `ubi_reader-0.8.7/ubireader/ubi/block/layout.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubi/block/sort.py` & `ubi_reader-0.8.7/ubireader/ubi/block/sort.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubi/defines.py` & `ubi_reader-0.8.7/ubireader/ubi/defines.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubi/display.py` & `ubi_reader-0.8.7/ubireader/ubi/display.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubi/headers.py` & `ubi_reader-0.8.7/ubireader/ubi/headers.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubi/image.py` & `ubi_reader-0.8.7/ubireader/ubi/image.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubi/volume.py` & `ubi_reader-0.8.7/ubireader/ubi/volume.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubi_io.py` & `ubi_reader-0.8.7/ubireader/ubi_io.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubifs/__init__.py` & `ubi_reader-0.8.7/ubireader/ubifs/__init__.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubifs/defines.py` & `ubi_reader-0.8.7/ubireader/ubifs/defines.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubifs/display.py` & `ubi_reader-0.8.7/ubireader/ubifs/display.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubifs/list.py` & `ubi_reader-0.8.7/ubireader/ubifs/list.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubifs/misc.py` & `ubi_reader-0.8.7/ubireader/ubifs/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #############################################################
 
-import lzo
+from lzallright.lzallright import LZOCompressor as lzo
 import struct
 import zlib
 from ubireader.ubifs.defines import *
 from ubireader.debug import error
 
 # For happy printing
 ino_types = ['file', 'dir','lnk','blk','chr','fifo','sock']
```

### Comparing `ubi_reader-0.8.5/ubireader/ubifs/nodes.py` & `ubi_reader-0.8.7/ubireader/ubifs/nodes.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubifs/output.py` & `ubi_reader-0.8.7/ubireader/ubifs/output.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/ubifs/walk.py` & `ubi_reader-0.8.7/ubireader/ubifs/walk.py`

 * *Files identical despite different names*

### Comparing `ubi_reader-0.8.5/ubireader/utils.py` & `ubi_reader-0.8.7/ubireader/utils.py`

 * *Files identical despite different names*

