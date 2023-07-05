# Comparing `tmp/hive_builder-3.6.7.tar.gz` & `tmp/hive_builder-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive_builder-3.6.7.tar", max compression
+gzip compressed data, was "hive_builder-3.6.8.tar", max compression
```

## Comparing `hive_builder-3.6.7.tar` & `hive_builder-3.6.8.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0     1074 2023-06-23 13:30:01.643440 hive_builder-3.6.7/LICENSE
--rw-r--r--   0        0        0     1231 2023-06-23 13:30:01.643440 hive_builder-3.6.7/README.md
--rwxr-xr-x   0        0        0      312 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/__init__.py
--rw-r--r--   0        0        0     1031 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/hive-completion.sh
--rw-r--r--   0        0        0    26952 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/hive.py
--rw-r--r--   0        0        0    14020 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/lib/azure_rm_storageshare.py
--rw-r--r--   0        0        0    14954 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/lib/hive_vagrant.py
--rw-r--r--   0        0        0     5832 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/build-images.yml
--rw-r--r--   0        0        0     1943 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/build-infra.yml
--rw-r--r--   0        0        0     1084 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/build-networks.yml
--rw-r--r--   0        0        0     2447 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/build-volumes.yml
--rw-r--r--   0        0        0       81 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/addon/tasks/main.yml
--rw-r--r--   0        0        0       40 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-certificate/files/extfile.cnf
--rw-r--r--   0        0        0     1783 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml
--rw-r--r--   0        0        0      356 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-syslog/tasks/main.yml
--rw-r--r--   0        0        0      946 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2
--rw-r--r--   0        0        0      650 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml
--rw-r--r--   0        0        0      351 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/tasks/main.yml
--rw-r--r--   0        0        0       49 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/vars/main.yml
--rw-r--r--   0        0        0      323 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/tasks/main.yml
--rw-r--r--   0        0        0       49 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/vars/main.yml
--rw-r--r--   0        0        0      409 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/tasks/main.yml
--rw-r--r--   0        0        0       49 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/vars/main.yml
--rw-r--r--   0        0        0      274 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/python-aptk/tasks/main.yml
--rw-r--r--   0        0        0     9564 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/deploy-services.yml
--rw-r--r--   0        0        0     2558 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/group_vars/hosts.yml
--rw-r--r--   0        0        0      129 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/group_vars/mother.yml
--rw-r--r--   0        0        0     1015 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/initialize-services.yml
--rw-r--r--   0        0        0     2430 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/iptables.yml
--rw-r--r--   0        0        0     2479 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/push-image.yml
--rw-r--r--   0        0        0     3107 2023-06-23 13:30:01.659441 hive_builder-3.6.7/hive_builder/playbooks/roles/aws/tasks/build-aws.yml
--rw-r--r--   0        0        0     3627 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/aws/tasks/create_instance.yml
--rw-r--r--   0        0        0     2665 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml
--rw-r--r--   0        0        0      327 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/aws/tasks/main.yml
--rw-r--r--   0        0        0      217 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/aws/tasks/stop-aws.yml
--rw-r--r--   0        0        0       46 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/aws/templates/aws_cli_config.j2
--rw-r--r--   0        0        0      102 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/aws/templates/aws_cli_credentials.j2
--rw-r--r--   0        0        0      138 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/aws/templates/azure_cli_credentials.j2
--rw-r--r--   0        0        0      138 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/aws/templates/cloudstack.ini.j2
--rw-r--r--   0        0        0     1497 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/aws/vars/main.yml
--rw-r--r--   0        0        0     3273 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/azure/tasks/build-azure.yml
--rw-r--r--   0        0        0     3434 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/azure/tasks/create_instance.yml
--rw-r--r--   0        0        0     1932 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml
--rw-r--r--   0        0        0      326 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/azure/tasks/main.yml
--rw-r--r--   0        0        0      297 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/azure/tasks/stop-azure.yml
--rw-r--r--   0        0        0      647 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/azure/vars/main.yml
--rw-r--r--   0        0        0      589 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/backup-tools/tasks/main.yml
--rw-r--r--   0        0        0      179 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/backup-tools/templates/backup.service
--rw-r--r--   0        0        0      126 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/backup-tools/templates/backup.timer
--rw-r--r--   0        0        0     5210 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh
--rw-r--r--   0        0        0       85 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/base/files/NetworkManager-wait-online.service.d/override.conf
--rw-r--r--   0        0        0     1210 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml
--rw-r--r--   0        0        0     1796 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/base/tasks/growfs.yml
--rw-r--r--   0        0        0     6801 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/base/tasks/main.yml
--rw-r--r--   0        0        0       77 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/ca/files/extfile.cnf
--rw-r--r--   0        0        0     1290 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/ca/tasks/main.yml
--rw-r--r--   0        0        0      268 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/ca/vars/main.yml
--rw-r--r--   0        0        0     4726 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker/tasks/main.yml
--rw-r--r--   0        0        0      321 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker/templates/daemon.json.j2
--rw-r--r--   0        0        0      331 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker/templates/override.conf
--rw-r--r--   0        0        0     2301 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client/tasks/main.yml
--rw-r--r--   0        0        0     1770 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client/templates/dcp
--rw-r--r--   0        0        0     1467 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client/templates/dexec
--rw-r--r--   0        0        0      678 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client/templates/dsh
--rw-r--r--   0        0        0      170 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client/vars/main.yml
--rw-r--r--   0        0        0     1032 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml
--rw-r--r--   0        0        0      233 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client-proxy/templates/config.json.j2
--rw-r--r--   0        0        0      147 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/docker-compose/tasks/main.yml
--rw-r--r--   0        0        0      229 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/drbd/files/drbd-resource@.service
--rw-r--r--   0        0        0      309 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/drbd/files/waitdevice
--rw-r--r--   0        0        0     3060 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/drbd/tasks/main.yml
--rw-r--r--   0        0        0     3381 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/drbd/tasks/vg.yml
--rw-r--r--   0        0        0      442 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/drbd/vars/main.yml
--rw-r--r--   0        0        0     5426 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml
--rw-r--r--   0        0        0     1568 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/drbd-resource/templates/volume.res
--rw-r--r--   0        0        0      421 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/drbd-resource/vars/main.yml
--rw-r--r--   0        0        0    27684 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py
--rw-r--r--   0        0        0     1411 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml
--rw-r--r--   0        0        0      309 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/follow-swarm-service/templates/follow-swarm-service.service
--rw-r--r--   0        0        0     2850 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml
--rw-r--r--   0        0        0     3021 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml
--rw-r--r--   0        0        0     3289 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml
--rw-r--r--   0        0        0      314 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/gcp/tasks/main.yml
--rw-r--r--   0        0        0      396 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/gcp/tasks/stop-gcp.yml
--rw-r--r--   0        0        0      741 2023-06-23 13:30:01.663441 hive_builder-3.6.7/hive_builder/playbooks/roles/gcp/vars/main.yml
--rw-r--r--   0        0        0      338 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/hostsfile/tasks/main.yml
--rw-r--r--   0        0        0     1403 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/internal-network/tasks/main.yml
--rw-r--r--   0        0        0      625 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/iptables/tasks/main.yml
--rw-r--r--   0        0        0     4319 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/kickstart/tasks/main.yml
--rw-r--r--   0        0        0     3345 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2
--rw-r--r--   0        0        0      171 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/kickstart/vars/main.yml
--rw-r--r--   0        0        0      118 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/monitor-service-log/handlers/main.yml
--rw-r--r--   0        0        0      875 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml
--rw-r--r--   0        0        0     1017 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2
--rw-r--r--   0        0        0     2436 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml
--rw-r--r--   0        0        0     2001 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml
--rw-r--r--   0        0        0     2528 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml
--rw-r--r--   0        0        0      531 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/ntp-client/tasks/main.yml
--rw-r--r--   0        0        0     2650 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/pip-venv/tasks/main.yml
--rw-r--r--   0        0        0      403 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/prepared/tasks/main.yml
--rw-r--r--   0        0        0      665 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/prepared/tasks/setup.yml
--rw-r--r--   0        0        0       79 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/prepared/vars/main.yml
--rw-r--r--   0        0        0      394 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/reboot/handlers/main.yml
--rw-r--r--   0        0        0     1712 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/registry/tasks/main.yml
--rw-r--r--   0        0        0       57 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/registry/templates/daemon.json.j2
--rw-r--r--   0        0        0      985 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/registry/templates/registry.yml.j2
--rw-r--r--   0        0        0      118 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/rsyslogd/handlers/main.yml
--rw-r--r--   0        0        0     1338 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml
--rw-r--r--   0        0        0     3184 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/rsyslogd/templates/services.conf
--rw-r--r--   0        0        0      788 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/service-backup/tasks/main.yml
--rw-r--r--   0        0        0     5337 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2
--rw-r--r--   0        0        0     1148 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml
--rw-r--r--   0        0        0     6226 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/swarm/tasks/main.yml
--rw-r--r--   0        0        0      220 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/tls-certificate/handlers/main.yml
--rw-r--r--   0        0        0     2912 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml
--rw-r--r--   0        0        0      188 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/tls-certificate/templates/extfile.cnf
--rw-r--r--   0        0        0      508 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/tls-certificate/vars/main.yml
--rw-r--r--   0        0        0      433 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/users/tasks/known-hosts.yml
--rw-r--r--   0        0        0     1157 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/users/tasks/main.yml
--rw-r--r--   0        0        0       40 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/users/templates/sudoer.j2
--rw-r--r--   0        0        0     3160 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/vagrant/files/Vagrantfile
--rw-r--r--   0        0        0     1078 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/vagrant/files/growfs.sh
--rw-r--r--   0        0        0     2413 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/vagrant/tasks/main.yml
--rw-r--r--   0        0        0     1116 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2
--rw-r--r--   0        0        0     3414 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml
--rw-r--r--   0        0        0     8115 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml
--rw-r--r--   0        0        0     1601 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml
--rw-r--r--   0        0        0     2337 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/files/hive-server.xml
--rw-r--r--   0        0        0     4694 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/tasks/main.yml
--rw-r--r--   0        0        0     2638 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2
--rw-r--r--   0        0        0      269 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/vars/main.yml
--rw-r--r--   0        0        0      144 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/ausearch.conf
--rw-r--r--   0        0        0    14795 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py
--rw-r--r--   0        0        0     1337 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py
--rw-r--r--   0        0        0      269 2023-06-23 13:30:01.667441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/drbd-resource.conf
--rw-r--r--   0        0        0     6520 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/hive.te
--rw-r--r--   0        0        0     4960 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn
--rw-r--r--   0        0        0      115 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/service_discovery_blacklist
--rw-r--r--   0        0        0       62 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/sudoers.zabbix
--rw-r--r--   0        0        0      360 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/userparameter_systemd_services.conf
--rw-r--r--   0        0        0      739 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh
--rw-r--r--   0        0        0      461 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_restart_check.sh
--rw-r--r--   0        0        0      389 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/handlers/main.yml
--rw-r--r--   0        0        0     6203 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml
--rw-r--r--   0        0        0     1397 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2
--rw-r--r--   0        0        0      345 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/templates/docker-volume.j2
--rw-r--r--   0        0        0      354 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.service
--rw-r--r--   0        0        0      196 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.timer
--rw-r--r--   0        0        0    10611 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2
--rw-r--r--   0        0        0      681 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml
--rw-r--r--   0        0        0     2482 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/playbooks/setup-hosts.yml
--rw-r--r--   0        0        0    20038 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/plugins/hive_inventory.py
--rw-r--r--   0        0        0    14761 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/plugins/hive_services.py
--rw-r--r--   0        0        0      235 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/requirements.yml
--rw-r--r--   0        0        0    11579 2023-06-23 13:30:01.675441 hive_builder-3.6.7/hive_builder/variables_metainf.yml
--rw-r--r--   0        0        0      633 2023-06-23 13:30:01.675441 hive_builder-3.6.7/pyproject.toml
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 hive_builder-3.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-05 01:42:50.382812 hive_builder-3.6.8/LICENSE
+-rw-r--r--   0        0        0     1231 2023-07-05 01:42:50.382812 hive_builder-3.6.8/README.md
+-rwxr-xr-x   0        0        0      312 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/__init__.py
+-rw-r--r--   0        0        0     1031 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/hive-completion.sh
+-rw-r--r--   0        0        0    26952 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/hive.py
+-rw-r--r--   0        0        0    14020 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/lib/azure_rm_storageshare.py
+-rw-r--r--   0        0        0    14954 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/lib/hive_vagrant.py
+-rw-r--r--   0        0        0     5832 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/build-images.yml
+-rw-r--r--   0        0        0     1943 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/build-infra.yml
+-rw-r--r--   0        0        0     1084 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/build-networks.yml
+-rw-r--r--   0        0        0     2447 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/build-volumes.yml
+-rw-r--r--   0        0        0       81 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/addon/tasks/main.yml
+-rw-r--r--   0        0        0       40 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-certificate/files/extfile.cnf
+-rw-r--r--   0        0        0     1783 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml
+-rw-r--r--   0        0        0      356 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-syslog/tasks/main.yml
+-rw-r--r--   0        0        0      946 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2
+-rw-r--r--   0        0        0      650 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml
+-rw-r--r--   0        0        0      351 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/tasks/main.yml
+-rw-r--r--   0        0        0       49 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/vars/main.yml
+-rw-r--r--   0        0        0      323 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/tasks/main.yml
+-rw-r--r--   0        0        0       49 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/vars/main.yml
+-rw-r--r--   0        0        0      409 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/tasks/main.yml
+-rw-r--r--   0        0        0       49 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/vars/main.yml
+-rw-r--r--   0        0        0      274 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/python-aptk/tasks/main.yml
+-rw-r--r--   0        0        0     9564 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/deploy-services.yml
+-rw-r--r--   0        0        0     2558 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/group_vars/hosts.yml
+-rw-r--r--   0        0        0      129 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/group_vars/mother.yml
+-rw-r--r--   0        0        0     1015 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/initialize-services.yml
+-rw-r--r--   0        0        0     2430 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/iptables.yml
+-rw-r--r--   0        0        0     2479 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/push-image.yml
+-rw-r--r--   0        0        0     3107 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/build-aws.yml
+-rw-r--r--   0        0        0     3627 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/create_instance.yml
+-rw-r--r--   0        0        0     2665 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml
+-rw-r--r--   0        0        0      327 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/main.yml
+-rw-r--r--   0        0        0      217 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/stop-aws.yml
+-rw-r--r--   0        0        0       46 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/templates/aws_cli_config.j2
+-rw-r--r--   0        0        0      102 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/templates/aws_cli_credentials.j2
+-rw-r--r--   0        0        0      138 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/templates/azure_cli_credentials.j2
+-rw-r--r--   0        0        0      138 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/templates/cloudstack.ini.j2
+-rw-r--r--   0        0        0     1497 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/vars/main.yml
+-rw-r--r--   0        0        0     3273 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/build-azure.yml
+-rw-r--r--   0        0        0     3434 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/create_instance.yml
+-rw-r--r--   0        0        0     1932 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml
+-rw-r--r--   0        0        0      326 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/main.yml
+-rw-r--r--   0        0        0      297 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/stop-azure.yml
+-rw-r--r--   0        0        0      647 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/vars/main.yml
+-rw-r--r--   0        0        0      589 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/tasks/main.yml
+-rw-r--r--   0        0        0      179 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/templates/backup.service
+-rw-r--r--   0        0        0      126 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/templates/backup.timer
+-rw-r--r--   0        0        0     5210 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh
+-rw-r--r--   0        0        0       85 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/base/files/NetworkManager-wait-online.service.d/override.conf
+-rw-r--r--   0        0        0     1210 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml
+-rw-r--r--   0        0        0     1796 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/growfs.yml
+-rw-r--r--   0        0        0     6801 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/main.yml
+-rw-r--r--   0        0        0       77 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/ca/files/extfile.cnf
+-rw-r--r--   0        0        0     1290 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/ca/tasks/main.yml
+-rw-r--r--   0        0        0      268 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/ca/vars/main.yml
+-rw-r--r--   0        0        0     4726 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker/tasks/main.yml
+-rw-r--r--   0        0        0      321 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker/templates/daemon.json.j2
+-rw-r--r--   0        0        0      331 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker/templates/override.conf
+-rw-r--r--   0        0        0     2301 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/tasks/main.yml
+-rw-r--r--   0        0        0     1770 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dcp
+-rw-r--r--   0        0        0     1467 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dexec
+-rw-r--r--   0        0        0      678 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dsh
+-rw-r--r--   0        0        0      170 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/vars/main.yml
+-rw-r--r--   0        0        0     1032 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml
+-rw-r--r--   0        0        0      233 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client-proxy/templates/config.json.j2
+-rw-r--r--   0        0        0      147 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-compose/tasks/main.yml
+-rw-r--r--   0        0        0      229 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/files/drbd-resource@.service
+-rw-r--r--   0        0        0      309 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/files/waitdevice
+-rw-r--r--   0        0        0     3060 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/tasks/main.yml
+-rw-r--r--   0        0        0     3381 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/tasks/vg.yml
+-rw-r--r--   0        0        0      442 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/vars/main.yml
+-rw-r--r--   0        0        0     5426 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml
+-rw-r--r--   0        0        0     1568 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd-resource/templates/volume.res
+-rw-r--r--   0        0        0      421 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd-resource/vars/main.yml
+-rw-r--r--   0        0        0    27684 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py
+-rw-r--r--   0        0        0     1411 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml
+-rw-r--r--   0        0        0      309 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/follow-swarm-service/templates/follow-swarm-service.service
+-rw-r--r--   0        0        0     2850 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml
+-rw-r--r--   0        0        0     3021 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml
+-rw-r--r--   0        0        0     3289 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml
+-rw-r--r--   0        0        0      314 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/main.yml
+-rw-r--r--   0        0        0      396 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/stop-gcp.yml
+-rw-r--r--   0        0        0      741 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/vars/main.yml
+-rw-r--r--   0        0        0      338 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/hostsfile/tasks/main.yml
+-rw-r--r--   0        0        0     1403 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/internal-network/tasks/main.yml
+-rw-r--r--   0        0        0      625 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/iptables/tasks/main.yml
+-rw-r--r--   0        0        0     4319 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/kickstart/tasks/main.yml
+-rw-r--r--   0        0        0     3345 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2
+-rw-r--r--   0        0        0      171 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/kickstart/vars/main.yml
+-rw-r--r--   0        0        0      118 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/monitor-service-log/handlers/main.yml
+-rw-r--r--   0        0        0      875 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml
+-rw-r--r--   0        0        0     1017 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2
+-rw-r--r--   0        0        0     2436 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml
+-rw-r--r--   0        0        0     2001 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml
+-rw-r--r--   0        0        0     2528 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml
+-rw-r--r--   0        0        0      531 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/ntp-client/tasks/main.yml
+-rw-r--r--   0        0        0     2650 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/pip-venv/tasks/main.yml
+-rw-r--r--   0        0        0      403 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/prepared/tasks/main.yml
+-rw-r--r--   0        0        0      665 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/prepared/tasks/setup.yml
+-rw-r--r--   0        0        0       79 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/prepared/vars/main.yml
+-rw-r--r--   0        0        0      394 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/reboot/handlers/main.yml
+-rw-r--r--   0        0        0     1712 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/registry/tasks/main.yml
+-rw-r--r--   0        0        0       57 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/registry/templates/daemon.json.j2
+-rw-r--r--   0        0        0      985 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/registry/templates/registry.yml.j2
+-rw-r--r--   0        0        0      118 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/rsyslogd/handlers/main.yml
+-rw-r--r--   0        0        0     1338 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml
+-rw-r--r--   0        0        0     3184 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/rsyslogd/templates/services.conf
+-rw-r--r--   0        0        0      788 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/service-backup/tasks/main.yml
+-rw-r--r--   0        0        0     5337 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2
+-rw-r--r--   0        0        0     1148 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml
+-rw-r--r--   0        0        0     7628 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/swarm/tasks/main.yml
+-rw-r--r--   0        0        0      220 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/tls-certificate/handlers/main.yml
+-rw-r--r--   0        0        0     2912 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml
+-rw-r--r--   0        0        0      188 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/tls-certificate/templates/extfile.cnf
+-rw-r--r--   0        0        0      508 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/tls-certificate/vars/main.yml
+-rw-r--r--   0        0        0      433 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/users/tasks/known-hosts.yml
+-rw-r--r--   0        0        0     1157 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/users/tasks/main.yml
+-rw-r--r--   0        0        0       40 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/users/templates/sudoer.j2
+-rw-r--r--   0        0        0     3160 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/files/Vagrantfile
+-rw-r--r--   0        0        0     1078 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/files/growfs.sh
+-rw-r--r--   0        0        0     2413 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/tasks/main.yml
+-rw-r--r--   0        0        0     1116 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2
+-rw-r--r--   0        0        0     3414 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml
+-rw-r--r--   0        0        0     8115 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml
+-rw-r--r--   0        0        0     1601 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml
+-rw-r--r--   0        0        0     2337 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-server.xml
+-rw-r--r--   0        0        0     4694 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/tasks/main.yml
+-rw-r--r--   0        0        0     2638 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2
+-rw-r--r--   0        0        0      269 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/vars/main.yml
+-rw-r--r--   0        0        0      144 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/ausearch.conf
+-rw-r--r--   0        0        0    14795 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py
+-rw-r--r--   0        0        0     1337 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py
+-rw-r--r--   0        0        0      269 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/drbd-resource.conf
+-rw-r--r--   0        0        0     6520 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/hive.te
+-rw-r--r--   0        0        0     4960 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn
+-rw-r--r--   0        0        0      115 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/service_discovery_blacklist
+-rw-r--r--   0        0        0       62 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/sudoers.zabbix
+-rw-r--r--   0        0        0      360 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/userparameter_systemd_services.conf
+-rw-r--r--   0        0        0      739 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh
+-rw-r--r--   0        0        0      461 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_restart_check.sh
+-rw-r--r--   0        0        0      389 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/handlers/main.yml
+-rw-r--r--   0        0        0     6203 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml
+-rw-r--r--   0        0        0     1397 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2
+-rw-r--r--   0        0        0      345 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/docker-volume.j2
+-rw-r--r--   0        0        0      354 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.service
+-rw-r--r--   0        0        0      196 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.timer
+-rw-r--r--   0        0        0    10611 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2
+-rw-r--r--   0        0        0      681 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml
+-rw-r--r--   0        0        0     2482 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/setup-hosts.yml
+-rw-r--r--   0        0        0    20038 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/plugins/hive_inventory.py
+-rw-r--r--   0        0        0    14761 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/plugins/hive_services.py
+-rw-r--r--   0        0        0      235 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/requirements.yml
+-rw-r--r--   0        0        0    11579 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/variables_metainf.yml
+-rw-r--r--   0        0        0      633 2023-07-05 01:42:50.402812 hive_builder-3.6.8/pyproject.toml
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 hive_builder-3.6.8/PKG-INFO
```

### Comparing `hive_builder-3.6.7/LICENSE` & `hive_builder-3.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/README.md` & `hive_builder-3.6.8/README.md`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/hive-completion.sh` & `hive_builder-3.6.8/hive_builder/hive-completion.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/hive.py` & `hive_builder-3.6.8/hive_builder/hive.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/lib/azure_rm_storageshare.py` & `hive_builder-3.6.8/hive_builder/lib/azure_rm_storageshare.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/lib/hive_vagrant.py` & `hive_builder-3.6.8/hive_builder/lib/hive_vagrant.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/build-images.yml` & `hive_builder-3.6.8/hive_builder/playbooks/build-images.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/build-infra.yml` & `hive_builder-3.6.8/hive_builder/playbooks/build-infra.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/build-networks.yml` & `hive_builder-3.6.8/hive_builder/playbooks/build-networks.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/build-volumes.yml` & `hive_builder-3.6.8/hive_builder/playbooks/build-volumes.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2` & `hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/deploy-services.yml` & `hive_builder-3.6.8/hive_builder/playbooks/deploy-services.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/group_vars/hosts.yml` & `hive_builder-3.6.8/hive_builder/playbooks/group_vars/hosts.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/initialize-services.yml` & `hive_builder-3.6.8/hive_builder/playbooks/initialize-services.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/iptables.yml` & `hive_builder-3.6.8/hive_builder/playbooks/iptables.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/push-image.yml` & `hive_builder-3.6.8/hive_builder/playbooks/push-image.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/aws/tasks/build-aws.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/build-aws.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/aws/tasks/create_instance.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/create_instance.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/aws/vars/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/aws/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/azure/tasks/build-azure.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/build-azure.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/azure/tasks/create_instance.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/create_instance.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/azure/vars/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/azure/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/backup-tools/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh` & `hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/base/tasks/growfs.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/growfs.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/base/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/ca/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/ca/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/docker/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/docker/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client/templates/dcp` & `hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dcp`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client/templates/dexec` & `hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dexec`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client/templates/dsh` & `hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dsh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/drbd/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/drbd/tasks/vg.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/tasks/vg.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/drbd-resource/templates/volume.res` & `hive_builder-3.6.8/hive_builder/playbooks/roles/drbd-resource/templates/volume.res`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py` & `hive_builder-3.6.8/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/gcp/vars/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/internal-network/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/internal-network/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/iptables/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/iptables/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/kickstart/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/kickstart/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2` & `hive_builder-3.6.8/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2` & `hive_builder-3.6.8/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/ntp-client/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/ntp-client/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/pip-venv/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/pip-venv/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/prepared/tasks/setup.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/prepared/tasks/setup.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/registry/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/registry/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/registry/templates/registry.yml.j2` & `hive_builder-3.6.8/hive_builder/playbooks/roles/registry/templates/registry.yml.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/rsyslogd/templates/services.conf` & `hive_builder-3.6.8/hive_builder/playbooks/roles/rsyslogd/templates/services.conf`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/service-backup/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/service-backup/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2` & `hive_builder-3.6.8/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/swarm/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/swarm/tasks/main.yml`

 * *Files 15% similar despite different names*

