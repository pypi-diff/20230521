# Comparing `tmp/tsutsuji_trackcomputer-1.6.0-py3-none-any.whl.zip` & `tmp/tsutsuji_trackcomputer-1.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 58077 bytes, number of entries: 21
+Zip file size: 58426 bytes, number of entries: 21
 -rw-r--r--  2.0 unx        0 b- defN 21-Aug-22 02:52 tsutsuji/__init__.py
 -rw-r--r--  2.0 unx      647 b- defN 21-Sep-01 10:48 tsutsuji/__main__.py
--rw-r--r--  2.0 unx       22 b- defN 23-May-06 01:49 tsutsuji/_version.py
--rw-r--r--  2.0 unx    26141 b- defN 22-Sep-11 03:22 tsutsuji/backimg.py
+-rw-r--r--  2.0 unx       22 b- defN 23-May-20 05:19 tsutsuji/_version.py
+-rw-r--r--  2.0 unx    26323 b- defN 23-May-20 13:13 tsutsuji/backimg.py
 -rw-r--r--  2.0 unx     5514 b- defN 22-Nov-23 06:36 tsutsuji/config.py
 -rw-r--r--  2.0 unx     2155 b- defN 22-Apr-09 01:12 tsutsuji/cui2.py
 -rw-r--r--  2.0 unx     5753 b- defN 23-May-06 01:49 tsutsuji/curvetrackplot.py
 -rw-r--r--  2.0 unx    17026 b- defN 22-Sep-11 03:22 tsutsuji/drawcursor.py
 -rw-r--r--  2.0 unx    19787 b- defN 23-May-06 01:49 tsutsuji/gui_tsutsuji.py
 -rw-r--r--  2.0 unx     5060 b- defN 22-Sep-11 03:22 tsutsuji/kml2track.py
--rw-r--r--  2.0 unx     5551 b- defN 22-Nov-23 06:36 tsutsuji/kp_offset.py
+-rw-r--r--  2.0 unx     6311 b- defN 23-May-21 01:02 tsutsuji/kp_offset.py
 -rw-r--r--  2.0 unx    13102 b- defN 23-May-06 01:49 tsutsuji/math.py
 -rw-r--r--  2.0 unx    28724 b- defN 23-May-06 01:49 tsutsuji/measure.py
 -rw-r--r--  2.0 unx    69046 b- defN 23-May-06 01:49 tsutsuji/solver.py
--rw-r--r--  2.0 unx    34854 b- defN 23-May-06 01:49 tsutsuji/track_control.py
+-rw-r--r--  2.0 unx    35058 b- defN 23-May-21 01:45 tsutsuji/track_control.py
 -rw-r--r--  2.0 unx    10318 b- defN 22-Sep-11 03:22 tsutsuji/trackwindow.py
--rw-r--r--  2.0 unx     9723 b- defN 23-May-06 02:04 tsutsuji_trackcomputer-1.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3468 b- defN 23-May-06 02:04 tsutsuji_trackcomputer-1.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 02:04 tsutsuji_trackcomputer-1.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-06 02:04 tsutsuji_trackcomputer-1.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1702 b- defN 23-May-06 02:04 tsutsuji_trackcomputer-1.6.0.dist-info/RECORD
-21 files, 258694 bytes uncompressed, 55335 bytes compressed:  78.6%
+-rw-r--r--  2.0 unx     9723 b- defN 23-May-21 02:00 tsutsuji_trackcomputer-1.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3468 b- defN 23-May-21 02:00 tsutsuji_trackcomputer-1.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 02:00 tsutsuji_trackcomputer-1.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-21 02:00 tsutsuji_trackcomputer-1.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1702 b- defN 23-May-21 02:00 tsutsuji_trackcomputer-1.6.1.dist-info/RECORD
+21 files, 259840 bytes uncompressed, 55684 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: tsutsuji/track_control.py
 Comment: 
 
 Filename: tsutsuji/trackwindow.py
 Comment: 
 
-Filename: tsutsuji_trackcomputer-1.6.0.dist-info/LICENSE
+Filename: tsutsuji_trackcomputer-1.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: tsutsuji_trackcomputer-1.6.0.dist-info/METADATA
+Filename: tsutsuji_trackcomputer-1.6.1.dist-info/METADATA
 Comment: 
 
