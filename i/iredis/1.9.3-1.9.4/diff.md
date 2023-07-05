# Comparing `tmp/iredis-1.9.3.tar.gz` & `tmp/iredis-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iredis-1.9.3.tar", max compression
+gzip compressed data, was "iredis-1.9.4.tar", max compression
```

## Comparing `iredis-1.9.3.tar` & `iredis-1.9.4.tar`

### file list

```diff
@@ -1,327 +1,356 @@
--rw-r--r--   0        0        0     1475 2021-07-07 06:40:15.049557 iredis-1.9.3/LICENSE
--rw-r--r--   0        0        0     8650 2021-07-07 06:40:15.049557 iredis-1.9.3/README.md
--rw-r--r--   0        0        0       22 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/__init__.py
--rw-r--r--   0        0        0      967 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/bottom.py
--rw-r--r--   0        0        0    25626 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/client.py
--rw-r--r--   0        0        0     4768 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/commands.py
--rw-r--r--   0        0        0    12714 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/completers.py
--rw-r--r--   0        0        0     4148 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/config.py
--rw-r--r--   0        0        0        0 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/__init__.py
--rw-r--r--   0        0        0    13244 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/command_syntax.csv
--rw-r--r--   0        0        0        0 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/__init__.py
--rw-r--r--   0        0        0     1722 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-cat.md
--rw-r--r--   0        0        0      579 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-deluser.md
--rw-r--r--   0        0        0     1996 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-genpass.md
--rw-r--r--   0        0        0      760 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-getuser.md
--rw-r--r--   0        0        0      153 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-help.md
--rw-r--r--   0        0        0      584 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-list.md
--rw-r--r--   0        0        0      923 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-load.md
--rw-r--r--   0        0        0     1161 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-log.md
--rw-r--r--   0        0        0      523 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-save.md
--rw-r--r--   0        0        0     5763 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-setuser.md
--rw-r--r--   0        0        0      204 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-users.md
--rw-r--r--   0        0        0      273 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/acl-whoami.md
--rw-r--r--   0        0        0     1907 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/append.md
--rw-r--r--   0        0        0     1660 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/auth.md
--rw-r--r--   0        0        0     1591 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/bgrewriteaof.md
--rw-r--r--   0        0        0      927 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/bgsave.md
--rw-r--r--   0        0        0     2506 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/bitcount.md
--rw-r--r--   0        0        0     6912 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/bitfield.md
--rw-r--r--   0        0        0     2153 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/bitop.md
--rw-r--r--   0        0        0     2365 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/bitpos.md
--rw-r--r--   0        0        0     7842 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/blpop.md
--rw-r--r--   0        0        0      971 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/brpop.md
--rw-r--r--   0        0        0      780 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/brpoplpush.md
--rw-r--r--   0        0        0     1262 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/bzpopmax.md
--rw-r--r--   0        0        0     1193 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/bzpopmin.md
--rw-r--r--   0        0        0     1032 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-caching.md
--rw-r--r--   0        0        0      300 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-getname.md
--rw-r--r--   0        0        0      701 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-getredir.md
--rw-r--r--   0        0        0      818 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-id.md
--rw-r--r--   0        0        0     3124 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-kill.md
--rw-r--r--   0        0        0     2593 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-list.md
--rw-r--r--   0        0        0     1799 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-pause.md
--rw-r--r--   0        0        0      881 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-reply.md
--rw-r--r--   0        0        0     1116 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-setname.md
--rw-r--r--   0        0        0     2884 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-tracking.md
--rw-r--r--   0        0        0     2466 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/client-unblock.md
--rw-r--r--   0        0        0     2243 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/cluster-addslots.md
--rw-r--r--   0        0        0      706 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/cluster-bumpepoch.md
--rw-r--r--   0        0        0     1867 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands/cluster-count-failure-reports.md
--rw-r--r--   0        0        0      403 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-countkeysinslot.md
--rw-r--r--   0        0        0     1881 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-delslots.md
--rw-r--r--   0        0        0     4249 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-failover.md
--rw-r--r--   0        0        0      204 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-flushslots.md
--rw-r--r--   0        0        0     2738 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-forget.md
--rw-r--r--   0        0        0      774 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-getkeysinslot.md
--rw-r--r--   0        0        0     2661 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-info.md
--rw-r--r--   0        0        0     1175 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-keyslot.md
--rw-r--r--   0        0        0     2687 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-meet.md
--rw-r--r--   0        0        0      192 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-myid.md
--rw-r--r--   0        0        0     7467 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-nodes.md
--rw-r--r--   0        0        0      806 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-replicas.md
--rw-r--r--   0        0        0     1219 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-replicate.md
--rw-r--r--   0        0        0     1316 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-reset.md
--rw-r--r--   0        0        0      779 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-saveconfig.md
--rw-r--r--   0        0        0     1167 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-set-config-epoch.md
--rw-r--r--   0        0        0     6919 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-setslot.md
--rw-r--r--   0        0        0     1147 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-slaves.md
--rw-r--r--   0        0        0     3255 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/cluster-slots.md
--rw-r--r--   0        0        0      177 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/command-count.md
--rw-r--r--   0        0        0      616 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/command-getkeys.md
--rw-r--r--   0        0        0      377 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/command-info.md
--rw-r--r--   0        0        0     4848 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/command.md
--rw-r--r--   0        0        0     1776 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/config-get.md
--rw-r--r--   0        0        0      364 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/config-resetstat.md
--rw-r--r--   0        0        0     1848 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/config-rewrite.md
--rw-r--r--   0        0        0     2554 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/config-set.md
--rw-r--r--   0        0        0       87 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/dbsize.md
--rw-r--r--   0        0        0      141 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/debug-object.md
--rw-r--r--   0        0        0      154 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/debug-segfault.md
--rw-r--r--   0        0        0      545 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/decr.md
--rw-r--r--   0        0        0      499 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/decrby.md
--rw-r--r--   0        0        0      207 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/del.md
--rw-r--r--   0        0        0      258 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/discard.md
--rw-r--r--   0        0        0     1003 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/dump.md
--rw-r--r--   0        0        0       91 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/echo.md
--rw-r--r--   0        0        0    36215 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/eval.md
--rw-r--r--   0        0        0      182 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/evalsha.md
--rw-r--r--   0        0        0      496 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/exec.md
--rw-r--r--   0        0        0      969 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/exists.md
--rw-r--r--   0        0        0     6733 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/expire.md
--rw-r--r--   0        0        0      852 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/expireat.md
--rw-r--r--   0        0        0      719 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/flushall.md
--rw-r--r--   0        0        0      280 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/flushdb.md
--rw-r--r--   0        0        0     2481 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/geoadd.md
--rw-r--r--   0        0        0     1257 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/geodecode.md
--rw-r--r--   0        0        0     1019 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/geodist.md
--rw-r--r--   0        0        0     2450 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/geoencode.md
--rw-r--r--   0        0        0     1702 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/geohash.md
--rw-r--r--   0        0        0     1083 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/geopos.md
--rw-r--r--   0        0        0     4549 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/georadius.md
--rw-r--r--   0        0        0      849 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/georadiusbymember.md
--rw-r--r--   0        0        0      349 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/get.md
--rw-r--r--   0        0        0      488 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/getbit.md
--rw-r--r--   0        0        0      665 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/getrange.md
--rw-r--r--   0        0        0      708 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/getset.md
--rw-r--r--   0        0        0      666 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hdel.md
--rw-r--r--   0        0        0     2310 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hello.md
--rw-r--r--   0        0        0      307 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hexists.md
--rw-r--r--   0        0        0      296 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hget.md
--rw-r--r--   0        0        0      395 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hgetall.md
--rw-r--r--   0        0        0      607 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hincrby.md
--rw-r--r--   0        0        0     1214 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hincrbyfloat.md
--rw-r--r--   0        0        0      239 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hkeys.md
--rw-r--r--   0        0        0      247 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hlen.md
--rw-r--r--   0        0        0      517 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hmget.md
--rw-r--r--   0        0        0      438 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hmset.md
--rw-r--r--   0        0        0       38 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hscan.md
--rw-r--r--   0        0        0      390 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hset.md
--rw-r--r--   0        0        0      487 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hsetnx.md
--rw-r--r--   0        0        0      429 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hstrlen.md
--rw-r--r--   0        0        0      234 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/hvals.md
--rw-r--r--   0        0        0     5370 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/incr.md
--rw-r--r--   0        0        0      499 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/incrby.md
--rw-r--r--   0        0        0     1690 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/incrbyfloat.md
--rw-r--r--   0        0        0    16297 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/info.md
--rw-r--r--   0        0        0     1218 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/keys.md
--rw-r--r--   0        0        0      296 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/lastsave.md
--rw-r--r--   0        0        0     1768 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/latency-doctor.md
--rw-r--r--   0        0        0     1609 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/latency-graph.md
--rw-r--r--   0        0        0      264 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/latency-help.md
--rw-r--r--   0        0        0     1063 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/latency-history.md
--rw-r--r--   0        0        0      917 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/latency-latest.md
--rw-r--r--   0        0        0      879 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/latency-reset.md
--rw-r--r--   0        0        0      586 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/lindex.md
--rw-r--r--   0        0        0      505 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/linsert.md
--rw-r--r--   0        0        0      332 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/llen.md
--rw-r--r--   0        0        0     1922 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/lolwut.md
--rw-r--r--   0        0        0      278 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/lpop.md
--rw-r--r--   0        0        0     3214 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/lpos.md
--rw-r--r--   0        0        0      945 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/lpush.md
--rw-r--r--   0        0        0      558 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/lpushx.md
--rw-r--r--   0        0        0     1287 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/lrange.md
--rw-r--r--   0        0        0      824 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/lrem.md
--rw-r--r--   0        0        0      330 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/lset.md
--rw-r--r--   0        0        0     1460 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/ltrim.md
--rw-r--r--   0        0        0      175 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/memory-doctor.md
--rw-r--r--   0        0        0      156 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/memory-help.md
--rw-r--r--   0        0        0      312 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/memory-malloc-stats.md
--rw-r--r--   0        0        0      264 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/memory-purge.md
--rw-r--r--   0        0        0     2607 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/memory-stats.md
--rw-r--r--   0        0        0     1081 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/memory-usage.md
--rw-r--r--   0        0        0      336 2021-07-07 06:40:15.057557 iredis-1.9.3/iredis/data/commands/mget.md
--rw-r--r--   0        0        0     3841 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/migrate.md
--rw-r--r--   0        0        0      336 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/module-list.md
--rw-r--r--   0        0        0      482 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/module-load.md
--rw-r--r--   0        0        0      339 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/module-unload.md
--rw-r--r--   0        0        0     2716 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/monitor.md
--rw-r--r--   0        0        0      385 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/move.md
--rw-r--r--   0        0        0      477 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/mset.md
--rw-r--r--   0        0        0      745 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/msetnx.md
--rw-r--r--   0        0        0      189 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/multi.md
--rw-r--r--   0        0        0     3116 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/object.md
--rw-r--r--   0        0        0      409 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/persist.md
--rw-r--r--   0        0        0      305 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/pexpire.md
--rw-r--r--   0        0        0      350 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/pexpireat.md
--rw-r--r--   0        0        0     1139 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/pfadd.md
--rw-r--r--   0        0        0     4364 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/pfcount.md
--rw-r--r--   0        0        0      637 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/pfmerge.md
--rw-r--r--   0        0        0      513 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/ping.md
--rw-r--r--   0        0        0      201 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/psetex.md
--rw-r--r--   0        0        0      315 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/psubscribe.md
--rw-r--r--   0        0        0      391 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/psync.md
--rw-r--r--   0        0        0      730 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/pttl.md
--rw-r--r--   0        0        0      113 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/publish.md
--rw-r--r--   0        0        0     1551 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/pubsub.md
--rw-r--r--   0        0        0      275 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/punsubscribe.md
--rw-r--r--   0        0        0      172 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/quit.md
--rw-r--r--   0        0        0      141 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/randomkey.md
--rw-r--r--   0        0        0      882 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/readonly.md
--rw-r--r--   0        0        0      355 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/readwrite.md
--rw-r--r--   0        0        0      722 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/rename.md
--rw-r--r--   0        0        0      615 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/renamenx.md
--rw-r--r--   0        0        0      972 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/replicaof.md
--rw-r--r--   0        0        0     1205 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/restore.md
--rw-r--r--   0        0        0     3074 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/role.md
--rw-r--r--   0        0        0      276 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/rpop.md
--rw-r--r--   0        0        0     3049 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/rpoplpush.md
--rw-r--r--   0        0        0      943 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/rpush.md
--rw-r--r--   0        0        0      558 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/rpushx.md
--rw-r--r--   0        0        0      641 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sadd.md
--rw-r--r--   0        0        0      710 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/save.md
--rw-r--r--   0        0        0    13713 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/scan.md
--rw-r--r--   0        0        0      257 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/scard.md
--rw-r--r--   0        0        0     1273 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/script-debug.md
--rw-r--r--   0        0        0      823 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/script-exists.md
--rw-r--r--   0        0        0      154 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/script-flush.md
--rw-r--r--   0        0        0      795 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/script-kill.md
--rw-r--r--   0        0        0      657 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/script-load.md
--rw-r--r--   0        0        0      451 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sdiff.md
--rw-r--r--   0        0        0      378 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sdiffstore.md
--rw-r--r--   0        0        0     1294 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/select.md
--rw-r--r--   0        0        0     2520 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/set.md
--rw-r--r--   0        0        0     5268 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/setbit.md
--rw-r--r--   0        0        0      607 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/setex.md
--rw-r--r--   0        0        0     4309 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/setnx.md
--rw-r--r--   0        0        0     1692 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/setrange.md
--rw-r--r--   0        0        0     3044 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/shutdown.md
--rw-r--r--   0        0        0      573 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sinter.md
--rw-r--r--   0        0        0      380 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sinterstore.md
--rw-r--r--   0        0        0      307 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sismember.md
--rw-r--r--   0        0        0     1297 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/slaveof.md
--rw-r--r--   0        0        0     3319 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/slowlog.md
--rw-r--r--   0        0        0      254 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/smembers.md
--rw-r--r--   0        0        0      901 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/smove.md
--rw-r--r--   0        0        0     4723 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sort.md
--rw-r--r--   0        0        0     1140 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/spop.md
--rw-r--r--   0        0        0     2838 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/srandmember.md
--rw-r--r--   0        0        0      649 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/srem.md
--rw-r--r--   0        0        0       38 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sscan.md
--rw-r--r--   0        0        0     3767 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/stralgo.md
--rw-r--r--   0        0        0      288 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/strlen.md
--rw-r--r--   0        0        0      250 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/subscribe.md
--rw-r--r--   0        0        0      426 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sunion.md
--rw-r--r--   0        0        0      380 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sunionstore.md
--rw-r--r--   0        0        0      529 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/swapdb.md
--rw-r--r--   0        0        0      450 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/sync.md
--rw-r--r--   0        0        0      403 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/time.md
--rw-r--r--   0        0        0      217 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/touch.md
--rw-r--r--   0        0        0      837 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/ttl.md
--rw-r--r--   0        0        0      367 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/type.md
--rw-r--r--   0        0        0      542 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/unlink.md
--rw-r--r--   0        0        0      275 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/unsubscribe.md
--rw-r--r--   0        0        0      216 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/unwatch.md
--rw-r--r--   0        0        0     3265 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/wait.md
--rw-r--r--   0        0        0      158 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/watch.md
--rw-r--r--   0        0        0     1240 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xack.md
--rw-r--r--   0        0        0     3920 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xadd.md
--rw-r--r--   0        0        0     4184 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xclaim.md
--rw-r--r--   0        0        0     1869 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xdel.md
--rw-r--r--   0        0        0     2884 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xgroup.md
--rw-r--r--   0        0        0     5137 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xinfo.md
--rw-r--r--   0        0        0      637 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xlen.md
--rw-r--r--   0        0        0     4613 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xpending.md
--rw-r--r--   0        0        0     5866 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xrange.md
--rw-r--r--   0        0        0     8068 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xread.md
--rw-r--r--   0        0        0     6341 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xreadgroup.md
--rw-r--r--   0        0        0     2693 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xrevrange.md
--rw-r--r--   0        0        0     1205 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/xtrim.md
--rw-r--r--   0        0        0     4433 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zadd.md
--rw-r--r--   0        0        0      281 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zcard.md
--rw-r--r--   0        0        0      604 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zcount.md
--rw-r--r--   0        0        0      816 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zincrby.md
--rw-r--r--   0        0        0      977 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zinterstore.md
--rw-r--r--   0        0        0      721 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zlexcount.md
--rw-r--r--   0        0        0      552 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zpopmax.md
--rw-r--r--   0        0        0      552 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zpopmin.md
--rw-r--r--   0        0        0     1945 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zrange.md
--rw-r--r--   0        0        0     3129 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zrangebylex.md
--rw-r--r--   0        0        0     3247 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zrangebyscore.md
--rw-r--r--   0        0        0      605 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zrank.md
--rw-r--r--   0        0        0      575 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zrem.md
--rw-r--r--   0        0        0      701 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zremrangebylex.md
--rw-r--r--   0        0        0      623 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zremrangebyrank.md
--rw-r--r--   0        0        0      407 2021-07-07 06:40:15.061557 iredis-1.9.3/iredis/data/commands/zremrangebyscore.md
--rw-r--r--   0        0        0      545 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/data/commands/zrevrange.md
--rw-r--r--   0        0        0      518 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/data/commands/zrevrangebylex.md
--rw-r--r--   0        0        0      758 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/data/commands/zrevrangebyscore.md
--rw-r--r--   0        0        0      607 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/data/commands/zrevrank.md
--rw-r--r--   0        0        0       38 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/data/commands/zscan.md
--rw-r--r--   0        0        0      331 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/data/commands/zscore.md
--rw-r--r--   0        0        0     1379 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/data/commands/zunionstore.md
--rw-r--r--   0        0        0   103287 2021-07-07 06:40:15.053557 iredis-1.9.3/iredis/data/commands.json
--rw-r--r--   0        0        0      694 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/data/dangerous_commands.csv
--rw-r--r--   0        0        0     2079 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/data/iredisrc
--rw-r--r--   0        0        0    13613 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/entry.py
--rw-r--r--   0        0        0      420 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/exceptions.py
--rw-r--r--   0        0        0      642 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/key_bindings.py
--rw-r--r--   0        0        0     3955 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/lexer.py
--rw-r--r--   0        0        0     1932 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/markdown.py
--rw-r--r--   0        0        0     2310 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/processors.py
--rw-r--r--   0        0        0    25169 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/redis_grammar.py
--rw-r--r--   0        0        0    13575 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/renders.py
--rw-r--r--   0        0        0     2890 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/style.py
--rw-r--r--   0        0        0     9569 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/utils.py
--rw-r--r--   0        0        0     1621 2021-07-07 06:40:15.065557 iredis-1.9.3/iredis/warning.py
--rw-r--r--   0        0        0     1518 2021-07-07 06:40:15.065557 iredis-1.9.3/pyproject.toml
--rw-r--r--   0        0        0        0 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/__init__.py
--rw-r--r--   0        0        0      787 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_cli_pubsub.py
--rw-r--r--   0        0        0     2470 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_cli_start.py
--rw-r--r--   0        0        0     1483 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_command_input.py
--rw-r--r--   0        0        0     1219 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_completer.py
--rw-r--r--   0        0        0      590 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_config.py
--rw-r--r--   0        0        0     1523 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_dsn.py
--rw-r--r--   0        0        0     1085 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_history.py
--rw-r--r--   0        0        0      472 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_on_error.py
--rw-r--r--   0        0        0     3383 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_pager.py
--rw-r--r--   0        0        0      240 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_self_implemented_command.py
--rw-r--r--   0        0        0      571 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_shell_pipeline.py
--rw-r--r--   0        0        0      898 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_string_execute.py
--rw-r--r--   0        0        0     1769 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_transaction.py
--rw-r--r--   0        0        0     1343 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/test_warning.py
--rw-r--r--   0        0        0      248 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/cli_tests/wrappager.py
--rw-r--r--   0        0        0     3372 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/conftest.py
--rw-r--r--   0        0        0     1737 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_base_token.py
--rw-r--r--   0        0        0     8517 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_cluster.py
--rw-r--r--   0        0        0     2982 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_connection.py
--rw-r--r--   0        0        0     5805 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_generic_parse.py
--rw-r--r--   0        0        0     1011 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_geo.py
--rw-r--r--   0        0        0     1294 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_hash_parse.py
--rw-r--r--   0        0        0      163 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_hll_parse.py
--rw-r--r--   0        0        0     2897 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_list_parse.py
--rw-r--r--   0        0        0      428 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_pubsub.py
--rw-r--r--   0        0        0      801 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_script.py
--rw-r--r--   0        0        0     6513 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_server.py
--rw-r--r--   0        0        0     1258 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_set_parse.py
--rw-r--r--   0        0        0     4681 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_sorted_set_parse.py
--rw-r--r--   0        0        0    12661 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_stream.py
--rw-r--r--   0        0        0     9962 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/command_parse/test_string_parse.py
--rw-r--r--   0        0        0    16062 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/test_client.py
--rw-r--r--   0        0        0    11472 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/test_completers.py
--rw-r--r--   0        0        0     7134 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/test_entry.py
--rw-r--r--   0        0        0      763 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/test_markdown_doc_render.py
--rw-r--r--   0        0        0    14882 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/test_render_functions.py
--rw-r--r--   0        0        0     4064 2021-07-07 06:40:15.065557 iredis-1.9.3/tests/unittests/test_utils.py
--rw-r--r--   0        0        0     9986 2021-07-07 06:40:27.899457 iredis-1.9.3/setup.py
--rw-r--r--   0        0        0    10059 2021-07-07 06:40:27.900376 iredis-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1475 2021-07-15 10:17:12.611496 iredis-1.9.4/LICENSE
+-rw-r--r--   0        0        0     8666 2021-07-15 10:17:12.611496 iredis-1.9.4/README.md
+-rw-r--r--   0        0        0       22 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/__init__.py
+-rw-r--r--   0        0        0      967 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/bottom.py
+-rw-r--r--   0        0        0    26242 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/client.py
+-rw-r--r--   0        0        0     4768 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/commands.py
+-rw-r--r--   0        0        0    12714 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/completers.py
+-rw-r--r--   0        0        0     4148 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/config.py
+-rw-r--r--   0        0        0        0 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/__init__.py
+-rw-r--r--   0        0        0    13244 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/command_syntax.csv
+-rw-r--r--   0        0        0        0 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/__init__.py
+-rw-r--r--   0        0        0     1722 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-cat.md
+-rw-r--r--   0        0        0      579 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-deluser.md
+-rw-r--r--   0        0        0     1996 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-genpass.md
+-rw-r--r--   0        0        0      840 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-getuser.md
+-rw-r--r--   0        0        0      153 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-help.md
+-rw-r--r--   0        0        0      590 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-list.md
+-rw-r--r--   0        0        0      923 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-load.md
+-rw-r--r--   0        0        0     1161 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-log.md
+-rw-r--r--   0        0        0      523 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-save.md
+-rw-r--r--   0        0        0     6211 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-setuser.md
+-rw-r--r--   0        0        0      204 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-users.md
+-rw-r--r--   0        0        0      273 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/acl-whoami.md
+-rw-r--r--   0        0        0     1907 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/append.md
+-rw-r--r--   0        0        0     1726 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/auth.md
+-rw-r--r--   0        0        0     1591 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/bgrewriteaof.md
+-rw-r--r--   0        0        0      927 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/bgsave.md
+-rw-r--r--   0        0        0     2506 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/bitcount.md
+-rw-r--r--   0        0        0     6940 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/bitfield.md
+-rw-r--r--   0        0        0     2153 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/bitop.md
+-rw-r--r--   0        0        0     2365 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/bitpos.md
+-rw-r--r--   0        0        0      858 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/blmove.md
+-rw-r--r--   0        0        0     7923 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/blpop.md
+-rw-r--r--   0        0        0     1054 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/brpop.md
+-rw-r--r--   0        0        0      957 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/brpoplpush.md
+-rw-r--r--   0        0        0     1343 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/bzpopmax.md
+-rw-r--r--   0        0        0     1275 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/bzpopmin.md
+-rw-r--r--   0        0        0     1031 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-caching.md
+-rw-r--r--   0        0        0      300 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-getname.md
+-rw-r--r--   0        0        0      701 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-getredir.md
+-rw-r--r--   0        0        0      818 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-id.md
+-rw-r--r--   0        0        0      392 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-info.md
+-rw-r--r--   0        0        0     3112 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-kill.md
+-rw-r--r--   0        0        0     3357 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-list.md
+-rw-r--r--   0        0        0     2903 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-pause.md
+-rw-r--r--   0        0        0      881 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-reply.md
+-rw-r--r--   0        0        0     1116 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-setname.md
+-rw-r--r--   0        0        0     3107 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-tracking.md
+-rw-r--r--   0        0        0     1190 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-trackinginfo.md
+-rw-r--r--   0        0        0     2466 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-unblock.md
+-rw-r--r--   0        0        0      163 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/client-unpause.md
+-rw-r--r--   0        0        0     2242 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-addslots.md
+-rw-r--r--   0        0        0      706 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-bumpepoch.md
+-rw-r--r--   0        0        0     1867 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-count-failure-reports.md
+-rw-r--r--   0        0        0      403 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-countkeysinslot.md
+-rw-r--r--   0        0        0     1880 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-delslots.md
+-rw-r--r--   0        0        0     4249 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-failover.md
+-rw-r--r--   0        0        0      205 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-flushslots.md
+-rw-r--r--   0        0        0     2738 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-forget.md
+-rw-r--r--   0        0        0      774 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-getkeysinslot.md
+-rw-r--r--   0        0        0     2661 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-info.md
+-rw-r--r--   0        0        0     1175 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-keyslot.md
+-rw-r--r--   0        0        0     2687 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-meet.md
+-rw-r--r--   0        0        0      192 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-myid.md
+-rw-r--r--   0        0        0     7530 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-nodes.md
+-rw-r--r--   0        0        0      806 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-replicas.md
+-rw-r--r--   0        0        0     1219 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-replicate.md
+-rw-r--r--   0        0        0     1316 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-reset.md
+-rw-r--r--   0        0        0      779 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-saveconfig.md
+-rw-r--r--   0        0        0     1167 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-set-config-epoch.md
+-rw-r--r--   0        0        0     6928 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-setslot.md
+-rw-r--r--   0        0        0     1147 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-slaves.md
+-rw-r--r--   0        0        0     3255 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/cluster-slots.md
+-rw-r--r--   0        0        0      177 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/command-count.md
+-rw-r--r--   0        0        0      616 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/command-getkeys.md
+-rw-r--r--   0        0        0      377 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/command-info.md
+-rw-r--r--   0        0        0     5089 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/command.md
+-rw-r--r--   0        0        0     1776 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/config-get.md
+-rw-r--r--   0        0        0      364 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/config-resetstat.md
+-rw-r--r--   0        0        0     1848 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands/config-rewrite.md
+-rw-r--r--   0        0        0     2554 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/config-set.md
+-rw-r--r--   0        0        0      600 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/copy.md
+-rw-r--r--   0        0        0       87 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/dbsize.md
+-rw-r--r--   0        0        0      141 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/debug-object.md
+-rw-r--r--   0        0        0      154 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/debug-segfault.md
+-rw-r--r--   0        0        0      545 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/decr.md
+-rw-r--r--   0        0        0      499 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/decrby.md
+-rw-r--r--   0        0        0      207 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/del.md
+-rw-r--r--   0        0        0      258 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/discard.md
+-rw-r--r--   0        0        0     1003 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/dump.md
+-rw-r--r--   0        0        0       91 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/echo.md
+-rw-r--r--   0        0        0    37382 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/eval.md
+-rw-r--r--   0        0        0      648 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/eval_ro.md
+-rw-r--r--   0        0        0      182 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/evalsha.md
+-rw-r--r--   0        0        0      319 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/evalsha_ro.md
+-rw-r--r--   0        0        0      496 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/exec.md
+-rw-r--r--   0        0        0      969 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/exists.md
+-rw-r--r--   0        0        0     6733 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/expire.md
+-rw-r--r--   0        0        0      852 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/expireat.md
+-rw-r--r--   0        0        0      575 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/expiretime.md
+-rw-r--r--   0        0        0     4470 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/failover.md
+-rw-r--r--   0        0        0      914 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/flushall.md
+-rw-r--r--   0        0        0      695 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/flushdb.md
+-rw-r--r--   0        0        0     3315 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/geoadd.md
+-rw-r--r--   0        0        0     1257 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/geodecode.md
+-rw-r--r--   0        0        0     1019 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/geodist.md
+-rw-r--r--   0        0        0     2450 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/geoencode.md
+-rw-r--r--   0        0        0     1702 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/geohash.md
+-rw-r--r--   0        0        0     1083 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/geopos.md
+-rw-r--r--   0        0        0     4865 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/georadius.md
+-rw-r--r--   0        0        0      982 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/georadiusbymember.md
+-rw-r--r--   0        0        0     3474 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/geosearch.md
+-rw-r--r--   0        0        0      486 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/geosearchstore.md
+-rw-r--r--   0        0        0      349 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/get.md
+-rw-r--r--   0        0        0      488 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/getbit.md
+-rw-r--r--   0        0        0      387 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/getdel.md
+-rw-r--r--   0        0        0      816 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/getex.md
+-rw-r--r--   0        0        0      665 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/getrange.md
+-rw-r--r--   0        0        0      908 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/getset.md
+-rw-r--r--   0        0        0      666 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hdel.md
+-rw-r--r--   0        0        0     2974 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hello.md
+-rw-r--r--   0        0        0      307 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hexists.md
+-rw-r--r--   0        0        0      296 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hget.md
+-rw-r--r--   0        0        0      395 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hgetall.md
+-rw-r--r--   0        0        0      607 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hincrby.md
+-rw-r--r--   0        0        0     1214 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hincrbyfloat.md
+-rw-r--r--   0        0        0      239 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hkeys.md
+-rw-r--r--   0        0        0      247 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hlen.md
+-rw-r--r--   0        0        0      517 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hmget.md
+-rw-r--r--   0        0        0      441 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hmset.md
+-rw-r--r--   0        0        0     1872 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hrandfield.md
+-rw-r--r--   0        0        0       38 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hscan.md
+-rw-r--r--   0        0        0      390 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hset.md
+-rw-r--r--   0        0        0      487 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hsetnx.md
+-rw-r--r--   0        0        0      429 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hstrlen.md
+-rw-r--r--   0        0        0      234 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/hvals.md
+-rw-r--r--   0        0        0     5339 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/incr.md
+-rw-r--r--   0        0        0      499 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/incrby.md
+-rw-r--r--   0        0        0     1690 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/incrbyfloat.md
+-rw-r--r--   0        0        0    19420 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/info.md
+-rw-r--r--   0        0        0     1218 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/keys.md
+-rw-r--r--   0        0        0      296 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lastsave.md
+-rw-r--r--   0        0        0     1768 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/latency-doctor.md
+-rw-r--r--   0        0        0     1609 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/latency-graph.md
+-rw-r--r--   0        0        0      264 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/latency-help.md
+-rw-r--r--   0        0        0     1063 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/latency-history.md
+-rw-r--r--   0        0        0      917 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/latency-latest.md
+-rw-r--r--   0        0        0      880 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/latency-reset.md
+-rw-r--r--   0        0        0      586 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lindex.md
+-rw-r--r--   0        0        0      505 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/linsert.md
+-rw-r--r--   0        0        0      332 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/llen.md
+-rw-r--r--   0        0        0     3369 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lmove.md
+-rw-r--r--   0        0        0     1922 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lolwut.md
+-rw-r--r--   0        0        0      702 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lpop.md
+-rw-r--r--   0        0        0     3453 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lpos.md
+-rw-r--r--   0        0        0      945 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lpush.md
+-rw-r--r--   0        0        0      558 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lpushx.md
+-rw-r--r--   0        0        0     1287 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lrange.md
+-rw-r--r--   0        0        0      824 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lrem.md
+-rw-r--r--   0        0        0      330 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/lset.md
+-rw-r--r--   0        0        0     1460 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/ltrim.md
+-rw-r--r--   0        0        0      175 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/memory-doctor.md
+-rw-r--r--   0        0        0      156 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/memory-help.md
+-rw-r--r--   0        0        0      312 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/memory-malloc-stats.md
+-rw-r--r--   0        0        0      264 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/memory-purge.md
+-rw-r--r--   0        0        0     2607 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/memory-stats.md
+-rw-r--r--   0        0        0     1120 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/memory-usage.md
+-rw-r--r--   0        0        0      336 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/mget.md
+-rw-r--r--   0        0        0     3823 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/migrate.md
+-rw-r--r--   0        0        0      336 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/module-list.md
+-rw-r--r--   0        0        0      482 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/module-load.md
+-rw-r--r--   0        0        0      339 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/module-unload.md
+-rw-r--r--   0        0        0     2785 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/monitor.md
+-rw-r--r--   0        0        0      385 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/move.md
+-rw-r--r--   0        0        0      477 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/mset.md
+-rw-r--r--   0        0        0      745 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/msetnx.md
+-rw-r--r--   0        0        0      189 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/multi.md
+-rw-r--r--   0        0        0     3116 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/object.md
+-rw-r--r--   0        0        0      409 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/persist.md
+-rw-r--r--   0        0        0      305 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/pexpire.md
+-rw-r--r--   0        0        0      350 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/pexpireat.md
+-rw-r--r--   0        0        0      517 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/pexpiretime.md
+-rw-r--r--   0        0        0     1139 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/pfadd.md
+-rw-r--r--   0        0        0     4364 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/pfcount.md
+-rw-r--r--   0        0        0      637 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/pfmerge.md
+-rw-r--r--   0        0        0      513 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/ping.md
+-rw-r--r--   0        0        0      201 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/psetex.md
+-rw-r--r--   0        0        0      315 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/psubscribe.md
+-rw-r--r--   0        0        0      391 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/psync.md
+-rw-r--r--   0        0        0      730 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/pttl.md
+-rw-r--r--   0        0        0      450 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/publish.md
+-rw-r--r--   0        0        0     1872 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/pubsub.md
+-rw-r--r--   0        0        0      275 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/punsubscribe.md
+-rw-r--r--   0        0        0      172 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/quit.md
+-rw-r--r--   0        0        0      141 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/randomkey.md
+-rw-r--r--   0        0        0      882 2021-07-15 10:17:12.619495 iredis-1.9.4/iredis/data/commands/readonly.md
+-rw-r--r--   0        0        0      355 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/readwrite.md
+-rw-r--r--   0        0        0      722 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/rename.md
+-rw-r--r--   0        0        0      615 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/renamenx.md
+-rw-r--r--   0        0        0      972 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/replicaof.md
+-rw-r--r--   0        0        0      866 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/reset.md
+-rw-r--r--   0        0        0     1205 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/restore.md
+-rw-r--r--   0        0        0     3074 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/role.md
+-rw-r--r--   0        0        0      694 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/rpop.md
+-rw-r--r--   0        0        0     3141 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/rpoplpush.md
+-rw-r--r--   0        0        0      943 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/rpush.md
+-rw-r--r--   0        0        0      558 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/rpushx.md
+-rw-r--r--   0        0        0      639 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sadd.md
+-rw-r--r--   0        0        0      710 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/save.md
+-rw-r--r--   0        0        0    13713 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/scan.md
+-rw-r--r--   0        0        0      257 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/scard.md
+-rw-r--r--   0        0        0     1274 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/script-debug.md
+-rw-r--r--   0        0        0      823 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/script-exists.md
+-rw-r--r--   0        0        0      699 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/script-flush.md
+-rw-r--r--   0        0        0      795 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/script-kill.md
+-rw-r--r--   0        0        0      657 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/script-load.md
+-rw-r--r--   0        0        0      451 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sdiff.md
+-rw-r--r--   0        0        0      378 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sdiffstore.md
+-rw-r--r--   0        0        0     1294 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/select.md
+-rw-r--r--   0        0        0     3270 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/set.md
+-rw-r--r--   0        0        0     5269 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/setbit.md
+-rw-r--r--   0        0        0      607 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/setex.md
+-rw-r--r--   0        0        0     4310 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/setnx.md
+-rw-r--r--   0        0        0     1692 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/setrange.md
+-rw-r--r--   0        0        0     3044 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/shutdown.md
+-rw-r--r--   0        0        0      573 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sinter.md
+-rw-r--r--   0        0        0      380 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sinterstore.md
+-rw-r--r--   0        0        0      307 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sismember.md
+-rw-r--r--   0        0        0     1297 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/slaveof.md
+-rw-r--r--   0        0        0     3438 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/slowlog.md
+-rw-r--r--   0        0        0      254 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/smembers.md
+-rw-r--r--   0        0        0      435 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/smismember.md
+-rw-r--r--   0        0        0      901 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/smove.md
+-rw-r--r--   0        0        0     4723 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sort.md
+-rw-r--r--   0        0        0     1139 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/spop.md
+-rw-r--r--   0        0        0     2568 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/srandmember.md
+-rw-r--r--   0        0        0      649 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/srem.md
+-rw-r--r--   0        0        0       38 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sscan.md
+-rw-r--r--   0        0        0     3801 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/stralgo.md
+-rw-r--r--   0        0        0      288 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/strlen.md
+-rw-r--r--   0        0        0      330 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/subscribe.md
+-rw-r--r--   0        0        0      426 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sunion.md
+-rw-r--r--   0        0        0      380 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sunionstore.md
+-rw-r--r--   0        0        0      529 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/swapdb.md
+-rw-r--r--   0        0        0      450 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/sync.md
+-rw-r--r--   0        0        0      403 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/time.md
+-rw-r--r--   0        0        0      217 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/touch.md
+-rw-r--r--   0        0        0      837 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/ttl.md
+-rw-r--r--   0        0        0      367 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/type.md
+-rw-r--r--   0        0        0      542 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/unlink.md
+-rw-r--r--   0        0        0      275 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/unsubscribe.md
+-rw-r--r--   0        0        0      216 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/unwatch.md
+-rw-r--r--   0        0        0     3265 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/wait.md
+-rw-r--r--   0        0        0      158 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/watch.md
+-rw-r--r--   0        0        0     1268 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xack.md
+-rw-r--r--   0        0        0     4029 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xadd.md
+-rw-r--r--   0        0        0     3384 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xautoclaim.md
+-rw-r--r--   0        0        0     4304 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xclaim.md
+-rw-r--r--   0        0        0     1869 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xdel.md
+-rw-r--r--   0        0        0     3364 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xgroup.md
+-rw-r--r--   0        0        0     5161 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xinfo.md
+-rw-r--r--   0        0        0      637 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xlen.md
+-rw-r--r--   0        0        0     5567 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xpending.md
+-rw-r--r--   0        0        0     7510 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xrange.md
+-rw-r--r--   0        0        0     8068 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xread.md
+-rw-r--r--   0        0        0     6975 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xreadgroup.md
+-rw-r--r--   0        0        0     1294 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xrevrange.md
+-rw-r--r--   0        0        0     2467 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/xtrim.md
+-rw-r--r--   0        0        0     4961 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zadd.md
+-rw-r--r--   0        0        0      281 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zcard.md
+-rw-r--r--   0        0        0      604 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zcount.md
+-rw-r--r--   0        0        0      418 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zdiff.md
+-rw-r--r--   0        0        0      558 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zdiffstore.md
+-rw-r--r--   0        0        0      816 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zincrby.md
+-rw-r--r--   0        0        0      499 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zinter.md
+-rw-r--r--   0        0        0      977 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zinterstore.md
+-rw-r--r--   0        0        0      721 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zlexcount.md
+-rw-r--r--   0        0        0      442 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zmscore.md
+-rw-r--r--   0        0        0      552 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zpopmax.md
+-rw-r--r--   0        0        0      552 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zpopmin.md
+-rw-r--r--   0        0        0     1949 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrandmember.md
+-rw-r--r--   0        0        0     6225 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrange.md
+-rw-r--r--   0        0        0     3269 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrangebylex.md
+-rw-r--r--   0        0        0     3389 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrangebyscore.md
+-rw-r--r--   0        0        0      287 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrangestore.md
+-rw-r--r--   0        0        0      605 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrank.md
+-rw-r--r--   0        0        0      575 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrem.md
+-rw-r--r--   0        0        0      701 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zremrangebylex.md
+-rw-r--r--   0        0        0      623 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zremrangebyrank.md
+-rw-r--r--   0        0        0      407 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zremrangebyscore.md
+-rw-r--r--   0        0        0      683 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrevrange.md
+-rw-r--r--   0        0        0      669 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrevrangebylex.md
+-rw-r--r--   0        0        0      911 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrevrangebyscore.md
+-rw-r--r--   0        0        0      607 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zrevrank.md
+-rw-r--r--   0        0        0       38 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zscan.md
+-rw-r--r--   0        0        0      331 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zscore.md
+-rw-r--r--   0        0        0      492 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zunion.md
+-rw-r--r--   0        0        0     1379 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/commands/zunionstore.md
+-rw-r--r--   0        0        0   129652 2021-07-15 10:17:12.615496 iredis-1.9.4/iredis/data/commands.json
+-rw-r--r--   0        0        0      694 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/dangerous_commands.csv
+-rw-r--r--   0        0        0     2079 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/data/iredisrc
+-rw-r--r--   0        0        0    13644 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/entry.py
+-rw-r--r--   0        0        0      420 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/exceptions.py
+-rw-r--r--   0        0        0      642 2021-07-15 10:17:12.623496 iredis-1.9.4/iredis/key_bindings.py
+-rw-r--r--   0        0        0     3955 2021-07-15 10:17:12.627496 iredis-1.9.4/iredis/lexer.py
+-rw-r--r--   0        0        0     1932 2021-07-15 10:17:12.627496 iredis-1.9.4/iredis/markdown.py
+-rw-r--r--   0        0        0     2310 2021-07-15 10:17:12.627496 iredis-1.9.4/iredis/processors.py
+-rw-r--r--   0        0        0    25169 2021-07-15 10:17:12.627496 iredis-1.9.4/iredis/redis_grammar.py
+-rw-r--r--   0        0        0    13890 2021-07-15 10:17:12.627496 iredis-1.9.4/iredis/renders.py
+-rw-r--r--   0        0        0     2890 2021-07-15 10:17:12.627496 iredis-1.9.4/iredis/style.py
+-rw-r--r--   0        0        0     9569 2021-07-15 10:17:12.627496 iredis-1.9.4/iredis/utils.py
+-rw-r--r--   0        0        0     1621 2021-07-15 10:17:12.627496 iredis-1.9.4/iredis/warning.py
+-rw-r--r--   0        0        0     1518 2021-07-15 10:17:12.627496 iredis-1.9.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/__init__.py
+-rw-r--r--   0        0        0      787 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_cli_pubsub.py
+-rw-r--r--   0        0        0     2470 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_cli_start.py
+-rw-r--r--   0        0        0     1791 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_command_input.py
+-rw-r--r--   0        0        0     1219 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_completer.py
+-rw-r--r--   0        0        0      590 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_config.py
+-rw-r--r--   0        0        0     1523 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_dsn.py
+-rw-r--r--   0        0        0     1085 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_history.py
+-rw-r--r--   0        0        0      472 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_on_error.py
+-rw-r--r--   0        0        0     3383 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_pager.py
+-rw-r--r--   0        0        0      240 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_self_implemented_command.py
+-rw-r--r--   0        0        0      571 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_shell_pipeline.py
+-rw-r--r--   0        0        0      898 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_string_execute.py
+-rw-r--r--   0        0        0     1769 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_transaction.py
+-rw-r--r--   0        0        0     1343 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/test_warning.py
+-rw-r--r--   0        0        0      248 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/cli_tests/wrappager.py
+-rw-r--r--   0        0        0     3372 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/conftest.py
+-rw-r--r--   0        0        0      337 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/helpers.py
+-rw-r--r--   0        0        0        0 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/__init__.py
+-rw-r--r--   0        0        0     1737 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_base_token.py
+-rw-r--r--   0        0        0     8517 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_cluster.py
+-rw-r--r--   0        0        0     2982 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_connection.py
+-rw-r--r--   0        0        0     5805 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_generic_parse.py
+-rw-r--r--   0        0        0     1011 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_geo.py
+-rw-r--r--   0        0        0     1294 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_hash_parse.py
+-rw-r--r--   0        0        0      163 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_hll_parse.py
+-rw-r--r--   0        0        0     2897 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_list_parse.py
+-rw-r--r--   0        0        0      428 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_pubsub.py
+-rw-r--r--   0        0        0      801 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_script.py
+-rw-r--r--   0        0        0     6513 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_server.py
+-rw-r--r--   0        0        0     1258 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_set_parse.py
+-rw-r--r--   0        0        0     4681 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_sorted_set_parse.py
+-rw-r--r--   0        0        0    12661 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_stream.py
+-rw-r--r--   0        0        0     9962 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/command_parse/test_string_parse.py
+-rw-r--r--   0        0        0    16325 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/test_client.py
+-rw-r--r--   0        0        0    11472 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/test_completers.py
+-rw-r--r--   0        0        0     7134 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/test_entry.py
+-rw-r--r--   0        0        0      763 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/test_markdown_doc_render.py
+-rw-r--r--   0        0        0    15039 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/test_render_functions.py
+-rw-r--r--   0        0        0     4064 2021-07-15 10:17:12.627496 iredis-1.9.4/tests/unittests/test_utils.py
+-rw-r--r--   0        0        0    10002 2021-07-15 10:17:36.077772 iredis-1.9.4/setup.py
+-rw-r--r--   0        0        0    10075 2021-07-15 10:17:36.078728 iredis-1.9.4/PKG-INFO
```

### Comparing `iredis-1.9.3/LICENSE` & `iredis-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/README.md` & `iredis-1.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </p>
 
 <h3 align="center">Interactive Redis: A Cli for Redis with AutoCompletion and Syntax Highlighting.</h3>
 
 <p align="center">
 <a href="https://github.com/laixintao/iredis/actions"><img src="https://github.com/laixintao/iredis/workflows/Test/badge.svg" alt="Github Action"></a>
 <a href="https://badge.fury.io/py/iredis"><img src="https://badge.fury.io/py/iredis.svg" alt="PyPI version"></a>
