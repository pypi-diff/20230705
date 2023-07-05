# Comparing `tmp/aleksis_core-3.1.1.tar.gz` & `tmp/aleksis_core-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_core-3.1.1.tar", max compression
+gzip compressed data, was "aleksis_core-3.1.2.tar", max compression
```

## Comparing `aleksis_core-3.1.1.tar` & `aleksis_core-3.1.2.tar`

### file list

```diff
@@ -1,490 +1,490 @@
--rw-r--r--   0        0        0    37422 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/CHANGELOG.rst
--rw-r--r--   0        0        0    14353 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/LICENCE.rst
--rw-r--r--   0        0        0     3786 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/README.rst
--rw-r--r--   0        0        0      194 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/aleksis/core/__init__.py
--rw-r--r--   0        0        0      464 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/aleksis/core/__main__.py
--rw-r--r--   0        0        0      510 2023-07-02 00:08:43.991237 aleksis_core-3.1.1/aleksis/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2023-07-02 00:08:45.299286 aleksis_core-3.1.1/aleksis/core/__pycache__/__main__.cpython-311.pyc
--rw-r--r--   0        0        0     2061 2023-07-02 00:08:49.007426 aleksis_core-3.1.1/aleksis/core/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0    11380 2023-07-02 00:08:46.695339 aleksis_core-3.1.1/aleksis/core/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     2533 2023-07-02 00:08:44.035239 aleksis_core-3.1.1/aleksis/core/__pycache__/celery.cpython-311.pyc
--rw-r--r--   0        0        0     3716 2023-07-02 00:08:49.135430 aleksis_core-3.1.1/aleksis/core/__pycache__/checks.cpython-311.pyc
--rw-r--r--   0        0        0    17897 2023-07-02 00:08:48.555409 aleksis_core-3.1.1/aleksis/core/__pycache__/data_checks.cpython-311.pyc
--rw-r--r--   0        0        0     5154 2023-07-02 00:08:49.147431 aleksis_core-3.1.1/aleksis/core/__pycache__/health_checks.cpython-311.pyc
--rw-r--r--   0        0        0     8423 2023-07-02 00:08:48.595410 aleksis_core-3.1.1/aleksis/core/__pycache__/managers.cpython-311.pyc
--rw-r--r--   0        0        0    30729 2023-07-02 00:08:48.559409 aleksis_core-3.1.1/aleksis/core/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0        0        0    85606 2023-07-02 00:08:47.999388 aleksis_core-3.1.1/aleksis/core/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0    22237 2023-07-02 00:08:49.227434 aleksis_core-3.1.1/aleksis/core/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1370 2023-07-02 00:08:46.723340 aleksis_core-3.1.1/aleksis/core/__pycache__/registries.cpython-311.pyc
--rw-r--r--   0        0        0    16523 2023-07-02 00:08:49.047427 aleksis_core-3.1.1/aleksis/core/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0    43565 2023-07-02 00:08:45.323287 aleksis_core-3.1.1/aleksis/core/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     3825 2023-07-02 00:08:48.607411 aleksis_core-3.1.1/aleksis/core/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0        0        0      950 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/aleksis/core/admin.py
--rw-r--r--   0        0        0     8519 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/aleksis/core/apps.py
--rw-r--r--   0        0        0     1338 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/aleksis/core/celery.py
--rw-r--r--   0        0        0     2751 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/aleksis/core/checks.py
--rw-r--r--   0        0        0    11534 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/aleksis/core/data_checks.py
--rw-r--r--   0        0        0      741 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/aleksis/core/decorators.py
--rw-r--r--   0        0        0     5556 2023-07-02 00:07:11.875772 aleksis_core-3.1.1/aleksis/core/filters.py
--rw-r--r--   0        0        0    31619 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/forms.py
--rw-r--r--   0        0        0     3175 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/app/apollo.js
--rw-r--r--   0        0        0     1089 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/app/dateTimeFormats.js
--rw-r--r--   0        0        0      197 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/app/i18n.js
--rw-r--r--   0        0        0      157 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/app/router.js
--rw-r--r--   0        0        0      133 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/app/sentry.js
--rw-r--r--   0        0        0      793 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/app/vuetify.js
--rw-r--r--   0        0        0     3679 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/LegacyBaseTemplate.vue
--rw-r--r--   0        0        0      158 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/Parent.vue
--rw-r--r--   0        0        0      335 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/about/About.vue
--rw-r--r--   0        0        0     1971 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/about/AboutAleksis.vue
--rw-r--r--   0        0        0     3831 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/about/InstalledAppCard.vue
--rw-r--r--   0        0        0     1003 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/about/InstalledAppsList.vue
--rw-r--r--   0        0        0      351 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/about/installedApps.graphql
--rw-r--r--   0        0        0     2411 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/AccountMenu.vue
--rw-r--r--   0        0        0     9590 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/App.vue
--rw-r--r--   0        0        0      314 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/BrandLogo.vue
--rw-r--r--   0        0        0     1064 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/ErrorPage.vue
--rw-r--r--   0        0        0     1470 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/LanguageForm.vue
--rw-r--r--   0        0        0     3778 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/SideNav.vue
--rw-r--r--   0        0        0     1454 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/SidenavSearch.vue
--rw-r--r--   0        0        0      747 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/SnackbarItem.vue
--rw-r--r--   0        0        0     1932 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/Splash.vue
--rw-r--r--   0        0        0      124 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/customMenu.graphql
--rw-r--r--   0        0        0      205 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/dynamicRoutes.graphql
--rw-r--r--   0        0        0       42 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/messages.graphql
--rw-r--r--   0        0        0       59 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/ping.graphql
--rw-r--r--   0        0        0      139 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/searchSnippets.graphql
--rw-r--r--   0        0        0      412 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/systemProperties.graphql
--rw-r--r--   0        0        0      322 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/app/whoAmI.graphql
--rw-r--r--   0        0        0     2558 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
--rw-r--r--   0        0        0     1884 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
--rw-r--r--   0        0        0      220 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
--rw-r--r--   0        0        0       65 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
--rw-r--r--   0        0        0     3482 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
--rw-r--r--   0        0        0     1910 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
--rw-r--r--   0        0        0      925 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
--rw-r--r--   0        0        0      432 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
--rw-r--r--   0        0        0      191 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
--rw-r--r--   0        0        0      118 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
--rw-r--r--   0        0        0      655 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/generic/AvatarClickbox.vue
--rw-r--r--   0        0        0      212 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/generic/BackButton.vue
--rw-r--r--   0        0        0      598 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/generic/ButtonMenu.vue
--rw-r--r--   0        0        0      981 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/generic/DetailView.vue
--rw-r--r--   0        0        0      408 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/generic/ListView.vue
--rw-r--r--   0        0        0      268 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/generic/MessageBox.vue
--rw-r--r--   0        0        0     1914 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/generic/ObjectOverview.vue
--rw-r--r--   0        0        0      269 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/generic/SmallContainer.vue
--rw-r--r--   0        0        0     2017 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/generic/UpdateIndicator.vue
--rw-r--r--   0        0        0     3232 2023-07-02 00:07:11.879773 aleksis_core-3.1.1/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
--rw-r--r--   0        0        0      706 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/group/GroupCollection.vue
--rw-r--r--   0        0        0     3034 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/notifications/NotificationItem.vue
--rw-r--r--   0        0        0     2530 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/notifications/NotificationList.vue
--rw-r--r--   0        0        0      107 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
--rw-r--r--   0        0        0      200 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/notifications/myNotifications.graphql
--rw-r--r--   0        0        0     1017 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/pdf/DownloadPDF.vue
--rw-r--r--   0        0        0       78 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/pdf/pdf.graphql
--rw-r--r--   0        0        0     1410 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/person/AdditionalImage.vue
--rw-r--r--   0        0        0     1082 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/person/AvatarContent.vue
--rw-r--r--   0        0        0     2892 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/person/PersonActions.vue
--rw-r--r--   0        0        0      527 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
--rw-r--r--   0        0        0      759 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/person/PersonCollection.vue
--rw-r--r--   0        0        0     7423 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/person/PersonOverview.vue
--rw-r--r--   0        0        0      108 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/person/avatarContent.graphql
--rw-r--r--   0        0        0      196 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/person/personActions.graphql
--rw-r--r--   0        0        0      575 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/person/personOverview.graphql
--rw-r--r--   0        0        0     3858 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/two_factor/TwoFactor.vue
--rw-r--r--   0        0        0     1512 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
--rw-r--r--   0        0        0      589 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
--rw-r--r--   0        0        0      385 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/components/two_factor/twoFactor.graphql
--rw-r--r--   0        0        0      390 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/css/global.scss
--rw-r--r--   0        0        0     2561 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/index.js
--rw-r--r--   0        0        0    10763 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/messages/de.json
--rw-r--r--   0        0        0     9741 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/messages/en.json
--rw-r--r--   0        0        0    12252 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/messages/ru.json
--rw-r--r--   0        0        0    14534 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/messages/uk.json
--rw-r--r--   0        0        0     1211 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/mixins/aleksis.js
--rw-r--r--   0        0        0      538 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/mixins/error404.js
--rw-r--r--   0        0        0     3441 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/mixins/menus.js
--rw-r--r--   0        0        0     2256 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/mixins/offline.js
--rw-r--r--   0        0        0      736 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/mixins/permissions.js
--rw-r--r--   0        0        0     2154 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/mixins/routes.js
--rw-r--r--   0        0        0     1619 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/mixins/useRegisterSW.js
--rw-r--r--   0        0        0     6380 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/plugins/aleksis.js
--rw-r--r--   0        0        0      450 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/routeValidators.js
--rw-r--r--   0        0        0    36573 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/frontend/routes.js
--rw-r--r--   0        0        0     2642 2023-07-02 00:07:11.883773 aleksis_core-3.1.1/aleksis/core/health_checks.py
--rw-r--r--   0        0        0      487 2023-07-02 00:08:49.587447 aleksis_core-3.1.1/aleksis/core/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74307 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      463 2023-07-02 00:08:49.579447 aleksis_core-3.1.1/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      894 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    63806 2023-07-02 00:08:49.707452 aleksis_core-3.1.1/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   126085 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      567 2023-07-02 00:08:49.683451 aleksis_core-3.1.1/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1118 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      942 2023-07-02 00:08:49.707452 aleksis_core-3.1.1/aleksis/core/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    77782 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-07-02 00:08:49.691451 aleksis_core-3.1.1/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      810 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     2584 2023-07-02 00:08:49.711452 aleksis_core-3.1.1/aleksis/core/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    82875 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-02 00:08:49.695451 aleksis_core-3.1.1/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2023-07-02 00:08:49.587447 aleksis_core-3.1.1/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74237 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-02 00:08:49.571447 aleksis_core-3.1.1/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    80303 2023-07-02 00:08:49.723452 aleksis_core-3.1.1/aleksis/core/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   144575 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2023-07-02 00:08:49.699452 aleksis_core-3.1.1/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1321 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2023-07-02 00:08:49.723452 aleksis_core-3.1.1/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74177 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-07-02 00:08:49.715452 aleksis_core-3.1.1/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    77610 2023-07-02 00:08:49.603448 aleksis_core-3.1.1/aleksis/core/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   131787 2023-07-02 00:07:11.887773 aleksis_core-3.1.1/aleksis/core/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2023-07-02 00:08:49.679451 aleksis_core-3.1.1/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1331 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/management/__init__.py
--rw-r--r--   0        0        0     3957 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/management/commands/convert_urls_to_routes.py
--rw-r--r--   0        0        0      945 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/management/commands/vite.py
--rw-r--r--   0        0        0      439 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/management/commands/webpack_bundle.py
--rw-r--r--   0        0        0     4690 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/managers.py
--rw-r--r--   0        0        0    51004 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0001_initial.py
--rw-r--r--   0        0        0     2473 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0002_school_term.py
--rw-r--r--   0        0        0      531 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0003_drop_image_cropping.py
--rw-r--r--   0        0        0      796 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
--rw-r--r--   0        0        0     1252 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0005_timestamped_activity_notification.py
--rw-r--r--   0        0        0     1567 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0006_dashboard_widget_size.py
--rw-r--r--   0        0        0     1396 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0007_dashboard_widget_order.py
--rw-r--r--   0        0        0     2311 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0008_data_check_result.py
--rw-r--r--   0        0        0     1052 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0009_default_dashboard.py
--rw-r--r--   0        0        0      952 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0010_external_link_widget.py
--rw-r--r--   0        0        0      829 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0011_globalpermissions_options.py
--rw-r--r--   0        0        0      501 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0012_valid_from_announcement.py
--rw-r--r--   0        0        0     2270 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0013_pdf_file.py
--rw-r--r--   0        0        0      533 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0014_alter_pdffile_file.py
--rw-r--r--   0        0        0     1174 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0015_oauth_permissions.py
--rw-r--r--   0        0        0     1538 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0016_taskuserassignment.py
--rw-r--r--   0        0        0      426 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0017_dashboardwidget_broken.py
--rw-r--r--   0        0        0      897 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0018_pdffile_html_file.py
--rw-r--r--   0        0        0     2177 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
--rw-r--r--   0        0        0      542 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0020_pdf_file_person_optional.py
--rw-r--r--   0        0        0     1084 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
--rw-r--r--   0        0        0      923 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0022_public_favicon.py
--rw-r--r--   0        0        0     6340 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0023_oauth_application_model.py
--rw-r--r--   0        0        0      714 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0024_oauth_grant_types_optional.py
--rw-r--r--   0        0        0     1717 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0025_oauth_align_user_fk.py
--rw-r--r--   0        0        0      582 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
--rw-r--r--   0        0        0      457 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0027_person_place_of_birth.py
--rw-r--r--   0        0        0      947 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0028_char_field_not_null.py
--rw-r--r--   0        0        0     1465 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0029_invitations.py
--rw-r--r--   0        0        0     1776 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0030_user_attributes.py
--rw-r--r--   0        0        0      526 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0031_oauthapplication_icon.py
--rw-r--r--   0        0        0      340 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0032_remove_person_is_active.py
--rw-r--r--   0        0        0     2416 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0033_update_photo_avatar.py
--rw-r--r--   0        0        0      816 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0034_invite_permission.py
--rw-r--r--   0        0        0     1781 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0035_preference_model_unique.py
--rw-r--r--   0        0        0      626 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0036_additionalfields_helptext_required.py
--rw-r--r--   0        0        0      917 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0037_add_static_content_widget.py
--rw-r--r--   0        0        0      522 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0038_notification_send_at.py
--rw-r--r--   0        0        0     1029 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0039_personal_ical_url.py
--rw-r--r--   0        0        0      613 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
--rw-r--r--   0        0        0      516 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0041_update_gender_choices.py
--rw-r--r--   0        0        0      547 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0042_pdffile_empty.py
--rw-r--r--   0        0        0     2261 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0043_task_assignment_meta.py
--rw-r--r--   0        0        0      532 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0044_task_assignment_result_fetched.py
--rw-r--r--   0        0        0      486 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
--rw-r--r--   0        0        0   290966 2023-07-02 00:07:11.891773 aleksis_core-3.1.1/aleksis/core/migrations/0046_notification_create_field_icon.py
--rw-r--r--   0        0        0     2717 2023-07-02 00:07:11.895773 aleksis_core-3.1.1/aleksis/core/migrations/0047_add_room_model.py
--rw-r--r--   0        0        0   893996 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/migrations/0048_delete_personalicalurl.py
--rw-r--r--   0        0        0      580 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
--rw-r--r--   0        0        0        0 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/migrations/__init__.py
--rw-r--r--   0        0        0    19163 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/mixins.py
--rw-r--r--   0        0        0    51781 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/models.py
--rw-r--r--   0        0        0    13478 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/preferences.py
--rw-r--r--   0        0        0      692 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/registries.py
--rw-r--r--   0        0        0    16018 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/rules.py
--rw-r--r--   0        0        0     7486 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/__init__.py
--rw-r--r--   0        0        0     1301 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/base.py
--rw-r--r--   0        0        0     3049 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/celery_progress.py
--rw-r--r--   0        0        0      585 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/custom_menu.py
--rw-r--r--   0        0        0      459 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/dynamic_routes.py
--rw-r--r--   0        0        0     2046 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/group.py
--rw-r--r--   0        0        0     1743 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/installed_apps.py
--rw-r--r--   0        0        0      265 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/message.py
--rw-r--r--   0        0        0     1296 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/notification.py
--rw-r--r--   0        0        0     1179 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/oauth.py
--rw-r--r--   0        0        0      535 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/pdf.py
--rw-r--r--   0        0        0      124 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/permissions.py
--rw-r--r--   0        0        0     9708 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/person.py
--rw-r--r--   0        0        0      191 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/room.py
--rw-r--r--   0        0        0      163 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/school_term.py
--rw-r--r--   0        0        0      868 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/search.py
--rw-r--r--   0        0        0     1343 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/site_preferences.py
--rw-r--r--   0        0        0     1651 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/system_properties.py
--rw-r--r--   0        0        0     3297 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/two_factor.py
--rw-r--r--   0        0        0      829 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/schema/user.py
--rw-r--r--   0        0        0      418 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/search_indexes.py
--rw-r--r--   0        0        0    39500 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/settings.py
--rw-r--r--   0        0        0    49621 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/static/img/aleksis-banner.svg
--rw-r--r--   0        0        0     1862 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/static/img/aleksis-favicon.png
--rw-r--r--   0        0        0    17172 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/static/img/aleksis-icon-maskable.png
--rw-r--r--   0        0        0     7843 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/static/img/aleksis-icon-maskable.svg
--rw-r--r--   0        0        0    31902 2023-07-02 00:07:11.899773 aleksis_core-3.1.1/aleksis/core/static/img/aleksis-icon.png
--rw-r--r--   0        0        0     7346 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/img/aleksis-icon.svg
--rw-r--r--   0        0        0    19126 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/img/fallback.png
--rw-r--r--   0        0        0     2237 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/img/hero.svg
--rw-r--r--   0        0        0      490 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/js/copy_button.js
--rw-r--r--   0        0        0      521 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/js/edit_dashboard.js
--rw-r--r--   0        0        0      618 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/js/helper.js
--rw-r--r--   0        0        0      984 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/js/include_ajax_live.js
--rw-r--r--   0        0        0     4350 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/js/main.js
--rw-r--r--   0        0        0     1654 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/js/multi_select.js
--rw-r--r--   0        0        0     3495 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/js/search.js
--rw-r--r--   0        0        0     2578 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/js/serviceworker.js
--rw-r--r--   0        0        0      271 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/print-simple.css
--rw-r--r--   0        0        0     1627 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/print.css
--rw-r--r--   0        0        0      187 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/print_landscape.css
--rw-r--r--   0        0        0     1064 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/public/materialize-custom.scss
--rw-r--r--   0        0        0    15745 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/public/style.scss
--rw-r--r--   0        0        0    11345 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/static/public/theme.scss
--rw-r--r--   0        0        0     6876 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/tables.py
--rw-r--r--   0        0        0     2330 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/tasks.py
--rw-r--r--   0        0        0      838 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/403.html
--rw-r--r--   0        0        0      789 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/404.html
--rw-r--r--   0        0        0      918 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/500.html
--rw-r--r--   0        0        0       76 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/503.html
--rw-r--r--   0        0        0      851 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/account_inactive.html
--rw-r--r--   0        0        0      169 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/email/base_message.txt
--rw-r--r--   0        0        0      525 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0        0        0     1255 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/email_confirm.html
--rw-r--r--   0        0        0      804 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/password_change.html
--rw-r--r--   0        0        0      888 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/password_change_disabled.html
--rw-r--r--   0        0        0     1376 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/password_reset.html
--rw-r--r--   0        0        0      825 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     2305 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      649 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      500 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/password_set.html
--rw-r--r--   0        0        0      888 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/signup.html
--rw-r--r--   0        0        0      838 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/signup_closed.html
--rw-r--r--   0        0        0      820 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/verification_email_required.html
--rw-r--r--   0        0        0     1160 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/account/verification_sent.html
--rw-r--r--   0        0        0      979 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/components/chips.html
--rw-r--r--   0        0        0      350 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/components/materialize-chips.html
--rw-r--r--   0        0        0      225 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/components/msgbox.html
--rw-r--r--   0        0        0      958 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/components/pagination.html
--rw-r--r--   0        0        0      486 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/components/text_collapsible.html
--rw-r--r--   0        0        0      483 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/core/additional_field/edit.html
--rw-r--r--   0        0        0      594 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/core/additional_field/list.html
--rw-r--r--   0        0        0     1053 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/core/announcement/form.html
--rw-r--r--   0        0        0     1900 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/core/announcement/list.html
--rw-r--r--   0        0        0     3099 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/core/base.html
--rw-r--r--   0        0        0     2454 2023-07-02 00:07:11.903773 aleksis_core-3.1.1/aleksis/core/templates/core/base_print.html
--rw-r--r--   0        0        0     1178 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/base_simple_print.html
--rw-r--r--   0        0        0      628 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/dashboard_widget/create.html
--rw-r--r--   0        0        0      635 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
--rw-r--r--   0        0        0      626 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/dashboard_widget/edit.html
--rw-r--r--   0        0        0      262 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
--rw-r--r--   0        0        0     1349 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/dashboard_widget/list.html
--rw-r--r--   0        0        0      226 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
--rw-r--r--   0        0        0     3879 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/data_check/list.html
--rw-r--r--   0        0        0     2233 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/edit_dashboard.html
--rw-r--r--   0        0        0        0 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/empty.html
--rw-r--r--   0        0        0     5310 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/group/child_groups.html
--rw-r--r--   0        0        0      650 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/group/edit.html
--rw-r--r--   0        0        0     3382 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/group/full.html
--rw-r--r--   0        0        0     1019 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/group/list.html
--rw-r--r--   0        0        0      465 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/group_type/edit.html
--rw-r--r--   0        0        0      564 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/group_type/list.html
--rw-r--r--   0        0        0     2504 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/index.html
--rw-r--r--   0        0        0      777 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/pages/delete.html
--rw-r--r--   0        0        0     6832 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/pages/system_status.html
--rw-r--r--   0        0        0      603 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/pages/test_pdf.html
--rw-r--r--   0        0        0       93 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/address.html
--rw-r--r--   0        0        0      189 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/admins_list.html
--rw-r--r--   0        0        0     1632 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/announcements.html
--rw-r--r--   0        0        0     1472 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/avatar_content.html
--rw-r--r--   0        0        0      319 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/copy_button.html
--rw-r--r--   0        0        0     1089 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/crud_events.html
--rw-r--r--   0        0        0      389 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/edit_dashboard_widget.html
--rw-r--r--   0        0        0     1624 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/meta.html
--rw-r--r--   0        0        0      414 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/on_page_menu.html
--rw-r--r--   0        0        0      260 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/save_button.html
--rw-r--r--   0        0        0     2374 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/splash_screen.html
--rw-r--r--   0        0        0      325 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/partials/turnable.html
--rw-r--r--   0        0        0      915 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/perms/assign.html
--rw-r--r--   0        0        0     2478 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/perms/list.html
--rw-r--r--   0        0        0      376 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/person/collection.html
--rw-r--r--   0        0        0      649 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/person/create.html
--rw-r--r--   0        0        0      645 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/person/edit.html
--rw-r--r--   0        0        0     1165 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/person/list.html
--rw-r--r--   0        0        0      455 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/school_term/create.html
--rw-r--r--   0        0        0      451 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/school_term/edit.html
--rw-r--r--   0        0        0      556 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/school_term/list.html
--rw-r--r--   0        0        0      935 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/core/vue_index.html
--rw-r--r--   0        0        0     3921 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/django_tables2/materialize.html
--rw-r--r--   0        0        0      981 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/dynamic_preferences/form.html
--rw-r--r--   0        0        0      376 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/dynamic_preferences/sections.html
--rw-r--r--   0        0        0      764 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/invitations/disabled.html
--rw-r--r--   0        0        0     1281 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/invitations/enter.html
--rw-r--r--   0        0        0     1162 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/invitations/forms/_invite.html
--rw-r--r--   0        0        0      102 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/invitations/messages/invite_accepted.txt
--rw-r--r--   0        0        0      171 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/material/field_errors.html
--rw-r--r--   0        0        0     1232 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
--rw-r--r--   0        0        0     1897 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/material/fields/colorfield_colorwidget.html
--rw-r--r--   0        0        0     1009 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
--rw-r--r--   0        0        0     1009 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/material/fields/django_select2_select2widget.html
--rw-r--r--   0        0        0      253 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/material/non_field_errors.html
--rw-r--r--   0        0        0      663 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/oauth2_provider/application/create.html
--rw-r--r--   0        0        0     2335 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/oauth2_provider/application/detail.html
--rw-r--r--   0        0        0      669 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/oauth2_provider/application/edit.html
--rw-r--r--   0        0        0     1074 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/oauth2_provider/application/list.html
--rw-r--r--   0        0        0     2686 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/oauth2_provider/authorize.html
--rw-r--r--   0        0        0      887 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/offline.html
--rw-r--r--   0        0        0       42 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/search/indexes/core/group_text.txt
--rw-r--r--   0        0        0       69 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/search/indexes/core/person_text.txt
--rw-r--r--   0        0        0       42 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/search/indexes/core/room_text.txt
--rw-r--r--   0        0        0     3171 2023-07-02 00:07:11.907774 aleksis_core-3.1.1/aleksis/core/templates/search/search.html
--rw-r--r--   0        0        0      243 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/search/searchbar_snippet.html
--rw-r--r--   0        0        0      150 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/search/searchbar_snippets.html
--rw-r--r--   0        0        0      169 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/sms/notification.txt
--rw-r--r--   0        0        0      893 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0     1268 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1289 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/socialaccount/login.html
--rw-r--r--   0        0        0      809 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/socialaccount/login_cancelled.html
--rw-r--r--   0        0        0     1012 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/socialaccount/signup.html
--rw-r--r--   0        0        0     1434 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      630 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/templated_email/base.email
--rw-r--r--   0        0        0     1527 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/templated_email/celery_failure.email
--rw-r--r--   0        0        0      994 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/templated_email/data_checks.email
--rw-r--r--   0        0        0      990 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/templated_email/email.css
--rw-r--r--   0        0        0     1102 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/templated_email/invitation.email
--rw-r--r--   0        0        0     1461 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/templated_email/notification.email
--rw-r--r--   0        0        0      668 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/templated_email/person_changed.email
--rw-r--r--   0        0        0      219 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/two_factor/_base_focus.html
--rw-r--r--   0        0        0      877 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/two_factor/_wizard_actions.html
--rw-r--r--   0        0        0      119 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/two_factor/_wizard_forms.html
--rw-r--r--   0        0        0     1780 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0        0        0     6712 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/login.html
--rw-r--r--   0        0        0      943 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/otp_required.html
--rw-r--r--   0        0        0      986 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/phone_register.html
--rw-r--r--   0        0        0     3312 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/setup.html
--rw-r--r--   0        0        0     2127 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/setup_complete.html
--rw-r--r--   0        0        0      786 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templates/two_factor/profile/disable.html
--rw-r--r--   0        0        0        0 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templatetags/__init__.py
--rw-r--r--   0        0        0       99 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templatetags/apps.py
--rw-r--r--   0        0        0      394 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templatetags/dashboard.py
--rw-r--r--   0        0        0     1618 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templatetags/data_helpers.py
--rw-r--r--   0        0        0     1523 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templatetags/html_helpers.py
--rw-r--r--   0        0        0      206 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/templatetags/msg_box.py
--rw-r--r--   0        0        0     3696 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/browser/test_selenium.py
--rw-r--r--   0        0        0     6596 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/models/test.pdf
--rw-r--r--   0        0        0     6562 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/models/test_group.py
--rw-r--r--   0        0        0     1520 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/models/test_group_sync.py
--rw-r--r--   0        0        0     3049 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/models/test_notification.py
--rw-r--r--   0        0        0     4003 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/models/test_pdffile.py
--rw-r--r--   0        0        0      427 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/models/test_person.py
--rw-r--r--   0        0        0     5503 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/regression/test_regression.py
--rw-r--r--   0        0        0      683 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/regression/view_oauth.py
--rw-r--r--   0        0        0     1021 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/templatetags/test_data_helpers.py
--rw-r--r--   0        0        0     2292 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/tests/views/test_account.py
--rw-r--r--   0        0        0    18734 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/urls.py
--rw-r--r--   0        0        0        0 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/util/__init__.py
--rw-r--r--   0        0        0      176 2023-07-02 00:08:44.515257 aleksis_core-3.1.1/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    13595 2023-07-02 00:08:46.723340 aleksis_core-3.1.1/aleksis/core/util/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    10101 2023-07-02 00:08:48.607411 aleksis_core-3.1.1/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
--rw-r--r--   0        0        0    24932 2023-07-02 00:08:44.519257 aleksis_core-3.1.1/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     1500 2023-07-02 00:08:45.103279 aleksis_core-3.1.1/aleksis/core/util/__pycache__/email.cpython-311.pyc
--rw-r--r--   0        0        0      771 2023-07-02 00:08:48.627411 aleksis_core-3.1.1/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     5712 2023-07-02 00:08:48.611411 aleksis_core-3.1.1/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0     9548 2023-07-02 00:08:49.051427 aleksis_core-3.1.1/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
--rw-r--r--   0        0        0     2181 2023-07-02 00:08:46.759341 aleksis_core-3.1.1/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
--rw-r--r--   0        0        0      664 2023-07-02 00:08:46.755341 aleksis_core-3.1.1/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
--rw-r--r--   0        0        0    10148 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/util/apps.py
--rw-r--r--   0        0        0     5970 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/util/auth_helpers.py
--rw-r--r--   0        0        0     7920 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/util/celery_progress.py
--rw-r--r--   0        0        0      197 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/util/context_processors.py
--rw-r--r--   0        0        0    16042 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/util/core_helpers.py
--rw-r--r--   0        0        0      986 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/util/email.py
--rw-r--r--   0        0        0     1175 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/util/forms.py
--rw-r--r--   0        0        0     2895 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/util/frontend_helpers.py
--rw-r--r--   0        0        0     2375 2023-07-02 00:07:11.911774 aleksis_core-3.1.1/aleksis/core/util/ldap.py
--rw-r--r--   0        0        0   192829 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/licenses.json
--rw-r--r--   0        0        0     2255 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/messages.py
--rw-r--r--   0        0        0     2091 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/middlewares.py
--rw-r--r--   0        0        0      850 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/model_helpers.py
--rw-r--r--   0        0        0     3732 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/notifications.py
--rw-r--r--   0        0        0     6131 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/pdf.py
--rw-r--r--   0        0        0     5583 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/predicates.py
--rw-r--r--   0        0        0      936 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/sass_helpers.py
--rw-r--r--   0        0        0      524 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/search.py
--rw-r--r--   0        0        0      130 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/spdx.py
--rw-r--r--   0        0        0     1673 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/util/tables.py
--rw-r--r--   0        0        0    55996 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/views.py
--rw-r--r--   0        0        0    10201 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/vite.config.js
--rw-r--r--   0        0        0      173 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/aleksis/core/wsgi.py
--rw-r--r--   0        0        0       45 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/conftest.py
--rw-r--r--   0        0        0      581 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/docs/Makefile
--rw-r--r--   0        0        0   127432 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/docs/_static/2fa.png
--rw-r--r--   0        0        0    71362 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/docs/_static/accept_invite.png
--rw-r--r--   0        0        0    72621 2023-07-02 00:07:11.915774 aleksis_core-3.1.1/docs/_static/create_dashboard_widget.png
--rw-r--r--   0        0        0    41935 2023-07-02 00:07:11.919774 aleksis_core-3.1.1/docs/_static/create_social_application.png
--rw-r--r--   0        0        0    72508 2023-07-02 00:07:11.919774 aleksis_core-3.1.1/docs/_static/dashboard.png
--rw-r--r--   0        0        0    87601 2023-07-02 00:07:11.919774 aleksis_core-3.1.1/docs/_static/dashboard_widgets.png
--rw-r--r--   0        0        0   119523 2023-07-02 00:07:11.919774 aleksis_core-3.1.1/docs/_static/data_checks.png
--rw-r--r--   0        0        0    81386 2023-07-02 00:07:11.919774 aleksis_core-3.1.1/docs/_static/edit_dashboard.png
--rw-r--r--   0        0        0    85722 2023-07-02 00:07:11.919774 aleksis_core-3.1.1/docs/_static/edit_default_dashboard.png
--rw-r--r--   0        0        0   107979 2023-07-02 00:07:11.923774 aleksis_core-3.1.1/docs/_static/invitations.png
--rw-r--r--   0        0        0   177681 2023-07-02 00:07:11.923774 aleksis_core-3.1.1/docs/_static/invite_existing.png
--rw-r--r--   0        0        0    44868 2023-07-02 00:07:11.923774 aleksis_core-3.1.1/docs/_static/pwa_desktop_chromium.png
--rw-r--r--   0        0        0    69215 2023-07-02 00:07:11.923774 aleksis_core-3.1.1/docs/_static/pwa_mobile_chromium.png
--rw-r--r--   0        0        0   128479 2023-07-02 00:07:11.923774 aleksis_core-3.1.1/docs/_static/pwa_mobile_firefox.png
--rw-r--r--   0        0        0   108973 2023-07-02 00:07:11.923774 aleksis_core-3.1.1/docs/_static/pwa_mobile_safari.png
--rw-r--r--   0        0        0    69804 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/_static/signup.png
--rw-r--r--   0        0        0      132 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/00_index.rst
--rw-r--r--   0        0        0     4231 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/01_core_concepts.rst
--rw-r--r--   0        0        0     8059 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/10_install.rst
--rw-r--r--   0        0        0     1872 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/15_config_files.rst
--rw-r--r--   0        0        0     2086 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/16_config_options.rst
--rw-r--r--   0        0        0     1648 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/17_storage.rst
--rw-r--r--   0        0        0      803 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/18_mail.rst
--rw-r--r--   0        0        0     1509 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/21_ldap.rst
--rw-r--r--   0        0        0     3037 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/22_registration.rst
--rw-r--r--   0        0        0     1467 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/23_socialaccounts.rst
--rw-r--r--   0        0        0     3218 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/31_monitoring.rst
--rw-r--r--   0        0        0     1012 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/32_tasks.rst
--rw-r--r--   0        0        0     1393 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/33_data_checks.rst
--rw-r--r--   0        0        0     4610 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/admin/50_dashboard.rst
--rw-r--r--   0        0        0     6393 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/conf.py
--rw-r--r--   0        0        0      132 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/dev/00_index.rst
--rw-r--r--   0        0        0     4000 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/dev/01_setup.rst
--rw-r--r--   0        0        0     1427 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/dev/02_install_apps.rst
--rw-r--r--   0        0        0     3117 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/dev/03_run_tests.rst
--rw-r--r--   0        0        0     4519 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/dev/04_materialize_templates.rst
--rw-r--r--   0        0        0      289 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/dev/05_extensible_models.rst
--rw-r--r--   0        0        0     1148 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/dev/06_merging_app_settings.rst
--rw-r--r--   0        0        0     1349 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/dev/10_dashboard_widgets.rst
--rw-r--r--   0        0        0      514 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/index.rst
--rw-r--r--   0        0        0      787 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/make.bat
--rw-r--r--   0        0        0       95 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/00_index.rst
--rw-r--r--   0        0        0       69 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/01_checks.rst
--rw-r--r--   0        0        0       70 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/02_managers.rst
--rw-r--r--   0        0        0       64 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/03_mixins.rst
--rw-r--r--   0        0        0       84 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/04_models.rst
--rw-r--r--   0        0        0      108 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/05_registries.rst
--rw-r--r--   0        0        0       93 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/06_search_indexes.rst
--rw-r--r--   0        0        0       79 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/07_tables.rst
--rw-r--r--   0        0        0       90 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/08_tasks.rst
--rw-r--r--   0        0        0     1017 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/09_utils.rst
--rw-r--r--   0        0        0       71 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/10_views.rst
--rw-r--r--   0        0        0       77 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/11_filters.rst
--rw-r--r--   0        0        0      373 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/ref/core/12_template_tags.rst
--rw-r--r--   0        0        0      112 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/user/00_index.rst
--rw-r--r--   0        0        0     1152 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/user/01_registration.rst
--rw-r--r--   0        0        0     3465 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/user/02_personal_account.rst
--rw-r--r--   0        0        0     1770 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/user/10_dashboard.rst
--rw-r--r--   0        0        0     2607 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/docs/user/20_pwa.rst
--rw-r--r--   0        0        0     4596 2023-07-02 00:07:32.364543 aleksis_core-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     2599 2023-07-02 00:07:11.927774 aleksis_core-3.1.1/tox.ini
--rw-r--r--   0        0        0     8565 1970-01-01 00:00:00.000000 aleksis_core-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    38157 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/CHANGELOG.rst
+-rw-r--r--   0        0        0    14353 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/LICENCE.rst
+-rw-r--r--   0        0        0     3786 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/README.rst
+-rw-r--r--   0        0        0      194 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/aleksis/core/__init__.py
+-rw-r--r--   0        0        0      464 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/aleksis/core/__main__.py
+-rw-r--r--   0        0        0      510 2023-07-05 19:58:31.878172 aleksis_core-3.1.2/aleksis/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1068 2023-07-05 19:58:35.354303 aleksis_core-3.1.2/aleksis/core/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0        0        0     2061 2023-07-05 19:58:42.118558 aleksis_core-3.1.2/aleksis/core/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0    11380 2023-07-05 19:58:38.138408 aleksis_core-3.1.2/aleksis/core/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     2533 2023-07-05 19:58:31.942174 aleksis_core-3.1.2/aleksis/core/__pycache__/celery.cpython-311.pyc
+-rw-r--r--   0        0        0     3716 2023-07-05 19:58:42.298565 aleksis_core-3.1.2/aleksis/core/__pycache__/checks.cpython-311.pyc
+-rw-r--r--   0        0        0    17897 2023-07-05 19:58:41.434532 aleksis_core-3.1.2/aleksis/core/__pycache__/data_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     5154 2023-07-05 19:58:42.318566 aleksis_core-3.1.2/aleksis/core/__pycache__/health_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     8423 2023-07-05 19:58:41.518535 aleksis_core-3.1.2/aleksis/core/__pycache__/managers.cpython-311.pyc
+-rw-r--r--   0        0        0    31446 2023-07-05 19:58:41.454533 aleksis_core-3.1.2/aleksis/core/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0        0        0    85606 2023-07-05 19:58:40.354492 aleksis_core-3.1.2/aleksis/core/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0    22237 2023-07-05 19:58:42.478572 aleksis_core-3.1.2/aleksis/core/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1370 2023-07-05 19:58:38.198410 aleksis_core-3.1.2/aleksis/core/__pycache__/registries.cpython-311.pyc
+-rw-r--r--   0        0        0    16523 2023-07-05 19:58:42.154559 aleksis_core-3.1.2/aleksis/core/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0    44046 2023-07-05 19:58:35.430306 aleksis_core-3.1.2/aleksis/core/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0     3825 2023-07-05 19:58:41.542537 aleksis_core-3.1.2/aleksis/core/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0        0        0      950 2023-07-05 19:54:43.393550 aleksis_core-3.1.2/aleksis/core/admin.py
+-rw-r--r--   0        0        0     8519 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/apps.py
+-rw-r--r--   0        0        0     1338 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/celery.py
+-rw-r--r--   0        0        0     2751 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/checks.py
+-rw-r--r--   0        0        0    11534 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/data_checks.py
+-rw-r--r--   0        0        0      741 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/decorators.py
+-rw-r--r--   0        0        0     5556 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/filters.py
+-rw-r--r--   0        0        0    31619 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/forms.py
+-rw-r--r--   0        0        0     3175 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/apollo.js
+-rw-r--r--   0        0        0     1089 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/dateTimeFormats.js
+-rw-r--r--   0        0        0      197 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/i18n.js
+-rw-r--r--   0        0        0      157 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/router.js
+-rw-r--r--   0        0        0      133 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/sentry.js
+-rw-r--r--   0        0        0      793 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/app/vuetify.js
+-rw-r--r--   0        0        0     4485 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/LegacyBaseTemplate.vue
+-rw-r--r--   0        0        0      158 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/Parent.vue
+-rw-r--r--   0        0        0      335 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/about/About.vue
+-rw-r--r--   0        0        0     1971 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/about/AboutAleksis.vue
+-rw-r--r--   0        0        0     3831 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/about/InstalledAppCard.vue
+-rw-r--r--   0        0        0     1003 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/about/InstalledAppsList.vue
+-rw-r--r--   0        0        0      351 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/about/installedApps.graphql
+-rw-r--r--   0        0        0     2411 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/AccountMenu.vue
+-rw-r--r--   0        0        0     9590 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/App.vue
+-rw-r--r--   0        0        0      314 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/BrandLogo.vue
+-rw-r--r--   0        0        0     1064 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/ErrorPage.vue
+-rw-r--r--   0        0        0     1470 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/LanguageForm.vue
+-rw-r--r--   0        0        0     3778 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/SideNav.vue
+-rw-r--r--   0        0        0     1454 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/SidenavSearch.vue
+-rw-r--r--   0        0        0      747 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/SnackbarItem.vue
+-rw-r--r--   0        0        0     1932 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/Splash.vue
+-rw-r--r--   0        0        0      124 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/customMenu.graphql
+-rw-r--r--   0        0        0      205 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/dynamicRoutes.graphql
+-rw-r--r--   0        0        0       42 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/messages.graphql
+-rw-r--r--   0        0        0       59 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/ping.graphql
+-rw-r--r--   0        0        0      139 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/searchSnippets.graphql
+-rw-r--r--   0        0        0      412 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/systemProperties.graphql
+-rw-r--r--   0        0        0      322 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/app/whoAmI.graphql
+-rw-r--r--   0        0        0     2558 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
+-rw-r--r--   0        0        0     1884 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
+-rw-r--r--   0        0        0      220 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
+-rw-r--r--   0        0        0       65 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
+-rw-r--r--   0        0        0     3482 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
+-rw-r--r--   0        0        0     1910 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
+-rw-r--r--   0        0        0      925 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
+-rw-r--r--   0        0        0      432 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
+-rw-r--r--   0        0        0      191 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
+-rw-r--r--   0        0        0      118 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
+-rw-r--r--   0        0        0      655 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/AvatarClickbox.vue
+-rw-r--r--   0        0        0      212 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/BackButton.vue
+-rw-r--r--   0        0        0      598 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/ButtonMenu.vue
+-rw-r--r--   0        0        0      981 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/DetailView.vue
+-rw-r--r--   0        0        0      408 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/ListView.vue
+-rw-r--r--   0        0        0      268 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/MessageBox.vue
+-rw-r--r--   0        0        0     1914 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/ObjectOverview.vue
+-rw-r--r--   0        0        0      269 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/SmallContainer.vue
+-rw-r--r--   0        0        0     2017 2023-07-05 19:54:43.397550 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/UpdateIndicator.vue
+-rw-r--r--   0        0        0     3232 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
+-rw-r--r--   0        0        0      706 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/group/GroupCollection.vue
+-rw-r--r--   0        0        0     3034 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/NotificationItem.vue
+-rw-r--r--   0        0        0     2616 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/NotificationList.vue
+-rw-r--r--   0        0        0      107 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
+-rw-r--r--   0        0        0      200 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/myNotifications.graphql
+-rw-r--r--   0        0        0     1017 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/pdf/DownloadPDF.vue
+-rw-r--r--   0        0        0       78 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/pdf/pdf.graphql
+-rw-r--r--   0        0        0     1410 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/AdditionalImage.vue
+-rw-r--r--   0        0        0     1082 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/AvatarContent.vue
+-rw-r--r--   0        0        0     2892 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonActions.vue
+-rw-r--r--   0        0        0      527 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
+-rw-r--r--   0        0        0      759 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonCollection.vue
+-rw-r--r--   0        0        0     7423 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonOverview.vue
+-rw-r--r--   0        0        0      108 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/avatarContent.graphql
+-rw-r--r--   0        0        0      196 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/personActions.graphql
+-rw-r--r--   0        0        0      575 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/person/personOverview.graphql
+-rw-r--r--   0        0        0     3858 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactor.vue
+-rw-r--r--   0        0        0     1512 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
+-rw-r--r--   0        0        0      589 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
+-rw-r--r--   0        0        0      385 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/twoFactor.graphql
+-rw-r--r--   0        0        0      390 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/css/global.scss
+-rw-r--r--   0        0        0     2561 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/index.js
+-rw-r--r--   0        0        0    10763 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/messages/de.json
+-rw-r--r--   0        0        0     9741 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/messages/en.json
+-rw-r--r--   0        0        0    12252 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/messages/ru.json
+-rw-r--r--   0        0        0    14534 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/messages/uk.json
+-rw-r--r--   0        0        0     1211 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/aleksis.js
+-rw-r--r--   0        0        0      538 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/error404.js
+-rw-r--r--   0        0        0     3441 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/menus.js
+-rw-r--r--   0        0        0     2256 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/offline.js
+-rw-r--r--   0        0        0      736 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/permissions.js
+-rw-r--r--   0        0        0     2154 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/routes.js
+-rw-r--r--   0        0        0     1619 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/mixins/useRegisterSW.js
+-rw-r--r--   0        0        0     6380 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/plugins/aleksis.js
+-rw-r--r--   0        0        0      450 2023-07-05 19:54:43.401551 aleksis_core-3.1.2/aleksis/core/frontend/routeValidators.js
+-rw-r--r--   0        0        0    36573 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/frontend/routes.js
+-rw-r--r--   0        0        0     2642 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/health_checks.py
+-rw-r--r--   0        0        0      487 2023-07-05 19:58:43.062594 aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74307 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      463 2023-07-05 19:58:43.050593 aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      894 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    63806 2023-07-05 19:58:43.038593 aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   126085 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      567 2023-07-05 19:58:43.006592 aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1118 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      942 2023-07-05 19:58:42.990591 aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    77782 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-07-05 19:58:43.022592 aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      810 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     2584 2023-07-05 19:58:43.146597 aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    82875 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-05 19:58:43.146597 aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2023-07-05 19:58:43.106596 aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74237 2023-07-05 19:54:43.405551 aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-05 19:58:43.058594 aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    80303 2023-07-05 19:58:43.146597 aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   144575 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2023-07-05 19:58:43.182598 aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1321 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2023-07-05 19:58:42.998592 aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74177 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-07-05 19:58:42.990591 aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    77610 2023-07-05 19:58:43.118596 aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   131787 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2023-07-05 19:58:43.070594 aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1331 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/management/__init__.py
+-rw-r--r--   0        0        0     3957 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/management/commands/convert_urls_to_routes.py
+-rw-r--r--   0        0        0      945 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/management/commands/vite.py
+-rw-r--r--   0        0        0      439 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/management/commands/webpack_bundle.py
+-rw-r--r--   0        0        0     4690 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/managers.py
+-rw-r--r--   0        0        0    51004 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2473 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0002_school_term.py
+-rw-r--r--   0        0        0      531 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0003_drop_image_cropping.py
+-rw-r--r--   0        0        0      796 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
+-rw-r--r--   0        0        0     1252 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0005_timestamped_activity_notification.py
+-rw-r--r--   0        0        0     1567 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0006_dashboard_widget_size.py
+-rw-r--r--   0        0        0     1396 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0007_dashboard_widget_order.py
+-rw-r--r--   0        0        0     2311 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0008_data_check_result.py
+-rw-r--r--   0        0        0     1052 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0009_default_dashboard.py
+-rw-r--r--   0        0        0      952 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0010_external_link_widget.py
+-rw-r--r--   0        0        0      829 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0011_globalpermissions_options.py
+-rw-r--r--   0        0        0      501 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0012_valid_from_announcement.py
+-rw-r--r--   0        0        0     2270 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0013_pdf_file.py
+-rw-r--r--   0        0        0      533 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0014_alter_pdffile_file.py
+-rw-r--r--   0        0        0     1174 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0015_oauth_permissions.py
+-rw-r--r--   0        0        0     1538 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0016_taskuserassignment.py
+-rw-r--r--   0        0        0      426 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0017_dashboardwidget_broken.py
+-rw-r--r--   0        0        0      897 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0018_pdffile_html_file.py
+-rw-r--r--   0        0        0     2177 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
+-rw-r--r--   0        0        0      542 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0020_pdf_file_person_optional.py
+-rw-r--r--   0        0        0     1084 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
+-rw-r--r--   0        0        0      923 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0022_public_favicon.py
+-rw-r--r--   0        0        0     6340 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0023_oauth_application_model.py
+-rw-r--r--   0        0        0      714 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0024_oauth_grant_types_optional.py
+-rw-r--r--   0        0        0     1717 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0025_oauth_align_user_fk.py
+-rw-r--r--   0        0        0      582 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
+-rw-r--r--   0        0        0      457 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0027_person_place_of_birth.py
+-rw-r--r--   0        0        0      947 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0028_char_field_not_null.py
+-rw-r--r--   0        0        0     1465 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0029_invitations.py
+-rw-r--r--   0        0        0     1776 2023-07-05 19:54:43.409551 aleksis_core-3.1.2/aleksis/core/migrations/0030_user_attributes.py
+-rw-r--r--   0        0        0      526 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0031_oauthapplication_icon.py
+-rw-r--r--   0        0        0      340 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0032_remove_person_is_active.py
+-rw-r--r--   0        0        0     2416 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0033_update_photo_avatar.py
+-rw-r--r--   0        0        0      816 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0034_invite_permission.py
+-rw-r--r--   0        0        0     1781 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0035_preference_model_unique.py
+-rw-r--r--   0        0        0      626 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0036_additionalfields_helptext_required.py
+-rw-r--r--   0        0        0      917 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0037_add_static_content_widget.py
+-rw-r--r--   0        0        0      522 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0038_notification_send_at.py
+-rw-r--r--   0        0        0     1029 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0039_personal_ical_url.py
+-rw-r--r--   0        0        0      613 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
+-rw-r--r--   0        0        0      516 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0041_update_gender_choices.py
+-rw-r--r--   0        0        0      547 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0042_pdffile_empty.py
+-rw-r--r--   0        0        0     2261 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0043_task_assignment_meta.py
+-rw-r--r--   0        0        0      532 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0044_task_assignment_result_fetched.py
+-rw-r--r--   0        0        0      486 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
+-rw-r--r--   0        0        0   290966 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0046_notification_create_field_icon.py
+-rw-r--r--   0        0        0     2717 2023-07-05 19:54:43.413551 aleksis_core-3.1.2/aleksis/core/migrations/0047_add_room_model.py
+-rw-r--r--   0        0        0   893996 2023-07-05 19:54:43.417551 aleksis_core-3.1.2/aleksis/core/migrations/0048_delete_personalicalurl.py
+-rw-r--r--   0        0        0      580 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/migrations/__init__.py
+-rw-r--r--   0        0        0    19769 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/mixins.py
+-rw-r--r--   0        0        0    51781 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/models.py
+-rw-r--r--   0        0        0    13478 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/preferences.py
+-rw-r--r--   0        0        0      692 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/registries.py
+-rw-r--r--   0        0        0    16018 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/rules.py
+-rw-r--r--   0        0        0     7486 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/__init__.py
+-rw-r--r--   0        0        0     1301 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/base.py
+-rw-r--r--   0        0        0     3049 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/celery_progress.py
+-rw-r--r--   0        0        0      585 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/custom_menu.py
+-rw-r--r--   0        0        0      459 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/dynamic_routes.py
+-rw-r--r--   0        0        0     2046 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/group.py
+-rw-r--r--   0        0        0     1743 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/installed_apps.py
+-rw-r--r--   0        0        0      265 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/message.py
+-rw-r--r--   0        0        0     1296 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/notification.py
+-rw-r--r--   0        0        0     1179 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/oauth.py
+-rw-r--r--   0        0        0      535 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/pdf.py
+-rw-r--r--   0        0        0      124 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/permissions.py
+-rw-r--r--   0        0        0     9708 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/person.py
+-rw-r--r--   0        0        0      191 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/room.py
+-rw-r--r--   0        0        0      163 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/school_term.py
+-rw-r--r--   0        0        0      868 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/search.py
+-rw-r--r--   0        0        0     1343 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/site_preferences.py
+-rw-r--r--   0        0        0     1651 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/system_properties.py
+-rw-r--r--   0        0        0     3297 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/two_factor.py
+-rw-r--r--   0        0        0      829 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/schema/user.py
+-rw-r--r--   0        0        0      418 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/search_indexes.py
+-rw-r--r--   0        0        0    39939 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/settings.py
+-rw-r--r--   0        0        0    49621 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-banner.svg
+-rw-r--r--   0        0        0     1862 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-favicon.png
+-rw-r--r--   0        0        0    17172 2023-07-05 19:54:43.421551 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon-maskable.png
+-rw-r--r--   0        0        0     7843 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon-maskable.svg
+-rw-r--r--   0        0        0    31902 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon.png
+-rw-r--r--   0        0        0     7346 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon.svg
+-rw-r--r--   0        0        0    19126 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/img/fallback.png
+-rw-r--r--   0        0        0     2237 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/img/hero.svg
+-rw-r--r--   0        0        0      490 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/copy_button.js
+-rw-r--r--   0        0        0      521 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/edit_dashboard.js
+-rw-r--r--   0        0        0      618 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/helper.js
+-rw-r--r--   0        0        0      984 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/include_ajax_live.js
+-rw-r--r--   0        0        0     4350 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/main.js
+-rw-r--r--   0        0        0     1654 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/multi_select.js
+-rw-r--r--   0        0        0     3495 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/search.js
+-rw-r--r--   0        0        0     2578 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/js/serviceworker.js
+-rw-r--r--   0        0        0      271 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/print-simple.css
+-rw-r--r--   0        0        0     1627 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/print.css
+-rw-r--r--   0        0        0      187 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/print_landscape.css
+-rw-r--r--   0        0        0     1064 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/public/materialize-custom.scss
+-rw-r--r--   0        0        0    15745 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/public/style.scss
+-rw-r--r--   0        0        0    11345 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/static/public/theme.scss
+-rw-r--r--   0        0        0     6876 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/tables.py
+-rw-r--r--   0        0        0     2330 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/tasks.py
+-rw-r--r--   0        0        0      838 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/403.html
+-rw-r--r--   0        0        0      789 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/404.html
+-rw-r--r--   0        0        0      918 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/500.html
+-rw-r--r--   0        0        0       76 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/503.html
+-rw-r--r--   0        0        0      851 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/account_inactive.html
+-rw-r--r--   0        0        0      169 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/email/base_message.txt
+-rw-r--r--   0        0        0      525 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0        0        0     1255 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/email_confirm.html
+-rw-r--r--   0        0        0      804 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_change.html
+-rw-r--r--   0        0        0      888 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_change_disabled.html
+-rw-r--r--   0        0        0     1376 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_reset.html
+-rw-r--r--   0        0        0      825 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     2305 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      649 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      500 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/password_set.html
+-rw-r--r--   0        0        0      888 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/signup.html
+-rw-r--r--   0        0        0      838 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      820 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/verification_email_required.html
+-rw-r--r--   0        0        0     1160 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      979 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/components/chips.html
+-rw-r--r--   0        0        0      350 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/components/materialize-chips.html
+-rw-r--r--   0        0        0      225 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/components/msgbox.html
+-rw-r--r--   0        0        0      958 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/components/pagination.html
+-rw-r--r--   0        0        0      486 2023-07-05 19:54:43.425552 aleksis_core-3.1.2/aleksis/core/templates/components/text_collapsible.html
+-rw-r--r--   0        0        0      483 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/additional_field/edit.html
+-rw-r--r--   0        0        0      594 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/additional_field/list.html
+-rw-r--r--   0        0        0     1053 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/announcement/form.html
+-rw-r--r--   0        0        0     1900 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/announcement/list.html
+-rw-r--r--   0        0        0     3099 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/base.html
+-rw-r--r--   0        0        0     2454 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/base_print.html
+-rw-r--r--   0        0        0     1178 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/base_simple_print.html
+-rw-r--r--   0        0        0      628 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/create.html
+-rw-r--r--   0        0        0      635 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
+-rw-r--r--   0        0        0      626 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/edit.html
+-rw-r--r--   0        0        0      262 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
+-rw-r--r--   0        0        0     1349 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/list.html
+-rw-r--r--   0        0        0      226 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
+-rw-r--r--   0        0        0     3879 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/data_check/list.html
+-rw-r--r--   0        0        0     2233 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/edit_dashboard.html
+-rw-r--r--   0        0        0        0 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/empty.html
+-rw-r--r--   0        0        0     5310 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group/child_groups.html
+-rw-r--r--   0        0        0      650 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group/edit.html
+-rw-r--r--   0        0        0     3382 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group/full.html
+-rw-r--r--   0        0        0     1019 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group/list.html
+-rw-r--r--   0        0        0      465 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group_type/edit.html
+-rw-r--r--   0        0        0      564 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/group_type/list.html
+-rw-r--r--   0        0        0     2504 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/index.html
+-rw-r--r--   0        0        0      777 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/pages/delete.html
+-rw-r--r--   0        0        0     6832 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/pages/system_status.html
+-rw-r--r--   0        0        0      603 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/pages/test_pdf.html
+-rw-r--r--   0        0        0       93 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/address.html
+-rw-r--r--   0        0        0      189 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/admins_list.html
+-rw-r--r--   0        0        0     1632 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/announcements.html
+-rw-r--r--   0        0        0     1472 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/avatar_content.html
+-rw-r--r--   0        0        0      319 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/copy_button.html
+-rw-r--r--   0        0        0     1089 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/crud_events.html
+-rw-r--r--   0        0        0      389 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/edit_dashboard_widget.html
+-rw-r--r--   0        0        0     1624 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/meta.html
+-rw-r--r--   0        0        0      414 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/on_page_menu.html
+-rw-r--r--   0        0        0      260 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/save_button.html
+-rw-r--r--   0        0        0     2374 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/splash_screen.html
+-rw-r--r--   0        0        0      325 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/partials/turnable.html
+-rw-r--r--   0        0        0      915 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/perms/assign.html
+-rw-r--r--   0        0        0     2478 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/perms/list.html
+-rw-r--r--   0        0        0      376 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/person/collection.html
+-rw-r--r--   0        0        0      649 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/person/create.html
+-rw-r--r--   0        0        0      645 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/person/edit.html
+-rw-r--r--   0        0        0     1165 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/person/list.html
+-rw-r--r--   0        0        0      455 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/school_term/create.html
+-rw-r--r--   0        0        0      451 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/school_term/edit.html
+-rw-r--r--   0        0        0      556 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/school_term/list.html
+-rw-r--r--   0        0        0      935 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/core/vue_index.html
+-rw-r--r--   0        0        0     3921 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/django_tables2/materialize.html
+-rw-r--r--   0        0        0      981 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/dynamic_preferences/form.html
+-rw-r--r--   0        0        0      376 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/dynamic_preferences/sections.html
+-rw-r--r--   0        0        0      764 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/invitations/disabled.html
+-rw-r--r--   0        0        0     1281 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/invitations/enter.html
+-rw-r--r--   0        0        0     1162 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/invitations/forms/_invite.html
+-rw-r--r--   0        0        0      102 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/invitations/messages/invite_accepted.txt
+-rw-r--r--   0        0        0      171 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/field_errors.html
+-rw-r--r--   0        0        0     1232 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
+-rw-r--r--   0        0        0     1897 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/fields/colorfield_colorwidget.html
+-rw-r--r--   0        0        0     1009 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
+-rw-r--r--   0        0        0     1009 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/fields/django_select2_select2widget.html
+-rw-r--r--   0        0        0      253 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/material/non_field_errors.html
+-rw-r--r--   0        0        0      663 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/create.html
+-rw-r--r--   0        0        0     2335 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/detail.html
+-rw-r--r--   0        0        0      669 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/edit.html
+-rw-r--r--   0        0        0     1074 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/list.html
+-rw-r--r--   0        0        0     2686 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/authorize.html
+-rw-r--r--   0        0        0      887 2023-07-05 19:54:43.429552 aleksis_core-3.1.2/aleksis/core/templates/offline.html
+-rw-r--r--   0        0        0       42 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/indexes/core/group_text.txt
+-rw-r--r--   0        0        0       69 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/indexes/core/person_text.txt
+-rw-r--r--   0        0        0       42 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/indexes/core/room_text.txt
+-rw-r--r--   0        0        0     3171 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/search.html
+-rw-r--r--   0        0        0      243 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/searchbar_snippet.html
+-rw-r--r--   0        0        0      150 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/search/searchbar_snippets.html
+-rw-r--r--   0        0        0      169 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/sms/notification.txt
+-rw-r--r--   0        0        0      893 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0     1268 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1289 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      809 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0        0        0     1012 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0     1434 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      630 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/base.email
+-rw-r--r--   0        0        0     1527 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/celery_failure.email
+-rw-r--r--   0        0        0      994 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/data_checks.email
+-rw-r--r--   0        0        0      990 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/email.css
+-rw-r--r--   0        0        0     1102 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/invitation.email
+-rw-r--r--   0        0        0     1461 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/notification.email
+-rw-r--r--   0        0        0      668 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/templated_email/person_changed.email
+-rw-r--r--   0        0        0      219 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/_base_focus.html
+-rw-r--r--   0        0        0      877 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0        0        0      119 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0        0        0     1780 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0        0        0     6712 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/login.html
+-rw-r--r--   0        0        0      943 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/otp_required.html
+-rw-r--r--   0        0        0      986 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/phone_register.html
+-rw-r--r--   0        0        0     3312 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/setup.html
+-rw-r--r--   0        0        0     2127 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/setup_complete.html
+-rw-r--r--   0        0        0      786 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templates/two_factor/profile/disable.html
+-rw-r--r--   0        0        0        0 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/apps.py
+-rw-r--r--   0        0        0      394 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/dashboard.py
+-rw-r--r--   0        0        0     1618 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/data_helpers.py
+-rw-r--r--   0        0        0     1523 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/html_helpers.py
+-rw-r--r--   0        0        0      206 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/templatetags/msg_box.py
+-rw-r--r--   0        0        0     3696 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/browser/test_selenium.py
+-rw-r--r--   0        0        0     6596 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test.pdf
+-rw-r--r--   0        0        0     6562 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test_group.py
+-rw-r--r--   0        0        0     1520 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test_group_sync.py
+-rw-r--r--   0        0        0     3049 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test_notification.py
+-rw-r--r--   0        0        0     4003 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test_pdffile.py
+-rw-r--r--   0        0        0      427 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/models/test_person.py
+-rw-r--r--   0        0        0     5503 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/regression/test_regression.py
+-rw-r--r--   0        0        0      683 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/regression/view_oauth.py
+-rw-r--r--   0        0        0     1021 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/templatetags/test_data_helpers.py
+-rw-r--r--   0        0        0     2292 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/tests/views/test_account.py
+-rw-r--r--   0        0        0    18734 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/urls.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/util/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-05 19:58:33.254224 aleksis_core-3.1.2/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14902 2023-07-05 19:58:38.202410 aleksis_core-3.1.2/aleksis/core/util/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0    10101 2023-07-05 19:58:41.534536 aleksis_core-3.1.2/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
+-rw-r--r--   0        0        0    24932 2023-07-05 19:58:33.266224 aleksis_core-3.1.2/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     1500 2023-07-05 19:58:35.266300 aleksis_core-3.1.2/aleksis/core/util/__pycache__/email.cpython-311.pyc
+-rw-r--r--   0        0        0      771 2023-07-05 19:58:41.570537 aleksis_core-3.1.2/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     5712 2023-07-05 19:58:41.542537 aleksis_core-3.1.2/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0     9548 2023-07-05 19:58:42.170560 aleksis_core-3.1.2/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
+-rw-r--r--   0        0        0     2181 2023-07-05 19:58:38.274413 aleksis_core-3.1.2/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0      664 2023-07-05 19:58:38.270413 aleksis_core-3.1.2/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
+-rw-r--r--   0        0        0    10969 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/util/apps.py
+-rw-r--r--   0        0        0     5970 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/util/auth_helpers.py
+-rw-r--r--   0        0        0     7920 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/util/celery_progress.py
+-rw-r--r--   0        0        0      197 2023-07-05 19:54:43.433552 aleksis_core-3.1.2/aleksis/core/util/context_processors.py
+-rw-r--r--   0        0        0    16042 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/core_helpers.py
+-rw-r--r--   0        0        0      986 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/email.py
+-rw-r--r--   0        0        0     1175 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/forms.py
+-rw-r--r--   0        0        0     2895 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/frontend_helpers.py
+-rw-r--r--   0        0        0     2375 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/ldap.py
+-rw-r--r--   0        0        0   192829 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/licenses.json
+-rw-r--r--   0        0        0     2255 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/messages.py
+-rw-r--r--   0        0        0     2091 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/middlewares.py
+-rw-r--r--   0        0        0      850 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/model_helpers.py
+-rw-r--r--   0        0        0     3732 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/notifications.py
+-rw-r--r--   0        0        0     6131 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/pdf.py
+-rw-r--r--   0        0        0     5583 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/predicates.py
+-rw-r--r--   0        0        0      936 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/sass_helpers.py
+-rw-r--r--   0        0        0      524 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/search.py
+-rw-r--r--   0        0        0      130 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/spdx.py
+-rw-r--r--   0        0        0     1673 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/util/tables.py
+-rw-r--r--   0        0        0    55996 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/views.py
+-rw-r--r--   0        0        0    10257 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/vite.config.js
+-rw-r--r--   0        0        0      173 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/aleksis/core/wsgi.py
+-rw-r--r--   0        0        0       45 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/conftest.py
+-rw-r--r--   0        0        0      581 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/docs/Makefile
+-rw-r--r--   0        0        0   127432 2023-07-05 19:54:43.437552 aleksis_core-3.1.2/docs/_static/2fa.png
+-rw-r--r--   0        0        0    71362 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/accept_invite.png
+-rw-r--r--   0        0        0    72621 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/create_dashboard_widget.png
+-rw-r--r--   0        0        0    41935 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/create_social_application.png
+-rw-r--r--   0        0        0    72508 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/dashboard.png
+-rw-r--r--   0        0        0    87601 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/dashboard_widgets.png
+-rw-r--r--   0        0        0   119523 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/data_checks.png
+-rw-r--r--   0        0        0    81386 2023-07-05 19:54:43.441552 aleksis_core-3.1.2/docs/_static/edit_dashboard.png
+-rw-r--r--   0        0        0    85722 2023-07-05 19:54:43.445552 aleksis_core-3.1.2/docs/_static/edit_default_dashboard.png
+-rw-r--r--   0        0        0   107979 2023-07-05 19:54:43.445552 aleksis_core-3.1.2/docs/_static/invitations.png
+-rw-r--r--   0        0        0   177681 2023-07-05 19:54:43.445552 aleksis_core-3.1.2/docs/_static/invite_existing.png
+-rw-r--r--   0        0        0    44868 2023-07-05 19:54:43.445552 aleksis_core-3.1.2/docs/_static/pwa_desktop_chromium.png
+-rw-r--r--   0        0        0    69215 2023-07-05 19:54:43.445552 aleksis_core-3.1.2/docs/_static/pwa_mobile_chromium.png
+-rw-r--r--   0        0        0   128479 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/_static/pwa_mobile_firefox.png
+-rw-r--r--   0        0        0   108973 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/_static/pwa_mobile_safari.png
+-rw-r--r--   0        0        0    69804 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/_static/signup.png
+-rw-r--r--   0        0        0      132 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     4231 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/01_core_concepts.rst
+-rw-r--r--   0        0        0     8067 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/10_install.rst
+-rw-r--r--   0        0        0     1872 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/15_config_files.rst
+-rw-r--r--   0        0        0     2086 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/16_config_options.rst
+-rw-r--r--   0        0        0     1648 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/17_storage.rst
+-rw-r--r--   0        0        0      803 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/18_mail.rst
+-rw-r--r--   0        0        0     1509 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/21_ldap.rst
+-rw-r--r--   0        0        0     3037 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/22_registration.rst
+-rw-r--r--   0        0        0     1467 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/23_socialaccounts.rst
+-rw-r--r--   0        0        0     3218 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/31_monitoring.rst
+-rw-r--r--   0        0        0     1012 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/32_tasks.rst
+-rw-r--r--   0        0        0     1393 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/33_data_checks.rst
+-rw-r--r--   0        0        0     4610 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/admin/50_dashboard.rst
+-rw-r--r--   0        0        0     6393 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/conf.py
+-rw-r--r--   0        0        0      132 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/00_index.rst
+-rw-r--r--   0        0        0     4058 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/01_setup.rst
+-rw-r--r--   0        0        0     1427 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/02_install_apps.rst
+-rw-r--r--   0        0        0     3117 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/03_run_tests.rst
+-rw-r--r--   0        0        0     4519 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/04_materialize_templates.rst
+-rw-r--r--   0        0        0      289 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/05_extensible_models.rst
+-rw-r--r--   0        0        0     1148 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/06_merging_app_settings.rst
+-rw-r--r--   0        0        0     1349 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/dev/10_dashboard_widgets.rst
+-rw-r--r--   0        0        0      514 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/make.bat
+-rw-r--r--   0        0        0       95 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/00_index.rst
+-rw-r--r--   0        0        0       69 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/01_checks.rst
+-rw-r--r--   0        0        0       70 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/02_managers.rst
+-rw-r--r--   0        0        0       64 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/03_mixins.rst
+-rw-r--r--   0        0        0       84 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/04_models.rst
+-rw-r--r--   0        0        0      108 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/05_registries.rst
+-rw-r--r--   0        0        0       93 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/06_search_indexes.rst
+-rw-r--r--   0        0        0       79 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/07_tables.rst
+-rw-r--r--   0        0        0       90 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/08_tasks.rst
+-rw-r--r--   0        0        0     1017 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/09_utils.rst
+-rw-r--r--   0        0        0       71 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/10_views.rst
+-rw-r--r--   0        0        0       77 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/11_filters.rst
+-rw-r--r--   0        0        0      373 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/ref/core/12_template_tags.rst
+-rw-r--r--   0        0        0      112 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/user/00_index.rst
+-rw-r--r--   0        0        0     1152 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/user/01_registration.rst
+-rw-r--r--   0        0        0     3465 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/user/02_personal_account.rst
+-rw-r--r--   0        0        0     1770 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/user/10_dashboard.rst
+-rw-r--r--   0        0        0     2607 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/docs/user/20_pwa.rst
+-rw-r--r--   0        0        0     5377 2023-07-05 19:55:26.067160 aleksis_core-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2599 2023-07-05 19:54:43.449552 aleksis_core-3.1.2/tox.ini
+-rw-r--r--   0        0        0     8603 1970-01-01 00:00:00.000000 aleksis_core-3.1.2/PKG-INFO
```

### Comparing `aleksis_core-3.1.1/CHANGELOG.rst` & `aleksis_core-3.1.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,35 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`3.1.1` - 2023-07-01
---------------------
+`3.1.2`_ - 2023-07-05
+---------------------
+
+Changed
+~~~~~~~
+
+* uWSGI is now installed together with AlekSIS-Core per default.
+
+Fixed
+~~~~~
+
+* Notifications were not properly shown in the frontend.
+* [Dev] Log levels were not correctly propagated to all loggers
+* [Dev] Log format did not contain all essential information
+* When navigating from legacy to legacy page, the latter would reload once for no reason.
+* The oauth authorization page was not accessible when the service worker was active.
+* [Docker] Clear obsolete bundle parts when adding apps using ONBUILD
+* Extensible forms that used a subset of fields did not render properly
+
+`3.1.1`_ - 2023-07-01
+---------------------
 
 Fixed
 ~~~~~
 
 * Progress page didn't work properly.
 * About page failed to load for apps with an unknown licence.
 * QUeries for persons with partial permissions failed.
@@ -158,21 +177,21 @@
 * Model for rooms
 
 Changed
 ~~~~~~~
 
 * Show languages in local language
 * Rewrite of frontend (base template) using Vuetify
-  * Frontend bundling migrated from Webpack to Vite (cf. installation docs)
-  * [Dev] The runuwsgi dev server now starts a Vite dev server with HMR in the
-    background
+    * Frontend bundling migrated from Webpack to Vite (cf. installation docs)
+    * [Dev] The runuwsgi dev server now starts a Vite dev server with HMR in the
+      background
 * OIDC scope "profile" now exposes the avatar instead of the official photo
 * Based on Django 4.0
-  * Use built-in Redis cache backend
-  * Introduce PBKDF2-SHA1 password hashing
+    * Use built-in Redis cache backend
+    * Introduce PBKDF2-SHA1 password hashing
 * Persistent database connections are now health-checked as to not fail
   requests
 * [Dev] The undocumented field `check` on `DataCheckResult` was renamed to `data_check`
 * Frontend bundling migrated from Webpack to Vite
 * Get dashboard widgets and data checks from apps with new registration mechanism.
 * Use write-through cache for sessions to retain on clear_cache
 * Better error page with redirect option to login page when user has no permission to access a route.
@@ -190,16 +209,16 @@
   because of its related name
 
 Removed
 ~~~~~~~
 
 * iCal feed URLs for birthdays (will be reintroduced later)
 * [Dev] Django debug toolbar
-  * It caused major performance issues and is not useful with the new
-    frontend anymore
+    * It caused major performance issues and is not useful with the new
+      frontend anymore
 
 `2.12.3`_ - 2023-03-07
 ----------------------
 
 Fixed
 ~~~~~
 
@@ -342,17 +361,15 @@
 
 Fixed
 ~~~~~
 
 * The menu button used to be displayed twice on smaller screens.
 * The icons were loaded from external servers instead from local server.
 * Weekdays were not translated if system locales were missing
-
-  * Added locales-all to base image and note to docs
-
+    * Added locales-all to base image and note to docs
 * The icons in the account menu were still the old ones.
 * Due to a merge error, the once removed account menu in the sidenav appeared again.
 * Scheduled notifications were shown on dashboard before time.
 * Remove broken notifications menu item in favor of item next to account menu.
 * Serve OAuth discovery information under root of domain
 * [OAuth2] Resources which are protected with client credentials
   allowed access if no scopes were allowed (CVE-2022-29773).
@@ -548,19 +565,17 @@
 * Too long headlines didn't break in another line.
 
 Changed
 ~~~~~~~
 
 * Configuration files are now deep merged by default
 * Improvements for shell_plus module loading
-
-  * core.Group model now takes precedence over auth.Group
-  * Name collisions are resolved by prefixing with the app label
-  * Apps can extend SHELL_PLUS_APP_PREFIXES and SHELL_PLUS_DONT_LOAD
-
+    * core.Group model now takes precedence over auth.Group
+    * Name collisions are resolved by prefixing with the app label
+    * Apps can extend SHELL_PLUS_APP_PREFIXES and SHELL_PLUS_DONT_LOAD
 * [Docker] Base image now contains curl, grep, less, sed, and pspg
 * Views raising a 404 error can now customise the message that is displayed on the error page
 * OpenID Connect is enabled by default now, without RSA support
 * Login and authorization pages for OAuth2/OpenID Connect now indicate that the user is in progress
   to authorize an external application.
 * Tables can be scrolled horizontally.
 * Overhauled person detail page
@@ -1175,7 +1190,8 @@
 .. _3.0b0: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.0b0
 .. _3.0b1: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.0b1
 .. _3.0b2: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.0b2
 .. _3.0b3: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.0b3
 .. _3.0: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.0
 .. _3.1: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.1
 .. _3.1.1: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.1.1
+.. _3.1.2: https://edugit.org/AlekSIS/official/AlekSIS-Core/-/tags/3.1.2
```

### Comparing `aleksis_core-3.1.1/LICENCE.rst` & `aleksis_core-3.1.2/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/README.rst` & `aleksis_core-3.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/__main__.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/__main__.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 464
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/admin.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/admin.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 950
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/apps.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/apps.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 8519
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/celery.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/celery.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 1338
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/checks.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/checks.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 2751
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/data_checks.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/data_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 11534
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/health_checks.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/health_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 2642
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/managers.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/managers.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 4690
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/mixins.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/mixins.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
-files sz: 19163
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+files sz: 19769
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d015a010100640064036c026d
@@ -15,36 +15,36 @@
       195a196d1a5a1a01006400640c6c1b6d1c5a1c6d1d5a1d01006400640d6c
       1e6d1f5a1f01006400640e6c206d215a216d225a2201006400640f6c236d
       245a240100640064106c256d265a266d275a270100640064116c286d295a
       2a0100640064126c2b6d2c5a2c6d2d5a2d0100640064136c2e6d2f5a2f6d
       305a300100640064016c315a31640064146c326d335a330100640064156c
       346d355a350100640064166c366d375a370100640064176c386d395a3901
       00640064186c3a6d3b5a3b6d3c5a3c0100640064196c3d6d3e5a3e6d3f5a
-      3f01006400641a6c406d415a4101006400641b6c426d435a430100640064
-      1c6c446d455a4501006400641d6c466d475a4701006400641e6c486d495a
-      496d4a5a4a6d4b5a4b010002004700641f8400642065176a4c0000000000
-      0000006a4d0000000000000000a6030000ab0300000000000000005a4e64
-      2184005a4f0200470064228400642365176a500000000000000000654eac
-      24a6040000ab0400000000000000005a5102004700642584006426654e65
-      41a6040000ab0400000000000000005a5202004700642784006428655165
-      456552ac24a6050000ab0500000000000000005a53020047006429840064
-      2a6554a6030000ab0300000000000000005a5502004700642b8400642c65
-      176a500000000000000000a6030000ab0300000000000000005a56020047
-      00642d8400642e6522a6030000ab0300000000000000005a570200470064
-      2f8400643065216557ac24a6040000ab0400000000000000005a58020047
-      0064318400643265376547a6040000ab0400000000000000005a59020047
-      006433840064346530a6030000ab0300000000000000005a5a0200470064
-      3584006436650fa6030000ab0300000000000000005a5b02004700643784
-      006438655a652ca6040000ab0400000000000000005a5c02004700643984
-      00643a655a652da6040000ab0400000000000000005a5d02004700643b84
-      00643c652fa6030000ab0300000000000000005a5e02004700643d840064
-      3e6551a6030000ab0300000000000000005a5f02004700643f8400644065
-      58a6030000ab0300000000000000005a60020047006441840064426535a6
-      030000ab0300000000000000005a6102004700644384006444a6020000ab
-      0200000000000000005a6264015300
+      3f6d405a4001006400641a6c416d425a4201006400641b6c436d445a4401
+      006400641c6c456d465a4601006400641d6c476d485a4801006400641e6c
+      496d4a5a4a6d4b5a4b6d4c5a4c010002004700641f8400642065176a4d00
+      000000000000006a4e0000000000000000a6030000ab0300000000000000
+      005a4f642184005a500200470064228400642365176a5100000000000000
+      00654fac24a6040000ab0400000000000000005a52020047006425840064
+      26654f6542a6040000ab0400000000000000005a53020047006427840064
+      28655265466553ac24a6050000ab0500000000000000005a540200470064
+      298400642a6555a6030000ab0300000000000000005a5602004700642b84
+      00642c65176a510000000000000000a6030000ab0300000000000000005a
+      5702004700642d8400642e6522a6030000ab0300000000000000005a5802
+      004700642f8400643065216558ac24a6040000ab0400000000000000005a
+      590200470064318400643265376548a6040000ab0400000000000000005a
+      5a020047006433840064346530a6030000ab0300000000000000005a5b02
+      004700643584006436650fa6030000ab0300000000000000005a5c020047
+      00643784006438655b652ca6040000ab0400000000000000005a5d020047
+      0064398400643a655b652da6040000ab0400000000000000005a5e020047
+      00643b8400643c652fa6030000ab0300000000000000005a5f0200470064
+      3d8400643e6552a6030000ab0300000000000000005a6002004700643f84
+      0064406559a6030000ab0300000000000000005a61020047006441840064
+      426535a6030000ab0300000000000000005a6202004700644384006444a6
+      020000ab0200000000000000005a6364015300
      0           0 RESUME                   0
    
      3           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
@@ -237,262 +237,264 @@
                336 IMPORT_FROM             59 (IntegerField)
                338 STORE_NAME              59 (IntegerField)
                340 IMPORT_FROM             60 (JSONFieldMixin)
                342 STORE_NAME              60 (JSONFieldMixin)
                344 POP_TOP
    
     30         346 LOAD_CONST               0 (0)
-               348 LOAD_CONST              25 (('Layout', 'LayoutNode'))
+               348 LOAD_CONST              25 (('Fieldset', 'Layout', 'LayoutNode'))
                350 IMPORT_NAME             61 (material.base)
-               352 IMPORT_FROM             62 (Layout)
-               354 STORE_NAME              62 (Layout)
-               356 IMPORT_FROM             63 (LayoutNode)
-               358 STORE_NAME              63 (LayoutNode)
-               360 POP_TOP
-   
-    31         362 LOAD_CONST               0 (0)
-               364 LOAD_CONST              26 (('PolymorphicModelBase',))
-               366 IMPORT_NAME             64 (polymorphic.base)
-               368 IMPORT_FROM             65 (PolymorphicModelBase)
-               370 STORE_NAME              65 (PolymorphicModelBase)
-               372 POP_TOP
-   
-    32         374 LOAD_CONST               0 (0)
-               376 LOAD_CONST              27 (('PolymorphicManager',))
-               378 IMPORT_NAME             66 (polymorphic.managers)
-               380 IMPORT_FROM             67 (PolymorphicManager)
-               382 STORE_NAME              67 (PolymorphicManager)
-               384 POP_TOP
-   
-    33         386 LOAD_CONST               0 (0)
-               388 LOAD_CONST              28 (('PolymorphicModel',))
-               390 IMPORT_NAME             68 (polymorphic.models)
-               392 IMPORT_FROM             69 (PolymorphicModel)
-               394 STORE_NAME              69 (PolymorphicModel)
-               396 POP_TOP
-   
-    34         398 LOAD_CONST               0 (0)
-               400 LOAD_CONST              29 (('ObjectPermissionsModelAdmin',))
-               402 IMPORT_NAME             70 (rules.contrib.admin)
-               404 IMPORT_FROM             71 (ObjectPermissionsModelAdmin)
-               406 STORE_NAME              71 (ObjectPermissionsModelAdmin)
-               408 POP_TOP
-   
-    36         410 LOAD_CONST               0 (0)
-               412 LOAD_CONST              30 (('CurrentSiteManagerWithoutMigrations', 'PolymorphicCurrentSiteManager', 'SchoolTermRelatedQuerySet'))
-               414 IMPORT_NAME             72 (aleksis.core.managers)
-               416 IMPORT_FROM             73 (CurrentSiteManagerWithoutMigrations)
-               418 STORE_NAME              73 (CurrentSiteManagerWithoutMigrations)
-               420 IMPORT_FROM             74 (PolymorphicCurrentSiteManager)
-               422 STORE_NAME              74 (PolymorphicCurrentSiteManager)
-               424 IMPORT_FROM             75 (SchoolTermRelatedQuerySet)
-               426 STORE_NAME              75 (SchoolTermRelatedQuerySet)
-               428 POP_TOP
-   
-    43         430 PUSH_NULL
-               432 LOAD_BUILD_CLASS
-               434 LOAD_CONST              31 (<code object _ExtensibleModelBase, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 43>)
-               436 MAKE_FUNCTION            0
-               438 LOAD_CONST              32 ('_ExtensibleModelBase')
-               440 LOAD_NAME               23 (models)
-               442 LOAD_ATTR               76 (base)
-               452 LOAD_ATTR               77 (ModelBase)
-               462 PRECALL                  3
-               466 CALL                     3
-               476 STORE_NAME              78 (_ExtensibleModelBase)
-   
-    63         478 LOAD_CONST              33 (<code object _generate_one_to_one_proxy_property, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 63>)
-               480 MAKE_FUNCTION            0
-               482 STORE_NAME              79 (_generate_one_to_one_proxy_property)
-   
-    85         484 PUSH_NULL
-               486 LOAD_BUILD_CLASS
-               488 LOAD_CONST              34 (<code object ExtensibleModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 85>)
-               490 MAKE_FUNCTION            0
-               492 LOAD_CONST              35 ('ExtensibleModel')
-               494 LOAD_NAME               23 (models)
-               496 LOAD_ATTR               80 (Model)
-               506 LOAD_NAME               78 (_ExtensibleModelBase)
-               508 KW_NAMES                36
-               510 PRECALL                  4
-               514 CALL                     4
-               524 STORE_NAME              81 (ExtensibleModel)
-   
-   374         526 PUSH_NULL
-               528 LOAD_BUILD_CLASS
-               530 LOAD_CONST              37 (<code object _ExtensiblePolymorphicModelBase, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 374>)
-               532 MAKE_FUNCTION            0
-               534 LOAD_CONST              38 ('_ExtensiblePolymorphicModelBase')
-               536 LOAD_NAME               78 (_ExtensibleModelBase)
-               538 LOAD_NAME               65 (PolymorphicModelBase)
-               540 PRECALL                  4
-               544 CALL                     4
-               554 STORE_NAME              82 (_ExtensiblePolymorphicModelBase)
-   
-   378         556 PUSH_NULL
-               558 LOAD_BUILD_CLASS
-               560 LOAD_CONST              39 (<code object ExtensiblePolymorphicModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 378>)
-               562 MAKE_FUNCTION            0
-               564 LOAD_CONST              40 ('ExtensiblePolymorphicModel')
-   
-   379         566 LOAD_NAME               81 (ExtensibleModel)
-               568 LOAD_NAME               69 (PolymorphicModel)
-               570 LOAD_NAME               82 (_ExtensiblePolymorphicModelBase)
-   
-   378         572 KW_NAMES                36
-               574 PRECALL                  5
-               578 CALL                     5
-               588 STORE_NAME              83 (ExtensiblePolymorphicModel)
-   
-   390         590 PUSH_NULL
-               592 LOAD_BUILD_CLASS
-               594 LOAD_CONST              41 (<code object PureDjangoModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 390>)
-               596 MAKE_FUNCTION            0
-               598 LOAD_CONST              42 ('PureDjangoModel')
-               600 LOAD_NAME               84 (object)
-               602 PRECALL                  3
-               606 CALL                     3
-               616 STORE_NAME              85 (PureDjangoModel)
-   
-   396         618 PUSH_NULL
-               620 LOAD_BUILD_CLASS
-               622 LOAD_CONST              43 (<code object GlobalPermissionModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 396>)
-               624 MAKE_FUNCTION            0
-               626 LOAD_CONST              44 ('GlobalPermissionModel')
-               628 LOAD_NAME               23 (models)
-               630 LOAD_ATTR               80 (Model)
-               640 PRECALL                  3
-               644 CALL                     3
-               654 STORE_NAME              86 (GlobalPermissionModel)
-   
-   407         656 PUSH_NULL
-               658 LOAD_BUILD_CLASS
-               660 LOAD_CONST              45 (<code object _ExtensibleFormMetaclass, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 407>)
-               662 MAKE_FUNCTION            0
-               664 LOAD_CONST              46 ('_ExtensibleFormMetaclass')
-               666 LOAD_NAME               34 (ModelFormMetaclass)
-               668 PRECALL                  3
-               672 CALL                     3
-               682 STORE_NAME              87 (_ExtensibleFormMetaclass)
-   
-   423         684 PUSH_NULL
-               686 LOAD_BUILD_CLASS
-               688 LOAD_CONST              47 (<code object ExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 423>)
-               690 MAKE_FUNCTION            0
-               692 LOAD_CONST              48 ('ExtensibleForm')
-               694 LOAD_NAME               33 (ModelForm)
-               696 LOAD_NAME               87 (_ExtensibleFormMetaclass)
-               698 KW_NAMES                36
-               700 PRECALL                  4
-               704 CALL                     4
-               714 STORE_NAME              88 (ExtensibleForm)
-   
-   453         716 PUSH_NULL
-               718 LOAD_BUILD_CLASS
-               720 LOAD_CONST              49 (<code object BaseModelAdmin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 453>)
-               722 MAKE_FUNCTION            0
-               724 LOAD_CONST              50 ('BaseModelAdmin')
-               726 LOAD_NAME               55 (GuardedModelAdmin)
-               728 LOAD_NAME               71 (ObjectPermissionsModelAdmin)
-               730 PRECALL                  4
-               734 CALL                     4
-               744 STORE_NAME              89 (BaseModelAdmin)
-   
-   459         746 PUSH_NULL
-               748 LOAD_BUILD_CLASS
-               750 LOAD_CONST              51 (<code object SuccessMessageMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 459>)
-               752 MAKE_FUNCTION            0
-               754 LOAD_CONST              52 ('SuccessMessageMixin')
-               756 LOAD_NAME               48 (ModelFormMixin)
-               758 PRECALL                  3
-               762 CALL                     3
-               772 STORE_NAME              90 (SuccessMessageMixin)
-   
-   468         774 PUSH_NULL
-               776 LOAD_BUILD_CLASS
-               778 LOAD_CONST              53 (<code object SuccessNextMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 468>)
-               780 MAKE_FUNCTION            0
-               782 LOAD_CONST              54 ('SuccessNextMixin')
-               784 LOAD_NAME               15 (RedirectURLMixin)
-               786 PRECALL                  3
-               790 CALL                     3
-               800 STORE_NAME              91 (SuccessNextMixin)
-   
-   475         802 PUSH_NULL
-               804 LOAD_BUILD_CLASS
-               806 LOAD_CONST              55 (<code object AdvancedCreateView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 475>)
-               808 MAKE_FUNCTION            0
-               810 LOAD_CONST              56 ('AdvancedCreateView')
-               812 LOAD_NAME               90 (SuccessMessageMixin)
-               814 LOAD_NAME               44 (CreateView)
-               816 PRECALL                  4
-               820 CALL                     4
-               830 STORE_NAME              92 (AdvancedCreateView)
-   
-   479         832 PUSH_NULL
-               834 LOAD_BUILD_CLASS
-               836 LOAD_CONST              57 (<code object AdvancedEditView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 479>)
-               838 MAKE_FUNCTION            0
-               840 LOAD_CONST              58 ('AdvancedEditView')
-               842 LOAD_NAME               90 (SuccessMessageMixin)
-               844 LOAD_NAME               45 (UpdateView)
-               846 PRECALL                  4
-               850 CALL                     4
-               860 STORE_NAME              93 (AdvancedEditView)
-   
-   483         862 PUSH_NULL
-               864 LOAD_BUILD_CLASS
-               866 LOAD_CONST              59 (<code object AdvancedDeleteView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 483>)
-               868 MAKE_FUNCTION            0
-               870 LOAD_CONST              60 ('AdvancedDeleteView')
-               872 LOAD_NAME               47 (DeleteView)
-               874 PRECALL                  3
-               878 CALL                     3
-               888 STORE_NAME              94 (AdvancedDeleteView)
-   
-   502         890 PUSH_NULL
-               892 LOAD_BUILD_CLASS
-               894 LOAD_CONST              61 (<code object SchoolTermRelatedExtensibleModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 502>)
-               896 MAKE_FUNCTION            0
-               898 LOAD_CONST              62 ('SchoolTermRelatedExtensibleModel')
-               900 LOAD_NAME               81 (ExtensibleModel)
-               902 PRECALL                  3
-               906 CALL                     3
-               916 STORE_NAME              95 (SchoolTermRelatedExtensibleModel)
-   
-   520         918 PUSH_NULL
-               920 LOAD_BUILD_CLASS
-               922 LOAD_CONST              63 (<code object SchoolTermRelatedExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 520>)
-               924 MAKE_FUNCTION            0
-               926 LOAD_CONST              64 ('SchoolTermRelatedExtensibleForm')
-               928 LOAD_NAME               88 (ExtensibleForm)
-               930 PRECALL                  3
-               934 CALL                     3
-               944 STORE_NAME              96 (SchoolTermRelatedExtensibleForm)
-   
-   537         946 PUSH_NULL
-               948 LOAD_BUILD_CLASS
-               950 LOAD_CONST              65 (<code object PublicFilePreferenceMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 537>)
-               952 MAKE_FUNCTION            0
-               954 LOAD_CONST              66 ('PublicFilePreferenceMixin')
-               956 LOAD_NAME               53 (FilePreference)
-               958 PRECALL                  3
-               962 CALL                     3
-               972 STORE_NAME              97 (PublicFilePreferenceMixin)
-   
-   548         974 PUSH_NULL
-               976 LOAD_BUILD_CLASS
-               978 LOAD_CONST              67 (<code object RegistryObject, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 548>)
-               980 MAKE_FUNCTION            0
-               982 LOAD_CONST              68 ('RegistryObject')
-               984 PRECALL                  2
-               988 CALL                     2
-               998 STORE_NAME              98 (RegistryObject)
-              1000 LOAD_CONST               1 (None)
-              1002 RETURN_VALUE
+               352 IMPORT_FROM             62 (Fieldset)
+               354 STORE_NAME              62 (Fieldset)
+               356 IMPORT_FROM             63 (Layout)
+               358 STORE_NAME              63 (Layout)
+               360 IMPORT_FROM             64 (LayoutNode)
+               362 STORE_NAME              64 (LayoutNode)
+               364 POP_TOP
+   
+    31         366 LOAD_CONST               0 (0)
+               368 LOAD_CONST              26 (('PolymorphicModelBase',))
+               370 IMPORT_NAME             65 (polymorphic.base)
+               372 IMPORT_FROM             66 (PolymorphicModelBase)
+               374 STORE_NAME              66 (PolymorphicModelBase)
+               376 POP_TOP
+   
+    32         378 LOAD_CONST               0 (0)
+               380 LOAD_CONST              27 (('PolymorphicManager',))
+               382 IMPORT_NAME             67 (polymorphic.managers)
+               384 IMPORT_FROM             68 (PolymorphicManager)
+               386 STORE_NAME              68 (PolymorphicManager)
+               388 POP_TOP
+   
+    33         390 LOAD_CONST               0 (0)
+               392 LOAD_CONST              28 (('PolymorphicModel',))
+               394 IMPORT_NAME             69 (polymorphic.models)
+               396 IMPORT_FROM             70 (PolymorphicModel)
+               398 STORE_NAME              70 (PolymorphicModel)
+               400 POP_TOP
+   
+    34         402 LOAD_CONST               0 (0)
+               404 LOAD_CONST              29 (('ObjectPermissionsModelAdmin',))
+               406 IMPORT_NAME             71 (rules.contrib.admin)
+               408 IMPORT_FROM             72 (ObjectPermissionsModelAdmin)
+               410 STORE_NAME              72 (ObjectPermissionsModelAdmin)
+               412 POP_TOP
+   
+    36         414 LOAD_CONST               0 (0)
+               416 LOAD_CONST              30 (('CurrentSiteManagerWithoutMigrations', 'PolymorphicCurrentSiteManager', 'SchoolTermRelatedQuerySet'))
+               418 IMPORT_NAME             73 (aleksis.core.managers)
+               420 IMPORT_FROM             74 (CurrentSiteManagerWithoutMigrations)
+               422 STORE_NAME              74 (CurrentSiteManagerWithoutMigrations)
+               424 IMPORT_FROM             75 (PolymorphicCurrentSiteManager)
+               426 STORE_NAME              75 (PolymorphicCurrentSiteManager)
+               428 IMPORT_FROM             76 (SchoolTermRelatedQuerySet)
+               430 STORE_NAME              76 (SchoolTermRelatedQuerySet)
+               432 POP_TOP
+   
+    43         434 PUSH_NULL
+               436 LOAD_BUILD_CLASS
+               438 LOAD_CONST              31 (<code object _ExtensibleModelBase, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 43>)
+               440 MAKE_FUNCTION            0
+               442 LOAD_CONST              32 ('_ExtensibleModelBase')
+               444 LOAD_NAME               23 (models)
+               446 LOAD_ATTR               77 (base)
+               456 LOAD_ATTR               78 (ModelBase)
+               466 PRECALL                  3
+               470 CALL                     3
+               480 STORE_NAME              79 (_ExtensibleModelBase)
+   
+    63         482 LOAD_CONST              33 (<code object _generate_one_to_one_proxy_property, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 63>)
+               484 MAKE_FUNCTION            0
+               486 STORE_NAME              80 (_generate_one_to_one_proxy_property)
+   
+    85         488 PUSH_NULL
+               490 LOAD_BUILD_CLASS
+               492 LOAD_CONST              34 (<code object ExtensibleModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 85>)
+               494 MAKE_FUNCTION            0
+               496 LOAD_CONST              35 ('ExtensibleModel')
+               498 LOAD_NAME               23 (models)
+               500 LOAD_ATTR               81 (Model)
+               510 LOAD_NAME               79 (_ExtensibleModelBase)
+               512 KW_NAMES                36
+               514 PRECALL                  4
+               518 CALL                     4
+               528 STORE_NAME              82 (ExtensibleModel)
+   
+   374         530 PUSH_NULL
+               532 LOAD_BUILD_CLASS
+               534 LOAD_CONST              37 (<code object _ExtensiblePolymorphicModelBase, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 374>)
+               536 MAKE_FUNCTION            0
+               538 LOAD_CONST              38 ('_ExtensiblePolymorphicModelBase')
+               540 LOAD_NAME               79 (_ExtensibleModelBase)
+               542 LOAD_NAME               66 (PolymorphicModelBase)
+               544 PRECALL                  4
+               548 CALL                     4
+               558 STORE_NAME              83 (_ExtensiblePolymorphicModelBase)
+   
+   378         560 PUSH_NULL
+               562 LOAD_BUILD_CLASS
+               564 LOAD_CONST              39 (<code object ExtensiblePolymorphicModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 378>)
+               566 MAKE_FUNCTION            0
+               568 LOAD_CONST              40 ('ExtensiblePolymorphicModel')
+   
+   379         570 LOAD_NAME               82 (ExtensibleModel)
+               572 LOAD_NAME               70 (PolymorphicModel)
+               574 LOAD_NAME               83 (_ExtensiblePolymorphicModelBase)
+   
+   378         576 KW_NAMES                36
+               578 PRECALL                  5
+               582 CALL                     5
+               592 STORE_NAME              84 (ExtensiblePolymorphicModel)
+   
+   390         594 PUSH_NULL
+               596 LOAD_BUILD_CLASS
+               598 LOAD_CONST              41 (<code object PureDjangoModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 390>)
+               600 MAKE_FUNCTION            0
+               602 LOAD_CONST              42 ('PureDjangoModel')
+               604 LOAD_NAME               85 (object)
+               606 PRECALL                  3
+               610 CALL                     3
+               620 STORE_NAME              86 (PureDjangoModel)
+   
+   396         622 PUSH_NULL
+               624 LOAD_BUILD_CLASS
+               626 LOAD_CONST              43 (<code object GlobalPermissionModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 396>)
+               628 MAKE_FUNCTION            0
+               630 LOAD_CONST              44 ('GlobalPermissionModel')
+               632 LOAD_NAME               23 (models)
+               634 LOAD_ATTR               81 (Model)
+               644 PRECALL                  3
+               648 CALL                     3
+               658 STORE_NAME              87 (GlobalPermissionModel)
+   
+   407         660 PUSH_NULL
+               662 LOAD_BUILD_CLASS
+               664 LOAD_CONST              45 (<code object _ExtensibleFormMetaclass, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 407>)
+               666 MAKE_FUNCTION            0
+               668 LOAD_CONST              46 ('_ExtensibleFormMetaclass')
+               670 LOAD_NAME               34 (ModelFormMetaclass)
+               672 PRECALL                  3
+               676 CALL                     3
+               686 STORE_NAME              88 (_ExtensibleFormMetaclass)
+   
+   423         688 PUSH_NULL
+               690 LOAD_BUILD_CLASS
+               692 LOAD_CONST              47 (<code object ExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 423>)
+               694 MAKE_FUNCTION            0
+               696 LOAD_CONST              48 ('ExtensibleForm')
+               698 LOAD_NAME               33 (ModelForm)
+               700 LOAD_NAME               88 (_ExtensibleFormMetaclass)
+               702 KW_NAMES                36
+               704 PRECALL                  4
+               708 CALL                     4
+               718 STORE_NAME              89 (ExtensibleForm)
+   
+   467         720 PUSH_NULL
+               722 LOAD_BUILD_CLASS
+               724 LOAD_CONST              49 (<code object BaseModelAdmin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 467>)
+               726 MAKE_FUNCTION            0
+               728 LOAD_CONST              50 ('BaseModelAdmin')
+               730 LOAD_NAME               55 (GuardedModelAdmin)
+               732 LOAD_NAME               72 (ObjectPermissionsModelAdmin)
+               734 PRECALL                  4
+               738 CALL                     4
+               748 STORE_NAME              90 (BaseModelAdmin)
+   
+   473         750 PUSH_NULL
+               752 LOAD_BUILD_CLASS
+               754 LOAD_CONST              51 (<code object SuccessMessageMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 473>)
+               756 MAKE_FUNCTION            0
+               758 LOAD_CONST              52 ('SuccessMessageMixin')
+               760 LOAD_NAME               48 (ModelFormMixin)
+               762 PRECALL                  3
+               766 CALL                     3
+               776 STORE_NAME              91 (SuccessMessageMixin)
+   
+   482         778 PUSH_NULL
+               780 LOAD_BUILD_CLASS
+               782 LOAD_CONST              53 (<code object SuccessNextMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 482>)
+               784 MAKE_FUNCTION            0
+               786 LOAD_CONST              54 ('SuccessNextMixin')
+               788 LOAD_NAME               15 (RedirectURLMixin)
+               790 PRECALL                  3
+               794 CALL                     3
+               804 STORE_NAME              92 (SuccessNextMixin)
+   
+   489         806 PUSH_NULL
+               808 LOAD_BUILD_CLASS
+               810 LOAD_CONST              55 (<code object AdvancedCreateView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 489>)
+               812 MAKE_FUNCTION            0
+               814 LOAD_CONST              56 ('AdvancedCreateView')
+               816 LOAD_NAME               91 (SuccessMessageMixin)
+               818 LOAD_NAME               44 (CreateView)
+               820 PRECALL                  4
+               824 CALL                     4
+               834 STORE_NAME              93 (AdvancedCreateView)
+   
+   493         836 PUSH_NULL
+               838 LOAD_BUILD_CLASS
+               840 LOAD_CONST              57 (<code object AdvancedEditView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 493>)
+               842 MAKE_FUNCTION            0
+               844 LOAD_CONST              58 ('AdvancedEditView')
+               846 LOAD_NAME               91 (SuccessMessageMixin)
+               848 LOAD_NAME               45 (UpdateView)
+               850 PRECALL                  4
+               854 CALL                     4
+               864 STORE_NAME              94 (AdvancedEditView)
+   
+   497         866 PUSH_NULL
+               868 LOAD_BUILD_CLASS
+               870 LOAD_CONST              59 (<code object AdvancedDeleteView, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 497>)
+               872 MAKE_FUNCTION            0
+               874 LOAD_CONST              60 ('AdvancedDeleteView')
+               876 LOAD_NAME               47 (DeleteView)
+               878 PRECALL                  3
+               882 CALL                     3
+               892 STORE_NAME              95 (AdvancedDeleteView)
+   
+   516         894 PUSH_NULL
+               896 LOAD_BUILD_CLASS
+               898 LOAD_CONST              61 (<code object SchoolTermRelatedExtensibleModel, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 516>)
+               900 MAKE_FUNCTION            0
+               902 LOAD_CONST              62 ('SchoolTermRelatedExtensibleModel')
+               904 LOAD_NAME               82 (ExtensibleModel)
+               906 PRECALL                  3
+               910 CALL                     3
+               920 STORE_NAME              96 (SchoolTermRelatedExtensibleModel)
+   
+   534         922 PUSH_NULL
+               924 LOAD_BUILD_CLASS
+               926 LOAD_CONST              63 (<code object SchoolTermRelatedExtensibleForm, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 534>)
+               928 MAKE_FUNCTION            0
+               930 LOAD_CONST              64 ('SchoolTermRelatedExtensibleForm')
+               932 LOAD_NAME               89 (ExtensibleForm)
+               934 PRECALL                  3
+               938 CALL                     3
+               948 STORE_NAME              97 (SchoolTermRelatedExtensibleForm)
+   
+   551         950 PUSH_NULL
+               952 LOAD_BUILD_CLASS
+               954 LOAD_CONST              65 (<code object PublicFilePreferenceMixin, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 551>)
+               956 MAKE_FUNCTION            0
+               958 LOAD_CONST              66 ('PublicFilePreferenceMixin')
+               960 LOAD_NAME               53 (FilePreference)
+               962 PRECALL                  3
+               966 CALL                     3
+               976 STORE_NAME              98 (PublicFilePreferenceMixin)
+   
+   562         978 PUSH_NULL
+               980 LOAD_BUILD_CLASS
+               982 LOAD_CONST              67 (<code object RegistryObject, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 562>)
+               984 MAKE_FUNCTION            0
+               986 LOAD_CONST              68 ('RegistryObject')
+               988 PRECALL                  2
+               992 CALL                     2
+              1002 STORE_NAME              99 (RegistryObject)
+              1004 LOAD_CONST               1 (None)
+              1006 RETURN_VALUE
    consts
       0
       None
       ('datetime',)
       ('Any', 'Callable', 'ClassVar', 'List', 'Optional', 'Union')
       ('settings',)
       ('messages',)
@@ -511,15 +513,15 @@
       ('CreateView', 'UpdateView')
       ('DeleteView', 'ModelFormMixin')
       ('preferences_settings',)
       ('FilePreference',)
       ('GuardedModelAdmin',)
       ('ObjectPermissionChecker',)
       ('IntegerField', 'JSONFieldMixin')
-      ('Layout', 'LayoutNode')
+      ('Fieldset', 'Layout', 'LayoutNode')
       ('PolymorphicModelBase',)
       ('PolymorphicManager',)
       ('PolymorphicModel',)
       ('ObjectPermissionsModelAdmin',)
       ('CurrentSiteManagerWithoutMigrations', 'PolymorphicCurrentSiteManager', 'SchoolTermRelatedQuerySet')
       code
          argcount  : 0
@@ -2892,22 +2894,34 @@
                       60 RETURN_VALUE
          consts
             'ExtensibleForm'
             'Base model for extensible forms.\n\n    This mixin adds functionality which allows\n    - apps to add layout nodes to the layout used by django-material\n\n    :Add layout nodes:\n\n    .. code-block:: python\n\n        from material import Fieldset\n\n        from aleksis.core.forms import ExampleForm\n\n        node = Fieldset("field_name")\n        ExampleForm.add_node_to_layout(node)\n\n    '
             'node'
             code
                argcount  : 2
-               nlocals   : 2
-               stacksize : 3
+               nlocals   : 6
+               stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab01000000000000000001007405000000
                   000000000000007c006a0000000000000000008e007c005f030000000000
-                  00000064015300
+                  0000007c0167017d027c0272b17c02a00400000000000000000000000000
+                  00000000000000a6000000ab0000000000000000007d03740b0000000000
+                  00000000007c03740c00000000000000000000a6020000ab020000000000
+                  000000720b7c027c016a0700000000000000007a0d00007d026e79740b00
+                  0000000000000000007c03741000000000000000000000a6020000ab0200
+                  0000000000000072027c036e067c036a0900000000000000007d04741500
+                  0000000000000000007c006a0b00000000000000006a0c00000000000000
+                  007c046701a6020000ab0200000000000000007c04190000000000000000
+                  007d057c006a0b00000000000000006a0d0000000000000000a001000000
+                  00000000000000000000000000000000007c04a6010000ab010000000000
+                  00000001007c057c006a0e00000000000000007c043c000000741f000000
+                  000000000000007c007c047c05a6030000ab03000000000000000001007c
+                  02b0af6401530064015300
                442           0 RESUME                   0
                
                449           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (base_layout)
                             14 LOAD_METHOD              1 (append)
                             36 LOAD_FAST                1 (node)
                             38 PRECALL                  1
@@ -2916,27 +2930,107 @@
                
                450          54 LOAD_GLOBAL              5 (NULL + Layout)
                             66 LOAD_FAST                0 (cls)
                             68 LOAD_ATTR                0 (base_layout)
                             78 CALL_FUNCTION_EX         0
                             80 LOAD_FAST                0 (cls)
                             82 STORE_ATTR               3 (layout)
-                            92 LOAD_CONST               1 (None)
-                            94 RETURN_VALUE
+               
+               452          92 LOAD_FAST                1 (node)
+                            94 BUILD_LIST               1
+                            96 STORE_FAST               2 (visit_nodes)
+               
+               453          98 LOAD_FAST                2 (visit_nodes)
+                           100 POP_JUMP_FORWARD_IF_FALSE   177 (to 456)
+               
+               454     >>  102 LOAD_FAST                2 (visit_nodes)
+                           104 LOAD_METHOD              4 (pop)
+                           126 PRECALL                  0
+                           130 CALL                     0
+                           140 STORE_FAST               3 (current_node)
+               
+               455         142 LOAD_GLOBAL             11 (NULL + isinstance)
+                           154 LOAD_FAST                3 (current_node)
+                           156 LOAD_GLOBAL             12 (Fieldset)
+                           168 PRECALL                  2
+                           172 CALL                     2
+                           182 POP_JUMP_FORWARD_IF_FALSE    11 (to 206)
+               
+               456         184 LOAD_FAST                2 (visit_nodes)
+                           186 LOAD_FAST                1 (node)
+                           188 LOAD_ATTR                7 (elements)
+                           198 BINARY_OP               13 (+=)
+                           202 STORE_FAST               2 (visit_nodes)
+                           204 JUMP_FORWARD           121 (to 448)
+               
+               459     >>  206 LOAD_GLOBAL             11 (NULL + isinstance)
+                           218 LOAD_FAST                3 (current_node)
+                           220 LOAD_GLOBAL             16 (str)
+                           232 PRECALL                  2
+                           236 CALL                     2
+                           246 POP_JUMP_FORWARD_IF_FALSE     2 (to 252)
+                           248 LOAD_FAST                3 (current_node)
+                           250 JUMP_FORWARD             6 (to 264)
+                       >>  252 LOAD_FAST                3 (current_node)
+                           254 LOAD_ATTR                9 (field_name)
+               
+               458     >>  264 STORE_FAST               4 (field_name)
+               
+               461         266 LOAD_GLOBAL             21 (NULL + fields_for_model)
+                           278 LOAD_FAST                0 (cls)
+                           280 LOAD_ATTR               11 (_meta)
+                           290 LOAD_ATTR               12 (model)
+                           300 LOAD_FAST                4 (field_name)
+                           302 BUILD_LIST               1
+                           304 PRECALL                  2
+                           308 CALL                     2
+                           318 LOAD_FAST                4 (field_name)
+                           320 BINARY_SUBSCR
+                           330 STORE_FAST               5 (field)
+               
+               462         332 LOAD_FAST                0 (cls)
+                           334 LOAD_ATTR               11 (_meta)
+                           344 LOAD_ATTR               13 (fields)
+                           354 LOAD_METHOD              1 (append)
+                           376 LOAD_FAST                4 (field_name)
+                           378 PRECALL                  1
+                           382 CALL                     1
+                           392 POP_TOP
+               
+               463         394 LOAD_FAST                5 (field)
+                           396 LOAD_FAST                0 (cls)
+                           398 LOAD_ATTR               14 (base_fields)
+                           408 LOAD_FAST                4 (field_name)
+                           410 STORE_SUBSCR
+               
+               464         414 LOAD_GLOBAL             31 (NULL + setattr)
+                           426 LOAD_FAST                0 (cls)
+                           428 LOAD_FAST                4 (field_name)
+                           430 LOAD_FAST                5 (field)
+                           432 PRECALL                  3
+                           436 CALL                     3
+                           446 POP_TOP
+               
+               453     >>  448 LOAD_FAST                2 (visit_nodes)
+                           450 POP_JUMP_BACKWARD_IF_TRUE   175 (to 102)
+                           452 LOAD_CONST               1 (None)
+                           454 RETURN_VALUE
+                       >>  456 LOAD_CONST               1 (None)
+                           458 RETURN_VALUE
                consts
                   'Add a node to `layout` attribute.\n\n        :param node: django-material layout node (Fieldset, Row etc.)\n        :type node: LayoutNode\n        '
                   None
-               names      ('base_layout', 'append', 'Layout', 'layout')
-               varnames   ('cls', 'node')
+               names      ('base_layout', 'append', 'Layout', 'layout', 'pop', 'isinstance', 'Fieldset', 'elements', 'str', 'field_name', 'fields_for_model', '_meta', 'model', 'fields', 'base_fields', 'setattr')
+               varnames   ('cls', 'node', 'visit_nodes', 'current_node', 'field_name', 'field')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'add_node_to_layout'
                firstlineno 442
-               lnotab 0x02073401
+               lnotab 0x0207340126020601040128012a0116033aff020342013e01140122f5
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'classmethod', 'Union', 'LayoutNode', 'str', 'add_node_to_layout')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'ExtensibleForm'
@@ -2945,73 +3039,73 @@
       'ExtensibleForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025300
-         453           0 RESUME                   0
+         467           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('BaseModelAdmin')
                        8 STORE_NAME               2 (__qualname__)
          
-         454          10 LOAD_CONST               1 ('A base class for ModelAdmin combining django-guardian and rules.')
+         468          10 LOAD_CONST               1 ('A base class for ModelAdmin combining django-guardian and rules.')
                       12 STORE_NAME               3 (__doc__)
          
-         456          14 LOAD_CONST               2 (None)
+         470          14 LOAD_CONST               2 (None)
                       16 RETURN_VALUE
          consts
             'BaseModelAdmin'
             'A base class for ModelAdmin combining django-guardian and rules.'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'BaseModelAdmin'
-         firstlineno 453
+         firstlineno 467
          lnotab 0x0a010402
       'BaseModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a02550064015a036504650519000000000000
             000000650664023c00000064036507640465086604880066016405840c5a
             09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
-         459           2 RESUME                   0
+         473           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('SuccessMessageMixin')
                       10 STORE_NAME               2 (__qualname__)
                       12 SETUP_ANNOTATIONS
          
-         460          14 LOAD_CONST               1 (None)
+         474          14 LOAD_CONST               1 (None)
                       16 STORE_NAME               3 (success_message)
                       18 LOAD_NAME                4 (Optional)
                       20 LOAD_NAME                5 (str)
                       22 BINARY_SUBSCR
                       32 LOAD_NAME                6 (__annotations__)
                       34 LOAD_CONST               2 ('success_message')
                       36 STORE_SUBSCR
          
-         462          40 LOAD_CONST               3 ('form')
+         476          40 LOAD_CONST               3 ('form')
                       42 LOAD_NAME                7 (BaseForm)
                       44 LOAD_CONST               4 ('return')
                       46 LOAD_NAME                8 (HttpResponse)
                       48 BUILD_TUPLE              4
                       50 LOAD_CLOSURE             0 (__class__)
                       52 BUILD_TUPLE              1
-                      54 LOAD_CONST               5 (<code object form_valid, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 462>)
+                      54 LOAD_CONST               5 (<code object form_valid, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 476>)
                       56 MAKE_FUNCTION           12 (annotations, closure)
                       58 STORE_NAME               9 (form_valid)
                       60 LOAD_CLOSURE             0 (__class__)
                       62 COPY                     1
                       64 STORE_NAME              10 (__classcell__)
                       66 RETURN_VALUE
          consts
@@ -3029,31 +3123,31 @@
                   0x950197007c006a000000000000000000721f7403000000000000000000
                   006a0200000000000000007c006a0300000000000000007c006a00000000
                   0000000000a6020000ab0200000000000000000100740900000000000000
                   000000a6000000ab000000000000000000a0050000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000005300
                              0 COPY_FREE_VARS           1
                
-               462           2 RESUME                   0
+               476           2 RESUME                   0
                
-               463           4 LOAD_FAST                0 (self)
+               477           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (success_message)
                             16 POP_JUMP_FORWARD_IF_FALSE    31 (to 80)
                
-               464          18 LOAD_GLOBAL              3 (NULL + messages)
+               478          18 LOAD_GLOBAL              3 (NULL + messages)
                             30 LOAD_ATTR                2 (success)
                             40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (request)
                             52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                0 (success_message)
                             64 PRECALL                  2
                             68 CALL                     2
                             78 POP_TOP
                
-               465     >>   80 LOAD_GLOBAL              9 (NULL + super)
+               479     >>   80 LOAD_GLOBAL              9 (NULL + super)
                             92 PRECALL                  0
                             96 CALL                     0
                            106 LOAD_METHOD              5 (form_valid)
                            128 LOAD_FAST                1 (form)
                            130 PRECALL                  1
                            134 CALL                     1
                            144 RETURN_VALUE
@@ -3061,50 +3155,50 @@
                   None
                names      ('success_message', 'messages', 'success', 'request', 'super', 'form_valid')
                varnames   ('self', 'form')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'form_valid'
-               firstlineno 462
+               firstlineno 476
                lnotab 0x04010e013e01
          names      ('__name__', '__module__', '__qualname__', 'success_message', 'Optional', 'str', '__annotations__', 'BaseForm', 'HttpResponse', 'form_valid', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'SuccessMessageMixin'
-         firstlineno 459
+         firstlineno 473
          lnotab 0x0e011a02
       'SuccessMessageMixin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0364026504660288006601640384
             0c5a05880078015a065300
                        0 MAKE_CELL                0 (__class__)
          
-         468           2 RESUME                   0
+         482           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('SuccessNextMixin')
                       10 STORE_NAME               2 (__qualname__)
          
-         469          12 LOAD_CONST               1 ('next')
+         483          12 LOAD_CONST               1 ('next')
                       14 STORE_NAME               3 (redirect_field_name)
          
-         471          16 LOAD_CONST               2 ('return')
+         485          16 LOAD_CONST               2 ('return')
                       18 LOAD_NAME                4 (str)
                       20 BUILD_TUPLE              2
                       22 LOAD_CLOSURE             0 (__class__)
                       24 BUILD_TUPLE              1
-                      26 LOAD_CONST               3 (<code object get_success_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 471>)
+                      26 LOAD_CONST               3 (<code object get_success_url, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 485>)
                       28 MAKE_FUNCTION           12 (annotations, closure)
                       30 STORE_NAME               5 (get_success_url)
                       32 LOAD_CLOSURE             0 (__class__)
                       34 COPY                     1
                       36 STORE_NAME               6 (__classcell__)
                       38 RETURN_VALUE
          consts
@@ -3119,17 +3213,17 @@
                code
                   0x950197007401000000000000000000006a0100000000000000007c00a6
                   010000ab010000000000000000701f740500000000000000000000a60000
                   00ab000000000000000000a0030000000000000000000000000000000000
                   000000a6000000ab0000000000000000005300
                              0 COPY_FREE_VARS           1
                
-               471           2 RESUME                   0
+               485           2 RESUME                   0
                
-               472           4 LOAD_GLOBAL              1 (NULL + LoginView)
+               486           4 LOAD_GLOBAL              1 (NULL + LoginView)
                             16 LOAD_ATTR                1 (get_redirect_url)
                             26 LOAD_FAST                0 (self)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 JUMP_IF_TRUE_OR_POP     31 (to 106)
                             44 LOAD_GLOBAL              5 (NULL + super)
                             56 PRECALL                  0
@@ -3142,110 +3236,110 @@
                   None
                names      ('LoginView', 'get_redirect_url', 'super', 'get_success_url')
                varnames   ('self',)
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_success_url'
-               firstlineno 471
+               firstlineno 485
                lnotab 0x0401
          names      ('__name__', '__module__', '__qualname__', 'redirect_field_name', 'str', 'get_success_url', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'SuccessNextMixin'
-         firstlineno 468
+         firstlineno 482
          lnotab 0x0c010402
       'SuccessNextMixin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015300
-         475           0 RESUME                   0
+         489           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdvancedCreateView')
                        8 STORE_NAME               2 (__qualname__)
          
-         476          10 LOAD_CONST               1 (None)
+         490          10 LOAD_CONST               1 (None)
                       12 RETURN_VALUE
          consts
             'AdvancedCreateView'
             None
          names      ('__name__', '__module__', '__qualname__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'AdvancedCreateView'
-         firstlineno 475
+         firstlineno 489
          lnotab 0x0a01
       'AdvancedCreateView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015300
-         479           0 RESUME                   0
+         493           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdvancedEditView')
                        8 STORE_NAME               2 (__qualname__)
          
-         480          10 LOAD_CONST               1 (None)
+         494          10 LOAD_CONST               1 (None)
                       12 RETURN_VALUE
          consts
             'AdvancedEditView'
             None
          names      ('__name__', '__module__', '__qualname__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'AdvancedEditView'
-         firstlineno 479
+         firstlineno 493
          lnotab 0x0a01
       'AdvancedEditView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a02550064015a0364025a0465056506190000
             00000000000000650764033c00000088006601640484085a08880078015a
             095300
                        0 MAKE_CELL                0 (__class__)
          
-         483           2 RESUME                   0
+         497           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdvancedDeleteView')
                       10 STORE_NAME               2 (__qualname__)
                       12 SETUP_ANNOTATIONS
          
-         484          14 LOAD_CONST               1 ('Common confirm view for deleting.\n\n    .. warning ::\n\n        Using this view, objects are deleted permanently after confirming.\n        We recommend to include the mixin :class:`reversion.views.RevisionMixin`\n        from `django-reversion` to enable soft-delete.\n    ')
+         498          14 LOAD_CONST               1 ('Common confirm view for deleting.\n\n    .. warning ::\n\n        Using this view, objects are deleted permanently after confirming.\n        We recommend to include the mixin :class:`reversion.views.RevisionMixin`\n        from `django-reversion` to enable soft-delete.\n    ')
                       16 STORE_NAME               3 (__doc__)
          
-         493          18 LOAD_CONST               2 (None)
+         507          18 LOAD_CONST               2 (None)
                       20 STORE_NAME               4 (success_message)
                       22 LOAD_NAME                5 (Optional)
                       24 LOAD_NAME                6 (str)
                       26 BINARY_SUBSCR
                       36 LOAD_NAME                7 (__annotations__)
                       38 LOAD_CONST               3 ('success_message')
                       40 STORE_SUBSCR
          
-         495          44 LOAD_CLOSURE             0 (__class__)
+         509          44 LOAD_CLOSURE             0 (__class__)
                       46 BUILD_TUPLE              1
-                      48 LOAD_CONST               4 (<code object form_valid, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 495>)
+                      48 LOAD_CONST               4 (<code object form_valid, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 509>)
                       50 MAKE_FUNCTION            8 (closure)
                       52 STORE_NAME               8 (form_valid)
                       54 LOAD_CLOSURE             0 (__class__)
                       56 COPY                     1
                       58 STORE_NAME               9 (__classcell__)
                       60 RETURN_VALUE
          consts
@@ -3263,121 +3357,121 @@
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   0100000000000000007d027c006a020000000000000000721f7407000000
                   000000000000006a0400000000000000007c006a0500000000000000007c
                   006a020000000000000000a6020000ab02000000000000000001007c0253
                   00
                              0 COPY_FREE_VARS           1
                
-               495           2 RESUME                   0
+               509           2 RESUME                   0
                
-               496           4 LOAD_GLOBAL              1 (NULL + super)
+               510           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (form_valid)
                             52 LOAD_FAST                1 (form)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 STORE_FAST               2 (r)
                
-               497          70 LOAD_FAST                0 (self)
+               511          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                2 (success_message)
                             82 POP_JUMP_FORWARD_IF_FALSE    31 (to 146)
                
-               498          84 LOAD_GLOBAL              7 (NULL + messages)
+               512          84 LOAD_GLOBAL              7 (NULL + messages)
                             96 LOAD_ATTR                4 (success)
                            106 LOAD_FAST                0 (self)
                            108 LOAD_ATTR                5 (request)
                            118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                2 (success_message)
                            130 PRECALL                  2
                            134 CALL                     2
                            144 POP_TOP
                
-               499     >>  146 LOAD_FAST                2 (r)
+               513     >>  146 LOAD_FAST                2 (r)
                            148 RETURN_VALUE
                consts
                   None
                names      ('super', 'form_valid', 'success_message', 'messages', 'success', 'request')
                varnames   ('self', 'form', 'r')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'form_valid'
-               firstlineno 495
+               firstlineno 509
                lnotab 0x040142010e013e01
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'success_message', 'Optional', 'str', '__annotations__', 'form_valid', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'AdvancedDeleteView'
-         firstlineno 483
+         firstlineno 497
          lnotab 0x0e0104091a02
       'AdvancedDeleteView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 8
          flags     : 0
          code
             0x970065005a0164005a0264015a030200020065046a0500000000000000
             006506a6010000ab010000000000000000a6000000ab0000000000000000
             005a07020065086a090000000000000000640265086a0a00000000000000
             0064030200650b6404a6010000ab01000000000000000064056405ac06a6
             060000ab0600000000000000005a0c02004700640784006408a6020000ab
             0200000000000000005a0d64095300
-         502           0 RESUME                   0
+         516           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SchoolTermRelatedExtensibleModel')
                        8 STORE_NAME               2 (__qualname__)
          
-         503          10 LOAD_CONST               1 ('Add relation to school term.')
+         517          10 LOAD_CONST               1 ('Add relation to school term.')
                       12 STORE_NAME               3 (__doc__)
          
-         505          14 PUSH_NULL
+         519          14 PUSH_NULL
                       16 PUSH_NULL
                       18 LOAD_NAME                4 (CurrentSiteManagerWithoutMigrations)
                       20 LOAD_ATTR                5 (from_queryset)
                       30 LOAD_NAME                6 (SchoolTermRelatedQuerySet)
                       32 PRECALL                  1
                       36 CALL                     1
                       46 PRECALL                  0
                       50 CALL                     0
                       60 STORE_NAME               7 (objects)
          
-         507          62 PUSH_NULL
+         521          62 PUSH_NULL
                       64 LOAD_NAME                8 (models)
                       66 LOAD_ATTR                9 (ForeignKey)
          
-         508          76 LOAD_CONST               2 ('core.SchoolTerm')
+         522          76 LOAD_CONST               2 ('core.SchoolTerm')
          
-         509          78 LOAD_NAME                8 (models)
+         523          78 LOAD_NAME                8 (models)
                       80 LOAD_ATTR               10 (CASCADE)
          
-         510          90 LOAD_CONST               3 ('+')
+         524          90 LOAD_CONST               3 ('+')
          
-         511          92 PUSH_NULL
+         525          92 PUSH_NULL
                       94 LOAD_NAME               11 (_)
                       96 LOAD_CONST               4 ('Linked school term')
                       98 PRECALL                  1
                      102 CALL                     1
          
-         512         112 LOAD_CONST               5 (True)
+         526         112 LOAD_CONST               5 (True)
          
-         513         114 LOAD_CONST               5 (True)
+         527         114 LOAD_CONST               5 (True)
          
-         507         116 KW_NAMES                 6
+         521         116 KW_NAMES                 6
                      118 PRECALL                  6
                      122 CALL                     6
                      132 STORE_NAME              12 (school_term)
          
-         516         134 PUSH_NULL
+         530         134 PUSH_NULL
                      136 LOAD_BUILD_CLASS
-                     138 LOAD_CONST               7 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 516>)
+                     138 LOAD_CONST               7 (<code object Meta, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 530>)
                      140 MAKE_FUNCTION            0
                      142 LOAD_CONST               8 ('Meta')
                      144 PRECALL                  2
                      148 CALL                     2
                      158 STORE_NAME              13 (Meta)
                      160 LOAD_CONST               9 (None)
                      162 RETURN_VALUE
@@ -3391,69 +3485,69 @@
             ('on_delete', 'related_name', 'verbose_name', 'blank', 'null')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               516           0 RESUME                   0
+               530           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('SchoolTermRelatedExtensibleModel.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               517          10 LOAD_CONST               1 (True)
+               531          10 LOAD_CONST               1 (True)
                             12 STORE_NAME               3 (abstract)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'SchoolTermRelatedExtensibleModel.Meta'
                   True
                   None
                names      ('__name__', '__module__', '__qualname__', 'abstract')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'Meta'
-               firstlineno 516
+               firstlineno 530
                lnotab 0x0a01
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'CurrentSiteManagerWithoutMigrations', 'from_queryset', 'SchoolTermRelatedQuerySet', 'objects', 'models', 'ForeignKey', 'CASCADE', '_', 'school_term', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'SchoolTermRelatedExtensibleModel'
-         firstlineno 502
+         firstlineno 516
          lnotab 0x0a01040230020e0102010c0102011401020102fa1209
       'SchoolTermRelatedExtensibleModel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0388006601640284085a04880078
             015a055300
                        0 MAKE_CELL                0 (__class__)
          
-         520           2 RESUME                   0
+         534           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('SchoolTermRelatedExtensibleForm')
                       10 STORE_NAME               2 (__qualname__)
          
-         521          12 LOAD_CONST               1 ("Extensible form for school term related data.\n\n    .. warning::\n        This doesn't automatically include the field `school_term` in `fields` or `layout`,\n        it just sets an initial value.\n    ")
+         535          12 LOAD_CONST               1 ("Extensible form for school term related data.\n\n    .. warning::\n        This doesn't automatically include the field `school_term` in `fields` or `layout`,\n        it just sets an initial value.\n    ")
                       14 STORE_NAME               3 (__doc__)
          
-         528          16 LOAD_CLOSURE             0 (__class__)
+         542          16 LOAD_CLOSURE             0 (__class__)
                       18 BUILD_TUPLE              1
-                      20 LOAD_CONST               2 (<code object __init__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 528>)
+                      20 LOAD_CONST               2 (<code object __init__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 542>)
                       22 MAKE_FUNCTION            8 (closure)
                       24 STORE_NAME               4 (__init__)
                       26 LOAD_CLOSURE             0 (__class__)
                       28 COPY                     1
                       30 STORE_NAME               5 (__classcell__)
                       32 RETURN_VALUE
          consts
@@ -3467,37 +3561,37 @@
                code
                   0x95019700640164026c006d017d03010064037c027601720c64047c036a
                   02000000000000000069017c0264053c0000000200740700000000000000
                   000000a6000000ab0000000000000000006a0400000000000000007c0169
                   007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               528           2 RESUME                   0
+               542           2 RESUME                   0
                
-               529           4 LOAD_CONST               1 (0)
+               543           4 LOAD_CONST               1 (0)
                              6 LOAD_CONST               2 (('SchoolTerm',))
                              8 IMPORT_NAME              0 (aleksis.core.models)
                             10 IMPORT_FROM              1 (SchoolTerm)
                             12 STORE_FAST               3 (SchoolTerm)
                             14 POP_TOP
                
-               531          16 LOAD_CONST               3 ('instance')
+               545          16 LOAD_CONST               3 ('instance')
                             18 LOAD_FAST                2 (kwargs)
                             20 CONTAINS_OP              1
                             22 POP_JUMP_FORWARD_IF_FALSE    12 (to 48)
                
-               532          24 LOAD_CONST               4 ('school_term')
+               546          24 LOAD_CONST               4 ('school_term')
                             26 LOAD_FAST                3 (SchoolTerm)
                             28 LOAD_ATTR                2 (current)
                             38 BUILD_MAP                1
                             40 LOAD_FAST                2 (kwargs)
                             42 LOAD_CONST               5 ('initial')
                             44 STORE_SUBSCR
                
-               534     >>   48 PUSH_NULL
+               548     >>   48 PUSH_NULL
                             50 LOAD_GLOBAL              7 (NULL + super)
                             62 PRECALL                  0
                             66 CALL                     0
                             76 LOAD_ATTR                4 (__init__)
                             86 LOAD_FAST                1 (args)
                             88 BUILD_MAP                0
                             90 LOAD_FAST                2 (kwargs)
@@ -3515,44 +3609,44 @@
                   'initial'
                names      ('aleksis.core.models', 'SchoolTerm', 'current', 'super', '__init__')
                varnames   ('self', 'args', 'kwargs', 'SchoolTerm')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       '__init__'
-               firstlineno 528
+               firstlineno 542
                lnotab 0x04010c0208011802
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'SchoolTermRelatedExtensibleForm'
-         firstlineno 520
+         firstlineno 534
          lnotab 0x0c010407
       'SchoolTermRelatedExtensibleForm'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0364025a04640384005a0564045300
-         537           0 RESUME                   0
+         551           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PublicFilePreferenceMixin')
                        8 STORE_NAME               2 (__qualname__)
          
-         538          10 LOAD_CONST               1 ('Uploads a file to the public namespace.')
+         552          10 LOAD_CONST               1 ('Uploads a file to the public namespace.')
                       12 STORE_NAME               3 (__doc__)
          
-         540          14 LOAD_CONST               2 ('public')
+         554          14 LOAD_CONST               2 ('public')
                       16 STORE_NAME               4 (upload_path)
          
-         542          18 LOAD_CONST               3 (<code object get_upload_path, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 542>)
+         556          18 LOAD_CONST               3 (<code object get_upload_path, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 556>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get_upload_path)
                       24 LOAD_CONST               4 (None)
                       26 RETURN_VALUE
          consts
             'PublicFilePreferenceMixin'
             'Uploads a file to the public namespace.'
@@ -3564,50 +3658,50 @@
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c006a03000000000000000074
                   08000000000000000000006a0500000000000000007c00a0060000000000
                   000000000000000000000000000000a6000000ab000000000000000000a6
                   030000ab0300000000000000005300
-               542           0 RESUME                   0
+               556           0 RESUME                   0
                
-               543           2 LOAD_GLOBAL              0 (os)
+               557           2 LOAD_GLOBAL              0 (os)
                             14 LOAD_ATTR                1 (path)
                             24 LOAD_METHOD              2 (join)
                
-               544          46 LOAD_FAST                0 (self)
+               558          46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (upload_path)
                             58 LOAD_GLOBAL              8 (preferences_settings)
                             70 LOAD_ATTR                5 (FILE_PREFERENCE_UPLOAD_DIR)
                             80 LOAD_FAST                0 (self)
                             82 LOAD_METHOD              6 (identifier)
                            104 PRECALL                  0
                            108 CALL                     0
                
-               543         118 PRECALL                  3
+               557         118 PRECALL                  3
                            122 CALL                     3
                            132 RETURN_VALUE
                consts
                   None
                names      ('os', 'path', 'join', 'upload_path', 'preferences_settings', 'FILE_PREFERENCE_UPLOAD_DIR', 'identifier')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_upload_path'
-               firstlineno 542
+               firstlineno 556
                lnotab 0x02012c0148ff
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'upload_path', 'get_upload_path')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'PublicFilePreferenceMixin'
-         firstlineno 537
+         firstlineno 551
          lnotab 0x0a0104020402
       'PublicFilePreferenceMixin'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
@@ -3615,91 +3709,91 @@
             0x970065005a0164005a02550064015a0364025a04650565066507650864
             006602190000000000000000001900000000000000000019000000000000
             000000650964033c00000064045a0a650565081900000000000000000065
             0964053c000000640684005a0b650c64078400a6000000ab000000000000
             0000005a0d650e64088400a6000000ab0000000000000000005a0f650e64
             098400a6000000ab0000000000000000005a10650c640a8400a6000000ab
             0000000000000000005a1164025300
-         548           0 RESUME                   0
+         562           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('RegistryObject')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         549          12 LOAD_CONST               1 ('Generic registry to allow registration of subclasses over all apps.')
+         563          12 LOAD_CONST               1 ('Generic registry to allow registration of subclasses over all apps.')
                       14 STORE_NAME               3 (__doc__)
          
-         551          16 LOAD_CONST               2 (None)
+         565          16 LOAD_CONST               2 (None)
                       18 STORE_NAME               4 (_registry)
                       20 LOAD_NAME                5 (ClassVar)
                       22 LOAD_NAME                6 (Optional)
                       24 LOAD_NAME                7 (dict)
                       26 LOAD_NAME                8 (str)
                       28 LOAD_CONST               0 ('RegistryObject')
                       30 BUILD_TUPLE              2
                       32 BINARY_SUBSCR
                       42 BINARY_SUBSCR
                       52 BINARY_SUBSCR
                       62 LOAD_NAME                9 (__annotations__)
                       64 LOAD_CONST               3 ('_registry')
                       66 STORE_SUBSCR
          
-         552          70 LOAD_CONST               4 ('')
+         566          70 LOAD_CONST               4 ('')
                       72 STORE_NAME              10 (name)
                       74 LOAD_NAME                5 (ClassVar)
                       76 LOAD_NAME                8 (str)
                       78 BINARY_SUBSCR
                       88 LOAD_NAME                9 (__annotations__)
                       90 LOAD_CONST               5 ('name')
                       92 STORE_SUBSCR
          
-         554          96 LOAD_CONST               6 (<code object __init_subclass__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 554>)
+         568          96 LOAD_CONST               6 (<code object __init_subclass__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 568>)
                       98 MAKE_FUNCTION            0
                      100 STORE_NAME              11 (__init_subclass__)
          
-         562         102 LOAD_NAME               12 (classmethod)
+         576         102 LOAD_NAME               12 (classmethod)
          
-         563         104 LOAD_CONST               7 (<code object _register, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 562>)
+         577         104 LOAD_CONST               7 (<code object _register, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 576>)
                      106 MAKE_FUNCTION            0
          
-         562         108 PRECALL                  0
+         576         108 PRECALL                  0
                      112 CALL                     0
          
-         563         122 STORE_NAME              13 (_register)
+         577         122 STORE_NAME              13 (_register)
          
-         567         124 LOAD_NAME               14 (classproperty)
+         581         124 LOAD_NAME               14 (classproperty)
          
-         568         126 LOAD_CONST               8 (<code object registered_objects_dict, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 567>)
+         582         126 LOAD_CONST               8 (<code object registered_objects_dict, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 581>)
                      128 MAKE_FUNCTION            0
          
-         567         130 PRECALL                  0
+         581         130 PRECALL                  0
                      134 CALL                     0
          
-         568         144 STORE_NAME              15 (registered_objects_dict)
+         582         144 STORE_NAME              15 (registered_objects_dict)
          
-         571         146 LOAD_NAME               14 (classproperty)
+         585         146 LOAD_NAME               14 (classproperty)
          
-         572         148 LOAD_CONST               9 (<code object registered_objects_list, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 571>)
+         586         148 LOAD_CONST               9 (<code object registered_objects_list, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 585>)
                      150 MAKE_FUNCTION            0
          
-         571         152 PRECALL                  0
+         585         152 PRECALL                  0
                      156 CALL                     0
          
-         572         166 STORE_NAME              16 (registered_objects_list)
+         586         166 STORE_NAME              16 (registered_objects_list)
          
-         575         168 LOAD_NAME               12 (classmethod)
+         589         168 LOAD_NAME               12 (classmethod)
          
-         576         170 LOAD_CONST              10 (<code object get_object_by_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 575>)
+         590         170 LOAD_CONST              10 (<code object get_object_by_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py", line 589>)
                      172 MAKE_FUNCTION            0
          
-         575         174 PRECALL                  0
+         589         174 PRECALL                  0
                      178 CALL                     0
          
-         576         188 STORE_NAME              17 (get_object_by_name)
+         590         188 STORE_NAME              17 (get_object_by_name)
                      190 LOAD_CONST               2 (None)
                      192 RETURN_VALUE
          consts
             'RegistryObject'
             'Generic registry to allow registration of subclasses over all apps.'
             None
             '_registry'
@@ -3712,40 +3806,40 @@
                flags     : 3
                code
                   0x97007401000000000000000000007c0064016400a6030000ab03000000
                   0000000000800969007c005f010000000000000000640053007c006a0200
                   00000000000000730c7c006a0300000000000000007c005f020000000000
                   0000007c00a0040000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               554           0 RESUME                   0
+               568           0 RESUME                   0
                
-               555           2 LOAD_GLOBAL              1 (NULL + getattr)
+               569           2 LOAD_GLOBAL              1 (NULL + getattr)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_CONST               1 ('_registry')
                             18 LOAD_CONST               0 (None)
                             20 PRECALL                  3
                             24 CALL                     3
                             34 POP_JUMP_FORWARD_IF_NOT_NONE     9 (to 54)
                
-               556          36 BUILD_MAP                0
+               570          36 BUILD_MAP                0
                             38 LOAD_FAST                0 (cls)
                             40 STORE_ATTR               1 (_registry)
                             50 LOAD_CONST               0 (None)
                             52 RETURN_VALUE
                
-               558     >>   54 LOAD_FAST                0 (cls)
+               572     >>   54 LOAD_FAST                0 (cls)
                             56 LOAD_ATTR                2 (name)
                             66 POP_JUMP_FORWARD_IF_TRUE    12 (to 92)
                
-               559          68 LOAD_FAST                0 (cls)
+               573          68 LOAD_FAST                0 (cls)
                             70 LOAD_ATTR                3 (__name__)
                             80 LOAD_FAST                0 (cls)
                             82 STORE_ATTR               2 (name)
                
-               560     >>   92 LOAD_FAST                0 (cls)
+               574     >>   92 LOAD_FAST                0 (cls)
                             94 LOAD_METHOD              4 (_register)
                            116 PRECALL                  0
                            120 CALL                     0
                            130 POP_TOP
                            132 LOAD_CONST               0 (None)
                            134 RETURN_VALUE
                consts
@@ -3753,93 +3847,93 @@
                   '_registry'
                names      ('getattr', '_registry', 'name', '__name__', '_register')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       '__init_subclass__'
-               firstlineno 554
+               firstlineno 568
                lnotab 0x0201220112020e011801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000721f7c006a0000000000000000007c
                   006a010000000000000000760172137c007c006a0100000000000000007c
                   006a0000000000000000003c000000640053006400530064005300
-               562           0 RESUME                   0
+               576           0 RESUME                   0
                
-               564           2 LOAD_FAST                0 (cls)
+               578           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (name)
                             14 POP_JUMP_FORWARD_IF_FALSE    31 (to 78)
                             16 LOAD_FAST                0 (cls)
                             18 LOAD_ATTR                0 (name)
                             28 LOAD_FAST                0 (cls)
                             30 LOAD_ATTR                1 (_registry)
                             40 CONTAINS_OP              1
                             42 POP_JUMP_FORWARD_IF_FALSE    19 (to 82)
                
-               565          44 LOAD_FAST                0 (cls)
+               579          44 LOAD_FAST                0 (cls)
                             46 LOAD_FAST                0 (cls)
                             48 LOAD_ATTR                1 (_registry)
                             58 LOAD_FAST                0 (cls)
                             60 LOAD_ATTR                0 (name)
                             70 STORE_SUBSCR
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                
-               564     >>   78 LOAD_CONST               0 (None)
+               578     >>   78 LOAD_CONST               0 (None)
                             80 RETURN_VALUE
                        >>   82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                names      ('name', '_registry')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       '_register'
-               firstlineno 562
+               firstlineno 576
                lnotab 0x02022a0122ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               567           0 RESUME                   0
+               581           0 RESUME                   0
                
-               569           2 LOAD_FAST                0 (cls)
+               583           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (_registry)
                             14 RETURN_VALUE
                consts
                   None
                names      ('_registry',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'registered_objects_dict'
-               firstlineno 567
+               firstlineno 581
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   000000a6010000ab0100000000000000005300
-               571           0 RESUME                   0
+               585           0 RESUME                   0
                
-               573           2 LOAD_GLOBAL              1 (NULL + list)
+               587           2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_ATTR                1 (_registry)
                             26 LOAD_METHOD              2 (values)
                             48 PRECALL                  0
                             52 CALL                     0
                             62 PRECALL                  1
                             66 CALL                     1
@@ -3848,27 +3942,27 @@
                   None
                names      ('list', '_registry', 'values')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'registered_objects_list'
-               firstlineno 571
+               firstlineno 585
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab010000000000000000010064005300
-               575           0 RESUME                   0
+               589           0 RESUME                   0
                
-               577           2 LOAD_FAST                0 (cls)
+               591           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (registered_objects_dict)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_FAST                1 (name)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
@@ -3877,32 +3971,32 @@
                   None
                names      ('registered_objects_dict', 'get')
                varnames   ('cls', 'name')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
                name       'get_object_by_name'
-               firstlineno 575
+               firstlineno 589
                lnotab 0x0202
          names      ('__name__', '__module__', '__qualname__', '__doc__', '_registry', 'ClassVar', 'Optional', 'dict', 'str', '__annotations__', 'name', '__init_subclass__', 'classmethod', '_register', 'classproperty', 'registered_objects_dict', 'registered_objects_list', 'get_object_by_name')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
          name       'RegistryObject'
-         firstlineno 548
+         firstlineno 562
          lnotab
             0x0c01040236011a020608020104ff0e010204020104ff0e010203020104
             ff0e010203020104ff0e01
       'RegistryObject'
-   names      ('os', 'datetime', 'typing', 'Any', 'Callable', 'ClassVar', 'List', 'Optional', 'Union', 'django.conf', 'settings', 'django.contrib', 'messages', 'django.contrib.auth.views', 'LoginView', 'RedirectURLMixin', 'django.contrib.contenttypes.models', 'ContentType', 'django.contrib.sites.managers', 'CurrentSiteManager', 'django.contrib.sites.models', 'Site', 'django.db', 'models', 'django.db.models', 'JSONField', 'QuerySet', 'django.db.models.fields', 'CharField', 'TextField', 'django.forms.forms', 'BaseForm', 'django.forms.models', 'ModelForm', 'ModelFormMetaclass', 'django.http', 'HttpResponse', 'django.utils.functional', 'classproperty', 'lazy', 'django.utils.translation', 'gettext', '_', 'django.views.generic', 'CreateView', 'UpdateView', 'django.views.generic.edit', 'DeleteView', 'ModelFormMixin', 'reversion', 'dynamic_preferences.settings', 'preferences_settings', 'dynamic_preferences.types', 'FilePreference', 'guardian.admin', 'GuardedModelAdmin', 'guardian.core', 'ObjectPermissionChecker', 'jsonstore.fields', 'IntegerField', 'JSONFieldMixin', 'material.base', 'Layout', 'LayoutNode', 'polymorphic.base', 'PolymorphicModelBase', 'polymorphic.managers', 'PolymorphicManager', 'polymorphic.models', 'PolymorphicModel', 'rules.contrib.admin', 'ObjectPermissionsModelAdmin', 'aleksis.core.managers', 'CurrentSiteManagerWithoutMigrations', 'PolymorphicCurrentSiteManager', 'SchoolTermRelatedQuerySet', 'base', 'ModelBase', '_ExtensibleModelBase', '_generate_one_to_one_proxy_property', 'Model', 'ExtensibleModel', '_ExtensiblePolymorphicModelBase', 'ExtensiblePolymorphicModel', 'object', 'PureDjangoModel', 'GlobalPermissionModel', '_ExtensibleFormMetaclass', 'ExtensibleForm', 'BaseModelAdmin', 'SuccessMessageMixin', 'SuccessNextMixin', 'AdvancedCreateView', 'AdvancedEditView', 'AdvancedDeleteView', 'SchoolTermRelatedExtensibleModel', 'SchoolTermRelatedExtensibleForm', 'PublicFilePreferenceMixin', 'RegistryObject')
+   names      ('os', 'datetime', 'typing', 'Any', 'Callable', 'ClassVar', 'List', 'Optional', 'Union', 'django.conf', 'settings', 'django.contrib', 'messages', 'django.contrib.auth.views', 'LoginView', 'RedirectURLMixin', 'django.contrib.contenttypes.models', 'ContentType', 'django.contrib.sites.managers', 'CurrentSiteManager', 'django.contrib.sites.models', 'Site', 'django.db', 'models', 'django.db.models', 'JSONField', 'QuerySet', 'django.db.models.fields', 'CharField', 'TextField', 'django.forms.forms', 'BaseForm', 'django.forms.models', 'ModelForm', 'ModelFormMetaclass', 'django.http', 'HttpResponse', 'django.utils.functional', 'classproperty', 'lazy', 'django.utils.translation', 'gettext', '_', 'django.views.generic', 'CreateView', 'UpdateView', 'django.views.generic.edit', 'DeleteView', 'ModelFormMixin', 'reversion', 'dynamic_preferences.settings', 'preferences_settings', 'dynamic_preferences.types', 'FilePreference', 'guardian.admin', 'GuardedModelAdmin', 'guardian.core', 'ObjectPermissionChecker', 'jsonstore.fields', 'IntegerField', 'JSONFieldMixin', 'material.base', 'Fieldset', 'Layout', 'LayoutNode', 'polymorphic.base', 'PolymorphicModelBase', 'polymorphic.managers', 'PolymorphicManager', 'polymorphic.models', 'PolymorphicModel', 'rules.contrib.admin', 'ObjectPermissionsModelAdmin', 'aleksis.core.managers', 'CurrentSiteManagerWithoutMigrations', 'PolymorphicCurrentSiteManager', 'SchoolTermRelatedQuerySet', 'base', 'ModelBase', '_ExtensibleModelBase', '_generate_one_to_one_proxy_property', 'Model', 'ExtensibleModel', '_ExtensiblePolymorphicModelBase', 'ExtensiblePolymorphicModel', 'object', 'PureDjangoModel', 'GlobalPermissionModel', '_ExtensibleFormMetaclass', 'ExtensibleForm', 'BaseModelAdmin', 'SuccessMessageMixin', 'SuccessNextMixin', 'AdvancedCreateView', 'AdvancedEditView', 'AdvancedDeleteView', 'SchoolTermRelatedExtensibleModel', 'SchoolTermRelatedExtensibleForm', 'PublicFilePreferenceMixin', 'RegistryObject')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/mixins.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020308010c0120020c010c0110010c010c010c010c01100110010c
-      0110010c0110010c011001100208010c010c010c010c01100110010c010c
+      0110010c0110010c011001100208010c010c010c010c01100114010c010c
       010c010c021407301406162a7f007f00231e040a0106ff120c1c06260b1c
-      10201e1e061c091c071e041e041c131c121c111c0b
+      10202c1e061c091c071e041e041c131c121c111c0b
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/models.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/models.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 51781
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/preferences.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/preferences.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 13478
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/registries.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/registries.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 692
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/rules.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/rules.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 16018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/settings.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/settings.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
-files sz: 39500
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+files sz: 39939
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 18
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -330,116 +330,125 @@
       01646c9001646d900164686702900164559c02670e9001646e9001646f90
       016470a01c00000000000000000000000000000000000000006700900164
       71a201a6010000ab010000000000000000900164729c0569015ae8900164
       735ae9670090016474a2015aea670090016475a2015aeb670090016476a2
       015aec640f5aed640f5aee020065036508a6010000ab0100000000000000
       005aef900164776701651da0220000000000000000000000000000000000
       0000009001647890016479a6020000ab0200000000000000009001647a9c
-      0265ef9001647b3c0000009001647c9001647d690165ef9001647e190000
-      000000000000009001647f3c00000065ef9001647e190000000000000000
-      0090016477190000000000000000009001648019000000000000000000a0
-      f0000000000000000000000000000000000000000090016481a6010000ab
-      010000000000000000010065ef9001647e19000000000000000000900164
-      7719000000000000000000900164823d00651da022000000000000000000
-      000000000000000000000090016483640fa6020000ab0200000000000000
-      00732b65ef90016484190000000000000000009001648519000000000000
-      0000009001647e19000000000000000000a0f00000000000000000000000
-      00000000000000000090016486a6010000ab010000000000000000010065
-      1da022000000000000000000000000000000000000000090016487641ea6
-      020000ab02000000000000000073139001647f6701641e900164889c0265
-      ef9001648419000000000000000000900164893c00000090016477670165
-      1da022000000000000000000000000000000000000000090016478900164
-      79a6020000ab020000000000000000641e9001648a9c0365ef9001648419
-      0000000000000000009001648b3c000000640f5af164015af26524a04300
-      000000000000000000000000000000000000009001648ca6010000ab0100
-      000000000000000100654da0430000000000000000000000000000000000
-      0000009001648da6010000ab010000000000000000010064379001648e65
-      419001648f9c0269015af3900164905af4640f5af59001641a5af6641e5a
-      f7651da02200000000000000000000000000000000000000009001649190
-      016492a6020000ab020000000000000000651da022000000000000000000
-      00000000000000000000009001649390016494a6020000ab020000000000
-      000000900164959c025af8651da022000000000000000000000000000000
-      00000000009001649690016497a6020000ab0200000000000000005af965
-      1da022000000000000000000000000000000000000000090016498900164
-      97a6020000ab0200000000000000005afa641e5afb651da0220000000000
-      000000000000000000000000000000900164996401a6020000ab02000000
-      00000000005afc651da02200000000000000000000000000000000000000
-      009001649a6401a6020000ab0200000000000000005afd9001649b5afe90
-      01649c9001649d67025aff651da022000000000000000000000000000000
-      00000000009001649e6451a6020000ab020000000000000000a08f000000
-      0000000000000000000000000000000000a6000000ab0000000000000000
-      00900164256b0200000000900272a56531a0430000000000000000000000
-      0000000000000000009001649fa6010000ab010000000000000000010090
-      01642690015a0065ffa0f000000000000000000000000000000000000000
-      009001649ca6010000ab0100000000000000000100651da0220000000000
-      000000000000000000000000000000900164a0641ea6020000ab02000000
-      00000000007234900164a190015a01651da0220000000000000000000000
-      000000000000000000900164a26451a6020000ab02000000000000000090
-      015a02651da0220000000000000000000000000000000000000000900164
-      a36488a6020000ab02000000000000000090015a03651da0220000000000
-      000000000000000000000000000000900164a46451a6020000ab02000000
-      000000000090015a04651da0220000000000000000000000000000000000
-      000000900164a56451a6020000ab02000000000000000090015a05651da0
-      220000000000000000000000000000000000000000900164a66451a60200
-      00ab02000000000000000090015a06651da0220000000000000000000000
-      000000000000000000900164a76451a6020000ab02000000000000000090
-      015a07651da0220000000000000000000000000000000000000000900164
-      a86451a6020000ab02000000000000000090015a08651da0220000000000
-      000000000000000000000000000000900164a96451a6020000ab02000000
-      000000000090015a09651da0220000000000000000000000000000000000
-      000000900164aa900164aba6020000ab02000000000000000090015a0a65
-      1da0220000000000000000000000000000000000000000900164ac6451a6
-      020000ab02000000000000000090015a0b651da022000000000000000000
-      0000000000000000000000900164ad6451a6020000ab0200000000000000
-      0090015a0c651da022000000000000000000000000000000000000000090
-      0164ae640fa6020000ab02000000000000000090015a0d651da022000000
-      0000000000000000000000000000000000900164af6488a6020000ab0200
-      0000000000000090015a0e651da022000000000000000000000000000000
-      0000000000900164b06451a6020000ab02000000000000000090015a0f65
-      1da0220000000000000000000000000000000000000000900164b1641ea6
-      020000ab02000000000000000090015a10651da022000000000000000000
-      0000000000000000000000900164b26451a6020000ab0200000000000000
-      0090015a11651da022000000000000000000000000000000000000000090
-      0164b36451a6020000ab02000000000000000090015a12651da022000000
-      0000000000000000000000000000000000900164b46900a6020000ab0200
-      0000000000000090015a13651da022000000000000000000000000000000
-      0000000000900164b5641ea6020000ab02000000000000000090015a1465
-      1da0220000000000000000000000000000000000000000900164b66451a6
-      020000ab02000000000000000090015a15651da022000000000000000000
-      0000000000000000000000900164b7640fa6020000ab0200000000000000
-      0090015a16651da022000000000000000000000000000000000000000090
-      0164b86401a6020000ab02000000000000000090015a17651da022000000
-      0000000000000000000000000000000000900164b9641ea6020000ab0200
-      0000000000000090015a18651da022000000000000000000000000000000
-      0000000000900164ba640fa6020000ab02000000000000000090015a1965
-      1da0220000000000000000000000000000000000000000900164bb640fa6
-      020000ab02000000000000000090015a1a6e08900164bc90015a00900164
-      bd90015a1b9001650090015a1c651da02200000000000000000000000000
-      00000000000000900164be641ea6020000ab02000000000000000090015a
-      1d9001651d72c76400640190016c1e90015a1e6400900164bf90016c1f90
-      016d2090015a2001006400900164c090016c2190016d2290015a22010064
-      00900164c190016c2390016d2490015a2401006400900164c290016c2590
-      016d2690015a260100651da0220000000000000000000000000000000000
-      000000900164c3a6010000ab010000000000000000651da0220000000000
-      000000000000000000000000000000900164c4a6010000ab010000000000
-      000000651da0220000000000000000000000000000000000000000900164
-      c5900164c6a6020000ab020000000000000000651da02200000000000000
-      00000000000000000000000000900164c7641ea6020000ab020000000000
-      000000900164c8900165269b009d02643a900164c99c0690015a27020090
-      01651e90016a280000000000000000900164d3900164ca02009001652290
-      0164cb9001accca6010000ab010000000000000000020090016524a60000
-      00ab000000000000000000020090016520a6000000ab0000000000000000
-      006703690190016527a4018e010100900164cd90015a29900164ce900164
-      ce690190015a2a670090015a2b02006511900164cf9001652aa6020000ab
-      020000000000000000010002006511900164d09001652ba6020000ab0200
-      000000000000000100900164d190015a2c6531a043000000000000000000
-      0000000000000000000000900164d2a6010000ab01000000000000000001
-      0002009001652da6000000ab0000000000000000009001a02e0000000000
-      00000000000000000000000000000002006510a6000000ab000000000000
-      000000a6010000ab010000000000000000010064015300
+      0265ef9001647b3c0000009001647c9001647d9001647e9c0265ef900164
+      7f19000000000000000000900164803c0000009001648190016482690165
+      ef9001648319000000000000000000900164843c00000065ef9001648319
+      000000000000000000900164771900000000000000000090016485190000
+      00000000000000a0f0000000000000000000000000000000000000000090
+      016486a6010000ab010000000000000000010065ef900164831900000000
+      00000000009001647719000000000000000000900164873d009001648065
+      ef9001648319000000000000000000900164771900000000000000000090
+      0164883c000000651da02200000000000000000000000000000000000000
+      0090016489640fa6020000ab020000000000000000732b65ef9001648a19
+      0000000000000000009001648b1900000000000000000090016483190000
+      00000000000000a0f0000000000000000000000000000000000000000090
+      01648ca6010000ab0100000000000000000100651da02200000000000000
+      000000000000000000000000009001648d641ea6020000ab020000000000
+      0000007313900164846701641e9001648e9c0265ef9001648a1900000000
+      00000000009001648f3c000000900164776701651da02200000000000000
+      000000000000000000000000009001647890016479a6020000ab02000000
+      0000000000641e900164909c0365ef9001648a1900000000000000000090
+      0164913c000000651da02200000000000000000000000000000000000000
+      009001647890016479a6020000ab02000000000000000065ef9001648a19
+      0000000000000000009001648b19000000000000000000900164873c0000
+      00651da02200000000000000000000000000000000000000009001647890
+      016479a6020000ab02000000000000000065ef9001648a19000000000000
+      0000009001649219000000000000000000900164873c000000640f5af164
+      015af26524a0430000000000000000000000000000000000000000900164
+      93a6010000ab0100000000000000000100654da043000000000000000000
+      000000000000000000000090016494a6010000ab01000000000000000001
+      006437900164956541900164969c0269015af3900164975af4640f5af590
+      01641a5af6641e5af7651da0220000000000000000000000000000000000
+      0000009001649890016499a6020000ab020000000000000000651da02200
+      000000000000000000000000000000000000009001649a9001649ba60200
+      00ab0200000000000000009001649c9c025af8651da02200000000000000
+      000000000000000000000000009001649d9001649ea6020000ab02000000
+      00000000005af9651da02200000000000000000000000000000000000000
+      009001649f9001649ea6020000ab0200000000000000005afa641e5afb65
+      1da0220000000000000000000000000000000000000000900164a06401a6
+      020000ab0200000000000000005afc651da0220000000000000000000000
+      000000000000000000900164a16401a6020000ab0200000000000000005a
+      fd900164a25afe900164a3900164a467025aff651da02200000000000000
+      00000000000000000000000000900164a56451a6020000ab020000000000
+      000000a08f0000000000000000000000000000000000000000a6000000ab
+      000000000000000000900164256b0200000000900272a56531a043000000
+      0000000000000000000000000000000000900164a6a6010000ab01000000
+      000000000001009001642690015a0065ffa0f00000000000000000000000
+      000000000000000000900164a3a6010000ab010000000000000000010065
+      1da0220000000000000000000000000000000000000000900164a7641ea6
+      020000ab0200000000000000007234900164a890015a01651da022000000
+      0000000000000000000000000000000000900164a96451a6020000ab0200
+      0000000000000090015a02651da022000000000000000000000000000000
+      0000000000900164aa6488a6020000ab02000000000000000090015a0365
+      1da0220000000000000000000000000000000000000000900164ab6451a6
+      020000ab02000000000000000090015a04651da022000000000000000000
+      0000000000000000000000900164ac6451a6020000ab0200000000000000
+      0090015a05651da022000000000000000000000000000000000000000090
+      0164ad6451a6020000ab02000000000000000090015a06651da022000000
+      0000000000000000000000000000000000900164ae6451a6020000ab0200
+      0000000000000090015a07651da022000000000000000000000000000000
+      0000000000900164af6451a6020000ab02000000000000000090015a0865
+      1da0220000000000000000000000000000000000000000900164b06451a6
+      020000ab02000000000000000090015a09651da022000000000000000000
+      0000000000000000000000900164b1900164b2a6020000ab020000000000
+      00000090015a0a651da02200000000000000000000000000000000000000
+      00900164b36451a6020000ab02000000000000000090015a0b651da02200
+      00000000000000000000000000000000000000900164b46451a6020000ab
+      02000000000000000090015a0c651da02200000000000000000000000000
+      00000000000000900164b5640fa6020000ab02000000000000000090015a
+      0d651da0220000000000000000000000000000000000000000900164b664
+      88a6020000ab02000000000000000090015a0e651da02200000000000000
+      00000000000000000000000000900164b76451a6020000ab020000000000
+      00000090015a0f651da02200000000000000000000000000000000000000
+      00900164b8641ea6020000ab02000000000000000090015a10651da02200
+      00000000000000000000000000000000000000900164b96451a6020000ab
+      02000000000000000090015a11651da02200000000000000000000000000
+      00000000000000900164ba6451a6020000ab02000000000000000090015a
+      12651da0220000000000000000000000000000000000000000900164bb69
+      00a6020000ab02000000000000000090015a13651da02200000000000000
+      00000000000000000000000000900164bc641ea6020000ab020000000000
+      00000090015a14651da02200000000000000000000000000000000000000
+      00900164bd6451a6020000ab02000000000000000090015a15651da02200
+      00000000000000000000000000000000000000900164be640fa6020000ab
+      02000000000000000090015a16651da02200000000000000000000000000
+      00000000000000900164bf6401a6020000ab02000000000000000090015a
+      17651da0220000000000000000000000000000000000000000900164c064
+      1ea6020000ab02000000000000000090015a18651da02200000000000000
+      00000000000000000000000000900164c1640fa6020000ab020000000000
+      00000090015a19651da02200000000000000000000000000000000000000
+      00900164c2640fa6020000ab02000000000000000090015a1a6e08900164
+      c390015a00900164c490015a1b9001650090015a1c651da0220000000000
+      000000000000000000000000000000900164c5641ea6020000ab02000000
+      000000000090015a1d9001651d72c76400640190016c1e90015a1e640090
+      0164c690016c1f90016d2090015a2001006400900164c790016c2190016d
+      2290015a2201006400900164c890016c2390016d2490015a240100640090
+      0164c990016c2590016d2690015a260100651da022000000000000000000
+      0000000000000000000000900164caa6010000ab01000000000000000065
+      1da0220000000000000000000000000000000000000000900164cba60100
+      00ab010000000000000000651da022000000000000000000000000000000
+      0000000000900164cc900164cda6020000ab020000000000000000651da0
+      220000000000000000000000000000000000000000900164ce641ea60200
+      00ab020000000000000000900164cf900165269b009d02643a900164d09c
+      0690015a2702009001651e90016a280000000000000000900164da900164
+      d1020090016522900164d29001acd3a6010000ab01000000000000000002
+      0090016524a6000000ab000000000000000000020090016520a6000000ab
+      0000000000000000006703690190016527a4018e010100900164d490015a
+      29900164d5900164d5690190015a2a670090015a2b02006511900164d690
+      01652aa6020000ab020000000000000000010002006511900164d7900165
+      2ba6020000ab0200000000000000000100900164d890015a2c6531a04300
+      00000000000000000000000000000000000000900164d9a6010000ab0100
+      00000000000000010002009001652da6000000ab00000000000000000090
+      01a02e000000000000000000000000000000000000000002006510a60000
+      00ab000000000000000000a6010000ab0100000000000000000100640153
+      00
       0            0 RESUME                   0
    
       1            2 LOAD_CONST               0 (0)
                    4 LOAD_CONST               1 (None)
                    6 IMPORT_NAME              0 (os)
                    8 STORE_NAME               0 (os)
    
@@ -3103,801 +3112,869 @@
                 9806 LOAD_CONST             378 (('handlers', 'level'))
                 9808 BUILD_CONST_KEY_MAP      2
                 9810 LOAD_NAME              239 (LOGGING)
                 9812 EXTENDED_ARG             1
                 9814 LOAD_CONST             379 ('root')
                 9816 STORE_SUBSCR
    
-    939         9820 EXTENDED_ARG             1
-                9822 LOAD_CONST             380 ('class')
-                9824 EXTENDED_ARG             1
-                9826 LOAD_CONST             381 ('logging.NullHandler')
-                9828 BUILD_MAP                1
-                9830 LOAD_NAME              239 (LOGGING)
-                9832 EXTENDED_ARG             1
-                9834 LOAD_CONST             382 ('handlers')
-                9836 BINARY_SUBSCR
-                9846 EXTENDED_ARG             1
-                9848 LOAD_CONST             383 ('null')
-                9850 STORE_SUBSCR
-   
-    941         9854 LOAD_NAME              239 (LOGGING)
-                9856 EXTENDED_ARG             1
-                9858 LOAD_CONST             382 ('handlers')
-                9860 BINARY_SUBSCR
+    940         9820 EXTENDED_ARG             1
+                9822 LOAD_CONST             380 ('{asctime} {levelname} {name}[{process}]: {msg}')
+   
+    941         9824 EXTENDED_ARG             1
+                9826 LOAD_CONST             381 ('{')
+   
+    939         9828 EXTENDED_ARG             1
+                9830 LOAD_CONST             382 (('format', 'style'))
+                9832 BUILD_CONST_KEY_MAP      2
+                9834 LOAD_NAME              239 (LOGGING)
+                9836 EXTENDED_ARG             1
+                9838 LOAD_CONST             383 ('formatters')
+                9840 BINARY_SUBSCR
+                9850 EXTENDED_ARG             1
+                9852 LOAD_CONST             384 ('verbose')
+                9854 STORE_SUBSCR
+   
+    944         9858 EXTENDED_ARG             1
+                9860 LOAD_CONST             385 ('class')
+                9862 EXTENDED_ARG             1
+                9864 LOAD_CONST             386 ('logging.NullHandler')
+                9866 BUILD_MAP                1
+                9868 LOAD_NAME              239 (LOGGING)
                 9870 EXTENDED_ARG             1
-                9872 LOAD_CONST             375 ('console')
+                9872 LOAD_CONST             387 ('handlers')
                 9874 BINARY_SUBSCR
                 9884 EXTENDED_ARG             1
-                9886 LOAD_CONST             384 ('filters')
-                9888 BINARY_SUBSCR
-                9898 LOAD_METHOD            240 (remove)
-                9920 EXTENDED_ARG             1
-                9922 LOAD_CONST             385 ('require_debug_true')
-                9924 PRECALL                  1
-                9928 CALL                     1
-                9938 POP_TOP
-   
-    943         9940 LOAD_NAME              239 (LOGGING)
-                9942 EXTENDED_ARG             1
-                9944 LOAD_CONST             382 ('handlers')
-                9946 BINARY_SUBSCR
-                9956 EXTENDED_ARG             1
-                9958 LOAD_CONST             375 ('console')
-                9960 BINARY_SUBSCR
-                9970 EXTENDED_ARG             1
-                9972 LOAD_CONST             386 ('level')
-                9974 DELETE_SUBSCR
-   
-    945         9976 LOAD_NAME               29 (_settings)
-                9978 LOAD_METHOD             34 (get)
-               10000 EXTENDED_ARG             1
-               10002 LOAD_CONST             387 ('logging.mail_admins')
-               10004 LOAD_CONST              15 (True)
-               10006 PRECALL                  2
-               10010 CALL                     2
-               10020 POP_JUMP_FORWARD_IF_TRUE    43 (to 10108)
-   
-    946        10022 LOAD_NAME              239 (LOGGING)
-               10024 EXTENDED_ARG             1
-               10026 LOAD_CONST             388 ('loggers')
-               10028 BINARY_SUBSCR
-               10038 EXTENDED_ARG             1
-               10040 LOAD_CONST             389 ('django')
-               10042 BINARY_SUBSCR
-               10052 EXTENDED_ARG             1
-               10054 LOAD_CONST             382 ('handlers')
-               10056 BINARY_SUBSCR
-               10066 LOAD_METHOD            240 (remove)
-               10088 EXTENDED_ARG             1
-               10090 LOAD_CONST             390 ('mail_admins')
-               10092 PRECALL                  1
-               10096 CALL                     1
-               10106 POP_TOP
+                9886 LOAD_CONST             388 ('null')
+                9888 STORE_SUBSCR
    
-    948     >> 10108 LOAD_NAME               29 (_settings)
-               10110 LOAD_METHOD             34 (get)
+    946         9892 LOAD_NAME              239 (LOGGING)
+                9894 EXTENDED_ARG             1
+                9896 LOAD_CONST             387 ('handlers')
+                9898 BINARY_SUBSCR
+                9908 EXTENDED_ARG             1
+                9910 LOAD_CONST             375 ('console')
+                9912 BINARY_SUBSCR
+                9922 EXTENDED_ARG             1
+                9924 LOAD_CONST             389 ('filters')
+                9926 BINARY_SUBSCR
+                9936 LOAD_METHOD            240 (remove)
+                9958 EXTENDED_ARG             1
+                9960 LOAD_CONST             390 ('require_debug_true')
+                9962 PRECALL                  1
+                9966 CALL                     1
+                9976 POP_TOP
+   
+    948         9978 LOAD_NAME              239 (LOGGING)
+                9980 EXTENDED_ARG             1
+                9982 LOAD_CONST             387 ('handlers')
+                9984 BINARY_SUBSCR
+                9994 EXTENDED_ARG             1
+                9996 LOAD_CONST             375 ('console')
+                9998 BINARY_SUBSCR
+               10008 EXTENDED_ARG             1
+               10010 LOAD_CONST             391 ('level')
+               10012 DELETE_SUBSCR
+   
+    950        10014 EXTENDED_ARG             1
+               10016 LOAD_CONST             384 ('verbose')
+               10018 LOAD_NAME              239 (LOGGING)
+               10020 EXTENDED_ARG             1
+               10022 LOAD_CONST             387 ('handlers')
+               10024 BINARY_SUBSCR
+               10034 EXTENDED_ARG             1
+               10036 LOAD_CONST             375 ('console')
+               10038 BINARY_SUBSCR
+               10048 EXTENDED_ARG             1
+               10050 LOAD_CONST             392 ('formatter')
+               10052 STORE_SUBSCR
+   
+    952        10056 LOAD_NAME               29 (_settings)
+               10058 LOAD_METHOD             34 (get)
+               10080 EXTENDED_ARG             1
+               10082 LOAD_CONST             393 ('logging.mail_admins')
+               10084 LOAD_CONST              15 (True)
+               10086 PRECALL                  2
+               10090 CALL                     2
+               10100 POP_JUMP_FORWARD_IF_TRUE    43 (to 10188)
+   
+    953        10102 LOAD_NAME              239 (LOGGING)
+               10104 EXTENDED_ARG             1
+               10106 LOAD_CONST             394 ('loggers')
+               10108 BINARY_SUBSCR
+               10118 EXTENDED_ARG             1
+               10120 LOAD_CONST             395 ('django')
+               10122 BINARY_SUBSCR
                10132 EXTENDED_ARG             1
-               10134 LOAD_CONST             391 ('logging.disallowed_host')
-               10136 LOAD_CONST              30 (False)
-               10138 PRECALL                  2
-               10142 CALL                     2
-               10152 POP_JUMP_FORWARD_IF_TRUE    19 (to 10192)
-   
-    950        10154 EXTENDED_ARG             1
-               10156 LOAD_CONST             383 ('null')
-               10158 BUILD_LIST               1
-   
-    951        10160 LOAD_CONST              30 (False)
-   
-    949        10162 EXTENDED_ARG             1
-               10164 LOAD_CONST             392 (('handlers', 'propagate'))
-               10166 BUILD_CONST_KEY_MAP      2
-               10168 LOAD_NAME              239 (LOGGING)
-               10170 EXTENDED_ARG             1
-               10172 LOAD_CONST             388 ('loggers')
-               10174 BINARY_SUBSCR
-               10184 EXTENDED_ARG             1
-               10186 LOAD_CONST             393 ('django.security.DisallowedHost')
-               10188 STORE_SUBSCR
-   
-    955     >> 10192 EXTENDED_ARG             1
-               10194 LOAD_CONST             375 ('console')
-               10196 BUILD_LIST               1
-   
-    956        10198 LOAD_NAME               29 (_settings)
-               10200 LOAD_METHOD             34 (get)
-               10222 EXTENDED_ARG             1
-               10224 LOAD_CONST             376 ('logging.level')
-               10226 EXTENDED_ARG             1
-               10228 LOAD_CONST             377 ('WARNING')
-               10230 PRECALL                  2
-               10234 CALL                     2
-   
-    957        10244 LOAD_CONST              30 (False)
-   
-    954        10246 EXTENDED_ARG             1
-               10248 LOAD_CONST             394 (('handlers', 'level', 'propagate'))
-               10250 BUILD_CONST_KEY_MAP      3
-               10252 LOAD_NAME              239 (LOGGING)
-               10254 EXTENDED_ARG             1
-               10256 LOAD_CONST             388 ('loggers')
-               10258 BINARY_SUBSCR
-               10268 EXTENDED_ARG             1
-               10270 LOAD_CONST             395 ('celery')
-               10272 STORE_SUBSCR
-   
-    962        10276 LOAD_CONST              15 (True)
-               10278 STORE_NAME             241 (GUARDIAN_RAISE_403)
-   
-    963        10280 LOAD_CONST               1 (None)
-               10282 STORE_NAME             242 (ANONYMOUS_USER_NAME)
-   
-    965        10284 LOAD_NAME               36 (SILENCED_SYSTEM_CHECKS)
-               10286 LOAD_METHOD             67 (append)
-               10308 EXTENDED_ARG             1
-               10310 LOAD_CONST             396 ('guardian.W001')
-               10312 PRECALL                  1
-               10316 CALL                     1
-               10326 POP_TOP
-   
-    968        10328 LOAD_NAME               77 (AUTHENTICATION_BACKENDS)
-               10330 LOAD_METHOD             67 (append)
-               10352 EXTENDED_ARG             1
-               10354 LOAD_CONST             397 ('rules.permissions.ObjectPermissionBackend')
-               10356 PRECALL                  1
-               10360 CALL                     1
-               10370 POP_TOP
-   
-    971        10372 LOAD_CONST              55 ('default')
-   
-    972        10374 EXTENDED_ARG             1
-               10376 LOAD_CONST             398 ('haystack_redis.RedisEngine')
-   
-    973        10378 LOAD_NAME               65 (REDIS_URL)
-   
-    971        10380 EXTENDED_ARG             1
-               10382 LOAD_CONST             399 (('ENGINE', 'PATH'))
-               10384 BUILD_CONST_KEY_MAP      2
-   
-    970        10386 BUILD_MAP                1
-               10388 STORE_NAME             243 (HAYSTACK_CONNECTIONS)
-   
-    977        10390 EXTENDED_ARG             1
-               10392 LOAD_CONST             400 ('celery_haystack.signals.CelerySignalProcessor')
-               10394 STORE_NAME             244 (HAYSTACK_SIGNAL_PROCESSOR)
-   
-    978        10396 LOAD_CONST              15 (True)
-               10398 STORE_NAME             245 (CELERY_HAYSTACK_IGNORE_RESULT)
-   
-    980        10400 EXTENDED_ARG             1
-               10402 LOAD_CONST             282 (10)
-               10404 STORE_NAME             246 (HAYSTACK_SEARCH_RESULTS_PER_PAGE)
-   
-    982        10406 LOAD_CONST              30 (False)
-               10408 STORE_NAME             247 (DJANGO_EASY_AUDIT_WATCH_REQUEST_EVENTS)
-   
-    985        10410 LOAD_NAME               29 (_settings)
-               10412 LOAD_METHOD             34 (get)
-               10434 EXTENDED_ARG             1
-               10436 LOAD_CONST             401 ('health.disk_usage_max_percent')
-               10438 EXTENDED_ARG             1
-               10440 LOAD_CONST             402 (90)
-               10442 PRECALL                  2
-               10446 CALL                     2
-   
-    986        10456 LOAD_NAME               29 (_settings)
-               10458 LOAD_METHOD             34 (get)
-               10480 EXTENDED_ARG             1
-               10482 LOAD_CONST             403 ('health.memory_min_mb')
-               10484 EXTENDED_ARG             1
-               10486 LOAD_CONST             404 (500)
-               10488 PRECALL                  2
-               10492 CALL                     2
-   
-    984        10502 EXTENDED_ARG             1
-               10504 LOAD_CONST             405 (('DISK_USAGE_MAX', 'MEMORY_MIN'))
-               10506 BUILD_CONST_KEY_MAP      2
-               10508 STORE_NAME             248 (HEALTH_CHECK)
-   
-    989        10510 LOAD_NAME               29 (_settings)
-               10512 LOAD_METHOD             34 (get)
-               10534 EXTENDED_ARG             1
-               10536 LOAD_CONST             406 ('backup.database.check_seconds')
-               10538 EXTENDED_ARG             1
-               10540 LOAD_CONST             407 (7200)
-               10542 PRECALL                  2
-               10546 CALL                     2
-               10556 STORE_NAME             249 (DBBACKUP_CHECK_SECONDS)
-   
-    990        10558 LOAD_NAME               29 (_settings)
-               10560 LOAD_METHOD             34 (get)
-               10582 EXTENDED_ARG             1
-               10584 LOAD_CONST             408 ('backup.media.check_seconds')
-               10586 EXTENDED_ARG             1
-               10588 LOAD_CONST             407 (7200)
-               10590 PRECALL                  2
-               10594 CALL                     2
-               10604 STORE_NAME             250 (MEDIABACKUP_CHECK_SECONDS)
-   
-    992        10606 LOAD_CONST              30 (False)
-               10608 STORE_NAME             251 (PROMETHEUS_EXPORT_MIGRATIONS)
-   
-    993        10610 LOAD_NAME               29 (_settings)
-               10612 LOAD_METHOD             34 (get)
-               10634 EXTENDED_ARG             1
-               10636 LOAD_CONST             409 ('prometheus.metrics.port')
-               10638 LOAD_CONST               1 (None)
-               10640 PRECALL                  2
-               10644 CALL                     2
-               10654 STORE_NAME             252 (PROMETHEUS_METRICS_EXPORT_PORT)
-   
-    994        10656 LOAD_NAME               29 (_settings)
-               10658 LOAD_METHOD             34 (get)
-               10680 EXTENDED_ARG             1
-               10682 LOAD_CONST             410 ('prometheus.metrucs.address')
-               10684 LOAD_CONST               1 (None)
-               10686 PRECALL                  2
-               10690 CALL                     2
-               10700 STORE_NAME             253 (PROMETHEUS_METRICS_EXPORT_ADDRESS)
-   
-    996        10702 EXTENDED_ARG             1
-               10704 LOAD_CONST             411 (('REQUEST_SCHEME', 'https'))
-               10706 STORE_NAME             254 (SECURE_PROXY_SSL_HEADER)
-   
-    999        10708 EXTENDED_ARG             1
-               10710 LOAD_CONST             412 ('django.core.files.uploadhandler.MemoryFileUploadHandler')
-   
-   1000        10712 EXTENDED_ARG             1
-               10714 LOAD_CONST             413 ('django.core.files.uploadhandler.TemporaryFileUploadHandler')
-   
-    998        10716 BUILD_LIST               2
-               10718 STORE_NAME             255 (FILE_UPLOAD_HANDLERS)
-   
-   1003        10720 LOAD_NAME               29 (_settings)
-               10722 LOAD_METHOD             34 (get)
-               10744 EXTENDED_ARG             1
-               10746 LOAD_CONST             414 ('storage.type')
-               10748 LOAD_CONST              81 ('')
-               10750 PRECALL                  2
-               10754 CALL                     2
-               10764 LOAD_METHOD            143 (lower)
-               10786 PRECALL                  0
-               10790 CALL                     0
-               10800 EXTENDED_ARG             1
-               10802 LOAD_CONST             293 ('s3')
-               10804 COMPARE_OP               2 (==)
-               10810 EXTENDED_ARG             2
-               10812 POP_JUMP_FORWARD_IF_FALSE   677 (to 12168)
-   
-   1004        10814 LOAD_NAME               49 (INSTALLED_APPS)
-               10816 LOAD_METHOD             67 (append)
-               10838 EXTENDED_ARG             1
-               10840 LOAD_CONST             415 ('storages')
-               10842 PRECALL                  1
-               10846 CALL                     1
-               10856 POP_TOP
-   
-   1006        10858 EXTENDED_ARG             1
-               10860 LOAD_CONST             294 ('storages.backends.s3boto3.S3Boto3Storage')
-               10862 EXTENDED_ARG             1
-               10864 STORE_NAME             256 (DEFAULT_FILE_STORAGE)
-   
-   1007        10866 LOAD_NAME              255 (FILE_UPLOAD_HANDLERS)
-               10868 LOAD_METHOD            240 (remove)
-               10890 EXTENDED_ARG             1
-               10892 LOAD_CONST             412 ('django.core.files.uploadhandler.MemoryFileUploadHandler')
-               10894 PRECALL                  1
-               10898 CALL                     1
-               10908 POP_TOP
-   
-   1009        10910 LOAD_NAME               29 (_settings)
-               10912 LOAD_METHOD             34 (get)
-               10934 EXTENDED_ARG             1
-               10936 LOAD_CONST             416 ('storage.s3.static.enabled')
-               10938 LOAD_CONST              30 (False)
-               10940 PRECALL                  2
-               10944 CALL                     2
-               10954 POP_JUMP_FORWARD_IF_FALSE    52 (to 11060)
-   
-   1010        10956 EXTENDED_ARG             1
-               10958 LOAD_CONST             417 ('storages.backends.s3boto3.S3StaticStorage')
-               10960 EXTENDED_ARG             1
-               10962 STORE_NAME             257 (STATICFILES_STORAGE)
-   
-   1011        10964 LOAD_NAME               29 (_settings)
-               10966 LOAD_METHOD             34 (get)
-               10988 EXTENDED_ARG             1
-               10990 LOAD_CONST             418 ('storage.s3.static.bucket_name')
-               10992 LOAD_CONST              81 ('')
-               10994 PRECALL                  2
-               10998 CALL                     2
-               11008 EXTENDED_ARG             1
-               11010 STORE_NAME             258 (AWS_STORAGE_BUCKET_NAME_STATIC)
-   
-   1012        11012 LOAD_NAME               29 (_settings)
-               11014 LOAD_METHOD             34 (get)
-   
-   1013        11036 EXTENDED_ARG             1
-               11038 LOAD_CONST             419 ('storage.s3.static.max_age_seconds')
-               11040 LOAD_CONST             136 (86400)
-   
-   1012        11042 PRECALL                  2
-               11046 CALL                     2
-               11056 EXTENDED_ARG             1
-               11058 STORE_NAME             259 (AWS_S3_MAX_AGE_SECONDS_CACHED_STATIC)
-   
-   1016     >> 11060 LOAD_NAME               29 (_settings)
-               11062 LOAD_METHOD             34 (get)
-               11084 EXTENDED_ARG             1
-               11086 LOAD_CONST             420 ('storage.s3.region_name')
-               11088 LOAD_CONST              81 ('')
-               11090 PRECALL                  2
-               11094 CALL                     2
-               11104 EXTENDED_ARG             1
-               11106 STORE_NAME             260 (AWS_REGION)
-   
-   1017        11108 LOAD_NAME               29 (_settings)
-               11110 LOAD_METHOD             34 (get)
-               11132 EXTENDED_ARG             1
-               11134 LOAD_CONST             421 ('storage.s3.access_key')
-               11136 LOAD_CONST              81 ('')
-               11138 PRECALL                  2
-               11142 CALL                     2
-               11152 EXTENDED_ARG             1
-               11154 STORE_NAME             261 (AWS_ACCESS_KEY_ID)
-   
-   1018        11156 LOAD_NAME               29 (_settings)
-               11158 LOAD_METHOD             34 (get)
-               11180 EXTENDED_ARG             1
-               11182 LOAD_CONST             422 ('storage.s3.secret_key')
-               11184 LOAD_CONST              81 ('')
-               11186 PRECALL                  2
-               11190 CALL                     2
-               11200 EXTENDED_ARG             1
-               11202 STORE_NAME             262 (AWS_SECRET_ACCESS_KEY)
-   
-   1019        11204 LOAD_NAME               29 (_settings)
-               11206 LOAD_METHOD             34 (get)
-               11228 EXTENDED_ARG             1
-               11230 LOAD_CONST             423 ('storage.s3.session_token')
-               11232 LOAD_CONST              81 ('')
-               11234 PRECALL                  2
-               11238 CALL                     2
-               11248 EXTENDED_ARG             1
-               11250 STORE_NAME             263 (AWS_SESSION_TOKEN)
-   
-   1020        11252 LOAD_NAME               29 (_settings)
-               11254 LOAD_METHOD             34 (get)
-               11276 EXTENDED_ARG             1
-               11278 LOAD_CONST             424 ('storage.s3.bucket_name')
-               11280 LOAD_CONST              81 ('')
-               11282 PRECALL                  2
-               11286 CALL                     2
-               11296 EXTENDED_ARG             1
-               11298 STORE_NAME             264 (AWS_STORAGE_BUCKET_NAME)
-   
-   1021        11300 LOAD_NAME               29 (_settings)
-               11302 LOAD_METHOD             34 (get)
-               11324 EXTENDED_ARG             1
-               11326 LOAD_CONST             425 ('storage.s3.location')
-               11328 LOAD_CONST              81 ('')
-               11330 PRECALL                  2
-               11334 CALL                     2
-               11344 EXTENDED_ARG             1
-               11346 STORE_NAME             265 (AWS_LOCATION)
-   
-   1022        11348 LOAD_NAME               29 (_settings)
-               11350 LOAD_METHOD             34 (get)
-               11372 EXTENDED_ARG             1
-               11374 LOAD_CONST             426 ('storage.s3.addressing_style')
-               11376 EXTENDED_ARG             1
-               11378 LOAD_CONST             427 ('auto')
-               11380 PRECALL                  2
-               11384 CALL                     2
-               11394 EXTENDED_ARG             1
-               11396 STORE_NAME             266 (AWS_S3_ADDRESSING_STYLE)
-   
-   1023        11398 LOAD_NAME               29 (_settings)
-               11400 LOAD_METHOD             34 (get)
-               11422 EXTENDED_ARG             1
-               11424 LOAD_CONST             428 ('storage.s3.endpoint_url')
-               11426 LOAD_CONST              81 ('')
-               11428 PRECALL                  2
-               11432 CALL                     2
-               11442 EXTENDED_ARG             1
-               11444 STORE_NAME             267 (AWS_S3_ENDPOINT_URL)
-   
-   1024        11446 LOAD_NAME               29 (_settings)
-               11448 LOAD_METHOD             34 (get)
-               11470 EXTENDED_ARG             1
-               11472 LOAD_CONST             429 ('storage.s3.key_prefix')
-               11474 LOAD_CONST              81 ('')
-               11476 PRECALL                  2
-               11480 CALL                     2
-               11490 EXTENDED_ARG             1
-               11492 STORE_NAME             268 (AWS_S3_KEY_PREFIX)
-   
-   1025        11494 LOAD_NAME               29 (_settings)
-               11496 LOAD_METHOD             34 (get)
-               11518 EXTENDED_ARG             1
-               11520 LOAD_CONST             430 ('storage.s3.bucket_auth')
-               11522 LOAD_CONST              15 (True)
-               11524 PRECALL                  2
-               11528 CALL                     2
-               11538 EXTENDED_ARG             1
-               11540 STORE_NAME             269 (AWS_S3_BUCKET_AUTH)
-   
-   1026        11542 LOAD_NAME               29 (_settings)
-               11544 LOAD_METHOD             34 (get)
-               11566 EXTENDED_ARG             1
-               11568 LOAD_CONST             431 ('storage.s3.max_age_seconds')
-               11570 LOAD_CONST             136 (86400)
-               11572 PRECALL                  2
-               11576 CALL                     2
-               11586 EXTENDED_ARG             1
-               11588 STORE_NAME             270 (AWS_S3_MAX_AGE_SECONDS)
-   
-   1027        11590 LOAD_NAME               29 (_settings)
-               11592 LOAD_METHOD             34 (get)
-               11614 EXTENDED_ARG             1
-               11616 LOAD_CONST             432 ('storage.s3.public_url')
-               11618 LOAD_CONST              81 ('')
-               11620 PRECALL                  2
-               11624 CALL                     2
-               11634 EXTENDED_ARG             1
-               11636 STORE_NAME             271 (AWS_S3_PUBLIC_URL)
-   
-   1028        11638 LOAD_NAME               29 (_settings)
-               11640 LOAD_METHOD             34 (get)
-               11662 EXTENDED_ARG             1
-               11664 LOAD_CONST             433 ('storage.s3.reduced_redundancy')
-               11666 LOAD_CONST              30 (False)
-               11668 PRECALL                  2
-               11672 CALL                     2
-               11682 EXTENDED_ARG             1
-               11684 STORE_NAME             272 (AWS_S3_REDUCED_REDUNDANCY)
-   
-   1029        11686 LOAD_NAME               29 (_settings)
-               11688 LOAD_METHOD             34 (get)
-               11710 EXTENDED_ARG             1
-               11712 LOAD_CONST             434 ('storage.s3.content_disposition')
-               11714 LOAD_CONST              81 ('')
-               11716 PRECALL                  2
-               11720 CALL                     2
-               11730 EXTENDED_ARG             1
-               11732 STORE_NAME             273 (AWS_S3_CONTENT_DISPOSITION)
-   
-   1030        11734 LOAD_NAME               29 (_settings)
-               11736 LOAD_METHOD             34 (get)
-               11758 EXTENDED_ARG             1
-               11760 LOAD_CONST             435 ('storage.s3.content_language')
-               11762 LOAD_CONST              81 ('')
-               11764 PRECALL                  2
-               11768 CALL                     2
-               11778 EXTENDED_ARG             1
-               11780 STORE_NAME             274 (AWS_S3_CONTENT_LANGUAGE)
-   
-   1031        11782 LOAD_NAME               29 (_settings)
-               11784 LOAD_METHOD             34 (get)
-               11806 EXTENDED_ARG             1
-               11808 LOAD_CONST             436 ('storage.s3.metadata')
-               11810 BUILD_MAP                0
-               11812 PRECALL                  2
-               11816 CALL                     2
-               11826 EXTENDED_ARG             1
-               11828 STORE_NAME             275 (AWS_S3_METADATA)
-   
-   1032        11830 LOAD_NAME               29 (_settings)
-               11832 LOAD_METHOD             34 (get)
-               11854 EXTENDED_ARG             1
-               11856 LOAD_CONST             437 ('storage.s3.encrypt_key')
-               11858 LOAD_CONST              30 (False)
-               11860 PRECALL                  2
-               11864 CALL                     2
-               11874 EXTENDED_ARG             1
-               11876 STORE_NAME             276 (AWS_S3_ENCRYPT_KEY)
-   
-   1033        11878 LOAD_NAME               29 (_settings)
-               11880 LOAD_METHOD             34 (get)
-               11902 EXTENDED_ARG             1
-               11904 LOAD_CONST             438 ('storage.s3.kms_encryption_key_id')
-               11906 LOAD_CONST              81 ('')
-               11908 PRECALL                  2
-               11912 CALL                     2
-               11922 EXTENDED_ARG             1
-               11924 STORE_NAME             277 (AWS_S3_KMS_ENCRYPTION_KEY_ID)
-   
-   1034        11926 LOAD_NAME               29 (_settings)
-               11928 LOAD_METHOD             34 (get)
-               11950 EXTENDED_ARG             1
-               11952 LOAD_CONST             439 ('storage.s3.gzip')
-               11954 LOAD_CONST              15 (True)
-               11956 PRECALL                  2
-               11960 CALL                     2
-               11970 EXTENDED_ARG             1
-               11972 STORE_NAME             278 (AWS_S3_GZIP)
-   
-   1035        11974 LOAD_NAME               29 (_settings)
-               11976 LOAD_METHOD             34 (get)
-               11998 EXTENDED_ARG             1
-               12000 LOAD_CONST             440 ('storage.s3.signature_version')
-               12002 LOAD_CONST               1 (None)
-               12004 PRECALL                  2
-               12008 CALL                     2
-               12018 EXTENDED_ARG             1
-               12020 STORE_NAME             279 (AWS_S3_SIGNATURE_VERSION)
-   
-   1036        12022 LOAD_NAME               29 (_settings)
-               12024 LOAD_METHOD             34 (get)
-               12046 EXTENDED_ARG             1
-               12048 LOAD_CONST             441 ('storage.s3.file_overwrite')
-               12050 LOAD_CONST              30 (False)
-               12052 PRECALL                  2
-               12056 CALL                     2
-               12066 EXTENDED_ARG             1
-               12068 STORE_NAME             280 (AWS_S3_FILE_OVERWRITE)
-   
-   1037        12070 LOAD_NAME               29 (_settings)
-               12072 LOAD_METHOD             34 (get)
-               12094 EXTENDED_ARG             1
-               12096 LOAD_CONST             442 ('storage.s3.verify')
-               12098 LOAD_CONST              15 (True)
-               12100 PRECALL                  2
-               12104 CALL                     2
-               12114 EXTENDED_ARG             1
-               12116 STORE_NAME             281 (AWS_S3_VERIFY)
-   
-   1038        12118 LOAD_NAME               29 (_settings)
-               12120 LOAD_METHOD             34 (get)
-               12142 EXTENDED_ARG             1
-               12144 LOAD_CONST             443 ('storage.s3.use_ssl')
-               12146 LOAD_CONST              15 (True)
-               12148 PRECALL                  2
-               12152 CALL                     2
-               12162 EXTENDED_ARG             1
-               12164 STORE_NAME             282 (AWS_S3_USE_SSL)
-               12166 JUMP_FORWARD             8 (to 12184)
-   
-   1040     >> 12168 EXTENDED_ARG             1
-               12170 LOAD_CONST             444 ('titofisto.TitofistoStorage')
-               12172 EXTENDED_ARG             1
-               12174 STORE_NAME             256 (DEFAULT_FILE_STORAGE)
-   
-   1041        12176 EXTENDED_ARG             1
-               12178 LOAD_CONST             445 (600)
-               12180 EXTENDED_ARG             1
-               12182 STORE_NAME             283 (TITOFISTO_TIMEOUT)
-   
-   1043     >> 12184 EXTENDED_ARG             1
-               12186 LOAD_NAME              256 (DEFAULT_FILE_STORAGE)
-               12188 EXTENDED_ARG             1
-               12190 STORE_NAME             284 (SASS_PROCESSOR_STORAGE)
-   
-   1045        12192 LOAD_NAME               29 (_settings)
-               12194 LOAD_METHOD             34 (get)
-               12216 EXTENDED_ARG             1
-               12218 LOAD_CONST             446 ('health.sentry.enabled')
-               12220 LOAD_CONST              30 (False)
-               12222 PRECALL                  2
-               12226 CALL                     2
-               12236 EXTENDED_ARG             1
-               12238 STORE_NAME             285 (SENTRY_ENABLED)
-   
-   1046        12240 EXTENDED_ARG             1
-               12242 LOAD_NAME              285 (SENTRY_ENABLED)
-               12244 POP_JUMP_FORWARD_IF_FALSE   199 (to 12644)
-   
-   1047        12246 LOAD_CONST               0 (0)
-               12248 LOAD_CONST               1 (None)
-               12250 EXTENDED_ARG             1
-               12252 IMPORT_NAME            286 (sentry_sdk)
-               12254 EXTENDED_ARG             1
-               12256 STORE_NAME             286 (sentry_sdk)
-   
-   1048        12258 LOAD_CONST               0 (0)
-               12260 EXTENDED_ARG             1
-               12262 LOAD_CONST             447 (('CeleryIntegration',))
-               12264 EXTENDED_ARG             1
-               12266 IMPORT_NAME            287 (sentry_sdk.integrations.celery)
-               12268 EXTENDED_ARG             1
-               12270 IMPORT_FROM            288 (CeleryIntegration)
-               12272 EXTENDED_ARG             1
-               12274 STORE_NAME             288 (CeleryIntegration)
-               12276 POP_TOP
-   
-   1049        12278 LOAD_CONST               0 (0)
-               12280 EXTENDED_ARG             1
-               12282 LOAD_CONST             448 (('DjangoIntegration',))
-               12284 EXTENDED_ARG             1
-               12286 IMPORT_NAME            289 (sentry_sdk.integrations.django)
-               12288 EXTENDED_ARG             1
-               12290 IMPORT_FROM            290 (DjangoIntegration)
-               12292 EXTENDED_ARG             1
-               12294 STORE_NAME             290 (DjangoIntegration)
-               12296 POP_TOP
-   
-   1050        12298 LOAD_CONST               0 (0)
-               12300 EXTENDED_ARG             1
-               12302 LOAD_CONST             449 (('RedisIntegration',))
-               12304 EXTENDED_ARG             1
-               12306 IMPORT_NAME            291 (sentry_sdk.integrations.redis)
-               12308 EXTENDED_ARG             1
-               12310 IMPORT_FROM            292 (RedisIntegration)
-               12312 EXTENDED_ARG             1
-               12314 STORE_NAME             292 (RedisIntegration)
-               12316 POP_TOP
-   
-   1052        12318 LOAD_CONST               0 (0)
-               12320 EXTENDED_ARG             1
-               12322 LOAD_CONST             450 (('__version__',))
-               12324 EXTENDED_ARG             1
-               12326 IMPORT_NAME            293 (aleksis.core)
-               12328 EXTENDED_ARG             1
-               12330 IMPORT_FROM            294 (__version__)
-               12332 EXTENDED_ARG             1
-               12334 STORE_NAME             294 (__version__)
-               12336 POP_TOP
-   
-   1055        12338 LOAD_NAME               29 (_settings)
-               12340 LOAD_METHOD             34 (get)
+               10134 LOAD_CONST             387 ('handlers')
+               10136 BINARY_SUBSCR
+               10146 LOAD_METHOD            240 (remove)
+               10168 EXTENDED_ARG             1
+               10170 LOAD_CONST             396 ('mail_admins')
+               10172 PRECALL                  1
+               10176 CALL                     1
+               10186 POP_TOP
+   
+    955     >> 10188 LOAD_NAME               29 (_settings)
+               10190 LOAD_METHOD             34 (get)
+               10212 EXTENDED_ARG             1
+               10214 LOAD_CONST             397 ('logging.disallowed_host')
+               10216 LOAD_CONST              30 (False)
+               10218 PRECALL                  2
+               10222 CALL                     2
+               10232 POP_JUMP_FORWARD_IF_TRUE    19 (to 10272)
+   
+    957        10234 EXTENDED_ARG             1
+               10236 LOAD_CONST             388 ('null')
+               10238 BUILD_LIST               1
+   
+    958        10240 LOAD_CONST              30 (False)
+   
+    956        10242 EXTENDED_ARG             1
+               10244 LOAD_CONST             398 (('handlers', 'propagate'))
+               10246 BUILD_CONST_KEY_MAP      2
+               10248 LOAD_NAME              239 (LOGGING)
+               10250 EXTENDED_ARG             1
+               10252 LOAD_CONST             394 ('loggers')
+               10254 BINARY_SUBSCR
+               10264 EXTENDED_ARG             1
+               10266 LOAD_CONST             399 ('django.security.DisallowedHost')
+               10268 STORE_SUBSCR
+   
+    962     >> 10272 EXTENDED_ARG             1
+               10274 LOAD_CONST             375 ('console')
+               10276 BUILD_LIST               1
+   
+    963        10278 LOAD_NAME               29 (_settings)
+               10280 LOAD_METHOD             34 (get)
+               10302 EXTENDED_ARG             1
+               10304 LOAD_CONST             376 ('logging.level')
+               10306 EXTENDED_ARG             1
+               10308 LOAD_CONST             377 ('WARNING')
+               10310 PRECALL                  2
+               10314 CALL                     2
+   
+    964        10324 LOAD_CONST              30 (False)
+   
+    961        10326 EXTENDED_ARG             1
+               10328 LOAD_CONST             400 (('handlers', 'level', 'propagate'))
+               10330 BUILD_CONST_KEY_MAP      3
+               10332 LOAD_NAME              239 (LOGGING)
+               10334 EXTENDED_ARG             1
+               10336 LOAD_CONST             394 ('loggers')
+               10338 BINARY_SUBSCR
+               10348 EXTENDED_ARG             1
+               10350 LOAD_CONST             401 ('celery')
+               10352 STORE_SUBSCR
+   
+    967        10356 LOAD_NAME               29 (_settings)
+               10358 LOAD_METHOD             34 (get)
+               10380 EXTENDED_ARG             1
+               10382 LOAD_CONST             376 ('logging.level')
+               10384 EXTENDED_ARG             1
+               10386 LOAD_CONST             377 ('WARNING')
+               10388 PRECALL                  2
+               10392 CALL                     2
+               10402 LOAD_NAME              239 (LOGGING)
+               10404 EXTENDED_ARG             1
+               10406 LOAD_CONST             394 ('loggers')
+               10408 BINARY_SUBSCR
+               10418 EXTENDED_ARG             1
+               10420 LOAD_CONST             395 ('django')
+               10422 BINARY_SUBSCR
+               10432 EXTENDED_ARG             1
+               10434 LOAD_CONST             391 ('level')
+               10436 STORE_SUBSCR
+   
+    968        10440 LOAD_NAME               29 (_settings)
+               10442 LOAD_METHOD             34 (get)
+               10464 EXTENDED_ARG             1
+               10466 LOAD_CONST             376 ('logging.level')
+               10468 EXTENDED_ARG             1
+               10470 LOAD_CONST             377 ('WARNING')
+               10472 PRECALL                  2
+               10476 CALL                     2
+               10486 LOAD_NAME              239 (LOGGING)
+               10488 EXTENDED_ARG             1
+               10490 LOAD_CONST             394 ('loggers')
+               10492 BINARY_SUBSCR
+               10502 EXTENDED_ARG             1
+               10504 LOAD_CONST             402 ('django.server')
+               10506 BINARY_SUBSCR
+               10516 EXTENDED_ARG             1
+               10518 LOAD_CONST             391 ('level')
+               10520 STORE_SUBSCR
+   
+    972        10524 LOAD_CONST              15 (True)
+               10526 STORE_NAME             241 (GUARDIAN_RAISE_403)
+   
+    973        10528 LOAD_CONST               1 (None)
+               10530 STORE_NAME             242 (ANONYMOUS_USER_NAME)
+   
+    975        10532 LOAD_NAME               36 (SILENCED_SYSTEM_CHECKS)
+               10534 LOAD_METHOD             67 (append)
+               10556 EXTENDED_ARG             1
+               10558 LOAD_CONST             403 ('guardian.W001')
+               10560 PRECALL                  1
+               10564 CALL                     1
+               10574 POP_TOP
+   
+    978        10576 LOAD_NAME               77 (AUTHENTICATION_BACKENDS)
+               10578 LOAD_METHOD             67 (append)
+               10600 EXTENDED_ARG             1
+               10602 LOAD_CONST             404 ('rules.permissions.ObjectPermissionBackend')
+               10604 PRECALL                  1
+               10608 CALL                     1
+               10618 POP_TOP
+   
+    981        10620 LOAD_CONST              55 ('default')
+   
+    982        10622 EXTENDED_ARG             1
+               10624 LOAD_CONST             405 ('haystack_redis.RedisEngine')
+   
+    983        10626 LOAD_NAME               65 (REDIS_URL)
+   
+    981        10628 EXTENDED_ARG             1
+               10630 LOAD_CONST             406 (('ENGINE', 'PATH'))
+               10632 BUILD_CONST_KEY_MAP      2
+   
+    980        10634 BUILD_MAP                1
+               10636 STORE_NAME             243 (HAYSTACK_CONNECTIONS)
+   
+    987        10638 EXTENDED_ARG             1
+               10640 LOAD_CONST             407 ('celery_haystack.signals.CelerySignalProcessor')
+               10642 STORE_NAME             244 (HAYSTACK_SIGNAL_PROCESSOR)
+   
+    988        10644 LOAD_CONST              15 (True)
+               10646 STORE_NAME             245 (CELERY_HAYSTACK_IGNORE_RESULT)
+   
+    990        10648 EXTENDED_ARG             1
+               10650 LOAD_CONST             282 (10)
+               10652 STORE_NAME             246 (HAYSTACK_SEARCH_RESULTS_PER_PAGE)
+   
+    992        10654 LOAD_CONST              30 (False)
+               10656 STORE_NAME             247 (DJANGO_EASY_AUDIT_WATCH_REQUEST_EVENTS)
+   
+    995        10658 LOAD_NAME               29 (_settings)
+               10660 LOAD_METHOD             34 (get)
+               10682 EXTENDED_ARG             1
+               10684 LOAD_CONST             408 ('health.disk_usage_max_percent')
+               10686 EXTENDED_ARG             1
+               10688 LOAD_CONST             409 (90)
+               10690 PRECALL                  2
+               10694 CALL                     2
+   
+    996        10704 LOAD_NAME               29 (_settings)
+               10706 LOAD_METHOD             34 (get)
+               10728 EXTENDED_ARG             1
+               10730 LOAD_CONST             410 ('health.memory_min_mb')
+               10732 EXTENDED_ARG             1
+               10734 LOAD_CONST             411 (500)
+               10736 PRECALL                  2
+               10740 CALL                     2
+   
+    994        10750 EXTENDED_ARG             1
+               10752 LOAD_CONST             412 (('DISK_USAGE_MAX', 'MEMORY_MIN'))
+               10754 BUILD_CONST_KEY_MAP      2
+               10756 STORE_NAME             248 (HEALTH_CHECK)
+   
+    999        10758 LOAD_NAME               29 (_settings)
+               10760 LOAD_METHOD             34 (get)
+               10782 EXTENDED_ARG             1
+               10784 LOAD_CONST             413 ('backup.database.check_seconds')
+               10786 EXTENDED_ARG             1
+               10788 LOAD_CONST             414 (7200)
+               10790 PRECALL                  2
+               10794 CALL                     2
+               10804 STORE_NAME             249 (DBBACKUP_CHECK_SECONDS)
+   
+   1000        10806 LOAD_NAME               29 (_settings)
+               10808 LOAD_METHOD             34 (get)
+               10830 EXTENDED_ARG             1
+               10832 LOAD_CONST             415 ('backup.media.check_seconds')
+               10834 EXTENDED_ARG             1
+               10836 LOAD_CONST             414 (7200)
+               10838 PRECALL                  2
+               10842 CALL                     2
+               10852 STORE_NAME             250 (MEDIABACKUP_CHECK_SECONDS)
+   
+   1002        10854 LOAD_CONST              30 (False)
+               10856 STORE_NAME             251 (PROMETHEUS_EXPORT_MIGRATIONS)
+   
+   1003        10858 LOAD_NAME               29 (_settings)
+               10860 LOAD_METHOD             34 (get)
+               10882 EXTENDED_ARG             1
+               10884 LOAD_CONST             416 ('prometheus.metrics.port')
+               10886 LOAD_CONST               1 (None)
+               10888 PRECALL                  2
+               10892 CALL                     2
+               10902 STORE_NAME             252 (PROMETHEUS_METRICS_EXPORT_PORT)
+   
+   1004        10904 LOAD_NAME               29 (_settings)
+               10906 LOAD_METHOD             34 (get)
+               10928 EXTENDED_ARG             1
+               10930 LOAD_CONST             417 ('prometheus.metrucs.address')
+               10932 LOAD_CONST               1 (None)
+               10934 PRECALL                  2
+               10938 CALL                     2
+               10948 STORE_NAME             253 (PROMETHEUS_METRICS_EXPORT_ADDRESS)
+   
+   1006        10950 EXTENDED_ARG             1
+               10952 LOAD_CONST             418 (('REQUEST_SCHEME', 'https'))
+               10954 STORE_NAME             254 (SECURE_PROXY_SSL_HEADER)
+   
+   1009        10956 EXTENDED_ARG             1
+               10958 LOAD_CONST             419 ('django.core.files.uploadhandler.MemoryFileUploadHandler')
+   
+   1010        10960 EXTENDED_ARG             1
+               10962 LOAD_CONST             420 ('django.core.files.uploadhandler.TemporaryFileUploadHandler')
+   
+   1008        10964 BUILD_LIST               2
+               10966 STORE_NAME             255 (FILE_UPLOAD_HANDLERS)
+   
+   1013        10968 LOAD_NAME               29 (_settings)
+               10970 LOAD_METHOD             34 (get)
+               10992 EXTENDED_ARG             1
+               10994 LOAD_CONST             421 ('storage.type')
+               10996 LOAD_CONST              81 ('')
+               10998 PRECALL                  2
+               11002 CALL                     2
+               11012 LOAD_METHOD            143 (lower)
+               11034 PRECALL                  0
+               11038 CALL                     0
+               11048 EXTENDED_ARG             1
+               11050 LOAD_CONST             293 ('s3')
+               11052 COMPARE_OP               2 (==)
+               11058 EXTENDED_ARG             2
+               11060 POP_JUMP_FORWARD_IF_FALSE   677 (to 12416)
+   
+   1014        11062 LOAD_NAME               49 (INSTALLED_APPS)
+               11064 LOAD_METHOD             67 (append)
+               11086 EXTENDED_ARG             1
+               11088 LOAD_CONST             422 ('storages')
+               11090 PRECALL                  1
+               11094 CALL                     1
+               11104 POP_TOP
+   
+   1016        11106 EXTENDED_ARG             1
+               11108 LOAD_CONST             294 ('storages.backends.s3boto3.S3Boto3Storage')
+               11110 EXTENDED_ARG             1
+               11112 STORE_NAME             256 (DEFAULT_FILE_STORAGE)
+   
+   1017        11114 LOAD_NAME              255 (FILE_UPLOAD_HANDLERS)
+               11116 LOAD_METHOD            240 (remove)
+               11138 EXTENDED_ARG             1
+               11140 LOAD_CONST             419 ('django.core.files.uploadhandler.MemoryFileUploadHandler')
+               11142 PRECALL                  1
+               11146 CALL                     1
+               11156 POP_TOP
+   
+   1019        11158 LOAD_NAME               29 (_settings)
+               11160 LOAD_METHOD             34 (get)
+               11182 EXTENDED_ARG             1
+               11184 LOAD_CONST             423 ('storage.s3.static.enabled')
+               11186 LOAD_CONST              30 (False)
+               11188 PRECALL                  2
+               11192 CALL                     2
+               11202 POP_JUMP_FORWARD_IF_FALSE    52 (to 11308)
+   
+   1020        11204 EXTENDED_ARG             1
+               11206 LOAD_CONST             424 ('storages.backends.s3boto3.S3StaticStorage')
+               11208 EXTENDED_ARG             1
+               11210 STORE_NAME             257 (STATICFILES_STORAGE)
+   
+   1021        11212 LOAD_NAME               29 (_settings)
+               11214 LOAD_METHOD             34 (get)
+               11236 EXTENDED_ARG             1
+               11238 LOAD_CONST             425 ('storage.s3.static.bucket_name')
+               11240 LOAD_CONST              81 ('')
+               11242 PRECALL                  2
+               11246 CALL                     2
+               11256 EXTENDED_ARG             1
+               11258 STORE_NAME             258 (AWS_STORAGE_BUCKET_NAME_STATIC)
+   
+   1022        11260 LOAD_NAME               29 (_settings)
+               11262 LOAD_METHOD             34 (get)
+   
+   1023        11284 EXTENDED_ARG             1
+               11286 LOAD_CONST             426 ('storage.s3.static.max_age_seconds')
+               11288 LOAD_CONST             136 (86400)
+   
+   1022        11290 PRECALL                  2
+               11294 CALL                     2
+               11304 EXTENDED_ARG             1
+               11306 STORE_NAME             259 (AWS_S3_MAX_AGE_SECONDS_CACHED_STATIC)
+   
+   1026     >> 11308 LOAD_NAME               29 (_settings)
+               11310 LOAD_METHOD             34 (get)
+               11332 EXTENDED_ARG             1
+               11334 LOAD_CONST             427 ('storage.s3.region_name')
+               11336 LOAD_CONST              81 ('')
+               11338 PRECALL                  2
+               11342 CALL                     2
+               11352 EXTENDED_ARG             1
+               11354 STORE_NAME             260 (AWS_REGION)
+   
+   1027        11356 LOAD_NAME               29 (_settings)
+               11358 LOAD_METHOD             34 (get)
+               11380 EXTENDED_ARG             1
+               11382 LOAD_CONST             428 ('storage.s3.access_key')
+               11384 LOAD_CONST              81 ('')
+               11386 PRECALL                  2
+               11390 CALL                     2
+               11400 EXTENDED_ARG             1
+               11402 STORE_NAME             261 (AWS_ACCESS_KEY_ID)
+   
+   1028        11404 LOAD_NAME               29 (_settings)
+               11406 LOAD_METHOD             34 (get)
+               11428 EXTENDED_ARG             1
+               11430 LOAD_CONST             429 ('storage.s3.secret_key')
+               11432 LOAD_CONST              81 ('')
+               11434 PRECALL                  2
+               11438 CALL                     2
+               11448 EXTENDED_ARG             1
+               11450 STORE_NAME             262 (AWS_SECRET_ACCESS_KEY)
+   
+   1029        11452 LOAD_NAME               29 (_settings)
+               11454 LOAD_METHOD             34 (get)
+               11476 EXTENDED_ARG             1
+               11478 LOAD_CONST             430 ('storage.s3.session_token')
+               11480 LOAD_CONST              81 ('')
+               11482 PRECALL                  2
+               11486 CALL                     2
+               11496 EXTENDED_ARG             1
+               11498 STORE_NAME             263 (AWS_SESSION_TOKEN)
+   
+   1030        11500 LOAD_NAME               29 (_settings)
+               11502 LOAD_METHOD             34 (get)
+               11524 EXTENDED_ARG             1
+               11526 LOAD_CONST             431 ('storage.s3.bucket_name')
+               11528 LOAD_CONST              81 ('')
+               11530 PRECALL                  2
+               11534 CALL                     2
+               11544 EXTENDED_ARG             1
+               11546 STORE_NAME             264 (AWS_STORAGE_BUCKET_NAME)
+   
+   1031        11548 LOAD_NAME               29 (_settings)
+               11550 LOAD_METHOD             34 (get)
+               11572 EXTENDED_ARG             1
+               11574 LOAD_CONST             432 ('storage.s3.location')
+               11576 LOAD_CONST              81 ('')
+               11578 PRECALL                  2
+               11582 CALL                     2
+               11592 EXTENDED_ARG             1
+               11594 STORE_NAME             265 (AWS_LOCATION)
+   
+   1032        11596 LOAD_NAME               29 (_settings)
+               11598 LOAD_METHOD             34 (get)
+               11620 EXTENDED_ARG             1
+               11622 LOAD_CONST             433 ('storage.s3.addressing_style')
+               11624 EXTENDED_ARG             1
+               11626 LOAD_CONST             434 ('auto')
+               11628 PRECALL                  2
+               11632 CALL                     2
+               11642 EXTENDED_ARG             1
+               11644 STORE_NAME             266 (AWS_S3_ADDRESSING_STYLE)
+   
+   1033        11646 LOAD_NAME               29 (_settings)
+               11648 LOAD_METHOD             34 (get)
+               11670 EXTENDED_ARG             1
+               11672 LOAD_CONST             435 ('storage.s3.endpoint_url')
+               11674 LOAD_CONST              81 ('')
+               11676 PRECALL                  2
+               11680 CALL                     2
+               11690 EXTENDED_ARG             1
+               11692 STORE_NAME             267 (AWS_S3_ENDPOINT_URL)
+   
+   1034        11694 LOAD_NAME               29 (_settings)
+               11696 LOAD_METHOD             34 (get)
+               11718 EXTENDED_ARG             1
+               11720 LOAD_CONST             436 ('storage.s3.key_prefix')
+               11722 LOAD_CONST              81 ('')
+               11724 PRECALL                  2
+               11728 CALL                     2
+               11738 EXTENDED_ARG             1
+               11740 STORE_NAME             268 (AWS_S3_KEY_PREFIX)
+   
+   1035        11742 LOAD_NAME               29 (_settings)
+               11744 LOAD_METHOD             34 (get)
+               11766 EXTENDED_ARG             1
+               11768 LOAD_CONST             437 ('storage.s3.bucket_auth')
+               11770 LOAD_CONST              15 (True)
+               11772 PRECALL                  2
+               11776 CALL                     2
+               11786 EXTENDED_ARG             1
+               11788 STORE_NAME             269 (AWS_S3_BUCKET_AUTH)
+   
+   1036        11790 LOAD_NAME               29 (_settings)
+               11792 LOAD_METHOD             34 (get)
+               11814 EXTENDED_ARG             1
+               11816 LOAD_CONST             438 ('storage.s3.max_age_seconds')
+               11818 LOAD_CONST             136 (86400)
+               11820 PRECALL                  2
+               11824 CALL                     2
+               11834 EXTENDED_ARG             1
+               11836 STORE_NAME             270 (AWS_S3_MAX_AGE_SECONDS)
+   
+   1037        11838 LOAD_NAME               29 (_settings)
+               11840 LOAD_METHOD             34 (get)
+               11862 EXTENDED_ARG             1
+               11864 LOAD_CONST             439 ('storage.s3.public_url')
+               11866 LOAD_CONST              81 ('')
+               11868 PRECALL                  2
+               11872 CALL                     2
+               11882 EXTENDED_ARG             1
+               11884 STORE_NAME             271 (AWS_S3_PUBLIC_URL)
+   
+   1038        11886 LOAD_NAME               29 (_settings)
+               11888 LOAD_METHOD             34 (get)
+               11910 EXTENDED_ARG             1
+               11912 LOAD_CONST             440 ('storage.s3.reduced_redundancy')
+               11914 LOAD_CONST              30 (False)
+               11916 PRECALL                  2
+               11920 CALL                     2
+               11930 EXTENDED_ARG             1
+               11932 STORE_NAME             272 (AWS_S3_REDUCED_REDUNDANCY)
+   
+   1039        11934 LOAD_NAME               29 (_settings)
+               11936 LOAD_METHOD             34 (get)
+               11958 EXTENDED_ARG             1
+               11960 LOAD_CONST             441 ('storage.s3.content_disposition')
+               11962 LOAD_CONST              81 ('')
+               11964 PRECALL                  2
+               11968 CALL                     2
+               11978 EXTENDED_ARG             1
+               11980 STORE_NAME             273 (AWS_S3_CONTENT_DISPOSITION)
+   
+   1040        11982 LOAD_NAME               29 (_settings)
+               11984 LOAD_METHOD             34 (get)
+               12006 EXTENDED_ARG             1
+               12008 LOAD_CONST             442 ('storage.s3.content_language')
+               12010 LOAD_CONST              81 ('')
+               12012 PRECALL                  2
+               12016 CALL                     2
+               12026 EXTENDED_ARG             1
+               12028 STORE_NAME             274 (AWS_S3_CONTENT_LANGUAGE)
+   
+   1041        12030 LOAD_NAME               29 (_settings)
+               12032 LOAD_METHOD             34 (get)
+               12054 EXTENDED_ARG             1
+               12056 LOAD_CONST             443 ('storage.s3.metadata')
+               12058 BUILD_MAP                0
+               12060 PRECALL                  2
+               12064 CALL                     2
+               12074 EXTENDED_ARG             1
+               12076 STORE_NAME             275 (AWS_S3_METADATA)
+   
+   1042        12078 LOAD_NAME               29 (_settings)
+               12080 LOAD_METHOD             34 (get)
+               12102 EXTENDED_ARG             1
+               12104 LOAD_CONST             444 ('storage.s3.encrypt_key')
+               12106 LOAD_CONST              30 (False)
+               12108 PRECALL                  2
+               12112 CALL                     2
+               12122 EXTENDED_ARG             1
+               12124 STORE_NAME             276 (AWS_S3_ENCRYPT_KEY)
+   
+   1043        12126 LOAD_NAME               29 (_settings)
+               12128 LOAD_METHOD             34 (get)
+               12150 EXTENDED_ARG             1
+               12152 LOAD_CONST             445 ('storage.s3.kms_encryption_key_id')
+               12154 LOAD_CONST              81 ('')
+               12156 PRECALL                  2
+               12160 CALL                     2
+               12170 EXTENDED_ARG             1
+               12172 STORE_NAME             277 (AWS_S3_KMS_ENCRYPTION_KEY_ID)
+   
+   1044        12174 LOAD_NAME               29 (_settings)
+               12176 LOAD_METHOD             34 (get)
+               12198 EXTENDED_ARG             1
+               12200 LOAD_CONST             446 ('storage.s3.gzip')
+               12202 LOAD_CONST              15 (True)
+               12204 PRECALL                  2
+               12208 CALL                     2
+               12218 EXTENDED_ARG             1
+               12220 STORE_NAME             278 (AWS_S3_GZIP)
+   
+   1045        12222 LOAD_NAME               29 (_settings)
+               12224 LOAD_METHOD             34 (get)
+               12246 EXTENDED_ARG             1
+               12248 LOAD_CONST             447 ('storage.s3.signature_version')
+               12250 LOAD_CONST               1 (None)
+               12252 PRECALL                  2
+               12256 CALL                     2
+               12266 EXTENDED_ARG             1
+               12268 STORE_NAME             279 (AWS_S3_SIGNATURE_VERSION)
+   
+   1046        12270 LOAD_NAME               29 (_settings)
+               12272 LOAD_METHOD             34 (get)
+               12294 EXTENDED_ARG             1
+               12296 LOAD_CONST             448 ('storage.s3.file_overwrite')
+               12298 LOAD_CONST              30 (False)
+               12300 PRECALL                  2
+               12304 CALL                     2
+               12314 EXTENDED_ARG             1
+               12316 STORE_NAME             280 (AWS_S3_FILE_OVERWRITE)
+   
+   1047        12318 LOAD_NAME               29 (_settings)
+               12320 LOAD_METHOD             34 (get)
+               12342 EXTENDED_ARG             1
+               12344 LOAD_CONST             449 ('storage.s3.verify')
+               12346 LOAD_CONST              15 (True)
+               12348 PRECALL                  2
+               12352 CALL                     2
                12362 EXTENDED_ARG             1
-               12364 LOAD_CONST             451 ('health.sentry.dsn')
-               12366 PRECALL                  1
-               12370 CALL                     1
-   
-   1056        12380 LOAD_NAME               29 (_settings)
-               12382 LOAD_METHOD             34 (get)
-               12404 EXTENDED_ARG             1
-               12406 LOAD_CONST             452 ('health.sentry.environment')
-               12408 PRECALL                  1
-               12412 CALL                     1
-   
-   1057        12422 LOAD_NAME               29 (_settings)
-               12424 LOAD_METHOD             34 (get)
-               12446 EXTENDED_ARG             1
-               12448 LOAD_CONST             453 ('health.sentry.traces_sample_rate')
-               12450 EXTENDED_ARG             1
-               12452 LOAD_CONST             454 (1.0)
-               12454 PRECALL                  2
-               12458 CALL                     2
-   
-   1058        12468 LOAD_NAME               29 (_settings)
-               12470 LOAD_METHOD             34 (get)
-               12492 EXTENDED_ARG             1
-               12494 LOAD_CONST             455 ('health.sentry.send_default_pii')
-               12496 LOAD_CONST              30 (False)
-               12498 PRECALL                  2
-               12502 CALL                     2
+               12364 STORE_NAME             281 (AWS_S3_VERIFY)
    
-   1059        12512 EXTENDED_ARG             1
-               12514 LOAD_CONST             456 ('aleksis-core@')
+   1048        12366 LOAD_NAME               29 (_settings)
+               12368 LOAD_METHOD             34 (get)
+               12390 EXTENDED_ARG             1
+               12392 LOAD_CONST             450 ('storage.s3.use_ssl')
+               12394 LOAD_CONST              15 (True)
+               12396 PRECALL                  2
+               12400 CALL                     2
+               12410 EXTENDED_ARG             1
+               12412 STORE_NAME             282 (AWS_S3_USE_SSL)
+               12414 JUMP_FORWARD             8 (to 12432)
+   
+   1050     >> 12416 EXTENDED_ARG             1
+               12418 LOAD_CONST             451 ('titofisto.TitofistoStorage')
+               12420 EXTENDED_ARG             1
+               12422 STORE_NAME             256 (DEFAULT_FILE_STORAGE)
+   
+   1051        12424 EXTENDED_ARG             1
+               12426 LOAD_CONST             452 (600)
+               12428 EXTENDED_ARG             1
+               12430 STORE_NAME             283 (TITOFISTO_TIMEOUT)
+   
+   1053     >> 12432 EXTENDED_ARG             1
+               12434 LOAD_NAME              256 (DEFAULT_FILE_STORAGE)
+               12436 EXTENDED_ARG             1
+               12438 STORE_NAME             284 (SASS_PROCESSOR_STORAGE)
+   
+   1055        12440 LOAD_NAME               29 (_settings)
+               12442 LOAD_METHOD             34 (get)
+               12464 EXTENDED_ARG             1
+               12466 LOAD_CONST             453 ('health.sentry.enabled')
+               12468 LOAD_CONST              30 (False)
+               12470 PRECALL                  2
+               12474 CALL                     2
+               12484 EXTENDED_ARG             1
+               12486 STORE_NAME             285 (SENTRY_ENABLED)
+   
+   1056        12488 EXTENDED_ARG             1
+               12490 LOAD_NAME              285 (SENTRY_ENABLED)
+               12492 POP_JUMP_FORWARD_IF_FALSE   199 (to 12892)
+   
+   1057        12494 LOAD_CONST               0 (0)
+               12496 LOAD_CONST               1 (None)
+               12498 EXTENDED_ARG             1
+               12500 IMPORT_NAME            286 (sentry_sdk)
+               12502 EXTENDED_ARG             1
+               12504 STORE_NAME             286 (sentry_sdk)
+   
+   1058        12506 LOAD_CONST               0 (0)
+               12508 EXTENDED_ARG             1
+               12510 LOAD_CONST             454 (('CeleryIntegration',))
+               12512 EXTENDED_ARG             1
+               12514 IMPORT_NAME            287 (sentry_sdk.integrations.celery)
                12516 EXTENDED_ARG             1
-               12518 LOAD_NAME              294 (__version__)
-               12520 FORMAT_VALUE             0
-               12522 BUILD_STRING             2
-   
-   1060        12524 LOAD_CONST              58 ('aleksis')
-   
-   1054        12526 EXTENDED_ARG             1
-               12528 LOAD_CONST             457 (('dsn', 'environment', 'traces_sample_rate', 'send_default_pii', 'release', 'in_app_include'))
-               12530 BUILD_CONST_KEY_MAP      6
+               12518 IMPORT_FROM            288 (CeleryIntegration)
+               12520 EXTENDED_ARG             1
+               12522 STORE_NAME             288 (CeleryIntegration)
+               12524 POP_TOP
+   
+   1059        12526 LOAD_CONST               0 (0)
+               12528 EXTENDED_ARG             1
+               12530 LOAD_CONST             455 (('DjangoIntegration',))
                12532 EXTENDED_ARG             1
-               12534 STORE_NAME             295 (SENTRY_SETTINGS)
+               12534 IMPORT_NAME            289 (sentry_sdk.integrations.django)
+               12536 EXTENDED_ARG             1
+               12538 IMPORT_FROM            290 (DjangoIntegration)
+               12540 EXTENDED_ARG             1
+               12542 STORE_NAME             290 (DjangoIntegration)
+               12544 POP_TOP
+   
+   1060        12546 LOAD_CONST               0 (0)
+               12548 EXTENDED_ARG             1
+               12550 LOAD_CONST             456 (('RedisIntegration',))
+               12552 EXTENDED_ARG             1
+               12554 IMPORT_NAME            291 (sentry_sdk.integrations.redis)
+               12556 EXTENDED_ARG             1
+               12558 IMPORT_FROM            292 (RedisIntegration)
+               12560 EXTENDED_ARG             1
+               12562 STORE_NAME             292 (RedisIntegration)
+               12564 POP_TOP
    
-   1062        12536 PUSH_NULL
-               12538 EXTENDED_ARG             1
-               12540 LOAD_NAME              286 (sentry_sdk)
-               12542 EXTENDED_ARG             1
-               12544 LOAD_ATTR              296 (init)
-               12554 EXTENDED_ARG             1
-               12556 LOAD_CONST             467 (())
-               12558 EXTENDED_ARG             1
-               12560 LOAD_CONST             458 ('integrations')
-   
-   1064        12562 PUSH_NULL
-               12564 EXTENDED_ARG             1
-               12566 LOAD_NAME              290 (DjangoIntegration)
+   1062        12566 LOAD_CONST               0 (0)
                12568 EXTENDED_ARG             1
-               12570 LOAD_CONST             459 ('function_name')
+               12570 LOAD_CONST             457 (('__version__',))
                12572 EXTENDED_ARG             1
-               12574 KW_NAMES               460
-               12576 PRECALL                  1
-               12580 CALL                     1
-   
-   1065        12590 PUSH_NULL
-               12592 EXTENDED_ARG             1
-               12594 LOAD_NAME              292 (RedisIntegration)
-               12596 PRECALL                  0
-               12600 CALL                     0
-   
-   1066        12610 PUSH_NULL
-               12612 EXTENDED_ARG             1
-               12614 LOAD_NAME              288 (CeleryIntegration)
-               12616 PRECALL                  0
-               12620 CALL                     0
-   
-   1063        12630 BUILD_LIST               3
-   
-   1062        12632 BUILD_MAP                1
-   
-   1068        12634 EXTENDED_ARG             1
-               12636 LOAD_NAME              295 (SENTRY_SETTINGS)
-   
-   1062        12638 DICT_MERGE               1
-               12640 CALL_FUNCTION_EX         1
-               12642 POP_TOP
-   
-   1071     >> 12644 EXTENDED_ARG             1
-               12646 LOAD_CONST             461 ('django_extensions.collision_resolvers.AppLabelPrefixCR')
-               12648 EXTENDED_ARG             1
-               12650 STORE_NAME             297 (SHELL_PLUS_MODEL_IMPORTS_RESOLVER)
-   
-   1073        12652 EXTENDED_ARG             1
-               12654 LOAD_CONST             462 ('auth')
-               12656 EXTENDED_ARG             1
-               12658 LOAD_CONST             462 ('auth')
-   
-   1072        12660 BUILD_MAP                1
-               12662 EXTENDED_ARG             1
-               12664 STORE_NAME             298 (SHELL_PLUS_APP_PREFIXES)
-   
-   1075        12666 BUILD_LIST               0
-               12668 EXTENDED_ARG             1
-               12670 STORE_NAME             299 (SHELL_PLUS_DONT_LOAD)
-   
-   1076        12672 PUSH_NULL
-               12674 LOAD_NAME               17 (merge_app_settings)
-               12676 EXTENDED_ARG             1
-               12678 LOAD_CONST             463 ('SHELL_PLUS_APP_PREFIXES')
-               12680 EXTENDED_ARG             1
-               12682 LOAD_NAME              298 (SHELL_PLUS_APP_PREFIXES)
-               12684 PRECALL                  2
-               12688 CALL                     2
-               12698 POP_TOP
-   
-   1077        12700 PUSH_NULL
-               12702 LOAD_NAME               17 (merge_app_settings)
-               12704 EXTENDED_ARG             1
-               12706 LOAD_CONST             464 ('SHELL_PLUS_DONT_LOAD')
-               12708 EXTENDED_ARG             1
-               12710 LOAD_NAME              299 (SHELL_PLUS_DONT_LOAD)
-               12712 PRECALL                  2
-               12716 CALL                     2
-               12726 POP_TOP
-   
-   1079        12728 EXTENDED_ARG             1
-               12730 LOAD_CONST             465 ('SAMEORIGIN')
-               12732 EXTENDED_ARG             1
-               12734 STORE_NAME             300 (X_FRAME_OPTIONS)
-   
-   1082        12736 LOAD_NAME               49 (INSTALLED_APPS)
-               12738 LOAD_METHOD             67 (append)
-               12760 EXTENDED_ARG             1
-               12762 LOAD_CONST             466 ('django_cleanup.apps.CleanupConfig')
-               12764 PRECALL                  1
-               12768 CALL                     1
-               12778 POP_TOP
-   
-   1084        12780 PUSH_NULL
-               12782 EXTENDED_ARG             1
-               12784 LOAD_NAME              301 (locals)
-               12786 PRECALL                  0
-               12790 CALL                     0
-               12800 EXTENDED_ARG             1
-               12802 LOAD_METHOD            302 (update)
-               12824 PUSH_NULL
-               12826 LOAD_NAME               16 (get_app_settings_overrides)
-               12828 PRECALL                  0
-               12832 CALL                     0
-               12842 PRECALL                  1
-               12846 CALL                     1
-               12856 POP_TOP
-               12858 LOAD_CONST               1 (None)
-               12860 RETURN_VALUE
+               12574 IMPORT_NAME            293 (aleksis.core)
+               12576 EXTENDED_ARG             1
+               12578 IMPORT_FROM            294 (__version__)
+               12580 EXTENDED_ARG             1
+               12582 STORE_NAME             294 (__version__)
+               12584 POP_TOP
+   
+   1065        12586 LOAD_NAME               29 (_settings)
+               12588 LOAD_METHOD             34 (get)
+               12610 EXTENDED_ARG             1
+               12612 LOAD_CONST             458 ('health.sentry.dsn')
+               12614 PRECALL                  1
+               12618 CALL                     1
+   
+   1066        12628 LOAD_NAME               29 (_settings)
+               12630 LOAD_METHOD             34 (get)
+               12652 EXTENDED_ARG             1
+               12654 LOAD_CONST             459 ('health.sentry.environment')
+               12656 PRECALL                  1
+               12660 CALL                     1
+   
+   1067        12670 LOAD_NAME               29 (_settings)
+               12672 LOAD_METHOD             34 (get)
+               12694 EXTENDED_ARG             1
+               12696 LOAD_CONST             460 ('health.sentry.traces_sample_rate')
+               12698 EXTENDED_ARG             1
+               12700 LOAD_CONST             461 (1.0)
+               12702 PRECALL                  2
+               12706 CALL                     2
+   
+   1068        12716 LOAD_NAME               29 (_settings)
+               12718 LOAD_METHOD             34 (get)
+               12740 EXTENDED_ARG             1
+               12742 LOAD_CONST             462 ('health.sentry.send_default_pii')
+               12744 LOAD_CONST              30 (False)
+               12746 PRECALL                  2
+               12750 CALL                     2
+   
+   1069        12760 EXTENDED_ARG             1
+               12762 LOAD_CONST             463 ('aleksis-core@')
+               12764 EXTENDED_ARG             1
+               12766 LOAD_NAME              294 (__version__)
+               12768 FORMAT_VALUE             0
+               12770 BUILD_STRING             2
+   
+   1070        12772 LOAD_CONST              58 ('aleksis')
+   
+   1064        12774 EXTENDED_ARG             1
+               12776 LOAD_CONST             464 (('dsn', 'environment', 'traces_sample_rate', 'send_default_pii', 'release', 'in_app_include'))
+               12778 BUILD_CONST_KEY_MAP      6
+               12780 EXTENDED_ARG             1
+               12782 STORE_NAME             295 (SENTRY_SETTINGS)
+   
+   1072        12784 PUSH_NULL
+               12786 EXTENDED_ARG             1
+               12788 LOAD_NAME              286 (sentry_sdk)
+               12790 EXTENDED_ARG             1
+               12792 LOAD_ATTR              296 (init)
+               12802 EXTENDED_ARG             1
+               12804 LOAD_CONST             474 (())
+               12806 EXTENDED_ARG             1
+               12808 LOAD_CONST             465 ('integrations')
+   
+   1074        12810 PUSH_NULL
+               12812 EXTENDED_ARG             1
+               12814 LOAD_NAME              290 (DjangoIntegration)
+               12816 EXTENDED_ARG             1
+               12818 LOAD_CONST             466 ('function_name')
+               12820 EXTENDED_ARG             1
+               12822 KW_NAMES               467
+               12824 PRECALL                  1
+               12828 CALL                     1
+   
+   1075        12838 PUSH_NULL
+               12840 EXTENDED_ARG             1
+               12842 LOAD_NAME              292 (RedisIntegration)
+               12844 PRECALL                  0
+               12848 CALL                     0
+   
+   1076        12858 PUSH_NULL
+               12860 EXTENDED_ARG             1
+               12862 LOAD_NAME              288 (CeleryIntegration)
+               12864 PRECALL                  0
+               12868 CALL                     0
+   
+   1073        12878 BUILD_LIST               3
+   
+   1072        12880 BUILD_MAP                1
+   
+   1078        12882 EXTENDED_ARG             1
+               12884 LOAD_NAME              295 (SENTRY_SETTINGS)
+   
+   1072        12886 DICT_MERGE               1
+               12888 CALL_FUNCTION_EX         1
+               12890 POP_TOP
+   
+   1081     >> 12892 EXTENDED_ARG             1
+               12894 LOAD_CONST             468 ('django_extensions.collision_resolvers.AppLabelPrefixCR')
+               12896 EXTENDED_ARG             1
+               12898 STORE_NAME             297 (SHELL_PLUS_MODEL_IMPORTS_RESOLVER)
+   
+   1083        12900 EXTENDED_ARG             1
+               12902 LOAD_CONST             469 ('auth')
+               12904 EXTENDED_ARG             1
+               12906 LOAD_CONST             469 ('auth')
+   
+   1082        12908 BUILD_MAP                1
+               12910 EXTENDED_ARG             1
+               12912 STORE_NAME             298 (SHELL_PLUS_APP_PREFIXES)
+   
+   1085        12914 BUILD_LIST               0
+               12916 EXTENDED_ARG             1
+               12918 STORE_NAME             299 (SHELL_PLUS_DONT_LOAD)
+   
+   1086        12920 PUSH_NULL
+               12922 LOAD_NAME               17 (merge_app_settings)
+               12924 EXTENDED_ARG             1
+               12926 LOAD_CONST             470 ('SHELL_PLUS_APP_PREFIXES')
+               12928 EXTENDED_ARG             1
+               12930 LOAD_NAME              298 (SHELL_PLUS_APP_PREFIXES)
+               12932 PRECALL                  2
+               12936 CALL                     2
+               12946 POP_TOP
+   
+   1087        12948 PUSH_NULL
+               12950 LOAD_NAME               17 (merge_app_settings)
+               12952 EXTENDED_ARG             1
+               12954 LOAD_CONST             471 ('SHELL_PLUS_DONT_LOAD')
+               12956 EXTENDED_ARG             1
+               12958 LOAD_NAME              299 (SHELL_PLUS_DONT_LOAD)
+               12960 PRECALL                  2
+               12964 CALL                     2
+               12974 POP_TOP
+   
+   1089        12976 EXTENDED_ARG             1
+               12978 LOAD_CONST             472 ('SAMEORIGIN')
+               12980 EXTENDED_ARG             1
+               12982 STORE_NAME             300 (X_FRAME_OPTIONS)
+   
+   1092        12984 LOAD_NAME               49 (INSTALLED_APPS)
+               12986 LOAD_METHOD             67 (append)
+               13008 EXTENDED_ARG             1
+               13010 LOAD_CONST             473 ('django_cleanup.apps.CleanupConfig')
+               13012 PRECALL                  1
+               13016 CALL                     1
+               13026 POP_TOP
+   
+   1094        13028 PUSH_NULL
+               13030 EXTENDED_ARG             1
+               13032 LOAD_NAME              301 (locals)
+               13034 PRECALL                  0
+               13038 CALL                     0
+               13048 EXTENDED_ARG             1
+               13050 LOAD_METHOD            302 (update)
+               13072 PUSH_NULL
+               13074 LOAD_NAME               16 (get_app_settings_overrides)
+               13076 PRECALL                  0
+               13080 CALL                     0
+               13090 PRECALL                  1
+               13094 CALL                     1
+               13104 POP_TOP
+               13106 LOAD_CONST               1 (None)
+               13108 RETURN_VALUE
    ExceptionTable:
      3782 to 3828 -> 3854 [1] lasti
      3854 to 3860 -> 3862 [3] lasti
      3868 to 3868 -> 3862 [3] lasti
    consts
       0
       None
@@ -4638,30 +4715,37 @@
       ('href', 'title', 'style')
       ('font-family', 'font-weight', 'text-decoration', 'font-variant')
       'console'
       'logging.level'
       'WARNING'
       ('handlers', 'level')
       'root'
+      '{asctime} {levelname} {name}[{process}]: {msg}'
+      '{'
+      ('format', 'style')
+      'formatters'
+      'verbose'
       'class'
       'logging.NullHandler'
       'handlers'
       'null'
       'filters'
       'require_debug_true'
       'level'
+      'formatter'
       'logging.mail_admins'
       'loggers'
       'django'
       'mail_admins'
       'logging.disallowed_host'
       ('handlers', 'propagate')
       'django.security.DisallowedHost'
       ('handlers', 'level', 'propagate')
       'celery'
+      'django.server'
       'guardian.W001'
       'rules.permissions.ObjectPermissionBackend'
       'haystack_redis.RedisEngine'
       ('ENGINE', 'PATH')
       'celery_haystack.signals.CelerySignalProcessor'
       'health.disk_usage_max_percent'
       90
@@ -4765,15 +4849,15 @@
       0206ff04045c01060206014eff1204100206022e0206022e010a01180130
       0104fe100406022e010a011801300104fe100406022e012c012c012c0230
       022e0106010601060104022e0106022e0130012e0140013a013a03360136
       fe08050a010801060106fc080638020801060106fd08063802040302010a
       03040108fe0605040108fe060d1202040108fe060c0202040108fe060e04
       0108fe06161201020112011401140110020402040104fe02fe06b7025104
       0104011a0108ff0eab06ff046b06030a030a040a0404030402160306012e
-      fe10052202560224022e0156022e02060102fe1e0606012e0102fd1e0804
-      0104022c032c030201040102fe06ff040706010402060204032e012efe08
-      053001300204012e012e020603040104fe04055e012c0208012c022e0108
-      013001180106ff1204300130013001300130013001320130013001300130
-      013001300130013001300130013001300130013001300132020801080208
-      02300106010c0114011401140214032a012a012e012c010c0102fa0a081a
-      021c01140114fd02ff020604fa0609080208ff060306011c011c0208032c
-      02
+      fe1006040104fe1e052202560224022a022e0156022e02060102fe1e0606
+      012e0102fd1e0654015404040104022c032c030201040102fe06ff040706
+      010402060204032e012efe08053001300204012e012e020603040104fe04
+      055e012c0208012c022e0108013001180106ff1204300130013001300130
+      013001320130013001300130013001300130013001300130013001300130
+      01300130013202080108020802300106010c0114011401140214032a012a
+      012e012c010c0102fa0a081a021c01140114fd02ff020604fa0609080208
+      ff060306011c011c0208032c02
```

### Comparing `aleksis_core-3.1.1/aleksis/core/__pycache__/tasks.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/__pycache__/tasks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 2330
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/admin.py` & `aleksis_core-3.1.2/aleksis/core/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/apps.py` & `aleksis_core-3.1.2/aleksis/core/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/celery.py` & `aleksis_core-3.1.2/aleksis/core/celery.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/checks.py` & `aleksis_core-3.1.2/aleksis/core/checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/data_checks.py` & `aleksis_core-3.1.2/aleksis/core/data_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/decorators.py` & `aleksis_core-3.1.2/aleksis/core/decorators.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/filters.py` & `aleksis_core-3.1.2/aleksis/core/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/forms.py` & `aleksis_core-3.1.2/aleksis/core/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/app/apollo.js` & `aleksis_core-3.1.2/aleksis/core/frontend/app/apollo.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/app/dateTimeFormats.js` & `aleksis_core-3.1.2/aleksis/core/frontend/app/dateTimeFormats.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/app/vuetify.js` & `aleksis_core-3.1.2/aleksis/core/frontend/app/vuetify.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/LegacyBaseTemplate.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/LegacyBaseTemplate.vue`

 * *Files 13% similar despite different names*

```diff
@@ -17,18 +17,17 @@
     "
     type="error"
   >
     {{ $t("legacy.unworthy") }}
   </message-box>
   <iframe
     v-else
-    :src="'/django' + $route.path + queryString"
+    :src="iFrameSrc"
     :height="iFrameHeight + 'px'"
     class="iframe-fullsize"
-    @load="load"
     ref="contentIFrame"
   ></iframe>
 </template>
 
 <script>
 export default {
   props: {
@@ -37,33 +36,37 @@
         type: Boolean,
         required: true,
       },
   },
   data: function () {
     return {
       iFrameHeight: 0,
+      iFrameSrc: undefined,
     };
   },
   computed: {
     queryString() {
       let qs = [];
       for (const [param, value] of Object.entries(this.$route.query)) {
         qs.push(`${param}=${encodeURIComponent(value)}`);
       }
       return "?" + qs.join("&");
     },
   },
   methods: {
+    getIFrameURL() {
+      const location = this.$refs.contentIFrame.contentWindow.location;
+      const url = new URL(location);
+      return url;
+    },
     /** Handle iframe data after inner page loaded */
     load() {
       // Write new location of iframe back to Vue Router
-      const location = this.$refs.contentIFrame.contentWindow.location;
-      const url = new URL(location);
-      const path = url.pathname.replace(/^\/django/, "");
-      const pathWithQueryString = path + encodeURI(url.search);
+      const path = this.getIFrameURL().pathname.replace(/^\/django/, "");
+      const pathWithQueryString = path + encodeURI(this.getIFrameURL().search);
       const routePath =
         path.charAt(path.length - 1) === "/" &&
         this.$route.path.charAt(path.length - 1) !== "/"
           ? this.$route.path + "/"
           : this.$route.path;
       if (path !== routePath) {
         this.$router.push(pathWithQueryString);
@@ -99,23 +102,44 @@
         }).observe(this.$refs.contentIFrame.contentDocument.body);
       }
 
       this.$root.contentLoading = false;
     },
   },
   watch: {
-    $route() {
+    $route(newRoute) {
       // Show loading animation once route changes
       this.$root.contentLoading = true;
 
+      // Only reload iFrame content when navigation comes from outsite the iFrame
+      const path = this.getIFrameURL().pathname.replace(/^\/django/, "");
+      const routePath =
+        path.charAt(path.length - 1) === "/" &&
+        newRoute.path.charAt(path.length - 1) !== "/"
+          ? newRoute.path + "/"
+          : newRoute.path;
+
+      if (path !== routePath) {
+        this.$refs.contentIFrame.contentWindow.location =
+          "/django" + this.$route.path + this.queryString;
+      } else {
+        this.$root.contentLoading = false;
+      }
+
       // Scroll to top only when route changes to not affect form submits etc.
       // A small duration to avoid flashing of the UI
       this.$vuetify.goTo(0, { duration: 10 });
     },
   },
+  mounted() {
+    this.$refs.contentIFrame.addEventListener("load", (e) => {
+      this.load();
+    });
+    this.iFrameSrc = "/django" + this.$route.path + this.queryString;
+  },
   name: "LegacyBaseTemplate",
 };
 </script>
 
 <style scoped>
 .iframe-fullsize {
   border: 0;
```

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/about/AboutAleksis.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/about/AboutAleksis.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/about/InstalledAppCard.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/about/InstalledAppCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/about/InstalledAppsList.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/about/InstalledAppsList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/app/AccountMenu.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/app/AccountMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/app/App.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/app/App.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/app/ErrorPage.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/app/ErrorPage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/app/LanguageForm.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/app/LanguageForm.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/app/SideNav.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/app/SideNav.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/app/SidenavSearch.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/app/SidenavSearch.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/app/SnackbarItem.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/app/SnackbarItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/app/Splash.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/app/Splash.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/celery_progress/TaskListItem.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/celery_progress/TaskListItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/generic/AvatarClickbox.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/AvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/generic/ButtonMenu.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/ButtonMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/generic/DetailView.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/DetailView.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/generic/ObjectOverview.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/ObjectOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/generic/UpdateIndicator.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/UpdateIndicator.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/group/GroupCollection.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/group/GroupCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/notifications/NotificationItem.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/NotificationItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/notifications/NotificationList.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/notifications/NotificationList.vue`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         class="mx-2"
       >
         <v-icon
           color="white"
           v-if="
             myNotifications &&
             myNotifications.person &&
-            myNotifications.person.notifications.length > 0
+            unreadNotifications.length > 0
           "
         >
           mdi-bell-badge-outline
         </v-icon>
         <v-icon color="white" v-else>mdi-bell-outline</v-icon>
       </v-btn>
     </template>
@@ -34,15 +34,15 @@
       type="paragraph"
     ></v-skeleton-loader>
     <v-list v-else nav three-line dense class="overflow-y-auto">
       <template
         v-if="
           myNotifications.person &&
           myNotifications.person.notifications &&
-          unreadNotifications.length
+          myNotifications.person.notifications.length
         "
       >
         <v-subheader>{{ $t("notifications.notifications") }}</v-subheader>
         <template v-for="notification in myNotifications.person.notifications">
           <NotificationItem
             :key="notification.id"
             :notification="notification"
@@ -84,12 +84,14 @@
     myNotifications: {
       query: gqlMyNotifications,
       pollInterval: 30000,
     },
   },
   computed: {
     unreadNotifications() {
-      return this.myNotifications.filter((n) => !n.read);
+      return this.myNotifications.person.notifications
+        ? this.myNotifications.person.notifications.filter((n) => !n.read)
+        : [];
     },
   },
 };
 </script>
```

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/pdf/DownloadPDF.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/pdf/DownloadPDF.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/person/AdditionalImage.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/person/AdditionalImage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/person/AvatarContent.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/person/AvatarContent.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/person/PersonActions.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonActions.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/person/PersonCollection.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/person/PersonOverview.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/person/PersonOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/person/personOverview.graphql` & `aleksis_core-3.1.2/aleksis/core/frontend/components/person/personOverview.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/two_factor/TwoFactor.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactor.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue` & `aleksis_core-3.1.2/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/index.js` & `aleksis_core-3.1.2/aleksis/core/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/messages/de.json` & `aleksis_core-3.1.2/aleksis/core/frontend/messages/de.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/messages/en.json` & `aleksis_core-3.1.2/aleksis/core/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/messages/ru.json` & `aleksis_core-3.1.2/aleksis/core/frontend/messages/ru.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/messages/uk.json` & `aleksis_core-3.1.2/aleksis/core/frontend/messages/uk.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/mixins/aleksis.js` & `aleksis_core-3.1.2/aleksis/core/frontend/mixins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/mixins/error404.js` & `aleksis_core-3.1.2/aleksis/core/frontend/mixins/error404.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/mixins/menus.js` & `aleksis_core-3.1.2/aleksis/core/frontend/mixins/menus.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/mixins/offline.js` & `aleksis_core-3.1.2/aleksis/core/frontend/mixins/offline.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/mixins/permissions.js` & `aleksis_core-3.1.2/aleksis/core/frontend/mixins/permissions.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/mixins/routes.js` & `aleksis_core-3.1.2/aleksis/core/frontend/mixins/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/mixins/useRegisterSW.js` & `aleksis_core-3.1.2/aleksis/core/frontend/mixins/useRegisterSW.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/plugins/aleksis.js` & `aleksis_core-3.1.2/aleksis/core/frontend/plugins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/frontend/routes.js` & `aleksis_core-3.1.2/aleksis/core/frontend/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/health_checks.py` & `aleksis_core-3.1.2/aleksis/core/health_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/ar/LC_MESSAGES/django.po` & `aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.2/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/fr/LC_MESSAGES/django.mo` & `aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/fr/LC_MESSAGES/django.po` & `aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.2/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/la/LC_MESSAGES/django.mo` & `aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/la/LC_MESSAGES/django.po` & `aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/la/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.2/aleksis/core/locale/la/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.2/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/ru/LC_MESSAGES/django.mo` & `aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/ru/LC_MESSAGES/django.po` & `aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.2/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/uk/LC_MESSAGES/django.mo` & `aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/uk/LC_MESSAGES/django.po` & `aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po` & `aleksis_core-3.1.2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/management/commands/convert_urls_to_routes.py` & `aleksis_core-3.1.2/aleksis/core/management/commands/convert_urls_to_routes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/management/commands/vite.py` & `aleksis_core-3.1.2/aleksis/core/management/commands/vite.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/managers.py` & `aleksis_core-3.1.2/aleksis/core/managers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0001_initial.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0002_school_term.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0002_school_term.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0003_drop_image_cropping.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0003_drop_image_cropping.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0004_add_permissions_for_group_stats.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0004_add_permissions_for_group_stats.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0005_timestamped_activity_notification.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0005_timestamped_activity_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0006_dashboard_widget_size.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0006_dashboard_widget_size.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0007_dashboard_widget_order.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0007_dashboard_widget_order.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0008_data_check_result.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0008_data_check_result.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0009_default_dashboard.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0009_default_dashboard.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0010_external_link_widget.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0010_external_link_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0011_globalpermissions_options.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0011_globalpermissions_options.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0013_pdf_file.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0013_pdf_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0014_alter_pdffile_file.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0014_alter_pdffile_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0015_oauth_permissions.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0015_oauth_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0016_taskuserassignment.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0016_taskuserassignment.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0018_pdffile_html_file.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0018_pdffile_html_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0019_fix_uniqueness_per_site.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0019_fix_uniqueness_per_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0020_pdf_file_person_optional.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0020_pdf_file_person_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0021_drop_persons_accounts_perm.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0021_drop_persons_accounts_perm.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0022_public_favicon.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0022_public_favicon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0023_oauth_application_model.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0023_oauth_application_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0024_oauth_grant_types_optional.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0024_oauth_grant_types_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0025_oauth_align_user_fk.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0025_oauth_align_user_fk.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0028_char_field_not_null.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0028_char_field_not_null.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0029_invitations.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0029_invitations.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0030_user_attributes.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0030_user_attributes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0031_oauthapplication_icon.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0031_oauthapplication_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0033_update_photo_avatar.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0033_update_photo_avatar.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0034_invite_permission.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0034_invite_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0035_preference_model_unique.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0035_preference_model_unique.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0036_additionalfields_helptext_required.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0036_additionalfields_helptext_required.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0037_add_static_content_widget.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0037_add_static_content_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0038_notification_send_at.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0038_notification_send_at.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0039_personal_ical_url.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0039_personal_ical_url.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0041_update_gender_choices.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0041_update_gender_choices.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0042_pdffile_empty.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0042_pdffile_empty.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0043_task_assignment_meta.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0043_task_assignment_meta.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0044_task_assignment_result_fetched.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0044_task_assignment_result_fetched.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0046_notification_create_field_icon.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0046_notification_create_field_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0047_add_room_model.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0047_add_room_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0048_delete_personalicalurl.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0048_delete_personalicalurl.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py` & `aleksis_core-3.1.2/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/mixins.py` & `aleksis_core-3.1.2/aleksis/core/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 import reversion
 from dynamic_preferences.settings import preferences_settings
 from dynamic_preferences.types import FilePreference
 from guardian.admin import GuardedModelAdmin
 from guardian.core import ObjectPermissionChecker
 from jsonstore.fields import IntegerField, JSONFieldMixin
-from material.base import Layout, LayoutNode
+from material.base import Fieldset, Layout, LayoutNode
 from polymorphic.base import PolymorphicModelBase
 from polymorphic.managers import PolymorphicManager
 from polymorphic.models import PolymorphicModel
 from rules.contrib.admin import ObjectPermissionsModelAdmin
 
 from aleksis.core.managers import (
     CurrentSiteManagerWithoutMigrations,
@@ -445,14 +445,28 @@
 
         :param node: django-material layout node (Fieldset, Row etc.)
         :type node: LayoutNode
         """
         cls.base_layout.append(node)
         cls.layout = Layout(*cls.base_layout)
 
+        visit_nodes = [node]
+        while visit_nodes:
+            current_node = visit_nodes.pop()
+            if isinstance(current_node, Fieldset):
+                visit_nodes += node.elements
+            else:
+                field_name = (
+                    current_node if isinstance(current_node, str) else current_node.field_name
+                )
+                field = fields_for_model(cls._meta.model, [field_name])[field_name]
+                cls._meta.fields.append(field_name)
+                cls.base_fields[field_name] = field
+                setattr(cls, field_name, field)
+
 
 class BaseModelAdmin(GuardedModelAdmin, ObjectPermissionsModelAdmin):
     """A base class for ModelAdmin combining django-guardian and rules."""
 
     pass
```

### Comparing `aleksis_core-3.1.1/aleksis/core/models.py` & `aleksis_core-3.1.2/aleksis/core/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/preferences.py` & `aleksis_core-3.1.2/aleksis/core/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/registries.py` & `aleksis_core-3.1.2/aleksis/core/registries.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/rules.py` & `aleksis_core-3.1.2/aleksis/core/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/__init__.py` & `aleksis_core-3.1.2/aleksis/core/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/base.py` & `aleksis_core-3.1.2/aleksis/core/schema/base.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/celery_progress.py` & `aleksis_core-3.1.2/aleksis/core/schema/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/custom_menu.py` & `aleksis_core-3.1.2/aleksis/core/schema/custom_menu.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/group.py` & `aleksis_core-3.1.2/aleksis/core/schema/group.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/installed_apps.py` & `aleksis_core-3.1.2/aleksis/core/schema/installed_apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/notification.py` & `aleksis_core-3.1.2/aleksis/core/schema/notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/oauth.py` & `aleksis_core-3.1.2/aleksis/core/schema/oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/pdf.py` & `aleksis_core-3.1.2/aleksis/core/schema/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/person.py` & `aleksis_core-3.1.2/aleksis/core/schema/person.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/search.py` & `aleksis_core-3.1.2/aleksis/core/schema/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/site_preferences.py` & `aleksis_core-3.1.2/aleksis/core/schema/site_preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/system_properties.py` & `aleksis_core-3.1.2/aleksis/core/schema/system_properties.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/two_factor.py` & `aleksis_core-3.1.2/aleksis/core/schema/two_factor.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/schema/user.py` & `aleksis_core-3.1.2/aleksis/core/schema/user.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/settings.py` & `aleksis_core-3.1.2/aleksis/core/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -931,20 +931,27 @@
 
 LOGGING = deepcopy(DEFAULT_LOGGING)
 # Set root logging level as default
 LOGGING["root"] = {
     "handlers": ["console"],
     "level": _settings.get("logging.level", "WARNING"),
 }
+# Configure global log Format
+LOGGING["formatters"]["verbose"] = {
+    "format": "{asctime} {levelname} {name}[{process}]: {msg}",
+    "style": "{",
+}
 # Add null handler for selective silencing
 LOGGING["handlers"]["null"] = {"class": "logging.NullHandler"}
 # Make console logging independent of DEBUG
 LOGGING["handlers"]["console"]["filters"].remove("require_debug_true")
 # Use root log level for console
 del LOGGING["handlers"]["console"]["level"]
+# Use verbose log format for console
+LOGGING["handlers"]["console"]["formatter"] = "verbose"
 # Disable exception mails if not desired
 if not _settings.get("logging.mail_admins", True):
     LOGGING["loggers"]["django"]["handlers"].remove("mail_admins")
 # Disable mails on disaalowed host by default
 if not _settings.get("logging.disallowed_host", False):
     LOGGING["loggers"]["django.security.DisallowedHost"] = {
         "handlers": ["null"],
@@ -952,14 +959,17 @@
     }
 # Configure logging explicitly for Celery
 LOGGING["loggers"]["celery"] = {
     "handlers": ["console"],
     "level": _settings.get("logging.level", "WARNING"),
     "propagate": False,
 }
+# Set Django log levels
+LOGGING["loggers"]["django"]["level"] = _settings.get("logging.level", "WARNING")
+LOGGING["loggers"]["django.server"]["level"] = _settings.get("logging.level", "WARNING")
 
 # Rules and permissions
 
 GUARDIAN_RAISE_403 = True
 ANONYMOUS_USER_NAME = None
 
 SILENCED_SYSTEM_CHECKS.append("guardian.W001")
```

### Comparing `aleksis_core-3.1.1/aleksis/core/static/img/aleksis-banner.svg` & `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-banner.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/img/aleksis-favicon.png` & `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-favicon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/img/aleksis-icon-maskable.png` & `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon-maskable.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/img/aleksis-icon-maskable.svg` & `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon-maskable.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/img/aleksis-icon.png` & `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/img/aleksis-icon.svg` & `aleksis_core-3.1.2/aleksis/core/static/img/aleksis-icon.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/img/fallback.png` & `aleksis_core-3.1.2/aleksis/core/static/img/fallback.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/img/hero.svg` & `aleksis_core-3.1.2/aleksis/core/static/img/hero.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/js/edit_dashboard.js` & `aleksis_core-3.1.2/aleksis/core/static/js/edit_dashboard.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/js/helper.js` & `aleksis_core-3.1.2/aleksis/core/static/js/helper.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/js/include_ajax_live.js` & `aleksis_core-3.1.2/aleksis/core/static/js/include_ajax_live.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/js/main.js` & `aleksis_core-3.1.2/aleksis/core/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/js/multi_select.js` & `aleksis_core-3.1.2/aleksis/core/static/js/multi_select.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/js/search.js` & `aleksis_core-3.1.2/aleksis/core/static/js/search.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/js/serviceworker.js` & `aleksis_core-3.1.2/aleksis/core/static/js/serviceworker.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/print.css` & `aleksis_core-3.1.2/aleksis/core/static/print.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/public/materialize-custom.scss` & `aleksis_core-3.1.2/aleksis/core/static/public/materialize-custom.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/public/style.scss` & `aleksis_core-3.1.2/aleksis/core/static/public/style.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/static/public/theme.scss` & `aleksis_core-3.1.2/aleksis/core/static/public/theme.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tables.py` & `aleksis_core-3.1.2/aleksis/core/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tasks.py` & `aleksis_core-3.1.2/aleksis/core/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/403.html` & `aleksis_core-3.1.2/aleksis/core/templates/403.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/404.html` & `aleksis_core-3.1.2/aleksis/core/templates/404.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/500.html` & `aleksis_core-3.1.2/aleksis/core/templates/500.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/account_inactive.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/account_inactive.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/email/email_confirmation_message.txt` & `aleksis_core-3.1.2/aleksis/core/templates/account/email/email_confirmation_message.txt`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/email_confirm.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/password_change.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/password_change_disabled.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/password_change_disabled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/password_reset.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/password_reset_done.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/password_reset_from_key.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/password_reset_from_key_done.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/password_reset_from_key_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/signup.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/signup_closed.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/verification_email_required.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/verification_email_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/account/verification_sent.html` & `aleksis_core-3.1.2/aleksis/core/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/components/chips.html` & `aleksis_core-3.1.2/aleksis/core/templates/components/chips.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/components/pagination.html` & `aleksis_core-3.1.2/aleksis/core/templates/components/pagination.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/additional_field/list.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/additional_field/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/announcement/form.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/announcement/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/announcement/list.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/announcement/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/base.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/base.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/base_print.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/base_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/base_simple_print.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/base_simple_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/dashboard_widget/create.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/dashboard_widget/edit.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/dashboard_widget/list.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/dashboard_widget/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/data_check/list.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/data_check/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/edit_dashboard.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/edit_dashboard.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/group/child_groups.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/group/child_groups.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/group/edit.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/group/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/group/full.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/group/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/group/list.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/group/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/group_type/list.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/group_type/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/index.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/pages/delete.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/pages/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/pages/system_status.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/pages/system_status.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/pages/test_pdf.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/pages/test_pdf.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/partials/announcements.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/partials/announcements.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/partials/avatar_content.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/partials/avatar_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/partials/crud_events.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/partials/crud_events.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/partials/meta.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/partials/meta.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/partials/splash_screen.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/partials/splash_screen.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/perms/assign.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/perms/assign.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/perms/list.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/perms/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/person/create.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/person/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/person/edit.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/person/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/person/list.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/person/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/school_term/list.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/school_term/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/core/vue_index.html` & `aleksis_core-3.1.2/aleksis/core/templates/core/vue_index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/django_tables2/materialize.html` & `aleksis_core-3.1.2/aleksis/core/templates/django_tables2/materialize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/dynamic_preferences/form.html` & `aleksis_core-3.1.2/aleksis/core/templates/dynamic_preferences/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/invitations/disabled.html` & `aleksis_core-3.1.2/aleksis/core/templates/invitations/disabled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/invitations/enter.html` & `aleksis_core-3.1.2/aleksis/core/templates/invitations/enter.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/invitations/forms/_invite.html` & `aleksis_core-3.1.2/aleksis/core/templates/invitations/forms/_invite.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html` & `aleksis_core-3.1.2/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/material/fields/colorfield_colorwidget.html` & `aleksis_core-3.1.2/aleksis/core/templates/material/fields/colorfield_colorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html` & `aleksis_core-3.1.2/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/material/fields/django_select2_select2widget.html` & `aleksis_core-3.1.2/aleksis/core/templates/material/fields/django_select2_select2widget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/oauth2_provider/application/create.html` & `aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/oauth2_provider/application/detail.html` & `aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/oauth2_provider/application/edit.html` & `aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/oauth2_provider/application/list.html` & `aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/application/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/oauth2_provider/authorize.html` & `aleksis_core-3.1.2/aleksis/core/templates/oauth2_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/offline.html` & `aleksis_core-3.1.2/aleksis/core/templates/offline.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/search/search.html` & `aleksis_core-3.1.2/aleksis/core/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/socialaccount/authentication_error.html` & `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/authentication_error.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/socialaccount/connections.html` & `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/socialaccount/login.html` & `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/socialaccount/login_cancelled.html` & `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/login_cancelled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/socialaccount/signup.html` & `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/socialaccount/snippets/provider_list.html` & `aleksis_core-3.1.2/aleksis/core/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/templated_email/base.email` & `aleksis_core-3.1.2/aleksis/core/templates/templated_email/base.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/templated_email/celery_failure.email` & `aleksis_core-3.1.2/aleksis/core/templates/templated_email/celery_failure.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/templated_email/data_checks.email` & `aleksis_core-3.1.2/aleksis/core/templates/templated_email/data_checks.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/templated_email/email.css` & `aleksis_core-3.1.2/aleksis/core/templates/templated_email/email.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/templated_email/invitation.email` & `aleksis_core-3.1.2/aleksis/core/templates/templated_email/invitation.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/templated_email/notification.email` & `aleksis_core-3.1.2/aleksis/core/templates/templated_email/notification.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/templated_email/person_changed.email` & `aleksis_core-3.1.2/aleksis/core/templates/templated_email/person_changed.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/two_factor/_wizard_actions.html` & `aleksis_core-3.1.2/aleksis/core/templates/two_factor/_wizard_actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/backup_tokens.html` & `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/login.html` & `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/otp_required.html` & `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/phone_register.html` & `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/phone_register.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/setup.html` & `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/two_factor/core/setup_complete.html` & `aleksis_core-3.1.2/aleksis/core/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templates/two_factor/profile/disable.html` & `aleksis_core-3.1.2/aleksis/core/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templatetags/data_helpers.py` & `aleksis_core-3.1.2/aleksis/core/templatetags/data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/templatetags/html_helpers.py` & `aleksis_core-3.1.2/aleksis/core/templatetags/html_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tests/browser/test_selenium.py` & `aleksis_core-3.1.2/aleksis/core/tests/browser/test_selenium.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tests/models/test.pdf` & `aleksis_core-3.1.2/aleksis/core/tests/models/test.pdf`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tests/models/test_group.py` & `aleksis_core-3.1.2/aleksis/core/tests/models/test_group.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tests/models/test_group_sync.py` & `aleksis_core-3.1.2/aleksis/core/tests/models/test_group_sync.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tests/models/test_notification.py` & `aleksis_core-3.1.2/aleksis/core/tests/models/test_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tests/models/test_pdffile.py` & `aleksis_core-3.1.2/aleksis/core/tests/models/test_pdffile.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tests/regression/test_regression.py` & `aleksis_core-3.1.2/aleksis/core/tests/regression/test_regression.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tests/regression/view_oauth.py` & `aleksis_core-3.1.2/aleksis/core/tests/regression/view_oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tests/templatetags/test_data_helpers.py` & `aleksis_core-3.1.2/aleksis/core/tests/templatetags/test_data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/tests/views/test_account.py` & `aleksis_core-3.1.2/aleksis/core/tests/views/test_account.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/urls.py` & `aleksis_core-3.1.2/aleksis/core/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/__pycache__/apps.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/util/__pycache__/apps.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,139 +1,144 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
-files sz: 10148
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
+files sz: 10969
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c026d035a036d045a046d
-      055a056d065a060100640064036c075a08640064046c096d0a5a0a6d0b5a
-      0b0100640064056c0c6d0d5a0d6d0e5a0e0100640064066c0f6d105a1001
-      00640064076c116d125a120100640064086c136d145a140100640064096c
-      156d165a170100640a640b6c186d195a190100640a640c6c1a6d1b5a1b01
-      00650372066400640d6c1c6d1d5a1d010002004700640e8400640f65086a
-      1e00000000000000006a1f0000000000000000a6030000ab030000000000
-      0000005a1f64035300
+      0x9700640064016c005a00640064026c016d025a020100640064036c036d
+      045a046d055a056d065a066d075a070100640064016c085a09640064046c
+      0a6d0b5a0b6d0c5a0c0100640064056c0d6d0e5a0e6d0f5a0f0100640064
+      066c106d115a110100640064076c126d135a130100640064086c146d155a
+      150100640064096c166d175a180100640a640b6c196d1a5a1a0100640a64
+      0c6c1b6d1c5a1c0100650472066400640d6c1d6d1e5a1e01000200470064
+      0e8400640f65096a1f00000000000000006a200000000000000000a60300
+      00ab0300000000000000005a2064015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('metadata',))
-                 6 IMPORT_NAME              0 (importlib)
-                 8 IMPORT_FROM              1 (metadata)
-                10 STORE_NAME               1 (metadata)
-                12 POP_TOP
+                 4 LOAD_CONST               1 (None)
+                 6 IMPORT_NAME              0 (logging)
+                 8 STORE_NAME               0 (logging)
    
-     2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('TYPE_CHECKING', 'Any', 'Optional', 'Sequence'))
-                18 IMPORT_NAME              2 (typing)
-                20 IMPORT_FROM              3 (TYPE_CHECKING)
-                22 STORE_NAME               3 (TYPE_CHECKING)
-                24 IMPORT_FROM              4 (Any)
-                26 STORE_NAME               4 (Any)
-                28 IMPORT_FROM              5 (Optional)
-                30 STORE_NAME               5 (Optional)
-                32 IMPORT_FROM              6 (Sequence)
-                34 STORE_NAME               6 (Sequence)
-                36 POP_TOP
+     2          10 LOAD_CONST               0 (0)
+                12 LOAD_CONST               2 (('metadata',))
+                14 IMPORT_NAME              1 (importlib)
+                16 IMPORT_FROM              2 (metadata)
+                18 STORE_NAME               2 (metadata)
+                20 POP_TOP
    
-     4          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               3 (None)
-                42 IMPORT_NAME              7 (django.apps)
-                44 STORE_NAME               8 (django)
+     3          22 LOAD_CONST               0 (0)
+                24 LOAD_CONST               3 (('TYPE_CHECKING', 'Any', 'Optional', 'Sequence'))
+                26 IMPORT_NAME              3 (typing)
+                28 IMPORT_FROM              4 (TYPE_CHECKING)
+                30 STORE_NAME               4 (TYPE_CHECKING)
+                32 IMPORT_FROM              5 (Any)
+                34 STORE_NAME               5 (Any)
+                36 IMPORT_FROM              6 (Optional)
+                38 STORE_NAME               6 (Optional)
+                40 IMPORT_FROM              7 (Sequence)
+                42 STORE_NAME               7 (Sequence)
+                44 POP_TOP
    
      5          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('user_logged_in', 'user_logged_out'))
-                50 IMPORT_NAME              9 (django.contrib.auth.signals)
-                52 IMPORT_FROM             10 (user_logged_in)
-                54 STORE_NAME              10 (user_logged_in)
-                56 IMPORT_FROM             11 (user_logged_out)
-                58 STORE_NAME              11 (user_logged_out)
-                60 POP_TOP
+                48 LOAD_CONST               1 (None)
+                50 IMPORT_NAME              8 (django.apps)
+                52 STORE_NAME               9 (django)
    
-     6          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('post_migrate', 'pre_migrate'))
-                66 IMPORT_NAME             12 (django.db.models.signals)
-                68 IMPORT_FROM             13 (post_migrate)
-                70 STORE_NAME              13 (post_migrate)
-                72 IMPORT_FROM             14 (pre_migrate)
-                74 STORE_NAME              14 (pre_migrate)
-                76 POP_TOP
+     6          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               4 (('user_logged_in', 'user_logged_out'))
+                58 IMPORT_NAME             10 (django.contrib.auth.signals)
+                60 IMPORT_FROM             11 (user_logged_in)
+                62 STORE_NAME              11 (user_logged_in)
+                64 IMPORT_FROM             12 (user_logged_out)
+                66 STORE_NAME              12 (user_logged_out)
+                68 POP_TOP
    
-     7          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               6 (('HttpRequest',))
-                82 IMPORT_NAME             15 (django.http)
-                84 IMPORT_FROM             16 (HttpRequest)
-                86 STORE_NAME              16 (HttpRequest)
-                88 POP_TOP
+     7          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               5 (('post_migrate', 'pre_migrate'))
+                74 IMPORT_NAME             13 (django.db.models.signals)
+                76 IMPORT_FROM             14 (post_migrate)
+                78 STORE_NAME              14 (post_migrate)
+                80 IMPORT_FROM             15 (pre_migrate)
+                82 STORE_NAME              15 (pre_migrate)
+                84 POP_TOP
    
-     9          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               7 (('preference_updated',))
-                94 IMPORT_NAME             17 (dynamic_preferences.signals)
-                96 IMPORT_FROM             18 (preference_updated)
-                98 STORE_NAME              18 (preference_updated)
-               100 POP_TOP
+     8          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               6 (('HttpRequest',))
+                90 IMPORT_NAME             16 (django.http)
+                92 IMPORT_FROM             17 (HttpRequest)
+                94 STORE_NAME              17 (HttpRequest)
+                96 POP_TOP
    
-    10         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               8 (('Licensing',))
-               106 IMPORT_NAME             19 (license_expression)
-               108 IMPORT_FROM             20 (Licensing)
-               110 STORE_NAME              20 (Licensing)
-               112 POP_TOP
+    10          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               7 (('preference_updated',))
+               102 IMPORT_NAME             18 (dynamic_preferences.signals)
+               104 IMPORT_FROM             19 (preference_updated)
+               106 STORE_NAME              19 (preference_updated)
+               108 POP_TOP
    
-    11         114 LOAD_CONST               0 (0)
-               116 LOAD_CONST               9 (('Request',))
-               118 IMPORT_NAME             21 (oauthlib.common)
-               120 IMPORT_FROM             22 (Request)
-               122 STORE_NAME              23 (OauthlibRequest)
-               124 POP_TOP
+    11         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               8 (('Licensing',))
+               114 IMPORT_NAME             20 (license_expression)
+               116 IMPORT_FROM             21 (Licensing)
+               118 STORE_NAME              21 (Licensing)
+               120 POP_TOP
    
-    13         126 LOAD_CONST              10 (1)
-               128 LOAD_CONST              11 (('copyright_years',))
-               130 IMPORT_NAME             24 (core_helpers)
-               132 IMPORT_FROM             25 (copyright_years)
-               134 STORE_NAME              25 (copyright_years)
-               136 POP_TOP
+    12         122 LOAD_CONST               0 (0)
+               124 LOAD_CONST               9 (('Request',))
+               126 IMPORT_NAME             22 (oauthlib.common)
+               128 IMPORT_FROM             23 (Request)
+               130 STORE_NAME              24 (OauthlibRequest)
+               132 POP_TOP
    
-    14         138 LOAD_CONST              10 (1)
-               140 LOAD_CONST              12 (('LICENSES',))
-               142 IMPORT_NAME             26 (spdx)
-               144 IMPORT_FROM             27 (LICENSES)
-               146 STORE_NAME              27 (LICENSES)
-               148 POP_TOP
+    14         134 LOAD_CONST              10 (1)
+               136 LOAD_CONST              11 (('copyright_years',))
+               138 IMPORT_NAME             25 (core_helpers)
+               140 IMPORT_FROM             26 (copyright_years)
+               142 STORE_NAME              26 (copyright_years)
+               144 POP_TOP
    
-    16         150 LOAD_NAME                3 (TYPE_CHECKING)
-               152 POP_JUMP_FORWARD_IF_FALSE     6 (to 166)
+    15         146 LOAD_CONST              10 (1)
+               148 LOAD_CONST              12 (('LICENSES',))
+               150 IMPORT_NAME             27 (spdx)
+               152 IMPORT_FROM             28 (LICENSES)
+               154 STORE_NAME              28 (LICENSES)
+               156 POP_TOP
    
-    17         154 LOAD_CONST               0 (0)
-               156 LOAD_CONST              13 (('AbstractApplication',))
-               158 IMPORT_NAME             28 (oauth2_provider.models)
-               160 IMPORT_FROM             29 (AbstractApplication)
-               162 STORE_NAME              29 (AbstractApplication)
-               164 POP_TOP
+    17         158 LOAD_NAME                4 (TYPE_CHECKING)
+               160 POP_JUMP_FORWARD_IF_FALSE     6 (to 174)
    
-    20     >>  166 PUSH_NULL
-               168 LOAD_BUILD_CLASS
-               170 LOAD_CONST              14 (<code object AppConfig, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 20>)
-               172 MAKE_FUNCTION            0
-               174 LOAD_CONST              15 ('AppConfig')
-               176 LOAD_NAME                8 (django)
-               178 LOAD_ATTR               30 (apps)
-               188 LOAD_ATTR               31 (AppConfig)
-               198 PRECALL                  3
-               202 CALL                     3
-               212 STORE_NAME              31 (AppConfig)
-               214 LOAD_CONST               3 (None)
-               216 RETURN_VALUE
+    18         162 LOAD_CONST               0 (0)
+               164 LOAD_CONST              13 (('AbstractApplication',))
+               166 IMPORT_NAME             29 (oauth2_provider.models)
+               168 IMPORT_FROM             30 (AbstractApplication)
+               170 STORE_NAME              30 (AbstractApplication)
+               172 POP_TOP
+   
+    21     >>  174 PUSH_NULL
+               176 LOAD_BUILD_CLASS
+               178 LOAD_CONST              14 (<code object AppConfig, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 21>)
+               180 MAKE_FUNCTION            0
+               182 LOAD_CONST              15 ('AppConfig')
+               184 LOAD_NAME                9 (django)
+               186 LOAD_ATTR               31 (apps)
+               196 LOAD_ATTR               32 (AppConfig)
+               206 PRECALL                  3
+               210 CALL                     3
+               220 STORE_NAME              32 (AppConfig)
+               222 LOAD_CONST               1 (None)
+               224 RETURN_VALUE
    consts
       0
+      None
       ('metadata',)
       ('TYPE_CHECKING', 'Any', 'Optional', 'Sequence')
-      None
       ('user_logged_in', 'user_logged_out')
       ('post_migrate', 'pre_migrate')
       ('HttpRequest',)
       ('preference_updated',)
       ('Licensing',)
       ('Request',)
       1
@@ -172,772 +177,834 @@
             0000000000000064206517652419000000000000000000640a651e651319
             000000000000000000660664298405a6000000ab0000000000000000005a
             2a650c642a651e6513190000000000000000006420652b640a6527651365
             166602190000000000000000006606642b8404a6000000ab000000000000
             0000005a2c642c84005a2d880078015a2e5300
                        0 MAKE_CELL                0 (__class__)
          
-          20           2 RESUME                   0
+          21           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AppConfig')
                       10 STORE_NAME               2 (__qualname__)
          
-          21          12 LOAD_CONST               1 ("An extended version of DJango's AppConfig container.")
+          22          12 LOAD_CONST               1 ("An extended version of DJango's AppConfig container.")
                       14 STORE_NAME               3 (__doc__)
          
-          23          16 LOAD_CONST               2 (False)
+          24          16 LOAD_CONST               2 (False)
                       18 STORE_NAME               4 (default)
          
-          24          20 LOAD_CONST               3 ('django.db.models.BigAutoField')
+          25          20 LOAD_CONST               3 ('django.db.models.BigAutoField')
                       22 STORE_NAME               5 (default_auto_field)
          
-          26          24 LOAD_CLOSURE             0 (__class__)
+          27          24 LOAD_CLOSURE             0 (__class__)
                       26 BUILD_TUPLE              1
-                      28 LOAD_CONST               4 (<code object __init_subclass__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 26>)
+                      28 LOAD_CONST               4 (<code object __init_subclass__, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 27>)
                       30 MAKE_FUNCTION            8 (closure)
                       32 STORE_NAME               6 (__init_subclass__)
          
-          30          34 LOAD_CLOSURE             0 (__class__)
+          32          34 LOAD_CLOSURE             0 (__class__)
                       36 BUILD_TUPLE              1
-                      38 LOAD_CONST               5 (<code object ready, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 30>)
+                      38 LOAD_CONST               5 (<code object ready, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 32>)
                       40 MAKE_FUNCTION            8 (closure)
                       42 STORE_NAME               7 (ready)
          
-          43          44 LOAD_CONST               6 (<code object get_distribution_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 43>)
+          50          44 LOAD_CONST               6 (<code object get_distribution_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 50>)
                       46 MAKE_FUNCTION            0
                       48 STORE_NAME               8 (get_distribution_name)
          
-          52          50 LOAD_CONST               7 (<code object get_distribution, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 52>)
+          59          50 LOAD_CONST               7 (<code object get_distribution, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 59>)
                       52 MAKE_FUNCTION            0
                       54 STORE_NAME               9 (get_distribution)
          
-          63          56 LOAD_CONST               8 (<code object get_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 63>)
+          70          56 LOAD_CONST               8 (<code object get_name, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 70>)
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME              10 (get_name)
          
-          73          62 LOAD_CONST               9 (<code object get_version, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 73>)
+          80          62 LOAD_CONST               9 (<code object get_version, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 80>)
                       64 MAKE_FUNCTION            0
                       66 STORE_NAME              11 (get_version)
          
-          84          68 LOAD_NAME               12 (classmethod)
+          91          68 LOAD_NAME               12 (classmethod)
          
-          85          70 LOAD_CONST              10 ('return')
+          92          70 LOAD_CONST              10 ('return')
                       72 LOAD_NAME               13 (tuple)
                       74 BUILD_TUPLE              2
-                      76 LOAD_CONST              11 (<code object get_licence, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 84>)
+                      76 LOAD_CONST              11 (<code object get_licence, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 91>)
                       78 MAKE_FUNCTION            4 (annotations)
          
-          84          80 PRECALL                  0
+          91          80 PRECALL                  0
                       84 CALL                     0
          
-          85          94 STORE_NAME              14 (get_licence)
+          92          94 STORE_NAME              14 (get_licence)
          
-         140          96 LOAD_NAME               12 (classmethod)
+         147          96 LOAD_NAME               12 (classmethod)
          
-         141          98 LOAD_CONST              12 (<code object get_licence_dict, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 140>)
+         148          98 LOAD_CONST              12 (<code object get_licence_dict, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 147>)
                      100 MAKE_FUNCTION            0
          
-         140         102 PRECALL                  0
+         147         102 PRECALL                  0
                      106 CALL                     0
          
-         141         116 STORE_NAME              15 (get_licence_dict)
+         148         116 STORE_NAME              15 (get_licence_dict)
          
-         150         118 LOAD_NAME               12 (classmethod)
+         157         118 LOAD_NAME               12 (classmethod)
          
-         151         120 LOAD_CONST              13 (<code object get_urls, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 150>)
+         158         120 LOAD_CONST              13 (<code object get_urls, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 157>)
                      122 MAKE_FUNCTION            0
          
-         150         124 PRECALL                  0
+         157         124 PRECALL                  0
                      128 CALL                     0
          
-         151         138 STORE_NAME              16 (get_urls)
+         158         138 STORE_NAME              16 (get_urls)
          
-         156         140 LOAD_NAME               12 (classmethod)
+         163         140 LOAD_NAME               12 (classmethod)
          
-         157         142 LOAD_CONST              14 (<code object get_urls_dict, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 156>)
+         164         142 LOAD_CONST              14 (<code object get_urls_dict, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 163>)
                      144 MAKE_FUNCTION            0
          
-         156         146 PRECALL                  0
+         163         146 PRECALL                  0
                      150 CALL                     0
          
-         157         160 STORE_NAME              17 (get_urls_dict)
+         164         160 STORE_NAME              17 (get_urls_dict)
          
-         162         162 LOAD_NAME               12 (classmethod)
+         169         162 LOAD_NAME               12 (classmethod)
          
-         163         164 LOAD_CONST              10 ('return')
+         170         164 LOAD_CONST              10 ('return')
                      166 LOAD_NAME               18 (Sequence)
                      168 LOAD_NAME               13 (tuple)
                      170 LOAD_NAME               19 (str)
                      172 LOAD_NAME               19 (str)
                      174 LOAD_NAME               19 (str)
                      176 BUILD_TUPLE              3
                      178 BINARY_SUBSCR
                      188 BINARY_SUBSCR
                      198 BUILD_TUPLE              2
-                     200 LOAD_CONST              15 (<code object get_copyright, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 162>)
+                     200 LOAD_CONST              15 (<code object get_copyright, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 169>)
                      202 MAKE_FUNCTION            4 (annotations)
          
-         162         204 PRECALL                  0
+         169         204 PRECALL                  0
                      208 CALL                     0
          
-         163         218 STORE_NAME              20 (get_copyright)
+         170         218 STORE_NAME              20 (get_copyright)
          
-         183         220 LOAD_NAME               12 (classmethod)
+         190         220 LOAD_NAME               12 (classmethod)
          
-         184         222 LOAD_CONST              16 (<code object get_copyright_dicts, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 183>)
+         191         222 LOAD_CONST              16 (<code object get_copyright_dicts, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 190>)
                      224 MAKE_FUNCTION            0
          
-         183         226 PRECALL                  0
+         190         226 PRECALL                  0
                      230 CALL                     0
          
-         184         240 STORE_NAME              21 (get_copyright_dicts)
+         191         240 STORE_NAME              21 (get_copyright_dicts)
          
-         192         242 NOP
+         199         242 NOP
          
-         193         244 NOP
+         200         244 NOP
          
-         194         246 NOP
+         201         246 NOP
          
-         195         248 NOP
+         202         248 NOP
          
-         189         250 LOAD_CONST              45 ((None, None, None, None))
+         196         250 LOAD_CONST              45 ((None, None, None, None))
                      252 LOAD_CONST              18 ('sender')
          
-         191         254 LOAD_NAME               22 (Any)
+         198         254 LOAD_NAME               22 (Any)
          
-         189         256 LOAD_CONST              19 ('section')
+         196         256 LOAD_CONST              19 ('section')
          
-         192         258 LOAD_NAME               23 (Optional)
+         199         258 LOAD_NAME               23 (Optional)
                      260 LOAD_NAME               19 (str)
                      262 BINARY_SUBSCR
          
-         189         272 LOAD_CONST              20 ('name')
+         196         272 LOAD_CONST              20 ('name')
          
-         193         274 LOAD_NAME               23 (Optional)
+         200         274 LOAD_NAME               23 (Optional)
                      276 LOAD_NAME               19 (str)
                      278 BINARY_SUBSCR
          
-         189         288 LOAD_CONST              21 ('old_value')
+         196         288 LOAD_CONST              21 ('old_value')
          
-         194         290 LOAD_NAME               23 (Optional)
+         201         290 LOAD_NAME               23 (Optional)
                      292 LOAD_NAME               22 (Any)
                      294 BINARY_SUBSCR
          
-         189         304 LOAD_CONST              22 ('new_value')
+         196         304 LOAD_CONST              22 ('new_value')
          
-         195         306 LOAD_NAME               23 (Optional)
+         202         306 LOAD_NAME               23 (Optional)
                      308 LOAD_NAME               22 (Any)
                      310 BINARY_SUBSCR
          
-         189         320 LOAD_CONST              10 ('return')
+         196         320 LOAD_CONST              10 ('return')
          
-         197         322 LOAD_CONST              17 (None)
+         204         322 LOAD_CONST              17 (None)
          
-         189         324 BUILD_TUPLE             12
-                     326 LOAD_CONST              23 (<code object preference_updated, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 189>)
+         196         324 BUILD_TUPLE             12
+                     326 LOAD_CONST              23 (<code object preference_updated, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 196>)
                      328 MAKE_FUNCTION            5 (defaults, annotations)
                      330 STORE_NAME              24 (preference_updated)
          
-         204         332 LOAD_CONST              24 ('app_config')
+         211         332 LOAD_CONST              24 ('app_config')
          
-         206         334 LOAD_NAME               25 (django)
+         213         334 LOAD_NAME               25 (django)
                      336 LOAD_ATTR               26 (apps)
                      346 LOAD_ATTR               27 (AppConfig)
          
-         204         356 LOAD_CONST              25 ('verbosity')
+         211         356 LOAD_CONST              25 ('verbosity')
          
-         207         358 LOAD_NAME               28 (int)
+         214         358 LOAD_NAME               28 (int)
          
-         204         360 LOAD_CONST              26 ('interactive')
+         211         360 LOAD_CONST              26 ('interactive')
          
-         208         362 LOAD_NAME               29 (bool)
+         215         362 LOAD_NAME               29 (bool)
          
-         204         364 LOAD_CONST              27 ('using')
+         211         364 LOAD_CONST              27 ('using')
          
-         209         366 LOAD_NAME               19 (str)
+         216         366 LOAD_NAME               19 (str)
          
-         204         368 LOAD_CONST              28 ('plan')
+         211         368 LOAD_CONST              28 ('plan')
          
-         210         370 LOAD_NAME               30 (list)
+         217         370 LOAD_NAME               30 (list)
                      372 LOAD_NAME               13 (tuple)
                      374 BINARY_SUBSCR
          
-         204         384 LOAD_CONST              29 ('apps')
+         211         384 LOAD_CONST              29 ('apps')
          
-         211         386 LOAD_NAME               25 (django)
+         218         386 LOAD_NAME               25 (django)
                      388 LOAD_ATTR               26 (apps)
                      398 LOAD_ATTR               31 (registry)
                      408 LOAD_ATTR               32 (Apps)
          
-         204         418 LOAD_CONST              10 ('return')
+         211         418 LOAD_CONST              10 ('return')
          
-         213         420 LOAD_CONST              17 (None)
+         220         420 LOAD_CONST              17 (None)
          
-         204         422 BUILD_TUPLE             14
-                     424 LOAD_CONST              30 (<code object pre_migrate, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 204>)
+         211         422 BUILD_TUPLE             14
+                     424 LOAD_CONST              30 (<code object pre_migrate, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 211>)
                      426 MAKE_FUNCTION            4 (annotations)
                      428 STORE_NAME              33 (pre_migrate)
          
-         220         430 LOAD_CONST              24 ('app_config')
+         227         430 LOAD_CONST              24 ('app_config')
          
-         222         432 LOAD_NAME               25 (django)
+         229         432 LOAD_NAME               25 (django)
                      434 LOAD_ATTR               26 (apps)
                      444 LOAD_ATTR               27 (AppConfig)
          
-         220         454 LOAD_CONST              25 ('verbosity')
+         227         454 LOAD_CONST              25 ('verbosity')
          
-         223         456 LOAD_NAME               28 (int)
+         230         456 LOAD_NAME               28 (int)
          
-         220         458 LOAD_CONST              26 ('interactive')
+         227         458 LOAD_CONST              26 ('interactive')
          
-         224         460 LOAD_NAME               29 (bool)
+         231         460 LOAD_NAME               29 (bool)
          
-         220         462 LOAD_CONST              27 ('using')
+         227         462 LOAD_CONST              27 ('using')
          
-         225         464 LOAD_NAME               19 (str)
+         232         464 LOAD_NAME               19 (str)
          
-         220         466 LOAD_CONST              10 ('return')
+         227         466 LOAD_CONST              10 ('return')
          
-         227         468 LOAD_CONST              17 (None)
+         234         468 LOAD_CONST              17 (None)
          
-         220         470 BUILD_TUPLE             10
-                     472 LOAD_CONST              31 (<code object post_migrate, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 220>)
+         227         470 BUILD_TUPLE             10
+                     472 LOAD_CONST              31 (<code object post_migrate, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 227>)
                      474 MAKE_FUNCTION            4 (annotations)
                      476 STORE_NAME              34 (post_migrate)
          
-         234         478 LOAD_CONST              18 ('sender')
+         241         478 LOAD_CONST              18 ('sender')
          
-         235         480 LOAD_NAME               35 (type)
+         242         480 LOAD_NAME               35 (type)
          
-         234         482 LOAD_CONST              32 ('request')
+         241         482 LOAD_CONST              32 ('request')
          
-         235         484 LOAD_NAME               23 (Optional)
+         242         484 LOAD_NAME               23 (Optional)
                      486 LOAD_NAME               36 (HttpRequest)
                      488 BINARY_SUBSCR
          
-         234         498 LOAD_CONST              33 ('user')
+         241         498 LOAD_CONST              33 ('user')
          
-         235         500 LOAD_CONST              34 ('User')
+         242         500 LOAD_CONST              34 ('User')
          
-         234         502 LOAD_CONST              10 ('return')
+         241         502 LOAD_CONST              10 ('return')
          
-         236         504 LOAD_CONST              17 (None)
+         243         504 LOAD_CONST              17 (None)
          
-         234         506 BUILD_TUPLE              8
-                     508 LOAD_CONST              35 (<code object user_logged_in, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 234>)
+         241         506 BUILD_TUPLE              8
+                     508 LOAD_CONST              35 (<code object user_logged_in, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 241>)
                      510 MAKE_FUNCTION            4 (annotations)
                      512 STORE_NAME              37 (user_logged_in)
          
-         243         514 LOAD_CONST              18 ('sender')
+         250         514 LOAD_CONST              18 ('sender')
          
-         244         516 LOAD_NAME               35 (type)
+         251         516 LOAD_NAME               35 (type)
          
-         243         518 LOAD_CONST              32 ('request')
+         250         518 LOAD_CONST              32 ('request')
          
-         244         520 LOAD_NAME               23 (Optional)
+         251         520 LOAD_NAME               23 (Optional)
                      522 LOAD_NAME               36 (HttpRequest)
                      524 BINARY_SUBSCR
          
-         243         534 LOAD_CONST              33 ('user')
+         250         534 LOAD_CONST              33 ('user')
          
-         244         536 LOAD_CONST              34 ('User')
+         251         536 LOAD_CONST              34 ('User')
          
-         243         538 LOAD_CONST              10 ('return')
+         250         538 LOAD_CONST              10 ('return')
          
-         245         540 LOAD_CONST              17 (None)
+         252         540 LOAD_CONST              17 (None)
          
-         243         542 BUILD_TUPLE              8
-                     544 LOAD_CONST              36 (<code object user_logged_out, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 243>)
+         250         542 BUILD_TUPLE              8
+                     544 LOAD_CONST              36 (<code object user_logged_out, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 250>)
                      546 MAKE_FUNCTION            4 (annotations)
                      548 STORE_NAME              38 (user_logged_out)
          
-         252         550 LOAD_NAME               12 (classmethod)
+         259         550 LOAD_NAME               12 (classmethod)
          
-         253         552 LOAD_CONST              10 ('return')
+         260         552 LOAD_CONST              10 ('return')
                      554 LOAD_NAME               39 (dict)
                      556 LOAD_NAME               19 (str)
                      558 LOAD_NAME               19 (str)
                      560 BUILD_TUPLE              2
                      562 BINARY_SUBSCR
                      572 BUILD_TUPLE              2
-                     574 LOAD_CONST              37 (<code object get_all_scopes, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 252>)
+                     574 LOAD_CONST              37 (<code object get_all_scopes, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 259>)
                      576 MAKE_FUNCTION            4 (annotations)
          
-         252         578 PRECALL                  0
+         259         578 PRECALL                  0
                      582 CALL                     0
          
-         253         592 STORE_NAME              40 (get_all_scopes)
+         260         592 STORE_NAME              40 (get_all_scopes)
          
-         257         594 LOAD_NAME               12 (classmethod)
+         264         594 LOAD_NAME               12 (classmethod)
          
-         260         596 NOP
+         267         596 NOP
          
-         261         598 NOP
+         268         598 NOP
          
-         258         600 LOAD_CONST              46 ((None, None))
+         265         600 LOAD_CONST              46 ((None, None))
                      602 LOAD_CONST              38 ('application')
          
-         260         604 LOAD_NAME               23 (Optional)
+         267         604 LOAD_NAME               23 (Optional)
                      606 LOAD_CONST              39 ('AbstractApplication')
                      608 BINARY_SUBSCR
          
-         258         618 LOAD_CONST              32 ('request')
+         265         618 LOAD_CONST              32 ('request')
          
-         261         620 LOAD_NAME               23 (Optional)
+         268         620 LOAD_NAME               23 (Optional)
                      622 LOAD_NAME               36 (HttpRequest)
                      624 BINARY_SUBSCR
          
-         258         634 LOAD_CONST              10 ('return')
+         265         634 LOAD_CONST              10 ('return')
          
-         264         636 LOAD_NAME               30 (list)
+         271         636 LOAD_NAME               30 (list)
                      638 LOAD_NAME               19 (str)
                      640 BINARY_SUBSCR
          
-         258         650 BUILD_TUPLE              6
-                     652 LOAD_CONST              40 (<code object get_available_scopes, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 257>)
+         265         650 BUILD_TUPLE              6
+                     652 LOAD_CONST              40 (<code object get_available_scopes, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 264>)
                      654 MAKE_FUNCTION            5 (defaults, annotations)
          
-         257         656 PRECALL                  0
+         264         656 PRECALL                  0
                      660 CALL                     0
          
-         258         670 STORE_NAME              41 (get_available_scopes)
+         265         670 STORE_NAME              41 (get_available_scopes)
          
-         268         672 LOAD_NAME               12 (classmethod)
+         275         672 LOAD_NAME               12 (classmethod)
          
-         271         674 NOP
+         278         674 NOP
          
-         272         676 NOP
+         279         676 NOP
          
-         269         678 LOAD_CONST              46 ((None, None))
+         276         678 LOAD_CONST              46 ((None, None))
                      680 LOAD_CONST              38 ('application')
          
-         271         682 LOAD_NAME               23 (Optional)
+         278         682 LOAD_NAME               23 (Optional)
                      684 LOAD_CONST              39 ('AbstractApplication')
                      686 BINARY_SUBSCR
          
-         269         696 LOAD_CONST              32 ('request')
+         276         696 LOAD_CONST              32 ('request')
          
-         272         698 LOAD_NAME               23 (Optional)
+         279         698 LOAD_NAME               23 (Optional)
                      700 LOAD_NAME               36 (HttpRequest)
                      702 BINARY_SUBSCR
          
-         269         712 LOAD_CONST              10 ('return')
+         276         712 LOAD_CONST              10 ('return')
          
-         275         714 LOAD_NAME               30 (list)
+         282         714 LOAD_NAME               30 (list)
                      716 LOAD_NAME               19 (str)
                      718 BINARY_SUBSCR
          
-         269         728 BUILD_TUPLE              6
-                     730 LOAD_CONST              41 (<code object get_default_scopes, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 268>)
+         276         728 BUILD_TUPLE              6
+                     730 LOAD_CONST              41 (<code object get_default_scopes, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 275>)
                      732 MAKE_FUNCTION            5 (defaults, annotations)
          
-         268         734 PRECALL                  0
+         275         734 PRECALL                  0
                      738 CALL                     0
          
-         269         748 STORE_NAME              42 (get_default_scopes)
+         276         748 STORE_NAME              42 (get_default_scopes)
          
-         279         750 LOAD_NAME               12 (classmethod)
+         286         750 LOAD_NAME               12 (classmethod)
          
-         280         752 LOAD_CONST              42 ('scopes')
+         287         752 LOAD_CONST              42 ('scopes')
                      754 LOAD_NAME               30 (list)
                      756 LOAD_NAME               19 (str)
                      758 BINARY_SUBSCR
                      768 LOAD_CONST              32 ('request')
                      770 LOAD_NAME               43 (OauthlibRequest)
                      772 LOAD_CONST              10 ('return')
                      774 LOAD_NAME               39 (dict)
                      776 LOAD_NAME               19 (str)
                      778 LOAD_NAME               22 (Any)
                      780 BUILD_TUPLE              2
                      782 BINARY_SUBSCR
                      792 BUILD_TUPLE              6
-                     794 LOAD_CONST              43 (<code object get_additional_claims, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 279>)
+                     794 LOAD_CONST              43 (<code object get_additional_claims, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 286>)
                      796 MAKE_FUNCTION            4 (annotations)
          
-         279         798 PRECALL                  0
+         286         798 PRECALL                  0
                      802 CALL                     0
          
-         280         812 STORE_NAME              44 (get_additional_claims)
+         287         812 STORE_NAME              44 (get_additional_claims)
          
-         284         814 LOAD_CONST              44 (<code object _maintain_default_data, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 284>)
+         291         814 LOAD_CONST              44 (<code object _maintain_default_data, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 291>)
                      816 MAKE_FUNCTION            0
                      818 STORE_NAME              45 (_maintain_default_data)
                      820 LOAD_CLOSURE             0 (__class__)
                      822 COPY                     1
                      824 STORE_NAME              46 (__classcell__)
                      826 RETURN_VALUE
          consts
             'AppConfig'
             "An extended version of DJango's AppConfig container."
             False
             'django.db.models.BigAutoField'
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 2
+               stacksize : 5
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a0010000000000000000000000000000000000000000a6000000ab0000
-                  00000000000000010064017c005f02000000000000000064005300
+                  00000000000000010064017c005f02000000000000000074070000000000
+                  00000000006a0400000000000000007c006a0500000000000000009b0064
+                  027c006a0600000000000000009b009d03a6010000ab0100000000000000
+                  007c005f07000000000000000064005300
                              0 COPY_FREE_VARS           1
                
-                26           2 RESUME                   0
+                27           2 RESUME                   0
                
-                27           4 LOAD_GLOBAL              1 (NULL + super)
+                28           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__init_subclass__)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 POP_TOP
                
-                28          68 LOAD_CONST               1 (True)
+                29          68 LOAD_CONST               1 (True)
                             70 LOAD_FAST                0 (cls)
                             72 STORE_ATTR               2 (default)
-                            82 LOAD_CONST               0 (None)
-                            84 RETURN_VALUE
+               
+                30          82 LOAD_GLOBAL              7 (NULL + logging)
+                            94 LOAD_ATTR                4 (getLogger)
+                           104 LOAD_FAST                0 (cls)
+                           106 LOAD_ATTR                5 (__module__)
+                           116 FORMAT_VALUE             0
+                           118 LOAD_CONST               2 ('.')
+                           120 LOAD_FAST                0 (cls)
+                           122 LOAD_ATTR                6 (__name__)
+                           132 FORMAT_VALUE             0
+                           134 BUILD_STRING             3
+                           136 PRECALL                  1
+                           140 CALL                     1
+                           150 LOAD_FAST                0 (cls)
+                           152 STORE_ATTR               7 (_logger)
+                           162 LOAD_CONST               0 (None)
+                           164 RETURN_VALUE
                consts
                   None
                   True
-               names      ('super', '__init_subclass__', 'default')
+                  '.'
+               names      ('super', '__init_subclass__', 'default', 'logging', 'getLogger', '__module__', '__name__', '_logger')
                varnames   ('cls',)
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       '__init_subclass__'
-               firstlineno 26
-               lnotab 0x04014001
+               firstlineno 27
+               lnotab 0x040140010e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
-                  0x95019700740100000000000000000000a6000000ab0000000000000000
-                  00a0010000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000001007405000000000000000000006a0300000000000000
-                  007c006a0200000000000000007c00ac01a6020000ab0200000000000000
-                  0001007409000000000000000000006a0300000000000000007c006a0400
-                  000000000000007c00ac01a6020000ab0200000000000000000100740b00
-                  0000000000000000006a0300000000000000007c006a0500000000000000
-                  00a6010000ab0100000000000000000100740d000000000000000000006a
-                  0300000000000000007c006a060000000000000000a6010000ab01000000
-                  00000000000100740f000000000000000000006a0300000000000000007c
-                  006a070000000000000000a6010000ab01000000000000000001007c00a0
-                  0500000000000000000000000000000000000000007c00a6010000ab0100
-                  00000000000000010064005300
+                  0x950197007c006a000000000000000000a0010000000000000000000000
+                  0000000000000000006401a6010000ab0100000000000000000100740500
+                  000000000000000000a6000000ab000000000000000000a0030000000000
+                  000000000000000000000000000000a6000000ab00000000000000000001
+                  007409000000000000000000006a0500000000000000007c006a04000000
+                  00000000007c00ac02a6020000ab0200000000000000000100740d000000
+                  000000000000006a0500000000000000007c006a0600000000000000007c
+                  00ac02a6020000ab0200000000000000000100740f000000000000000000
+                  006a0500000000000000007c006a070000000000000000a6010000ab0100
+                  0000000000000001007411000000000000000000006a0500000000000000
+                  007c006a080000000000000000a6010000ab010000000000000000010074
+                  13000000000000000000006a0500000000000000007c006a090000000000
+                  000000a6010000ab01000000000000000001007c006a0000000000000000
+                  00a00100000000000000000000000000000000000000006403a6010000ab
+                  01000000000000000001007c006a000000000000000000a0010000000000
+                  0000000000000000000000000000006404a6010000ab0100000000000000
+                  0001007c00a00700000000000000000000000000000000000000007c00a6
+                  010000ab01000000000000000001007c006a000000000000000000a00100
+                  000000000000000000000000000000000000006405a6010000ab01000000
+                  0000000000010064005300
                              0 COPY_FREE_VARS           1
                
-                30           2 RESUME                   0
+                32           2 RESUME                   0
                
-                31           4 LOAD_GLOBAL              1 (NULL + super)
-                            16 PRECALL                  0
-                            20 CALL                     0
-                            30 LOAD_METHOD              1 (ready)
-                            52 PRECALL                  0
-                            56 CALL                     0
-                            66 POP_TOP
+                33           4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (_logger)
+                            16 LOAD_METHOD              1 (debug)
+                            38 LOAD_CONST               1 ('Running app.ready')
+                            40 PRECALL                  1
+                            44 CALL                     1
+                            54 POP_TOP
                
-                34          68 LOAD_GLOBAL              5 (NULL + pre_migrate)
-                            80 LOAD_ATTR                3 (connect)
-                            90 LOAD_FAST                0 (self)
-                            92 LOAD_ATTR                2 (pre_migrate)
-                           102 LOAD_FAST                0 (self)
-                           104 KW_NAMES                 1
-                           106 PRECALL                  2
-                           110 CALL                     2
-                           120 POP_TOP
-               
-                35         122 LOAD_GLOBAL              9 (NULL + post_migrate)
-                           134 LOAD_ATTR                3 (connect)
-                           144 LOAD_FAST                0 (self)
-                           146 LOAD_ATTR                4 (post_migrate)
-                           156 LOAD_FAST                0 (self)
-                           158 KW_NAMES                 1
-                           160 PRECALL                  2
-                           164 CALL                     2
-                           174 POP_TOP
-               
-                36         176 LOAD_GLOBAL             11 (NULL + preference_updated)
-                           188 LOAD_ATTR                3 (connect)
-                           198 LOAD_FAST                0 (self)
-                           200 LOAD_ATTR                5 (preference_updated)
-                           210 PRECALL                  1
-                           214 CALL                     1
-                           224 POP_TOP
-               
-                37         226 LOAD_GLOBAL             13 (NULL + user_logged_in)
-                           238 LOAD_ATTR                3 (connect)
-                           248 LOAD_FAST                0 (self)
-                           250 LOAD_ATTR                6 (user_logged_in)
-                           260 PRECALL                  1
-                           264 CALL                     1
-                           274 POP_TOP
-               
-                38         276 LOAD_GLOBAL             15 (NULL + user_logged_out)
-                           288 LOAD_ATTR                3 (connect)
-                           298 LOAD_FAST                0 (self)
-                           300 LOAD_ATTR                7 (user_logged_out)
-                           310 PRECALL                  1
-                           314 CALL                     1
-                           324 POP_TOP
+                35          56 LOAD_GLOBAL              5 (NULL + super)
+                            68 PRECALL                  0
+                            72 CALL                     0
+                            82 LOAD_METHOD              3 (ready)
+                           104 PRECALL                  0
+                           108 CALL                     0
+                           118 POP_TOP
                
-                41         326 LOAD_FAST                0 (self)
-                           328 LOAD_METHOD              5 (preference_updated)
+                38         120 LOAD_GLOBAL              9 (NULL + pre_migrate)
+                           132 LOAD_ATTR                5 (connect)
+                           142 LOAD_FAST                0 (self)
+                           144 LOAD_ATTR                4 (pre_migrate)
+                           154 LOAD_FAST                0 (self)
+                           156 KW_NAMES                 2
+                           158 PRECALL                  2
+                           162 CALL                     2
+                           172 POP_TOP
+               
+                39         174 LOAD_GLOBAL             13 (NULL + post_migrate)
+                           186 LOAD_ATTR                5 (connect)
+                           196 LOAD_FAST                0 (self)
+                           198 LOAD_ATTR                6 (post_migrate)
+                           208 LOAD_FAST                0 (self)
+                           210 KW_NAMES                 2
+                           212 PRECALL                  2
+                           216 CALL                     2
+                           226 POP_TOP
+               
+                40         228 LOAD_GLOBAL             15 (NULL + preference_updated)
+                           240 LOAD_ATTR                5 (connect)
+                           250 LOAD_FAST                0 (self)
+                           252 LOAD_ATTR                7 (preference_updated)
+                           262 PRECALL                  1
+                           266 CALL                     1
+                           276 POP_TOP
+               
+                41         278 LOAD_GLOBAL             17 (NULL + user_logged_in)
+                           290 LOAD_ATTR                5 (connect)
+                           300 LOAD_FAST                0 (self)
+                           302 LOAD_ATTR                8 (user_logged_in)
+                           312 PRECALL                  1
+                           316 CALL                     1
+                           326 POP_TOP
+               
+                42         328 LOAD_GLOBAL             19 (NULL + user_logged_out)
+                           340 LOAD_ATTR                5 (connect)
                            350 LOAD_FAST                0 (self)
-                           352 PRECALL                  1
-                           356 CALL                     1
-                           366 POP_TOP
-                           368 LOAD_CONST               0 (None)
-                           370 RETURN_VALUE
+                           352 LOAD_ATTR                9 (user_logged_out)
+                           362 PRECALL                  1
+                           366 CALL                     1
+                           376 POP_TOP
+               
+                43         378 LOAD_FAST                0 (self)
+                           380 LOAD_ATTR                0 (_logger)
+                           390 LOAD_METHOD              1 (debug)
+                           412 LOAD_CONST               3 ('Default signal handlers connected')
+                           414 PRECALL                  1
+                           418 CALL                     1
+                           428 POP_TOP
+               
+                46         430 LOAD_FAST                0 (self)
+                           432 LOAD_ATTR                0 (_logger)
+                           442 LOAD_METHOD              1 (debug)
+                           464 LOAD_CONST               4 ('Force-loading preferences')
+                           466 PRECALL                  1
+                           470 CALL                     1
+                           480 POP_TOP
+               
+                47         482 LOAD_FAST                0 (self)
+                           484 LOAD_METHOD              7 (preference_updated)
+                           506 LOAD_FAST                0 (self)
+                           508 PRECALL                  1
+                           512 CALL                     1
+                           522 POP_TOP
+               
+                48         524 LOAD_FAST                0 (self)
+                           526 LOAD_ATTR                0 (_logger)
+                           536 LOAD_METHOD              1 (debug)
+                           558 LOAD_CONST               5 ('Preferences loaded')
+                           560 PRECALL                  1
+                           564 CALL                     1
+                           574 POP_TOP
+                           576 LOAD_CONST               0 (None)
+                           578 RETURN_VALUE
                consts
                   None
+                  'Running app.ready'
                   ('sender',)
-               names      ('super', 'ready', 'pre_migrate', 'connect', 'post_migrate', 'preference_updated', 'user_logged_in', 'user_logged_out')
+                  'Default signal handlers connected'
+                  'Force-loading preferences'
+                  'Preferences loaded'
+               names      ('_logger', 'debug', 'super', 'ready', 'pre_migrate', 'connect', 'post_migrate', 'preference_updated', 'user_logged_in', 'user_logged_out')
                varnames   ('self',)
                freevars   ('__class__',)
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'ready'
-               firstlineno 30
-               lnotab 0x0401400336013601320132013203
+               firstlineno 32
+               lnotab 0x04013402400336013601320132013201340334012a01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006401a6020000ab020000000000
                   00000072077c006a01000000000000000053007c006a0200000000000000
                   00a0030000000000000000000000000000000000000000a6000000ab0000
                   00000000000000a004000000000000000000000000000000000000000064
                   02a6010000ab010000000000000000722d7c006a020000000000000000a0
                   030000000000000000000000000000000000000000a6000000ab00000000
                   0000000000a0050000000000000000000000000000000000000000640264
                   03a6020000ab020000000000000000530064045300
-                43           0 RESUME                   0
+                50           0 RESUME                   0
                
-                45           2 LOAD_GLOBAL              1 (NULL + hasattr)
+                52           2 LOAD_GLOBAL              1 (NULL + hasattr)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_CONST               1 ('dist_name')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_JUMP_FORWARD_IF_FALSE     7 (to 48)
                
-                46          34 LOAD_FAST                0 (self)
+                53          34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                1 (dist_name)
                             46 RETURN_VALUE
                
-                47     >>   48 LOAD_FAST                0 (self)
+                54     >>   48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                2 (name)
                             60 LOAD_METHOD              3 (lower)
                             82 PRECALL                  0
                             86 CALL                     0
                             96 LOAD_METHOD              4 (startswith)
                            118 LOAD_CONST               2 ('aleksis.apps.')
                            120 PRECALL                  1
                            124 CALL                     1
                            134 POP_JUMP_FORWARD_IF_FALSE    45 (to 226)
                
-                48         136 LOAD_FAST                0 (self)
+                55         136 LOAD_FAST                0 (self)
                            138 LOAD_ATTR                2 (name)
                            148 LOAD_METHOD              3 (lower)
                            170 PRECALL                  0
                            174 CALL                     0
                            184 LOAD_METHOD              5 (replace)
                            206 LOAD_CONST               2 ('aleksis.apps.')
                            208 LOAD_CONST               3 ('AlekSIS-App-')
                            210 PRECALL                  2
                            214 CALL                     2
                            224 RETURN_VALUE
                
-                50     >>  226 LOAD_CONST               4 (None)
+                57     >>  226 LOAD_CONST               4 (None)
                            228 RETURN_VALUE
                consts
                   'Get distribution name of application package.'
                   'dist_name'
                   'aleksis.apps.'
                   'AlekSIS-App-'
                   None
                names      ('hasattr', 'dist_name', 'name', 'lower', 'startswith', 'replace')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_distribution_name'
-               firstlineno 43
+               firstlineno 50
                lnotab 0x020220010e0158015a02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d017c01722e09007403000000000000000000
                   006a0200000000000000007c01a6010000ab0100000000000000007d026e
                   1623007402000000000000000000006a0300000000000000002400720401
                   0059006401530077007803590077017c02530064015300
-                52           0 RESUME                   0
+                59           0 RESUME                   0
                
-                54           2 LOAD_FAST                0 (self)
+                61           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (get_distribution_name)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (dist_name)
                
-                55          42 LOAD_FAST                1 (dist_name)
+                62          42 LOAD_FAST                1 (dist_name)
                             44 POP_JUMP_FORWARD_IF_FALSE    46 (to 138)
                
-                56          46 NOP
+                63          46 NOP
                
-                57          48 LOAD_GLOBAL              3 (NULL + metadata)
+                64          48 LOAD_GLOBAL              3 (NULL + metadata)
                             60 LOAD_ATTR                2 (distribution)
                             70 LOAD_FAST                1 (dist_name)
                             72 PRECALL                  1
                             76 CALL                     1
                             86 STORE_FAST               2 (dist)
                             88 JUMP_FORWARD            22 (to 134)
                        >>   90 PUSH_EXC_INFO
                
-                58          92 LOAD_GLOBAL              2 (metadata)
+                65          92 LOAD_GLOBAL              2 (metadata)
                            104 LOAD_ATTR                3 (PackageNotFoundError)
                            114 CHECK_EXC_MATCH
                            116 POP_JUMP_FORWARD_IF_FALSE     4 (to 126)
                            118 POP_TOP
                
-                59         120 POP_EXCEPT
+                66         120 POP_EXCEPT
                            122 LOAD_CONST               1 (None)
                            124 RETURN_VALUE
                
-                58     >>  126 RERAISE                  0
+                65     >>  126 RERAISE                  0
                        >>  128 COPY                     3
                            130 POP_EXCEPT
                            132 RERAISE                  1
                
-                61     >>  134 LOAD_FAST                2 (dist)
+                68     >>  134 LOAD_FAST                2 (dist)
                            136 RETURN_VALUE
                
-                55     >>  138 LOAD_CONST               1 (None)
+                62     >>  138 LOAD_CONST               1 (None)
                            140 RETURN_VALUE
                ExceptionTable:
                  48 to 86 -> 90 [0]
                  90 to 118 -> 128 [1] lasti
                  126 to 126 -> 128 [1] lasti
                consts
                   'Get distribution of application package.'
                   None
                names      ('get_distribution_name', 'metadata', 'distribution', 'PackageNotFoundError')
                varnames   ('self', 'dist_name', 'dist')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_distribution'
-               firstlineno 52
+               firstlineno 59
                lnotab 0x02022801040102012c011c0106ff080304fa
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006401a6020000ab020000000000
                   00000072077c006a01000000000000000053007c00a00200000000000000
                   00000000000000000000000000a6000000ab0000000000000000007d017c
                   0172027c0153007c006a0300000000000000005300
-                63           0 RESUME                   0
+                70           0 RESUME                   0
                
-                65           2 LOAD_GLOBAL              1 (NULL + hasattr)
+                72           2 LOAD_GLOBAL              1 (NULL + hasattr)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_CONST               1 ('verbose_name')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_JUMP_FORWARD_IF_FALSE     7 (to 48)
                
-                66          34 LOAD_FAST                0 (self)
+                73          34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                1 (verbose_name)
                             46 RETURN_VALUE
                
-                68     >>   48 LOAD_FAST                0 (self)
+                75     >>   48 LOAD_FAST                0 (self)
                             50 LOAD_METHOD              2 (get_distribution_name)
                             72 PRECALL                  0
                             76 CALL                     0
                             86 STORE_FAST               1 (dist_name)
                
-                69          88 LOAD_FAST                1 (dist_name)
+                76          88 LOAD_FAST                1 (dist_name)
                             90 POP_JUMP_FORWARD_IF_FALSE     2 (to 96)
                
-                70          92 LOAD_FAST                1 (dist_name)
+                77          92 LOAD_FAST                1 (dist_name)
                             94 RETURN_VALUE
                
-                71     >>   96 LOAD_FAST                0 (self)
+                78     >>   96 LOAD_FAST                0 (self)
                             98 LOAD_ATTR                3 (name)
                            108 RETURN_VALUE
                consts
                   'Get name of application package.'
                   'verbose_name'
                names      ('hasattr', 'verbose_name', 'get_distribution_name', 'name')
                varnames   ('self', 'dist_name')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_name'
-               firstlineno 63
+               firstlineno 70
                lnotab 0x020220010e02280104010401
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006401a6020000ab020000000000
                   00000072077c006a01000000000000000053007c00a00200000000000000
                   00000000000000000000000000a6000000ab0000000000000000007d017c
                   0172077c016a010000000000000000530064025300
-                73           0 RESUME                   0
+                80           0 RESUME                   0
                
-                75           2 LOAD_GLOBAL              1 (NULL + hasattr)
+                82           2 LOAD_GLOBAL              1 (NULL + hasattr)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_CONST               1 ('version')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_JUMP_FORWARD_IF_FALSE     7 (to 48)
                
-                76          34 LOAD_FAST                0 (self)
+                83          34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                1 (version)
                             46 RETURN_VALUE
                
-                78     >>   48 LOAD_FAST                0 (self)
+                85     >>   48 LOAD_FAST                0 (self)
                             50 LOAD_METHOD              2 (get_distribution)
                             72 PRECALL                  0
                             76 CALL                     0
                             86 STORE_FAST               1 (dist)
                
-                79          88 LOAD_FAST                1 (dist)
+                86          88 LOAD_FAST                1 (dist)
                             90 POP_JUMP_FORWARD_IF_FALSE     7 (to 106)
                
-                80          92 LOAD_FAST                1 (dist)
+                87          92 LOAD_FAST                1 (dist)
                             94 LOAD_ATTR                1 (version)
                            104 RETURN_VALUE
                
-                82     >>  106 LOAD_CONST               2 ('unknown')
+                89     >>  106 LOAD_CONST               2 ('unknown')
                            108 RETURN_VALUE
                consts
                   'Get version of application package.'
                   'version'
                   'unknown'
                names      ('hasattr', 'version', 'get_distribution')
                varnames   ('self', 'dist')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_version'
-               firstlineno 73
+               firstlineno 80
                lnotab 0x020220010e02280104010e02
             'return'
             code
                argcount  : 1
                nlocals   : 12
                stacksize : 8
                flags     : 3
@@ -957,166 +1024,166 @@
                   020000ab0200000000000000007d0a7c0a80037c037d0a6e117c0a640c19
                   0000000000000000007d0b640d7c0b9b00640e9d037c0a640f3c0000007c
                   076410190000000000000000006f077c0a6410190000000000000000007c
                   0764103c0000007c076411190000000000000000006f077c0a6411190000
                   000000000000007c0764113c0000007c08a00b0000000000000000000000
                   0000000000000000007c0aa6010000ab01000000000000000001008c817c
                   067c077c086603530064127c027c03670166035300
-                84           0 RESUME                   0
+                91           0 RESUME                   0
                
-                88           2 LOAD_GLOBAL              1 (NULL + getattr)
+                95           2 LOAD_GLOBAL              1 (NULL + getattr)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_CONST               1 ('licence')
                             18 LOAD_CONST               2 (None)
                             20 PRECALL                  3
                             24 CALL                     3
                             34 STORE_FAST               1 (licence)
                
-                91          36 LOAD_CONST               3 (False)
+                98          36 LOAD_CONST               3 (False)
                
-                92          38 LOAD_CONST               3 (False)
+                99          38 LOAD_CONST               3 (False)
                
-                90          40 LOAD_CONST               4 (('isFsfLibre', 'isOsiApproved'))
+                97          40 LOAD_CONST               4 (('isFsfLibre', 'isOsiApproved'))
                             42 BUILD_CONST_KEY_MAP      2
                             44 STORE_FAST               2 (default_flags)
                
-                95          46 LOAD_CONST               3 (False)
+               102          46 LOAD_CONST               3 (False)
                
-                96          48 LOAD_CONST               3 (False)
+               103          48 LOAD_CONST               3 (False)
                
-                97          50 LOAD_CONST               3 (False)
+               104          50 LOAD_CONST               3 (False)
                
-                98          52 LOAD_CONST               5 ('unknown')
+               105          52 LOAD_CONST               5 ('unknown')
                
-                99          54 LOAD_CONST               6 ('Unknown Licence')
+               106          54 LOAD_CONST               6 ('Unknown Licence')
                
-               100          56 LOAD_CONST               7 (-1)
+               107          56 LOAD_CONST               7 (-1)
                
-               101          58 LOAD_CONST               8 ('')
+               108          58 LOAD_CONST               8 ('')
                
-                94          60 LOAD_CONST               9 (('isDeprecatedLicenseId', 'isFsfLibre', 'isOsiApproved', 'licenseId', 'name', 'referenceNumber', 'url'))
+               101          60 LOAD_CONST               9 (('isDeprecatedLicenseId', 'isFsfLibre', 'isOsiApproved', 'licenseId', 'name', 'referenceNumber', 'url'))
                             62 BUILD_CONST_KEY_MAP      7
                             64 STORE_FAST               3 (default_dict)
                
-               103          66 LOAD_FAST                1 (licence)
+               110          66 LOAD_FAST                1 (licence)
                             68 POP_JUMP_FORWARD_IF_FALSE   239 (to 548)
                
-               105          70 LOAD_GLOBAL              3 (NULL + Licensing)
+               112          70 LOAD_GLOBAL              3 (NULL + Licensing)
                             82 LOAD_GLOBAL              5 (NULL + LICENSES)
                             94 LOAD_ATTR                3 (keys)
                            104 PRECALL                  0
                            108 CALL                     0
                            118 PRECALL                  1
                            122 CALL                     1
                            132 STORE_FAST               4 (licensing)
                
-               106         134 LOAD_FAST                4 (licensing)
+               113         134 LOAD_FAST                4 (licensing)
                            136 LOAD_METHOD              4 (parse)
                            158 LOAD_FAST                1 (licence)
                            160 PRECALL                  1
                            164 CALL                     1
                            174 LOAD_METHOD              5 (simplify)
                            196 PRECALL                  0
                            200 CALL                     0
                            210 STORE_FAST               5 (parsed)
                
-               107         212 LOAD_FAST                5 (parsed)
+               114         212 LOAD_FAST                5 (parsed)
                            214 LOAD_METHOD              6 (render_as_readable)
                            236 PRECALL                  0
                            240 CALL                     0
                            250 STORE_FAST               6 (readable)
                
-               111         252 LOAD_CONST              10 (True)
+               118         252 LOAD_CONST              10 (True)
                
-               112         254 LOAD_CONST              10 (True)
+               119         254 LOAD_CONST              10 (True)
                
-               110         256 LOAD_CONST               4 (('isFsfLibre', 'isOsiApproved'))
+               117         256 LOAD_CONST               4 (('isFsfLibre', 'isOsiApproved'))
                            258 BUILD_CONST_KEY_MAP      2
                            260 STORE_FAST               7 (flags)
                
-               116         262 BUILD_LIST               0
+               123         262 BUILD_LIST               0
                            264 STORE_FAST               8 (licence_dicts)
                
-               117         266 LOAD_FAST                5 (parsed)
+               124         266 LOAD_FAST                5 (parsed)
                            268 LOAD_ATTR                7 (symbols)
                            278 GET_ITER
                        >>  280 FOR_ITER               128 (to 538)
                            282 STORE_FAST               9 (symbol)
                
-               119         284 LOAD_GLOBAL              5 (NULL + LICENSES)
+               126         284 LOAD_GLOBAL              5 (NULL + LICENSES)
                            296 LOAD_ATTR                8 (get)
                            306 LOAD_FAST                9 (symbol)
                            308 LOAD_ATTR                9 (key)
                            318 LOAD_METHOD             10 (rstrip)
                            340 LOAD_CONST              11 ('+')
                            342 PRECALL                  1
                            346 CALL                     1
                            356 LOAD_CONST               2 (None)
                            358 PRECALL                  2
                            362 CALL                     2
                            372 STORE_FAST              10 (licence_dict)
                
-               121         374 LOAD_FAST               10 (licence_dict)
+               128         374 LOAD_FAST               10 (licence_dict)
                            376 POP_JUMP_FORWARD_IF_NOT_NONE     3 (to 384)
                
-               123         378 LOAD_FAST                3 (default_dict)
+               130         378 LOAD_FAST                3 (default_dict)
                            380 STORE_FAST              10 (licence_dict)
                            382 JUMP_FORWARD            17 (to 418)
                
-               126     >>  384 LOAD_FAST               10 (licence_dict)
+               133     >>  384 LOAD_FAST               10 (licence_dict)
                            386 LOAD_CONST              12 ('licenseId')
                            388 BINARY_SUBSCR
                            398 STORE_FAST              11 (licence_id)
                
-               127         400 LOAD_CONST              13 ('https://spdx.org/licenses/')
+               134         400 LOAD_CONST              13 ('https://spdx.org/licenses/')
                            402 LOAD_FAST               11 (licence_id)
                            404 FORMAT_VALUE             0
                            406 LOAD_CONST              14 ('.html')
                            408 BUILD_STRING             3
                            410 LOAD_FAST               10 (licence_dict)
                            412 LOAD_CONST              15 ('url')
                            414 STORE_SUBSCR
                
-               130     >>  418 LOAD_FAST                7 (flags)
+               137     >>  418 LOAD_FAST                7 (flags)
                            420 LOAD_CONST              16 ('isFsfLibre')
                            422 BINARY_SUBSCR
                            432 JUMP_IF_FALSE_OR_POP     7 (to 448)
                            434 LOAD_FAST               10 (licence_dict)
                            436 LOAD_CONST              16 ('isFsfLibre')
                            438 BINARY_SUBSCR
                        >>  448 LOAD_FAST                7 (flags)
                            450 LOAD_CONST              16 ('isFsfLibre')
                            452 STORE_SUBSCR
                
-               131         456 LOAD_FAST                7 (flags)
+               138         456 LOAD_FAST                7 (flags)
                            458 LOAD_CONST              17 ('isOsiApproved')
                            460 BINARY_SUBSCR
                            470 JUMP_IF_FALSE_OR_POP     7 (to 486)
                            472 LOAD_FAST               10 (licence_dict)
                            474 LOAD_CONST              17 ('isOsiApproved')
                            476 BINARY_SUBSCR
                        >>  486 LOAD_FAST                7 (flags)
                            488 LOAD_CONST              17 ('isOsiApproved')
                            490 STORE_SUBSCR
                
-               133         494 LOAD_FAST                8 (licence_dicts)
+               140         494 LOAD_FAST                8 (licence_dicts)
                            496 LOAD_METHOD             11 (append)
                            518 LOAD_FAST               10 (licence_dict)
                            520 PRECALL                  1
                            524 CALL                     1
                            534 POP_TOP
                            536 JUMP_BACKWARD          129 (to 280)
                
-               135     >>  538 LOAD_FAST                6 (readable)
+               142     >>  538 LOAD_FAST                6 (readable)
                            540 LOAD_FAST                7 (flags)
                            542 LOAD_FAST                8 (licence_dicts)
                            544 BUILD_TUPLE              3
                            546 RETURN_VALUE
                
-               138     >>  548 LOAD_CONST              18 ('Unknown')
+               145     >>  548 LOAD_CONST              18 ('Unknown')
                            550 LOAD_FAST                2 (default_flags)
                            552 LOAD_FAST                3 (default_dict)
                            554 BUILD_LIST               1
                            556 BUILD_TUPLE              3
                            558 RETURN_VALUE
                consts
                   'Get tuple of licence information of application package.'
@@ -1140,77 +1207,77 @@
                   'Unknown'
                names      ('getattr', 'Licensing', 'LICENSES', 'keys', 'parse', 'simplify', 'render_as_readable', 'symbols', 'get', 'key', 'rstrip', 'append')
                varnames   ('cls', 'licence', 'default_flags', 'default_dict', 'licensing', 'parsed', 'readable', 'flags', 'licence_dicts', 'symbol', 'licence_dict', 'licence_id')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_licence'
-               firstlineno 84
+               firstlineno 91
                lnotab
                   0x02042203020102fe060502010201020102010201020102f90609040240
                   014e012804020102fe0606040112025a020402060310011203260126022c
                   020a03
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d017c016401190000000000000000007c0164
                   02190000000000000000007c0164031900000000000000000064049c0353
                   00
-               140           0 RESUME                   0
+               147           0 RESUME                   0
                
-               143           2 LOAD_FAST                0 (cls)
+               150           2 LOAD_FAST                0 (cls)
                              4 LOAD_METHOD              0 (get_licence)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (licence)
                
-               145          42 LOAD_FAST                1 (licence)
+               152          42 LOAD_FAST                1 (licence)
                             44 LOAD_CONST               1 (0)
                             46 BINARY_SUBSCR
                
-               146          56 LOAD_FAST                1 (licence)
+               153          56 LOAD_FAST                1 (licence)
                             58 LOAD_CONST               2 (1)
                             60 BINARY_SUBSCR
                
-               147          70 LOAD_FAST                1 (licence)
+               154          70 LOAD_FAST                1 (licence)
                             72 LOAD_CONST               3 (2)
                             74 BINARY_SUBSCR
                
-               144          84 LOAD_CONST               4 (('verbose_name', 'flags', 'licences'))
+               151          84 LOAD_CONST               4 (('verbose_name', 'flags', 'licences'))
                             86 BUILD_CONST_KEY_MAP      3
                             88 RETURN_VALUE
                consts
                   'Get licence information of application package.'
                   0
                   1
                   2
                   ('verbose_name', 'flags', 'licences')
                names      ('get_licence',)
                varnames   ('cls', 'licence')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_licence_dict'
-               firstlineno 140
+               firstlineno 147
                lnotab 0x020328020e010e010efd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000007c0064016900a6030000ab03000000
                   00000000005300
-               150           0 RESUME                   0
+               157           0 RESUME                   0
                
-               153           2 LOAD_GLOBAL              1 (NULL + getattr)
+               160           2 LOAD_GLOBAL              1 (NULL + getattr)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_CONST               1 ('urls')
                             18 BUILD_MAP                0
                             20 PRECALL                  3
                             24 CALL                     3
                             34 RETURN_VALUE
                consts
@@ -1218,35 +1285,35 @@
                   'urls'
                names      ('getattr',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_urls'
-               firstlineno 150
+               firstlineno 157
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d01640184007c01a001000000000000000000
                   0000000000000000000000a6000000ab0000000000000000004400a60000
                   00ab0000000000000000005300
-               156           0 RESUME                   0
+               163           0 RESUME                   0
                
-               159           2 LOAD_FAST                0 (cls)
+               166           2 LOAD_FAST                0 (cls)
                              4 LOAD_METHOD              0 (get_urls)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (urls)
                
-               160          42 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 160>)
+               167          42 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 167>)
                             44 MAKE_FUNCTION            0
                             46 LOAD_FAST                1 (urls)
                             48 LOAD_METHOD              1 (items)
                             70 PRECALL                  0
                             74 CALL                     0
                             84 GET_ITER
                             86 PRECALL                  0
@@ -1258,15 +1325,15 @@
                      argcount  : 1
                      nlocals   : 3
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d0a5c0200007d017d027c017c0264009c0291028c0b53
                         00
-                     160           0 RESUME                   0
+                     167           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                10 (to 28)
                                    8 UNPACK_SEQUENCE          2
                                   12 STORE_FAST               1 (key)
                                   14 STORE_FAST               2 (value)
                                   16 LOAD_FAST                1 (key)
@@ -1280,23 +1347,23 @@
                         ('name', 'url')
                      names      ()
                      varnames   ('.0', 'key', 'value')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                      name       '<listcomp>'
-                     firstlineno 160
+                     firstlineno 167
                      lnotab 0x
                names      ('get_urls', 'items')
                varnames   ('cls', 'urls')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_urls_dict'
-               firstlineno 156
+               firstlineno 163
                lnotab 0x02032801
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 7
                flags     : 3
                code
@@ -1305,107 +1372,107 @@
                   0167007d027c0144005d5c7d037c02a00200000000000000000000000000
                   000000000000007407000000000000000000007c03640219000000000000
                   000000740800000000000000000000a6020000ab02000000000000000072
                   087c036402190000000000000000006e14740b000000000000000000007c
                   03640219000000000000000000a6010000ab0100000000000000007c0364
                   03190000000000000000007c036404190000000000000000006603a60100
                   00ab01000000000000000001008c5d7c025300
-               162           0 RESUME                   0
+               169           0 RESUME                   0
                
-               165           2 LOAD_GLOBAL              1 (NULL + getattr)
+               172           2 LOAD_GLOBAL              1 (NULL + getattr)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_CONST               1 ('copyright_info')
                             18 LOAD_GLOBAL              3 (NULL + tuple)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 PRECALL                  3
                             48 CALL                     3
                             58 STORE_FAST               1 (copyrights)
                
-               167          60 BUILD_LIST               0
+               174          60 BUILD_LIST               0
                             62 STORE_FAST               2 (copyrights_processed)
                
-               168          64 LOAD_FAST                1 (copyrights)
+               175          64 LOAD_FAST                1 (copyrights)
                             66 GET_ITER
                        >>   68 FOR_ITER                92 (to 254)
                             70 STORE_FAST               3 (copyright_info)
                
-               169          72 LOAD_FAST                2 (copyrights_processed)
+               176          72 LOAD_FAST                2 (copyrights_processed)
                             74 LOAD_METHOD              2 (append)
                
-               173          96 LOAD_GLOBAL              7 (NULL + isinstance)
+               180          96 LOAD_GLOBAL              7 (NULL + isinstance)
                            108 LOAD_FAST                3 (copyright_info)
                            110 LOAD_CONST               2 (0)
                            112 BINARY_SUBSCR
                            122 LOAD_GLOBAL              8 (str)
                            134 PRECALL                  2
                            138 CALL                     2
                
-               172         148 POP_JUMP_FORWARD_IF_FALSE     8 (to 166)
+               179         148 POP_JUMP_FORWARD_IF_FALSE     8 (to 166)
                            150 LOAD_FAST                3 (copyright_info)
                            152 LOAD_CONST               2 (0)
                            154 BINARY_SUBSCR
                            164 JUMP_FORWARD            20 (to 206)
                
-               174     >>  166 LOAD_GLOBAL             11 (NULL + copyright_years)
+               181     >>  166 LOAD_GLOBAL             11 (NULL + copyright_years)
                            178 LOAD_FAST                3 (copyright_info)
                            180 LOAD_CONST               2 (0)
                            182 BINARY_SUBSCR
                            192 PRECALL                  1
                            196 CALL                     1
                
-               175     >>  206 LOAD_FAST                3 (copyright_info)
+               182     >>  206 LOAD_FAST                3 (copyright_info)
                            208 LOAD_CONST               3 (1)
                            210 BINARY_SUBSCR
                
-               176         220 LOAD_FAST                3 (copyright_info)
+               183         220 LOAD_FAST                3 (copyright_info)
                            222 LOAD_CONST               4 (2)
                            224 BINARY_SUBSCR
                
-               170         234 BUILD_TUPLE              3
+               177         234 BUILD_TUPLE              3
                
-               169         236 PRECALL                  1
+               176         236 PRECALL                  1
                            240 CALL                     1
                            250 POP_TOP
                            252 JUMP_BACKWARD           93 (to 68)
                
-               180     >>  254 LOAD_FAST                2 (copyrights_processed)
+               187     >>  254 LOAD_FAST                2 (copyrights_processed)
                            256 RETURN_VALUE
                consts
                   'Get copyright information tuples for application package.'
                   'copyright_info'
                   0
                   1
                   2
                names      ('getattr', 'tuple', 'append', 'isinstance', 'str', 'copyright_years')
                varnames   ('cls', 'copyrights', 'copyrights_processed', 'copyright_info')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_copyright'
-               firstlineno 162
+               firstlineno 169
                lnotab 0x02033a0204010801180434ff120228010e010efa02ff120b
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d01640184007c014400a6000000ab00000000
                   00000000005300
-               183           0 RESUME                   0
+               190           0 RESUME                   0
                
-               186           2 LOAD_FAST                0 (cls)
+               193           2 LOAD_FAST                0 (cls)
                              4 LOAD_METHOD              0 (get_copyright)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (infos)
                
-               187          42 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 187>)
+               194          42 LOAD_CONST               1 (<code object <listcomp>, file "/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py", line 194>)
                             44 MAKE_FUNCTION            0
                             46 LOAD_FAST                1 (infos)
                             48 GET_ITER
                             50 PRECALL                  0
                             54 CALL                     0
                             64 RETURN_VALUE
                consts
@@ -1415,15 +1482,15 @@
                      nlocals   : 2
                      stacksize : 6
                      flags     : 19
                      code
                         0x970067007c005d1a7d017c016400190000000000000000007c01640119
                         0000000000000000007c0164021900000000000000000064039c0391028c
                         1b5300
-                     187           0 RESUME                   0
+                     194           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                26 (to 60)
                                    8 STORE_FAST               1 (info)
                                   10 LOAD_FAST                1 (info)
                                   12 LOAD_CONST               0 (0)
                                   14 BINARY_SUBSCR
@@ -1445,89 +1512,89 @@
                         ('years', 'name', 'email')
                      names      ()
                      varnames   ('.0', 'info')
                      freevars   ()
                      cellvars   ()
                      filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                      name       '<listcomp>'
-                     firstlineno 187
+                     firstlineno 194
                      lnotab 0x
                names      ('get_copyright',)
                varnames   ('cls', 'infos')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_copyright_dicts'
-               firstlineno 183
+               firstlineno 190
                lnotab 0x02032801
             None
             'sender'
             'section'
             'name'
             'old_value'
             'new_value'
             code
                argcount  : 6
                nlocals   : 7
                stacksize : 1
                flags     : 11
                code 0x970064015300
-               189           0 RESUME                   0
+               196           0 RESUME                   0
                
-               202           2 LOAD_CONST               1 (None)
+               209           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'Call on every app instance if a dynamic preference changes, and once on startup.\n\n        By default, it does nothing.\n        '
                   None
                names      ()
                varnames   ('self', 'sender', 'section', 'name', 'old_value', 'new_value', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'preference_updated'
-               firstlineno 189
+               firstlineno 196
                lnotab 0x020d
             'app_config'
             'verbosity'
             'interactive'
             'using'
             'plan'
             'apps'
             code
                argcount  : 7
                nlocals   : 8
                stacksize : 1
                flags     : 11
                code 0x970064015300
-               204           0 RESUME                   0
+               211           0 RESUME                   0
                
-               218           2 LOAD_CONST               1 (None)
+               225           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'Call on every app instance before its models are migrated.\n\n        By default, it does nothing.\n        '
                   None
                names      ()
                varnames   ('self', 'app_config', 'verbosity', 'interactive', 'using', 'plan', 'apps', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'pre_migrate'
-               firstlineno 204
+               firstlineno 211
                lnotab 0x020e
             code
                argcount  : 5
                nlocals   : 6
                stacksize : 2
                flags     : 11
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064015300
-               220           0 RESUME                   0
+               227           0 RESUME                   0
                
-               232           2 LOAD_FAST                0 (self)
+               239           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (_maintain_default_data)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               1 (None)
                             44 RETURN_VALUE
                consts
@@ -1535,96 +1602,96 @@
                   None
                names      ('_maintain_default_data',)
                varnames   ('self', 'app_config', 'verbosity', 'interactive', 'using', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'post_migrate'
-               firstlineno 220
+               firstlineno 227
                lnotab 0x020c
             'request'
             'user'
             'User'
             code
                argcount  : 4
                nlocals   : 5
                stacksize : 1
                flags     : 11
                code 0x970064015300
-               234           0 RESUME                   0
+               241           0 RESUME                   0
                
-               241           2 LOAD_CONST               1 (None)
+               248           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'Call after a user logged in.\n\n        By default, it does nothing.\n        '
                   None
                names      ()
                varnames   ('self', 'sender', 'request', 'user', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'user_logged_in'
-               firstlineno 234
+               firstlineno 241
                lnotab 0x0207
             code
                argcount  : 4
                nlocals   : 5
                stacksize : 1
                flags     : 11
                code 0x970064015300
-               243           0 RESUME                   0
+               250           0 RESUME                   0
                
-               250           2 LOAD_CONST               1 (None)
+               257           2 LOAD_CONST               1 (None)
                              4 RETURN_VALUE
                consts
                   'Call after a user logged out.\n\n        By default, it does nothing.\n        '
                   None
                names      ()
                varnames   ('self', 'sender', 'request', 'user', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'user_logged_out'
-               firstlineno 243
+               firstlineno 250
                lnotab 0x0207
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970069005300
-               252           0 RESUME                   0
+               259           0 RESUME                   0
                
-               255           2 BUILD_MAP                0
+               262           2 BUILD_MAP                0
                              4 RETURN_VALUE
                consts
                   'Return all OAuth scopes and their descriptions for this app.'
                names      ()
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_all_scopes'
-               firstlineno 252
+               firstlineno 259
                lnotab 0x0203
             'application'
             'AbstractApplication'
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 4
                flags     : 15
                code
                   0x97007401000000000000000000007c00a0010000000000000000000000
                   000000000000000000a6000000ab000000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab000000000000000000a6
                   010000ab0100000000000000005300
-               257           0 RESUME                   0
+               264           0 RESUME                   0
                
-               266           2 LOAD_GLOBAL              1 (NULL + list)
+               273           2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_METHOD              1 (get_all_scopes)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 LOAD_METHOD              2 (keys)
                             74 PRECALL                  0
                             78 CALL                     0
@@ -1635,205 +1702,281 @@
                   'Return a list of all OAuth scopes available to the request and application.'
                names      ('list', 'get_all_scopes', 'keys')
                varnames   ('cls', 'application', 'request', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_available_scopes'
-               firstlineno 257
+               firstlineno 264
                lnotab 0x0209
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 1
                flags     : 15
                code 0x970067005300
-               268           0 RESUME                   0
+               275           0 RESUME                   0
                
-               277           2 BUILD_LIST               0
+               284           2 BUILD_LIST               0
                              4 RETURN_VALUE
                consts
                   'Return a list of all OAuth scopes to always include for this request and application.'
                names      ()
                varnames   ('cls', 'application', 'request', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_default_scopes'
-               firstlineno 268
+               firstlineno 275
                lnotab 0x0209
             'scopes'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970069005300
-               279           0 RESUME                   0
+               286           0 RESUME                   0
                
-               282           2 BUILD_MAP                0
+               289           2 BUILD_MAP                0
                              4 RETURN_VALUE
                consts
                   'Get claim data for requested scopes.'
                names      ()
                varnames   ('cls', 'scopes', 'request')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       'get_additional_claims'
-               firstlineno 279
+               firstlineno 286
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 7
                stacksize : 8
                flags     : 3
                code
-                  0x9700640164026c006d017d010100640164036c026d037d0201007c006a
-                  0400000000000000007302640053007c00a0050000000000000000000000
-                  000000000000000000a6000000ab00000000000000000044005d7c7d0374
-                  0d000000000000000000007c036404a6020000ab02000000000000000072
-                  147c03a0070000000000000000000000000000000000000000a6000000ab
-                  0000000000000000000100740d000000000000000000007c036405a60200
-                  00ab02000000000000000072467c026a080000000000000000a009000000
-                  00000000000000000000000000000000007c03a6010000ab010000000000
-                  0000007d047c036a0a000000000000000044005d245c0200007d057d067c
-                  016a080000000000000000a00b0000000000000000000000000000000000
-                  0000007c057c0464067c066901ac07a6030000ab03000000000000000001
-                  008c258c7d64005300
-               284           0 RESUME                   0
-               
-               285           2 LOAD_CONST               1 (0)
-                             4 LOAD_CONST               2 (('Permission',))
-                             6 IMPORT_NAME              0 (django.contrib.auth.models)
-                             8 IMPORT_FROM              1 (Permission)
-                            10 STORE_FAST               1 (Permission)
-                            12 POP_TOP
-               
-               286          14 LOAD_CONST               1 (0)
-                            16 LOAD_CONST               3 (('ContentType',))
-                            18 IMPORT_NAME              2 (django.contrib.contenttypes.models)
-                            20 IMPORT_FROM              3 (ContentType)
-                            22 STORE_FAST               2 (ContentType)
-                            24 POP_TOP
-               
-               288          26 LOAD_FAST                0 (self)
-                            28 LOAD_ATTR                4 (models_module)
-                            38 POP_JUMP_FORWARD_IF_TRUE     2 (to 44)
-               
-               290          40 LOAD_CONST               0 (None)
-                            42 RETURN_VALUE
-               
-               292     >>   44 LOAD_FAST                0 (self)
-                            46 LOAD_METHOD              5 (get_models)
-                            68 PRECALL                  0
-                            72 CALL                     0
-                            82 GET_ITER
-                       >>   84 FOR_ITER               124 (to 334)
-                            86 STORE_FAST               3 (model)
-               
-               293          88 LOAD_GLOBAL             13 (NULL + hasattr)
-                           100 LOAD_FAST                3 (model)
-                           102 LOAD_CONST               4 ('maintain_default_data')
-                           104 PRECALL                  2
-                           108 CALL                     2
-                           118 POP_JUMP_FORWARD_IF_FALSE    20 (to 160)
-               
-               295         120 LOAD_FAST                3 (model)
-                           122 LOAD_METHOD              7 (maintain_default_data)
-                           144 PRECALL                  0
-                           148 CALL                     0
-                           158 POP_TOP
-               
-               296     >>  160 LOAD_GLOBAL             13 (NULL + hasattr)
-                           172 LOAD_FAST                3 (model)
-                           174 LOAD_CONST               5 ('extra_permissions')
-                           176 PRECALL                  2
-                           180 CALL                     2
-                           190 POP_JUMP_FORWARD_IF_FALSE    70 (to 332)
-               
-               297         192 LOAD_FAST                2 (ContentType)
-                           194 LOAD_ATTR                8 (objects)
-                           204 LOAD_METHOD              9 (get_for_model)
-                           226 LOAD_FAST                3 (model)
-                           228 PRECALL                  1
-                           232 CALL                     1
-                           242 STORE_FAST               4 (ct)
-               
-               298         244 LOAD_FAST                3 (model)
-                           246 LOAD_ATTR               10 (extra_permissions)
-                           256 GET_ITER
-                       >>  258 FOR_ITER                36 (to 332)
-                           260 UNPACK_SEQUENCE          2
-                           264 STORE_FAST               5 (perm)
-                           266 STORE_FAST               6 (verbose_name)
-               
-               299         268 LOAD_FAST                1 (Permission)
-                           270 LOAD_ATTR                8 (objects)
-                           280 LOAD_METHOD             11 (get_or_create)
-               
-               300         302 LOAD_FAST                5 (perm)
-               
-               301         304 LOAD_FAST                4 (ct)
-               
-               302         306 LOAD_CONST               6 ('name')
-                           308 LOAD_FAST                6 (verbose_name)
-                           310 BUILD_MAP                1
-               
-               299         312 KW_NAMES                 7
-                           314 PRECALL                  3
-                           318 CALL                     3
-                           328 POP_TOP
-                           330 JUMP_BACKWARD           37 (to 258)
-                       >>  332 JUMP_BACKWARD          125 (to 84)
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  0000000000000064017c00a0020000000000000000000000000000000000
+                  000000a6000000ab000000000000000000a6020000ab0200000000000000
+                  000100640264036c036d047d010100640264046c056d067d0201007c006a
+                  0700000000000000007302640053007c00a0080000000000000000000000
+                  000000000000000000a6000000ab000000000000000000440090015d097d
+                  037413000000000000000000007c036405a6020000ab0200000000000000
+                  00724c7c006a000000000000000000a00a00000000000000000000000000
+                  0000000000000064067c036a0b00000000000000006a0c00000000000000
+                  007c00a0020000000000000000000000000000000000000000a6000000ab
+                  000000000000000000a6030000ab03000000000000000001007c03a00d00
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  00000001007413000000000000000000007c036407a6020000ab02000000
+                  0000000000729a7c006a000000000000000000a00a000000000000000000
+                  000000000000000000000064087c036a0b00000000000000006a0c000000
+                  00000000007c00a0020000000000000000000000000000000000000000a6
+                  000000ab000000000000000000a6030000ab03000000000000000001007c
+                  026a0e0000000000000000a00f0000000000000000000000000000000000
+                  0000007c03a6010000ab0100000000000000007d047c036a100000000000
+                  00000044005d405c0200007d057d067c006a000000000000000000a00100
+                  0000000000000000000000000000000000000064097c057c06a6030000ab
+                  03000000000000000001007c016a0e0000000000000000a0110000000000
+                  0000000000000000000000000000007c057c04640a7c066901ac0ba60300
+                  00ab03000000000000000001008c4190018c0b64005300
+               291           0 RESUME                   0
+               
+               292           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (_logger)
+                            14 LOAD_METHOD              1 (debug)
+                            36 LOAD_CONST               1 ('Maintaining default data for %s')
+                            38 LOAD_FAST                0 (self)
+                            40 LOAD_METHOD              2 (get_name)
+                            62 PRECALL                  0
+                            66 CALL                     0
+                            76 PRECALL                  2
+                            80 CALL                     2
+                            90 POP_TOP
+               
+               294          92 LOAD_CONST               2 (0)
+                            94 LOAD_CONST               3 (('Permission',))
+                            96 IMPORT_NAME              3 (django.contrib.auth.models)
+                            98 IMPORT_FROM              4 (Permission)
+                           100 STORE_FAST               1 (Permission)
+                           102 POP_TOP
+               
+               295         104 LOAD_CONST               2 (0)
+                           106 LOAD_CONST               4 (('ContentType',))
+                           108 IMPORT_NAME              5 (django.contrib.contenttypes.models)
+                           110 IMPORT_FROM              6 (ContentType)
+                           112 STORE_FAST               2 (ContentType)
+                           114 POP_TOP
+               
+               297         116 LOAD_FAST                0 (self)
+                           118 LOAD_ATTR                7 (models_module)
+                           128 POP_JUMP_FORWARD_IF_TRUE     2 (to 134)
+               
+               299         130 LOAD_CONST               0 (None)
+                           132 RETURN_VALUE
+               
+               301     >>  134 LOAD_FAST                0 (self)
+                           136 LOAD_METHOD              8 (get_models)
+                           158 PRECALL                  0
+                           162 CALL                     0
+                           172 GET_ITER
+                       >>  174 EXTENDED_ARG             1
+                           176 FOR_ITER               265 (to 708)
+                           178 STORE_FAST               3 (model)
+               
+               302         180 LOAD_GLOBAL             19 (NULL + hasattr)
+                           192 LOAD_FAST                3 (model)
+                           194 LOAD_CONST               5 ('maintain_default_data')
+                           196 PRECALL                  2
+                           200 CALL                     2
+                           210 POP_JUMP_FORWARD_IF_FALSE    76 (to 364)
+               
+               304         212 LOAD_FAST                0 (self)
+                           214 LOAD_ATTR                0 (_logger)
+                           224 LOAD_METHOD             10 (info)
+               
+               305         246 LOAD_CONST               6 ('Maintaining default data of %s in %s')
+                           248 LOAD_FAST                3 (model)
+                           250 LOAD_ATTR               11 (_meta)
+                           260 LOAD_ATTR               12 (model_name)
+                           270 LOAD_FAST                0 (self)
+                           272 LOAD_METHOD              2 (get_name)
+                           294 PRECALL                  0
+                           298 CALL                     0
+               
+               304         308 PRECALL                  3
+                           312 CALL                     3
+                           322 POP_TOP
+               
+               307         324 LOAD_FAST                3 (model)
+                           326 LOAD_METHOD             13 (maintain_default_data)
+                           348 PRECALL                  0
+                           352 CALL                     0
+                           362 POP_TOP
+               
+               308     >>  364 LOAD_GLOBAL             19 (NULL + hasattr)
+                           376 LOAD_FAST                3 (model)
+                           378 LOAD_CONST               7 ('extra_permissions')
+                           380 PRECALL                  2
+                           384 CALL                     2
+                           394 POP_JUMP_FORWARD_IF_FALSE   154 (to 704)
+               
+               309         396 LOAD_FAST                0 (self)
+                           398 LOAD_ATTR                0 (_logger)
+                           408 LOAD_METHOD             10 (info)
+               
+               310         430 LOAD_CONST               8 ('Maintaining extra permissions for %s in %s')
+               
+               311         432 LOAD_FAST                3 (model)
+                           434 LOAD_ATTR               11 (_meta)
+                           444 LOAD_ATTR               12 (model_name)
+               
+               312         454 LOAD_FAST                0 (self)
+                           456 LOAD_METHOD              2 (get_name)
+                           478 PRECALL                  0
+                           482 CALL                     0
+               
+               309         492 PRECALL                  3
+                           496 CALL                     3
+                           506 POP_TOP
+               
+               314         508 LOAD_FAST                2 (ContentType)
+                           510 LOAD_ATTR               14 (objects)
+                           520 LOAD_METHOD             15 (get_for_model)
+                           542 LOAD_FAST                3 (model)
+                           544 PRECALL                  1
+                           548 CALL                     1
+                           558 STORE_FAST               4 (ct)
+               
+               315         560 LOAD_FAST                3 (model)
+                           562 LOAD_ATTR               16 (extra_permissions)
+                           572 GET_ITER
+                       >>  574 FOR_ITER                64 (to 704)
+                           576 UNPACK_SEQUENCE          2
+                           580 STORE_FAST               5 (perm)
+                           582 STORE_FAST               6 (verbose_name)
+               
+               316         584 LOAD_FAST                0 (self)
+                           586 LOAD_ATTR                0 (_logger)
+                           596 LOAD_METHOD              1 (debug)
+                           618 LOAD_CONST               9 ('Creating %s (%s)')
+                           620 LOAD_FAST                5 (perm)
+                           622 LOAD_FAST                6 (verbose_name)
+                           624 PRECALL                  3
+                           628 CALL                     3
+                           638 POP_TOP
+               
+               317         640 LOAD_FAST                1 (Permission)
+                           642 LOAD_ATTR               14 (objects)
+                           652 LOAD_METHOD             17 (get_or_create)
+               
+               318         674 LOAD_FAST                5 (perm)
+               
+               319         676 LOAD_FAST                4 (ct)
+               
+               320         678 LOAD_CONST              10 ('name')
+                           680 LOAD_FAST                6 (verbose_name)
+                           682 BUILD_MAP                1
+               
+               317         684 KW_NAMES                11
+                           686 PRECALL                  3
+                           690 CALL                     3
+                           700 POP_TOP
+                           702 JUMP_BACKWARD           65 (to 574)
+                       >>  704 EXTENDED_ARG             1
+                           706 JUMP_BACKWARD          267 (to 174)
                
-               292     >>  334 LOAD_CONST               0 (None)
-                           336 RETURN_VALUE
+               301     >>  708 LOAD_CONST               0 (None)
+                           710 RETURN_VALUE
                consts
                   None
+                  'Maintaining default data for %s'
                   0
                   ('Permission',)
                   ('ContentType',)
                   'maintain_default_data'
+                  'Maintaining default data of %s in %s'
                   'extra_permissions'
+                  'Maintaining extra permissions for %s in %s'
+                  'Creating %s (%s)'
                   'name'
                   ('codename', 'content_type', 'defaults')
-               names      ('django.contrib.auth.models', 'Permission', 'django.contrib.contenttypes.models', 'ContentType', 'models_module', 'get_models', 'hasattr', 'maintain_default_data', 'objects', 'get_for_model', 'extra_permissions', 'get_or_create')
+               names      ('_logger', 'debug', 'get_name', 'django.contrib.auth.models', 'Permission', 'django.contrib.contenttypes.models', 'ContentType', 'models_module', 'get_models', 'hasattr', 'info', '_meta', 'model_name', 'maintain_default_data', 'objects', 'get_for_model', 'extra_permissions', 'get_or_create')
                varnames   ('self', 'Permission', 'ContentType', 'model', 'ct', 'perm', 'verbose_name')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
                name       '_maintain_default_data'
-               firstlineno 284
+               firstlineno 291
                lnotab
-                  0x02010c010c020e0204022c012002280120013401180122010201020106
-                  fd16f9
+                  0x02015a020c010c020e0204022e01200222013eff100328012001220102
+                  01160126fd100534011801380122010201020106fd18f0
             (None, None, None, None)
             (None, None)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'default', 'default_auto_field', '__init_subclass__', 'ready', 'get_distribution_name', 'get_distribution', 'get_name', 'get_version', 'classmethod', 'tuple', 'get_licence', 'get_licence_dict', 'get_urls', 'get_urls_dict', 'Sequence', 'str', 'get_copyright', 'get_copyright_dicts', 'Any', 'Optional', 'preference_updated', 'django', 'apps', 'AppConfig', 'int', 'bool', 'list', 'registry', 'Apps', 'pre_migrate', 'post_migrate', 'type', 'HttpRequest', 'user_logged_in', 'user_logged_out', 'dict', 'get_all_scopes', 'get_available_scopes', 'get_default_scopes', 'OauthlibRequest', 'get_additional_claims', '_maintain_default_data', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
          name       'AppConfig'
-         firstlineno 20
+         firstlineno 21
          lnotab
-            0x0c010402040104020a040a0d0609060b060a060b02010aff0e01023702
+            0x0c010402040104020a050a120609060b060a060b02010aff0e01023702
             0104ff0e010209020104ff0e010205020104ff0e010205020128ff0e0102
             14020104ff0e01020802010201020102fa040202fe02030efd02040efc02
             050efb02060efa020802f8080f020216fe020302fd020402fc020502fb02
             060efa020720f9020902f70810020216fe020302fd020402fc020502fb02
             0702f9080e020102ff02010eff020102ff020202fe0809020102ff02010e
             ff020102ff020202fe080902011aff0e0102040203020102fd04020efe02
             030efd02060efa06ff0e01020a0203020102fd04020efe02030efd02060e
             fa06ff0e01020a02012eff0e010204
       'AppConfig'
-   names      ('importlib', 'metadata', 'typing', 'TYPE_CHECKING', 'Any', 'Optional', 'Sequence', 'django.apps', 'django', 'django.contrib.auth.signals', 'user_logged_in', 'user_logged_out', 'django.db.models.signals', 'post_migrate', 'pre_migrate', 'django.http', 'HttpRequest', 'dynamic_preferences.signals', 'preference_updated', 'license_expression', 'Licensing', 'oauthlib.common', 'Request', 'OauthlibRequest', 'core_helpers', 'copyright_years', 'spdx', 'LICENSES', 'oauth2_provider.models', 'AbstractApplication', 'apps', 'AppConfig')
+   names      ('logging', 'importlib', 'metadata', 'typing', 'TYPE_CHECKING', 'Any', 'Optional', 'Sequence', 'django.apps', 'django', 'django.contrib.auth.signals', 'user_logged_in', 'user_logged_out', 'django.db.models.signals', 'post_migrate', 'pre_migrate', 'django.http', 'HttpRequest', 'dynamic_preferences.signals', 'preference_updated', 'license_expression', 'Licensing', 'oauthlib.common', 'Request', 'OauthlibRequest', 'core_helpers', 'copyright_years', 'spdx', 'LICENSES', 'oauth2_provider.models', 'AbstractApplication', 'apps', 'AppConfig')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/util/apps.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c0118020801100110010c020c010c010c020c010c0204010c
-      03
+      0x00ff020108010c0118020801100110010c020c010c010c020c010c0204
+      010c03
```

### Comparing `aleksis_core-3.1.1/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 7920
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 26
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 16042
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/util/__pycache__/email.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/util/__pycache__/email.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 986
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 850
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/util/__pycache__/notifications.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/util/__pycache__/notifications.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 3732
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/util/__pycache__/predicates.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/util/__pycache__/predicates.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 5583
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 936
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/util/__pycache__/spdx.cpython-311.pyc` & `aleksis_core-3.1.2/aleksis/core/util/__pycache__/spdx.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xafbfa064 (Sun Jul  2 00:07:11 2023 UTC)
+moddate:  0x83caa564 (Wed Jul  5 19:54:43 2023 UTC)
 files sz: 130
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-3.1.1/aleksis/core/util/apps.py` & `aleksis_core-3.1.2/aleksis/core/util/apps.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from importlib import metadata
 from typing import TYPE_CHECKING, Any, Optional, Sequence
 
 import django.apps
 from django.contrib.auth.signals import user_logged_in, user_logged_out
 from django.db.models.signals import post_migrate, pre_migrate
 from django.http import HttpRequest
@@ -22,27 +23,33 @@
 
     default = False
     default_auto_field = "django.db.models.BigAutoField"
 
     def __init_subclass__(cls):
         super().__init_subclass__()
         cls.default = True
+        cls._logger = logging.getLogger(f"{cls.__module__}.{cls.__name__}")
 
     def ready(self):
+        self._logger.debug("Running app.ready")
+
         super().ready()
 
         # Register default listeners
         pre_migrate.connect(self.pre_migrate, sender=self)
         post_migrate.connect(self.post_migrate, sender=self)
         preference_updated.connect(self.preference_updated)
         user_logged_in.connect(self.user_logged_in)
         user_logged_out.connect(self.user_logged_out)
+        self._logger.debug("Default signal handlers connected")
 
         # Getting an app ready means it should look at its config once
+        self._logger.debug("Force-loading preferences")
         self.preference_updated(self)
+        self._logger.debug("Preferences loaded")
 
     def get_distribution_name(self):
         """Get distribution name of application package."""
         if hasattr(self, "dist_name"):
             return self.dist_name
         elif self.name.lower().startswith("aleksis.apps."):
             return self.name.lower().replace("aleksis.apps.", "AlekSIS-App-")
@@ -278,26 +285,37 @@
 
     @classmethod
     def get_additional_claims(cls, scopes: list[str], request: OauthlibRequest) -> dict[str, Any]:
         """Get claim data for requested scopes."""
         return {}
 
     def _maintain_default_data(self):
+        self._logger.debug("Maintaining default data for %s", self.get_name())
+
         from django.contrib.auth.models import Permission
         from django.contrib.contenttypes.models import ContentType
 
         if not self.models_module:
             # This app does not have any models, so bail out early
             return
 
         for model in self.get_models():
             if hasattr(model, "maintain_default_data"):
                 # Method implemented by each model object; can be left out
+                self._logger.info(
+                    "Maintaining default data of %s in %s", model._meta.model_name, self.get_name()
+                )
                 model.maintain_default_data()
             if hasattr(model, "extra_permissions"):
+                self._logger.info(
+                    "Maintaining extra permissions for %s in %s",
+                    model._meta.model_name,
+                    self.get_name(),
+                )
                 ct = ContentType.objects.get_for_model(model)
                 for perm, verbose_name in model.extra_permissions:
+                    self._logger.debug("Creating %s (%s)", perm, verbose_name)
                     Permission.objects.get_or_create(
                         codename=perm,
                         content_type=ct,
                         defaults={"name": verbose_name},
                     )
```

### Comparing `aleksis_core-3.1.1/aleksis/core/util/auth_helpers.py` & `aleksis_core-3.1.2/aleksis/core/util/auth_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/celery_progress.py` & `aleksis_core-3.1.2/aleksis/core/util/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/core_helpers.py` & `aleksis_core-3.1.2/aleksis/core/util/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/email.py` & `aleksis_core-3.1.2/aleksis/core/util/email.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/forms.py` & `aleksis_core-3.1.2/aleksis/core/util/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/frontend_helpers.py` & `aleksis_core-3.1.2/aleksis/core/util/frontend_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/ldap.py` & `aleksis_core-3.1.2/aleksis/core/util/ldap.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/licenses.json` & `aleksis_core-3.1.2/aleksis/core/util/licenses.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/messages.py` & `aleksis_core-3.1.2/aleksis/core/util/messages.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/middlewares.py` & `aleksis_core-3.1.2/aleksis/core/util/middlewares.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/model_helpers.py` & `aleksis_core-3.1.2/aleksis/core/util/model_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/notifications.py` & `aleksis_core-3.1.2/aleksis/core/util/notifications.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/pdf.py` & `aleksis_core-3.1.2/aleksis/core/util/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/predicates.py` & `aleksis_core-3.1.2/aleksis/core/util/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/sass_helpers.py` & `aleksis_core-3.1.2/aleksis/core/util/sass_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/search.py` & `aleksis_core-3.1.2/aleksis/core/util/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/util/tables.py` & `aleksis_core-3.1.2/aleksis/core/util/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/views.py` & `aleksis_core-3.1.2/aleksis/core/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/aleksis/core/vite.config.js` & `aleksis_core-3.1.2/aleksis/core/vite.config.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -206,15 +206,17 @@
             },
             scope: "/",
             base: "/",
             workbox: {
                 navigateFallback: "/",
                 directoryIndex: null,
                 navigateFallbackAllowlist: [
-                    new RegExp("^/(?!(django|admin|graphql|__icons__))[^.]*$"),
+                    new RegExp(
+                        "^/(?!(django|admin|graphql|__icons__|oauth/authorize))[^.]*$"
+                    ),
                 ],
                 additionalManifestEntries: [{
                     url: "/",
                     revision: crypto.randomUUID()
                 }, {
                     url: "/django/offline/",
                     revision: crypto.randomUUID()
@@ -222,15 +224,15 @@
                 inlineWorkboxRuntime: true,
                 modifyURLPrefix: {
                     "": "/static/",
                 },
                 globPatterns: ["**/*.{js,css,eot,woff,woff2,ttf}"],
                 runtimeCaching: [{
                     urlPattern: new RegExp(
-                        "^/(?!(django|admin|graphql|__icons__))[^.]*$"
+                        "^/(?!(django|admin|graphql|__icons__|oauth/authorize))[^.]*$"
                     ),
                     handler: "CacheFirst",
                 }, {
                     urlPattern: new RegExp("/django/.*"),
                     handler: "NetworkFirst",
                     options: {
                         cacheName: "aleksis-legacy-cache",
```

### Comparing `aleksis_core-3.1.1/docs/Makefile` & `aleksis_core-3.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/2fa.png` & `aleksis_core-3.1.2/docs/_static/2fa.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/accept_invite.png` & `aleksis_core-3.1.2/docs/_static/accept_invite.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/create_dashboard_widget.png` & `aleksis_core-3.1.2/docs/_static/create_dashboard_widget.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/create_social_application.png` & `aleksis_core-3.1.2/docs/_static/create_social_application.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/dashboard.png` & `aleksis_core-3.1.2/docs/_static/dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/dashboard_widgets.png` & `aleksis_core-3.1.2/docs/_static/dashboard_widgets.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/data_checks.png` & `aleksis_core-3.1.2/docs/_static/data_checks.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/edit_dashboard.png` & `aleksis_core-3.1.2/docs/_static/edit_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/edit_default_dashboard.png` & `aleksis_core-3.1.2/docs/_static/edit_default_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/invitations.png` & `aleksis_core-3.1.2/docs/_static/invitations.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/invite_existing.png` & `aleksis_core-3.1.2/docs/_static/invite_existing.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/pwa_desktop_chromium.png` & `aleksis_core-3.1.2/docs/_static/pwa_desktop_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/pwa_mobile_chromium.png` & `aleksis_core-3.1.2/docs/_static/pwa_mobile_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/pwa_mobile_firefox.png` & `aleksis_core-3.1.2/docs/_static/pwa_mobile_firefox.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/pwa_mobile_safari.png` & `aleksis_core-3.1.2/docs/_static/pwa_mobile_safari.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/_static/signup.png` & `aleksis_core-3.1.2/docs/_static/signup.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/01_core_concepts.rst` & `aleksis_core-3.1.2/docs/admin/01_core_concepts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/10_install.rst` & `aleksis_core-3.1.2/docs/admin/10_install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
    apt install libmariadb-dev libldap2-dev libsasl2-dev
 
 After that, you can install the aleksis meta-package, or only `aleksis-core`:
 
 .. code-block:: shell
    pip3 install --break-system-packages aleksis
    aleksis-admin vite build
-   aleksis-admin collectstatic
+   aleksis-admin collectstatic --clear
    aleksis-admin migrate
    aleksis-admin createinitialrevisions
 
 Make dynamic content writable for webserver
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To make AlekSIS® able to write dynamic content, you need to assign permissions to the webserver user.
```

### Comparing `aleksis_core-3.1.1/docs/admin/15_config_files.rst` & `aleksis_core-3.1.2/docs/admin/15_config_files.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/16_config_options.rst` & `aleksis_core-3.1.2/docs/admin/16_config_options.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/17_storage.rst` & `aleksis_core-3.1.2/docs/admin/17_storage.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/18_mail.rst` & `aleksis_core-3.1.2/docs/admin/18_mail.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/21_ldap.rst` & `aleksis_core-3.1.2/docs/admin/21_ldap.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/22_registration.rst` & `aleksis_core-3.1.2/docs/admin/22_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/23_socialaccounts.rst` & `aleksis_core-3.1.2/docs/admin/23_socialaccounts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/31_monitoring.rst` & `aleksis_core-3.1.2/docs/admin/31_monitoring.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/32_tasks.rst` & `aleksis_core-3.1.2/docs/admin/32_tasks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/33_data_checks.rst` & `aleksis_core-3.1.2/docs/admin/33_data_checks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/admin/50_dashboard.rst` & `aleksis_core-3.1.2/docs/admin/50_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/conf.py` & `aleksis_core-3.1.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-Core"
 copyright = "2019-2023 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.1"
 # The full version, including alpha/beta/rc tags
-release = "3.1.1"
+release = "3.1.2"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_core-3.1.1/docs/dev/01_setup.rst` & `aleksis_core-3.1.2/docs/dev/01_setup.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 AlekSIS and all official apps use `Poetry`_ to manage virtualenvs and
 dependencies. You should make yourself a bit comfortable with poetry
 by reading its documentation.
 
 Poetry makes a lot of stuff very easy, especially managing a virtual
 environment that contains AlekSIS and everything you need to run the
-framework and selected apps.
+framework and selected apps. The minimum supported version of Poetry
+is 1.2.0.
 
 Also, `Yarn`_ is needed to resolve JavaScript dependencies.
 
 For repository management, `myrepos` is required.
 
 Setup database and message broker
 ---------------------------------
@@ -87,15 +88,15 @@
 3. Run database migrations
 
 All three steps can be done with the ``poetry shell`` command and
 ``aleksis-admin``::
 
   ALEKSIS_maintenance__debug=true ALEKSIS_database__password=aleksis poetry shell
    poetry run aleksis-admin vite build
-   poetry run aleksis-admin collectstatic
+   poetry run aleksis-admin collectstatic --clear
    poetry run aleksis-admin compilemessages
    poetry run aleksis-admin migrate
    poetry run aleksis-admin createinitialrevisions
 
 Running the development server
 ------------------------------
```

### Comparing `aleksis_core-3.1.1/docs/dev/02_install_apps.rst` & `aleksis_core-3.1.2/docs/dev/02_install_apps.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/dev/03_run_tests.rst` & `aleksis_core-3.1.2/docs/dev/03_run_tests.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/dev/04_materialize_templates.rst` & `aleksis_core-3.1.2/docs/dev/04_materialize_templates.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/dev/06_merging_app_settings.rst` & `aleksis_core-3.1.2/docs/dev/06_merging_app_settings.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/dev/10_dashboard_widgets.rst` & `aleksis_core-3.1.2/docs/dev/10_dashboard_widgets.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/index.rst` & `aleksis_core-3.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/make.bat` & `aleksis_core-3.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/ref/core/09_utils.rst` & `aleksis_core-3.1.2/docs/ref/core/09_utils.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/user/01_registration.rst` & `aleksis_core-3.1.2/docs/user/01_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/user/02_personal_account.rst` & `aleksis_core-3.1.2/docs/user/02_personal_account.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/user/10_dashboard.rst` & `aleksis_core-3.1.2/docs/user/10_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/docs/user/20_pwa.rst` & `aleksis_core-3.1.2/docs/user/20_pwa.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/pyproject.toml` & `aleksis_core-3.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-Core"
-version = "3.1.1"
+version = "3.1.2"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -24,20 +24,17 @@
     "Jonathan Weth <dev@jonathanweth.de>",
     "Hangzhi Yu <yuha@katharineum.de>",
     "Lloyd Meins <meinsll@katharineum.de>",
     "magicfelix <felix@felix-zauberer.de>",
     "Benedict Suska <benedict.suska@teckids.de>",
     "Lukas Weichelt <lukas.weichelt@teckids.de>"
 ]
-maintainers = [
-    "Jonathan Weth <dev@jonathanweth.de>",
-    "Dominik George <dominik.george@teckids.org>"
-]
+maintainers = ["Jonathan Weth <dev@jonathanweth.de>", "Dominik George <dominik.george@teckids.org>"]
 license = "EUPL-1.2-or-later"
-homepage = "https://aleksis.org/"
+homepage = "https://aleksis.org"
 repository = "https://edugit.org/AlekSIS/official/AlekSIS-Core"
 documentation = "https://aleksis.org/AlekSIS-Core/docs/html/"
 keywords = ["SIS", "education", "school", "digitisation", "school apps"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Django :: 4.1",
@@ -46,18 +43,21 @@
     "Topic :: Education",
     "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Typing :: Typed",
 ]
 
 [[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
+
+[[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
-secondary = true
-
+priority = "supplemental"
 [tool.poetry.dependencies]
 python = "^3.9"
 Django = "^4.1"
 django-any-js = "^1.1"
 django-tables2 = "^2.1"
 django-phonenumber-field = {version = "^6.1", extras = ["phonenumbers"]}
 django-sass-processor = "1.2.2"
@@ -123,28 +123,65 @@
 django-cte = "^1.1.5"
 pycountry = "^22.0.0"
 django-iconify = "^0.3"
 customidenticon = "^0.1.5"
 graphene-django = "^3.0.0"
 selenium = "^4.4.3"
 django-vite = "^2.0.2"
+uwsgi = "^2.0.21"
 
 [tool.poetry.extras]
 ldap = ["django-auth-ldap"]
 s3 = ["boto3", "django-storages"]
 sentry = ["sentry-sdk"]
 
-[tool.poetry.dev-dependencies]
-aleksis-builddeps = {version=">=2023.1.dev0", allow-prereleases=true}
-selenium = "<4.10.0"
-uwsgi = "^2.0"
-
 [tool.poetry.scripts]
 aleksis-admin = 'aleksis.core.__main__:aleksis_cmd'
 
+[tool.poetry.group.dev.dependencies]
+django-stubs = "^4.2"
+
+safety = "^2.3.5"
+
+flake8 = "^6.0.0"
+flake8-django = "^1.0.0"
+flake8-fixme = "^1.1.1"
+flake8-mypy = "^17.8.0"
+flake8-bandit = "^4.1.1"
+flake8-builtins = "^2.0.0"
+flake8-docstrings = "^1.5.0"
+flake8-rst-docstrings = "^0.3.0"
+
+black = ">=21.0"
+flake8-black = "^0.3.0"
+
+isort = "^5.0.0"
+flake8-isort = "^6.0.0"
+
+curlylint = "^0.13.0"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.2"
+pytest-django = "^4.1"
+pytest-django-testing-postgresql = "^0.2"
+pytest-cov = "^4.0.0"
+pytest-sugar = "^0.9.2"
+selenium = "<4.10.0"
+freezegun = "^1.1.0"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.0"
+sphinxcontrib-django = "^2.3.0"
+sphinxcontrib-svg2pdfconverter = "^1.1.1"
+sphinx-autodoc-typehints = "^1.7"
+sphinx_material = "^0.0.35"
+
 [tool.black]
 line-length = 100
 exclude = "/migrations/"
 
 [build-system]
-requires = ["poetry>=1.0"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `aleksis_core-3.1.1/tox.ini` & `aleksis_core-3.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.1.1/PKG-INFO` & `aleksis_core-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aleksis-core
-Version: 3.1.1
+Version: 3.1.2
 Summary: AlekSIS (School Information System) — Core
-Home-page: https://aleksis.org/
+Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,digitisation,school apps
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
 Maintainer-email: dev@jonathanweth.de
 Requires-Python: >=3.9,<4.0
@@ -94,14 +94,15 @@
 Requires-Dist: psutil (>=5.7.0,<6.0.0)
 Requires-Dist: psycopg2 (>=2.8,<3.0)
 Requires-Dist: pycountry (>=22.0.0,<23.0.0)
 Requires-Dist: python-gnupg (>=0.5.0,<0.6.0)
 Requires-Dist: rules (>=3.0,<4.0)
 Requires-Dist: selenium (>=4.4.3,<5.0.0)
 Requires-Dist: sentry-sdk (>=1.4.3,<2.0.0) ; extra == "sentry"
+Requires-Dist: uwsgi (>=2.0.21,<3.0.0)
 Project-URL: Documentation, https://aleksis.org/AlekSIS-Core/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-Core
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — Core (Core functionality and app framework)
 =================================================================================
```