-Filename: tsutsuji_trackcomputer-1.6.0.dist-info/WHEEL
+Filename: tsutsuji_trackcomputer-1.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: tsutsuji_trackcomputer-1.6.0.dist-info/top_level.txt
+Filename: tsutsuji_trackcomputer-1.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tsutsuji_trackcomputer-1.6.0.dist-info/RECORD
+Filename: tsutsuji_trackcomputer-1.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tsutsuji/_version.py

```diff
@@ -1 +1 @@
-__version__ = '1.6.0'
+__version__ = '1.6.1'
```

## tsutsuji/backimg.py

```diff
@@ -399,131 +399,145 @@
     def sendtopmost(self,event=None):
         self.master.lift()
         self.master.focus_force()
     def closewindow(self):
         self.master.withdraw()
         self.master = None
         self.mainwindow.sendtopmost()
-    def getimg(self, scalex, as_ratio):
+    def getimg(self, scalex, as_ratio, maptilenumwarning=36):
         if False:
             import pdb
             pdb.set_trace()
 
-        if self.toshow:
-            self.img = None
+        if not self.toshow:
+            return
 
-            if '{z}' not in self.template_url or \
-               '{x}' not in self.template_url or \
-               '{y}' not in self.template_url:
-                raise Exception('Invalid template_url')
-            else:
-                url_base = self.template_url.replace('{z}', '{:d}').replace('{x}', '{:d}').replace('{y}', '{:d}')
-
-            width = scalex
-            height = scalex*as_ratio
-
-            if self.autozoom:
-                
-                tilenumx = int(width/123)
-                zoom = 18 - int(np.sqrt((tilenumx/2)))
-                '''
+        if '{z}' not in self.template_url or \
+           '{x}' not in self.template_url or \
+           '{y}' not in self.template_url:
+            raise Exception('Invalid template_url')
+        else:
+            url_base = self.template_url.replace('{z}', '{:d}').replace('{x}', '{:d}').replace('{y}', '{:d}')
+
+        width = scalex
+        height = scalex*as_ratio
+
+        if self.autozoom:
+
+            tilenumx = int(width/123)
+            zoom = 18 - int(np.sqrt((tilenumx/2)))
+            '''
+            zoom = 18
+            for count in range(1,18):
+                tilenumx = int(width/(123*count))
+                if tilenumx**2 <= 8:
+                    zoom = 18-(count-1)
+                    break
+            '''
+            if zoom > 18:
                 zoom = 18
-                for count in range(1,18):
-                    tilenumx = int(width/(123*count))
-                    if tilenumx**2 <= 8:
-                        zoom = 18-(count-1)
-                        break
-                '''
-                if zoom > 18:
-                    zoom = 18
-                if zoom < 0:
-                    zoom = 0
-            else:
-                zoom = self.zoom
-
-            # 基準となる緯度経度をorigin_metricだけオフセット
-            origin = math.calc_xy2pl(self.origin_metric[1],\
-                                     -self.origin_metric[0],\
-                                     self.origin_longlat[1],\
-                                     self.origin_longlat[0])
-            origin = [origin[1],origin[0]]
-
-            canvas_center = [self.mainwindow.viewpos_v[0].get(),\
-                             self.mainwindow.viewpos_v[1].get()]
-
-            # プロット画面の左上(lu)、右下(rd)座標を求め、緯度経度に変換する
-            border_lu = math.calc_xy2pl(-(-height/2 + canvas_center[1]),\
-                                        (-width/2 + canvas_center[0]),\
-                                        origin[1],\
-                                        origin[0])
-            border_rd = math.calc_xy2pl(-(height/2 + canvas_center[1]),\
-                                        (width/2 + canvas_center[0]),\
-                                        origin[1],\
-                                        origin[0])
-
-            # プロット画面の左上、右下を含むマップタイル座標を求める
-            # (1)座標を緯度経度->ピクセル座標に変換、(2)タイル座標に変換、(3)タイル内での相対位置を求める
-            px_lu = [math.long2px(border_lu[1],zoom), math.lat2py(border_lu[0],zoom)]
-            tile_lu =[int(px_lu[0]/256), int(px_lu[1]/256)]
-            rel_lu = [px_lu[0]%256, px_lu[1]%256]
-
-            px_rd = [math.long2px(border_rd[1],zoom), math.lat2py(border_rd[0],zoom)]
-            tile_rd =[int(px_rd[0]/256), int(px_rd[1]/256)]
-            rel_rd = [px_rd[0]%256, px_rd[1]%256]
-
-            # 右上、左下を含むタイルの端点座標をm単位で求める
-            pos_tile_corner = {}
-            pos_tile_corner['lu'] = math.calc_pl2xy(math.py2lat(tile_lu[1]*256, zoom),\
-                                                    math.px2long((tile_lu[0])*256, zoom),\
-                                                    origin[1],\
-                                                    origin[0])
-            pos_tile_corner['rd'] = math.calc_pl2xy(math.py2lat((tile_rd[1]+1)*256, zoom),\
-                                                    math.px2long((tile_rd[0]+1)*256, zoom),\
-                                                    origin[1],\
-                                                    origin[0])
-
-            # 取得するマップタイルの表示範囲
-            extent = [pos_tile_corner['lu'][1],\
-                      pos_tile_corner['rd'][1], \
-                      -pos_tile_corner['lu'][0],\
-                      -pos_tile_corner['rd'][0]]
-
-            # マップタイルデータ取得
-            x_min = tile_lu[0]
-            x_max = tile_rd[0]
-            y_min = tile_lu[1]
-            y_max = tile_rd[1]
-
-            x_num = x_max-x_min +1
-            y_num = y_max-y_min +1
-
-            result = Image.new('RGB', (256*x_num, 256*y_num), (0,0,0))
-
-            counts = 0
-            for i in range(0,x_num):
-                for j in range(0,y_num):
-                    url_toget = url_base.format(zoom,x_min+i,y_min+j)
-
-                    try:
-                        if url_toget not in self.img_cache.keys():
-                            self.img_cache[url_toget] = Image.open(io.BytesIO(requests.get(url_toget, timeout=(10.0,10.0)).content))
-                            message = ''
-                        else:
-                            message = 'cached'
-                        result.paste(self.img_cache[url_toget], (256*i, 256*j))
-                    except Exception as e:
-                        message = 'ERROR' #e
-
-                    print('{:d}/{:d}'.format(counts+1,x_num*y_num),url_toget,message)
-                    counts +=1
-            print('Done')
-
-            self.img = result
-            self.extent = extent
-            self.filename = 'x{:d}y{:d}z{:d}'.format(x_min,y_min,zoom)
+            if zoom < 0:
+                zoom = 0
+        else:
+            zoom = self.zoom
+
+        # 基準となる緯度経度をorigin_metricだけオフセット
+        origin = math.calc_xy2pl(self.origin_metric[1],\
+                                 -self.origin_metric[0],\
+                                 self.origin_longlat[1],\
+                                 self.origin_longlat[0])
+        origin = [origin[1],origin[0]]
+
+        canvas_center = [self.mainwindow.viewpos_v[0].get(),\
+                         self.mainwindow.viewpos_v[1].get()]
+
+        # プロット画面の左上(lu)、右下(rd)座標を求め、緯度経度に変換する
+        border_lu = math.calc_xy2pl(-(-height/2 + canvas_center[1]),\
+                                    (-width/2 + canvas_center[0]),\
+                                    origin[1],\
+                                    origin[0])
+        border_rd = math.calc_xy2pl(-(height/2 + canvas_center[1]),\
+                                    (width/2 + canvas_center[0]),\
+                                    origin[1],\
+                                    origin[0])
+
+        # プロット画面の左上、右下を含むマップタイル座標を求める
+        # (1)座標を緯度経度->ピクセル座標に変換、(2)タイル座標に変換、(3)タイル内での相対位置を求める
+        px_lu = [math.long2px(border_lu[1],zoom), math.lat2py(border_lu[0],zoom)]
+        tile_lu =[int(px_lu[0]/256), int(px_lu[1]/256)]
+        rel_lu = [px_lu[0]%256, px_lu[1]%256]
+
+        px_rd = [math.long2px(border_rd[1],zoom), math.lat2py(border_rd[0],zoom)]
+        tile_rd =[int(px_rd[0]/256), int(px_rd[1]/256)]
+        rel_rd = [px_rd[0]%256, px_rd[1]%256]
+
+        # 右上、左下を含むタイルの端点座標をm単位で求める
+        pos_tile_corner = {}
+        pos_tile_corner['lu'] = math.calc_pl2xy(math.py2lat(tile_lu[1]*256, zoom),\
+                                                math.px2long((tile_lu[0])*256, zoom),\
+                                                origin[1],\
+                                                origin[0])
+        pos_tile_corner['rd'] = math.calc_pl2xy(math.py2lat((tile_rd[1]+1)*256, zoom),\
+                                                math.px2long((tile_rd[0]+1)*256, zoom),\
+                                                origin[1],\
+                                                origin[0])
+
+        # 取得するマップタイルの表示範囲
+        extent = [pos_tile_corner['lu'][1],\
+                  pos_tile_corner['rd'][1], \
+                  -pos_tile_corner['lu'][0],\
+                  -pos_tile_corner['rd'][0]]
+
+        # マップタイルデータ取得
+        x_min = tile_lu[0]
+        x_max = tile_rd[0]
+        y_min = tile_lu[1]
+        y_max = tile_rd[1]
+
+        x_num = x_max-x_min +1
+        y_num = y_max-y_min +1
+
+        imgnum = 0
+        for i in range(0,x_num):
+            for j in range(0,y_num):
+                url_toget = url_base.format(zoom,x_min+i,y_min+j)
+
+                if url_toget not in self.img_cache.keys():
+                    imgnum +=1
+
+        if imgnum > maptilenumwarning:
+            if not tk.messagebox.askokcancel('get {:d} maptiles'.format(imgnum),'{:d} 枚のmaptileをダウンロードします。続行しますか？'.format(imgnum)):
+                print('Cancelled')
+                return
+        
+        self.img = None
+        result = Image.new('RGB', (256*x_num, 256*y_num), (0,0,0))
+
+        counts = 0
+        for i in range(0,x_num):
+            for j in range(0,y_num):
+                url_toget = url_base.format(zoom,x_min+i,y_min+j)
+
+                try:
+                    if url_toget not in self.img_cache.keys():
+                        self.img_cache[url_toget] = Image.open(io.BytesIO(requests.get(url_toget, timeout=(10.0,10.0)).content))
+                        message = ''
+                    else:
+                        message = 'cached'
+                    result.paste(self.img_cache[url_toget], (256*i, 256*j))
+                except Exception as e:
+                    message = 'ERROR' #e
+
+                print('{:d}/{:d}'.format(counts+1,x_num*y_num),url_toget,message)
+                counts +=1
+        print('Done')
+
+        self.img = result
+        self.extent = extent
+        self.filename = 'x{:d}y{:d}z{:d}'.format(x_min,y_min,zoom)
     def showimg(self,ax,as_ratio=1,ymag=1):
         if self.toshow and self.img is not None:
             ax.imshow(self.img,alpha=self.alpha,extent=[self.extent[0],self.extent[1],self.extent[3],self.extent[2]],aspect=ymag)
     def setparams_fromcfg(self, cfgd):
         if cfgd is not None:
             self.toshow = cfgd['toshow']
             self.alpha = cfgd['alpha']
```

