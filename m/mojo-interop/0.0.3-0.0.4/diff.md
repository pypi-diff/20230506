# Comparing `tmp/mojo_interop-0.0.3.tar.gz` & `tmp/mojo_interop-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_interop-0.0.3.tar", max compression
+gzip compressed data, was "mojo_interop-0.0.4.tar", max compression
```

## Comparing `mojo_interop-0.0.3.tar` & `mojo_interop-0.0.4.tar`

### file list

```diff
@@ -1,286 +1,284 @@
--rw-r--r--   0        0        0     1083 2023-04-30 20:18:46.226836 mojo_interop-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      434 2023-04-30 21:10:35.023558 mojo_interop-0.0.3/README.rst
--rw-r--r--   0        0        0      738 2023-05-04 03:15:54.501002 mojo_interop-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1630 2023-04-30 20:54:05.542332 mojo_interop-0.0.3/source/packages/mojo/factories/xmodsfactory.py
--rw-r--r--   0        0        0        0 2023-04-21 02:40:59.664563 mojo_interop-0.0.3/source/packages/mojo/interop/clients/base/__init__.py
--rw-r--r--   0        0        0     1256 2023-04-29 04:47:55.261890 mojo_interop-0.0.3/source/packages/mojo/interop/clients/base/baseclient.py
--rw-r--r--   0        0        0    11119 2023-04-29 04:59:09.638689 mojo_interop-0.0.3/source/packages/mojo/interop/clients/base/baseclientcoordinator.py
--rw-r--r--   0        0        0     7353 2023-05-04 03:15:14.049604 mojo_interop-0.0.3/source/packages/mojo/interop/clients/base/baseclientcoordinatorcoupling.py
--rw-r--r--   0        0        0      180 2023-04-23 00:21:47.238814 mojo_interop-0.0.3/source/packages/mojo/interop/clients/constants.py
--rw-r--r--   0        0        0        0 2023-04-26 04:50:59.262714 mojo_interop-0.0.3/source/packages/mojo/interop/clients/linux/__init__.py
--rw-r--r--   0        0        0      631 2023-04-29 04:52:31.831858 mojo_interop-0.0.3/source/packages/mojo/interop/clients/linux/linuxclient.py
--rw-r--r--   0        0        0     1409 2023-04-29 04:52:31.843858 mojo_interop-0.0.3/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py
--rw-r--r--   0        0        0     1309 2023-05-04 03:14:22.674410 mojo_interop-0.0.3/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py
--rw-r--r--   0        0        0        0 2023-04-21 02:40:59.664563 mojo_interop-0.0.3/source/packages/mojo/interop/clients/osx/__init__.py
--rw-r--r--   0        0        0      629 2023-04-29 04:52:31.843858 mojo_interop-0.0.3/source/packages/mojo/interop/clients/osx/osxclient.py
--rw-r--r--   0        0        0     1385 2023-04-29 04:52:31.847858 mojo_interop-0.0.3/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py
--rw-r--r--   0        0        0     1289 2023-05-04 03:13:42.847067 mojo_interop-0.0.3/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py
--rw-r--r--   0        0        0        0 2023-04-26 04:43:08.306443 mojo_interop-0.0.3/source/packages/mojo/interop/clients/windows/__init__.py
--rw-r--r--   0        0        0      633 2023-04-29 04:52:31.851858 mojo_interop-0.0.3/source/packages/mojo/interop/clients/windows/windowsclient.py
--rw-r--r--   0        0        0     1433 2023-04-29 04:52:31.851858 mojo_interop-0.0.3/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py
--rw-r--r--   0        0        0     1329 2023-05-04 03:14:09.238628 mojo_interop-0.0.3/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py
--rw-r--r--   0        0        0        0 2023-04-29 04:48:41.254217 mojo_interop-0.0.3/source/packages/mojo/interop/clusters/base/__init__.py
--rw-r--r--   0        0        0     1255 2023-04-29 04:50:19.978920 mojo_interop-0.0.3/source/packages/mojo/interop/clusters/base/basenode.py
--rw-r--r--   0        0        0    11028 2023-04-29 04:59:36.494880 mojo_interop-0.0.3/source/packages/mojo/interop/clusters/base/basenodecoordinator.py
--rw-r--r--   0        0        0     7340 2023-05-04 03:15:40.765203 mojo_interop-0.0.3/source/packages/mojo/interop/clusters/base/basenodecoordinatorcoupling.py
--rw-r--r--   0        0        0      519 2022-12-08 19:53:16.276698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/__init__.py
--rw-r--r--   0        0        0     2272 2023-04-30 21:03:13.691162 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsaddress.py
--rw-r--r--   0        0        0      639 2023-04-30 21:03:11.207140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsapi.py
--rw-r--r--   0        0        0     9720 2023-03-17 03:47:56.259994 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsconst.py
--rw-r--r--   0        0        0     2121 2023-04-30 21:03:11.207140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnshostinfo.py
--rw-r--r--   0        0        0     9274 2023-04-30 21:03:11.207140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py
--rw-r--r--   0        0        0    15537 2023-04-30 21:03:11.223140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py
--rw-r--r--   0        0        0     1862 2023-04-30 21:03:11.207140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnspointer.py
--rw-r--r--   0        0        0     2250 2023-04-30 21:03:11.207140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsquestion.py
--rw-r--r--   0        0        0      832 2023-03-16 05:21:20.896073 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py
--rw-r--r--   0        0        0     6850 2023-04-30 21:03:11.223140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsrecord.py
--rw-r--r--   0        0        0     3606 2023-04-30 21:03:11.223140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsserver.py
--rw-r--r--   0        0        0     2719 2023-04-30 21:03:11.207140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsservice.py
--rw-r--r--   0        0        0     2004 2023-04-30 21:03:11.207140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnstext.py
--rw-r--r--   0        0        0     3750 2023-04-30 21:03:11.207140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsutil.py
--rw-r--r--   0        0        0     2807 2023-04-30 21:03:11.207140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsvalidation.py
--rw-r--r--   0        0        0     1052 2023-03-17 15:51:43.102472 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/exceptions.py
--rw-r--r--   0        0        0     2615 2023-04-30 21:03:11.223140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/mdnsagent.py
--rw-r--r--   0        0        0     6279 2023-04-30 21:03:11.223140 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py
--rw-r--r--   0        0        0     2505 2023-03-17 06:36:21.314128 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py
--rw-r--r--   0        0        0     1294 2023-03-16 22:12:31.133035 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/testmessages.py
--rw-r--r--   0        0        0        0 2023-03-25 19:42:09.132533 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/power/dlipower/__init__.py
--rw-r--r--   0        0        0      894 2023-03-28 16:14:15.598469 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py
--rw-r--r--   0        0        0     3767 2023-03-28 16:14:15.598469 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py
--rw-r--r--   0        0        0     6138 2023-04-29 04:47:55.337890 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py
--rw-r--r--   0        0        0     7794 2023-03-25 18:55:12.050499 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/serial/tcpserialagent.py
--rw-r--r--   0        0        0     4913 2023-04-29 04:47:55.329891 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py
--rw-r--r--   0        0        0     6059 2023-04-29 04:47:55.333891 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py
--rw-r--r--   0        0        0     1398 2023-04-29 04:47:55.321890 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py
--rw-r--r--   0        0        0        0 2023-03-24 06:52:51.435618 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/ssh/__init__.py
--rw-r--r--   0        0        0    70641 2023-03-28 16:14:15.598469 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/ssh/sshagent.py
--rw-r--r--   0        0        0    12109 2023-04-29 04:47:55.353891 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py
--rw-r--r--   0        0        0     7541 2023-04-29 04:47:55.349891 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py
--rw-r--r--   0        0        0     1255 2023-04-29 04:47:55.353891 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/ssh/sshdevice.py
--rw-r--r--   0        0        0      540 2023-03-20 16:55:58.998382 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/__init__.py
--rw-r--r--   0        0        0      319 2023-03-20 16:55:58.990382 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/aliases.py
--rw-r--r--   0        0        0     2431 2023-03-21 07:47:58.411623 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/aspectsupnp.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/content/__init__.py
--rw-r--r--   0        0        0    15564 2023-03-21 07:49:16.837478 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/content/didllite.py
--rw-r--r--   0        0        0      557 2023-03-20 16:55:59.002382 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/devices/__init__.py
--rw-r--r--   0        0        0    14091 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py
--rw-r--r--   0        0        0     1761 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py
--rw-r--r--   0        0        0    44978 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py
--rw-r--r--   0        0        0      494 2023-03-20 16:55:59.002382 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/embeddeddevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/rootdevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/services/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/embeddeddevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/rootdevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/__init__.py
--rw-r--r--   0        0        0     3512 2023-04-30 20:52:11.401306 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py
--rw-r--r--   0        0        0     6222 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py
--rw-r--r--   0        0        0    11201 2023-04-30 20:52:11.657309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py
--rw-r--r--   0        0        0    11596 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py
--rw-r--r--   0        0        0    14933 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py
--rw-r--r--   0        0        0    20201 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py
--rw-r--r--   0        0        0    13583 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py
--rw-r--r--   0        0        0    16776 2023-04-30 20:52:11.589308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py
--rw-r--r--   0        0        0     6120 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py
--rw-r--r--   0        0        0    12568 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py
--rw-r--r--   0        0        0    17020 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py
--rw-r--r--   0        0        0     4574 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py
--rw-r--r--   0        0        0      630 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py
--rw-r--r--   0        0        0     4109 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py
--rw-r--r--   0        0        0    11330 2023-04-30 20:52:11.049303 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py
--rw-r--r--   0        0        0    12948 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py
--rw-r--r--   0        0        0     4161 2023-04-30 20:52:11.597308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py
--rw-r--r--   0        0        0     4161 2023-04-30 20:52:11.589308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py
--rw-r--r--   0        0        0     5719 2023-04-30 20:52:11.513307 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py
--rw-r--r--   0        0        0     9453 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py
--rw-r--r--   0        0        0    11449 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py
--rw-r--r--   0        0        0    13534 2023-04-30 20:52:11.597308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py
--rw-r--r--   0        0        0    23744 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py
--rw-r--r--   0        0        0     4429 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py
--rw-r--r--   0        0        0     7462 2023-04-30 20:52:11.657309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py
--rw-r--r--   0        0        0    10870 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py
--rw-r--r--   0        0        0     7731 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py
--rw-r--r--   0        0        0     8828 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py
--rw-r--r--   0        0        0    10006 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py
--rw-r--r--   0        0        0     2043 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py
--rw-r--r--   0        0        0     3992 2023-04-30 20:52:10.993303 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py
--rw-r--r--   0        0        0     4959 2023-04-30 20:52:11.573308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py
--rw-r--r--   0        0        0     3828 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py
--rw-r--r--   0        0        0     3166 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py
--rw-r--r--   0        0        0     2039 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py
--rw-r--r--   0        0        0     3577 2023-04-30 20:52:11.597308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py
--rw-r--r--   0        0        0     3071 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py
--rw-r--r--   0        0        0     4686 2023-04-30 20:52:11.657309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py
--rw-r--r--   0        0        0     9951 2023-04-30 20:52:11.597308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py
--rw-r--r--   0        0        0     1782 2023-04-30 20:52:11.597308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py
--rw-r--r--   0        0        0     8071 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py
--rw-r--r--   0        0        0     3931 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py
--rw-r--r--   0        0        0     3931 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py
--rw-r--r--   0        0        0    10240 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py
--rw-r--r--   0        0        0    10240 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py
--rw-r--r--   0        0        0     4675 2023-04-30 20:52:11.657309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py
--rw-r--r--   0        0        0     5801 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py
--rw-r--r--   0        0        0    11116 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py
--rw-r--r--   0        0        0     1691 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py
--rw-r--r--   0        0        0     3288 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py
--rw-r--r--   0        0        0     2107 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py
--rw-r--r--   0        0        0     2712 2023-04-30 20:52:11.189304 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py
--rw-r--r--   0        0        0     4718 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py
--rw-r--r--   0        0        0     5214 2023-04-30 20:52:11.657309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py
--rw-r--r--   0        0        0     5733 2023-04-30 20:52:11.321306 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py
--rw-r--r--   0        0        0     1751 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py
--rw-r--r--   0        0        0    20947 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py
--rw-r--r--   0        0        0    22560 2023-04-30 20:52:11.293305 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py
--rw-r--r--   0        0        0    26952 2023-04-30 20:52:11.657309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py
--rw-r--r--   0        0        0     7336 2023-04-30 20:52:11.261305 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py
--rw-r--r--   0        0        0    11158 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py
--rw-r--r--   0        0        0    11158 2023-04-30 20:52:11.597308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py
--rw-r--r--   0        0        0     9804 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py
--rw-r--r--   0        0        0    10325 2023-04-30 20:52:11.629308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py
--rw-r--r--   0        0        0     2199 2023-04-30 20:52:11.157304 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py
--rw-r--r--   0        0        0     3257 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py
--rw-r--r--   0        0        0     4234 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py
--rw-r--r--   0        0        0     7786 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py
--rw-r--r--   0        0        0     8132 2023-04-30 20:52:11.597308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py
--rw-r--r--   0        0        0     6178 2023-04-30 20:52:11.081303 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py
--rw-r--r--   0        0        0     1351 2023-04-30 20:52:11.217305 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py
--rw-r--r--   0        0        0    12414 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py
--rw-r--r--   0        0        0    15214 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py
--rw-r--r--   0        0        0     5133 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py
--rw-r--r--   0        0        0     6600 2023-04-30 20:52:11.657309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py
--rw-r--r--   0        0        0    17131 2023-04-30 20:52:11.601308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py
--rw-r--r--   0        0        0    30991 2023-04-30 20:52:11.633308 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/__init__.py
--rw-r--r--   0        0        0      479 2023-03-20 16:55:59.002382 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/dynamic/__init__.py
--rw-r--r--   0        0        0      247 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:BinaryLight:1.xml
--rw-r--r--   0        0        0      280 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DigitalSecurityCamera:1.xml
--rw-r--r--   0        0        0      420 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DimmableLight:1.xml
--rw-r--r--   0        0        0     1159 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml
--rw-r--r--   0        0        0     1865 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml
--rw-r--r--   0        0        0      459 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:1.xml
--rw-r--r--   0        0        0      604 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml
--rw-r--r--   0        0        0      208 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:LANDevice:1.xml
--rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:1.xml
--rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:2.xml
--rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml
--rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml
--rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml
--rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml
--rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml
--rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml
--rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml
--rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Printer:1.xml
--rw-r--r--   0        0        0      187 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAClient:1.xml
--rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:1.xml
--rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:2.xml
--rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:1.xml
--rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:2.xml
--rw-r--r--   0        0        0      300 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIClientDevice:1.xml
--rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIServerDevice:1.xml
--rw-r--r--   0        0        0      561 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml
--rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:1.xml
--rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:2.xml
--rw-r--r--   0        0        0      419 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:1.xml
--rw-r--r--   0        0        0      622 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml
--rw-r--r--   0        0        0      416 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:1.xml
--rw-r--r--   0        0        0      936 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml
--rw-r--r--   0        0        0     1090 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml
--rw-r--r--   0        0        0     1244 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml
--rw-r--r--   0        0        0      338 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:1.xml
--rw-r--r--   0        0        0      340 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:2.xml
--rw-r--r--   0        0        0      490 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WLANAccessPointDevice:1.xml
--rw-r--r--   0        0        0    21478 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml
--rw-r--r--   0        0        0    22506 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml
--rw-r--r--   0        0        0    32819 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml
--rw-r--r--   0        0        0     3894 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml
--rw-r--r--   0        0        0     5779 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml
--rw-r--r--   0        0        0    10054 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml
--rw-r--r--   0        0        0    22061 2022-12-08 19:53:16.288698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml
--rw-r--r--   0        0        0    27823 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml
--rw-r--r--   0        0        0     5740 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml
--rw-r--r--   0        0        0    15507 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml
--rw-r--r--   0        0        0    22397 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml
--rw-r--r--   0        0        0     4082 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml
--rw-r--r--   0        0        0     2151 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml
--rw-r--r--   0        0        0     5359 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml
--rw-r--r--   0        0        0    11356 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml
--rw-r--r--   0        0        0    12959 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml
--rw-r--r--   0        0        0     7870 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml
--rw-r--r--   0        0        0     6485 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml
--rw-r--r--   0        0        0     8455 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml
--rw-r--r--   0        0        0    14206 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml
--rw-r--r--   0        0        0    15034 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml
--rw-r--r--   0        0        0    17600 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml
--rw-r--r--   0        0        0    27620 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml
--rw-r--r--   0        0        0     4821 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml
--rw-r--r--   0        0        0     7808 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml
--rw-r--r--   0        0        0     8486 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml
--rw-r--r--   0        0        0     4783 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml
--rw-r--r--   0        0        0     6607 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml
--rw-r--r--   0        0        0     8457 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml
--rw-r--r--   0        0        0     2249 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml
--rw-r--r--   0        0        0     3447 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml
--rw-r--r--   0        0        0     5176 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml
--rw-r--r--   0        0        0     2637 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml
--rw-r--r--   0        0        0     4564 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml
--rw-r--r--   0        0        0     3751 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml
--rw-r--r--   0        0        0     3673 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml
--rw-r--r--   0        0        0     2461 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml
--rw-r--r--   0        0        0     4528 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml
--rw-r--r--   0        0        0     7628 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml
--rw-r--r--   0        0        0     1045 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml
--rw-r--r--   0        0        0    15694 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml
--rw-r--r--   0        0        0     3331 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml
--rw-r--r--   0        0        0     3234 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml
--rw-r--r--   0        0        0    12147 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml
--rw-r--r--   0        0        0    12076 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml
--rw-r--r--   0        0        0     4682 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml
--rw-r--r--   0        0        0    13539 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml
--rw-r--r--   0        0        0    25446 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml
--rw-r--r--   0        0        0     1919 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml
--rw-r--r--   0        0        0     3445 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml
--rw-r--r--   0        0        0     2800 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml
--rw-r--r--   0        0        0     3264 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml
--rw-r--r--   0        0        0     4324 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml
--rw-r--r--   0        0        0     4744 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml
--rw-r--r--   0        0        0     6642 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml
--rw-r--r--   0        0        0     2399 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml
--rw-r--r--   0        0        0    24162 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml
--rw-r--r--   0        0        0    25624 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml
--rw-r--r--   0        0        0    29018 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml
--rw-r--r--   0        0        0    13767 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml
--rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml
--rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml
--rw-r--r--   0        0        0    13686 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml
--rw-r--r--   0        0        0    14103 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml
--rw-r--r--   0        0        0     1285 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml
--rw-r--r--   0        0        0     2951 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml
--rw-r--r--   0        0        0     3412 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml
--rw-r--r--   0        0        0     7592 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml
--rw-r--r--   0        0        0     8319 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml
--rw-r--r--   0        0        0     4926 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml
--rw-r--r--   0        0        0      754 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml
--rw-r--r--   0        0        0    14359 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml
--rw-r--r--   0        0        0    19829 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml
--rw-r--r--   0        0        0     7097 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml
--rw-r--r--   0        0        0     6730 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml
--rw-r--r--   0        0        0    18555 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml
--rw-r--r--   0        0        0    39224 2022-12-08 19:53:16.292698 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml
--rw-r--r--   0        0        0    16858 2023-04-30 20:52:10.965302 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py
--rw-r--r--   0        0        0     2631 2023-03-20 16:55:58.994382 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/paths.py
--rw-r--r--   0        0        0      481 2023-03-20 16:55:59.002382 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/services/__init__.py
--rw-r--r--   0        0        0     5518 2023-03-21 07:56:39.142504 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py
--rw-r--r--   0        0        0    26076 2023-04-30 20:52:11.669309 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py
--rw-r--r--   0        0        0    11691 2023-04-30 20:52:10.937302 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/soap.py
--rw-r--r--   0        0        0      943 2023-04-30 20:52:10.853301 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnpconstants.py
--rw-r--r--   0        0        0    55895 2023-04-30 20:52:13.489325 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py
--rw-r--r--   0        0        0     7480 2023-04-30 21:01:15.502130 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py
--rw-r--r--   0        0        0     2628 2023-03-21 08:17:25.473613 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnperrors.py
--rw-r--r--   0        0        0    11109 2023-04-30 20:52:10.881301 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnpfactory.py
--rw-r--r--   0        0        0    21613 2023-03-21 08:16:35.890071 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py
--rw-r--r--   0        0        0      494 2023-03-20 16:55:59.002382 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/xml/__init__.py
--rw-r--r--   0        0        0    20710 2023-03-21 08:11:33.022274 mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py
--rw-r--r--   0        0        0     2471 1970-01-01 00:00:00.000000 mojo_interop-0.0.3/setup.py
--rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 mojo_interop-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-30 20:18:46.226836 mojo_interop-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      434 2023-04-30 21:10:35.023558 mojo_interop-0.0.4/README.rst
+-rw-r--r--   0        0        0      738 2023-05-06 21:02:35.570798 mojo_interop-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1630 2023-04-30 20:54:05.542332 mojo_interop-0.0.4/source/packages/mojo/factories/xmodsfactory.py
+-rw-r--r--   0        0        0      180 2023-04-23 00:21:47.238814 mojo_interop-0.0.4/source/packages/mojo/interop/clients/constants.py
+-rw-r--r--   0        0        0        0 2023-04-26 04:50:59.262714 mojo_interop-0.0.4/source/packages/mojo/interop/clients/linux/__init__.py
+-rw-r--r--   0        0        0      634 2023-05-06 19:38:19.555362 mojo_interop-0.0.4/source/packages/mojo/interop/clients/linux/linuxclient.py
+-rw-r--r--   0        0        0     1412 2023-05-06 19:38:34.671483 mojo_interop-0.0.4/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py
+-rw-r--r--   0        0        0     1289 2023-05-06 19:53:48.915347 mojo_interop-0.0.4/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py
+-rw-r--r--   0        0        0        0 2023-04-21 02:40:59.664563 mojo_interop-0.0.4/source/packages/mojo/interop/clients/osx/__init__.py
+-rw-r--r--   0        0        0      633 2023-05-06 19:40:03.716205 mojo_interop-0.0.4/source/packages/mojo/interop/clients/osx/osxclient.py
+-rw-r--r--   0        0        0     1388 2023-05-06 19:41:35.468963 mojo_interop-0.0.4/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py
+-rw-r--r--   0        0        0     1271 2023-05-06 19:53:59.927446 mojo_interop-0.0.4/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py
+-rw-r--r--   0        0        0        0 2023-04-26 04:43:08.306443 mojo_interop-0.0.4/source/packages/mojo/interop/clients/windows/__init__.py
+-rw-r--r--   0        0        0      637 2023-05-06 19:40:17.036314 mojo_interop-0.0.4/source/packages/mojo/interop/clients/windows/windowsclient.py
+-rw-r--r--   0        0        0     1436 2023-05-06 19:41:59.749166 mojo_interop-0.0.4/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py
+-rw-r--r--   0        0        0     1307 2023-05-06 19:54:10.971544 mojo_interop-0.0.4/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:44:21.610368 mojo_interop-0.0.4/source/packages/mojo/interop/clusters/__init__.py
+-rw-r--r--   0        0        0       69 2023-05-06 21:03:43.255179 mojo_interop-0.0.4/source/packages/mojo/interop/clusters/constants.py
+-rw-r--r--   0        0        0      509 2023-05-06 21:01:12.882371 mojo_interop-0.0.4/source/packages/mojo/interop/clusters/raspberrypi/picluster.py
+-rw-r--r--   0        0        0      624 2023-05-06 19:48:13.812380 mojo_interop-0.0.4/source/packages/mojo/interop/clusters/raspberrypi/pinode.py
+-rw-r--r--   0        0        0     1529 2023-05-06 21:01:52.014567 mojo_interop-0.0.4/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinator.py
+-rw-r--r--   0        0        0     1324 2023-05-06 19:53:41.375280 mojo_interop-0.0.4/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinatorcoupling.py
+-rw-r--r--   0        0        0      519 2022-12-08 19:53:16.276698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/__init__.py
+-rw-r--r--   0        0        0     2272 2023-04-30 21:03:13.691162 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsaddress.py
+-rw-r--r--   0        0        0      639 2023-04-30 21:03:11.207140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsapi.py
+-rw-r--r--   0        0        0     9720 2023-03-17 03:47:56.259994 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsconst.py
+-rw-r--r--   0        0        0     2121 2023-04-30 21:03:11.207140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnshostinfo.py
+-rw-r--r--   0        0        0     9274 2023-04-30 21:03:11.207140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py
+-rw-r--r--   0        0        0    15537 2023-04-30 21:03:11.223140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py
+-rw-r--r--   0        0        0     1862 2023-04-30 21:03:11.207140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnspointer.py
+-rw-r--r--   0        0        0     2250 2023-04-30 21:03:11.207140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsquestion.py
+-rw-r--r--   0        0        0      832 2023-03-16 05:21:20.896073 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py
+-rw-r--r--   0        0        0     6850 2023-04-30 21:03:11.223140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsrecord.py
+-rw-r--r--   0        0        0     3606 2023-04-30 21:03:11.223140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsserver.py
+-rw-r--r--   0        0        0     2719 2023-04-30 21:03:11.207140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsservice.py
+-rw-r--r--   0        0        0     2004 2023-04-30 21:03:11.207140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnstext.py
+-rw-r--r--   0        0        0     3750 2023-04-30 21:03:11.207140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsutil.py
+-rw-r--r--   0        0        0     2807 2023-04-30 21:03:11.207140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsvalidation.py
+-rw-r--r--   0        0        0     1052 2023-03-17 15:51:43.102472 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/exceptions.py
+-rw-r--r--   0        0        0     2615 2023-04-30 21:03:11.223140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/mdnsagent.py
+-rw-r--r--   0        0        0     6279 2023-04-30 21:03:11.223140 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py
+-rw-r--r--   0        0        0     2505 2023-03-17 06:36:21.314128 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py
+-rw-r--r--   0        0        0     1294 2023-03-16 22:12:31.133035 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/testmessages.py
+-rw-r--r--   0        0        0        0 2023-03-25 19:42:09.132533 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/power/dlipower/__init__.py
+-rw-r--r--   0        0        0      894 2023-03-28 16:14:15.598469 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py
+-rw-r--r--   0        0        0     3767 2023-03-28 16:14:15.598469 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py
+-rw-r--r--   0        0        0     6138 2023-04-29 04:47:55.337890 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py
+-rw-r--r--   0        0        0     7794 2023-03-25 18:55:12.050499 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/serial/tcpserialagent.py
+-rw-r--r--   0        0        0     4913 2023-04-29 04:47:55.329891 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py
+-rw-r--r--   0        0        0     6059 2023-04-29 04:47:55.333891 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py
+-rw-r--r--   0        0        0     1398 2023-04-29 04:47:55.321890 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py
+-rw-r--r--   0        0        0        0 2023-03-24 06:52:51.435618 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/ssh/__init__.py
+-rw-r--r--   0        0        0    70641 2023-03-28 16:14:15.598469 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/ssh/sshagent.py
+-rw-r--r--   0        0        0    12109 2023-04-29 04:47:55.353891 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py
+-rw-r--r--   0        0        0     7541 2023-04-29 04:47:55.349891 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py
+-rw-r--r--   0        0        0     1255 2023-04-29 04:47:55.353891 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/ssh/sshdevice.py
+-rw-r--r--   0        0        0      540 2023-03-20 16:55:58.998382 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/__init__.py
+-rw-r--r--   0        0        0      319 2023-03-20 16:55:58.990382 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/aliases.py
+-rw-r--r--   0        0        0     2431 2023-03-21 07:47:58.411623 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/aspectsupnp.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/content/__init__.py
+-rw-r--r--   0        0        0    15564 2023-03-21 07:49:16.837478 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/content/didllite.py
+-rw-r--r--   0        0        0      557 2023-03-20 16:55:59.002382 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/devices/__init__.py
+-rw-r--r--   0        0        0    14091 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py
+-rw-r--r--   0        0        0     1761 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py
+-rw-r--r--   0        0        0    44978 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py
+-rw-r--r--   0        0        0      494 2023-03-20 16:55:59.002382 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/embeddeddevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/rootdevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/services/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/embeddeddevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/rootdevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/__init__.py
+-rw-r--r--   0        0        0     3512 2023-04-30 20:52:11.401306 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py
+-rw-r--r--   0        0        0     6222 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    11201 2023-04-30 20:52:11.657309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py
+-rw-r--r--   0        0        0    11596 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py
+-rw-r--r--   0        0        0    14933 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py
+-rw-r--r--   0        0        0    20201 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py
+-rw-r--r--   0        0        0    13583 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    16776 2023-04-30 20:52:11.589308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     6120 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py
+-rw-r--r--   0        0        0    12568 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    17020 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     4574 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py
+-rw-r--r--   0        0        0      630 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py
+-rw-r--r--   0        0        0     4109 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py
+-rw-r--r--   0        0        0    11330 2023-04-30 20:52:11.049303 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    12948 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     4161 2023-04-30 20:52:11.597308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py
+-rw-r--r--   0        0        0     4161 2023-04-30 20:52:11.589308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py
+-rw-r--r--   0        0        0     5719 2023-04-30 20:52:11.513307 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py
+-rw-r--r--   0        0        0     9453 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py
+-rw-r--r--   0        0        0    11449 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py
+-rw-r--r--   0        0        0    13534 2023-04-30 20:52:11.597308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py
+-rw-r--r--   0        0        0    23744 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py
+-rw-r--r--   0        0        0     4429 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py
+-rw-r--r--   0        0        0     7462 2023-04-30 20:52:11.657309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py
+-rw-r--r--   0        0        0    10870 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py
+-rw-r--r--   0        0        0     7731 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py
+-rw-r--r--   0        0        0     8828 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py
+-rw-r--r--   0        0        0    10006 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py
+-rw-r--r--   0        0        0     2043 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py
+-rw-r--r--   0        0        0     3992 2023-04-30 20:52:10.993303 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py
+-rw-r--r--   0        0        0     4959 2023-04-30 20:52:11.573308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py
+-rw-r--r--   0        0        0     3828 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py
+-rw-r--r--   0        0        0     3166 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py
+-rw-r--r--   0        0        0     2039 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py
+-rw-r--r--   0        0        0     3577 2023-04-30 20:52:11.597308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py
+-rw-r--r--   0        0        0     3071 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py
+-rw-r--r--   0        0        0     4686 2023-04-30 20:52:11.657309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py
+-rw-r--r--   0        0        0     9951 2023-04-30 20:52:11.597308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py
+-rw-r--r--   0        0        0     1782 2023-04-30 20:52:11.597308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py
+-rw-r--r--   0        0        0     8071 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py
+-rw-r--r--   0        0        0     3931 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py
+-rw-r--r--   0        0        0     3931 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py
+-rw-r--r--   0        0        0    10240 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py
+-rw-r--r--   0        0        0    10240 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py
+-rw-r--r--   0        0        0     4675 2023-04-30 20:52:11.657309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py
+-rw-r--r--   0        0        0     5801 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py
+-rw-r--r--   0        0        0    11116 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py
+-rw-r--r--   0        0        0     1691 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py
+-rw-r--r--   0        0        0     3288 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py
+-rw-r--r--   0        0        0     2107 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py
+-rw-r--r--   0        0        0     2712 2023-04-30 20:52:11.189304 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py
+-rw-r--r--   0        0        0     4718 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py
+-rw-r--r--   0        0        0     5214 2023-04-30 20:52:11.657309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py
+-rw-r--r--   0        0        0     5733 2023-04-30 20:52:11.321306 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py
+-rw-r--r--   0        0        0     1751 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py
+-rw-r--r--   0        0        0    20947 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py
+-rw-r--r--   0        0        0    22560 2023-04-30 20:52:11.293305 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py
+-rw-r--r--   0        0        0    26952 2023-04-30 20:52:11.657309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py
+-rw-r--r--   0        0        0     7336 2023-04-30 20:52:11.261305 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py
+-rw-r--r--   0        0        0    11158 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py
+-rw-r--r--   0        0        0    11158 2023-04-30 20:52:11.597308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py
+-rw-r--r--   0        0        0     9804 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py
+-rw-r--r--   0        0        0    10325 2023-04-30 20:52:11.629308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py
+-rw-r--r--   0        0        0     2199 2023-04-30 20:52:11.157304 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py
+-rw-r--r--   0        0        0     3257 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py
+-rw-r--r--   0        0        0     4234 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py
+-rw-r--r--   0        0        0     7786 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0     8132 2023-04-30 20:52:11.597308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py
+-rw-r--r--   0        0        0     6178 2023-04-30 20:52:11.081303 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0     1351 2023-04-30 20:52:11.217305 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0    12414 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py
+-rw-r--r--   0        0        0    15214 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py
+-rw-r--r--   0        0        0     5133 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py
+-rw-r--r--   0        0        0     6600 2023-04-30 20:52:11.657309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0    17131 2023-04-30 20:52:11.601308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py
+-rw-r--r--   0        0        0    30991 2023-04-30 20:52:11.633308 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/__init__.py
+-rw-r--r--   0        0        0      479 2023-03-20 16:55:59.002382 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/dynamic/__init__.py
+-rw-r--r--   0        0        0      247 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:BinaryLight:1.xml
+-rw-r--r--   0        0        0      280 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DigitalSecurityCamera:1.xml
+-rw-r--r--   0        0        0      420 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DimmableLight:1.xml
+-rw-r--r--   0        0        0     1159 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml
+-rw-r--r--   0        0        0     1865 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml
+-rw-r--r--   0        0        0      459 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:1.xml
+-rw-r--r--   0        0        0      604 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml
+-rw-r--r--   0        0        0      208 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:LANDevice:1.xml
+-rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:1.xml
+-rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:2.xml
+-rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml
+-rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml
+-rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml
+-rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml
+-rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml
+-rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml
+-rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml
+-rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Printer:1.xml
+-rw-r--r--   0        0        0      187 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAClient:1.xml
+-rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:1.xml
+-rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:2.xml
+-rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:1.xml
+-rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:2.xml
+-rw-r--r--   0        0        0      300 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIClientDevice:1.xml
+-rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIServerDevice:1.xml
+-rw-r--r--   0        0        0      561 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml
+-rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:1.xml
+-rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:2.xml
+-rw-r--r--   0        0        0      419 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:1.xml
+-rw-r--r--   0        0        0      622 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml
+-rw-r--r--   0        0        0      416 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:1.xml
+-rw-r--r--   0        0        0      936 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml
+-rw-r--r--   0        0        0     1090 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml
+-rw-r--r--   0        0        0     1244 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml
+-rw-r--r--   0        0        0      338 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:1.xml
+-rw-r--r--   0        0        0      340 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:2.xml
+-rw-r--r--   0        0        0      490 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WLANAccessPointDevice:1.xml
+-rw-r--r--   0        0        0    21478 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml
+-rw-r--r--   0        0        0    22506 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml
+-rw-r--r--   0        0        0    32819 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml
+-rw-r--r--   0        0        0     3894 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml
+-rw-r--r--   0        0        0     5779 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml
+-rw-r--r--   0        0        0    10054 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml
+-rw-r--r--   0        0        0    22061 2022-12-08 19:53:16.288698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml
+-rw-r--r--   0        0        0    27823 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml
+-rw-r--r--   0        0        0     5740 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml
+-rw-r--r--   0        0        0    15507 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml
+-rw-r--r--   0        0        0    22397 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml
+-rw-r--r--   0        0        0     4082 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml
+-rw-r--r--   0        0        0     2151 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml
+-rw-r--r--   0        0        0     5359 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml
+-rw-r--r--   0        0        0    11356 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml
+-rw-r--r--   0        0        0    12959 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml
+-rw-r--r--   0        0        0     7870 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml
+-rw-r--r--   0        0        0     6485 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml
+-rw-r--r--   0        0        0     8455 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml
+-rw-r--r--   0        0        0    14206 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml
+-rw-r--r--   0        0        0    15034 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml
+-rw-r--r--   0        0        0    17600 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml
+-rw-r--r--   0        0        0    27620 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml
+-rw-r--r--   0        0        0     4821 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml
+-rw-r--r--   0        0        0     7808 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml
+-rw-r--r--   0        0        0     8486 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml
+-rw-r--r--   0        0        0     4783 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml
+-rw-r--r--   0        0        0     6607 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml
+-rw-r--r--   0        0        0     8457 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml
+-rw-r--r--   0        0        0     2249 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml
+-rw-r--r--   0        0        0     3447 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml
+-rw-r--r--   0        0        0     5176 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml
+-rw-r--r--   0        0        0     2637 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml
+-rw-r--r--   0        0        0     4564 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml
+-rw-r--r--   0        0        0     3751 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml
+-rw-r--r--   0        0        0     3673 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml
+-rw-r--r--   0        0        0     2461 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml
+-rw-r--r--   0        0        0     4528 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml
+-rw-r--r--   0        0        0     7628 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml
+-rw-r--r--   0        0        0     1045 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml
+-rw-r--r--   0        0        0    15694 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml
+-rw-r--r--   0        0        0     3331 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml
+-rw-r--r--   0        0        0     3234 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml
+-rw-r--r--   0        0        0    12147 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml
+-rw-r--r--   0        0        0    12076 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml
+-rw-r--r--   0        0        0     4682 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml
+-rw-r--r--   0        0        0    13539 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml
+-rw-r--r--   0        0        0    25446 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml
+-rw-r--r--   0        0        0     1919 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml
+-rw-r--r--   0        0        0     3445 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml
+-rw-r--r--   0        0        0     2800 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml
+-rw-r--r--   0        0        0     3264 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml
+-rw-r--r--   0        0        0     4324 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml
+-rw-r--r--   0        0        0     4744 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml
+-rw-r--r--   0        0        0     6642 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml
+-rw-r--r--   0        0        0     2399 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml
+-rw-r--r--   0        0        0    24162 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml
+-rw-r--r--   0        0        0    25624 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml
+-rw-r--r--   0        0        0    29018 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml
+-rw-r--r--   0        0        0    13767 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml
+-rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml
+-rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml
+-rw-r--r--   0        0        0    13686 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml
+-rw-r--r--   0        0        0    14103 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml
+-rw-r--r--   0        0        0     1285 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml
+-rw-r--r--   0        0        0     2951 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml
+-rw-r--r--   0        0        0     3412 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml
+-rw-r--r--   0        0        0     7592 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml
+-rw-r--r--   0        0        0     8319 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml
+-rw-r--r--   0        0        0     4926 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml
+-rw-r--r--   0        0        0      754 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml
+-rw-r--r--   0        0        0    14359 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml
+-rw-r--r--   0        0        0    19829 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml
+-rw-r--r--   0        0        0     7097 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml
+-rw-r--r--   0        0        0     6730 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml
+-rw-r--r--   0        0        0    18555 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml
+-rw-r--r--   0        0        0    39224 2022-12-08 19:53:16.292698 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml
+-rw-r--r--   0        0        0    16858 2023-04-30 20:52:10.965302 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py
+-rw-r--r--   0        0        0     2631 2023-03-20 16:55:58.994382 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/paths.py
+-rw-r--r--   0        0        0      481 2023-03-20 16:55:59.002382 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/services/__init__.py
+-rw-r--r--   0        0        0     5518 2023-03-21 07:56:39.142504 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py
+-rw-r--r--   0        0        0    26076 2023-04-30 20:52:11.669309 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py
+-rw-r--r--   0        0        0    11691 2023-04-30 20:52:10.937302 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/soap.py
+-rw-r--r--   0        0        0      943 2023-04-30 20:52:10.853301 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnpconstants.py
+-rw-r--r--   0        0        0    55895 2023-04-30 20:52:13.489325 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py
+-rw-r--r--   0        0        0     7480 2023-04-30 21:01:15.502130 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py
+-rw-r--r--   0        0        0     2628 2023-03-21 08:17:25.473613 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnperrors.py
+-rw-r--r--   0        0        0    11109 2023-04-30 20:52:10.881301 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnpfactory.py
+-rw-r--r--   0        0        0    21613 2023-03-21 08:16:35.890071 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py
+-rw-r--r--   0        0        0      494 2023-03-20 16:55:59.002382 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/xml/__init__.py
+-rw-r--r--   0        0        0    20710 2023-03-21 08:11:33.022274 mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py
+-rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 mojo_interop-0.0.4/setup.py
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 mojo_interop-0.0.4/PKG-INFO
```

### Comparing `mojo_interop-0.0.3/LICENSE.txt` & `mojo_interop-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/pyproject.toml` & `mojo_interop-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-interop"
 description = "Automation Mojo Interop Extensions"
