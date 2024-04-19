# Comparing `tmp/python_ipware-2.0.4.tar.gz` & `tmp/python_ipware-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ipware-2.0.4.tar", last modified: Thu Apr 18 15:32:55 2024, max compression
+gzip compressed data, was "python_ipware-2.0.5.tar", last modified: Fri Apr 19 19:42:29 2024, max compression
```

## Comparing `python_ipware-2.0.4.tar` & `python_ipware-2.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:32:55.889346 python_ipware-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-18 15:32:51.000000 python_ipware-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-18 15:32:55.889346 python_ipware-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14113 2024-04-18 15:32:51.000000 python_ipware-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-18 15:32:51.000000 python_ipware-2.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:32:55.889346 python_ipware-2.0.4/python_ipware/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 15:32:51.000000 python_ipware-2.0.4/python_ipware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 15:32:51.000000 python_ipware-2.0.4/python_ipware/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:32:51.000000 python_ipware-2.0.4/python_ipware/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-04-18 15:32:51.000000 python_ipware-2.0.4/python_ipware/python_ipware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:32:55.889346 python_ipware-2.0.4/python_ipware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-18 15:32:55.000000 python_ipware-2.0.4/python_ipware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-18 15:32:55.000000 python_ipware-2.0.4/python_ipware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:32:55.000000 python_ipware-2.0.4/python_ipware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 15:32:55.000000 python_ipware-2.0.4/python_ipware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 15:32:55.000000 python_ipware-2.0.4/python_ipware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:32:55.889346 python_ipware-2.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:32:55.889346 python_ipware-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18211 2024-04-18 15:32:51.000000 python_ipware-2.0.4/tests/tests_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-18 15:32:51.000000 python_ipware-2.0.4/tests/tests_ipv6.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:29.628545 python_ipware-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-19 19:42:24.000000 python_ipware-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-19 19:42:29.628545 python_ipware-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14113 2024-04-19 19:42:24.000000 python_ipware-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-19 19:42:24.000000 python_ipware-2.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:29.628545 python_ipware-2.0.5/python_ipware/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-19 19:42:24.000000 python_ipware-2.0.5/python_ipware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 19:42:24.000000 python_ipware-2.0.5/python_ipware/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:24.000000 python_ipware-2.0.5/python_ipware/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-04-19 19:42:24.000000 python_ipware-2.0.5/python_ipware/python_ipware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:29.628545 python_ipware-2.0.5/python_ipware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-19 19:42:29.000000 python_ipware-2.0.5/python_ipware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 19:42:29.000000 python_ipware-2.0.5/python_ipware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:42:29.000000 python_ipware-2.0.5/python_ipware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 19:42:29.000000 python_ipware-2.0.5/python_ipware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 19:42:29.000000 python_ipware-2.0.5/python_ipware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:42:29.628545 python_ipware-2.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:29.628545 python_ipware-2.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18872 2024-04-19 19:42:24.000000 python_ipware-2.0.5/tests/tests_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-19 19:42:24.000000 python_ipware-2.0.5/tests/tests_ipv6.py
```

### Comparing `python_ipware-2.0.4/LICENSE` & `python_ipware-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ipware-2.0.4/PKG-INFO` & `python_ipware-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ipware
-Version: 2.0.4
+Version: 2.0.5
 Summary: A Python package to retrieve user's IP address
 Author-email: Val Neekman <info@neekware.com>
 License: MIT
 Project-URL: Documentation, https://github.com/un33k/python-ipware#readme
 Project-URL: Issues, https://github.com/un33k/python-ipware/issues
 Project-URL: Source, https://github.com/un33k/python-ipware
 Project-URL: Changelog, https://github.com/un33k/python-ipware/blob/main/CHANGELOG.md