-<img src="https://badgen.net/badge/python/3.6%20|%203.7%20|%203.8/" alt="Python version">
+<img src="https://badgen.net/badge/python/3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9/" alt="Python version">
 <a href="https://pepy.tech/project/iredis"><img src="https://pepy.tech/badge/iredis" alt="Download stats"></a>
 <a href="https://t.me/iredis_users"><img src="https://badgen.net/badge/icon/join?icon=telegram&amp;label=usergroup" alt="Chat on telegram"></a>
 <a href="https://console.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/laixintao/iredis&amp;cloudshell_print=docs/cloudshell/run-in-docker.txt"><img src="https://badgen.net/badge/run/GoogleCloudShell/blue?icon=terminal" alt="Open in Cloud Shell"></a>
 </p>
 
 <p align="center">
   <img src="./docs/assets/demo.svg" alt="demo">
@@ -152,16 +152,16 @@
 - <kbd>Ctrl</kbd> + <kbd>X</kbd> <kbd>Ctrl</kbd> + <kbd>E</kbd> to open an
   editor to edit command, or <kbd>V</kbd> in vi-mode.
 
 ## Development
 
 ### Release Strategy
 
-IRedis is built and released by `GitHub Actions`. Whenever a tag is pushed to the
-`master` branch, a new release is built and uploaded to pypi.org, it's very
+IRedis is built and released by `GitHub Actions`. Whenever a tag is pushed to
+the `master` branch, a new release is built and uploaded to pypi.org, it's very
 convenient.
 
 Thus, we release as often as possible, so that users can always enjoy the new
 features and bugfixes quickly. Any bugfix or new feature will get at least a
 patch release, whereas big features will get a minor release.
 
 ### Setup Environment
```

### Comparing `iredis-1.9.3/iredis/bottom.py` & `iredis-1.9.4/iredis/bottom.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/client.py` & `iredis-1.9.4/iredis/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,25 +68,17 @@
         self.port = port
         self.db = db
         self.path = path
         # FIXME username is not using...
         self.username = username
         self.client_name = client_name
         self.scheme = scheme
+        self.password = password
 
-        self.connection = self.create_connection(
-            host,
-            port,
-            db,
-            password,
-            path,
-            scheme,
-            username,
-            client_name=client_name,
-        )
+        self.build_connection()
 
         # all command upper case
         self.answer_callbacks = command2callback
         self.set_default_pager(config)
         try:
             self.connection.connect()
         except Exception as e:
@@ -100,14 +92,29 @@
                 config.no_version_reason = str(e)
         else:
             config.no_version_reason = "--no-info flag activated"
 
         if config.version and re.match(r"([\d\.]+)", config.version):
             self.auth_compat(config.version)
 
+    def build_connection(self):
+        """
+        create a new connection and replace ``self.connection``
+        """
+        self.connection = self.create_connection(
+            self.host,
+            self.port,
+            self.db,
+            self.password,
+            self.path,
+            self.scheme,
+            self.username,
+            client_name=self.client_name,
+        )
+
     def create_connection(
         self,
         host=None,
         port=None,
         db=0,
         password=None,
         path=None,
@@ -248,14 +255,23 @@
                         response_message, command_name, *args, **options
                     )
                 raise e
 
             except redis.exceptions.ExecAbortError:
                 config.transaction = False
                 raise
