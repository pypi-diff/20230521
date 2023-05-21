# Comparing `tmp/aa_structures-2.3.0.tar.gz` & `tmp/aa_structures-2.3.1b1.tar.gz`

## Comparing `aa_structures-2.3.0.tar` & `aa_structures-2.3.1b1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/__init__.py
--rw-r--r--   0        0        0    36110 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/admin.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/app_settings.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/apps.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/auth_hooks.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/checks.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/constants.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/forms.py
--rw-r--r--   0        0        0    18949 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/managers.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/providers.py
--rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/swagger.json
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tasks.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/urls.py
--rw-r--r--   0        0        0    21820 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/__init__.py
--rw-r--r--   0        0        0    71519 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/notification_embeds.py
--rw-r--r--   0        0        0    16436 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/notification_timers.py
--rw-r--r--   0        0        0    19834 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/serializers.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/sovereignty.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/core/starbases.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/helpers/__init__.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/helpers/general.py
--rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/django.pot
--rw-r--r--   0        0        0    13634 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    61204 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47274 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    55691 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47267 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47024 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ko/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    47437 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    47505 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    58962 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/management/commands/__init__.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/management/commands/structures_load_eve.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/management/commands/structures_preload_eveuniverse.py
--rw-r--r--   0        0        0    59315 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/migrations/0002_remove_eveuniverse_relation_names.py
--rw-r--r--   0        0        0    44042 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/migrations/0003_add_localization_and_unique_key.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/migrations/__init__.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/models/__init__.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/models/eveuniverse.py
--rw-r--r--   0        0        0    42691 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/models/notifications.py
--rw-r--r--   0        0        0    53967 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/models/owners.py
--rw-r--r--   0        0        0    37256 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/models/structures.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/css/global.css
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/css/main.css
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/eve_symbol_128.png
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/structures_logo.png
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/0h.png
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/0l.png
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/0m.png
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/0r.png
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/0s.png
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/1h.png
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/1l.png
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/1m.png
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/1r.png
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/2h.png
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/2l.png
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/2m.png
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/2r.png
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/3h.png
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/3l.png
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/3m.png
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/3r.png
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/4h.png
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/4l.png
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/4m.png
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/4s.png
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/5h.png
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/5l.png
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/5m.png
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/5s.png
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/6h.png
--rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/6l.png
--rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/6m.png
--rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/7h.png
--rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/7l.png
--rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/7m.png
--rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/8h.png
--rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/8l.png
--rw-r--r--   0        0        0     9541 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/8m.png
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/blank.png
--rw-r--r--   0        0        0    16840 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/circle.png
--rw-r--r--   0        0        0    33523 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/dustwheel.png
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/h.png
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/l.png
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/m.png
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/noship.png
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/r.png
--rw-r--r--   0        0        0    43642 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis.png
--rw-r--r--   0        0        0    43560 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_blue.png
--rw-r--r--   0        0        0    42833 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_darkred.png
--rw-r--r--   0        0        0    38343 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_default.png
--rw-r--r--   0        0        0    42868 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_revelations.png
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/base.html
--rw-r--r--   0        0        0    21200 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/main.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/fitting_assets.html
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/fitting_gfx.html
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/poco_details.html
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/starbase_detail.html
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/structure_details.html
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/modals/tab_general_detail.html
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/partials/jump_gates_list.html
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/partials/poco_list.html
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/partials/structure_list.html
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/partials/structure_summary.html
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/templatetags/detail_title.html
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/templatetags/list_asset.html
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/templatetags/list_item.html
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/templatetags/list_tax_item.html
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templates/structures/templatetags/list_title.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templatetags/__init__.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/templatetags/structures.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/__init__.py
--rw-r--r--   0        0        0    21127 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_admin.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_checks.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_helpers.py
--rw-r--r--   0        0        0    20151 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_integration.py
--rw-r--r--   0        0        0    26102 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_managers_1.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_managers_3.py
--rw-r--r--   0        0        0    18409 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_tasks.py
--rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/test_views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/__init__.py
--rw-r--r--   0        0        0    13532 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_notification_embeds.py
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_notification_structuretimers.py
--rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_notifications_timerboard.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_serializers.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_sovereignty.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/core/test_starbases.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/__init__.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_eveuniverse.py
--rw-r--r--   0        0        0    38429 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_notifications_1.py
--rw-r--r--   0        0        0    31553 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_notifications_2.py
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_notifications_3.py
--rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_notifications_discord.py
--rw-r--r--   0        0        0    26807 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_owners_1.py
--rw-r--r--   0        0        0    54158 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_owners_2.py
--rw-r--r--   0        0        0    37407 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_owners_3.py
--rw-r--r--   0        0        0    37744 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/models/test_structures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/__init__.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0    33188 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/entities.json
--rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/esi_data.json
--rw-r--r--   0        0        0   979813 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/factories.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/factories_2.py
--rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/generate_notifications.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/generate_notifications_2.py
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/generate_structures.py
--rw-r--r--   0        0        0    26820 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/helpers.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/tasks_loadtest.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/tests/testdata/test_generate_structures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/__init__.py
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/core.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/managers.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/tests/__init__.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/tests/test_core.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_structures-2.3.0/structures/webhooks/tests/test_utils.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 aa_structures-2.3.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_structures-2.3.0/LICENSE
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 aa_structures-2.3.0/README.md
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 aa_structures-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 aa_structures-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/__init__.py
+-rw-r--r--   0        0        0    36110 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/admin.py
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/app_settings.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/apps.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/auth_hooks.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/checks.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/constants.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/forms.py
+-rw-r--r--   0        0        0    18949 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/managers.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/providers.py
+-rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/swagger.json
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tasks.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/urls.py
+-rw-r--r--   0        0        0    21820 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/core/__init__.py
+-rw-r--r--   0        0        0    71519 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/core/notification_embeds.py
+-rw-r--r--   0        0        0    16436 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/core/notification_timers.py
+-rw-r--r--   0        0        0    19834 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/core/serializers.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/core/sovereignty.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/core/starbases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/helpers/__init__.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/helpers/general.py
+-rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/django.pot
+-rw-r--r--   0        0        0    13634 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    61204 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47274 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    55691 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47267 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47024 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47227 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47437 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47505 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    58962 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/management/commands/__init__.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/management/commands/structures_load_eve.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/management/commands/structures_preload_eveuniverse.py
+-rw-r--r--   0        0        0    59315 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/migrations/0002_remove_eveuniverse_relation_names.py
+-rw-r--r--   0        0        0    44042 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/migrations/0003_add_localization_and_unique_key.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/migrations/__init__.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/models/__init__.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/models/eveuniverse.py
+-rw-r--r--   0        0        0    42745 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/models/notifications.py
+-rw-r--r--   0        0        0    53967 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/models/owners.py
+-rw-r--r--   0        0        0    37256 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/models/structures.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/css/global.css
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/css/main.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/eve_symbol_128.png
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/structures_logo.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/0h.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/0l.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/0m.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/0r.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/0s.png
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/1h.png
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/1l.png
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/1m.png
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/1r.png
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/2h.png
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/2l.png
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/2m.png
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/2r.png
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/3h.png
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/3l.png
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/3m.png
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/3r.png
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/4h.png
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/4l.png
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/4m.png
+-rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/4s.png
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/5h.png
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/5l.png
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/5m.png
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/5s.png
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/6h.png
+-rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/6l.png
+-rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/6m.png
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/7h.png
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/7l.png
+-rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/7m.png
+-rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/8h.png
+-rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/8l.png
+-rw-r--r--   0        0        0     9541 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/8m.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/blank.png
+-rw-r--r--   0        0        0    16840 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/circle.png
+-rw-r--r--   0        0        0    33523 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/dustwheel.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/h.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/l.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/m.png
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/noship.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/r.png
+-rw-r--r--   0        0        0    43642 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/tyrannis.png
+-rw-r--r--   0        0        0    43560 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/tyrannis_blue.png
+-rw-r--r--   0        0        0    42833 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/tyrannis_darkred.png
+-rw-r--r--   0        0        0    38343 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/tyrannis_default.png
+-rw-r--r--   0        0        0    42868 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/static/structures/img/panel/tyrannis_revelations.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/base.html
+-rw-r--r--   0        0        0    21200 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/main.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/modals/fitting_assets.html
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/modals/fitting_gfx.html
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/modals/poco_details.html
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/modals/starbase_detail.html
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/modals/structure_details.html
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/modals/tab_general_detail.html
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/partials/jump_gates_list.html
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/partials/poco_list.html
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/partials/structure_list.html
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/partials/structure_summary.html
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/templatetags/detail_title.html
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/templatetags/list_asset.html
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/templatetags/list_item.html
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/templatetags/list_tax_item.html
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templates/structures/templatetags/list_title.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templatetags/__init__.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/templatetags/structures.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/__init__.py
+-rw-r--r--   0        0        0    21127 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/test_admin.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/test_checks.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/test_helpers.py
+-rw-r--r--   0        0        0    23524 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/test_integration.py
+-rw-r--r--   0        0        0    26102 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/test_managers_1.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/test_managers_3.py
+-rw-r--r--   0        0        0    18409 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/test_tasks.py
+-rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/test_views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/core/__init__.py
+-rw-r--r--   0        0        0    13532 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/core/test_notification_embeds.py
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/core/test_notification_structuretimers.py
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/core/test_notifications_timerboard.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/core/test_serializers.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/core/test_sovereignty.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/core/test_starbases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/models/__init__.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/models/test_eveuniverse.py
+-rw-r--r--   0        0        0    39346 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/models/test_notifications_1.py
+-rw-r--r--   0        0        0    31553 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/models/test_notifications_2.py
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/models/test_notifications_3.py
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/models/test_notifications_discord.py
+-rw-r--r--   0        0        0    26807 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/models/test_owners_1.py
+-rw-r--r--   0        0        0    54158 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/models/test_owners_2.py
+-rw-r--r--   0        0        0    37407 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/models/test_owners_3.py
+-rw-r--r--   0        0        0    37744 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/models/test_structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    33188 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/entities.json
+-rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0   979813 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/factories.py
+-rw-r--r--   0        0        0    10857 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/factories_2.py
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/generate_notifications.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/generate_notifications_2.py
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/generate_structures.py
+-rw-r--r--   0        0        0    26820 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/helpers.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/tasks_loadtest.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/tests/testdata/test_generate_structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/webhooks/__init__.py
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/webhooks/core.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/webhooks/managers.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/webhooks/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/webhooks/tests/__init__.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/webhooks/tests/test_core.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/structures/webhooks/tests/test_utils.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/LICENSE
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/README.md
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/pyproject.toml
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 aa_structures-2.3.1b1/PKG-INFO
```

### Comparing `aa_structures-2.3.0/structures/admin.py` & `aa_structures-2.3.1b1/structures/admin.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/app_settings.py` & `aa_structures-2.3.1b1/structures/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/auth_hooks.py` & `aa_structures-2.3.1b1/structures/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/checks.py` & `aa_structures-2.3.1b1/structures/checks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/constants.py` & `aa_structures-2.3.1b1/structures/constants.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/managers.py` & `aa_structures-2.3.1b1/structures/managers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/swagger.json` & `aa_structures-2.3.1b1/structures/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tasks.py` & `aa_structures-2.3.1b1/structures/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/urls.py` & `aa_structures-2.3.1b1/structures/urls.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/views.py` & `aa_structures-2.3.1b1/structures/views.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/core/notification_embeds.py` & `aa_structures-2.3.1b1/structures/core/notification_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/core/notification_timers.py` & `aa_structures-2.3.1b1/structures/core/notification_timers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/core/serializers.py` & `aa_structures-2.3.1b1/structures/core/serializers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/core/sovereignty.py` & `aa_structures-2.3.1b1/structures/core/sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/core/starbases.py` & `aa_structures-2.3.1b1/structures/core/starbases.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/helpers/general.py` & `aa_structures-2.3.1b1/structures/helpers/general.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/django.pot` & `aa_structures-2.3.1b1/structures/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/de/LC_MESSAGES/django.mo` & `aa_structures-2.3.1b1/structures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/de/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/en/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/es/LC_MESSAGES/django.mo` & `aa_structures-2.3.1b1/structures/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/es/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/fr_FR/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/it_IT/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/ja/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/ko/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/ko_KR/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/ru/LC_MESSAGES/django.mo` & `aa_structures-2.3.1b1/structures/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/ru/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/uk/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_structures-2.3.1b1/structures/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_structures-2.3.1b1/structures/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/management/commands/structures_load_eve.py` & `aa_structures-2.3.1b1/structures/management/commands/structures_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/management/commands/structures_preload_eveuniverse.py` & `aa_structures-2.3.1b1/structures/management/commands/structures_preload_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/migrations/0001_initial_new.py` & `aa_structures-2.3.1b1/structures/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/migrations/0002_remove_eveuniverse_relation_names.py` & `aa_structures-2.3.1b1/structures/migrations/0002_remove_eveuniverse_relation_names.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/migrations/0003_add_localization_and_unique_key.py` & `aa_structures-2.3.1b1/structures/migrations/0003_add_localization_and_unique_key.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/models/eveuniverse.py` & `aa_structures-2.3.1b1/structures/models/eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/models/notifications.py` & `aa_structures-2.3.1b1/structures/models/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
             # sov
             cls.SOV_ENTOSIS_CAPTURE_STARTED,
             cls.SOV_COMMAND_NODE_EVENT_STARTED,
             cls.SOV_ALL_CLAIM_ACQUIRED_MSG,
             cls.SOV_STRUCTURE_REINFORCED,
             cls.SOV_STRUCTURE_DESTROYED,
             cls.SOV_ALL_CLAIM_LOST_MSG,
