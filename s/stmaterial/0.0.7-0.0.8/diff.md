# Comparing `tmp/stmaterial-0.0.7.tar.gz` & `tmp/stmaterial-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stmaterial-0.0.7.tar", last modified: Tue May 16 14:59:27 2023, max compression
+gzip compressed data, was "stmaterial-0.0.8.tar", last modified: Sun May 21 04:53:14 2023, max compression
```

## Comparing `stmaterial-0.0.7.tar` & `stmaterial-0.0.8.tar`

### file list

```diff
@@ -1,208 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:27.742927 stmaterial-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-16 14:59:01.190998 stmaterial-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-16 14:59:01.190998 stmaterial-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-16 14:59:01.190998 stmaterial-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-16 14:59:01.190998 stmaterial-0.0.7/docs/_images/a.png
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-16 14:59:01.190998 stmaterial-0.0.7/docs/_images/b.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.190998 stmaterial-0.0.7/docs/_images/books/
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-05-16 14:59:01.190998 stmaterial-0.0.7/docs/_images/books/benders分解.png
--rw-r--r--   0 runner    (1001) docker     (123)   394770 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/books/内点法.png
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/c.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/links/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/links/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)   164525 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/links/gallery/jupyter_book.png
--rw-r--r--   0 runner    (1001) docker     (123)    93132 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/links/gallery/matplotlib.png
--rw-r--r--   0 runner    (1001) docker     (123)   112977 2023-05-16 14:59:01.194998 stmaterial-0.0.7/docs/_images/links/gallery/pandas.png
--rw-r--r--   0 runner    (1001) docker     (123)   204727 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_images/links/gallery/sphinx_design.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/links/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/links/gallery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/logo-.png
--rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/blog.md
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/kitchen-sink/typography.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/examples/reference/text-formatting.md
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/posts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/posts/plangs/
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/posts/plangs/2021-python-pathlib.md
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/posts/plangs/2022-python-setup.md
--rw-r--r--   0 runner    (1001) docker     (123)    18997 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/posts/plangs/2022-python-typing.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/header.md
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/sidenav.md
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/source-buttons.md
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/user_guide/variables.md
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-16 14:59:01.198998 stmaterial-0.0.7/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-16 14:59:01.198998 stmaterial-0.0.7/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   220389 2023-05-16 14:59:01.198998 stmaterial-0.0.7/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-16 14:59:01.198998 stmaterial-0.0.7/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 14:59:01.198998 stmaterial-0.0.7/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-16 14:59:01.198998 stmaterial-0.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.198998 stmaterial-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/_navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/_translations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/scripts/gumshoe-patched.js
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/scripts/materialize.js
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/scripts/stmaterial.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/base/_theme.sass
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/base/_typography.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_searchbox.scss
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_sidenav-icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/components/_table-of-contents.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_admonitions.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_api.sass
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_code.sass
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_lists.sass
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_spans.scss
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_ablog.scss
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_myst-nb.scss
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_tippy.sass
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/patch/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/patch/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/patch/_patch.scss
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/patch/_test.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_article.sass
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_headnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_stm-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/stmaterial.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_colors.scss
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/stmaterial theme.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3567 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/headnav-items.html
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/license.html
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/postnav.html
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/partials/_icon_links_declaration.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/static/images/github.svg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/theme/stmaterial/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-16 14:59:01.202998 stmaterial-0.0.7/src/stmaterial/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:59:01.202998 stmaterial-0.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-16 14:59:01.202998 stmaterial-0.0.7/webpack.config.js
--rw-r--r--   0        0        0     4153 1970-01-01 00:00:00.000000 stmaterial-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:14.192907 stmaterial-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-21 04:52:53.956531 stmaterial-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-21 04:52:53.956531 stmaterial-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-21 04:52:53.956531 stmaterial-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.960531 stmaterial-0.0.8/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-21 04:52:53.956531 stmaterial-0.0.8/docs/_images/a.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-21 04:52:53.956531 stmaterial-0.0.8/docs/_images/b.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.956531 stmaterial-0.0.8/docs/_images/books/
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-05-21 04:52:53.956531 stmaterial-0.0.8/docs/_images/books/benders分解.png
+-rw-r--r--   0 runner    (1001) docker     (123)   394770 2023-05-21 04:52:53.960531 stmaterial-0.0.8/docs/_images/books/内点法.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-21 04:52:53.960531 stmaterial-0.0.8/docs/_images/c.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.960531 stmaterial-0.0.8/docs/_images/links/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/_images/links/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)   164525 2023-05-21 04:52:53.960531 stmaterial-0.0.8/docs/_images/links/gallery/jupyter_book.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93132 2023-05-21 04:52:53.960531 stmaterial-0.0.8/docs/_images/links/gallery/matplotlib.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112977 2023-05-21 04:52:53.960531 stmaterial-0.0.8/docs/_images/links/gallery/pandas.png
+-rw-r--r--   0 runner    (1001) docker     (123)   204727 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/_images/links/gallery/sphinx_design.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/_static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/_static/links/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/_static/links/gallery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/_static/logo-.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/blog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/kitchen-sink/typography.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/pages/fullwidth.md
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/pages/hidesidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/pages/hidetoc.md
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/pages/hidetocnav.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/pages/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/examples/reference/text-formatting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/posts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/posts/plangs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/posts/plangs/2021-python-pathlib.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/posts/plangs/2022-python-setup.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18997 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/posts/plangs/2022-python-typing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/user_guide/header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/user_guide/sidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/user_guide/source-buttons.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/user_guide/tocnav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/user_guide/variables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-21 04:52:53.964531 stmaterial-0.0.8/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-21 04:52:53.964531 stmaterial-0.0.8/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220389 2023-05-21 04:52:53.968531 stmaterial-0.0.8/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-21 04:52:53.968531 stmaterial-0.0.8/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-21 04:52:53.968531 stmaterial-0.0.8/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-21 04:52:53.968531 stmaterial-0.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/
+-rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17690 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/_translations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/scripts/gumshoe-patched.js
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/scripts/materialize.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/scripts/stmaterial.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/base/_theme.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/base/_typography.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_searchbox.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_sidenav-icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_sidenav-toggle.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/components/_table-of-contents.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_admonitions.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_api.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_code.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_gui-labels.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_lists.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_spans.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/extensions/_myst-nb.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/extensions/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/extensions/_tippy.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/patch/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/patch/_patch.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/patch/_test.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/sections/_article.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/sections/_headnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/sections/_stm-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/stmaterial.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/variables/_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/translations/jsons/stmaterial theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-21 04:52:53.968531 stmaterial-0.0.8/src/stmaterial/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3567 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/headnav-items.html
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/license.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/postnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/sidenav-toggle.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/partials/_icon_links_declaration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/static/images/github.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/theme/stmaterial/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-21 04:52:53.972531 stmaterial-0.0.8/src/stmaterial/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:52:53.972531 stmaterial-0.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-21 04:52:53.972531 stmaterial-0.0.8/webpack.config.js
+-rw-r--r--   0        0        0     4153 1970-01-01 00:00:00.000000 stmaterial-0.0.8/PKG-INFO
```

### Comparing `stmaterial-0.0.7/LICENSE` & `stmaterial-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/README.md` & `stmaterial-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_images/a.png` & `stmaterial-0.0.8/docs/_images/a.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_images/b.png` & `stmaterial-0.0.8/docs/_images/b.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_images/books/benders分解.png` & `stmaterial-0.0.8/docs/_images/books/benders分解.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_images/books/内点法.png` & `stmaterial-0.0.8/docs/_images/books/内点法.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_images/c.png` & `stmaterial-0.0.8/docs/_images/c.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_images/links/gallery/jupyter_book.png` & `stmaterial-0.0.8/docs/_images/links/gallery/jupyter_book.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_images/links/gallery/matplotlib.png` & `stmaterial-0.0.8/docs/_images/links/gallery/matplotlib.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_images/links/gallery/pandas.png` & `stmaterial-0.0.8/docs/_images/links/gallery/pandas.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_images/links/gallery/sphinx_design.png` & `stmaterial-0.0.8/docs/_images/links/gallery/sphinx_design.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_static/favicon.png` & `stmaterial-0.0.8/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_static/links/gallery.yaml` & `stmaterial-0.0.8/docs/_static/links/gallery.yaml`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_static/logo-.png` & `stmaterial-0.0.8/docs/_static/logo-.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/_static/logo.png` & `stmaterial-0.0.8/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/conf.py` & `stmaterial-0.0.8/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,26 +46,26 @@
 templates_path = ["_templates"]
 html_static_path = ["_static"]
 html_theme = "stmaterial"
 html_title = "sphinx theme of material"
 html_favicon = "_static/favicon.png"
 html_last_updated_fmt = ""
 html_logo = "_static/logo-.png"
-html_show_sourcelink = False
+html_show_sourcelink = True
 
 todo_include_todos = True
 
 
 html_theme_options = {
     "header_links_before_dropdown": 4,
     "source_repository": "https://github.com/zclab/stmaterial",
     "source_branch": "main",
     "source_directory": "docs/",
     "show_back_to_top": True,
-    "fix_header_nav": True,
+    "fix_header_nav": False,
     "logo": {"text": "Stmaterial", "logo": "_static/logo.png"},
     "external_links": [
         {"name": "Furo", "url": "https://pradyunsg.me/furo/quickstart/"},
         {
             "name": "Sphinx book theme",
             "url": "https://sphinx-book-theme.readthedocs.io/en/latest/",
         },
@@ -137,26 +137,24 @@
     "css_variables": {
         "primary-color": "#3949ab",
         "primary-color-dark": "#283593",
         "primary-color-raised-hover-solid": "#5c6bc0",
         "primary-color-raised-focus-solid": "#5c6bc0",
     },
     "navigation_with_keys": True,
-    "article_top_right": "searchbox.html",
+    "article_top_right": ["searchbox.html", "sidenav-toggle.html", "sourcelink.html"],
 }
 
-
 blog_path = "blog"
 blog_post_pattern = "posts/*/*"
 blog_authors = {
     "zclab": ("子川", "https://github.com/zclab"),
 }
 
 html_sidebars = {
-    "index": [],
     "posts/**": [
         "search-field.html",
         "ablog/postcard.html",
         "ablog/categories.html",
         "ablog/tagcloud.html",
         "ablog/recentposts.html",
     ],
```

