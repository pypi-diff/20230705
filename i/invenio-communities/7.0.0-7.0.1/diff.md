# Comparing `tmp/invenio-communities-7.0.0.tar.gz` & `tmp/invenio-communities-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-communities-7.0.0.tar", last modified: Thu Jun 15 11:49:07 2023, max compression
+gzip compressed data, was "dist/invenio-communities-7.0.1.tar", last modified: Wed Jul  5 16:03:26 2023, max compression
```

## Comparing `invenio-communities-7.0.0.tar` & `invenio-communities-7.0.1.tar`

### file list

```diff
@@ -1,657 +1,741 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.eslintrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.prettierrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/administration/communities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/02cd82910727_update_role_id_type_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/37b21951084c_update_role_id_type_downgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/90642d415317_create_communities_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/alembic/fbe746957cfc_create_member_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/api.js
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/GroupsApi.js
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/UsersApi.js
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CommunitiesCarousel.js
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/CommunityTypeLabel.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/context.js
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/context.js
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/index.js
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/appUrls.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/
--rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)   130749 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/cache/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/dumpers/featured.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/entity_resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v1/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v2/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/v7/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/pidslug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/resources/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/communities/services/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/communities/services/uow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/fixtures/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/fixtures/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/members/services/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    24616 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/members/services/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/notifications/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/records/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/records/records/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/searchapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_details.html
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_search.html
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/access-status-label.html
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/communities_carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/new.html
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/request.html
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13804 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/invenio_communities/views/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/views/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/views/communities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/views/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/views/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/invenio_communities/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32162 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 11:49:06.000000 invenio-communities-7.0.0/invenio_communities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/run-js-linter.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/cache/test_identity_redis_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_alembic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_community_ui_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_relations_organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_relations_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29959 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/communities/tests_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/members/
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/members/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/members/test_members_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/members/test_members_no_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/members/test_members_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    34235 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/members/test_members_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/jsonschemas/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/jsonschemas/mocks/mock-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v6/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v6/mocks/mock-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:49:07.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v7/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/mappings/v7/mocks/mock-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/mock_module/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/records/test_mockrecords_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-15 11:48:57.000000 invenio-communities-7.0.0/tests/test_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/.eslintrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/.prettierrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/administration/communities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/alembic/02cd82910727_update_role_id_type_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/alembic/37b21951084c_update_role_id_type_downgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/alembic/90642d415317_create_communities_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/alembic/fbe746957cfc_create_member_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/GroupsApi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/UsersApi.js
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CommunitiesCarousel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/CommunityTypeLabel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/context.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/context.js
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/routes/appUrls.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de_AT/
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de_AT/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de_DE/
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de_DE/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en_AT/
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en_AT/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en_HU/
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en_HU/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es_CU/
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es_CU/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es_MX/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es_MX/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa_IR/
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa_IR/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr_CI/
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr_CI/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr_FR/
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr_FR/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hi_IN/
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hi_IN/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu_HU/
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu_HU/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ne/
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ne/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv_SE/
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv_SE/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk_UA/
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk_UA/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130749 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/cache/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/dumpers/featured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/entity_resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/jsonschemas/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/os-v1/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/os-v2/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/v7/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/systemfields/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/records/systemfields/pidslug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/resources/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/resources/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/communities/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/services/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/services/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/services/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/services/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/communities/services/uow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/fixtures/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/fixtures/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v1/communitymembers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v1/communitymembers/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v2/communitymembers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v2/communitymembers/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/v7/communitymembers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/v7/communitymembers/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/members/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/services/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/services/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/services/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/services/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24616 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/members/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/notifications/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/records/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/records/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/records/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/records/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/records/records/systemfields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/records/records/systemfields/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/records/records/systemfields/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/records/records/systemfields/communities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/records/records/systemfields/communities/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/records/records/systemfields/communities/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/searchapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_details.html
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/administration/community_search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/about/
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/access-status-label.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/macros/communities_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/request.html
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13508 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10929 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/views/communities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/views/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/views/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/invenio_communities/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35303 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/invenio_communities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/run-js-linter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/cache/test_identity_redis_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/communities/test_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/communities/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/communities/test_community_ui_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/communities/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/communities/test_relations_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/communities/test_relations_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29959 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/communities/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/communities/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/communities/tests_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/members/
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/members/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/members/test_members_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/members/test_members_no_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/members/test_members_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34235 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/members/test_members_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/records/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/mock_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/mock_module/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/records/mock_module/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/mock_module/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/records/mock_module/jsonschemas/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/mock_module/jsonschemas/mocks/mock-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/records/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/records/mock_module/mappings/v6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/mock_module/mappings/v6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/records/mock_module/mappings/v6/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/mock_module/mappings/v6/mocks/mock-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/records/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:03:26.000000 invenio-communities-7.0.1/tests/records/mock_module/mappings/v7/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/mock_module/mappings/v7/mocks/mock-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/mock_module/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/records/test_mockrecords_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-05 16:03:19.000000 invenio-communities-7.0.1/tests/test_notifications.py
```

### Comparing `invenio-communities-7.0.0/.editorconfig` & `invenio-communities-7.0.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/.tx/config` & `invenio-communities-7.0.1/.tx/config`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2016-2021 CERN.
-# Copyright (C)      2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 #
 # 1) Create message catalog:
 #    $ python setup.py extract_messages
@@ -20,17 +20,17 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio-communities-messages]
+[o:inveniosoftware:p:invenio:r:invenio-communities-messages]
 file_filter = invenio_communities/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_communities/translations/messages.pot
 source_lang = en
 type = PO
 
 # Translate JavaScript strings
 # 1) Navigate to the invenio_communities/assets/semantic-ui/translations/invenio_communities/ folder
@@ -55,12 +55,12 @@
 # 9) Pull translations for all languages from Transifex
 #    $ tx pull -a
 # 10) Compile .po files for all languages
 #    $ npm run compile_catalog
 # 11) Convert .po file for a single language
 #    $ npm run compile_catalog lang <lang>
 
-[invenio.invenio-communities-messages-ui]
+[o:inveniosoftware:p:invenio:r:invenio-communities-messages-ui]
 file_filter = invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/<lang>/messages.po
 source_file = invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-communities-7.0.0/AUTHORS.rst` & `invenio-communities-7.0.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/CHANGES.rst` & `invenio-communities-7.0.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 
 Changes
 =======
+Version 7.0.1 (released 2023-07-05)
+
+- tests: fix users update
 
 Version 7.0.0 (released 2023-06-15)
 -----------------------------------
 
 - cache: adds unmanaged groups to be cached and loaded in the identity
 - adds identity cache
 - add groups as community members
```

### Comparing `invenio-communities-7.0.0/CONTRIBUTING.rst` & `invenio-communities-7.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/LICENSE` & `invenio-communities-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/MANIFEST.in` & `invenio-communities-7.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/PKG-INFO` & `invenio-communities-7.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-communities
-Version: 7.0.0
+Version: 7.0.1
 Summary: InvenioRDM module for the communities feature.
 Home-page: https://github.com/inveniosoftware/invenio-communities
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -44,14 +44,17 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         
         Changes
         =======
+        Version 7.0.1 (released 2023-07-05)
+        
+        - tests: fix users update
         
         Version 7.0.0 (released 2023-06-15)
         -----------------------------------
         
         - cache: adds unmanaged groups to be cached and loaded in the identity
         - adds identity cache
         - add groups as community members
```

### Comparing `invenio-communities-7.0.0/README.rst` & `invenio-communities-7.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/docs/Makefile` & `invenio-communities-7.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/docs/conf.py` & `invenio-communities-7.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/docs/index.rst` & `invenio-communities-7.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/docs/make.bat` & `invenio-communities-7.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/administration/communities.py` & `invenio-communities-7.0.1/invenio_communities/administration/communities.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/alembic/02cd82910727_update_role_id_type_upgrade.py` & `invenio-communities-7.0.1/invenio_communities/alembic/02cd82910727_update_role_id_type_upgrade.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/alembic/37b21951084c_update_role_id_type_downgrade.py` & `invenio-communities-7.0.1/invenio_communities/alembic/37b21951084c_update_role_id_type_downgrade.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py` & `invenio-communities-7.0.1/invenio_communities/alembic/5b478fe7ef7f_create_featured_communities_table.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/alembic/90642d415317_create_communities_branch.py` & `invenio-communities-7.0.1/invenio_communities/alembic/90642d415317_create_communities_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py` & `invenio-communities-7.0.1/invenio_communities/alembic/a3f5a8635cbb_remove_version_table.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py` & `invenio-communities-7.0.1/invenio_communities/alembic/de9c14cbb0b2_create_communities_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py` & `invenio-communities-7.0.1/invenio_communities/alembic/f701a32e6fbe_create_communities_members_table.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/alembic/fbe746957cfc_create_member_tables.py` & `invenio-communities-7.0.1/invenio_communities/alembic/fbe746957cfc_create_member_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/FeatureModal.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/details.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/featured.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/administration/search.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityApi.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/CommunityLinksExtractor.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/InvitationsContextProvider.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/invitations/api.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/MembersContextProvider.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/members/api.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/api/serializers.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CarouselItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CommunitiesCarousel.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/CommunitiesCarousel.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesCarousel/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemComputer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityCompactItemMobile.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemComputer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/communitiesItems/CommunityItemMobile.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunities.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/FeaturedCommunity.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/featuredCommunities/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/frontpage.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/labels/RestrictedLabel.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/new.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/search.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesEmptySearchResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/CommunitiesSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/community/searchComponents/ResultsGridItemTemplate.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/Filters.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ActionDropdown.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorMessage.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/ErrorPopup.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabel.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/FilterLabels.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/MembersSearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/RemoveMemberModal.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/SuccessIcon.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/RadioSelection.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActions.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsBulkActionsManager.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SearchResultsRowCheckbox.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/bulk_actions/SelectedMembers.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/dropdowns.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/components/modal_manager/ModalContextProvider.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsResultsContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/InvitationsSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/GroupTabPane.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/InvitationsMembersModal.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MemberSearchBar.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/invitationsModal/MembersWithRoleSelection.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/invitations/request_actions/InvitationActionButtons.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersEmptyResults.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResult.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersResultsGridItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/components/MembersSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMemberBulkActions.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/ManagerMembersResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/MembersSearchAppContext.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/manager_view/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/member_view/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/PublicMembersSearchLayout.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/members/members/public_view/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/requests/requests.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/components/CommunitySettingsForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/curationPolicy/CurationPolicyForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/pages/CommunityPagesForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/privileges/CommunityPriviledgesForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CommunityProfileForm.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/CustomFieldSerializer.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DangerZone.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteButton.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/DeleteCommunityModal.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/LogoUploader.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/RenameCommunitySlugButton.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/js/invenio_communities/settings/profile/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/i18next.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: Afrikaans (https://app.transifex.com/inveniosoftware/teams/23537/af/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: af\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/af/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
 # Bessem Aamira <bessemamira@gmail.com>, 2022
-# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022
+# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
-"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023\n"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/ar/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
@@ -143,33 +143,33 @@
 msgid "Uploaded on"
 msgstr "تم التحميل على"
 
 msgid "Search guide"
 msgstr "دليل البحث"
 
 msgid "We couldn't find any matches for "
-msgstr "لا يمكن إيجاد أي تطابق مع"
+msgstr "لا يمكن إيجاد أي تطابق مع "
 
 msgid "your search"
 msgstr "بحثك"
 
 msgid "Start over"
 msgstr "يبدأ من "
 
 msgid "ProTip"
 msgstr "نصيحة محترف"
 
 msgid "will give you all the publications from 2017 until today"
-msgstr "سوف نقدم لك جميع المنشورات إبتداءا من سنة 2017 "
+msgstr "سوف نقدم لك جميع المنشورات إبتداء من سنة 2017 "
 
 msgid "For more tips, check out our "
-msgstr "لمزيد من النصائح، قم بالاطلاع على"
+msgstr "لمزيد من النصائح، قم بالاطلاع على "
 
 msgid " for defining advanced search queries"
-msgstr "للإنشاء أستعلاما متقدما"
+msgstr " لإنشاء مقاربات بحث متقدّمة"
 
 msgid "ORCID profile"
 msgstr "الملف الشخصي أوركيد ORCID"
 
 msgid "ROR profile"
 msgstr "الملف الشخصي لسجل  ROR"
 
@@ -245,21 +245,21 @@
 msgid "result(s) found"
 msgstr "النتيجة"
 
 msgid "Member since"
 msgstr "عضو منذ"
 
 msgid "Visibility"
-msgstr "رؤية"
+msgstr "مرئيّة"
 
 msgid "Search members..."
 msgstr "البحث في الأعضاء..."
 
 msgid "Public"
-msgstr "عام"
+msgstr "مشاع"
 
 msgid "Hidden"
 msgstr "مخفي"
 
 msgid "Change roles"
 msgstr "تغيير الأدوار"
 
@@ -337,15 +337,15 @@
 msgid "Search in invitations..."
 msgstr "البحث في الدعوات..."
 
 msgid "This community has no public members."
 msgstr "هذا المجتمع لا يضم أعضاء عامة."
 
 msgid "No matching members found."
-msgstr "لا يوجد اي غضو يوافق البحث."
+msgstr "لا يوجد اي عضو يوافق البحث."
 
 msgid "Actions"
 msgstr "العمليات"
 
 msgid "Add groups"
 msgstr "أضف مجموعات"
 
@@ -376,35 +376,37 @@
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 msgstr[4] ""
 msgstr[5] ""
 
 msgid "Search..."
-msgstr ""
+msgstr "البحث ..."
 
 msgid ""
 "Users must set profile visibility to \"Public\" in order to be invited to a "
 "community."
 msgstr ""
+"يجب على المستخدمين تهيئة مرئية الملف الشخصي على \"مشاع\" لتتم دعوتهم إلى "
+"المجتمع."
 
 msgid "Your community membership is visible to everyone."
-msgstr ""
+msgstr "عضويتك للمجتمع مرئية من الجميع"
 
 msgid ""
 "Your community membership is only visible to other members of the community."
-msgstr ""
+msgstr "عضويتك للمجتمع مرئية لأعصاء المجموعة فقط."
 
 msgid "Opened {{difference}} by"
 msgstr "مفتوح {{difference}} من طرف"
 
 msgid "Expires at:"
-msgstr ""
+msgstr "تنتهي في:"
 
 msgid "File must be smaller than "
-msgstr ""
+msgstr "الملف يجب ان يكون أصغر من"
 
 msgid "It may take a few moments for changes to be visible everywhere"
-msgstr ""
+msgstr "مرئية التغييرات في كل مكان ستتطلب بعض الوقت"
 
 msgid "New unique identifier of the community"
-msgstr ""
+msgstr "معرّف وحيد جديد للمجتمع"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ar/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/bg/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2022\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Zacharias Zacharodimos <zacharias.zacharodimos@cern.ch>, 2022\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/de/)\n"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/de/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Mart Jantson, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/teams/23537/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/teams/23537/et/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: Estonian (Estonia) (https://app.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: et_EE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/teams/23537/fa/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/fr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: Galician (https://app.transifex.com/inveniosoftware/teams/23537/gl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
 # Andrea Dömötör, 2022