## tsutsuji/kp_offset.py

```diff
@@ -19,15 +19,15 @@
 
 import os
 import sys
 import pathlib
 import re
 import argparse
 
-from lark import Lark, Transformer, v_args
+from lark import Lark, Transformer, v_args, Visitor
 
 from kobushi import loadmapgrammer as lgr
 from kobushi import loadheader as lhe
 
 def readfile(filename, offset_label, offset_val, result_list, input_root, include_file=None, inverse_kp = False):
     '''マップファイルを読み込み、距離程に指定のラベルを加算した文字列を生成する
     
@@ -49,14 +49,26 @@
       Trueの場合、読み込んだ距離程を-1倍して出力する
     -----
 
     result_listのフォーマット
       [{'filename':str, 'data':str}, ...]
     
     '''
+    if False:
+        import pdb
+        pdb.set_trace()
+
+    class detectDistance(Visitor):
+        def __init__(self, *args, **kwargs):
+            super().__init__()
+            self.isdistance = args[0]
+        def call_predefined_variable(self, tree):
+            if tree.children[0].value == 'distance':
+                self.isdistance[0] = True
+    
     path, rootpath, header_enc = lhe.loadheader(filename, 'BveTs Map ',2)
     fp = open(path,'r',encoding=header_enc)
     fp.readline()
     fbuff = fp.read()
     fp.close()
 
     output = 'BveTs Map 2.02\n'
@@ -83,18 +95,26 @@
                                offset_label,\
                                offset_val,\
                                result_list,\
                                input_root = input_root,\
                                include_file = re.sub('\'','',tree.children[0].children[0]))
                     output += pre_elem + elem + ';'
                 elif tree.data == 'set_distance':
-                    if inverse_kp:
-                        output += pre_elem + offset_label + ' - ({:s})'.format(elem) + ';'
+                    isdistance = [False]
+                    detectDistance(isdistance).visit(tree)
+                    if not isdistance[0]:
+                        if inverse_kp:
+                            output += pre_elem + offset_label + ' - ({:s})'.format(elem) + ';'
+                        else:
+                            output += pre_elem + offset_label + ' + ' +  elem + ';'
                     else:
-                        output += pre_elem + offset_label + ' + ' +  elem + ';'
+                        if inverse_kp:
+                            output += pre_elem + ' - ({:s})'.format(elem) + ';'
+                        else:
+                            output += pre_elem +  elem + ';'
                 else:
                     output += pre_elem + elem + ';'
             else:
                 output += pre_elem
         
         if ix_comm < len(comm):
             output += comm[ix_comm]
```