-            cls.SOV_ALL_ANCHORING_MSG,
+            # cls.SOV_ALL_ANCHORING_MSG, # This notif is not broadcasted to all corporations
             # wars
             cls.WAR_ALLY_JOINED_WAR_AGGRESSOR_MSG,
             cls.WAR_ALLY_JOINED_WAR_AllY_MSG,
             cls.WAR_ALLY_JOINED_WAR_DEFENDER_MSG,
             cls.WAR_CORP_WAR_SURRENDER_MSG,
             cls.WAR_CORPORATION_BECAME_ELIGIBLE,
             cls.WAR_CORPORATION_NO_LONGER_ELIGIBLE,
```

### Comparing `aa_structures-2.3.0/structures/models/owners.py` & `aa_structures-2.3.1b1/structures/models/owners.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/models/structures.py` & `aa_structures-2.3.1b1/structures/models/structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/css/global.css` & `aa_structures-2.3.1b1/structures/static/structures/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/css/main.css` & `aa_structures-2.3.1b1/structures/static/structures/css/main.css`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/Spinner-1s-64px-dark.gif` & `aa_structures-2.3.1b1/structures/static/structures/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/Spinner-1s-64px-light.gif` & `aa_structures-2.3.1b1/structures/static/structures/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/eve_symbol_128.png` & `aa_structures-2.3.1b1/structures/static/structures/img/eve_symbol_128.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/0h.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/0h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/0l.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/0l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/0m.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/0m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/0r.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/0r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/0s.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/0s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/1h.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/1h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/1l.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/1l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/1m.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/1m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/1r.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/1r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/2h.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/2h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/2l.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/2l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/2m.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/2m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/2r.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/2r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/3h.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/3h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/3l.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/3l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/3m.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/3m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/3r.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/3r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/4h.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/4h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/4l.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/4l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/4m.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/4m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/4s.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/4s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/5h.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/5h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/5l.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/5l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/5m.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/5m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/5s.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/5s.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/6h.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/6h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/6l.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/6l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/6m.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/6m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/7h.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/7h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/7l.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/7l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/7m.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/7m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/8h.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/8h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/8l.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/8l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/8m.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/8m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/circle.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/circle.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/dustwheel.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/h.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/h.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/l.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/l.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/m.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/m.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/noship.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/noship.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/r.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/r.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_blue.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_darkred.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_default.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/static/structures/img/panel/tyrannis_revelations.png` & `aa_structures-2.3.1b1/structures/static/structures/img/panel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/main.html` & `aa_structures-2.3.1b1/structures/templates/structures/main.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/modals/fitting_gfx.html` & `aa_structures-2.3.1b1/structures/templates/structures/modals/fitting_gfx.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/modals/poco_details.html` & `aa_structures-2.3.1b1/structures/templates/structures/modals/poco_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/modals/starbase_detail.html` & `aa_structures-2.3.1b1/structures/templates/structures/modals/starbase_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/modals/structure_details.html` & `aa_structures-2.3.1b1/structures/templates/structures/modals/structure_details.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/modals/tab_general_detail.html` & `aa_structures-2.3.1b1/structures/templates/structures/modals/tab_general_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/partials/jump_gates_list.html` & `aa_structures-2.3.1b1/structures/templates/structures/partials/jump_gates_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/partials/poco_list.html` & `aa_structures-2.3.1b1/structures/templates/structures/partials/poco_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/partials/structure_list.html` & `aa_structures-2.3.1b1/structures/templates/structures/partials/structure_list.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/partials/structure_summary.html` & `aa_structures-2.3.1b1/structures/templates/structures/partials/structure_summary.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templates/structures/templatetags/list_item.html` & `aa_structures-2.3.1b1/structures/templates/structures/templatetags/list_item.html`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/templatetags/structures.py` & `aa_structures-2.3.1b1/structures/templatetags/structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/test_admin.py` & `aa_structures-2.3.1b1/structures/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/test_checks.py` & `aa_structures-2.3.1b1/structures/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/test_helpers.py` & `aa_structures-2.3.1b1/structures/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/test_integration.py` & `aa_structures-2.3.1b1/structures/tests/test_integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 from app_utils.django import app_labels
 from app_utils.esi import EsiStatus
 from app_utils.esi_testing import EsiClientStub, EsiEndpoint
 
 from .. import tasks
 from ..models import NotificationType, Structure
 from .testdata.factories_2 import (
+    EveEntityAllianceFactory,
     EveEntityCorporationFactory,
     NotificationFactory,
     OwnerFactory,
+    RawNotificationFactory,
     StarbaseFactory,
     StructureFactory,
     WebhookFactory,
     datetime_to_esi,
 )
 from .testdata.load_eveuniverse import load_eveuniverse
 