```

### Comparing `python_ipware-2.0.4/README.md` & `python_ipware-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `python_ipware-2.0.4/pyproject.toml` & `python_ipware-2.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_ipware-2.0.4/python_ipware/python_ipware.py` & `python_ipware-2.0.5/python_ipware/python_ipware.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,346 +1,335 @@
 import ipaddress
 import logging
 
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 IpAddressType = Union[ipaddress.IPv4Address, ipaddress.IPv6Address]
 OptionalIpAddressType = Optional[IpAddressType]
 
 logger = logging.getLogger(__name__)
 
 
 class IpWareMeta:
     """
-    A class that handles meta data frm an HTTP request.
+    A class to manage metadata extracted from HTTP request headers, primarily for identifying
+    the client's IP address behind load balancers and proxies.
     """
 
     def __init__(
-        self,
-        precedence: Optional[Tuple[str, ...]] = None,
-        leftmost: bool = True,
+        self, precedence: Optional[Tuple[str, ...]] = None, leftmost: bool = True
     ) -> None:
-        self.precedence = precedence or (
-            "X_FORWARDED_FOR",  # Load balancers or proxies such as AWS ELB (default client is `left-most` [`<client>, <proxy1>, <proxy2>`])
-            "HTTP_X_FORWARDED_FOR",  # Similar to X_FORWARDED_TO
-            "HTTP_CLIENT_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
-            "HTTP_X_REAL_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
-            "HTTP_X_FORWARDED",  # Squid and others
-            "HTTP_X_CLUSTER_CLIENT_IP",  # Rackspace LB and Riverbed Stingray
-            "HTTP_FORWARDED_FOR",  # RFC 7239
-            "HTTP_FORWARDED",  # RFC 7239
-            "HTTP_CF_CONNECTING_IP",  # CloudFlare
-            "X-CLIENT-IP",  # Microsoft Azure
-            "X-REAL-IP",  # NGINX
-            "X-CLUSTER-CLIENT-IP",  # Rackspace Cloud Load Balancers
-            "X_FORWARDED",  # Squid
-            "FORWARDED_FOR",  # RFC 7239
-            "CF-CONNECTING-IP",  # CloudFlare
-            "TRUE-CLIENT-IP",  # CloudFlare Enterprise,
-            "FASTLY-CLIENT-IP",  # Firebase, Fastly
-            "FORWARDED",  # RFC 7239
-            "CLIENT-IP",  # Akamai and Cloudflare: True-Client-IP and Fastly: Fastly-Client-IP
-            "REMOTE_ADDR",  # Default
-        )
+        """
+        Initializes the metadata handler with a precedence list of HTTP headers and the position of the client IP.
+
+        :param precedence: A tuple of header names that define the order to check for a valid IP.
+                           If not provided, a default list of commonly used headers is applied.
+        :param leftmost: A boolean that indicates whether to use the left-most IP in the header
+                         when multiple IPs are listed (typically the case with proxies).
+        """
+        # Default precedence list of headers if none is provided
+        if precedence is None:
+            precedence = (
+                "X_FORWARDED_FOR",  # Common header for proxies, load balancers, like AWS ELB. Default to the left-most IP.
+                "HTTP_X_FORWARDED_FOR",  # Alternative header similar to `X_FORWARDED_FOR`.
+                "HTTP_CLIENT_IP",  # Header used by some providers like Amazon EC2, Heroku.
+                "HTTP_X_REAL_IP",  # Header used by some providers like Amazon EC2, Heroku.
+                "HTTP_X_FORWARDED",  # Used by Squid and similar software.
+                "HTTP_X_CLUSTER_CLIENT_IP",  # Used by Rackspace LB, Riverbed Stingray.
+                "HTTP_FORWARDED_FOR",  # Standard header defined by RFC 7239.
+                "HTTP_FORWARDED",  # Standard header defined by RFC 7239.
+                "HTTP_CF_CONNECTING_IP",  # Used by CloudFlare.
+                "X-CLIENT-IP",  # Used by Microsoft Azure.
+                "X-REAL-IP",  # Commonly used by NGINX.
+                "X-CLUSTER-CLIENT-IP",  # Used by Rackspace Cloud Load Balancers.
+                "X_FORWARDED",  # Used by Squid.
+                "FORWARDED_FOR",  # Standard header defined by RFC 7239.
+                "CF-CONNECTING-IP",  # Used by CloudFlare.
+                "TRUE-CLIENT-IP",  # Header for CloudFlare Enterprise.
+                "FASTLY-CLIENT-IP",  # Used by Fastly, Firebase.
+                "FORWARDED",  # Standard header defined by RFC 7239.
+                "CLIENT-IP",  # Used by Akamai, Cloudflare's True-Client-IP, and Fastly's Fastly-Client-IP.
+                "REMOTE_ADDR",  # The default IP address header (direct connection).
+            )
+
+        self.precedence = precedence
         self.leftmost = leftmost
 
 
 class IpWareIpAddress:
     """
-    A class that handles IP address data from an HTTP request.
+    A class for handling and parsing IP address data from HTTP requests.
     """
 
-    def extract_ipv4_only(self, ip_address: str) -> str:
+    def extract_ipv4(self, ip_address: str) -> str:
         """
-        Given an IPv4 address or address:port, it extracts the IP address
-        @param ip_str: IP address or address:port
-        @return: IP address
-        """
-
-        if ip_address:
-            # handle ipv4 addresses with port
-            if ":" in ip_address:
-                ip_address = ip_address.split(":")[0]
-                return ip_address.strip()
+        Extracts the IPv4 address from a given string that may include a port number.
 
-            return ip_address.strip()
+        Args:
+            ip_address (str): An IPv4 address possibly including a port (e.g., "192.168.1.1:8080").
 
-        return ""
-
-    def extract_ipv6_only(self, ip_address: str) -> str:
-        """
-        Given an IPv6 address or address:port, it extracts the IP address
-        @param ip_str: IP address or address:port
-        @return: IP address
+        Returns:
+            str: The IPv4 address without the port. Returns an empty string if input is None.
         """
-
         if ip_address:
-            # handle ipv6 addresses with port
-            if "]:" in ip_address:
-                ip_address = ip_address.split("]:")[0]
-                ip_address = ip_address.replace("[", "")
-                return ip_address.strip()
+            return ip_address.split(":")[0].strip()
+        return ""
 
-            return ip_address.strip()
+    def extract_ipv6(self, ip_address: str) -> str:
+        """
+        Extracts the IPv6 address from a given string that may include a port number.
 
-        return ""
+        Args:
+            ip_address (str): An IPv6 address possibly including a port (e.g., "[2001:db8::1]:8080").
 
-    def get_ip_object(
-        self,
-        ip_str: str,
-    ) -> OptionalIpAddressType:
+        Returns:
+            str: The IPv6 address without brackets or port. Returns an empty string if input is None.
         """
-        Given an IP address or address:port, it parses the IP address
-        @param ip_str: IP address or address:port
-        @return: IP address of type IPv4Address or IPv6Address
+        if ip_address and "]:" in ip_address:
+            return ip_address.split("]:")[0].replace("[", "").strip()
+        return ip_address.strip() if ip_address else ""
+
+    def parse_ip_address(self, ip_str: str):
         """
+        Parses the given IP address string to an IPv4Address or IPv6Address object.
 
-        ip: OptionalIpAddressType = None
-        if ip_str:
+        Args:
+            ip_str (str): An IP address possibly including a port.
+
+        Returns:
+            ipaddress.IPv4Address|ipaddress.IPv6Address|None: The parsed IP object or None if the address is invalid.
+        """
+        try:
+            # First, try to parse as IPv6.
+            ipv6 = self.extract_ipv6(ip_str)
+            ip = ipaddress.IPv6Address(ipv6)
+            return ip.ipv4_mapped or ip
+        except ipaddress.AddressValueError:
             try:
-                # try to parse as IPv6 address with optional port
-                ipv6 = self.extract_ipv6_only(ip_str)
-                ip = ipaddress.IPv6Address(ipv6)
-                ip = ip.ipv4_mapped or ip
+                # If IPv6 parsing fails, try to parse as IPv4.
+                ipv4 = self.extract_ipv4(ip_str)
+                return ipaddress.IPv4Address(ipv4)
             except ipaddress.AddressValueError:
-                try:
-                    # try to parse as IPv4 address with optional port
-                    ipv4 = self.extract_ipv4_only(ip_str)
-                    ip = ipaddress.IPv4Address(ipv4)
-                except ipaddress.AddressValueError:
-                    # not a valid IP address, return None
-                    logger.info("Invalid ip address. {0}".format(ip_str))
-                    ip = None
-        return ip
+                # Log error if IP is invalid
+                # print(f"Invalid IP address: {ip_str}")
+                return None
 
     def get_ips_from_string(
         self,
         ip_str: str,
-    ) -> Optional[List[IpAddressType]]:
-        """
-        Given a comma separated list of IP addresses or address:port, it parses the IP addresses
-        @param ip_str: comma separated list of IP addresses or address:port
-        @return: list of IP addresses of type IPv4Address or IPv6Address
+        strict: bool = False,
+    ) -> Optional[List[Union[ipaddress.IPv4Address, ipaddress.IPv6Address]]]:
         """
-        ip_list: List[IpAddressType] = []
+        Parses a comma-separated list of IP addresses, each possibly including a port.
 
+        Args:
+            ip_str (str): A comma-separated list of IP addresses or address:port entries.
+            strict (bool): True to bail out on first invalid ip, False to skip invalid ip
+        Returns:
+            List[ipaddress.IPv4Address|ipaddress.IPv6Address]|None: A list of IP address objects or None if any IP is invalid.
+        """
+        ip_list = []
         for ip_address in ip_str.split(","):
-            ip = self.get_ip_object(ip_address.strip())
+            ip = self.parse_ip_address(ip_address.strip())
             if ip:
                 ip_list.append(ip)
             else:
-                # we have at least one invalid IP address, return empty list, instead
-                return None
+                if strict:
+                    return None
 
         if not self.leftmost:
             ip_list.reverse()
 
         return ip_list
 
 
 class IpWareProxy:
     """
-    A class that handles proxy data from an HTTP request.
+    A class to handle proxy data from an HTTP request, including validating
+    proxy counts and trusted proxy lists.
     """
 
     def __init__(
-        self,
-        proxy_count: Optional[int] = None,
-        proxy_list: Optional[List[str]] = None,
+        self, proxy_count: Optional[int] = None, proxy_list: Optional[List[str]] = None
     ) -> None:
-        self.proxy_count = proxy_count
-        self.proxy_list = self._is_valid_proxy_trusted_list(proxy_list or [])
+        """
+        Initialize the IpWareProxy class with optional proxy count and proxy list.
 
-    def _is_valid_proxy_trusted_list(self, proxy_list: Any) -> List[str]:
+        Args:
+            proxy_count: The expected number of proxies, can be None if no specific count is enforced.
+            proxy_list: A list of partial IP addresses as trusted proxies, can be None.
         """
-        Checks if the proxy list is a valid list of strings
-        @return: proxy list or raises an exception
+        if proxy_count is not None and proxy_count < 0:
+            raise ValueError("proxy_count must be non-negative")
+        self.proxy_count = proxy_count
+        self.proxy_list = self._validate_proxy_list(proxy_list or [])
+
+    def _validate_proxy_list(self, proxy_list: List[str]) -> List[str]:
         """
+        Validates that the proxy list contains only strings.
+
+        Args:
+            proxy_list: A list of proxies.
 
-        if not isinstance(proxy_list, list):
-            raise ValueError("Parameter must be a list")
-        if not all(isinstance(x, str) for x in proxy_list):
-            raise ValueError("All elements in list must be strings")
+        Returns:
+            The proxy list if all items are valid strings.
 
+        Raises:
+            ValueError: If the proxy list is not a list of strings.
+        """
+        if not all(isinstance(ip, str) for ip in proxy_list):
+            raise ValueError("All elements in the proxy list must be strings.")
         return proxy_list
 
-    def is_proxy_count_valid(
-        self, ip_list: List[IpAddressType], strict: bool = False
-    ) -> bool:
+    def is_proxy_count_valid(self, ip_list: List[str], strict: bool = False) -> bool:
         """
-        Checks if the proxy count is valid
-        @param ip_list: list of ip addresses
-        @param strict: if True, we must have exactly proxy_count proxies, including `0` proxies
-        @return: True if the proxy count is valid, False otherwise
+        Validates the proxy count against a list of IP addresses.
+
+        Args:
+            ip_list: A list of IP addresses from the request headers.
+            strict: If True, the number of proxies must exactly match the proxy_count.
+
+        Returns:
+            True if the proxy count is valid, False otherwise.
         """
-        # No proxy count check is required
         if self.proxy_count is None:
-            return True
-
-        ip_count: int = len(ip_list)
+            return True  # No proxy count specified, so always valid.
 
+        ip_count = len(ip_list)
         if strict:
-            # our first proxy takes the last ip address and treats it as client ip
-            return self.proxy_count == ip_count - 1
+            return ip_count - 1 == self.proxy_count
+            # Exact match required, excluding client's own IP.
 
-        # the client could have gone through their own proxy and included extra ips
-        # client could be sending in the header: X-Forwarded-For: <fake_ip>, <client_ip>
-        return ip_count - 1 > self.proxy_count
+        return ip_count - 1 >= self.proxy_count
+        # Allow more proxies than the count, excluding client's IP.
 
     def is_proxy_trusted_list_valid(
-        self,
-        ip_list: List[IpAddressType],
-        strict: bool = False,
+        self, ip_list: List[str], strict: bool = False
     ) -> bool:
         """
-        Checks if the proxy list is valid (all proxies are in the proxy_list)
-        @param ip_list: list of ip addresses
-        @param strict: if True, we must have exactly proxy_count proxies
-        @return: client's best match ip address or False
+        Checks if all proxies in the incoming list are trusted based on the proxy_list.
+
+        Args:
+            ip_list: A list of IP addresses from the request headers.
+            strict: If True, the number of proxies must exactly match the length of proxy_list.
+
+        Returns:
+            True if all proxies are trusted, False otherwise.
         """
         if not self.proxy_list:
-            return True
+            return True  # No specific proxies to trust, so always valid.
 
         ip_count = len(ip_list)
         proxy_list_count = len(self.proxy_list)
 
-        # in strict mode, total ip count must be 1 more than proxy count
         if strict and ip_count - 1 != proxy_list_count:
-            return False
+            return False  # Strict mode: Exact count match required.
 
-        # total ip count (client + proxies) must be more than proxy count
         if ip_count - 1 < proxy_list_count:
-            return False
+            return False  # Not enough IPs to match the trusted proxies.
 
-        # start from the end, slice the incoming ip list to the same length as the trusted proxy list
-        ip_list_slice = ip_list[-proxy_list_count:]
-        for index, value in enumerate(ip_list_slice):
-            if not str(value).startswith(self.proxy_list[index]):
-                return False
-
-        return True
+        # Verify each proxy against the trusted list by comparing each corresponding element.
+        return all(
+            str(ip).startswith(trusted_proxy_pattern)
+            for ip, trusted_proxy_pattern in zip(
+                ip_list[-proxy_list_count:], self.proxy_list
+            )
+        )
 
 
 class IpWare(IpWareMeta, IpWareProxy, IpWareIpAddress):
     """
-    A class that makes best effort to determine the client's IP address.
+    A class that makes a best effort to determine the client's IP address.
     """
 
     def __init__(
         self,
         precedence: Optional[Tuple[str, ...]] = None,
         leftmost: bool = True,
         proxy_count: Optional[int] = None,
         proxy_list: Optional[List[str]] = None,
     ) -> None:
         IpWareMeta.__init__(self, precedence, leftmost)
         IpWareProxy.__init__(self, proxy_count, proxy_list)
 
     def get_meta_value(self, meta: Dict[str, str], key: str) -> str:
         """
-        Given a key, it returns a cleaned up version of the value
-        @param key: the key to lookup
-        @return: the value of the key or empty string
+        Returns a cleaned up version of the value for a given key.
+        @param key: The key to look up.
+        @return: The value of the key or an empty string if the key is not found.
         """
         meta = meta or {}
         return meta.get(key, meta.get(key.replace("_", "-"), "")).strip()
 
     def get_meta_values(self, meta: Dict[str, str]) -> List[str]:
         """
-        Given a list of keys, it returns a list of cleaned up values
-        @return: a list of values
+        Returns a list of cleaned up values for the keys defined in 'precedence'.
+        @return: A list of values.
         """
         meta_list: List[str] = []
         for key in self.precedence:
             value = self.get_meta_value(meta, key).strip()
             if value:
                 meta_list.append(value)
-
         return meta_list
 
     def get_client_ip(
         self,
         meta: Dict[str, str],
         strict: bool = False,
     ) -> Tuple[OptionalIpAddressType, bool]:
         """
         Returns the client's IP address.
         """
-
         loopback_list: List[IpAddressType] = []
         private_list: List[OptionalIpAddressType] = []
 
         for ip_str in self.get_meta_values(meta):
-
-            ip_list = self.get_ips_from_string(ip_str)
+            ip_list = self.get_ips_from_string(ip_str, strict)
             if not ip_list:
                 continue
 
             proxy_count_validated = self.is_proxy_count_valid(ip_list, strict)
             if not proxy_count_validated:
                 continue
 
             proxy_list_validated = self.is_proxy_trusted_list_valid(ip_list, strict)
             if not proxy_list_validated:
                 continue
 
-            client_ip, trusted_route = self.get_best_ip(
-                ip_list, proxy_count_validated, proxy_list_validated
-            )
-
-            # we found a global ip, return it
-            if client_ip is not None and client_ip.is_global:
-                return client_ip, trusted_route
-
-            # we found a private ip, save it
-            if client_ip is not None and client_ip.is_loopback:
-                loopback_list.append(client_ip)
-            else:
-                # if not global (public) or loopback (local), we treat it asd private
-                private_list.append(client_ip)
+            client_ip, trusted_route = self.get_best_ip(ip_list)
+            if client_ip is not None:
+                if client_ip.is_global:
+                    return client_ip, trusted_route
+                if client_ip.is_loopback:
+                    loopback_list.append(client_ip)
+                else:
+                    private_list.append(client_ip)
 
-        # we have not been able to locate a global ip
-        # it could be the server is running on the intranet
-        # we will return the first private ip we found
         if private_list:
             return private_list[0], False
-
-        # we have not been able to locate a global ip, nor a private ip
-        # it could be the server is running on a loopback address serving local requests
         if loopback_list:
             return loopback_list[0], False
-
-        # we were unable to find any ip address
         return None, False
 
     def get_best_ip(
         self,
         ip_list: List[IpAddressType],
-        proxy_count_validated: bool = True,
-        proxy_list_validated: bool = True,
     ) -> Tuple[OptionalIpAddressType, bool]:
         """
-        Returns the best possible ip for the client.
+        Determines the best possible IP address for the client from a list of IP addresses.
         """
-
         if not ip_list:
-            logger.warning("Invalid ip list provided.")
+            logger.warning("Invalid IP list provided.")
             return None, False
 
-        # the incoming ips match our trusted proxy list
-        if len(self.proxy_list) > 0 and proxy_list_validated:
+        if self.proxy_list and len(self.proxy_list) > 0:
             best_client_ip_index = len(self.proxy_list) + 1
             best_client_ip = ip_list[-best_client_ip_index]
             return best_client_ip, True
 
-        # the incoming ips match our proxy count
-        if (
-            self.proxy_count is not None
-            and self.proxy_count > 0
-            and proxy_count_validated
-        ):
+        if self.proxy_count is not None:
             best_client_ip_index = self.proxy_count + 1
             best_client_ip = ip_list[-best_client_ip_index]
             return best_client_ip, True
 
-        # we don't track proxy related info, so we just return the first ip
         return ip_list[0], False
```