## tsutsuji/track_control.py

```diff
@@ -574,17 +574,19 @@
         if False:
             import pdb
             pdb.set_trace()
 
         # generate結果をincludeする擬似マップファイルを生成
         output_file = ''
 
-        path = self.conf.track_data[self.conf.general['owntrack']]['file']
+        # 自軌道ファイルをinclude
+        path = self.conf.general['output_path'].joinpath(pathlib.Path('owntrack')).joinpath(self.conf.track_data[self.conf.general['owntrack']]['file'].name)
         output_file += 'include \'{:s}\';\n'.format(str(path))
 
+        # 他軌道ファイルをinclude
         for tr_l in [i for i in self.conf.track_keys + self.conf.kml_keys + self.conf.csv_keys if (i!= self.conf.general['owntrack'] and i not in self.exclude_tracks)]:
             path = self.conf.general['output_path'].joinpath(pathlib.Path('{:s}_converted.txt'.format(tr_l)))
             output_file += 'include \'{:s}\';\n'.format(str(path))
 
         otmap_path = self.conf.general['output_path'].joinpath(pathlib.Path('tmpmap.txt'))
 
         # kobushi-trackviewerのマップパーサーへoutput_fileを渡す
@@ -595,15 +597,15 @@
                                                   virtualfilename = otmap_path)
 
         # 座標生成する距離程範囲を設定
         if self.conf.track_data[self.conf.general['owntrack']]['endpoint'] > max(self.track[self.conf.general['owntrack']]['data'].controlpoints.list_cp):
             endkp = self.conf.track_data[self.conf.general['owntrack']]['endpoint']
         else:
             endkp = max(self.track[self.conf.general['owntrack']]['data'].controlpoints.list_cp)
-        self.ot_map_source.cp_arbdistribution = [min(self.track[self.conf.general['owntrack']]['data'].controlpoints.list_cp),\
+        self.ot_map_source.cp_arbdistribution = [min(self.track[self.conf.general['owntrack']]['data'].controlpoints.list_cp)+self.conf.general['origin_distance'],\
                                             endkp + self.conf.general['unit_length'],\
                                             self.conf.general['unit_length']]
 
         # kobushi-trackviewerの軌道ジェネレータで自軌道座標を生成
         self.ot_data_ownt = trackgenerator.TrackGenerator(self.ot_map_source,\
                                                      x0 = self.conf.track_data[self.conf.general['owntrack']]['z'],\
                                                      y0 = self.conf.track_data[self.conf.general['owntrack']]['x'],\
```

