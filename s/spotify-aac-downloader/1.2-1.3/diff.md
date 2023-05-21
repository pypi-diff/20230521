# Comparing `tmp/spotify-aac-downloader-1.2.tar.gz` & `tmp/spotify_aac_downloader-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify-aac-downloader-1.2.tar", last modified: Tue Apr 25 17:49:46 2023, max compression
+gzip compressed data, was "spotify_aac_downloader-1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spotify-aac-downloader-1.2.tar` & `spotify_aac_downloader-1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1137 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/.github/workflows/main.yml
--rw-r--r--   0        0        0       96 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/.gitignore
--rw-r--r--   0        0        0     2742 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/README.md
--rw-r--r--   0        0        0      536 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/requirements.txt
--rw-r--r--   0        0        0     4619 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/spotify_aac_downloader/__init__.py
--rw-r--r--   0        0        0       58 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/spotify_aac_downloader/__main__.py
--rw-r--r--   0        0        0    10581 2023-04-25 17:49:40.656050 spotify-aac-downloader-1.2/spotify_aac_downloader/spotify_aac_downloader.py
--rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 spotify-aac-downloader-1.2/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-05-21 04:46:25.267285 spotify_aac_downloader-1.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0       96 2023-05-21 04:46:25.267285 spotify_aac_downloader-1.3/.gitignore
+-rw-r--r--   0        0        0     2861 2023-05-21 04:46:25.267285 spotify_aac_downloader-1.3/README.md
+-rw-r--r--   0        0        0      536 2023-05-21 04:46:25.267285 spotify_aac_downloader-1.3/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-21 04:46:25.267285 spotify_aac_downloader-1.3/requirements.txt
+-rw-r--r--   0        0        0     4921 2023-05-21 04:46:25.267285 spotify_aac_downloader-1.3/spotify_aac_downloader/__init__.py
+-rw-r--r--   0        0        0       92 2023-05-21 04:46:25.267285 spotify_aac_downloader-1.3/spotify_aac_downloader/__main__.py
+-rw-r--r--   0        0        0    10313 2023-05-21 04:46:25.267285 spotify_aac_downloader-1.3/spotify_aac_downloader/spotify_aac_downloader.py
+-rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 spotify_aac_downloader-1.3/PKG-INFO
```

### Comparing `spotify-aac-downloader-1.2/.github/workflows/main.yml` & `spotify_aac_downloader-1.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `spotify-aac-downloader-1.2/pyproject.toml` & `spotify_aac_downloader-1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify-aac-downloader-1.2/spotify_aac_downloader/__init__.py` & `spotify_aac_downloader-1.3/spotify_aac_downloader/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,108 +1,109 @@
 import shutil
 import argparse
 import traceback
+
 from .spotify_aac_downloader import SpotifyAacDownloader
 
-__version__ = '1.2'
+__version__ = '1.3'
 
 
 def main():
-    if not shutil.which('ffmpeg'):
-        raise Exception('ffmpeg is not on PATH')
+    for tool in ['ffmpeg']:
+        if not shutil.which(tool):
+            raise Exception(f'{tool} is not on PATH')
     parser = argparse.ArgumentParser(
-        description = 'Download songs/albums/playlists directly from Spotify in AAC',
-        formatter_class = argparse.ArgumentDefaultsHelpFormatter
+        description='Download songs/albums/playlists directly from Spotify in AAC',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument(
         'url',
         help='Spotify song/album/playlist URL(s)',
         nargs='*',
-        metavar = '<url>'
     )
     parser.add_argument(
         '-u',
         '--urls-txt',
-        help = 'Read URLs from a text file',
-        nargs = '?'
+        help='Read URLs from a text file',
+        action='store_true',
     )
     parser.add_argument(
         '-f',
         '--final-path',
-        default = 'Spotify',
-        help = 'Final Path'
+        default='./Spotify',
+        help='Final Path',
     )
     parser.add_argument(
         '-t',
         '--temp-path',
-        default = 'temp',
-        help = 'Temp Path'
+        default='./temp',
+        help='Temp Path',
     )
     parser.add_argument(
         '-c',
         '--cookies-location',
-        default = 'cookies.txt',
-        help = 'Cookies location'
+        default='./cookies.txt',
+        help='Cookies location',
     )
     parser.add_argument(
         '-w',
         '--wvd-location',
-        default = '*.wvd',
-        help = '.wvd file location'
+        default='./*.wvd',
+        help='.wvd file location (ignored if using -l/--lrc-only)',
     )
     parser.add_argument(
         '-n',
         '--no-lrc',
-        action = 'store_true',
-        help = "Don't create .lrc file"
+        action='store_true',
+        help="Don't create .lrc files",
+    )
+    parser.add_argument(
+        '-l',
+        '--lrc-only',
+        action='store_true',
+        help='Skip downloading songs and only create .lrc files',
     )
     parser.add_argument(
         '-p',
         '--premium-quality',
-        action = 'store_true',
-        help = 'Download 256kbps AAC instead of 128kbps AAC'
+        action='store_true',
+        help='Download 256kbps AAC instead of 128kbps AAC',
     )
     parser.add_argument(
         '-o',
         '--overwrite',
-        action = 'store_true',
-        help = 'Overwrite existing files'
-    )
-    parser.add_argument(
-        '-s',
-        '--skip-cleanup',
-        action = 'store_true',
-        help = 'Skip cleanup'
+        action='store_true',
+        help='Overwrite existing files',
     )
     parser.add_argument(
         '-e',
         '--print-exceptions',
-        action = 'store_true',
-        help = 'Print execeptions'
+        action='store_true',
+        help='Print execeptions',
     )
     parser.add_argument(
         '-v',
         '--version',
-        action = 'version'
+        action='version',
     )
     args = parser.parse_args()
-    if not args.url and not args.urls_txt:
-        parser.error('you must specify an url or a text file using -u/--urls-txt')
     if args.urls_txt:
-        with open(args.urls_txt, 'r', encoding = 'utf8') as f:
-            args.url = f.read().splitlines()
+        _url = []
+        for url_txt in args.url:
+            with open(url_txt, 'r', encoding='utf8') as f:
+                _url.extend(f.read().splitlines())
+        args.url = _url
     dl = SpotifyAacDownloader(
         args.final_path,
         args.cookies_location,
         args.temp_path,
         args.wvd_location,
         args.premium_quality,
         args.overwrite,
-        args.skip_cleanup,
-        args.no_lrc
+        args.lrc_only,
     )
     download_queue = []
     error_count = 0
     for i, url in enumerate(args.url):
         try:
             download_queue.append(dl.get_download_queue(url.strip()))
         except KeyboardInterrupt:
@@ -118,26 +119,32 @@
             try:
                 track_id = track['id']
                 gid = dl.uri_to_gid(track_id)
                 metadata = dl.get_metadata(gid)
                 unsynced_lyrics, synced_lyrics = dl.get_lyrics(track_id)
                 tags = dl.get_tags(metadata, unsynced_lyrics)
                 final_location = dl.get_final_location(tags)
+                if args.lrc_only:
+                    final_location.parent.mkdir(parents=True, exist_ok=True)
+                    dl.make_lrc(final_location, synced_lyrics)
+                    continue
                 if not args.overwrite and final_location.exists():
                     continue
                 file_id = dl.get_file_id(metadata)
                 pssh = dl.get_pssh(file_id)
                 decryption_key = dl.get_decryption_key(pssh)
                 stream_url = dl.get_stream_url(file_id)
                 encrypted_location = dl.get_encrypted_location(track_id)
                 dl.download(encrypted_location, stream_url)
                 fixed_location = dl.get_fixed_location(track_id)
                 dl.fixup(decryption_key, encrypted_location, fixed_location)
+                final_location.parent.mkdir(parents=True, exist_ok=True)
                 dl.make_final(fixed_location, final_location, tags)
-                dl.make_lrc(final_location, synced_lyrics)
+                if not args.no_lrc:
+                    dl.make_lrc(final_location, synced_lyrics)
             except KeyboardInterrupt:
                 exit(1)
             except:
                 error_count += 1
                 print(f'Failed to download "{track["name"]}" (track {j + 1}/{len(url)} from URL {i + 1}/{len(download_queue)})')
                 if args.print_exceptions:
                     traceback.print_exc()
```

