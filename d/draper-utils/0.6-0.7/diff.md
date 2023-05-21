# Comparing `tmp/draper-utils-0.6.tar.gz` & `tmp/draper-utils-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draper-utils-0.6.tar", last modified: Mon Mar  6 19:07:29 2023, max compression
+gzip compressed data, was "draper-utils-0.7.tar", last modified: Sun May 21 15:48:14 2023, max compression
```

## Comparing `draper-utils-0.6.tar` & `draper-utils-0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 19:07:29.476862 draper-utils-0.6/
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 draper-utils-0.6/LICENCE.txt
--rw-rw-rw-   0        0        0      355 2023-03-06 19:07:29.475862 draper-utils-0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 draper-utils-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-06 19:07:29.425861 draper-utils-0.6/draper_utils/
--rw-rw-rw-   0        0        0        0 2023-01-28 21:06:51.000000 draper-utils-0.6/draper_utils/__init__.py
--rw-rw-rw-   0        0        0       66 2023-01-28 21:06:51.000000 draper-utils-0.6/draper_utils/admin.py
--rw-rw-rw-   0        0        0      161 2023-01-28 21:06:51.000000 draper-utils-0.6/draper_utils/apps.py
-drwxrwxrwx   0        0        0        0 2023-03-06 19:07:29.436860 draper-utils-0.6/draper_utils/management/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 draper-utils-0.6/draper_utils/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 19:07:29.448860 draper-utils-0.6/draper_utils/management/commands/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 draper-utils-0.6/draper_utils/management/commands/__init__.py
--rw-rw-rw-   0        0        0    13677 2023-03-03 02:58:21.000000 draper-utils-0.6/draper_utils/management/commands/import_projects.py
--rw-rw-rw-   0        0        0    10160 2023-01-31 19:04:52.000000 draper-utils-0.6/draper_utils/management/commands/setup_project_center.py
-drwxrwxrwx   0        0        0        0 2023-03-06 19:07:29.449860 draper-utils-0.6/draper_utils/migrations/
--rw-rw-rw-   0        0        0        0 2023-01-28 21:06:51.000000 draper-utils-0.6/draper_utils/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-01-28 21:06:51.000000 draper-utils-0.6/draper_utils/models.py
-drwxrwxrwx   0        0        0        0 2023-03-06 19:07:29.474860 draper-utils-0.6/draper_utils/sql/
--rw-rw-rw-   0        0        0       79 2023-01-04 12:10:24.000000 draper-utils-0.6/draper_utils/sql/list_project_activities.sql
--rw-rw-rw-   0        0        0      279 2023-02-09 18:41:35.000000 draper-utils-0.6/draper_utils/sql/list_project_assigned_users.sql
--rw-rw-rw-   0        0        0      228 2023-02-16 02:03:32.000000 draper-utils-0.6/draper_utils/sql/list_project_categories.sql
--rw-rw-rw-   0        0        0      172 2023-01-02 16:39:10.000000 draper-utils-0.6/draper_utils/sql/list_project_stages.sql
--rw-rw-rw-   0        0        0      178 2023-01-02 16:22:17.000000 draper-utils-0.6/draper_utils/sql/list_project_statuses.sql
--rw-rw-rw-   0        0        0      609 2023-02-05 20:55:33.000000 draper-utils-0.6/draper_utils/sql/list_project_users.sql
--rw-rw-rw-   0        0        0      399 2023-01-14 16:07:20.000000 draper-utils-0.6/draper_utils/sql/list_projects.sql
--rw-rw-rw-   0        0        0       63 2023-01-28 21:06:51.000000 draper-utils-0.6/draper_utils/tests.py
--rw-rw-rw-   0        0        0     7345 2023-01-29 13:45:21.000000 draper-utils-0.6/draper_utils/utils.py
--rw-rw-rw-   0        0        0       66 2023-01-28 21:06:51.000000 draper-utils-0.6/draper_utils/views.py
-drwxrwxrwx   0        0        0        0 2023-03-06 19:07:29.435862 draper-utils-0.6/draper_utils.egg-info/
--rw-rw-rw-   0        0        0      355 2023-03-06 19:07:29.000000 draper-utils-0.6/draper_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      925 2023-03-06 19:07:29.000000 draper-utils-0.6/draper_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 19:07:29.000000 draper-utils-0.6/draper_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-31 20:41:35.000000 draper-utils-0.6/draper_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-03-06 19:07:29.000000 draper-utils-0.6/draper_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-06 19:07:29.000000 draper-utils-0.6/draper_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-06 19:07:29.476862 draper-utils-0.6/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-03-06 19:06:28.000000 draper-utils-0.6/setup.py
+drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2023-05-21 15:48:14.343786 draper-utils-0.7/
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2023-04-25 12:52:17.000000 draper-utils-0.7/LICENCE.txt
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      331 2023-05-21 15:48:14.343786 draper-utils-0.7/PKG-INFO
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2023-04-25 12:52:17.000000 draper-utils-0.7/README.md
+drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2023-05-21 15:48:14.343786 draper-utils-0.7/draper_utils/
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/__init__.py
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)       63 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/admin.py
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      155 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/apps.py
+drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2023-05-21 15:48:14.343786 draper-utils-0.7/draper_utils/management/
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/management/__init__.py
+drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2023-05-21 15:48:14.343786 draper-utils-0.7/draper_utils/management/commands/
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/management/commands/__init__.py
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)    13951 2023-05-21 12:56:03.000000 draper-utils-0.7/draper_utils/management/commands/import_projects.py
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)     3095 2023-05-07 14:12:45.000000 draper-utils-0.7/draper_utils/management/commands/setup_project_center.py
+drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2023-05-21 15:48:14.343786 draper-utils-0.7/draper_utils/migrations/
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/migrations/__init__.py
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)       57 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/models.py
+drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2023-05-21 15:48:14.343786 draper-utils-0.7/draper_utils/sql/
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)       79 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/sql/list_project_activities.sql
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      270 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/sql/list_project_assigned_users.sql
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      228 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/sql/list_project_categories.sql
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      172 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/sql/list_project_stages.sql
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      178 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/sql/list_project_statuses.sql
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      609 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/sql/list_project_users.sql
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      399 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/sql/list_projects.sql
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)       60 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/tests.py
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)     7169 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/utils.py
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)       63 2023-04-25 12:52:17.000000 draper-utils-0.7/draper_utils/views.py
+drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2023-05-21 15:48:14.343786 draper-utils-0.7/draper_utils.egg-info/
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      331 2023-05-21 15:48:14.000000 draper-utils-0.7/draper_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      925 2023-05-21 15:48:14.000000 draper-utils-0.7/draper_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        1 2023-05-21 15:48:14.000000 draper-utils-0.7/draper_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        1 2023-04-25 12:53:21.000000 draper-utils-0.7/draper_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        7 2023-05-21 15:48:14.000000 draper-utils-0.7/draper_utils.egg-info/requires.txt
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)       13 2023-05-21 15:48:14.000000 draper-utils-0.7/draper_utils.egg-info/top_level.txt
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)       38 2023-05-21 15:48:14.343786 draper-utils-0.7/setup.cfg
+-rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      915 2023-05-21 15:48:09.000000 draper-utils-0.7/setup.py
```

### Comparing `draper-utils-0.6/draper_utils/management/commands/import_projects.py` & `draper-utils-0.7/draper_utils/management/commands/import_projects.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,296 +1,310 @@
-import time
-from genericpath import exists
-from os.path import abspath, join, dirname
-import requests
-
-from sqlalchemy import create_engine
-from sqlalchemy import text
-
-from django.contrib.auth import authenticate
-from django.core.management.base import BaseCommand
-from project_center.models import Project, ProjectCategory, ProjectStatus, ProjectStage, ProjectActivity, User, Company
-from django.conf import settings
-from django.core.files.base import ContentFile
-from django.utils.timezone import make_aware
-from django.template.defaultfilters import slugify
-from django.contrib.auth.models import Group
-
-
-def full_path(filename):
-    return abspath(join(dirname(__file__), filename))
-
-
-class Command(BaseCommand):
-    help = """Imports Projects and related models from a legacy database."""
-
-    def add_arguments(self, parser):
-        parser.add_argument(
-            '--limit', action='store', dest='limit', default=None,
-            help="Import Limit"
-        )
-        parser.add_argument(
-            '--order', action='store', dest='order', default=None,
-            help="Import Order"
-        )
-        parser.add_argument(
-            '--reset', action='store_true', dest='reset', default=False,
-            help="Clear all projects before importing"
-        )
-
-    def import_projects(self, engine, file, limit=None, order=None):
-        with engine.connect() as conn:
-            with open(file) as file:
-                query = file.read()
-                if order:
-                    query = str(query).strip()
-                    query += ' ORDER BY ' + order
-                if limit:
-                    query = str(query).strip()
-                    query += ' LIMIT ' + limit
-                result = conn.execute(text(query))
-                for row in result:
-                    try:
-                        project_category = ProjectCategory.objects.get(import_id=int(row.category_id))
-                    except:
-                        project_category = None
-                    try:
-                        project_status = ProjectStatus.objects.get(import_id=int(row.status_id))
-                    except:
-                        project_status = None
-                    try:
-                        project_stage = ProjectStage.objects.get(import_id=int(row.stage_id))
-                    except:
-                        project_stage = None
-                    try:
-                        project_date = make_aware(row.job_date)
-                    except:
-                        project_date = None
-
-                    company, created = Company.objects.update_or_create(name=settings.PROJECT_CENTER_DEFAULT_COMPANY_NAME)
-                    project, created = Project.objects.update_or_create(
-                        import_id=int(row.project_id),
-                    defaults={
-                        'title':row.project_title,
-                        'slug':'{slug}-{project_id}'.format(slug=slugify(row.project_title), project_id=row.project_id),
-                        'date':project_date,
-                        'code':row.project_code,
-                        'internal':row.is_internal,
-                        'category': project_category,
-                        'status': project_status,
-                        'stage': project_stage,
-                        'company':company
-                    })
-
-                    project.save()
-                    # first_rec = (project.history.first())
-                    # last_rec = (project.history.last())
-                    # first_rec.history_date = row.job_date
-                    # first_rec.history_change_reason = 'Project Created'
-                    # first_rec.history_type = '+'
-                    # first_rec.history_user_id = User.objects.get(import_id=row.user_id).id
-                    # first_rec.save()
-                    # last_rec.delete()
-                    print('Importing Project ' + project.title + '...')
-                    activities = self.import_project_activities(
-                        engine=engine,
-                        file=full_path('../../sql/list_project_activities.sql'),
-                        project=project,
-                        limit=None)
-                    assigned_users = self.import_project_assigned_users(engine=engine, project=project, limit=None)
-                    print('Project {title} import complete. Activities: {num_activities}. Users: {num_users}'.format(
-                        title=project.title,
-                        num_users=str(len(assigned_users)),
-                        num_activities=str(len(activities))))
-
-    def import_project_categories(self, engine, file):
-        with engine.connect() as conn:
-            with open(file) as file:
-                query = text(file.read())
-                result = conn.execute(query)
-                for row in result:
-                    category, created = ProjectCategory.objects.update_or_create(
-                        import_id=int(row.category_id),
-                    defaults={
-                        'name':row.category_name,
-                        'display':row.category_enabled,
-                    })
-
-    def import_project_status(self, engine, file):
-        with engine.connect() as conn:
-            with open(file) as file:
-                query = text(file.read())
-                result = conn.execute(query)
-                for row in result:
-                    status, created = ProjectStatus.objects.update_or_create(
-                        import_id=int(row.status_id),
-                    defaults={
-                        'name':row.status_name,
-                        'display': row.status_enabled,
-                    })
-
-
-    def import_project_stages(self, engine, file):
-        with engine.connect() as conn:
-            with open(file) as file:
-                query = text(file.read())
-                result = conn.execute(query)
-                for row in result:
-                    status, created = ProjectStage.objects.update_or_create(
-                        import_id=int(row.stage_id),
-                    defaults={
-                        'name':row.stage_name,
-                        'display':row.stage_enabled,
-                    })
-
-    def import_project_users(self, engine, file):
-        company, created = Company.objects.update_or_create(name=settings.PROJECT_CENTER_DEFAULT_COMPANY_NAME)
-        usergroup, created = Group.objects.get_or_create(name=settings.PROJECT_CENTER_USER_GROUP_NAME)
-        admin_usergroup, created = Group.objects.get_or_create(name=settings.PROJECT_CENTER_ADMINISTRATOR_GROUP_NAME)
-        company_admin_usergroup, created = Group.objects.get_or_create(
-            name=settings.PROJECT_CENTER_COMPANY_ADMINISTRATOR_GROUP_NAME
-        )
-
-        with engine.connect() as conn:
-            with open(file) as file:
-                query = text(file.read())
-                result = conn.execute(query)
-                for row in result:
-                    user, created = User.objects.update_or_create(
-                        import_id=int(row.user_id),
-                    defaults={
-                        'first_name':row.first_name,
-                        'last_name': row.last_name,
-                        'email': row.email,
-                        'username': row.email,
-                        'company':company,
-                        'title': row.title,
-                        'address_1': row.address_1
-                    })
-                    # if created or not user.companies:
-                    #     user.companies.add(company)
-                    #     user.save()
-                    if row.enabled == 1:
-                        user.is_staff = True
-                    else:
-                        user.is_staff = False
-                    if row.email_notify == 1:
-                        user.email_notify = True
-                    else:
-                        user.email_notify = False
-                    if created or user.groups.filter(name=settings.PROJECT_CENTER_USER_GROUP_NAME).exists() is False:
-                        user.set_password(row.password)
-                        user.groups.add(usergroup)
-                    user.save()
-
-
-    def import_project_assigned_users(self, engine, project, limit=None):
-        with engine.connect() as conn:
-            query = 'SELECT ' \
-                    'DISTINCT(ssm_commdep_projects_users.user_id), ' \
-                    'ss_users.last_name, ' \
-                    'ssm_commdep_projects_users.is_owner  ' \
-                    'FROM ' \
-                    'ssm_commdep_projects_users  ' \
-                    'LEFT JOIN ' \
-                    'ssm_commdep_projects ' \
-                    'ON  ssm_commdep_projects.id = ssm_commdep_projects_users.project_id ' \
-                    'LEFT JOIN ss_users ' \
-                    'ON ss_users.id = ssm_commdep_projects_users.user_id  ' \
-                    'WHERE ssm_commdep_projects_users.project_id = {project_id} ' \
-                    'GROUP BY ' \
-                    'ssm_commdep_projects_users.user_id, ' \
-                    'ss_users.last_name, ' \
-                    'ssm_commdep_projects_users.is_owner '.format(project_id=project.import_id)
-            result = conn.execute(text(query))
-            users = []
-            for row in result:
-                try:
-                    user = User.objects.get(
-                        import_id=int(row.user_id)
-                    )
-                    users.append(user)
-                    project.users.add(user)
-                except Exception as e:
-                    pass
-            project.save()
-            return users
-
-
-    def import_project_activities(self, engine, file, project=None, limit=None):
-        with engine.connect() as conn:
-            with open(file) as file:
-                query = 'SELECT * FROM `ssm_commdep_projects_activities` WHERE ' \
-                        'project_id = {project_id}'.format(project_id=project.import_id)
-
-                result = conn.execute(text(query))
-                activities = []
-                for row in result:
-                    try:
-                        project = Project.objects.get(import_id=int(row.project_id))
-                    except:
-                        project = None
-                    try:
-                        activity_date =  make_aware(row.activity_date)
-                    except:
-                        activity_date = None
-                    if row.file_name:
-                        url = 'http://uw.commdep.com/projects/uw/{project_id}/{activity_id}/{file_name}'.format(
-                            project_id=row.project_id,
-                            activity_id=row.activity_id,
-                            file_name=row.file_name,
-
-                        )
-
-                    else:
-                        url = None
-
-                    activity, created = ProjectActivity.objects.update_or_create(
-                        import_id=int(row.activity_id),
-                    defaults={
-                        'name':row.activity_name,
-                        'project':project,
-                        'date':activity_date,
-                        'user':User.objects.get(import_id=row.creator_id),
-                        'notes':row.notes,
-                    })
-                    activity._change_reason = activity.name
-                    activity.save()
-                    if url:
-                        r = requests.get(url)
-                        if r.status_code == 200:
-                            data = r.content
-                            filename = url.split('/')[-1]
-                            activity.file.save(filename, ContentFile(data))
-                            activity.save()
-                    activities.append(activity)
-                return activities
-
-
-    def handle(self, *args, **options):
-        engine = create_engine(settings.PROJECT_CENTER_IMPORT_DATABASE_URL)
-        limit = options['limit']
-        order = options['order']
-        reset = options['reset']
-        tic = time.perf_counter()
-        if reset:
-            projects = Project.objects.all().delete()
-            activities = ProjectActivity.objects.all().delete()
-            stages = ProjectStage.objects.all().delete()
-            statuses = ProjectStatus.objects.all().delete()
-            categories = ProjectCategory.objects.all().delete()
-            companies = Company.objects.all().delete()
-            groups = Group.objects.all().delete()
-            users = User.objects.filter(is_superuser=False).all().delete()
-        self.import_project_categories(engine, full_path('../../sql/list_project_categories.sql'))
-        self.import_project_status(engine, full_path('../../sql/list_project_statuses.sql'))
-        self.import_project_stages(engine, full_path('../../sql/list_project_stages.sql'))
-        self.import_project_users(engine, full_path('../../sql/list_project_users.sql'))
-        self.import_projects(engine, full_path('../../sql/list_projects.sql'), limit=limit, order=order)
-        # self.import_project_activities(engine, full_path('../../sql/list_project_activities.sql'), limit=limit)
-        toc = time.perf_counter()
-        print(toc - tic)
-        # if user:
-        #     user.delete()
-
-        # for x in (get_candidate_data_rest(candidate_id).keys()):
+import time
+from genericpath import exists
+from os.path import abspath, join, dirname
+import requests
+
+from sqlalchemy import create_engine
+from sqlalchemy import text
+
+from django.contrib.auth import authenticate
+from django.core.management.base import BaseCommand
+from project_center.models import Project, ProjectCategory, ProjectStatus, ProjectStage, ProjectActivity, User, Company
+from django.conf import settings
+from django.core.files.base import ContentFile
+from django.utils.timezone import make_aware
+from django.template.defaultfilters import slugify
+from django.contrib.auth.models import Group
+
+
+def full_path(filename):
+    return abspath(join(dirname(__file__), filename))
+
+
+class Command(BaseCommand):
+    help = """Imports Projects and related models from a legacy database."""
+
+    def add_arguments(self, parser):
+        parser.add_argument(
+            '--limit', action='store', dest='limit', default=None,
+            help="Import Limit"
+        )
+        parser.add_argument(
+            '--order', action='store', dest='order', default=None,
+            help="Import Order"
+        )
+        parser.add_argument(
+            '--reset', action='store_true', dest='reset', default=False,
+            help="Clear all projects before importing"
+        )
+
+        parser.add_argument(
+            '--offset', action='store', dest='offset', default=None,
+            help="Number of records to offset when beginning import sequence"
+        )
+
+    def import_projects(self, engine, file, limit=None, order=None, offset=None):
+        with engine.connect() as conn:
+            with open(file) as file:
+                query = file.read()
+                if order:
+                    query = str(query).strip()
+                    query += ' ORDER BY ' + order
+                if limit:
+                    query = str(query).strip()
+                    query += ' LIMIT ' + limit
+                if offset:
+                    query = str(query).strip()
+                    query += ' OFFSET ' + offset
+                result = conn.execute(text(query))
+                for row in result:
+                    try:
+                        project_category = ProjectCategory.objects.get(import_id=int(row.category_id))
+                    except:
+                        project_category = None
+                    try:
+                        project_status = ProjectStatus.objects.get(import_id=int(row.status_id))
+                    except:
+                        project_status = None
+                    try:
+                        project_stage = ProjectStage.objects.get(import_id=int(row.stage_id))
+                    except:
+                        project_stage = None
+                    try:
+                        project_date = make_aware(row.job_date)
+                    except:
+                        project_date = None
+
+                    company, created = Company.objects.update_or_create(name=settings.PROJECT_CENTER_DEFAULT_COMPANY_NAME)
+                    project, created = Project.objects.update_or_create(
+                        import_id=int(row.project_id),
+                    defaults={
+                        'title':row.project_title,
+                        'slug':'{slug}-{project_id}'.format(slug=slugify(row.project_title), project_id=row.project_id),
+                        'date':project_date,
+                        'code':row.project_code,
+                        'internal':row.is_internal,
+                        'category': project_category,
+                        'status': project_status,
+                        'stage': project_stage,
+                        'company':company
+                    })
+
+                    project.save()
+                    # first_rec = (project.history.first())
+                    # last_rec = (project.history.last())
+                    # first_rec.history_date = row.job_date
+                    # first_rec.history_change_reason = 'Project Created'
+                    # first_rec.history_type = '+'
+                    # first_rec.history_user_id = User.objects.get(import_id=row.user_id).id
+                    # first_rec.save()
+                    # last_rec.delete()
+                    print('Importing Project ' + project.title + '...')
+                    activities = self.import_project_activities(
+                        engine=engine,
+                        file=full_path('../../sql/list_project_activities.sql'),
+                        project=project,
+                        limit=None)
+                    assigned_users = self.import_project_assigned_users(engine=engine, project=project, limit=None)
+                    print('Project {title} import complete. Activities: {num_activities}. Users: {num_users}'.format(
+                        title=project.title,
+                        num_users=str(len(assigned_users)),
+                        num_activities=str(len(activities))))
+
+    def import_project_categories(self, engine, file):
+        with engine.connect() as conn:
+            with open(file) as file:
+                query = text(file.read())
+                result = conn.execute(query)
+                for row in result:
+                    category, created = ProjectCategory.objects.update_or_create(
+                        import_id=int(row.category_id),
+                    defaults={
+                        'name':row.category_name,
+                        'display':row.category_enabled,
+                    })
+
+    def import_project_status(self, engine, file):
+        with engine.connect() as conn:
+            with open(file) as file:
+                query = text(file.read())
+                result = conn.execute(query)
+                for row in result:
+                    status, created = ProjectStatus.objects.update_or_create(
+                        import_id=int(row.status_id),
+                    defaults={
+                        'name':row.status_name,
+                        'display': row.status_enabled,
+                    })
+
+
+    def import_project_stages(self, engine, file):
+        with engine.connect() as conn:
+            with open(file) as file:
+                query = text(file.read())
+                result = conn.execute(query)
+                for row in result:
+                    status, created = ProjectStage.objects.update_or_create(
+                        import_id=int(row.stage_id),
+                    defaults={
+                        'name':row.stage_name,
+                        'display':row.stage_enabled,
+                    })
+
+    def import_project_users(self, engine, file):
+        company, created = Company.objects.update_or_create(name=settings.PROJECT_CENTER_DEFAULT_COMPANY_NAME)
+        usergroup, created = Group.objects.get_or_create(name=settings.PROJECT_CENTER_USER_GROUP_NAME)
+        admin_usergroup, created = Group.objects.get_or_create(name=settings.PROJECT_CENTER_ADMINISTRATOR_GROUP_NAME)
+        company_admin_usergroup, created = Group.objects.get_or_create(
+            name=settings.PROJECT_CENTER_COMPANY_ADMINISTRATOR_GROUP_NAME
+        )
+
+        with engine.connect() as conn:
+            with open(file) as file:
+                query = text(file.read())
+                result = conn.execute(query)
+                for row in result:
+                    user, created = User.objects.update_or_create(
+                        import_id=int(row.user_id),
+                    defaults={
+                        'first_name':row.first_name,
+                        'last_name': row.last_name,
+                        'email': row.email,
+                        'username': row.email,
+                        'company':company,
+                        'title': row.title,
+                        'address_1': row.address_1
+                    })
+                    # if created or not user.companies:
+                    #     user.companies.add(company)
+                    #     user.save()
+                    if row.enabled == 1:
+                        user.is_staff = True
+                    else:
+                        user.is_staff = False
+                    if row.email_notify == 1:
+                        user.email_notify = True
+                    else:
+                        user.email_notify = False
+                    if created or user.groups.filter(name=settings.PROJECT_CENTER_USER_GROUP_NAME).exists() is False:
+                        user.set_password(row.password)
+                        user.groups.add(usergroup)
+                    user.save()
+
+
+    def import_project_assigned_users(self, engine, project, limit=None):
+        with engine.connect() as conn:
+            query = 'SELECT ' \
+                    'DISTINCT(ssm_commdep_projects_users.user_id), ' \
+                    'ss_users.last_name, ' \
+                    'ssm_commdep_projects_users.is_owner  ' \
+                    'FROM ' \
+                    'ssm_commdep_projects_users  ' \
+                    'LEFT JOIN ' \
+                    'ssm_commdep_projects ' \
+                    'ON  ssm_commdep_projects.id = ssm_commdep_projects_users.project_id ' \
+                    'LEFT JOIN ss_users ' \
+                    'ON ss_users.id = ssm_commdep_projects_users.user_id  ' \
+                    'WHERE ssm_commdep_projects_users.project_id = {project_id} ' \
+                    'GROUP BY ' \
+                    'ssm_commdep_projects_users.user_id, ' \
+                    'ss_users.last_name, ' \
+                    'ssm_commdep_projects_users.is_owner '.format(project_id=project.import_id)
+            result = conn.execute(text(query))
+            users = []
+            for row in result:
+                try:
+                    user = User.objects.get(
+                        import_id=int(row.user_id)
+                    )
+                    users.append(user)
+                    project.users.add(user)
+                except Exception as e:
+                    pass
+            project.save()
+            return users
+
+
+    def import_project_activities(self, engine, file, project=None, limit=None):
+        with engine.connect() as conn:
+            with open(file) as file:
+                query = 'SELECT * FROM `ssm_commdep_projects_activities` WHERE ' \
+                        'project_id = {project_id}'.format(project_id=project.import_id)
+
+                result = conn.execute(text(query))
+                activities = []
+                for row in result:
+                    try:
+                        project = Project.objects.get(import_id=int(row.project_id))
+                    except:
+                        project = None
+                    try:
+                        activity_date =  make_aware(row.activity_date)
+                    except:
+                        activity_date = None
+                    if row.file_name:
+                        url = 'http://uw.commdep.com/projects/uw/{project_id}/{activity_id}/{file_name}'.format(
+                            project_id=row.project_id,
+                            activity_id=row.activity_id,
+                            file_name=row.file_name,
+
+                        )
+
+                    else:
+                        url = None
+
+                    activity, created = ProjectActivity.objects.update_or_create(
+                        import_id=int(row.activity_id),
+                    defaults={
+                        'name':row.activity_name,
+                        'project':project,
+                        'date':activity_date,
+                        'user':User.objects.get(import_id=row.creator_id),
+                        'notes':row.notes,
+                    })
+                    activity._change_reason = activity.name
+                    activity.save()
+                    if url:
+                        r = requests.get(url)
+                        if r.status_code == 200:
+                            data = r.content
+                            filename = url.split('/')[-1]
+                            activity.file.save(filename, ContentFile(data))
+                            activity.save()
+                    activities.append(activity)
+                return activities
+
+
+    def handle(self, *args, **options):
+        engine = create_engine(settings.PROJECT_CENTER_IMPORT_DATABASE_URL)
+        limit = options['limit']
+        order = options['order']
+        reset = options['reset']
+        offset = options['offset']
+        tic = time.perf_counter()
+        print(f'Begin Import. Limit: {limit}. Offset: {offset}. Order: {order}. Reset: {reset}.'.format(
+            limit=limit,
+        offset=offset,
+        order=order,
+        reset=reset))
+        if reset:
+            projects = Project.objects.all().delete()
+            activities = ProjectActivity.objects.all().delete()
+            stages = ProjectStage.objects.all().delete()
+            statuses = ProjectStatus.objects.all().delete()
+            categories = ProjectCategory.objects.all().delete()
+            companies = Company.objects.all().delete()
+            groups = Group.objects.all().delete()
+            users = User.objects.filter(is_superuser=False).all().delete()
+        self.import_project_categories(engine, full_path('../../sql/list_project_categories.sql'))
+        self.import_project_status(engine, full_path('../../sql/list_project_statuses.sql'))
+        self.import_project_stages(engine, full_path('../../sql/list_project_stages.sql'))
+        self.import_project_users(engine, full_path('../../sql/list_project_users.sql'))
+        self.import_projects(engine, full_path('../../sql/list_projects.sql'), limit=limit, order=order, offset=offset)
+        # self.import_project_activities(engine, full_path('../../sql/list_project_activities.sql'), limit=limit)
+        toc = time.perf_counter()
+        print(toc - tic)
+        # if user:
+        #     user.delete()
+
+        # for x in (get_candidate_data_rest(candidate_id).keys()):
         #     print(x)