## Comparing `tsutsuji_trackcomputer-1.6.0.dist-info/LICENSE` & `tsutsuji_trackcomputer-1.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsutsuji_trackcomputer-1.6.0.dist-info/METADATA` & `tsutsuji_trackcomputer-1.6.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsutsuji-trackcomputer
-Version: 1.6.0
+Version: 1.6.1
 Summary: Track building helper for Bve trainsim 5/6
 Home-page: https://github.com/konawasabi/tsutsuji-trackcomputer/
 Author: Konawasabi
 Author-email: webmaster@konawasabi.riceball.jp
 License: Apache License 2.0
 Keywords: BVE trainsim
 Description-Content-Type: text/markdown
```

## Comparing `tsutsuji_trackcomputer-1.6.0.dist-info/RECORD` & `tsutsuji_trackcomputer-1.6.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 tsutsuji/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tsutsuji/__main__.py,sha256=7Gk_TYmLmfVa9AdkoLxZE8B46Qg3mou2ijm6dpmU8CM,647
-tsutsuji/_version.py,sha256=bYN93DTWr8alkTnO3wj31CU5gqTshxIcsbXUcJcUAc8,22
-tsutsuji/backimg.py,sha256=NCpPyjXcG-sZ5dI4URb8MePcxfWUa6MgtINHW13E740,26141
+tsutsuji/_version.py,sha256=purtuLvskAhEdNLSjxoYqUibNFbOHk0IB5Wc4KCA7l4,22
+tsutsuji/backimg.py,sha256=T-ZX2URk12oOd6UUXCSqoZIZNyO1EO2ILHL_3r2aCjE,26323
 tsutsuji/config.py,sha256=cCqC_9R7D7SxvlGq4fGnNzbOAPQCMOfSYPGQLXfX2c4,5514
 tsutsuji/cui2.py,sha256=spk94smgq-bPZCFfT5wblgNY-o5Ir7mZ6Hx-7E9Zspw,2155
 tsutsuji/curvetrackplot.py,sha256=2XH3sqzdWKamAjDjdVb9xTfsZU0j24k7UUgew1HE9PQ,5753
 tsutsuji/drawcursor.py,sha256=1pmDNX4KFZx6-He3kGh5ONkYIxB-nabl2TiWLk-yocU,17026
 tsutsuji/gui_tsutsuji.py,sha256=76-f718L0JGYSO5W3DsY_fwR583cak_71zP6BVCzoT4,19787
 tsutsuji/kml2track.py,sha256=uJtPMpgi3t2ljZhUkyWj2B2j6jAB3h_tHjwfaFfoDQs,5060