+# Dorottya Szemigán, 2023
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Last-Translator: Dorottya Szemigán, 2023\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
@@ -146,21 +147,21 @@
 msgid "Search guide"
 msgstr "Keresési segédlet"
 
 msgid "We couldn't find any matches for "
 msgstr "Nincs találat erre:"
 
 msgid "your search"
-msgstr "az ön keresése"
+msgstr "az Ön keresése"
 
 msgid "Start over"
 msgstr "Újrakezdés"
 
 msgid "ProTip"
-msgstr "ProTipp"
+msgstr "ProTip"
 
 msgid "will give you all the publications from 2017 until today"
 msgstr "megadjuk az összes publikációt 2017-től máig"
 
 msgid "For more tips, check out our "
 msgstr "További tippekért keresse fel: "
 
@@ -222,16 +223,16 @@
 msgstr "Keresés email, teljes név vagy felhasználónév alapján"
 
 msgid "Invite"
 msgstr "Meghívás"
 
 msgid "You are about to invite <1>{{selectedCount}}</1> users"
 msgid_plural "You are about to invite <1>{{selectedCount}}</1> users"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "Ön <1>{{selectedCount}}</1> felhasználót készül meghívni"
+msgstr[1] "Ön <1>{{selectedCount}}</1> felhasználót készül meghívni"
 
 msgid "Name"
 msgstr "Név"
 
 msgid "Status"
 msgstr "Állapot"
 
@@ -263,16 +264,16 @@
 msgstr "Láthatósági beállítások módosítása"
 
 msgid "Remove from community"
 msgstr "Eltávolítás a közösségből"
 
 msgid "You have selected <1>{{selectedCount}}</1> users"
 msgid_plural "You have selected <1>{{selectedCount}}</1> users"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "Ön <1>{{selectedCount}}</1> felhasználót választott ki"
+msgstr[1] "Ön <1>{{selectedCount}}</1> felhasználót választott ki"
 
 msgid "You"
 msgstr "Ön"
 
 msgid "Leave..."
 msgstr "Kilépés..."
 
@@ -303,15 +304,15 @@
 msgid "Search records in community..."
 msgstr "Rekordok keresése a közösségben..."
 
 msgid ""
 "This is your community's unique identifier. You will be able to access your "
 "community through the URL:"
 msgstr ""
-"Ez az ön közösségének egyéni azonosítója. A közösséget ezen a linken érheti "
+"Ez az Ön közösségének egyéni azonosítója. A közösséget ezen a linken érheti "
 "el:"
 
 msgid "bulk actions"
 msgstr "több művelet"
 
 msgid "remove {{name}}"
 msgstr "{{name}} eltávolítása"
@@ -362,33 +363,33 @@
 msgstr "Arra készül, hogy elhagyja ezt a közösséget."
 
 msgid "You are about to remove this user from this community."
 msgstr "Arra készül, hogy eltávolítsa ezt a felhasználót a közösségből."
 
 msgid "You are about to add <1>{{selectedCount}}</1> groups."
 msgid_plural "You are about to add <1>{{selectedCount}}</1> groups."
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "Ön <1>{{selectedCount}}</1> csoportot készül hozzáadni"
+msgstr[1] "Ön <1>{{selectedCount}}</1> csoportot készül hozzáadni"
 
 msgid "Search..."
 msgstr "Keresés..."
 
 msgid ""
 "Users must set profile visibility to \"Public\" in order to be invited to a "
 "community."
 msgstr ""
 "Ahhoz, hogy meghívhassák egy közösségbe, a profil láthatóságát "
 "\"Nyilvános\"-ra kell állítania."
 
 msgid "Your community membership is visible to everyone."
-msgstr "Az ön közösségi tagsága mindenki számára látható."
+msgstr "Az Ön közösségi tagsága mindenki számára látható."
 
 msgid ""
 "Your community membership is only visible to other members of the community."
-msgstr "Az ön közösségi tagsága csak a közösség tagjai számára látható."
+msgstr "Az Ön közösségi tagsága csak a közösség tagjai számára látható."
 
 msgid "Opened {{difference}} by"
 msgstr "{{difference}} megnyitva általa:"
 
 msgid "Expires at:"
 msgstr "Lejár ekkor:"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/index.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # 
 # Translators:
 # Zacharias Zacharodimos <zacharias.zacharodimos@cern.ch>, 2022
 # Jiří Kunčar <jiri.kuncar@gmail.com>, 2022
 # Alizee Pace <alizee.pace@gmail.com>, 2022
 # Tibor Simko <tibor.simko@cern.ch>, 2022
+# Fare Fare <fare@polito.it>, 2023
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Last-Translator: Fare Fare <fare@polito.it>, 2023\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
@@ -107,15 +108,15 @@
 msgid "Setup your new community"
 msgstr ""
 
 msgid "Identifier"
 msgstr "Identificatore"
 
 msgid "Community visibility"
