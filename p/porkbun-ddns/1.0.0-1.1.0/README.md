# Comparing `tmp/porkbun_ddns-1.0.0-py3-none-any.whl.zip` & `tmp/porkbun_ddns-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11055 bytes, number of entries: 12
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-28 05:08 porkbun_ddns/__init__.py
--rw-r--r--  2.0 unx     3593 b- defN 24-Apr-28 05:08 porkbun_ddns/cli.py
--rw-r--r--  2.0 unx     3796 b- defN 24-Apr-28 05:08 porkbun_ddns/config.py
--rw-r--r--  2.0 unx       45 b- defN 24-Apr-28 05:08 porkbun_ddns/errors.py
--rw-r--r--  2.0 unx     1507 b- defN 24-Apr-28 05:08 porkbun_ddns/helpers.py
--rw-r--r--  2.0 unx     9822 b- defN 24-Apr-28 05:08 porkbun_ddns/porkbun_ddns.py
--rw-r--r--  2.0 unx     1061 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6905 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      987 b- defN 24-Apr-28 05:08 porkbun_ddns-1.0.0.dist-info/RECORD
-12 files, 27914 bytes uncompressed, 9387 bytes compressed:  66.4%
+Zip file size: 11096 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       38 b- defN 24-May-11 12:06 porkbun_ddns/__init__.py
+-rw-r--r--  2.0 unx     3593 b- defN 24-May-11 12:06 porkbun_ddns/cli.py
+-rw-r--r--  2.0 unx     3796 b- defN 24-May-11 12:06 porkbun_ddns/config.py
+-rw-r--r--  2.0 unx       45 b- defN 24-May-11 12:06 porkbun_ddns/errors.py
+-rw-r--r--  2.0 unx     1601 b- defN 24-May-11 12:06 porkbun_ddns/helpers.py
+-rw-r--r--  2.0 unx     9984 b- defN 24-May-11 12:06 porkbun_ddns/porkbun_ddns.py
+-rw-r--r--  2.0 unx     1061 b- defN 24-May-11 12:07 porkbun_ddns-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6892 b- defN 24-May-11 12:07 porkbun_ddns-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-11 12:07 porkbun_ddns-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 24-May-11 12:07 porkbun_ddns-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-May-11 12:07 porkbun_ddns-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      987 b- defN 24-May-11 12:07 porkbun_ddns-1.1.0.dist-info/RECORD
+12 files, 28157 bytes uncompressed, 9428 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: porkbun_ddns/helpers.py
 Comment: 
 
 Filename: porkbun_ddns/porkbun_ddns.py
 Comment: 
 
-Filename: porkbun_ddns-1.0.0.dist-info/LICENSE
+Filename: porkbun_ddns-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: porkbun_ddns-1.0.0.dist-info/METADATA
+Filename: porkbun_ddns-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: porkbun_ddns-1.0.0.dist-info/WHEEL
+Filename: porkbun_ddns-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: porkbun_ddns-1.0.0.dist-info/entry_points.txt
+Filename: porkbun_ddns-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: porkbun_ddns-1.0.0.dist-info/top_level.txt
+Filename: porkbun_ddns-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: porkbun_ddns-1.0.0.dist-info/RECORD
+Filename: porkbun_ddns-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## porkbun_ddns/helpers.py