-tsutsuji/kp_offset.py,sha256=JQw1YrfCk81_Xbxa1QycMmQGCnbMiuXtaHxsMg6D4Vw,5551
+tsutsuji/kp_offset.py,sha256=IcWVmcs_TRVlAI1xbyACaYqfWd3Stt4WCTbSpPibJ9w,6311
 tsutsuji/math.py,sha256=m-BN4gritBsqiAcfJTp4G3sXCrGcY2IemHCiZlNLDgQ,13102
 tsutsuji/measure.py,sha256=1oCB2nuzpg3CGVUbqlQYr7NygsYlBofuBNMHVNyh7gs,28724
 tsutsuji/solver.py,sha256=Sa4eM5MAIUbsCdQ8AJ_tf7plzkLoIN1wX6ktDZSVS5k,69046
-tsutsuji/track_control.py,sha256=HaGJbMQMyc3oypuwzT-wx1FUDwgGONVeKB0JdtUzP4o,34854
+tsutsuji/track_control.py,sha256=Dqu3Hqtg-X2BbRY1zYRYAI0CpM0iautPfcfUYmq5QR8,35058
 tsutsuji/trackwindow.py,sha256=c2c1bsR2AIwqWCEwjPVnMkwLWgJbjpng8Xpso6pHhzU,10318
-tsutsuji_trackcomputer-1.6.0.dist-info/LICENSE,sha256=F1Ts-WBWMCb_LIZ9VTntNMKH8rjOlcBwWWGRItqwCrs,9723
-tsutsuji_trackcomputer-1.6.0.dist-info/METADATA,sha256=JcYVCzKQmJ6FzBwUm8k57_B08r886cbRN4FsoVbroNg,3468
-tsutsuji_trackcomputer-1.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tsutsuji_trackcomputer-1.6.0.dist-info/top_level.txt,sha256=-4EP2VNLqJy2zJugsOEOF9q-Ir7baVH8QYXuuNtm_0s,9
-tsutsuji_trackcomputer-1.6.0.dist-info/RECORD,,
+tsutsuji_trackcomputer-1.6.1.dist-info/LICENSE,sha256=F1Ts-WBWMCb_LIZ9VTntNMKH8rjOlcBwWWGRItqwCrs,9723
+tsutsuji_trackcomputer-1.6.1.dist-info/METADATA,sha256=GJTKixkEW7lV66-qLona3IINsPngXa23v8yR15Irh4M,3468
+tsutsuji_trackcomputer-1.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tsutsuji_trackcomputer-1.6.1.dist-info/top_level.txt,sha256=-4EP2VNLqJy2zJugsOEOF9q-Ir7baVH8QYXuuNtm_0s,9
+tsutsuji_trackcomputer-1.6.1.dist-info/RECORD,,
```