@@ -427,14 +429,99 @@
 
         if StructureTimer:
             self.assertTrue(StructureTimer.objects.exists())
 
         if AuthTimer:
             self.assertTrue(AuthTimer.objects.exists())
 
+    def test_should_fetch_and_send_notification_when_enabled_for_webhook(
+        self, mock_esi_2, mock_esi, mock_execute
+    ):
+        # given
+        webhook = WebhookFactory(
+            notification_types=[NotificationType.WAR_CORPORATION_BECAME_ELIGIBLE]
+        )
+        owner = OwnerFactory(webhooks=[webhook], is_alliance_main=True)
+        eve_character = owner.characters.first().character_ownership.character
+        # corporation_id = owner.corporation.corporation_id
+        notif = RawNotificationFactory()
+        endpoints = [
+            EsiEndpoint(
+                "Character",
+                "get_characters_character_id_notifications",
+                "character_id",
+                needs_token=True,
+                data={
+                    str(eve_character.character_id): [notif],
+                },
+            ),
+        ]
+        mock_esi.client = mock_esi_2.client = EsiClientStub.create_from_endpoints(
+            endpoints
+        )
+        # when
+        tasks.fetch_all_notifications.delay()
+        # then
+        self.assertTrue(mock_execute.called)
+        embed = mock_execute.call_args[1]["embeds"][0]
+        self.assertIn("now eligible", embed.description)
+
+    def test_should_fetch_and_send_notification_when_enabled_for_webhook_all_anchoring(
+        self, mock_esi_2, mock_esi, mock_execute
+    ):
+        # given
+        webhook = WebhookFactory(
+            notification_types=[NotificationType.SOV_ALL_ANCHORING_MSG]
+        )
+        owner = OwnerFactory(webhooks=[webhook], is_alliance_main=False)
+        eve_character = owner.characters.first().character_ownership.character
+        alliance = EveEntityAllianceFactory(
+            id=owner.corporation.alliance_id,
+            name=owner.corporation.alliance.alliance_name,
+        )
+        corporation = EveEntityCorporationFactory(
+            id=owner.corporation.corporation_id, name=owner.corporation.corporation_name
+        )
+        starbase = StarbaseFactory(owner=owner)
+        notif = RawNotificationFactory(
+            type="AllAnchoringMsg",
+            sender=corporation,
+            data={
+                "allianceID": alliance.id,
+                "corpID": corporation.id,
+                "corpsPresent": [{"allianceID": alliance.id, "corpID": corporation.id}],
+                "moonID": starbase.eve_moon.id,
+                "solarSystemID": starbase.eve_solar_system.id,
+                "towers": [
+                    {"moonID": starbase.eve_moon.id, "typeID": starbase.eve_type.id}
+                ],
+                "typeID": starbase.eve_type.id,
+            },
+        )
+        endpoints = [
+            EsiEndpoint(
+                "Character",
+                "get_characters_character_id_notifications",
+                "character_id",
+                needs_token=True,
+                data={
+                    str(eve_character.character_id): [notif],
+                },
+            ),
+        ]
+        mock_esi.client = mock_esi_2.client = EsiClientStub.create_from_endpoints(
+            endpoints
+        )
+        # when
+        tasks.fetch_all_notifications.delay()
+        # then
+        self.assertTrue(mock_execute.called)
+        embed = mock_execute.call_args[1]["embeds"][0]
+        self.assertIn("has anchored in", embed.description)
+
     @patch(NOTIFICATIONS_PATH + ".STRUCTURES_ADD_TIMERS", True)
     def test_should_fetch_new_notification_from_esi_and_send_to_webhook_and_create_timers(
         self, mock_esi_2, mock_esi, mock_execute
     ):
         # given
         sender = EveEntityCorporationFactory()
         structure = StructureFactory(
@@ -504,15 +591,15 @@
             notification_types=[
                 NotificationType.SOV_STRUCTURE_REINFORCED,
                 NotificationType.SOV_STRUCTURE_DESTROYED,
                 NotificationType.SOV_ALL_CLAIM_ACQUIRED_MSG,
                 NotificationType.SOV_ALL_CLAIM_LOST_MSG,
             ]
         )