-version = "0.0.3"
+version = "0.0.4"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/factories/xmodsfactory.py` & `mojo_interop-0.0.4/source/packages/mojo/factories/xmodsfactory.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/base/baseclient.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 
+
+
 from typing import TYPE_CHECKING
 
 from mojo.xmods.landscaping.landscapedevice import LandscapeDevice
 from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
 
-from mojo.interop.protocols.ssh.sshagent import SshAgent
+from mojo.interop.protocols.serial.tcpserialagent import TcpSerialAgent
 
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
     from mojo.xmods.landscaping.coordinators.coordinatorbase import CoordinatorBase
 
-class BaseClient(LandscapeDevice):
+class TcpSerialDevice(LandscapeDevice):
 
     def __init__(self, lscape: "Landscape", coordinator: "CoordinatorBase",
                  friendly_id:FriendlyIdentifier, device_type: str, device_config: dict):
         super().__init__(lscape, coordinator, friendly_id, device_type, device_config)
 
         self._host = device_config["host"]
+        self._port = device_config["port"]
         return
 
     @property
     def host(self) -> str:
         return self._host
 
     @property
-    def ssh(self) -> SshAgent:
+    def port(self) -> int:
+        return self._port
+
+    @property
+    def serial(self) -> TcpSerialAgent:
         ext = self._extensions["network/ssh"]
         return ext
 
     def enhance(self):
         """
             Called to allow a device to enhance its metadata past what is declared in the
             configuration file.  For device that only have a hint, this might trigger a
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/base/baseclientcoordinator.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-.. module:: baseclientcoordinator
+.. module:: sshcoordinator
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: Contains the BaseClientPoolCoordinator which is used for managing connectivity with pools of OSX capable devices
+    :synopsis: Contains the SshPoolCoordinator which is used for managing connectivity with pools of ssh capable devices
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
@@ -25,73 +25,70 @@
 from mojo.xmods.exceptions import ConfigurationError
 from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
 
 from mojo.xmods.landscaping.coordinators.coordinatorbase import CoordinatorBase
 from mojo.xmods.landscaping.landscapeparameters import LandscapeActivationParams
 from mojo.xmods.landscaping.landscapedevice import LandscapeDevice
 
-from mojo.interop.clients.base.baseclient import BaseClient
-
 from mojo.interop.protocols.ssh.sshagent import SshAgent
+from mojo.interop.protocols.ssh.sshdevice import SshDevice
 
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
+SUPPORTED_INTEGRATION_CLASS = "network/ssh"
 
-def format_client_configuration_error(message, next_dev_config):
+def format_ssh_device_configuration_error(message, sshdev_config):
     """