### Comparing `spotify-aac-downloader-1.2/spotify_aac_downloader/spotify_aac_downloader.py` & `spotify_aac_downloader-1.3/spotify_aac_downloader/spotify_aac_downloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from pathlib import Path
 import glob
 from http.cookiejar import MozillaCookieJar
 import re
-import requests
 import functools
 import datetime
 import subprocess
 import shutil
+
 from pywidevine import Cdm, Device, PSSH
+import requests
 import base62
-from mutagen.mp4 import MP4, MP4Cover
 from yt_dlp import YoutubeDL
+from mutagen.mp4 import MP4, MP4Cover
 
 
 class SpotifyAacDownloader:
-    def __init__(self, final_path, cookies_location, temp_path, wvd_location, premium_quality, overwrite, skip_cleanup, no_lrc):
+    def __init__(self, final_path, cookies_location, temp_path, wvd_location, premium_quality, overwrite, lrc_only):
         self.temp_path = Path(temp_path)
         self.final_path = Path(final_path)
-        self.skip_cleanup = skip_cleanup
-        self.no_lrc = no_lrc
         self.overwrite = overwrite
         if premium_quality:
             self.audio_quality = 'MP4_256'
         else:
             self.audio_quality = 'MP4_128'
-        wvd_location = glob.glob(wvd_location)
-        if not wvd_location:
-            raise Exception('.wvd file not found')
-        self.cdm = Cdm.from_device(Device.load(Path(wvd_location[0])))
-        self.cdm_session = self.cdm.open()
-        cookies = MozillaCookieJar(Path(cookies_location))
-        cookies.load(ignore_discard = True, ignore_expires = True)
+        if not lrc_only:
+            wvd_location = glob.glob(wvd_location)
+            if not wvd_location:
+                raise Exception('.wvd file not found')
+            self.cdm = Cdm.from_device(Device.load(wvd_location[0]))
+            self.cdm_session = self.cdm.open()
+        cookies = MozillaCookieJar(cookies_location)
+        cookies.load(ignore_discard=True, ignore_expires=True)
         self.session = requests.Session()
         self.session.headers.update({
             'app-platform': 'WebPlayer',
             'accept': 'application/json',
             'accept-language': 'pt-BR,pt;q=0.9,en-US;q=0.8,en;q=0.7,zh-CN;q=0.6,zh;q=0.5,ru;q=0.4,es;q=0.3,ja;q=0.2',
             'content-type': 'application/json',
             'origin': 'https://open.spotify.com',
@@ -47,15 +47,15 @@
             'sec-fetch-site': 'same-site',
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36',
         })
         self.session.cookies.update(cookies)
         web_page = self.session.get('https://open.spotify.com/').text
         token = re.search(r'accessToken":"(.*?)"', web_page).group(1)
         self.session.headers.update({
-            'authorization': f'Bearer {token}'
+            'authorization': f'Bearer {token}',
         })
     
 
     def get_download_queue(self, url):
         uri = url.split('/')[-1].split('?')[0]
         download_queue = []
         if 'album' in url:
@@ -70,15 +70,15 @@
 
 
     def uri_to_gid(self, uri):
         return hex(base62.decode(uri, base62.CHARSET_INVERTED))[2:].zfill(32)
     
 
     def gid_to_uri(self, gid):
-        return base62.encode(int(gid, 16), charset = base62.CHARSET_INVERTED).zfill(22)
+        return base62.encode(int(gid, 16), charset=base62.CHARSET_INVERTED).zfill(22)
     
 
     def get_track(self, track_id):
         return self.session.get(f'https://api.spotify.com/v1/tracks/{track_id}').json()
     
 
     @functools.lru_cache()
@@ -102,16 +102,16 @@
         return playlist
     
 
     def get_metadata(self, gid):
         return self.session.get(f'https://spclient.wg.spotify.com/metadata/4/track/{gid}?market=from_token').json()
 
 
-    def get_file_id(self, track):
-        return next(i["file_id"] for i in track["file"] if i["format"] == self.audio_quality)
+    def get_file_id(self, metadata):
+        return next(i["file_id"] for i in metadata["file"] if i["format"] == self.audio_quality)
     
 
     def get_pssh(self, file_id):
         return self.session.get(f'https://seektables.scdn.co/seektable/{file_id}.json').json()['pssh']
     
 
     def get_decryption_key(self, pssh):