### Comparing `stmaterial-0.0.7/docs/develop.md` & `stmaterial-0.0.8/docs/develop.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/admonitions.rst` & `stmaterial-0.0.8/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/api.rst` & `stmaterial-0.0.8/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/blocks.rst` & `stmaterial-0.0.8/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/generic.rst` & `stmaterial-0.0.8/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/images.rst` & `stmaterial-0.0.8/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/index.md` & `stmaterial-0.0.8/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/lists.rst` & `stmaterial-0.0.8/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/really-long.md` & `stmaterial-0.0.8/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/sphinx-design.md` & `stmaterial-0.0.8/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/structure.rst` & `stmaterial-0.0.8/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/tables.rst` & `stmaterial-0.0.8/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/kitchen-sink/typography.rst` & `stmaterial-0.0.8/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/reference/admonitions.md` & `stmaterial-0.0.8/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/reference/api.md` & `stmaterial-0.0.8/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/reference/code-blocks.md` & `stmaterial-0.0.8/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/reference/hyperlinks.md` & `stmaterial-0.0.8/docs/examples/reference/hyperlinks.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 ```{stm-demo}
 Hyperlinks can take various forms, so here's a list of them:
 
 - standalone hyperlink: <https://python.org/>
 - hyperlink using references: [link][markdown-external-hyperlink]
 - hyperlink with inline URL: [link](https://python.org/)
-- hyperlink to a different page: [link](../../user_guide/quickstart)
+- hyperlink to a different page: [link](../../user_guide/sidenav)
 - hyperlink to a specific API element: {class}`pathlib.Path`
 
 [markdown-external-hyperlink]: https://python.org/
 
 +++
 
 Hyperlinks can take various forms, so here's a list of them:
 
 - standalone hyperlink: https://python.org/
 - hyperlink using references: `link <link>`__
 - hyperlink with inline URL: `link <https://python.org/>`_
-- hyperlink to a different page: :doc:`link <../../user_guide/quickstart>`
+- hyperlink to a different page: :doc:`link <../../user_guide/sidenav>`
 - hyperlink to a specific API element: :class:`pathlib.Path`
 
 .. _link: https://python.org/
 ```
```

### Comparing `stmaterial-0.0.7/docs/examples/reference/images.md` & `stmaterial-0.0.8/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/reference/index.md` & `stmaterial-0.0.8/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/reference/lists.md` & `stmaterial-0.0.8/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/reference/tables.md` & `stmaterial-0.0.8/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/reference/tabs.md` & `stmaterial-0.0.8/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/examples/reference/text-formatting.md` & `stmaterial-0.0.8/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/posts/plangs/2021-python-pathlib.md` & `stmaterial-0.0.8/docs/posts/plangs/2021-python-pathlib.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/posts/plangs/2022-python-setup.md` & `stmaterial-0.0.8/docs/posts/plangs/2022-python-setup.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/posts/plangs/2022-python-typing.md` & `stmaterial-0.0.8/docs/posts/plangs/2022-python-typing.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/user_guide/header.md` & `stmaterial-0.0.8/docs/user_guide/header.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/user_guide/sidenav.md` & `stmaterial-0.0.8/docs/user_guide/sidenav.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 start-after: "# sidebar-start"
 end-before: "# sidebar-end"
 ---
 ```
 
 ## Hiding sidenav
 
-Stmaterial supports hiding the sidenav. To explicitly hide it on a specific page, `hide-sidenav` can be set in the [File-Wide metadata][sphinx-file-wide-metadata] for that page..
+Stmaterial supports hiding the sidenav. To explicitly hide it on a specific page, `hide-sidenav` can be set in the [File-Wide metadata][sphinx-file-wide-metadata] for that page. See [Page example with hidding sidenav](../examples/pages/hidesidenav.md).
 
 ````{tab} reStructuredText
 ```rst
 :hide-sidenav:
 
 [page contents]
 ```
```

### Comparing `stmaterial-0.0.7/docs/user_guide/source-buttons.md` & `stmaterial-0.0.8/docs/user_guide/source-buttons.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/docs/user_guide/variables.md` & `stmaterial-0.0.8/docs/user_guide/variables.md`

 * *Files 26% similar despite different names*

```diff
@@ -12,21 +12,34 @@
 html_theme_options = {
     "css_variables": {
         "sidenav-width": "320px",
     },
 }
 ```
 
-## changing colors
+## changing appearance colors of the theme
 
-You can change the colors of the theme by specifying corresponding variables, for example:
+You can change the appearance colors of the theme by specifying corresponding variables, for example:
 
 ```py
 html_theme_options = {
     "css_variables": {
         "primary-color": "#3949ab",
         "primary-color-dark": "#283593",
         "primary-color-raised-hover-solid": "#5c6bc0",
         "primary-color-raised-focus-solid": "#5c6bc0",
     },
 }
 ```
+
+Your can also change the dark appearance of the theme by specifying corresponding dark css variables, for example:
+
+```py
+html_theme_options = {
+    "dark_css_variables": {
+        "primary-color": "#3949ab",
+        "primary-color-dark": "#283593",
+        "primary-color-raised-hover-solid": "#5c6bc0",
+        "primary-color-raised-focus-solid": "#5c6bc0",
+    },
+}
+```
```

### Comparing `stmaterial-0.0.7/docs/web-components.rst` & `stmaterial-0.0.8/docs/web-components.rst`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/noxfile.py` & `stmaterial-0.0.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/package-lock.json` & `stmaterial-0.0.8/package-lock.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/package.json` & `stmaterial-0.0.8/package.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/pyproject.toml` & `stmaterial-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/__init__.py` & `stmaterial-0.0.8/src/stmaterial/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sphinx.locale import get_translation
 from ._navigation import add_toctree_functions
 from ._transforms import ShortenLinkTransform, WrapTableAndMathInAContainerTransform
 from .utils import get_theme_options, config_provided_by_user
 from .directives import GalleryDirective
 
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 logger = logging.getLogger(__name__)
 
 MESSAGE_CATALOG_NAME = "stmaterial"
 _KNOWN_STYLES_IN_USE: Dict[str, Optional[Style]] = {
     "light": None,
     "dark": None,
 }
@@ -283,15 +283,15 @@
 
 def _builder_inited(app: sphinx.application.Sphinx) -> None:
     if app.config.html_theme != "stmaterial":
         return
     if "stmaterial" in app.config.extensions:
         raise Exception(
             "Did you list 'stmaterial' in the `extensions` in conf.py? "
-            "If so, please remove it. ssdoc does not work with non-HTML builders "
+            "If so, please remove it. stmaterial does not work with non-HTML builders "
             "and specifying it as an `html_theme` is sufficient."
         )
 
     if not isinstance(app.builder, StandaloneHTMLBuilder):
         raise Exception(
             "stmaterial is being used as an extension in a non-HTML build. "
             "This should not happen."
@@ -339,14 +339,33 @@
     else:
         for icon in header_icons:
             svg = icon.get("svg")
             if svg:
                 svg = f"_static/{svg}"
                 icon["svg"] = svg
 
+    # Add an analytics ID to the site if provided
+    analytics = theme_options.get("analytics", {})
+    if analytics:
+        # Google Analytics
+        gid = analytics.get("google_analytics_id")
+
+        if gid:
+            gid_js_path = f"https://www.googletagmanager.com/gtag/js?id={gid}"
+            gid_script = f"""
+                window.dataLayer = window.dataLayer || [];
+                function gtag(){{ dataLayer.push(arguments); }}
+                gtag('js', new Date());
+                gtag('config', '{gid}');
+            """
+
+            # Link the JS files
+            app.add_js_file(gid_js_path, loading_method="async")
+            app.add_js_file(None, body=gid_script)
+
 
 def update_and_remove_templates(
     app: sphinx.application.Sphinx, pagename: str, templatename: str, context, doctree
 ) -> None:
     template_sections = [
         "theme_footer",
         "theme_footer_content",
@@ -394,17 +413,14 @@
     app.connect("builder-inited", _builder_inited)
     app.connect("builder-inited", _update_config)
     app.connect("build-finished", _overwrite_pygments_css)
     # Include component templates
     app.config.templates_path.append(str(theme_dir / "components"))
     app.config.html_static_path.append(str(theme_dir / "static/images"))
 
-    # extensions = ["sphinx_design", "sphinx_copybutton", "sphinx_togglebutton", "sphinx_subfigure"]
-    # activate_extensions(app, extensions)
-
     app.add_directive("gallery-grid", GalleryDirective)
 
     return {
         "parallel_read_safe": True,
         "parallel_write_safe": True,
         "version": __version__,
     }
```

### Comparing `stmaterial-0.0.7/src/stmaterial/_navigation.py` & `stmaterial-0.0.8/src/stmaterial/_navigation.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/_transforms.py` & `stmaterial-0.0.8/src/stmaterial/_transforms.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/_translations.py` & `stmaterial-0.0.8/src/stmaterial/_translations.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/scripts/gumshoe-patched.js` & `stmaterial-0.0.8/src/stmaterial/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/scripts/stmaterial.js` & `stmaterial-0.0.8/src/stmaterial/assets/scripts/stmaterial.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/base/_typography.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/base/_typography.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_back-to-top.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/components/_back-to-top.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_brand-logo.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/components/_brand-logo.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_prev-next.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_search-field.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/components/_search-field.sass`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,27 @@
   display: flex
   align-items: center
   position: relative
   color: var(--font-color-medium)
 
   span.material-icons
     display: flex
+    padding-left: 5px
     position: absolute
 
   .search-button__kbd-shortcut
     display: flex
     position: absolute
     right: 5px
 
 
 input:not([type]):not(.browser-default)
   border-top: $input-border
   margin: 0.68rem 0
-  padding-left: calc(var(--header-horizontal-spacing) + 10px)
+  padding-left: calc(var(--header-horizontal-spacing) + 15px)
   background-color: var(--background-color-sidenav)
   color: var(--font-color-main)
 
   &:focus:not([readonly])
     border-top: 1px solid var(--input-focus-color)
     border-bottom: 1px solid var(--input-focus-color)
     box-shadow: 2px 4px 2px 1px rgba(0, 0, 0, 0.2)
```

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_searchbox.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/components/_searchbox.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/components/_table-of-contents.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/components/_table-of-contents.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_admonitions.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/content/_admonitions.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_api.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/content/_api.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_code.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/content/_code.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_footnotes.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_images.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_lists.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/content/_lists.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_misc.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_sidebar.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_tables.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/content/_target.sass` & `stmaterial-0.0.8/src/stmaterial/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_ablog.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/extensions/_ablog.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/extensions/_timeline.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/extensions/_timeline.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/patch/_test.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/components/_search-button.scss`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-.section {
-  padding-top: 0;
-}
-
 /*************************
  * Search button
  */
 // Search link icon should be a bit bigger since it is separate from icon links
 
 // __search-container will only show up when we use the search pop-up bar
 .search-button__search-container,
```

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_footer.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/sections/_footer.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_headnav.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/sections/_headnav.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/sections/_sidebar-toggle.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/sections/_stm-sidenav.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/sections/_stm-sidenav.scss`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
       display: flex;
       flex-direction: column;
       height: 100%;
       // width: $sidenav-width;
 
       .sidenav-menu {
         flex-grow: 1;
-        padding: 0 0 0 var(--header-horizontal-spacing);
+        padding: 0 0 20px var(--header-horizontal-spacing);
         overflow: auto;
         margin-top: 1rem;
 
         .sidenav-menulist {
           list-style: none;
           margin: 0;
           padding-left: 0;
```

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_admonitions.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_colors.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/variables/_colors.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/styles/variables/_icons.scss` & `stmaterial-0.0.8/src/stmaterial/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/translations/README.md` & `stmaterial-0.0.8/src/stmaterial/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/Edit this page.json` & `stmaterial-0.0.8/src/stmaterial/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/assets/translations/jsons/On this page.json` & `stmaterial-0.0.8/src/stmaterial/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/demo/module.py` & `stmaterial-0.0.8/src/stmaterial/demo/module.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/demo/sphinxext.py` & `stmaterial-0.0.8/src/stmaterial/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/directives.py` & `stmaterial-0.0.8/src/stmaterial/directives.py`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/base.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/base.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/breadcrumbs.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/edit-this-page.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/postnav.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/postnav.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/prev-next.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/components/search-field.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/components/search-field.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/domainindex.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/domainindex.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/genindex.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/genindex.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/layout.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/layout.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/partials/_head_css_variables.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 {#
 This is where user-provided CSS variables get converted into actual values.
 #}
-{% macro declare_css_variables(user_customisations, pygments_theme) -%}
+{% macro declare_css_variables(user_customisations, pygments_theme, fixed_headnav) -%}
 --color-code-background: {{ pygments_theme.background }};
 --color-code-foreground: {{ pygments_theme.foreground }};
+{% if fixed_headnav %}
+--article-top-position: inherit;
+{% endif %}
 {% if user_customisations -%}
 {% for name, value in user_customisations.items() -%}
 --{{ name }}: {{ value }};
 {% endfor %}
 {%- endif %}
 {%- endmacro %}
 
@@ -39,13 +42,13 @@
     {{ declare_font_variables(theme_custom_fonts) }}
 
     html {
         font-family: var(--font-stack);
     }
 
     :root {
-        {{ declare_css_variables(theme_css_variables, stmaterial_pygments.light) }}
+        {{ declare_css_variables(theme_css_variables, stmaterial_pygments.light, theme_fix_header_nav) }}
     }
     :root[theme="dark"] {
-        {{ declare_css_variables(theme_dark_css_variables, stmaterial_pygments.dark) }}
+        {{ declare_css_variables(theme_dark_css_variables, stmaterial_pygments.dark, theme_fix_header_nav) }}
     }
 </style>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {# This is where user-provided CSS variables get converted into actual values.
-#} {% macro declare_css_variables(user_customisations, pygments_theme) -%} --
-color-code-background: {{ pygments_theme.background }}; --color-code-
-foreground: {{ pygments_theme.foreground }}; {% if user_customisations -%} {%
+#} {% macro declare_css_variables(user_customisations, pygments_theme,
+fixed_headnav) -%} --color-code-background: {{ pygments_theme.background }}; --
+color-code-foreground: {{ pygments_theme.foreground }}; {% if fixed_headnav %}
+--article-top-position: inherit; {% endif %} {% if user_customisations -%} {%
 for name, value in user_customisations.items() -%} --{{ name }}: {{ value }};
 {% endfor %} {%- endif %} {%- endmacro %} {% macro declare_font_variables
 (user_customisations) -%} {% if user_customisations -%} {% for src in
 user_customisations.src -%} @font-face { font-family: {
 { user_customisations.name }}; font-weight: {{ src.weight }}; font-style:
 normal; font-display: swap; src: url({{ src.url }}) format({
 { user_customisations.type }}); } {% endfor %} {% if
```

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/partials/_icon_links_declaration.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/partials/_icon_links_declaration.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/search.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/search.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/article-bottom.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/article-top.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/sections/article-top.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/sections/headnav.html` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/sections/headnav.html`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/static/images/github.svg` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/static/images/github.svg`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/src/stmaterial/theme/stmaterial/theme.conf` & `stmaterial-0.0.8/src/stmaterial/theme/stmaterial/theme.conf`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # sidebar-end
 
 [options]
 navigation_depth = 4
 show_nav_level = 1
 show_toc_level = 1
 logo =
+analytics =
 header_links_before_dropdown = 4
 external_links =
 header_icons =
 footer_icons =
 sidenav_icons =
 use_edit_page_button=
 source_repository=
@@ -25,15 +26,15 @@
 show_prev_next = True
 show_back_to_top = True
 fix_header_nav =
 css_variables =
 dark_css_variables =
 footer =
 footer_content = sphinx-version.html, copyright.html
-toc_title =
+toc_title = On this page
 search_bar_text = Search the docs ...
 dropdown_label_name = More
 navigation_with_keys = True
 article_top_left = breadcrumbs.html
-article_top_right = sourcelink.html
+article_top_right = searchbox.html, sidenav-toggle.html, sourcelink.html
 article_bottom_left = last-updated.html
 article_bottom_right = edit-this-page.html
```

### Comparing `stmaterial-0.0.7/src/stmaterial/utils.py` & `stmaterial-0.0.8/src/stmaterial/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from sphinx.application import Sphinx
 from typing import Iterator
 from docutils.nodes import Node
 
 
 def config_provided_by_user(app: Sphinx, key: str) -> bool:
     """Check if the user has manually provided the config.
-    REMOVE when pydata v0.14 is released and import from there.
+    This is from pydata sphinx theme.
     """
     return any(key in ii for ii in [app.config.overrides, app.config._raw_config])
 
 
 def get_theme_options(app: Sphinx):
     """Return theme options for the application w/ a fallback if they don't exist.
     In general we want to modify app.builder.theme_options if it exists, so prefer that first.
```

### Comparing `stmaterial-0.0.7/webpack.config.js` & `stmaterial-0.0.8/webpack.config.js`

 * *Files identical despite different names*

### Comparing `stmaterial-0.0.7/PKG-INFO` & `stmaterial-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stmaterial
-Version: 0.0.7
+Version: 0.0.8
 Summary: A sphinx theme of materializecss.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stmaterial Version: 0.0.7 Summary: A sphinx theme
+Metadata-Version: 2.1 Name: stmaterial Version: 0.0.8 Summary: A sphinx theme
 of materializecss. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

