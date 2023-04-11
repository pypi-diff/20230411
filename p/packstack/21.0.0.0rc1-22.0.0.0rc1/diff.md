# Comparing `tmp/packstack-21.0.0.0rc1.tar.gz` & `tmp/packstack-22.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packstack-21.0.0.0rc1.tar", last modified: Thu Oct 20 13:41:32 2022, max compression
+gzip compressed data, was "packstack-22.0.0.0rc1.tar", last modified: Tue Apr 11 16:00:36 2023, max compression
```

## Comparing `packstack-21.0.0.0rc1.tar` & `packstack-22.0.0.0rc1.tar`

### file list

```diff
@@ -1,371 +1,371 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.061824 packstack-21.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/.testr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9283 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5501 2022-10-20 13:41:31.000000 packstack-21.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    74200 2022-10-20 13:41:31.000000 packstack-21.0.0.0rc1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/Gemfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11345 2022-10-20 13:41:32.061824 packstack-21.0.0.0rc1/PKG-INFO
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3783 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/Puppetfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8303 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/Rakefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.997824 packstack-21.0.0.0rc1/docs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5576 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/docs/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8548 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/docs/conf.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    54829 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/docs/packstack.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.997824 packstack-21.0.0.0rc1/packstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.001824 packstack-21.0.0.0rc1/packstack/installer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3649 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/basedefs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.005824 packstack-21.0.0.0rc1/packstack/installer/core/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/core/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/core/arch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15319 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/core/drones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2170 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/core/parameters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3650 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/core/sequences.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2167 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5765 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/output_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5264 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/processors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40967 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/run_setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5347 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/setup_controller.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.005824 packstack-21.0.0.0rc1/packstack/installer/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4379 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/utils/datastructures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1382 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/utils/decorators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4447 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/utils/network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/utils/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/utils/shortcuts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/utils/strings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/installer/validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.005824 packstack-21.0.0.0rc1/packstack/modules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/modules/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/modules/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2816 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/modules/documentation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6529 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/modules/ospluginutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/modules/puppet.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.013824 packstack-21.0.0.0rc1/packstack/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/amqp_002.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4082 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/aodh_810.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7677 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/ceilometer_800.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28691 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/cinder_250.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7836 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/dashboard_500.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4612 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/glance_200.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3495 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/gnocchi_790.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6709 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/heat_650.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3805 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/ironic_275.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26987 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/keystone_100.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4040 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/magnum_920.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24727 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/manila_355.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/mariadb_003.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40818 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/neutron_350.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20087 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/nova_300.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/openstack_client_400.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2295 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/postscript_951.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    54002 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/prescript_000.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17382 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/provision_700.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11822 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/puppet_950.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3845 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/sahara_900.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11565 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/ssl_001.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11752 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/swift_600.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5575 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/plugins/trove_850.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.993824 packstack-21.0.0.0rc1/packstack/puppet/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.989824 packstack-21.0.0.0rc1/packstack/puppet/modules/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.013824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/Gemfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/Rakefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.989824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.013824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/default_hypervisor.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/home_dir.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/mariadb.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8175 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns_support.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/network.rb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.989824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.989824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.017824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/choose_my_ip.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_interface.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_ip.rb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.021824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.021824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2219 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/enable_rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.021824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1556 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/apache.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.021824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/nova_disabled.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1457 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/chrony.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.021824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.025824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/lvm.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8184 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/netapp.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/nfs.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/solidfire.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/vmdk.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backup.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2114 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/firewall.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.025824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.025824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/file.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/swift.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1472 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1764 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/gnocchi.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.025824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/cfn.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2237 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2678 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/horizon.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.025824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.029824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/aodh.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/cinder.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/glance.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/gnocchi.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/heat.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/ironic.pp
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      586 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/magnum.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/manila.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/neutron.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/nova.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/placement.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/sahara.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/swift.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/trove.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6814 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.029824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1313 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1613 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.029824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.029824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1652 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/generic.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternative.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternfs.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/netapp.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/network.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1470 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.029824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3685 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services.pp
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18244 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services_remote.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2436 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/memcached.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/netns.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.033824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/api.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1475 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/bridge.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/dhcp.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/l3.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/lb_agent.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/metadata.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/metering.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ml2.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/notifications.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_agent.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_metadata.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_northd.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_agent.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_bridge.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/sriov.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/vpnaas.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.037824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3790 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/api.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.037824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/common.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.037824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/ironic.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/libvirt.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/vmware.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4234 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/conductor.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/metadata.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/neutron.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/nfs.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.037824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched/ironic.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/vncproxy.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3093 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2963 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/openstackclient.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/placement.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/prereqs.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.037824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1995 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/bridge.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/glance.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7480 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/tempest.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3925 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/redis.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.037824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2099 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.037824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/fs.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3447 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/proxy.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ringbuilder.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/storage.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.037824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.037824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/spec/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/spec/spec_helper.rb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.993824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.993824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.993824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.037824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/choose_my_ip_spec.rb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.041824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/templates/openstack-neutron.modules.erb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.041824 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1753 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/generate_ssl_certs.sh.erb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.041824 packstack-21.0.0.0rc1/packstack/puppet/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/templates/compute.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5787 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/templates/controller.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/templates/controller_post.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/puppet/templates/network.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/packstack/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.001824 packstack-21.0.0.0rc1/packstack.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11345 2022-10-20 13:41:31.000000 packstack-21.0.0.0rc1/packstack.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15446 2022-10-20 13:41:31.000000 packstack-21.0.0.0rc1/packstack.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-10-20 13:41:31.000000 packstack-21.0.0.0rc1/packstack.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-10-20 13:41:31.000000 packstack-21.0.0.0rc1/packstack.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-10-20 13:41:31.000000 packstack-21.0.0.0rc1/packstack.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-10-20 13:41:31.000000 packstack-21.0.0.0rc1/packstack.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2022-10-20 13:41:31.000000 packstack-21.0.0.0rc1/packstack.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2022-10-20 13:41:31.000000 packstack-21.0.0.0rc1/packstack.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.041824 packstack-21.0.0.0rc1/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/playbooks/packstack-centos9-pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/playbooks/packstack-integration-tempest.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/playbooks/packstack-multinode.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/playbooks/packstack-post-compute.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/playbooks/upload-logs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.993824 packstack-21.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.057824 packstack-21.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/Add-Panko-service-63a8a966013abeaa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/Panko-has-been-removed-fb234a047231d84f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/Remove-CONFIG_NEUTRON_ML2_SUPPORTED_PCI_VENDOR_DEVS-param-926649e4eef08b44.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/Remove-FWaaS-deployment-41cfa0b709cd9a3f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/Remove-Heat-Cloudwatch-07e55f1c35a16ee4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/Remove-PKI-and-UUID-Keystone-token-formats-618f4b0dc4cf782f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/Remove-deprecated-keystone-ldap-params-848d0eaf7a24273e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/Replace-keystone-token-flush-cron-job-with-fernet-rotation-5b1fccf2bc6add91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/Support-for-extracted-placement-service-8ae75efbb1ad25b5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/add-parameter-messages-47d9cf6996f58230.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/add-skip-tempest-tests-option-86cf59ec5a61d349.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/add-support-to-ovn-networking-ae6e0176270265c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/add_cinder_solidfire-9b62f78b86a52a09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/admin-token-removed-64ae39c4ecd28f15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/aodh-move-to-mariadb-9e36b7cfdbbd2aa5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/bp-add-magnum-support-74d88638fe4b2c6c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/ceilometer-with-wsgi-a46d2ff0ceabaaf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/change-default-nagios-b190de0737165bf9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/check-unexpected-options-2f2d26ebe54da6c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/create-uec-image-70073744430d1538.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/custom-tempest-flavors-baa5cf02235f78dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/demo-allocation-pools-c535e4235c7edcb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/demo-image-properties-9994f2981a8c00a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/disable-rabbitmq-repositories-d5cb9dc8f1246a39.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/drop-mongodb-a9771fb4f0430a4c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/gnocchi-and-aodh-00da52a4c45588fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/install-tempest-from-rpm-fd59c072011f372b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/integration-tests-d5f86a29cc037329.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/keystone-evenlet-dropped-6f85670db62f7b91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/keystone-v3-note-065b6302b49285f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/l3-agent-multiple-networks-9d1837c4187055be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/manifest-execution-refactor-418c27bbc03df064.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/move-to-pymysql-b5f1a40ededa8fb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/neutron-ovs-bridges-compute-0aec0e39c1b1b84b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/nova-cert-86fb2f0ddc53b032.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/nova-cpu-manager-8440f026c4a0165e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/nova-migration-improvements-85b208c2b45a3fbe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/nova-placement-api-acf32977978da6fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/ovs-bridges-on-network-nodes-890c51cbbddf8f1c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/ovs-tunnel-subnets-8955593d3004852e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/packstack-moved-from-stackforge-766c35141b5480c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/qpid-removal-f754f589e335ae0c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/register-satellite6-server-796a5f89b39386a4.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.993824 packstack-21.0.0.0rc1/releasenotes/notes/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.057824 packstack-21.0.0.0rc1/releasenotes/notes/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/releasenotes/notes/add-custom-lvm-name-090af5002950706d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-cinder-gluster-6c54d9f440424259.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-collector-api-5b494f09593197f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-config-gnocchi-install-ecfe10ce59f1d0da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-epel-support-3732f53a2e45d64c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-glance-registry-6076539ab6ce1a8b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-lbaas-0054d83972c5afcf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-legacy-nova-filters-d6e21a5e8f5c31a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-nagios-deployment-21362a84a3ac446f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-nova-network-8fe352ac6eb22ecb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-retry-filter-nova-05e84f3fd020d8ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/remove-uec-images-d876bd8c805d9633.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/renamed-ssl-subject-parameters-c2a52d17c349a59f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/reno-for-release-notes-66c17b84c946591f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/service-workers-and-mariadb-c2a6ba903f36b57e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/swift-s3-removal-ee3ddc2ee21a56cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/switch-default-neutron-driver-to-ovn-0eb7053b81c7794d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/notes/update-puppet-module-usage-4ed869e87e67caaf.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.057824 packstack-21.0.0.0rc1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.057824 packstack-21.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.057824 packstack-21.0.0.0rc1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8804 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.993824 packstack-21.0.0.0rc1/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:31.993824 packstack-21.0.0.0rc1/roles/packstack-integration-tempest/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.057824 packstack-21.0.0.0rc1/roles/packstack-integration-tempest/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/roles/packstack-integration-tempest/tasks/main.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11311 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2022-10-20 13:41:32.065824 packstack-21.0.0.0rc1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.057824 packstack-21.0.0.0rc1/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.061824 packstack-21.0.0.0rc1/tests/installer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/installer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/installer/test_arch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7721 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/installer/test_drones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1535 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/installer/test_processors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5203 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/installer/test_run_setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3226 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/installer/test_sequences.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/installer/test_setup_params.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4187 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/installer/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4300 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/installer/test_validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.061824 packstack-21.0.0.0rc1/tests/modules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/modules/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/modules/test_ospluginutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/modules/test_puppet.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1297 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/scenario-py3.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      265 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/scenario000.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1396 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/scenario001.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1497 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/scenario002.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1269 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/scenario003.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5552 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tests/test_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-10-20 13:41:32.061824 packstack-21.0.0.0rc1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5250 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tools/copy-logs.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3711 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tools/fix_disk_layout.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1184 2022-10-20 13:41:03.000000 packstack-21.0.0.0rc1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.989063 packstack-22.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9469 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5501 2023-04-11 16:00:36.000000 packstack-22.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    74512 2023-04-11 16:00:36.000000 packstack-22.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/Gemfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11345 2023-04-11 16:00:36.989063 packstack-22.0.0.0rc1/PKG-INFO
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3783 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/Puppetfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8303 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/Rakefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.925062 packstack-22.0.0.0rc1/docs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5576 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/docs/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8548 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/docs/conf.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    54829 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/docs/packstack.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.925062 packstack-22.0.0.0rc1/packstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.929062 packstack-22.0.0.0rc1/packstack/installer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3649 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/basedefs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.929062 packstack-22.0.0.0rc1/packstack/installer/core/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/core/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/core/arch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15319 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/core/drones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2170 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/core/parameters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3650 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/core/sequences.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2167 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5765 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/output_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5264 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/processors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40967 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/run_setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5347 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/setup_controller.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.929062 packstack-22.0.0.0rc1/packstack/installer/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4379 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/utils/datastructures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1382 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/utils/decorators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4447 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/utils/network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/utils/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/utils/shortcuts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/utils/strings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/installer/validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.933062 packstack-22.0.0.0rc1/packstack/modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/modules/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/modules/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2816 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/modules/documentation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6529 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/modules/ospluginutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/modules/puppet.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.937062 packstack-22.0.0.0rc1/packstack/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/amqp_002.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4082 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/aodh_810.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7677 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/ceilometer_800.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28691 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/cinder_250.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7836 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/dashboard_500.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4612 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/glance_200.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3495 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/gnocchi_790.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6709 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/heat_650.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3805 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/ironic_275.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26987 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/keystone_100.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4040 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/magnum_920.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24727 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/manila_355.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/mariadb_003.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40818 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/neutron_350.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20087 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/nova_300.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/openstack_client_400.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2295 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/postscript_951.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    54002 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/prescript_000.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17382 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/provision_700.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11822 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/puppet_950.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3845 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/sahara_900.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11565 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/ssl_001.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11752 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/swift_600.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5575 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/plugins/trove_850.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.917062 packstack-22.0.0.0rc1/packstack/puppet/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.913062 packstack-22.0.0.0rc1/packstack/puppet/modules/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.937062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/Gemfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/Rakefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.913062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.941062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/default_hypervisor.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/home_dir.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/mariadb.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8175 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns_support.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/network.rb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.913062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.913062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.941062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/choose_my_ip.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_interface.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_ip.rb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.945062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.945062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2219 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/enable_rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.945062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1556 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/apache.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.949062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/nova_disabled.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1457 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/chrony.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.949062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.949062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/lvm.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8184 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/netapp.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/nfs.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/solidfire.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/vmdk.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backup.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2251 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/firewall.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.949062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.949062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/file.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/swift.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1472 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1764 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/gnocchi.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.949062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/cfn.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2678 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/horizon.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.949062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.953063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/aodh.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/cinder.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/glance.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/gnocchi.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/heat.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/ironic.pp
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      586 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/magnum.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/manila.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/neutron.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/nova.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/placement.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/sahara.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/swift.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/trove.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6766 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.953063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1313 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1613 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.953063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.957063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1661 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/generic.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternative.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternfs.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/netapp.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/network.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1470 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.957063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3685 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services.pp
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18244 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services_remote.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2436 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/memcached.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/netns.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.961063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/api.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1475 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/bridge.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/dhcp.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/l3.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/lb_agent.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/metadata.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/metering.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ml2.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/notifications.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_agent.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_metadata.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_northd.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_agent.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_bridge.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/sriov.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/vpnaas.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.961063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3790 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/api.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.961063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/common.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.961063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/ironic.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/libvirt.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/vmware.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4234 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/conductor.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/metadata.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/neutron.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/nfs.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.961063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched/ironic.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/vncproxy.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3093 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2963 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/openstackclient.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/placement.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/prereqs.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.965063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1995 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/bridge.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/glance.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7480 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/tempest.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3940 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/redis.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.965063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2099 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.965063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/fs.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3447 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/proxy.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ringbuilder.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/storage.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.965063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.965063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/spec/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/spec/spec_helper.rb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.917062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.917062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.917062 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.965063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/choose_my_ip_spec.rb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.965063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/templates/openstack-neutron.modules.erb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.965063 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1753 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/generate_ssl_certs.sh.erb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.969063 packstack-22.0.0.0rc1/packstack/puppet/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/templates/compute.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5787 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/templates/controller.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/templates/controller_post.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/puppet/templates/network.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/packstack/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.925062 packstack-22.0.0.0rc1/packstack.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11345 2023-04-11 16:00:36.000000 packstack-22.0.0.0rc1/packstack.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15446 2023-04-11 16:00:36.000000 packstack-22.0.0.0rc1/packstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-11 16:00:36.000000 packstack-22.0.0.0rc1/packstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2023-04-11 16:00:36.000000 packstack-22.0.0.0rc1/packstack.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-11 16:00:36.000000 packstack-22.0.0.0rc1/packstack.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-04-11 16:00:36.000000 packstack-22.0.0.0rc1/packstack.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-04-11 16:00:36.000000 packstack-22.0.0.0rc1/packstack.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2023-04-11 16:00:36.000000 packstack-22.0.0.0rc1/packstack.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.969063 packstack-22.0.0.0rc1/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/playbooks/packstack-centos9-pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/playbooks/packstack-integration-tempest.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/playbooks/packstack-multinode.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/playbooks/packstack-post-compute.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/playbooks/upload-logs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.917062 packstack-22.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.981063 packstack-22.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/Add-Panko-service-63a8a966013abeaa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/Panko-has-been-removed-fb234a047231d84f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/Remove-CONFIG_NEUTRON_ML2_SUPPORTED_PCI_VENDOR_DEVS-param-926649e4eef08b44.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/Remove-FWaaS-deployment-41cfa0b709cd9a3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/Remove-Heat-Cloudwatch-07e55f1c35a16ee4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/Remove-PKI-and-UUID-Keystone-token-formats-618f4b0dc4cf782f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/Remove-deprecated-keystone-ldap-params-848d0eaf7a24273e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/Replace-keystone-token-flush-cron-job-with-fernet-rotation-5b1fccf2bc6add91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/Support-for-extracted-placement-service-8ae75efbb1ad25b5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/add-parameter-messages-47d9cf6996f58230.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/add-skip-tempest-tests-option-86cf59ec5a61d349.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/add-support-to-ovn-networking-ae6e0176270265c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/add_cinder_solidfire-9b62f78b86a52a09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/admin-token-removed-64ae39c4ecd28f15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/aodh-move-to-mariadb-9e36b7cfdbbd2aa5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/bp-add-magnum-support-74d88638fe4b2c6c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/ceilometer-with-wsgi-a46d2ff0ceabaaf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/change-default-nagios-b190de0737165bf9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/check-unexpected-options-2f2d26ebe54da6c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/create-uec-image-70073744430d1538.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/custom-tempest-flavors-baa5cf02235f78dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/demo-allocation-pools-c535e4235c7edcb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/demo-image-properties-9994f2981a8c00a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/disable-rabbitmq-repositories-d5cb9dc8f1246a39.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/drop-mongodb-a9771fb4f0430a4c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/gnocchi-and-aodh-00da52a4c45588fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/install-tempest-from-rpm-fd59c072011f372b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/integration-tests-d5f86a29cc037329.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/keystone-evenlet-dropped-6f85670db62f7b91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/keystone-v3-note-065b6302b49285f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/l3-agent-multiple-networks-9d1837c4187055be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/manifest-execution-refactor-418c27bbc03df064.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/move-to-pymysql-b5f1a40ededa8fb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/neutron-ovs-bridges-compute-0aec0e39c1b1b84b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/nova-cert-86fb2f0ddc53b032.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/nova-cpu-manager-8440f026c4a0165e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/nova-migration-improvements-85b208c2b45a3fbe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/nova-placement-api-acf32977978da6fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/ovs-bridges-on-network-nodes-890c51cbbddf8f1c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/ovs-tunnel-subnets-8955593d3004852e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/packstack-moved-from-stackforge-766c35141b5480c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/qpid-removal-f754f589e335ae0c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/register-satellite6-server-796a5f89b39386a4.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.917062 packstack-22.0.0.0rc1/releasenotes/notes/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.981063 packstack-22.0.0.0rc1/releasenotes/notes/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/releasenotes/notes/add-custom-lvm-name-090af5002950706d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-cinder-gluster-6c54d9f440424259.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-collector-api-5b494f09593197f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-config-gnocchi-install-ecfe10ce59f1d0da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-epel-support-3732f53a2e45d64c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-glance-registry-6076539ab6ce1a8b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-lbaas-0054d83972c5afcf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-legacy-nova-filters-d6e21a5e8f5c31a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-nagios-deployment-21362a84a3ac446f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-nova-network-8fe352ac6eb22ecb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-retry-filter-nova-05e84f3fd020d8ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/remove-uec-images-d876bd8c805d9633.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/renamed-ssl-subject-parameters-c2a52d17c349a59f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/reno-for-release-notes-66c17b84c946591f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/service-workers-and-mariadb-c2a6ba903f36b57e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/swift-s3-removal-ee3ddc2ee21a56cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/switch-default-neutron-driver-to-ovn-0eb7053b81c7794d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/notes/update-puppet-module-usage-4ed869e87e67caaf.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.985063 packstack-22.0.0.0rc1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.985063 packstack-22.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.985063 packstack-22.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8804 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.917062 packstack-22.0.0.0rc1/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.917062 packstack-22.0.0.0rc1/roles/packstack-integration-tempest/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.985063 packstack-22.0.0.0rc1/roles/packstack-integration-tempest/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/roles/packstack-integration-tempest/tasks/main.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11311 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2023-04-11 16:00:36.993063 packstack-22.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.985063 packstack-22.0.0.0rc1/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.989063 packstack-22.0.0.0rc1/tests/installer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/installer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/installer/test_arch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7721 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/installer/test_drones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1535 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/installer/test_processors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5203 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/installer/test_run_setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3226 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/installer/test_sequences.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/installer/test_setup_params.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4187 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/installer/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4300 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/installer/test_validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.989063 packstack-22.0.0.0rc1/tests/modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/modules/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/modules/test_ospluginutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/modules/test_puppet.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1297 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/scenario-py3.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      265 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/scenario000.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1396 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/scenario001.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1497 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/scenario002.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1269 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/scenario003.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5552 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tests/test_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-11 16:00:36.989063 packstack-22.0.0.0rc1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5250 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tools/copy-logs.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3711 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tools/fix_disk_layout.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2023-04-11 16:00:08.000000 packstack-22.0.0.0rc1/tox.ini
```

### Comparing `packstack-21.0.0.0rc1/.zuul.yaml` & `packstack-22.0.0.0rc1/.zuul.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -85,19 +85,19 @@
     name: packstack-centos9s-multinode-scenario002-tempest
     parent: packstack-multinode-centos9
     post-run: playbooks/packstack-post-compute.yaml
     vars:
       scenario: scenario002
 
 - secret:
-    name: packstack_git_mirror_credentials
+    name: packstack_git_mirror_credentials_master
     data:
       user: git
       host: github.com
-      host_key: github.com ssh-rsa AAAAB3NzaC1yc2EAAAABIwAAAQEAq2A7hRGmdnm9tUDbO9IDSwBK6TbQa+PXYPCPy6rbTrTtw7PHkccKrpp0yVhp5HdEIcKr6pLlVDBfOLX9QUsyCOV0wzfjIJNlGEYsdlLJizHhbn2mUjvSAHQqZETYP81eFzLQNnPHt4EVVUh7VfDESU84KezmD5QlWpXLmvU31/yMf+Se8xhHTvKSCZIFImWwoG6mbUoWf9nzpIoaSjB+weqqUUmpaaasXVal72J+UX2B+2RPW3RcT0eOzQgqlJL3RKrTJvdsjE3JEAvGq3lGHSZXy28G3skua2SmVi/w4yCE6gbODqnTWlg7+wC604ydGXA8VJiS5ap43JXiUFFAaQ==
+      host_key: github.com ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCj7ndNxQowgcQnjshcLrqPEiiphnt+VTTvDP6mHBL9j1aNUkY4Ue1gvwnGLVlOhGeYrnZaMgRK6+PKCUXaDbC7qtbW8gIkhL7aGCsOr/C56SJMy/BCZfxd1nWzAOxSDPgVsmerOBYfNqltV9/hWCqBywINIR+5dIg6JTJ72pcEpEjcYgXkE2YEFXV1JHnsKgbLWNlhScqb2UmyRkQyytRLtL+38TGxkxCflmO+5Z8CSSNY7GidjMIZ7Q4zMjA2n1nGrlTDkzwDCsw+wqFPGQA179cnfGWOWRVruj16z6XyvxvjJwbz0wQZ75XK5tKSb7FNyeIEs4TT4jk+S4dhPeAUC5y+bDYirYgM4GC7uEnztnZyaVWQ7B381AK4Qdrwt51ZqExKbQpTUNn+EjqoTwvqNj4kqx5QUCI0ThS/YkOxJCXmPUWZbhjpCg56i+2aB6CmK2JGhn57K5mj0MNdBXA4/WnwH6XoPWJzK5Nyu2zB3nAZp+S5hpQs+p1vN1/wsjk=
       ssh_key: !encrypted/pkcs1-oaep
         - Rd6fA6jCgfkqHDdNFG4abPZlnsV7mc8ki0AZDANf7dZmopQONSKVVmP7uQ15b57vB8BiK
           Crk4TP0yJEDZBjOSlwGywHbEE0UhGNQU6Gm13XDE0U7gvPJ1kWqMxmDRXr96f0ibpNuNL
           B112HZS09FSMklx+FhGFsQoZMr8xutVbmCcSHZnKPY50Sa6KrgIuvlCyL9/Py5zDEBNaZ
           dGD9mirxn8nP8GzVmRl+r43ccc1BoVRgM0uAoQCROBabvdF6iV8x3JKKAjX0tCDZFpdQG
           uCUNY2+E4fBEOlVrX4Oc3PzO2YkiqaPbu5oMrs56qXlZ3TCiu8EDadatU6FaSjTT96wSL
           XoOLOqO+5yZ/n4WMua07ANbjj6Q2lvysoemJNUWKMkFhTEhVlNTOx/wnZMeJaIS+eKRDN