-msgstr ""
+msgstr "Visibilità della community"
 
 msgid "Create community"
 msgstr ""
 
 msgid "Message"
 msgstr "Messaggio"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/teams/23537/ja/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: no\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/teams/23537/pt/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/teams/23537/ro/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: Kinyarwanda (https://app.transifex.com/inveniosoftware/teams/23537/rw/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: rw\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
 # Sam Arbid, 2022
+# Rim Sharif, 2023
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Last-Translator: Rim Sharif, 2023\n"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/teams/23537/sv/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
@@ -31,27 +32,27 @@
 msgid "Cancel"
 msgstr "Avbryt"
 
 msgid "Maximum number of characters is 2000"
 msgstr "Maximalt antal tecken är 2000"
 
 msgid "Must be a valid URL"
-msgstr "Måste vara en giltig webbadress"
+msgstr "Måste vara en giltig URL"
 
 msgid "Profile picture"
 msgstr "Profilbild"
 
 msgid "Upload new picture"
 msgstr "Ladda upp ny bild"
 
 msgid "Delete picture"
 msgstr "Ta bort bild"
 
 msgid "Are you sure you want to delete this picture?"
-msgstr "Är du säker på att du vill ta bort den här bilden?"
+msgstr "Är du säker på att du vill radera den här bilden?"
 
 msgid "Danger zone"
 msgstr "Farozon"
 
 msgid "Change identifier"
 msgstr "Ändra identifierare"
 
@@ -86,15 +87,15 @@
 msgid "Organizations"
 msgstr "Organisationer"
 
 msgid "Save"
 msgstr "Spara"
 
 msgid "Change"
-msgstr "Förändra"
+msgstr "Ändra"
 
 msgid "Saved"
 msgstr "Sparad"
 
 msgid "Member"
 msgstr "Medlem"
 
@@ -119,15 +120,15 @@
 msgid "Message"
 msgstr "Meddelande"
 
 msgid "View"
 msgstr "Vy"
 
 msgid "{{total}} result(s) found"
-msgstr "{{total}} result(at) hittades"
+msgstr "{{total}} resultat hittades"
 
 msgid "Sort by"
 msgstr "Sortera efter"
 
 msgid "results per page"
 msgstr "resultat per sida"
 
@@ -218,15 +219,15 @@
 msgid "Invite members"
 msgstr "Bjud in medlemmar"
 
 msgid "Search by email, full name or username"
 msgstr "Sök med e-post, fullständigt namn eller användarnamn"
 
 msgid "Invite"
-msgstr "Inbjudan"
+msgstr "Bjud in"
 
 msgid "You are about to invite <1>{{selectedCount}}</1> users"
 msgid_plural "You are about to invite <1>{{selectedCount}}</1> users"
 msgstr[0] "Du är på väg att bjuda in <1>{{selectedCount}}</1> användare"
 msgstr[1] "Du är på väg att bjuda in <1>{{selectedCount}}</1> användare"
 
 msgid "Name"
@@ -235,15 +236,15 @@
 msgid "Status"
 msgstr "Status"
 
 msgid "Expires"
 msgstr "Upphör att gälla"
 
 msgid "result(s) found"
-msgstr "result(at) hittades"
+msgstr "resultat hittades"
 
 msgid "Member since"
 msgstr "Medlem sedan"
 
 msgid "Visibility"
 msgstr "Synlighet"
 
@@ -304,15 +305,15 @@
 msgstr "Sök poster i community..."
 
 msgid ""
 "This is your community's unique identifier. You will be able to access your "
 "community through the URL:"
 msgstr ""
 "Detta är din communitys unika identifierare. Du kommer att kunna komma åt "
-"din community via URL:en:"
+"din community via URL:"
 
 msgid "bulk actions"
 msgstr "massåtgärder"
 
 msgid "remove {{name}}"
 msgstr "ta bort {{name}}"
 
@@ -334,24 +335,24 @@
 msgid "This community has no public members."
 msgstr "Denna community har inga offentliga medlemmar."
 
 msgid "No matching members found."
 msgstr "Inga matchande medlemmar hittades."
 
 msgid "Actions"
-msgstr "Aktioner"
+msgstr "Åtgärder"
 
 msgid "Add groups"
 msgstr "Lägg till grupper"
 
 msgid "Restricted"
 msgstr "Begränsad"
 
 msgid "Search records..."
-msgstr "Sök rekord..."
+msgstr "Sök poster..."
 
 msgid "Selected groups"
 msgstr "Utvalda grupper"
 
 msgid "Selected members"
 msgstr "Utvalda medlemmar"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk_UA/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2022
-# 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/inveniosoftware/teams/23537/uk_UA/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: uk\n"
+"Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
 msgstr ""
 
 msgid "Search for organizations..."
@@ -125,15 +121,15 @@
 msgid "Sort by"
 msgstr ""
 
 msgid "results per page"
 msgstr ""
 
 msgid "Search"
-msgstr "Пошук"
+msgstr ""
 
 msgid "Search communities..."
 msgstr ""
 
 msgid "New community"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Kalven Richie, 2022\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 
 msgid ""
 msgstr ""
 "Project-Id-Version: i18next-conv\n"
 "POT-Creation-Date: 2022-10-12T07:39:56.031Z\n"
 "PO-Revision-Date: 2022-03-10 09:30+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_TW\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "mime-version: 1.0\n"
 
 msgid "Description"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/package-lock.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/package.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot` & `invenio-communities-7.0.1/invenio_communities/assets/semantic-ui/translations/invenio_communities/translations.pot`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/cache/cache.py` & `invenio-communities-7.0.1/invenio_communities/cache/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,7 +43,11 @@
     @abstractmethod
     def delete(self, key):
         """Delete the specific key."""
 
     @abstractmethod
     def flush(self):
         """Flush the cache."""
+
+    @abstractmethod
+    def append(self):
+        """Flush the cache."""
```

### Comparing `invenio-communities-7.0.0/invenio_communities/cache/redis.py` & `invenio-communities-7.0.1/invenio_communities/cache/redis.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/cli.py` & `invenio-communities-7.0.1/invenio_communities/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/__init__.py` & `invenio-communities-7.0.1/invenio_communities/communities/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/dumpers/featured.py` & `invenio-communities-7.0.1/invenio_communities/communities/dumpers/featured.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/entity_resolvers.py` & `invenio-communities-7.0.1/invenio_communities/communities/entity_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/records/api.py` & `invenio-communities-7.0.1/invenio_communities/communities/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json` & `invenio-communities-7.0.1/invenio_communities/communities/records/jsonschemas/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json` & `invenio-communities-7.0.1/invenio_communities/communities/records/jsonschemas/communities/definitions-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json` & `invenio-communities-7.0.1/invenio_communities/communities/records/mappings/os-v1/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json` & `invenio-communities-7.0.1/invenio_communities/communities/records/mappings/os-v2/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json` & `invenio-communities-7.0.1/invenio_communities/communities/records/mappings/v7/communities/communities-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/records/models.py` & `invenio-communities-7.0.1/invenio_communities/communities/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/access.py` & `invenio-communities-7.0.1/invenio_communities/communities/records/systemfields/access.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/records/systemfields/pidslug.py` & `invenio-communities-7.0.1/invenio_communities/communities/records/systemfields/pidslug.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/resources/config.py` & `invenio-communities-7.0.1/invenio_communities/communities/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/resources/resource.py` & `invenio-communities-7.0.1/invenio_communities/communities/resources/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/resources/serializer.py` & `invenio-communities-7.0.1/invenio_communities/communities/resources/serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/resources/ui_schema.py` & `invenio-communities-7.0.1/invenio_communities/communities/resources/ui_schema.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/schema.py` & `invenio-communities-7.0.1/invenio_communities/communities/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/services/__init__.py` & `invenio-communities-7.0.1/invenio_communities/communities/services/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/services/components.py` & `invenio-communities-7.0.1/invenio_communities/communities/services/components.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/services/config.py` & `invenio-communities-7.0.1/invenio_communities/communities/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/services/facets.py` & `invenio-communities-7.0.1/invenio_communities/communities/services/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/services/links.py` & `invenio-communities-7.0.1/invenio_communities/communities/services/links.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/services/results.py` & `invenio-communities-7.0.1/invenio_communities/communities/services/results.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/services/service.py` & `invenio-communities-7.0.1/invenio_communities/communities/services/service.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/services/sort.py` & `invenio-communities-7.0.1/invenio_communities/communities/services/sort.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/communities/services/uow.py` & `invenio-communities-7.0.1/invenio_communities/communities/services/uow.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/config.py` & `invenio-communities-7.0.1/invenio_communities/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/errors.py` & `invenio-communities-7.0.1/invenio_communities/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/ext.py` & `invenio-communities-7.0.1/invenio_communities/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/fixtures/demo.py` & `invenio-communities-7.0.1/invenio_communities/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/fixtures/tasks.py` & `invenio-communities-7.0.1/invenio_communities/fixtures/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/generators.py` & `invenio-communities-7.0.1/invenio_communities/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/__init__.py` & `invenio-communities-7.0.1/invenio_communities/members/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/errors.py` & `invenio-communities-7.0.1/invenio_communities/members/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/records/api.py` & `invenio-communities-7.0.1/invenio_communities/members/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json` & `invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v1/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json` & `invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v1/communitymembers/members/member-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json` & `invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v2/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json` & `invenio-communities-7.0.1/invenio_communities/members/records/mappings/os-v2/communitymembers/members/member-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json` & `invenio-communities-7.0.1/invenio_communities/members/records/mappings/v7/communitymembers/archivedinvitations/archivedinvitation-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json` & `invenio-communities-7.0.1/invenio_communities/members/records/mappings/v7/communitymembers/members/member-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/records/models.py` & `invenio-communities-7.0.1/invenio_communities/members/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/resources/config.py` & `invenio-communities-7.0.1/invenio_communities/members/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/resources/resource.py` & `invenio-communities-7.0.1/invenio_communities/members/resources/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/services/components.py` & `invenio-communities-7.0.1/invenio_communities/members/services/components.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/services/config.py` & `invenio-communities-7.0.1/invenio_communities/members/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/services/facets.py` & `invenio-communities-7.0.1/invenio_communities/members/services/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/services/fields.py` & `invenio-communities-7.0.1/invenio_communities/members/services/fields.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/services/request.py` & `invenio-communities-7.0.1/invenio_communities/members/services/request.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/services/schemas.py` & `invenio-communities-7.0.1/invenio_communities/members/services/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/members/services/service.py` & `invenio-communities-7.0.1/invenio_communities/members/services/service.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/notifications/generators.py` & `invenio-communities-7.0.1/invenio_communities/notifications/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/permissions.py` & `invenio-communities-7.0.1/invenio_communities/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/proxies.py` & `invenio-communities-7.0.1/invenio_communities/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/records/records/models.py` & `invenio-communities-7.0.1/invenio_communities/records/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/context.py` & `invenio-communities-7.0.1/invenio_communities/records/records/systemfields/communities/context.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/field.py` & `invenio-communities-7.0.1/invenio_communities/records/records/systemfields/communities/field.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/records/records/systemfields/communities/manager.py` & `invenio-communities-7.0.1/invenio_communities/records/records/systemfields/communities/manager.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/roles.py` & `invenio-communities-7.0.1/invenio_communities/roles.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/searchapp.py` & `invenio-communities-7.0.1/invenio_communities/searchapp.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/tasks.py` & `invenio-communities-7.0.1/invenio_communities/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/about/index.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/curation_policy/index.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/header.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/macros/custom_fields.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/members/invitations.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/members/members.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/curation_policy.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/pages.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/privileges.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/details/settings/profile.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/communities_carousel.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/macros/communities_carousel.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/macros/featured_communities.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/new.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/new.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/request.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/request.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/search.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/search.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html` & `invenio-communities-7.0.1/invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/af/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-communities 3.1.0*

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 6174 653a 2032 3031 362d 3038 2d31 3820  ate: 2016-08-18 
 000000d0: 3132 3a32 392b 3030 3030 0a4c 6173 742d  12:29+0000.Last-
 000000e0: 5472 616e 736c 6174 6f72 3a20 4655 4c4c  Translator: FULL
 000000f0: 204e 414d 4520 3c45 4d41 494c 4041 4444   NAME <EMAIL@ADD
 00000100: 5245 5353 3e0a 4c61 6e67 7561 6765 3a20  RESS>.Language: 
 00000110: 6166 0a4c 616e 6775 6167 652d 5465 616d  af.Language-Team
 00000120: 3a20 4166 7269 6b61 616e 7320 2868 7474  : Afrikaans (htt
-00000130: 7073 3a2f 2f77 7777 2e74 7261 6e73 6966  ps://www.transif
+00000130: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
 00000140: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
 00000150: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
 00000160: 3337 2f61 662f 290a 506c 7572 616c 2d46  37/af/).Plural-F
 00000170: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
 00000180: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
 00000190: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
 000001a0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/af/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: German (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/de_AT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: af\n"
+"Language: de_AT\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_communities/config.py:52 invenio_communities/config.py:137
 #: invenio_communities/config.py:179
 #: invenio_communities/members/services/config.py:38
 #: invenio_communities/members/services/config.py:77
 #: invenio_communities/members/services/config.py:108
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ar/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 25% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023\n"
 "Language: ar\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/"
 "ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
@@ -19,17 +19,17 @@
 "\n"
 "    The community you are trying to access was removed from %(sitename)s. "
 "The\n"
 "    metadata of the community is kept for archival purposes.\n"
 "  "
 msgstr ""
 "\n"
-"    تمت إزالة المجوعة الذي تحاول الوصول إليه من %(sitename)s.  تم الابقاء "
+"    تمت إزالة المجموعة التي تحاول الوصول إليها من %(sitename)s.  تم الابقاء "
 "على\n"
-"    الميتاداتا (البيانات الوصفية) للمجموعة لأغراض الأرشفة والحفظ.\n"
+"    الميتاداتا للمجموعة لأغراض الأرشفة والحفظ.\n"
 "  "
 
 msgid " members"
 msgstr "الأعضاء"
 
 msgid " requests"
 msgstr "الطلبات"
@@ -46,15 +46,15 @@
 msgid "A featured community entry with {q} does not exist."
 msgstr "لا وجود لمجموعة مميزة بمدخل {q}."
 
 msgid "A new ID value is required for the renaming."
 msgstr "إضافة معرف جديد إجباري لإعادة التسمية."
 
 msgid "About this community"
-msgstr "حوا هذه المجموعة"
+msgstr "حول هذه المجموعة"
 
 msgid "Accepted"
 msgstr "تم القبول"
 
 msgid "Best match"
 msgstr "أفضل تطابق "
 
@@ -120,20 +120,27 @@
 
 msgid "Invitations"
 msgstr "الدعوات"
 
 msgid "Least recently updated"
 msgstr "الأقل تحيينا مؤخرًا"
 
+msgid "Logo size limit exceeded. Limit: {limit} bytes Given: {file_size} bytes"
+msgstr ""
+"تجاوز للحد الاقصى لحجم الترخيمة. Limit: {limit} bytes Given: {file_size}"
+
 msgid "Manager"
 msgstr "المشرف"
 
 msgid "Members"
 msgstr "الأعضاء"
 
+msgid "Missing fields 'role' and/or 'visible'."
+msgstr "الحقول 'دور' و / أو 'المرئية' مفقودة"
+
 msgid "Must be false"
 msgstr "يجب أن تكون خاطئة"
 
 msgid "My communities"
 msgstr "مجتمعي"
 
 msgid "Name"
@@ -174,15 +181,15 @@
 msgid "Profile"
 msgstr "الملف الشّخصي"
 
 msgid "Project"
 msgstr "مشروع"
 
 msgid "Public"
-msgstr "عام"
+msgstr "مشاع"
 
 msgid "Reader"
 msgstr "القارئ"
 
 msgid "Recently updated"
 msgstr "المحدثة مؤخرا"
 
@@ -215,14 +222,17 @@
 
 msgid "The ID should be modified through the renaming URL instead."
 msgstr "ينبغي تعديل المعرف من خلال إعادة تسمية العنوان URL ."
 
 msgid "The ID should contain only letters with numbers or dashes."
 msgstr "يجب أن يتكون المعرف ID فقط من حروف  اضافة لارقام أو شُرَط."
 
+msgid "The community is not public."
+msgstr "المجموعة ليست عامة."
+
 msgid "The community is restricted to users with access."
 msgstr "المجموعة حصريّة للأعضاء المخوّل لهم الولوج"
 
 msgid "Tombstone"
 msgstr "تمثال"
 
 msgid "Topic"
@@ -242,12 +252,18 @@
 
 msgid "You can only set public visibility on your own membership."
 msgstr "يمكنك فقط تبيان مرئية عامة على عضويتك."
 
 msgid "You cannot change your own role."
 msgstr "لا يمكنك تغيير دورك."
 
+msgid "You will join as \"{role}\" (changed from: \"{previous}\")."
+msgstr "ستلتحق بدور \"{role}\" (تغيير عوضا: \"{previous}\")"
+
+msgid "You will join as \"{role}\"."
+msgstr "ستلتحق مع دور \"{role}\""
+
 msgid "Your community is publicly accessible and shows up in search results."
 msgstr "مجموعتك متاح للجميع وتظهر في نتائج البحث."
 
 msgid "Your community is restricted to users with access."
 msgstr "مجموعتك غير متاحة للمستخدمينمن غيرالأعضاء."
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ar/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/ar/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-communities
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
-# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022
 # Bessem Aamira <bessemamira@gmail.com>, 2022
+# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023\n"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
@@ -106,14 +106,15 @@
 msgid "A featured community entry with {q} does not exist."
 msgstr "لا وجود لمجموعة مميزة بمدخل {q}."
 
 #: invenio_communities/errors.py:41
 msgid ""
 "Logo size limit exceeded. Limit: {limit} bytes Given: {file_size} bytes"
 msgstr ""
+"تجاوز للحد الاقصى لحجم الترخيمة. Limit: {limit} bytes Given: {file_size}"
 
 #: invenio_communities/communities/schema.py:40
 msgid "Field cannot be blank or longer than {max_} characters."
 msgstr "لا يمكن أن يكون الحقل فارغًا أوان يزيد طوله عن {max_} حرفًا."
 
 #: invenio_communities/communities/schema.py:52
 msgid "The ID must not be an Universally Unique IDentifier (UUID)."
@@ -133,15 +134,15 @@
 
 #: invenio_communities/communities/services/components.py:57
 msgid "A new ID value is required for the renaming."
 msgstr "إضافة معرف جديد إجباري لإعادة التسمية."
 
 #: invenio_communities/communities/services/components.py:116
 msgid "The community is not public."
-msgstr ""
+msgstr "المجموعة ليست عامة."
 
 #: invenio_communities/communities/services/config.py:57
 msgid "Featured"
 msgstr "بارز"
 
 #: invenio_communities/communities/services/facets.py:15
 msgid "Type"
@@ -169,15 +170,15 @@
 #: invenio_communities/members/services/facets.py:35
 msgid "Visibility"
 msgstr "رؤية"
 
 #: invenio_communities/communities/services/facets.py:28
 #: invenio_communities/members/services/facets.py:36
 msgid "Public"
-msgstr "عام"
+msgstr "مشاع"
 
 #: invenio_communities/communities/services/facets.py:29
 #: invenio_communities/communities/services/facets.py:49
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:31
 msgid "Restricted"
 msgstr "مقيدة"
 
@@ -229,15 +230,15 @@
 
 #: invenio_communities/members/services/request.py:74
 msgid "Community invitation"
 msgstr "دعوات المجموعة"
 
 #: invenio_communities/members/services/schemas.py:88
 msgid "Missing fields 'role' and/or 'visible'."
-msgstr ""
+msgstr "الحقول 'دور' و / أو 'المرئية' مفقودة"
 
 #: invenio_communities/members/services/schemas.py:116
 msgid "Untitled"
 msgstr "بدون عنوان"
 
 #: invenio_communities/members/services/service.py:180
 msgid "Must be false"
@@ -249,15 +250,15 @@
 
 #: invenio_communities/members/services/service.py:269
 msgid "Invitation to join \"{community}\""
 msgstr "دعوة للإلتحاق بـ \"{community}\""
 
 #: invenio_communities/members/services/service.py:289
 msgid "You will join as \"{role}\"."
-msgstr ""
+msgstr "ستلتحق مع دور \"{role}\""
 
 #: invenio_communities/members/services/service.py:465
 #: invenio_communities/members/services/service.py:585
 msgid "A community must have at least one owner."
 msgstr "يجب ان يكون لمجموعة على الأقل عضو مالك."
 
 #: invenio_communities/members/services/service.py:494
@@ -266,15 +267,15 @@
 
 #: invenio_communities/members/services/service.py:502
 msgid "You can only set public visibility on your own membership."
 msgstr "يمكنك فقط تبيان مرئية عامة على عضويتك."
 
 #: invenio_communities/members/services/service.py:510
 msgid "You will join as \"{role}\" (changed from: \"{previous}\")."
-msgstr ""
+msgstr "ستلتحق بدور \"{role}\" (تغيير عوضا: \"{previous}\")"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:12
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:24
 #: invenio_communities/templates/semantic-ui/invenio_communities/search.html:22
 msgid "Communities"
 msgstr "مجتمعات"
 
@@ -321,29 +322,29 @@
 msgid ""
 "\n"
 "    The community you are trying to access was removed from %(sitename)s. The\n"
 "    metadata of the community is kept for archival purposes.\n"
 "  "
 msgstr ""
 "\n"
-"    تمت إزالة المجوعة الذي تحاول الوصول إليه من %(sitename)s.  تم الابقاء على\n"
-"    الميتاداتا (البيانات الوصفية) للمجموعة لأغراض الأرشفة والحفظ.\n"
+"    تمت إزالة المجموعة التي تحاول الوصول إليها من %(sitename)s.  تم الابقاء على\n"
+"    الميتاداتا للمجموعة لأغراض الأرشفة والحفظ.\n"
 "  "
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:29
 msgid "Community visibility"
 msgstr "مرئية المجتمع"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:30
 msgid "The community is restricted to users with access."
 msgstr "المجموعة حصريّة للأعضاء المخوّل لهم الولوج"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:73
 msgid "About this community"
-msgstr "حوا هذه المجموعة"
+msgstr "حول هذه المجموعة"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:90
 msgid "New upload"
 msgstr "إيداع جديد"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html:12
 msgid " members"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/bg/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/bg/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: bg\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/bg/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/bg/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/bg/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ca/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: ca\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ca/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ca/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/ca/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/cs/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: cs\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/"
 "cs/)\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/cs/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/cs/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/da/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,18 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-communities 3.1.0\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 09:34+0200\n"
-"PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2022\n"
-"Language: da\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/"
-"da/)\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Status"
-msgstr "Status"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/da/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/ne/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # Translations template for invenio-communities.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-communities
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Jiří Kunčar <jiri.kuncar@gmail.com>, 2022
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2022\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: Nepali (https://app.transifex.com/inveniosoftware/teams/23537/ne/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: da\n"
+"Language: ne\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_communities/config.py:52 invenio_communities/config.py:137
 #: invenio_communities/config.py:179
 #: invenio_communities/members/services/config.py:38
 #: invenio_communities/members/services/config.py:77
 #: invenio_communities/members/services/config.py:108
@@ -187,15 +183,15 @@
 #: invenio_communities/members/services/facets.py:17
 msgid "Role"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:23
 #: invenio_communities/members/services/facets.py:41
 msgid "Status"
-msgstr "Status"
+msgstr ""
 
 #: invenio_communities/members/services/facets.py:25
 msgid "Submitted"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:26
 msgid "Expired"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/de/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/de/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,15 +3,15 @@
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Hermann Schranzhofer <hermann.schranzhofer@tugraz.at>, "
 "2022\n"
 "Language: de\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/"
 "de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/de/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/de/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Hermann Schranzhofer <hermann.schranzhofer@tugraz.at>, 2022\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/de/)\n"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/el/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/el/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: el\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/"
 "el/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/el/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/el/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/en/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/es/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/es/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
 "Language: es\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/es/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/es/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/et/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/et/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Mart Jantson, 2022\n"
 "Language: et\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/et/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/et/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/et/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Mart Jantson, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/teams/23537/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/teams/23537/et/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-communities 3.1.0*

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 000000d0: 3132 3a32 392b 3030 3030 0a4c 6173 742d  12:29+0000.Last-
 000000e0: 5472 616e 736c 6174 6f72 3a20 4655 4c4c  Translator: FULL
 000000f0: 204e 414d 4520 3c45 4d41 494c 4041 4444   NAME <EMAIL@ADD
 00000100: 5245 5353 3e0a 4c61 6e67 7561 6765 3a20  RESS>.Language: 
 00000110: 6574 5f45 450a 4c61 6e67 7561 6765 2d54  et_EE.Language-T
 00000120: 6561 6d3a 2045 7374 6f6e 6961 6e20 2845  eam: Estonian (E
 00000130: 7374 6f6e 6961 2920 2868 7474 7073 3a2f  stonia) (https:/
-00000140: 2f77 7777 2e74 7261 6e73 6966 6578 2e63  /www.transifex.c
+00000140: 2f61 7070 2e74 7261 6e73 6966 6578 2e63  /app.transifex.c
 00000150: 6f6d 2f69 6e76 656e 696f 736f 6674 7761  om/inveniosoftwa
 00000160: 7265 2f74 6561 6d73 2f32 3335 3337 2f65  re/teams/23537/e
 00000170: 745f 4545 2f29 0a50 6c75 7261 6c2d 466f  t_EE/).Plural-Fo
 00000180: 726d 733a 206e 706c 7572 616c 733d 323b  rms: nplurals=2;
 00000190: 2070 6c75 7261 6c3d 286e 2021 3d20 3129   plural=(n != 1)
 000001a0: 3b0a 4d49 4d45 2d56 6572 7369 6f6e 3a20  ;.MIME-Version: 
 000001b0: 312e 300a 436f 6e74 656e 742d 5479 7065  1.0.Content-Type
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: English (Hungary) (https://app.transifex.com/inveniosoftware/teams/23537/en_HU/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: et_EE\n"
+"Language: en_HU\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_communities/config.py:52 invenio_communities/config.py:137
 #: invenio_communities/config.py:179
 #: invenio_communities/members/services/config.py:38
 #: invenio_communities/members/services/config.py:77
 #: invenio_communities/members/services/config.py:108
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/fa/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: fa\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/fa/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/fa/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/da/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Translations template for invenio-communities.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-communities
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2022
+# Jiří Kunčar <jiri.kuncar@gmail.com>, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2022\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: fa\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Language: da\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_communities/config.py:52 invenio_communities/config.py:137
 #: invenio_communities/config.py:179
 #: invenio_communities/members/services/config.py:38
 #: invenio_communities/members/services/config.py:77
 #: invenio_communities/members/services/config.py:108
 msgid "Best match"
@@ -83,26 +83,26 @@
 #: invenio_communities/config.py:96
 msgid "Can manage members, curate records and view restricted records."
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:37
 #: invenio_communities/config.py:106
 msgid "Owner"
-msgstr "مالک"
+msgstr ""
 
 #: invenio_communities/config.py:107
 msgid "Full administrative access to the entire community."
 msgstr ""
 
 #: invenio_communities/config.py:141 invenio_communities/config.py:183
 #: invenio_communities/members/services/config.py:42
 #: invenio_communities/members/services/config.py:81
 #: invenio_communities/members/services/config.py:112
 msgid "Name"
-msgstr "نام"
+msgstr ""
 
 #: invenio_communities/errors.py:26
 msgid "A featured community entry with {q} does not exist."
 msgstr ""
 
 #: invenio_communities/errors.py:41
 msgid ""
@@ -187,15 +187,15 @@
 #: invenio_communities/members/services/facets.py:17
 msgid "Role"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:23
 #: invenio_communities/members/services/facets.py:41
 msgid "Status"
-msgstr "وضعیت"
+msgstr "Status"
 
 #: invenio_communities/members/services/facets.py:25
 msgid "Submitted"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:26
 msgid "Expired"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/fr/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
 "Language: fr\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/"
 "fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/fr/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/fr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/gl/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-communities 3.1.0*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 6174 653a 2032 3031 362d 3038 2d31 3820  ate: 2016-08-18 
 000000d0: 3132 3a32 392b 3030 3030 0a4c 6173 742d  12:29+0000.Last-
 000000e0: 5472 616e 736c 6174 6f72 3a20 4655 4c4c  Translator: FULL
 000000f0: 204e 414d 4520 3c45 4d41 494c 4041 4444   NAME <EMAIL@ADD
 00000100: 5245 5353 3e0a 4c61 6e67 7561 6765 3a20  RESS>.Language: 
 00000110: 676c 0a4c 616e 6775 6167 652d 5465 616d  gl.Language-Team
 00000120: 3a20 4761 6c69 6369 616e 2028 6874 7470  : Galician (http
-00000130: 733a 2f2f 7777 772e 7472 616e 7369 6665  s://www.transife
+00000130: 733a 2f2f 6170 702e 7472 616e 7369 6665  s://app.transife
 00000140: 782e 636f 6d2f 696e 7665 6e69 6f73 6f66  x.com/inveniosof
 00000150: 7477 6172 652f 7465 616d 732f 3233 3533  tware/teams/2353
 00000160: 372f 676c 2f29 0a50 6c75 7261 6c2d 466f  7/gl/).Plural-Fo
 00000170: 726d 733a 206e 706c 7572 616c 733d 323b  rms: nplurals=2;
 00000180: 2070 6c75 7261 6c3d 286e 2021 3d20 3129   plural=(n != 1)
 00000190: 3b0a 4d49 4d45 2d56 6572 7369 6f6e 3a20  ;.MIME-Version: 
 000001a0: 312e 300a 436f 6e74 656e 742d 5479 7065  1.0.Content-Type
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/gl/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: German (Germany) (https://app.transifex.com/inveniosoftware/teams/23537/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: gl\n"
+"Language: de_DE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_communities/config.py:52 invenio_communities/config.py:137
 #: invenio_communities/config.py:179
 #: invenio_communities/members/services/config.py:38
 #: invenio_communities/members/services/config.py:77
 #: invenio_communities/members/services/config.py:108
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/hr/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/hr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: hr\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hr/)\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/hr/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/hr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/hu/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
+"Last-Translator: Dorottya Szemigán, 2023\n"
 "Language: hu\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
@@ -263,12 +263,12 @@
 msgstr "Ön \"{role}\"-ként fog csatlakozni (cserélve erről: \"{previous}\")."
 
 msgid "You will join as \"{role}\"."
 msgstr "Ön \"{role}\"-ként fog csatlakozni."
 
 msgid "Your community is publicly accessible and shows up in search results."
 msgstr ""
-"Az ön közössége nyilvánosan elérhető, és megjelenik a keresési találatokban."
+"Az Ön közössége nyilvánosan elérhető, és megjelenik a keresési találatokban."
 
 msgid "Your community is restricted to users with access."
 msgstr ""
-"Az ön közössége csak a hozzáféréssel rendelkező tagok számára elérhető."
+"Az Ön közössége csak a hozzáféréssel rendelkező tagok számára elérhető."
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/hu/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/hu/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-communities
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Andrea Dömötör, 2022
+# Dorottya Szemigán, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Last-Translator: Dorottya Szemigán, 2023\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
@@ -376,20 +377,20 @@
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html:19
 msgid "Privileges"
 msgstr "Jogok"
 
 #: invenio_communities/views/communities.py:29
 msgid "Your community is publicly accessible and shows up in search results."
 msgstr ""
-"Az ön közössége nyilvánosan elérhető, és megjelenik a keresési találatokban."
+"Az Ön közössége nyilvánosan elérhető, és megjelenik a keresési találatokban."
 
 #: invenio_communities/views/communities.py:37
 msgid "Your community is restricted to users with access."
 msgstr ""
-"Az ön közössége csak a hozzáféréssel rendelkező tagok számára elérhető."
+"Az Ön közössége csak a hozzáféréssel rendelkező tagok számára elérhető."
 
 #: invenio_communities/views/ui.py:121
 msgid "Requests"
 msgstr "Kérések"
 
 #: invenio_communities/views/ui.py:135
 msgid "Settings"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/it/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/it/LC_MESSAGES/messages.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
+"Last-Translator: Fare Fare <fare@polito.it>, 2023\n"
 "Language: it\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/it/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
@@ -20,14 +20,17 @@
 
 msgid "Closed"
 msgstr "Chiuso"
 
 msgid "Communities"
 msgstr "Comunità"
 
+msgid "Community visibility"
+msgstr "Visibilità della community"
+
 msgid "Event"
 msgstr "Evento"
 
 msgid "Invitations"
 msgstr "Inviti"
 
 msgid "Members"
@@ -38,14 +41,17 @@
 
 msgid "Name"
 msgstr "Nome"
 
 msgid "New community"
 msgstr "Nuova comunità"
 
+msgid "New upload"
+msgstr "Nuovo caricamento"
+
 msgid "Open"
 msgstr "Apri"
 
 msgid "Owner"
 msgstr "Proprietario"
 
 msgid "Profile"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/it/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/sk/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # Translations template for invenio-communities.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-communities
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Zacharias Zacharodimos <zacharias.zacharodimos@cern.ch>, 2022
-# Jiří Kunčar <jiri.kuncar@gmail.com>, 2022
+# Ivan Masár <helix84@centrum.sk>, 2022
 # Tibor Simko <tibor.simko@cern.ch>, 2022
-# Alizee Pace <alizee.pace@gmail.com>, 2022
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: it\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: sk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 #: invenio_communities/config.py:52 invenio_communities/config.py:137
 #: invenio_communities/config.py:179
 #: invenio_communities/members/services/config.py:38
 #: invenio_communities/members/services/config.py:77
 #: invenio_communities/members/services/config.py:108
 msgid "Best match"
@@ -46,15 +44,15 @@
 #: invenio_communities/members/services/config.py:89
 #: invenio_communities/members/services/config.py:120
 msgid "Oldest"
 msgstr ""
 
 #: invenio_communities/config.py:64
 msgid "Version"
-msgstr "Versione"
+msgstr "Verzia"
 
 #: invenio_communities/config.py:68
 msgid "Recently updated"
 msgstr ""
 
 #: invenio_communities/config.py:72
 msgid "Least recently updated"
@@ -86,26 +84,26 @@
 #: invenio_communities/config.py:96
 msgid "Can manage members, curate records and view restricted records."
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:37
 #: invenio_communities/config.py:106
 msgid "Owner"
-msgstr "Proprietario"
+msgstr "Vlastník"
 
 #: invenio_communities/config.py:107
 msgid "Full administrative access to the entire community."
 msgstr ""
 
 #: invenio_communities/config.py:141 invenio_communities/config.py:183
 #: invenio_communities/members/services/config.py:42
 #: invenio_communities/members/services/config.py:81
 #: invenio_communities/members/services/config.py:112
 msgid "Name"
-msgstr "Nome"
+msgstr "Meno"
 
 #: invenio_communities/errors.py:26
 msgid "A featured community entry with {q} does not exist."
 msgstr ""
 
 #: invenio_communities/errors.py:41
 msgid ""
@@ -142,23 +140,23 @@
 
 #: invenio_communities/communities/services/config.py:57
 msgid "Featured"
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:15
 msgid "Type"
-msgstr "Tipo"
+msgstr ""
 
 #: invenio_communities/communities/services/facets.py:17
 msgid "Organization"
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:18
 msgid "Event"
-msgstr "Evento"
+msgstr ""
 
 #: invenio_communities/communities/services/facets.py:19
 msgid "Topic"
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:20
 msgid "Project"
@@ -170,35 +168,35 @@
 #: invenio_communities/members/services/facets.py:35
 msgid "Visibility"
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:28
 #: invenio_communities/members/services/facets.py:36
 msgid "Public"
-msgstr "Publico"
+msgstr "Verejný"
 
 #: invenio_communities/communities/services/facets.py:29
 #: invenio_communities/communities/services/facets.py:49
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:31
 msgid "Restricted"
-msgstr "Limitato"
+msgstr "Chránené"
 
 #: invenio_communities/communities/services/facets.py:48
 #: invenio_communities/members/services/facets.py:36
 msgid "Hidden"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:17
 msgid "Role"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:23
 #: invenio_communities/members/services/facets.py:41
 msgid "Status"
-msgstr "Stato"
+msgstr "Stav"
 
 #: invenio_communities/members/services/facets.py:25
 msgid "Submitted"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:26
 msgid "Expired"
@@ -210,23 +208,23 @@
 
 #: invenio_communities/members/services/facets.py:28
 msgid "Declined"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:29
 msgid "Cancelled"
-msgstr "Annullato"
+msgstr "Zrušené"
 
 #: invenio_communities/members/services/facets.py:42
 msgid "Open"
-msgstr "Apri"
+msgstr "Otvorená"
 
 #: invenio_communities/members/services/facets.py:42
 msgid "Closed"
-msgstr "Chiuso"
+msgstr "Zatvorená"
 
 #: invenio_communities/members/services/fields.py:20
 msgid "Invalid role."
 msgstr ""
 
 #: invenio_communities/members/services/request.py:74
 msgid "Community invitation"
@@ -273,15 +271,15 @@
 msgid "You will join as \"{role}\" (changed from: \"{previous}\")."
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:12
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:24
 #: invenio_communities/templates/semantic-ui/invenio_communities/search.html:22
 msgid "Communities"
-msgstr "Comunità"
+msgstr "Komunity"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:30
 msgid ""
 "Organize, curate and collaborate on records for your institution, project, "
 "topic or event."
 msgstr ""
 
@@ -289,19 +287,19 @@
 #: invenio_communities/templates/semantic-ui/invenio_communities/search.html:12
 msgid "Search communities"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:46
 #: invenio_communities/templates/semantic-ui/invenio_communities/new.html:12
 msgid "New community"
-msgstr "Nuova comunità"
+msgstr "Nová komunita"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:56
 msgid "My communities"
-msgstr "Le mie comunità"
+msgstr "Moje komunity"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:58
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:68
 msgid "See all"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:66
@@ -344,31 +342,31 @@
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html:12
 msgid " members"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html:19
 #: invenio_communities/views/ui.py:128
 msgid "Members"
-msgstr "Membri"
+msgstr "Členovia"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html:20
 msgid "Invitations"
-msgstr "Inviti"
+msgstr "Pozvánky"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html:12
 msgid " requests"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html:11
 msgid " settings"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html:18
 msgid "Profile"
-msgstr "Profilo"
+msgstr "Profil"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html:19
 msgid "Privileges"
 msgstr ""
 
 #: invenio_communities/views/communities.py:29
 msgid "Your community is publicly accessible and shows up in search results."
@@ -376,12 +374,12 @@
 
 #: invenio_communities/views/communities.py:37
 msgid "Your community is restricted to users with access."
 msgstr ""
 
 #: invenio_communities/views/ui.py:121
 msgid "Requests"
-msgstr "Richieste"
+msgstr "Požiadavky"
 
 #: invenio_communities/views/ui.py:135
 msgid "Settings"
-msgstr "Impostazioni"
+msgstr "Nastavenia"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ja/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/ja/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: ja\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ja/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ja/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # Translations template for invenio-communities.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-communities
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2022
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Spanish (Cuba) (https://app.transifex.com/inveniosoftware/teams/23537/es_CU/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ja\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: es_CU\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: invenio_communities/config.py:52 invenio_communities/config.py:137
 #: invenio_communities/config.py:179
 #: invenio_communities/members/services/config.py:38
 #: invenio_communities/members/services/config.py:77
 #: invenio_communities/members/services/config.py:108
 msgid "Best match"
@@ -83,26 +79,26 @@
 #: invenio_communities/config.py:96
 msgid "Can manage members, curate records and view restricted records."
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:37
 #: invenio_communities/config.py:106
 msgid "Owner"
-msgstr "所有者"
+msgstr ""
 
 #: invenio_communities/config.py:107
 msgid "Full administrative access to the entire community."
 msgstr ""
 
 #: invenio_communities/config.py:141 invenio_communities/config.py:183
 #: invenio_communities/members/services/config.py:42
 #: invenio_communities/members/services/config.py:81
 #: invenio_communities/members/services/config.py:112
 msgid "Name"
-msgstr "名前"
+msgstr ""
 
 #: invenio_communities/errors.py:26
 msgid "A featured community entry with {q} does not exist."
 msgstr ""
 
 #: invenio_communities/errors.py:41
 msgid ""
@@ -187,15 +183,15 @@
 #: invenio_communities/members/services/facets.py:17
 msgid "Role"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:23
 #: invenio_communities/members/services/facets.py:41
 msgid "Status"
-msgstr "状態"
+msgstr ""
 
 #: invenio_communities/members/services/facets.py:25
 msgid "Submitted"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:26
 msgid "Expired"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ka/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/ka/LC_MESSAGES/messages.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: ka\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ka/)\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ka/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/ka/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/lt/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/lt/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: lt\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/lt/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/lt/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/lt/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/messages.pot` & `invenio-communities-7.0.1/invenio_communities/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/no/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,27 +1,24 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language: no\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/no/)\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: zh_TW\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/"
+"teams/23537/zh_TW/)\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-msgid "Cancelled"
-msgstr "Kansellert"
-
 msgid "Name"
-msgstr "Navn"
+msgstr "名稱"
 
 msgid "Owner"
-msgstr "Eier"
+msgstr "擁有者"
 
 msgid "Status"
-msgstr "Status"
+msgstr "狀態"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/no/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/no/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: no\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/pl/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: pl\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/"
 "pl/)\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/pl/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/pl/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/pt/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: pt\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/"
 "teams/23537/pt/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/pt/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/pt/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/teams/23537/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pt\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ro/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/ro/LC_MESSAGES/messages.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: ro\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ro/)\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
 "2:1));\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ro/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/ro/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/teams/23537/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ru/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: ru\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ru/)\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/ru/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/ru/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/rw/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-communities 3.1.0*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 6174 653a 2032 3031 362d 3038 2d31 3820  ate: 2016-08-18 
 000000d0: 3132 3a32 392b 3030 3030 0a4c 6173 742d  12:29+0000.Last-
 000000e0: 5472 616e 736c 6174 6f72 3a20 4655 4c4c  Translator: FULL
 000000f0: 204e 414d 4520 3c45 4d41 494c 4041 4444   NAME <EMAIL@ADD
 00000100: 5245 5353 3e0a 4c61 6e67 7561 6765 3a20  RESS>.Language: 
 00000110: 7277 0a4c 616e 6775 6167 652d 5465 616d  rw.Language-Team
 00000120: 3a20 4b69 6e79 6172 7761 6e64 6120 2868  : Kinyarwanda (h
-00000130: 7474 7073 3a2f 2f77 7777 2e74 7261 6e73  ttps://www.trans
+00000130: 7474 7073 3a2f 2f61 7070 2e74 7261 6e73  ttps://app.trans
 00000140: 6966 6578 2e63 6f6d 2f69 6e76 656e 696f  ifex.com/invenio
 00000150: 736f 6674 7761 7265 2f74 6561 6d73 2f32  software/teams/2
 00000160: 3335 3337 2f72 772f 290a 506c 7572 616c  3537/rw/).Plural
 00000170: 2d46 6f72 6d73 3a20 6e70 6c75 7261 6c73  -Forms: nplurals
 00000180: 3d32 3b20 706c 7572 616c 3d28 6e20 213d  =2; plural=(n !=
 00000190: 2031 293b 0a4d 494d 452d 5665 7273 696f   1);.MIME-Versio
 000001a0: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/rw/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: English (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/en_AT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: rw\n"
+"Language: en_AT\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_communities/config.py:52 invenio_communities/config.py:137
 #: invenio_communities/config.py:179
 #: invenio_communities/members/services/config.py:38
 #: invenio_communities/members/services/config.py:77
 #: invenio_communities/members/services/config.py:108
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/sk/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: sk\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/"
 "sk/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/sk/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/it/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # Translations template for invenio-communities.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-communities
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Ivan Masár <helix84@centrum.sk>, 2022
+# Zacharias Zacharodimos <zacharias.zacharodimos@cern.ch>, 2022
+# Jiří Kunčar <jiri.kuncar@gmail.com>, 2022
 # Tibor Simko <tibor.simko@cern.ch>, 2022
+# Alizee Pace <alizee.pace@gmail.com>, 2022
+# Fare Fare <fare@polito.it>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Last-Translator: Fare Fare <fare@polito.it>, 2023\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: sk\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Language: it\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: invenio_communities/config.py:52 invenio_communities/config.py:137
 #: invenio_communities/config.py:179
 #: invenio_communities/members/services/config.py:38
 #: invenio_communities/members/services/config.py:77
 #: invenio_communities/members/services/config.py:108
 msgid "Best match"
@@ -44,15 +47,15 @@
 #: invenio_communities/members/services/config.py:89
 #: invenio_communities/members/services/config.py:120
 msgid "Oldest"
 msgstr ""
 
 #: invenio_communities/config.py:64
 msgid "Version"
-msgstr "Verzia"
+msgstr "Versione"
 
 #: invenio_communities/config.py:68
 msgid "Recently updated"
 msgstr ""
 
 #: invenio_communities/config.py:72
 msgid "Least recently updated"
@@ -84,26 +87,26 @@
 #: invenio_communities/config.py:96
 msgid "Can manage members, curate records and view restricted records."
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:37
 #: invenio_communities/config.py:106
 msgid "Owner"
-msgstr "Vlastník"
+msgstr "Proprietario"
 
 #: invenio_communities/config.py:107
 msgid "Full administrative access to the entire community."
 msgstr ""
 
 #: invenio_communities/config.py:141 invenio_communities/config.py:183
 #: invenio_communities/members/services/config.py:42
 #: invenio_communities/members/services/config.py:81
 #: invenio_communities/members/services/config.py:112
 msgid "Name"
-msgstr "Meno"
+msgstr "Nome"
 
 #: invenio_communities/errors.py:26
 msgid "A featured community entry with {q} does not exist."
 msgstr ""
 
 #: invenio_communities/errors.py:41
 msgid ""
@@ -140,23 +143,23 @@
 
 #: invenio_communities/communities/services/config.py:57
 msgid "Featured"
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:15
 msgid "Type"
-msgstr ""
+msgstr "Tipo"
 
 #: invenio_communities/communities/services/facets.py:17
 msgid "Organization"
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:18
 msgid "Event"
-msgstr ""
+msgstr "Evento"
 
 #: invenio_communities/communities/services/facets.py:19
 msgid "Topic"
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:20
 msgid "Project"
@@ -168,35 +171,35 @@
 #: invenio_communities/members/services/facets.py:35
 msgid "Visibility"
 msgstr ""
 
 #: invenio_communities/communities/services/facets.py:28
 #: invenio_communities/members/services/facets.py:36
 msgid "Public"
-msgstr "Verejný"
+msgstr "Publico"
 
 #: invenio_communities/communities/services/facets.py:29
 #: invenio_communities/communities/services/facets.py:49
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:31
 msgid "Restricted"
-msgstr "Chránené"
+msgstr "Limitato"
 
 #: invenio_communities/communities/services/facets.py:48
 #: invenio_communities/members/services/facets.py:36
 msgid "Hidden"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:17
 msgid "Role"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:23
 #: invenio_communities/members/services/facets.py:41
 msgid "Status"
-msgstr "Stav"
+msgstr "Stato"
 
 #: invenio_communities/members/services/facets.py:25
 msgid "Submitted"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:26
 msgid "Expired"
@@ -208,23 +211,23 @@
 
 #: invenio_communities/members/services/facets.py:28
 msgid "Declined"
 msgstr ""
 
 #: invenio_communities/members/services/facets.py:29
 msgid "Cancelled"
-msgstr "Zrušené"
+msgstr "Annullato"
 
 #: invenio_communities/members/services/facets.py:42
 msgid "Open"
-msgstr "Otvorená"
+msgstr "Apri"
 
 #: invenio_communities/members/services/facets.py:42
 msgid "Closed"
-msgstr "Zatvorená"
+msgstr "Chiuso"
 
 #: invenio_communities/members/services/fields.py:20
 msgid "Invalid role."
 msgstr ""
 
 #: invenio_communities/members/services/request.py:74
 msgid "Community invitation"
@@ -271,15 +274,15 @@
 msgid "You will join as \"{role}\" (changed from: \"{previous}\")."
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:12
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:24
 #: invenio_communities/templates/semantic-ui/invenio_communities/search.html:22
 msgid "Communities"
-msgstr "Komunity"
+msgstr "Comunità"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:30
 msgid ""
 "Organize, curate and collaborate on records for your institution, project, "
 "topic or event."
 msgstr ""
 
@@ -287,19 +290,19 @@
 #: invenio_communities/templates/semantic-ui/invenio_communities/search.html:12
 msgid "Search communities"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:46
 #: invenio_communities/templates/semantic-ui/invenio_communities/new.html:12
 msgid "New community"
-msgstr "Nová komunita"
+msgstr "Nuova comunità"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:56
 msgid "My communities"
-msgstr "Moje komunity"
+msgstr "Le mie comunità"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:58
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:68
 msgid "See all"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:66
@@ -321,52 +324,52 @@
 "    The community you are trying to access was removed from %(sitename)s. The\n"
 "    metadata of the community is kept for archival purposes.\n"
 "  "
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:29
 msgid "Community visibility"
-msgstr ""
+msgstr "Visibilità della community"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:30
 msgid "The community is restricted to users with access."
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:73
 msgid "About this community"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:90
 msgid "New upload"
-msgstr ""
+msgstr "Nuovo caricamento"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html:12
 msgid " members"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html:19
 #: invenio_communities/views/ui.py:128
 msgid "Members"
-msgstr "Členovia"
+msgstr "Membri"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html:20
 msgid "Invitations"
-msgstr "Pozvánky"
+msgstr "Inviti"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html:12
 msgid " requests"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html:11
 msgid " settings"
 msgstr ""
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html:18
 msgid "Profile"
-msgstr "Profil"
+msgstr "Profilo"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html:19
 msgid "Privileges"
 msgstr ""
 
 #: invenio_communities/views/communities.py:29
 msgid "Your community is publicly accessible and shows up in search results."
@@ -374,12 +377,12 @@
 
 #: invenio_communities/views/communities.py:37
 msgid "Your community is restricted to users with access."
 msgstr ""
 
 #: invenio_communities/views/ui.py:121
 msgid "Requests"
-msgstr "Požiadavky"
+msgstr "Richieste"
 
 #: invenio_communities/views/ui.py:135
 msgid "Settings"
-msgstr "Nastavenia"
+msgstr "Impostazioni"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/sv/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
+"Last-Translator: Rim Sharif, 2023\n"
 "Language: sv\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
@@ -18,23 +18,24 @@
 "\n"
 "    The community you are trying to access was removed from %(sitename)s. "
 "The\n"
 "    metadata of the community is kept for archival purposes.\n"
 "  "
 msgstr ""
 "\n"
-"    Gemenskapen du försöker komma åt togs bort från %(sitename)s. Den \n"
-"    metadata från gemenskapen bevaras för arkivändamål.\n"
+"    Den community som du försöker komma åt togs bort från %(sitename)s. "
+"Metadatan\n"
+"    från denna community bevaras för arkivändamål.\n"
 "  "
 
 msgid " members"
 msgstr " medlemmar"
 
 msgid " requests"
-msgstr "Begäran"
+msgstr "förfrågningar"
 
 msgid " settings"
 msgstr "inställningar"
 
 msgid "A community must have at least one owner."
 msgstr "En grupp måste ha minst en ägare."
 
@@ -53,21 +54,21 @@
 msgid "Accepted"
 msgstr "Accepterad"
 
 msgid "Best match"
 msgstr "Bästa matchningen"
 
 msgid "Can curate records and view restricted records."
-msgstr "Kan kurera rekord och se begränsade rekord."
+msgstr "Kan kurera poster och se begränsade poster."
 
 msgid "Can manage members, curate records and view restricted records."
-msgstr "Kan hantera medlemmar, kurera poster och visa begränsade rekord."
+msgstr "Kan hantera medlemmar, kurera poster och visa begränsade poster."
 
 msgid "Can view restricted records."
-msgstr "Kan se begränsade rekord."
+msgstr "Kan se begränsade poster."
 
 msgid "Cancelled"
 msgstr "Avbruten"
 
 msgid "Closed"
 msgstr "Stängd"
 
@@ -151,15 +152,15 @@
 msgid "New community"
 msgstr "Ny community"
 
 msgid "New upload"
 msgstr "Ny uppladdning"
 
 msgid "Newest"
-msgstr "Nyaste"
+msgstr "Nyast"
 
 msgid "Oldest"
 msgstr "Äldst"
 
 msgid "Open"
 msgstr "Öppen"
 
@@ -203,33 +204,33 @@
 msgid "Role"
 msgstr "Roll"
 
 msgid "Search communities"
 msgstr "Sök efter communities"
 
 msgid "See all"
-msgstr "Se allt"
+msgstr "Se alla"
 
 msgid "Settings"
-msgstr "inställningar"
+msgstr "Inställningar"
 
 msgid "Status"
 msgstr "Status"
 
 msgid "Submitted"
-msgstr "Skickade in"
+msgstr "Inskickad"
 
 msgid "The ID must not be an Universally Unique IDentifier (UUID)."
 msgstr "ID:t får inte vara en Universally Unique IDentifier (UUID)."
 
 msgid "The ID should be modified through the renaming URL instead."
-msgstr "ID:t bör ändras genom att byta namn på URL istället."
+msgstr "ID bör ändras genom att byta namn på URL istället."
 
 msgid "The ID should contain only letters with numbers or dashes."
-msgstr "ID:t ska endast innehålla bokstäver med siffror eller bindestreck."
+msgstr "ID ska endast innehålla bokstäver med siffror eller bindestreck."
 
 msgid "The community is not public."
 msgstr "community är inte offentligt."
 
 msgid "The community is restricted to users with access."
 msgstr "community är begränsad till användare med åtkomst."
 
@@ -239,15 +240,15 @@
 msgid "Topic"
 msgstr "Ämne"
 
 msgid "Type"
 msgstr "Typ"
 
 msgid "Untitled"
-msgstr "Namnlös"
+msgstr "Ingen titel"
 
 msgid "Version"
 msgstr "Version"
 
 msgid "Visibility"
 msgstr "Synlighet"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/sv/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/sv/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 # This file is distributed under the same license as the invenio-communities
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
 # Sam Arbid, 2022
+# Rim Sharif, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Last-Translator: Rim Sharif, 2023\n"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/teams/23537/sv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
@@ -33,15 +34,15 @@
 msgstr "Bästa matchningen"
 
 #: invenio_communities/config.py:56 invenio_communities/config.py:145
 #: invenio_communities/config.py:187
 #: invenio_communities/members/services/config.py:85
 #: invenio_communities/members/services/config.py:116
 msgid "Newest"
-msgstr "Nyaste"
+msgstr "Nyast"
 
 #: invenio_communities/config.py:60 invenio_communities/config.py:149
 #: invenio_communities/config.py:191
 #: invenio_communities/members/services/config.py:89
 #: invenio_communities/members/services/config.py:120
 msgid "Oldest"
 msgstr "Äldst"
@@ -61,33 +62,33 @@
 #: invenio_communities/communities/services/facets.py:38
 #: invenio_communities/config.py:82
 msgid "Reader"
 msgstr "Läsare"
 
 #: invenio_communities/config.py:83
 msgid "Can view restricted records."
-msgstr "Kan se begränsade rekord."
+msgstr "Kan se begränsade poster."
 
 #: invenio_communities/communities/services/facets.py:40
 #: invenio_communities/config.py:88
 msgid "Curator"
 msgstr "Kurator"
 
 #: invenio_communities/config.py:89
 msgid "Can curate records and view restricted records."
-msgstr "Kan kurera rekord och se begränsade rekord."
+msgstr "Kan kurera poster och se begränsade poster."
 
 #: invenio_communities/communities/services/facets.py:39
 #: invenio_communities/config.py:95
 msgid "Manager"
 msgstr "Manager"
 
 #: invenio_communities/config.py:96
 msgid "Can manage members, curate records and view restricted records."
-msgstr "Kan hantera medlemmar, kurera poster och visa begränsade rekord."
+msgstr "Kan hantera medlemmar, kurera poster och visa begränsade poster."
 
 #: invenio_communities/communities/services/facets.py:37
 #: invenio_communities/config.py:106
 msgid "Owner"
 msgstr "Ägare"
 
 #: invenio_communities/config.py:107
@@ -118,23 +119,23 @@
 
 #: invenio_communities/communities/schema.py:52
 msgid "The ID must not be an Universally Unique IDentifier (UUID)."
 msgstr "ID:t får inte vara en Universally Unique IDentifier (UUID)."
 
 #: invenio_communities/communities/schema.py:122
 msgid "The ID should contain only letters with numbers or dashes."
-msgstr "ID:t ska endast innehålla bokstäver med siffror eller bindestreck."
+msgstr "ID ska endast innehålla bokstäver med siffror eller bindestreck."
 
 #: invenio_communities/communities/services/components.py:31
 msgid "A community with this identifier already exists."
 msgstr "En community med denna identifierare finns redan."
 
 #: invenio_communities/communities/services/components.py:49
 msgid "The ID should be modified through the renaming URL instead."
-msgstr "ID:t bör ändras genom att byta namn på URL istället."
+msgstr "ID bör ändras genom att byta namn på URL istället."
 
 #: invenio_communities/communities/services/components.py:57
 msgid "A new ID value is required for the renaming."
 msgstr "Ett nytt ID-värde krävs för att byta namn."
 
 #: invenio_communities/communities/services/components.py:116
 msgid "The community is not public."
@@ -194,15 +195,15 @@
 #: invenio_communities/members/services/facets.py:23
 #: invenio_communities/members/services/facets.py:41
 msgid "Status"
 msgstr "Status"
 
 #: invenio_communities/members/services/facets.py:25
 msgid "Submitted"
-msgstr "Skickade in"
+msgstr "Inskickad"
 
 #: invenio_communities/members/services/facets.py:26
 msgid "Expired"
 msgstr "Utgånget"
 
 #: invenio_communities/members/services/facets.py:27
 msgid "Accepted"
@@ -234,15 +235,15 @@
 
 #: invenio_communities/members/services/schemas.py:88
 msgid "Missing fields 'role' and/or 'visible'."
 msgstr "Saknade fält \"roll\" och/eller \"synlig\"."
 
 #: invenio_communities/members/services/schemas.py:116
 msgid "Untitled"
-msgstr "Namnlös"
+msgstr "Ingen titel"
 
 #: invenio_communities/members/services/service.py:180
 msgid "Must be false"
 msgstr "Måste vara falskt"
 
 #: invenio_communities/members/services/service.py:202
 msgid "Invalid member type: email"
@@ -300,15 +301,15 @@
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:56
 msgid "My communities"
 msgstr "Mina communities"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:58
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:68
 msgid "See all"
-msgstr "Se allt"
+msgstr "Se alla"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/frontpage.html:66
 msgid "New communities"
 msgstr "Nya communities"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/tombstone.html:12
 msgid "Tombstone"
@@ -323,16 +324,16 @@
 msgid ""
 "\n"
 "    The community you are trying to access was removed from %(sitename)s. The\n"
 "    metadata of the community is kept for archival purposes.\n"
 "  "
 msgstr ""
 "\n"
-"    Gemenskapen du försöker komma åt togs bort från %(sitename)s. Den \n"
-"    metadata från gemenskapen bevaras för arkivändamål.\n"
+"    Den community som du försöker komma åt togs bort från %(sitename)s. Metadatan\n"
+"    från denna community bevaras för arkivändamål.\n"
 "  "
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:29
 msgid "Community visibility"
 msgstr "Community synlighet"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/header.html:30
@@ -358,15 +359,15 @@
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/members/base.html:20
 msgid "Invitations"
 msgstr "Inbjudningar"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/requests/index.html:12
 msgid " requests"
-msgstr "Begäran"
+msgstr "förfrågningar"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html:11
 msgid " settings"
 msgstr "inställningar"
 
 #: invenio_communities/templates/semantic-ui/invenio_communities/details/settings/base.html:18
 msgid "Profile"
@@ -386,8 +387,8 @@
 
 #: invenio_communities/views/ui.py:121
 msgid "Requests"
 msgstr "Förfrågningar"
 
 #: invenio_communities/views/ui.py:135
 msgid "Settings"
-msgstr "inställningar"
+msgstr "Inställningar"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/tr/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,15 +3,15 @@
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume."
 "com>, 2022\n"
 "Language: tr\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/tr/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/tr/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/tr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/uk/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-communities 3.1.0*

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 b902 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 c902 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d63 6f6d 6d75 6e69   invenio-communi
 00000050: 7469 6573 2033 2e31 2e30 0a52 6570 6f72  ties 3.1.0.Repor
 00000060: 742d 4d73 6769 642d 4275 6773 2d54 6f3a  t-Msgid-Bugs-To:
 00000070: 2069 6e66 6f40 696e 7665 6e69 6f73 6f66   info@inveniosof
 00000080: 7477 6172 652e 6f72 670a 504f 542d 4372  tware.org.POT-Cr
 00000090: 6561 7469 6f6e 2d44 6174 653a 2032 3032  eation-Date: 202
 000000a0: 322d 3130 2d31 3220 3039 3a33 342b 3032  2-10-12 09:34+02
 000000b0: 3030 0a50 4f2d 5265 7669 7369 6f6e 2d44  00.PO-Revision-D
 000000c0: 6174 653a 2032 3031 362d 3038 2d31 3820  ate: 2016-08-18 
 000000d0: 3132 3a32 392b 3030 3030 0a4c 6173 742d  12:29+0000.Last-
 000000e0: 5472 616e 736c 6174 6f72 3a20 4655 4c4c  Translator: FULL
 000000f0: 204e 414d 4520 3c45 4d41 494c 4041 4444   NAME <EMAIL@ADD
 00000100: 5245 5353 3e0a 4c61 6e67 7561 6765 3a20  RESS>.Language: 
-00000110: 756b 0a4c 616e 6775 6167 652d 5465 616d  uk.Language-Team
-00000120: 3a20 556b 7261 696e 6961 6e20 2868 7474  : Ukrainian (htt
-00000130: 7073 3a2f 2f77 7777 2e74 7261 6e73 6966  ps://www.transif
-00000140: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
-00000150: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
-00000160: 3337 2f75 6b2f 290a 506c 7572 616c 2d46  37/uk/).Plural-F
-00000170: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d34  orms: nplurals=4
-00000180: 3b20 706c 7572 616c 3d28 6e20 2520 3120  ; plural=(n % 1 
-00000190: 3d3d 2030 2026 2620 6e20 2520 3130 203d  == 0 && n % 10 =
-000001a0: 3d20 3120 2626 206e 2025 2031 3030 2021  = 1 && n % 100 !
-000001b0: 3d20 3131 203f 2030 203a 206e 2025 2031  = 11 ? 0 : n % 1
-000001c0: 203d 3d20 3020 2626 206e 2025 2031 3020   == 0 && n % 10 
-000001d0: 3e3d 2032 2026 2620 6e20 2520 3130 203c  >= 2 && n % 10 <
-000001e0: 3d20 3420 2626 2028 6e20 2520 3130 3020  = 4 && (n % 100 
-000001f0: 3c20 3132 207c 7c20 6e20 2520 3130 3020  < 12 || n % 100 
-00000200: 3e20 3134 2920 3f20 3120 3a20 6e20 2520  > 14) ? 1 : n % 
-00000210: 3120 3d3d 2030 2026 2620 286e 2025 2031  1 == 0 && (n % 1
-00000220: 3020 3d3d 3020 7c7c 2028 6e20 2520 3130  0 ==0 || (n % 10
-00000230: 203e 3d35 2026 2620 6e20 2520 3130 203c   >=5 && n % 10 <
-00000240: 3d39 2920 7c7c 2028 6e20 2520 3130 3020  =9) || (n % 100 
-00000250: 3e3d 3131 2026 2620 6e20 2520 3130 3020  >=11 && n % 100 
-00000260: 3c3d 3134 2029 2920 3f20 323a 2033 293b  <=14 )) ? 2: 3);
-00000270: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
-00000280: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
-00000290: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
-000002a0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
-000002b0: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
-000002c0: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
-000002d0: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
-000002e0: 2e31 322e 310a 00                        .12.1..
+00000110: 756b 5f55 410a 4c61 6e67 7561 6765 2d54  uk_UA.Language-T
+00000120: 6561 6d3a 2055 6b72 6169 6e69 616e 2028  eam: Ukrainian (
+00000130: 556b 7261 696e 6529 2028 6874 7470 733a  Ukraine) (https:
+00000140: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
+00000150: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
+00000160: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
+00000170: 756b 5f55 412f 290a 506c 7572 616c 2d46  uk_UA/).Plural-F
+00000180: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d34  orms: nplurals=4
+00000190: 3b20 706c 7572 616c 3d28 6e20 2520 3120  ; plural=(n % 1 
+000001a0: 3d3d 2030 2026 2620 6e20 2520 3130 203d  == 0 && n % 10 =
+000001b0: 3d20 3120 2626 206e 2025 2031 3030 2021  = 1 && n % 100 !
+000001c0: 3d20 3131 203f 2030 203a 206e 2025 2031  = 11 ? 0 : n % 1
+000001d0: 203d 3d20 3020 2626 206e 2025 2031 3020   == 0 && n % 10 
+000001e0: 3e3d 2032 2026 2620 6e20 2520 3130 203c  >= 2 && n % 10 <
+000001f0: 3d20 3420 2626 2028 6e20 2520 3130 3020  = 4 && (n % 100 
+00000200: 3c20 3132 207c 7c20 6e20 2520 3130 3020  < 12 || n % 100 
+00000210: 3e20 3134 2920 3f20 3120 3a20 6e20 2520  > 14) ? 1 : n % 
+00000220: 3120 3d3d 2030 2026 2620 286e 2025 2031  1 == 0 && (n % 1
+00000230: 3020 3d3d 3020 7c7c 2028 6e20 2520 3130  0 ==0 || (n % 10
+00000240: 203e 3d35 2026 2620 6e20 2520 3130 203c   >=5 && n % 10 <
+00000250: 3d39 2920 7c7c 2028 6e20 2520 3130 3020  =9) || (n % 100 
+00000260: 3e3d 3131 2026 2620 6e20 2520 3130 3020  >=11 && n % 100 
+00000270: 3c3d 3134 2029 2920 3f20 323a 2033 293b  <=14 )) ? 2: 3);
+00000280: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
+00000290: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
+000002a0: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
+000002b0: 7273 6574 3d75 7466 2d38 0a43 6f6e 7465  rset=utf-8.Conte
+000002c0: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
+000002d0: 6469 6e67 3a20 3862 6974 0a47 656e 6572  ding: 8bit.Gener
+000002e0: 6174 6564 2d42 793a 2042 6162 656c 2032  ated-By: Babel 2
+000002f0: 2e31 322e 310a 00                        .12.1..
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/uk/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/inveniosoftware/teams/23537/uk_UA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: uk\n"
+"Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: invenio_communities/config.py:52 invenio_communities/config.py:137
 #: invenio_communities/config.py:179
 #: invenio_communities/members/services/config.py:38
 #: invenio_communities/members/services/config.py:77
 #: invenio_communities/members/services/config.py:108
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Weizheng Lu, 2022\n"
 "Language: zh_CN\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/"
 "teams/23537/zh_CN/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Weizheng Lu, 2022\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-communities-7.0.1/invenio_communities/translations/no/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,24 +1,27 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language: zh_TW\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/"
-"teams/23537/zh_TW/)\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: no\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/"
+"teams/23537/no/)\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
+msgid "Cancelled"
+msgstr "Kansellert"
+
 msgid "Name"
-msgstr "名稱"
+msgstr "Navn"
 
 msgid "Owner"
-msgstr "擁有者"
+msgstr "Eier"
 
 msgid "Status"
-msgstr "狀態"
+msgstr "Status"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-communities-7.0.1/invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-communities 3.1.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:34+0200\n"
 "PO-Revision-Date: 2016-08-18 12:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: zh_TW\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-communities-7.0.0/invenio_communities/utils.py` & `invenio-communities-7.0.1/invenio_communities/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,40 +4,25 @@
 # Copyright (C) 2016-2022 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Utilities."""
 
-from flask import current_app, session
+from flask import session
 from flask_principal import Identity
 from invenio_accounts.models import Role
 from invenio_accounts.proxies import current_db_change_history
 
 from .generators import CommunityRoleNeed
 from .proxies import current_communities, current_identities_cache
 
 IDENTITY_KEY = "user-communities:"
 
 
-def add_to_community_cache(community_id, identity_id):
-    """Updates the community cache."""
-    community_cache = current_identities_cache.get(community_id)
-    if community_cache and identity_id not in community_cache:
-        community_cache.append(identity_id)
-    else:
-        community_cache = [identity_id]
-    # This cache is set to the same duration as the identity caches, because it should not expire before
-    # This cache has a risk of being eternal therefore a cronjob that clears all the cache has to be set on a daily basis
-    current_identities_cache.set(
-        community_id,
-        community_cache,
-    )
-
-
 def load_community_needs(identity):
     """Add community-related needs to the freshly loaded identity.
 
     Note that this function is intended to be called as handler for the
     identity-loaded signal, where we don't have control over the handler
     execution order.
     Thus, the given identity may not be fully initialized and still missing
```

### Comparing `invenio-communities-7.0.0/invenio_communities/views/__init__.py` & `invenio-communities-7.0.1/invenio_communities/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/views/api.py` & `invenio-communities-7.0.1/invenio_communities/views/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/views/communities.py` & `invenio-communities-7.0.1/invenio_communities/views/communities.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/views/decorators.py` & `invenio-communities-7.0.1/invenio_communities/views/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/views/ui.py` & `invenio-communities-7.0.1/invenio_communities/views/ui.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities/webpack.py` & `invenio-communities-7.0.1/invenio_communities/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/invenio_communities.egg-info/PKG-INFO` & `invenio-communities-7.0.1/invenio_communities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-communities
-Version: 7.0.0
+Version: 7.0.1
 Summary: InvenioRDM module for the communities feature.
 Home-page: https://github.com/inveniosoftware/invenio-communities
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -44,14 +44,17 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         
         Changes
         =======
+        Version 7.0.1 (released 2023-07-05)
+        
+        - tests: fix users update
         
         Version 7.0.0 (released 2023-06-15)
         -----------------------------------
         
         - cache: adds unmanaged groups to be cached and loaded in the identity
         - adds identity cache
         - add groups as community members
```

### Comparing `invenio-communities-7.0.0/invenio_communities.egg-info/SOURCES.txt` & `invenio-communities-7.0.1/invenio_communities.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -183,42 +183,54 @@
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ca/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/cs/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/da/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de/translations.json
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de_AT/messages.po
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/de_DE/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/el/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en/translations.json
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en_AT/messages.po
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/en_HU/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es/translations.json
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es_CU/messages.po
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/es_MX/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/et_EE/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa/translations.json
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fa_IR/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr/translations.json
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr_CI/messages.po
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/fr_FR/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/gl/translations.json
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hi_IN/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hr/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu/translations.json
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/hu_HU/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/it/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ja/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ka/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/lt/translations.json
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ne/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/no/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pl/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/pt/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ro/messages.po
@@ -227,18 +239,20 @@
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/ru/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/rw/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sk/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv/translations.json
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/sv_SE/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/tr/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk/translations.json
+invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/uk_UA/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_CN/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/messages.po
 invenio_communities/assets/semantic-ui/translations/invenio_communities/messages/zh_TW/translations.json
 invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/compileCatalog.js
 invenio_communities/assets/semantic-ui/translations/invenio_communities/scripts/initCatalog.js
 invenio_communities/cache/__init__.py
@@ -353,42 +367,66 @@
 invenio_communities/translations/ca/LC_MESSAGES/messages.po
 invenio_communities/translations/cs/LC_MESSAGES/messages.mo
 invenio_communities/translations/cs/LC_MESSAGES/messages.po
 invenio_communities/translations/da/LC_MESSAGES/messages.mo
 invenio_communities/translations/da/LC_MESSAGES/messages.po
 invenio_communities/translations/de/LC_MESSAGES/messages.mo
 invenio_communities/translations/de/LC_MESSAGES/messages.po
+invenio_communities/translations/de_AT/LC_MESSAGES/messages.mo
+invenio_communities/translations/de_AT/LC_MESSAGES/messages.po
+invenio_communities/translations/de_DE/LC_MESSAGES/messages.mo
+invenio_communities/translations/de_DE/LC_MESSAGES/messages.po
 invenio_communities/translations/el/LC_MESSAGES/messages.mo
 invenio_communities/translations/el/LC_MESSAGES/messages.po
 invenio_communities/translations/en/LC_MESSAGES/messages.mo
 invenio_communities/translations/en/LC_MESSAGES/messages.po
+invenio_communities/translations/en_AT/LC_MESSAGES/messages.mo
+invenio_communities/translations/en_AT/LC_MESSAGES/messages.po
+invenio_communities/translations/en_HU/LC_MESSAGES/messages.mo
+invenio_communities/translations/en_HU/LC_MESSAGES/messages.po
 invenio_communities/translations/es/LC_MESSAGES/messages.mo
 invenio_communities/translations/es/LC_MESSAGES/messages.po
+invenio_communities/translations/es_CU/LC_MESSAGES/messages.mo
+invenio_communities/translations/es_CU/LC_MESSAGES/messages.po
+invenio_communities/translations/es_MX/LC_MESSAGES/messages.mo
+invenio_communities/translations/es_MX/LC_MESSAGES/messages.po
 invenio_communities/translations/et/LC_MESSAGES/messages.mo
 invenio_communities/translations/et/LC_MESSAGES/messages.po
 invenio_communities/translations/et_EE/LC_MESSAGES/messages.mo
 invenio_communities/translations/et_EE/LC_MESSAGES/messages.po
 invenio_communities/translations/fa/LC_MESSAGES/messages.mo
 invenio_communities/translations/fa/LC_MESSAGES/messages.po
+invenio_communities/translations/fa_IR/LC_MESSAGES/messages.mo
+invenio_communities/translations/fa_IR/LC_MESSAGES/messages.po
 invenio_communities/translations/fr/LC_MESSAGES/messages.mo
 invenio_communities/translations/fr/LC_MESSAGES/messages.po
+invenio_communities/translations/fr_CI/LC_MESSAGES/messages.mo
+invenio_communities/translations/fr_CI/LC_MESSAGES/messages.po
+invenio_communities/translations/fr_FR/LC_MESSAGES/messages.mo
+invenio_communities/translations/fr_FR/LC_MESSAGES/messages.po
 invenio_communities/translations/gl/LC_MESSAGES/messages.mo
 invenio_communities/translations/gl/LC_MESSAGES/messages.po
+invenio_communities/translations/hi_IN/LC_MESSAGES/messages.mo
+invenio_communities/translations/hi_IN/LC_MESSAGES/messages.po
 invenio_communities/translations/hr/LC_MESSAGES/messages.mo
 invenio_communities/translations/hr/LC_MESSAGES/messages.po
 invenio_communities/translations/hu/LC_MESSAGES/messages.mo
 invenio_communities/translations/hu/LC_MESSAGES/messages.po
+invenio_communities/translations/hu_HU/LC_MESSAGES/messages.mo
+invenio_communities/translations/hu_HU/LC_MESSAGES/messages.po
 invenio_communities/translations/it/LC_MESSAGES/messages.mo
 invenio_communities/translations/it/LC_MESSAGES/messages.po
 invenio_communities/translations/ja/LC_MESSAGES/messages.mo
 invenio_communities/translations/ja/LC_MESSAGES/messages.po
 invenio_communities/translations/ka/LC_MESSAGES/messages.mo
 invenio_communities/translations/ka/LC_MESSAGES/messages.po
 invenio_communities/translations/lt/LC_MESSAGES/messages.mo
 invenio_communities/translations/lt/LC_MESSAGES/messages.po
+invenio_communities/translations/ne/LC_MESSAGES/messages.mo
+invenio_communities/translations/ne/LC_MESSAGES/messages.po
 invenio_communities/translations/no/LC_MESSAGES/messages.mo
 invenio_communities/translations/no/LC_MESSAGES/messages.po
 invenio_communities/translations/pl/LC_MESSAGES/messages.mo
 invenio_communities/translations/pl/LC_MESSAGES/messages.po
 invenio_communities/translations/pt/LC_MESSAGES/messages.mo
 invenio_communities/translations/pt/LC_MESSAGES/messages.po
 invenio_communities/translations/ro/LC_MESSAGES/messages.mo
@@ -397,18 +435,22 @@
 invenio_communities/translations/ru/LC_MESSAGES/messages.po
 invenio_communities/translations/rw/LC_MESSAGES/messages.mo
 invenio_communities/translations/rw/LC_MESSAGES/messages.po
 invenio_communities/translations/sk/LC_MESSAGES/messages.mo
 invenio_communities/translations/sk/LC_MESSAGES/messages.po
 invenio_communities/translations/sv/LC_MESSAGES/messages.mo
 invenio_communities/translations/sv/LC_MESSAGES/messages.po
+invenio_communities/translations/sv_SE/LC_MESSAGES/messages.mo
+invenio_communities/translations/sv_SE/LC_MESSAGES/messages.po
 invenio_communities/translations/tr/LC_MESSAGES/messages.mo
 invenio_communities/translations/tr/LC_MESSAGES/messages.po
 invenio_communities/translations/uk/LC_MESSAGES/messages.mo
 invenio_communities/translations/uk/LC_MESSAGES/messages.po
+invenio_communities/translations/uk_UA/LC_MESSAGES/messages.mo
+invenio_communities/translations/uk_UA/LC_MESSAGES/messages.po
 invenio_communities/translations/zh_CN/LC_MESSAGES/messages.mo
 invenio_communities/translations/zh_CN/LC_MESSAGES/messages.po
 invenio_communities/translations/zh_TW/LC_MESSAGES/messages.mo
 invenio_communities/translations/zh_TW/LC_MESSAGES/messages.po
 invenio_communities/views/__init__.py
 invenio_communities/views/api.py
 invenio_communities/views/communities.py
```

### Comparing `invenio-communities-7.0.0/invenio_communities.egg-info/entry_points.txt` & `invenio-communities-7.0.1/invenio_communities.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/run-js-linter.sh` & `invenio-communities-7.0.1/run-js-linter.sh`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/run-tests.sh` & `invenio-communities-7.0.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/setup.cfg` & `invenio-communities-7.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/cache/test_identity_redis_cache.py` & `invenio-communities-7.0.1/tests/cache/test_identity_redis_cache.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/communities/conftest.py` & `invenio-communities-7.0.1/tests/communities/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/communities/test_alembic.py` & `invenio-communities-7.0.1/tests/communities/test_alembic.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/communities/test_cli.py` & `invenio-communities-7.0.1/tests/communities/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/communities/test_community_ui_serializer.py` & `invenio-communities-7.0.1/tests/communities/test_community_ui_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/communities/test_components.py` & `invenio-communities-7.0.1/tests/communities/test_components.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/communities/test_relations_organizations.py` & `invenio-communities-7.0.1/tests/communities/test_relations_organizations.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/communities/test_relations_types.py` & `invenio-communities-7.0.1/tests/communities/test_relations_types.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/communities/test_resources.py` & `invenio-communities-7.0.1/tests/communities/test_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/communities/test_services.py` & `invenio-communities-7.0.1/tests/communities/test_services.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/communities/tests_views.py` & `invenio-communities-7.0.1/tests/communities/tests_views.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/conftest.py` & `invenio-communities-7.0.1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from invenio_access.permissions import any_user as any_user_need
 from invenio_access.permissions import superuser_access
 from invenio_accounts.models import Role
 from invenio_admin.permissions import action_admin_access
 from invenio_app.factory import create_api
 from invenio_records_resources.services.custom_fields import TextCF
 from invenio_requests.proxies import current_events_service, current_requests_service
-from invenio_users_resources.records import UserAggregate
+from invenio_users_resources.proxies import current_users_service
 from invenio_vocabularies.proxies import current_service as vocabulary_service
 from invenio_vocabularies.records.api import Vocabulary
 
 from invenio_communities.communities.records.api import Community
 from invenio_communities.members.records.api import Member
 from invenio_communities.proxies import current_communities
 
@@ -448,15 +448,16 @@
             role=name,
             visible=False,
             active=True,
         )
         member_service.indexer.index(m)
         Member.index.refresh()
     # reindexing users to make sure the user service is up-to-date
-    UserAggregate.index.refresh()
+    current_users_service.indexer.process_bulk_queue()
+    current_users_service.record_cls.index.refresh()
     db.session.commit()
     return users
 
 
 @pytest.fixture(scope="module")
 def cli_runner(base_app):
     """Create a CLI runner for testing a CLI command."""
```

### Comparing `invenio-communities-7.0.0/tests/members/conftest.py` & `invenio-communities-7.0.1/tests/members/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/members/test_members_components.py` & `invenio-communities-7.0.1/tests/members/test_members_components.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/members/test_members_no_groups.py` & `invenio-communities-7.0.1/tests/members/test_members_no_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/members/test_members_resource.py` & `invenio-communities-7.0.1/tests/members/test_members_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/members/test_members_services.py` & `invenio-communities-7.0.1/tests/members/test_members_services.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/records/conftest.py` & `invenio-communities-7.0.1/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/records/mock_module/api.py` & `invenio-communities-7.0.1/tests/records/mock_module/api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/records/mock_module/models.py` & `invenio-communities-7.0.1/tests/records/mock_module/models.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/records/test_mockrecords_api.py` & `invenio-communities-7.0.1/tests/records/test_mockrecords_api.py`

 * *Files identical despite different names*

### Comparing `invenio-communities-7.0.0/tests/test_notifications.py` & `invenio-communities-7.0.1/tests/test_notifications.py`

 * *Files identical despite different names*