-        Takes an error message and an client configuration info dictionary and
+        Takes an error message and an SSH device configuration info dictionary and
         formats a configuration error message.
     """
     error_lines = [
         message,
         "DEVICE:"
     ]
 
-    dev_repr_lines = pprint.pformat(next_dev_config, indent=4).splitlines(False)
+    dev_repr_lines = pprint.pformat(sshdev_config, indent=4).splitlines(False)
     for dline in dev_repr_lines:
         error_lines.append("    " + dline)
     
     errmsg = os.linesep.join(error_lines)
     return errmsg
 
-class BaseClientCoordinator(CoordinatorBase):
+class SshCoordinator(CoordinatorBase):
     """
-        The :class:`BaseClientPoolCoordinator` creates a pool of agents that can be used to
-        coordinate the interop activities of the automation process and remote OSX
-        client.
+        The :class:`SshPoolCoordinator` creates a pool of agents that can be used to
+        coordinate the interop activities of the automation process and remote SSH
+        nodes.
     """
     # pylint: disable=attribute-defined-outside-init
 
-    INTEGRATION_CLASS = ""
-    CLIENT_TYPE = BaseClient
-
     def __init__(self, lscape: "Landscape", *args, **kwargs):
         super().__init__(lscape, *args, **kwargs)
 
         self._cl_upnp_hint_to_ip_lookup: Dict[str, str] = {}
         self._cl_ip_to_host_lookup: Dict[str, str] = {}
         return
 
     def activate(self, activation_params: LandscapeActivationParams):
         """
             Called by the :class:`LandscapeOperationalLayer` in order for the coordinator to be able to
             potentially enhanced devices.
         """
         return
 
-    def create_landscape_device(self, landscape: "Landscape", device_info: Dict[str, Any]) -> Tuple[FriendlyIdentifier, BaseClient]:
+    def create_landscape_device(self, landscape: "Landscape", device_info: Dict[str, Any]) -> Tuple[FriendlyIdentifier, SshDevice]:
         """
             Called to declare a declared landscape device for a given coordinator.
         """
         host = device_info["host"]
         dev_type = device_info["deviceType"]
         fid = FriendlyIdentifier(host, host)
 
-        device = self.CLIENT_TYPE(landscape, self, fid, dev_type, device_info)
+        device = SshDevice(landscape, self, fid, dev_type, device_info)
         
         coord_ref = weakref.ref(self)
         device_ref = weakref.ref(device)
 
         ssh_agent = SshAgent(host, device.ssh_credential)
         ssh_agent.initialize(coord_ref, device_ref, host, host, device_info)
 
@@ -119,106 +116,127 @@
                 status, stdout, stderr = agent.run_cmd(cmd)
                 results.append((host, ipaddr, status, stdout, stderr, None))
             except Exception as xcpt: # pylint: disable=broad-except
                 results.append((host, ipaddr, None, None, None, xcpt))
 
         return results
 
-    def extend_devices(self, next_devices: List[LandscapeDevice], upnp_coord: Optional[CoordinatorBase]=None):
+    def extend_devices(self, sshdevices: List[LandscapeDevice], upnp_coord: Optional[CoordinatorBase]=None):
         """