@@ -123,24 +123,22 @@
         ).content
         self.cdm.parse_license(self.cdm_session, license)
         return next(i for i in self.cdm.get_keys(self.cdm_session) if i.type == "CONTENT").key.hex()
     
     
     def get_stream_url(self, file_id):
         return self.session.get(
-            f'https://gue1-spclient.spotify.com/storage-resolve/v2/files/audio/interactive/11/{file_id}?version=10000000&product=9&platform=39&alt=json'
+            f'https://gue1-spclient.spotify.com/storage-resolve/v2/files/audio/interactive/11/{file_id}?version=10000000&product=9&platform=39&alt=json',
         ).json()['cdnurl'][0]
     
 
     def get_artist(self, artist_list):
         if len(artist_list) == 1:
             return artist_list[0]['name']
-        artist = ', '.join(i['name'] for i in artist_list[:-1])
-        artist += f' & {artist_list[-1]["name"]}'
-        return artist
+        return ', '.join(i['name'] for i in artist_list[:-1]) + f' & {artist_list[-1]["name"]}'
     
 
     def get_synced_lyrics_formated_time(self, time):
         formated_time = datetime.datetime.fromtimestamp(time / 1000.0)
         return formated_time.strftime('%M:%S.%f')[:-4]
 
     
@@ -159,47 +157,46 @@
     
 
     @functools.lru_cache()
     def get_cover(self, url):
         return requests.get(url).content
     
 
-    def get_tags(self, track, unsynced_lyrics):
-        album = self.get_album(self.gid_to_uri(track['album']['gid']))
+    def get_tags(self, metadata, unsynced_lyrics):
+        album = self.get_album(self.gid_to_uri(metadata['album']['gid']))
         copyright = next(i['text'] for i in album['copyrights'] if i['type'] == 'P')
         if album['release_date_precision'] == 'year':
             release_date = album['release_date'] + '-01-01'
         else:
             release_date = album['release_date']