+            except KeyboardInterrupt:
+                logger.warning("received KeyboardInterrupt... rebuild connection...")
+                connection.disconnect()
+                connection.connect()
+                print(
+                    "KeyboardInterrupt received! User canceled reading response!",
+                    file=sys.stderr,
+                )
+                return None
             else:
                 return response
         raise last_error
 
     def reissue_with_redirect(self, response, *args, **kwargs):
         """
         For redis cluster, when server response a "MOVE ..." response, we auto-
```

### Comparing `iredis-1.9.3/iredis/commands.py` & `iredis-1.9.4/iredis/commands.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/completers.py` & `iredis-1.9.4/iredis/completers.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/config.py` & `iredis-1.9.4/iredis/config.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/command_syntax.csv` & `iredis-1.9.4/iredis/data/command_syntax.csv`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 scripting,SCRIPT FLUSH,command,render_simple_string
 scripting,SCRIPT KILL,command,render_simple_string
 scripting,SCRIPT LOAD,command_lua_any,render_bulk_string_decode
 server,ACL CAT,command_categorynamex,render_list
 server,ACL DELUSER,command_usernames,render_int
 server,ACL GENPASS,command_countx,render_bulk_string
 server,ACL GETUSER,command_username,render_list
-server,ACL HELP,command,render_list
+server,ACL HELP,command,render_help
 server,ACL LIST,command,render_list
 server,ACL LOAD,command,render_simple_string
 server,ACL LOG,command_count_or_resetx,render_list_or_string
 server,ACL SAVE,command,render_simple_string
 server,ACL SETUSER,command_username_rules,render_simple_string
 server,ACL USERS,command,render_list
 server,ACL WHOAMI,command,render_bulk_string
@@ -148,20 +148,20 @@
 server,FLUSHALL,command_asyncx,render_simple_string
 server,FLUSHDB,command_asyncx,render_simple_string
 server,INFO,command_sectionx,render_bulk_string_decode
 server,LOLWUT,command_version,render_bytes
 server,LASTSAVE,command,render_unixtime
 server,LATENCY DOCTOR,command,render_bulk_string_decode
 server,LATENCY GRAPH,command_graphevent,render_bulk_string_decode
-server,LATENCY HELP,command,render_list
+server,LATENCY HELP,command,render_help
 server,LATENCY HISTORY,command_graphevent,render_list
 server,LATENCY LATEST,command,render_list
 server,LATENCY RESET,command_graphevents,render_int
 server,MEMORY DOCTOR,command,render_bulk_string_decode
-server,MEMORY HELP,command,render_list
+server,MEMORY HELP,command,render_help
 server,MEMORY MALLOC-STATS,command,render_bulk_string_decode
 server,MEMORY PURGE,command,render_simple_string
 server,MEMORY STATS,command,render_nested_pair
 server,MEMORY USAGE,command_key_samples_count,render_int
 server,MODULE LIST,command,render_list
 server,MODULE LOAD,command_any,render_simple_string
 server,MODULE UNLOAD,command_any,render_simple_string
```

### Comparing `iredis-1.9.3/iredis/data/commands/acl-cat.md` & `iredis-1.9.4/iredis/data/commands/acl-cat.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/acl-deluser.md` & `iredis-1.9.4/iredis/data/commands/acl-deluser.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/acl-genpass.md` & `iredis-1.9.4/iredis/data/commands/acl-genpass.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/acl-getuser.md` & `iredis-1.9.4/iredis/data/commands/acl-getuser.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 patterns. Note that command rules are returned as a string in the same format
 used with the `ACL SETUSER` command. This description of command rules reflects
 the user's effective permissions, so while it may not be identical to the set of
 rules used to configure the user, it is still functionally identical.
 
 @array-reply: a list of ACL rule definitions for the user.
 
+@history
+
+- `>= 6.2`: Added Pub/Sub channel patterns.
+
 @examples
 
 Here's the default configuration for the default user:
 
 ```
 > ACL GETUSER default
 1) "flags"
@@ -21,8 +25,10 @@
    4) "nopass"
 3) "passwords"
 4) (empty array)
 5) "commands"
 6) "+@all"
 7) "keys"
 8) 1) "*"
+9) "channels"
+10) 1) "*"
 ```
```

### Comparing `iredis-1.9.3/iredis/data/commands/acl-list.md` & `iredis-1.9.4/iredis/data/commands/acl-list.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 
 An array of strings.
 
 @examples
 
 ```
 > ACL LIST
-1) "user antirez on #9f86d081884c7d659a2feaa0c55ad015a3bf4f1b2b0b822cd15d6c15b0f00a08 ~objects:* +@all -@admin -@dangerous"
-2) "user default on nopass ~* +@all"
+1) "user antirez on #9f86d081884c7d659a2feaa0c55ad015a3bf4f1b2b0b822cd15d6c15b0f00a08 ~objects:* &* +@all -@admin -@dangerous"
+2) "user default on nopass ~* &* +@all"
 ```
```

### Comparing `iredis-1.9.3/iredis/data/commands/acl-load.md` & `iredis-1.9.4/iredis/data/commands/acl-load.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/acl-log.md` & `iredis-1.9.4/iredis/data/commands/acl-log.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/acl-save.md` & `iredis-1.9.4/iredis/data/commands/acl-save.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/acl-setuser.md` & `iredis-1.9.4/iredis/data/commands/acl-setuser.md`

 * *Files 5% similar despite different names*

```diff
@@ -51,18 +51,25 @@
   connections already authenticated with such a user, the connections will
   continue to work as expected. To also kill the old connections you can use
   `CLIENT KILL` with the user option. An alternative is to delete the user with
   `ACL DELUSER`, that will result in all the connections authenticated as the
   deleted user to be disconnected.
 - `~<pattern>`: add the specified key pattern (glob style pattern, like in the
   `KEYS` command), to the list of key patterns accessible by the user. You can
-  add as many key patterns you want to the same user. Example: `~objects:*`
+  add multiple key patterns to the same user. Example: `~objects:*`
 - `allkeys`: alias for `~*`, it allows the user to access all the keys.
-- `resetkey`: removes all the key patterns from the list of key patterns the
+- `resetkeys`: removes all the key patterns from the list of key patterns the
   user can access.
+- `&<pattern>`: add the specified glob style pattern to the list of Pub/Sub
+  channel patterns accessible by the user. You can add multiple channel patterns
+  to the same user. Example: `&chatroom:*`
+- `allchannels`: alias for `&*`, it allows the user to access all Pub/Sub
+  channels.
+- `resetchannels`: removes all channel patterns from the list of Pub/Sub channel
+  patterns the user can access.
 - `+<command>`: add this command to the list of the commands the user can call.
   Example: `+zadd`.
 - `+@<category>`: add all the commands in the specified category to the list of
   commands the user is able to execute. Example: `+@string` (adds all the string
   commands). For a list of categories check the `ACL CAT` command.
 - `+<command>|<subcommand>`: add the specified command to the list of the
   commands the user can execute, but only for the specified subcommand. Example:
@@ -83,15 +90,15 @@
 - `nopass`: the user is set as a "no password" user. It means that it will be
   possible to authenticate as such user with any password. By default, the
   `default` special user is set as "nopass". The `nopass` rule will also reset
   all the configured passwords for the user.
 - `>password`: Add the specified clear text password as an hashed password in
   the list of the users passwords. Every user can have many active passwords, so
   that password rotation will be simpler. The specified password is not stored
-  in cleartext inside the server. Example: `>mypassword`.
+  as clear text inside the server. Example: `>mypassword`.
 - `#<hashedpassword>`: Add the specified hashed password to the list of user
   passwords. A Redis hashed password is hashed with SHA256 and translated into a
   hexadecimal string. Example:
   `#c3ab8ff13720e8ad9047dd39466b3c8974e592c2fa383d4a3960714caef0c4f2`.
 - `<password`: Like `>password` but removes the password instead of adding it.
 - `!<hashedpassword>`: Like `#<hashedpassword>` but removes the password instead
   of adding it.
@@ -100,14 +107,18 @@
 
 @return
 
 @simple-string-reply: `OK` on success.
 
 If the rules contain errors, the error is returned.
 
+@history
+
+- `>= 6.2`: Added Pub/Sub channel patterns.
+
 @examples
 
 ```
 > ACL SETUSER alan allkeys +@string +@set -SADD >alanpassword
 +OK
 
 > ACL SETUSER antirez heeyyyy
```

### Comparing `iredis-1.9.3/iredis/data/commands/append.md` & `iredis-1.9.4/iredis/data/commands/append.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/auth.md` & `iredis-1.9.4/iredis/data/commands/auth.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 In order to authenticate the current connection with one of the connections
 defined in the ACL list (see `ACL SETUSER`) and the official
 [ACL guide](/topics/acl) for more information.
 
 When ACLs are used, the single argument form of the command, where only the
 password is specified, assumes that the implicit username is "default".
 
+@history
+
+- `>= 6.0.0`: Added ACL style (username and password).
+
 ## Security notice
 
 Because of the high performance nature of Redis, it is possible to try a lot of
 passwords in parallel in very short time, so make sure to generate a strong and
 very long password so that this attack is infeasible. A good way to generate
 strong passwords is via the `ACL GENPASS` command.
```

### Comparing `iredis-1.9.3/iredis/data/commands/bgrewriteaof.md` & `iredis-1.9.4/iredis/data/commands/bgrewriteaof.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/bgsave.md` & `iredis-1.9.4/iredis/data/commands/bgsave.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/bitcount.md` & `iredis-1.9.4/iredis/data/commands/bitcount.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/bitfield.md` & `iredis-1.9.4/iredis/data/commands/bitfield.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,34 +16,34 @@
 
     > BITFIELD mykey INCRBY i5 100 1 GET u4 0
     1) (integer) 1
     2) (integer) 0
 
 Note that:
 
-1. Addressing with `GET` bits outside the current string length (including the
+1. Addressing with `!GET` bits outside the current string length (including the
    case the key does not exist at all), results in the operation to be performed
    like the missing part all consists of bits set to 0.
-2. Addressing with `SET` or `INCRBY` bits outside the current string length will
-   enlarge the string, zero-padding it, as needed, for the minimal length
+2. Addressing with `!SET` or `!INCRBY` bits outside the current string length
+   will enlarge the string, zero-padding it, as needed, for the minimal length
    needed, according to the most far bit touched.
 
 ## Supported subcommands and integer types
 
 The following is the list of supported commands.
 
 - **GET** `<type>` `<offset>` -- Returns the specified bit field.
 - **SET** `<type>` `<offset>` `<value>` -- Set the specified bit field and
   returns its old value.
 - **INCRBY** `<type>` `<offset>` `<increment>` -- Increments or decrements (if a
   negative increment is given) the specified bit field and returns the new
   value.
 
 There is another subcommand that only changes the behavior of successive
-`INCRBY` subcommand calls by setting the overflow behavior:
+`!INCRBY` and `!SET` subcommands calls by setting the overflow behavior:
 
 - **OVERFLOW** `[WRAP|SAT|FAIL]`
 
 Where an integer type is expected, it can be composed by prefixing with `i` for
 signed integers and `u` for unsigned integers with the number of bits of our
 integer type. So for example `u8` is an unsigned integer of 8 bits and `i16` is
 a signed integer of 16 bits.
@@ -87,16 +87,17 @@
   increment of 10, will result into the value 127, and further increments will
   always keep the value at 127. The same happens on underflows, but towards the
   value is blocked at the most negative value.
 - **FAIL**: in this mode no operation is performed on overflows or underflows
   detected. The corresponding return value is set to NULL to signal the
   condition to the caller.
 
-Note that each `OVERFLOW` statement only affects the `INCRBY` commands that
-follow it in the list of subcommands, up to the next `OVERFLOW` statement.
+Note that each `OVERFLOW` statement only affects the `!INCRBY` and `!SET`
+commands that follow it in the list of subcommands, up to the next `OVERFLOW`
+statement.
 
 By default, **WRAP** is used if not otherwise specified.
 
     > BITFIELD mykey incrby u2 100 1 OVERFLOW SAT incrby u2 102 1
     1) (integer) 1
     2) (integer) 1
     > BITFIELD mykey incrby u2 100 1 OVERFLOW SAT incrby u2 102 1
```

### Comparing `iredis-1.9.3/iredis/data/commands/bitop.md` & `iredis-1.9.4/iredis/data/commands/bitop.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/bitpos.md` & `iredis-1.9.4/iredis/data/commands/bitpos.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/blpop.md` & `iredis-1.9.4/iredis/data/commands/blpop.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 of the key unblocking it and the popped value.
 
 When `BLPOP` causes a client to block and a non-zero timeout is specified, the
 client will unblock returning a `nil` multi-bulk value when the specified
 timeout has expired without a push operation against at least one of the
 specified keys.
 
-**The timeout argument is interpreted as an integer value specifying the maximum
+**The timeout argument is interpreted as a double value specifying the maximum
 number of seconds to block**. A timeout of zero can be used to block
 indefinitely.
 
 ## What key is served first? What client? What element? Priority ordering details.
 
 - If the client tries to blocks for multiple keys, but at least one key contains
   elements, the returned key / element pair is the first key from left to right
@@ -125,14 +125,18 @@
 @array-reply: specifically:
 
 - A `nil` multi-bulk when no element could be popped and the timeout expired.
 - A two-element multi-bulk with the first element being the name of the key
   where an element was popped and the second element being the value of the
   popped element.
 
+@history
+
+- `>= 6.0`: `timeout` is interpreted as a double instead of an integer.
+
 @examples
 
 ```
 redis> DEL list1 list2
 (integer) 0
 redis> RPUSH list1 a b c
 (integer) 3
```

### Comparing `iredis-1.9.3/iredis/data/commands/brpop.md` & `iredis-1.9.4/iredis/data/commands/brpop.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 @array-reply: specifically:
 
 - A `nil` multi-bulk when no element could be popped and the timeout expired.
 - A two-element multi-bulk with the first element being the name of the key
   where an element was popped and the second element being the value of the
   popped element.
 
+@history
+
+- `>= 6.0`: `timeout` is interpreted as a double instead of an integer.
+
 @examples
 
 ```
 redis> DEL list1 list2
 (integer) 0
 redis> RPUSH list1 a b c
 (integer) 3
```

### Comparing `iredis-1.9.3/iredis/data/commands/brpoplpush.md` & `iredis-1.9.4/iredis/data/commands/brpoplpush.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 `BRPOPLPUSH` is the blocking variant of `RPOPLPUSH`. When `source` contains
 elements, this command behaves exactly like `RPOPLPUSH`. When used inside a
 `MULTI`/`EXEC` block, this command behaves exactly like `RPOPLPUSH`. When
 `source` is empty, Redis will block the connection until another client pushes
 to it or until `timeout` is reached. A `timeout` of zero can be used to block
 indefinitely.
 
+As per Redis 6.2.0, BRPOPLPUSH is considered deprecated. Please prefer `BLMOVE`
+in new code.
+
 See `RPOPLPUSH` for more information.
 
 @return
 
 @bulk-string-reply: the element being popped from `source` and pushed to
 `destination`. If `timeout` is reached, a @nil-reply is returned.
 
+@history
+
+- `>= 6.0`: `timeout` is interpreted as a double instead of an integer.
+
 ## Pattern: Reliable queue
 
 Please see the pattern description in the `RPOPLPUSH` documentation.
 
 ## Pattern: Circular list
 
 Please see the pattern description in the `RPOPLPUSH` documentation.
```

### Comparing `iredis-1.9.3/iredis/data/commands/bzpopmax.md` & `iredis-1.9.4/iredis/data/commands/bzpopmax.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 `BZPOPMAX` is the blocking variant of the sorted set `ZPOPMAX` primitive.
 
 It is the blocking version because it blocks the connection when there are no
 members to pop from any of the given sorted sets. A member with the highest
 score is popped from first sorted set that is non-empty, with the given keys
 being checked in the order that they are given.
 
-The `timeout` argument is interpreted as an integer value specifying the maximum
+The `timeout` argument is interpreted as a double value specifying the maximum
 number of seconds to block. A timeout of zero can be used to block indefinitely.
 
 See the [BZPOPMIN documentation][cb] for the exact semantics, since `BZPOPMAX`
 is identical to `BZPOPMIN` with the only difference being that it pops members
 with the highest scores instead of popping the ones with the lowest scores.
 
 [cb]: /commands/bzpopmin
@@ -19,14 +19,18 @@
 @array-reply: specifically:
 
 - A `nil` multi-bulk when no element could be popped and the timeout expired.
 - A three-element multi-bulk with the first element being the name of the key
   where a member was popped, the second element is the popped member itself, and
   the third element is the score of the popped element.
 
+@history
+
+- `>= 6.0`: `timeout` is interpreted as a double instead of an integer.
+
 @examples
 
 ```
 redis> DEL zset1 zset2
 (integer) 0
 redis> ZADD zset1 0 a 1 b 2 c
 (integer) 3
```

### Comparing `iredis-1.9.3/iredis/data/commands/bzpopmin.md` & `iredis-1.9.4/iredis/data/commands/bzpopmin.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 `BZPOPMIN` is the blocking variant of the sorted set `ZPOPMIN` primitive.
 
 It is the blocking version because it blocks the connection when there are no
 members to pop from any of the given sorted sets. A member with the lowest score
 is popped from first sorted set that is non-empty, with the given keys being
 checked in the order that they are given.
 
-The `timeout` argument is interpreted as an integer value specifying the maximum
+The `timeout` argument is interpreted as an double value specifying the maximum
 number of seconds to block. A timeout of zero can be used to block indefinitely.
 
 See the [BLPOP documentation][cl] for the exact semantics, since `BZPOPMIN` is
 identical to `BLPOP` with the only difference being the data structure being
 popped from.
 
 [cl]: /commands/blpop
@@ -19,14 +19,18 @@
 @array-reply: specifically:
 
 - A `nil` multi-bulk when no element could be popped and the timeout expired.
 - A three-element multi-bulk with the first element being the name of the key
   where a member was popped, the second element is the popped member itself, and
   the third element is the score of the popped element.
 
+@history
+
+- `>= 6.0`: `timeout` is interpreted as a double instead of an integer.
+
 @examples
 
 ```
 redis> DEL zset1 zset2
 (integer) 0
 redis> ZADD zset1 0 a 1 b 2 c
 (integer) 3
```

### Comparing `iredis-1.9.3/iredis/data/commands/client-caching.md` & `iredis-1.9.4/iredis/data/commands/client-caching.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 This command controls the tracking of the keys in the next command executed by
 the connection, when tracking is enabled in `OPTIN` or `OPTOUT` mode. Please
 check the [client side caching documentation](/topics/client-side-caching) for
-background informations.
+background information.
 
 When tracking is enabled Redis, using the `CLIENT TRACKING` command, it is
 possible to specify the `OPTIN` or `OPTOUT` options, so that keys in read only
 commands are not automatically remembered by the server to be invalidated later.
 When we are in `OPTIN` mode, we can enable the tracking of the keys in the next
 command by calling `CLIENT CACHING yes` immediately before it. Similarly when we
 are in `OPTOUT` mode, and keys are normally tracked, we can avoid the keys in
```

### Comparing `iredis-1.9.3/iredis/data/commands/client-getredir.md` & `iredis-1.9.4/iredis/data/commands/client-getredir.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/client-id.md` & `iredis-1.9.4/iredis/data/commands/client-id.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/client-kill.md` & `iredis-1.9.4/iredis/data/commands/client-kill.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-The `CLIENT KILL` command closes a given client connection. Up to Redis 2.8.11
-it was possible to close a connection only by client address, using the
-following form:
+The `CLIENT KILL` command closes a given client connection. This command support
+two formats, the old format:
 
     CLIENT KILL addr:port
 
 The `ip:port` should match a line returned by the `CLIENT LIST` command (`addr`
 field).
 
-However starting with Redis 2.8.12 or greater, the command accepts the following
-form:
+The new format:
 
     CLIENT KILL <filter> <value> ... ... <filter> <value>
 
 With the new form it is possible to kill clients by different attributes instead
 of killing just by address. The following filters are available:
 
 - `CLIENT KILL ADDR ip:port`. This is exactly the same as the old
   three-arguments behavior.
-- `CLIENT KILL ID client-id`. Allows to kill a client by its unique `ID` field,
-  which was introduced in the `CLIENT LIST` command starting from Redis 2.8.12.
-- `CLIENT KILL TYPE type`, where _type_ is one of `normal`, `master`, `slave`
-  and `pubsub` (the `master` type is available from v3.2). This closes the
-  connections of **all the clients** in the specified class. Note that clients
-  blocked into the `MONITOR` command are considered to belong to the `normal`
-  class.
+- `CLIENT KILL LADDR ip:port`. Kill all clients connected to specified local
+  (bind) address.
+- `CLIENT KILL ID client-id`. Allows to kill a client by its unique `ID` field.
+  Client `ID`'s are retrieved using the `CLIENT LIST` command.
+- `CLIENT KILL TYPE type`, where _type_ is one of `normal`, `master`, `replica`
+  and `pubsub`. This closes the connections of **all the clients** in the
+  specified class. Note that clients blocked into the `MONITOR` command are
+  considered to belong to the `normal` class.
 - `CLIENT KILL USER username`. Closes all the connections that are authenticated
   with the specified [ACL](/topics/acl) username, however it returns an error if
   the username does not map to an existing ACL user.
 - `CLIENT KILL SKIPME yes/no`. By default this option is set to `yes`, that is,
   the client calling the command will not get killed, however setting this
   option to `no` will have the effect of also killing the client calling the
   command.
 
-**Note: starting with Redis 5 the project is no longer using the slave word. You
-can use `TYPE replica` instead, however the old form is still supported for
-backward compatibility.**
-
 It is possible to provide multiple filters at the same time. The command will
 handle multiple filters via logical AND. For example:
 
     CLIENT KILL addr 127.0.0.1:12345 type pubsub
 
 is valid and will kill only a pubsub client with the specified address. This
 format containing multiple filters is rarely useful currently.
@@ -67,7 +62,16 @@
 When called with the three arguments format:
 
 @simple-string-reply: `OK` if the connection exists and has been closed
 
 When called with the filter / value format:
 
 @integer-reply: the number of clients killed.
+
+@history
+
+- `>= 2.8.12`: Added new filter format.
+- `>= 2.8.12`: `ID` option.
+- `>= 3.2`: Added `master` type in for `TYPE` option.
+- `>= 5`: Replaced `slave` `TYPE` with `replica`. `slave` still supported for
+  backward compatibility.
+- `>= 6.2`: `LADDR` option.
```

### Comparing `iredis-1.9.3/iredis/data/commands/client-pause.md` & `iredis-1.9.4/iredis/data/commands/client-pause.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,62 @@
 `CLIENT PAUSE` is a connections control command able to suspend all the Redis
 clients for the specified amount of time (in milliseconds).
 
 The command performs the following actions:
 
-- It stops processing all the pending commands from normal and pub/sub clients.
-  However interactions with replicas will continue normally.
+- It stops processing all the pending commands from normal and pub/sub clients
+  for the given mode. However interactions with replicas will continue normally.
+  Note that clients are formally paused when they try to execute a command, so
+  no work is taken on the server side for inactive clients.
 - However it returns OK to the caller ASAP, so the `CLIENT PAUSE` command
   execution is not paused by itself.
 - When the specified amount of time has elapsed, all the clients are unblocked:
   this will trigger the processing of all the commands accumulated in the query
   buffer of every client during the pause.
 
+Client pause currently supports two modes:
+
+- `ALL`: This is the default mode. All client commands are blocked.
+- `WRITE`: Clients are only blocked if they attempt to execute a write command.
+
+For the `WRITE` mode, some commands have special behavior:
+
+- `EVAL`/`EVALSHA`: Will block client for all scripts.
+- `PUBLISH`: Will block client.
+- `PFCOUNT`: Will block client.
+- `WAIT`: Acknowledgements will be delayed, so this command will appear blocked.
+
 This command is useful as it makes able to switch clients from a Redis instance
 to another one in a controlled way. For example during an instance upgrade the
 system administrator could do the following:
 
 - Pause the clients using `CLIENT PAUSE`
 - Wait a few seconds to make sure the replicas processed the latest replication
   stream from the master.
 - Turn one of the replicas into a master.
 - Reconfigure clients to connect with the new master.
 
-It is possible to send `CLIENT PAUSE` in a MULTI/EXEC block together with the
-`INFO replication` command in order to get the current master offset at the time
-the clients are blocked. This way it is possible to wait for a specific offset
-in the replica side in order to make sure all the replication stream was
-processed.
+Since Redis 6.2, the recommended mode for client pause is `WRITE`. This mode
+will stop all replication traffic, can be aborted with the `CLIENT UNPAUSE`
+command, and allows reconfiguring the old master without risking accepting
+writes after the failover. This is also the mode used during cluster failover.
+
+For versions before 6.2, it is possible to send `CLIENT PAUSE` in a MULTI/EXEC
+block together with the `INFO replication` command in order to get the current
+master offset at the time the clients are blocked. This way it is possible to
+wait for a specific offset in the replica side in order to make sure all the
+replication stream was processed.
 
 Since Redis 3.2.10 / 4.0.0, this command also prevents keys to be evicted or
 expired during the time clients are paused. This way the dataset is guaranteed
 to be static not just from the point of view of clients not being able to write,
 but also from the point of view of internal operations.
 
 @return
 
 @simple-string-reply: The command returns OK or an error if the timeout is
 invalid.
+
+@history
+
+- `>= 3.2.10`: Client pause prevents client pause and key eviction as well.
+- `>= 6.2`: CLIENT PAUSE WRITE mode added along with the `mode` option.
```

### Comparing `iredis-1.9.3/iredis/data/commands/client-reply.md` & `iredis-1.9.4/iredis/data/commands/client-reply.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/client-setname.md` & `iredis-1.9.4/iredis/data/commands/client-setname.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/client-tracking.md` & `iredis-1.9.4/iredis/data/commands/client-tracking.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,17 @@
   requested by the connection. Instead when the broadcasting mode is not
   enabled, Redis will track which keys are fetched using read-only commands, and
   will report invalidation messages only for such keys.
 - `PREFIX <prefix>`: for broadcasting, register a given key prefix, so that
   notifications will be provided only for keys starting with this string. This
   option can be given multiple times to register multiple prefixes. If
   broadcasting is enabled without this option, Redis will send notifications for
-  every key.
+  every key. You can't delete a single prefix, but you can delete all prefixes
+  by disabling and re-enabling tracking. Using this option adds the additional
+  time complexity of O(N^2), where N is the total number of prefixes tracked.
 - `OPTIN`: when broadcasting is NOT active, normally don't track keys in read
   only commands, unless they are called immediately after a `CLIENT CACHING yes`
   command.
 - `OPTOUT`: when broadcasting is NOT active, normally track keys in read only
   commands, unless they are called immediately after a `CLIENT CACHING no`
   command.
 - `NOLOOP`: don't send notifications about keys modified by this connection
```

### Comparing `iredis-1.9.3/iredis/data/commands/client-unblock.md` & `iredis-1.9.4/iredis/data/commands/client-unblock.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-addslots.md` & `iredis-1.9.4/iredis/data/commands/cluster-addslots.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,14 @@
 Note that once a node assigns a set of slots to itself, it will start
 propagating this information in heartbeat packet headers. However the other
 nodes will accept the information only if they have the slot as not already
 bound with another node, or if the configuration epoch of the node advertising
 the new hash slot, is greater than the node currently listed in the table.
 
 This means that this command should be used with care only by applications
-orchestrating Redis Cluster, like `redis-trib`, and the command if used out of
+orchestrating Redis Cluster, like `redis-cli`, and the command if used out of
 the right context can leave the cluster in a wrong state or cause data loss.
 
 @return
 
 @simple-string-reply: `OK` if the command was successful. Otherwise an error is
 returned.
```

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-bumpepoch.md` & `iredis-1.9.4/iredis/data/commands/cluster-bumpepoch.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-count-failure-reports.md` & `iredis-1.9.4/iredis/data/commands/cluster-count-failure-reports.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-delslots.md` & `iredis-1.9.4/iredis/data/commands/cluster-delslots.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,14 @@
     > CLUSTER DELSLOTS 5000 5001
     OK
 
 ## Usage in Redis Cluster
 
 This command only works in cluster mode and may be useful for debugging and in
 order to manually orchestrate a cluster configuration when a new cluster is
-created. It is currently not used by `redis-trib`, and mainly exists for API
+created. It is currently not used by `redis-cli`, and mainly exists for API
 completeness.
 
 @return
 
 @simple-string-reply: `OK` if the command was successful. Otherwise an error is
 returned.
```

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-failover.md` & `iredis-1.9.4/iredis/data/commands/cluster-failover.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-forget.md` & `iredis-1.9.4/iredis/data/commands/cluster-forget.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-getkeysinslot.md` & `iredis-1.9.4/iredis/data/commands/cluster-getkeysinslot.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-info.md` & `iredis-1.9.4/iredis/data/commands/cluster-info.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-keyslot.md` & `iredis-1.9.4/iredis/data/commands/cluster-keyslot.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-meet.md` & `iredis-1.9.4/iredis/data/commands/cluster-meet.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-nodes.md` & `iredis-1.9.4/iredis/data/commands/cluster-nodes.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 happens to be exactly the same as the one used by Redis Cluster itself in order
 to store on disk the cluster state (however the on disk cluster state has a few
 additional info appended at the end).
 
 Note that normally clients willing to fetch the map between Cluster hash slots
 and node addresses should use `CLUSTER SLOTS` instead. `CLUSTER NODES`, that
 provides more information, should be used for administrative tasks, debugging,
-and configuration inspections. It is also used by `redis-trib` in order to
-manage a cluster.
+and configuration inspections. It is also used by `redis-cli` in order to manage
+a cluster.
 
 ## Serialization format
 
 The output of the command is just a space-separated CSV string, where each line
 represents a node in the cluster. The following is an example of output:
 
 ```
@@ -37,16 +37,16 @@
 The meaning of each filed is the following:
 
 1. `id`: The node ID, a 40 characters random string generated when a node is
    created and never changed again (unless `CLUSTER RESET HARD` is used).
 2. `ip:port@cport`: The node address where clients should contact the node to
    run queries.
 3. `flags`: A list of comma separated flags: `myself`, `master`, `slave`,
-   `fail?`, `fail`, `handshake`, `noaddr`, `noflags`. Flags are explained in
-   detail in the next section.
+   `fail?`, `fail`, `handshake`, `noaddr`, `nofailover`, `noflags`. Flags are
+   explained in detail in the next section.
 4. `master`: If the node is a replica, and the master is known, the master node
    ID, otherwise the "-" character.
 5. `ping-sent`: Milliseconds unix time at which the currently active ping was
    sent, or zero if there are no pending pings.
 6. `pong-recv`: Milliseconds unix time the last pong was received.
 7. `config-epoch`: The configuration epoch (or version) of the current node (or
    of the current master if the node is a replica). Each time there is a
@@ -70,14 +70,15 @@
 - `slave`: Node is a replica.
 - `fail?`: Node is in `PFAIL` state. Not reachable for the node you are
   contacting, but still logically reachable (not in `FAIL` state).
 - `fail`: Node is in `FAIL` state. It was not reachable for multiple nodes that
   promoted the `PFAIL` state to `FAIL`.
 - `handshake`: Untrusted node, we are handshaking.
 - `noaddr`: No address known for this node.
+- `nofailover`: Replica will not try to failover.
 - `noflags`: No flags at all.
 
 ## Notes on published config epochs
 
 Replicas broadcast their master's config epochs (in order to get an `UPDATE`
 message if they are found to be stale), so the real config epoch of the replica
 (which is meaningless more or less, since they don't serve hash slots) can be
```

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-replicas.md` & `iredis-1.9.4/iredis/data/commands/cluster-replicas.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-replicate.md` & `iredis-1.9.4/iredis/data/commands/cluster-replicate.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-reset.md` & `iredis-1.9.4/iredis/data/commands/cluster-reset.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-saveconfig.md` & `iredis-1.9.4/iredis/data/commands/cluster-saveconfig.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-set-config-epoch.md` & `iredis-1.9.4/iredis/data/commands/cluster-set-config-epoch.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-setslot.md` & `iredis-1.9.4/iredis/data/commands/cluster-setslot.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,18 @@
 3. Without `ASKING` the behavior is the same as usually. This guarantees that
    clients with a broken hash slots mapping will not write for error in the
    target node, creating a new version of a key that has yet to be migrated.
 
 ## CLUSTER SETSLOT `<slot>` STABLE
 
 This subcommand just clears migrating / importing state from the slot. It is
-mainly used to fix a cluster stuck in a wrong state by `redis-trib fix`.
-Normally the two states are cleared automatically at the end of the migration
-using the `SETSLOT ... NODE ...` subcommand as explained in the next section.
+mainly used to fix a cluster stuck in a wrong state by
+`redis-cli --cluster fix`. Normally the two states are cleared automatically at
+the end of the migration using the `SETSLOT ... NODE ...` subcommand as
+explained in the next section.
 
 ## CLUSTER SETSLOT `<slot>` NODE `<node-id>`
 
 The `NODE` subcommand is the one with the most complex semantics. It associates
 the hash slot with the specified node, however the command works only in
 specific situations and has different side effects depending on the slot state.
 The following is the set of pre-conditions and side effects of the command:
```

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-slaves.md` & `iredis-1.9.4/iredis/data/commands/cluster-slaves.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/cluster-slots.md` & `iredis-1.9.4/iredis/data/commands/cluster-slots.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/command-getkeys.md` & `iredis-1.9.4/iredis/data/commands/command-getkeys.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/command.md` & `iredis-1.9.4/iredis/data/commands/command.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 ### Flags
 
 Command flags is @array-reply containing one or more status replies:
 
 - _write_ - command may result in modifications
 - _readonly_ - command will never modify keys
-- _denyoom_ - reject command if currently OOM
+- _denyoom_ - reject command if currently out of memory
 - _admin_ - server admin command
 - _pubsub_ - pubsub-related command
 - _noscript_ - deny this command from scripts
 - _random_ - command has random results, dangerous for scripts
 - _sort_for_script_ - if called from script, sort output
 - _loading_ - allow command while database is loading
 - _stale_ - allow command while replica has stale data
@@ -105,16 +105,20 @@
 flag `movablekeys` is added to the command flags @array-reply. Your Redis
 Cluster client needs to parse commands marked `movablekeys` to locate all
 relevant key positions.
 
 Complete list of commands currently requiring key location parsing:
 
 - `SORT` - optional `STORE` key, optional `BY` weights, optional `GET` keys
+- `ZUNION` - keys stop when `WEIGHT` or `AGGREGATE` starts
 - `ZUNIONSTORE` - keys stop when `WEIGHT` or `AGGREGATE` starts
+- `ZINTER` - keys stop when `WEIGHT` or `AGGREGATE` starts
 - `ZINTERSTORE` - keys stop when `WEIGHT` or `AGGREGATE` starts
+- `ZDIFF` - keys stop after `numkeys` count arguments
+- `ZDIFFSTORE` - keys stop after `numkeys` count arguments
 - `EVAL` - keys stop after `numkeys` count arguments
 - `EVALSHA` - keys stop after `numkeys` count arguments
 
 Also see `COMMAND GETKEYS` for getting your Redis server tell you where keys are
 in any given command.
 
 ### First Key in Argument List
```

#### html2text {}

```diff
@@ -21,39 +21,42 @@
 name itself. Examples: - `GET` arity is 2 since the command only accepts one
 argument and always has the format `GET _key_`. - `MGET` arity is -2 since the
 command accepts at a minimum one argument, but up to an unlimited number: `MGET
 _key1_ [key2] [key3] ...`. Also note with `MGET`, the -1 value for "last key
 position" means the list of keys may have unlimited length. ### Flags Command
 flags is @array-reply containing one or more status replies: - _write_ -
 command may result in modifications - _readonly_ - command will never modify
-keys - _denyoom_ - reject command if currently OOM - _admin_ - server admin
-command - _pubsub_ - pubsub-related command - _noscript_ - deny this command
-from scripts - _random_ - command has random results, dangerous for scripts -
-_sort_for_script_ - if called from script, sort output - _loading_ - allow
-command while database is loading - _stale_ - allow command while replica has
-stale data - _skip_monitor_ - do not show this command in MONITOR - _asking_ -
-cluster related - accept even if importing - _fast_ - command operates in
-constant or log(N) time. Used for latency monitoring. - _movablekeys_ - keys
-have no pre-determined position. You must discover keys yourself. ### Movable
-Keys ``` 1) 1) "sort" 2) (integer) -2 3) 1) write 2) denyoom 3) movablekeys 4)
-(integer) 1 5) (integer) 1 6) (integer) 1 ``` Some Redis commands have no
-predetermined key locations. For those commands, flag `movablekeys` is added to
-the command flags @array-reply. Your Redis Cluster client needs to parse
-commands marked `movablekeys` to locate all relevant key positions. Complete
-list of commands currently requiring key location parsing: - `SORT` - optional
-`STORE` key, optional `BY` weights, optional `GET` keys - `ZUNIONSTORE` - keys
-stop when `WEIGHT` or `AGGREGATE` starts - `ZINTERSTORE` - keys stop when
-`WEIGHT` or `AGGREGATE` starts - `EVAL` - keys stop after `numkeys` count
-arguments - `EVALSHA` - keys stop after `numkeys` count arguments Also see
-`COMMAND GETKEYS` for getting your Redis server tell you where keys are in any
-given command. ### First Key in Argument List For most commands the first key
-is position 1. Position 0 is always the command name itself. ### Last Key in
-Argument List Redis commands usually accept one key, two keys, or an unlimited
-number of keys. If a command accepts one key, the first key and last key
-positions is 1. If a command accepts two keys (e.g. `BRPOPLPUSH`, `SMOVE`,
+keys - _denyoom_ - reject command if currently out of memory - _admin_ - server
+admin command - _pubsub_ - pubsub-related command - _noscript_ - deny this
+command from scripts - _random_ - command has random results, dangerous for
+scripts - _sort_for_script_ - if called from script, sort output - _loading_ -
+allow command while database is loading - _stale_ - allow command while replica
+has stale data - _skip_monitor_ - do not show this command in MONITOR -
+_asking_ - cluster related - accept even if importing - _fast_ - command
+operates in constant or log(N) time. Used for latency monitoring. -
+_movablekeys_ - keys have no pre-determined position. You must discover keys
+yourself. ### Movable Keys ``` 1) 1) "sort" 2) (integer) -2 3) 1) write 2)
+denyoom 3) movablekeys 4) (integer) 1 5) (integer) 1 6) (integer) 1 ``` Some
+Redis commands have no predetermined key locations. For those commands, flag
+`movablekeys` is added to the command flags @array-reply. Your Redis Cluster
+client needs to parse commands marked `movablekeys` to locate all relevant key
+positions. Complete list of commands currently requiring key location parsing:
+- `SORT` - optional `STORE` key, optional `BY` weights, optional `GET` keys -
+`ZUNION` - keys stop when `WEIGHT` or `AGGREGATE` starts - `ZUNIONSTORE` - keys
+stop when `WEIGHT` or `AGGREGATE` starts - `ZINTER` - keys stop when `WEIGHT`
+or `AGGREGATE` starts - `ZINTERSTORE` - keys stop when `WEIGHT` or `AGGREGATE`
+starts - `ZDIFF` - keys stop after `numkeys` count arguments - `ZDIFFSTORE` -
+keys stop after `numkeys` count arguments - `EVAL` - keys stop after `numkeys`
+count arguments - `EVALSHA` - keys stop after `numkeys` count arguments Also
+see `COMMAND GETKEYS` for getting your Redis server tell you where keys are in
+any given command. ### First Key in Argument List For most commands the first
+key is position 1. Position 0 is always the command name itself. ### Last Key
+in Argument List Redis commands usually accept one key, two keys, or an
+unlimited number of keys. If a command accepts one key, the first key and last
+key positions is 1. If a command accepts two keys (e.g. `BRPOPLPUSH`, `SMOVE`,
 `RENAME`, ...) then the last key position is the location of the last key in
 the argument list. If a command accepts an unlimited number of keys, the last
 key position is -1. ### Step Count
 1) 1) "mset"       1) 1) "mget"
    2) (integer) -3    2) (integer) -2
    3) 1) write        3) 1) readonly
       2) denyoom      4) (integer) 1
```

### Comparing `iredis-1.9.3/iredis/data/commands/config-get.md` & `iredis-1.9.4/iredis/data/commands/config-get.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/config-rewrite.md` & `iredis-1.9.4/iredis/data/commands/config-rewrite.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/config-set.md` & `iredis-1.9.4/iredis/data/commands/config-set.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 All the configuration parameters set using `CONFIG SET` are immediately loaded
 by Redis and will take effect starting with the next command executed.
 
 All the supported parameters have the same meaning of the equivalent
 configuration parameter used in the [redis.conf][hgcarr22rc] file, with the
 following important differences:
 
-[hgcarr22rc]: http://github.com/redis/redis/raw/2.8/redis.conf
+[hgcarr22rc]: http://github.com/redis/redis/raw/6.0/redis.conf
 
 - In options where bytes or other quantities are specified, it is not possible
   to use the `redis.conf` abbreviated form (`10k`, `2gb` ... and so forth),
   everything should be specified as a well-formed 64-bit integer, in the base
   unit of the configuration directive. However since Redis version 3.0 or
   greater, it is possible to use `CONFIG SET` with memory units for `maxmemory`,
   client output buffers, and replication backlog size.
```

### Comparing `iredis-1.9.3/iredis/data/commands/decr.md` & `iredis-1.9.4/iredis/data/commands/decr.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/dump.md` & `iredis-1.9.4/iredis/data/commands/dump.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/eval.md` & `iredis-1.9.4/iredis/data/commands/eval.md`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,35 @@
 ```
 
 Using `redis.pcall()` no error is raised, but an error object is returned in the
 format specified above (as a Lua table with an `err` field). The script can pass
 the exact error to the user by returning the error object returned by
 `redis.pcall()`.
 
+## Running Lua under low memory conditions
+
+When the memory usage in Redis exceeds the `maxmemory` limit, the first write
+command encountered in the Lua script that uses additional memory will cause the
+script to abort (unless `redis.pcall` was used). However, one thing to caution
+here is that if the first write command does not use additional memory such as
+DEL, LREM, or SREM, etc, Redis will allow it to run and all subsequent commands
+in the Lua script will execute to completion for atomicity. If the subsequent
+writes in the script generate additional memory, the Redis memory usage can go
+over `maxmemory`.
+
+Another possible way for Lua script to cause Redis memory usage to go above
+`maxmemory` happens when the script execution starts when Redis is slightly
+below `maxmemory` so the first write command in the script is allowed. As the
+script executes, subsequent write commands continue to generate memory and
+causes the Redis server to go above `maxmemory`.
+
+In those scenarios, it is recommended to configure the `maxmemory-policy` not to
+use `noeviction`. Also Lua scripts should be short so that evictions of items
+can happen in between Lua scripts.
+
 ## Bandwidth and EVALSHA
 
 The `EVAL` command forces you to send the script body again and again. Redis
 does not need to recompile the script every time as it uses an internal caching
 mechanism, however paying the cost of the additional bandwidth may not be
 optimal in many contexts.
 
@@ -615,21 +636,21 @@
 
 The semantic change between patch level releases was needed since the old
 behavior was inherently incompatible with the Redis replication layer and was
 the cause of bugs.
 
 ## Using Lua scripting in RESP3 mode
 
-Starting with Redis version 6, the server supports two differnent protocols. One
+Starting with Redis version 6, the server supports two different protocols. One
 is called RESP2, and is the old protocol: all the new connections to the server
 start in this mode. However clients are able to negotiate the new protocol using
 the `HELLO` command: this way the connection is put in RESP3 mode. In this mode
 certain commands, like for instance `HGETALL`, reply with a new data type (the
 Map data type in this specific case). The RESP3 protocol is semantically more
-powerful, however most scripts are ok with using just RESP2.
+powerful, however most scripts are OK with using just RESP2.
 
 The Lua engine always assumes to run in RESP2 mode when talking with Redis, so
 whatever the connection that is invoking the `EVAL` or `EVALSHA` command is in
 RESP2 or RESP3 mode, Lua scripts will, by default, still see the same kind of
 replies they used to see in the past from Redis, when calling commands using the
 `redis.call()` built-in function.
 
@@ -665,15 +686,15 @@
 
 - Lua boolean -> Redis boolean true or false. **Note that this is a change
   compared to the RESP2 mode**, where returning true from Lua returned the
   number 1 to the Redis client, and returning false used to return NULL.
 - Lua table with a single `map` field set to a field-value Lua table -> Redis
   map reply.
 - Lua table with a single `set` field set to a field-value Lua table -> Redis
-  set reply, the values are discared and can be anything.
+  set reply, the values are discarded and can be anything.
 - Lua table with a single `double` field set to a field-value Lua table -> Redis
   double reply.
 - Lua null -> Redis RESP3 new null reply (protocol `"_\r\n"`).
 - All the RESP2 old conversions still apply unless specified above.
 
 There is one key thing to understand: in case Lua replies with RESP3 types, but
 the connection calling Lua is in RESP2 mode, Redis will automatically convert
```

### Comparing `iredis-1.9.3/iredis/data/commands/exists.md` & `iredis-1.9.4/iredis/data/commands/exists.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/expire.md` & `iredis-1.9.4/iredis/data/commands/expire.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/expireat.md` & `iredis-1.9.4/iredis/data/commands/expireat.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/geoadd.md` & `iredis-1.9.4/iredis/data/commands/set.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,90 @@
-Adds the specified geospatial items (latitude, longitude, name) to the specified
-key. Data is stored into the key as a sorted set, in a way that makes it
-possible to later retrieve items using a query by radius with the `GEORADIUS` or
-`GEORADIUSBYMEMBER` commands.
-
-The command takes arguments in the standard format x,y so the longitude must be
-specified before the latitude. There are limits to the coordinates that can be
-indexed: areas very near to the poles are not indexable. The exact limits, as
-specified by EPSG:900913 / EPSG:3785 / OSGEO:41001 are the following:
-
-- Valid longitudes are from -180 to 180 degrees.
-- Valid latitudes are from -85.05112878 to 85.05112878 degrees.
-
-The command will report an error when the user attempts to index coordinates
-outside the specified ranges.
-
-**Note:** there is no **GEODEL** command because you can use `ZREM` in order to
-remove elements. The Geo index structure is just a sorted set.
-
-## How does it work?
-
-The way the sorted set is populated is using a technique called
-[Geohash](https://en.wikipedia.org/wiki/Geohash). Latitude and Longitude bits
-are interleaved in order to form an unique 52 bit integer. We know that a sorted
-set double score can represent a 52 bit integer without losing precision.
-
-This format allows for radius querying by checking the 1+8 areas needed to cover
-the whole radius, and discarding elements outside the radius. The areas are
-checked by calculating the range of the box covered removing enough bits from
-the less significant part of the sorted set score, and computing the score range
-to query in the sorted set for each area.
-
-## What Earth model does it use?
-
-It just assumes that the Earth is a sphere, since the used distance formula is
-the Haversine formula. This formula is only an approximation when applied to the
-Earth, which is not a perfect sphere. The introduced errors are not an issue
-when used in the context of social network sites that need to query by radius
-and most other applications. However in the worst case the error may be up to
-0.5%, so you may want to consider other systems for error-critical applications.
+Set `key` to hold the string `value`. If `key` already holds a value, it is
+overwritten, regardless of its type. Any previous time to live associated with
+the key is discarded on successful `SET` operation.
+
+## Options
+
+The `SET` command supports a set of options that modify its behavior:
+
+- `EX` _seconds_ -- Set the specified expire time, in seconds.
+- `PX` _milliseconds_ -- Set the specified expire time, in milliseconds.
+- `EXAT` _timestamp-seconds_ -- Set the specified Unix time at which the key
+  will expire, in seconds.
+- `PXAT` _timestamp-milliseconds_ -- Set the specified Unix time at which the
+  key will expire, in milliseconds.
+- `NX` -- Only set the key if it does not already exist.
+- `XX` -- Only set the key if it already exist.
+- `KEEPTTL` -- Retain the time to live associated with the key.
+- `GET` -- Return the old string stored at key, or nil if key did not exist. An
+  error is returned and `SET` aborted if the value stored at key is not a
+  string.
+
+Note: Since the `SET` command options can replace `SETNX`, `SETEX`, `PSETEX`,
+`GETSET`, it is possible that in future versions of Redis these commands will be
+deprecated and finally removed.
 
 @return
 
-@integer-reply, specifically:
+@simple-string-reply: `OK` if `SET` was executed correctly.
 
-- The number of elements added to the sorted set, not including elements already
-  existing for which the score was updated.
+@nil-reply: `(nil)` if the `SET` operation was not performed because the user
+specified the `NX` or `XX` option but the condition was not met.
+
+If the command is issued with the `GET` option, the above does not apply. It
+will instead reply as follows, regardless if the `SET` was actually performed:
+
+@bulk-string-reply: the old string value stored at key.
+
+@nil-reply: `(nil)` if the key did not exist.
+
+@history
+
+- `>= 2.6.12`: Added the `EX`, `PX`, `NX` and `XX` options.
+- `>= 6.0`: Added the `KEEPTTL` option.
+- `>= 6.2`: Added the `GET`, `EXAT` and `PXAT` option.
+- `>= 7.0`: Allowed the `NX` and `GET` options to be used together.
 
 @examples
 
 ```cli
-GEOADD Sicily 13.361389 38.115556 "Palermo" 15.087269 37.502669 "Catania"
-GEODIST Sicily Palermo Catania
-GEORADIUS Sicily 15 37 100 km
-GEORADIUS Sicily 15 37 200 km
+SET mykey "Hello"
+GET mykey
+
+SET anotherkey "will expire in a minute" EX 60
 ```
+
+## Patterns
+
+**Note:** The following pattern is discouraged in favor of
+[the Redlock algorithm](https://redis.io/topics/distlock) which is only a bit
+more complex to implement, but offers better guarantees and is fault tolerant.
+
+The command `SET resource-name anystring NX EX max-lock-time` is a simple way to
+implement a locking system with Redis.
+
+A client can acquire the lock if the above command returns `OK` (or retry after
+some time if the command returns Nil), and remove the lock just using `DEL`.
+
+The lock will be auto-released after the expire time is reached.
+
+It is possible to make this system more robust modifying the unlock schema as
+follows:
+
+- Instead of setting a fixed string, set a non-guessable large random string,
+  called token.
+- Instead of releasing the lock with `DEL`, send a script that only removes the
+  key if the value matches.
+
+This avoids that a client will try to release the lock after the expire time
+deleting the key created by another client that acquired the lock later.
+
+An example of unlock script would be similar to the following:
+
+    if redis.call("get",KEYS[1]) == ARGV[1]
+    then
+        return redis.call("del",KEYS[1])
+    else
+        return 0
+    end
+
+The script should be called with `EVAL ...script... 1 resource-name token-value`
```

### Comparing `iredis-1.9.3/iredis/data/commands/geodecode.md` & `iredis-1.9.4/iredis/data/commands/geodecode.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/geodist.md` & `iredis-1.9.4/iredis/data/commands/geodist.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/geoencode.md` & `iredis-1.9.4/iredis/data/commands/geoencode.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/geohash.md` & `iredis-1.9.4/iredis/data/commands/geohash.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/geopos.md` & `iredis-1.9.4/iredis/data/commands/geopos.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/georadius.md` & `iredis-1.9.4/iredis/data/commands/georadius.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Return the members of a sorted set populated with geospatial information using
 `GEOADD`, which are within the borders of the area specified with the center
 location and the maximum distance from the center (the radius).
 
+As per Redis 6.2.0, GEORADIUS command family are considered deprecated. Please
+prefer `GEOSEARCH` and `GEOSEARCHSTORE` in new code.
+
 This manual page also covers the `GEORADIUS_RO` and `GEORADIUSBYMEMBER_RO`
 variants (see the section below for more information).
 
 The common use case for this command is to retrieve geospatial items near a
 specified point not farther than a given amount of meters (or other units). This
 allows, for example, to suggest mobile users of an application nearby places.
 
@@ -34,19 +37,21 @@
 - `ASC`: Sort returned items from the nearest to the farthest, relative to the
   center.
 - `DESC`: Sort returned items from the farthest to the nearest, relative to the
   center.
 
 By default all the matching items are returned. It is possible to limit the
 results to the first N matching items by using the **COUNT `<count>`** option.
-However note that internally the command needs to perform an effort proportional
-to the number of items matching the specified area, so to query very large areas
-with a very small `COUNT` option may be slow even if just a few results are
-returned. On the other hand `COUNT` can be a very effective way to reduce
-bandwidth usage if normally just the first results are used.
+When `ANY` is provided the command will return as soon as enough matches are
+found, so the results may not be the ones closest to the specified point, but on
+the other hand, the effort invested by the server is significantly lower. When
+`ANY` is not provided, the command will perform an effort that is proportional
+to the number of items matching the specified area and sort them, so to query
+very large areas with a very small `COUNT` option may be slow even if just a few
+results are returned.
 
 By default the command returns the items to the client. It is possible to store
 the results with one of these options:
 
 - `!STORE`: Store the items in a sorted set populated with their geospatial
   information.
 - `!STOREDIST`: Store the items in a sorted set populated with their distance
@@ -89,14 +94,18 @@
 for Redis 4.0, so instead two read only variants of the commands were added.
 They are exactly like the original commands but refuse the `STORE` and
 `STOREDIST` options. The two variants are called `GEORADIUS_RO` and
 `GEORADIUSBYMEMBER_RO`, and can safely be used in replicas.
 
 Both commands were introduced in Redis 3.2.10 and Redis 4.0.0 respectively.
 
+@history
+
+- `>= 6.2`: Added the `ANY` option for `COUNT`.
+
 @examples
 
 ```cli
 GEOADD Sicily 13.361389 38.115556 "Palermo" 15.087269 37.502669 "Catania"
 GEORADIUS Sicily 15 37 200 km WITHDIST
 GEORADIUS Sicily 15 37 200 km WITHCOORD
 GEORADIUS Sicily 15 37 200 km WITHDIST WITHCOORD
```

### Comparing `iredis-1.9.3/iredis/data/commands/georadiusbymember.md` & `iredis-1.9.4/iredis/data/commands/georadiusbymember.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 This command is exactly like `GEORADIUS` with the sole difference that instead
 of taking, as the center of the area to query, a longitude and latitude value,
 it takes the name of a member already existing inside the geospatial index
 represented by the sorted set.
 
+As per Redis 6.2.0, GEORADIUS command family are considered deprecated. Please
+prefer `GEOSEARCH` and `GEOSEARCHSTORE` in new code.
+
 The position of the specified member is used as the center of the query.
 
 Please check the example below and the `GEORADIUS` documentation for more
 information about the command and its options.
 
 Note that `GEORADIUSBYMEMBER_RO` is also available since Redis 3.2.10 and Redis
 4.0.0 in order to provide a read-only command that can be used in replicas. See
```

### Comparing `iredis-1.9.3/iredis/data/commands/getrange.md` & `iredis-1.9.4/iredis/data/commands/getrange.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/hdel.md` & `iredis-1.9.4/iredis/data/commands/hdel.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/hincrby.md` & `iredis-1.9.4/iredis/data/commands/hincrby.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/hincrbyfloat.md` & `iredis-1.9.4/iredis/data/commands/hincrbyfloat.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/hmget.md` & `iredis-1.9.4/iredis/data/commands/hmget.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/incr.md` & `iredis-1.9.4/iredis/data/commands/incr.md`

 * *Files 5% similar despite different names*

```diff
@@ -61,22 +61,22 @@
 
 The more simple and direct implementation of this pattern is the following:
 
 ```
 FUNCTION LIMIT_API_CALL(ip)
 ts = CURRENT_UNIX_TIME()
 keyname = ip+":"+ts
-current = GET(keyname)
-IF current != NULL AND current > 10 THEN
+MULTI
+    INCR(keyname)
+    EXPIRE(keyname,10)
+EXEC
+current = RESPONSE_OF_INCR_WITHIN_MULTI
+IF current > 10 THEN
     ERROR "too many requests per second"
 ELSE
-    MULTI
-        INCR(keyname,1)
-        EXPIRE(keyname,10)
-    EXEC
     PERFORM_API_CALL()
 END
 ```
 
 Basically we have a counter for every IP, for every different second. But this
 counters are always incremented setting an expire of 10 seconds so that they'll
 be removed by Redis automatically when the current second is a different one.
@@ -115,15 +115,15 @@
 This can be fixed easily turning the `INCR` with optional `EXPIRE` into a Lua
 script that is send using the `EVAL` command (only available since Redis version
 2.6).
 
 ```
 local current
 current = redis.call("incr",KEYS[1])
-if tonumber(current) == 1 then
+if current == 1 then
     redis.call("expire",KEYS[1],1)
 end
 ```
 
 There is a different way to fix this issue without using scripting, but using
 Redis lists instead of counters. The implementation is more complex and uses
 more advanced features but has the advantage of remembering the IP addresses of
```

### Comparing `iredis-1.9.3/iredis/data/commands/incrbyfloat.md` & `iredis-1.9.4/iredis/data/commands/incrbyfloat.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/info.md` & `iredis-1.9.4/iredis/data/commands/info.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 - `replication`: Master/replica replication information
 - `cpu`: CPU consumption statistics
 - `commandstats`: Redis command statistics
 - `cluster`: Redis Cluster section
 - `modules`: Modules section
 - `keyspace`: Database related statistics
 - `modules`: Module related sections
+- `errorstats`: Redis error statistics
 
 It can also take the following values:
 
 - `all`: Return all sections (excluding module generated ones)
 - `default`: Return only the default set of sections
 - `everything`: Includes `all` and `modules`
 
@@ -56,34 +57,41 @@
 - `multiplexing_api`: Event loop mechanism used by Redis
 - `atomicvar_api`: Atomicvar API used by Redis
 - `gcc_version`: Version of the GCC compiler used to compile the Redis server
 - `process_id`: PID of the server process
 - `run_id`: Random value identifying the Redis server (to be used by Sentinel
   and Cluster)
 - `tcp_port`: TCP/IP listen port
+- `server_time_in_usec`: Epoch-based system time with microsecond precision
 - `uptime_in_seconds`: Number of seconds since Redis server start
 - `uptime_in_days`: Same value expressed in days
 - `hz`: The server's current frequency setting
 - `configured_hz`: The server's configured frequency setting
 - `lru_clock`: Clock incrementing every minute, for LRU management
 - `executable`: The path to the server's executable
 - `config_file`: The path to the config file
 
 Here is the meaning of all fields in the **clients** section:
 
 - `connected_clients`: Number of client connections (excluding connections from
   replicas)
+- `cluster_connections`: An approximation of the number of sockets used by the
+  cluster's bus
+- `maxclients`: The value of the `maxclients` configuration directive. This is
+  the upper limit for the sum of `connected_clients`, `connected_slaves` and
+  `cluster_connections`.
 - `client_longest_output_list`: Longest output list among current client
   connections
 - `client_biggest_input_buf`: Biggest input buffer among current client
   connections
 - `blocked_clients`: Number of clients pending on a blocking call (`BLPOP`,
-  `BRPOP`, `BRPOPLPUSH`, `BZPOPMIN`, `BZPOPMAX`)
+  `BRPOP`, `BRPOPLPUSH`, `BLMOVE`, `BZPOPMIN`, `BZPOPMAX`)
 - `tracking_clients`: Number of clients being tracked (`CLIENT TRACKING`)
 - `clients_in_timeout_table`: Number of clients in the clients timeout table
+- `io_threads_active`: Flag indicating if I/O threads are active
 
 Here is the meaning of all fields in the **memory** section:
 
 - `used_memory`: Total number of bytes allocated by Redis using its allocator
   (either standard **libc**, **jemalloc**, or an alternative allocator such as
   [**tcmalloc**][hcgcpgp])
 - `used_memory_human`: Human readable representation of previous value
@@ -139,38 +147,47 @@
 
 Additional introspective information about the server's memory can be obtained
 by referring to the `MEMORY STATS` command and the `MEMORY DOCTOR`.
 
 Here is the meaning of all fields in the **persistence** section:
 
 - `loading`: Flag indicating if the load of a dump file is on-going
+- `current_cow_size`: The size in bytes of copy-on-write memory while a child
+  fork is running
+- `current_fork_perc`: The percentage of progress of the current fork process.
+  For AOF and RDB forks it is the percentage of `current_save_keys_processed`
+  out of `current_save_keys_total`.
+- `current_save_keys_processed`: Number of keys processed by the current save
+  operation
+- `current_save_keys_total`: Number of keys at the beginning of the current save
+  operation
 - `rdb_changes_since_last_save`: Number of changes since the last dump
 - `rdb_bgsave_in_progress`: Flag indicating a RDB save is on-going
 - `rdb_last_save_time`: Epoch-based timestamp of last successful RDB save
 - `rdb_last_bgsave_status`: Status of the last RDB save operation
 - `rdb_last_bgsave_time_sec`: Duration of the last RDB save operation in seconds
 - `rdb_current_bgsave_time_sec`: Duration of the on-going RDB save operation if
   any
-- `rdb_last_cow_size`: The size in bytes of copy-on-write allocations during the
-  last RDB save operation
+- `rdb_last_cow_size`: The size in bytes of copy-on-write memory during the last
+  RDB save operation
 - `aof_enabled`: Flag indicating AOF logging is activated
 - `aof_rewrite_in_progress`: Flag indicating a AOF rewrite operation is on-going
 - `aof_rewrite_scheduled`: Flag indicating an AOF rewrite operation will be
   scheduled once the on-going RDB save is complete.
 - `aof_last_rewrite_time_sec`: Duration of the last AOF rewrite operation in
   seconds
 - `aof_current_rewrite_time_sec`: Duration of the on-going AOF rewrite operation
   if any
 - `aof_last_bgrewrite_status`: Status of the last AOF rewrite operation
 - `aof_last_write_status`: Status of the last write operation to the AOF
-- `aof_last_cow_size`: The size in bytes of copy-on-write allocations during the
-  last AOF rewrite operation
+- `aof_last_cow_size`: The size in bytes of copy-on-write memory during the last
+  AOF rewrite operation
 - `module_fork_in_progress`: Flag indicating a module fork is on-going
-- `module_fork_last_cow_size`: The size in bytes of copy-on-write allocations
-  during the last module fork operation
+- `module_fork_last_cow_size`: The size in bytes of copy-on-write memory during
+  the last module fork operation
 
 `rdb_changes_since_last_save` refers to the number of operations that produced
 some kind of changes in the dataset since the last time either `SAVE` or
 `BGSAVE` was called.
 
 If AOF is activated, these additional fields will be added:
 
@@ -183,14 +200,16 @@
 - `aof_pending_bio_fsync`: Number of fsync pending jobs in background I/O queue
 - `aof_delayed_fsync`: Delayed fsync counter
 
 If a load operation is on-going, these additional fields will be added:
 
 - `loading_start_time`: Epoch-based timestamp of the start of the load operation
 - `loading_total_bytes`: Total file size
+- `loading_rdb_used_mem`: The memory usage of the server that had generated the
+  RDB file at the time of the file's creation
 - `loading_loaded_bytes`: Number of bytes already loaded
 - `loading_loaded_perc`: Same value expressed as a percentage
 - `loading_eta_seconds`: ETA in seconds for the load to be complete
 
 Here is the meaning of all fields in the **stats** section:
 
 - `total_connections_received`: Total number of connections accepted by the
@@ -214,14 +233,15 @@
   expiry cycles
 - `evicted_keys`: Number of evicted keys due to `maxmemory` limit
 - `keyspace_hits`: Number of successful lookup of keys in the main dictionary
 - `keyspace_misses`: Number of failed lookup of keys in the main dictionary
 - `pubsub_channels`: Global number of pub/sub channels with client subscriptions
 - `pubsub_patterns`: Global number of pub/sub pattern with client subscriptions
 - `latest_fork_usec`: Duration of the latest fork operation in microseconds
+- `total_forks`: Total number of fork operations since the server start
 - `migrate_cached_sockets`: The number of sockets open for `MIGRATE` purposes
 - `slave_expires_tracked_keys`: The number of keys tracked for expiry purposes
   (applicable only to writable replicas)
 - `active_defrag_hits`: Number of value reallocations performed by active the
   defragmentation process
 - `active_defrag_misses`: Number of aborted value reallocations started by the
   active defragmentation process
@@ -231,20 +251,30 @@
 - `tracking_total_keys`: Number of keys being tracked by the server
 - `tracking_total_items`: Number of items, that is the sum of clients number for
   each key, that are being tracked
 - `tracking_total_prefixes`: Number of tracked prefixes in server's prefix table
   (only applicable for broadcast mode)
 - `unexpected_error_replies`: Number of unexpected error replies, that are types
   of errors from an AOF load or replication
+- `total_error_replies`: Total number of issued error replies, that is the sum
+  of rejected commands (errors prior command execution) and failed commands
+  (errors within the command execution)
+- `total_reads_processed`: Total number of read events processed
+- `total_writes_processed`: Total number of write events processed
+- `io_threaded_reads_processed`: Number of read events processed by the main and
+  I/O threads
+- `io_threaded_writes_processed`: Number of write events processed by the main
+  and I/O threads
 
 Here is the meaning of all fields in the **replication** section:
 
 - `role`: Value is "master" if the instance is replica of no one, or "slave" if
   the instance is a replica of some master instance. Note that a replica can be
   master of another replica (chained replication).
+- `master_failover_state`: The state of an ongoing failover, if any.
 - `master_replid`: The replication ID of the Redis server.
 - `master_replid2`: The secondary replication ID, used for PSYNC after a
   failover.
 - `master_repl_offset`: The server's current replication offset
 - `second_repl_offset`: The offset up to which replication IDs are accepted
 - `repl_backlog_active`: Flag indicating replication backlog is active
 - `repl_backlog_size`: Total size in bytes of the replication backlog buffer
@@ -263,15 +293,23 @@
 - `master_sync_in_progress`: Indicate the master is syncing to the replica
 - `slave_repl_offset`: The replication offset of the replica instance
 - `slave_priority`: The priority of the instance as a candidate for failover
 - `slave_read_only`: Flag indicating if the replica is read-only
 
 If a SYNC operation is on-going, these additional fields are provided:
 
-- `master_sync_left_bytes`: Number of bytes left before syncing is complete
+- `master_sync_total_bytes`: Total number of bytes that need to be transferred.
+  this may be 0 when the size is unknown (for example, when the
+  `repl-diskless-sync` configuration directive is used)
+- `master_sync_read_bytes`: Number of bytes already transferred
+- `master_sync_left_bytes`: Number of bytes left before syncing is complete (may
+  be negative when `master_sync_total_bytes` is 0)
+- `master_sync_perc`: The percentage `master_sync_read_bytes` from
+  `master_sync_total_bytes`, or an approximation that uses
+  `loading_rdb_used_mem` when `master_sync_total_bytes` is 0
 - `master_sync_last_io_seconds_ago`: Number of seconds since last transfer I/O
   during a SYNC operation
 
 If the link between master and replica is down, an additional field is provided:
 
 - `master_link_down_since_seconds`: Number of seconds since the link is down
 
@@ -287,26 +325,44 @@
 
 For each replica, the following line is added:
 
 - `slaveXXX`: id, IP address, port, state, offset, lag
 
 Here is the meaning of all fields in the **cpu** section:
 
-- `used_cpu_sys`: System CPU consumed by the Redis server
-- `used_cpu_user`:User CPU consumed by the Redis server
+- `used_cpu_sys`: System CPU consumed by the Redis server, which is the sum of
+  system CPU consumed by all threads of the server process (main thread and
+  background threads)
+- `used_cpu_user`: User CPU consumed by the Redis server, which is the sum of
+  user CPU consumed by all threads of the server process (main thread and
+  background threads)
 - `used_cpu_sys_children`: System CPU consumed by the background processes
 - `used_cpu_user_children`: User CPU consumed by the background processes
+- `used_cpu_sys_main_thread`: System CPU consumed by the Redis server main
+  thread
+- `used_cpu_user_main_thread`: User CPU consumed by the Redis server main thread
 
 The **commandstats** section provides statistics based on the command type,
-including the number of calls, the total CPU time consumed by these commands,
-and the average CPU consumed per command execution.
+including the number of calls that reached command execution (not rejected), the
+total CPU time consumed by these commands, the average CPU consumed per command
+execution, the number of rejected calls (errors prior command execution), and
+the number of failed calls (errors within the command execution).
 
 For each command type, the following line is added:
 
-- `cmdstat_XXX`: `calls=XXX,usec=XXX,usec_per_call=XXX`
+- `cmdstat_XXX`:
+  `calls=XXX,usec=XXX,usec_per_call=XXX,rejected_calls=XXX,failed_calls=XXX`
+
+The **errorstats** section enables keeping track of the different errors that
+occurred within Redis, based upon the reply error prefix ( The first word after
+the "-", up to the first space. Example: `ERR` ).
+
+For each error type, the following line is added:
+
+- `errorstat_XXX`: `count=XXX`
 
 The **cluster** section currently only contains a unique field:
 
 - `cluster_enabled`: Indicate Redis cluster is enabled
 
 The **modules** section contains additional information about loaded modules if
 the modules provide it. The field part of properties lines in this section is
```

### Comparing `iredis-1.9.3/iredis/data/commands/keys.md` & `iredis-1.9.4/iredis/data/commands/keys.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/latency-doctor.md` & `iredis-1.9.4/iredis/data/commands/latency-doctor.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/latency-graph.md` & `iredis-1.9.4/iredis/data/commands/latency-graph.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/latency-history.md` & `iredis-1.9.4/iredis/data/commands/latency-history.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/latency-latest.md` & `iredis-1.9.4/iredis/data/commands/latency-latest.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/latency-reset.md` & `iredis-1.9.4/iredis/data/commands/latency-reset.md`

 * *Files 12% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 - `fork`
 - `rdb-unlink-temp-file`
 
 For more information refer to the [Latency Monitoring Framework page][lm].
 
 [lm]: /topics/latency-monitor
 
-@reply
+@return
 
 @integer-reply: the number of event time series that were reset.
```

### Comparing `iredis-1.9.3/iredis/data/commands/lindex.md` & `iredis-1.9.4/iredis/data/commands/lindex.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/lolwut.md` & `iredis-1.9.4/iredis/data/commands/lolwut.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/lpos.md` & `iredis-1.9.4/iredis/data/commands/lpos.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 The command returns the index of matching elements inside a Redis list. By
 default, when no options are given, it will scan the list from head to tail,
 looking for the first match of "element". If the element is found, its index
 (the zero-based position in the list) is returned. Otherwise, if no match is
-found, NULL is returned.
+found, `nil` is returned.
 
 ```
 > RPUSH mylist a b c 1 2 3 c c
 > LPOS mylist c
 2
 ```
 
@@ -60,33 +60,37 @@
 
 When `COUNT` is used, it is possible to specify 0 as the number of matches, as a
 way to tell the command we want all the matches found returned as an array of
 indexes. This is better than giving a very large `COUNT` option because it is
 more general.
 
 ```
-> LPOS mylist COUNT 0
+> LPOS mylist c COUNT 0
 [2,6,7]
 ```
 
 When `COUNT` is used and no match is found, an empty array is returned. However
-when `COUNT` is not used and there are no matches, the command returns NULL.
+when `COUNT` is not used and there are no matches, the command returns `nil`.
 
 Finally, the `MAXLEN` option tells the command to compare the provided element
 only with a given maximum number of list items. So for instance specifying
 `MAXLEN 1000` will make sure that the command performs only 1000 comparisons,
 effectively running the algorithm on a subset of the list (the first part or the
 last part depending on the fact we use a positive or negative rank). This is
 useful to limit the maximum complexity of the command. It is also useful when we
 expect the match to be found very early, but want to be sure that in case this
 is not true, the command does not take too much time to run.
 
+When `MAXLEN` is used, it is possible to specify 0 as the maximum number of
+comparisons, as a way to tell the command we want unlimited comparisons. This is
+better than giving a very large `MAXLEN` option because it is more general.
+
 @return
 
-The command returns the integer representing the matching element, or null if
+The command returns the integer representing the matching element, or `nil` if
 there is no match. However, if the `COUNT` option is given the command returns
 an array (empty if there are no matches).
 
 @examples
 
 ```cli
 RPUSH mylist a b c d 1 2 3 4 3 3 3
```

### Comparing `iredis-1.9.3/iredis/data/commands/lpush.md` & `iredis-1.9.4/iredis/data/commands/lpush.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/lpushx.md` & `iredis-1.9.4/iredis/data/commands/lpushx.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/lrange.md` & `iredis-1.9.4/iredis/data/commands/lrange.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/lrem.md` & `iredis-1.9.4/iredis/data/commands/lrem.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/ltrim.md` & `iredis-1.9.4/iredis/data/commands/ltrim.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/memory-stats.md` & `iredis-1.9.4/iredis/data/commands/memory-stats.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/memory-usage.md` & `iredis-1.9.4/iredis/data/commands/memory-usage.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 OK
 127.0.0.1:6379> MEMORY USAGE cento
 (integer) 153
 ```
 
 @return
 
-@integer-reply: the memory usage in bytes
+@integer-reply: the memory usage in bytes, or `nil` when the key does not exist.
```

### Comparing `iredis-1.9.3/iredis/data/commands/migrate.md` & `iredis-1.9.4/iredis/data/commands/migrate.md`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,18 @@
 - `KEYS` -- If the key argument is an empty string, the command will instead
   migrate all the keys that follow the `KEYS` option (see the above section for
   more info).
 - `AUTH` -- Authenticate with the given password to the remote instance.
 - `AUTH2` -- Authenticate with the given username and password pair (Redis 6 or
   greater ACL auth style).
 
-`COPY` and `REPLACE` are available only in 3.0 and above. `KEYS` is available
-starting with Redis 3.0.6. `AUTH` is available starting with Redis 4.0.7.
-`AUTH2` is available starting with Redis 6.0.0.
+@history
+
+- `>= 3.0.0`: Added the `COPY` and `REPLACE` options.
+- `>= 3.0.6`: Added the `KEYS` option.
+- `>= 4.0.7`: Added the `AUTH` option.
+- `>= 6.0.0`: Added the `AUTH2` option.
 
 @return
 
 @simple-string-reply: The command returns OK on success, or `NOKEY` if no keys
 were found in the source instance.
```

### Comparing `iredis-1.9.3/iredis/data/commands/monitor.md` & `iredis-1.9.4/iredis/data/commands/monitor.md`

 * *Files 12% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 +1339518099.363765 [0 127.0.0.1:60866] "del" "x"
 +1339518100.544926 [0 127.0.0.1:60866] "get" "x"
 QUIT
 +OK
 Connection closed by foreign host.
 ```
 
-Manually issue the `QUIT` command to stop a `MONITOR` stream running via
-`telnet`.
+Manually issue the `QUIT` or `RESET` commands to stop a `MONITOR` stream running
+via `telnet`.
 
 ## Commands not logged by MONITOR
 
 Because of security concerns, all administrative commands are not logged by
 `MONITOR`'s output.
 
 Furthermore, the following commands are also not logged:
@@ -86,8 +86,9 @@
 @return
 
 **Non standard return value**, just dumps the received commands in an infinite
 flow.
 
 @history
 
-- `>=6.0`: `AUTH` excluded from the command's output.
+- `>= 6.2`: `RESET` can be called to exit monitor mode.
+- `>= 6.0`: `AUTH` excluded from the command's output.
```

### Comparing `iredis-1.9.3/iredis/data/commands/msetnx.md` & `iredis-1.9.4/iredis/data/commands/msetnx.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/object.md` & `iredis-1.9.4/iredis/data/commands/object.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/pfadd.md` & `iredis-1.9.4/iredis/data/commands/pfadd.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/pfcount.md` & `iredis-1.9.4/iredis/data/commands/pfcount.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/pfmerge.md` & `iredis-1.9.4/iredis/data/commands/pfmerge.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/ping.md` & `iredis-1.9.4/iredis/data/commands/ping.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/pttl.md` & `iredis-1.9.4/iredis/data/commands/pttl.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/pubsub.md` & `iredis-1.9.4/iredis/data/commands/pubsub.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 The PUBSUB command is an introspection command that allows to inspect the state
 of the Pub/Sub subsystem. It is composed of subcommands that are documented
 separately. The general form is:
 
     PUBSUB <subcommand> ... args ...
 
+Cluster note: in a Redis Cluster clients can subscribe to every node, and can
+also publish to every other node. The cluster will make sure that published
+messages are forwarded as needed. That said, `PUBSUB`'s replies in a cluster
+only report information from the node's Pub/Sub context, rather than the entire
+cluster.
+
 # PUBSUB CHANNELS [pattern]
 
 Lists the currently _active channels_. An active channel is a Pub/Sub channel
 with one or more subscribers (not including clients subscribed to patterns).
 
 If no `pattern` is specified, all the channels are listed, otherwise if pattern
 is specified only channels matching the specified glob-style pattern are listed.
```

### Comparing `iredis-1.9.3/iredis/data/commands/readonly.md` & `iredis-1.9.4/iredis/data/commands/readonly.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/rename.md` & `iredis-1.9.4/iredis/data/commands/rename.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/renamenx.md` & `iredis-1.9.4/iredis/data/commands/renamenx.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/replicaof.md` & `iredis-1.9.4/iredis/data/commands/replicaof.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/restore.md` & `iredis-1.9.4/iredis/data/commands/restore.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/role.md` & `iredis-1.9.4/iredis/data/commands/role.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/rpoplpush.md` & `iredis-1.9.4/iredis/data/commands/rpoplpush.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 `a,b` and `destination` holding `c,x,y,z`.
 
 If `source` does not exist, the value `nil` is returned and no operation is
 performed. If `source` and `destination` are the same, the operation is
 equivalent to removing the last element from the list and pushing it as first
 element of the list, so it can be considered as a list rotation command.
 
+As per Redis 6.2.0, RPOPLPUSH is considered deprecated. Please prefer `LMOVE` in
+new code.
+
 @return
 
 @bulk-string-reply: the element being popped and pushed.
 
 @examples
 
 ```cli
```

### Comparing `iredis-1.9.3/iredis/data/commands/rpush.md` & `iredis-1.9.4/iredis/data/commands/rpush.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/rpushx.md` & `iredis-1.9.4/iredis/data/commands/rpushx.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/sadd.md` & `iredis-1.9.4/iredis/data/commands/sadd.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 created before adding the specified members.
 
 An error is returned when the value stored at `key` is not a set.
 
 @return
 
 @integer-reply: the number of elements that were added to the set, not including
-all the elements already present into the set.
+all the elements already present in the set.
 
 @history
 
 - `>= 2.4`: Accepts multiple `member` arguments. Redis versions before 2.4 are
   only able to add a single member per call.
 
 @examples
```

### Comparing `iredis-1.9.3/iredis/data/commands/save.md` & `iredis-1.9.4/iredis/data/commands/save.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/scan.md` & `iredis-1.9.4/iredis/data/commands/scan.md`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 work the server has to do to complete a full iteration, and for rare types you
 may receive no elements in many iterations.
 
 ## Multiple parallel iterations
 
 It is possible for an infinite number of clients to iterate the same collection
 at the same time, as the full state of the iterator is in the cursor, that is
-obtained and returned to the client at every call. Server side no state is taken
+obtained and returned to the client at every call. No server side state is taken
 at all.
 
 ## Terminating iterations in the middle
 
 Since there is no state server side, but the full state is captured by the
 cursor, the caller is free to terminate an iteration half-way without signaling
 this to the server in any way. An infinite number of iterations can be started
```

### Comparing `iredis-1.9.3/iredis/data/commands/script-debug.md` & `iredis-1.9.4/iredis/data/commands/script-debug.md`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 block and all changes to the data are **rolled back** after the session
 finishes, so debugging can be restarted using the same initial state. The
 alternative synchronous debug mode blocks the server while the debugging session
 is active and retains all changes to the data set once it ends.
 
 - `YES`. Enable non-blocking asynchronous debugging of Lua scripts (changes are
   discarded).
-- `SYNC`. Enable blocking synchronous debugging of Lua scripts (saves changes to
-  data).
+- `!SYNC`. Enable blocking synchronous debugging of Lua scripts (saves changes
+  to data).
 - `NO`. Disables scripts debug mode.
 
 @return
 
 @simple-string-reply: `OK`.
```

### Comparing `iredis-1.9.3/iredis/data/commands/script-exists.md` & `iredis-1.9.4/iredis/data/commands/script-exists.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/script-kill.md` & `iredis-1.9.4/iredis/data/commands/script-kill.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/script-load.md` & `iredis-1.9.4/iredis/data/commands/script-load.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/select.md` & `iredis-1.9.4/iredis/data/commands/select.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/setbit.md` & `iredis-1.9.4/iredis/data/commands/setbit.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Sets or clears the bit at _offset_ in the string value stored at _key_.
 
-The bit is either set or cleared depending on _value_, which can be either 0
-or 1.
+The bit is either set or cleared depending on _value_, which can be either 0 or
+
+1.
 
 When _key_ does not exist, a new string value is created. The string is grown to
 make sure it can hold a bit at _offset_. The _offset_ argument is required to be
 greater than or equal to 0, and smaller than 2^32 (this limits bitmaps to
 512MB). When the string at _key_ is grown, added bits are set to 0.
 
 **Warning**: When setting the last possible bit (_offset_ equal to 2^32 -1) and
```

### Comparing `iredis-1.9.3/iredis/data/commands/setex.md` & `iredis-1.9.4/iredis/data/commands/setex.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/setnx.md` & `iredis-1.9.4/iredis/data/commands/setnx.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```
 
 ## Design pattern: Locking with `!SETNX`
 
 **Please note that:**
 
 1. The following pattern is discouraged in favor of
-   [the Redlock algorithm](http://redis.io/topics/distlock) which is only a bit
+   [the Redlock algorithm](https://redis.io/topics/distlock) which is only a bit
    more complex to implement, but offers better guarantees and is fault
    tolerant.
 2. We document the old pattern anyway because certain existing implementations
    link to this page as a reference. Moreover it is an interesting example of
    how Redis commands can be used in order to mount programming primitives.
 3. Anyway even assuming a single-instance locking primitive, starting with
    2.6.12 it is possible to create a much simpler locking primitive, equivalent
```

### Comparing `iredis-1.9.3/iredis/data/commands/setrange.md` & `iredis-1.9.4/iredis/data/commands/setrange.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/shutdown.md` & `iredis-1.9.4/iredis/data/commands/shutdown.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/sinter.md` & `iredis-1.9.4/iredis/data/commands/sinter.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/slaveof.md` & `iredis-1.9.4/iredis/data/commands/slaveof.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/slowlog.md` & `iredis-1.9.4/iredis/data/commands/slowlog.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 about the slow command executions. This makes the slow log remarkably fast at
 the point that you can enable the logging of all the commands (setting the
 _slowlog-log-slower-than_ config parameter to zero) with minor performance hit.
 
 To read the slow log the **SLOWLOG GET** command is used, that returns every
 entry in the slow log. It is possible to return only the N most recent entries
 passing an additional argument to the command (for instance **SLOWLOG GET 10**).
+The default requested length is 10 (when the argument is omitted). It's possible
+to pass -1 to get the entire slowlog.
 
 Note that you need a recent version of redis-cli in order to read the slow log
 output, since it uses some features of the protocol that were not formerly
 implemented in redis-cli (deeply nested multi bulk replies).
 
 ## Output format
```

### Comparing `iredis-1.9.3/iredis/data/commands/smove.md` & `iredis-1.9.4/iredis/data/commands/smove.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/sort.md` & `iredis-1.9.4/iredis/data/commands/sort.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/srandmember.md` & `iredis-1.9.4/iredis/data/commands/lmove.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,77 @@
-When called with just the `key` argument, return a random element from the set
-value stored at `key`.
+Atomically returns and removes the first/last element (head/tail depending on
+the `wherefrom` argument) of the list stored at `source`, and pushes the element
+at the first/last element (head/tail depending on the `whereto` argument) of the
+list stored at `destination`.
+
+For example: consider `source` holding the list `a,b,c`, and `destination`
+holding the list `x,y,z`. Executing `LMOVE source destination RIGHT LEFT`
+results in `source` holding `a,b` and `destination` holding `c,x,y,z`.
+
+If `source` does not exist, the value `nil` is returned and no operation is
+performed. If `source` and `destination` are the same, the operation is
+equivalent to removing the first/last element from the list and pushing it as
+first/last element of the list, so it can be considered as a list rotation
+command (or a no-op if `wherefrom` is the same as `whereto`).
 
-Starting from Redis version 2.6, when called with the additional `count`
-argument, return an array of `count` **distinct elements** if `count` is
-positive. If called with a negative `count` the behavior changes and the command
-is allowed to return the **same element multiple times**. In this case the
-number of returned elements is the absolute value of the specified `count`.
-
-When called with just the key argument, the operation is similar to `SPOP`,
-however while `SPOP` also removes the randomly selected element from the set,
-`SRANDMEMBER` will just return a random element without altering the original
-set in any way.
+This command comes in place of the now deprecated `RPOPLPUSH`. Doing
+`LMOVE RIGHT LEFT` is equivalent.
 
 @return
 
-@bulk-string-reply: without the additional `count` argument the command returns
-a Bulk Reply with the randomly selected element, or `nil` when `key` does not
-exist. @array-reply: when the additional `count` argument is passed the command
-returns an array of elements, or an empty array when `key` does not exist.
+@bulk-string-reply: the element being popped and pushed.
 
 @examples
 
 ```cli
-SADD myset one two three
-SRANDMEMBER myset
-SRANDMEMBER myset 2
-SRANDMEMBER myset -5
+RPUSH mylist "one"
+RPUSH mylist "two"
+RPUSH mylist "three"
+LMOVE mylist myotherlist RIGHT LEFT
+LMOVE mylist myotherlist LEFT RIGHT
+LRANGE mylist 0 -1
+LRANGE myotherlist 0 -1
 ```
 
-## Specification of the behavior when count is passed
+## Pattern: Reliable queue
 
-When a count argument is passed and is positive, the elements are returned as if
-every selected element is removed from the set (like the extraction of numbers
-in the game of Bingo). However elements are **not removed** from the Set. So
-basically:
-
-- No repeated elements are returned.
-- If count is bigger than the number of elements inside the Set, the command
-  will only return the whole set without additional elements.
-
-When instead the count is negative, the behavior changes and the extraction
-happens as if you put the extracted element inside the bag again after every
-extraction, so repeated elements are possible, and the number of elements
-requested is always returned as we can repeat the same elements again and again,
-with the exception of an empty Set (non existing key) that will always produce
-an empty array as a result.
-
-## Distribution of returned elements
-
-The distribution of the returned elements is far from perfect when the number of
-elements in the set is small, this is due to the fact that we used an
-approximated random element function that does not really guarantees good
-distribution.
-
-The algorithm used, that is implemented inside dict.c, samples the hash table
-buckets to find a non-empty one. Once a non empty bucket is found, since we use
-chaining in our hash table implementation, the number of elements inside the
-bucket is checked and a random element is selected.
-
-This means that if you have two non-empty buckets in the entire hash table, and
-one has three elements while one has just one, the element that is alone in its
-bucket will be returned with much higher probability.
+Redis is often used as a messaging server to implement processing of background
+jobs or other kinds of messaging tasks. A simple form of queue is often obtained
+pushing values into a list in the producer side, and waiting for this values in
+the consumer side using `RPOP` (using polling), or `BRPOP` if the client is
+better served by a blocking operation.
+
+However in this context the obtained queue is not _reliable_ as messages can be
+lost, for example in the case there is a network problem or if the consumer
+crashes just after the message is received but it is still to process.
+
+`LMOVE` (or `BLMOVE` for the blocking variant) offers a way to avoid this
+problem: the consumer fetches the message and at the same time pushes it into a
+_processing_ list. It will use the `LREM` command in order to remove the message
+from the _processing_ list once the message has been processed.
+
+An additional client may monitor the _processing_ list for items that remain
+there for too much time, and will push those timed out items into the queue
+again if needed.
+
+## Pattern: Circular list
+
+Using `LMOVE` with the same source and destination key, a client can visit all
+the elements of an N-elements list, one after the other, in O(N) without
+transferring the full list from the server to the client using a single `LRANGE`
+operation.
+
+The above pattern works even if the following two conditions:
+
+- There are multiple clients rotating the list: they'll fetch different
+  elements, until all the elements of the list are visited, and the process
+  restarts.
+- Even if other clients are actively pushing new items at the end of the list.
+
+The above makes it very simple to implement a system where a set of items must
+be processed by N workers continuously as fast as possible. An example is a
+monitoring system that must check that a set of web sites are reachable, with
+the smallest delay possible, using a number of parallel workers.
+
+Note that this implementation of workers is trivially scalable and reliable,
+because even if a message is lost the item is still in the queue and will be
+processed at the next iteration.
```

### Comparing `iredis-1.9.3/iredis/data/commands/srem.md` & `iredis-1.9.4/iredis/data/commands/srem.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/stralgo.md` & `iredis-1.9.4/iredis/data/commands/stralgo.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 The first argument of the command selects the algorithm to use, right now the
 argument must be "LCS", since this is the only implemented one.
 
 ## LCS algorithm
 
 ```
-STRALGO LCS [KEYS ...] [STRINGS ...] [LEN] [IDX] [MINMATCHLEN <len>] [WITHMATCHLEN]
+STRALGO LCS STRINGS <string_a> <string_b> | KEYS <key_a> <key_b> [LEN] [IDX] [MINMATCHLEN <len>] [WITHMATCHLEN]
 ```
 
 The LCS subcommand implements the longest common subsequence algorithm. Note
 that this is different than the longest common string algorithm, since matching
 characters in the string does not need to be contiguous.
 
 For instance the LCS between "foo" and "fao" is "fo", since scanning the two
@@ -109,13 +109,13 @@
 
 @return
 
 For the LCS algorithm:
 
 - Without modifiers the string representing the longest common substring is
   returned.
-- When LEN is given the command returns the length of the longest common
+- When `LEN` is given the command returns the length of the longest common
   substring.
-- When IDX is given the command returns an array with the LCS length and all the
-  ranges in both the strings, start and end offset for each string, where there
-  are matches. When WITHMATCHLEN is given each array representing a match will
-  also have the length of the match (see examples).
+- When `IDX` is given the command returns an array with the LCS length and all
+  the ranges in both the strings, start and end offset for each string, where
+  there are matches. When `WITHMATCHLEN` is given each array representing a
+  match will also have the length of the match (see examples).
```

### Comparing `iredis-1.9.3/iredis/data/commands/swapdb.md` & `iredis-1.9.4/iredis/data/commands/swapdb.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/ttl.md` & `iredis-1.9.4/iredis/data/commands/ttl.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/unlink.md` & `iredis-1.9.4/iredis/data/commands/unlink.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/wait.md` & `iredis-1.9.4/iredis/data/commands/wait.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/xack.md` & `iredis-1.9.4/iredis/data/commands/xack.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-The `XACK` command removes one or multiple messages from the _pending entries
-list_ (PEL) of a stream consumer group. A message is pending, and as such stored
+The `XACK` command removes one or multiple messages from the _Pending Entries
+List_ (PEL) of a stream consumer group. A message is pending, and as such stored
 inside the PEL, when it was delivered to some consumer, normally as a side
 effect of calling `XREADGROUP`, or when a consumer took ownership of a message
 calling `XCLAIM`. The pending message was delivered to some consumer but the
 server is yet not sure it was processed at least once. So new calls to
 `XREADGROUP` to grab the messages history for a consumer (for instance using an
 ID of 0), will return such message. Similarly the pending message will be listed
 by the `XPENDING` command, that inspects the PEL.
@@ -13,13 +13,17 @@
 entry about this message is also purged, releasing memory from the Redis server.
 
 @return
 
 @integer-reply, specifically:
 
 The command returns the number of messages successfully acknowledged. Certain
-message IDs may no longer be part of the PEL (for example because they have been
-already acknowledge), and XACK will not count them as successfully acknowledged.
+message IDs may no longer be part of the PEL (for example because they have
+already been acknowledged), and XACK will not count them as successfully
+acknowledged.
 
-```cli
-XACK mystream mygroup 1526569495631-0
+@examples
+
+```
+redis> XACK mystream mygroup 1526569495631-0
+(integer) 1
 ```
```

### Comparing `iredis-1.9.3/iredis/data/commands/xadd.md` & `iredis-1.9.4/iredis/data/commands/xadd.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Appends the specified stream entry to the stream at the specified key. If the
 key does not exist, as a side effect of running this command the key is created
-with a stream value.
+with a stream value. The creation of stream's key can be disabled with the
+`NOMKSTREAM` option.
 
 An entry is composed of a set of field-value pairs, it is basically a small
 dictionary. The field-value pairs are stored in the same order they are given by
 the user, and commands to read the stream such as `XRANGE` or `XREAD` are
 guaranteed to return the fields and values exactly in the same order they were
 added by `XADD`.
 
 `XADD` is the _only Redis command_ that can add data to a stream, but there are
 other commands, such as `XDEL` and `XTRIM`, that are able to remove data from a
 stream.
 
 ## Specifying a Stream ID as an argument
 
-A stream entry ID identifies a given entry inside a stream. The `XADD` command
-will auto-generate a unique ID for you if the ID argument specified is the `*`
-character (asterisk ASCII character). However, while useful only in very rare
-cases, it is possible to specify a well-formed ID, so that the new entry will be
-added exactly with the specified ID.
+A stream entry ID identifies a given entry inside a stream.
+
+The `XADD` command will auto-generate a unique ID for you if the ID argument
+specified is the `*` character (asterisk ASCII character). However, while useful
+only in very rare cases, it is possible to specify a well-formed ID, so that the
+new entry will be added exactly with the specified ID.
 
 IDs are specified by two numbers separated by a `-` character:
 
     1526919030474-55
 
 Both quantities are 64-bit numbers. When an ID is auto-generated, the first part
 is the Unix time in milliseconds of the Redis instance generating the ID. The
@@ -35,52 +37,57 @@
 ID in the stream has a time greater than the current local time of the instance,
 the top entry time will be used instead, and the sequence part of the ID
 incremented. This may happen when, for instance, the local clock jumps backward,
 or if after a failover the new master has a different absolute time.
 
 When a user specified an explicit ID to `XADD`, the minimum valid ID is `0-1`,
 and the user _must_ specify an ID which is greater than any other ID currently
-inside the stream, otherwise the command will fail. Usually resorting to
-specific IDs is useful only if you have another system generating unique IDs
-(for instance an SQL table) and you really want the Redis stream IDs to match
-the one of this other system.
+inside the stream, otherwise the command will fail and return an error. Usually
+resorting to specific IDs is useful only if you have another system generating
+unique IDs (for instance an SQL table) and you really want the Redis stream IDs
+to match the one of this other system.
 
 ## Capped streams
 
-It is possible to limit the size of the stream to a maximum number of elements
-using the **MAXLEN** option.
+`XADD` incorporates the same semantics as the `XTRIM` command - refer to its
+documentation page for more information. This allows adding new entries and
+keeping the stream's size in check with a single call to `XADD`, effectively
+capping the stream with an arbitrary threshold. Although exact trimming is
+possible and is the default, due to the internal representation of steams it is
+more efficient to add an entry and trim stream with `XADD` using **almost
+exact** trimming (the `~` argument).
 
-Trimming with **MAXLEN** can be expensive compared to just adding entries with
-`XADD`: streams are represented by macro nodes into a radix tree, in order to be
-very memory efficient. Altering the single macro node, consisting of a few tens
-of elements, is not optimal. So it is possible to give the command in the
-following special form:
+For example, calling `XADD` in the following form:
 
     XADD mystream MAXLEN ~ 1000 * ... entry fields here ...
 
-The `~` argument between the **MAXLEN** option and the actual count means that
-the user is not really requesting that the stream length is exactly 1000 items,
-but instead it could be a few tens of entries more, but never less than 1000
-items. When this option modifier is used, the trimming is performed only when
-Redis is able to remove a whole macro node. This makes it much more efficient,
-and it is usually what you want.
+Will add a new entry but will also evict old entries so that the stream will
+contain only 1000 entries, or at most a few tens more.
 
 ## Additional information about streams
 
 For further information about Redis streams please check our
 [introduction to Redis Streams document](/topics/streams-intro).
 
 @return
 
 @bulk-string-reply, specifically:
 
 The command returns the ID of the added entry. The ID is the one auto-generated
 if `*` is passed as ID argument, otherwise the command just returns the same ID
 specified by the user during insertion.
 
+The command returns a @nil-reply when used with the `NOMKSTREAM` option and the
+key doesn't exist.
+
+@history
+
+- `>= 6.2`: Added the `NOMKSTREAM` option, `MINID` trimming strategy and the
+  `LIMIT` option.
+
 @examples
 
 ```cli
 XADD mystream * name Sara surname OConnor
 XADD mystream * field1 value1 field2 value2 field3 value3
 XLEN mystream
 XRANGE mystream - +
```

### Comparing `iredis-1.9.3/iredis/data/commands/xclaim.md` & `iredis-1.9.4/iredis/data/commands/xclaim.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 In the context of a stream consumer group, this command changes the ownership of
 a pending message, so that the new owner is the consumer specified as the
 command argument. Normally this is what happens:
 
 1. There is a stream with an associated consumer group.
 2. Some consumer A reads a message via `XREADGROUP` from a stream, in the
    context of that consumer group.
-3. As a side effect a pending message entry is created in the pending entries
-   list (PEL) of the consumer group: it means the message was delivered to a
+3. As a side effect a pending message entry is created in the Pending Entries
+   List (PEL) of the consumer group: it means the message was delivered to a
    given consumer, but it was not yet acknowledged via `XACK`.
 4. Then suddenly that consumer fails forever.
 5. Other consumers may inspect the list of pending messages, that are stale for
    quite some time, using the `XPENDING` command. In order to continue
    processing such messages, they use `XCLAIM` to acquire the ownership of the
-   message and continue.
+   message and continue. As of Redis 6.2, consumers can use the `XAUTOCLAIM`
+   command to automatically scan and claim stale pending messages.
 
 This dynamic is clearly explained in the
 [Stream intro documentation](/topics/streams-intro).
 
 Note that the message is claimed only if its idle time is greater the minimum
 idle time we specify when calling `XCLAIM`. Because as a side effect `XCLAIM`
 will also reset the idle time (since this is a new attempt at processing the
@@ -64,15 +65,15 @@
 
 @array-reply, specifically:
 
 The command returns all the messages successfully claimed, in the same format as
 `XRANGE`. However if the `JUSTID` option was specified, only the message IDs are
 reported, without including the actual message.
 
-Example:
+@examples
 
 ```
 > XCLAIM mystream mygroup Alice 3600000 1526569498055-0
 1) 1) 1526569498055-0
    2) 1) "message"
       2) "orange"
 ```
```

### Comparing `iredis-1.9.3/iredis/data/commands/xdel.md` & `iredis-1.9.4/iredis/data/commands/xdel.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/xgroup.md` & `iredis-1.9.4/iredis/data/commands/xgroup.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,58 +7,75 @@
 - Set the consumer group _last delivered ID_ to something else.
 
 To create a new consumer group, use the following form:
 
     XGROUP CREATE mystream consumer-group-name $
 
 The last argument is the ID of the last item in the stream to consider already
-delivered. In the above case we used the special ID '\$' (that means: the ID of
+delivered. In the above case we used the special ID '$' (that means: the ID of
 the last item in the stream). In this case the consumers fetching data from that
 consumer group will only see new elements arriving in the stream.
 
 If instead you want consumers to fetch the whole stream history, use zero as the
 starting ID for the consumer group:
 
     XGROUP CREATE mystream consumer-group-name 0
 
 Of course it is also possible to use any other valid ID. If the specified
 consumer group already exists, the command returns a `-BUSYGROUP` error.
-Otherwise the operation is performed and OK is returned. There are no hard
-limits to the number of consumer groups you can associate to a given stream.
+Otherwise, the operation is performed and a @simple-string-reply `OK` is
+returned. There are no hard limits to the number of consumer groups you can
+associate with a given stream.
 
 If the specified stream doesn't exist when creating a group, an error will be
 returned. You can use the optional `MKSTREAM` subcommand as the last argument
 after the `ID` to automatically create the stream, if it doesn't exist. Note
 that if the stream is created in this way it will have a length of 0:
 
     XGROUP CREATE mystream consumer-group-name $ MKSTREAM
 
 A consumer group can be destroyed completely by using the following form:
 
     XGROUP DESTROY mystream consumer-group-name
 
 The consumer group will be destroyed even if there are active consumers and
 pending messages, so make sure to call this command only when really needed.
+This form returns an @integer-reply with the number of destroyed consumer groups
+(0 or 1).
+
+Consumers in a consumer group are auto-created every time a new consumer name is
+mentioned by some command. They can also be explicitly created by using the
+following form:
+
+    XGROUP CREATECONSUMER mystream consumer-group-name myconsumer123
+
+This form returns an @integer-reply with the number of created consumers (0 or
+1).
 
 To just remove a given consumer from a consumer group, the following form is
 used:
 
     XGROUP DELCONSUMER mystream consumer-group-name myconsumer123
 
-Consumers in a consumer group are auto-created every time a new consumer name is
-mentioned by some command. However sometimes it may be useful to remove old
-consumers since they are no longer used. This form returns the number of pending
-messages that the consumer had before it was deleted.
+Sometimes it may be useful to remove old consumers since they are no longer
+used. This form returns an @integer-reply with the number of pending messages
+that the consumer had before it was deleted.
 
 Finally it possible to set the next message to deliver using the `SETID`
 subcommand. Normally the next ID is set when the consumer is created, as the
 last argument of `XGROUP CREATE`. However using this form the next ID can be
 modified later without deleting and creating the consumer group again. For
 instance if you want the consumers in a consumer group to re-process all the
 messages in a stream, you may want to set its next ID to 0:
 
     XGROUP SETID mystream consumer-group-name 0
 
+This form returns a @simple-string-reply `OK` or an error.
+
 Finally to get some help if you don't remember the syntax, use the HELP
 subcommand:
 
     XGROUP HELP
+
+@history
+
+- `>= 6.2.0`: Supports the `CREATECONSUMER` subcommand.
```

### Comparing `iredis-1.9.3/iredis/data/commands/xinfo.md` & `iredis-1.9.4/iredis/data/commands/xinfo.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 same as the last entry ID in case some entry was deleted. Finally the full first
 and last entry in the stream are shown, in order to give some sense about what
 is the stream content.
 
 - `XINFO STREAM <key> FULL [COUNT <count>]`
 
 In this form the command returns the entire state of the stream, including
-entries, groups, consumers and PELs. This form is available since Redis 6.0.
+entries, groups, consumers and Pending Entries Lists (PELs). This form is
+available since Redis 6.0.
 
 ```
 > XADD mystream * foo bar
 "1588152471065-0"
 > XADD mystream * foo bar2
 "1588152473531-0"
 > XGROUP CREATE mystream mygroup 0-0
```

### Comparing `iredis-1.9.3/iredis/data/commands/xlen.md` & `iredis-1.9.4/iredis/data/commands/xlen.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/xpending.md` & `iredis-1.9.4/iredis/data/commands/xpending.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Fetching data from a stream via a consumer group, and not acknowledging such
 data, has the effect of creating _pending entries_. This is well explained in
 the `XREADGROUP` command, and even better in our
 [introduction to Redis Streams](/topics/streams-intro). The `XACK` command will
-immediately remove the pending entry from the Pending Entry List (PEL) since
+immediately remove the pending entry from the Pending Entries List (PEL) since
 once a message is successfully processed, there is no longer need for the
 consumer group to track it and to remember the current owner of the message.
 
 The `XPENDING` command is the interface to inspect the list of pending messages,
 and is as thus a very important command in order to observe and understand what
 is happening with a streams consumer groups: what clients are active, what
 messages are pending to be consumed, or to see if there are idle messages.
@@ -54,28 +54,31 @@
 ```
 
 In this form, the command outputs the total number of pending messages for this
 consumer group, which is one, followed by the smallest and greatest ID among the
 pending messages, and then list every consumer in the consumer group with at
 least one pending message, and the number of pending messages it has.
 
-This is a good overview, but sometimes we are interested in the details. In
-order to see all the pending messages with more associated information we need
-to also pass a range of IDs, in a similar way we do it with `XRANGE`, and a non
-optional _count_ argument, to limit the number of messages returned per call:
+## Extended form of XPENDING
+
+The summary provides a good overview, but sometimes we are interested in the
+details. In order to see all the pending messages with more associated
+information we need to also pass a range of IDs, in a similar way we do it with
+`XRANGE`, and a non optional _count_ argument, to limit the number of messages
+returned per call:
 
 ```
 > XPENDING mystream group55 - + 10
 1) 1) 1526984818136-0
    2) "consumer-123"
    3) (integer) 196415
    4) (integer) 1
 ```
 
-In the extended form we no longer see the summary information, instead there are
+In the extended form we no longer see the summary information, instead there is
 detailed information for each message in the pending entries list. For each
 message four attributes are returned:
 
 1. The ID of the message.
 2. The name of the consumer that fetched the message and has still to
    acknowledge it. We call it the current _owner_ of the message.
 3. The number of milliseconds that elapsed since the last time this message was
@@ -83,28 +86,55 @@
 4. The number of times this message was delivered.
 
 The deliveries counter, that is the fourth element in the array, is incremented
 when some other consumer _claims_ the message with `XCLAIM`, or when the message
 is delivered again via `XREADGROUP`, when accessing the history of a consumer in
 a consumer group (see the `XREADGROUP` page for more info).
 
-Finally it is possible to pass an additional argument to the command, in order
-to see the messages having a specific owner:
+It is possible to pass an additional argument to the command, in order to see
+the messages having a specific owner:
 
 ```
 > XPENDING mystream group55 - + 10 consumer-123
 ```
 
 But in the above case the output would be the same, since we have pending
 messages only for a single consumer. However what is important to keep in mind
 is that this operation, filtering by a specific consumer, is not inefficient
 even when there are many pending messages from many consumers: we have a pending
 entries list data structure both globally, and for every consumer, so we can
 very efficiently show just messages pending for a single consumer.
 
+## Idle time filter
+
+Since version 6.2 it is possible to filter entries by their idle-time, given in
+milliseconds (useful for `XCLAIM`ing entries that have not been processed for
+some time):
+
+```
+> XPENDING mystream group55 IDLE 9000 - + 10
+> XPENDING mystream group55 IDLE 9000 - + 10 consumer-123
+```
+
+The first case will return the first 10 (or less) PEL entries of the entire
+group that are idle for over 9 seconds, whereas in the second case only those of
+`consumer-123`.
+
+## Exclusive ranges and iterating the PEL
+
+The `XPENDING` command allows iterating over the pending entries just like
+`XRANGE` and `XREVRANGE` allow for the stream's entries. You can do this by
+prefixing the ID of the last-read pending entry with the `(` character that
+denotes an open (exclusive) range, and proving it to the subsequent call to the
+command.
+
 @return
 
 @array-reply, specifically:
 
 The command returns data in different format depending on the way it is called,
 as previously explained in this page. However the reply is always an array of
 items.
+
+@history
+
+- `>= 6.2.0`: Added the `IDLE` option and exclusive range intervals.
```

### Comparing `iredis-1.9.3/iredis/data/commands/xrange.md` & `iredis-1.9.4/iredis/data/commands/xrange.md`

 * *Files 18% similar despite different names*

```diff
@@ -63,14 +63,21 @@
 get all the entries within such millisecond, because the sequence number range
 will be from zero to the maximum.
 
 Used in this way `XRANGE` works as a range query command to obtain entries in a
 specified time. This is very handy in order to access the history of past events
 in a stream.
 
+## Exclusive ranges
+
+The range is close (inclusive) by default, meaning that the reply can include
+entries with IDs matching the query's start and end intervals. It is possible to
+specify an open interval (exclusive) by prefixing the ID with the character `(`.
+This is useful for iterating the stream, as explained below.
+
 ## Returning a maximum number of entries
 
 Using the **COUNT** option it is possible to reduce the number of entries
 reported. This is a very important feature even if it may look marginal, because
 it allows, for instance, to model operations such as _give me the entry greater
 or equal to the following_:
 
@@ -106,22 +113,22 @@
    2) 1) "name"
       2) "Jane"
       3) "surname"
       4) "Austen"
 ```
 
 Then instead of starting the iteration again from `-`, as the start of the range
-we use the entry ID of the _last_ entry returned by the previous `XRANGE` call,
-adding the sequence part of the ID by one.
+we use the entry ID of the _last_ entry returned by the previous `XRANGE` call
+as an exclusive interval.
 
-The ID of the last entry is `1526985685298-0`, so we just add 1 to the sequence
-to obtain `1526985685298-1`, and continue our iteration:
+The ID of the last entry is `1526985685298-0`, so we just prefix it with a '(',
+and continue our iteration:
 
 ```
-> XRANGE writers 1526985685298-1 + COUNT 2
+> XRANGE writers (1526985685298-0 + COUNT 2
 1) 1) 1526985691746-0
    2) 1) "name"
       2) "Toni"
       3) "surname"
       4) "Morrison"
 2) 1) 1526985712947-0
    2) 1) "name"
@@ -135,14 +142,45 @@
 by providing a given incomplete start ID. Moreover, we can limit the iteration
 to a given ID or time, by providing an end ID or incomplete ID instead of `+`.
 
 The command `XREAD` is also able to iterate the stream. The command `XREVRANGE`
 can iterate the stream reverse, from higher IDs (or times) to lower IDs (or
 times).
 
+### Iterating with earlier versions of Redis
+
+While exclusive range intervals are only available from Redis 6.2, it is still
+possible to use a similar stream iteration pattern with earlier versions. You
+start fetching from the stream the same way as described above to obtain the
+first entries.
+
+For the subsequent calls, you'll need to programmatically advance the last
+entry's ID returned. Most Redis client should abstract this detail, but the
+implementation can also be in the application if needed. In the example above,
+this means incrementing the sequence of `1526985685298-0` by one, from 0 to 1.
+The second call would, therefore, be:
+
+```
+> XRANGE writers 1526985685298-1 + COUNT 2
+1) 1) 1526985691746-0
+   2) 1) "name"
+      2) "Toni"
+...
+```
+
+Also, note that once the sequence part of the last ID equals
+18446744073709551615, you'll need to increment the timestamp and reset the
+sequence part to 0. For example, incrementing the ID
+`1526985685298-18446744073709551615` should result in `1526985685299-0`.
+
+A symmetrical pattern applies to iterating the stream with `XREVRANGE`. The only
+difference is that the client needs to decrement the ID for the subsequent
+calls. When decrementing an ID with a sequence part of 0, the timestamp needs to
+be decremented by 1 and the sequence set to 18446744073709551615.
+
 ## Fetching single items
 
 If you look for an `XGET` command you'll be disappointed because `XRANGE` is
 effectively the way to go in order to fetch a single entry from a stream. All
 you have to do is to specify the ID two times in the arguments of XRANGE:
 
 ```
@@ -166,14 +204,18 @@
 @array-reply, specifically:
 
 The command returns the entries with IDs matching the specified range. The
 returned entries are complete, that means that the ID and all the fields they
 are composed are returned. Moreover, the entries are returned with their fields
 and values in the exact same order as `XADD` added them.
 
+@history
+
+- `>= 6.2` Added exclusive ranges.
+
 @examples
 
 ```cli
 XADD writers * name Virginia surname Woolf
 XADD writers * name Jane surname Austen
 XADD writers * name Toni surname Morrison
 XADD writers * name Agatha surname Christie
```

### Comparing `iredis-1.9.3/iredis/data/commands/xread.md` & `iredis-1.9.4/iredis/data/commands/xread.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/xreadgroup.md` & `iredis-1.9.4/iredis/data/commands/xreadgroup.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 is just a string.
 
 One of the guarantees of consumer groups is that a given consumer can only see
 the history of messages that were delivered to it, so a message has just a
 single owner. However there is a special feature called _message claiming_ that
 allows other consumers to claim messages in case there is a non recoverable
 failure of some consumer. In order to implement such semantics, consumer groups
-require explicit acknowledgement of the messages successfully processed by the
+require explicit acknowledgment of the messages successfully processed by the
 consumer, via the `XACK` command. This is needed because the stream will track,
 for each consumer group, who is processing what message.
 
 This is how to understand if you want to use a consumer group or not:
 
 1. If you have a stream and multiple clients, and you want all the clients to
    get all the messages, you do not need a consumer group.
@@ -84,15 +84,15 @@
 no differences in this regard.
 
 ## What happens when a message is delivered to a consumer?
 
 Two things:
 
 1. If the message was never delivered to anyone, that is, if we are talking
-   about a new message, then a PEL (Pending Entry List) is created.
+   about a new message, then a PEL (Pending Entries List) is created.
 2. If instead the message was already delivered to this consumer, and it is just
    re-fetching the same message again, then the _last delivery counter_ is
    updated to the current time, and the _number of deliveries_ is incremented by
    one. You can access those message properties using the `XPENDING` command.
 
 ## Usage example
 
@@ -125,7 +125,23 @@
 remain in the pending entries list, so we can access our history by giving
 `XREADGROUP` initially an ID of 0, and performing the same loop. Once providing
 an ID of 0 the reply is an empty set of messages, we know that we processed and
 acknowledged all the pending messages: we can start to use `>` as ID, in order
 to get the new messages and rejoin the consumers that are processing new things.
 
 To see how the command actually replies, please check the `XREAD` command page.
+
+@return
+
+@array-reply, specifically:
+
+The command returns an array of results: each element of the returned array is
+an array composed of a two element containing the key name and the entries
+reported for that key. The entries reported are full stream entries, having IDs
+and the list of all the fields and values. Field and values are guaranteed to be
+reported in the same order they were added by `XADD`.
+
+When **BLOCK** is used, on timeout a null reply is returned.
+
+Reading the [Redis Streams introduction](/topics/streams-intro) is highly
+suggested in order to understand more about the streams overall behavior and
+semantics.
```

### Comparing `iredis-1.9.3/iredis/data/commands/zadd.md` & `iredis-1.9.4/iredis/data/commands/zadd.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,30 +6,36 @@
 If `key` does not exist, a new sorted set with the specified members as sole
 members is created, like if the sorted set was empty. If the key exists but does
 not hold a sorted set, an error is returned.
 
 The score values should be the string representation of a double precision
 floating point number. `+inf` and `-inf` values are valid values as well.
 
-## ZADD options (Redis 3.0.2 or greater)
+## ZADD options
 
 ZADD supports a list of options, specified after the name of the key and before
 the first score argument. Options are:
 
-- **XX**: Only update elements that already exist. Never add elements.
-- **NX**: Don't update already existing elements. Always add new elements.
+- **XX**: Only update elements that already exist. Don't add new elements.
+- **NX**: Only add new elements. Don't update already existing elements.
+- **LT**: Only update existing elements if the new score is **less than** the
+  current score. This flag doesn't prevent adding new elements.
+- **GT**: Only update existing elements if the new score is **greater than** the
+  current score. This flag doesn't prevent adding new elements.
 - **CH**: Modify the return value from the number of new elements added, to the
   total number of elements changed (CH is an abbreviation of _changed_). Changed
   elements are **new elements added** and elements already existing for which
   **the score was updated**. So elements specified in the command line having
   the same score as they had in the past are not counted. Note: normally the
   return value of `ZADD` only counts the number of new elements added.
 - **INCR**: When this option is specified `ZADD` acts like `ZINCRBY`. Only one
   score-element pair can be specified in this mode.
 
+Note: The **GT**, **LT** and **NX** options are mutually exclusive.
+
 ## Range of integer scores that can be expressed precisely
 
 Redis sorted sets use a _double 64-bit floating point number_ to represent the
 score. In all the architectures we support, this is represented as an **IEEE 754
 floating point number**, that is able to represent precisely integer numbers
 between `-(2^53)` and `+(2^53)` included. In more practical terms, all the
 integers between -9007199254740992 and 9007199254740992 are perfectly
@@ -70,27 +76,31 @@
 range queries on elements are possible using the command `ZRANGEBYLEX` (Note: it
 is also possible to query sorted sets by range of scores using `ZRANGEBYSCORE`).
 
 @return
 
 @integer-reply, specifically:
 
-- The number of elements added to the sorted set, not including elements already
-  existing for which the score was updated.
+- When used without optional arguments, the number of elements added to the
+  sorted set (excluding score updates).
+- If the `CH` option is specified, the number of elements that were changed
+  (added or updated).
 
 If the `INCR` option is specified, the return value will be @bulk-string-reply:
 
 - The new score of `member` (a double precision floating point number)
   represented as string, or `nil` if the operation was aborted (when called with
   either the `XX` or the `NX` option).
 
 @history
 
 - `>= 2.4`: Accepts multiple elements. In Redis versions older than 2.4 it was
   possible to add or update a single member per call.
+- `>= 3.0.2`: Added the `XX`, `NX`, `CH` and `INCR` options.
+- `>= 6.2`: Added the `GT` and `LT` options.
 
 @examples
 
 ```cli
 ZADD myzset 1 "one"
 ZADD myzset 1 "uno"
 ZADD myzset 2 "two" 3 "three"
```

### Comparing `iredis-1.9.3/iredis/data/commands/zcount.md` & `iredis-1.9.4/iredis/data/commands/zcount.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/zincrby.md` & `iredis-1.9.4/iredis/data/commands/zincrby.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/zinterstore.md` & `iredis-1.9.4/iredis/data/commands/zinterstore.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/zlexcount.md` & `iredis-1.9.4/iredis/data/commands/zlexcount.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/zpopmax.md` & `iredis-1.9.4/iredis/data/commands/zpopmax.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/zpopmin.md` & `iredis-1.9.4/iredis/data/commands/zpopmin.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/zrangebylex.md` & `iredis-1.9.4/iredis/data/commands/zrangebylex.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 If the elements in the sorted set have different scores, the returned elements
 are unspecified.
 
 The elements are considered to be ordered from lower to higher strings as
 compared byte-by-byte using the `memcmp()` C function. Longer strings are
 considered greater than shorter strings if the common part is identical.
 
+As per Redis 6.2.0, this command is considered deprecated. Please prefer using
+the `ZRANGE` command with the `BYLEX` argument in new code.
+
 The optional `LIMIT` argument can be used to only get a range of the matching
 elements (similar to _SELECT LIMIT offset, count_ in SQL). A negative `count`
 returns all elements from the `offset`. Keep in mind that if `offset` is large,
 the sorted set needs to be traversed for `offset` elements before getting to the
 elements to return, which can add up to O(N) time complexity.
 
 ## How to specify intervals
```

### Comparing `iredis-1.9.3/iredis/data/commands/zrangebyscore.md` & `iredis-1.9.4/iredis/data/commands/zrangebyscore.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 and `max` (including elements with score equal to `min` or `max`). The elements
 are considered to be ordered from low to high scores.
 
 The elements having the same score are returned in lexicographical order (this
 follows from a property of the sorted set implementation in Redis and does not
 involve further computation).
 
+As per Redis 6.2.0, this command is considered deprecated. Please prefer using
+the `ZRANGE` command with the `BYSCORE` argument in new code.
+
 The optional `LIMIT` argument can be used to only get a range of the matching
 elements (similar to _SELECT LIMIT offset, count_ in SQL). A negative `count`
 returns all elements from the `offset`. Keep in mind that if `offset` is large,
 the sorted set needs to be traversed for `offset` elements before getting to the
 elements to return, which can add up to O(N) time complexity.
 
 The optional `WITHSCORES` argument makes the command return both the element and
```

### Comparing `iredis-1.9.3/iredis/data/commands/zrank.md` & `iredis-1.9.4/iredis/data/commands/zrank.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/zrem.md` & `iredis-1.9.4/iredis/data/commands/zrem.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/zremrangebylex.md` & `iredis-1.9.4/iredis/data/commands/zremrangebylex.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 When all the elements in a sorted set are inserted with the same score, in order
 to force lexicographical ordering, this command removes all elements in the
 sorted set stored at `key` between the lexicographical range specified by `min`
 and `max`.
 
 The meaning of `min` and `max` are the same of the `ZRANGEBYLEX` command.
-Similarly, this command actually returns the same elements that `ZRANGEBYLEX`
+Similarly, this command actually removes the same elements that `ZRANGEBYLEX`
 would return if called with the same `min` and `max` arguments.
 
 @return
 
 @integer-reply: the number of elements removed.
 
 @examples
```

### Comparing `iredis-1.9.3/iredis/data/commands/zremrangebyrank.md` & `iredis-1.9.4/iredis/data/commands/zremrangebyrank.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/zrevrangebylex.md` & `iredis-1.9.4/iredis/data/commands/zrevrangebylex.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 When all the elements in a sorted set are inserted with the same score, in order
 to force lexicographical ordering, this command returns all the elements in the
 sorted set at `key` with a value between `max` and `min`.
 
 Apart from the reversed ordering, `ZREVRANGEBYLEX` is similar to `ZRANGEBYLEX`.
 
+As per Redis 6.2.0, this command is considered deprecated. Please prefer using
+the `ZRANGE` command with the `BYLEX` and `REV` arguments in new code.
+
 @return
 
 @array-reply: list of elements in the specified score range.
 
 @examples
 
 ```cli
```

### Comparing `iredis-1.9.3/iredis/data/commands/zrevrangebyscore.md` & `iredis-1.9.4/iredis/data/commands/zrevrangebyscore.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 The elements having the same score are returned in reverse lexicographical
 order.
 
 Apart from the reversed ordering, `ZREVRANGEBYSCORE` is similar to
 `ZRANGEBYSCORE`.
 
+As per Redis 6.2.0, this command is considered deprecated. Please prefer using
+the `ZRANGE` command with the `BYSCORE` and `REV` arguments in new code.
+
 @return
 
 @array-reply: list of elements in the specified score range (optionally with
 their scores).
 
 @examples
```

### Comparing `iredis-1.9.3/iredis/data/commands/zrevrank.md` & `iredis-1.9.4/iredis/data/commands/zrevrank.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands/zunionstore.md` & `iredis-1.9.4/iredis/data/commands/zunionstore.md`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/commands.json` & `iredis-1.9.4/iredis/data/commands.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8910991892610315%*

 * *Differences: {"'ACL GETUSER'": "OrderedDict([('summary', 'Get the rules for a specific ACL user'), "*

 * *                  "('complexity', 'O(N). Where N is the number of password, command and pattern "*

 * *                  "rules that the user has.'), ('arguments', [OrderedDict([('name', 'username'), "*

 * *                  "('type', 'string')])]), ('since', '6.0.0'), ('group', 'server')])",*

 * * "'ACL HELP'": "OrderedDict([('summary', 'Show helpful text about the different subcommands'), "*

 * *               "('complexity', 'O(1)'), ('s […]*

```diff
@@ -34,14 +34,32 @@
             }
         ],
         "complexity": "O(1)",
         "group": "server",
         "since": "6.0.0",
         "summary": "Generate a pseudorandom secure password to use for ACL users"
     },
+    "ACL GETUSER": {
+        "arguments": [
+            {
+                "name": "username",
+                "type": "string"
+            }
+        ],
+        "complexity": "O(N). Where N is the number of password, command and pattern rules that the user has.",
+        "group": "server",
+        "since": "6.0.0",
+        "summary": "Get the rules for a specific ACL user"
+    },
+    "ACL HELP": {
+        "complexity": "O(1)",
+        "group": "server",
+        "since": "6.0.0",
+        "summary": "Show helpful text about the different subcommands"
+    },
     "ACL LIST": {
         "complexity": "O(N). Where N is the number of configured users.",
         "group": "server",
         "since": "6.0.0",
         "summary": "List the current ACL rules in ACL config file format"
     },
     "ACL LOAD": {
@@ -68,16 +86,21 @@
         "group": "server",
         "since": "6.0.0",
         "summary": "Save the current ACL rules in the configured ACL file"
     },
     "ACL SETUSER": {
         "arguments": [
             {
+                "name": "username",
+                "type": "string"
+            },
+            {
                 "multiple": true,
                 "name": "rule",
+                "optional": true,
                 "type": "string"
             }
         ],
         "complexity": "O(N). Where N is the number of rules provided.",
         "group": "server",
         "since": "6.0.0",
         "summary": "Modify or create the rules for a specific ACL user"
@@ -109,14 +132,19 @@
         "group": "string",
         "since": "2.0.0",
         "summary": "Append a value to a key"
     },
     "AUTH": {
         "arguments": [
             {
+                "name": "username",
+                "optional": true,
+                "type": "string"
+            },
+            {
                 "name": "password",
                 "type": "string"
             }
         ],
         "group": "connection",
         "since": "1.0.0",
         "summary": "Authenticate to the server"
@@ -156,15 +184,15 @@
                 "type": [
                     "integer",
                     "integer"
                 ]
             }
         ],
         "complexity": "O(N)",
-        "group": "string",
+        "group": "bitmap",
         "since": "2.6.0",
         "summary": "Count set bits in a string"
     },
     "BITFIELD": {
         "arguments": [
             {
                 "name": "key",
@@ -218,15 +246,15 @@
                     "FAIL"
                 ],
                 "optional": true,
                 "type": "enum"
             }
         ],
         "complexity": "O(1) for each subcommand specified",
-        "group": "string",
+        "group": "bitmap",
         "since": "3.2.0",
         "summary": "Perform arbitrary bitfield integer operations on strings"
     },
     "BITOP": {
         "arguments": [
             {
                 "name": "operation",
@@ -239,74 +267,116 @@
             {
                 "multiple": true,
                 "name": "key",
                 "type": "key"
             }
         ],
         "complexity": "O(N)",
-        "group": "string",
+        "group": "bitmap",
         "since": "2.6.0",
         "summary": "Perform bitwise operations between strings"
     },
     "BITPOS": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
                 "name": "bit",
                 "type": "integer"
             },
             {
-                "name": "start",
-                "optional": true,
-                "type": "integer"
-            },
-            {
-                "name": "end",
+                "block": [
+                    {
+                        "name": "start",
+                        "type": "integer"
+                    },
+                    {
+                        "name": "end",
+                        "optional": true,
+                        "type": "integer"
+                    }
+                ],
+                "name": "index",
                 "optional": true,
-                "type": "integer"
+                "type": "block"
             }
         ],
         "complexity": "O(N)",
-        "group": "string",
+        "group": "bitmap",
         "since": "2.8.7",
         "summary": "Find first bit set or clear in a string"
     },
+    "BLMOVE": {
+        "arguments": [
+            {
+                "name": "source",
+                "type": "key"
+            },
+            {
+                "name": "destination",
+                "type": "key"
+            },
+            {
+                "enum": [
+                    "LEFT",
+                    "RIGHT"
+                ],
+                "name": "wherefrom",
+                "type": "enum"
+            },
+            {
+                "enum": [
+                    "LEFT",
+                    "RIGHT"
+                ],
+                "name": "whereto",
+                "type": "enum"
+            },
+            {
+                "name": "timeout",
+                "type": "double"
+            }
+        ],
+        "complexity": "O(1)",
+        "group": "list",
+        "since": "6.2.0",
+        "summary": "Pop an element from a list, push it to another list and return it; or block until one is available"
+    },
     "BLPOP": {
         "arguments": [
             {
                 "multiple": true,
                 "name": "key",
                 "type": "key"
             },
             {
                 "name": "timeout",
-                "type": "integer"
+                "type": "double"
             }
         ],
-        "complexity": "O(1)",
+        "complexity": "O(N) where N is the number of provided keys.",
         "group": "list",
         "since": "2.0.0",
         "summary": "Remove and get the first element in a list, or block until one is available"
     },
     "BRPOP": {
         "arguments": [
             {
                 "multiple": true,
                 "name": "key",
                 "type": "key"
             },
             {
                 "name": "timeout",
-                "type": "integer"
+                "type": "double"
             }
         ],
-        "complexity": "O(1)",
+        "complexity": "O(N) where N is the number of provided keys.",
         "group": "list",
         "since": "2.0.0",
         "summary": "Remove and get the last element in a list, or block until one is available"
     },
     "BRPOPLPUSH": {
         "arguments": [
             {
@@ -315,15 +385,15 @@
             },
             {
                 "name": "destination",
                 "type": "key"
             },
             {
                 "name": "timeout",
-                "type": "integer"
+                "type": "double"
             }
         ],
         "complexity": "O(1)",
         "group": "list",
         "since": "2.2.0",
         "summary": "Pop an element from a list, push it to another list and return it; or block until one is available"
     },
@@ -332,15 +402,15 @@
             {
                 "multiple": true,
                 "name": "key",
                 "type": "key"
             },
             {
                 "name": "timeout",
-                "type": "integer"
+                "type": "double"
             }
         ],
         "complexity": "O(log(N)) with N being the number of elements in the sorted set.",
         "group": "sorted_set",
         "since": "5.0.0",
         "summary": "Remove and return the member with the highest score from one or more sorted sets, or block until one is available"
     },
@@ -349,15 +419,15 @@
             {
                 "multiple": true,
                 "name": "key",
                 "type": "key"
             },
             {
                 "name": "timeout",
-                "type": "integer"
+                "type": "double"
             }
         ],
         "complexity": "O(log(N)) with N being the number of elements in the sorted set.",
         "group": "sorted_set",
         "since": "5.0.0",
         "summary": "Remove and return the member with the lowest score from one or more sorted sets, or block until one is available"
     },
@@ -391,14 +461,20 @@
     },
     "CLIENT ID": {
         "complexity": "O(1)",
         "group": "connection",
         "since": "5.0.0",
         "summary": "Returns the client ID for the current connection"
     },
+    "CLIENT INFO": {
+        "complexity": "O(1)",
+        "group": "connection",
+        "since": "6.2.0",
+        "summary": "Returns information about the current client connection."
+    },
     "CLIENT KILL": {
         "arguments": [
             {
                 "name": "ip:port",
                 "optional": true,
                 "type": "string"
             },
@@ -416,20 +492,32 @@
                     "slave",
                     "pubsub"
                 ],
                 "optional": true,
                 "type": "enum"
             },
             {
+                "command": "USER",
+                "name": "username",
+                "optional": true,
+                "type": "string"
+            },
+            {
                 "command": "ADDR",
                 "name": "ip:port",
                 "optional": true,
                 "type": "string"
             },
             {
+                "command": "LADDR",
+                "name": "ip:port",
+                "optional": true,
+                "type": "string"
+            },
+            {
                 "command": "SKIPME",
                 "name": "yes/no",
                 "optional": true,
                 "type": "string"
             }
         ],
         "complexity": "O(N) where N is the number of client connections",
@@ -445,26 +533,50 @@
                     "normal",
                     "master",
                     "replica",
                     "pubsub"
                 ],
                 "optional": true,
                 "type": "enum"
+            },
+            {
+                "block": [
+                    {
+                        "command": "ID"
+                    },
+                    {
+                        "multiple": true,
+                        "name": "client-id",
+                        "type": "integer"
+                    }
+                ],
+                "name": "id",
+                "optional": true,
+                "type": "block"
             }
         ],
         "complexity": "O(N) where N is the number of client connections",
         "group": "connection",
         "since": "2.4.0",
         "summary": "Get the list of client connections"
     },
     "CLIENT PAUSE": {
         "arguments": [
             {
                 "name": "timeout",
                 "type": "integer"
+            },
+            {
+                "enum": [
+                    "WRITE",
+                    "ALL"
+                ],
+                "name": "mode",
+                "optional": true,
+                "type": "enum"
             }
         ],
         "complexity": "O(1)",
         "group": "connection",
         "since": "2.9.50",
         "summary": "Stop processing commands from clients for some time"
     },
@@ -478,15 +590,15 @@
                 ],
                 "name": "reply-mode",
                 "type": "enum"
             }
         ],
         "complexity": "O(1)",
         "group": "connection",
-        "since": "3.2",
+        "since": "3.2.0",
         "summary": "Instruct the server whether to reply to commands"
     },
     "CLIENT SETNAME": {
         "arguments": [
             {
                 "name": "connection-name",
                 "type": "string"
@@ -511,17 +623,18 @@
                 "command": "REDIRECT",
                 "name": "client-id",
                 "optional": true,
                 "type": "integer"
             },
             {
                 "command": "PREFIX",
+                "multiple": true,
                 "name": "prefix",
                 "optional": true,
-                "type": "srting"
+                "type": "string"
             },
             {
                 "enum": [
                     "BCAST"
                 ],
                 "name": "BCAST",
                 "optional": true,
@@ -548,19 +661,25 @@
                     "NOLOOP"
                 ],
                 "name": "NOLOOP",
                 "optional": true,
                 "type": "enum"
             }
         ],
-        "complexity": "O(1)",
+        "complexity": "O(1). Some options may introduce additional complexity.",
         "group": "connection",
         "since": "6.0.0",
         "summary": "Enable or disable server assisted client side caching support"
     },
+    "CLIENT TRACKINGINFO": {
+        "complexity": "O(1)",
+        "group": "connection",
+        "since": "6.2.0",
+        "summary": "Return information about server assisted client side caching for the current connection"
+    },
     "CLIENT UNBLOCK": {
         "arguments": [
             {
                 "name": "client-id",
                 "type": "integer"
             },
             {
@@ -574,14 +693,20 @@
             }
         ],
         "complexity": "O(log N) where N is the number of client connections",
         "group": "connection",
         "since": "5.0.0",
         "summary": "Unblock a client blocked in a blocking command from a different connection"
     },
+    "CLIENT UNPAUSE": {
+        "complexity": "O(N) Where N is the number of paused clients",
+        "group": "connection",
+        "since": "6.2.0",
+        "summary": "Resume processing of clients that were paused"
+    },
     "CLUSTER ADDSLOTS": {
         "arguments": [
             {
                 "multiple": true,
                 "name": "slot",
                 "type": "integer"
             }
@@ -899,14 +1024,44 @@
                 "type": "string"
             }
         ],
         "group": "server",
         "since": "2.0.0",
         "summary": "Set a configuration parameter to the given value"
     },
+    "COPY": {
+        "arguments": [
+            {
+                "name": "source",
+                "type": "key"
+            },
+            {
+                "name": "destination",
+                "type": "key"
+            },
+            {
+                "command": "DB",
+                "name": "destination-db",
+                "optional": true,
+                "type": "integer"
+            },
+            {
+                "enum": [
+                    "REPLACE"
+                ],
+                "name": "replace",
+                "optional": true,
+                "type": "enum"
+            }
+        ],
+        "complexity": "O(N) worst case for collections, where N is the number of nested items. O(1) for string values.",
+        "group": "generic",
+        "since": "6.2.0",
+        "summary": "Copy a key"
+    },
     "DBSIZE": {
         "group": "server",
         "since": "1.0.0",
         "summary": "Return the number of keys in the selected database"
     },
     "DEBUG OBJECT": {
         "arguments": [
@@ -973,15 +1128,15 @@
     "DUMP": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             }
         ],
-        "complexity": "O(1) to access the key and additional O(N*M) to serialized it, where N is the number of Redis objects composing the value and M their average size. For small string values the time complexity is thus O(1)+O(1*M) where M is small, so simply O(1).",
+        "complexity": "O(1) to access the key and additional O(N*M) to serialize it, where N is the number of Redis objects composing the value and M their average size. For small string values the time complexity is thus O(1)+O(1*M) where M is small, so simply O(1).",
         "group": "generic",
         "since": "2.6.0",
         "summary": "Return a serialized version of the value stored at the specified key."
     },
     "ECHO": {
         "arguments": [
             {
@@ -1002,19 +1157,21 @@
             {
                 "name": "numkeys",
                 "type": "integer"
             },
             {
                 "multiple": true,
                 "name": "key",
+                "optional": true,
                 "type": "key"
             },
             {
                 "multiple": true,
                 "name": "arg",
+                "optional": true,
                 "type": "string"
             }
         ],
         "complexity": "Depends on the script that is executed.",
         "group": "scripting",
         "since": "2.6.0",
         "summary": "Execute a Lua script server side"
@@ -1028,41 +1185,95 @@
             {
                 "name": "numkeys",
                 "type": "integer"
             },
             {
                 "multiple": true,
                 "name": "key",
+                "optional": true,
                 "type": "key"
             },
             {
                 "multiple": true,
                 "name": "arg",
+                "optional": true,
                 "type": "string"
             }
         ],
         "complexity": "Depends on the script that is executed.",
         "group": "scripting",
         "since": "2.6.0",
         "summary": "Execute a Lua script server side"
     },
+    "EVALSHA_RO": {
+        "arguments": [
+            {
+                "name": "sha1",
+                "type": "string"
+            },
+            {
+                "name": "numkeys",
+                "type": "integer"
+            },
+            {
+                "multiple": true,
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "multiple": true,
+                "name": "arg",
+                "type": "string"
+            }
+        ],
+        "complexity": "Depends on the script that is executed.",
+        "group": "scripting",
+        "since": "7.0.0",
+        "summary": "Execute a read-only Lua script server side"
+    },
+    "EVAL_RO": {
+        "arguments": [
+            {
+                "name": "script",
+                "type": "string"
+            },
+            {
+                "name": "numkeys",
+                "type": "integer"
+            },
+            {
+                "multiple": true,
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "multiple": true,
+                "name": "arg",
+                "type": "string"
+            }
+        ],
+        "complexity": "Depends on the script that is executed.",
+        "group": "scripting",
+        "since": "7.0.0",
+        "summary": "Execute a read-only Lua script server side"
+    },
     "EXEC": {
         "group": "transactions",
         "since": "1.2.0",
         "summary": "Execute all commands issued after MULTI"
     },
     "EXISTS": {
         "arguments": [
             {
                 "multiple": true,
                 "name": "key",
                 "type": "key"
             }
         ],
-        "complexity": "O(1)",
+        "complexity": "O(N) where N is the number of keys to check.",
         "group": "generic",
         "since": "1.0.0",
         "summary": "Determine if a key exists"
     },
     "EXPIRE": {
         "arguments": [
             {
@@ -1091,51 +1302,123 @@
             }
         ],
         "complexity": "O(1)",
         "group": "generic",
         "since": "1.2.0",
         "summary": "Set the expiration for a key as a UNIX timestamp"
     },
+    "EXPIRETIME": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            }
+        ],
+        "complexity": "O(1)",
+        "group": "generic",
+        "since": "7.0.0",
+        "summary": "Get the expiration Unix timestamp for a key"
+    },
+    "FAILOVER": {
+        "arguments": [
+            {
+                "block": [
+                    {
+                        "command": "TO"
+                    },
+                    {
+                        "name": "host",
+                        "type": "string"
+                    },
+                    {
+                        "name": "port",
+                        "type": "integer"
+                    },
+                    {
+                        "command": "FORCE",
+                        "optional": true
+                    }
+                ],
+                "name": "target",
+                "optional": true,
+                "type": "block"
+            },
+            {
+                "command": "ABORT",
+                "optional": true
+            },
+            {
+                "command": "TIMEOUT",
+                "name": "milliseconds",
+                "optional": true,
+                "type": "integer"
+            }
+        ],
+        "group": "server",
+        "since": "6.2.0",
+        "summary": "Start a coordinated failover between this server and one of its replicas."
+    },
     "FLUSHALL": {
         "arguments": [
             {
                 "enum": [
-                    "ASYNC"
+                    "ASYNC",
+                    "SYNC"
                 ],
                 "name": "async",
                 "optional": true,
                 "type": "enum"
             }
         ],
+        "complexity": "O(N) where N is the total number of keys in all databases",
         "group": "server",
         "since": "1.0.0",
         "summary": "Remove all keys from all databases"
     },
     "FLUSHDB": {
         "arguments": [
             {
                 "enum": [
-                    "ASYNC"
+                    "ASYNC",
+                    "SYNC"
                 ],
                 "name": "async",
                 "optional": true,
                 "type": "enum"
             }
         ],
+        "complexity": "O(N) where N is the number of keys in the selected database",
         "group": "server",
         "since": "1.0.0",
         "summary": "Remove all keys from the current database"
     },
     "GEOADD": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
+                "enum": [
+                    "NX",
+                    "XX"
+                ],
+                "name": "condition",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "enum": [
+                    "CH"
+                ],
+                "name": "change",
+                "optional": true,
+                "type": "enum"
+            },
+            {
                 "multiple": true,
                 "name": [
                     "longitude",
                     "latitude",
                     "member"
                 ],
                 "type": [
@@ -1206,15 +1489,15 @@
             },
             {
                 "multiple": true,
                 "name": "member",
                 "type": "string"
             }
         ],
-        "complexity": "O(log(N)) for each member requested, where N is the number of elements in the sorted set.",
+        "complexity": "O(N) where N is the number of members requested.",
         "group": "geo",
         "since": "3.2.0",
         "summary": "Returns longitude and latitude of members of a geospatial index"
     },
     "GEORADIUS": {
         "arguments": [
             {
@@ -1264,18 +1547,32 @@
                     "WITHHASH"
                 ],
                 "name": "withhash",
                 "optional": true,
                 "type": "enum"
             },
             {
-                "command": "COUNT",
+                "block": [
+                    {
+                        "command": "COUNT",
+                        "name": "count",
+                        "type": "integer"
+                    },
+                    {
+                        "enum": [
+                            "ANY"
+                        ],
+                        "name": "any",
+                        "optional": true,
+                        "type": "enum"
+                    }
+                ],
                 "name": "count",
                 "optional": true,
-                "type": "integer"
+                "type": "block"
             },
             {
                 "enum": [
                     "ASC",
                     "DESC"
                 ],
                 "name": "order",
@@ -1345,18 +1642,32 @@
                     "WITHHASH"
                 ],
                 "name": "withhash",
                 "optional": true,
                 "type": "enum"
             },
             {
-                "command": "COUNT",
+                "block": [
+                    {
+                        "command": "COUNT",
+                        "name": "count",
+                        "type": "integer"
+                    },
+                    {
+                        "enum": [
+                            "ANY"
+                        ],
+                        "name": "any",
+                        "optional": true,
+                        "type": "enum"
+                    }
+                ],
                 "name": "count",
                 "optional": true,
-                "type": "integer"
+                "type": "block"
             },
             {
                 "enum": [
                     "ASC",
                     "DESC"
                 ],
                 "name": "order",
@@ -1377,14 +1688,264 @@
             }
         ],
         "complexity": "O(N+log(M)) where N is the number of elements inside the bounding box of the circular area delimited by center and radius and M is the number of items inside the index.",
         "group": "geo",
         "since": "3.2.0",
         "summary": "Query a sorted set representing a geospatial index to fetch members matching a given maximum distance from a member"
     },
+    "GEOSEARCH": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "command": "FROMMEMBER",
+                "name": "member",
+                "optional": true,
+                "type": "string"
+            },
+            {
+                "command": "FROMLONLAT",
+                "name": [
+                    "longitude",
+                    "latitude"
+                ],
+                "optional": true,
+                "type": [
+                    "double",
+                    "double"
+                ]
+            },
+            {
+                "block": [
+                    {
+                        "command": "BYRADIUS",
+                        "name": "radius",
+                        "type": "double"
+                    },
+                    {
+                        "enum": [
+                            "m",
+                            "km",
+                            "ft",
+                            "mi"
+                        ],
+                        "name": "unit",
+                        "type": "enum"
+                    }
+                ],
+                "name": "circle",
+                "optional": true,
+                "type": "block"
+            },
+            {
+                "block": [
+                    {
+                        "command": "BYBOX",
+                        "name": "width",
+                        "type": "double"
+                    },
+                    {
+                        "name": "height",
+                        "type": "double"
+                    },
+                    {
+                        "enum": [
+                            "m",
+                            "km",
+                            "ft",
+                            "mi"
+                        ],
+                        "name": "unit",
+                        "type": "enum"
+                    }
+                ],
+                "name": "box",
+                "optional": true,
+                "type": "block"
+            },
+            {
+                "enum": [
+                    "ASC",
+                    "DESC"
+                ],
+                "name": "order",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "block": [
+                    {
+                        "command": "COUNT",
+                        "name": "count",
+                        "type": "integer"
+                    },
+                    {
+                        "enum": [
+                            "ANY"
+                        ],
+                        "name": "any",
+                        "optional": true,
+                        "type": "enum"
+                    }
+                ],
+                "name": "count",
+                "optional": true,
+                "type": "block"
+            },
+            {
+                "enum": [
+                    "WITHCOORD"
+                ],
+                "name": "withcoord",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "enum": [
+                    "WITHDIST"
+                ],
+                "name": "withdist",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "enum": [
+                    "WITHHASH"
+                ],
+                "name": "withhash",
+                "optional": true,
+                "type": "enum"
+            }
+        ],
+        "complexity": "O(N+log(M)) where N is the number of elements in the grid-aligned bounding box area around the shape provided as the filter and M is the number of items inside the shape",
+        "group": "geo",
+        "since": "6.2",
+        "summary": "Query a sorted set representing a geospatial index to fetch members inside an area of a box or a circle."
+    },
+    "GEOSEARCHSTORE": {
+        "arguments": [
+            {
+                "name": "destination",
+                "type": "key"
+            },
+            {
+                "name": "source",
+                "type": "key"
+            },
+            {
+                "command": "FROMMEMBER",
+                "name": "member",
+                "optional": true,
+                "type": "string"
+            },
+            {
+                "command": "FROMLONLAT",
+                "name": [
+                    "longitude",
+                    "latitude"
+                ],
+                "optional": true,
+                "type": [
+                    "double",
+                    "double"
+                ]
+            },
+            {
+                "block": [
+                    {
+                        "command": "BYRADIUS",
+                        "name": "radius",
+                        "type": "double"
+                    },
+                    {
+                        "enum": [
+                            "m",
+                            "km",
+                            "ft",
+                            "mi"
+                        ],
+                        "name": "unit",
+                        "type": "enum"
+                    }
+                ],
+                "name": "circle",
+                "optional": true,
+                "type": "block"
+            },
+            {
+                "block": [
+                    {
+                        "command": "BYBOX",
+                        "name": "width",
+                        "type": "double"
+                    },
+                    {
+                        "name": "height",
+                        "type": "double"
+                    },
+                    {
+                        "enum": [
+                            "m",
+                            "km",
+                            "ft",
+                            "mi"
+                        ],
+                        "name": "unit",
+                        "type": "enum"
+                    }
+                ],
+                "name": "box",
+                "optional": true,
+                "type": "block"
+            },
+            {
+                "enum": [
+                    "ASC",
+                    "DESC"
+                ],
+                "name": "order",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "block": [
+                    {
+                        "command": "COUNT",
+                        "name": "count",
+                        "type": "integer"
+                    },
+                    {
+                        "enum": [
+                            "ANY"
+                        ],
+                        "name": "any",
+                        "optional": true,
+                        "type": "enum"
+                    }
+                ],
+                "name": "count",
+                "optional": true,
+                "type": "block"
+            },
+            {
+                "enum": [
+                    "STOREDIST"
+                ],
+                "name": "storedist",
+                "optional": true,
+                "type": "enum"
+            }
+        ],
+        "complexity": "O(N+log(M)) where N is the number of elements in the grid-aligned bounding box area around the shape provided as the filter and M is the number of items inside the shape",
+        "group": "geo",
+        "since": "6.2",
+        "summary": "Query a sorted set representing a geospatial index to fetch members inside an area of a box or a circle, and store the result in another key."
+    },
     "GET": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             }
         ],
@@ -1401,18 +1962,54 @@
             },
             {
                 "name": "offset",
                 "type": "integer"
             }
         ],
         "complexity": "O(1)",
-        "group": "string",
+        "group": "bitmap",
         "since": "2.2.0",
         "summary": "Returns the bit value at offset in the string value stored at key"
     },
+    "GETDEL": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            }
+        ],
+        "complexity": "O(1)",
+        "group": "string",
+        "since": "6.2.0",
+        "summary": "Get the value of a key and delete the key"
+    },
+    "GETEX": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "enum": [
+                    "EX seconds",
+                    "PX milliseconds",
+                    "EXAT timestamp",
+                    "PXAT milliseconds-timestamp",
+                    "PERSIST"
+                ],
+                "name": "expiration",
+                "optional": true,
+                "type": "enum"
+            }
+        ],
+        "complexity": "O(1)",
+        "group": "string",
+        "since": "6.2.0",
+        "summary": "Get the value of a key and optionally set its expiration"
+    },
     "GETRANGE": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
@@ -1461,40 +2058,47 @@
         "group": "hash",
         "since": "2.0.0",
         "summary": "Delete one or more hash fields"
     },
     "HELLO": {
         "arguments": [
             {
-                "name": "protover",
-                "type": "integer"
-            },
-            {
-                "command": "AUTH",
-                "name": [
-                    "username",
-                    "password"
+                "block": [
+                    {
+                        "name": "protover",
+                        "type": "integer"
+                    },
+                    {
+                        "command": "AUTH",
+                        "name": [
+                            "username",
+                            "password"
+                        ],
+                        "optional": true,
+                        "type": [
+                            "string",
+                            "string"
+                        ]
+                    },
+                    {
+                        "command": "SETNAME",
+                        "name": "clientname",
+                        "optional": true,
+                        "type": "string"
+                    }
                 ],
+                "name": "arguments",
                 "optional": true,
-                "type": [
-                    "string",
-                    "string"
-                ]
-            },
-            {
-                "command": "SETNAME",
-                "name": "clientname",
-                "optional": true,
-                "type": "string"
+                "type": "block"
             }
         ],
         "complexity": "O(1)",
         "group": "connection",
         "since": "6.0.0",
-        "summary": "switch Redis protocol"
+        "summary": "Handshake with Redis"
     },
     "HEXISTS": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
@@ -1636,14 +2240,45 @@
             }
         ],
         "complexity": "O(N) where N is the number of fields being set.",
         "group": "hash",
         "since": "2.0.0",
         "summary": "Set multiple hash fields to multiple values"
     },
+    "HRANDFIELD": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "block": [
+                    {
+                        "name": "count",
+                        "type": "integer"
+                    },
+                    {
+                        "enum": [
+                            "WITHVALUES"
+                        ],
+                        "name": "withvalues",
+                        "optional": true,
+                        "type": "enum"
+                    }
+                ],
+                "name": "options",
+                "optional": true,
+                "type": "block"
+            }
+        ],
+        "complexity": "O(N) where N is the number of fields returned",
+        "group": "hash",
+        "since": "6.2.0",
+        "summary": "Get one or multiple random fields from a hash"
+    },
     "HSCAN": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
@@ -1848,14 +2483,15 @@
         "group": "server",
         "since": "2.8.13",
         "summary": "Return the latest latency samples for all events."
     },
     "LATENCY RESET": {
         "arguments": [
             {
+                "multiple": true,
                 "name": "event",
                 "optional": true,
                 "type": "string"
             }
         ],
         "group": "server",
         "since": "2.8.13",
@@ -1913,14 +2549,46 @@
             }
         ],
         "complexity": "O(1)",
         "group": "list",
         "since": "1.0.0",
         "summary": "Get the length of a list"
     },
+    "LMOVE": {
+        "arguments": [
+            {
+                "name": "source",
+                "type": "key"
+            },
+            {
+                "name": "destination",
+                "type": "key"
+            },
+            {
+                "enum": [
+                    "LEFT",
+                    "RIGHT"
+                ],
+                "name": "wherefrom",
+                "type": "enum"
+            },
+            {
+                "enum": [
+                    "LEFT",
+                    "RIGHT"
+                ],
+                "name": "whereto",
+                "type": "enum"
+            }
+        ],
+        "complexity": "O(1)",
+        "group": "list",
+        "since": "6.2.0",
+        "summary": "Pop an element from a list, push it to another list and return it"
+    },
     "LOLWUT": {
         "arguments": [
             {
                 "command": "VERSION",
                 "name": "version",
                 "optional": true,
                 "type": "integer"
@@ -1931,20 +2599,59 @@
         "summary": "Display some computer art and the Redis version"
     },
     "LPOP": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
+            },
+            {
+                "name": "count",
+                "optional": true,
+                "type": "integer"
             }
         ],
-        "complexity": "O(1)",
+        "complexity": "O(N) where N is the number of elements returned",
         "group": "list",
         "since": "1.0.0",
-        "summary": "Remove and get the first element in a list"
+        "summary": "Remove and get the first elements in a list"
+    },
+    "LPOS": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "name": "element",
+                "type": "string"
+            },
+            {
+                "command": "RANK",
+                "name": "rank",
+                "optional": true,
+                "type": "integer"
+            },
+            {
+                "command": "COUNT",
+                "name": "num-matches",
+                "optional": true,
+                "type": "integer"
+            },
+            {
+                "command": "MAXLEN",
+                "name": "len",
+                "optional": true,
+                "type": "integer"
+            }
+        ],
+        "complexity": "O(N) where N is the number of elements in the list, for the average case. When searching for elements near the head or the tail of the list, or when the MAXLEN option is provided, the command may run in constant time.",
+        "group": "list",
+        "since": "6.0.6",
+        "summary": "Return the index of matching elements on a list"
     },
     "LPUSH": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
@@ -2157,14 +2864,20 @@
             {
                 "command": "AUTH",
                 "name": "password",
                 "optional": true,
                 "type": "string"
             },
             {
+                "command": "AUTH2",
+                "name": "username password",
+                "optional": true,
+                "type": "string"
+            },
+            {
                 "command": "KEYS",
                 "name": "key",
                 "optional": true,
                 "type": "key",
                 "variadic": true
             }
         ],
@@ -2331,23 +3044,36 @@
             }
         ],
         "complexity": "O(1)",
         "group": "generic",
         "since": "2.6.0",
         "summary": "Set the expiration for a key as a UNIX timestamp specified in milliseconds"
     },
+    "PEXPIRETIME": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            }
+        ],
+        "complexity": "O(1)",
+        "group": "generic",
+        "since": "7.0.0",
+        "summary": "Get the expiration Unix timestamp for a key in milliseconds"
+    },
     "PFADD": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
                 "multiple": true,
                 "name": "element",
+                "optional": true,
                 "type": "string"
             }
         ],
         "complexity": "O(1) to add every element.",
         "group": "hyperloglog",
         "since": "2.8.9",
         "summary": "Adds the specified elements to the specified HyperLogLog."
@@ -2572,14 +3298,19 @@
                 "type": "string"
             }
         ],
         "group": "server",
         "since": "5.0.0",
         "summary": "Make the server a replica of another instance, or promote it as master."
     },
+    "RESET": {
+        "group": "connection",
+        "since": "6.2",
+        "summary": "Reset the connection"
+    },
     "RESTORE": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
@@ -2630,20 +3361,25 @@
         "summary": "Return the role of the instance in the context of replication"
     },
     "RPOP": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
+            },
+            {
+                "name": "count",
+                "optional": true,
+                "type": "integer"
             }
         ],
-        "complexity": "O(1)",
+        "complexity": "O(N) where N is the number of elements returned",
         "group": "list",
         "since": "1.0.0",
-        "summary": "Remove and get the last element in a list"
+        "summary": "Remove and get the last elements in a list"
     },
     "RPOPLPUSH": {
         "arguments": [
             {
                 "name": "source",
                 "type": "key"
             },
@@ -2782,14 +3518,25 @@
         ],
         "complexity": "O(N) with N being the number of scripts to check (so checking a single script is an O(1) operation).",
         "group": "scripting",
         "since": "2.6.0",
         "summary": "Check existence of scripts in the script cache."
     },
     "SCRIPT FLUSH": {
+        "arguments": [
+            {
+                "enum": [
+                    "ASYNC",
+                    "SYNC"
+                ],
+                "name": "async",
+                "optional": true,
+                "type": "enum"
+            }
+        ],
         "complexity": "O(N) with N being the number of scripts in cache",
         "group": "scripting",
         "since": "2.6.0",
         "summary": "Remove all the scripts from the script cache."
     },
     "SCRIPT KILL": {
         "complexity": "O(1)",
@@ -2859,15 +3606,18 @@
             {
                 "name": "value",
                 "type": "string"
             },
             {
                 "enum": [
                     "EX seconds",
-                    "PX milliseconds"
+                    "PX milliseconds",
+                    "EXAT timestamp",
+                    "PXAT milliseconds-timestamp",
+                    "KEEPTTL"
                 ],
                 "name": "expiration",
                 "optional": true,
                 "type": "enum"
             },
             {
                 "enum": [
@@ -2876,17 +3626,17 @@
                 ],
                 "name": "condition",
                 "optional": true,
                 "type": "enum"
             },
             {
                 "enum": [
-                    "KEEPTTL"
+                    "GET"
                 ],
-                "name": "keepttl",
+                "name": "get",
                 "optional": true,
                 "type": "enum"
             }
         ],
         "complexity": "O(1)",
         "group": "string",
         "since": "1.0.0",
@@ -2904,15 +3654,15 @@
             },
             {
                 "name": "value",
                 "type": "integer"
             }
         ],
         "complexity": "O(1)",
-        "group": "string",
+        "group": "bitmap",
         "since": "2.2.0",
         "summary": "Sets or clears the bit at offset in the string value stored at key"
     },
     "SETEX": {
         "arguments": [
             {
                 "name": "key",
@@ -3069,14 +3819,31 @@
             }
         ],
         "complexity": "O(N) where N is the set cardinality.",
         "group": "set",
         "since": "1.0.0",
         "summary": "Get all the members in a set"
     },
+    "SMISMEMBER": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "multiple": true,
+                "name": "member",
+                "type": "string"
+            }
+        ],
+        "complexity": "O(N) where N is the number of elements being checked for membership",
+        "group": "set",
+        "since": "6.2.0",
+        "summary": "Returns the membership associated with the given elements for a set"
+    },
     "SMOVE": {
         "arguments": [
             {
                 "name": "source",
                 "type": "key"
             },
             {
@@ -3161,15 +3928,15 @@
             },
             {
                 "name": "count",
                 "optional": true,
                 "type": "integer"
             }
         ],
-        "complexity": "O(1)",
+        "complexity": "Without the count argument O(1), otherwise O(N) where N is the value of the passed count.",
         "group": "set",
         "since": "1.0.0",
         "summary": "Remove and return one or multiple random members from a set"
     },
     "SRANDMEMBER": {
         "arguments": [
             {
@@ -3314,14 +4081,15 @@
                 "type": "integer"
             },
             {
                 "name": "index2",
                 "type": "integer"
             }
         ],
+        "complexity": "O(N) where N is the count of clients watching or blocking on keys from both databases.",
         "group": "server",
         "since": "4.0.0",
         "summary": "Swaps two Redis databases"
     },
     "SYNC": {
         "group": "server",
         "since": "1.0.0",
@@ -3456,34 +4224,116 @@
     "XADD": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
-                "name": "ID",
-                "type": "string"
+                "command": "NOMKSTREAM",
+                "optional": true
+            },
+            {
+                "block": [
+                    {
+                        "enum": [
+                            "MAXLEN",
+                            "MINID"
+                        ],
+                        "name": "strategy",
+                        "type": "enum"
+                    },
+                    {
+                        "enum": [
+                            "=",
+                            "~"
+                        ],
+                        "name": "operator",
+                        "optional": true,
+                        "type": "enum"
+                    },
+                    {
+                        "name": "threshold",
+                        "type": "string"
+                    },
+                    {
+                        "command": "LIMIT",
+                        "name": "count",
+                        "optional": true,
+                        "type": "integer"
+                    }
+                ],
+                "name": "trim",
+                "optional": true,
+                "type": "block"
+            },
+            {
+                "enum": [
+                    "*",
+                    "ID"
+                ],
+                "type": "enum"
             },
             {
                 "multiple": true,
                 "name": [
                     "field",
                     "value"
                 ],
                 "type": [
                     "string",
                     "string"
                 ]
             }
         ],
-        "complexity": "O(1)",
+        "complexity": "O(1) when adding a new entry, O(N) when trimming where N being the number of entires evicted.",
         "group": "stream",
         "since": "5.0.0",
         "summary": "Appends a new entry to a stream"
     },
+    "XAUTOCLAIM": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "name": "group",
+                "type": "string"
+            },
+            {
+                "name": "consumer",
+                "type": "string"
+            },
+            {
+                "name": "min-idle-time",
+                "type": "string"
+            },
+            {
+                "name": "start",
+                "type": "string"
+            },
+            {
+                "command": "COUNT",
+                "name": "count",
+                "optional": true,
+                "type": "integer"
+            },
+            {
+                "enum": [
+                    "JUSTID"
+                ],
+                "name": "justid",
+                "optional": true
+            }
+        ],
+        "complexity": "O(1) if COUNT is small.",
+        "group": "stream",
+        "since": "6.2.0",
+        "summary": "Changes (or acquires) ownership of messages in a consumer group, as if the messages were delivered to the specified consumer."
+    },
     "XCLAIM": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
@@ -3557,50 +4407,92 @@
         "group": "stream",
         "since": "5.0.0",
         "summary": "Removes the specified entries from the stream. Returns the number of items actually deleted, that may be different from the number of IDs passed in case certain IDs do not exist."
     },
     "XGROUP": {
         "arguments": [
             {
-                "command": "CREATE",
-                "name": [
-                    "key",
-                    "groupname",
-                    "id-or-$"
+                "block": [
+                    {
+                        "command": "CREATE",
+                        "name": [
+                            "key",
+                            "groupname"
+                        ],
+                        "type": [
+                            "key",
+                            "string"
+                        ]
+                    },
+                    {
+                        "enum": [
+                            "ID",
+                            "$"
+                        ],
+                        "name": "id",
+                        "type": "enum"
+                    },
+                    {
+                        "command": "MKSTREAM",
+                        "optional": true
+                    }
+                ],
+                "name": "create",
+                "optional": true,
+                "type": "block"
+            },
+            {
+                "block": [
+                    {
+                        "command": "SETID",
+                        "name": [
+                            "key",
+                            "groupname"
+                        ],
+                        "type": [
+                            "key",
+                            "string"
+                        ]
+                    },
+                    {
+                        "enum": [
+                            "ID",
+                            "$"
+                        ],
+                        "name": "id",
+                        "type": "enum"
+                    }
                 ],
+                "name": "setid",
                 "optional": true,
-                "type": [
-                    "key",
-                    "string",
-                    "string"
-                ]
+                "type": "block"
             },
             {
-                "command": "SETID",
+                "command": "DESTROY",
                 "name": [
                     "key",
-                    "groupname",
-                    "id-or-$"
+                    "groupname"
                 ],
                 "optional": true,
                 "type": [
                     "key",
-                    "string",
                     "string"
                 ]
             },
             {
-                "command": "DESTROY",
+                "command": "CREATECONSUMER",
                 "name": [
                     "key",
-                    "groupname"
+                    "groupname",
+                    "consumername"
                 ],
                 "optional": true,
                 "type": [
                     "key",
+                    "string",
                     "string"
                 ]
             },
             {
                 "command": "DELCONSUMER",
                 "name": [
                     "key",
@@ -3666,46 +4558,58 @@
                 "name": "key",
                 "type": "key"
             }
         ],
         "complexity": "O(1)",
         "group": "stream",
         "since": "5.0.0",
-        "summary": "Return the number of entires in a stream"
+        "summary": "Return the number of entries in a stream"
     },
     "XPENDING": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
                 "name": "group",
                 "type": "string"
             },
             {
-                "name": [
-                    "start",
-                    "end",
-                    "count"
+                "block": [
+                    {
+                        "command": "IDLE",
+                        "name": "min-idle-time",
+                        "optional": true,
+                        "type": "integer"
+                    },
+                    {
+                        "name": "start",
+                        "type": "string"
+                    },
+                    {
+                        "name": "end",
+                        "type": "string"
+                    },
+                    {
+                        "name": "count",
+                        "type": "integer"
+                    },
+                    {
+                        "name": "consumer",
+                        "optional": true,
+                        "type": "string"
+                    }
                 ],
+                "name": "filters",
                 "optional": true,
-                "type": [
-                    "string",
-                    "string",
-                    "integer"
-                ]
-            },
-            {
-                "name": "consumer",
-                "optional": true,
-                "type": "string"
+                "type": "block"
             }
         ],
-        "complexity": "O(N) with N being the number of elements returned, so asking for a small fixed number of entries per call is O(1). When the command returns just the summary it runs in O(1) time assuming the list of consumers is small, otherwise there is additional O(N) time needed to iterate every consumer.",
+        "complexity": "O(N) with N being the number of elements returned, so asking for a small fixed number of entries per call is O(1). O(M), where M is the total number of entries scanned when used with the IDLE filter. When the command returns just the summary and the list of consumers is small, it runs in O(1) time; otherwise, an additional O(N) time for iterating every consumer.",
         "group": "stream",
         "since": "5.0.0",
         "summary": "Return information and entries from a stream consumer group pending entries list, that are messages fetched but never acknowledged."
     },
     "XRANGE": {
         "arguments": [
             {
@@ -3756,15 +4660,15 @@
             {
                 "multiple": true,
                 "name": "key",
                 "type": "key"
             },
             {
                 "multiple": true,
-                "name": "id",
+                "name": "ID",
                 "type": "string"
             }
         ],
         "complexity": "For each stream mentioned: O(N) with N being the number of elements being returned, it means that XREAD-ing with a fixed COUNT is O(1). Note that when the BLOCK option is used, XADD will pay O(M) time in order to serve the M clients blocked on the stream getting new data.",
         "group": "stream",
         "since": "5.0.0",
         "summary": "Return never seen elements in multiple streams, with IDs greater than the ones reported by the caller for each stream. Can block."
@@ -3854,31 +4758,45 @@
     "XTRIM": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
-                "enum": [
-                    "MAXLEN"
+                "block": [
+                    {
+                        "enum": [
+                            "MAXLEN",
+                            "MINID"
+                        ],
+                        "name": "strategy",
+                        "type": "enum"
+                    },
+                    {
+                        "enum": [
+                            "=",
+                            "~"
+                        ],
+                        "name": "operator",
+                        "optional": true,
+                        "type": "enum"
+                    },
+                    {
+                        "name": "threshold",
+                        "type": "string"
+                    },
+                    {
+                        "command": "LIMIT",
+                        "name": "count",
+                        "optional": true,
+                        "type": "integer"
+                    }
                 ],
-                "name": "strategy",
-                "type": "enum"
-            },
-            {
-                "enum": [
-                    "~"
-                ],
-                "name": "approx",
-                "optional": true,
-                "type": "enum"
-            },
-            {
-                "name": "count",
-                "type": "integer"
+                "name": "trim",
+                "type": "block"
             }
         ],
         "complexity": "O(N), with N being the number of evicted entries. Constant times are very small however, since entries are organized in macro nodes containing multiple entries that can be released with a single deallocation.",
         "group": "stream",
         "since": "5.0.0",
         "summary": "Trims the stream to (approximately if '~' is passed) a certain size"
     },
@@ -3895,14 +4813,23 @@
                 ],
                 "name": "condition",
                 "optional": true,
                 "type": "enum"
             },
             {
                 "enum": [
+                    "GT",
+                    "LT"
+                ],
+                "name": "comparison",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "enum": [
                     "CH"
                 ],
                 "name": "change",
                 "optional": true,
                 "type": "enum"
             },
             {
@@ -3958,14 +4885,60 @@
             }
         ],
         "complexity": "O(log(N)) with N being the number of elements in the sorted set.",
         "group": "sorted_set",
         "since": "2.0.0",
         "summary": "Count the members in a sorted set with scores within the given values"
     },
+    "ZDIFF": {
+        "arguments": [
+            {
+                "name": "numkeys",
+                "type": "integer"
+            },
+            {
+                "multiple": true,
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "enum": [
+                    "WITHSCORES"
+                ],
+                "name": "withscores",
+                "optional": true,
+                "type": "enum"
+            }
+        ],
+        "complexity": "O(L + (N-K)log(N)) worst case where L is the total number of elements in all the sets, N is the size of the first set, and K is the size of the result set.",
+        "group": "sorted_set",
+        "since": "6.2.0",
+        "summary": "Subtract multiple sorted sets"
+    },
+    "ZDIFFSTORE": {
+        "arguments": [
+            {
+                "name": "destination",
+                "type": "key"
+            },
+            {
+                "name": "numkeys",
+                "type": "integer"
+            },
+            {
+                "multiple": true,
+                "name": "key",
+                "type": "key"
+            }
+        ],
+        "complexity": "O(L + (N-K)log(N)) worst case where L is the total number of elements in all the sets, N is the size of the first set, and K is the size of the result set.",
+        "group": "sorted_set",
+        "since": "6.2.0",
+        "summary": "Subtract multiple sorted sets and store the resulting sorted set in a new key"
+    },
     "ZINCRBY": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
@@ -3978,14 +4951,57 @@
             }
         ],
         "complexity": "O(log(N)) where N is the number of elements in the sorted set.",
         "group": "sorted_set",
         "since": "1.2.0",
         "summary": "Increment the score of a member in a sorted set"
     },
+    "ZINTER": {
+        "arguments": [
+            {
+                "name": "numkeys",
+                "type": "integer"
+            },
+            {
+                "multiple": true,
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "command": "WEIGHTS",
+                "name": "weight",
+                "optional": true,
+                "type": "integer",
+                "variadic": true
+            },
+            {
+                "command": "AGGREGATE",
+                "enum": [
+                    "SUM",
+                    "MIN",
+                    "MAX"
+                ],
+                "name": "aggregate",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "enum": [
+                    "WITHSCORES"
+                ],
+                "name": "withscores",
+                "optional": true,
+                "type": "enum"
+            }
+        ],
+        "complexity": "O(N*K)+O(M*log(M)) worst case with N being the smallest input sorted set, K being the number of input sorted sets and M being the number of elements in the resulting sorted set.",
+        "group": "sorted_set",
+        "since": "6.2.0",
+        "summary": "Intersect multiple sorted sets"
+    },
     "ZINTERSTORE": {
         "arguments": [
             {
                 "name": "destination",
                 "type": "key"
             },
             {
@@ -4037,14 +5053,31 @@
             }
         ],
         "complexity": "O(log(N)) with N being the number of elements in the sorted set.",
         "group": "sorted_set",
         "since": "2.8.9",
         "summary": "Count the number of members in a sorted set between a given lexicographical range"
     },
+    "ZMSCORE": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "multiple": true,
+                "name": "member",
+                "type": "string"
+            }
+        ],
+        "complexity": "O(N) where N is the number of members being requested.",
+        "group": "sorted_set",
+        "since": "6.2.0",
+        "summary": "Get the score associated with the given members in a sorted set"
+    },
     "ZPOPMAX": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
@@ -4071,41 +5104,101 @@
             }
         ],
         "complexity": "O(log(N)*M) with N being the number of elements in the sorted set, and M being the number of elements popped.",
         "group": "sorted_set",
         "since": "5.0.0",
         "summary": "Remove and return members with the lowest scores in a sorted set"
     },
+    "ZRANDMEMBER": {
+        "arguments": [
+            {
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "block": [
+                    {
+                        "name": "count",
+                        "type": "integer"
+                    },
+                    {
+                        "enum": [
+                            "WITHSCORES"
+                        ],
+                        "name": "withscores",
+                        "optional": true,
+                        "type": "enum"
+                    }
+                ],
+                "name": "options",
+                "optional": true,
+                "type": "block"
+            }
+        ],
+        "complexity": "O(N) where N is the number of elements returned",
+        "group": "sorted_set",
+        "since": "6.2.0",
+        "summary": "Get one or multiple random elements from a sorted set"
+    },
     "ZRANGE": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
-                "name": "start",
-                "type": "integer"
+                "name": "min",
+                "type": "string"
             },
             {
-                "name": "stop",
-                "type": "integer"
+                "name": "max",
+                "type": "string"
+            },
+            {
+                "enum": [
+                    "BYSCORE",
+                    "BYLEX"
+                ],
+                "name": "sortby",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "enum": [
+                    "REV"
+                ],
+                "name": "rev",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "command": "LIMIT",
+                "name": [
+                    "offset",
+                    "count"
+                ],
+                "optional": true,
+                "type": [
+                    "integer",
+                    "integer"
+                ]
             },
             {
                 "enum": [
                     "WITHSCORES"
                 ],
                 "name": "withscores",
                 "optional": true,
                 "type": "enum"
             }
         ],
         "complexity": "O(log(N)+M) with N being the number of elements in the sorted set and M the number of elements returned.",
         "group": "sorted_set",
         "since": "1.2.0",
-        "summary": "Return a range of members in a sorted set, by index"
+        "summary": "Return a range of members in a sorted set"
     },
     "ZRANGEBYLEX": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
@@ -4171,14 +5264,67 @@
             }
         ],
         "complexity": "O(log(N)+M) with N being the number of elements in the sorted set and M the number of elements being returned. If M is constant (e.g. always asking for the first 10 elements with LIMIT), you can consider it O(log(N)).",
         "group": "sorted_set",
         "since": "1.0.5",
         "summary": "Return a range of members in a sorted set, by score"
     },
+    "ZRANGESTORE": {
+        "arguments": [
+            {
+                "name": "dst",
+                "type": "key"
+            },
+            {
+                "name": "src",
+                "type": "key"
+            },
+            {
+                "name": "min",
+                "type": "string"
+            },
+            {
+                "name": "max",
+                "type": "string"
+            },
+            {
+                "enum": [
+                    "BYSCORE",
+                    "BYLEX"
+                ],
+                "name": "sortby",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "enum": [
+                    "REV"
+                ],
+                "name": "rev",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "command": "LIMIT",
+                "name": [
+                    "offset",
+                    "count"
+                ],
+                "optional": true,
+                "type": [
+                    "integer",
+                    "integer"
+                ]
+            }
+        ],
+        "complexity": "O(log(N)+M) with N being the number of elements in the sorted set and M the number of elements stored into the destination key.",
+        "group": "sorted_set",
+        "since": "6.2.0",
+        "summary": "Store a range of members from sorted set into another key"
+    },
     "ZRANK": {
         "arguments": [
             {
                 "name": "key",
                 "type": "key"
             },
             {
@@ -4424,14 +5570,57 @@
             }
         ],
         "complexity": "O(1)",
         "group": "sorted_set",
         "since": "1.2.0",
         "summary": "Get the score associated with the given member in a sorted set"
     },
+    "ZUNION": {
+        "arguments": [
+            {
+                "name": "numkeys",
+                "type": "integer"
+            },
+            {
+                "multiple": true,
+                "name": "key",
+                "type": "key"
+            },
+            {
+                "command": "WEIGHTS",
+                "name": "weight",
+                "optional": true,
+                "type": "integer",
+                "variadic": true
+            },
+            {
+                "command": "AGGREGATE",
+                "enum": [
+                    "SUM",
+                    "MIN",
+                    "MAX"
+                ],
+                "name": "aggregate",
+                "optional": true,
+                "type": "enum"
+            },
+            {
+                "enum": [
+                    "WITHSCORES"
+                ],
+                "name": "withscores",
+                "optional": true,
+                "type": "enum"
+            }
+        ],
+        "complexity": "O(N)+O(M*log(M)) with N being the sum of the sizes of the input sorted sets, and M being the number of elements in the resulting sorted set.",
+        "group": "sorted_set",
+        "since": "6.2.0",
+        "summary": "Add multiple sorted sets"
+    },
     "ZUNIONSTORE": {
         "arguments": [
             {
                 "name": "destination",
                 "type": "key"
             },
             {
```

### Comparing `iredis-1.9.3/iredis/data/dangerous_commands.csv` & `iredis-1.9.4/iredis/data/dangerous_commands.csv`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/data/iredisrc` & `iredis-1.9.4/iredis/data/iredisrc`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/entry.py` & `iredis-1.9.4/iredis/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,16 @@
     )
     # raw config
     if raw is not None:
         config.raw = raw
     if not sys.stdout.isatty():
         config.raw = True
 
-    config.newbie_mode = newbie
+    if newbie is not None:
+        config.newbie_mode = newbie
 
     if decode is not None:
         config.decode = decode
     if rainbow is not None:
         config.rainbow = rainbow
     if shell is not None:
         config.shell = shell
```

### Comparing `iredis-1.9.3/iredis/key_bindings.py` & `iredis-1.9.4/iredis/key_bindings.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/lexer.py` & `iredis-1.9.4/iredis/lexer.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/markdown.py` & `iredis-1.9.4/iredis/markdown.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/processors.py` & `iredis-1.9.4/iredis/processors.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/redis_grammar.py` & `iredis-1.9.4/iredis/redis_grammar.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/renders.py` & `iredis-1.9.4/iredis/renders.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,14 +167,24 @@
         """
         if text is None:
             return NIL
         text = ensure_str(text)
         return FormattedText([("class:success", text)])
 
     @staticmethod