-            Processes a list of device configs and creates and registers devices and OSX clients along with
-            a SSH client device extensions attached with the landscape for the devices not already registered.
+            Processes a list of device configs and creates and registers devices and SSH device extensions
+            attached with the landscape for the devices not already registered.  If a device has already
+            been registered by the UPNP coordinator then a device extension is created and attached to the
+            existing device.
 
-            :param next_devices: A list of osx device configuration dictionaries.
+            :param sshdevices: A list of ssh device configuration dictionaries.
         """
 
-        lscape: "Landscape" = self.landscape
+        lscape = self.landscape
 
-        dev_config_errors = []
+        ssh_config_errors = []
 
-        dev_devices_available = []
-        dev_devices_unavailable = []
+        ssh_devices_available = []
+        ssh_devices_unavailable = []
 
-        for next_dev in next_devices:
-            next_dev_config = next_dev.device_config
-            ssh_credential_list = next_dev.ssh_credentials
+        for sshdev in sshdevices:
+            sshdev_config = sshdev.device_config
+            ssh_credential_list = sshdev.ssh_credentials
             if len(ssh_credential_list) == 0:
-                errmsg = format_client_configuration_error(
-                        "All OSX client devices must have at least one valid credential.", next_dev_config)
+                errmsg = format_ssh_device_configuration_error(
+                        "All SSH devices must have at least one valid credential.", sshdev_config)
                 raise ConfigurationError(errmsg) from None
 
             ssh_cred_by_role = {}
             for ssh_cred in ssh_credential_list:
                 cred_role = ssh_cred.role
                 if cred_role not in ssh_cred_by_role:
                     ssh_cred_by_role[cred_role] = ssh_cred
                 else:
-                    errmsg = format_client_configuration_error(
-                        "The OSX client device had more than one credentials with the role '{}'".format(cred_role), next_dev_config)
+                    errmsg = format_ssh_device_configuration_error(
+                        "The SSH device had more than one credentials with the role '{}'".format(cred_role), sshdev_config)
                     raise ConfigurationError(errmsg) from None
 
             if "priv" not in ssh_cred_by_role:
-                errmsg = format_client_configuration_error(
-                        "All OSX client devices must have a 'priv' credential.", next_dev_config)
+                errmsg = format_ssh_device_configuration_error(
+                        "All SSH devices must have a 'priv' credential.", sshdev_config)
                 raise ConfigurationError(errmsg) from None
 
             priv_cred = ssh_cred_by_role["priv"]
 
-            dev_type = next_dev_config["deviceType"]
+            dev_type = sshdev_config["deviceType"]
 
             host = None
             upnp_hint = None
-            if "host" in next_dev_config:
-                host = next_dev_config["host"]
-            else:
-                pass
+            if "host" in sshdev_config:
+                host = sshdev_config["host"]
+            elif dev_type == "network/upnp":
+                upnp_config = sshdev_config["upnp"]
+
+                if "hint" in upnp_config:
+                    upnp_hint = upnp_config["hint"]
+                elif "USN" in upnp_config:
+                    upnp_hint = upnp_config["USN"]
+                if upnp_coord is not None:
+                    upnp_dev = upnp_coord.lookup_device_by_upnp_hint(upnp_hint)
+                    dev = upnp_dev.basedevice
+                    if dev is not None:
+                        ipaddr = upnp_dev.IPAddress
+                        host = ipaddr
+                        sshdev_config["host"] = host
+                        self._cl_upnp_hint_to_ip_lookup[upnp_hint] = ipaddr
+                else:
+                    ssh_config_errors.append(sshdev_config)
 
             if host is not None:
-                called_id = next_dev.identity
+                called_id = dev.identity
                 ip = socket.gethostbyname(host)
                 self._cl_ip_to_host_lookup[ip] = host
 
                 agent = SshAgent(host, priv_cred, users=ssh_cred_by_role, called_id=called_id)
 
-                next_dev_config["ipaddr"] = agent.ipaddr
+                sshdev_config["ipaddr"] = agent.ipaddr
                 try:
                     status, stdout, stderr = agent.run_cmd("echo Hello")
                     if status == 0 and stdout.strip() == "Hello":
-                        dev_devices_available.append(next_dev_config)
+                        ssh_devices_available.append(sshdev_config)
                     else:
-                        dev_devices_unavailable.append(next_dev_config)
+                        ssh_devices_unavailable.append(sshdev_config)
                 except:
-                    dev_devices_unavailable.append(next_dev_config)
+                    ssh_devices_unavailable.append(sshdev_config)
 
                 self._cl_children[host] = agent
 
                 coord_ref = weakref.ref(self)
 
-                fdid = FriendlyIdentifier(host, host)
-                basedevice = lscape.create_landscape_device(fdid, dev_type, next_dev_config)
-                basedevice = lscape._enhance_landscape_device(basedevice, agent)
-                basedevice.initialize_features()
+                basedevice = None
+                if upnp_hint is not None:
+                    basedevice = lscape._internal_lookup_device_by_hint(upnp_hint) # pylint: disable=protected-access
+                else:
+                    fdid = FriendlyIdentifier(host, host)
+                    basedevice = lscape._create_landscape_device(fdid, dev_type, sshdev_config)
+                    basedevice = lscape._enhance_landscape_device(basedevice, agent)
+                    basedevice.initialize_features()
 
                 basedevice.attach_extension("ssh", agent)
 
                 basedevice_ref = weakref.ref(basedevice)
-                agent.initialize(coord_ref, basedevice_ref, host, ip, next_dev_config)
+                agent.initialize(coord_ref, basedevice_ref, host, ip, sshdev_config)
 
                 # If this device does not have a USN or hint then it is not a UPNP device so the
-                # BaseClientPoolCoordinator is repsonsible for activating it
+                # SshPoolCoordinator is repsonsible for activating it
                 if upnp_hint is None:
                     lscape._internal_activate_device(host)
 
             else:
-                dev_config_errors.append(next_dev_config)
+                ssh_config_errors.append(sshdev_config)
 
-        self._available_devices = dev_devices_available
-        self._unavailable_devices = dev_devices_unavailable
+        self._available_devices = ssh_devices_available
+        self._unavailable_devices = ssh_devices_unavailable
 
-        return dev_config_errors, dev_devices_available, dev_devices_unavailable
+        return ssh_config_errors, ssh_devices_available, ssh_devices_unavailable
 
     def lookup_device_by_host(self, host: str) -> Union[LandscapeDevice, None]:
         """
             Looks up the agent for a device by its hostname.  If the
             agent is not found then the API returns None.
 
             :param host: The host name of the LandscapeDevice to search for.