-        total_tracks = [i['track_number'] for i in album['tracks']['items'] if i['disc_number'] == track['disc_number']][-1]
+        total_tracks = [i['track_number'] for i in album['tracks']['items'] if i['disc_number'] == metadata['disc_number']][-1]
         total_discs = album['tracks']['items'][-1]['disc_number']
         tags = {
-            '\xa9nam': [track['name']],
-            '\xa9ART': [self.get_artist(track['artist'])],
-            'aART': [self.get_artist(track['album']['artist'])],
-            '\xa9alb': [track['album']['name']],
-            'trkn': [(track['number'], total_tracks)],
-            'disk': [(track['disc_number'], total_discs)],
+            '\xa9nam': [metadata['name']],
+            '\xa9ART': [self.get_artist(metadata['artist'])],
+            'aART': [self.get_artist(metadata['album']['artist'])],
+            '\xa9alb': [metadata['album']['name']],
+            'trkn': [(metadata['number'], total_tracks)],
+            'disk': [(metadata['disc_number'], total_discs)],
             '\xa9day': [f'{release_date}T00:00:00Z'],
-            'covr': [MP4Cover(self.get_cover('https://i.scdn.co/image/' + next(i['file_id'] for i in track['album']['cover_group']['image'] if i['size'] == 'LARGE')), MP4Cover.FORMAT_JPEG)],
-            '\xa9cmt': [f'https://open.spotify.com/track/{track["canonical_uri"].split(":")[-1]}'],
+            'covr': [MP4Cover(self.get_cover('https://i.scdn.co/image/' + next(i['file_id'] for i in metadata['album']['cover_group']['image'] if i['size'] == 'LARGE')))],
+            '\xa9cmt': [f'https://open.spotify.com/track/{metadata["canonical_uri"].split(":")[-1]}'],
             'cprt': [copyright],
-            'rtng': [1] if 'explicit' in track else [0],
+            'rtng': [1] if 'explicit' in metadata else [0],
         }
         if unsynced_lyrics is not None:
             tags['\xa9lyr'] = [unsynced_lyrics]
         return tags
     
 
     def get_sanizated_string(self, dirty_string, is_folder):
-        for character in ['\\', '/', ':', '*', '?', '"', '<', '>', '|', ';']:
-            dirty_string = dirty_string.replace(character, '_')
+        dirty_string = re.sub(r'[\\/:\*\?"<>\|;]', '_', dirty_string)
         if is_folder:
             dirty_string = dirty_string[:40]
-            if dirty_string[-1:] == '.':
+            if dirty_string.endswith('.'):
                 dirty_string = dirty_string[:-1] + '_'
         else:
             dirty_string = dirty_string[:36]
         return dirty_string.strip()
     
 
     def get_encrypted_location(self, track_id):
@@ -208,18 +205,18 @@
 
     def get_fixed_location(self, track_id):
         return self.temp_path / f'{track_id}_fixed.m4a'
     
 
     def get_final_location(self, tags):
         if tags['disk'][0][1] > 1:
-            file_name = self.get_sanizated_string(f'{tags["disk"][0][0]}-{tags["trkn"][0][0]:02d} {tags["©nam"][0]}', False) + '.m4a'
+            file_name = self.get_sanizated_string(f'{tags["disk"][0][0]}-{tags["trkn"][0][0]:02d} {tags["©nam"][0]}', False)
         else:
-            file_name = self.get_sanizated_string(f'{tags["trkn"][0][0]:02d} {tags["©nam"][0]}', False) + '.m4a'
-        return self.final_path / self.get_sanizated_string(tags['aART'][0], True) / self.get_sanizated_string(tags['\xa9alb'][0], True) / file_name
+            file_name = self.get_sanizated_string(f'{tags["trkn"][0][0]:02d} {tags["©nam"][0]}', False)
+        return self.final_path / self.get_sanizated_string(tags['aART'][0], True) / self.get_sanizated_string(tags['\xa9alb'][0], True) / (file_name + '.m4a')
         
     
     def download(self, encrypted_location, stream_url):
         with YoutubeDL({
             'quiet': True,
             'no_warnings': True,
             'outtmpl': str(encrypted_location),
@@ -241,29 +238,28 @@
                 decryption_key,
                 '-i',
                 encrypted_location,
                 '-c',
                 'copy',
                 fixed_location,
             ],
-            check = True
+            check=True
         )
     
 
     def make_final(self, fixed_location, final_location, tags):
-        final_location.parent.mkdir(parents = True, exist_ok = True)
-        shutil.copy(fixed_location, final_location)
-        file = MP4(final_location)
+        file = MP4(fixed_location)
         file.clear()
         file.update(tags)
         file.save()
+        shutil.move(fixed_location, final_location)
 
 
     def make_lrc(self, final_location, synced_lyrics):