+    def render_help(raw):
+        """
+        render help text message.
+        the comand like ``ACL HELP`` and ``MEMORY HELP``
+        will return a list of strings.
+        we render it as plain text
+        """
+        return FormattedText([("class:string", _render_raw_list(raw).decode())])
+
+    @staticmethod
     def render_transaction_queue(text):
         """
         Used when client session is in a transaction.
 
         Response message should be "QUEUE" or Error.
         """
         text = ensure_str(text)
```

### Comparing `iredis-1.9.3/iredis/style.py` & `iredis-1.9.4/iredis/style.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/utils.py` & `iredis-1.9.4/iredis/utils.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/iredis/warning.py` & `iredis-1.9.4/iredis/warning.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/pyproject.toml` & `iredis-1.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iredis"
-version = "1.9.3"
+version = "1.9.4"
 description = "Terminal client for Redis with auto-completion and syntax highlighting."
 authors = ["laixintao <laixintao1995@163.com>"]
 readme = 'README.md'
 license = "BSD-3-Clause"
 repository = 'https://github.com/laixintao/iredis'
 homepage = "https://github.com/laixintao/iredis"
 keywords=["Redis", "key-value store", "Commandline tools", "Redis Client"]
```

### Comparing `iredis-1.9.3/tests/cli_tests/test_cli_pubsub.py` & `iredis-1.9.4/tests/cli_tests/test_cli_pubsub.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/cli_tests/test_cli_start.py` & `iredis-1.9.4/tests/cli_tests/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/cli_tests/test_command_input.py` & `iredis-1.9.4/tests/cli_tests/test_command_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,7 +55,20 @@
     cli.expect("auth")
     cli.expect(r"\*{11}")
 
 
 def test_hello_command_is_not_supported(cli):
     cli.sendline("hello 3")
     cli.expect("IRedis currently not support RESP3")
