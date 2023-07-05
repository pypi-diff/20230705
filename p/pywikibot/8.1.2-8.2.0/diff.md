# Comparing `tmp/pywikibot-8.1.2.tar.gz` & `tmp/pywikibot-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywikibot-8.1.2.tar", last modified: Sun Apr 23 07:55:56 2023, max compression
+gzip compressed data, was "pywikibot-8.2.0.tar", last modified: Wed Jul  5 08:35:04 2023, max compression
```

## Comparing `pywikibot-8.1.2.tar` & `pywikibot-8.2.0.tar`

### file list

```diff
@@ -1,311 +1,312 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.433088 pywikibot-8.1.2/
--rw-rw-rw-   0        0        0     4115 2023-04-10 16:20:49.000000 pywikibot-8.1.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     1086 2023-04-10 16:20:49.000000 pywikibot-8.1.2/LICENSE
--rw-rw-rw-   0        0        0       40 2023-04-10 16:20:49.000000 pywikibot-8.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    14626 2023-04-23 07:55:56.432156 pywikibot-8.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5495 2023-04-10 16:20:49.000000 pywikibot-8.1.2/README.rst
--rw-rw-rw-   0        0        0     6351 2023-04-16 15:04:28.000000 pywikibot-8.1.2/make_dist.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.307106 pywikibot-8.1.2/pywikibot/
--rw-rw-rw-   0        0        0    55820 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/__init__.py
--rw-rw-rw-   0        0        0      794 2023-04-23 07:34:55.000000 pywikibot-8.1.2/pywikibot/__metadata__.py
--rw-rw-rw-   0        0        0     1886 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/_wbtypes.py
--rw-rw-rw-   0        0        0     4476 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/backports.py
--rw-rw-rw-   0        0        0    96117 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/bot.py
--rw-rw-rw-   0        0        0    21207 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/bot_choice.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.382276 pywikibot-8.1.2/pywikibot/comms/
--rw-rw-rw-   0        0        0      121 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/comms/__init__.py
--rw-rw-rw-   0        0        0    15749 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/comms/eventstreams.py
--rw-rw-rw-   0        0        0    19597 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/comms/http.py
--rw-rw-rw-   0        0        0    46527 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/config.py
--rw-rw-rw-   0        0        0    46135 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/cosmetic_changes.py
--rw-rw-rw-   0        0        0     2090 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/daemonize.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.393057 pywikibot-8.1.2/pywikibot/data/
--rw-rw-rw-   0        0        0      160 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.404032 pywikibot-8.1.2/pywikibot/data/api/
--rw-rw-rw-   0        0        0     3174 2023-04-22 08:48:04.000000 pywikibot-8.1.2/pywikibot/data/api/__init__.py
--rw-rw-rw-   0        0        0    41816 2023-04-14 14:19:36.000000 pywikibot-8.1.2/pywikibot/data/api/_generators.py
--rw-rw-rw-   0        0        0     7398 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/api/_optionset.py
--rw-rw-rw-   0        0        0    23233 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/api/_paraminfo.py
--rw-rw-rw-   0        0        0    52512 2023-04-16 16:10:48.000000 pywikibot-8.1.2/pywikibot/data/api/_requests.py
--rw-rw-rw-   0        0        0    14143 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/memento.py
--rw-rw-rw-   0        0        0     2919 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/mysql.py
--rw-rw-rw-   0        0        0     8969 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/sparql.py
--rw-rw-rw-   0        0        0     3970 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/data/wikistats.py
--rw-rw-rw-   0        0        0    96940 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/date.py
--rw-rw-rw-   0        0        0    24879 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/diff.py
--rw-rw-rw-   0        0        0     2042 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/echo.py
--rw-rw-rw-   0        0        0     7830 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/editor.py
--rw-rw-rw-   0        0        0    21221 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.459884 pywikibot-8.1.2/pywikibot/families/
--rw-rw-rw-   0        0        0      118 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/__init__.py
--rw-rw-rw-   0        0        0     4303 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/commons_family.py
--rw-rw-rw-   0        0        0      443 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/foundation_family.py
--rw-rw-rw-   0        0        0      463 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/i18n_family.py
--rw-rw-rw-   0        0        0      355 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/incubator_family.py
--rw-rw-rw-   0        0        0      662 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/lingualibre_family.py
--rw-rw-rw-   0        0        0      401 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/mediawiki_family.py
--rw-rw-rw-   0        0        0      593 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/meta_family.py
--rw-rw-rw-   0        0        0     1330 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/osm_family.py
--rw-rw-rw-   0        0        0      369 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/outreach_family.py
--rw-rw-rw-   0        0        0      361 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/species_family.py
--rw-rw-rw-   0        0        0      638 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/vikidia_family.py
--rw-rw-rw-   0        0        0     2418 2023-04-16 15:09:16.000000 pywikibot-8.1.2/pywikibot/families/wikibooks_family.py
--rw-rw-rw-   0        0        0     3782 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikidata_family.py
--rw-rw-rw-   0        0        0     1742 2023-04-18 14:17:02.000000 pywikibot-8.1.2/pywikibot/families/wikihow_family.py
--rw-rw-rw-   0        0        0     1009 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikimania_family.py
--rw-rw-rw-   0        0        0      777 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikimediachapter_family.py
--rw-rw-rw-   0        0        0     1832 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/families/wikinews_family.py
--rw-rw-rw-   0        0        0    10737 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/families/wikipedia_family.py
--rw-rw-rw-   0        0        0     2886 2023-04-21 05:58:04.000000 pywikibot-8.1.2/pywikibot/families/wikiquote_family.py
--rw-rw-rw-   0        0        0     5335 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/families/wikisource_family.py
--rw-rw-rw-   0        0        0      495 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikispore_family.py
--rw-rw-rw-   0        0        0      425 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikitech_family.py
--rw-rw-rw-   0        0        0     1150 2023-04-14 14:19:20.000000 pywikibot-8.1.2/pywikibot/families/wikiversity_family.py
--rw-rw-rw-   0        0        0     1027 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/families/wikivoyage_family.py
--rw-rw-rw-   0        0        0     3850 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/families/wiktionary_family.py
--rw-rw-rw-   0        0        0     2414 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/families/wowwiki_family.py
--rw-rw-rw-   0        0        0    37565 2023-04-18 14:17:02.000000 pywikibot-8.1.2/pywikibot/family.py
--rw-rw-rw-   0        0        0    33191 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/fixes.py
--rw-rw-rw-   0        0        0    20119 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/flow.py
--rw-rw-rw-   0        0        0    30038 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/i18n.py
--rw-rw-rw-   0        0        0     8343 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/interwiki_graph.py
--rw-rw-rw-   0        0        0    13245 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/logentries.py
--rw-rw-rw-   0        0        0    12508 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/logging.py
--rw-rw-rw-   0        0        0    22781 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/login.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.482845 pywikibot-8.1.2/pywikibot/page/
--rw-rw-rw-   0        0        0     2350 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/__init__.py
--rw-rw-rw-   0        0        0    86912 2023-04-17 14:18:54.000000 pywikibot-8.1.2/pywikibot/page/_basepage.py
--rw-rw-rw-   0        0        0    14617 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_category.py
--rw-rw-rw-   0        0        0    19000 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_collections.py
--rw-rw-rw-   0        0        0     2183 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_decorators.py
--rw-rw-rw-   0        0        0    14648 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_filepage.py
--rw-rw-rw-   0        0        0    29601 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_links.py
--rw-rw-rw-   0        0        0     8515 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_page.py
--rw-rw-rw-   0        0        0     2997 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_revision.py
--rw-rw-rw-   0        0        0     4049 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_toolforge.py
--rw-rw-rw-   0        0        0    16348 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/page/_user.py
--rw-rw-rw-   0        0        0    86375 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/page/_wikibase.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.490821 pywikibot-8.1.2/pywikibot/pagegenerators/
--rw-rw-rw-   0        0        0    29164 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/pagegenerators/__init__.py
--rw-rw-rw-   0        0        0    40342 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/pagegenerators/_factory.py
--rw-rw-rw-   0        0        0    19272 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/pagegenerators/_filters.py
--rw-rw-rw-   0        0        0    44438 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/pagegenerators/_generators.py
--rw-rw-rw-   0        0        0     3938 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/plural.py
--rw-rw-rw-   0        0        0    48967 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/proofreadpage.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.504819 pywikibot-8.1.2/pywikibot/scripts/
--rw-rw-rw-   0        0        0      882 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/__init__.py
--rw-rw-rw-   0        0        0    12032 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/scripts/generate_family_file.py
--rw-rw-rw-   0        0        0    20029 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/scripts/generate_user_files.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.515767 pywikibot-8.1.2/pywikibot/scripts/i18n/
--rw-rw-rw-   0        0        0      309 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.346323 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/
--rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ab.json
--rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/af.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/an.json
--rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ar.json
--rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/arc.json
--rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ast.json
--rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/av.json
--rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/awa.json
--rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/az.json
--rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/azb.json
--rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ba.json
--rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bar.json
--rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bcc.json
--rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/be-tarask.json
--rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/be.json
--rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bg.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bjn.json
--rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bn.json
--rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bo.json
--rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/br.json
--rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bs.json
--rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ca.json
--rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ce.json
--rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ckb.json
--rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/cs.json
--rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/csb.json
--rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/cy.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/da.json
--rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/de.json
--rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/diq.json
--rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/el.json
--rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/en.json
--rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/eo.json
--rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/es.json
--rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/et.json
--rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/eu.json
--rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fa.json
--rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fi.json
--rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fo.json
--rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fr.json
--rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/frp.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/frr.json
--rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fy.json
--rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ga.json
--rw-rw-rw-   0        0        0     1082 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/gl.json
--rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/gsw.json
--rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hak.json
--rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/haw.json
--rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/he.json
--rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hi.json
--rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hr.json
--rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hsb.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hu.json
--rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hy.json
--rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ia.json
--rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/id.json
--rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ie.json
--rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ig.json
--rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ilo.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/io.json
--rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/is.json
--rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/it.json
--rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ja.json
--rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/jv.json
--rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kab.json
--rw-rw-rw-   0        0        0     1068 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kk.json
--rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/km.json
--rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kn.json
--rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ko.json
--rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/krc.json
--rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ksh.json
--rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ku.json
--rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ky.json
--rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/la.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lb.json
--rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/li.json
--rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lki.json
--rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lt.json
--rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lv.json
--rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/map-bms.json
--rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mg.json
--rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/min.json
--rw-rw-rw-   0        0        0     1353 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mk.json
--rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ml.json
--rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mni.json
--rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mr.json
--rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ms.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mt.json
--rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/my.json
--rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nan.json
--rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nb.json
--rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nds-nl.json
--rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nds.json
--rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ne.json
--rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/new.json
--rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nl.json
--rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nn.json
--rw-rw-rw-   0        0        0     1344 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nqo.json
--rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nyn.json
--rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/oc.json
--rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/olo.json
--rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/or.json
--rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pa.json
--rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pdc.json
--rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pfl.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pl.json
--rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pms.json
--rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pt-br.json
--rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pt.json
--rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/qqq.json
--rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ro.json
--rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ru.json
--rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/scn.json
--rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sco.json
--rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sd.json
--rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sh.json
--rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/si.json
--rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sk.json
--rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/skr-arab.json
--rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sl.json
--rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sms.json
--rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/so.json
--rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sq.json
--rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sr.json
--rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/su.json
--rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sv.json
--rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sw.json
--rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/szl.json
--rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ta.json
--rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/te.json
--rw-rw-rw-   0        0        0      101 2023-04-06 12:04:37.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tg.json
--rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/th.json
--rw-rw-rw-   0        0        0      155 2023-04-06 12:04:37.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tk.json
--rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tl.json
--rw-rw-rw-   0        0        0     1115 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tly.json
--rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tr.json
--rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tt.json
--rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/uk.json
--rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ur.json
--rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/uz.json
--rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/vec.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/vep.json
--rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/vi.json
--rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/vo.json
--rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/war.json
--rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/yi.json
--rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/yue.json
--rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/zh.json
--rw-rw-rw-   0        0        0     6093 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/login.py
--rw-rw-rw-   0        0        0     3246 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/preload_sites.py
--rw-rw-rw-   0        0        0     1791 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/shell.py
--rw-rw-rw-   0        0        0     3313 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/scripts/version.py
--rw-rw-rw-   0        0        0    18384 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/scripts/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.384219 pywikibot-8.1.2/pywikibot/site/
--rw-rw-rw-   0        0        0      744 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/__init__.py
--rw-rw-rw-   0        0        0   112506 2023-04-16 16:10:48.000000 pywikibot-8.1.2/pywikibot/site/_apisite.py
--rw-rw-rw-   0        0        0    15858 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/site/_basesite.py
--rw-rw-rw-   0        0        0    38276 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_datasite.py
--rw-rw-rw-   0        0        0     4254 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_decorators.py
--rw-rw-rw-   0        0        0    27978 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_extensions.py
--rw-rw-rw-   0        0        0    93641 2023-04-17 14:52:33.000000 pywikibot-8.1.2/pywikibot/site/_generators.py
--rw-rw-rw-   0        0        0     3003 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_interwikimap.py
--rw-rw-rw-   0        0        0    14558 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_namespace.py
--rw-rw-rw-   0        0        0     1667 2023-04-18 14:53:43.000000 pywikibot-8.1.2/pywikibot/site/_obsoletesites.py
--rw-rw-rw-   0        0        0    14354 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_siteinfo.py
--rw-rw-rw-   0        0        0     4868 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/site/_tokenwallet.py
--rw-rw-rw-   0        0        0    25321 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/site/_upload.py
--rw-rw-rw-   0        0        0    11156 2023-04-21 07:28:37.000000 pywikibot-8.1.2/pywikibot/site_detect.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.392197 pywikibot-8.1.2/pywikibot/specialbots/
--rw-rw-rw-   0        0        0      371 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/specialbots/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/specialbots/_unlink.py
--rw-rw-rw-   0        0        0    20247 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/specialbots/_upload.py
--rw-rw-rw-   0        0        0    84825 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/textlib.py
--rw-rw-rw-   0        0        0    12074 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/throttle.py
--rw-rw-rw-   0        0        0    15061 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/time.py
--rw-rw-rw-   0        0        0     3267 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/titletranslate.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.414139 pywikibot-8.1.2/pywikibot/tools/
--rw-rw-rw-   0        0        0    27376 2023-04-23 07:41:13.000000 pywikibot-8.1.2/pywikibot/tools/__init__.py
--rw-rw-rw-   0        0        0    25547 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/tools/_deprecate.py
--rw-rw-rw-   0        0        0     1205 2023-04-22 12:39:46.000000 pywikibot-8.1.2/pywikibot/tools/_logging.py
--rw-rw-rw-   0        0        0    22207 2023-04-22 12:39:47.000000 pywikibot-8.1.2/pywikibot/tools/_unidata.py
--rw-rw-rw-   0        0        0     4084 2023-04-23 07:34:23.000000 pywikibot-8.1.2/pywikibot/tools/chars.py
--rw-rw-rw-   0        0        0     8765 2023-04-22 12:39:47.000000 pywikibot-8.1.2/pywikibot/tools/collections.py
--rw-rw-rw-   0        0        0    11075 2023-04-22 12:39:47.000000 pywikibot-8.1.2/pywikibot/tools/djvu.py
--rw-rw-rw-   0        0        0     4021 2023-04-22 12:39:47.000000 pywikibot-8.1.2/pywikibot/tools/formatter.py
--rw-rw-rw-   0        0        0     9745 2023-04-22 12:39:48.000000 pywikibot-8.1.2/pywikibot/tools/itertools.py
--rw-rw-rw-   0        0        0     7334 2023-04-22 12:39:48.000000 pywikibot-8.1.2/pywikibot/tools/threading.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.427106 pywikibot-8.1.2/pywikibot/userinterfaces/
--rw-rw-rw-   0        0        0      870 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/__init__.py
--rw-rw-rw-   0        0        0     1906 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/_interface_base.py
--rw-rw-rw-   0        0        0     2687 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/buffer_interface.py
--rw-rw-rw-   0        0        0    22100 2023-04-16 15:04:28.000000 pywikibot-8.1.2/pywikibot/userinterfaces/gui.py
--rw-rw-rw-   0        0        0      457 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface.py
--rw-rw-rw-   0        0        0    24536 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_base.py
--rw-rw-rw-   0        0        0     2114 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_unix.py
--rw-rw-rw-   0        0        0     2012 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_win32.py
--rw-rw-rw-   0        0        0    90310 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/userinterfaces/transliteration.py
--rw-rw-rw-   0        0        0    16698 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/version.py
--rw-rw-rw-   0        0        0     7366 2023-04-10 16:20:49.000000 pywikibot-8.1.2/pywikibot/xmlreader.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:55.375086 pywikibot-8.1.2/pywikibot.egg-info/
--rw-rw-rw-   0        0        0    14626 2023-04-23 07:55:54.000000 pywikibot-8.1.2/pywikibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10447 2023-04-23 07:55:55.000000 pywikibot-8.1.2/pywikibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:55:54.000000 pywikibot-8.1.2/pywikibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-23 07:55:54.000000 pywikibot-8.1.2/pywikibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1228 2023-04-23 07:55:54.000000 pywikibot-8.1.2/pywikibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-23 07:55:54.000000 pywikibot-8.1.2/pywikibot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 07:55:56.433444 pywikibot-8.1.2/setup.cfg
--rw-rw-rw-   0        0        0    13116 2023-04-15 09:02:53.000000 pywikibot-8.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:55:56.430478 pywikibot-8.1.2/tests/
--rw-rw-rw-   0        0        0     2814 2023-04-16 15:04:28.000000 pywikibot-8.1.2/tests/tests_tests.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.304314 pywikibot-8.2.0/
+-rw-rw-rw-   0        0        0     4133 2023-07-02 16:47:05.000000 pywikibot-8.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0      177 2023-05-16 07:53:09.000000 pywikibot-8.2.0/CODE_OF_CONDUCT.rst
+-rw-rw-rw-   0        0        0     1086 2023-05-16 07:53:09.000000 pywikibot-8.2.0/LICENSE
+-rw-rw-rw-   0        0        0       88 2023-07-02 16:47:05.000000 pywikibot-8.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    15888 2023-07-05 08:35:04.303317 pywikibot-8.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5502 2023-07-02 16:47:05.000000 pywikibot-8.2.0/README.rst
+-rw-rw-rw-   0        0        0     6529 2023-07-05 08:22:11.000000 pywikibot-8.2.0/ROADMAP.rst
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.079578 pywikibot-8.2.0/pywikibot/
+-rw-rw-rw-   0        0        0    55546 2023-07-05 07:19:34.000000 pywikibot-8.2.0/pywikibot/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-07-05 08:22:11.000000 pywikibot-8.2.0/pywikibot/__metadata__.py
+-rw-rw-rw-   0        0        0     1886 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/_wbtypes.py
+-rw-rw-rw-   0        0        0     5655 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/backports.py
+-rw-rw-rw-   0        0        0    94724 2023-07-04 09:42:32.000000 pywikibot-8.2.0/pywikibot/bot.py
+-rw-rw-rw-   0        0        0    21197 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/bot_choice.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.133434 pywikibot-8.2.0/pywikibot/comms/
+-rw-rw-rw-   0        0        0      121 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/comms/__init__.py
+-rw-rw-rw-   0        0        0    15771 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/comms/eventstreams.py
+-rw-rw-rw-   0        0        0    20087 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/comms/http.py
+-rw-rw-rw-   0        0        0    46549 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/config.py
+-rw-rw-rw-   0        0        0    45958 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/cosmetic_changes.py
+-rw-rw-rw-   0        0        0     2090 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/daemonize.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.144404 pywikibot-8.2.0/pywikibot/data/
+-rw-rw-rw-   0        0        0      160 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.153381 pywikibot-8.2.0/pywikibot/data/api/
+-rw-rw-rw-   0        0        0     3174 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/api/__init__.py
+-rw-rw-rw-   0        0        0    41575 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/api/_generators.py
+-rw-rw-rw-   0        0        0     7368 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/api/_optionset.py
+-rw-rw-rw-   0        0        0    23238 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/api/_paraminfo.py
+-rw-rw-rw-   0        0        0    53439 2023-07-04 09:42:32.000000 pywikibot-8.2.0/pywikibot/data/api/_requests.py
+-rw-rw-rw-   0        0        0    14120 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/memento.py
+-rw-rw-rw-   0        0        0     2919 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/data/mysql.py
+-rw-rw-rw-   0        0        0     8902 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/data/sparql.py
+-rw-rw-rw-   0        0        0     3970 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/data/wikistats.py
+-rw-rw-rw-   0        0        0    96751 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/date.py
+-rw-rw-rw-   0        0        0    24902 2023-07-04 16:05:52.000000 pywikibot-8.2.0/pywikibot/diff.py
+-rw-rw-rw-   0        0        0     2042 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/echo.py
+-rw-rw-rw-   0        0        0     7918 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/editor.py
+-rw-rw-rw-   0        0        0    21189 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.210229 pywikibot-8.2.0/pywikibot/families/
+-rw-rw-rw-   0        0        0      118 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/families/__init__.py
+-rw-rw-rw-   0        0        0     1656 2023-07-04 16:26:13.000000 pywikibot-8.2.0/pywikibot/families/commons_family.py
+-rw-rw-rw-   0        0        0      443 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/families/foundation_family.py
+-rw-rw-rw-   0        0        0      338 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/i18n_family.py
+-rw-rw-rw-   0        0        0      355 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/incubator_family.py
+-rw-rw-rw-   0        0        0      583 2023-07-04 16:26:13.000000 pywikibot-8.2.0/pywikibot/families/lingualibre_family.py
+-rw-rw-rw-   0        0        0      401 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/mediawiki_family.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/meta_family.py
+-rw-rw-rw-   0        0        0     1205 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/osm_family.py
+-rw-rw-rw-   0        0        0      369 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/outreach_family.py
+-rw-rw-rw-   0        0        0      361 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/species_family.py
+-rw-rw-rw-   0        0        0      513 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/vikidia_family.py
+-rw-rw-rw-   0        0        0     2418 2023-07-05 07:54:18.000000 pywikibot-8.2.0/pywikibot/families/wikibooks_family.py
+-rw-rw-rw-   0        0        0      958 2023-07-04 16:26:13.000000 pywikibot-8.2.0/pywikibot/families/wikidata_family.py
+-rw-rw-rw-   0        0        0     1631 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikihow_family.py
+-rw-rw-rw-   0        0        0     1009 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/families/wikimania_family.py
+-rw-rw-rw-   0        0        0      777 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikimediachapter_family.py
+-rw-rw-rw-   0        0        0     1832 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikinews_family.py
+-rw-rw-rw-   0        0        0    10732 2023-07-05 07:54:18.000000 pywikibot-8.2.0/pywikibot/families/wikipedia_family.py
+-rw-rw-rw-   0        0        0     2886 2023-07-05 07:54:18.000000 pywikibot-8.2.0/pywikibot/families/wikiquote_family.py
+-rw-rw-rw-   0        0        0     5335 2023-07-05 07:54:18.000000 pywikibot-8.2.0/pywikibot/families/wikisource_family.py
+-rw-rw-rw-   0        0        0      431 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikispore_family.py
+-rw-rw-rw-   0        0        0      425 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/families/wikitech_family.py
+-rw-rw-rw-   0        0        0     1150 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikiversity_family.py
+-rw-rw-rw-   0        0        0     1027 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wikivoyage_family.py
+-rw-rw-rw-   0        0        0     3850 2023-07-05 07:54:18.000000 pywikibot-8.2.0/pywikibot/families/wiktionary_family.py
+-rw-rw-rw-   0        0        0     2414 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/families/wowwiki_family.py
+-rw-rw-rw-   0        0        0    41181 2023-07-04 16:26:13.000000 pywikibot-8.2.0/pywikibot/family.py
+-rw-rw-rw-   0        0        0    33191 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/fixes.py
+-rw-rw-rw-   0        0        0    20119 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/flow.py
+-rw-rw-rw-   0        0        0    29992 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/i18n.py
+-rw-rw-rw-   0        0        0     8278 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/interwiki_graph.py
+-rw-rw-rw-   0        0        0    13177 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/logentries.py
+-rw-rw-rw-   0        0        0    12508 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/logging.py
+-rw-rw-rw-   0        0        0    22771 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/login.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.230176 pywikibot-8.2.0/pywikibot/page/
+-rw-rw-rw-   0        0        0     2350 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/__init__.py
+-rw-rw-rw-   0        0        0    86838 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_basepage.py
+-rw-rw-rw-   0        0        0    14599 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_category.py
+-rw-rw-rw-   0        0        0    18914 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_collections.py
+-rw-rw-rw-   0        0        0     2139 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_decorators.py
+-rw-rw-rw-   0        0        0    17407 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_filepage.py
+-rw-rw-rw-   0        0        0    29329 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_links.py
+-rw-rw-rw-   0        0        0     8515 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_page.py
+-rw-rw-rw-   0        0        0     2997 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/page/_revision.py
+-rw-rw-rw-   0        0        0     4049 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_toolforge.py
+-rw-rw-rw-   0        0        0    16266 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/page/_user.py
+-rw-rw-rw-   0        0        0    85875 2023-07-05 07:19:34.000000 pywikibot-8.2.0/pywikibot/page/_wikibase.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.237158 pywikibot-8.2.0/pywikibot/pagegenerators/
+-rw-rw-rw-   0        0        0    29391 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/pagegenerators/__init__.py
+-rw-rw-rw-   0        0        0    40292 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/pagegenerators/_factory.py
+-rw-rw-rw-   0        0        0    19242 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/pagegenerators/_filters.py
+-rw-rw-rw-   0        0        0    45143 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/pagegenerators/_generators.py
+-rw-rw-rw-   0        0        0     3938 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/plural.py
+-rw-rw-rw-   0        0        0    48615 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/proofreadpage.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.251120 pywikibot-8.2.0/pywikibot/scripts/
+-rw-rw-rw-   0        0        0      882 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/scripts/__init__.py
+-rw-rw-rw-   0        0        0    11922 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/generate_family_file.py
+-rw-rw-rw-   0        0        0    20021 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/generate_user_files.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.253116 pywikibot-8.2.0/pywikibot/scripts/i18n/
+-rw-rw-rw-   0        0        0      309 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.241483 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/
+-rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ab.json
+-rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/af.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/an.json
+-rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ar.json
+-rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/arc.json
+-rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ast.json
+-rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/av.json
+-rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/awa.json
+-rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/az.json
+-rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/azb.json
+-rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ba.json
+-rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bar.json
+-rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bcc.json
+-rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json
+-rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/be.json
+-rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bg.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bjn.json
+-rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bn.json
+-rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bo.json
+-rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/br.json
+-rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bs.json
+-rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ca.json
+-rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ce.json
+-rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ckb.json
+-rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/cs.json
+-rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/csb.json
+-rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/cy.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/da.json
+-rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/de.json
+-rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/diq.json
+-rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/el.json
+-rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/en.json
+-rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/eo.json
+-rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/es.json
+-rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/et.json
+-rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/eu.json
+-rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fa.json
+-rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fi.json
+-rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fo.json
+-rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fr.json
+-rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/frp.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/frr.json
+-rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fy.json
+-rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ga.json
+-rw-rw-rw-   0        0        0     1082 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/gl.json
+-rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/gsw.json
+-rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hak.json
+-rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/haw.json
+-rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/he.json
+-rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hi.json
+-rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hr.json
+-rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hsb.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hu.json
+-rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hy.json
+-rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ia.json
+-rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/id.json
+-rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ie.json
+-rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ig.json
+-rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ilo.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/io.json
+-rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/is.json
+-rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/it.json
+-rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ja.json
+-rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/jv.json
+-rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kab.json
+-rw-rw-rw-   0        0        0     1068 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kk.json
+-rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/km.json
+-rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kn.json
+-rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ko.json
+-rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/krc.json
+-rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ksh.json
+-rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ku.json
+-rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ky.json
+-rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/la.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lb.json
+-rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/li.json
+-rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lki.json
+-rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lt.json
+-rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lv.json
+-rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/map-bms.json
+-rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mg.json
+-rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/min.json
+-rw-rw-rw-   0        0        0     1353 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mk.json
+-rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ml.json
+-rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mni.json
+-rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mr.json
+-rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ms.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mt.json
+-rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/my.json
+-rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nan.json
+-rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nb.json
+-rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json
+-rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nds.json
+-rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ne.json
+-rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/new.json
+-rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nl.json
+-rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nn.json
+-rw-rw-rw-   0        0        0     1344 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nqo.json
+-rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nyn.json
+-rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/oc.json
+-rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/olo.json
+-rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/or.json
+-rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pa.json
+-rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pdc.json
+-rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pfl.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pl.json
+-rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pms.json
+-rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pt-br.json
+-rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pt.json
+-rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/qqq.json
+-rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ro.json
+-rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ru.json
+-rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/scn.json
+-rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sco.json
+-rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sd.json
+-rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sh.json
+-rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/si.json
+-rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sk.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/skr-arab.json
+-rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sl.json
+-rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sms.json
+-rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/so.json
+-rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sq.json
+-rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sr.json
+-rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/su.json
+-rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sv.json
+-rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sw.json
+-rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/szl.json
+-rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ta.json
+-rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/te.json
+-rw-rw-rw-   0        0        0      101 2023-04-06 12:04:37.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tg.json
+-rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/th.json
+-rw-rw-rw-   0        0        0      155 2023-04-06 12:04:37.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tk.json
+-rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tl.json
+-rw-rw-rw-   0        0        0     1115 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tly.json
+-rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tr.json
+-rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tt.json
+-rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/uk.json
+-rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ur.json
+-rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/uz.json
+-rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/vec.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/vep.json
+-rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/vi.json
+-rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/vo.json
+-rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/war.json
+-rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/yi.json
+-rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/yue.json
+-rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/zh.json
+-rw-rw-rw-   0        0        0     6096 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/login.py
+-rw-rw-rw-   0        0        0     3225 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/preload_sites.py
+-rw-rw-rw-   0        0        0     2033 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/shell.py
+-rw-rw-rw-   0        0        0     3291 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/version.py
+-rw-rw-rw-   0        0        0    18351 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/scripts/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.263423 pywikibot-8.2.0/pywikibot/site/
+-rw-rw-rw-   0        0        0      744 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/site/__init__.py
+-rw-rw-rw-   0        0        0   112230 2023-07-04 16:26:14.000000 pywikibot-8.2.0/pywikibot/site/_apisite.py
+-rw-rw-rw-   0        0        0    15515 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_basesite.py
+-rw-rw-rw-   0        0        0    38219 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_datasite.py
+-rw-rw-rw-   0        0        0     4254 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/site/_decorators.py
+-rw-rw-rw-   0        0        0    27970 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_extensions.py
+-rw-rw-rw-   0        0        0    93527 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_generators.py
+-rw-rw-rw-   0        0        0     3003 2023-05-20 13:58:11.000000 pywikibot-8.2.0/pywikibot/site/_interwikimap.py
+-rw-rw-rw-   0        0        0    14558 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/site/_namespace.py
+-rw-rw-rw-   0        0        0     1595 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_obsoletesites.py
+-rw-rw-rw-   0        0        0    14357 2023-07-04 09:42:32.000000 pywikibot-8.2.0/pywikibot/site/_siteinfo.py
+-rw-rw-rw-   0        0        0     4868 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_tokenwallet.py
+-rw-rw-rw-   0        0        0    25199 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site/_upload.py
+-rw-rw-rw-   0        0        0    11156 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/site_detect.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.267413 pywikibot-8.2.0/pywikibot/specialbots/
+-rw-rw-rw-   0        0        0      371 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/specialbots/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/specialbots/_unlink.py
+-rw-rw-rw-   0        0        0    20160 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/specialbots/_upload.py
+-rw-rw-rw-   0        0        0    87550 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/textlib.py
+-rw-rw-rw-   0        0        0    12074 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/throttle.py
+-rw-rw-rw-   0        0        0    14991 2023-07-04 09:42:32.000000 pywikibot-8.2.0/pywikibot/time.py
+-rw-rw-rw-   0        0        0     3267 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/titletranslate.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.285365 pywikibot-8.2.0/pywikibot/tools/
+-rw-rw-rw-   0        0        0    28023 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/__init__.py
+-rw-rw-rw-   0        0        0    25727 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/_deprecate.py
+-rw-rw-rw-   0        0        0     1205 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/tools/_logging.py
+-rw-rw-rw-   0        0        0    22207 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/tools/_unidata.py
+-rw-rw-rw-   0        0        0     4076 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/chars.py
+-rw-rw-rw-   0        0        0     8765 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/tools/collections.py
+-rw-rw-rw-   0        0        0    10946 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/djvu.py
+-rw-rw-rw-   0        0        0     4018 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/formatter.py
+-rw-rw-rw-   0        0        0     9866 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/itertools.py
+-rw-rw-rw-   0        0        0     7210 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/tools/threading.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.299327 pywikibot-8.2.0/pywikibot/userinterfaces/
+-rw-rw-rw-   0        0        0      870 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/__init__.py
+-rw-rw-rw-   0        0        0     1906 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/_interface_base.py
+-rw-rw-rw-   0        0        0     2687 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/buffer_interface.py
+-rw-rw-rw-   0        0        0    22102 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/userinterfaces/gui.py
+-rw-rw-rw-   0        0        0      457 2023-05-15 15:00:32.000000 pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface.py
+-rw-rw-rw-   0        0        0    24478 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_base.py
+-rw-rw-rw-   0        0        0     2114 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_unix.py
+-rw-rw-rw-   0        0        0     2012 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_win32.py
+-rw-rw-rw-   0        0        0    90310 2023-05-16 07:53:09.000000 pywikibot-8.2.0/pywikibot/userinterfaces/transliteration.py
+-rw-rw-rw-   0        0        0    16654 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/version.py
+-rw-rw-rw-   0        0        0     7366 2023-07-02 16:47:05.000000 pywikibot-8.2.0/pywikibot/xmlreader.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:03.127450 pywikibot-8.2.0/pywikibot.egg-info/
+-rw-rw-rw-   0        0        0    15888 2023-07-05 08:35:02.000000 pywikibot-8.2.0/pywikibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10466 2023-07-05 08:35:03.000000 pywikibot-8.2.0/pywikibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 08:35:02.000000 pywikibot-8.2.0/pywikibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-05 08:35:02.000000 pywikibot-8.2.0/pywikibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1228 2023-07-05 08:35:02.000000 pywikibot-8.2.0/pywikibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-05 08:35:02.000000 pywikibot-8.2.0/pywikibot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 08:35:04.304314 pywikibot-8.2.0/setup.cfg
+-rw-rw-rw-   0        0        0    13228 2023-07-02 16:47:05.000000 pywikibot-8.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:04.301324 pywikibot-8.2.0/tests/
+-rw-rw-rw-   0        0        0     2814 2023-07-02 16:47:05.000000 pywikibot-8.2.0/tests/tests_tests.py
```

### Comparing `pywikibot-8.1.2/AUTHORS.rst` & `pywikibot-8.2.0/AUTHORS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     dennisroczek
     Denny Vrandecic
     DMaggot
     Didicodes
     Diwanshu Mittal
     Dmytro Dziuma
     Dr03ramos
+    Draco flavus
     DrTrigon
     Dvorapa
 
 E
 -
 
 ::
```

### Comparing `pywikibot-8.1.2/LICENSE` & `pywikibot-8.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/PKG-INFO` & `pywikibot-8.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.1.2
+Version: 8.2.0
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -154,15 +154,15 @@
 `MediaWiki API <https://www.mediawiki.org/wiki/API:Main_page>`_
 version 1.27 or higher.
 
 Also included are various general function scripts that can be adapted for
 different tasks.
 
 For further information about the library excluding scripts see
-the full `code documentation <https://doc.wikimedia.org/pywikibot/>`_.
+the full `code documentation <https://doc.wikimedia.org/pywikibot/stable/>`_.
 
 Quick start
 ===========
 
 .. code:: text
 
     pip install requests
@@ -257,22 +257,42 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Add support for guwwikinews (T334461)
-* Add support for kbdwiktionary (T333271)
-* Fix tools.chars.url2stringparsing for multiple encodings (T335224)
+* Add support for gpewiki (T335989)
+* family.WikibaseFamilyand family.DefaultWikibaseFamilywere added to familymodule
+* Remove incorrect time normalization in page.Claim(T338748, T325860, T57755)
+* Add support for other types of diffs in Site.compare()
+* Improvements for textlib.extract_sectionsfunction (T338748)
+* Backport ``itertools.batched()`` from Python 3.12 which replaces tools.itertools.itergroup
+* Upcast page types in pagegenerators.RecentChangesPageGenerator(T340450)
+* Enable FilePage.download()to download thumbnails (T247095)
+* Refactor tools.compute_file_hashand use ``hashlib.file_digest`` with Python 3.11
+* Url ends with curly bracket in textlib.compileLinkR(T338029)
+* Allows spaces in environment variables for editor.TextEditor(T102465, T323078)
+* Add textlib.get_regexespublic function (T336144)
+* Return 'https' scheme with family.Family.protocol(T326046)
+* Use ``build`` instead of ``setuptools.setup()`` to build the distribution
+* Raise ``ConnectionError`` on ``requests.ReadTimeout`` in comms.http.error_handling_callback
+* Raise exceptions.ServerErroron ``requests.ReadTimeout`` in comms.http.error_handling_callback
+* Do not evaluate pywikibot.Sitewith dict.pop() as default value (T335720)
+* L10N updates
+* family.Familyclass was rewritten. ``obsolete.setter`` was removed,
+  family.Family.interwiki_replacementsreturns an invariant mapping,
+  family.Family.interwiki_removalsreturns a frozenset. ``closed_wikis``,
+  ``removed_wikis`` and ``code_aliases`` are family.Familyclass attributes.  (T334834)
 
 
 Deprecations
 ------------
 
+* 8.2.0: *normalize* parameter of WbTime.toTimestrand WbTime.toWikibasewill be removed
 * 8.1.0: Dependency of exceptions.NoSiteLinkErrorfrom exceptions.NoPageErrorwill be removed
 * 8.1.0: ``exceptions.Server414Error`` is deprecated in favour of exceptions.Client414Error
 * 8.0.0: Timestamp.clone()method is deprecated
   in favour of ``Timestamp.replace()`` method.
 * 8.0.0: family.Family.maximum_GET_lengthmethod is deprecated in favour of
   config.maximum_GET_length(T325957)
 * 8.0.0: ``addOnly`` parameter of textlib.replaceLanguageLinksand
@@ -295,18 +315,16 @@
 * 7.4.0: ``FilePage.usingPages()`` was renamed to using_pages()
 * 7.2.0: ``tb`` parameter of exception()function was renamed to ``exc_info``
 * 7.2.0: XMLDumpOldPageGenerator is deprecated in favour of a ``content`` parameter of
   XMLDumpPageGenerator(T306134)
 * 7.2.0: RedirectPageBot and NoRedirectPageBot bot classes are deprecated in favour of
   use_redirectsattribute
 * 7.2.0: tools.formatter.color_formatis deprecated and will be removed
-* 7.1.0: Unused `get_redirect` parameter of Page.getOldVersion() will be removed
-* 7.1.0: APISite._simple_request() will be removed in favour of APISite.simple_request()
+* 7.1.0: Unused ``get_redirect`` parameter of Page.getOldVersion()will be removed
 * 7.0.0: User.isBlocked() method is renamed to is_blocked for consistency
-* 7.0.0: Private BaseBot counters _treat_counter, _save_counter, _skip_counter will be removed in favour of collections.Counter counter attribute
 * 7.0.0: A boolean watch parameter in Page.save() is deprecated and will be desupported
 * 7.0.0: baserevid parameter of editSource(), editQualifier(), removeClaims(), removeSources(), remove_qualifiers() DataSite methods will be removed
 * 7.0.0: Values of APISite.allpages() parameter filterredir other than True, False and None are deprecated
 * 7.0.0: The i18n identifier 'cosmetic_changes-append' will be removed in favour of 'pywikibot-cosmetic-changes'
 * 6.5.0: OutputOption.output() method will be removed in favour of OutputOption.out property
 * 6.5.0: Infinite rotating file handler with logfilecount of -1 is deprecated
 * 6.4.0: 'allow_duplicates' parameter of tools.itertools.intersect_generatorsas positional argument is deprecated, use keyword argument instead
```

### Comparing `pywikibot-8.1.2/README.rst` & `pywikibot-8.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 `MediaWiki API <https://www.mediawiki.org/wiki/API:Main_page>`_
 version 1.27 or higher.
 
 Also included are various general function scripts that can be adapted for
 different tasks.
 
 For further information about the library excluding scripts see
-the full `code documentation <https://doc.wikimedia.org/pywikibot/>`_.
+the full `code documentation <https://doc.wikimedia.org/pywikibot/stable/>`_.
 
 Quick start
 ===========
 
 .. code:: text
 
     pip install requests
```

### Comparing `pywikibot-8.1.2/pywikibot/__init__.py` & `pywikibot-8.2.0/pywikibot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     log,
     output,
     stdout,
     warning,
 )
 from pywikibot.site import APISite, BaseSite, DataSite
 from pywikibot.time import Timestamp
-from pywikibot.tools import normalize_username
+from pywikibot.tools import normalize_username, remove_last_args
 
 
 ItemPageStrNoneType = Union[str, 'ItemPage', None]
 ToDecimalType = Union[int, float, str, 'Decimal', None]
 
 __all__ = (
     '__copyright__', '__description__', '__download_url__', '__license__',
@@ -144,16 +144,15 @@
 
     @property
     def entity(self) -> str:
         """Return the entity uri of the globe."""
         if not self._entity:
             if self.globe not in self.site.globes():
                 raise exceptions.CoordinateGlobeUnknownError(
-                    '{} is not supported in Wikibase yet.'
-                    .format(self.globe))
+                    f'{self.globe} is not supported in Wikibase yet.')
             return self.site.globes()[self.globe]
 
         if isinstance(self._entity, ItemPage):
             return self._entity.concept_uri()
 
         return self._entity
 
@@ -431,16 +430,15 @@
         self.after = after
         self.before = before
         self.timezone = timezone
         if calendarmodel is None:
             if site is None:
                 site = Site().data_repository()
                 if site is None:
-                    raise ValueError('Site {} has no data repository'
-                                     .format(Site()))
+                    raise ValueError(f'Site {Site()} has no data repository')
             calendarmodel = site.calendarmodel()
         self.calendarmodel = calendarmodel
         # if precision is given it overwrites the autodetection above
         if precision is not None:
             if (isinstance(precision, int)
                     and precision in self.PRECISION.values()):
                 self.precision = precision
@@ -676,32 +674,30 @@
             kwargs['hour'] = self.hour
         if self.precision >= self.PRECISION['minute']:
             kwargs['minute'] = self.minute
         if self.precision >= self.PRECISION['second']:
             kwargs['second'] = self.second
         return type(self)(**kwargs)
 
-    def toTimestr(self, force_iso: bool = False,
-                  normalize: bool = False) -> str:
+    @remove_last_args(['normalize'])  # since 8.2.0
+    def toTimestr(self, force_iso: bool = False) -> str:
         """Convert the data to a UTC date/time string.
 
         .. seealso:: :meth:`fromTimestr` for differences between output
            with and without *force_iso* parameter.
 
         .. versionchanged:: 8.0
            *normalize* parameter was added.
+        .. versionchanged:: 8.2
+           *normalize* parameter was removed due to :phab:`T340495` and
+           :phab:`57755`
 
         :param force_iso: whether the output should be forced to ISO 8601
-        :param normalize: whether the output should be normalized (see
-            :meth:`normalize` for details)
         :return: Timestamp in a format resembling ISO 8601
         """
-        if normalize:
-            return self.normalize().toTimestr(force_iso=force_iso,
-                                              normalize=False)
         if force_iso:
             return Timestamp._ISO8601Format_new.format(
                 self.year, max(1, self.month), max(1, self.day),
                 self.hour, self.minute, self.second)
         return self.FORMATSTR.format(self.year, self.month, self.day,
                                      self.hour, self.minute, self.second)
 
@@ -722,25 +718,27 @@
         ts = Timestamp.fromISOformat(
             self.toTimestr(force_iso=True).lstrip('+'))
         if timezone_aware:
             ts = ts.replace(tzinfo=datetime.timezone(
                 datetime.timedelta(minutes=self.timezone)))
         return ts
 
-    def toWikibase(self, normalize: bool = False) -> Dict[str, Any]:
+    @remove_last_args(['normalize'])  # since 8.2.0
+    def toWikibase(self) -> Dict[str, Any]:
         """Convert the data to a JSON object for the Wikibase API.
 
         .. versionchanged:: 8.0
            *normalize* parameter was added.
+        .. versionchanged:: 8.2
+           *normalize* parameter was removed due to :phab:`T340495` and
+           :phab:`57755`
 
-        :param normalize: Whether to normalize the WbTime object before
-            converting it to a JSON object (see :func:`normalize` for details)
         :return: Wikibase JSON
         """
-        json = {'time': self.toTimestr(normalize=normalize),
+        json = {'time': self.toTimestr(),
                 'precision': self.precision,
                 'after': self.after,
                 'before': self.before,
                 'timezone': self.timezone,
                 'calendarmodel': self.calendarmodel
                 }
         return json
@@ -1010,17 +1008,16 @@
         :param data_site: The site serving as a repository for the given
             data type.
         :param ending: Required filetype-like ending in page titles.
             E.g. '.map'
         :param label: Label describing the data type in error messages.
         """
         if not isinstance(page, Page):
-            raise ValueError(
-                'Page {} must be a pywikibot.Page object not a {}.'
-                .format(page, type(page)))
+            raise ValueError(f'Page {page} must be a pywikibot.Page object '
+                             f'not a {type(page)}.')
 
         # validate page exists
         if not page.exists():
             raise ValueError(f'Page {page} must exist.')
 
         # validate page is on the right site, and that site supports the type
         if not data_site:
@@ -1300,16 +1297,15 @@
             with suppress(exceptions.UnknownFamilyError):
                 fam = Family.load(code)
         # Fallback to config defaults
         code = code or _config.mylang
         fam = fam or _config.family
 
     if not (code and fam):
-        raise ValueError('Missing Site {}'
-                         .format('code' if not code else 'family'))
+        raise ValueError(f"Missing Site {'code' if not code else 'family'}")
 
     if not isinstance(fam, Family):
         fam = Family.load(fam)
 
     interface = interface or fam.interface(code)
 
     # config.usernames is initialised with a defaultdict for each family name
@@ -1333,16 +1329,15 @@
     if not issubclass(interface, BaseSite):
         warning(f'Site called with interface={interface.__name__}')
 
     user = normalize_username(user)
     key = f'{interface.__name__}:{fam}:{code}:{user}'
     if key not in _sites or not isinstance(_sites[key], interface):
         _sites[key] = interface(code=code, fam=fam, user=user)
-        debug("Instantiated {} object '{}'"
-              .format(interface.__name__, _sites[key]))
+        debug(f"Instantiated {interface.__name__} object '{_sites[key]}'")
 
         if _sites[key].code != code:
             warn('Site {} instantiated using different code "{}"'
                  .format(_sites[key], code), UserWarning, 2)
 
     return _sites[key]
```

### Comparing `pywikibot-8.1.2/pywikibot/__metadata__.py` & `pywikibot-8.2.0/pywikibot/__metadata__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Distributed under the terms of the MIT license.
 #
 from time import strftime
 
 
 __name__ = 'pywikibot'
-__version__ = '8.1.2'
+__version__ = '8.2.0'
 __description__ = 'Python MediaWiki Bot Framework'
 __maintainer__ = 'The Pywikibot team'
 __maintainer_email__ = 'pywikibot@lists.wikimedia.org'
 __license__ = 'MIT License'
 __url__ = 'https://www.mediawiki.org/wiki/Manual:Pywikibot'
 __download_url__ = 'https://pywikibot.toolforge.org/'
 __copyright__ = '(C) Pywikibot team, 2003-' + strftime('%Y')
```

### Comparing `pywikibot-8.1.2/pywikibot/_wbtypes.py` & `pywikibot-8.2.0/pywikibot/_wbtypes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/backports.py` & `pywikibot-8.2.0/pywikibot/backports.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """This module contains backports to support older Python versions."""
 #
-# (C) Pywikibot team, 2014-2022
+# (C) Pywikibot team, 2014-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import sys
 from typing import Any
 
 
@@ -160,7 +160,47 @@
         .. versionadded:: 7.6
         """
         a, b = tee(iterable)
         next(b, None)
         return zip(a, b)
 else:
     from itertools import pairwise
+
+
+# gh-98363
+if PYTHON_VERSION < (3, 12) or SPHINX_RUNNING:
+    def batched(iterable, n: int) -> Generator[tuple, None, None]:
+        """Batch data from the *iterable* into tuples of length *n*.
+
+        .. note:: The last batch may be shorter than *n*.
+
+        Example:
+
+        >>> i = batched(range(25), 10)
+        >>> print(next(i))
+        (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)
+        >>> print(next(i))
+        (10, 11, 12, 13, 14, 15, 16, 17, 18, 19)
+        >>> print(next(i))
+        (20, 21, 22, 23, 24)
+        >>> print(next(i))
+        Traceback (most recent call last):
+         ...
+        StopIteration
+
+        .. seealso:: :python:`itertools.batched
+           <library/itertools.html#itertools.batched>`,
+           backported from Python 3.12.
+        .. versionadded:: 8.2
+
+        :param n: How many items of the iterable to get in one chunk
+        """
+        group = []
+        for item in iterable:
+            group.append(item)
+            if len(group) == n:
+                yield tuple(group)
+                group.clear()
+        if group:
+            yield tuple(group)
+else:
+    from itertools import batched
```

### Comparing `pywikibot-8.1.2/pywikibot/bot.py` & `pywikibot-8.2.0/pywikibot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 whether they exist.
 
 Additionally there is the :py:obj:`AutomaticTWSummaryBot` which subclasses
 :py:obj:`CurrentPageBot` and automatically defines the summary when
 ``put_current`` is used.
 """
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 __all__ = (
     'CRITICAL', 'ERROR', 'INFO', 'WARNING', 'DEBUG', 'INPUT', 'STDOUT',
     'VERBOSE', 'critical', 'debug', 'error', 'exception', 'log', 'warning',
     'output', 'stdout', 'LoggingFormatter',
@@ -171,15 +171,14 @@
     output,
     stdout,
     warning,
 )
 from pywikibot.throttle import Throttle
 from pywikibot.tools import (
     PYTHON_VERSION,
-    deprecated,
     issue_deprecation_warning,
     strtobool,
 )
 from pywikibot.tools._logging import LoggingFormatter
 
 
 if TYPE_CHECKING:
@@ -417,16 +416,16 @@
         pid = str(pid_int) + '-' if pid_int > 1 else ''
 
         if config.logfilename:
             # keep config.logfilename unchanged
             logfile = config.datafilepath('logs', config.logfilename)
         else:
             # add PID to logfle name
-            logfile = config.datafilepath('logs', '{}-{}bot.log'
-                                          .format(module_name, pid))
+            logfile = config.datafilepath('logs',
+                                          f'{module_name}-{pid}bot.log')
 
         # give up infinite rotating file handler with logfilecount of -1;
         # set it to 999 and use the standard implementation
         max_count = config.logfilecount
         if max_count == -1:  # pragma: no cover
             max_count = 999
             issue_deprecation_warning('config.logfilecount with value -1',
@@ -470,16 +469,16 @@
 def writelogheader() -> None:
     """
     Save additional version, system and status info to the log file in use.
 
     This may help the user to track errors or report bugs.
     """
     log('')
-    log('=== Pywikibot framework v{} -- Logging header ==='
-        .format(pywikibot.__version__))
+    log(f'=== Pywikibot framework v{pywikibot.__version__} -- Logging header'
+        ' ===')
 
     # script call
     log(f'COMMAND: {sys.argv}')
 
     # script call time stamp
     log(f'DATE: {datetime.datetime.utcnow()} UTC')
 
@@ -508,15 +507,15 @@
         check_package_list += sys.modules
 
     log('PACKAGES:')
     packages = version.package_versions(check_package_list)
     for name in sorted(packages.keys()):
         info = packages[name]
         info.setdefault('path',
-                        '[{}]'.format(info.get('type', 'path unknown')))
+                        f"[{info.get('type', 'path unknown')}]")
         info.setdefault('ver', '??')
         if 'err' in info:
             log('  {name}: {err}'.format_map(info))
         else:
             log('  {name} ({path}) = {ver}'.format_map(info))
 
     # imported modules
@@ -794,20 +793,19 @@
         question = 'Should the link '
         if self.context > 0:
             rng = self.current_range
             text = self.current_text
             # at the beginning of the link, start red color.
             # at the end of the link, reset the color to default
             pywikibot.info(text[max(0, rng[0] - self.context): rng[0]]
-                           + '<<lightred>>{}<<default>>'.format(
-                               text[rng[0]: rng[1]])
+                           + f'<<lightred>>{text[rng[0]:rng[1]]}<<default>>'
                            + text[rng[1]: rng[1] + self.context])
         else:
-            question += '<<lightred>>{}<<default>> '.format(
-                self._old.canonical_title())
+            question += (
+                f'<<lightred>>{self._old.canonical_title()}<<default>> ')
 
         if self._new is False:
             question += 'be unlinked?'
         else:
             question += 'target to <<lightpurple>>{}<<default>>?'.format(
                 self._new.canonical_title())
 
@@ -944,16 +942,16 @@
                 config.logfilename = value
         elif option == '-nolog':
             commandlog = False
             config.log = []
         elif option in ('-cosmeticchanges', '-cc'):
             config.cosmetic_changes = (strtobool(value) if value
                                        else not config.cosmetic_changes)
-            output('NOTE: option cosmetic_changes is {}\n'
-                   .format(config.cosmetic_changes))
+            output(f'NOTE: option cosmetic_changes is '
+                   f'{config.cosmetic_changes}\n')
         elif option == '-simulate':
             config.simulate = value or True
         #
         #  DEBUG control:
         #
         #    The framework has four layers (by default, others can be added),
         #    each designated by a string --
@@ -1155,16 +1153,15 @@
     """
 
     def __init__(self, classname: str, options: Dict[str, Any]) -> None:
         self._classname = classname
         super().__init__(options)
 
     def __missing__(self, key: str) -> None:
-        raise Error("'{}' is not a valid option for {}."
-                    .format(key, self._classname))
+        raise Error(f"'{key}' is not a valid option for {self._classname}.")
 
     def __getattr__(self, name: str) -> Any:
         """Get item from dict."""
         return self.__getitem__(name)
 
     def __setattr__(self, name: str, value: Any) -> None:
         """Set item or attribute."""
@@ -1239,16 +1236,15 @@
 
         # self.opt contains all available options including defaults
         self.opt = _OptionDict(self.__class__.__name__, self.available_options)
         # update the options overridden from defaults
         self.opt.update((opt, options[opt])
                         for opt in received_options & valid_options)
         for opt in received_options - valid_options:
-            pywikibot.warning('{} is not a valid option. It was ignored.'
-                              .format(opt))
+            pywikibot.warning(f'{opt} is not a valid option. It was ignored.')
 
 
 class BaseBot(OptionHandler):
 
     """Generic Bot to be subclassed.
 
     Only accepts `generator` and options defined in
@@ -1360,44 +1356,14 @@
            renamed to `generator_completed` to become a public attribute.
         """
 
         #: instance variable to hold the default page type
         self.treat_page_type: Any = pywikibot.page.BasePage
 
     @property
-    @deprecated("self.counter['read']", since='7.0.0')
-    def _treat_counter(self):
-        return self.counter['read']
-
-    @_treat_counter.setter
-    @deprecated("self.counter['read']", since='7.0.0')
-    def _treat_counter(self, value) -> None:
-        self.counter['read'] = value
-
-    @property
-    @deprecated("self.counter['write']", since='7.0.0')
-    def _save_counter(self):
-        return self.counter['write']
-
-    @_save_counter.setter
-    @deprecated("self.counter['write']", since='7.0.0')
-    def _save_counter(self, value) -> None:
-        self.counter['write'] = value
-
-    @property
-    @deprecated("self.counter['skip']", since='7.0.0')
-    def _skip_counter(self):
-        return self.counter['skip']
-
-    @_skip_counter.setter
-    @deprecated("self.counter['skip']", since='7.0.0')
-    def _skip_counter(self, value) -> None:
-        self.counter['skip'] = value
-
-    @property
     def current_page(self) -> 'pywikibot.page.BasePage':
         """Return the current working page as a property."""
         assert self._current_page is not None
         return self._current_page
 
     @current_page.setter
     def current_page(self, page: 'pywikibot.page.BasePage') -> None:
@@ -1412,16 +1378,15 @@
         :param page: the working page
         """
         if page != self._current_page:
             self._current_page = page
             msg = f'Working on {page.title()!r}'
             if config.colorized_output:
                 log(msg)
-                stdout('\n\n>>> <<lightpurple>>{}<<default>> <<<'
-                       .format(page.title()))
+                stdout(f'\n\n>>> <<lightpurple>>{page.title()}<<default>> <<<')
             else:
                 stdout(msg)
 
     def user_confirm(self, question: str) -> bool:
         """Obtain user response if bot option 'always' not enabled."""
         if self.opt.always:
             return True
@@ -1472,15 +1437,15 @@
         self.current_page = page
 
         show_diff = kwargs.pop('show_diff', True)
         if show_diff:
             pywikibot.showDiff(oldtext, newtext)
 
         if 'summary' in kwargs:
-            pywikibot.info('Edit summary: {}'.format(kwargs['summary']))
+            pywikibot.info(f"Edit summary: {kwargs['summary']}")
 
         page.text = newtext
         return self._save_page(page, page.save, **kwargs)
 
     def _save_page(self, page: 'pywikibot.page.BasePage',
                    func: Callable[..., Any], *args: Any,
                    **kwargs: Any) -> bool:
@@ -1516,30 +1481,29 @@
         try:
             func(*args, **kwargs)
             self.counter['write'] += 1
         except PageSaveRelatedError as e:
             if not ignore_save_related_errors:
                 raise
             if isinstance(e, EditConflictError):
-                pywikibot.info('Skipping {} because of edit conflict'
-                               .format(page.title()))
+                pywikibot.info(
+                    f'Skipping {page.title()} because of edit conflict')
             elif isinstance(e, SpamblacklistError):
                 pywikibot.info('Cannot change {} because of blacklist '
                                'entry {}'.format(page.title(), e.url))
             elif isinstance(e, LockedPageError):
-                pywikibot.info('Skipping {} (locked page)'
-                               .format(page.title()))
+                pywikibot.info(f'Skipping {page.title()} (locked page)')
             else:
                 pywikibot.error('Skipping {} because of a save related '
                                 'error: {}'.format(page.title(), e))
         except ServerError as e:
             if not ignore_server_errors:
                 raise
-            pywikibot.error('Server Error while processing {}: {}'
-                            .format(page.title(), e))
+            pywikibot.error(
+                f'Server Error while processing {page.title()}: {e}')
         else:
             return True
         return False
 
     def quit(self) -> None:
         """Cleanup and quit processing."""
         raise QuitKeyboardInterrupt
@@ -1563,16 +1527,15 @@
             read_seconds = int(read_delta.total_seconds())
 
         # wait until pending threads finished but don't close the queue
         pywikibot.stopme()
 
         pywikibot.info()
         for op, count in self.counter.items():
-            pywikibot.info('{} {} operation{}'
-                           .format(count, op, 's' if count > 1 else ''))
+            pywikibot.info(f"{count} {op} operation{'s' if count > 1 else ''}")
 
         if hasattr(self, '_start_ts'):
             write_delta = pywikibot.Timestamp.now() - self._start_ts
             write_seconds = int(write_delta.total_seconds())
             if write_delta.days:
                 pywikibot.info(
                     'Execution time: {d.days} days, {d.seconds} seconds'
@@ -1705,16 +1668,15 @@
 
                 # Process the page
                 self.counter['read'] += 1
                 self.treat(page)
 
             self.generator_completed = True
         except QuitKeyboardInterrupt:
-            pywikibot.info('\nUser quit {} bot run...'
-                           .format(self.__class__.__name__))
+            pywikibot.info(f'\nUser quit {self.__class__.__name__} bot run...')
         except KeyboardInterrupt:
             if config.verbose_output:
                 raise
 
             pywikibot.info('\nKeyboardInterrupt during {} bot run...'
                            .format(self.__class__.__name__))
         finally:
@@ -1844,16 +1806,16 @@
         if self._site:
             # Warn in any case where the site is (probably) changed after
             # setting it the first time. The appropriate variant is not to use
             # self.site at all or define it once and never change it again
             if self._site == value:
                 pywikibot.warning('Defined site without changing it.')
             else:
-                pywikibot.warning('Changed the site from "{}" to '
-                                  '"{}"'.format(self._site, value))
+                pywikibot.warning(
+                    f'Changed the site from "{self._site}" to "{value}"')
         self._site = value
 
     def init_page(self, item: Any) -> 'pywikibot.page.BasePage':
         """Set site if not defined."""
         page = super().init_page(item)
         if not self._site:
             self.site = page.site
@@ -2233,15 +2195,15 @@
             if data is None:
                 diff = entity.toJSON(diffto=getattr(entity, '_content', None))
             else:
                 diff = entity._normalizeData(data)
             pywikibot.info(json.dumps(diff, indent=4, sort_keys=True))
 
         if 'summary' in kwargs:
-            pywikibot.info('Change summary: {}'.format(kwargs['summary']))
+            pywikibot.info(f"Change summary: {kwargs['summary']}")
 
         # TODO PageSaveRelatedErrors should be actually raised in editEntity
         # (bug T86083)
         return self._save_page(
             entity, entity.editEntity, data,
             ignore_save_related_errors=ignore_save_related_errors,
             ignore_server_errors=ignore_server_errors, **kwargs)
@@ -2272,16 +2234,15 @@
         self.current_page = item
 
         if source:
             sourceclaim = self.getSource(source)
             if sourceclaim:
                 claim.addSource(sourceclaim)
 
-        pywikibot.info('Adding {} --> {}'.format(claim.getID(),
-                                                 claim.getTarget()))
+        pywikibot.info(f'Adding {claim.getID()} --> {claim.getTarget()}')
         return self._save_page(item, item.addClaim, claim, bot=bot, **kwargs)
 
     def getSource(self, site: 'BaseSite') -> Optional['pywikibot.page.Claim']:
         """
         Create a Claim usable as a source for Wikibase statements.
 
         :param site: site that is the source of assertions.
```

### Comparing `pywikibot-8.1.2/pywikibot/bot_choice.py` & `pywikibot-8.2.0/pywikibot/bot_choice.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         :return: Text with the options formatted into it
         """
         formatted_options = []
         for option in options:
             formatted_options.append(option.format(default=default))
         # remove color highlights before fill function
-        text = '{} ({})'.format(text, ', '.join(formatted_options))
+        text = f"{text} ({', '.join(formatted_options)})"
         pattern = '<<[a-z]+>>'
         highlights = re.findall(pattern, text)
         return fill(re.sub(pattern, '{}', text), width=77).format(*highlights)
 
     @property
     def stop(self) -> bool:
         """Return whether this option stops asking."""
```

### Comparing `pywikibot-8.1.2/pywikibot/comms/eventstreams.py` & `pywikibot-8.2.0/pywikibot/comms/eventstreams.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 This module requires sseclient to be installed::
 
     pip install "sseclient<0.0.23,>=0.0.18"
 
 .. versionadded:: 3.0
 """
 #
-# (C) Pywikibot team, 2017-2022
+# (C) Pywikibot team, 2017-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import json
 from functools import partial
 from typing import Optional
 
@@ -139,15 +139,18 @@
            parameter.
         """
         if isinstance(EventSource, Exception):
             raise ImportError('sseclient is required for EventStreams;\n'
                               'install it with "pip install sseclient"\n')
         self.filter = {'all': [], 'any': [], 'none': []}
         self._total = None
-        self._site = kwargs.pop('site', Site())
+        try:
+            self._site = kwargs.pop('site')
+        except KeyError:  # T335720
+            self._site = Site()
 
         self._streams = kwargs.pop('streams', None)
         if self._streams and not isinstance(self._streams, str):
             self._streams = ','.join(self._streams)
 
         self._since = kwargs.pop('since', None)
         if self._since:
@@ -331,27 +334,26 @@
                     warning(
                         'You may not have the right sseclient version;\n'
                         'sseclient >= 0.0.18 is required for eventstreams.\n'
                         "Install it with 'pip install \"sseclient>=0.0.18\"'")
             try:
                 event = next(self.source)
             except (ProtocolError, OSError, httplib.IncompleteRead) as e:
-                warning('Connection error: {}.\n'
-                        'Try to re-establish connection.'.format(e))
+                warning(
+                    f'Connection error: {e}.\nTry to re-establish connection.')
                 del self.source
                 if event is not None:
                     self.sse_kwargs['last_id'] = event.id
                 continue
             if event.event == 'message':
                 if event.data:
                     try:
                         element = json.loads(event.data)
                     except ValueError as e:
-                        warning('Could not load json data from\n{}\n{}'
-                                .format(event, e))
+                        warning(f'Could not load json data from\n{event}\n{e}')
                     else:
                         if self.streamfilter(element):
                             n += 1
                             yield element
                 elif not ignore_first_empty_warning:
                     warning('Empty message found.')
                 else:
```

### Comparing `pywikibot-8.1.2/pywikibot/comms/http.py` & `pywikibot-8.2.0/pywikibot/comms/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,44 +245,47 @@
         from fake_useragent import UserAgent
     except ImportError:
         raise ImportError(  # Actually complain when fake_useragent is missing.
             'fake_useragent must be installed to get fake UAs.')
     return UserAgent().random
 
 
-def request(site,
+def request(site: 'pywikibot.site.BaseSite',
             uri: Optional[str] = None,
             headers: Optional[dict] = None,
             **kwargs) -> requests.Response:
     """
     Request to Site with default error handling and response decoding.
 
     See :py:obj:`requests.Session.request` for additional parameters.
 
     The optional uri is a relative uri from site base uri including the
     document root '/'.
 
+    .. versionchanged:: 8.2
+       a *protocol* parameter can be given which is passed to the
+       :meth:`family.Family.base_url` method.
+
     :param site: The Site to connect to
-    :type site: pywikibot.site.BaseSite
     :param uri: the URI to retrieve
-    :keyword charset: Either a valid charset (usable for str.decode()) or None
-        to automatically chose the charset from the returned header (defaults
-        to latin-1)
-    :type charset: CodecInfo, str, None
+    :keyword Optional[CodecInfo, str] charset: Either a valid charset
+        (usable for str.decode()) or None to automatically chose the
+        charset from the returned header (defaults to latin-1)
+    :keyword Optional[str] protocol: a url scheme
     :return: The received data Response
     """
     kwargs.setdefault('verify', site.verify_SSL_certificate())
     if not headers:
         headers = {}
         format_string = None
     else:
         format_string = headers.get('user-agent')
     headers['user-agent'] = user_agent(site, format_string)
 
-    baseuri = site.base_url(uri)
+    baseuri = site.base_url(uri, protocol=kwargs.pop('protocol', None))
     r = fetch(baseuri, headers=headers, **kwargs)
     site.throttle.retry_after = int(r.headers.get('retry-after', 0))
     return r
 
 
 def get_authentication(uri: str) -> Optional[Tuple[str, str]]:
     """
@@ -318,30 +321,39 @@
     # TODO: do some error correcting stuff
     if isinstance(response, requests.exceptions.SSLError) \
        and 'certificate verify failed' in str(response):
         raise FatalServerError(str(response))
 
     if isinstance(response, requests.ConnectionError):
         msg = str(response)
-        if 'NewConnectionError' in msg \
+        if ('NewConnectionError' in msg or 'NameResolutionError' in msg) \
            and re.search(r'\[Errno (-2|8|11001)\]', msg):
             raise ConnectionError(response)
 
+    # catch requests.ReadTimeout and requests.ConnectTimeout and convert
+    # it to ServerError
+    if isinstance(response, requests.Timeout):
+        raise ServerError(response)
+
+    if isinstance(response, ValueError):
+        # MissingSchema, InvalidSchema, InvalidURL, InvalidHeader
+        raise FatalServerError(str(response))
+
     if isinstance(response, Exception):
         with suppress(Exception):
             # request exception may contain response and request attribute
             error('An error occurred for uri ' + response.request.url)
         raise response from None
 
     if response.status_code == HTTPStatus.REQUEST_URI_TOO_LONG:
         raise Client414Error(HTTPStatus(response.status_code).description)
 
     if response.status_code == HTTPStatus.GATEWAY_TIMEOUT:
-        raise Server504Error('Server {} timed out'
-                             .format(urlparse(response.url).netloc))
+        raise Server504Error(
+            f'Server {urlparse(response.url).netloc} timed out')
 
     if (not response.ok
             and response.status_code >= HTTPStatus.INTERNAL_SERVER_ERROR):
         raise ServerError(
             f'{response.status_code} Server Error: {response.reason}')
 
     # TODO: shall it raise? this might break some code, TBC
@@ -420,16 +432,15 @@
 
     charset = kwargs.pop('charset', None)
 
     auth = get_authentication(uri)
     if auth is not None and len(auth) == 4:
         if isinstance(requests_oauthlib, ImportError):
             warn(str(requests_oauthlib), ImportWarning)
-            error('OAuth authentication not supported: {}'
-                  .format(requests_oauthlib))
+            error(f'OAuth authentication not supported: {requests_oauthlib}')
             auth = None
         else:
             auth = requests_oauthlib.OAuth1(*auth)
 
     timeout = config.socket_timeout
 
     try:
@@ -516,16 +527,15 @@
         """Helper function to try decoding."""
         if encoding is None:
             return None
 
         try:
             content.decode(encoding)
         except LookupError:
-            pywikibot.warning('Unknown or invalid encoding {!r}'
-                              .format(encoding))
+            pywikibot.warning(f'Unknown or invalid encoding {encoding!r}')
         except UnicodeDecodeError as e:
             pywikibot.warning(f'{e} found in {content}')
         else:
             return encoding
 
         return None  # let chardet do the job
```

### Comparing `pywikibot-8.1.2/pywikibot/config.py` & `pywikibot-8.2.0/pywikibot/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 .. versionchanged:: 6.2
    config2 was renamed to config
 .. versionchanged:: 8.0
    Editor settings has been revised. *editor* variable is None by
    default. Editor detection functions were moved to :mod:`editor`.
 """
 #
-# (C) Pywikibot team, 2003-2022
+# (C) Pywikibot team, 2003-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import collections
 import copy
 import os
 import platform
@@ -365,16 +365,16 @@
             if OSWIN32:
                 win_version = int(platform.version().split('.')[0])
                 if win_version == 5:
                     sub_dir = ['Application Data']
                 elif win_version in (6, 10):
                     sub_dir = ['AppData', 'Roaming']
                 else:
-                    raise OSError('Windows version {} not supported yet.'
-                                  .format(win_version))
+                    raise OSError(
+                        f'Windows version {win_version} not supported yet.')
                 base_dir_cand.extend([[home] + sub_dir + ['Pywikibot'],
                                      [home] + sub_dir + ['pywikibot']])
             else:
                 base_dir_cand.append([home, '.pywikibot'])
 
             for dir_ in base_dir_cand:
                 dir_s = os.path.join(*dir_)
@@ -448,16 +448,16 @@
     :raises NotADirectoryError: folder_path is not a directory
     """
     suffix = '_family.py'
 
     if not os.path.exists(folder_path):
         if not_exists_ok:
             return
-        raise FileNotFoundError('Family folder {!r} does not exist'
-                                .format(folder_path))
+        raise FileNotFoundError(
+            f'Family folder {folder_path!r} does not exist')
 
     if os.path.isdir(folder_path):
         for file_name in os.listdir(folder_path):
             if file_name.endswith(suffix):
                 family_name = removesuffix(file_name, suffix)
                 family_files[family_name] = os.path.join(folder_path,
                                                          file_name)
@@ -799,15 +799,16 @@
 db_port = 3306
 
 # ############# HTTP SETTINGS ##############
 # Default socket timeout in seconds.
 # DO NOT set to None to disable timeouts. Otherwise this may freeze your
 # script.
 # You may assign either a tuple of two int or float values for connection and
-# read timeout, or a single value for both in a tuple.
+# read timeout, or a single value for both.
+# See also: https://requests.readthedocs.io/en/stable/user/advanced/#timeouts
 socket_timeout = (6.05, 45)
 
 
 # ############# COSMETIC CHANGES SETTINGS ##############
 # The bot can make some additional changes to each page it edits, e.g. fix
 # whitespace or positioning of category links.
```

### Comparing `pywikibot-8.1.2/pywikibot/cosmetic_changes.py` & `pywikibot-8.2.0/pywikibot/cosmetic_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 or by adding a list to the given one::
 
     cosmetic_changes_deny_script += ['your_script_name_1',
                                      'your_script_name_2']
 """
 #
-# (C) Pywikibot team, 2006-2022
+# (C) Pywikibot team, 2006-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import re
 from contextlib import suppress
 from enum import IntEnum
 from typing import Any, Union
@@ -64,15 +64,15 @@
 import pywikibot
 from pywikibot import textlib
 from pywikibot.backports import Callable, Dict, List, Match, Pattern
 from pywikibot.exceptions import InvalidTitleError
 from pywikibot.textlib import (
     FILE_LINK_REGEX,
     MultiTemplateMatchBuilder,
-    _get_regexes,
+    get_regexes,
 )
 from pywikibot.tools import first_lower, first_upper
 from pywikibot.tools.chars import url2string
 
 
 try:
     import stdnum.isbn as stdnum_isbn
@@ -663,30 +663,30 @@
             160,    # Non-breaking space (&nbsp;)
                     # - not supported by Firefox textareas
             173,    # Soft-hypen (&shy;) - enable editing
             8206,   # Left-to-right mark (&ltr;)
             8207,   # Right-to-left mark (&rtl;)
         ]
         if self.template:
-            ignore += [32]  # Space ( )
-            ignore += [58]  # Colon (:)
+            ignore.append(32)  # Space ( )
+            ignore.append(58)  # Colon (:)
         # TODO: T254350 - what other extension tags should be avoided?
         # (graph, math, score, timeline, etc.)
         text = pywikibot.html2unicode(
             text, ignore=ignore, exceptions=['comment', 'syntaxhighlight'])
         return text
 
     def removeEmptySections(self, text: str) -> str:
         """Cleanup empty sections."""
         # userspace contains article stubs without nobots/in use templates
         if self.namespace == 2:
             return text
 
         skippings = ['comment', 'category']
-        skip_regexes = _get_regexes(skippings, self.site)
+        skip_regexes = get_regexes(skippings, self.site)
         # site defined templates
         skip_templates = {
             'cs': ('Pahýl[ _]část',),  # stub section
         }
         if self.site.code in skip_templates:
             for template in skip_templates[self.site.code]:
                 skip_regexes.append(
@@ -695,31 +695,29 @@
         skip_regexes.append(re.compile(r'(?m)^[\*#] *$'))
 
         # get stripped sections
         stripped_text = textlib.removeLanguageLinks(text, self.site, '\n')
         for reg in skip_regexes:
             stripped_text = reg.sub(r'', stripped_text)
         strip_sections = textlib.extract_sections(
-            stripped_text, self.site)[1]
+            stripped_text, self.site).sections
 
         # get proper sections
         header, sections, footer = textlib.extract_sections(text, self.site)
 
         # iterate stripped sections and create a new page body
         new_body = []
         for i, strip_section in enumerate(strip_sections):
-            current_heading = sections[i][0]
+            current_dep = sections[i].level
             try:
-                next_heading = sections[i + 1][0]
+                next_dep = sections[i + 1].level
             except IndexError:
-                next_heading = ''
-            current_dep = (len(current_heading)
-                           - len(current_heading.lstrip('=')))
-            next_dep = len(next_heading) - len(next_heading.lstrip('='))
-            if strip_section[1].strip() or current_dep < next_dep:
+                next_dep = 0
+
+            if strip_section.content.strip() or current_dep < next_dep:
                 new_body.extend(sections[i])
         return header + ''.join(new_body) + footer
 
     def removeUselessSpaces(self, text: str) -> str:
         """Cleanup multiple or trailing spaces."""
         exceptions = ['comment', 'math', 'nowiki', 'pre', 'syntaxhighlight',
                       'startspace', 'table']
```

### Comparing `pywikibot-8.1.2/pywikibot/daemonize.py` & `pywikibot-8.2.0/pywikibot/daemonize.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/data/api/__init__.py` & `pywikibot-8.2.0/pywikibot/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/data/api/_generators.py` & `pywikibot-8.2.0/pywikibot/data/api/_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 .. versionchanged:: 7.6
    All Objects were changed from Iterable object to a Generator object.
    They are subclassed from
    :class:`tools.collections.GeneratorWrapper`
 """
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from abc import ABC, abstractmethod
 from typing import Union
 from warnings import warn
 
@@ -153,21 +153,20 @@
         .. versionchanged:: 7.6
            changed from iterator method to generator property
         """
         offset = self.starting_offset
         n = 0
         while True:
             self.request[self.continue_name] = offset
-            pywikibot.debug('{}: Request: {}'
-                            .format(type(self).__name__, self.request))
+            pywikibot.debug(f'{type(self).__name__}: Request: {self.request}')
             data = self.request.submit()
 
             n_items = len(data[self.data_name])
-            pywikibot.debug('{}: Retrieved {} items'
-                            .format(type(self).__name__, n_items))
+            pywikibot.debug(
+                f'{type(self).__name__}: Retrieved {n_items} items')
             if n_items > 0:
                 for item in data[self.data_name]:
                     yield item
                     n += 1
                     if self.limit is not None and n >= self.limit:
                         pywikibot.debug('{}: Stopped iterating due to '
                                         'exceeding item limit.'
@@ -557,17 +556,16 @@
                 # this ensures that page data will be iterated
                 # in the same order as received from server
                 resultdata = [resultdata[k]
                               for k in self.data['query']['pageids']]
             else:
                 resultdata = [resultdata[k]
                               for k in sorted(resultdata)]
-        pywikibot.debug('{name} received {keys}; limit={limit}'
-                        .format(name=type(self).__name__, keys=keys,
-                                limit=self.limit))
+        pywikibot.debug(
+            f'{type(self).__name__} received {keys}; limit={self.limit}')
         return resultdata
 
     def _extract_results(self, resultdata):
         """Extract results from resultdata."""
         for item in resultdata:
             result = self.result(item)
             if self._namespaces and not self._check_result_namespace(result):
@@ -807,17 +805,16 @@
         """Update old result dict with new_dict."""
         for k, v in new_dict.items():
             if isinstance(v, (str, int)):
                 old_dict.setdefault(k, v)
             elif isinstance(v, list):
                 old_dict.setdefault(k, []).extend(v)
             else:
-                raise ValueError(
-                    'continued API result had an unexpected type: {}'
-                    .format(type(v).__name__))
+                raise ValueError(f'continued API result had an unexpected '
+                                 f'type: {type(v).__name__}')
 
 
 class ListGenerator(QueryGenerator):
 
     """Generator for queries of type action=query&list=foo.
 
     See the API documentation for types of lists that can be queried.
@@ -874,21 +871,19 @@
         page._pageid = int(pagedict['pageid'])
     elif 'missing' in pagedict:
         page._pageid = 0  # Non-existent page
     else:
         # Something is wrong.
         if page.site.sametitle(page.title(), pagedict['title']) \
            and 'invalid' in pagedict:
-            raise InvalidTitleError('{}: {}'
-                                    .format(page, pagedict['invalidreason']))
+            raise InvalidTitleError(f"{page}: {pagedict['invalidreason']}")
         if int(pagedict['ns']) < 0:
             raise UnsupportedPageError(page)
-        raise RuntimeError(
-            "Page {} has neither 'pageid' nor 'missing' attribute"
-            .format(pagedict['title']))
+        raise RuntimeError(f"Page {pagedict['title']} has neither 'pageid'"
+                           " nor 'missing' attribute")
 
 
 def _update_contentmodel(page, pagedict: dict) -> None:
     """Update page content model."""
     page._contentmodel = pagedict.get('contentmodel')  # can be None
 
     if (page._contentmodel
@@ -999,16 +994,15 @@
 
     if 'lastrevid' in pagedict:
         page.latest_revision_id = pagedict['lastrevid']
 
     if 'imageinfo' in pagedict:
         if not isinstance(page, pywikibot.FilePage):
             raise RuntimeError(
-                '"imageinfo" found but {} is not a FilePage object'
-                .format(page))
+                f'"imageinfo" found but {page} is not a FilePage object')
         page._load_file_revisions(pagedict['imageinfo'])
 
     if 'categoryinfo' in pagedict:
         page._catinfo = pagedict['categoryinfo']
 
     if 'templates' in pagedict:
         _update_templates(page, pagedict['templates'])
```

### Comparing `pywikibot-8.1.2/pywikibot/data/api/_optionset.py` & `pywikibot-8.2.0/pywikibot/data/api/_optionset.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,16 +109,15 @@
             if value is True:
                 enabled.add(name)
             elif value is False:
                 disabled.add(name)
             elif value is None:
                 removed.add(name)
             else:
-                raise ValueError('Dict contains invalid value "{}"'.format(
-                    value))
+                raise ValueError(f'Dict contains invalid value "{value}"')
         invalid_names = (
             (enabled - self._valid_enable) | (disabled - self._valid_disable)
             | (removed - self._valid_enable - self._valid_disable)
         )
         if invalid_names and self._site_set:
             raise ValueError('Dict contains invalid name(s) "{}"'.format(
                 '", "'.join(invalid_names)))
```

### Comparing `pywikibot-8.1.2/pywikibot/data/api/_paraminfo.py` & `pywikibot-8.2.0/pywikibot/data/api/_paraminfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Object representing API parameter information."""
 #
-# (C) Pywikibot team, 2014-2022
+# (C) Pywikibot team, 2014-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from collections.abc import Container, Sized
 from typing import Any, Optional, Union
 
 import pywikibot
 from pywikibot import config
-from pywikibot.backports import Dict, removeprefix
-from pywikibot.tools.itertools import itergroup
+from pywikibot.backports import Dict, batched, removeprefix
 
 
 __all__ = ['ParamInfo']
 
 
 class ParamInfo(Sized, Container):
 
@@ -192,20 +191,21 @@
         """
         Fetch paraminfo for multiple modules without initializing beforehand.
 
         :param modules: API modules to load and which haven't been loaded yet.
         """
         def module_generator():
             """A generator yielding batches of modules."""
-            i = itergroup(sorted(modules), self._limit)
-            for batch in i:
+            # T340617: self._limit is not set for the first modules
+            # which is frozenset({'paraminfo', 'query', 'main'})
+            for batch in batched(sorted(modules), self._limit or 50):
                 for failed_module in failed_modules:
                     yield [failed_module]
-                del failed_modules[:]
-                yield batch
+                failed_modules.clear()
+                yield list(batch)
 
         modules -= set(self._paraminfo)
         if not modules:
             return
 
         assert 'query' in self._modules or 'paraminfo' not in self._paraminfo
 
@@ -396,16 +396,16 @@
 
                 name = mod_data.get('name')
                 php_class = mod_data.get('classname')
 
                 if not name and php_class:
                     name = removeprefix(php_class, 'Api').lower()
                     if name not in ('main', 'pageset'):
-                        pywikibot.warning('Unknown paraminfo module "{}"'
-                                          .format(php_class))
+                        pywikibot.warning(
+                            f'Unknown paraminfo module "{php_class}"')
                         name = '<unknown>:' + php_class
 
                     mod_data['name'] = name
 
                 if 'path' not in mod_data:
                     # query modules often contain 'ApiQuery' and have a suffix.
                     # 'ApiQuery' alone is the action 'query'
@@ -417,16 +417,15 @@
                         mod_data['path'] = name
 
                 path = mod_data['path']
 
                 if path in result_data:
                     # Only warn first time
                     if result_data[path] is not False:
-                        pywikibot.warning('Path "{}" is ambiguous.'
-                                          .format(path))
+                        pywikibot.warning(f'Path "{path}" is ambiguous.')
                     else:
                         pywikibot.log(f'Found another path "{path}"')
                     result_data[path] = False
                 else:
                     result_data[path] = mod_data
 
         return result_data
@@ -495,17 +494,16 @@
         param_data = [param for param in params
                       if param['name'] == param_name]
 
         if not param_data:
             return None
 
         if len(param_data) != 1:
-            raise RuntimeError(
-                'parameter data length is eiter empty or not unique.\n{}'
-                .format(param_data))
+            raise RuntimeError(f'parameter data length is eiter empty or not '
+                               f'unique.\n{param_data}')
         return param_data[0]
 
     @property
     def module_paths(self):
         """Set of all modules using their paths."""
         return self._module_set(True)
```

### Comparing `pywikibot-8.1.2/pywikibot/data/api/_requests.py` & `pywikibot-8.2.0/pywikibot/data/api/_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import re
 import traceback
 from collections.abc import MutableMapping
 from contextlib import suppress
 from email.mime.nonmultipart import MIMENonMultipart
 from pathlib import Path
 from typing import Any, Optional, Union
-from urllib.parse import unquote, urlencode
+from urllib.parse import unquote, urlencode, urlparse
 from warnings import warn
 
 import pywikibot
 from pywikibot import config
 from pywikibot.backports import Callable, Dict, Match, Tuple, removeprefix
 from pywikibot.comms import http
 from pywikibot.exceptions import (
@@ -670,21 +670,31 @@
                         f'Headers: {headers!r}\nURI: {uri!r}\nBody: {body!r}')
         return use_get, uri, body, headers
 
     def _http_request(self, use_get: bool, uri: str, data, headers,
                       paramstring) -> tuple:
         """Get or post a http request with exception handling.
 
+        .. versionchanged:: 8.2
+           change the scheme if the previous request didn't have json
+           content.
+
         :return: a tuple containing requests.Response object from
             http.request and use_get value
         """
+        kwargs = {}
+        schemes = ('http', 'https')
+        if self.json_warning and self.site.protocol() in schemes:
+            # retry with other scheme
+            kwargs['protocol'] = schemes[self.site.protocol() == 'http']
+
         try:
             response = http.request(self.site, uri=uri,
                                     method='GET' if use_get else 'POST',
-                                    data=data, headers=headers)
+                                    data=data, headers=headers, **kwargs)
         except Server504Error:
             pywikibot.log('Caught HTTP 504 error; retrying')
         except Client414Error:
             if use_get:
                 pywikibot.log('Caught HTTP 414 error; retrying')
                 use_get = False
             else:
@@ -704,14 +714,18 @@
             return response, use_get
         self.wait()
         return None, use_get
 
     def _json_loads(self, response) -> Optional[dict]:
         """Return a dict from requests.Response.
 
+        .. versionchanged:: 8.2
+           show a warning to add a ``protocoll()`` method to the family
+           file if suitable.
+
         :param response: a requests.Response object
         :type response: requests.Response
         :return: a data dict
         :raises pywikibot.exceptions.APIError: unknown action found
         :raises pywikibot.exceptions.APIError: unknown query result type
         """
         try:
@@ -749,15 +763,26 @@
                 if param.endswith('limit'):
                     # param values are stored a list of str
                     value = self[param][0]
                     if value.isdigit():
                         self[param] = [str(int(value) // 2)]
                         pywikibot.info(f'Set {param} = {self[param]}')
         else:
+            scheme = urlparse(response.url).scheme
+            if self.json_warning and scheme != self.site.protocol():
+                warn(f"""
+Your {self.site.family} family uses a wrong scheme {self.site.protocol()!r}
+but {scheme!r} is required. Please add the following code to your family file:
+
+    def protocol(self, code: str) -> str:
+        return '{scheme}'
+
+""", stacklevel=2)
             return result or {}
+
         self.wait()
         return None
 
     def _relogin(self, message: str = '') -> None:
         """Force re-login and inform user."""
         message += ' Forcing re-login.'
         pywikibot.error(f'{message.strip()}')
```

### Comparing `pywikibot-8.1.2/pywikibot/data/memento.py` & `pywikibot-8.2.0/pywikibot/data/memento.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,16 +283,16 @@
             session_set = True
         try:
             response = session.head(uri,
                                     headers=headers,
                                     allow_redirects=follow_redirects,
                                     timeout=timeout or 9)
         except (InvalidSchema, MissingSchema):
-            raise ValueError('Only HTTP URIs are supported, '
-                             'URI {} unrecognized.'.format(uri))
+            raise ValueError(
+                f'Only HTTP URIs are supported, URI {uri} unrecognized.')
         if session_set:
             session.close()
 
         return response
 
 
 # Save old static methods and update static methods of parent class
```

### Comparing `pywikibot-8.1.2/pywikibot/data/mysql.py` & `pywikibot-8.2.0/pywikibot/data/mysql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/data/sparql.py` & `pywikibot-8.2.0/pywikibot/data/sparql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """SPARQL Query interface."""
 #
-# (C) Pywikibot team, 2016-2022
+# (C) Pywikibot team, 2016-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from contextlib import suppress
 from typing import Optional
 from urllib.parse import quote
 
@@ -63,16 +63,16 @@
             except NotImplementedError:
                 raise NotImplementedError(
                     'Wiki version must be 1.28-wmf.23 or newer to '
                     'automatically extract the sparql endpoint. '
                     'Please provide the endpoint and entity_url '
                     'parameters instead of a repo.')
             if not self.endpoint:
-                raise Error('The site {} does not provide a sparql endpoint.'
-                            .format(repo))
+                raise Error(
+                    f'The site {repo} does not provide a sparql endpoint.')
         else:
             if not entity_url:
                 raise Error('If initialised with an endpoint the entity_url '
                             'must be provided.')
             self.endpoint = endpoint
             self.entity_url = entity_url
 
@@ -122,16 +122,15 @@
             values = {}
             for var in qvars:
                 if var not in row:
                     # var is not available (OPTIONAL is probably used)
                     values[var] = None
                 elif full_data:
                     if row[var]['type'] not in VALUE_TYPES:
-                        raise ValueError('Unknown type: {}'
-                                         .format(row[var]['type']))
+                        raise ValueError(f"Unknown type: {row[var]['type']}")
                     valtype = VALUE_TYPES[row[var]['type']]
                     values[var] = valtype(row[var],
                                           entity_url=self.entity_url)
                 else:
                     values[var] = row[var]['value']
             result.append(values)
         return result
```

### Comparing `pywikibot-8.1.2/pywikibot/data/wikistats.py` & `pywikibot-8.2.0/pywikibot/data/wikistats.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/date.py` & `pywikibot-8.2.0/pywikibot/date.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,26 +381,24 @@
     # %T is a year in TH: -- all years are shifted: 2005 => 'พ.ศ. 2548'
     'T': (_decimalDigits, lambda v: str(v + 543),
           lambda v: int(v) - 543),
 }
 
 # Allows to search for '(%%)|(%d)|(%R)|...", and allows one digit 1-9 to set
 # the size of zero-padding for numbers
-_reParameters = re.compile('|'.join(f'(%[1-9]?{s})'
-                                    for s in _digitDecoders))
+_reParameters = re.compile('|'.join(f'(%[1-9]?{s})' for s in _digitDecoders))
 
 # A map of sitecode+pattern to (re matching object and corresponding decoders)
 _escPtrnCache2 = {}
 
 
-def escapePattern2(pattern: str
-                   ) -> Tuple[Pattern[str], str,
-                              List[Union[decoder_type, decoder_type]]]:
-    """
-    Convert a string pattern into a regex expression and cache.
+def escapePattern2(
+    pattern: str
+) -> Tuple[Pattern[str], str, List[decoder_type]]:
+    """Convert a string pattern into a regex expression and cache.
 
     Allows matching of any _digitDecoders inside the string.
     Returns a compiled regex object and a list of digit decoders.
     """
     @singledispatch
     def decode(dec: decoder_type, subpattern: str, newpattern: str,
                strpattern: str) -> Tuple[str, str]:
@@ -423,16 +421,16 @@
 
     @decode.register(str)
     def _(dec: str, subpattern: str, newpattern: str,
           strpattern: str) -> Tuple[str, str]:
         # Special case for strings that are replaced instead of decoded
         # Keep the original text for strPattern
         assert len(subpattern) < 3, (
-            'Invalid pattern {}: Cannot use zero padding size '
-            'in {}!'.format(pattern, subpattern))
+            f'Invalid pattern {pattern}: Cannot use zero padding size '
+            f'in {subpattern}!')
         return newpattern + re.escape(dec), strpattern + subpattern
 
     if pattern not in _escPtrnCache2:
         newPattern = ''  # match starts at the beginning of the string
         strPattern = ''
         decoders: List[decoder_type] = []
         for s in _reParameters.split(pattern):
@@ -497,29 +495,29 @@
             'parameter count ({}) does not match decoder count ({})'
             .format(len(params), len(decoders)))
         # convert integer parameters into their textual representation
         str_params = tuple(_make_parameter(decoders[i], param)
                            for i, param in enumerate(params))
         return strPattern % str_params
     assert len(decoders) == 1, (
-        'A single parameter does not match {} decoders.'
-        .format(len(decoders)))
+        f'A single parameter does not match {len(decoders)} decoders.')
     # convert integer parameter into its textual representation
     assert isinstance(params, int)
     return strPattern % _make_parameter(decoders[0], params)
 
 
 @dh.register(str)
 def _(value: str, pattern: str, encf: encf_type, decf: decf_type,
       filter: Optional[Callable[[int], bool]] = None) -> int:
     compPattern, _strPattern, decoders = escapePattern2(pattern)
     m = compPattern.match(value)
     if m:
         # decode each found value using provided decoder
-        values = [decoder[2](m[i + 1]) for i, decoder in enumerate(decoders)]
+        values = [decoder[2](m[i])
+                  for i, decoder in enumerate(decoders, start=1)]
         decValue = decf(values)
 
         assert not isinstance(decValue, str), \
             'Decoder must not return a string!'
 
         # recursive call to re-encode and see if we get the original
         # (may through filter exception)
@@ -687,16 +685,16 @@
             self.data[key] = eval(expression)
         return self.data[key]
 
     def __setitem__(self, key: str, value: Callable[[int], str]) -> None:
         self.data[key] = value
 
     def __delitem__(self, key: str) -> None:
-        raise NotImplementedError("Deleting of key '{}' is not implemented"
-                                  .format(key))
+        raise NotImplementedError(
+            f"Deleting of key '{key}' is not implemented")
 
     def __iter__(self) -> Iterator[str]:
         return iter(self.data)
 
     def __len__(self) -> int:
         return len(self.data)
 
@@ -1672,15 +1670,15 @@
 
     The function must accept one parameter for the ->int or ->string
     conversions, just like everywhere else in the formats map.
     The patterns parameter is a list of 12 elements to be used for each month.
 
     :param lang: language code
     """
-    assert len(patterns) == 12, 'pattern %s does not have 12 elements' % lang
+    assert len(patterns) == 12, f'pattern {lang} does not have 12 elements'
 
     for i in range(12):
         if patterns[i] is not None:
             if isMnthOfYear:
                 formats[yrMnthFmts[i]][lang] = eval(
                     f'lambda v: dh_mnthOfYear(v, "{patterns[i]}")')
             else:
@@ -1986,16 +1984,15 @@
     if not lang:
         lang = Site().lang
     elif hasattr(lang, 'lang'):
         lang = lang.lang  # type: ignore[union-attr]
     max_day = calendar.monthrange(year, month)[1]
     if not 1 <= day <= max_day:
         raise ValueError(
-            'Wrong day value {day}; must be 1-{max_day}'
-            .format(day=day, max_day=max_day))
+            f'Wrong day value {day}; must be 1-{max_day}')
     assert isinstance(lang, str)
     return formats[dayMnthFmts[month - 1]][lang](day)
 
 
 def formatYear(lang: str, year: int) -> str:
     """Return year name in a language."""
     if year < 0:
```

### Comparing `pywikibot-8.1.2/pywikibot/diff.py` & `pywikibot-8.2.0/pywikibot/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Diff module."""
 #
-# (C) Pywikibot team, 2014-2022
+# (C) Pywikibot team, 2014-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import difflib
 import math
 from collections import abc
 from difflib import _format_range_unified  # type: ignore[attr-defined]
@@ -164,16 +164,15 @@
 
         line_ref: string.
         """
         color = line[0]
 
         if line_ref is None:
             if color in self.colors:
-                colored_line = '<<{color}>>{}<<default>>'.format(
-                    line, color=self.colors[color])
+                colored_line = f'<<{self.colors[color]}>>{line}<<default>>'
                 return colored_line
             return line
 
         colored_line = ''
         color_closed = True
         for char, char_ref in zip_longest(
             line, line_ref.strip(), fillvalue=' '
@@ -181,16 +180,15 @@
             char_tagged = char
             if color_closed:
                 if char_ref != ' ':
                     if char != ' ':
                         apply_color = self.colors[color]
                     else:
                         apply_color = 'default;' + self.bg_colors[color]
-                    char_tagged = '<<{color}>>{}'.format(char,
-                                                         color=apply_color)
+                    char_tagged = f'<<{apply_color}>>{char}'
                     color_closed = False
             else:
                 if char_ref == ' ':
                     char_tagged = f'<<default>>{char}'
                     color_closed = True
             colored_line += char_tagged
 
@@ -344,18 +342,18 @@
                 # self.context * 2, because if self.context is 2 the hunks
                 # would be directly adjacent when 4 lines in between and for
                 # anything below 4 they share lines.
                 # not super_hunk == first hunk as any other super_hunk is
                 # created with one hunk
                 if (not super_hunk or hunk.pre_context <= self.context * 2):
                     # previous hunk has shared/adjacent self.context lines
-                    super_hunk += [hunk]
+                    super_hunk.append(hunk)
                 else:
                     super_hunk = [hunk]
-                    super_hunks += [super_hunk]
+                    super_hunks.append(super_hunk)
         else:
             super_hunks = [[hunk] for hunk in hunks]
         return [_SuperHunk(sh) for sh in super_hunks]
 
     def _get_context_range(self, super_hunk: _SuperHunk
                            ) -> Tuple[Tuple[int, int], Tuple[int, int]]:
         """Dynamically determine context range for a super hunk."""
@@ -426,28 +424,28 @@
             super_hunk = super_hunks[position]
 
             next_pending = find_pending(position + 1, len(super_hunks))
             prev_pending = find_pending(position - 1, -1)
 
             answers = ['y', 'n', 'q', 'a', 'd', 'g']
             if next_pending is not None:
-                answers += ['j']
+                answers.append('j')
             if position < len(super_hunks) - 1:
-                answers += ['J']
+                answers.append('J')
             if prev_pending is not None:
-                answers += ['k']
+                answers.append('k')
             if position > 0:
-                answers += ['K']
+                answers.append('K')
             if len(super_hunk) > 1:
-                answers += ['s']
-            answers += ['?']
+                answers.append('s')
+            answers.append('?')
 
             pywikibot.info(self._generate_diff(super_hunk))
-            choice = pywikibot.input('Accept this hunk [{}]?'.format(
-                ','.join(answers)))
+            choice = pywikibot.input(
+                f"Accept this hunk [{','.join(answers)}]?")
             if choice not in answers:
                 choice = '?'
 
             if choice in ['y', 'n']:
                 super_hunk.reviewed = \
                     Hunk.APPR if choice == 'y' else Hunk.NOT_APPR
                 if next_pending is not None:
@@ -587,20 +585,24 @@
     else:
         pywikibot.info(template.format('None.', '', ''))
 
     return ''.join(text_list)
 
 
 def html_comparator(compare_string: str) -> Dict[str, List[str]]:
-    """List of added and deleted contexts from 'action=compare' html string.
+    """List of added and deleted contexts from ``action=compare`` html string.
 
-    This function is useful when combineds with site.py's "compare" method.
-    Site.compare() returns HTML that is useful for displaying on a page.
-    Here we use BeautifulSoup to get the un-HTML-ify the context of changes.
+    This function is useful when combined with :meth:`Site.compare()
+    <pywikibot.site._apisite.APISite.compare>` method. ``compare()``
+    returns HTML that is useful for displaying on a page. Here we use
+    ``BeautifulSoup`` to get the un-HTML-ify the context of changes.
     Finally we present the added and deleted contexts.
+
+    .. note:: ``beautifulsoup4`` package is needed for this function.
+
     :param compare_string: HTML string from MediaWiki API
     :return: deleted and added list of contexts
     """
     from bs4 import BeautifulSoup
 
     comparands: Dict[str, List[str]] = {'deleted-context': [],
                                         'added-context': []}
```

### Comparing `pywikibot-8.1.2/pywikibot/echo.py` & `pywikibot-8.2.0/pywikibot/echo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/editor.py` & `pywikibot-8.2.0/pywikibot/editor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Text editor class for your favourite editor."""
 #
 # (C) Pywikibot team, 2004-2022
 #
 # Distributed under the terms of the MIT license.
 #
 import os
+import shlex
 import subprocess
 import tempfile
 from pathlib import Path
 from sys import platform
 from textwrap import fill
 from typing import Optional
 
@@ -79,15 +80,16 @@
         # Windows editors
         elif self.editor.lower().endswith('notepad++.exe'):
             command = [f'-n{line + 1}']  # seems not to support columns
         else:
             command = []
 
         # See T102465 for problems relating to using self.editor unparsed.
-        command = [self.editor] + command + [file_name]
+        editor_cmd = [self.editor] if OSWIN32 else shlex.split(self.editor)
+        command = editor_cmd + command + [file_name]
         pywikibot.log(f'Running editor: {self._concat(command)}')
         return command
 
     @staticmethod
     def _concat(command: Sequence[str]) -> str:
         return ' '.join(f'{part!r}' if ' ' in part else part
                         for part in command)
```

### Comparing `pywikibot-8.1.2/pywikibot/exceptions.py` & `pywikibot-8.2.0/pywikibot/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
   - InterwikiRedirectPageError: Page is a redirect to another site
   - InvalidPageError: Page is invalid e.g. without history
   - NotEmailableError: The target user has disabled email
   - NoMoveTargetError: An expected move target page does not exist
 
 PageLoadRelatedError: any exception which happens while loading a Page.
   - InconsistentTitleError: Page receives a title inconsistent with query
-  - NoSiteLinkError: ItemPage has no sitelink to given language
+  - NoSiteLinkError: ItemPage has no sitelink to given site
 
 PageSaveRelatedError: page exceptions within the save operation on a Page
 
   - AbuseFilterDisallowedError: AbuseFilter disallowed
   - SpamblacklistError: MediaWiki spam filter detected a blacklisted URL
   - TitleblacklistError: MediaWiki detected a blacklisted page title
   - OtherPageSaveError: misc. other save related exception.
@@ -396,29 +396,29 @@
         """
         self.message = f"Query on {{}} returned data on '{actual}'"
         super().__init__(page)
 
 
 class NoSiteLinkError(PageLoadRelatedError, NoPageError):
 
-    """ItemPage has no sitelink to the given language.
+    """ItemPage has no sitelink to the given site.
 
     .. versionadded:: 8.1
     .. deprecated:: 8.1
        :exc:`NoPageError` dependency.
     """
 
-    def __init__(self, page: 'pywikibot.page.ItemPage', lang: str) -> None:
+    def __init__(self, page: 'pywikibot.page.ItemPage', dbname: str) -> None:
         """Initializer.
 
         :param page: ItemPage that caused the exception
-        :param lang: language code of the queried sitelink
+        :param dbname: site identifier of the queried sitelink
 
         """
-        self.message = f'Item {{}} has no sitelink to language {lang!r}'
+        self.message = f'Item {{}} has no sitelink to {dbname!r}'
         super().__init__(page)
 
 
 class SiteDefinitionError(Error):
 
     """Site does not exist."""
 
@@ -693,16 +693,16 @@
 
     def __init__(self, entity: 'pywikibot.page.WikibaseEntity') -> None:
         """
         Initializer.
 
         :param entity: Wikibase entity
         """
-        super().__init__("Entity '{}' doesn't exist on {}"
-                         .format(entity.id, entity.repo))
+        super().__init__(
+            f"Entity '{entity.id}' doesn't exist on {entity.repo}")
         self.entity = entity
 
 
 class CoordinateGlobeUnknownError(WikiBaseError, NotImplementedError):
 
     """This globe is not implemented yet in either WikiBase or pywikibot."""
```

### Comparing `pywikibot-8.1.2/pywikibot/families/lingualibre_family.py` & `pywikibot-8.2.0/pywikibot/families/lingualibre_family.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Family module for Lingua Libre.
 
 .. versionaddded: 6.5
 """
 #
-# (C) Pywikibot team, 2021-2022
+# (C) Pywikibot team, 2021-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from pywikibot import family
 
 
-class Family(family.WikimediaFamily):
+class Family(family.WikimediaFamily, family.WikibaseFamily):
 
     """Family class for Lingua Libre.
 
     .. versionaddded: 6.5
     """
 
     name = 'lingualibre'
@@ -24,11 +24,7 @@
     }
 
     interwiki_forward = 'wikipedia'
 
     def scriptpath(self, code) -> str:
         """Return the script path for this family."""
         return ''
-
-    def interface(self, code) -> str:
-        """Return 'DataSite'."""
-        return 'DataSite'
```

### Comparing `pywikibot-8.1.2/pywikibot/families/meta_family.py` & `pywikibot-8.2.0/pywikibot/families/meta_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/families/osm_family.py` & `pywikibot-8.2.0/pywikibot/families/osm_family.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Family module for OpenStreetMap wiki."""
 #
-# (C) Pywikibot team, 2009-2022
+# (C) Pywikibot team, 2009-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from pywikibot import family
 
 
 # The project wiki of OpenStreetMap (OSM).
@@ -39,11 +39,7 @@
         'en': ('/doc',),
     }
 
     # Templates that indicate an edit should be avoided
     edit_restricted_templates = {
         'en': ('In Bearbeitung',),
     }
-
-    def protocol(self, code) -> str:
-        """Return https as the protocol for this family."""
-        return 'https'
```

### Comparing `pywikibot-8.1.2/pywikibot/families/vikidia_family.py` & `pywikibot-8.2.0/pywikibot/families/vikidia_family.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 """Family module for Vikidia."""
 #
-# (C) Pywikibot team, 2010-2022
+# (C) Pywikibot team, 2010-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from pywikibot import family
 
 
 class Family(family.SubdomainFamily):
 
     """Family class for Vikidia."""
 
     name = 'vikidia'
     domain = 'vikidia.org'
 
     codes = [
-        'ca', 'de', 'el', 'en', 'es', 'eu', 'fr', 'hy', 'it', 'oc',
-        'pt', 'ru', 'scn',
+        'ca', 'de', 'el', 'en', 'es', 'eu', 'fr', 'hy', 'it', 'oc', 'pt', 'ru',
+        'scn',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['central', 'test']
-
-    def protocol(self, code) -> str:
-        """Return https as the protocol for this family."""
-        return 'https'
```

### Comparing `pywikibot-8.1.2/pywikibot/families/wikibooks_family.py` & `pywikibot-8.2.0/pywikibot/families/wikibooks_family.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'als', 'dk', 'tokipona',
     ]
 
     languages_by_size = [
         'en', 'vi', 'hu', 'de', 'fr', 'it', 'ja', 'pt', 'es', 'nl', 'pl', 'id',
         'he', 'fi', 'zh', 'fa', 'az', 'sq', 'ru', 'ca', 'eu', 'th', 'cs', 'da',
-        'ko', 'ba', 'sv', 'gl', 'hi', 'sr', 'uk', 'hr', 'no', 'tr', 'sa', 'ar',
-        'ta', 'bn', 'eo', 'sk', 'is', 'ro', 'si', 'bg', 'ms', 'mk', 'ka', 'tt',
-        'lt', 'el', 'li', 'sl', 'tl', 'ur', 'km', 'la', 'mr', 'kk', 'te', 'et',
-        'be', 'ia', 'shn', 'ml', 'oc', 'pa', 'hy', 'ne', 'cv', 'tg', 'ku',
-        'fy', 'af', 'bs', 'cy', 'mg', 'ky',
+        'ko', 'hi', 'ba', 'sv', 'gl', 'sr', 'uk', 'hr', 'no', 'tr', 'sa', 'ar',
+        'ta', 'bn', 'eo', 'is', 'sk', 'si', 'ro', 'bg', 'ms', 'mk', 'ka', 'tt',
+        'lt', 'el', 'li', 'sl', 'tl', 'ur', 'km', 'la', 'mr', 'kk', 'te',
+        'shn', 'et', 'be', 'ia', 'ml', 'oc', 'ne', 'hy', 'pa', 'cv', 'tg',
+        'ku', 'fy', 'af', 'bs', 'cy', 'mg', 'ky',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'en': ('Category redirect',),
         'es': ('Categoría redirigida',),
```

### Comparing `pywikibot-8.1.2/pywikibot/families/wikihow_family.py` & `pywikibot-8.2.0/pywikibot/families/wikihow_family.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Family module for wikiHow wiki.
 
 .. versionadded:: 3.0
 """
 #
-# (C) Pywikibot team, 2020-2022
+# (C) Pywikibot team, 2020-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from pywikibot import family
 from pywikibot.tools import classproperty
 
 
@@ -17,18 +17,18 @@
 
     .. versionadded:: 3.0
     """
 
     name = 'wikihow'
     domain = 'wikihow.com'
 
-    codes = (
+    codes = [
         'ar', 'cs', 'de', 'en', 'es', 'fr', 'hi', 'id', 'it', 'ja', 'ko', 'nl',
         'pt', 'ru', 'th', 'tr', 'vi', 'zh',
-    )
+    ]
 
     removed_wikis = ['ca', 'cy', 'fa', 'he', 'pl', 'ur']
 
     title_delimiter_and_aliases = '- '
     """.. versionadded:: 7.0"""
 
     @classproperty
@@ -56,11 +56,7 @@
             code = code_replacement.get(code, code)
             cls.langs[code] = 'www.' + domain
         return cls.langs
 
     def scriptpath(self, code) -> str:
         """Return the script path for this family."""
         return ''
-
-    def protocol(self, code) -> str:
-        """Return 'https' as the protocol."""
-        return 'https'
```

### Comparing `pywikibot-8.1.2/pywikibot/families/wikimania_family.py` & `pywikibot-8.2.0/pywikibot/families/wikimania_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/families/wikimediachapter_family.py` & `pywikibot-8.2.0/pywikibot/families/wikimediachapter_family.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Family class for WCH, WTO and WUG wikis hosted on wikimedia.org."""
 
     name = 'wikimediachapter'
     code_aliases = {
         'et': 'ee'
     }
 
-    closed_wikis = ['nz', 'pa-us', ]
+    closed_wikis = ['cn', 'nz', 'pa-us', ]
 
     codes = [
-        'am', 'ar', 'az', 'bd', 'be', 'br', 'ca', 'cn', 'co', 'dk', 'ec', 'ee',
-        'fi', 'ge', 'gr', 'hi', 'id', 'id-internal', 'il', 'mai', 'mk', 'mx',
-        'ng', 'nl', 'no', 'nyc', 'pl', 'pt', 'punjabi', 'romd', 'rs', 'ru',
-        'se', 'tr', 'ua', 'uk', 've', 'wb',
+        'am', 'ar', 'az', 'bd', 'be', 'br', 'ca', 'co', 'dk', 'ec', 'ee', 'fi',
+        'ge', 'gr', 'hi', 'id', 'id-internal', 'il', 'mai', 'mk', 'mx', 'ng',
+        'nl', 'no', 'nyc', 'pl', 'pt', 'punjabi', 'romd', 'rs', 'ru', 'se',
+        'tr', 'ua', 'uk', 've', 'wb',
     ]
```

### Comparing `pywikibot-8.1.2/pywikibot/families/wikinews_family.py` & `pywikibot-8.2.0/pywikibot/families/wikinews_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/closed.dblist
         'bg', 'hu', 'sd', 'th', 'tr',
     ]
 
     languages_by_size = [
         'ru', 'sr', 'pt', 'fr', 'en', 'pl', 'zh', 'de', 'es', 'it', 'ar', 'cs',
         'ca', 'nl', 'el', 'ta', 'li', 'sv', 'uk', 'fa', 'fi', 'ro', 'ja', 'eo',
-        'sq', 'no', 'ko', 'bs', 'he', 'guw',
+        'guw', 'sq', 'no', 'ko', 'bs', 'he',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'fa': ('الگو:رده بهتر',),
         'no': ('Kategoriomdirigering',),
```

### Comparing `pywikibot-8.1.2/pywikibot/families/wikipedia_family.py` & `pywikibot-8.2.0/pywikibot/families/wikipedia_family.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,56 +12,56 @@
 
     """Family module for Wikipedia."""
 
     name = 'wikipedia'
 
     closed_wikis = [
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/closed.dblist
-        'aa', 'cho', 'ho', 'hz', 'ii', 'kj', 'kr', 'lrc', 'mh', 'mus', 'ng',
-        'ten',
+        'aa', 'ak', 'cho', 'ho', 'hz', 'ii', 'kj', 'kr', 'lrc', 'mh', 'mus',
+        'na', 'ng', 'ten',
     ]
 
     removed_wikis = [
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'dk', 'mo', 'ru-sib', 'tlh', 'tokipona', 'zh_cn', 'zh_tw',
     ]
 
     languages_by_size = [
         'en', 'ceb', 'de', 'sv', 'fr', 'nl', 'ru', 'es', 'it', 'arz', 'pl',
-        'ja', 'zh', 'vi', 'war', 'uk', 'ar', 'pt', 'fa', 'ca', 'sr', 'id',
-        'ko', 'no', 'ce', 'fi', 'hu', 'cs', 'tr', 'tt', 'sh', 'ro',
+        'ja', 'zh', 'vi', 'uk', 'war', 'ar', 'pt', 'fa', 'ca', 'sr', 'id',
+        'ko', 'no', 'ce', 'fi', 'cs', 'hu', 'tr', 'tt', 'sh', 'ro',
         'zh-min-nan', 'eu', 'ms', 'eo', 'he', 'hy', 'da', 'bg', 'cy', 'sk',
-        'azb', 'uz', 'et', 'kk', 'be', 'simple', 'min', 'el', 'hr', 'lt', 'gl',
-        'az', 'ur', 'sl', 'ka', 'nn', 'hi', 'th', 'ta', 'la', 'bn', 'mk',
-        'ast', 'zh-yue', 'lld', 'lv', 'tg', 'af', 'my', 'mg', 'bs', 'mr', 'sq',
-        'oc', 'nds', 'ml', 'be-tarask', 'te', 'ky', 'br', 'sw', 'jv', 'new',
-        'vec', 'pnb', 'ht', 'pms', 'ba', 'lb', 'su', 'ku', 'ga', 'lmo', 'szl',
-        'is', 'fy', 'cv', 'ckb', 'pa', 'tl', 'an', 'wuu', 'diq', 'io', 'sco',
-        'vo', 'yo', 'ne', 'ia', 'gu', 'kn', 'als', 'avk', 'bar', 'scn', 'bpy',
-        'ha', 'crh', 'qu', 'nv', 'mn', 'xmf', 'si', 'ban', 'ps', 'frr',
-        'bat-smg', 'os', 'or', 'sah', 'cdo', 'gd', 'bug', 'yi', 'sd', 'ilo',
-        'am', 'nap', 'mzn', 'ig', 'li', 'gor', 'fo', 'hsb', 'map-bms', 'mai',
-        'bcl', 'eml', 'shn', 'ace', 'zh-classical', 'sa', 'wa', 'as', 'ie',
-        'lij', 'zu', 'mhr', 'hyw', 'hif', 'sn', 'mrj', 'tum', 'bjn', 'mni',
-        'km', 'hak', 'roa-tara', 'so', 'pam', 'rue', 'nso', 'bh', 'sat', 'se',
-        'myv', 'mi', 'vls', 'nds-nl', 'nah', 'sc', 'kw', 'glk', 'vep', 'kab',
-        'tk', 'dag', 'ary', 'gan', 'co', 'fiu-vro', 'bo', 'ab', 'rw', 'gv',
-        'skr', 'ug', 'zea', 'frp', 'udm', 'pcd', 'kv', 'csb', 'mt', 'gn',
-        'smn', 'ay', 'nrm', 'lez', 'lfn', 'olo', 'stq', 'mwl', 'lo', 'ang',
-        'fur', 'rm', 'lad', 'gom', 'koi', 'ext', 'tyv', 'dsb', 'av', 'ln',
-        'dty', 'kaa', 'pap', 'cbk-zam', 'mdf', 'dv', 'ksh', 'tw', 'ks', 'gag',
-        'bxr', 'pfl', 'lg', 'za', 'pi', 'pag', 'szy', 'haw', 'awa', 'tay',
-        'blk', 'inh', 'krc', 'xal', 'pdc', 'to', 'atj', 'arc', 'tcy', 'mnw',
-        'jam', 'kbp', 'na', 'wo', 'kbd', 'nia', 'nov', 'shi', 'anp', 'ki',
-        'nqo', 'bi', 'tpi', 'tet', 'jbo', 'roa-rup', 'xh', 'fj', 'om', 'kg',
-        'lbe', 'ty', 'guw', 'cu', 'trv', 'srn', 'sm', 'alt', 'gcr', 'chr',
-        'ltg', 'tn', 'ny', 'mad', 'st', 'pih', 'got', 'ee', 'rmy', 'ami', 'bm',
-        'ff', 've', 'ts', 'chy', 'ss', 'kcg', 'rn', 'pcm', 'ch', 'ik', 'pnt',
-        'guc', 'ady', 'iu', 'ak', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'gur',
-        'fat', 'cr',
+        'azb', 'uz', 'et', 'kk', 'simple', 'be', 'min', 'el', 'hr', 'lt', 'gl',
+        'az', 'ur', 'sl', 'ka', 'lld', 'nn', 'hi', 'th', 'ta', 'bn', 'la',
+        'mk', 'zh-yue', 'ast', 'lv', 'tg', 'af', 'my', 'mg', 'mr', 'bs', 'sq',
+        'oc', 'nds', 'te', 'ml', 'be-tarask', 'br', 'ky', 'sw', 'jv', 'new',
+        'lmo', 'pnb', 'vec', 'ht', 'pms', 'ba', 'lb', 'su', 'ku', 'ga', 'szl',
+        'is', 'fy', 'cv', 'pa', 'ckb', 'tl', 'an', 'wuu', 'diq', 'io', 'sco',
+        'vo', 'yo', 'ne', 'ia', 'gu', 'kn', 'als', 'avk', 'ha', 'bar', 'scn',
+        'crh', 'bpy', 'qu', 'nv', 'mn', 'xmf', 'ban', 'si', 'ps', 'frr',
+        'bat-smg', 'os', 'or', 'sah', 'mzn', 'cdo', 'ig', 'gd', 'bug', 'tum',
+        'yi', 'sd', 'ilo', 'am', 'nap', 'li', 'fo', 'gor', 'bcl', 'hsb',
+        'map-bms', 'mai', 'shn', 'eml', 'ace', 'zh-classical', 'sa', 'as',
+        'wa', 'ie', 'lij', 'zu', 'mhr', 'hyw', 'hif', 'sn', 'mrj', 'bjn',
+        'mni', 'km', 'hak', 'so', 'roa-tara', 'pam', 'rue', 'sat', 'nso', 'bh',
+        'se', 'mi', 'myv', 'vls', 'nds-nl', 'sc', 'dag', 'kw', 'vep', 'glk',
+        'bo', 'ary', 'co', 'tk', 'kab', 'gan', 'rw', 'fiu-vro', 'ab', 'gv',
+        'ug', 'nah', 'zea', 'skr', 'frp', 'udm', 'pcd', 'kv', 'mt', 'csb',
+        'gn', 'smn', 'ay', 'nrm', 'ks', 'lez', 'lfn', 'olo', 'mwl', 'stq',
+        'lo', 'ang', 'fur', 'rm', 'mdf', 'lad', 'gom', 'ext', 'kaa', 'tyv',
+        'koi', 'dsb', 'av', 'pap', 'ln', 'dty', 'tw', 'cbk-zam', 'dv', 'ksh',
+        'za', 'gag', 'bxr', 'pfl', 'lg', 'szy', 'pag', 'pi', 'tay', 'blk',
+        'haw', 'awa', 'inh', 'krc', 'xal', 'pdc', 'to', 'atj', 'tcy', 'arc',
+        'mnw', 'jam', 'kbp', 'wo', 'anp', 'kbd', 'nia', 'shi', 'nov', 'ki',
+        'nqo', 'bi', 'tpi', 'tet', 'xh', 'om', 'roa-rup', 'jbo', 'fj', 'lbe',
+        'kg', 'ty', 'guw', 'cu', 'trv', 'ami', 'ff', 'srn', 'sm', 'alt', 'gcr',
+        'chr', 'tn', 'mad', 'ltg', 'ny', 'st', 'pih', 'got', 'rmy', 'ee', 'bm',
+        'ss', 'pcm', 've', 'ts', 'chy', 'kcg', 'rn', 'gur', 'ch', 'ik', 'pnt',
+        'ady', 'fat', 'guc', 'iu', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'cr',
+        'gpe',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['test', 'test2']
 
     # Templates that indicate a category redirect
     # Redirects to these templates are automatically included
@@ -111,39 +111,39 @@
         'zh-yue': ('分類彈去',),
     }
 
     # Global bot allowed languages on
     # https://meta.wikimedia.org/wiki/BPI#Current_implementation
     # & https://meta.wikimedia.org/wiki/Special:WikiSets/2
     cross_allowed = [
-        'ab', 'ace', 'ady', 'af', 'ak', 'als', 'am', 'an', 'ang', 'ar', 'arc',
-        'arz', 'as', 'ast', 'atj', 'av', 'ay', 'az', 'ba', 'bar', 'bat-smg',
-        'bcl', 'be', 'be-tarask', 'bg', 'bh', 'bi', 'bjn', 'bm', 'bo', 'bpy',
-        'bug', 'bxr', 'ca', 'cbk-zam', 'cdo', 'ce', 'ceb', 'ch', 'chr', 'chy',
-        'ckb', 'co', 'cr', 'crh', 'cs', 'csb', 'cu', 'cv', 'cy', 'da', 'diq',
-        'dsb', 'dty', 'dz', 'ee', 'el', 'eml', 'en', 'eo', 'et', 'eu', 'ext',
-        'fa', 'ff', 'fi', 'fj', 'fo', 'frp', 'frr', 'fur', 'ga', 'gag', 'gan',
-        'gd', 'glk', 'gn', 'gom', 'gor', 'got', 'gu', 'gv', 'ha', 'hak', 'haw',
-        'he', 'hi', 'hif', 'hr', 'hsb', 'ht', 'hu', 'hy', 'ia', 'ie', 'ig',
-        'ik', 'ilo', 'inh', 'io', 'iu', 'ja', 'jam', 'jbo', 'jv', 'ka', 'kaa',
-        'kab', 'kbd', 'kg', 'ki', 'kk', 'kl', 'km', 'kn', 'ko', 'koi', 'krc',
-        'ks', 'ku', 'kv', 'kw', 'ky', 'la', 'lad', 'lb', 'lbe', 'lez', 'lfn',
-        'lg', 'li', 'lij', 'lmo', 'ln', 'lo', 'lt', 'ltg', 'lv', 'map-bms',
-        'mdf', 'meta', 'mg', 'mhr', 'mi', 'mk', 'ml', 'mn', 'mrj', 'ms', 'mwl',
-        'my', 'myv', 'mzn', 'na', 'nah', 'nap', 'nds-nl', 'ne', 'new', 'nl',
-        'no', 'nov', 'nrm', 'nso', 'nv', 'ny', 'oc', 'olo', 'om', 'or', 'os',
-        'pa', 'pag', 'pam', 'pap', 'pdc', 'pfl', 'pi', 'pih', 'pms', 'pnb',
-        'pnt', 'ps', 'qu', 'rm', 'rmy', 'rn', 'roa-rup', 'roa-tara', 'ru',
-        'rue', 'rw', 'sa', 'sah', 'sc', 'scn', 'sco', 'sd', 'se', 'sg', 'sh',
-        'shn', 'si', 'simple', 'sk', 'sm', 'sn', 'so', 'srn', 'ss', 'st',
-        'stq', 'su', 'sv', 'sw', 'szl', 'ta', 'tcy', 'te', 'tet', 'tg', 'th',
-        'ti', 'tk', 'tl', 'tn', 'to', 'tpi', 'tr', 'ts', 'tt', 'tum', 'tw',
-        'ty', 'tyv', 'udm', 'ug', 'uz', 've', 'vec', 'vep', 'vls', 'vo', 'wa',
-        'war', 'wo', 'xal', 'xh', 'xmf', 'yi', 'yo', 'za', 'zea', 'zh',
-        'zh-classical', 'zh-min-nan', 'zh-yue', 'zu',
+        'ab', 'ace', 'ady', 'af', 'als', 'am', 'an', 'ang', 'ar', 'arc', 'arz',
+        'as', 'ast', 'atj', 'av', 'ay', 'az', 'ba', 'bar', 'bat-smg', 'bcl',
+        'be', 'be-tarask', 'bg', 'bh', 'bi', 'bjn', 'bm', 'bo', 'bpy', 'bug',
+        'bxr', 'ca', 'cbk-zam', 'cdo', 'ce', 'ceb', 'ch', 'chr', 'chy', 'ckb',
+        'co', 'cr', 'crh', 'cs', 'csb', 'cu', 'cv', 'cy', 'da', 'diq', 'dsb',
+        'dty', 'dz', 'ee', 'el', 'eml', 'en', 'eo', 'et', 'eu', 'ext', 'fa',
+        'ff', 'fi', 'fj', 'fo', 'frp', 'frr', 'fur', 'ga', 'gag', 'gan', 'gd',
+        'glk', 'gn', 'gom', 'gor', 'got', 'gu', 'gv', 'ha', 'hak', 'haw', 'he',
+        'hi', 'hif', 'hr', 'hsb', 'ht', 'hu', 'hy', 'ia', 'ie', 'ig', 'ik',
+        'ilo', 'inh', 'io', 'iu', 'ja', 'jam', 'jbo', 'jv', 'ka', 'kaa', 'kab',
+        'kbd', 'kg', 'ki', 'kk', 'kl', 'km', 'kn', 'ko', 'koi', 'krc', 'ks',
+        'ku', 'kv', 'kw', 'ky', 'la', 'lad', 'lb', 'lbe', 'lez', 'lfn', 'lg',
+        'li', 'lij', 'lmo', 'ln', 'lo', 'lt', 'ltg', 'lv', 'map-bms', 'mdf',
+        'meta', 'mg', 'mhr', 'mi', 'mk', 'ml', 'mn', 'mrj', 'ms', 'mwl', 'my',
+        'myv', 'mzn', 'nah', 'nap', 'nds-nl', 'ne', 'new', 'nl', 'no', 'nov',
+        'nrm', 'nso', 'nv', 'ny', 'oc', 'olo', 'om', 'or', 'os', 'pa', 'pag',
+        'pam', 'pap', 'pdc', 'pfl', 'pi', 'pih', 'pms', 'pnb', 'pnt', 'ps',
+        'qu', 'rm', 'rmy', 'rn', 'roa-rup', 'roa-tara', 'ru', 'rue', 'rw',
+        'sa', 'sah', 'sc', 'scn', 'sco', 'sd', 'se', 'sg', 'sh', 'shn', 'si',
+        'simple', 'sk', 'sm', 'sn', 'so', 'srn', 'ss', 'st', 'stq', 'su', 'sv',
+        'sw', 'szl', 'ta', 'tcy', 'te', 'tet', 'tg', 'th', 'ti', 'tk', 'tl',
+        'tn', 'to', 'tpi', 'tr', 'ts', 'tt', 'tum', 'tw', 'ty', 'tyv', 'udm',
+        'ug', 'uz', 've', 'vec', 'vep', 'vls', 'vo', 'wa', 'war', 'wo', 'xal',
+        'xh', 'xmf', 'yi', 'yo', 'za', 'zea', 'zh', 'zh-classical',
+        'zh-min-nan', 'zh-yue', 'zu',
     ]
 
     # Languages that used to be coded in iso-8859-1
     latin1old = {
         'af', 'bs', 'co', 'cs', 'da', 'de', 'en', 'es', 'et', 'eu', 'fi', 'fr',
         'fy', 'ga', 'gl', 'ia', 'id', 'it', 'la', 'lt', 'lv', 'mi', 'mr', 'na',
         'nds', 'nl', 'no', 'pt', 'simple', 'sl', 'sv', 'sw', 'test', 'tt',
```

### Comparing `pywikibot-8.1.2/pywikibot/families/wikiquote_family.py` & `pywikibot-8.2.0/pywikibot/families/wikiquote_family.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
     removed_wikis = [
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'als', 'tokipona',
     ]
 
     languages_by_size = [
-        'it', 'en', 'pl', 'ru', 'cs', 'et', 'pt', 'fa', 'uk', 'he', 'de', 'fr',
-        'es', 'tr', 'eo', 'sk', 'bs', 'az', 'ca', 'fi', 'sr', 'zh', 'sl', 'lt',
-        'ar', 'su', 'bg', 'hy', 'hr', 'id', 'el', 'nn', 'sv', 'li', 'hu', 'ko',
-        'nl', 'sah', 'ja', 'la', 'ta', 'hi', 'gl', 'gu', 'ur', 'ig', 'be',
-        'guw', 'te', 'vi', 'tl', 'cy', 'no', 'bn', 'sq', 'ml', 'as', 'kn',
-        'ro', 'eu', 'ku', 'uz', 'ka', 'da', 'sa', 'is', 'bcl', 'br', 'th',
-        'mr', 'af', 'ky',
+        'it', 'en', 'pl', 'ru', 'cs', 'et', 'pt', 'fa', 'uk', 'he', 'fr', 'de',
+        'es', 'tr', 'eo', 'sk', 'bs', 'az', 'ca', 'fi', 'sr', 'lt', 'zh', 'sl',
+        'ar', 'su', 'id', 'bg', 'hy', 'hr', 'el', 'nn', 'sv', 'li', 'hu', 'ko',
+        'nl', 'ja', 'sah', 'la', 'ta', 'hi', 'ig', 'gl', 'gu', 'ur', 'guw',
+        'as', 'be', 'te', 'vi', 'tl', 'cy', 'bn', 'no', 'sq', 'ml', 'kn', 'ro',
+        'eu', 'ku', 'uz', 'ka', 'da', 'sa', 'is', 'bcl', 'th', 'br', 'mr',
+        'af', 'ky',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'en': ('Category redirect',),
         'ro': ('Redirect categorie',),
```

### Comparing `pywikibot-8.1.2/pywikibot/families/wikisource_family.py` & `pywikibot-8.2.0/pywikibot/families/wikisource_family.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
     removed_wikis = [
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'tokipona',
     ]
 
     languages_by_size = [
         'pl', 'en', 'ru', 'de', 'fr', 'zh', 'he', 'it', 'uk', 'ar', 'es',
-        'mul', 'gu', 'cs', 'sr', 'pt', 'fa', 'sv', 'bn', 'hu', 'ko', 'ta',
-        'ml', 'sa', 'te', 'sl', 'tr', 'vi', 'hy', 'la', 'el', 'ja', 'ro', 'fi',
-        'nl', 'nap', 'be', 'az', 'ca', 'hr', 'br', 'kn', 'no', 'th', 'id',
-        'eo', 'hi', 'is', 'vec', 'cy', 'ban', 'pms', 'mr', 'lij', 'da', 'et',
-        'mk', 'as', 'yi', 'bg', 'jv', 'wa', 'li', 'lt', 'pa', 'or', 'eu', 'gl',
+        'mul', 'gu', 'cs', 'sr', 'pt', 'bn', 'fa', 'sv', 'ko', 'hu', 'ta',
+        'ml', 'sa', 'te', 'sl', 'tr', 'vi', 'la', 'hy', 'el', 'be', 'ja', 'ro',
+        'nl', 'fi', 'nap', 'az', 'ca', 'hr', 'br', 'kn', 'no', 'id', 'th',
+        'hi', 'eo', 'is', 'cy', 'vec', 'ban', 'pms', 'mr', 'lij', 'da', 'et',
+        'as', 'mk', 'yi', 'bg', 'jv', 'wa', 'li', 'pa', 'lt', 'or', 'eu', 'gl',
         'bs', 'sah', 'sk', 'zh-min-nan', 'fo',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['beta']
 
     category_redirect_templates = {
```

### Comparing `pywikibot-8.1.2/pywikibot/families/wikiversity_family.py` & `pywikibot-8.2.0/pywikibot/families/wikiversity_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/families/wikivoyage_family.py` & `pywikibot-8.2.0/pywikibot/families/wikivoyage_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     """Family class for Wikivoyage."""
 
     name = 'wikivoyage'
 
     languages_by_size = [
         'en', 'de', 'pl', 'it', 'fa', 'fr', 'ru', 'zh', 'nl', 'pt', 'es', 'he',
-        'vi', 'fi', 'sv', 'el', 'eo', 'uk', 'bn', 'ja', 'ro', 'tr', 'ps',
+        'vi', 'fi', 'sv', 'el', 'eo', 'ja', 'uk', 'bn', 'ro', 'tr', 'ps',
         'shn', 'hi',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'bn': ('বিষয়শ্রেণী পুনর্নির্দেশ',),
         'zh': ('分类重定向',),
```

### Comparing `pywikibot-8.1.2/pywikibot/families/wiktionary_family.py` & `pywikibot-8.2.0/pywikibot/families/wiktionary_family.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,28 +30,28 @@
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'als', 'ba', 'dk', 'mo', 'tlh', 'tokipona',
     ]
 
     languages_by_size = [
         'en', 'fr', 'mg', 'zh', 'ru', 'de', 'es', 'sh', 'sv', 'nl', 'el', 'pl',
         'ku', 'lt', 'ca', 'it', 'hu', 'fi', 'ta', 'pt', 'tr', 'ja', 'io', 'hy',
-        'ko', 'kn', 'vi', 'sr', 'th', 'hi', 'ro', 'no', 'id', 'et', 'cs',
-        'skr', 'ml', 'my', 'uz', 'li', 'or', 'eo', 'te', 'fa', 'gl', 'ar',
-        'oc', 'jv', 'az', 'uk', 'eu', 'sg', 'is', 'ast', 'br', 'bn', 'da',
-        'mnw', 'lo', 'simple', 'la', 'hr', 'sk', 'shn', 'fj', 'ky', 'wa', 'bg',
-        'tg', 'ur', 'ps', 'cy', 'lmo', 'he', 'vo', 'om', 'sl', 'af',
+        'ko', 'kn', 'vi', 'sr', 'th', 'hi', 'ro', 'id', 'no', 'et', 'skr',
+        'cs', 'ml', 'my', 'uz', 'li', 'eo', 'or', 'te', 'fa', 'gl', 'ar', 'oc',
+        'sg', 'jv', 'is', 'az', 'uk', 'eu', 'ast', 'br', 'mnw', 'da', 'bn',
+        'simple', 'lo', 'la', 'hr', 'shn', 'sk', 'fj', 'ky', 'wa', 'bg', 'ur',
+        'cy', 'ps', 'tg', 'lmo', 'he', 'vo', 'om', 'sl', 'af', 'kbd',
         'zh-min-nan', 'scn', 'ms', 'tl', 'pa', 'fy', 'sw', 'ka', 'nn', 'min',
-        'lv', 'sq', 'nds', 'gor', 'lb', 'co', 'mn', 'pnb', 'bs', 'nah', 'yue',
-        'sa', 'kk', 'km', 'ckb', 'vec', 'be', 'diq', 'tk', 'mk', 'nia', 'sm',
-        'hsb', 'ks', 'shy', 'su', 'bcl', 'gd', 'ga', 'an', 'gom', 'mr', 'wo',
-        'mni', 'bjn', 'ia', 'ang', 'mt', 'fo', 'sd', 'tt', 'gn', 'so', 'ie',
-        'ha', 'mi', 'csb', 'ug', 'si', 'guw', 'st', 'hif', 'roa-rup', 'jbo',
-        'kl', 'zu', 'ay', 'yi', 'ln', 'gu', 'na', 'gv', 'kw', 'tpi', 'kcg',
+        'lv', 'kk', 'gor', 'nds', 'sq', 'lb', 'co', 'mn', 'bs', 'pnb', 'nah',
+        'yue', 'ckb', 'sa', 'km', 'be', 'vec', 'diq', 'tk', 'nia', 'mk', 'sm',
+        'hsb', 'ks', 'shy', 'su', 'ga', 'bcl', 'gd', 'an', 'gom', 'mr', 'wo',
+        'mni', 'bjn', 'ia', 'ang', 'mt', 'sd', 'fo', 'tt', 'ha', 'gn', 'so',
+        'si', 'ie', 'mi', 'csb', 'ug', 'guw', 'st', 'hif', 'roa-rup', 'jbo',
+        'kl', 'zu', 'ay', 'ln', 'yi', 'gu', 'na', 'gv', 'kw', 'tpi', 'kcg',
         'am', 'ne', 'rw', 'ts', 'ig', 'qu', 'ss', 'iu', 'chr', 'dv', 'ti',
-        'tn', 'kbd',
+        'tn',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'zh': ('分类重定向',),
     }
```

### Comparing `pywikibot-8.1.2/pywikibot/families/wowwiki_family.py` & `pywikibot-8.2.0/pywikibot/families/wowwiki_family.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 class Family(family.FandomFamily):
 
     """Family class for WOW Wiki."""
 
     name = 'wowwiki'
     domain = 'wowwiki.fandom.com'
 
-    codes = (
+    codes = [
         'ar', 'cs', 'da', 'de', 'el', 'en', 'es', 'et', 'fa', 'fi', 'fr', 'he',
         'hu', 'it', 'ja', 'ko', 'nl', 'no', 'pl', 'pt', 'pt-br', 'ru', 'uk',
         'zh', 'zh-tw',
-    )
+    ]
 
     removed_wikis = ['is', 'hr', 'lt', 'lv', 'ro', 'sk', 'sr', 'sv', 'tr']
 
     code_aliases = {'nn': 'no'}
 
     @classproperty
     def langs(cls):
```

### Comparing `pywikibot-8.1.2/pywikibot/family.py` & `pywikibot-8.2.0/pywikibot/family.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Objects representing MediaWiki families."""
 #
-# (C) Pywikibot team, 2004-2022
+# (C) Pywikibot team, 2004-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import collections
 import logging
 import string
 import sys
@@ -14,17 +14,19 @@
 from importlib import import_module
 from itertools import chain
 from os.path import basename, dirname, splitext
 from typing import Optional
 
 import pywikibot
 from pywikibot import config
-from pywikibot.backports import (  # skipcq: PY-W2000
+from pywikibot.backports import (
     Dict,
+    FrozenSet,
     List,
+    Mapping,
     Set,
     Tuple,
     removesuffix,
 )
 from pywikibot.exceptions import FamilyMaintenanceWarning, UnknownFamilyError
 from pywikibot.tools import classproperty, deprecated, remove_last_args
 
@@ -41,14 +43,16 @@
 class Family:
 
     """Parent singleton class for all wiki families.
 
     .. versionchanged:: 8.0
        ``alphabetic``, ``alphabetic_revised`` and ``fyinterwiki``
        attributes where removed.
+    .. versionchanged:: 8.2
+       :attr:`obsolete` setter was removed.
     """
 
     def __new__(cls):
         """Allocator."""
         # any Family class defined in this file are abstract
         if cls in globals().values():
             raise TypeError(
@@ -78,14 +82,27 @@
         """Get the singleton instance."""
         # This is a placeholder to invoke allocator before it's allocated.
         # Allocator will override this classproperty.
         return cls()
 
     name = None
 
+    #: Not open for edits; stewards can still edit.
+    closed_wikis: List[str] = []
+
+    #: Completely removed sites
+    removed_wikis: List[str] = []
+
+    code_aliases: Dict[str, str] = {}
+    """Code mappings which are only an alias, and there is no 'old' wiki.
+
+    For all except 'nl_nds', subdomains do exist as a redirect, but that
+    should not be relied upon.
+    """
+
     langs: Dict[str, str] = {}
 
     # A list of category redirect template names in different languages
     category_redirect_templates = {
         '_default': []
     }
 
@@ -157,23 +174,14 @@
 
     # Some families, e. g. commons and meta, are not multilingual and
     # forward interlanguage links to another family (wikipedia).
     # These families can set this variable to the name of the target
     # family.
     interwiki_forward = None
 
-    # Which language codes no longer exist and by which language code
-    # should they be replaced. If for example the language with code xx:
-    # now should get code yy:, add {'xx':'yy'} to obsolete.
-    interwiki_replacements: Dict[str, str] = {}
-
-    # Codes that should be removed, usually because the site has been
-    # taken down.
-    interwiki_removals: List[str] = []
-
     # Language codes of the largest wikis. They should be roughly sorted
     # by size.
     languages_by_size: List[str] = []
 
     # Some languages belong to a group where the possibility is high that
     # equivalent articles have identical titles among the group.
     language_groups = {
@@ -316,20 +324,18 @@
                 warnings.simplefilter('ignore', RuntimeWarning)
                 sys.path.append(dirname(family_file))
                 mod = import_module(splitext(basename(family_file))[0])
         except ImportError:
             raise UnknownFamilyError(f'Family {fam} does not exist')
         cls = mod.Family.instance
         if cls.name != fam:
-            warnings.warn(
-                'Family name {} does not match family module name {}'
-                .format(cls.name, fam),
-                FamilyMaintenanceWarning,
-                stacklevel=2,
-            )
+            warnings.warn(f'Family name {cls.name} does not match family '
+                          f'module name {fam}',
+                          FamilyMaintenanceWarning,
+                          stacklevel=2)
         # Family 'name' and the 'langs' codes must be ascii letters and digits,
         # and codes must be lower-case due to the Site loading algorithm;
         # codes can accept also underscore/dash.
         if not all(x in NAME_CHARACTERS for x in cls.name):
             warnings.warn(
                 'Name of family {} must be ASCII letters and digits '
                 '[a-zA-Z0-9]'.format(cls.name),
@@ -411,28 +417,30 @@
         if code in self.disambiguationTemplates:
             return self.disambiguationTemplates[code]
 
         if fallback:
             return self.disambiguationTemplates[fallback]
 
         raise KeyError(
-            'ERROR: title for disambig template in language {} unknown'
-            .format(code))
+            f'ERROR: title for disambig template in language {code} unknown')
 
     # Methods
     def protocol(self, code: str) -> str:
-        """
-        The protocol to use to connect to the site.
+        """The protocol to use to connect to the site.
 
-        May be overridden to return 'https'. Other protocols are not supported.
+        May be overridden to return 'http'. Other protocols are not
+        supported.
+
+        .. versionchanged:: 8.2
+           ``https`` is returned instead of ``http``.
 
         :param code: language code
         :return: protocol that this family uses
         """
-        return 'http'
+        return 'https'
 
     def verify_SSL_certificate(self, code: str) -> bool:
         """
         Return whether a HTTPS certificate should be verified.
 
         .. versionadded:: 5.3
            renamed from ignore_certificate_error
@@ -524,20 +532,19 @@
         """
         raise NotImplementedError('This family does not support EventStreams')
 
     def get_address(self, code, title) -> str:
         """Return the path to title using index.php with redirects disabled."""
         return f'{self.path(code)}?title={title}&redirect=no'
 
-    def interface(self, code) -> str:
+    def interface(self, code: str) -> str:
         """Return interface to use for code."""
         if code in self.interwiki_removals:
             if code in self.codes:
-                pywikibot.warn('Interwiki removal {} is in {} codes'
-                               .format(code, self))
+                pywikibot.warn(f'Interwiki removal {code} is in {self} codes')
             if code in self.closed_wikis:
                 return 'ClosedSite'
             if code in self.removed_wikis:
                 return 'RemovedSite'
 
         return config.site_interface
 
@@ -687,24 +694,14 @@
 
         :return: mapping of old codes to new codes (or None)
         """
         data = {code: None for code in self.interwiki_removals}
         data.update(self.interwiki_replacements)
         return types.MappingProxyType(data)
 
-    @obsolete.setter
-    def obsolete(self, data) -> None:
-        """Split obsolete dict into constituent parts."""
-        self.interwiki_removals[:] = [old for (old, new) in data.items()
-                                      if new is None]
-        self.interwiki_replacements.clear()
-        self.interwiki_replacements.update((old, new)
-                                           for (old, new) in data.items()
-                                           if new is not None)
-
     @classproperty
     def domains(cls) -> Set[str]:
         """
         Get list of unique domain names included in this family.
 
         These domains may also exist in another family.
         """
@@ -715,14 +712,40 @@
         """
         Get list of codes used by this family.
 
         :rtype: set of str
         """
         return set(cls.langs.keys())
 
+    @classproperty
+    def interwiki_replacements(cls) -> Mapping[str, str]:
+        """Return an interwiki code replacement mapping.
+
+        Which language codes no longer exist and by which language code
+        should they be replaced. If for example the language with code
+        xx: now should get code yy:, add {'xx':'yy'} to
+        :attr:`code_aliases`.
+
+        .. versionchanged:: 8.2
+           changed from dict to invariant mapping.
+        """
+        return types.MappingProxyType(cls.code_aliases)
+
+    @classproperty
+    def interwiki_removals(cls) -> FrozenSet[str]:
+        """Return a list of interwiki codes to be removed from wiki pages.
+
+        Codes that should be removed, usually because the site has been
+        taken down.
+
+        .. versionchanged:: 8.2
+           changed from list to invariant frozenset.
+        """
+        return frozenset(cls.removed_wikis + cls.closed_wikis)
+
 
 class SingleSiteFamily(Family):
 
     """Single site family."""
 
     def __new__(cls):
         """Initializer."""
@@ -757,35 +780,31 @@
     @classproperty
     def langs(cls):
         """Property listing family languages."""
         codes = cls.codes[:]
 
         if hasattr(cls, 'test_codes'):
             codes += cls.test_codes
-        if hasattr(cls, 'closed_wikis'):
-            codes += cls.closed_wikis
 
-        # shortcut this classproperty
-        cls.langs = {code: f'{code}.{cls.domain}'
-                     for code in codes}
+        codes += cls.closed_wikis
 
-        if hasattr(cls, 'code_aliases'):
-            cls.langs.update({alias: f'{code}.{cls.domain}'
-                              for alias, code in cls.code_aliases.items()})
+        # shortcut this classproperty
+        cls.langs = {code: f'{code}.{cls.domain}' for code in codes}
+        cls.langs.update({alias: f'{code}.{cls.domain}'
+                          for alias, code in cls.code_aliases.items()})
 
         return cls.langs
 
     @classproperty
     def codes(cls):
         """Property listing family codes."""
         if cls.languages_by_size:
             return cls.languages_by_size
         raise NotImplementedError(
-            'Family {} needs property "languages_by_size" or "codes"'
-            .format(cls.name))
+            f'Family {cls.name} needs property "languages_by_size" or "codes"')
 
     @classproperty
     def domains(cls):
         """Return the domain name of the sites in this family."""
         return [cls.domain]
 
 
@@ -803,18 +822,14 @@
         codes = cls.codes
 
         if hasattr(cls, 'code_aliases'):
             codes += tuple(cls.code_aliases.keys())
 
         return {code: cls.domain for code in codes}
 
-    def protocol(self, code) -> str:
-        """Return 'https' as the protocol."""
-        return 'https'
-
     def scriptpath(self, code):
         """Return the script path for this family."""
         return '' if code == 'en' else ('/' + code)
 
 
 class WikimediaFamily(Family):
 
@@ -930,19 +945,14 @@
         # Miss-spelling
         'nds_nl': 'nds-nl',
 
         # Renamed, see T11823
         'be-x-old': 'be-tarask',
     }
 
-    # Not open for edits; stewards can still edit.
-    closed_wikis: List[str] = []
-    # Completely removed
-    removed_wikis: List[str] = []
-
     # WikimediaFamily uses Wikibase for the category name containing
     # disambiguation pages for the various languages. We need the
     # Wikibase code and item number:
     disambcatname = {'wikidata': 'Q1982926'}
 
     # UrlShortener extension is only usable on metawiki, and this wiki can
     # process links to all WM domains.
@@ -956,32 +966,18 @@
             return cls.name + '.org'
         if cls.name in cls.wikimedia_org_families:
             return 'wikimedia.org'
 
         raise NotImplementedError(
             f"Family {cls.name} needs to define property 'domain'")
 
-    @classproperty
-    def interwiki_removals(cls):
-        """Return a list of interwiki codes to be removed from wiki pages."""
-        return frozenset(cls.removed_wikis + cls.closed_wikis)
-
-    @classproperty
-    def interwiki_replacements(cls):
-        """Return an interwiki code replacement mapping."""
-        return types.MappingProxyType(cls.code_aliases)
-
     def shared_image_repository(self, code):
         """Return Wikimedia Commons as the shared image repository."""
         return ('commons', 'commons')
 
-    def protocol(self, code) -> str:
-        """Return 'https' as the protocol."""
-        return 'https'
-
     def eventstreams_host(self, code) -> str:
         """Return 'https://stream.wikimedia.org' as the stream hostname."""
         return 'https://stream.wikimedia.org'
 
     def eventstreams_path(self, code) -> str:
         """Return path for EventStreams."""
         return '/v2/stream'
@@ -993,14 +989,108 @@
 
     @classproperty
     def domain(cls) -> str:
         """Return the parents domain with a subdomain prefix."""
         return f'{cls.name}.wikimedia.org'
 
 
+class WikibaseFamily(Family):
+
+    """A base class for a Wikibase Family.
+
+    .. versionadded:: 8.2
+    """
+
+    def interface(self, code) -> str:
+        """Return 'DataSite' for Wikibase family."""
+        return 'DataSite'
+
+    def entity_sources(self, code: str) -> Dict[str, Tuple[str, str]]:
+        """Provide reopsitory site information for entity types.
+
+        The result must be structured as follows:
+
+            {<entity type>: (<family code>, <family name>)}
+
+        for example:
+
+            {'property': ('test', 'wikidata')}
+
+        If an empty dict is returned, all entity types are found in the
+        current ``DataSite``.
+
+        The result is used by :meth:`DataSite.get_repo_for_entity_type
+        <pywikibot.site._datasite.DataSite.get_repo_for_entity_type>`
+        """
+        return {}
+
+
+class DefaultWikibaseFamily(WikibaseFamily):
+
+    """A base class for a Wikimedia Wikibase Family.
+
+    This class holds defauls for :meth:`calendarmodel`,
+    :meth:`default_globe` and :meth:`globes` to prevent code duplication.
+
+    .. warning:: Possibly you have to adjust the repository site in
+       :meth:`WikibaseFamily.entity_sources` to get the valid entity.
+
+    .. versionadded:: 8.2
+    """
+
+    def calendarmodel(self, code) -> str:
+        """Default calendar model for WbTime datatype."""
+        return 'http://www.wikidata.org/entity/Q1985727'
+
+    def default_globe(self, code) -> str:
+        """Default globe for Coordinate datatype."""
+        return 'earth'
+
+    def globes(self, code):
+        """Supported globes for Coordinate datatype."""
+        return {
+            'ariel': 'http://www.wikidata.org/entity/Q3343',
+            'bennu': 'http://www.wikidata.org/entity/Q11558',
+            'callisto': 'http://www.wikidata.org/entity/Q3134',
+            'ceres': 'http://www.wikidata.org/entity/Q596',
+            'deimos': 'http://www.wikidata.org/entity/Q7548',
+            'dione': 'http://www.wikidata.org/entity/Q15040',
+            'earth': 'http://www.wikidata.org/entity/Q2',
+            'enceladus': 'http://www.wikidata.org/entity/Q3303',
+            'eros': 'http://www.wikidata.org/entity/Q16711',
+            'europa': 'http://www.wikidata.org/entity/Q3143',
+            'ganymede': 'http://www.wikidata.org/entity/Q3169',
+            'gaspra': 'http://www.wikidata.org/entity/Q158244',
+            'hyperion': 'http://www.wikidata.org/entity/Q15037',
+            'iapetus': 'http://www.wikidata.org/entity/Q17958',
+            'io': 'http://www.wikidata.org/entity/Q3123',
+            'jupiter': 'http://www.wikidata.org/entity/Q319',
+            'lutetia': 'http://www.wikidata.org/entity/Q107556',
+            'mars': 'http://www.wikidata.org/entity/Q111',
+            'mercury': 'http://www.wikidata.org/entity/Q308',
+            'mimas': 'http://www.wikidata.org/entity/Q15034',
+            'miranda': 'http://www.wikidata.org/entity/Q3352',
+            'moon': 'http://www.wikidata.org/entity/Q405',
+            'oberon': 'http://www.wikidata.org/entity/Q3332',
+            'phobos': 'http://www.wikidata.org/entity/Q7547',
+            'phoebe': 'http://www.wikidata.org/entity/Q17975',
+            'pluto': 'http://www.wikidata.org/entity/Q339',
+            'rhea': 'http://www.wikidata.org/entity/Q15050',
+            'ryugu': 'http://www.wikidata.org/entity/Q1385178',
+            'steins': 'http://www.wikidata.org/entity/Q150249',
+            'tethys': 'http://www.wikidata.org/entity/Q15047',
+            'titan': 'http://www.wikidata.org/entity/Q2565',
+            'titania': 'http://www.wikidata.org/entity/Q3322',
+            'triton': 'http://www.wikidata.org/entity/Q3359',
+            'umbriel': 'http://www.wikidata.org/entity/Q3338',
+            'venus': 'http://www.wikidata.org/entity/Q313',
+            'vesta': 'http://www.wikidata.org/entity/Q3030',
+        }
+
+
 def AutoFamily(name: str, url: str) -> SingleSiteFamily:
     """
     Family that automatically loads the site configuration.
 
     :param name: Name for the family
     :param url: API endpoint URL of the wiki
     :return: Generated family class
```

### Comparing `pywikibot-8.1.2/pywikibot/fixes.py` & `pywikibot-8.2.0/pywikibot/fixes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/flow.py` & `pywikibot-8.2.0/pywikibot/flow.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/i18n.py` & `pywikibot-8.2.0/pywikibot/i18n.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,17 +479,16 @@
         for number, plural in re.findall(
             r'(?!$)(?: *(\d+) *= *)?(.*?)(?:\||$)', variants
         ):
             if number:
                 specific_entries[int(number)] = plural
             else:
                 assert not specific_entries, (
-                    'generic entries defined after specific in "{}"'
-                    .format(variants))
-                plural_entries += [plural]
+                    f'generic entries defined after specific in "{variants}"')
+                plural_entries.append(plural)
 
         if num in specific_entries:
             return specific_entries[num]
 
         assert callable(plural_value)
 
         index = plural_value(num)
@@ -621,16 +620,16 @@
             codes.extend(fallback)
         for code in codes:
             if code in lookup:
                 trans = lookup[code]
                 break
         else:
             if fallback is not False:
-                raise KeyError('No fallback key found in lookup dict for "{}"'
-                               .format(code))
+                raise KeyError(
+                    f'No fallback key found in lookup dict for "{code}"')
             trans = None
 
     if trans is None:
         if isinstance(xdict, dict) and 'wikipedia' in xdict:
             # fallback to wikipedia family
             return translate(code, xdict['wikipedia'],
                              parameters=parameters, fallback=fallback)
@@ -871,15 +870,15 @@
     localized.
 
     With ``stem=True`` the bundle names are given:
 
     >>> from pywikibot import i18n
     >>> bundles = sorted(i18n.bundles(stem=True))
     >>> len(bundles)
-    37
+    38
     >>> bundles[:4]
     ['add_text', 'archivebot', 'basic', 'blockpageschecker']
     >>> bundles[-5:]
     ['undelete', 'unprotect', 'unusedfiles', 'weblinkchecker', 'welcome']
     >>> 'pywikibot' in bundles
     True
 
@@ -908,15 +907,15 @@
 
     >>> from pywikibot import i18n
     >>> i18n.known_languages()[:10]
     ['ab', 'aeb', 'af', 'am', 'an', 'ang', 'anp', 'ar', 'arc', 'ary']
     >>> i18n.known_languages()[-10:]
     ['vo', 'vro', 'wa', 'war', 'xal', 'xmf', 'yi', 'yo', 'yue', 'zh']
     >>> len(i18n.known_languages())
-    253
+    252
 
     The implementation is roughly equivalent to:
 
     .. code-block:: Python
 
        langs = set()
        for dirpath in bundles():
```

### Comparing `pywikibot-8.1.2/pywikibot/interwiki_graph.py` & `pywikibot-8.2.0/pywikibot/interwiki_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,16 +158,15 @@
                 oppositeEdge = oppositeEdge[0]
                 oppositeEdge.set_dir('both')
             # workaround for sf.net bug 401: prevent duplicate edges
             # (it is unclear why duplicate edges occur)
             # https://sourceforge.net/p/pywikipediabot/bugs/401/
             elif self.graph.get_edge(sourceLabel, targetLabel):
                 pywikibot.error(
-                    'Tried to create duplicate edge from {} to {}'
-                    .format(refPage, page))
+                    f'Tried to create duplicate edge from {refPage} to {page}')
                 # duplicate edges would be bad because then get_edge() would
                 # give a list of edges, not a single edge when we handle the
                 # opposite edge.
             else:
                 # add edge
                 if refPage.site == page.site:
                     edge.set_color('blue')
@@ -190,16 +189,15 @@
 
     def createGraph(self) -> None:
         """
         Create graph of the interwiki links.
 
         For more info see https://meta.wikimedia.org/wiki/Interwiki_graphs
         """
-        pywikibot.info('Preparing graph for {}'
-                       .format(self.subject.origin.title()))
+        pywikibot.info(f'Preparing graph for {self.subject.origin.title()}')
         # create empty graph
         self.graph = pydot.Dot()
 
         self.octagon_sites = self._octagon_site_set()
 
         for page in self.subject.found_in.keys():
             # a node for each found page
```

### Comparing `pywikibot-8.1.2/pywikibot/logentries.py` & `pywikibot-8.2.0/pywikibot/logentries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Objects representing Mediawiki log entries."""
 #
-# (C) Pywikibot team, 2007-2022
+# (C) Pywikibot team, 2007-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import datetime
 from collections import UserDict
 from typing import Any, Optional, Type, Union
 
@@ -60,21 +60,20 @@
         for hidden_key, hidden_types in hidden.items():
             if hidden_key in self and key in hidden_types:
                 raise HiddenKeyError(
                     "Log entry ({}) has a hidden '{}' key and you don't have "
                     "permission to view it due to '{}'"
                     .format(self['type'], key, hidden_key))
 
-        raise KeyError('Log entry ({}) has no {!r} key'
-                       .format(self['type'], key))
+        raise KeyError(f"Log entry ({self['type']}) has no {key!r} key")
 
     def __repr__(self) -> str:
         """Return a string representation of LogEntry object."""
-        return '<{}({}, logid={})>'.format(type(self).__name__,
-                                           self.site.sitename, self.logid())
+        return (f'<{type(self).__name__}({self.site.sitename}, '
+                f'logid={self.logid()})>')
 
     def __hash__(self) -> int:
         """Combine site and logid as the hash."""
         return self.logid() ^ hash(self.site)
 
     def __eq__(self, other: Any) -> bool:
         """Compare if self is equal to other."""
```

### Comparing `pywikibot-8.1.2/pywikibot/logging.py` & `pywikibot-8.2.0/pywikibot/logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/login.py` & `pywikibot-8.2.0/pywikibot/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,17 +374,16 @@
 
         .. versionchanged:: 8.0
            2FA login was enabled.
         """
         if hasattr(self, '_waituntil') \
            and datetime.datetime.now() < self._waituntil:
             diff = self._waituntil - datetime.datetime.now()
-            pywikibot.warning(
-                'Too many tries, waiting {} seconds before retrying.'
-                .format(diff.seconds))
+            pywikibot.warning(f'Too many tries, waiting {diff.seconds}'
+                              ' seconds before retrying.')
             pywikibot.sleep(diff.seconds)
 
         self.site._loginstatus = LoginStatus.IN_PROGRESS
 
         # Bot passwords username contains @,
         # otherwise @ is not allowed in usernames.
         # @ in bot password is deprecated,
```

### Comparing `pywikibot-8.1.2/pywikibot/page/__init__.py` & `pywikibot-8.2.0/pywikibot/page/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/page/_basepage.py` & `pywikibot-8.2.0/pywikibot/page/_basepage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1320,16 +1320,16 @@
         cc = cc and self.site.lang not in config.cosmetic_changes_disable.get(
             family, [])
         cc = cc and self._check_bot_may_edit('cosmetic_changes')
         if not cc:
             return summary
 
         old = self.text
-        pywikibot.log('Cosmetic changes for {}-{} enabled.'
-                      .format(family, self.site.lang))
+        pywikibot.log(
+            f'Cosmetic changes for {family}-{self.site.lang} enabled.')
         # cc depends on page directly and via several other imports
         cc_toolkit = CosmeticChangesToolkit(self, ignore=CANCEL.MATCH)
         self.text = cc_toolkit.change(old)
 
         if summary and old.strip().replace(
                 '\r\n', '\n') != self.text.strip().replace('\r\n', '\n'):
             summary += i18n.twtranslate(self.site,
@@ -1892,16 +1892,16 @@
             return 0
 
         # Otherwise mark it for deletion
         if mark or hasattr(self.site, '_noMarkDeletePrompt'):
             answer = 'y'
         else:
             answer = pywikibot.input_choice(
-                "Can't delete {}; do you want to mark it for deletion instead?"
-                .format(self),
+                f"Can't delete {self};"
+                ' do you want to mark it for deletion instead?',
                 [('Yes', 'y'), ('No', 'n'), ('All', 'a')],
                 'n', automatic_quit=False)
             if answer == 'a':
                 answer = 'y'
                 self.site._noMarkDeletePrompt = True
         if answer == 'y':
             template = '{{delete|1=%s}}\n' % reason
@@ -1976,16 +1976,15 @@
 
         :param undelete: if False, mark the revision to remain deleted.
         """
         if not hasattr(self, '_deletedRevs'):
             self.loadDeletedRevisions()
         if timestamp not in self._deletedRevs:
             raise ValueError(
-                'Timestamp {} is not a deleted revision'
-                .format(timestamp))
+                f'Timestamp {timestamp} is not a deleted revision')
         self._deletedRevs[timestamp]['marked'] = undelete
 
     def undelete(self, reason: Optional[str] = None) -> None:
         """
         Undelete revisions based on the markers set by previous calls.
 
         If no calls have been made since loadDeletedRevisions(), everything
@@ -2102,16 +2101,16 @@
 
         if not self.has_permission():
             pywikibot.info(f"Can't edit {self}, skipping it...")
             return False
 
         if old_cat not in cats:
             if self.namespace() != 10:
-                pywikibot.error('{} is not in category {}!'
-                                .format(self, old_cat.title()))
+                pywikibot.error(
+                    f'{self} is not in category {old_cat.title()}!')
             else:
                 pywikibot.info('{} is not in category {}, skipping...'
                                .format(self, old_cat.title()))
             return False
 
         # This prevents the bot from adding new_cat if it is already present.
         if new_cat in cats:
```

### Comparing `pywikibot-8.1.2/pywikibot/page/_category.py` & `pywikibot-8.2.0/pywikibot/page/_category.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Object representing a MediaWiki category page."""
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from collections import defaultdict
 from typing import Any, Optional, Union
 
 import pywikibot
@@ -24,16 +24,16 @@
         Initializer.
 
         All parameters are the same as for Page() Initializer.
         """
         self.sortKey = sort_key
         super().__init__(source, title, ns=14)
         if self.namespace() != 14:
-            raise ValueError("'{}' is not in the category namespace!"
-                             .format(self.title()))
+            raise ValueError(
+                f"'{self.title()}' is not in the category namespace!")
 
     def aslink(self, sort_key: Optional[str] = None) -> str:
         """Return a link to place a page in this Category.
 
         .. warning:: Use this only to generate a "true" category link,
            not for interwikis or text links to category pages.
 
@@ -346,13 +346,13 @@
             cached = check_cache(pywikibot.Timestamp.fromISOformat(
                 member['timestamp']))
             yield from cached
             if total is not None:
                 total -= len(cached)
                 if total <= 0:
                     break
-            cache[page.oldest_revision.timestamp] += [page]
+            cache[page.oldest_revision.timestamp].append(page)
         else:
             # clear cache
             assert total is None or total > 0, \
                 'As many items as given in total already returned'
             yield from check_cache(pywikibot.Timestamp.min)
```

### Comparing `pywikibot-8.1.2/pywikibot/page/_collections.py` & `pywikibot-8.2.0/pywikibot/page/_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,28 +521,26 @@
                         obj.__class__.__name__))
 
     def __getitem__(self, index):
         if isinstance(index, str):
             try:
                 index = self._by_key[index]
             except KeyError as e:
-                raise ValueError('No entity with id {} was found'
-                                 .format(index)) from e
+                raise ValueError(f'No entity with id {index} was found') from e
         return self._data[index]
 
     def __setitem__(self, index, value):
         raise NotImplementedError
 
     def __delitem__(self, index):
         if isinstance(index, str):
             try:
                 index = self._by_key[index]
             except KeyError as e:
-                raise ValueError('No entity with id {} was found'
-                                 .format(index)) from e
+                raise ValueError(f'No entity with id {index} was found') from e
         obj = self._data[index]
         del self._data[index]
         del self._by_key[obj.id]
 
     def __len__(self):
         return len(self._data)
```

### Comparing `pywikibot-8.1.2/pywikibot/page/_decorators.py` & `pywikibot-8.2.0/pywikibot/page/_decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,16 +33,15 @@
         try:
             func(self, *args, **kwargs)
         # TODO: other "expected" error types to catch?
         except Error as edit_err:
             err = edit_err  # edit_err will be deleted in the end of the scope
             link = self.title(as_link=True)
             if do_async:
-                pywikibot.error('page {} not saved due to {}\n'
-                                .format(link, err))
+                pywikibot.error(f'page {link} not saved due to {err}\n')
             pywikibot.log(f'Error saving page {link} ({err})\n',
                           exc_info=True)
             if not callback and not do_async:
                 if isinstance(err, PageSaveRelatedError):
                     raise err
                 raise OtherPageSaveError(self, err)
         if callback:
```

### Comparing `pywikibot-8.1.2/pywikibot/page/_filepage.py` & `pywikibot-8.2.0/pywikibot/page/_filepage.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,22 @@
 * FileInfo: a structure holding imageinfo of latest revision of FilePage
 """
 #
 # (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
-import os.path
 from http import HTTPStatus
+from os import PathLike
+from pathlib import Path
+from typing import Optional, Union
+from urllib.parse import urlparse
 
 import pywikibot
+from pywikibot.backports import Iterable
 from pywikibot.comms import http
 from pywikibot.exceptions import NoPageError
 from pywikibot.page._page import Page
 from pywikibot.tools import compute_file_hash, deprecated
 
 
 __all__ = (
@@ -35,24 +39,23 @@
     """
 
     def __init__(self, source, title: str = '') -> None:
         """Initializer."""
         self._file_revisions = {}  # dictionary to cache File history.
         super().__init__(source, title, 6)
         if self.namespace() != 6:
-            raise ValueError("'{}' is not in the file namespace!"
-                             .format(self.title()))
+            raise ValueError(f"'{self.title()}' is not in the file namespace!")
 
     def _load_file_revisions(self, imageinfo) -> None:
         for file_rev in imageinfo:
             # filemissing in API response indicates most fields are missing
             # see https://gerrit.wikimedia.org/r/c/mediawiki/core/+/533482/
             if 'filemissing' in file_rev:
-                pywikibot.warning("File '{}' contains missing revisions"
-                                  .format(self.title()))
+                pywikibot.warning(
+                    f"File '{self.title()}' contains missing revisions")
                 continue
             file_revision = FileInfo(file_rev)
             self._file_revisions[file_revision.timestamp] = file_revision
 
     @property
     def latest_file_info(self):
         """
@@ -103,33 +106,39 @@
         """
         if not hasattr(self, '_imagePageHtml'):
             path = '{}/index.php?title={}'.format(self.site.scriptpath(),
                                                   self.title(as_url=True))
             self._imagePageHtml = http.request(self.site, path).text
         return self._imagePageHtml
 
-    def get_file_url(self, url_width=None, url_height=None,
-                     url_param=None) -> str:
-        """
-        Return the url or the thumburl of the file described on this page.
+    def get_file_url(self,
+                     url_width: Optional[int] = None,
+                     url_height: Optional[int] = None,
+                     url_param: Optional[int] = None) -> str:
+        """Return the url or the thumburl of the file described on this page.
 
         Fetch the information if not available.
 
-        Once retrieved, thumburl information will also be accessible as
-        latest_file_info attributes, named as in [1]:
-        - url, thumburl, thumbwidth and thumbheight
-
-        Parameters correspond to iiprops in:
-        [1] :api:`Imageinfo`
-
-        Parameters validation and error handling left to the API call.
-
-        :param url_width: see iiurlwidth in [1]
-        :param url_height: see iiurlheigth in [1]
-        :param url_param: see iiurlparam in [1]
+        Once retrieved, file information will also be accessible as
+        :attr:`latest_file_info` attributes, named as in :api:`Imageinfo`.
+        If *url_width*, *url_height* or *url_param* is given, additional
+        properties ``thumbwidth``, ``thumbheight``, ``thumburl`` and
+        ``responsiveUrls`` are provided.
+
+        .. note:: Parameters validation and error handling left to the
+           API call.
+        .. seealso::
+
+           * :meth:`APISite.loadimageinfo()
+             <pywikibot.site._apisite.APISite.loadimageinfo>`
+           * :api:`Imageinfo`
+
+        :param url_width: get info for a thumbnail with given width
+        :param url_height: get info for a thumbnail with given height
+        :param url_param:  get info for a thumbnail with given param
         :return: latest file url or thumburl
         """
         # Plain url is requested.
         if url_width is None and url_height is None and url_param is None:
             return self.latest_file_info.url
 
         # Thumburl is requested.
@@ -263,55 +272,105 @@
         if '://' in source:
             url = source
         else:
             filename = source
         return self.site.upload(self, source_filename=filename, source_url=url,
                                 **kwargs)
 
-    def download(self, filename=None, chunk_size=100 * 1024, revision=None):
-        """
-        Download to filename file of FilePage.
+    def download(self,
+                 filename: Union[None, str, PathLike, Iterable[str]] = None,
+                 chunk_size: int = 100 * 1024,
+                 revision: Optional['FileInfo'] = None, *,
+                 url_width: Optional[int] = None,
+                 url_height: Optional[int] = None,
+                 url_param: Optional[int] = None) -> bool:
+        """Download to filename file of FilePage.
+
+        **Usage examples:**
+
+        Download an image:
+
+        >>> site = pywikibot.Site('wikipedia:test')
+        >>> file = pywikibot.FilePage(site, 'Pywikibot MW gear icon.svg')
+        >>> file.download()
+        True
 
-        :param filename: filename where to save file:
-            None: self.title(as_filename=True, with_ns=False)
-            will be used
-            str: provided filename will be used.
-        :type filename: None or str
+        Pywikibot_MW_gear_icon.svg was downloaded.
+
+        Download a thumnail:
+
+        >>> file.download(url_param='120px')
+        True
+
+        The suffix has changed and Pywikibot_MW_gear_icon.png was
+        downloaded.
+
+        .. versionadded:: 8.2
+           *url_width*, *url_height* and *url_param* parameters.
+        .. versionchanged:: 8.2
+           *filename* argument may be also a path-like object or an
+           iterable of path segments.
+        .. note:: filename suffix is adjusted if target url's suffix is
+           different which may be the case if a thumbnail is loaded.
+        .. warning:: If a file already exists, it will be overridden
+           without further notes.
+        .. seealso:: :api:`Imageinfo` for new parameters
+
+        :param filename: filename where to save file. If ``None``,
+            ``self.title(as_filename=True, with_ns=False)`` will be used.
+            If an Iterable is specified the items will be used as path
+            segments. To specify the user directory path you have to use
+            either ``~`` or ``~user`` as first path segment e.g. ``~/foo``
+            or ``('~', 'foo')`` as filename. If only the user directory
+            specifier is given, the title is used as filename like for
+            None. If the suffix is missing or different from url (which
+            can happen if a *url_width*, *url_height* or *url_param*
+            argument is given), the file suffix is adjusted.
         :param chunk_size: the size of each chunk to be received and
             written to file.
-        :type chunk_size: int
-        :param revision: file revision to download:
-            None: self.latest_file_info will be used
-            FileInfo: provided revision will be used.
-        :type revision: None or FileInfo
+        :param revision: file revision to download. If None
+            :attr:`latest_file_info` will be used; otherwise provided
+            revision will be used.
+        :param url_width: download thumbnail with given width
+        :param url_height: download thumbnail with given height
+        :param url_param:  download thumbnail with given param
         :return: True if download is successful, False otherwise.
         :raise IOError: if filename cannot be written for any reason.
         """
-        if filename is None:
-            filename = self.title(as_filename=True, with_ns=False)
+        if not filename:
+            path = Path()
+        elif isinstance(filename, (str, PathLike)):
+            path = Path(filename)
+        else:
+            path = Path(*filename)
 
-        filename = os.path.expanduser(filename)
+        if path.stem in ('', '~', '~user'):
+            path = path / self.title(as_filename=True, with_ns=False)
 
-        if revision is None:
+        thumb = bool(url_width or url_height or url_param)
+        if thumb or revision is None:
+            url = self.get_file_url(url_width, url_height, url_param)
             revision = self.latest_file_info
+        else:
+            url = revision.url
 
-        req = http.fetch(revision.url, stream=True)
+        # adjust suffix
+        path = path.with_suffix(Path(urlparse(url).path).suffix)
+        # adjust user path
+        path = path.expanduser()
+        req = http.fetch(url, stream=True)
         if req.status_code == HTTPStatus.OK:
-            try:
-                with open(filename, 'wb') as f:
-                    for chunk in req.iter_content(chunk_size):
-                        f.write(chunk)
-            except OSError as e:
-                raise e
+            with open(path, 'wb') as f:
+                for chunk in req.iter_content(chunk_size):
+                    f.write(chunk)
+
+            return thumb or compute_file_hash(path) == revision.sha1
 
-            sha1 = compute_file_hash(filename)
-            return sha1 == revision.sha1
         pywikibot.warning(
-            'Unsuccessful request ({}): {}'
-            .format(req.status_code, req.url))
+            f'Unsuccessful request ({req.status_code}): {req.url}')
         return False
 
     def globalusage(self, total=None):
         """
         Iterate all global usage for this page.
 
         .. seealso:: :meth:`using_pages`
```

### Comparing `pywikibot-8.1.2/pywikibot/page/_links.py` & `pywikibot-8.2.0/pywikibot/page/_links.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 .. note::
    `Link` objects defined here represent a wiki-page's title, while
    :class:`pywikibot.Page` objects represent the page itself, including
    its contents.
 """
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import re
 import unicodedata
 from html.entities import name2codepoint
 
@@ -76,16 +76,15 @@
 
     def __repr__(self) -> str:
         """Return a more complete string representation."""
         assert isinstance(self._items, tuple)
         assert all(isinstance(item, str) for item in self._items)
 
         attrs = (f'{getattr(self, attr)!r}' for attr in self._items)
-        return 'pywikibot.page.{}({})'.format(type(self).__name__,
-                                              ', '.join(attrs))
+        return f"pywikibot.page.{type(self).__name__}({', '.join(attrs)})"
 
     def lookup_namespace(self):
         """
         Look up the namespace given the provided namespace id or name.
 
         :rtype: pywikibot.Namespace
         """
@@ -101,17 +100,16 @@
         if isinstance(self._nskey, int):
             try:
                 ns = self.site.namespaces[self._nskey]
             except KeyError:
                 ns = self.site.namespaces[default_nskey]
             return ns
 
-        raise TypeError(
-            'Invalid type "{}" for Page._nskey. Must be int or str.'
-            .format(type(self._nskey)))
+        raise TypeError(f'Invalid type "{type(self._nskey)}" for Page._nskey.'
+                        ' Must be int or str.')
 
     @property
     def site(self):
         """
         Return the site of the link.
 
         :rtype: pywikibot.Site
@@ -131,16 +129,15 @@
             self._namespace = self.lookup_namespace()
         return self._namespace
 
     def canonical_title(self):
         """Return full page title, including localized namespace."""
         # Avoid that ':' will be added to the title for Main ns.
         if self.namespace != Namespace.MAIN:
-            return '{}:{}'.format(self.site.namespace(self.namespace),
-                                  self.title)
+            return f'{self.site.namespace(self.namespace)}:{self.title}'
         return self.title
 
     def ns_title(self, onsite=None):
         """
         Return full page title, including namespace.
 
         :param onsite: site object
@@ -450,44 +447,40 @@
                         raise InvalidTitleError(
                             "The (non-)talk page of '{}' is a valid title "
                             'in another namespace.'.format(self._text))
 
         # Reject illegal characters.
         m = Link.illegal_titles_pattern.search(t)
         if m:
-            raise InvalidTitleError('{!r} contains illegal char(s) {!r}'
-                                    .format(t, m.group(0)))
+            raise InvalidTitleError(f'{t!r} contains illegal char(s) {m[0]!r}')
 
         # Pages with "/./" or "/../" appearing in the URLs will
         # often be unreachable due to the way web browsers deal
         # * with 'relative' URLs. Forbid them explicitly.
 
         if '.' in t and (t in ('.', '..')
                          or t.startswith(('./', '../'))
                          or '/./' in t
                          or '/../' in t
                          or t.endswith(('/.', '/..'))):
             raise InvalidTitleError(
-                "(contains . / combinations): '{}'"
-                .format(self._text))
+                f"(contains . / combinations): '{self._text}'")
 
         # Magic tilde sequences? Nu-uh!
         if '~~~' in t:
-            raise InvalidTitleError("(contains ~~~): '{}'"
-                                    .format(self._text))
+            raise InvalidTitleError(f"(contains ~~~): '{self._text}'")
 
         if self._namespace != -1 and len(t) > 255:
             raise InvalidTitleError(f"(over 255 bytes): '{t}'")
 
         # "empty" local links can only be self-links
         # with a fragment identifier.
         if not t.strip(' ') and not self._is_interwiki:  # T197642
             raise InvalidTitleError(
-                'The link [[{}]] does not contain a page title'
-                .format(self._text))
+                f'The link [[{self._text}]] does not contain a page title')
 
         # MediaWiki uses uppercase IP addresses
         if self._namespace in (2, 3) and is_ip_address(t):
             t = t.upper()
         elif self._site.namespaces[self._namespace].case == 'first-letter':
             t = first_upper(t)
 
@@ -546,15 +539,15 @@
             from the given site; otherwise, present as an internal link on
             the source site.
         """
         if onsite is None:
             onsite = self._source
         text = super().astext(onsite)
         if self.section:
-            text = '{}#{}]]'.format(text.rstrip(']'), self.section)
+            text = f"{text.rstrip(']')}#{self.section}]]"
 
         return text
 
     def _cmpkey(self):
         """
         Key for comparison of Link objects.
```

### Comparing `pywikibot-8.1.2/pywikibot/page/_page.py` & `pywikibot-8.2.0/pywikibot/page/_page.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/page/_revision.py` & `pywikibot-8.2.0/pywikibot/page/_revision.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/page/_toolforge.py` & `pywikibot-8.2.0/pywikibot/page/_toolforge.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/page/_user.py` & `pywikibot-8.2.0/pywikibot/page/_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,15 @@
             title = title[1:]
         elif ':#' in title:
             title = title.replace(':#', ':')
         else:
             self._isAutoblock = False
         super().__init__(source, title, ns=2)
         if self.namespace() != 2:
-            raise ValueError("'{}' is not in the user namespace!"
-                             .format(self.title()))
+            raise ValueError(f"'{self.title()}' is not in the user namespace!")
         if self._isAutoblock:
             # This user is probably being queried for purpose of lifting
             # an autoblock.
             pywikibot.info(
                 'This is an autoblock ID, you can only use to unblock it.')
 
     @property
@@ -271,16 +270,15 @@
 
         :return: None
         """
         try:
             self.site.blockuser(self, *args, **kwargs)
         except APIError as err:
             if err.code == 'invalidrange':
-                raise ValueError('{} is not a valid IP range.'
-                                 .format(self.username))
+                raise ValueError(f'{self.username} is not a valid IP range.')
 
             raise err
 
     def unblock(self, reason: Optional[str] = None) -> None:
         """
         Remove the block for the user.
```

### Comparing `pywikibot-8.1.2/pywikibot/page/_wikibase.py` & `pywikibot-8.2.0/pywikibot/page/_wikibase.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,23 +101,21 @@
         :param id_: Entity identifier.
         :type id_: str or None, -1 and None mean non-existing
         """
         self.repo = repo
         self.id = id_ if id_ is not None else '-1'
         if self.id != '-1' and not self.is_valid_id(self.id):
             raise InvalidTitleError(
-                "'{}' is not a valid {} page title"
-                .format(self.id, self.entity_type))
+                f"'{self.id}' is not a valid {self.entity_type} page title")
 
     def __repr__(self) -> str:
         if self.id != '-1':
             return 'pywikibot.page.{}({!r}, {!r})'.format(
                 self.__class__.__name__, self.repo, self.id)
-        return 'pywikibot.page.{}({!r})'.format(
-            self.__class__.__name__, self.repo)
+        return f'pywikibot.page.{self.__class__.__name__}({self.repo!r})'
 
     @classmethod
     def is_valid_id(cls, entity_id: str) -> bool:
         """
         Whether the string can be a valid id of the entity type.
 
         :param entity_id: The ID to test.
@@ -389,24 +387,22 @@
         """Get the file associated with the mediainfo."""
         if not hasattr(self, '_file'):
             if self.id == '-1':
                 # if the above doesn't apply, this entity is in an invalid
                 # state which needs to be raised as an exception, but also
                 # logged in case an exception handler is catching
                 # the generic Error
-                pywikibot.error('{} is in invalid state'
-                                .format(self.__class__.__name__))
-                raise Error('{} is in invalid state'
-                            .format(self.__class__.__name__))
+                msg = f'{self.__class__.__name__} is in invalid state'
+                pywikibot.error(msg)
+                raise Error(msg)
 
             page_id = self.getID(numeric=True)
             result = list(self.repo.load_pages_from_pageids([page_id]))
             if not result:
-                raise Error('There is no existing page with id "{}"'
-                            .format(page_id))
+                raise Error(f'There is no existing page with id "{page_id}"')
 
             page = result.pop()
             if page.namespace() != page.site.namespaces.FILE:
                 raise Error(f'Page with id "{page_id}" is not a file')
 
             self._file = FilePage(page)
 
@@ -497,25 +493,25 @@
                 # numerical namespace given
                 ns = int(kwargs['ns'])
                 if site.item_namespace.id == ns:
                     self._namespace = site.item_namespace
                 elif site.property_namespace.id == ns:
                     self._namespace = site.property_namespace
                 else:
-                    raise ValueError('{!r}: Namespace "{}" is not valid'
-                                     .format(site, int(ns)))
+                    raise ValueError(
+                        f'{site!r}: Namespace "{int(ns)}" is not valid')
 
         if 'entity_type' in kwargs:
             entity_type = kwargs.pop('entity_type')
             try:
                 entity_type_ns = site.get_namespace_for_entity_type(
                     entity_type)
             except EntityTypeUnknownError:
-                raise ValueError('Wikibase entity type "{}" unknown'
-                                 .format(entity_type))
+                raise ValueError(
+                    f'Wikibase entity type "{entity_type}" unknown')
 
             if self._namespace:
                 if self._namespace != entity_type_ns:
                     raise ValueError('Namespace "{}" is not valid for Wikibase'
                                      ' entity type "{}"'
                                      .format(int(kwargs['ns']), entity_type))
             else:
@@ -539,16 +535,16 @@
             # Use the _link to determine entity type.
             ns = self._link.namespace
             if self.site.item_namespace.id == ns:
                 self._namespace = self.site.item_namespace
             elif self.site.property_namespace.id == ns:
                 self._namespace = self.site.property_namespace
             else:
-                raise ValueError('{!r}: Namespace "{!r}" is not valid'
-                                 .format(self.site, ns))
+                raise ValueError(
+                    f'{self.site!r}: Namespace "{ns!r}" is not valid')
 
         WikibaseEntity.__init__(
             self,
             # .site forces a parse of the Link title to determine site
             self.site,
             # Link.__init__, called from Page.__init__, has cleaned the title
             # stripping whitespace and uppercasing the first letter according
@@ -885,18 +881,16 @@
         elif lazy_loading_id:
             params[site] = self._site.dbName()
             params[title] = self._title
         else:
             # if none of the above applies, this item is in an invalid state
             # which needs to be raise as an exception, but also logged in case
             # an exception handler is catching the generic Error.
-            pywikibot.error('{} is in invalid state'
-                            .format(self.__class__.__name__))
-            raise Error('{} is in invalid state'
-                        .format(self.__class__.__name__))
+            pywikibot.error(f'{self.__class__.__name__} is in invalid state')
+            raise Error(f'{self.__class__.__name__} is in invalid state')
 
         return params
 
     def title(self, **kwargs):
         """
         Return ID as title of the ItemPage.
 
@@ -956,16 +950,15 @@
             ItemPage for the page
         :raise pywikibot.exceptions.WikiBaseError: The site of the page
             has no data repository.
         """
         if hasattr(page, '_item'):
             return page._item
         if not page.site.has_data_repository:
-            raise WikiBaseError('{} has no data repository'
-                                .format(page.site))
+            raise WikiBaseError(f'{page.site} has no data repository')
         if not lazy_load and not page.exists():
             raise NoPageError(page)
 
         repo = page.site.data_repository()
         if hasattr(page,
                    '_pageprops') and page.properties().get('wikibase_item'):
             # If we have already fetched the pageprops for something else,
@@ -1074,15 +1067,16 @@
                 pg = pywikibot.Page(sl)
                 pg._item = self
                 yield pg
 
     def getSitelink(self, site, force: bool = False) -> str:
         """Return the title for the specific site.
 
-        If the item doesn't have that language, raise NoSiteLinkError.
+        If the item doesn't have a link to that site, raise
+        NoSiteLinkError.
 
         .. versionchanged:: 8.1
            raises NoSiteLinkError instead of NoPageError.
 
         :param site: Site to find the linked page of.
         :type site: pywikibot.Site or database name
         :param force: override caching
@@ -1091,15 +1085,17 @@
         :raise IsRedirectPageError: instance is a redirect page
         :raise NoSiteLinkError: site is not in :attr:`sitelinks`
         """
         if force or not hasattr(self, '_content'):
             self.get(force=force)
 
         if site not in self.sitelinks:
-            raise NoSiteLinkError(self, site.lang)
+            if not isinstance(site, str):
+                site = site.dbName()
+            raise NoSiteLinkError(self, site)
 
         return self.sitelinks[site].canonical_title()
 
     def setSitelink(self, sitelink: SITELINK_TYPE, **kwargs) -> None:
         """Set sitelinks. Calls :meth:`setSitelinks`.
 
         A *sitelink* can be a Page object, a BaseLink object or a
@@ -1702,16 +1698,15 @@
         :type value: object
 
         :exception ValueError: if value is not of the type
             required for the Claim type.
         """
         value_class = self.types[self.type]
         if not isinstance(value, value_class):
-            raise ValueError('{} is not type {}.'
-                             .format(value, value_class))
+            raise ValueError(f'{value} is not type {value_class}.')
         self.target = value
 
     def changeTarget(
         self,
         value=None,
         snaktype: str = 'value',
         **kwargs
@@ -1953,17 +1948,14 @@
         self._assert_mainsnak('{}s cannot have qualifiers')
         return any(qualifier.target_equals(target)
                    for qualifier in self.qualifiers.get(qualifier_id, []))
 
     def _formatValue(self) -> dict:
         """Format the target into the proper JSON value that Wikibase wants.
 
-        .. versionchanges:: 8.0
-           normalize the result if type is ``time``.
-
         :return: JSON value
         """
         # todo: eventually unify the following two groups
         if self.type in ('wikibase-item', 'wikibase-property'):
             value = {'entity-type': self.getTarget().entity_type,
                      'numeric-id': self.getTarget().getID(numeric=True)}
         elif self.type in (
@@ -1971,17 +1963,15 @@
             value = {'entity-type': self.getTarget().entity_type,
                      'id': self.getTarget().getID()}
         elif self.type in ('string', 'url', 'math', 'external-id',
                            'musical-notation'):
             value = self.getTarget()
         elif self.type == 'commonsMedia':
             value = self.getTarget().title(with_ns=False)
-        elif self.type == 'time':
-            value = self.getTarget().toWikibase(normalize=True)
-        elif self.type in ('globe-coordinate',
+        elif self.type in ('globe-coordinate', 'time',
                            'quantity', 'monolingualtext',
                            'geo-shape', 'tabular-data'):
             value = self.getTarget().toWikibase()
         else:  # WbUnknown
             pywikibot.warning(
                 f'{self.type} datatype is not supported yet.')
             value = self.getTarget().toWikibase()
```

### Comparing `pywikibot-8.1.2/pywikibot/pagegenerators/__init__.py` & `pywikibot-8.2.0/pywikibot/pagegenerators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,29 +86,30 @@
     YearPageGenerator,
     page_with_property_generator,
 )
 from pywikibot.tools.collections import DequeGenerator
 
 
 __all__ = (
+    # factory
     'GeneratorFactory',
-
+    # filter
     'CategoryFilterPageGenerator',
     'EdittimeFilterPageGenerator',
     'ItemClaimFilterPageGenerator',
     'NamespaceFilterPageGenerator',
     'PageTitleFilterPageGenerator',
     'QualityFilterPageGenerator',
     'RedirectFilterPageGenerator',
     'RegexBodyFilterPageGenerator',
     'RegexFilterPageGenerator',
     'SubpageFilterGenerator',
     'UserEditFilterGenerator',
     'WikibaseItemFilterPageGenerator',
-
+    # page generators
     'AllpagesPageGenerator',
     'AncientPagesPageGenerator',
     'CategorizedPageGenerator',
     'DayPageGenerator',
     'DeadendPagesPageGenerator',
     'FileLinksGenerator',
     'GoogleSearchPageGenerator',
@@ -125,15 +126,14 @@
     'NewimagesPageGenerator',
     'NewpagesPageGenerator',
     'page_with_property_generator',
     'PagesFromPageidGenerator',
     'PagesFromTitlesGenerator',
     'PetScanPageGenerator',
     'PrefixingPageGenerator',
-    'PreloadingGenerator',
     'RandomPageGenerator',
     'RandomRedirectPageGenerator',
     'RecentChangesPageGenerator',
     'SearchPageGenerator',
     'ShortPagesPageGenerator',
     'SubCategoriesPageGenerator',
     'TextIOPageGenerator',
@@ -150,14 +150,21 @@
     'WikibaseSearchItemPageGenerator',
     'WikidataPageFromItemGenerator',
     'WikidataSPARQLPageGenerator',
     'WithoutInterwikiPageGenerator',
     'XMLDumpOldPageGenerator',
     'XMLDumpPageGenerator',
     'YearPageGenerator',
+    # other generators
+    'DequePreloadingGenerator',
+    'PageClassGenerator',
+    'PageWithTalkPageGenerator',
+    'PreloadingEntityGenerator',
+    'PreloadingGenerator',
+    'RepeatingGenerator',
 )
 
 
 parameterHelp = """\
 GENERATOR OPTIONS
 =================
```

### Comparing `pywikibot-8.1.2/pywikibot/pagegenerators/_factory.py` & `pywikibot-8.2.0/pywikibot/pagegenerators/_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """GeneratorFactory module wich handles pagegenerators options."""
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import itertools
 import re
 import sys
 from datetime import timedelta
@@ -324,16 +324,15 @@
             startfrom = None
 
         # Insert "Category:" before category name to avoid parsing problems in
         # Link.parse() when categoryname contains ":";
         # Part before ":" might be interpreted as an interwiki prefix
         prefix = category.split(':', 1)[0]  # whole word if ":" not present
         if prefix not in self.site.namespaces[14]:
-            category = '{}:{}'.format(
-                self.site.namespace(14), category)
+            category = f'{self.site.namespace(14)}:{category}'
         cat = pywikibot.Category(pywikibot.Link(category,
                                                 source=self.site,
                                                 default_namespace=14))
         return cat, startfrom
 
     def getCategoryGen(self, category: str,  # noqa: N802
                        recurse: Union[int, bool] = False,
@@ -831,16 +830,16 @@
                 'Ql filtering needs a site with ProofreadPage extension.')
         int_values = [int(_) for _ in value.split(',')]
         if min(int_values) < 0 or max(int_values) > 4:  # Invalid input ql.
             valid_ql_list = [
                 '{}: {}'.format(*i)
                 for i in self.site.proofread_levels.items()]
             valid_ql = ', '.join(valid_ql_list)
-            pywikibot.warning('Acceptable values for -ql are:\n    {}'
-                              .format(valid_ql))
+            pywikibot.warning(
+                f'Acceptable values for -ql are:\n    {valid_ql}')
         self.qualityfilter_list = int_values
         return True
 
     def _handle_onlyif(self, value: str) -> HANDLER_RETURN_TYPE:
         """Handle `-onlyif` argument."""
         return self._onlyif_onlyifnot_handler(value, False)
```

### Comparing `pywikibot-8.1.2/pywikibot/pagegenerators/_filters.py` & `pywikibot-8.2.0/pywikibot/pagegenerators/_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,16 +228,15 @@
 
     for page in generator:
         if page.depth <= max_depth:
             yield page
         else:
             if show_filtered:
                 pywikibot.info(
-                    'Page {} is a subpage that is too deep. Skipping.'
-                    .format(page))
+                    f'Page {page} is a subpage that is too deep. Skipping.')
 
 
 class RegexFilter:
 
     """Regex filter."""
 
     @classmethod
```

### Comparing `pywikibot-8.1.2/pywikibot/pagegenerators/_generators.py` & `pywikibot-8.2.0/pywikibot/pagegenerators/_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Page filter generators provided by the pagegenerators module."""
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import calendar
 import codecs
 import io
 import re
@@ -18,25 +18,28 @@
 from requests.exceptions import ReadTimeout
 
 import pywikibot
 from pywikibot import config, date, xmlreader
 from pywikibot.backports import (
     Callable,
     Dict,
+    Generator,
     Iterable,
     Iterator,
     List,
     Sequence,
     Tuple,
+    batched,
 )
 from pywikibot.comms import http
 from pywikibot.exceptions import APIError, ServerError
+from pywikibot.site import Namespace
 from pywikibot.tools import deprecated
 from pywikibot.tools.collections import GeneratorWrapper
-from pywikibot.tools.itertools import filter_unique, itergroup
+from pywikibot.tools.itertools import filter_unique
 
 
 OPT_SITE_TYPE = Optional['pywikibot.site.BaseSite']
 OPT_TIMESTAMP_TYPE = Optional['pywikibot.Timestamp']
 NAMESPACE_OR_INT_TYPE = Union[int, 'pywikibot.site.Namespace']
 NAMESPACE_OR_STR_TYPE = Union[str, 'pywikibot.site.Namespace']
 
@@ -165,34 +168,57 @@
     # defaults to namespace 0 because that's how Special:Newpages defaults
     if site is None:
         site = pywikibot.Site()
     return (page for page, _ in site.newpages(namespaces=namespaces,
                                               total=total, returndict=True))
 
 
-def RecentChangesPageGenerator(site: OPT_SITE_TYPE = None,
-                               _filter_unique: Optional[Callable[
-                                   [Iterable['pywikibot.page.Page']],
-                                   Iterable['pywikibot.page.Page']]] = None,
-                               **kwargs: Any
-                               ) -> Iterable['pywikibot.page.Page']:
+def RecentChangesPageGenerator(
+    site: OPT_SITE_TYPE = None,
+    _filter_unique: Optional[Callable[[Iterable['pywikibot.Page']],
+                                      Iterable['pywikibot.Page']]] = None,
+    **kwargs: Any
+) -> Generator['pywikibot.Page', None, None]:
     """
     Generate pages that are in the recent changes list, including duplicates.
 
-    For parameters refer pywikibot.site.recentchanges
+    For keyword parameters refer :meth:`APISite.recentchanges()
+    <pywikibot.site._generators.GeneratorsMixin.recentchanges>`.
+
+    .. versionchanged:: 8.2
+       The YieldType depends on namespace. It can be
+       :class:`pywikibot.Page`, :class:`pywikibot.User`,
+       :class:`pywikibot.FilePage` or :class:`pywikibot.Category`.
 
     :param site: Site for generator results.
     """
+    def upcast(gen):
+        """Upcast pywikibot.Page type."""
+        for rc in gen:
+            # The title in a log entry may have been suppressed
+            if rc['type'] == 'log' and 'title' not in rc:
+                continue
+
+            ns = rc['ns']
+            if ns == Namespace.USER:
+                pageclass = pywikibot.User
+            elif ns == Namespace.FILE:
+                pageclass = pywikibot.FilePage
+            elif ns == Namespace.CATEGORY:
+                pageclass = pywikibot.Category
+            else:
+                pageclass = pywikibot.Page
+            yield pageclass(site, rc['title'])
+
     if site is None:
         site = pywikibot.Site()
 
     gen = site.recentchanges(**kwargs)
     gen.request['rcprop'] = 'title'
-    gen = (pywikibot.Page(site, rc['title'])
-           for rc in gen if rc['type'] != 'log' or 'title' in rc)
+    gen = upcast(gen)
 
     if _filter_unique:
         gen = _filter_unique(gen)
     return gen
 
 
 def UnconnectedPageGenerator(
@@ -428,16 +454,16 @@
     :param site: Site for generator results.
     """
     if site is None:
         site = pywikibot.Site()
 
     user = pywikibot.User(site, username)
     if not (user.isAnonymous() or user.isRegistered()):
-        pywikibot.warning('User "{}" does not exist on site "{}".'
-                          .format(user.username, site))
+        pywikibot.warning(
+            f'User "{user.username}" does not exist on site "{site}".')
 
     gen = (contrib[0] for contrib in user.contributions(
         namespaces=namespaces, total=total))
     if _filter_unique:
         return _filter_unique(gen)
     return gen
 
@@ -845,16 +871,15 @@
         https://de.wikipedia.org/wiki/en:Foobar
 
         .. versionchanged:: 7.6
            changed from iterator method to generator property
         """
         # restrict query to local site
         local_query = f'{self.query} site:{self.site.hostname()}'
-        base = 'http://{}{}'.format(self.site.hostname(),
-                                    self.site.articlepath)
+        base = f'http://{self.site.hostname()}{self.site.articlepath}'
         pattern = base.replace('{}', '(.+)')
         for url in self.queryGoogle(local_query):
             m = re.search(pattern, url)
             if m:
                 page = pywikibot.Page(pywikibot.Link(m[1], self.site))
                 if page.site == self.site:
                     yield page
@@ -1019,16 +1044,16 @@
                                   ) -> Iterator['pywikibot.page.Page']:
     """Generate pages from site based on sitelinks of item pages.
 
     :param gen: generator of :py:obj:`pywikibot.ItemPage`
     :param site: Site for generator results.
     """
     repo = site.data_repository()
-    for sublist in itergroup(gen, 50):
-        req = {'ids': [item.id for item in sublist],
+    for batch in batched(gen, 50):
+        req = {'ids': [item.id for item in batch],
                'sitefilter': site.dbName(),
                'action': 'wbgetentities',
                'props': 'sitelinks'}
 
         wbrequest = repo.simple_request(**req)
         wbdata = wbrequest.submit()
         entities = (item for item in wbdata['entities'].values() if
```

### Comparing `pywikibot-8.1.2/pywikibot/plural.py` & `pywikibot-8.2.0/pywikibot/plural.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/proofreadpage.py` & `pywikibot-8.2.0/pywikibot/proofreadpage.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,16 +513,16 @@
         num: Optional[int] = None
 
         if sep:
             base = left
             try:
                 num = int(right)
             except ValueError:
-                raise InvalidTitleError('{} contains invalid index {!r}'
-                                        .format(self, right))
+                raise InvalidTitleError(
+                    f'{self} contains invalid index {right!r}')
         else:
             base = right
 
         left, sep, right = base.rpartition('.')
         ext = right if sep else ''
 
         return base, ext, num
@@ -558,32 +558,30 @@
                             what_links_here.remove(page)
                             self._index = (page, what_links_here)
                             break
 
         index_page, others = self._index
         if others:
             pywikibot.warning(f'{self} linked to several Index pages.')
-            pywikibot.info('{}{!s}'.format(' ' * 9, [index_page] + others))
+            pywikibot.info(f"{' ' * 9}{[index_page] + others!s}")
 
             if index_page:
                 pywikibot.info(
-                    '{}Selected Index: {}'.format(' ' * 9, index_page))
-                pywikibot.info('{}remaining: {!s}'.format(' ' * 9, others))
+                    f"{' ' * 9}Selected Index: {index_page}")
+                pywikibot.info(f"{' ' * 9}remaining: {others!s}")
 
         if not index_page:
-            pywikibot.warning('Page {} is not linked to any Index page.'
-                              .format(self))
+            pywikibot.warning(f'Page {self} is not linked to any Index page.')
 
         return index_page
 
     @index.setter
     def index(self, value: 'IndexPage') -> None:
         if not isinstance(value, IndexPage):
-            raise TypeError('value {} must be an IndexPage object.'
-                            .format(value))
+            raise TypeError(f'value {value} must be an IndexPage object.')
         self._index = (value, [])
 
     @index.deleter
     def index(self) -> None:
         if hasattr(self, '_index'):
             del self._index
 
@@ -857,16 +855,15 @@
         try:
             url_image = soup.find(class_='prp-page-image')
             # if None raises AttributeError
             url_image = url_image.find('img')
             # if None raises TypeError.
             url_image = url_image['src']
         except (TypeError, AttributeError):
-            raise ValueError('No prp-page-image src found for {}.'
-                             .format(self))
+            raise ValueError(f'No prp-page-image src found for {self}.')
         else:
             url_image = 'https:' + url_image
 
         return url_image
 
     def _ocr_callback(self, cmd_uri: str,
                       parser_func: Optional[Callable[[str], str]] = None,
@@ -886,16 +883,15 @@
             parser_func = identity
 
         if not callable(parser_func):
             raise TypeError('Keyword parser_func must be callable.')
 
         if ocr_tool not in self._OCR_METHODS:
             raise TypeError(
-                "ocr_tool must be in {}, not '{}'."
-                .format(self._OCR_METHODS, ocr_tool))
+                f"ocr_tool must be in {self._OCR_METHODS}, not '{ocr_tool}'.")
 
         # wrong link fail with Exceptions
         for retry in range(5, 30, 5):
             pywikibot.debug(f'{ocr_tool}: get URI {cmd_uri!r}')
             try:
                 response = http.fetch(cmd_uri)
             except ReadTimeout as e:
@@ -979,16 +975,15 @@
             msg = 'ocr_tool required, must be among {}'
             raise TypeError(msg.format(self._OCR_METHODS))
 
         try:
             cmd_fmt = self._OCR_CMDS[ocr_tool]
         except KeyError:
             raise TypeError(
-                "ocr_tool must be in {}, not '{}'."
-                .format(self._OCR_METHODS, ocr_tool))
+                f"ocr_tool must be in {self._OCR_METHODS}, not '{ocr_tool}'.")
 
         params = {
             'url_image': url_image,
             'lang': self.site.lang,
             'user': self.site.user(),
         }
         cmd_uri = cmd_fmt.format_map(params)
@@ -1012,24 +1007,23 @@
         :raise ValueError: something went wrong with OCR process.
         """
         if ocr_tool is None:  # default value
             ocr_tool = self._PHETOOLS
 
         if ocr_tool not in self._OCR_METHODS:
             raise TypeError(
-                "ocr_tool must be in {}, not '{}'."
-                .format(self._OCR_METHODS, ocr_tool))
+                f"ocr_tool must be in {self._OCR_METHODS}, not '{ocr_tool}'.")
 
         # if _multi_page, try _do_hocr() first and fall back to _do_ocr()
         if ocr_tool == self._PHETOOLS and self._multi_page:
             error, text = self._do_hocr()
             if not error and isinstance(text, str):
                 return text
-            pywikibot.warning('{}: phetools hocr failed, falling back to ocr.'
-                              .format(self))
+            pywikibot.warning(
+                f'{self}: phetools hocr failed, falling back to ocr.')
 
         error, text = self._do_ocr(ocr_tool=ocr_tool)
 
         if not error and isinstance(text, str):
             return text
         raise ValueError(
             f'{self}: not possible to perform OCR. {text}')
@@ -1258,16 +1252,15 @@
             # the first ones, so if they start repeating, we are done.
             if page in self._labels_from_page:
                 break
 
             # Sanity check if WS site use page convention name/number.
             if page._num is not None:
                 assert page_cnt == int(page._num), (
-                    'Page number {} not recognised as page {}.'
-                    .format(page_cnt, title))
+                    f'Page number {page_cnt} not recognised as page {title}.')
 
             # Mapping: numbers <-> pages.
             self._page_from_numbers[page_cnt] = page
             self._numbers_from_page[page] = page_cnt
             # Mapping: numbers/pages as keys, labels as values.
             self._labels_from_page_number[page_cnt] = label
             self._labels_from_page[page] = label
@@ -1358,16 +1351,15 @@
         There is a 1-to-1 correspondence (each page has a label).
 
         :return: page label
         """
         try:
             return self._labels_from_page_number[page_number]
         except KeyError:
-            raise KeyError('Page number ".../{}" not in range.'
-                           .format(page_number))
+            raise KeyError(f'Page number ".../{page_number}" not in range.')
 
     @staticmethod
     def _get_from_label(mapping_dict: Dict[str, Any],
                         label: Union[int, str]) -> Any:
         """Helper function to get info from label."""
         # Convert label to string if an integer is passed.
         if isinstance(label, int):
```

### Comparing `pywikibot-8.1.2/pywikibot/scripts/__init__.py` & `pywikibot-8.2.0/pywikibot/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/generate_family_file.py` & `pywikibot-8.2.0/pywikibot/scripts/generate_family_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,26 +253,24 @@
 
         if os.path.exists(fn) and input(
                 f'{fn} already exists. Overwrite? (y/n) ').lower() == 'n':
             print('Terminating.')
             sys.exit(1)
 
         code_hostname_pairs = '\n        '.join(
-            "'{code}': '{hostname}',".format(
-                code=k, hostname=urlparse(w.server).netloc
-            ) for k, w in self.wikis.items())
+            f"'{k}': '{urlparse(w.server).netloc}',"
+            for k, w in self.wikis.items())
 
         code_path_pairs = '\n            '.join(
             f"'{k}': '{w.scriptpath}',"
             for k, w in self.wikis.items())
 
         code_protocol_pairs = '\n            '.join(
-            "'{code}': '{protocol}',".format(
-                code=k, protocol=urlparse(w.server).scheme
-            ) for k, w in self.wikis.items())
+            f"'{k}': '{urlparse(w.server).scheme}',"
+            for k, w in self.wikis.items())
 
         content = family_template % {
             'url': self.base_url, 'name': self.name,
             'code_hostname_pairs': code_hostname_pairs,
             'code_path_pairs': code_path_pairs,
             'code_protocol_pairs': code_protocol_pairs}
         if not verify:
```

### Comparing `pywikibot-8.1.2/pywikibot/scripts/generate_user_files.py` & `pywikibot-8.2.0/pywikibot/scripts/generate_user_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 .. versionchanged:: 7.0
    moved to pywikibot.scripts folder.
 .. versionchanged:: 8.0
    let user the choice which section to be copied.
    Also EXTERNAL EDITOR SETTINGS section can be copied.
 """
 #
-# (C) Pywikibot team, 2010-2022
+# (C) Pywikibot team, 2010-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import codecs
 import os
 import re
 import sys
@@ -391,16 +391,16 @@
             botpasswordpass = pywikibot.input(message, force=force,
                                               password=True)
             if botpasswordname and botpasswordpass:
                 botpasswords.append((username, botpasswordname,
                                      botpasswordpass))
 
     if not userlist:  # Show a sample
-        usernames = "# usernames['{}']['{}'] = 'MyUsername'".format(
-            main_family, main_code)
+        usernames = (
+            f"# usernames['{main_family}']['{main_code}'] = 'MyUsername'")
     else:
         usernames = '\n'.join(
             "usernames['{user.family}']['{user.code}'] = '{user.name}'"
             .format(user=user) for user in userlist)
         # Arbitrarily use the first key as default settings
         main_family, main_code = userlist[0].family, userlist[0].code
     botpasswords = '\n'.join(
```

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ar.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ar.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ast.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ast.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/az.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/az.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/azb.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/azb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ba.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ba.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bcc.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bcc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/be-tarask.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/be.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/be.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bg.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bn.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/br.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/bs.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/bs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ca.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ca.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ce.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ce.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ckb.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ckb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/cs.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/cs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/csb.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/csb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/cy.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/cy.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/da.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/da.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/de.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/de.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/diq.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/diq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/el.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/el.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/en.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/en.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/eo.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/eo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/es.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/es.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/eu.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/eu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fa.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fa.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fi.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fo.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/fr.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/fr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/frr.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/frr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/gl.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/gl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/gsw.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/gsw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hak.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hak.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/haw.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/haw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/he.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/he.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hi.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hsb.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hsb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/hu.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/hu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ia.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ia.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/id.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/id.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/io.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/io.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/is.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/is.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/it.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/it.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ja.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ja.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kab.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kab.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kk.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/km.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/km.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/kn.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/kn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ko.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ko.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/krc.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/krc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ksh.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ksh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lb.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lt.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/lv.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/lv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/map-bms.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/map-bms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mg.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/min.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/min.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/mk.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/mk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ml.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ml.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ms.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/my.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/my.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nan.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nan.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nb.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nds-nl.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ne.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ne.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/new.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/new.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nl.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/nqo.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/nqo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pl.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pms.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pt-br.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pt-br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/pt.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/pt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/qqq.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/qqq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ro.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ro.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ru.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ru.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sco.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sco.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sh.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/si.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/si.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sk.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sl.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/so.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/so.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sr.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sv.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/sw.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/sw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ta.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ta.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/te.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/te.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/th.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/th.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tly.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tly.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/tr.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/tr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/uk.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/uk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/ur.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/ur.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/vi.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/vi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/yue.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/yue.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/i18n/pywikibot/zh.json` & `pywikibot-8.2.0/pywikibot/scripts/i18n/pywikibot/zh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/scripts/login.py` & `pywikibot-8.2.0/pywikibot/scripts/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         elif arg == '-oauth':
             oauth = True
         elif arg == '-autocreate':
             autocreate = True
         elif arg == '-async':
             asyncronous = True
         else:
-            unknown_args += [arg]
+            unknown_args.append(arg)
 
     if pywikibot.bot.suggest_help(unknown_parameters=unknown_args):
         return
 
     if logall:
         namedict = config.usernames
     else:
```

### Comparing `pywikibot-8.1.2/pywikibot/scripts/preload_sites.py` & `pywikibot-8.2.0/pywikibot/scripts/preload_sites.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     python pwb.py -API_config_expiry:0 preload_sites [{<family>}]
 
 .. versionchanged:: 7.4
    script was moved to the framework scripts folder.
 """
 #
-# (C) Pywikibot team, 2021-2022
+# (C) Pywikibot team, 2021-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import os
 from concurrent.futures import ThreadPoolExecutor, wait
 from datetime import datetime
 from typing import Optional, Union
@@ -81,16 +81,16 @@
     start = datetime.now()
     if worker is None:
         # Python 3.8 default
         worker = min(32, (os.cpu_count() or 1) + 4)
     # to allow adding futures in preload_family the workers must be one
     # more than families are handled
     worker = max(len(families) * 2, worker)
-    pywikibot.info('Using {} workers to process {} families'
-                   .format(worker, len(families)))
+    pywikibot.info(
+        f'Using {worker} workers to process {len(families)} families')
     with ThreadPoolExecutor(worker) as executor:
         futures = {executor.submit(preload_family, family, executor)
                    for family in families}
         wait(futures)
     pywikibot.info(f'Loading time used: {datetime.now() - start}')
```

### Comparing `pywikibot-8.1.2/pywikibot/scripts/version.py` & `pywikibot-8.2.0/pywikibot/scripts/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,15 @@
 
     has_wikimedia_cert = False
     if (not hasattr(requests, 'certs')
             or not hasattr(requests.certs, 'where')
             or not callable(requests.certs.where)):
         pywikibot.info('  cacerts: not defined')
     elif not os.path.isfile(requests.certs.where()):
-        pywikibot.info('  cacerts: {} (missing)'.format(
-            requests.certs.where()))
+        pywikibot.info(f'  cacerts: {requests.certs.where()} (missing)')
     else:
         pywikibot.info('  cacerts: ' + requests.certs.where())
 
         with codecs.open(requests.certs.where(), 'r', 'utf-8') as cert_file:
             text = cert_file.read()
             if WMF_CACERT in text:
                 has_wikimedia_cert = True
```

### Comparing `pywikibot-8.1.2/pywikibot/scripts/wrapper.py` & `pywikibot-8.2.0/pywikibot/scripts/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,16 +209,15 @@
     else:
         format_string = '\nA package necessary for {} is {}.'
     print(format_string.format(script or 'pywikibot', variant))
     print('Please update required module{} with:\n\n'
           .format('s' if len(requirements) > 1 else ''))
 
     for requirement in requirements:
-        print('    pip install "{}"\n'
-              .format(str(requirement).partition(';')[0]))
+        print(f"    pip install \"{str(requirement).partition(';')[0]}\"\n")
 
 
 def check_modules(script=None):
     """Check whether mandatory modules are present.
 
     This also checks Python version when importing dependencies from setup.py
 
@@ -472,16 +471,16 @@
     if file_package:
         try:
             module = sys.modules[file_package]
         except KeyError:
             try:
                 module = import_module(file_package)
             except ImportError as e:
-                warn('Parent module {} not found: {}'
-                     .format(file_package, e), ImportWarning)
+                warn(f'Parent module {file_package} not found: {e}',
+                     ImportWarning)
 
     help_option = any(arg.startswith('-help:') or arg == '-help'
                       for arg in script_args)
     if site_package or check_modules(filename) or help_option:
         run_python_file(filename, script_args, module)
     return True
```

### Comparing `pywikibot-8.1.2/pywikibot/site/__init__.py` & `pywikibot-8.2.0/pywikibot/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/site/_apisite.py` & `pywikibot-8.2.0/pywikibot/site/_apisite.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 import datetime
 import re
 import time
 import typing
 from collections import OrderedDict, defaultdict, namedtuple
 from contextlib import suppress
 from textwrap import fill
-from typing import Any, Iterable, Optional, Type, TypeVar, Union
+from typing import Any, Optional, Type, TypeVar, Union
 
 import pywikibot
 from pywikibot import login
 from pywikibot.backports import DefaultDict, Dict, List, Match
 from pywikibot.backports import OrderedDict as OrderedDictType
-from pywikibot.backports import Pattern, Set, Tuple, removesuffix
+from pywikibot.backports import Iterable, Pattern, Set, Tuple, removesuffix
 from pywikibot.comms import http
 from pywikibot.data import api
 from pywikibot.exceptions import (
     AbuseFilterDisallowedError,
     APIError,
     ArticleExistsConflictError,
     CaptchaError,
@@ -281,23 +281,18 @@
     def _request(self, **kwargs: Any) -> api.Request:
         """Create a request by forwarding all parameters directly."""
         if 'expiry' in kwargs and kwargs['expiry'] is None:
             del kwargs['expiry']
 
         return self._request_class(kwargs)(site=self, **kwargs)
 
-    @deprecated('simple_request', since='7.1.0')
-    def _simple_request(self, **kwargs: Any) -> api.Request:
-        """DEPRECATED. Create a request using all kwargs as parameters."""
-        return self.simple_request(**kwargs)
-
     def simple_request(self, **kwargs: Any) -> api.Request:
         """Create a request by defining all kwargs as parameters.
 
-        .. versionchanged:: 7.1
+        .. versionadded:: 7.1
            `_simple_request` becomes a public method
         """
         return self._request_class({'parameters': kwargs}).create_simple(
             self, **kwargs)
 
     def logged_in(self) -> bool:
         """Verify the bot is logged into the site as the expected user.
@@ -354,17 +349,16 @@
         #       is not already IN_PROGRESS, however the
         #       login status may be left 'IN_PROGRESS' because
         #       of exceptions or if the first method of login
         #       (below) is successful. Instead, log the problem,
         #       to be increased to 'warning' level once majority
         #       of issues are resolved.
         if self._loginstatus == login.LoginStatus.IN_PROGRESS:
-            pywikibot.log(
-                '{!r}.login() called when a previous login was in progress.'
-                .format(self))
+            pywikibot.log(f'{self!r}.login() called when a previous login was '
+                          f'in progress.')
 
         # There are several ways that the site may already be
         # logged in, and we do not need to hit the server again.
         # logged_in() is False if _userinfo exists, which means this
         # will have no effect for the invocation from api.py
         if self.logged_in():
             self._loginstatus = login.LoginStatus.AS_USER
@@ -390,16 +384,15 @@
             pass
         except NoUsernameError as e:
             if not autocreate:
                 raise e
 
         if self.is_oauth_token_available():
             if self.userinfo['name'] == self.username():
-                error_msg = ('Logging in on {} via OAuth failed'
-                             .format(self))
+                error_msg = (f'Logging in on {self} via OAuth failed')
             elif self.username() is None:
                 error_msg = ('No username has been defined in your '
                              'user config file: you have to add in this '
                              'file the following line:\n'
                              'usernames[{family!r}][{lang!r}]= {username!r}'
                              .format(family=self.family,
                                      lang=self.lang,
@@ -544,16 +537,15 @@
             assert 'query' in uidata, \
                    "API userinfo response lacks 'query' key"
             assert 'userinfo' in uidata['query'], \
                    "API userinfo response lacks 'userinfo' key"
             self._userinfo = uidata['query']['userinfo']
             if self._loginstatus != login.LoginStatus.IN_PROGRESS \
                and ('anon' in self._userinfo or not self._userinfo.get('id')):
-                pywikibot.warning('No user is logged in on site {}'
-                                  .format(self))
+                pywikibot.warning(f'No user is logged in on site {self}')
         return self._userinfo
 
     @userinfo.deleter
     def userinfo(self) -> None:
         """Delete cached userinfo.
 
         .. versionadded:: 5.5
@@ -742,17 +734,16 @@
             return ''
 
         match = re.search(r'\((?:\:\?|\?\:)?\[(?P<pattern>.+?)\]'
                           r'(?P<letters>(\|.)*)\)?\+\)', linktrail)
         if not match:
             with suppress(KeyError):
                 return unresolved_linktrails[self.code]
-            raise KeyError(
-                '"{}": No linktrail pattern extracted from "{}"'
-                .format(self.code, linktrail))
+            raise KeyError(f'"{self.code}": No linktrail pattern extracted '
+                           f'from "{linktrail}"')
 
         pattern = match['pattern']
         letters = match['letters']
 
         if r'x{' in pattern:
             pattern = re.sub(r'\\x\{([A-F0-9]{4})\}',
                              lambda match: chr(int(match[1], 16)),
@@ -778,17 +769,15 @@
         :param is_ts: When comparing timestamps (with is_ts=True) the start
             is usually greater than end. Comparing titles this is vice versa.
         :raises AssertionError: start/end values are not comparabel types or
             are in the wrong order
         """
         if not (isinstance(end, type(start)) or isinstance(start, type(end))):
             raise TypeError(
-                'start ({!r}) and end ({!r}) must be comparable'
-                .format(start, end)
-            )
+                f'start ({start!r}) and end ({end!r}) must be comparable')
         if reverse ^ is_ts:
             low, high = end, start
             order = 'follow'
         else:
             low, high = start, end
             order = 'precede'
         msg = ('{method}: "start" must {order} "end" '
@@ -861,16 +850,16 @@
 
             # Check requested keys
             result = OrderedDict()
             for key in keys:
                 try:
                     result[key] = _mw_msg_cache[amlang][key]
                 except KeyError:
-                    raise KeyError("No message '{}' found for lang '{}'"
-                                   .format(key, amlang))
+                    raise KeyError(
+                        f"No message '{key}' found for lang '{amlang}'")
 
             return result
 
         return OrderedDict((key, _mw_msg_cache[amlang][key]) for key in keys)
 
     def mediawiki_message(
         self,
@@ -1088,17 +1077,16 @@
             _namespaces[ns] = namespace
 
         for item in self.siteinfo.get('namespacealiases'):
             ns = int(item['id'])
             try:
                 namespace = _namespaces[ns]
             except KeyError:
-                pywikibot.warning(
-                    'Broken namespace alias "{}" (id: {}) on {}'.format(
-                        item['*'], ns, self))
+                pywikibot.warning('Broken namespace alias "{}" (id: {}) on {}'
+                                  .format(item['*'], ns, self))
             else:
                 if item['*'] not in namespace:
                     namespace.aliases.append(item['*'])
 
         return _namespaces
 
     def has_extension(self, name: str) -> bool:
@@ -1201,16 +1189,16 @@
         if 'query' in data and 'wikibase' in data['query']:
             data = data['query']['wikibase']['repo']['url']
             url = data['base'] + data['scriptpath'] + '/index.php'
             try:
                 return pywikibot.Site(url=url, user=self.username(),
                                       interface='DataSite')
             except SiteDefinitionError as e:
-                pywikibot.warning('Site "{}" supports wikibase at "{}", but '
-                                  'creation failed: {}.'.format(self, url, e))
+                pywikibot.warning(f'Site "{self}" supports wikibase at '
+                                  f'"{url}", but creation failed: {e}.')
                 return None
         else:
             assert 'warnings' in data
             return None
 
     def is_image_repository(self) -> bool:
         """Return True if Site object is the image repository."""
@@ -1368,32 +1356,42 @@
         history: bool = False,
         url_width: Optional[int] = None,
         url_height: Optional[int] = None,
         url_param: Optional[str] = None
     ) -> None:
         """Load image info from api and save in page attributes.
 
-        Parameters correspond to iiprops in:
-        [1] :api:`Imageinfo`
-
-        Parameters validation and error handling left to the API call.
+        The following properties are loaded: ``timestamp``, ``user``,
+        ``comment``, ``url``, ``size``, ``sha1``, ``mime``, ``mediatype``,
+        ``metadata``, ``archivename`` and ``bitdepth``. If *url_width*,
+        *url_height* or *url_param* is given, additional properties
+        ``thumbwidth``, ``thumbheight``, ``thumburl`` and
+        ``responsiveUrls`` are given.
+
+        .. note:: Parameters validation and error handling left to the
+           API call.
+        .. versionchanged:: 8.2
+           *mediatype* and *bitdepth* properties were added.
+        .. seealso:: :api:`Imageinfo`
 
         :param history: if true, return the image's version history
-        :param url_width: see iiurlwidth in [1]
-        :param url_height: see iiurlheigth in [1]
-        :param url_param: see iiurlparam in [1]
-
-        """
-        args = {'titles': page.title(with_section=False),
-                'iiurlwidth': url_width,
-                'iiurlheight': url_height,
-                'iiurlparam': url_param,
-                'iiprop': ['timestamp', 'user', 'comment', 'url', 'size',
-                           'sha1', 'mime', 'metadata', 'archivename']
-                }
+        :param url_width: get info for a thumbnail with given width
+        :param url_height: get info for a thumbnail with given height
+        :param url_param:  get info for a thumbnail with given param
+        """
+        args = {
+            'titles': page.title(with_section=False),
+            'iiurlwidth': url_width,
+            'iiurlheight': url_height,
+            'iiurlparam': url_param,
+            'iiprop': [
+                'timestamp', 'user', 'comment', 'url', 'size', 'sha1', 'mime',
+                'mediatype', 'metadata', 'archivename', 'bitdepth',
+            ]
+        }
         if not history:
             args['total'] = 1
         query = self._generator(api.PropertyGenerator,
                                 type_arg='imageinfo',
                                 **args)
         self._update_page(page, query, verify_imageinfo=True)
 
@@ -1482,16 +1480,15 @@
             prop='info',
             titles=title,
             redirects=True
         )
         result = query.submit()
         if 'query' not in result or 'redirects' not in result['query']:
             raise RuntimeError(
-                "getredirtarget: No 'redirects' found for page {}."
-                .format(title))
+                f"getredirtarget: No 'redirects' found for page {title}.")
 
         redirmap = {item['from']: {'title': item['to'],
                                    'section': '#'
                                    + item['tofragment']
                                    if 'tofragment' in item
                                    and item['tofragment']
                                    else ''}
@@ -1500,17 +1497,16 @@
         # Normalize title
         for item in result['query'].get('normalized', []):
             if item['from'] == title:
                 title = item['to']
                 break
 
         if title not in redirmap:
-            raise RuntimeError(
-                "getredirtarget: 'redirects' contains no key for page {}."
-                .format(title))
+            raise RuntimeError(f"getredirtarget: 'redirects' contains no key "
+                               f'for page {title}.')
         target_title = '{title}{section}'.format_map(redirmap[title])
 
         if self.sametitle(title, target_title):
             raise CircularRedirectError(page)
 
         if 'pages' not in result['query']:
             # No "pages" element might indicate a circular redirect
@@ -1790,16 +1786,16 @@
                 'title': target,
                 'user': self.user(),
             }
             if err.code in self._dl_errors:
                 raise Error(
                     self._dl_errors[err.code].format_map(errdata)
                 ) from None
-            pywikibot.debug("revdelete: Unexpected error code '{}' received."
-                            .format(err.code))
+            pywikibot.debug(
+                f"revdelete: Unexpected error code '{err.code}' received.")
             raise
         else:
             if target:
                 page.clear_cache()
         finally:
             if target:
                 self.unlock_page(page)
@@ -1940,31 +1936,30 @@
         if basetimestamp and 'basetimestamp' not in kwargs:
             params['basetimestamp'] = basetimestamp
 
         watch_items = {'watch', 'unwatch', 'preferences', 'nochange'}
         if watch in watch_items:
             params['watchlist'] = watch
         elif watch:
-            pywikibot.warning("editpage: Invalid watch value '{}' ignored."
-                              .format(watch))
+            pywikibot.warning(
+                f"editpage: Invalid watch value '{watch}' ignored.")
         req = self.simple_request(**params)
 
         self.lock_page(page)
         try:
             while True:
                 try:
                     result = req.submit()
                     pywikibot.debug(f'editpage response: {result}')
                 except APIError as err:
                     if err.code.endswith('anon') and self.logged_in():
-                        pywikibot.debug("editpage: received '{}' even though "
-                                        'bot is logged in'.format(err.code))
+                        pywikibot.debug(f"editpage: received '{err.code}' "
+                                        f'even though bot is logged in')
                     if err.code == 'abusefilter-warning':
-                        pywikibot.warning('{info}\nRetrying.'
-                                          .format(info=err.info))
+                        pywikibot.warning(f'{err.info}\nRetrying.')
                         continue
                     if err.code in self._ep_errors:
                         exception = self._ep_errors[err.code]
                         if isinstance(exception, str):
                             errdata = {
                                 'site': self,
                                 'title': page.title(with_section=False),
@@ -1976,26 +1971,25 @@
                             ) from None
                         if issubclass(exception, AbuseFilterDisallowedError):
                             raise exception(page, info=err.info) from None
                         if issubclass(exception, SpamblacklistError):
                             urls = ', '.join(err.other[err.code]['matches'])
                             raise exception(page, url=urls) from None
                         raise exception(page) from None
-                    pywikibot.debug(
-                        "editpage: Unexpected error code '{}' received."
-                        .format(err.code))
+                    pywikibot.debug(f'editpage: Unexpected error code '
+                                    f"'{err.code}' received.")
                     raise
 
                 assert 'edit' in result and 'result' in result['edit'], result
 
                 if result['edit']['result'] == 'Success':
                     if 'nochange' in result['edit']:
                         # null edit, page not changed
-                        pywikibot.log('Page [[{}]] saved without any changes.'
-                                      .format(page.title()))
+                        pywikibot.log(f'Page [[{page.title()}]] saved without '
+                                      f'any changes.')
                         return True
                     page.latest_revision_id = result['edit']['newrevid']
                     # See:
                     # https://www.mediawiki.org/wiki/API:Wikimania_2006_API_discussion#Notes
                     # not safe to assume that saved text is the same as sent
                     del page.text
                     return True
@@ -2019,33 +2013,31 @@
                                                     self.hostname(),
                                                     captcha['url']))
                             req['captchaword'] = pywikibot.input(
                                 'Please view CAPTCHA in your browser, '
                                 'then type answer here:')
                             continue
 
-                        pywikibot.error(
-                            'editpage: unknown CAPTCHA response {}, '
-                            'page not saved'
-                            .format(captcha))
+                        pywikibot.error(f'editpage: unknown CAPTCHA response '
+                                        f'{captcha}, page not saved')
                         break
 
                     if 'spamblacklist' in result['edit']:
                         raise SpamblacklistError(
                             page, result['edit']['spamblacklist']) from None
 
                     if 'code' in result['edit'] and 'info' in result['edit']:
                         pywikibot.error(
                             'editpage: {}\n{}, '
                             .format(result['edit']['code'],
                                     result['edit']['info']))
                         break
 
-                    pywikibot.error('editpage: unknown failure reason {}'
-                                    .format(str(result)))
+                    pywikibot.error(
+                        f'editpage: unknown failure reason {result}')
                     break
 
                 pywikibot.error(
                     "editpage: Unknown result code '{}' received; "
                     'page not saved'.format(result['edit']['result']))
                 pywikibot.log(str(result))
                 break
@@ -2143,24 +2135,22 @@
         if timestamp:
             req['timestamp'] = timestamp
 
         self.lock_page(source)
         self.lock_page(dest)
         try:
             result = req.submit()
-            pywikibot.debug('mergehistory response: {result}'
-                            .format(result=result))
+            pywikibot.debug(f'mergehistory response: {result}')
         except APIError as err:
             if err.code in self._mh_errors:
                 on_error = self._mh_errors[err.code]
                 raise Error(on_error.format_map(errdata)) from None
 
             pywikibot.debug(
-                "mergehistory: Unexpected error code '{code}' received"
-                .format(code=err.code))
+                f"mergehistory: Unexpected error code '{err.code}' received")
             raise
         finally:
             self.unlock_page(source)
             self.unlock_page(dest)
 
         if 'mergehistory' not in result:
             pywikibot.error(f'mergehistory: {result}')
@@ -2228,16 +2218,15 @@
         newlink = pywikibot.Link(newtitle, self)
         newpage = pywikibot.Page(newlink)
         if newlink.namespace:
             newtitle = self.namespace(newlink.namespace) + ':' + newlink.title
         else:
             newtitle = newlink.title
         if oldtitle == newtitle:
-            raise Error('Cannot move page {} to its own title.'
-                        .format(oldtitle))
+            raise Error(f'Cannot move page {oldtitle} to its own title.')
         if not page.exists():
             raise NoPageError(page,
                               'Cannot move page {page} because it '
                               'does not exist on {site}.')
         token = self.tokens['csrf']
         self.lock_page(page)
         req = self.simple_request(action='move',
@@ -2249,17 +2238,16 @@
                                   to=newtitle)
         req['from'] = oldtitle  # "from" is a python keyword
         try:
             result = req.submit()
             pywikibot.debug(f'movepage response: {result}')
         except APIError as err:
             if err.code.endswith('anon') and self.logged_in():
-                pywikibot.debug(
-                    "movepage: received '{}' even though bot is logged in"
-                    .format(err.code))
+                pywikibot.debug(f"movepage: received '{err.code}' even though "
+                                f'bot is logged in')
 
             if err.code in self._mv_errors:
                 on_error = self._mv_errors[err.code]
                 if not isinstance(on_error, str):
                     # LockedPageError can be raised both if "from" or "to" page
                     # are locked for the user.
                     # Both pages locked is not considered
@@ -2284,16 +2272,16 @@
                     'newtitle': newtitle,
                     'newnamespace': self.namespace(newlink.namespace),
                     'user': self.user(),
                 }
 
                 raise Error(on_error.format_map(errdata)) from None
 
-            pywikibot.debug("movepage: Unexpected error code '{}' received."
-                            .format(err.code))
+            pywikibot.debug(
+                f"movepage: Unexpected error code '{err.code}' received.")
             raise
         finally:
             self.unlock_page(page)
         if 'move' not in result:
             pywikibot.error(f'movepage: {result}')
             raise Error('movepage: unexpected response')
         # TODO: Check for talkmove-error messages
@@ -2329,27 +2317,25 @@
 
         :param page: the Page to be rolled back (must exist)
         :keyword user: the last user to be rollbacked;
             default is page.latest_revision.user
         """
         if len(page._revisions) < 2:
             raise Error(
-                'Rollback of {} aborted; load revision history first.'
-                .format(page))
+                f'Rollback of {page} aborted; load revision history first.')
 
         user = kwargs.pop('user', page.latest_revision.user)
         for rev in sorted(page._revisions.values(), reverse=True,
                           key=lambda r: r.timestamp):
             # start with most recent revision first
             if rev.user != user:
                 break
         else:
-            raise Error(
-                'Rollback of {} aborted; only one user in revision history.'
-                .format(page))
+            raise Error(f'Rollback of {page} aborted; only one user in '
+                        f'revision history.')
 
         parameters = merge_unique_dicts(kwargs,
                                         action='rollback',
                                         title=page,
                                         token=self.tokens['rollback'],
                                         user=user)
         self.lock_page(page)
@@ -2362,16 +2348,16 @@
                 'title': page.title(with_section=False),
                 'user': self.user(),
             }
             if err.code in self._rb_errors:
                 raise Error(
                     self._rb_errors[err.code].format_map(errdata)
                 ) from None
-            pywikibot.debug("rollback: Unexpected error code '{}' received."
-                            .format(err.code))
+            pywikibot.debug(
+                f"rollback: Unexpected error code '{err.code}' received.")
             raise
         finally:
             self.unlock_page(page)
 
     # catalog of delete errors for use in error messages
     _dl_errors = {
         'noapiwrite': 'API editing not enabled on {site} wiki',
@@ -2466,16 +2452,16 @@
                 'user': self.user(),
             }
 
             if err.code in self._dl_errors:
                 raise Error(
                     self._dl_errors[err.code].format_map(errdata)
                 ) from None
-            pywikibot.debug('delete: Unexpected error code {!r} received.'
-                            .format(err.code))
+            pywikibot.debug(
+                f'delete: Unexpected error code {err.code!r} received.')
             raise
         else:
             if isinstance(page, pywikibot.page.BasePage):
                 page.clear_cache()
         finally:
             self.unlock_page(page)
 
@@ -2525,16 +2511,16 @@
                 'title': page.title(with_section=False),
                 'user': self.user(),
             }
             if err.code in self._dl_errors:
                 raise Error(
                     self._dl_errors[err.code].format_map(errdata)
                 ) from None
-            pywikibot.debug('undelete: Unexpected error code {!r} received.'
-                            .format(err.code))
+            pywikibot.debug(
+                f'undelete: Unexpected error code {err.code!r} received.')
             raise
         finally:
             self.unlock_page(page)
 
     _protect_errors = {
         'noapiwrite': 'API editing not enabled on {site} wiki',
         'writeapidenied': 'User {user} not allowed to edit through the API',
@@ -2626,16 +2612,16 @@
                 'site': self,
                 'user': self.user(),
             }
             if err.code in self._protect_errors:
                 raise Error(
                     self._protect_errors[err.code].format_map(errdata)
                 ) from None
-            pywikibot.debug("protect: Unexpected error code '{}' received."
-                            .format(err.code))
+            pywikibot.debug(
+                f"protect: Unexpected error code '{err.code}' received.")
             raise
         else:
             protection = {}
             for d in result['protect']['protections']:
                 expiry = d.pop('expiry')
                 ptype, level = d.popitem()
                 if level:
@@ -2861,24 +2847,30 @@
         :param force: force to retrieve userinfo ignoring cache
         """
         if force or not hasattr(self, '_property_names'):
             ppngen = self._generator(api.ListGenerator, 'pagepropnames')
             self._property_names = [pn['propname'] for pn in ppngen]
         return self._property_names
 
-    def compare(self, old: _CompType, diff: _CompType) -> str:
+    def compare(
+        self,
+        old: _CompType,
+        diff: _CompType,
+        difftype: str = 'table'
+    ) -> str:
         """
         Corresponding method to the 'action=compare' API action.
 
-        .. seealso: :api:`Compare`
+        .. hint:: Use :func:`diff.html_comparator` function to parse
+           result.
+        .. seealso:: :api:`Compare`
 
-        See: https://en.wikipedia.org/w/api.php?action=help&modules=compare
-        Use pywikibot.diff's html_comparator() method to parse result.
         :param old: starting revision ID, title, Page, or Revision
         :param diff: ending revision ID, title, Page, or Revision
+        :param difftype: type of diff. One of 'table' or 'inline'.
         :return: Returns an HTML string of a diff between two revisions.
         """
         # check old and diff types
         def get_param(item: object) -> Optional[Tuple[str, Union[str, int]]]:
             param = None
             if isinstance(item, str):
                 param = 'title', item
@@ -2895,12 +2887,13 @@
             raise TypeError('old parameter is of invalid type')
         diff_t = get_param(diff)
         if not diff_t:
             raise TypeError('diff parameter is of invalid type')
 
         params = {'action': 'compare',
                   f'from{old_t[0]}': old_t[1],
-                  f'to{diff_t[0]}': diff_t[1]}
+                  f'to{diff_t[0]}': diff_t[1],
+                  'difftype': difftype}
 
         req = self.simple_request(**params)
         data = req.submit()
         return data['compare']['*']
```

### Comparing `pywikibot-8.1.2/pywikibot/site/_basesite.py` & `pywikibot-8.2.0/pywikibot/site/_basesite.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #
 # (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import functools
 import re
-import sys
 import threading
 from typing import Optional
 from warnings import warn
 
 import pywikibot
 from pywikibot.backports import Pattern
 from pywikibot.exceptions import (
@@ -27,17 +26,14 @@
     SelfCallString,
     cached,
     first_upper,
     normalize_username,
 )
 
 
-PYTHON_312A7 = sys.version.split()[0] == '3.12.0a7'  # T334378 workaround
-
-
 class BaseSite(ComparableMixin):
 
     """Site methods that are independent of the communication interface."""
 
     def __init__(self, code: str, fam=None, user=None) -> None:
         """
         Initializer.
@@ -48,35 +44,34 @@
         :type fam: str or pywikibot.family.Family
         :param user: bot user name (optional)
         :type user: str
         """
         if code.lower() != code:
             # Note the Site function in __init__ also emits a UserWarning
             # for this condition, showing the callers file and line no.
-            pywikibot.log('BaseSite: code "{}" converted to lowercase'
-                          .format(code))
+            pywikibot.log(f'BaseSite: code "{code}" converted to lowercase')
             code = code.lower()
         if not all(x in pywikibot.family.CODE_CHARACTERS for x in code):
-            pywikibot.log('BaseSite: code "{}" contains invalid characters'
-                          .format(code))
+            pywikibot.log(
+                f'BaseSite: code "{code}" contains invalid characters')
         self.__code = code
         if isinstance(fam, str) or fam is None:
             self.__family = pywikibot.family.Family.load(fam)
         else:
             self.__family = fam
 
         self.obsolete = False
         # if we got an outdated language code, use the new one instead.
         if self.__code in self.__family.obsolete:
             if self.__family.obsolete[self.__code] is not None:
                 self.__code = self.__family.obsolete[self.__code]
                 # Note the Site function in __init__ emits a UserWarning
                 # for this condition, showing the callers file and line no.
-                pywikibot.log('Site {} instantiated using aliases code of {}'
-                              .format(self, code))
+                pywikibot.log(
+                    f'Site {self} instantiated using aliases code of {code}')
             else:
                 # no such language anymore
                 self.obsolete = True
                 pywikibot.log('Site {} instantiated and marked "obsolete" '
                               'to prevent access'.format(self))
         elif self.__code not in self.languages():
             if self.__family.name in self.__family.langs \
@@ -186,16 +181,14 @@
 
     def username(self) -> Optional[str]:
         """Return the username used for the site."""
         return self._username
 
     def __getattr__(self, attr):
         """Delegate undefined methods calls to the Family object."""
-        if PYTHON_312A7:  # T334378 workaround
-            print(end='')  # noqa: T001, T201
         try:
             method = getattr(self.family, attr)
             if not callable(method):
                 raise AttributeError
             f = functools.partial(method, self.code)
             if hasattr(method, '__doc__'):
                 f.__doc__ = method.__doc__
@@ -211,16 +204,15 @@
     @property
     def sitename(self):
         """String representing this Site's name and code."""
         return SelfCallString(self.__str__())
 
     def __repr__(self) -> str:
         """Return internal representation."""
-        return '{}("{}", "{}")'.format(
-            self.__class__.__name__, self.code, self.family)
+        return f'{self.__class__.__name__}("{self.code}", "{self.family}")'
 
     def __hash__(self):
         """Return hash value of instance."""
         return hash(repr(self))
 
     def languages(self):
         """Return list of all valid language codes for this site's Family."""
@@ -323,16 +315,16 @@
                 name = dp.getSitelink(self)
             except NoPageError:
                 raise Error(f'No disambiguation category name found in {repo} '
                             f'for {self}')
 
         else:  # fallback for non WM sites
             try:
-                name = '{}:{}'.format(Namespace.CATEGORY,
-                                      self.family.disambcatname[self.code])
+                name = (f'{Namespace.CATEGORY}:'
+                        f'{self.family.disambcatname[self.code]}')
             except KeyError:
                 raise Error(f'No disambiguation category name found in '
                             f'{self.family.name}_family for {self}')
 
         return pywikibot.Category(pywikibot.Link(name, self))
 
     def isInterwikiLink(self, text):  # noqa: N802
@@ -377,16 +369,15 @@
                 return default_ns, title
             return ns, name
 
         # Replace alias characters like underscores with title
         # delimiters like spaces and multiple combinations of them with
         # only one delimiter
         sep = self.family.title_delimiter_and_aliases[0]
-        pattern = re.compile('[{}]+'
-                             .format(self.family.title_delimiter_and_aliases))
+        pattern = re.compile(f'[{self.family.title_delimiter_and_aliases}]+')
         title1 = pattern.sub(sep, title1)
         title2 = pattern.sub(sep, title2)
         if title1 == title2:
             return True
 
         default_ns = self.namespaces[0]
         # determine whether titles contain namespace prefixes
```

### Comparing `pywikibot-8.1.2/pywikibot/site/_datasite.py` & `pywikibot-8.2.0/pywikibot/site/_datasite.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 import json
 import uuid
 from contextlib import suppress
 from typing import Any, Dict, List, Optional
 from warnings import warn
 
 import pywikibot
+from pywikibot.backports import batched
 from pywikibot.data import api
 from pywikibot.exceptions import (
     APIError,
     EntityTypeUnknownError,
     IsRedirectPageError,
     NoPageError,
     NoWikibaseEntityError,
 )
 from pywikibot.site._apisite import APISite
 from pywikibot.site._decorators import need_extension, need_right, need_version
 from pywikibot.tools import merge_unique_dicts, remove_last_args
-from pywikibot.tools.itertools import itergroup
 
 
 __all__ = ('DataSite', )
 
 
 class DataSite(APISite):
 
@@ -200,29 +200,28 @@
         req = self.simple_request(**params)
         data = req.submit()
         if 'success' not in data:
             raise APIError(data['errors'], '')
         return data['entities']
 
     def preload_entities(self, pagelist, groupsize: int = 50):
-        """
-        Yield subclasses of WikibaseEntity's with content prefilled.
+        """Yield subclasses of WikibaseEntity's with content prefilled.
 
-        Note that pages will be iterated in a different order
-        than in the underlying pagelist.
+        .. note:: Pages will be iterated in a different order than in
+           the underlying pagelist.
 
-        :param pagelist: an iterable that yields either WikibaseEntity objects,
-                         or Page objects linked to an ItemPage.
+        :param pagelist: an iterable that yields either WikibaseEntity
+            objects, or Page objects linked to an ItemPage.
         :param groupsize: how many pages to query at a time
         """
         if not hasattr(self, '_entity_namespaces'):
             self._cache_entity_namespaces()
-        for sublist in itergroup(pagelist, groupsize):
+        for batch in batched(pagelist, groupsize):
             req = {'ids': [], 'titles': [], 'sites': []}
-            for p in sublist:
+            for p in batch:
                 if isinstance(p, pywikibot.page.WikibaseEntity):
                     ident = p._defined_by()
                     for key in ident:
                         req[key].append(ident[key])
                 else:
                     if p.site == self and p.namespace() in (
                             self._entity_namespaces.values()):
@@ -774,16 +773,16 @@
                         pywikibot.error('{error-info} for value {raw!r}, '
                                         '{expected-format!r} format expected'
                                         .format_map(err))
                 raise ValueError(e) from None
             raise
 
         if 'results' not in data:
-            raise RuntimeError("Unexpected missing 'results' in query data\n{}"
-                               .format(data))
+            raise RuntimeError(
+                f"Unexpected missing 'results' in query data\n{data}")
 
         results = []
         for result_hash in data['results']:
             if 'value' not in result_hash:
                 # There should be an APIError occurred already
                 raise RuntimeError("Unexpected missing 'value' in query data:"
                                    '\n{}'.format(result_hash))
```

### Comparing `pywikibot-8.1.2/pywikibot/site/_decorators.py` & `pywikibot-8.2.0/pywikibot/site/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/site/_extensions.py` & `pywikibot-8.2.0/pywikibot/site/_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -751,11 +751,11 @@
                                   exchars=chars,
                                   exsentences=sentences,
                                   exintro=intro,
                                   explaintext=plaintext)
         data = req.submit()['query']['pages']
         if '-1' in data:
             msg = data['-1'].get('invalidreason',
-                                 'Unknown exception:\n{}'.format(data['-1']))
+                                 f"Unknown exception:\n{data['-1']}")
             raise Error(msg)
 
         return data[str(page.pageid)]['extract']
```

### Comparing `pywikibot-8.1.2/pywikibot/site/_generators.py` & `pywikibot-8.2.0/pywikibot/site/_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 import itertools
 import typing
 from contextlib import suppress
 from itertools import zip_longest
 from typing import Any, Optional, Union
 
 import pywikibot
-from pywikibot.backports import Dict, Generator, Iterable, List  # skipcq
+from pywikibot.backports import Dict, Generator, Iterable, List, batched
 from pywikibot.data import api
 from pywikibot.exceptions import (
     APIError,
     Error,
     InconsistentTitleError,
     InvalidTitleError,
     NoPageError,
     UserRightsError,
 )
 from pywikibot.site._decorators import need_right
 from pywikibot.site._namespace import NamespaceArgType
 from pywikibot.tools import is_ip_address, issue_deprecation_warning
-from pywikibot.tools.itertools import filter_unique, itergroup
+from pywikibot.tools.itertools import filter_unique
 
 
 class GeneratorsMixin:
 
     """API generators mixin to MediaWiki site."""
 
     def load_pages_from_pageids(self, pageids):
@@ -51,21 +51,21 @@
             pageids = pageids.replace('|', ',')
             pageids = pageids.split(',')
             pageids = [p.strip() for p in pageids]
 
         # Validate pageids.
         gen = (str(int(p)) for p in pageids if int(p) > 0)
 
-        for sublist in itergroup(filter_unique(gen), self.maxlimit):
+        for batch in batched(filter_unique(gen), self.maxlimit):
             # Store the order of the input data.
-            priority_dict = dict(zip(sublist, range(len(sublist))))
+            priority_dict = dict(zip(batch, range(len(batch))))
 
             prio_queue = []
             next_prio = 0
-            params = {'pageids': sublist, }
+            params = {'pageids': batch}
             rvgen = api.PropertyGenerator('info', site=self, parameters=params)
 
             for pagedata in rvgen:
                 title = pagedata['title']
                 pageid = str(pagedata['pageid'])
                 page = pywikibot.Page(pywikibot.Link(title, source=self))
                 api.update_page(page, pagedata)
@@ -134,33 +134,33 @@
             props += '|langlinks'
         if pageprops:
             props += '|pageprops'
         if categories:
             props += '|categories'
 
         groupsize = min(groupsize or self.maxlimit, self.maxlimit)
-        for sublist in itergroup(pagelist, groupsize):
+        for batch in batched(pagelist, groupsize):
             # Do not use p.pageid property as it will force page loading.
-            pageids = [str(p._pageid) for p in sublist
+            pageids = [str(p._pageid) for p in batch
                        if hasattr(p, '_pageid') and p._pageid > 0]
             cache = {}
             # In case of duplicates, return the first entry.
-            for priority, page in enumerate(sublist):
+            for priority, page in enumerate(batch):
                 try:
                     cache.setdefault(page.title(with_section=False),
                                      (priority, page))
                 except InvalidTitleError:
                     pywikibot.exception()
 
             prio_queue = []
             next_prio = 0
             rvgen = api.PropertyGenerator(props, site=self)
             rvgen.set_maximum_items(-1)  # suppress use of "rvlimit" parameter
 
-            if len(pageids) == len(sublist) \
+            if len(pageids) == len(batch) \
                and len(set(pageids)) <= self.maxlimit:
                 # only use pageids if all pages have them
                 rvgen.request['pageids'] = set(pageids)
             else:
                 rvgen.request['titles'] = list(cache.keys())
             rvgen.request['rvprop'] = self._rvprops(content=content)
             if not quiet:
@@ -1554,16 +1554,15 @@
     def _check_view_deleted(self, msg_prefix: str, prop: List[str]) -> None:
         """Check if the user can view deleted comments and content.
 
         :param msg_prefix: The calling method name
         :param prop: Requested props to check
         :raises UserRightsError: user cannot view a requested prop
         """
-        err = '{}: User:{} not authorized to view '.format(msg_prefix,
-                                                           self.user())
+        err = f'{msg_prefix}: User:{self.user()} not authorized to view '
         if not self.has_right('deletedhistory'):
             if self.mw_version < '1.34':
                 raise UserRightsError(err + 'deleted revisions.')
             if 'comment' in prop or 'parsedcomment' in prop:
                 raise UserRightsError(err + 'comments of deleted revisions.')
         if ('content' in prop and not (self.has_right('deletedtext')
                                        or self.has_right('undelete'))):
@@ -1897,15 +1896,15 @@
 
         :param special_page: Special page to query
         :param total: number of pages to return
         :raise AssertionError: special_page is not supported in SpecialPages.
         """
         param = self._paraminfo.parameter('query+querypage', 'page')
         assert special_page in param['type'], (
-            '{} not in {}'.format(special_page, param['type']))
+            f"{special_page} not in {param['type']}")
 
         return self._generator(api.PageGenerator,
                                type_arg='querypage', gqppage=special_page,
                                total=total)
 
     def longpages(self, total=None):
         """Yield Pages and lengths from Special:Longpages.
```

### Comparing `pywikibot-8.1.2/pywikibot/site/_interwikimap.py` & `pywikibot-8.2.0/pywikibot/site/_interwikimap.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/site/_namespace.py` & `pywikibot-8.2.0/pywikibot/site/_namespace.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/site/_obsoletesites.py` & `pywikibot-8.2.0/pywikibot/site/_obsoletesites.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 
 
 class ClosedSite(APISite):
     """Site closed to read-only mode."""
 
     def _closed_error(self, notice: str = '') -> None:
         """An error instead of pointless API call."""
-        pywikibot.error('Site {} has been closed. {}'.format(self.sitename,
-                                                             notice))
+        pywikibot.error(f'Site {self.sitename} has been closed. {notice}')
 
     def page_restrictions(
             self, page: 'pywikibot.Page') -> Dict[str, Tuple[str, str]]:
         """Return a dictionary reflecting page protections."""
         if not page.exists():
             raise NoPageError(page)
         if not hasattr(page, '_protection'):
```

### Comparing `pywikibot-8.1.2/pywikibot/site/_siteinfo.py` & `pywikibot-8.2.0/pywikibot/site/_siteinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
             props = []
         if force:
             props = [prop for prop in props if prop not in self._cache]
             if props:
                 pywikibot.debug(
                     "Load siteinfo properties '{}' along with 'general'"
                     .format("', '".join(props)))
-            props += ['general']
+            props.append('general')
             default_info = self._get_siteinfo(props, expiry)
             for prop in props:
                 self._cache[prop] = default_info[prop]
             if key in default_info:
                 return default_info[key]
         if key in self._cache['general'][0]:
             return self._cache['general'][0][key], self._cache['general']
```

### Comparing `pywikibot-8.1.2/pywikibot/site/_tokenwallet.py` & `pywikibot-8.2.0/pywikibot/site/_tokenwallet.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/site/_upload.py` & `pywikibot-8.2.0/pywikibot/site/_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Objects representing API upload to MediaWiki site."""
 #
-# (C) Pywikibot team, 2009-2022
+# (C) Pywikibot team, 2009-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import mimetypes
 import os
 from collections.abc import Iterable
 from typing import Optional
@@ -177,16 +177,15 @@
         file_size = None
 
         # make sure file actually exists
         if self.filename:
             if os.path.isfile(self.filename):
                 file_size = os.path.getsize(self.filename)
             elif offset is not False:
-                raise ValueError("File '{}' does not exist."
-                                 .format(self.filename))
+                raise ValueError(f"File '{self.filename}' does not exist.")
 
         # Verify the stash when a file key and offset is given:
         # requests the SHA1 and file size uploaded and compares it to
         # the local file. Also verify that offset is matching the
         # file size if the offset is an int. If offset is False if
         # verifies that the file size match with the local file.
         verify_stash = False
@@ -205,15 +204,15 @@
                 raise ValueError('Without a file key it cannot request the '
                                  'stash information')
             if not self.filename:
                 raise ValueError('Can request stash information only when '
                                  'using a file name.')
             props = ['size']
             if verify_stash:
-                props += ['sha1']
+                props.append('sha1')
             stash_info = self.site.stash_info(file_key, props)
             if offset is True:
                 offset = stash_info['size']
             elif offset is False:
                 if file_size != stash_info['size']:
                     raise ValueError(
                         'For the file key "{}" the server reported a size '
@@ -238,16 +237,16 @@
 
         assert offset is not True
         if file_key and file_size is None:
             assert offset is False
 
         data = {}
         if file_key and offset is False or offset == file_size:
-            pywikibot.log('Reused already upload file using filekey "{}"'
-                          .format(file_key))
+            pywikibot.log(
+                f'Reused already upload file using filekey "{file_key}"')
             # TODO: Use sessionkey instead of filekey if necessary
             final_request = self.site._request(
                 parameters={
                     'action': 'upload',
                     'token': token,
                     'filename': file_page_title,
                     'comment': self.comment,
@@ -266,16 +265,15 @@
             with open(self.filename, 'rb') as f:
                 final_request = self.site._request(
                     throttle=throttle, parameters={
                         'action': 'upload', 'token': token, 'text': self.text,
                         'filename': file_page_title, 'comment': self.comment})
                 if chunked_upload:
                     if offset > 0:
-                        pywikibot.log('Continuing upload from byte {}'
-                                      .format(offset))
+                        pywikibot.log(f'Continuing upload from byte {offset}')
                     poll = False
                     while True:
 
                         if poll:
                             # run a poll; not possible in first iteration
                             assert file_key
                             req = self.site.simple_request(
@@ -518,9 +516,9 @@
                     pywikibot.info('Upload successful.')
                 # If we receive a nochange, that would mean we're in simulation
                 # mode, don't attempt to access imageinfo
                 if 'nochange' not in result:
                     self.filepage._load_file_revisions([result['imageinfo']])
                 return True
 
-            raise Error('Unrecognized result: {}'
-                        .format(data_result or result['result']))
+            raise Error(
+                f"Unrecognized result: {data_result or result['result']}")
```

### Comparing `pywikibot-8.1.2/pywikibot/site_detect.py` & `pywikibot-8.2.0/pywikibot/site_detect.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/specialbots/_unlink.py` & `pywikibot-8.2.0/pywikibot/specialbots/_unlink.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/specialbots/_upload.py` & `pywikibot-8.2.0/pywikibot/specialbots/_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Special bot library containing UploadRobot.
 
 Do not import classes directly from here but from specialbots.
 """
 #
-# (C) Pywikibot team, 2003-2022
+# (C) Pywikibot team, 2003-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import os
 import tempfile
 from contextlib import suppress
 from http import HTTPStatus
@@ -154,16 +154,16 @@
                     # stream content to temp file (in chunks of 1Mb)
                     for chunk in response.iter_content(chunk_size=1024 * 1024):
                         fd.write(chunk)
 
                 # raised from connection lost during response.iter_content()
                 except requests.ConnectionError:
                     fd.flush()
-                    pywikibot.info('Connection closed at byte {}'
-                                   .format(path.stat().st_size))
+                    pywikibot.info(
+                        f'Connection closed at byte {path.stat().st_size}')
                 # raised from response.raise_for_status()
                 except requests.HTTPError as e:
                     # exit criteria if size is not available
                     # error on last iteration is OK, we're requesting
                     #    {'Range': 'bytes=file_len-'}
                     err = HTTPStatus.REQUESTED_RANGE_NOT_SATISFIABLE
                     if response.status_code == err and path.stat().st_size:
@@ -226,17 +226,16 @@
             filename = urlparse(filename).path
         filename = os.path.basename(filename)
         if self.use_filename:
             filename = self.use_filename
         if self.filename_prefix:
             filename = self.filename_prefix + filename
         if not self.keep_filename:
-            pywikibot.info(
-                '\nThe filename on the target wiki will default to: {}\n'
-                .format(filename))
+            pywikibot.info(f'\nThe filename on the target wiki will default '
+                           f'to: {filename}\n')
             assert not self.opt.always
             newfn = pywikibot.input(
                 'Enter a better name, or press enter to accept:')
             if newfn != '':
                 filename = newfn
         # FIXME: these 2 belong somewhere else, presumably in family
         # forbidden characters are handled by pywikibot/page.py
@@ -408,17 +407,16 @@
                 success = imagepage.upload(file_url,
                                            ignore_warnings=ignore_warnings,
                                            chunk_size=self.chunk_size,
                                            asynchronous=self.asynchronous,
                                            comment=self.summary)
             except APIError as error:
                 if error.code == 'uploaddisabled':
-                    pywikibot.error(
-                        'Upload error: Local file uploads are disabled on {}.'
-                        .format(site))
+                    pywikibot.error(f'Upload error: Local file uploads are '
+                                    f'disabled on {site}.')
                 elif error.code == 'copyuploadbaddomain' and not download \
                         and '://' in file_url:
                     pywikibot.error(error)
                     pywikibot.info('Downloading the file and retry...')
                     download = True
                     continue
                 else:
@@ -460,16 +458,15 @@
         if self.skip_run():
             return
         try:
             for file_url in self.url:
                 self.upload_file(file_url)
                 self.counter['read'] += 1
         except QuitKeyboardInterrupt:
-            pywikibot.info('\nUser quit {} bot run...'
-                           .format(self.__class__.__name__))
+            pywikibot.info(f'\nUser quit {self.__class__.__name__} bot run...')
         except KeyboardInterrupt:
             if config.verbose_output:
                 raise
 
             pywikibot.info('\nKeyboardInterrupt during {} bot run...'
                            .format(self.__class__.__name__))
         finally:
```

### Comparing `pywikibot-8.1.2/pywikibot/textlib.py` & `pywikibot-8.2.0/pywikibot/textlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-"""Functions for manipulating wiki-text.
-
-Unless otherwise noted, all functions take a unicode string as the
-argument and return a unicode string.
-"""
+"""Functions for manipulating wiki-text."""
 #
 # (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import re
 from collections import OrderedDict, namedtuple
 from collections.abc import Sequence
 from contextlib import suppress
 from html.parser import HTMLParser
 from typing import NamedTuple, Optional, Union
 
 import pywikibot
-from pywikibot.backports import Container, Dict, Iterable, List
+from pywikibot.backports import (
+    Callable,
+    Container,
+    Dict,
+    Iterable,
+    Match,
+    List,
+)
 from pywikibot.backports import OrderedDict as OrderedDictType
+from pywikibot.backports import Pattern
 from pywikibot.backports import Sequence as SequenceType
 from pywikibot.backports import Tuple
 from pywikibot.exceptions import InvalidTitleError, SiteDefinitionError
 from pywikibot.family import Family
 from pywikibot.time import TZoneFixedOffset
 from pywikibot.tools import (
     ModuleDeprecationWrapper,
@@ -38,15 +42,15 @@
 except ImportError:
     import mwparserfromhell as wikitextparser
 
 
 ETPType = List[Tuple[str, OrderedDictType[str, str]]]
 
 # cache for replaceExcept to avoid recompile or regexes each call
-_regex_cache = {}
+_regex_cache: Dict[str, Pattern[str]] = {}
 
 # The regex below collects nested templates, providing simpler
 # identification of templates used at the top-level of wikitext.
 # It doesn't match {{{1|...}}}, however it also does not match templates
 # with a numerical name. e.g. {{1|..}}. It will correctly match {{{x}} as
 # being {{x}} with leading '{' left in the wikitext.
 # Prefix msg: is not included in the 'name' group, but all others are
@@ -165,17 +169,15 @@
     .. versionadded:: 7.0
 
     :param case: if `case` is 'first-letter' the regex contains an
         upper/lower case set for the first letter
     """
     first = string[0]
     if first.isalpha() and case == 'first-letter':
-        pattern = '[{}{}]{}'.format(first.upper(),
-                                    first.lower(),
-                                    re.escape(string[1:]))
+        pattern = f'[{first.upper()}{first.lower()}]{re.escape(string[1:])}'
     else:
         pattern = re.escape(string)
     return pattern
 
 
 class MultiTemplateMatchBuilder:
 
@@ -245,15 +247,23 @@
 
 def _tag_regex(tag_name: str):
     """Return a compiled tag regex for the given tag name."""
     return re.compile(_tag_pattern(tag_name))
 
 
 def _create_default_regexes() -> None:
-    """Fill (and possibly overwrite) _regex_cache with default regexes."""
+    """Fill (and possibly overwrite) ``_regex_cache`` with default regexes.
+
+    The following keys are provided: ``category``, ``comment``, ``file``,
+    ``header``, ``hyperlink``, ``interwiki``, ``invoke``, ``link``,
+    ``pagelist``, ``property``, ``startcolon``, ``startspace``, ``table``,
+    ``template``.
+
+    :meta public:
+    """
     _regex_cache.update({
         # categories
         'category': (r'\[\[ *(?:%s)\s*:.*?\]\]',
                      lambda site: '|'.join(site.namespaces[14])),
         'comment': re.compile(r'<!--[\s\S]*?-->'),
         # files
         'file': (FILE_LINK_REGEX, lambda site: '|'.join(site.namespaces[6])),
@@ -296,49 +306,63 @@
         # TODO: handle nested tables.
         'table': re.compile(
             r'(?:(?<=\n)|\A){\|[\S\s]*?\n\|}|%s' % _tag_pattern('table')),
         'template': NESTED_TEMPLATE_REGEX,
     })
 
 
-def _get_regexes(keys, site):
-    """Fetch compiled regexes."""
+def get_regexes(
+    keys: Union[str, Iterable[str]],
+    site: Optional['pywikibot.site.BaseSite'] = None
+) -> List[Pattern[str]]:
+    """Fetch compiled regexes.
+
+    .. versionchanged:: 8.2
+       ``_get_regexes`` becomes a public function.
+       *keys* may be a single string; *site* is optional.
+
+    :param keys: a single key or an iterable of keys whose regex pattern
+        should be given
+    :param site: a BaseSite object needed for ``category``, ``file``,
+        ``interwiki``, ``invoke`` and ``property`` keys
+    :raises ValueError: site cannot be None.
+    """
     if not _regex_cache:
         _create_default_regexes()
 
-    result = []
+    if isinstance(keys, str):
+        keys = [keys]
 
+    result = []
     for exc in keys:
         if not isinstance(exc, str):
             # assume it's a regular expression
             result.append(exc)
             continue
 
         # assume the string is a reference to a standard regex above,
         # which may not yet have a site specific re compiled.
-        if exc in _regex_cache:
-            if isinstance(_regex_cache[exc], tuple):
-                if not site and exc in ('interwiki', 'property', 'invoke',
-                                        'category', 'file'):
-                    raise ValueError("Site cannot be None for the '{}' regex"
-                                     .format(exc))
-
-                if (exc, site) not in _regex_cache:
-                    re_text, re_var = _regex_cache[exc]
-                    _regex_cache[(exc, site)] = re.compile(
-                        re_text % re_var(site), re.VERBOSE)
-
-                result.append(_regex_cache[(exc, site)])
-            else:
-                result.append(_regex_cache[exc])
-        else:
+        if exc not in _regex_cache:
             # nowiki, noinclude, includeonly, timeline, math and other
             # extensions
             _regex_cache[exc] = _tag_regex(exc)
             result.append(_regex_cache[exc])
+        elif not isinstance(_regex_cache[exc], tuple):
+            result.append(_regex_cache[exc])
+        else:
+            if not site and exc in ('interwiki', 'property', 'invoke',
+                                    'category', 'file'):
+                raise ValueError(f'site cannot be None for the {exc!r} regex')
+
+            if (exc, site) not in _regex_cache:
+                re_text, re_var = _regex_cache[exc]
+                _regex_cache[(exc, site)] = re.compile(
+                    re_text % re_var(site), re.VERBOSE)
+
+            result.append(_regex_cache[(exc, site)])
 
         # handle aliases
         if exc == 'source':
             result.append(_tag_regex('syntaxhighlight'))
         elif exc == 'syntaxhighlight':
             result.append(_tag_regex('source'))
         elif exc == 'chem':
@@ -346,55 +370,64 @@
         elif exc == 'math':
             result.append(_tag_regex('chem'))
             result.append(_tag_regex('ce'))
 
     return result
 
 
-def replaceExcept(text: str, old, new, exceptions: list,
-                  caseInsensitive: bool = False, allowoverlap: bool = False,
-                  marker: str = '', site=None, count: int = 0) -> str:
-    """
-    Return text with 'old' replaced by 'new', ignoring specified types of text.
-
-    Skips occurrences of 'old' within exceptions; e.g., within nowiki tags or
-    HTML comments. If caseInsensitive is true, then use case insensitive
-    regex matching. If allowoverlap is true, overlapping occurrences are all
-    replaced (watch out when using this, it might lead to infinite loops!).
+def replaceExcept(text: str,
+                  old: Union[str, Pattern[str]],
+                  new: Union[str, Callable[[Match[str]], str]],
+                  exceptions: List[Union[str, Pattern[str]]],
+                  caseInsensitive: bool = False,
+                  allowoverlap: bool = False,
+                  marker: str = '',
+                  site: Optional['pywikibot.site.BaseSite'] = None,
+                  count: int = 0) -> str:
+    """
+    Return text with *old* replaced by *new*, ignoring specified types of text.
+
+    Skip occurrences of *old* within *exceptions*; e.g. within nowiki
+    tags or HTML comments. If *caseInsensitive* is true, then use case
+    insensitive regex matching. If *allowoverlap* is true, overlapping
+    occurrences are all replaced
+
+    .. caution:: Watch out when using *allowoverlap*, it might lead to
+       infinite loops!
 
     :param text: text to be modified
     :param old: a compiled or uncompiled regular expression
-    :param new: a unicode string (which can contain regular
-        expression references), or a function which takes
-        a match object as parameter. See parameter repl of
-        re.sub().
+    :param new: a string (which can contain regular expression
+        references), or a function which takes a match object as
+        parameter. See parameter *repl* of ``re.sub()``.
     :param exceptions: a list of strings or already compiled regex
-        objects which signal what to leave out. Strings might be like
-        ['math', 'table', 'template'] for example.
+        objects which signal what to leave out. List of strings might be
+        like ``['math', 'table', 'template']`` for example.
     :param marker: a string that will be added to the last replacement;
         if nothing is changed, it is added at the end
     :param count: how many replacements to do at most. See parameter
-        count of re.sub().
+        *count* of ``re.sub()``.
     """
     # if we got a string, compile it as a regular expression
     if isinstance(old, str):
         old = re.compile(old, flags=re.IGNORECASE if caseInsensitive else 0)
 
     # early termination if not relevant
     if not old.search(text):
         return text + marker
 
-    dontTouchRegexes = _get_regexes(exceptions, site)
+    dontTouchRegexes = get_regexes(exceptions, site)
 
     index = 0
     replaced = 0
     markerpos = len(text)
     while not count or replaced < count:
         if index > len(text):
             break
+
         match = old.search(text, index)
         if not match:
             # nothing left to replace
             break
 
         # check which exception will occur next.
         nextExceptionMatch = None
@@ -406,63 +439,65 @@
                 nextExceptionMatch = excMatch
 
         if nextExceptionMatch is not None \
                 and nextExceptionMatch.start() <= match.start():
             # an HTML comment or text in nowiki tags stands before the next
             # valid match. Skip.
             index = nextExceptionMatch.end()
+            continue
+
+        # We found a valid match. Replace it.
+        if callable(new):
+            # the parameter new can be a function which takes the match
+            # as a parameter.
+            replacement = new(match)
         else:
-            # We found a valid match. Replace it.
-            if callable(new):
-                # the parameter new can be a function which takes the match
-                # as a parameter.
-                replacement = new(match)
-            else:
-                # it is not a function, but a string.
+            # it is not a function, but a string.
 
-                # it is a little hack to make \n work. It would be better
-                # to fix it previously, but better than nothing.
-                new = new.replace('\\n', '\n')
-
-                # We cannot just insert the new string, as it may contain regex
-                # group references such as \2 or \g<name>.
-                # On the other hand, this approach does not work because it
-                # can't handle lookahead or lookbehind (see bug T123185).
-                # So we have to process the group references manually.
-                replacement = ''
-
-                group_regex = re.compile(r'\\(\d+)|\\g<(.+?)>')
-                last = 0
-                for group_match in group_regex.finditer(new):
-                    group_id = group_match[1] or group_match[2]
-                    with suppress(ValueError):
-                        group_id = int(group_id)
-
-                    try:
-                        replacement += new[last:group_match.start()]
-                        replacement += match[group_id] or ''
-                    except IndexError:
-                        raise IndexError('Invalid group reference: {}\n'
-                                         'Groups found: {}'
-                                         .format(group_id, match.groups()))
-                    last = group_match.end()
-                replacement += new[last:]
-
-            text = text[:match.start()] + replacement + text[match.end():]
-
-            # continue the search on the remaining text
-            if allowoverlap:
-                index = match.start() + 1
-            else:
-                index = match.start() + len(replacement)
-            if not match.group():
-                # When the regex allows to match nothing, shift by one char
-                index += 1
-            markerpos = match.start() + len(replacement)
-            replaced += 1
+            # it is a little hack to make \n work. It would be better
+            # to fix it previously, but better than nothing.
+            new = new.replace('\\n', '\n')
+
+            # We cannot just insert the new string, as it may contain regex
+            # group references such as \2 or \g<name>.
+            # On the other hand, this approach does not work because it
+            # can't handle lookahead or lookbehind (see bug T123185).
+            # So we have to process the group references manually.
+            replacement = ''
+
+            group_regex = re.compile(r'\\(\d+)|\\g<(.+?)>')
+            last = 0
+            for group_match in group_regex.finditer(new):
+                group_id = group_match[1] or group_match[2]
+                with suppress(ValueError):
+                    group_id = int(group_id)
+
+                try:
+                    replacement += new[last:group_match.start()]
+                    replacement += match[group_id] or ''
+                except IndexError:
+                    raise IndexError(f'Invalid group reference: {group_id}\n'
+                                     f'Groups found: {match.groups()}')
+                last = group_match.end()
+            replacement += new[last:]
+
+        text = text[:match.start()] + replacement + text[match.end():]
+
+        # continue the search on the remaining text
+        if allowoverlap:
+            index = match.start() + 1
+        else:
+            index = match.start() + len(replacement)
+
+        if not match.group():
+            # When the regex allows to match nothing, shift by one char
+            index += 1
+
+        markerpos = match.start() + len(replacement)
+        replaced += 1
 
     return text[:markerpos] + marker + text[markerpos:]
 
 
 def removeDisabledParts(text: str,
                         tags: Optional[Iterable] = None,
                         include: Optional[Container] = None,
@@ -480,15 +515,15 @@
     * source and syntaxhighlight tags
 
     .. versionchanged:: 7.0
        the order of removals will correspond to the tags argument
        if provided as an ordered collection (list, tuple)
 
     :param tags: The exact set of parts which should be removed using
-        keywords from textlib._get_regexes().
+        keywords from :func:`get_regexes`.
     :param include: Or, in alternative, default parts that shall not
         be removed.
     :param site: Site to be used for site-dependent regexes. Default
         disabled parts listed above do not need it.
     :return: text stripped from disabled parts.
     """
     if not tags:
@@ -498,15 +533,15 @@
     # this function would likely be different per script run because
     # the replacements would be done in different order and the disabled
     # parts may overlap and suppress each other
     # see https://docs.python.org/3/reference/datamodel.html#object.__hash__
     # ("Note" at the end of the section)
     if include:
         tags = [tag for tag in tags if tag not in include]
-    regexes = _get_regexes(tags, site)
+    regexes = get_regexes(tags, site)
     for regex in regexes:
         text = regex.sub('', text)
     return text
 
 
 def removeHTMLParts(text: str, keeptags: Optional[List[str]] = None) -> str:
     """
@@ -631,16 +666,15 @@
     that link. When it's False it unlinks it and just inserts the label. When
     it is a Link instance it'll use the target, section and label from that
     Link instance. If it's a Page instance it'll use just the target from the
     replacement and the section and label from the original link.
 
     If it's a string and the replacement was a sequence it converts it into a
     Page instance. If the replacement is done via a callable it'll use it like
-    unlinking and directly replace the link with the text itself. It only
-    supports unicode when used by the callable and bytes are not allowed.
+    unlinking and directly replace the link with the text itself.
 
     If either the section or label should be used the replacement can be a
     function which returns a Link instance and copies the value which should
     remaining.
 
     .. versionchanged:: 7.0
        `site` parameter is mandatory
@@ -791,16 +825,14 @@
 
         if new_link is False:
             # unlink - we remove the section if there's any
             assert isinstance(new_label, str), 'link text must be str.'
             new_link = new_label
 
         if isinstance(new_link, str):
-            # Nothing good can come out of the fact that bytes is returned so
-            # force unicode
             text = text[:start] + new_link + text[end:]
             # Make sure that next time around we will not find this same hit.
             curpos = start + len(new_link)
             continue
 
         if isinstance(new_link, bytes):
             raise ValueError('The result must be str and not bytes.')
@@ -851,16 +883,16 @@
                 must_piped = (
                     not parsed_link_title.startswith(new_link_title)
                     or parsed_new_label.namespace != new_link.namespace)
 
         if must_piped:
             new_text = f'[[{new_title}|{new_label}]]'
         else:
-            new_text = '[[{}]]{}'.format(new_label[:len(new_title)],
-                                         new_label[len(new_title):])
+            new_text = (f'[[{new_label[:len(new_title)]}]]'
+                        f'{new_label[len(new_title):]}')
 
         text = text[:start] + new_text + text[end:]
         # Make sure that next time around we will not find this same hit.
         curpos = start + len(new_text)
     return text
 
 
@@ -895,101 +927,191 @@
     # Adding the interwiki
     return replaceLanguageLinks(text, interwiki_inside, site)
 
 
 # -------------------------------
 # Functions dealing with sections
 # -------------------------------
+
+#: Head pattern
+HEAD_PATTERN = re.compile('{0}[^=]+{0}'.format('(={1,6})'))
+TITLE_PATTERN = re.compile("'{3}([^']+)'{3}")
+
 _Heading = namedtuple('_Heading', ('text', 'start', 'end'))
-_Section = namedtuple('_Section', ('title', 'content'))
-_Content = namedtuple('_Content', ('header', 'sections', 'footer'))
 
 
-def _extract_headings(text: str, site) -> list:
+class Section(NamedTuple):
+
+    """A namedtuple as part of :class:`Content` describing a page section.
+
+    .. versionchanged:: 8.2
+       ``_Section`` becomes a public class.
+    """
+
+    title: str  #: section title including equal signs
+    content: str  #: section content
+
+    @property
+    def level(self) -> int:
+        """Return the section level.
+
+        .. versionadded:: 8.2
+        """
+        m = HEAD_PATTERN.match(self.title)
+        return min(map(len, m.groups()))
+
+    @property
+    def heading(self) -> str:
+        """Return the section title without equal signs.
+
+        .. versionadded:: 8.2
+        """
+        level = self.level
+        return self.title[level:-level].strip()
+
+
+class Content(NamedTuple):
+
+    """A namedtuple as result of :func:`extract_sections` holding page content.
+
+    .. versionchanged:: 8.2
+       ``_Content`` becomes a public class.
+    """
+
+    header: str  #: the page header
+    sections: List[Section]  #: the page sections
+    footer: str  #: the page footer
+
+    @property
+    def title(self) -> str:
+        """Return the first main title found on the page.
+
+        The first main title is anything enclosed within triple quotes.
+
+        .. versionadded:: 8.2
+        """
+        m = TITLE_PATTERN.search(self.header)
+        return m[1].strip() if m else ''
+
+
+def _extract_headings(text: str) -> List[_Heading]:
     """Return _Heading objects."""
     headings = []
-    heading_regex = _get_regexes(['header'], site)[0]
+    heading_regex = get_regexes('header')[0]
     for match in heading_regex.finditer(text):
         start, end = match.span()
         if not isDisabled(text, start) and not isDisabled(text, end):
             headings.append(_Heading(match.group(), start, end))
     return headings
 
 
-def _extract_sections(text: str, headings) -> list:
-    """Return _Section objects."""
+def _extract_sections(text: str, headings) -> List[Section]:
+    """Return a list of :class:`Section` objects."""
+    sections = []
     if headings:
         # Assign them their contents
-        contents = []
         for i, heading in enumerate(headings):
             try:
                 next_heading = headings[i + 1]
             except IndexError:
-                contents.append(text[heading.end:])
+                content = text[heading.end:]
             else:
-                contents.append(text[heading.end:next_heading.start])
-        return [_Section(heading.text, content)
-                for heading, content in zip(headings, contents)]
-    return []
+                content = text[heading.end:next_heading.start]
+            sections.append(Section(heading.text, content))
+
+    return sections
 
 
 def extract_sections(
-    text: str, site=None
-) -> NamedTuple('_Content', [('header', str),  # noqa: F821
-                             ('sections', List[Tuple[str, str]]),  # noqa: F821
-                             ('footer', str)]):  # noqa: F821
-    """
-    Return section headings and contents found in text.
-
-    :return: The returned namedtuple contains the text parsed into
-        header, contents and footer parts: The header part is a string
-        containing text part above the first heading. The footer part
-        is also a string containing text part after the last section.
-        The section part is a list of tuples, each tuple containing a
-        string with section heading and a string with section content.
-        Example article::
-
-            '''A''' is a thing.
-
-            == History of A ==
-            Some history...
-
-            == Usage of A ==
-            Some usage...
-
-            [[Category:Things starting with A]]
-
-        ...is parsed into the following namedtuple::
-
-            result = extract_sections(text, site)
-            result.header = "'''A''' is a thing."
-            result.sections = [('== History of A ==', 'Some history...'),
-                               ('== Usage of A ==', 'Some usage...')]
-            result.footer = '[[Category:Things starting with A]]'
+    text: str,
+    site: Optional['pywikibot.site.BaseSite'] = None
+) -> Content:
+    """Return section headings and contents found in text.
+
+    The returned namedtuple :class:`Content` contains the text parsed
+    into *header*, *sections* and *footer* parts. The main title found
+    in the header which is the first text enclosed with ''' like
+    '''page title''' can be given by the *title* property.
+
+    The header part is a string containing text part above the first
+    heading.
+
+    The sections part is a list of :class:`Section` namedtuples, each
+    tuple containing a string with section title (including equal signs),
+    and a string with the section content. In addition the section
+    heading (the title without equal signs) can be given by the *heading*
+    property. Also the section level can be found by the *level*
+    property which is the number of the equal signs around the section
+    heading.
+
+    The footer part is also a string containing text part after the last
+    section.
+
+    **Examples:**
+
+    >>> text = \"\"\"
+    ... '''this''' is a Python module.
+    ...
+    ... == History of this ==
+    ... This set of principles was posted in 1999...
+    ...
+    ... == Usage of this ==
+    ... Enter "import this" for usage...
+    ...
+    ... === Details ===
+    ... The Zen of Python...
+    ...
+    ... [[Category:Programming principles]]
+    ... \"\"\"
+    >>> site = pywikibot.Site('wikipedia:en')
+    >>> result = extract_sections(text, site)
+    >>> result.header.strip()
+    "'''this''' is a Python module."
+    >>> result.sections[0].title
+    '== History of this =='
+    >>> result.sections[1].content.strip()
+    'Enter "import this" for usage...'
+    >>> result.sections[2].heading
+    'Details'
+    >>> result.sections[2].level
+    3
+    >>> result.footer.strip()
+    '[[Category:Programming principles]]'
+    >>> result.title
+    'this'
 
+    .. note:: sections and text from templates are not extracted but
+       embedded as plain text.
     .. versionadded:: 3.0
-    """
-    headings = _extract_headings(text, site)
+    .. versionchanged:: 8.2
+       The :class:`Content` and :class:`Section` class have additional
+       properties.
+
+    :return: The parsed namedtuple.
+    """  # noqa: D300, D301
+    headings = _extract_headings(text)
     sections = _extract_sections(text, headings)
     # Find header and footer contents
     header = text[:headings[0].start] if headings else text
-    cat_regex, interwiki_regex = _get_regexes(('category', 'interwiki'), site)
+    cat_regex, interwiki_regex = get_regexes(['category', 'interwiki'], site)
     langlink_pattern = interwiki_regex.pattern.replace(':?', '')
     last_section_content = sections[-1].content if sections else header
     footer = re.search(
         r'({})*\Z'.format(r'|'.join((langlink_pattern,
                                      cat_regex.pattern, r'\s'))),
         last_section_content).group().lstrip()
+
     if footer:
         if sections:
-            sections[-1] = _Section(
+            sections[-1] = Section(
                 sections[-1].title, last_section_content[:-len(footer)])
         else:
             header = header[:-len(footer)]
-    return _Content(header, sections, footer)
+
+    return Content(header, sections, footer)
 
 
 # -----------------------------------------------
 # Functions dealing with interwiki language links
 # -----------------------------------------------
 # Note - MediaWiki supports several kinds of interwiki links; two kinds are
 #        inter-language links. We deal here with those kinds only.
@@ -1234,15 +1356,15 @@
         above_interwiki.append(comment)
 
     if site.family.name == 'wikipedia' and site.code in ('ba', 'crh', 'krc'):
         comment = re.compile(r'<!-- [Ii]nterwikis -->')
         above_interwiki.append(comment)
 
     if above_interwiki:
-        interwiki = _get_regexes(['interwiki'], site)[0]
+        interwiki = get_regexes('interwiki', site)[0]
         first_interwiki = interwiki.search(newtext)
         for reg in above_interwiki:
             special = reg.search(newtext)
             if special and not isDisabled(newtext, special.start()):
                 newtext = (newtext[:special.start()].strip()
                            + newtext[special.end():])
                 newtext = (newtext[:first_interwiki.start()].strip()
@@ -1304,15 +1426,15 @@
         firstsites = []
         validlanglinks = insite.validLanguageLinks()
         for code in putfirst:
             if code in validlanglinks:
                 site = insite.getSite(code=code)
                 if site in sites:
                     del sites[sites.index(site)]
-                    firstsites += [site]
+                    firstsites.append(site)
         sites = firstsites + sites
     return sites
 
 
 # -------------------------------------
 # Functions dealing with category links
 # -------------------------------------
@@ -1343,21 +1465,20 @@
             rest = match_rest
         if '|' in rest:
             title, sortKey = rest.split('|', 1)
         else:
             title, sortKey = rest, None
         try:
             cat = pywikibot.Category(site,
-                                     '{}:{}'.format(match['namespace'], title),
+                                     f"{match['namespace']}:{title}",
                                      sort_key=sortKey)
         except InvalidTitleError:
             # Category title extracted contains invalid characters
             # Likely due to on-the-fly category name creation, see T154309
-            pywikibot.warning('Invalid category title extracted: {}'
-                              .format(title))
+            pywikibot.warning(f'Invalid category title extracted: {title}')
         else:
             result.append(cat)
 
     return result
 
 
 def removeCategoryLinks(text: str, site=None, marker: str = '') -> str:
@@ -1548,15 +1669,15 @@
         under_categories.append(stub)
 
     if site.family.name == 'wikipedia' and site.code in ('simple', 'en'):
         stub = re.compile(r'\{\{.*?stub *\}\}', re.I)
         under_categories.append(stub)
 
     if under_categories:
-        category = _get_regexes(['category'], site)[0]
+        category = get_regexes('category', site)[0]
         for last_category in category.finditer(newtext):
             pass
         for reg in under_categories:
             special = reg.search(newtext)
             if special and not isDisabled(newtext, special.start()):
                 newtext = (newtext[:special.start()].strip()
                            + newtext[special.end():])
@@ -1615,15 +1736,15 @@
     """Return a regex that matches external links."""
     # RFC 2396 says that URLs may only contain certain characters.
     # For this regex we also accept non-allowed characters, so that the bot
     # will later show these links as broken ('Non-ASCII Characters in URL').
     # Note: While allowing dots inside URLs, MediaWiki will regard
     # dots at the end of the URL as not part of that URL.
     # The same applies to comma, colon and some other characters.
-    notAtEnd = r'\]\s\.:;,<>"\|\)'
+    notAtEnd = r'\]\s\.:;,<>"\|\)}'
     # So characters inside the URL can be anything except whitespace,
     # closing squared brackets, quotation marks, greater than and less
     # than, and the last character also can't be parenthesis or another
     # character disallowed by MediaWiki.
     notInside = r'\]\s<>"'
     # The first half of this regular expression is required because '' is
     # not allowed inside links. For example, in this wiki text:
```

### Comparing `pywikibot-8.1.2/pywikibot/throttle.py` & `pywikibot-8.2.0/pywikibot/throttle.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/time.py` & `pywikibot-8.2.0/pywikibot/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,14 +441,12 @@
     if len(string) < 2:
         raise ValueError('Time period should be a numeric value followed by '
                          'its qualifier')
 
     key, duration = string[-1], string[:-1]
 
     if key not in MW_KEYS:
-        raise ValueError('Time period qualifier is unrecognized: {}'
-                         .format(string))
+        raise ValueError(f'Time period qualifier is unrecognized: {string}')
     if not duration.isdigit():
-        raise ValueError("Time period's duration should be numeric: {}"
-                         .format(string))
+        raise ValueError(f"Time period's duration should be numeric: {string}")
 
     return key, int(duration)
```

### Comparing `pywikibot-8.1.2/pywikibot/titletranslate.py` & `pywikibot-8.2.0/pywikibot/titletranslate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/tools/__init__.py` & `pywikibot-8.2.0/pywikibot/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import stat
 import subprocess
 import sys
 from contextlib import suppress
 from functools import total_ordering, wraps
 from importlib import import_module
 from types import TracebackType
-from typing import Any, Optional, Type
+from typing import Any, Optional, Type, Union
 from warnings import catch_warnings, showwarning, warn
 
 import pkg_resources
 
 import pywikibot  # T306760
 from pywikibot.backports import Callable
 from pywikibot.tools._deprecate import (
@@ -642,16 +642,16 @@
 
         try:
             process = subprocess.Popen(['7za', 'e', '-bd', '-so', filename],
                                        stdout=subprocess.PIPE,
                                        stderr=subprocess.PIPE,
                                        bufsize=65535)
         except OSError:
-            raise ValueError('7za is not installed or cannot uncompress "{}"'
-                             .format(filename))
+            raise ValueError(
+                f'7za is not installed or cannot uncompress "{filename}"')
 
         stderr = process.stderr.read()
         process.stderr.close()
         if stderr != b'':
             process.stdout.close()
             raise OSError(
                 f'Unexpected STDERR output from 7za {stderr}')
@@ -717,48 +717,56 @@
     if stat.S_ISREG(st_mode) and (st_mode - stat.S_IFREG != mode):
         os.chmod(filename, mode)
         # re-read and check changes
         if os.stat(filename).st_mode != st_mode and not quiet:
             warn(warn_str.format(filename, st_mode - stat.S_IFREG, mode))
 
 
-def compute_file_hash(filename: str, sha: str = 'sha1', bytes_to_read=None):
+def compute_file_hash(filename: Union[str, os.PathLike],
+                      sha: Union[str, Callable[[], Any]] = 'sha1',
+                      bytes_to_read: Optional[int] = None) -> str:
     """Compute file hash.
 
     Result is expressed as hexdigest().
 
     .. versionadded:: 3.0
+    .. versionchanged:: 8.2
+       *sha* may be  also a hash constructor, or a callable that returns
+       a hash object.
 
-    :param filename: filename path
-    :param sha: hashing function among the following in hashlib:
-        md5(), sha1(), sha224(), sha256(), sha384(), and sha512()
-        function name shall be passed as string, e.g. 'sha1'.
-    :param bytes_to_read: only the first bytes_to_read will be considered;
-        if file size is smaller, the whole file will be considered.
-    :type bytes_to_read: None or int
 
+    :param filename: filename path
+    :param sha: hash algorithm available with hashlib: ``sha1()``,
+        ``sha224()``, ``sha256()``, ``sha384()``, ``sha512()``,
+        ``blake2b()``, and ``blake2s()``. Additional algorithms like
+        ``md5()``, ``sha3_224()``, ``sha3_256()``, ``sha3_384()``,
+        ``sha3_512()``, ``shake_128()`` and ``shake_256()`` may also be
+        available. *sha* must either be a hash algorithm name as a str
+        like ``'sha1'`` (default), a hash constructor like
+        ``hashlib.sha1``, or a callable that returns a hash object like
+        ``lambda: hashlib.sha1()``.
+    :param bytes_to_read: only the first bytes_to_read will be
+        considered; if file size is smaller, the whole file will be
+        considered.
     """
-    size = os.path.getsize(filename)
-    if bytes_to_read is None:
-        bytes_to_read = size
-    else:
-        bytes_to_read = min(bytes_to_read, size)
-    step = 1 << 20
-
-    shas = ['md5', 'sha1', 'sha224', 'sha256', 'sha384', 'sha512']
-    assert sha in shas
-    sha = getattr(hashlib, sha)()  # sha instance
-
     with open(filename, 'rb') as f:
-        while bytes_to_read > 0:
-            read_bytes = f.read(min(bytes_to_read, step))
-            assert read_bytes  # make sure we actually read bytes
-            bytes_to_read -= len(read_bytes)
-            sha.update(read_bytes)
-    return sha.hexdigest()
+        if PYTHON_VERSION < (3, 11) or bytes_to_read is not None:
+            digest = sha() if callable(sha) else hashlib.new(sha)
+            size = os.path.getsize(filename)
+            bytes_to_read = min(bytes_to_read or size, size)
+            step = 1 << 20
+            while bytes_to_read > 0:
+                read_bytes = f.read(min(bytes_to_read, step))
+                assert read_bytes  # make sure we actually read bytes
+                bytes_to_read -= len(read_bytes)
+                digest.update(read_bytes)
+        else:
+            digest = hashlib.file_digest(f, sha)
+
+    return digest.hexdigest()
 
 
 def cached(*arg: Callable) -> Any:
     """Decorator to cache information of an object.
 
     The wrapper adds an attribute to the instance which holds the result
     of the decorated method. The attribute's name is the method name
@@ -826,15 +834,16 @@
     'EMPTY_DEFAULT',
     replacement_name='pywikibot.tools.collections.EMPTY_DEFAULT',
     since='7.6.0')
 
 # Deprecate objects which has to be imported from tools.itertools instead
 wrapper.add_deprecated_attr(
     'itergroup',
-    replacement_name='pywikibot.tools.itertools.itergroup',
+    # new replacement in 8.2
+    replacement_name='pywikibot.backports.batched',
     since='7.6.0')
 wrapper.add_deprecated_attr(
     'islice_with_ellipsis',
     replacement_name='pywikibot.tools.itertools.islice_with_ellipsis',
     since='7.6.0')
 wrapper.add_deprecated_attr(
     'intersect_generators',
```

### Comparing `pywikibot-8.1.2/pywikibot/tools/_deprecate.py` & `pywikibot-8.2.0/pywikibot/tools/_deprecate.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 # Distributed under the terms of the MIT license.
 #
 import collections
 import inspect
 import re
 import sys
 import types
+
 from contextlib import suppress
 from importlib import import_module
 from inspect import getfullargspec
-from typing import Any, Optional
+from typing import Any, Optional, Union
 from warnings import warn
 
 
 class _NotImplementedWarning(RuntimeWarning):
 
     """Feature that is no longer implemented.
 
@@ -57,16 +58,15 @@
         return
     # The current frame is add_decorated_full_name
     # The next frame is the decorator
     # The next frame is the object being decorated
     frame = sys._getframe(stacklevel + 1)
     class_name = frame.f_code.co_name
     if class_name and class_name != '<module>':
-        obj.__full_name__ = '{}.{}.{}'.format(obj.__module__,
-                                              class_name, obj.__name__)
+        obj.__full_name__ = f'{obj.__module__}.{class_name}.{obj.__name__}'
     else:
         obj.__full_name__ = f'{obj.__module__}.{obj.__name__}'
 
 
 def manage_wrapping(wrapper, obj) -> None:
     """Add attributes to wrapper and wrapped functions.
 
@@ -158,15 +158,15 @@
 
     if not __debug__:
         return obj  # pragma: no cover
 
     return outer_wrapper
 
 
-def _build_msg_string(instead: str, since: str) -> str:
+def _build_msg_string(instead: Optional[str], since: Optional[str]) -> str:
     """Build a deprecation warning message format string.
 
     .. versionadded:: 3.0
 
     .. versionchanged:: 7.0
        `since`parameter must be a release number, not a timestamp.
 
@@ -179,27 +179,32 @@
     if instead:
         msg = '{{0}} is deprecated{since}; use {{1}} instead.'
     else:
         msg = '{{0}} is deprecated{since}.'
     return msg.format(since=' since release ' + since if since else '')
 
 
-def issue_deprecation_warning(name: str, instead: str = '', depth: int = 2,
-                              warning_class=None, since: str = '') -> None:
+def issue_deprecation_warning(name: str,
+                              instead: Optional[str] = None,
+                              depth: int = 2, *,
+                              warning_class: Optional[type] = None,
+                              since: Optional[str] = None):
     """Issue a deprecation warning.
 
     .. versionchanged:: 7.0
-       `since` parameter must be a release number, not a timestamp.
+       *since* parameter must be a release number, not a timestamp.
+
+    .. versionchanged:: 8.2
+       *warning_class* and *since* are keyword-only parameters.
 
     :param name: the name of the deprecated object
     :param instead: suggested replacement for the deprecated object
     :param depth: depth + 1 will be used as stacklevel for the warnings
-    :param warning_class: a warning class (category) to be used, defaults to
-        FutureWarning
-    :type warning_class: type
+    :param warning_class: a warning class (category) to be used,
+        defaults to FutureWarning
     :param since: a version string string when the method was deprecated
     """
     msg = _build_msg_string(instead, since)
     if warning_class is None:
         warning_class = (FutureWarning
                          if instead else _NotImplementedWarning)
     warn(msg.format(name, instead), warning_class, depth + 1)
@@ -294,34 +299,34 @@
 
         return decorator(args[0])
 
     # Otherwise return a decorator, which returns a replacement function
     return decorator
 
 
-def deprecate_arg(old_arg: str, new_arg):
+def deprecate_arg(old_arg: str, new_arg: Union[str, None, bool]):
     """Decorator to declare old_arg deprecated and replace it with new_arg.
 
     Usage:
 
         @deprecate_arg('foo', 'bar')
         def my_function(bar='baz'): pass
         # replaces 'foo' keyword by 'bar' used by my_function
 
         @deprecare_arg('foo', None)
         def my_function(): pass
         # ignores 'foo' keyword no longer used by my_function
 
-    deprecated_args decorator should be used in favour of this
-    deprecate_arg decorator but it is held to deprecate args which become
-    a reserved word in future Python releases and to prevent syntax errors.
+    :func:`deprecated_args` decorator should be used in favour of this
+    ``deprecate_arg`` decorator but it is held to deprecate args which
+    become a reserved word in future Python releases and to prevent
+    syntax errors.
 
     :param old_arg: old keyword
     :param new_arg: new keyword
-    :type new_arg: str or None or bool
     """
     return deprecated_args(**{old_arg: new_arg})
 
 
 def deprecated_args(**arg_pairs):
     """Decorator to declare multiple args deprecated.
 
@@ -453,16 +458,15 @@
             :return: the value returned by the decorated function
             :rtype: any
             """
             name = obj.__full_name__
             depth = get_wrapper_depth(wrapper) + 1
             args, varargs, kwargs, *_ = getfullargspec(wrapper.__wrapped__)
             if varargs is not None and kwargs is not None:
-                raise ValueError('{} may not have * or ** args.'
-                                 .format(name))
+                raise ValueError(f'{name} may not have * or ** args.')
             deprecated = set(__kw) & set(arg_names)
             if len(__args) > len(args):
                 deprecated.update(arg_names[:len(__args) - len(args)])
             # remove at most |arg_names| entries from the back
             new_args = tuple(__args[:max(len(args),
                                          len(__args) - len(arg_names))])
             new_kwargs = {arg: val for arg, val in __kw.items()
@@ -480,28 +484,32 @@
 
         manage_wrapping(wrapper, obj)
 
         return wrapper
     return decorator
 
 
-def redirect_func(target, source_module: Optional[str] = None,
+def redirect_func(target, *,
+                  source_module: Optional[str] = None,
                   target_module: Optional[str] = None,
                   old_name: Optional[str] = None,
                   class_name: Optional[str] = None,
                   since: str = '',
                   future_warning: bool = True):
     """
     Return a function which can be used to redirect to 'target'.
 
     It also acts like marking that function deprecated and copies all
     parameters.
 
     .. versionchanged:: 7.0
-       ``since`` parameter must be a release number, not a timestamp.
+       *since* parameter must be a release number, not a timestamp.
+
+    .. versionchanged:: 8.2
+       All parameters except *target* are keyword-only parameters.
 
     :param target: The targeted function which is to be executed.
     :type target: callable
     :param source_module: The module of the old function. If '.' defaults
         to target_module. If 'None' (default) it tries to guess it from the
         executing function.
     :param target_module: The module of the target function. If
@@ -518,14 +526,15 @@
     :rtype: callable
     """
     def call(*a, **kw):
         issue_deprecation_warning(
             old_name, new_name, since=since,
             warning_class=None if future_warning else DeprecationWarning)
         return target(*a, **kw)
+
     if target_module is None:
         target_module = target.__module__
     if target_module and target_module[-1] != '.':
         target_module += '.'
     if source_module == '.':
         source_module = target_module
     elif source_module and source_module[-1] != '.':
@@ -590,21 +599,20 @@
         :param warning_message: The warning to display, with positional
             variables: {0} = module, {1} = attribute name, {2} = replacement.
         :param since: a version string string when the method was deprecated
         :param future_warning: if True a FutureWarning will be thrown,
             otherwise it provides a DeprecationWarning
         """
         if '.' in name:
-            raise ValueError('Deprecated name "{}" may not contain '
-                             '".".'.format(name))
+            raise ValueError(f'Deprecated name "{name}" may not contain ".".')
         if name in self._deprecated:
             raise ValueError(f'Name "{name}" is already deprecated.')
         if replacement is not None and hasattr(self._module, name):
-            raise ValueError('Module has already an attribute named '
-                             '"{}".'.format(name))
+            raise ValueError(
+                f'Module has already an attribute named "{name}".')
 
         if replacement_name is None:
             if hasattr(replacement, '__name__'):
                 replacement_name = replacement.__module__
                 if hasattr(replacement, '__self__'):
                     replacement_name += '.'
                     replacement_name += replacement.__self__.__class__.__name__
```

### Comparing `pywikibot-8.1.2/pywikibot/tools/_logging.py` & `pywikibot-8.2.0/pywikibot/tools/_logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/tools/_unidata.py` & `pywikibot-8.2.0/pywikibot/tools/_unidata.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/tools/chars.py` & `pywikibot-8.2.0/pywikibot/tools/chars.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pywikibot.tools._unidata import _category_cf
 
 
 # This is a set of all invisible characters
 # At the moment we've only added the characters from the Cf category
 _invisible_chars = _category_cf
 
-INVISIBLE_REGEX = re.compile('[{}]'.format(''.join(_invisible_chars)))
+INVISIBLE_REGEX = re.compile(f"[{''.join(_invisible_chars)}]")
 
 
 def contains_invisible(text):
     """Return True if the text contain any of the invisible characters."""
     return any(char in _invisible_chars for char in text)
```

### Comparing `pywikibot-8.1.2/pywikibot/tools/collections.py` & `pywikibot-8.2.0/pywikibot/tools/collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/tools/djvu.py` & `pywikibot-8.2.0/pywikibot/tools/djvu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Wrapper around djvulibre to access djvu files properties and content."""
 #
-# (C) Pywikibot team, 2015-2022
+# (C) Pywikibot team, 2015-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import os
 import re
 import subprocess
 from collections import Counter
@@ -71,17 +71,15 @@
         self._pat_form = re.compile(
             r' *?FORM:DJVU *?\[\d+\] *?(?P<id>{[^\}]*?})? *?\[P(?P<n>\d+)\]')
         self._pat_info = re.compile(
             r'DjVu.*?(?P<size>\d+x\d+).*?(?P<dpi>\d+) dpi')
 
     def __repr__(self) -> str:
         """Return a more complete string representation."""
-        return "{}.{}('{}')".format(self.__module__,
-                                    self.__class__.__name__,
-                                    self._filename)
+        return f"{self.__module__}.{type(self).__name__}('{self._filename}')"
 
     def __str__(self) -> str:
         """Return a string representation."""
         return f"{self.__class__.__name__}('{self._filename}')"
 
     def check_cache(fn):
         """Decorator to check if cache shall be cleared."""
@@ -219,16 +217,15 @@
         """
         Get page n for djvu file.
 
         :param n: page n of djvu file
         :param force: if True, refresh the cached data
         """
         if not self.has_text(force=force):
-            raise ValueError('Djvu file {} has no text layer.'
-                             .format(self.file))
+            raise ValueError(f'Djvu file {self.file} has no text layer.')
         res, stdoutdata = _call_cmd(['djvutxt', f'--page={n}',
                                      self.file])
         if not res:
             return False
         return self._remove_control_chars(stdoutdata)
 
     @check_page_number
```

### Comparing `pywikibot-8.1.2/pywikibot/tools/formatter.py` & `pywikibot-8.2.0/pywikibot/tools/formatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,24 +65,24 @@
 
 @deprecated('New color format pattern like <<color>>colored text<<default>>',
             since='7.2.0')
 def color_format(text: str, *args, **kwargs) -> str:
     r"""
     Do ``str.format`` without having to worry about colors.
 
-    It is automatically adding \03 in front of color fields so it's
-    unnecessary to add them manually. Any other \03 in the text is
+    It is automatically adding \\03 in front of color fields so it's
+    unnecessary to add them manually. Any other \\03 in the text is
     disallowed.
 
     You may use a variant {color} by assigning a valid color to a named
     parameter color.
 
     .. deprecated:: 7.2
-       new color format pattern like <<color>>colored text<<default>>
-       may be used instead.
+       new color format pattern like
+       ``f'<<{color}>>colored text<<default>>'`` can be used instead.
 
     :param text: The format template string
     :return: The formatted string
     :raises ValueError: Wrong format string or wrong keywords
     """
     colors = set(terminal_interface_base.colors)
     # Dot.product of colors to create all possible combinations of foreground
@@ -99,12 +99,11 @@
     if intersect:
         raise ValueError('Keyword argument(s) use valid color(s): '
                          + '", "'.join(intersect))
     try:
         text = text.format(*args, **kwargs)
     except KeyError as e:
         if str(e).strip("'") in colors:
-            raise ValueError(
-                'Color field "{}" in "{}" uses conversion information or '
-                'format spec'.format(e, text))
+            raise ValueError(f'Color field "{e}" in "{text}" uses conversion '
+                             f'information or format spec')
         raise
     return text
```

### Comparing `pywikibot-8.1.2/pywikibot/tools/itertools.py` & `pywikibot-8.2.0/pywikibot/tools/itertools.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 #
 import collections
 import itertools
 from contextlib import suppress
 from itertools import chain, zip_longest
 from typing import Any
 
-from pywikibot.backports import Generator
+from pywikibot.backports import batched, Generator, List
 from pywikibot.logging import debug
-from pywikibot.tools import issue_deprecation_warning
+from pywikibot.tools import deprecated, issue_deprecation_warning
 
 
 __all__ = (
     'filter_unique',
     'intersect_generators',
     'islice_with_ellipsis',
     'itergroup',
     'roundrobin_generators',
 )
 
 
+@deprecated('backports.batched()', since='8.2.0')
 def itergroup(iterable,
               size: int,
-              strict: bool = False) -> Generator[Any, None, None]:
+              strict: bool = False) -> Generator[List[Any], None, None]:
     """Make an iterator that returns lists of (up to) size items from iterable.
 
     Example:
 
     >>> i = itergroup(range(25), 10)
     >>> print(next(i))
     [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
@@ -43,29 +44,28 @@
     >>> print(next(i))
     [20, 21, 22, 23, 24]
     >>> print(next(i))
     Traceback (most recent call last):
      ...
     StopIteration
 
+    .. versionadded:: 7.6
+       The *strict* parameter.
+    .. deprecated:: 8.2
+       Use :func:`backports.batched` instead.
+
     :param size: How many items of the iterable to get in one chunk
     :param strict: If True, raise a ValueError if length of iterable is
         not divisible by `size`.
     :raises ValueError: iterable is not divisible by size
     """
-    group = []
-    for item in iterable:
-        group.append(item)
-        if len(group) == size:
-            yield group
-            group = []
-    if group:
-        if strict:
+    for group in batched(iterable, size):
+        if strict and len(group) < size:
             raise ValueError('iterable is not divisible by size.')
-        yield group
+        yield list(group)
 
 
 def islice_with_ellipsis(iterable, *args, marker: str = '…'):
     """
     Generator which yields the first n elements of the iterable.
 
     If more elements are available and marker is True, it returns an extra
```

### Comparing `pywikibot-8.1.2/pywikibot/tools/threading.py` & `pywikibot-8.2.0/pywikibot/tools/threading.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,33 +194,30 @@
         :param wait_time: how long to wait if active threads exceeds limit
         """
         self.limit = limit
         self.wait_time = wait_time
         super().__init__(*args)
         for item in self:
             if not isinstance(item, threading.Thread):
-                raise TypeError("Cannot add '{}' to ThreadList"
-                                .format(type(item)))
+                raise TypeError(f"Cannot add '{type(item)}' to ThreadList")
 
     def active_count(self):
         """Return the number of alive threads and delete all non-alive ones."""
         cnt = 0
         for item in self[:]:
             if item.is_alive():
                 cnt += 1
             else:
                 self.remove(item)
         return cnt
 
     def append(self, thd):
         """Add a thread to the pool and start it."""
         if not isinstance(thd, threading.Thread):
-            raise TypeError("Cannot append '{}' to ThreadList"
-                            .format(type(thd)))
+            raise TypeError(f"Cannot append '{type(thd)}' to ThreadList")
 
         while self.active_count() >= self.limit:
             time.sleep(self.wait_time)
 
         super().append(thd)
         thd.start()
-        pywikibot.logging.debug("thread {} ('{}') started"
-                                .format(len(self), type(thd)))
+        pywikibot.logging.debug(f"thread {len(self)} ('{type(thd)}') started")
```

### Comparing `pywikibot-8.1.2/pywikibot/userinterfaces/__init__.py` & `pywikibot-8.2.0/pywikibot/userinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/userinterfaces/_interface_base.py` & `pywikibot-8.2.0/pywikibot/userinterfaces/_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/userinterfaces/buffer_interface.py` & `pywikibot-8.2.0/pywikibot/userinterfaces/buffer_interface.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/userinterfaces/gui.py` & `pywikibot-8.2.0/pywikibot/userinterfaces/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #
 from typing import Optional
 
 import pywikibot
 from pywikibot.backports import Tuple
 from pywikibot.tools import PYTHON_VERSION
 
+
 try:
     import idlelib
 except ImportError as e:
     idlelib = e
     ConfigDialog = ReplaceDialog = SearchDialog = object()
     idleConf = MultiCallCreator = object()  # noqa:  N816
 else:
```

### Comparing `pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_base.py` & `pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
             issue_deprecation_warning(
                 'old color format variant like \03{color}',
                 'new color format like <<color>>',
                 since='7.3.0')
             text_parts = old_parts
         else:
             text_parts = new_parts
-        text_parts += ['default']
+        text_parts.append('default')
         # match.split() includes every regex group; for each matched color
         # fg_col:b_col, fg_col and bg_col are added to the resulting list.
         len_text_parts = len(text_parts[::4])
         for index, (text, next_color) in enumerate(zip(text_parts[::4],
                                                        text_parts[1::4])):
             current_color = color_stack[-1]
             if next_color == 'previous':
@@ -457,15 +457,15 @@
         if isinstance(options, Option):
             options = [options]
         else:  # make a copy
             options = list(options)
         if not options:
             raise ValueError('No options are given.')
         if automatic_quit:
-            options += [QuitKeyboardInterrupt()]
+            options.append(QuitKeyboardInterrupt())
         if default:
             default = default.lower()
         for i, option in enumerate(options):
             if not isinstance(option, Option):
                 if len(option) != 2:
                     raise ValueError('Option #{} does not consist of an '
                                      'option and shortcut.'.format(i))
@@ -511,16 +511,15 @@
             an answer.
         :param force: Automatically use the default.
         :return: Return a single Sequence entry.
         """
         # lock stream output
         with self.lock:
             if not force:
-                line_template = '{{0: >{}}}: {{1}}\n'.format(
-                    len(str(len(answers))))
+                line_template = f'{{0: >{len(str(len(answers)))}}}: {{1}}\n'
                 for i, entry in enumerate(answers, start=1):
                     self.stream_output(line_template.format(i, entry))
 
             while True:
                 choice = self.input(question, default=default, force=force)
 
                 try:
@@ -532,16 +531,15 @@
 
                 # User typed choice number
                 if 0 <= choice < len(answers):
                     return answers[choice]
 
                 if force:
                     raise ValueError(
-                        'Invalid value "{}" for default during force.'
-                        .format(default))
+                        f'Invalid value "{default}" for default during force.')
 
                 self.stream_output('Error: Invalid response\n')
 
     @staticmethod
     def editText(text: str,
                  jumpIndex: Optional[int] = None,
                  highlight: Optional[str] = None) -> Optional[str]:
```

### Comparing `pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_unix.py` & `pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_unix.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/userinterfaces/terminal_interface_win32.py` & `pywikibot-8.2.0/pywikibot/userinterfaces/terminal_interface_win32.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/userinterfaces/transliteration.py` & `pywikibot-8.2.0/pywikibot/userinterfaces/transliteration.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot/version.py` & `pywikibot-8.2.0/pywikibot/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,15 @@
             '', '-1 (unknown)', '0 (unknown)', '(unknown)')
         warn('Unable to detect version; exceptions raised:\n{!r}'
              .format(exceptions), UserWarning)
         exceptions = None
 
     # Git and SVN can silently fail, as it may be a nightly.
     if exceptions:
-        pywikibot.debug('version algorithm exceptions:\n{!r}'
-                        .format(exceptions))
+        pywikibot.debug(f'version algorithm exceptions:\n{exceptions!r}')
 
     if isinstance(date, str):
         datestring = date
     elif isinstance(date, time.struct_time):
         datestring = time.strftime('%Y/%m/%d, %H:%M:%S', date)
     else:
         warn('Unable to detect package date', UserWarning)
@@ -248,15 +247,15 @@
     if remote_pos == -1:
         tag = '?'
     else:
         s = tag.find('url = ', remote_pos)
         e = tag.find('\n', s)
         tag = tag[(s + 6):e]
         t = tag.strip().split('/')
-        tag = '[{}] {}'.format(t[0][:-1], '-'.join(t[3:]))
+        tag = f"[{t[0][:-1]}] {'-'.join(t[3:])}"
     dp = subprocess.Popen([cmd, '--no-pager',
                            'log', '-1',
                            '--pretty=format:"%ad|%an|%h|%H|%d"',
                            '--abbrev-commit',
                            '--date=iso'],
                           cwd=_program_dir,
                           stdout=subprocess.PIPE)
```

### Comparing `pywikibot-8.1.2/pywikibot/xmlreader.py` & `pywikibot-8.2.0/pywikibot/xmlreader.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/pywikibot.egg-info/PKG-INFO` & `pywikibot-8.2.0/pywikibot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.1.2
+Version: 8.2.0
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -154,15 +154,15 @@
 `MediaWiki API <https://www.mediawiki.org/wiki/API:Main_page>`_
 version 1.27 or higher.
 
 Also included are various general function scripts that can be adapted for
 different tasks.
 
 For further information about the library excluding scripts see
-the full `code documentation <https://doc.wikimedia.org/pywikibot/>`_.
+the full `code documentation <https://doc.wikimedia.org/pywikibot/stable/>`_.
 
 Quick start
 ===========
 
 .. code:: text
 
     pip install requests
@@ -257,22 +257,42 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Add support for guwwikinews (T334461)
-* Add support for kbdwiktionary (T333271)
-* Fix tools.chars.url2stringparsing for multiple encodings (T335224)
+* Add support for gpewiki (T335989)
+* family.WikibaseFamilyand family.DefaultWikibaseFamilywere added to familymodule
+* Remove incorrect time normalization in page.Claim(T338748, T325860, T57755)
+* Add support for other types of diffs in Site.compare()
+* Improvements for textlib.extract_sectionsfunction (T338748)
+* Backport ``itertools.batched()`` from Python 3.12 which replaces tools.itertools.itergroup
+* Upcast page types in pagegenerators.RecentChangesPageGenerator(T340450)
+* Enable FilePage.download()to download thumbnails (T247095)
+* Refactor tools.compute_file_hashand use ``hashlib.file_digest`` with Python 3.11
+* Url ends with curly bracket in textlib.compileLinkR(T338029)
+* Allows spaces in environment variables for editor.TextEditor(T102465, T323078)
+* Add textlib.get_regexespublic function (T336144)
+* Return 'https' scheme with family.Family.protocol(T326046)
+* Use ``build`` instead of ``setuptools.setup()`` to build the distribution
+* Raise ``ConnectionError`` on ``requests.ReadTimeout`` in comms.http.error_handling_callback
+* Raise exceptions.ServerErroron ``requests.ReadTimeout`` in comms.http.error_handling_callback
+* Do not evaluate pywikibot.Sitewith dict.pop() as default value (T335720)
+* L10N updates
+* family.Familyclass was rewritten. ``obsolete.setter`` was removed,
+  family.Family.interwiki_replacementsreturns an invariant mapping,
+  family.Family.interwiki_removalsreturns a frozenset. ``closed_wikis``,
+  ``removed_wikis`` and ``code_aliases`` are family.Familyclass attributes.  (T334834)
 
 
 Deprecations
 ------------
 
+* 8.2.0: *normalize* parameter of WbTime.toTimestrand WbTime.toWikibasewill be removed
 * 8.1.0: Dependency of exceptions.NoSiteLinkErrorfrom exceptions.NoPageErrorwill be removed
 * 8.1.0: ``exceptions.Server414Error`` is deprecated in favour of exceptions.Client414Error
 * 8.0.0: Timestamp.clone()method is deprecated
   in favour of ``Timestamp.replace()`` method.
 * 8.0.0: family.Family.maximum_GET_lengthmethod is deprecated in favour of
   config.maximum_GET_length(T325957)
 * 8.0.0: ``addOnly`` parameter of textlib.replaceLanguageLinksand
@@ -295,18 +315,16 @@
 * 7.4.0: ``FilePage.usingPages()`` was renamed to using_pages()
 * 7.2.0: ``tb`` parameter of exception()function was renamed to ``exc_info``
 * 7.2.0: XMLDumpOldPageGenerator is deprecated in favour of a ``content`` parameter of
   XMLDumpPageGenerator(T306134)
 * 7.2.0: RedirectPageBot and NoRedirectPageBot bot classes are deprecated in favour of
   use_redirectsattribute
 * 7.2.0: tools.formatter.color_formatis deprecated and will be removed
-* 7.1.0: Unused `get_redirect` parameter of Page.getOldVersion() will be removed
-* 7.1.0: APISite._simple_request() will be removed in favour of APISite.simple_request()
+* 7.1.0: Unused ``get_redirect`` parameter of Page.getOldVersion()will be removed
 * 7.0.0: User.isBlocked() method is renamed to is_blocked for consistency
-* 7.0.0: Private BaseBot counters _treat_counter, _save_counter, _skip_counter will be removed in favour of collections.Counter counter attribute
 * 7.0.0: A boolean watch parameter in Page.save() is deprecated and will be desupported
 * 7.0.0: baserevid parameter of editSource(), editQualifier(), removeClaims(), removeSources(), remove_qualifiers() DataSite methods will be removed
 * 7.0.0: Values of APISite.allpages() parameter filterredir other than True, False and None are deprecated
 * 7.0.0: The i18n identifier 'cosmetic_changes-append' will be removed in favour of 'pywikibot-cosmetic-changes'
 * 6.5.0: OutputOption.output() method will be removed in favour of OutputOption.out property
 * 6.5.0: Infinite rotating file handler with logfilecount of -1 is deprecated
 * 6.4.0: 'allow_duplicates' parameter of tools.itertools.intersect_generatorsas positional argument is deprecated, use keyword argument instead
```

### Comparing `pywikibot-8.1.2/pywikibot.egg-info/SOURCES.txt` & `pywikibot-8.2.0/pywikibot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 AUTHORS.rst
+CODE_OF_CONDUCT.rst
 LICENSE
 MANIFEST.in
 README.rst
-make_dist.py
+ROADMAP.rst
 setup.py
 pywikibot/__init__.py
 pywikibot/__metadata__.py
 pywikibot/_wbtypes.py
 pywikibot/backports.py
 pywikibot/bot.py
 pywikibot/bot_choice.py
```

### Comparing `pywikibot-8.1.2/pywikibot.egg-info/requires.txt` & `pywikibot-8.2.0/pywikibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-8.1.2/setup.py` & `pywikibot-8.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,106 +116,107 @@
 name = 'pywikibot'
 path = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(path, name, '__metadata__.py')) as f:
     exec(f.read(), None, metadata)
 assert metadata.__name__ == name
 
 
-def get_validated_version() -> str:  # pragma: no cover
+def get_validated_version() -> str:
     """Get a validated pywikibot module version string.
 
     The version number from pywikibot.__metadata__.__version__ is used.
     setup.py with 'sdist' option is used to create a new source distribution.
     In that case the version number is validated: Read tags from git.
     Verify that the new release is higher than the last repository tag
     and is not a developmental release.
 
     :return: pywikibot module version string
     :rtype: str
     """
     version = metadata.__version__
     if 'sdist' not in sys.argv:
-        return version
+        return version  # pragma: no cover
 
     # validate version for sdist
     from contextlib import suppress
     from subprocess import PIPE, run
 
     from pkg_resources import parse_version, safe_version
     try:
         tags = run(['git', 'tag'], check=True, stdout=PIPE,
                    universal_newlines=True).stdout.splitlines()
-    except Exception as e:
+    except Exception as e:  # pragma: no cover
         print(e)
         sys.exit('Creating source distribution canceled.')
 
-    for tag in ('stable', 'python2'):
-        with suppress(ValueError):
-            tags.remove(tag)
+    last_tag = None
+    if tags:  # pragma: no cover
+        for tag in ('stable', 'python2'):
+            with suppress(ValueError):
+                tags.remove(tag)
 
-    last_tag = tags[-1]
+        last_tag = tags[-1]
 
     warnings = []
-    if parse_version(version) < parse_version('0'):
+    if parse_version(version) < parse_version('0'):  # pragma: no cover
         # any version which is not a valid PEP 440 version will be considered
         # less than any valid PEP 440 version
         warnings.append(
             version + ' is not a valid version string following PEP 440.')
-    elif safe_version(version) != version:
-        warnings.append(
-            '{} does not follow PEP 440. Use {} as version string instead.'
-            .format(version, safe_version(version)))
-
-    if parse_version(version) <= parse_version(last_tag):
-        warnings.append(
-            'New version "{}" is not higher than last version "{}".'
-            .format(version, last_tag))
+    elif safe_version(version) != version:  # pragma: no cover
+        warnings.append(f'{version} does not follow PEP 440. Use '
+                        f'{safe_version(version)} as version string instead.')
+
+    if last_tag and parse_version(version) <= parse_version(last_tag):
+        warnings.append(  # pragma: no cover
+            f'New version {version!r} is not higher than last version '
+            f'{last_tag!r}.')
 
-    if warnings:
+    if warnings:  # pragma: no cover
         print(__doc__)
         print('\n\n'.join(warnings))
         sys.exit('\nBuild of distribution package canceled.')
 
     return version
 
 
-def read_desc(filename) -> str:  # pragma: no cover
+def read_desc(filename) -> str:
     """Read long description.
 
     Combine included restructured text files which must be done before
     uploading because the source isn't available after creating the package.
     """
     pattern = r'(?:\:\w+\:`([^`]+?)(?:<.+>)?` *)', r'\1'
     desc = []
     with open(filename) as f:
         for line in f:
             if line.strip().startswith('.. include::'):
                 include = os.path.relpath(line.rsplit('::')[1].strip())
                 if os.path.exists(include):
                     with open(include) as g:
                         desc.append(re.sub(pattern[0], pattern[1], g.read()))
-                else:
-                    print('Cannot include {}; file not found'.format(include))
+                else:  # pragma: no cover
+                    print(f'Cannot include {include}; file not found')
             else:
                 desc.append(re.sub(pattern[0], pattern[1], line))
     return ''.join(desc)
 
 
-def get_packages(name) -> List[str]:  # pragma: no cover
+def get_packages(name) -> List[str]:
     """Find framework packages."""
     try:
         from setuptools import find_namespace_packages
     except ImportError:
         sys.exit(
             'setuptools >= 40.1.0 is required to create a new distribution.')
     packages = find_namespace_packages(include=[name + '.*'])
     return [str(name)] + packages
 
 
-def main() -> None:  # pragma: no cover
+def main() -> None:
     """Setup entry point."""
     version = get_validated_version()
     setup(
         name=metadata.__name__,
         version=version,
         description=metadata.__description__,
         long_description=read_desc('README.rst'),
@@ -346,12 +347,12 @@
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: Utilities',
         ],
     )
 
     # Finally show distribution version before uploading
     if 'sdist' in sys.argv:
-        print('\nDistribution package created for version {}'.format(version))
+        print(f'\nDistribution package created for version {version}')
 
 
 if __name__ == '__main__':  # pragma: no cover
     main()
```

### Comparing `pywikibot-8.1.2/tests/tests_tests.py` & `pywikibot-8.2.0/tests/tests_tests.py`

 * *Files identical despite different names*