@@ -161,15 +161,15 @@
     parent: upload-git-mirror
     description: Mirrors x/packstack to redhat-openstack/packstack
     allowed-projects: x/packstack
     vars:
       git_mirror_repository: redhat-openstack/packstack
     secrets:
       - name: git_mirror_credentials
-        secret: packstack_git_mirror_credentials
+        secret: packstack_git_mirror_credentials_master
         pass-to-parent: true
 
 - project:
     check:
       jobs:
         - openstack-tox-pep8
         - openstack-tox-py39
```

### Comparing `packstack-21.0.0.0rc1/AUTHORS` & `packstack-22.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/ChangeLog` & `packstack-22.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 CHANGES
 =======
 
-21.0.0.0rc1
+22.0.0.0rc1
 -----------
 
+* Update github host keys
+* Move to project\_ terminology used in current Keystone v3 API
+* Enable snapshots in NFS backends and add nova section
+* Replace deprecated defined resource type of Manila
+* Heat: Use separate class to manage [trustee] options
+* Remove enable\_ssl from keystone.pp
+
+21.0.0
+------
+
 * Ceilometer: Remove redundant installation of pythonN-redis
 * Establish order between redis and aodh and ceilometer
 * Fix dependency between redis and gnocchi services
 * Ceilometer: Use built-in class to run ceilometer-upgrade
 * Drop firewall rule for ceilometer-api
 * Start redis before gnocchi-metricd when coordination uses redis
 * Gnocchi: Fix missing coordination backend