+
+
+def test_abort_reading_connection(cli):
+    cli.sendline("blpop mylist 30")
+    cli.send(chr(3))
+    cli.expect(
+        r"KeyboardInterrupt received! User canceled reading response!", timeout=10
+    )
+
+    cli.sendline("set foo bar")
+    cli.expect("OK")
+    cli.sendline("get foo")
+    cli.expect("bar")
```

### Comparing `iredis-1.9.3/tests/cli_tests/test_completer.py` & `iredis-1.9.4/tests/cli_tests/test_completer.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/cli_tests/test_config.py` & `iredis-1.9.4/tests/cli_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/cli_tests/test_dsn.py` & `iredis-1.9.4/tests/cli_tests/test_dsn.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/cli_tests/test_history.py` & `iredis-1.9.4/tests/cli_tests/test_history.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/cli_tests/test_pager.py` & `iredis-1.9.4/tests/cli_tests/test_pager.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/cli_tests/test_shell_pipeline.py` & `iredis-1.9.4/tests/cli_tests/test_shell_pipeline.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/cli_tests/test_string_execute.py` & `iredis-1.9.4/tests/cli_tests/test_string_execute.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/cli_tests/test_transaction.py` & `iredis-1.9.4/tests/cli_tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/cli_tests/test_warning.py` & `iredis-1.9.4/tests/cli_tests/test_warning.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/conftest.py` & `iredis-1.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_base_token.py` & `iredis-1.9.4/tests/unittests/command_parse/test_base_token.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_cluster.py` & `iredis-1.9.4/tests/unittests/command_parse/test_cluster.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_connection.py` & `iredis-1.9.4/tests/unittests/command_parse/test_connection.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_generic_parse.py` & `iredis-1.9.4/tests/unittests/command_parse/test_generic_parse.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_geo.py` & `iredis-1.9.4/tests/unittests/command_parse/test_geo.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_hash_parse.py` & `iredis-1.9.4/tests/unittests/command_parse/test_hash_parse.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_list_parse.py` & `iredis-1.9.4/tests/unittests/command_parse/test_list_parse.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_script.py` & `iredis-1.9.4/tests/unittests/command_parse/test_script.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_server.py` & `iredis-1.9.4/tests/unittests/command_parse/test_server.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_set_parse.py` & `iredis-1.9.4/tests/unittests/command_parse/test_set_parse.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_sorted_set_parse.py` & `iredis-1.9.4/tests/unittests/command_parse/test_sorted_set_parse.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_stream.py` & `iredis-1.9.4/tests/unittests/command_parse/test_stream.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/command_parse/test_string_parse.py` & `iredis-1.9.4/tests/unittests/command_parse/test_string_parse.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/test_client.py` & `iredis-1.9.4/tests/unittests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from prompt_toolkit.formatted_text import FormattedText
 
 from iredis.client import Client
 from iredis.config import config, load_config_files
 from iredis.completers import IRedisCompleter
 from iredis.entry import Rainbow, prompt_message
 from iredis.exceptions import NotSupport