-        if synced_lyrics and not self.no_lrc:
-            with open(final_location.with_suffix('.lrc'), 'w', encoding = 'utf8') as f:
+        if synced_lyrics:
+            with open(final_location.with_suffix('.lrc'), 'w', encoding='utf8') as f:
                 f.write(synced_lyrics)
     
 
     def cleanup(self):
-        if self.temp_path.exists() and not self.skip_cleanup:
+        if self.temp_path.exists():
             shutil.rmtree(self.temp_path)
```

### Comparing `spotify-aac-downloader-1.2/PKG-INFO` & `spotify_aac_downloader-1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: spotify-aac-downloader
-Version: 1.2
-Summary: Download songs/albums/playlists directly from Spotify in AAC
-Author: glomatico
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: pywidevine
-Requires-Dist: pyyaml
-Requires-Dist: pybase62
-Requires-Dist: yt-dlp
-Project-URL: repository, https://github.com/glomatico/spotify-aac-downloader
-
 # Spotify ✨ AAC ✨ Downloader
 A Python script to download songs/albums/playlists directly from Spotify in 256kbps/128kbps AAC.
 
 ## Setup
 1. Install Python 3.7 or newer
 2. Install spotify-aac-downloader with pip
     ```
@@ -33,38 +20,40 @@
         2. Create the .wvd file
             ```
             pywidevine create-device -t ANDROID -l 3 -k private_key.pem -c client_id.bin -o .
             ```
 
 ## Usage
 ```
-usage: spotify-aac-downloader [-h] [-u [URLS_TXT]] [-f FINAL_PATH] [-t TEMP_PATH] [-c COOKIES_LOCATION] [-w WVD_LOCATION] [-n]
-                   [-p] [-o] [-s] [-e] [-v]
-                   [<url> ...]
+usage: spotify-aac-downloader [-h] [-u] [-f FINAL_PATH] [-t TEMP_PATH]
+                   [-c COOKIES_LOCATION] [-w WVD_LOCATION] [-n] [-l] [-p] [-o]
+                   [-e] [-v]
+                   [url ...]
 
 Download songs/albums/playlists directly from Spotify in AAC
 
 positional arguments:
-  <url>                 Spotify song/album/playlist URL(s) (default: None)
+  url                   Spotify song/album/playlist URL(s) (default: None)
 
 options:
   -h, --help            show this help message and exit
-  -u [URLS_TXT], --urls-txt [URLS_TXT]
-                        Read URLs from a text file (default: None)
+  -u, --urls-txt        Read URLs from a text file (default: False)
   -f FINAL_PATH, --final-path FINAL_PATH
-                        Final Path (default: Spotify)
+                        Final Path (default: ./Spotify)
   -t TEMP_PATH, --temp-path TEMP_PATH
-                        Temp Path (default: temp)
+                        Temp Path (default: ./temp)
   -c COOKIES_LOCATION, --cookies-location COOKIES_LOCATION
-                        Cookies location (default: cookies.txt)
+                        Cookies location (default: ./cookies.txt)
   -w WVD_LOCATION, --wvd-location WVD_LOCATION
-                        .wvd file location (default: *.wvd)
-  -n, --no-lrc          Don't create .lrc file (default: False)
+                        .wvd file location (ignored if using -l/--lrc-only)
+                        (default: ./*.wvd)
+  -n, --no-lrc          Don't create .lrc files (default: False)
+  -l, --lrc-only        Skip downloading songs and only create .lrc files
+                        (default: False)
   -p, --premium-quality
-                        Download 256kbps AAC instead of 128kbps AAC (default: False)
+                        Download 256kbps AAC instead of 128kbps AAC (default:
+                        False)
   -o, --overwrite       Overwrite existing files (default: False)
-  -s, --skip-cleanup    Skip cleanup (default: False)
   -e, --print-exceptions
                         Print execeptions (default: False)
   -v, --version         show program's version number and exit
 ```
-
```