-        owner = OwnerFactory(webhooks=[webhook])
+        owner = OwnerFactory(webhooks=[webhook], is_alliance_main=True)
         NotificationFactory(
             owner=owner, notif_type=NotificationType.STRUCTURE_DESTROYED
         )
         NotificationFactory(
             owner=owner,
             notif_type=NotificationType.SOV_STRUCTURE_DESTROYED,
             text_from_dict={"solarSystemID": 30000474, "structureTypeID": 32226},
```

### Comparing `aa_structures-2.3.0/structures/tests/test_managers_1.py` & `aa_structures-2.3.1b1/structures/tests/test_managers_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/test_managers_3.py` & `aa_structures-2.3.1b1/structures/tests/test_managers_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/test_tasks.py` & `aa_structures-2.3.1b1/structures/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/test_views.py` & `aa_structures-2.3.1b1/structures/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/core/test_notification_embeds.py` & `aa_structures-2.3.1b1/structures/tests/core/test_notification_embeds.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/core/test_notification_structuretimers.py` & `aa_structures-2.3.1b1/structures/tests/core/test_notification_structuretimers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/core/test_notifications_timerboard.py` & `aa_structures-2.3.1b1/structures/tests/core/test_notifications_timerboard.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/core/test_serializers.py` & `aa_structures-2.3.1b1/structures/tests/core/test_serializers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/core/test_sovereignty.py` & `aa_structures-2.3.1b1/structures/tests/core/test_sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/core/test_starbases.py` & `aa_structures-2.3.1b1/structures/tests/core/test_starbases.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/models/test_eveuniverse.py` & `aa_structures-2.3.1b1/structures/tests/models/test_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/models/test_notifications_1.py` & `aa_structures-2.3.1b1/structures/tests/models/test_notifications_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,55 +117,81 @@
         _, cls.owner = set_owner_character(character_id=1001)
         load_notification_entities(cls.owner)
 
     def test_should_not_filter_non_alliance_notifications_1(self):
         # given
         self.owner.is_alliance_main = False
         self.owner.save()
-        notif = self.owner.notification_set.get(notification_id=1000000509)
+        notifs = self.owner.notification_set.exclude(
+            notif_type__in=NotificationType.relevant_for_alliance_level
+        )
         # when/then
-        self.assertFalse(notif.filter_for_alliance_level())
+        for notif in notifs:
+            with self.subTest(notif=str(notif)):
+                self.assertFalse(notif.filter_for_alliance_level())
 
     def test_should_not_filter_non_alliance_notifications_2(self):
         # given
         self.owner.is_alliance_main = True
         self.owner.save()
-        notif = self.owner.notification_set.get(notification_id=1000000509)
+        notifs = self.owner.notification_set.exclude(
+            notif_type__in=NotificationType.relevant_for_alliance_level
+        )
         # when/then
-        self.assertFalse(notif.filter_for_alliance_level())
+        for notif in notifs:
+            with self.subTest(notif=str(notif)):
+                self.assertFalse(notif.filter_for_alliance_level())
 
     def test_should_filter_alliance_notifications(self):
         # given
         self.owner.is_alliance_main = False
         self.owner.save()
-        notif = self.owner.notification_set.get(notification_id=1000000803)
+        notifs = self.owner.notification_set.filter(
+            notif_type__in=NotificationType.relevant_for_alliance_level
+        )
         # when/then
-        self.assertTrue(notif.filter_for_alliance_level())
+        for notif in notifs:
+            with self.subTest(notif=str(notif)):
+                self.assertTrue(notif.filter_for_alliance_level())
 
     def test_should_not_filter_alliance_notifications_1(self):
         # given
         self.owner.is_alliance_main = True
         self.owner.save()
+        notifs = self.owner.notification_set.filter(
+            notif_type__in=NotificationType.relevant_for_alliance_level
+        )
         # when/then
-        notif = self.owner.notification_set.get(notification_id=1000000803)
-        self.assertFalse(notif.filter_for_alliance_level())
+        for notif in notifs:
+            with self.subTest(notif=str(notif)):
+                self.assertFalse(notif.filter_for_alliance_level())
 
     def test_should_not_filter_alliance_notifications_2(self):
         # given
         self.owner.is_alliance_main = True
         self.owner.save()
-        notif = self.owner.notification_set.get(notification_id=1000000803)
-        self.assertFalse(notif.filter_for_alliance_level())
+        notifs = self.owner.notification_set.filter(
+            notif_type__in=NotificationType.relevant_for_alliance_level
+        )
+        # when/then
+        for notif in notifs:
+            with self.subTest(notif=str(notif)):
+                self.assertFalse(notif.filter_for_alliance_level())
 
     def test_should_not_filter_alliance_notifications_3(self):
         # given
         _, owner = set_owner_character(character_id=1102)  # corp with no alliance
         load_notification_entities(owner)
-        notif = owner.notification_set.get(notification_id=1000000803)
-        self.assertFalse(notif.filter_for_alliance_level())
+        notifs = self.owner.notification_set.filter(
+            notif_type__in=NotificationType.relevant_for_alliance_level
+        )
+        # when/then
+        for notif in notifs:
+            with self.subTest(notif=str(notif)):
+                self.assertFalse(notif.filter_for_alliance_level())
 
 
 class TestNotificationCreateFromStructure(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
```

### Comparing `aa_structures-2.3.0/structures/tests/models/test_notifications_2.py` & `aa_structures-2.3.1b1/structures/tests/models/test_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/models/test_notifications_3.py` & `aa_structures-2.3.1b1/structures/tests/models/test_notifications_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/models/test_notifications_discord.py` & `aa_structures-2.3.1b1/structures/tests/models/test_notifications_discord.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/models/test_owners_1.py` & `aa_structures-2.3.1b1/structures/tests/models/test_owners_1.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/models/test_owners_2.py` & `aa_structures-2.3.1b1/structures/tests/models/test_owners_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/models/test_owners_3.py` & `aa_structures-2.3.1b1/structures/tests/models/test_owners_3.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/models/test_structures.py` & `aa_structures-2.3.1b1/structures/tests/models/test_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/testdata/create_eveuniverse.py` & `aa_structures-2.3.1b1/structures/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/testdata/entities.json` & `aa_structures-2.3.1b1/structures/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/testdata/esi_data.json` & `aa_structures-2.3.1b1/structures/tests/testdata/esi_data.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/testdata/eveuniverse.json` & `aa_structures-2.3.1b1/structures/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/testdata/factories.py` & `aa_structures-2.3.1b1/structures/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/testdata/factories_2.py` & `aa_structures-2.3.1b1/structures/tests/testdata/factories_2.py`

 * *Files 9% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     class Meta:
         model = Owner
         django_get_or_create = ("corporation",)
 
     assets_last_update_at = factory.LazyFunction(now)
     character_ownership = None  # no longer used
     forwarding_last_update_at = factory.LazyFunction(now)
-    is_alliance_main = True
+    is_alliance_main = False
     is_up = True
     notifications_last_update_at = factory.LazyFunction(now)
     structures_last_update_at = factory.LazyFunction(now)
     corporation = factory.SubFactory(EveCorporationInfoFactory)
 
     @factory.post_generation
     def characters(
@@ -326,7 +326,40 @@
         reinforced_until = dt.datetime.fromisoformat(obj.details["reinforced_until"])
         starbase = StarbaseFactory(
             owner=obj.owner,
             state=Structure.State.POS_REINFORCED,
             state_timer_end=reinforced_until,
         )
         obj.structures.add(starbase)
+
+
+class RawNotificationFactory(factory.DictFactory):
+    """Create a raw notification as received from ESI."""
+
+    class Meta:
+        exclude = ("data", "timestamp_dt", "sender")
+
+    # excluded
+    data = None
+    timestamp_dt = None
+    sender = factory.SubFactory(EveEntityCorporationFactory, id=2902, name="CONCORD")
+
+    # included
+    notification_id = factory.Sequence(lambda o: 1999000000 + o)
+    type = "CorpBecameWarEligible"
+    sender_id = factory.LazyAttribute(lambda o: o.sender.id)
+    sender_type = factory.LazyAttribute(lambda o: o.sender.category)
+    is_read = True
+
+    @factory.lazy_attribute
+    def timestamp(self):
+        if not self.timestamp_dt:
+            timestamp_dt = now()
+        else:
+            timestamp_dt = self.timestamp_dt
+        return datetime_to_esi(timestamp_dt)
+
+    @factory.lazy_attribute
+    def text(self):
+        if not self.data:
+            return ""
+        return yaml.dump(self.data)
```

### Comparing `aa_structures-2.3.0/structures/tests/testdata/generate_notifications.py` & `aa_structures-2.3.1b1/structures/tests/testdata/generate_notifications.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/testdata/generate_notifications_2.py` & `aa_structures-2.3.1b1/structures/tests/testdata/generate_notifications_2.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/testdata/generate_structures.py` & `aa_structures-2.3.1b1/structures/tests/testdata/generate_structures.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/testdata/helpers.py` & `aa_structures-2.3.1b1/structures/tests/testdata/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/tests/testdata/tasks_loadtest.py` & `aa_structures-2.3.1b1/structures/tests/testdata/tasks_loadtest.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/webhooks/core.py` & `aa_structures-2.3.1b1/structures/webhooks/core.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/webhooks/managers.py` & `aa_structures-2.3.1b1/structures/webhooks/managers.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/webhooks/models.py` & `aa_structures-2.3.1b1/structures/webhooks/models.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/structures/webhooks/tests/test_core.py` & `aa_structures-2.3.1b1/structures/webhooks/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/LICENSE` & `aa_structures-2.3.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/README.md` & `aa_structures-2.3.1b1/README.md`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/pyproject.toml` & `aa_structures-2.3.1b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_structures-2.3.0/PKG-INFO` & `aa_structures-2.3.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-structures
-Version: 2.3.0
+Version: 2.3.1b1
 Summary: App for managing Eve Online structures with Alliance Auth
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-structures
 Project-URL: Documentation, https://aa-structures.readthedocs.io/en/latest/
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-structures
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-structures/-/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-structures/-/issues
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
```