```diff
@@ -1,16 +1,13 @@
-import logging
 import urllib.request
 import xml.etree.ElementTree as ET
 
-logger = logging.getLogger()
 
-
-def get_ips_from_fritzbox(fritzbox_ip):
-    """Retrieves the IP address of the Fritzbox router's external network interface.
+def get_ips_from_fritzbox(fritzbox_ip, ip_version=4):
+    """Retrieves the IP addresses of the Fritzbox router's external network interface.
 
     Args:
     ----
         fritzbox_ip (str): The IP address of the Fritzbox router.
 
     Returns:
     -------
@@ -19,25 +16,29 @@
     Raises:
     ------
         urllib.error.URLError: If there is a problem opening the URL.
 
         ValueError: If the provided `fritzbox_ip` is not a valid IP address.
 
         AttributeError: If the requested field is not found in the XML response.
-
     """
+
     schema = "GetExternalIPAddress"
     field = "NewExternalIPAddress"
 
+    if ip_version == 6:
+        schema = "X_AVM_DE_GetExternalIPv6Address"
+        field = "NewExternalIPv6Address"
+
     req = urllib.request.Request(
         "http://" + fritzbox_ip + ":49000/igdupnp/control/WANIPConn1")
     req.add_header("Content-Type", 'text/xml; charset="utf-8"')
     req.add_header(
         "SOAPAction", "urn:schemas-upnp-org:service:WANIPConnection:1#" + schema)
     data = '<?xml version="1.0" encoding="utf-8"?>' + \
         '<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" s:encodingStyle="http://schemas.xmlsoap.org/soap/encoding/">' + \
         "<s:Body>" + \
-        "<u:" + schema + ' xmlns:u="urn:schemas-upnp-org:service:WANIPConnection:1" />' + \
+        '<u:GetExternalIPAddress xmlns:u="urn:schemas-upnp-org:service:WANIPConnection:1" />' + \
         "</s:Body>" + \
         "</s:Envelope>"
     req.data = data.encode("utf8")
     return ET.fromstring(urllib.request.urlopen(req).read()).find(".//" + field).text
```

## porkbun_ddns/porkbun_ddns.py

```diff
@@ -51,15 +51,18 @@
         if self.static_ips:
             public_ips = self.static_ips
         else:
             public_ips = []
             if self.fritzbox_ip:
                 if self.ipv4:
                     public_ips.append(
-                        get_ips_from_fritzbox(self.fritzbox_ip))
+                        get_ips_from_fritzbox(self.fritzbox_ip, ip_version=4))
+                if self.ipv6:
+                    public_ips.append(
+                        get_ips_from_fritzbox(self.fritzbox_ip, ip_version=6))
             else:
                 if self.ipv4:
                     urls = ["https://v4.ident.me",
                             "https://api.ipify.org",
                             "https://ipv4.icanhazip.com"]
                     for url in urls:
                         try:
```

## Comparing `porkbun_ddns-1.0.0.dist-info/LICENSE` & `porkbun_ddns-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `porkbun_ddns-1.0.0.dist-info/METADATA` & `porkbun_ddns-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 1.0.0
+Version: 1.1.0
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
@@ -151,26 +151,24 @@
       # FRITZBOX: "192.168.178.1" # Use Fritz!BOX to obtain Public IP's
       # SLEEP: "300" # Seconds to sleep between DynDNS runs
       # IPV4: "TRUE" # Set IPv4 address
       # DEBUG: "FALSE" # DEBUG LOGGING
     restart: unless-stopped
 ```
 
-You have to use `docker run` if you want to use IPv6, see https://github.com/mietzen/porkbun-ddns/issues/34
+You have to use `docker run` with `-e IPV6="TRUE"` if you want to use IPv6, see https://github.com/mietzen/porkbun-ddns/issues/34
 
 # Docker run
 
 ```shell
 docker run -d \
   -e DOMAIN="domain.com" \
   -e SUBDOMAINS="my_subdomain,my_other_subdomain,my_subsubdomain.my_subdomain" \
   -e SECRETAPIKEY="<YOUR-SECRETAPIKEY>" \
   -e APIKEY="<YOUR-APIKEY>" \