@@ -494,16 +504,16 @@
 * Add release notes for the Mitaka cycle
 * Try setting the tuned profile more than once
 * Fix mode for rabbitmq.config
 * Start managing release notes in Packstack with Reno
 * Configure gnocchi statsd service
 * Make ceilometer metering backend configurable
 
-8.0.0rc1
---------
+8.0.0.0rc1
+----------
 
 * Deploy ceilometer api as wsgi
 * Add libyaml-devel to list of dependencies
 * Add a switch to install from source or binary
 * Allow arbitrary amount of lines between Subscription Name and Pool ID
 * Do not enable RabbitMQ repo during installation
 * Replacing keystone user-list with openstack user list
```

### Comparing `packstack-21.0.0.0rc1/Gemfile` & `packstack-22.0.0.0rc1/Gemfile`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/LICENSE` & `packstack-22.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/PKG-INFO` & `packstack-22.0.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packstack
-Version: 21.0.0.0rc1
+Version: 22.0.0.0rc1
 Summary: A utility to install OpenStack
 Home-page: http://www.rdoproject.org/
 Author: RDO
 Author-email: rdo-list@redhat.com
 License: UNKNOWN
 Description: Packstack
         =========
```

### Comparing `packstack-21.0.0.0rc1/Puppetfile` & `packstack-22.0.0.0rc1/Puppetfile`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/README.rst` & `packstack-22.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/Rakefile` & `packstack-22.0.0.0rc1/Rakefile`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/docs/Makefile` & `packstack-22.0.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/docs/conf.py` & `packstack-22.0.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/docs/packstack.rst` & `packstack-22.0.0.0rc1/docs/packstack.rst`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/LICENSE` & `packstack-22.0.0.0rc1/packstack/installer/LICENSE`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/basedefs.py` & `packstack-22.0.0.0rc1/packstack/installer/basedefs.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/core/arch.py` & `packstack-22.0.0.0rc1/packstack/installer/core/arch.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/core/drones.py` & `packstack-22.0.0.0rc1/packstack/installer/core/drones.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/core/parameters.py` & `packstack-22.0.0.0rc1/packstack/installer/core/parameters.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/core/sequences.py` & `packstack-22.0.0.0rc1/packstack/installer/core/sequences.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/exceptions.py` & `packstack-22.0.0.0rc1/packstack/installer/exceptions.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/output_messages.py` & `packstack-22.0.0.0rc1/packstack/installer/output_messages.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/processors.py` & `packstack-22.0.0.0rc1/packstack/installer/processors.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/run_setup.py` & `packstack-22.0.0.0rc1/packstack/installer/run_setup.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/setup_controller.py` & `packstack-22.0.0.0rc1/packstack/installer/setup_controller.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/utils/__init__.py` & `packstack-22.0.0.0rc1/packstack/installer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/utils/datastructures.py` & `packstack-22.0.0.0rc1/packstack/installer/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/utils/decorators.py` & `packstack-22.0.0.0rc1/packstack/installer/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/utils/network.py` & `packstack-22.0.0.0rc1/packstack/installer/utils/network.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/utils/shell.py` & `packstack-22.0.0.0rc1/packstack/installer/utils/shell.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/utils/shortcuts.py` & `packstack-22.0.0.0rc1/packstack/installer/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/utils/strings.py` & `packstack-22.0.0.0rc1/packstack/installer/utils/strings.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/installer/validators.py` & `packstack-22.0.0.0rc1/packstack/installer/validators.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/modules/common.py` & `packstack-22.0.0.0rc1/packstack/modules/common.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/modules/documentation.py` & `packstack-22.0.0.0rc1/packstack/modules/documentation.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/modules/ospluginutils.py` & `packstack-22.0.0.0rc1/packstack/modules/ospluginutils.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/modules/puppet.py` & `packstack-22.0.0.0rc1/packstack/modules/puppet.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/amqp_002.py` & `packstack-22.0.0.0rc1/packstack/plugins/amqp_002.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/aodh_810.py` & `packstack-22.0.0.0rc1/packstack/plugins/aodh_810.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/ceilometer_800.py` & `packstack-22.0.0.0rc1/packstack/plugins/ceilometer_800.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/cinder_250.py` & `packstack-22.0.0.0rc1/packstack/plugins/cinder_250.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/dashboard_500.py` & `packstack-22.0.0.0rc1/packstack/plugins/dashboard_500.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/glance_200.py` & `packstack-22.0.0.0rc1/packstack/plugins/glance_200.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/gnocchi_790.py` & `packstack-22.0.0.0rc1/packstack/plugins/gnocchi_790.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/heat_650.py` & `packstack-22.0.0.0rc1/packstack/plugins/heat_650.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/ironic_275.py` & `packstack-22.0.0.0rc1/packstack/plugins/ironic_275.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/keystone_100.py` & `packstack-22.0.0.0rc1/packstack/plugins/keystone_100.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/magnum_920.py` & `packstack-22.0.0.0rc1/packstack/plugins/magnum_920.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/manila_355.py` & `packstack-22.0.0.0rc1/packstack/plugins/manila_355.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/mariadb_003.py` & `packstack-22.0.0.0rc1/packstack/plugins/mariadb_003.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/neutron_350.py` & `packstack-22.0.0.0rc1/packstack/plugins/neutron_350.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/nova_300.py` & `packstack-22.0.0.0rc1/packstack/plugins/nova_300.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/openstack_client_400.py` & `packstack-22.0.0.0rc1/packstack/plugins/openstack_client_400.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/postscript_951.py` & `packstack-22.0.0.0rc1/packstack/plugins/postscript_951.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/prescript_000.py` & `packstack-22.0.0.0rc1/packstack/plugins/prescript_000.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/provision_700.py` & `packstack-22.0.0.0rc1/packstack/plugins/provision_700.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/puppet_950.py` & `packstack-22.0.0.0rc1/packstack/plugins/puppet_950.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/sahara_900.py` & `packstack-22.0.0.0rc1/packstack/plugins/sahara_900.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/ssl_001.py` & `packstack-22.0.0.0rc1/packstack/plugins/ssl_001.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/swift_600.py` & `packstack-22.0.0.0rc1/packstack/plugins/swift_600.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/plugins/trove_850.py` & `packstack-22.0.0.0rc1/packstack/plugins/trove_850.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns.py` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/choose_my_ip.rb` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/choose_my_ip.rb`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_interface.rb` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_interface.rb`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/enable_rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/enable_rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/apache.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/apache.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/chrony.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/chrony.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/lvm.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/lvm.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/netapp.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/netapp.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/solidfire.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/solidfire.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder.pp`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,19 @@
 
     class { 'cinder::scheduler': }
 
     class { 'cinder::volume': }
 
     class { 'cinder::client': }
 