```diff
@@ -59,22 +59,60 @@
   iptables:
     ip_version: ipv6
     table: nat
     chain: OUTPUT
     jump: DOCKER
   when: hive_internal_cidr_v6 is defined
 
-- name: add masquarade rule for nat table 1
-  iptables:
-    ip_version: ipv6
-    table: nat
-    chain: POSTROUTING
-    jump: MASQUERADE
-    out_interface: docker_gwbridge
-  when: hive_internal_cidr_v6 is defined
+- name: check masqrade rule for nat table exists
+  shell: /usr/sbin/ip6tables-save | fgrep -q 'addrtype --src-type LOCAL'
+  check_mode: False
+  failed_when: False
+  changed_when: False
+  register: check
+  become: yes
+  when: hive_internal_cidr_v6 is defined
+
+- name: insert rule
+  shell: ip6tables -t nat -I POSTROUTING -o docker_gwbridge -s ::/0 -d ::/0 -m addrtype --src-type LOCAL -j MASQUERADE  
+  become: yes
+  when: check.rc != 0 and hive_internal_cidr_v6 is defined
+
+- name: insert masquarade rule in filter table for docker_gwbridge and make setting persistent
+  blockinfile:
+    dest: /etc/sysconfig/ip6tables
+    insertafter: "^:OUTPUT ACCEPT"
+    block: |
+      -N DOCKER
+      -A FORWARD -o docker_gwbridge -m conntrack --ctstate RELATED,ESTABLISHED -j ACCEPT 
+      -A FORWARD -o docker_gwbridge -j DOCKER
+      -A FORWARD -i docker_gwbridge ! -o docker_gwbridge -j ACCEPT
+      -A FORWARD -i docker_gwbridge -o docker_gwbridge -j DROP
+    marker: "# {mark} HIVE-BUILDER MANAGED BLOCK for IPv6 in docker_gwbridge for filter table"
+  when: hive_internal_cidr_v6 is defined
+
+- name: insert masquarade rule in nat table for docker_gwbridge and make setting persistent
+  blockinfile:
+    dest: /etc/sysconfig/ip6tables
+    insertafter: EOF
+    block: |
+      *nat
+      -N DOCKER
+      -I POSTROUTING ! -o docker_gwbridge -s {{subnet_v6}} -d ::/0 -j MASQUERADE
+      -I POSTROUTING -o docker_gwbridge -s ::/0 -d ::/0 -m addrtype --src-type LOCAL -j MASQUERADE
+      -I OUTPUT -p all -j DOCKER
+      -I PREROUTING -j DOCKER
+      COMMIT
+    marker: "# {mark} HIVE-BUILDER MANAGED BLOCK for IPv6 in docker_gwbridge for nat table"
+  when: hive_internal_cidr_v6 is defined
+
+- name: Enable service ip6tables
+  service:
+    name: ip6tables
+    enabled: yes
 
 - name: add masquarade rule for nat table 2
   iptables:
     ip_version: ipv6
     table: nat
     chain: POSTROUTING
     jump: MASQUERADE
@@ -127,21 +165,14 @@
     ip_version: ipv6
     chain: FORWARD
     jump: DROP
     in_interface : docker_gwbridge
     out_interface : docker_gwbridge
   when: hive_internal_cidr_v6 is defined
 
-- name: set forward policy to DROP
-  iptables:
-    ip_version: ipv6
-    chain: FORWARD
-    policy: DROP
-  when: hive_internal_cidr_v6 is defined
-
 - name: initialize master node
   shell: "docker swarm init --advertise-addr {{ hive_private_ip }}"
   when: "'first_hive' in group_names and hive_docker_info.stdout == 'inactive'"
   register: swarm_init
 
 - name: remove ingress subnet
   shell: "yes | docker network rm ingress"
```

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/users/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/users/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/vagrant/files/Vagrantfile` & `hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/files/Vagrantfile`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/vagrant/files/growfs.sh` & `hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/files/growfs.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/vagrant/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2` & `hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/files/hive-server.xml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-server.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/hive.te` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/hive.te`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml` & `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/playbooks/setup-hosts.yml` & `hive_builder-3.6.8/hive_builder/playbooks/setup-hosts.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/plugins/hive_inventory.py` & `hive_builder-3.6.8/hive_builder/plugins/hive_inventory.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/hive_builder/plugins/hive_services.py` & `hive_builder-3.6.8/hive_builder/plugins/hive_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,17 +169,17 @@
     if 'volumes' in self.options or self.options.get('standalone', False):
       volumes_value = self.options.get('volumes', AnsibleSequence([]))
       if type(volumes_value) != AnsibleSequence:
         raise AnsibleParserError(f'"volumes" must be list type in service {self.name}, but {type(volumes_value)}')
       volumes = []
       if self.options.get('standalone', False):
         volumes = [
-            {'source': '/sys/fs/cgroup', 'target': '/sys/fs/cgroup', 'readonly': True},
             {'source': '', 'target': '/run', 'type': 'tmpfs'},
-            {'source': '', 'target': '/tmp', 'type': 'tmpfs'}
+            {'source': '', 'target': '/tmp', 'type': 'tmpfs'},
+            {'source': '/sys/fs/cgroup', 'target': '/sys/fs/cgroup', 'readonly': True}
         ]
       for volume in volumes_value:
         if type(volume) == AnsibleUnicode:
           raise AnsibleParserError(f'we do not support short syntax {text_type(volume)} in volume at service {self.name}')
         elif type(volume) == AnsibleMapping:
           if 'source' not in volume or 'target' not in volume:
               raise AnsibleParserError(f'both "source" and "target" must be specified in volume at service {self.name}')
```

### Comparing `hive_builder-3.6.7/hive_builder/variables_metainf.yml` & `hive_builder-3.6.8/hive_builder/variables_metainf.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.7/pyproject.toml` & `hive_builder-3.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hive-builder"
-version = "3.6.7"
+version = "3.6.8"
 description = "Building docker swarm environment"
 authors = ["Mitsuru Nakakawaj <mitsuru@procube.jp>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "hive_builder"}]
 
 [tool.poetry.dependencies]
```

### Comparing `hive_builder-3.6.7/PKG-INFO` & `hive_builder-3.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-builder
-Version: 3.6.7
+Version: 3.6.8
 Summary: Building docker swarm environment
 License: MIT
 Author: Mitsuru Nakakawaj
 Author-email: mitsuru@procube.jp
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