+from ..helpers import formatted_text_rematch
 
 
 @pytest.fixture
 def completer():
     return IRedisCompleter()
 
 
@@ -255,62 +256,63 @@
 
 
 def test_peek_string(iredis_client, clean_redis):
     clean_redis.set("foo", "bar")
     peek_result = list(iredis_client.do_peek("foo"))
 
     assert peek_result[0][0] == ("class:dockey", "key: ")
-    assert re.match(r"string \(embstr\)  mem: 5\d bytes, ttl: -1", peek_result[0][1][1])
+    assert re.match(r"string \(embstr\)  mem: \d+ bytes, ttl: -1", peek_result[0][1][1])
     assert peek_result[0][2:] == [
         ("", "\n"),
         ("class:dockey", "strlen: "),
         ("", "3"),
         ("", "\n"),
         ("class:dockey", "value: "),
         ("", '"bar"'),
     ]
 
 
 def test_peek_list_fetch_all(iredis_client, clean_redis):
     clean_redis.lpush("mylist", *[f"hello-{index}" for index in range(5)])
     peek_result = list(iredis_client.do_peek("mylist"))
 
-    assert peek_result == [
+    formatted_text_rematch(
+        peek_result[0],
         FormattedText(
             [
                 ("class:dockey", "key: "),
-                ("", "list (quicklist)  mem: 176 bytes, ttl: -1"),
+                ("", r"list \(quicklist\)  mem: \d+ bytes, ttl: -1"),
                 ("", "\n"),
                 ("class:dockey", "llen: "),
                 ("", "5"),
                 ("", "\n"),
                 ("class:dockey", "elements: "),
                 ("", "\n"),
-                ("", "1)"),
+                ("", r"1\)"),
                 ("", " "),
                 ("class:string", '"hello-4"'),
                 ("", "\n"),
-                ("", "2)"),
+                ("", r"2\)"),
                 ("", " "),
                 ("class:string", '"hello-3"'),
                 ("", "\n"),
-                ("", "3)"),
+                ("", r"3\)"),
                 ("", " "),
                 ("class:string", '"hello-2"'),
                 ("", "\n"),
-                ("", "4)"),
+                ("", r"4\)"),
                 ("", " "),
                 ("class:string", '"hello-1"'),
                 ("", "\n"),
-                ("", "5)"),
+                ("", r"5\)"),
                 ("", " "),
                 ("class:string", '"hello-0"'),
             ]
-        )
-    ]
+        ),
+    )
 
 
 def test_peek_list_fetch_part(iredis_client, clean_redis):
     clean_redis.lpush("mylist", *[f"hello-{index}" for index in range(40)])
     peek_result = list(iredis_client.do_peek("mylist"))
     assert len(peek_result[0]) == 91
 