+    class { 'cinder::nova':
+      password => lookup('CONFIG_NOVA_KS_PW'),
+      auth_url => lookup('CONFIG_KEYSTONE_ADMIN_URL'),
+    }
+
     $cinder_keystone_admin_username = lookup('CONFIG_KEYSTONE_ADMIN_USERNAME')
     $cinder_keystone_admin_password = lookup('CONFIG_KEYSTONE_ADMIN_PW')
     $cinder_keystone_auth_url = lookup('CONFIG_KEYSTONE_PUBLIC_URL')
     $cinder_keystone_api = lookup('CONFIG_KEYSTONE_API_VERSION')
 
     class { 'cinder::backends':
       enabled_backends => lookup('CONFIG_CINDER_BACKEND', { merge => 'unique' }),
```

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/firewall.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/firewall.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/swift.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/swift.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/ceilometer.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/ceilometer.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/gnocchi.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/gnocchi.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/cfn.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/cfn.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/rabbitmq.pp`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
     if lookup('CONFIG_CEILOMETER_INSTALL') == 'y' {
       $heat_notification_driver = 'messagingv2'
     } else {
       $heat_notification_driver = $::os_service_default
     }
 
+    class { 'heat::trustee':
+      password => lookup('CONFIG_HEAT_KS_PW'),
+      auth_url => lookup('CONFIG_KEYSTONE_ADMIN_URL'),
+    }
     class { 'heat::keystone::authtoken':
       password             => lookup('CONFIG_HEAT_KS_PW'),
       www_authenticate_uri => lookup('CONFIG_KEYSTONE_PUBLIC_URL'),
       auth_url             => lookup('CONFIG_KEYSTONE_ADMIN_URL'),
     }
 
     class { 'heat::logging':
```

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/horizon.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/horizon.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/cinder.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/cinder.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/heat.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/heat.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/magnum.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/magnum.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/manila.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/manila.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/placement.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/placement.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/swift.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/swift.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone.pp`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
       database_connection => "mysql+pymysql://keystone_admin:${keystone_cfg_ks_db_pw}@${keystone_cfg_mariadb_host}/keystone",
     }
 
     class { 'keystone':
       token_provider      => $keystone_token_provider_str,
       enable_fernet_setup => true,
       service_name        => 'httpd',
-      enable_ssl          => $keystone_use_ssl,
       default_domain      => 'Default',
     }
 
     class { 'keystone::wsgi::apache':
       workers => lookup('CONFIG_SERVICE_WORKERS'),
       ssl     => $keystone_use_ssl
     }
```

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/generic.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/generic.pp`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       ensure  => present,
       id      => '66',
       ram     => '512',
       disk    => '1',
       vcpus   => '1',
       require => [ Class['::nova::api'], Class['::nova::keystone::auth'] ],
     }