@@ -257,19 +275,19 @@
         finally:
             self._coord_lock.release()
 
         return device
 
     def verify_connectivity(self, cmd: str = "echo 'It Works'", user: Optional[str] = None, raiseerror: bool = True) -> List[tuple]:
         """
-            Loops through the nodes in the OSX client pool and utilizes the credentials for the specified user in order to verify
+            Loops through the nodes in the SSH pool and utilizes the credentials for the specified user in order to verify
             connectivity with the remote node.
 
             :param cmd: A command to run on the remote machine in order
-                        to verify that osx connectivity can be establish.
+                        to verify that ssh connectivity can be establish.
             :param user: The name of the user credentials to use for connectivity.
                          If the 'user' parameter is not provided, then the
                          credentials of the default or priviledged user will be used.
             :param raiseerror: A boolean value indicating if this API should raise an Exception on failure.
 
             :returns: A list of errors encountered when verifying connectivity with the devices managed or watched by the coordinator.
         """
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/base/baseclientcoordinatorcoupling.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 """
-.. module:: baseclientcoordinatorcoupling
+.. module:: sshcoordinatorcoupling
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: Contains a BaseClientCoordinatorCoupling object to use for working with the OSX clients.
+    :synopsis: Contains a SshCoordinatorCoupling object to use for working with the computer nodes via SSH
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
 __version__ = "1.0.0"
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
-
 from typing import Any, Dict, List, Tuple, TYPE_CHECKING
 
-from functools import partial
-
 from mojo.xmods.exceptions import SemanticError
 from mojo.xmods.landscaping.coupling.coordinatorcoupling import CoordinatorCoupling
 from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
 from mojo.xmods.landscaping.landscape import LandscapeDevice
-from mojo.interop.clients.osx.osxclientcoordinator import BaseClientCoordinator
+from mojo.interop.protocols.ssh.sshcoordinator import SshCoordinator
 
 from mojo.xmods.landscaping.precedence import StartupLevel
 
 # Types imported only for type checking purposes
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
-SUPPORTED_INTEGRATION_CLASS = "network/client-osx"
+SUPPORTED_INTEGRATION_CLASS = "network/ssh"
 
-def is_matching_client_config(integ_class, device_info):
-    is_matching_client = False
+def is_ssh_device_config(device_info):
+    is_ssh_dev = False
 
     dev_type = device_info["deviceType"]
-    if dev_type == integ_class:
-        is_matching_client = True
+    if dev_type == SUPPORTED_INTEGRATION_CLASS:
+        is_ssh_dev = True
 
-    return is_matching_client
+    return is_ssh_dev
 
-class BaseClientCoordinatorCoupling(CoordinatorCoupling):
+class SshCoordinatorCoupling(CoordinatorCoupling):
     """
-        The BaseClientCoordinatorCoupling handle the requirement registration for the OSX coordinator.
+        The SshCoordinatorCoupling handle the requirement registration for the SSH coordinator.
     """
 
-    pathbase = "/osx"
+    pathbase = "/ssh"
 
     integration_section: str = "devices"
     integration_leaf: str = "deviceType"
     integration_class: str = SUPPORTED_INTEGRATION_CLASS
 
     def __init__(self, *args, **kwargs):
         """
-            The default contructor for an :class:`BaseClientCoordinatorIntegration`.
+            The default contructor for an :class:`SshPoolCoordinatorIntegration`.
         """
         super().__init__(*args, **kwargs)
         return
 
     @classmethod
     def attach_to_environment(cls, landscape: "Landscape"):
         """
@@ -71,17 +68,17 @@
         """
 
         cls.landscape = landscape
         layer_config = landscape.layer_configuration
 
         device_list = layer_config.get_device_configs()
         if len(device_list) > 0:
-            dev_client_list = [dev for dev in filter(partial(is_matching_client_config, cls.integration_class), device_list)]
+            ssh_device_list = [dev for dev in filter(is_ssh_device_config, device_list)]
 
-            if len(dev_client_list) > 0:
+            if len(ssh_device_list) > 0:
                 layer_integ = landscape.layer_integration
                 layer_integ.register_integration_dependency(cls)
 
         return
 
     @classmethod
     def collect_resources(cls):
@@ -94,24 +91,27 @@
         return
 
     @classmethod
     def create_coordinator(cls, landscape: "Landscape") -> object:
         """
             This API is called so that the landscape can create a coordinator for a given integration role.
         """
-        cls.coordinator = BaseClientCoordinator(landscape)
+        cls.coordinator = SshCoordinator(landscape)
         return cls.coordinator
 
     @classmethod
     def declare_precedence(cls) -> int:
         """
             This API is called so that the IntegrationCoupling can declare an ordinal precedence that should be
             utilized for bringing up its integration state.
         """
-        return StartupLevel.PrimaryProtocol
+        # Because SSH is a protocol that can be used by other coordinators as well, we are considered a
+        # secondary protocol.  That is because the SSH coordinator may be called on to add an extension
+        # to devices that it did not create and so does not own such as a UPNP device.
+        return StartupLevel.SecondaryProtocol
 
     @classmethod
     def diagnostic(cls, label: str, level: int, diag_folder: str):
         """
             The API is called by the :class:`akit.sequencer.Sequencer` object when the automation sequencer is
             building out a diagnostic package at a diagnostic point in the automation sequence.  Example diagnostic
             points are:
@@ -139,30 +139,32 @@
         """
 
         lscape = cls.landscape
         layer_integ = lscape.layer_integration
 
         device_list = layer_integ.get_devices()
         if len(device_list) > 0:
-            dev_client_list = [dev for dev in filter(partial(is_matching_client_config, cls.integration_class), device_list)]
+            ssh_device_list = [dev for dev in filter(is_ssh_device_config, device_list)]
+
+            if len(ssh_device_list) == 0:
+                raise SemanticError("We should have not been called if no SSH devices are available.")
 
-            if len(dev_client_list) == 0:
-                raise SemanticError("We should have not been called if no OSX devices are available.")
+            upnp_coord = cls.landscape._internal_get_upnp_coord()
 
-            dev_config_errors, matching_device_results, missing_device_results = cls.coordinator.attach_to_devices(
-                dev_client_list)
+            ssh_config_errors, matching_device_results, missing_device_results = cls.coordinator.attach_to_devices(
+                ssh_device_list, upnp_coord=upnp_coord)
 
-            dev_scan_results = {
-                "osx": {
+            ssh_scan_results = {
+                "ssh": {
                     "matching_devices": matching_device_results,
                     "missing_devices": missing_device_results
                 }
             }
 
-        return (dev_config_errors, dev_scan_results)
+        return (ssh_config_errors, ssh_scan_results)
 
     @classmethod
     def establish_presence(cls) -> Tuple[List[str], dict]:
         """
             This API is called so the `IntegrationCoupling` can establish presence with any compute or storage
             resources.
 
@@ -172,28 +174,28 @@
         return
 
     @classmethod
     def validate_item_configuration(cls, item_info: Dict[str, Any]) -> Tuple[List[str], List[str]]:
         """
             Validate the item configuration.
 
-            -   deviceType: network/client-osx
+            -   deviceType: network/ssh
                 name: raspey03
                 host: 172.16.1.33
                 credentials:
                 -    pi-cluster
                 features:
                     isolation: false
                 skip: false
         """
         errors = []
         warnings = []
         
         if "host" not in item_info:
-            errmsg = "Device configuration 'network/client-osx' must have a 'host' field."
+            errmsg = "Device configuration 'network/ssh' must have a 'host' field."
             errors.append(errmsg)
 
         if "credentials" not in item_info:
-            warnmsg = "Device configuration 'network/client-osx' should have a 'credentials' field."
+            warnmsg = "Device configuration 'network/ssh' should have a 'credentials' field."
             warnings.append(warnmsg)
 
         return errors, warnings
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/linux/linuxclient.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/clients/linux/linuxclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 from typing import TYPE_CHECKING
 
 from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
-
-from mojo.interop.clients.base.baseclient import BaseClient
+from mojo.xmods.landscaping.client.clientbase import ClientBase
 
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
     from mojo.xmods.landscaping.coordinators.coordinatorbase import CoordinatorBase
 
-class LinuxClient(BaseClient):
+class LinuxClient(ClientBase):
 
     def __init__(self, lscape: "Landscape", coordinator: "CoordinatorBase",
                  friendly_id:FriendlyIdentifier, device_type: str, device_config: dict):
         super().__init__(lscape, coordinator, friendly_id, device_type, device_config)
         return
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 from typing import TYPE_CHECKING
 
-from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_LINUX_CLIENT
-
-from mojo.interop.clients.base.baseclientcoordinator import BaseClientCoordinator
+from mojo.xmods.landscaping.client.clientcoordinatorbase import ClientCoordinatorBase
 
+from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_LINUX_CLIENT
 from mojo.interop.clients.linux.linuxclient import LinuxClient
 
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
-class LinuxClientCoordinator(BaseClientCoordinator):
+class LinuxClientCoordinator(ClientCoordinatorBase):
     """
         The :class:`LinuxPoolCoordinator` creates a pool of agents that can be used to
         coordinate the interop activities of the automation process and remote Linux
         client.
     """
 
     INTEGRATION_CLASS = INTEGRATION_CLASS_FOR_LINUX_CLIENT
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-.. module:: linuxclientcoordinatorcoupling
+.. module:: osxclientcoordinatorcoupling
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: Contains a LinuxClientCoordinatorCoupling object to use for working with the LINUX clients.
+    :synopsis: Contains a OsxClientCoordinatorCoupling object to use for working with the OSX clients.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
@@ -13,27 +13,26 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 from typing import TYPE_CHECKING
 
-from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_LINUX_CLIENT
-from mojo.interop.clients.base.baseclientcoordinatorcoupling import BaseClientCoordinatorCoupling
+from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_OSX_CLIENT
+from mojo.xmods.landscaping.client.clientcoordinatorcouplingbase import ClientCoordinatorCouplingBase
 
-class LinuxClientCoordinatorCoupling(BaseClientCoordinatorCoupling):
+
+class OsxClientCoordinatorCoupling(ClientCoordinatorCouplingBase):
     """
-        The LinuxClientCoordinatorCoupling handle the requirement registration for the Linux coordinator.
+        The OsxClientCoordinatorCoupling handle the requirement registration for the OSX coordinator.
     """
 
-    pathbase = "/linux"
-
     integration_section: str = "devices"
     integration_leaf: str = "deviceType"
-    integration_class: str = INTEGRATION_CLASS_FOR_LINUX_CLIENT
+    integration_class: str = INTEGRATION_CLASS_FOR_OSX_CLIENT
 
     def __init__(self, *args, **kwargs):
         """
-            The default contructor for an :class:`LinuxCoordinatorIntegration`.
+            The default contructor for an :class:`OsxCoordinatorIntegration`.
         """
         super().__init__(*args, **kwargs)
         return
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/osx/osxclient.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/clients/windows/windowsclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 from typing import TYPE_CHECKING
 
 from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
+from mojo.xmods.landscaping.client.clientbase import ClientBase
 
-from mojo.interop.clients.base.baseclient import BaseClient
 
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
     from mojo.xmods.landscaping.coordinators.coordinatorbase import CoordinatorBase
 
-class OsxClient(BaseClient):
+class WindowsClient(ClientBase):
 
     def __init__(self, lscape: "Landscape", coordinator: "CoordinatorBase",
                  friendly_id:FriendlyIdentifier, device_type: str, device_config: dict):
         super().__init__(lscape, coordinator, friendly_id, device_type, device_config)
         return
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 from typing import TYPE_CHECKING
 
-from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_OSX_CLIENT
-
-from mojo.interop.clients.base.baseclientcoordinator import BaseClientCoordinator
+from mojo.xmods.landscaping.client.clientcoordinatorbase import ClientCoordinatorBase
 
+from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_OSX_CLIENT
 from mojo.interop.clients.osx.osxclient import OsxClient
 
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
-class OsxClientCoordinator(BaseClientCoordinator):
+class OsxClientCoordinator(ClientCoordinatorBase):
     """
         The :class:`OsxPoolCoordinator` creates a pool of agents that can be used to
         coordinate the interop activities of the automation process and remote OSX
         client.
     """
 
     INTEGRATION_CLASS = INTEGRATION_CLASS_FOR_OSX_CLIENT
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-.. module:: osxclientcoordinatorcoupling
+.. module:: linuxclientcoordinatorcoupling
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: Contains a OsxClientCoordinatorCoupling object to use for working with the OSX clients.
+    :synopsis: Contains a LinuxClientCoordinatorCoupling object to use for working with the LINUX clients.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
@@ -13,27 +13,26 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 from typing import TYPE_CHECKING
 
-from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_OSX_CLIENT
-from mojo.interop.clients.base.baseclientcoordinatorcoupling import BaseClientCoordinatorCoupling
+from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_LINUX_CLIENT
+from mojo.xmods.landscaping.client.clientcoordinatorcouplingbase import ClientCoordinatorCouplingBase
 
-class OsxClientCoordinatorCoupling(BaseClientCoordinatorCoupling):
+
+class LinuxClientCoordinatorCoupling(ClientCoordinatorCouplingBase):
     """
-        The OsxClientCoordinatorCoupling handle the requirement registration for the OSX coordinator.
+        The LinuxClientCoordinatorCoupling handle the requirement registration for the Linux coordinator.
     """
 
-    pathbase = "/osx"
-
     integration_section: str = "devices"
     integration_leaf: str = "deviceType"
-    integration_class: str = INTEGRATION_CLASS_FOR_OSX_CLIENT
+    integration_class: str = INTEGRATION_CLASS_FOR_LINUX_CLIENT
 
     def __init__(self, *args, **kwargs):
         """
-            The default contructor for an :class:`OsxCoordinatorIntegration`.
+            The default contructor for an :class:`LinuxCoordinatorIntegration`.
         """
         super().__init__(*args, **kwargs)
         return
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/windows/windowsclient.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/clients/osx/osxclient.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 from typing import TYPE_CHECKING
 
 from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
+from mojo.xmods.landscaping.client.clientbase import ClientBase
 
-from mojo.interop.clients.base.baseclient import BaseClient
 
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
     from mojo.xmods.landscaping.coordinators.coordinatorbase import CoordinatorBase
 
-class WindowsClient(BaseClient):
+class OsxClient(ClientBase):
 
     def __init__(self, lscape: "Landscape", coordinator: "CoordinatorBase",
                  friendly_id:FriendlyIdentifier, device_type: str, device_config: dict):
         super().__init__(lscape, coordinator, friendly_id, device_type, device_config)
         return
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 from typing import TYPE_CHECKING
 
-from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_WINDOWS_CLIENT
-
-from mojo.interop.clients.base.baseclientcoordinator import BaseClientCoordinator
+from mojo.xmods.landscaping.client.clientcoordinatorbase import ClientCoordinatorBase
 
+from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_WINDOWS_CLIENT
 from mojo.interop.clients.windows.windowsclient import WindowsClient
 
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
-class WindowsClientCoordinator(BaseClientCoordinator):
+class WindowsClientCoordinator(ClientCoordinatorBase):
     """
         The :class:`WindowsPoolCoordinator` creates a pool of agents that can be used to
         coordinate the interop activities of the automation process and remote Windows
         client.
     """
 
     INTEGRATION_CLASS = INTEGRATION_CLASS_FOR_WINDOWS_CLIENT
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,23 +14,22 @@
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 from typing import TYPE_CHECKING
 
 from mojo.interop.clients.constants import INTEGRATION_CLASS_FOR_WINDOWS_CLIENT
-from mojo.interop.clients.base.baseclientcoordinatorcoupling import BaseClientCoordinatorCoupling
+from mojo.xmods.landscaping.client.clientcoordinatorcouplingbase import ClientCoordinatorCouplingBase
 
-class WindowsClientCoordinatorCoupling(BaseClientCoordinatorCoupling):
+
+class WindowsClientCoordinatorCoupling(ClientCoordinatorCouplingBase):
     """
         The WindowsClientCoordinatorCoupling handle the requirement registration for the Windows coordinator.
     """
 
-    pathbase = "/windows"
-
     integration_section: str = "devices"
     integration_leaf: str = "deviceType"
     integration_class: str = INTEGRATION_CLASS_FOR_WINDOWS_CLIENT
 
     def __init__(self, *args, **kwargs):
         """
             The default contructor for an :class:`WindowsCoordinatorIntegration`.
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clusters/base/basenode.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/ssh/sshdevice.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 
-
 from typing import TYPE_CHECKING
 
 from mojo.xmods.landscaping.landscapedevice import LandscapeDevice
 from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
 
 from mojo.interop.protocols.ssh.sshagent import SshAgent
 
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
     from mojo.xmods.landscaping.coordinators.coordinatorbase import CoordinatorBase
 
-class BaseNode(LandscapeDevice):
+class SshDevice(LandscapeDevice):
 
     def __init__(self, lscape: "Landscape", coordinator: "CoordinatorBase",
                  friendly_id:FriendlyIdentifier, device_type: str, device_config: dict):
         super().__init__(lscape, coordinator, friendly_id, device_type, device_config)
 
         self._host = device_config["host"]
         return
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/clusters/base/basenodecoordinatorcoupling.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,114 @@
 """