```

### Comparing `draper-utils-0.6/draper_utils/sql/list_project_users.sql` & `draper-utils-0.7/draper_utils/sql/list_project_users.sql`

 * *Files identical despite different names*

### Comparing `draper-utils-0.6/draper_utils/utils.py` & `draper-utils-0.7/draper_utils/utils.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-import time
-from genericpath import exists
-from os.path import abspath, join, dirname
-import requests
-
-from sqlalchemy import create_engine
-from sqlalchemy import text
-
-from django.contrib.auth import authenticate
-from django.core.management.base import BaseCommand
-from project_center.models import Project, ProjectCategory, ProjectStatus, ProjectStage, ProjectActivity, User, Company
-from django.conf import settings
-from django.core.files.base import ContentFile
-from django.utils.timezone import make_aware
-from django.template.defaultfilters import slugify
-from django.contrib.auth.models import Group
-
-
-def full_path(filename):
-    return abspath(join(dirname(__file__), filename))
-
-def import_project_categories(engine, file):
-    with engine.connect() as conn:
-        with open(file) as file:
-            query = text(file.read())
-            result = conn.execute(query)
-            for row in result:
-                category, created = ProjectCategory.objects.update_or_create(
-                    import_id=int(row.category_id),
-                defaults={
-                    'name':row.category_name
-                })
-
-def import_project_status(engine, file):
-    with engine.connect() as conn:
-        with open(file) as file:
-            query = text(file.read())
-            result = conn.execute(query)
-            for row in result:
-                status, created = ProjectStatus.objects.update_or_create(
-                    import_id=int(row.status_id),
-                defaults={
-                    'name':row.status_name
-                })
-
-
-def import_project_stages(engine, file):
-    with engine.connect() as conn:
-        with open(file) as file:
-            query = text(file.read())
-            result = conn.execute(query)
-            for row in result:
-                status, created = ProjectStage.objects.update_or_create(
-                    import_id=int(row.stage_id),
-                defaults={
-                    'name':row.stage_name
-                })
-
-def import_project_users(engine, file):
-    company, created = Company.objects.update_or_create(name='Veolia')
-    usergroup, created = Group.objects.get_or_create(name='Commdep User')
-    with engine.connect() as conn:
-        with open(file) as file:
-            query = text(file.read())
-            result = conn.execute(query)
-            for row in result:
-                user, created = User.objects.update_or_create(
-                    import_id=int(row.user_id),
-                defaults={
-                    'first_name':row.first_name,
-                    'last_name': row.last_name,
-                    'email': row.email,
-                    'username': row.email,
-                    'company':company
-                })
-                # if created or not user.companies:
-                #     user.companies.add(company)
-                #     user.save()
-                if created or user.groups.filter(name='Commdep User').exists() is False:
-                    user.set_password(row.password)
-
-                    user.groups.add(usergroup)
-                    user.save()
-
-def import_project_activities(engine, file, project=None, limit=None):
-        with engine.connect() as conn:
-            with open(file) as file:
-                query = 'SELECT * FROM `ssm_commdep_projects_activities` WHERE ' \
-                        'project_id = {project_id}'.format(project_id=project.import_id)
-
-                result = conn.execute(text(query))
-                for row in result:
-                    try:
-                        project = Project.objects.get(import_id=int(row.project_id))
-                    except:
-                        project = None
-                    try:
-                        activity_date =  make_aware(row.activity_date)
-                    except:
-                        activity_date = None
-                    if row.file_name:
-                        url = 'http://uw.commdep.com/projects/uw/{project_id}/{activity_id}/{file_name}'.format(
-                            project_id=row.project_id,
-                            activity_id=row.activity_id,
-                            file_name=row.file_name,
-
-                        )
-
-                    else:
-                        url = None
-
-                    print(url)
-                    activity, created = ProjectActivity.objects.update_or_create(
-                        import_id=int(row.activity_id),
-                    defaults={
-                        'name':row.activity_name,
-                        'project':project,
-                        'date':activity_date,
-                        'user':User.objects.get(import_id=row.creator_id),
-                    })
-                    activity._change_reason = activity.name
-                    activity.save()
-                    if url:
-                        r = requests.get(url)
-                        if r.status_code == 200:
-                            data = r.content
-                            filename = url.split('/')[-1]
-                            activity.file.save(filename, ContentFile(data))
-                            activity.save()
-
-def import_projects(engine, file, limit=None, order=None):
-    with engine.connect() as conn:
-        with open(file) as file:
-            query = file.read()
-            if order:
-                query = str(query).strip()
-                query += ' ORDER BY ' + order
-            if limit:
-                query = str(query).strip()
-                query += ' LIMIT ' + limit
-            result = conn.execute(text(query))
-            for row in result:
-                try:
-                    project_category = ProjectCategory.objects.get(import_id=int(row.category_id))
-                except:
-                    project_category = None
-                try:
-                    project_status = ProjectStatus.objects.get(import_id=int(row.status_id))
-                except:
-                    project_status = None
-                try:
-                    project_stage = ProjectStage.objects.get(import_id=int(row.stage_id))
-                except:
-                    project_stage = None
-
-                company, created = Company.objects.update_or_create(name='Veolia')
-                project, created = Project.objects.update_or_create(
-                    import_id=int(row.project_id),
-                    defaults={
-                        'title': row.project_title,
-                        'slug': '{slug}-{project_id}'.format(slug=slugify(row.project_title),
-                                                             project_id=row.project_id),
-                        'code': row.project_code,
-                        'internal': row.is_internal,
-                        'category': project_category,
-                        'status': project_status,
-                        'stage': project_stage,
-                        'company': company
-                    })
-
-                project.save()
-
-                import_project_activities(
-                    engine=engine,
-                    file=full_path('list_project_activities.sql'),
-                    project=project,
+import time
+from genericpath import exists
+from os.path import abspath, join, dirname
+import requests
+
+from sqlalchemy import create_engine
+from sqlalchemy import text
+
+from django.contrib.auth import authenticate
+from django.core.management.base import BaseCommand
+from project_center.models import Project, ProjectCategory, ProjectStatus, ProjectStage, ProjectActivity, User, Company
+from django.conf import settings
+from django.core.files.base import ContentFile
+from django.utils.timezone import make_aware
+from django.template.defaultfilters import slugify
+from django.contrib.auth.models import Group
+
+
+def full_path(filename):
+    return abspath(join(dirname(__file__), filename))
+
+def import_project_categories(engine, file):
+    with engine.connect() as conn:
+        with open(file) as file:
+            query = text(file.read())
+            result = conn.execute(query)
+            for row in result:
+                category, created = ProjectCategory.objects.update_or_create(
+                    import_id=int(row.category_id),
+                defaults={
+                    'name':row.category_name
+                })
+
+def import_project_status(engine, file):
+    with engine.connect() as conn:
+        with open(file) as file:
+            query = text(file.read())
+            result = conn.execute(query)
+            for row in result:
+                status, created = ProjectStatus.objects.update_or_create(
+                    import_id=int(row.status_id),
+                defaults={
+                    'name':row.status_name
+                })
+
+
+def import_project_stages(engine, file):
+    with engine.connect() as conn:
+        with open(file) as file:
+            query = text(file.read())
+            result = conn.execute(query)
+            for row in result:
+                status, created = ProjectStage.objects.update_or_create(
+                    import_id=int(row.stage_id),
+                defaults={
+                    'name':row.stage_name
+                })
+
+def import_project_users(engine, file):
+    company, created = Company.objects.update_or_create(name='Veolia')
+    usergroup, created = Group.objects.get_or_create(name='Commdep User')
+    with engine.connect() as conn:
+        with open(file) as file:
+            query = text(file.read())
+            result = conn.execute(query)
+            for row in result:
+                user, created = User.objects.update_or_create(
+                    import_id=int(row.user_id),
+                defaults={
+                    'first_name':row.first_name,
+                    'last_name': row.last_name,
+                    'email': row.email,
+                    'username': row.email,
+                    'company':company
+                })
+                # if created or not user.companies:
+                #     user.companies.add(company)
+                #     user.save()
+                if created or user.groups.filter(name='Commdep User').exists() is False:
+                    user.set_password(row.password)
+
+                    user.groups.add(usergroup)
+                    user.save()
+
+def import_project_activities(engine, file, project=None, limit=None):
+        with engine.connect() as conn:
+            with open(file) as file:
+                query = 'SELECT * FROM `ssm_commdep_projects_activities` WHERE ' \
+                        'project_id = {project_id}'.format(project_id=project.import_id)
+
+                result = conn.execute(text(query))
+                for row in result:
+                    try:
+                        project = Project.objects.get(import_id=int(row.project_id))
+                    except:
+                        project = None
+                    try:
+                        activity_date =  make_aware(row.activity_date)
+                    except:
+                        activity_date = None
+                    if row.file_name:
+                        url = 'http://uw.commdep.com/projects/uw/{project_id}/{activity_id}/{file_name}'.format(
+                            project_id=row.project_id,
+                            activity_id=row.activity_id,
+                            file_name=row.file_name,
+
+                        )
+
+                    else:
+                        url = None
+
+                    print(url)
+                    activity, created = ProjectActivity.objects.update_or_create(
+                        import_id=int(row.activity_id),
+                    defaults={
+                        'name':row.activity_name,
+                        'project':project,
+                        'date':activity_date,
+                        'user':User.objects.get(import_id=row.creator_id),
+                    })
+                    activity._change_reason = activity.name
+                    activity.save()
+                    if url:
+                        r = requests.get(url)
+                        if r.status_code == 200:
+                            data = r.content
+                            filename = url.split('/')[-1]
+                            activity.file.save(filename, ContentFile(data))
+                            activity.save()
+
+def import_projects(engine, file, limit=None, order=None):
+    with engine.connect() as conn:
+        with open(file) as file:
+            query = file.read()
+            if order:
+                query = str(query).strip()
+                query += ' ORDER BY ' + order
+            if limit:
+                query = str(query).strip()
+                query += ' LIMIT ' + limit
+            result = conn.execute(text(query))
+            for row in result:
+                try:
+                    project_category = ProjectCategory.objects.get(import_id=int(row.category_id))
+                except:
+                    project_category = None
+                try:
+                    project_status = ProjectStatus.objects.get(import_id=int(row.status_id))
+                except:
+                    project_status = None
+                try:
+                    project_stage = ProjectStage.objects.get(import_id=int(row.stage_id))
+                except:
+                    project_stage = None
+
+                company, created = Company.objects.update_or_create(name='Veolia')
+                project, created = Project.objects.update_or_create(
+                    import_id=int(row.project_id),
+                    defaults={
+                        'title': row.project_title,
+                        'slug': '{slug}-{project_id}'.format(slug=slugify(row.project_title),
+                                                             project_id=row.project_id),
+                        'code': row.project_code,
+                        'internal': row.is_internal,
+                        'category': project_category,
+                        'status': project_status,
+                        'stage': project_stage,
+                        'company': company
+                    })
+
+                project.save()
+
+                import_project_activities(
+                    engine=engine,
+                    file=full_path('list_project_activities.sql'),
+                    project=project,
                     limit=None)
```

### Comparing `draper-utils-0.6/draper_utils.egg-info/SOURCES.txt` & `draper-utils-0.7/draper_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