-    -> manila::service_instance{ 'generic':
+    -> manila::backend::service_instance{ 'generic':
       service_image_location     => lookup('CONFIG_MANILA_SERVICE_IMAGE_LOCATION'),
       service_instance_user      => lookup('CONFIG_MANILA_SERVICE_INSTANCE_USER'),
       service_instance_password  => lookup('CONFIG_MANILA_SERVICE_INSTANCE_PASSWORD'),
       service_instance_flavor_id => 66,
     }
 
     class { 'manila::compute::nova':
```

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternfs.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternfs.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/netapp.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/netapp.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/network.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/network.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services_remote.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services_remote.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/api.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/api.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/bridge.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/bridge.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/lb_agent.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/lb_agent.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ml2.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ml2.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_agent.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_agent.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_metadata.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_metadata.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_agent.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_agent.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/api.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/api.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/libvirt.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/libvirt.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/neutron.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/neutron.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/openstackclient.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/openstackclient.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/placement.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/placement.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/bridge.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/bridge.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/glance.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/glance.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/tempest.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/tempest.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision.pp`

 * *Files 8% similar despite different names*

```diff
@@ -4,52 +4,52 @@
     $provision_tempest         = str2bool(lookup('CONFIG_PROVISION_TEMPEST'))
     $provision_neutron         = str2bool(lookup('CONFIG_NEUTRON_INSTALL'))
     $heat_available            = str2bool(lookup('CONFIG_HEAT_INSTALL'))
 
     if $provision_demo {
       $username             = 'demo'
       $password             = lookup('CONFIG_KEYSTONE_DEMO_PW')
-      $tenant_name          = 'demo'
+      $project_name         = 'demo'
       $floating_range       = lookup('CONFIG_PROVISION_DEMO_FLOATRANGE')
       $allocation_pools     = lookup('CONFIG_PROVISION_DEMO_ALLOCATION_POOLS')
     } elsif $provision_tempest {
       $username             = lookup('CONFIG_PROVISION_TEMPEST_USER')
       $password             = lookup('CONFIG_PROVISION_TEMPEST_USER_PW')
-      $tenant_name          = 'tempest'
+      $project_name         = 'tempest'
       $floating_range       = lookup('CONFIG_PROVISION_TEMPEST_FLOATRANGE')
       $allocation_pools     = []
       if (empty($username) or empty($password)) {
         fail("Both CONFIG_PROVISION_TEMPEST_USER and
         CONFIG_PROVISION_TEMPEST_USER_PW need to be configured.")
       }
     }
 
     if $provision_demo or $provision_tempest {
 
       # Keystone
-      $admin_tenant_name = 'admin'
-      keystone_tenant { $tenant_name:
+      $admin_project_name = 'admin'
+      keystone_tenant { $project_name:
         ensure      => present,
         enabled     => true,
         description => 'default tenant',
       }
 
       keystone_user { $username:
         ensure   => present,
         enabled  => true,
         password => $password,
       }
 
       if $heat_available {
-        keystone_user_role { "${username}@${tenant_name}":
+        keystone_user_role { "${username}@${project_name}":
           ensure => present,
           roles  => ['_member_', 'heat_stack_owner'],
         }
       } else {
-        keystone_user_role { "${username}@${tenant_name}":
+        keystone_user_role { "${username}@${project_name}":
           ensure => present,
           roles  => ['_member_'],
         }
       }
 
       ## Neutron
       if $provision_neutron {
@@ -62,40 +62,40 @@
         $public_physnet       = lookup('CONFIG_NEUTRON_OVS_EXTERNAL_PHYSNET')
 
         $neutron_deps = [Neutron_network[$public_network_name]]
 
         neutron_network { $public_network_name:
           ensure                    => present,
           router_external           => true,
-          tenant_name               => $admin_tenant_name,
+          project_name              => $admin_project_name,
           provider_network_type     => 'flat',
           provider_physical_network => $public_physnet,
         }
         neutron_subnet { $public_subnet_name:
           ensure           => 'present',
           cidr             => $floating_range,
           allocation_pools => $allocation_pools,
           enable_dhcp      => false,
           network_name     => $public_network_name,
-          tenant_name      => $admin_tenant_name,
+          project_name     => $admin_project_name,
         }
         neutron_network { $private_network_name:
-          ensure      => present,
-          tenant_name => $tenant_name,
+          ensure       => present,
+          project_name => $project_name,
         }
         neutron_subnet { $private_subnet_name:
-          ensure       => present,
-          cidr         => $fixed_range,
-          network_name => $private_network_name,
-          tenant_name  => $tenant_name,
+          ensure        => present,
+          cidr          => $fixed_range,
+          network_name  => $private_network_name,
+          project_name  => $project_name,
         }
         # Tenant-owned router - assumes network namespace isolation
         neutron_router { $router_name:
           ensure               => present,
-          tenant_name          => $tenant_name,
+          project_name         => $project_name,
           gateway_network_name => $public_network_name,
           # A neutron_router resource must explicitly declare a dependency on
           # the first subnet of the gateway network.
           require              => Neutron_subnet[$public_subnet_name],
         }
         neutron_router_interface { "${router_name}:${private_subnet_name}":
           ensure => present,
```

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ceilometer.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ceilometer.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/proxy.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/proxy.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ringbuilder.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ringbuilder.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/storage.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/storage.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/rabbitmq.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove.pp` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove.pp`

 * *Files 6% similar despite different names*

```diff
@@ -35,11 +35,9 @@
       workers => lookup('CONFIG_SERVICE_WORKERS'),
     }
 
     class { 'trove::guestagent::service_credentials':
       password => lookup('CONFIG_TROVE_KS_PW'),
       auth_url => lookup('CONFIG_KEYSTONE_PUBLIC_URL_VERSIONLESS'),
     }
-    class { 'trove::taskmanager':
-      use_guestagent_template => false,
-    }
+    class { 'trove::taskmanager': }
 }
```

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/choose_my_ip_spec.rb` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/choose_my_ip_spec.rb`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/generate_ssl_certs.sh.erb` & `packstack-22.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/generate_ssl_certs.sh.erb`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/templates/compute.pp` & `packstack-22.0.0.0rc1/packstack/puppet/templates/compute.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/templates/controller.pp` & `packstack-22.0.0.0rc1/packstack/puppet/templates/controller.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/puppet/templates/network.pp` & `packstack-22.0.0.0rc1/packstack/puppet/templates/network.pp`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack/version.py` & `packstack-22.0.0.0rc1/packstack/version.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/packstack.egg-info/PKG-INFO` & `packstack-22.0.0.0rc1/packstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packstack
-Version: 21.0.0.0rc1
+Version: 22.0.0.0rc1
 Summary: A utility to install OpenStack
 Home-page: http://www.rdoproject.org/
 Author: RDO
 Author-email: rdo-list@redhat.com
 License: UNKNOWN
 Description: Packstack
         =========
```

### Comparing `packstack-21.0.0.0rc1/packstack.egg-info/SOURCES.txt` & `packstack-22.0.0.0rc1/packstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/playbooks/packstack-centos9-pre.yaml` & `packstack-22.0.0.0rc1/playbooks/packstack-centos9-pre.yaml`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/playbooks/packstack-multinode.yaml` & `packstack-22.0.0.0rc1/playbooks/packstack-multinode.yaml`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/releasenotes/notes/add-parameter-messages-47d9cf6996f58230.yaml` & `packstack-22.0.0.0rc1/releasenotes/notes/add-parameter-messages-47d9cf6996f58230.yaml`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/releasenotes/notes/add-support-to-ovn-networking-ae6e0176270265c6.yaml` & `packstack-22.0.0.0rc1/releasenotes/notes/add-support-to-ovn-networking-ae6e0176270265c6.yaml`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/releasenotes/notes/integration-tests-d5f86a29cc037329.yaml` & `packstack-22.0.0.0rc1/releasenotes/notes/integration-tests-d5f86a29cc037329.yaml`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/releasenotes/notes/l3-agent-multiple-networks-9d1837c4187055be.yaml` & `packstack-22.0.0.0rc1/releasenotes/notes/l3-agent-multiple-networks-9d1837c4187055be.yaml`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/releasenotes/notes/manifest-execution-refactor-418c27bbc03df064.yaml` & `packstack-22.0.0.0rc1/releasenotes/notes/manifest-execution-refactor-418c27bbc03df064.yaml`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/releasenotes/notes/remove-nova-network-8fe352ac6eb22ecb.yaml` & `packstack-22.0.0.0rc1/releasenotes/notes/remove-nova-network-8fe352ac6eb22ecb.yaml`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/releasenotes/notes/renamed-ssl-subject-parameters-c2a52d17c349a59f.yaml` & `packstack-22.0.0.0rc1/releasenotes/notes/renamed-ssl-subject-parameters-c2a52d17c349a59f.yaml`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/releasenotes/source/conf.py` & `packstack-22.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/run_tests.sh` & `packstack-22.0.0.0rc1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/setup.cfg` & `packstack-22.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/installer/test_arch.py` & `packstack-22.0.0.0rc1/tests/installer/test_arch.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/installer/test_drones.py` & `packstack-22.0.0.0rc1/tests/installer/test_drones.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/installer/test_processors.py` & `packstack-22.0.0.0rc1/tests/installer/test_processors.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/installer/test_run_setup.py` & `packstack-22.0.0.0rc1/tests/installer/test_run_setup.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/installer/test_sequences.py` & `packstack-22.0.0.0rc1/tests/installer/test_sequences.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/installer/test_setup_params.py` & `packstack-22.0.0.0rc1/tests/installer/test_setup_params.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/installer/test_utils.py` & `packstack-22.0.0.0rc1/tests/installer/test_utils.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/installer/test_validators.py` & `packstack-22.0.0.0rc1/tests/installer/test_validators.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/modules/test_ospluginutils.py` & `packstack-22.0.0.0rc1/tests/modules/test_ospluginutils.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/modules/test_puppet.py` & `packstack-22.0.0.0rc1/tests/modules/test_puppet.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/scenario-py3.sh` & `packstack-22.0.0.0rc1/tests/scenario-py3.sh`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/scenario001.sh` & `packstack-22.0.0.0rc1/tests/scenario001.sh`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/scenario002.sh` & `packstack-22.0.0.0rc1/tests/scenario002.sh`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/scenario003.sh` & `packstack-22.0.0.0rc1/tests/scenario003.sh`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tests/test_base.py` & `packstack-22.0.0.0rc1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tools/copy-logs.sh` & `packstack-22.0.0.0rc1/tools/copy-logs.sh`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tools/fix_disk_layout.sh` & `packstack-22.0.0.0rc1/tools/fix_disk_layout.sh`

 * *Files identical despite different names*

### Comparing `packstack-21.0.0.0rc1/tox.ini` & `packstack-22.0.0.0rc1/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tox]
 minversion = 2.0
 envlist = py27,py39,pep8,releasenotes
-skipsdist = True
+skipsdist = False
 
 [testenv]
 usedevelop = True
 setenv = VIRTUAL_ENV={envdir}
          LANG=en_US.UTF-8
          LANGUAGE=en_US:en
          LC_ALL=C
 deps =
   -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/test-requirements.txt
   -r{toxinidir}/requirements.txt
 
+allowlist_externals = /usr/bin/find
 commands = /usr/bin/find . -type f -name "*.pyc" -delete
            stestr run {posargs}
 
 [tox:jenkins]
 sitepackages = True
 
 [testenv:pep8]
```