@@ -330,45 +332,51 @@
 
 
 def test_peek_zset_fetch_all(iredis_client, clean_redis):
     clean_redis.zadd(
         "myzset", dict(zip([f"hello-{index}" for index in range(3)], range(3)))
     )
     peek_result = list(iredis_client.do_peek("myzset"))
-    assert peek_result[0][0:9] == FormattedText(
-        [
-            ("class:dockey", "key: "),
-            ("", "zset (ziplist)  mem: 92 bytes, ttl: -1"),
-            ("", "\n"),
-            ("class:dockey", "zcount: "),
-            ("", "3"),
-            ("", "\n"),
-            ("class:dockey", "members: "),
-            ("", "\n"),
-            ("", "1)"),
-        ]
+    formatted_text_rematch(
+        peek_result[0][0:9],
+        FormattedText(
+            [
+                ("class:dockey", "key: "),
+                ("", r"zset \(ziplist\)  mem: \d+ bytes, ttl: -1"),
+                ("", "\n"),
+                ("class:dockey", "zcount: "),
+                ("", "3"),
+                ("", "\n"),
+                ("class:dockey", "members: "),
+                ("", "\n"),
+                ("", r"1\)"),
+            ]
+        ),
     )
 
 
 def test_peek_zset_fetch_part(iredis_client, clean_redis):
     clean_redis.zadd(
         "myzset", dict(zip([f"hello-{index}" for index in range(40)], range(40)))
     )
     peek_result = list(iredis_client.do_peek("myzset"))
-    assert peek_result[0][0:8] == FormattedText(
-        [
-            ("class:dockey", "key: "),
-            ("", "zset (ziplist)  mem: 556 bytes, ttl: -1"),
-            ("", "\n"),
-            ("class:dockey", "zcount: "),
-            ("", "40"),
-            ("", "\n"),
-            ("class:dockey", "members (first 40): "),
-            ("", "\n"),
-        ]
+    formatted_text_rematch(
+        peek_result[0][0:8],
+        FormattedText(
+            [
+                ("class:dockey", "key: "),
+                ("", r"zset \(ziplist\)  mem: \d+ bytes, ttl: -1"),
+                ("", "\n"),
+                ("class:dockey", "zcount: "),
+                ("", "40"),
+                ("", "\n"),
+                ("class:dockey", r"members \(first 40\): "),
+                ("", "\n"),
+            ]
+        ),
     )
 
 
 def test_peek_hash_fetch_all(iredis_client, clean_redis):
     for key, value in zip(
         [f"hello-{index}" for index in range(3)], [f"hi-{index}" for index in range(3)]
     ):
```

### Comparing `iredis-1.9.3/tests/unittests/test_completers.py` & `iredis-1.9.4/tests/unittests/test_completers.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/test_entry.py` & `iredis-1.9.4/tests/unittests/test_entry.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/test_markdown_doc_render.py` & `iredis-1.9.4/tests/unittests/test_markdown_doc_render.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/tests/unittests/test_render_functions.py` & `iredis-1.9.4/tests/unittests/test_render_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,7 +480,13 @@
 
 def test_render_bytes(config):
     assert renders.OutputRender.render_bytes(b"bytes\n") == b"bytes"
 
 
 def test_render_bytes_raw(config):
     assert renders.OutputRender.render_raw(b"bytes\n") == b"bytes\n"
+
+
+def test_render_help(config):
+    assert renders.OutputRender.render_help([b"foo", b"bar"]) == FormattedText(
+        [("class:string", "foo\nbar")]
+    )
```

### Comparing `iredis-1.9.3/tests/unittests/test_utils.py` & `iredis-1.9.4/tests/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `iredis-1.9.3/setup.py` & `iredis-1.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
  'wcwidth==0.1.9']
 
 entry_points = \
 {'console_scripts': ['iredis = iredis.entry:main']}
 
 setup_kwargs = {
     'name': 'iredis',
-    'version': '1.9.3',
+    'version': '1.9.4',
     'description': 'Terminal client for Redis with auto-completion and syntax highlighting.',
-    'long_description': '<p align="center">\n  <img width="100" height="100" src="https://raw.githubusercontent.com/laixintao/iredis/master/docs/assets/logo.png" />\n</p>\n\n<h3 align="center">Interactive Redis: A Cli for Redis with AutoCompletion and Syntax Highlighting.</h3>\n\n<p align="center">\n<a href="https://github.com/laixintao/iredis/actions"><img src="https://github.com/laixintao/iredis/workflows/Test/badge.svg" alt="Github Action"></a>\n<a href="https://badge.fury.io/py/iredis"><img src="https://badge.fury.io/py/iredis.svg" alt="PyPI version"></a>\n<img src="https://badgen.net/badge/python/3.6%20|%203.7%20|%203.8/" alt="Python version">\n<a href="https://pepy.tech/project/iredis"><img src="https://pepy.tech/badge/iredis" alt="Download stats"></a>\n<a href="https://t.me/iredis_users"><img src="https://badgen.net/badge/icon/join?icon=telegram&amp;label=usergroup" alt="Chat on telegram"></a>\n<a href="https://console.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/laixintao/iredis&amp;cloudshell_print=docs/cloudshell/run-in-docker.txt"><img src="https://badgen.net/badge/run/GoogleCloudShell/blue?icon=terminal" alt="Open in Cloud Shell"></a>\n</p>\n\n<p align="center">\n  <img src="./docs/assets/demo.svg" alt="demo">\n</p>\n\nIRedis is a terminal client for redis with auto-completion and syntax\nhighlighting. IRedis lets you type Redis commands smoothly, and displays results\nin a user-friendly format.\n\nIRedis is an alternative for redis-cli. In most cases, IRedis behaves exactly\nthe same as redis-cli. Besides, it is safer to use IRedis on production servers\nthan redis-cli: IRedis will prevent accidentally running dangerous commands,\nlike `KEYS *` (see\n[Redis docs / Latency generated by slow commands](https://redis.io/topics/latency#latency-generated-by-slow-commands)).\n\n## Features\n\n- Advanced code completion. If you run command `KEYS` then run `DEL`, IRedis\n  will auto-complete your command based on `KEYS` result.\n- Command validation. IRedis will validate command while you are typing, and\n  highlight errors. E.g. try `CLUSTER MEET IP PORT`, IRedis will validate IP and\n  PORT for you.\n- Command highlighting, fully based on redis grammar. Any valid command in\n  IRedis shell is a valid redis command.\n- Human-friendly result display.\n- _pipeline_ feature, you can use your favorite shell tools to parse redis\'\n  response, like `get json | jq .`.\n- Support pager for long output.\n- Support connection via URL, `iredis --url redis://example.com:6379/1`.\n- Store server configuration: `iredis -d prod-redis` (see [dsn](#using-dsn) for\n  more).\n- `peek` command to check the key\'s type then automatically call\n  `get`/`lrange`/`sscan`, etc, depending on types. You don\'t need to call the\n  `type` command then type another command to get the value. `peek` will also\n  display the key\'s length and memory usage.\n- <kbd>Ctrl</kbd> + <kbd>C</kbd> to cancel the current typed command, this won\'t\n  exit IRedis, exactly like bash behaviour. Use <kbd>Ctrl</kbd> + <kbd>D</kbd>\n  to send a EOF to exit IRedis.\n- <kbd>Ctrl</kbd> + <kbd>R</kbd> to open **reverse-i-search** to search through\n  your command history.\n- Auto suggestions. (Like [fish shell](http://fishshell.com/).)\n- Support `--encode=utf-8`, to decode Redis\' bytes responses.\n- Command hint on bottom, include command syntax, supported redis version, and\n  time complexity.\n- Official docs with built-in `HELP` command, try `HELP SET`!\n- Written in pure Python, but IRedis was packaged into a single binary with\n  [PyOxidizer](https://github.com/indygreg/PyOxidizer), you can use cURL to\n  download and run, it just works, even you don\'t have a Python interpreter.\n- Hide password for `AUTH` command.\n- Says "Goodbye!" to you when you exit!\n- For full features, please see: [iredis.io](https://www.iredis.io)\n\n## Install\n\nInstall via pip:\n\n```\npip install iredis\n```\n\n[pipx](https://github.com/pipxproject/pipx) is recommended:\n\n```\npipx install iredis\n```\n\nOr you can download the executable binary with cURL(or wget), untar, then run.\nIt is especially useful when you don\'t have a python interpreter(E.g. the\n[official Redis docker image](https://hub.docker.com/_/redis/) which doesn\'t\nhave Python installed.):\n\n```\nwget  https://github.com/laixintao/iredis/releases/latest/download/iredis.tar.gz \\\n && tar -xzf iredis.tar.gz \\\n && ./iredis\n```\n\n(Check the [release page](https://github.com/laixintao/iredis/releases) if you\nwant to download an old version of IRedis.)\n\n## Usage\n\nOnce you install IRedis, you will know how to use it. Just remember, IRedis\nsupports similar options like redis-cli, like `-h` for redis-server\'s host and\n`-p` for port.\n\n```\n$ iredis --help\n```\n\n### Using DSN\n\nIRedis support storing server configuration in config file. Here is a DSN\nconfig:\n\n```\n[alias_dsn]\ndev=redis://localhost:6379/4\nstaging=redis://username:password@staging-redis.example.com:6379/1\n```\n\nPut this in your `iredisrc` then connect via `iredis -d staging` or\n`iredis -d dev`.\n\n### Configuration\n\nIRedis supports config files. Command-line options will always take precedence\nover config. Configuration resolution from highest to lowest precedence is:\n\n- _Options from command line_\n- `$PWD/.iredisrc`\n- `~/.iredisrc` (this path can be changed with `iredis --iredisrc $YOUR_PATH`)\n- `/etc/iredisrc`\n- default config in IRedis package.\n\nYou can copy the _self-explained_ default config here:\n\nhttps://raw.githubusercontent.com/laixintao/iredis/master/iredis/data/iredisrc\n\nAnd then make your own changes.\n\n(If you are using an old versions of IRedis, please use the config file below,\nand change the version in URL):\n\nhttps://raw.githubusercontent.com/laixintao/iredis/v1.0.4/iredis/data/iredisrc\n\n### Keys\n\nIRedis support unix/readline-style REPL keyboard shortcuts, which means keys\nlike <kbd>Ctrl</kbd> + <kbd>F</kbd> to forward work.\n\nAlso:\n\n- <kbd>Ctrl</kbd> + <kbd>D</kbd> (i.e. EOF) to exit; you can also use the `exit`\n  command.\n- <kbd>Ctrl</kbd> + <kbd>L</kbd> to clear screen; you can also use the `clear`\n  command.\n- <kbd>Ctrl</kbd> + <kbd>X</kbd> <kbd>Ctrl</kbd> + <kbd>E</kbd> to open an\n  editor to edit command, or <kbd>V</kbd> in vi-mode.\n\n## Development\n\n### Release Strategy\n\nIRedis is built and released by `GitHub Actions`. Whenever a tag is pushed to the\n`master` branch, a new release is built and uploaded to pypi.org, it\'s very\nconvenient.\n\nThus, we release as often as possible, so that users can always enjoy the new\nfeatures and bugfixes quickly. Any bugfix or new feature will get at least a\npatch release, whereas big features will get a minor release.\n\n### Setup Environment\n\nIRedis favors [poetry](https://github.com/sdispater/poetry) as package\nmanagement tool. To setup a develop environment on your computer:\n\nFirst, install poetry (you can do it in a python\'s virtualenv):\n\n```\npip install poetry\n```\n\nThen run (which is similar to `pip install -e .`):\n\n```\npoetry install\n```\n\n**Be careful running testcases locally, it may flush you db!!!**\n\n### Development Logs\n\nThis is a command-line tool, so we don\'t write logs to stdout.\n\nYou can `tail -f ~/.iredis.log` to see logs, the log is pretty clear, you can\nsee what actually happens from log files.\n\n### Catch Up with Latest Redis-doc\n\nIRedis use a git submodule to track current-up-to-date redis-doc version. To\ncatch up with latest:\n\n1. Git pull in redis-doc\n2. Copy doc files to `/data`: `cp -r redis-doc/commands* iredis/data`\n3. Prettier\n   markdown`prettier --prose-wrap always iredis/data/commands/*.md --write`\n4. Check the diff, update IRedis\' code if needed.\n\n## Related Projects\n\n- [redis-tui](https://github.com/mylxsw/redis-tui)\n\nIf you like iredis, you may also like other cli tools by\n[dbcli](https://www.dbcli.com/):\n\n- [pgcli](https://www.pgcli.com) - Postgres Client with Auto-completion and\n  Syntax Highlighting\n- [mycli](https://www.mycli.net) - MySQL/MariaDB/Percona Client with\n  Auto-completion and Syntax Highlighting\n- [litecli](https://litecli.com) - SQLite Client with Auto-completion and Syntax\n  Highlighting\n- [mssql-cli](https://github.com/dbcli/mssql-cli) - Microsoft SQL Server Client\n  with Auto-completion and Syntax Highlighting\n- [athenacli](https://github.com/dbcli/athenacli) - AWS Athena Client with\n  Auto-completion and Syntax Highlighting\n- [vcli](https://github.com/dbcli/vcli) - VerticaDB client\n- [iredis](https://github.com/laixintao/iredis/) - Client for Redis with\n  AutoCompletion and Syntax Highlighting\n\nIRedis is build on the top of\n[prompt_toolkit](https://github.com/jonathanslenders/python-prompt-toolkit), a\nPython library (by [Jonathan Slenders](https://twitter.com/jonathan_s)) for\nbuilding rich commandline applications.\n',
+    'long_description': '<p align="center">\n  <img width="100" height="100" src="https://raw.githubusercontent.com/laixintao/iredis/master/docs/assets/logo.png" />\n</p>\n\n<h3 align="center">Interactive Redis: A Cli for Redis with AutoCompletion and Syntax Highlighting.</h3>\n\n<p align="center">\n<a href="https://github.com/laixintao/iredis/actions"><img src="https://github.com/laixintao/iredis/workflows/Test/badge.svg" alt="Github Action"></a>\n<a href="https://badge.fury.io/py/iredis"><img src="https://badge.fury.io/py/iredis.svg" alt="PyPI version"></a>\n<img src="https://badgen.net/badge/python/3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9/" alt="Python version">\n<a href="https://pepy.tech/project/iredis"><img src="https://pepy.tech/badge/iredis" alt="Download stats"></a>\n<a href="https://t.me/iredis_users"><img src="https://badgen.net/badge/icon/join?icon=telegram&amp;label=usergroup" alt="Chat on telegram"></a>\n<a href="https://console.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/laixintao/iredis&amp;cloudshell_print=docs/cloudshell/run-in-docker.txt"><img src="https://badgen.net/badge/run/GoogleCloudShell/blue?icon=terminal" alt="Open in Cloud Shell"></a>\n</p>\n\n<p align="center">\n  <img src="./docs/assets/demo.svg" alt="demo">\n</p>\n\nIRedis is a terminal client for redis with auto-completion and syntax\nhighlighting. IRedis lets you type Redis commands smoothly, and displays results\nin a user-friendly format.\n\nIRedis is an alternative for redis-cli. In most cases, IRedis behaves exactly\nthe same as redis-cli. Besides, it is safer to use IRedis on production servers\nthan redis-cli: IRedis will prevent accidentally running dangerous commands,\nlike `KEYS *` (see\n[Redis docs / Latency generated by slow commands](https://redis.io/topics/latency#latency-generated-by-slow-commands)).\n\n## Features\n\n- Advanced code completion. If you run command `KEYS` then run `DEL`, IRedis\n  will auto-complete your command based on `KEYS` result.\n- Command validation. IRedis will validate command while you are typing, and\n  highlight errors. E.g. try `CLUSTER MEET IP PORT`, IRedis will validate IP and\n  PORT for you.\n- Command highlighting, fully based on redis grammar. Any valid command in\n  IRedis shell is a valid redis command.\n- Human-friendly result display.\n- _pipeline_ feature, you can use your favorite shell tools to parse redis\'\n  response, like `get json | jq .`.\n- Support pager for long output.\n- Support connection via URL, `iredis --url redis://example.com:6379/1`.\n- Store server configuration: `iredis -d prod-redis` (see [dsn](#using-dsn) for\n  more).\n- `peek` command to check the key\'s type then automatically call\n  `get`/`lrange`/`sscan`, etc, depending on types. You don\'t need to call the\n  `type` command then type another command to get the value. `peek` will also\n  display the key\'s length and memory usage.\n- <kbd>Ctrl</kbd> + <kbd>C</kbd> to cancel the current typed command, this won\'t\n  exit IRedis, exactly like bash behaviour. Use <kbd>Ctrl</kbd> + <kbd>D</kbd>\n  to send a EOF to exit IRedis.\n- <kbd>Ctrl</kbd> + <kbd>R</kbd> to open **reverse-i-search** to search through\n  your command history.\n- Auto suggestions. (Like [fish shell](http://fishshell.com/).)\n- Support `--encode=utf-8`, to decode Redis\' bytes responses.\n- Command hint on bottom, include command syntax, supported redis version, and\n  time complexity.\n- Official docs with built-in `HELP` command, try `HELP SET`!\n- Written in pure Python, but IRedis was packaged into a single binary with\n  [PyOxidizer](https://github.com/indygreg/PyOxidizer), you can use cURL to\n  download and run, it just works, even you don\'t have a Python interpreter.\n- Hide password for `AUTH` command.\n- Says "Goodbye!" to you when you exit!\n- For full features, please see: [iredis.io](https://www.iredis.io)\n\n## Install\n\nInstall via pip:\n\n```\npip install iredis\n```\n\n[pipx](https://github.com/pipxproject/pipx) is recommended:\n\n```\npipx install iredis\n```\n\nOr you can download the executable binary with cURL(or wget), untar, then run.\nIt is especially useful when you don\'t have a python interpreter(E.g. the\n[official Redis docker image](https://hub.docker.com/_/redis/) which doesn\'t\nhave Python installed.):\n\n```\nwget  https://github.com/laixintao/iredis/releases/latest/download/iredis.tar.gz \\\n && tar -xzf iredis.tar.gz \\\n && ./iredis\n```\n\n(Check the [release page](https://github.com/laixintao/iredis/releases) if you\nwant to download an old version of IRedis.)\n\n## Usage\n\nOnce you install IRedis, you will know how to use it. Just remember, IRedis\nsupports similar options like redis-cli, like `-h` for redis-server\'s host and\n`-p` for port.\n\n```\n$ iredis --help\n```\n\n### Using DSN\n\nIRedis support storing server configuration in config file. Here is a DSN\nconfig:\n\n```\n[alias_dsn]\ndev=redis://localhost:6379/4\nstaging=redis://username:password@staging-redis.example.com:6379/1\n```\n\nPut this in your `iredisrc` then connect via `iredis -d staging` or\n`iredis -d dev`.\n\n### Configuration\n\nIRedis supports config files. Command-line options will always take precedence\nover config. Configuration resolution from highest to lowest precedence is:\n\n- _Options from command line_\n- `$PWD/.iredisrc`\n- `~/.iredisrc` (this path can be changed with `iredis --iredisrc $YOUR_PATH`)\n- `/etc/iredisrc`\n- default config in IRedis package.\n\nYou can copy the _self-explained_ default config here:\n\nhttps://raw.githubusercontent.com/laixintao/iredis/master/iredis/data/iredisrc\n\nAnd then make your own changes.\n\n(If you are using an old versions of IRedis, please use the config file below,\nand change the version in URL):\n\nhttps://raw.githubusercontent.com/laixintao/iredis/v1.0.4/iredis/data/iredisrc\n\n### Keys\n\nIRedis support unix/readline-style REPL keyboard shortcuts, which means keys\nlike <kbd>Ctrl</kbd> + <kbd>F</kbd> to forward work.\n\nAlso:\n\n- <kbd>Ctrl</kbd> + <kbd>D</kbd> (i.e. EOF) to exit; you can also use the `exit`\n  command.\n- <kbd>Ctrl</kbd> + <kbd>L</kbd> to clear screen; you can also use the `clear`\n  command.\n- <kbd>Ctrl</kbd> + <kbd>X</kbd> <kbd>Ctrl</kbd> + <kbd>E</kbd> to open an\n  editor to edit command, or <kbd>V</kbd> in vi-mode.\n\n## Development\n\n### Release Strategy\n\nIRedis is built and released by `GitHub Actions`. Whenever a tag is pushed to\nthe `master` branch, a new release is built and uploaded to pypi.org, it\'s very\nconvenient.\n\nThus, we release as often as possible, so that users can always enjoy the new\nfeatures and bugfixes quickly. Any bugfix or new feature will get at least a\npatch release, whereas big features will get a minor release.\n\n### Setup Environment\n\nIRedis favors [poetry](https://github.com/sdispater/poetry) as package\nmanagement tool. To setup a develop environment on your computer:\n\nFirst, install poetry (you can do it in a python\'s virtualenv):\n\n```\npip install poetry\n```\n\nThen run (which is similar to `pip install -e .`):\n\n```\npoetry install\n```\n\n**Be careful running testcases locally, it may flush you db!!!**\n\n### Development Logs\n\nThis is a command-line tool, so we don\'t write logs to stdout.\n\nYou can `tail -f ~/.iredis.log` to see logs, the log is pretty clear, you can\nsee what actually happens from log files.\n\n### Catch Up with Latest Redis-doc\n\nIRedis use a git submodule to track current-up-to-date redis-doc version. To\ncatch up with latest:\n\n1. Git pull in redis-doc\n2. Copy doc files to `/data`: `cp -r redis-doc/commands* iredis/data`\n3. Prettier\n   markdown`prettier --prose-wrap always iredis/data/commands/*.md --write`\n4. Check the diff, update IRedis\' code if needed.\n\n## Related Projects\n\n- [redis-tui](https://github.com/mylxsw/redis-tui)\n\nIf you like iredis, you may also like other cli tools by\n[dbcli](https://www.dbcli.com/):\n\n- [pgcli](https://www.pgcli.com) - Postgres Client with Auto-completion and\n  Syntax Highlighting\n- [mycli](https://www.mycli.net) - MySQL/MariaDB/Percona Client with\n  Auto-completion and Syntax Highlighting\n- [litecli](https://litecli.com) - SQLite Client with Auto-completion and Syntax\n  Highlighting\n- [mssql-cli](https://github.com/dbcli/mssql-cli) - Microsoft SQL Server Client\n  with Auto-completion and Syntax Highlighting\n- [athenacli](https://github.com/dbcli/athenacli) - AWS Athena Client with\n  Auto-completion and Syntax Highlighting\n- [vcli](https://github.com/dbcli/vcli) - VerticaDB client\n- [iredis](https://github.com/laixintao/iredis/) - Client for Redis with\n  AutoCompletion and Syntax Highlighting\n\nIRedis is build on the top of\n[prompt_toolkit](https://github.com/jonathanslenders/python-prompt-toolkit), a\nPython library (by [Jonathan Slenders](https://twitter.com/jonathan_s)) for\nbuilding rich commandline applications.\n',
     'author': 'laixintao',
     'author_email': 'laixintao1995@163.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/laixintao/iredis',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['iredis',
 'iredis.data', 'iredis.data.commands', 'tests', 'tests.cli_tests',
 'tests.unittests', 'tests.unittests.command_parse'] package_data = \ {'':
 ['*']} install_requires = \ ['Pygments>=2,<3', 'click>=7.0,<8.0',
 'configobj>=5.0,<6.0', 'importlib-resources>=5.1.0,<6.0.0',
 'mistune>=0.8,<0.9', 'pendulum>=2.0,<3.0', 'prompt_toolkit>=3,<4',
 'redis>=3,<4', 'wcwidth==0.1.9'] entry_points = \ {'console_scripts': ['iredis
-= iredis.entry:main']} setup_kwargs = { 'name': 'iredis', 'version': '1.9.3',
+= iredis.entry:main']} setup_kwargs = { 'name': 'iredis', 'version': '1.9.4',
 'description': 'Terminal client for Redis with auto-completion and syntax
 highlighting.', 'long_description': '
   \n [https://raw.githubusercontent.com/laixintao/iredis/master/docs/assets/
                                   logo.png]\n
 \n\n
     **** Interactive Redis: A Cli for Redis with AutoCompletion and Syntax
                               Highlighting. ****
@@ -79,15 +79,15 @@
 raw.githubusercontent.com/laixintao/iredis/v1.0.4/iredis/data/iredisrc\n\n###
 Keys\n\nIRedis support unix/readline-style REPL keyboard shortcuts, which means
 keys\nlike Ctrl + F to forward work.\n\nAlso:\n\n- Ctrl + D (i.e. EOF) to exit;
 you can also use the `exit`\n command.\n- Ctrl + L to clear screen; you can
 also use the `clear`\n command.\n- Ctrl + X Ctrl + E to open an\n editor to
 edit command, or V in vi-mode.\n\n## Development\n\n### Release
 Strategy\n\nIRedis is built and released by `GitHub Actions`. Whenever a tag is
-pushed to the\n`master` branch, a new release is built and uploaded to
+pushed to\nthe `master` branch, a new release is built and uploaded to
 pypi.org, it\'s very\nconvenient.\n\nThus, we release as often as possible, so
 that users can always enjoy the new\nfeatures and bugfixes quickly. Any bugfix
 or new feature will get at least a\npatch release, whereas big features will
 get a minor release.\n\n### Setup Environment\n\nIRedis favors [poetry](https:/
 /github.com/sdispater/poetry) as package\nmanagement tool. To setup a develop
 environment on your computer:\n\nFirst, install poetry (you can do it in a
 python\'s virtualenv):\n\n```\npip install poetry\n```\n\nThen run (which is
```

### Comparing `iredis-1.9.3/PKG-INFO` & `iredis-1.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iredis
-Version: 1.9.3
+Version: 1.9.4
 Summary: Terminal client for Redis with auto-completion and syntax highlighting.
 Home-page: https://github.com/laixintao/iredis
 License: BSD-3-Clause
 Keywords: Redis,key-value store,Commandline tools,Redis Client
 Author: laixintao
 Author-email: laixintao1995@163.com
 Requires-Python: >=3.6,<4.0
@@ -39,15 +39,15 @@
 </p>
 
 <h3 align="center">Interactive Redis: A Cli for Redis with AutoCompletion and Syntax Highlighting.</h3>
 
 <p align="center">
 <a href="https://github.com/laixintao/iredis/actions"><img src="https://github.com/laixintao/iredis/workflows/Test/badge.svg" alt="Github Action"></a>
 <a href="https://badge.fury.io/py/iredis"><img src="https://badge.fury.io/py/iredis.svg" alt="PyPI version"></a>
-<img src="https://badgen.net/badge/python/3.6%20|%203.7%20|%203.8/" alt="Python version">
+<img src="https://badgen.net/badge/python/3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9/" alt="Python version">
 <a href="https://pepy.tech/project/iredis"><img src="https://pepy.tech/badge/iredis" alt="Download stats"></a>
 <a href="https://t.me/iredis_users"><img src="https://badgen.net/badge/icon/join?icon=telegram&amp;label=usergroup" alt="Chat on telegram"></a>
 <a href="https://console.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/laixintao/iredis&amp;cloudshell_print=docs/cloudshell/run-in-docker.txt"><img src="https://badgen.net/badge/run/GoogleCloudShell/blue?icon=terminal" alt="Open in Cloud Shell"></a>
 </p>
 
 <p align="center">
   <img src="./docs/assets/demo.svg" alt="demo">
@@ -188,16 +188,16 @@
 - <kbd>Ctrl</kbd> + <kbd>X</kbd> <kbd>Ctrl</kbd> + <kbd>E</kbd> to open an
   editor to edit command, or <kbd>V</kbd> in vi-mode.
 
 ## Development
 
 ### Release Strategy
 
-IRedis is built and released by `GitHub Actions`. Whenever a tag is pushed to the
-`master` branch, a new release is built and uploaded to pypi.org, it's very
+IRedis is built and released by `GitHub Actions`. Whenever a tag is pushed to
+the `master` branch, a new release is built and uploaded to pypi.org, it's very
 convenient.
 
 Thus, we release as often as possible, so that users can always enjoy the new
 features and bugfixes quickly. Any bugfix or new feature will get at least a
 patch release, whereas big features will get a minor release.
 
 ### Setup Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iredis Version: 1.9.3 Summary: Terminal client for
+Metadata-Version: 2.1 Name: iredis Version: 1.9.4 Summary: Terminal client for
 Redis with auto-completion and syntax highlighting. Home-page: https://
 github.com/laixintao/iredis License: BSD-3-Clause Keywords: Redis,key-value
 store,Commandline tools,Redis Client Author: laixintao Author-email:
 laixintao1995@163.com Requires-Python: >=3.6,<4.0 Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: Console Classifier: Environment
 :: Console :: Curses Classifier: Environment :: MacOS X Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: BSD License
```