-  -e IPV4="TRUE" \
-  -e IPV6="TRUE" \
   --name porkbun-ddns \
   --restart unless-stopped \
   mietzen/porkbun-ddns:latest
 ```
 
 # Python
 
@@ -183,12 +181,12 @@
 
 
 config = Config(DEFAULT_ENDPOINT, "YOUR-APIKEY", "YOUR-SECRETAPIKEY")
 porkbun_ddns = PorkbunDDNS(config, 'domain.com')
 # config = extract_config(Path("./config.json"))
 # porkbun_ddns = PorkbunDDNS(config, 'domain.com')
 # porkbun_ddns_ip = PorkbunDDNS(config, 'domain.com', public_ips=['1.2.3.4','1234:abcd:0:4567::8900'])
-# porkbun_ddns_fritz = PorkbunDDNS(config, 'domain.com', fritzbox='fritz.box', ipv6=False)
+# porkbun_ddns_fritz = PorkbunDDNS(config, 'domain.com', fritzbox_ip='fritz.box', ipv6=False)
 
 porkbun_ddns.set_subdomain('my_subdomain')
 porkbun_ddns.update_records()
 ```
```

## Comparing `porkbun_ddns-1.0.0.dist-info/RECORD` & `porkbun_ddns-1.1.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 porkbun_ddns/__init__.py,sha256=XumKSWFK5qfGiCSkPPcNCaE44OLJ4r1upBBwJm5s_1Q,38
 porkbun_ddns/cli.py,sha256=0ulurkVBJNBKNAYAX_4vVbCjN75jgACPqA-FFKRcSi8,3593
 porkbun_ddns/config.py,sha256=QMvapsNLQw8HajK6XkW6asJz-XsMs51mnmjQxXz4PVw,3796
 porkbun_ddns/errors.py,sha256=Kv2CY-7lQf6WtYJGUfjjGFKMpvgP85qo4SX38f09_NU,45
-porkbun_ddns/helpers.py,sha256=j6_auR6ffQr51NFOY1i9-EJ7_D4FPFovhpVf5c3hkbE,1507
-porkbun_ddns/porkbun_ddns.py,sha256=h6-HyGfwTENNk5FRKUJcsxT3XOinrUuyjfwNCufEBik,9822
-porkbun_ddns-1.0.0.dist-info/LICENSE,sha256=WbmjIVUkxwQ1vDNiEe2eMKL3-6nYRBN1qUv7rdvvSvY,1061
-porkbun_ddns-1.0.0.dist-info/METADATA,sha256=EscoXJVf_3SwpHtg50btUQe8YMItxY4R9pIKaStVgEA,6905
-porkbun_ddns-1.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-porkbun_ddns-1.0.0.dist-info/entry_points.txt,sha256=Ux4_6ekA_PZiOxw-7MbJOvQVo_7IJQzaYS24EzSjwbg,55
-porkbun_ddns-1.0.0.dist-info/top_level.txt,sha256=8hi5L7CGOlYLIOlnnPPToRxZqnZ1UkpUmCYbgYZO2JA,13
-porkbun_ddns-1.0.0.dist-info/RECORD,,
+porkbun_ddns/helpers.py,sha256=hNAF5G7-kR89pWJx8mPZGIm-L4oHhpUm1NT8vcEx-Ho,1601
+porkbun_ddns/porkbun_ddns.py,sha256=0myhALghv_bkDGn5YXfF0wzbQBxFSjylrqP2ok30Ul8,9984
+porkbun_ddns-1.1.0.dist-info/LICENSE,sha256=WbmjIVUkxwQ1vDNiEe2eMKL3-6nYRBN1qUv7rdvvSvY,1061
+porkbun_ddns-1.1.0.dist-info/METADATA,sha256=eDJDIEJLTO5TFs9DEuKa1Brl1I7sM4l1W0_k7YoW5Rw,6892
+porkbun_ddns-1.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+porkbun_ddns-1.1.0.dist-info/entry_points.txt,sha256=Ux4_6ekA_PZiOxw-7MbJOvQVo_7IJQzaYS24EzSjwbg,55
+porkbun_ddns-1.1.0.dist-info/top_level.txt,sha256=8hi5L7CGOlYLIOlnnPPToRxZqnZ1UkpUmCYbgYZO2JA,13
+porkbun_ddns-1.1.0.dist-info/RECORD,,
```