### Comparing `python_ipware-2.0.4/python_ipware.egg-info/PKG-INFO` & `python_ipware-2.0.5/python_ipware.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ipware
-Version: 2.0.4
+Version: 2.0.5
 Summary: A Python package to retrieve user's IP address
 Author-email: Val Neekman <info@neekware.com>
 License: MIT
 Project-URL: Documentation, https://github.com/un33k/python-ipware#readme
 Project-URL: Issues, https://github.com/un33k/python-ipware/issues
 Project-URL: Source, https://github.com/un33k/python-ipware
 Project-URL: Changelog, https://github.com/un33k/python-ipware/blob/main/CHANGELOG.md
```

### Comparing `python_ipware-2.0.4/tests/tests_ipv4.py` & `python_ipware-2.0.5/tests/tests_ipv4.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,20 +73,35 @@
         self.assertEqual(r, (IPv4Address("177.139.233.138"), False))
 
     def test_error_only(self):
         meta = {
             "HTTP_X_FORWARDED_FOR": "unknown, 177.139.233.139, 198.84.193.157, 198.84.193.158",
         }
         r = self.ipware.get_client_ip(meta)
-        self.assertEqual(r, (None, False))
+        self.assertEqual(r, (IPv4Address("177.139.233.139"), False))
 
-    def test_error_first(self):
+    def test_error_only_strict(self):
         meta = {
             "HTTP_X_FORWARDED_FOR": "unknown, 177.139.233.139, 198.84.193.157, 198.84.193.158",
+        }
+        r = self.ipware.get_client_ip(meta, strict=True)
+        self.assertEqual(r, (None, False))
+
+    def test_error_only_first_strict(self):
+        meta = {
             "X_FORWARDED_FOR": "177.139.233.138, 198.84.193.157, 198.84.193.158",
+            "HTTP_X_FORWARDED_FOR": "unknown, 177.139.233.139, 198.84.193.157, 198.84.193.158",
+        }
+        r = self.ipware.get_client_ip(meta, strict=True)
+        self.assertEqual(r, (IPv4Address("177.139.233.138"), False))
+
+    def test_error_first(self):
+        meta = {
+            "X_FORWARDED_FOR": "unknown, 177.139.233.138, 198.84.193.157, 198.84.193.158",
+            "HTTP_X_FORWARDED_FOR": "177.139.233.139, 198.84.193.157, 198.84.193.158",
         }
         r = self.ipware.get_client_ip(meta)
         self.assertEqual(r, (IPv4Address("177.139.233.138"), False))
 
     def test_singleton(self):
         meta = {
             "HTTP_X_FORWARDED_FOR": "177.139.233.139",
@@ -218,23 +233,23 @@
 
     def test_proxy_count_zero_dont_care_proxy_pass(self):
         ipware = IpWare(proxy_count=0)
         meta = {
             "HTTP_X_FORWARDED_FOR": "177.139.233.139, 198.84.193.157, 198.84.193.158",
         }
         r = ipware.get_client_ip(meta)
-        self.assertEqual(r, (IPv4Address("177.139.233.139"), False))
+        self.assertEqual(r, (IPv4Address("198.84.193.158"), True))
 
     def test_proxy_count_zero_exact_zero_proxy_pass(self):
         ipware = IpWare(proxy_count=0)
         meta = {
             "HTTP_X_FORWARDED_FOR": "177.139.233.139",
         }
         r = ipware.get_client_ip(meta, strict=True)
-        self.assertEqual(r, (IPv4Address("177.139.233.139"), False))
+        self.assertEqual(r, (IPv4Address("177.139.233.139"), True))
 
     def test_proxy_count_zero_exact_zero_proxy_fail(self):
         ipware = IpWare(proxy_count=0)
         meta = {
             "HTTP_X_FORWARDED_FOR": "177.139.233.139, 198.84.193.157, 198.84.193.158",
         }
         r = ipware.get_client_ip(meta, strict=True)
```

### Comparing `python_ipware-2.0.4/tests/tests_ipv6.py` & `python_ipware-2.0.5/tests/tests_ipv6.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,22 +65,30 @@
         self.assertEqual(r, (IPv6Address("3ffe:1900:4545:3:200:f8ff:fe21:67cf"), False))
 
     def test_error_only(self):
         meta = {
             "X_FORWARDED_FOR": "unknown, 3ffe:1900:4545:3:200:f8ff:fe21:67cf, 2606:4700:4700::1111, 2001:4860:4860::8888",
         }
         r = self.ipware.get_client_ip(meta)
+        self.assertEqual(r, (IPv6Address("3ffe:1900:4545:3:200:f8ff:fe21:67cf"), False))
+
+    def test_error_only_strict(self):
+        meta = {
+            "X_FORWARDED_FOR": "unknown, 3ffe:1900:4545:3:200:f8ff:fe21:67cf, 2606:4700:4700::1111, 2001:4860:4860::8888",
+        }
+        r = self.ipware.get_client_ip(meta, strict=True)
         self.assertEqual(r, (None, False))
 
     def test_first_error_bailout(self):
         meta = {
             "HTTP_X_FORWARDED_FOR": "unknown, 3ffe:1900:4545:3:200:f8ff:fe21:67cf, 2606:4700:4700::1111, 2001:4860:4860::8888",
+            "X_FORWARDED_FOR": "2606:4700:4700::1111, 2001:4860:4860::8888",
         }
         r = self.ipware.get_client_ip(meta)
-        self.assertEqual(r, (None, False))
+        self.assertEqual(r, (IPv6Address("2606:4700:4700::1111"), False))
 
     def test_with_error_best_match(self):
         meta = {
             "HTTP_X_FORWARDED_FOR": "unknown, 3ffe:1900:4545:3:200:f8ff:fe21:67cf, 2606:4700:4700::1111, 2001:4860:4860::8888",
             "X_FORWARDED_FOR": "3ffe:1900:4545:3:200:f8ff:fe21:67cf, 2606:4700:4700::1111, 2001:4860:4860::8888",
         }
         r = self.ipware.get_client_ip(meta)
```