-.. module:: basenodecoordinatorcoupling
+.. module:: powercoordinatorcoupling
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: Contains a BaseNodeCoordinatorCoupling object to use for working with the OSX clients.
+    :synopsis: Contains a PowerCoordinatorCoupling object to use for working with standard
+               power agent types.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
 __version__ = "1.0.0"
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
-
 from typing import Any, Dict, List, Tuple, TYPE_CHECKING
 
-from functools import partial
-
 from mojo.xmods.exceptions import SemanticError
 from mojo.xmods.landscaping.coupling.coordinatorcoupling import CoordinatorCoupling
 from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
 from mojo.xmods.landscaping.landscape import LandscapeDevice
-from mojo.interop.clusters.base.basenodecoordinator import BaseNodeCoordinator
+from mojo.interop.protocols.ssh.sshcoordinator import SshCoordinator
 
 from mojo.xmods.landscaping.precedence import StartupLevel
 
 # Types imported only for type checking purposes
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
-SUPPORTED_INTEGRATION_CLASS = "network/node-base"
+SUPPORTED_INTEGRATION_CLASS = "network/dlipower"
 
-def is_matching_client_config(integ_class, device_info):
-    is_matching_client = False
+def is_dlipower_type(config_info) -> bool:
+    is_sst = False
 
-    dev_type = device_info["deviceType"]
-    if dev_type == integ_class:
-        is_matching_client = True
+    if "powerType" in config_info:
+        stval = config_info["powerType"]
+        if stval == SUPPORTED_INTEGRATION_CLASS:
+            is_sst = True
 
-    return is_matching_client
+    return is_sst
 
-class BaseNodeCoordinatorCoupling(CoordinatorCoupling):
+class PowerCoordinatorCoupling(CoordinatorCoupling):
     """
-        The BaseNodeCoordinatorCoupling handle the requirement registration for the OSX coordinator.
+        The PowerCoordinatorCoupling handle the requirement registration for the SSH coordinator.
     """
 
-    pathbase = "/base"
-
-    integration_section: str = "devices"
-    integration_leaf: str = "deviceType"
+    integration_section: str = "power"
+    integration_leaf: str = "powerType"
     integration_class: str = SUPPORTED_INTEGRATION_CLASS
 
     def __init__(self, *args, **kwargs):
         """
-            The default contructor for an :class:`BaseNodeCoordinatorIntegration`.
+            The default contructor for an :class:`PowerCoordinatorIntegration`.
         """
         super().__init__(*args, **kwargs)
         return
 
     @classmethod
     def attach_to_environment(cls, landscape: "Landscape"):
         """
             This API is called so that the IntegrationCoupling can process configuration information.  The :class:`IntegrationCoupling`
             will verify that it has a valid environment and configuration to run in.
 
-            :raises :class:`mojo.xmods.exceptions.AKitMissingConfigError`, :class:`mojo.xmods.exceptions.ConfigurationError`:
+            :raises :class:`mojo.xmods.exceptions.ConfigurationError`:
         """
 
         cls.landscape = landscape
         layer_config = landscape.layer_configuration
 
-        device_list = layer_config.get_device_configs()
-        if len(device_list) > 0:
-            dev_client_list = [dev for dev in filter(partial(is_matching_client_config, cls.integration_class), device_list)]
+        power_list = layer_config.get_serial_configs()
+        if len(power_list) > 0:
+            supported_power_list = [pconf for pconf in filter(is_dlipower_type, power_list)]
 
-            if len(dev_client_list) > 0:
+            if len(supported_power_list) > 0:
                 layer_integ = landscape.layer_integration
                 layer_integ.register_integration_dependency(cls)
 
         return
 
     @classmethod
     def collect_resources(cls):
         """
             This API is called so the `IntegrationCoupling` can connect with a resource management
             system and gain access to the resources required for the automation run.
 
-            :raises :class:`mojo.xmods.exceptions.AKitResourceError`:
+            :raises :class:`mojo.xmods.exceptions.ResourceError`:
         """
         return
 
     @classmethod
     def create_coordinator(cls, landscape: "Landscape") -> object:
         """
             This API is called so that the landscape can create a coordinator for a given integration role.
         """
-        cls.coordinator = BaseNodeCoordinator(landscape)
+        cls.coordinator = SshCoordinator(landscape)
         return cls.coordinator
 
     @classmethod
     def declare_precedence(cls) -> int:
         """
             This API is called so that the IntegrationCoupling can declare an ordinal precedence that should be
             utilized for bringing up its integration state.
         """
-        return StartupLevel.PrimaryProtocol
+        return StartupLevel.Power
 
     @classmethod
     def diagnostic(cls, label: str, level: int, diag_folder: str):
         """
             The API is called by the :class:`akit.sequencer.Sequencer` object when the automation sequencer is
             building out a diagnostic package at a diagnostic point in the automation sequence.  Example diagnostic
             points are:
@@ -134,35 +131,17 @@
             This API is called so the `IntegrationCoupling` can establish connectivity with any compute or storage
             resources.
 
             :returns: A tuple with a list of error messages for failed connections and dict of connectivity
                       reports for devices devices based on the coordinator.
         """
 
-        lscape = cls.landscape
-        layer_integ = lscape.layer_integration
+        config_errors = [], scan_results = {}
 
-        device_list = layer_integ.get_devices()
-        if len(device_list) > 0:
-            dev_client_list = [dev for dev in filter(partial(is_matching_client_config, cls.integration_class), device_list)]
-
-            if len(dev_client_list) == 0:
-                raise SemanticError("We should have not been called if no OSX devices are available.")
-
-            dev_config_errors, matching_device_results, missing_device_results = cls.coordinator.attach_to_devices(
-                dev_client_list)
-
-            dev_scan_results = {
-                "osx": {
-                    "matching_devices": matching_device_results,
-                    "missing_devices": missing_device_results
-                }
-            }
-
-        return (dev_config_errors, dev_scan_results)
+        return config_errors, scan_results
 
     @classmethod
     def establish_presence(cls) -> Tuple[List[str], dict]:
         """
             This API is called so the `IntegrationCoupling` can establish presence with any compute or storage
             resources.
 
@@ -171,29 +150,21 @@
         """
         return
 
     @classmethod
     def validate_item_configuration(cls, item_info: Dict[str, Any]) -> Tuple[List[str], List[str]]:
         """
             Validate the item configuration.
-
-            -   deviceType: network/client-osx
-                name: raspey03
-                host: 172.16.1.33
-                credentials:
-                -    pi-cluster
-                features:
-                    isolation: false
-                skip: false
         """
         errors = []
         warnings = []
         
         if "host" not in item_info:
-            errmsg = "Device configuration 'network/client-osx' must have a 'host' field."
+            errmsg = "Serial configuration 'network/dlipower' must have a 'host' field."
             errors.append(errmsg)
 
-        if "credentials" not in item_info:
-            warnmsg = "Device configuration 'network/client-osx' should have a 'credentials' field."
+        if "port" not in item_info:
+            warnmsg = "Device configuration 'network/dlipower' should have a 'port' field."
             warnings.append(warnmsg)
 
-        return errors, warnings
+        return errors, warnings
+
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/__init__.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsaddress.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsaddress.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsapi.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsapi.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsconst.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsconst.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnshostinfo.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnshostinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnspointer.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnspointer.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsquestion.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsquestion.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsrecord.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsrecord.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsserver.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsserver.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsservice.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsservice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnstext.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnstext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsutil.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsutil.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/dnsvalidation.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/dnsvalidation.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/exceptions.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/mdnsagent.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/mdnsagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/dns/testmessages.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/dns/testmessages.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
-.. module:: powercoordinatorcoupling
+.. module:: serialcoordinatorcoupling
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: Contains a PowerCoordinatorCoupling object to use for working with standard
-               power agent types.
+    :synopsis: Contains a TcpSerialCoordinatorCoupling object to use for working with standard
+               serial agent types.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
@@ -14,50 +14,47 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 from typing import Any, Dict, List, Tuple, TYPE_CHECKING
 
-from mojo.xmods.exceptions import SemanticError
 from mojo.xmods.landscaping.coupling.coordinatorcoupling import CoordinatorCoupling
-from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
-from mojo.xmods.landscaping.landscape import LandscapeDevice
 from mojo.interop.protocols.ssh.sshcoordinator import SshCoordinator
 
 from mojo.xmods.landscaping.precedence import StartupLevel
 
 # Types imported only for type checking purposes
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
-SUPPORTED_INTEGRATION_CLASS = "network/dlipower"
+SUPPORTED_INTEGRATION_CLASS = "network/tcpserial"
 
-def is_dlipower_type(config_info) -> bool:
+def is_tcp_serial_type(config_info) -> bool:
     is_sst = False
 
-    if "powerType" in config_info:
-        stval = config_info["powerType"]
+    if "serialType" in config_info:
+        stval = config_info["serialType"]
         if stval == SUPPORTED_INTEGRATION_CLASS:
             is_sst = True
 
     return is_sst
 
-class PowerCoordinatorCoupling(CoordinatorCoupling):
+class TcpSerialCoordinatorCoupling(CoordinatorCoupling):
     """
-        The PowerCoordinatorCoupling handle the requirement registration for the SSH coordinator.
+        The TcpSerialCoordinatorCoupling handle the requirement registration for the SSH coordinator.
     """
 
-    integration_section: str = "power"
-    integration_leaf: str = "powerType"
+    integration_section: str = "serial"
+    integration_leaf: str = "serialType"
     integration_class: str = SUPPORTED_INTEGRATION_CLASS
 
     def __init__(self, *args, **kwargs):
         """
-            The default contructor for an :class:`PowerCoordinatorIntegration`.
+            The default contructor for an :class:`TcpSerialCoordinatorIntegration`.
         """
         super().__init__(*args, **kwargs)
         return
 
     @classmethod
     def attach_to_environment(cls, landscape: "Landscape"):
         """
@@ -66,19 +63,19 @@
 
             :raises :class:`mojo.xmods.exceptions.ConfigurationError`:
         """
 
         cls.landscape = landscape
         layer_config = landscape.layer_configuration
 
-        power_list = layer_config.get_serial_configs()
-        if len(power_list) > 0:
-            supported_power_list = [pconf for pconf in filter(is_dlipower_type, power_list)]
+        serial_list = layer_config.get_serial_configs()
+        if len(serial_list) > 0:
+            supported_serial_list = [sconf for sconf in filter(is_tcp_serial_type, serial_list)]
 
-            if len(supported_power_list) > 0:
+            if len(supported_serial_list) > 0:
                 layer_integ = landscape.layer_integration
                 layer_integ.register_integration_dependency(cls)
 
         return
 
     @classmethod
     def collect_resources(cls):
@@ -100,15 +97,16 @@
 
     @classmethod
     def declare_precedence(cls) -> int:
         """
             This API is called so that the IntegrationCoupling can declare an ordinal precedence that should be
             utilized for bringing up its integration state.
         """
-        return StartupLevel.Power
+        # We need to call the base class, it sets the 'logger' member
+        return StartupLevel.Serial
 
     @classmethod
     def diagnostic(cls, label: str, level: int, diag_folder: str):
         """
             The API is called by the :class:`akit.sequencer.Sequencer` object when the automation sequencer is
             building out a diagnostic package at a diagnostic point in the automation sequence.  Example diagnostic
             points are:
@@ -155,16 +153,15 @@
         """
             Validate the item configuration.
         """
         errors = []
         warnings = []
         
         if "host" not in item_info:
-            errmsg = "Serial configuration 'network/dlipower' must have a 'host' field."
+            errmsg = "Serial configuration 'network/tcpserial' must have a 'host' field."
             errors.append(errmsg)
 
         if "port" not in item_info:
-            warnmsg = "Device configuration 'network/dlipower' should have a 'port' field."
+            warnmsg = "Device configuration 'network/tcpserial' should have a 'port' field."
             warnings.append(warnmsg)
 
-        return errors, warnings
-
+        return errors, warnings
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/serial/tcpserialagent.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/serial/tcpserialagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,103 @@
 """
-.. module:: serialcoordinatorcoupling
+.. module:: automationpodcoupling
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: Contains a TcpSerialCoordinatorCoupling object to use for working with standard
-               serial agent types.
+    :synopsis: Contains a UpnpCoordinatorIntegration object to use for working with the nodes of a cluster
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
-__copyright__ = "Copyright 2023, Myron W Walker"
+__copyright__ = "Copyright 2020, Myron W Walker"
 __credits__ = []
 __version__ = "1.0.0"
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
-from typing import Any, Dict, List, Tuple, TYPE_CHECKING
+from typing import Dict, List, Tuple, TYPE_CHECKING
 
+from mojo.xmods.xcollections.context import ContextPaths
+from mojo.xmods.exceptions import ConfigurationError, SemanticError
 from mojo.xmods.landscaping.coupling.coordinatorcoupling import CoordinatorCoupling
-from mojo.interop.protocols.ssh.sshcoordinator import SshCoordinator
 
-from mojo.xmods.landscaping.precedence import StartupLevel
+from mojo.interop.protocols.upnp.upnpcoordinator import UpnpCoordinator
 
 # Types imported only for type checking purposes
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
-SUPPORTED_INTEGRATION_CLASS = "network/tcpserial"
-
-def is_tcp_serial_type(config_info) -> bool:
-    is_sst = False
-
-    if "serialType" in config_info:
-        stval = config_info["serialType"]
-        if stval == SUPPORTED_INTEGRATION_CLASS:
-            is_sst = True
-
-    return is_sst
-
-class TcpSerialCoordinatorCoupling(CoordinatorCoupling):
+class UpnpCoordinatorIntegration(CoordinatorCoupling):
     """
-        The TcpSerialCoordinatorCoupling handle the requirement registration for the SSH coordinator.
+        The UpnpCoordinatorIntegration handle the requirement registration for the UPNP coordinator.
     """
 
-    integration_section: str = "serial"
-    integration_leaf: str = "serialType"
-    integration_class: str = SUPPORTED_INTEGRATION_CLASS
+    pathbase = "/upnp"
 
     def __init__(self, *args, **kwargs):
         """
-            The default contructor for an :class:`TcpSerialCoordinatorIntegration`.
+            The default contructor for an :class:`UpnpCoordinatorIntegration`.
         """
-        super().__init__(*args, **kwargs)
+        super(UpnpCoordinatorIntegration, self).__init__(*args, **kwargs)
         return
 
     @classmethod
-    def attach_to_environment(cls, landscape: "Landscape"):
+    def attach_to_environment(cls, constraints: Dict={}):
         """
             This API is called so that the IntegrationCoupling can process configuration information.  The :class:`IntegrationCoupling`
             will verify that it has a valid environment and configuration to run in.
 
-            :raises :class:`mojo.xmods.exceptions.ConfigurationError`:
+            :raises :class:`akit.exceptions.AKitMissingConfigError`, :class:`akit.exceptions.AKitInvalidConfigError`:
         """
 
-        cls.landscape = landscape
-        layer_config = landscape.layer_configuration
+        upnp_device_hints = cls.landscape.get_upnp_device_config_lookup_table()
+        if len(upnp_device_hints) > 0:
+            cls.landscape.activate_integration_point("coordinator/upnp", cls.create_coordinator)
 
-        serial_list = layer_config.get_serial_configs()
-        if len(serial_list) > 0:
-            supported_serial_list = [sconf for sconf in filter(is_tcp_serial_type, serial_list)]
-
-            if len(supported_serial_list) > 0:
-                layer_integ = landscape.layer_integration
-                layer_integ.register_integration_dependency(cls)
+        return
 
+    @classmethod
+    def attach_to_framework(cls, landscape: "Landscape"):
+        """
+            This API is called so that the IntegrationCoupling can attach to the test framework and participate with
+            registration processes.  This allows the framework to ignore the bringing-up of couplings that are not being
+            included by a test.
+        """
+        super(UpnpCoordinatorIntegration, cls).attach_to_framework(landscape)
+        cls.landscape.register_integration_point("coordinator/upnp", cls)
         return
 
     @classmethod
     def collect_resources(cls):
         """
             This API is called so the `IntegrationCoupling` can connect with a resource management
             system and gain access to the resources required for the automation run.
 
-            :raises :class:`mojo.xmods.exceptions.ResourceError`:
+            :raises :class:`akit.exceptions.AKitResourceError`:
         """
         return
 
     @classmethod
     def create_coordinator(cls, landscape: "Landscape") -> object:
         """
             This API is called so that the landscape can create a coordinator for a given integration role.
         """
-        cls.coordinator = SshCoordinator(landscape)
+        cls.coordinator = UpnpCoordinator(landscape)
         return cls.coordinator
 
     @classmethod
     def declare_precedence(cls) -> int:
         """
             This API is called so that the IntegrationCoupling can declare an ordinal precedence that should be
             utilized for bringing up its integration state.
         """
         # We need to call the base class, it sets the 'logger' member
-        return StartupLevel.Serial
+        super(UpnpCoordinatorIntegration, cls).declare_precedence()
+        return
 
     @classmethod
     def diagnostic(cls, label: str, level: int, diag_folder: str):
         """
             The API is called by the :class:`akit.sequencer.Sequencer` object when the automation sequencer is
             building out a diagnostic package at a diagnostic point in the automation sequence.  Example diagnostic
             points are:
@@ -117,51 +108,90 @@
             Each diagnostic package has its own storage location so derived :class:`akit.scope.ScopeCoupling` objects
             can simply write to their specified output folder.
 
             :param label: The label associated with this diagnostic.
             :param level: The maximum diagnostic level to run dianostics for.
             :param diag_folder: The output folder path where the diagnostic information should be written.
         """
+
         return
 
     @classmethod
-    def establish_connectivity(cls, allow_missing_devices: bool=False) -> Tuple[List[str], dict]:
+    def establish_connectivity(cls, allow_missing_devices: bool=False, upnp_recording: bool = False, allow_unknown_devices: bool = False) -> Tuple[List[str], dict]:
         """
             This API is called so the `IntegrationCoupling` can establish connectivity with any compute or storage
             resources.
 
             :returns: A tuple with a list of error messages for failed connections and dict of connectivity
                       reports for devices devices based on the coordinator.
         """
+        lscape = cls.landscape
+
+        exclude_interfaces = ["lo"]
+
+        runtime_exclude_interfaces = cls.context.lookup(ContextPaths.UPNP_EXCLUDE_INTERFACES)
+        if runtime_exclude_interfaces is not None:
+            exclude_interfaces = runtime_exclude_interfaces
 
-        config_errors = [], scan_results = {}
+        upnp_hint_table = lscape.get_upnp_device_config_lookup_table()
+        
+        if len(upnp_hint_table) == 0:
+            raise SemanticError("we should not have been called if the upnp device config had 0 devices.") from None
+
+        required_devices = None
+        if not allow_missing_devices:
+            required_devices = [usn for usn in upnp_hint_table.keys()]
+
+        found_device_results, matching_device_results, missing_device_results = cls.coordinator.startup_scan(
+            upnp_hint_table, watchlist=upnp_hint_table, required_devices=required_devices, exclude_interfaces=exclude_interfaces,
+            upnp_recording=upnp_recording, allow_unknown_devices=allow_unknown_devices)
+
+        conn_results = {
+            "upnp": {
+                "found": found_device_results,
+                "matching": matching_device_results,
+                "missing": missing_device_results
+            }
+        }
 
-        return config_errors, scan_results
+        conn_errors = []
+
+        return (conn_errors, conn_results)
 
     @classmethod
     def establish_presence(cls) -> Tuple[List[str], dict]:
         """
             This API is called so the `IntegrationCoupling` can establish presence with any compute or storage
             resources.
 
             :returns: A tuple with a list of error messages for failed connections and dict of connectivity
                       reports for devices devices based on the coordinator.
         """
+        if cls.coordinator is not None:
+            cls.coordinator.establish_presence()
         return
 
-    @classmethod
-    def validate_item_configuration(cls, item_info: Dict[str, Any]) -> Tuple[List[str], List[str]]:
+    def checkout_upnp_device(self, usn):
         """
-            Validate the item configuration.
+            Checkout a device from the device pool by USN.
         """
-        errors = []
-        warnings = []
-        
-        if "host" not in item_info:
-            errmsg = "Serial configuration 'network/tcpserial' must have a 'host' field."
-            errors.append(errmsg)
-
-        if "port" not in item_info:
-            warnmsg = "Device configuration 'network/tcpserial' should have a 'port' field."
-            warnings.append(warnmsg)
+        codev = None
+
+        if usn in self.upnp_devices_pool:
+            codev = self.upnp_devices_pool.pop(usn)
+            self.upnp_devices_inuse[usn] = codev
+
+        return codev
+
+    def checkin_upnp_device(self, codev):
+        """
+            Checkin a device to the device pool.
+        """
+        usn = codev["USN"]
+
+        if usn in self.upnp_devices_inuse:
+            codev = self.upnp_devices_inuse.pop(usn)
+            self.upnp_devices_pool[usn] = codev
+
+        return
 
-        return errors, warnings
+
```

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/ssh/sshagent.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/ssh/sshagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/__init__.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/aspectsupnp.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/aspectsupnp.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/content/didllite.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/content/didllite.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/devices/__init__.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/paths.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/paths.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/soap.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/soap.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnpconstants.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnpconstants.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnperrors.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnperrors.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnpfactory.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnpfactory.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py` & `mojo_interop-0.0.4/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.3/setup.py` & `mojo_interop-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 package_dir = \
 {'': 'source/packages'}
 
 packages = \
 ['mojo',
  'mojo.factories',
  'mojo.interop.clients',
- 'mojo.interop.clients.base',
  'mojo.interop.clients.linux',
  'mojo.interop.clients.osx',
  'mojo.interop.clients.windows',
- 'mojo.interop.clusters.base',
+ 'mojo.interop.clusters',
+ 'mojo.interop.clusters.raspberrypi',
  'mojo.interop.protocols.dns',
  'mojo.interop.protocols.power.dlipower',
  'mojo.interop.protocols.serial',
  'mojo.interop.protocols.ssh',
  'mojo.interop.protocols.upnp',
  'mojo.interop.protocols.upnp.content',
  'mojo.interop.protocols.upnp.devices',
@@ -40,15 +40,15 @@
                                            'standard/services/UPnP/*']}
 
 install_requires = \
 ['mojo-networking>=0.0.4,<0.1.0', 'mojo-xmodules>=0.0.25,<0.1.0']
 
 setup_kwargs = {
     'name': 'mojo-interop',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Automation Mojo Interop Extensions',
     'long_description': '===============================\nAutomation Mojo Interop Package\n===============================\n\nThis *Automation Mojo Interop Package* contains interop extensions that add interop functionality to\nthe test environment *Landscape* object for a variety of platform clients, clusters, and protocols.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_interop-0.0.3/PKG-INFO` & `mojo_interop-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-interop
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automation Mojo Interop Extensions
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

