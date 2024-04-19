# Comparing `tmp/bdkpython-1.0.0a7-cp39-cp39-win_amd64.whl.zip` & `tmp/bdkpython-1.0.0a9-cp38-cp38-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2609005 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       27 b- defN 24-Mar-26 22:06 bdkpython/__init__.py
--rw-rw-rw-  2.0 fat   193509 b- defN 24-Mar-26 22:09 bdkpython/bdk.py
--rw-rw-rw-  2.0 fat  4460544 b- defN 24-Mar-26 22:12 bdkpython/bdkffi.dll
--rw-rw-rw-  2.0 fat      483 b- defN 24-Mar-26 22:12 bdkpython-1.0.0a7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Mar-26 22:12 bdkpython-1.0.0a7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Mar-26 22:12 bdkpython-1.0.0a7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      545 b- defN 24-Mar-26 22:12 bdkpython-1.0.0a7.dist-info/RECORD
-7 files, 4655218 bytes uncompressed, 2608049 bytes compressed:  44.0%
+Zip file size: 2916290 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       27 b- defN 24-Apr-19 20:38 bdkpython/__init__.py
+-rw-r--r--  2.0 unx   237649 b- defN 24-Apr-19 20:39 bdkpython/bdk.py
+-rwxr-xr-x  2.0 unx  5831360 b- defN 24-Apr-19 20:41 bdkpython/libbdkffi.dylib
+-rw-r--r--  2.0 unx      522 b- defN 24-Apr-19 20:41 bdkpython-1.0.0a9.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 24-Apr-19 20:41 bdkpython-1.0.0a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-19 20:41 bdkpython-1.0.0a9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      550 b- defN 24-Apr-19 20:41 bdkpython-1.0.0a9.dist-info/RECORD
+7 files, 6070226 bytes uncompressed, 2915324 bytes compressed:  52.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: bdkpython/__init__.py
 Comment: 
 
 Filename: bdkpython/bdk.py
 Comment: 
 
-Filename: bdkpython/bdkffi.dll
+Filename: bdkpython/libbdkffi.dylib
 Comment: 
 
-Filename: bdkpython-1.0.0a7.dist-info/METADATA
+Filename: bdkpython-1.0.0a9.dist-info/METADATA
 Comment: 
 
-Filename: bdkpython-1.0.0a7.dist-info/WHEEL
+Filename: bdkpython-1.0.0a9.dist-info/WHEEL
 Comment: 
 
-Filename: bdkpython-1.0.0a7.dist-info/top_level.txt
+Filename: bdkpython-1.0.0a9.dist-info/top_level.txt
 Comment: 
 
-Filename: bdkpython-1.0.0a7.dist-info/RECORD
+Filename: bdkpython-1.0.0a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bdkpython/bdk.py

```diff
@@ -488,15 +488,15 @@
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_bumpfeetxbuilder_allow_shrinking() != 57772:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_bumpfeetxbuilder_enable_rbf() != 30060:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_bumpfeetxbuilder_enable_rbf_with_sequence() != 3682:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_bumpfeetxbuilder_finish() != 1377:
+    if lib.uniffi_bdkffi_checksum_method_bumpfeetxbuilder_finish() != 43492:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_descriptor_as_string() != 23756:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_descriptor_as_string_private() != 64930:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_descriptorpublickey_as_string() != 37256:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
@@ -510,37 +510,41 @@
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_descriptorsecretkey_derive() != 48028:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_descriptorsecretkey_extend() != 7383:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_descriptorsecretkey_secret_bytes() != 40876:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_esploraclient_broadcast() != 15506:
+    if lib.uniffi_bdkffi_checksum_method_esploraclient_broadcast() != 21200:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_esploraclient_full_scan() != 17276:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_feerate_as_sat_per_vb() != 60213:
+    if lib.uniffi_bdkffi_checksum_method_feerate_to_sat_per_kwu() != 2433:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_feerate_sat_per_kwu() != 7799:
+    if lib.uniffi_bdkffi_checksum_method_feerate_to_sat_per_vb_ceil() != 21019:
+        raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
+    if lib.uniffi_bdkffi_checksum_method_feerate_to_sat_per_vb_floor() != 54438:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_mnemonic_as_string() != 3181:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_partiallysignedtransaction_extract_tx() != 10768:
+    if lib.uniffi_bdkffi_checksum_method_psbt_extract_tx() != 60519:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_partiallysignedtransaction_serialize() != 39126:
+    if lib.uniffi_bdkffi_checksum_method_psbt_serialize() != 33309:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_script_to_bytes() != 31368:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_transaction_is_coin_base() != 42930:
+    if lib.uniffi_bdkffi_checksum_method_transaction_is_coinbase() != 14454:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_transaction_is_explicitly_rbf() != 32682:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_transaction_is_lock_time_enabled() != 48885:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_transaction_size() != 63453:
+    if lib.uniffi_bdkffi_checksum_method_transaction_serialize() != 62862:
+        raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
+    if lib.uniffi_bdkffi_checksum_method_transaction_total_size() != 12759:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_transaction_txid() != 29904:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_transaction_version() != 15271:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_transaction_vsize() != 3804:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
@@ -562,15 +566,15 @@
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_txbuilder_enable_rbf_with_sequence() != 26979:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_txbuilder_fee_absolute() != 59649:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_txbuilder_fee_rate() != 60371:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_txbuilder_finish() != 46844:
+    if lib.uniffi_bdkffi_checksum_method_txbuilder_finish() != 40018:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_txbuilder_manually_selected_only() != 12623:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_txbuilder_only_spend_change() != 18757:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_txbuilder_set_recipients() != 20461:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
@@ -582,33 +586,39 @@
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_wallet_calculate_fee_rate() != 61555:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_wallet_get_address() != 16446:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_wallet_get_balance() != 41846:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
+    if lib.uniffi_bdkffi_checksum_method_wallet_get_tx() != 59450:
+        raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_wallet_is_mine() != 10423:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
+    if lib.uniffi_bdkffi_checksum_method_wallet_list_output() != 27359:
+        raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
+    if lib.uniffi_bdkffi_checksum_method_wallet_list_unspent() != 25643:
+        raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_wallet_network() != 32197:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_method_wallet_sent_and_received() != 15077:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_wallet_sign() != 50512:
+    if lib.uniffi_bdkffi_checksum_method_wallet_sign() != 17213:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_wallet_transactions() != 16490:
+    if lib.uniffi_bdkffi_checksum_method_wallet_transactions() != 37950:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_method_wallet_try_get_internal_address() != 3117:
+    if lib.uniffi_bdkffi_checksum_method_wallet_try_get_internal_address() != 5184:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_constructor_address_new() != 21417:
+    if lib.uniffi_bdkffi_checksum_constructor_address_new() != 45929:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_constructor_bumpfeetxbuilder_new() != 47086:
+    if lib.uniffi_bdkffi_checksum_constructor_bumpfeetxbuilder_new() != 4758:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_derivationpath_new() != 4674:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_constructor_descriptor_new() != 57251:
+    if lib.uniffi_bdkffi_checksum_constructor_descriptor_new() != 56307:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_descriptor_new_bip44() != 46337:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_descriptor_new_bip44_public() != 54845:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_descriptor_new_bip49() != 56932:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
@@ -626,29 +636,29 @@
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_descriptorsecretkey_from_string() != 50158:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_descriptorsecretkey_new() != 47131:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_esploraclient_new() != 45557:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_constructor_feerate_from_sat_per_kwu() != 29960:
+    if lib.uniffi_bdkffi_checksum_constructor_feerate_from_sat_per_kwu() != 60699:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_constructor_feerate_from_sat_per_vb() != 9910:
+    if lib.uniffi_bdkffi_checksum_constructor_feerate_from_sat_per_vb() != 50427:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_mnemonic_from_entropy() != 11964:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_mnemonic_from_string() != 45294:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_mnemonic_new() != 26468:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_constructor_partiallysignedtransaction_new() != 32051:
+    if lib.uniffi_bdkffi_checksum_constructor_psbt_new() != 58680:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_script_new() != 36370:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
-    if lib.uniffi_bdkffi_checksum_constructor_transaction_new() != 25307:
+    if lib.uniffi_bdkffi_checksum_constructor_transaction_new() != 45575:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_txbuilder_new() != 978:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
     if lib.uniffi_bdkffi_checksum_constructor_wallet_new() != 64341:
         raise InternalError("UniFFI API checksum mismatch: try cleaning and rebuilding your project")
 
 # A ctypes library to expose the extern-C FFI definitions.
@@ -705,15 +715,15 @@
 _UniffiLib.uniffi_bdkffi_fn_free_bumpfeetxbuilder.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_free_bumpfeetxbuilder.restype = None
 _UniffiLib.uniffi_bdkffi_fn_constructor_bumpfeetxbuilder_new.argtypes = (
     _UniffiRustBuffer,
-    ctypes.c_float,
+    ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_constructor_bumpfeetxbuilder_new.restype = ctypes.c_void_p
 _UniffiLib.uniffi_bdkffi_fn_method_bumpfeetxbuilder_allow_shrinking.argtypes = (
     ctypes.c_void_p,
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
@@ -954,33 +964,38 @@
 _UniffiLib.uniffi_bdkffi_fn_clone_feerate.restype = ctypes.c_void_p
 _UniffiLib.uniffi_bdkffi_fn_free_feerate.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_free_feerate.restype = None
 _UniffiLib.uniffi_bdkffi_fn_constructor_feerate_from_sat_per_kwu.argtypes = (
-    ctypes.c_float,
+    ctypes.c_uint64,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_constructor_feerate_from_sat_per_kwu.restype = ctypes.c_void_p
 _UniffiLib.uniffi_bdkffi_fn_constructor_feerate_from_sat_per_vb.argtypes = (
-    ctypes.c_float,
+    ctypes.c_uint64,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_constructor_feerate_from_sat_per_vb.restype = ctypes.c_void_p
-_UniffiLib.uniffi_bdkffi_fn_method_feerate_as_sat_per_vb.argtypes = (
+_UniffiLib.uniffi_bdkffi_fn_method_feerate_to_sat_per_kwu.argtypes = (
+    ctypes.c_void_p,
+    ctypes.POINTER(_UniffiRustCallStatus),
+)
+_UniffiLib.uniffi_bdkffi_fn_method_feerate_to_sat_per_kwu.restype = ctypes.c_uint64
+_UniffiLib.uniffi_bdkffi_fn_method_feerate_to_sat_per_vb_ceil.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
-_UniffiLib.uniffi_bdkffi_fn_method_feerate_as_sat_per_vb.restype = ctypes.c_float
-_UniffiLib.uniffi_bdkffi_fn_method_feerate_sat_per_kwu.argtypes = (
+_UniffiLib.uniffi_bdkffi_fn_method_feerate_to_sat_per_vb_ceil.restype = ctypes.c_uint64
+_UniffiLib.uniffi_bdkffi_fn_method_feerate_to_sat_per_vb_floor.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
-_UniffiLib.uniffi_bdkffi_fn_method_feerate_sat_per_kwu.restype = ctypes.c_float
+_UniffiLib.uniffi_bdkffi_fn_method_feerate_to_sat_per_vb_floor.restype = ctypes.c_uint64
 _UniffiLib.uniffi_bdkffi_fn_clone_mnemonic.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_clone_mnemonic.restype = ctypes.c_void_p
 _UniffiLib.uniffi_bdkffi_fn_free_mnemonic.argtypes = (
     ctypes.c_void_p,
@@ -1003,39 +1018,39 @@
 )
 _UniffiLib.uniffi_bdkffi_fn_constructor_mnemonic_new.restype = ctypes.c_void_p
 _UniffiLib.uniffi_bdkffi_fn_method_mnemonic_as_string.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_method_mnemonic_as_string.restype = _UniffiRustBuffer
-_UniffiLib.uniffi_bdkffi_fn_clone_partiallysignedtransaction.argtypes = (
+_UniffiLib.uniffi_bdkffi_fn_clone_psbt.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
-_UniffiLib.uniffi_bdkffi_fn_clone_partiallysignedtransaction.restype = ctypes.c_void_p
-_UniffiLib.uniffi_bdkffi_fn_free_partiallysignedtransaction.argtypes = (
+_UniffiLib.uniffi_bdkffi_fn_clone_psbt.restype = ctypes.c_void_p
+_UniffiLib.uniffi_bdkffi_fn_free_psbt.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
-_UniffiLib.uniffi_bdkffi_fn_free_partiallysignedtransaction.restype = None
-_UniffiLib.uniffi_bdkffi_fn_constructor_partiallysignedtransaction_new.argtypes = (
+_UniffiLib.uniffi_bdkffi_fn_free_psbt.restype = None
+_UniffiLib.uniffi_bdkffi_fn_constructor_psbt_new.argtypes = (
     _UniffiRustBuffer,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
-_UniffiLib.uniffi_bdkffi_fn_constructor_partiallysignedtransaction_new.restype = ctypes.c_void_p
-_UniffiLib.uniffi_bdkffi_fn_method_partiallysignedtransaction_extract_tx.argtypes = (
+_UniffiLib.uniffi_bdkffi_fn_constructor_psbt_new.restype = ctypes.c_void_p
+_UniffiLib.uniffi_bdkffi_fn_method_psbt_extract_tx.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
-_UniffiLib.uniffi_bdkffi_fn_method_partiallysignedtransaction_extract_tx.restype = ctypes.c_void_p
-_UniffiLib.uniffi_bdkffi_fn_method_partiallysignedtransaction_serialize.argtypes = (
+_UniffiLib.uniffi_bdkffi_fn_method_psbt_extract_tx.restype = ctypes.c_void_p
+_UniffiLib.uniffi_bdkffi_fn_method_psbt_serialize.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
-_UniffiLib.uniffi_bdkffi_fn_method_partiallysignedtransaction_serialize.restype = _UniffiRustBuffer
+_UniffiLib.uniffi_bdkffi_fn_method_psbt_serialize.restype = _UniffiRustBuffer
 _UniffiLib.uniffi_bdkffi_fn_clone_script.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_clone_script.restype = ctypes.c_void_p
 _UniffiLib.uniffi_bdkffi_fn_free_script.argtypes = (
     ctypes.c_void_p,
@@ -1063,34 +1078,39 @@
 )
 _UniffiLib.uniffi_bdkffi_fn_free_transaction.restype = None
 _UniffiLib.uniffi_bdkffi_fn_constructor_transaction_new.argtypes = (
     _UniffiRustBuffer,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_constructor_transaction_new.restype = ctypes.c_void_p
-_UniffiLib.uniffi_bdkffi_fn_method_transaction_is_coin_base.argtypes = (
+_UniffiLib.uniffi_bdkffi_fn_method_transaction_is_coinbase.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
-_UniffiLib.uniffi_bdkffi_fn_method_transaction_is_coin_base.restype = ctypes.c_int8
+_UniffiLib.uniffi_bdkffi_fn_method_transaction_is_coinbase.restype = ctypes.c_int8
 _UniffiLib.uniffi_bdkffi_fn_method_transaction_is_explicitly_rbf.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_method_transaction_is_explicitly_rbf.restype = ctypes.c_int8
 _UniffiLib.uniffi_bdkffi_fn_method_transaction_is_lock_time_enabled.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_method_transaction_is_lock_time_enabled.restype = ctypes.c_int8
-_UniffiLib.uniffi_bdkffi_fn_method_transaction_size.argtypes = (
+_UniffiLib.uniffi_bdkffi_fn_method_transaction_serialize.argtypes = (
+    ctypes.c_void_p,
+    ctypes.POINTER(_UniffiRustCallStatus),
+)
+_UniffiLib.uniffi_bdkffi_fn_method_transaction_serialize.restype = _UniffiRustBuffer
+_UniffiLib.uniffi_bdkffi_fn_method_transaction_total_size.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
-_UniffiLib.uniffi_bdkffi_fn_method_transaction_size.restype = ctypes.c_uint64
+_UniffiLib.uniffi_bdkffi_fn_method_transaction_total_size.restype = ctypes.c_uint64
 _UniffiLib.uniffi_bdkffi_fn_method_transaction_txid.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_method_transaction_txid.restype = _UniffiRustBuffer
 _UniffiLib.uniffi_bdkffi_fn_method_transaction_version.argtypes = (
     ctypes.c_void_p,
@@ -1261,20 +1281,36 @@
 )
 _UniffiLib.uniffi_bdkffi_fn_method_wallet_get_address.restype = _UniffiRustBuffer
 _UniffiLib.uniffi_bdkffi_fn_method_wallet_get_balance.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_method_wallet_get_balance.restype = _UniffiRustBuffer
+_UniffiLib.uniffi_bdkffi_fn_method_wallet_get_tx.argtypes = (
+    ctypes.c_void_p,
+    _UniffiRustBuffer,
+    ctypes.POINTER(_UniffiRustCallStatus),
+)
+_UniffiLib.uniffi_bdkffi_fn_method_wallet_get_tx.restype = _UniffiRustBuffer
 _UniffiLib.uniffi_bdkffi_fn_method_wallet_is_mine.argtypes = (
     ctypes.c_void_p,
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_method_wallet_is_mine.restype = ctypes.c_int8
+_UniffiLib.uniffi_bdkffi_fn_method_wallet_list_output.argtypes = (
+    ctypes.c_void_p,
+    ctypes.POINTER(_UniffiRustCallStatus),
+)
+_UniffiLib.uniffi_bdkffi_fn_method_wallet_list_output.restype = _UniffiRustBuffer
+_UniffiLib.uniffi_bdkffi_fn_method_wallet_list_unspent.argtypes = (
+    ctypes.c_void_p,
+    ctypes.POINTER(_UniffiRustCallStatus),
+)
+_UniffiLib.uniffi_bdkffi_fn_method_wallet_list_unspent.restype = _UniffiRustBuffer
 _UniffiLib.uniffi_bdkffi_fn_method_wallet_network.argtypes = (
     ctypes.c_void_p,
     ctypes.POINTER(_UniffiRustCallStatus),
 )
 _UniffiLib.uniffi_bdkffi_fn_method_wallet_network.restype = _UniffiRustBuffer
 _UniffiLib.uniffi_bdkffi_fn_method_wallet_sent_and_received.argtypes = (
     ctypes.c_void_p,
@@ -1626,44 +1662,50 @@
 _UniffiLib.uniffi_bdkffi_checksum_method_descriptorsecretkey_secret_bytes.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_esploraclient_broadcast.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_esploraclient_broadcast.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_esploraclient_full_scan.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_esploraclient_full_scan.restype = ctypes.c_uint16
-_UniffiLib.uniffi_bdkffi_checksum_method_feerate_as_sat_per_vb.argtypes = (
+_UniffiLib.uniffi_bdkffi_checksum_method_feerate_to_sat_per_kwu.argtypes = (
 )
-_UniffiLib.uniffi_bdkffi_checksum_method_feerate_as_sat_per_vb.restype = ctypes.c_uint16
-_UniffiLib.uniffi_bdkffi_checksum_method_feerate_sat_per_kwu.argtypes = (
+_UniffiLib.uniffi_bdkffi_checksum_method_feerate_to_sat_per_kwu.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_feerate_to_sat_per_vb_ceil.argtypes = (
 )
-_UniffiLib.uniffi_bdkffi_checksum_method_feerate_sat_per_kwu.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_feerate_to_sat_per_vb_ceil.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_feerate_to_sat_per_vb_floor.argtypes = (
+)
+_UniffiLib.uniffi_bdkffi_checksum_method_feerate_to_sat_per_vb_floor.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_mnemonic_as_string.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_mnemonic_as_string.restype = ctypes.c_uint16
-_UniffiLib.uniffi_bdkffi_checksum_method_partiallysignedtransaction_extract_tx.argtypes = (
+_UniffiLib.uniffi_bdkffi_checksum_method_psbt_extract_tx.argtypes = (
 )
-_UniffiLib.uniffi_bdkffi_checksum_method_partiallysignedtransaction_extract_tx.restype = ctypes.c_uint16
-_UniffiLib.uniffi_bdkffi_checksum_method_partiallysignedtransaction_serialize.argtypes = (
+_UniffiLib.uniffi_bdkffi_checksum_method_psbt_extract_tx.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_psbt_serialize.argtypes = (
 )
-_UniffiLib.uniffi_bdkffi_checksum_method_partiallysignedtransaction_serialize.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_psbt_serialize.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_script_to_bytes.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_script_to_bytes.restype = ctypes.c_uint16
-_UniffiLib.uniffi_bdkffi_checksum_method_transaction_is_coin_base.argtypes = (
+_UniffiLib.uniffi_bdkffi_checksum_method_transaction_is_coinbase.argtypes = (
 )
-_UniffiLib.uniffi_bdkffi_checksum_method_transaction_is_coin_base.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_transaction_is_coinbase.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_transaction_is_explicitly_rbf.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_transaction_is_explicitly_rbf.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_transaction_is_lock_time_enabled.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_transaction_is_lock_time_enabled.restype = ctypes.c_uint16
-_UniffiLib.uniffi_bdkffi_checksum_method_transaction_size.argtypes = (
+_UniffiLib.uniffi_bdkffi_checksum_method_transaction_serialize.argtypes = (
+)
+_UniffiLib.uniffi_bdkffi_checksum_method_transaction_serialize.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_transaction_total_size.argtypes = (
 )
-_UniffiLib.uniffi_bdkffi_checksum_method_transaction_size.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_transaction_total_size.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_transaction_txid.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_transaction_txid.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_transaction_version.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_transaction_version.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_transaction_vsize.argtypes = (
@@ -1728,17 +1770,26 @@
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_calculate_fee_rate.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_get_address.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_get_address.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_get_balance.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_get_balance.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_wallet_get_tx.argtypes = (
+)
+_UniffiLib.uniffi_bdkffi_checksum_method_wallet_get_tx.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_is_mine.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_is_mine.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_wallet_list_output.argtypes = (
+)
+_UniffiLib.uniffi_bdkffi_checksum_method_wallet_list_output.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_method_wallet_list_unspent.argtypes = (
+)
+_UniffiLib.uniffi_bdkffi_checksum_method_wallet_list_unspent.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_network.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_network.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_sent_and_received.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_sent_and_received.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_method_wallet_sign.argtypes = (
@@ -1809,17 +1860,17 @@
 _UniffiLib.uniffi_bdkffi_checksum_constructor_mnemonic_from_entropy.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_constructor_mnemonic_from_string.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_constructor_mnemonic_from_string.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_constructor_mnemonic_new.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_constructor_mnemonic_new.restype = ctypes.c_uint16
-_UniffiLib.uniffi_bdkffi_checksum_constructor_partiallysignedtransaction_new.argtypes = (
+_UniffiLib.uniffi_bdkffi_checksum_constructor_psbt_new.argtypes = (
 )
-_UniffiLib.uniffi_bdkffi_checksum_constructor_partiallysignedtransaction_new.restype = ctypes.c_uint16
+_UniffiLib.uniffi_bdkffi_checksum_constructor_psbt_new.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_constructor_script_new.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_constructor_script_new.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_constructor_transaction_new.argtypes = (
 )
 _UniffiLib.uniffi_bdkffi_checksum_constructor_transaction_new.restype = ctypes.c_uint16
 _UniffiLib.uniffi_bdkffi_checksum_constructor_txbuilder_new.argtypes = (
@@ -1913,23 +1964,14 @@
     def read(buf):
         return buf.read_i64()
 
     @staticmethod
     def write(value, buf):
         buf.write_i64(value)
 
-class _UniffiConverterFloat(_UniffiConverterPrimitiveFloat):
-    @staticmethod
-    def read(buf):
-        return buf.read_float()
-
-    @staticmethod
-    def write(value, buf):
-        buf.write_float(value)
-
 class _UniffiConverterBool:
     @classmethod
     def check_lower(cls, value):
         return not not value
 
     @classmethod
     def lower(cls, value):
@@ -1997,15 +2039,15 @@
 
     _pointer: ctypes.c_void_p
     def __init__(self, address: "str",network: "Network"):
         _UniffiConverterString.check_lower(address)
         
         _UniffiConverterTypeNetwork.check_lower(network)
         
-        self._pointer = _rust_call_with_error(_UniffiConverterTypeAlpha3Error,_UniffiLib.uniffi_bdkffi_fn_constructor_address_new,
+        self._pointer = _rust_call_with_error(_UniffiConverterTypeAddressError,_UniffiLib.uniffi_bdkffi_fn_constructor_address_new,
         _UniffiConverterString.lower(address),
         _UniffiConverterTypeNetwork.lower(network))
 
     def __del__(self):
         # In case of partial initialization of instances.
         pointer = getattr(self, "_pointer", None)
         if pointer is not None:
@@ -2115,22 +2157,22 @@
         raise NotImplementedError
     def finish(self, wallet: "Wallet"):
         raise NotImplementedError
 
 class BumpFeeTxBuilder:
 
     _pointer: ctypes.c_void_p
-    def __init__(self, txid: "str",fee_rate: "float"):
+    def __init__(self, txid: "str",fee_rate: "FeeRate"):
         _UniffiConverterString.check_lower(txid)
         
-        _UniffiConverterFloat.check_lower(fee_rate)
+        _UniffiConverterTypeFeeRate.check_lower(fee_rate)
         
         self._pointer = _rust_call(_UniffiLib.uniffi_bdkffi_fn_constructor_bumpfeetxbuilder_new,
         _UniffiConverterString.lower(txid),
-        _UniffiConverterFloat.lower(fee_rate))
+        _UniffiConverterTypeFeeRate.lower(fee_rate))
 
     def __del__(self):
         # In case of partial initialization of instances.
         pointer = getattr(self, "_pointer", None)
         if pointer is not None:
             _rust_call(_UniffiLib.uniffi_bdkffi_fn_free_bumpfeetxbuilder, pointer)
 
@@ -2179,18 +2221,18 @@
         )
 
 
 
 
 
 
-    def finish(self, wallet: "Wallet") -> "PartiallySignedTransaction":
+    def finish(self, wallet: "Wallet") -> "Psbt":
         _UniffiConverterTypeWallet.check_lower(wallet)
         
-        return _UniffiConverterTypePartiallySignedTransaction.lift(
+        return _UniffiConverterTypePsbt.lift(
             _rust_call_with_error(
     _UniffiConverterTypeAlpha3Error,_UniffiLib.uniffi_bdkffi_fn_method_bumpfeetxbuilder_finish,self._uniffi_clone_pointer(),
         _UniffiConverterTypeWallet.lower(wallet))
         )
 
 
 
@@ -2296,15 +2338,15 @@
 
     _pointer: ctypes.c_void_p
     def __init__(self, descriptor: "str",network: "Network"):
         _UniffiConverterString.check_lower(descriptor)
         
         _UniffiConverterTypeNetwork.check_lower(network)
         
-        self._pointer = _rust_call_with_error(_UniffiConverterTypeAlpha3Error,_UniffiLib.uniffi_bdkffi_fn_constructor_descriptor_new,
+        self._pointer = _rust_call_with_error(_UniffiConverterTypeDescriptorError,_UniffiLib.uniffi_bdkffi_fn_constructor_descriptor_new,
         _UniffiConverterString.lower(descriptor),
         _UniffiConverterTypeNetwork.lower(network))
 
     def __del__(self):
         # In case of partial initialization of instances.
         pointer = getattr(self, "_pointer", None)
         if pointer is not None:
@@ -2797,15 +2839,15 @@
         return inst
 
 
     def broadcast(self, transaction: "Transaction"):
         _UniffiConverterTypeTransaction.check_lower(transaction)
         
         _rust_call_with_error(
-    _UniffiConverterTypeAlpha3Error,_UniffiLib.uniffi_bdkffi_fn_method_esploraclient_broadcast,self._uniffi_clone_pointer(),
+    _UniffiConverterTypeEsploraError,_UniffiLib.uniffi_bdkffi_fn_method_esploraclient_broadcast,self._uniffi_clone_pointer(),
         _UniffiConverterTypeTransaction.lower(transaction))
 
 
 
 
 
 
@@ -2856,17 +2898,19 @@
     @classmethod
     def write(cls, value: EsploraClientProtocol, buf: _UniffiRustBuffer):
         buf.write_u64(cls.lower(value))
 
 
 
 class FeeRateProtocol(typing.Protocol):
-    def as_sat_per_vb(self, ):
+    def to_sat_per_kwu(self, ):
         raise NotImplementedError
-    def sat_per_kwu(self, ):
+    def to_sat_per_vb_ceil(self, ):
+        raise NotImplementedError
+    def to_sat_per_vb_floor(self, ):
         raise NotImplementedError
 
 class FeeRate:
 
     _pointer: ctypes.c_void_p
 
     def __del__(self):
@@ -2884,47 +2928,57 @@
         # Lightly yucky way to bypass the usual __init__ logic
         # and just create a new instance with the required pointer.
         inst = cls.__new__(cls)
         inst._pointer = pointer
         return inst
 
     @classmethod
-    def from_sat_per_kwu(cls, sat_per_kwu: "float"):
-        _UniffiConverterFloat.check_lower(sat_per_kwu)
+    def from_sat_per_kwu(cls, sat_per_kwu: "int"):
+        _UniffiConverterUInt64.check_lower(sat_per_kwu)
         
         # Call the (fallible) function before creating any half-baked object instances.
         pointer = _rust_call(_UniffiLib.uniffi_bdkffi_fn_constructor_feerate_from_sat_per_kwu,
-        _UniffiConverterFloat.lower(sat_per_kwu))
+        _UniffiConverterUInt64.lower(sat_per_kwu))
         return cls._make_instance_(pointer)
 
 
     @classmethod
-    def from_sat_per_vb(cls, sat_per_vb: "float"):
-        _UniffiConverterFloat.check_lower(sat_per_vb)
+    def from_sat_per_vb(cls, sat_per_vb: "int"):
+        _UniffiConverterUInt64.check_lower(sat_per_vb)
         
         # Call the (fallible) function before creating any half-baked object instances.
-        pointer = _rust_call(_UniffiLib.uniffi_bdkffi_fn_constructor_feerate_from_sat_per_vb,
-        _UniffiConverterFloat.lower(sat_per_vb))
+        pointer = _rust_call_with_error(_UniffiConverterTypeFeeRateError,_UniffiLib.uniffi_bdkffi_fn_constructor_feerate_from_sat_per_vb,
+        _UniffiConverterUInt64.lower(sat_per_vb))
         return cls._make_instance_(pointer)
 
 
 
-    def as_sat_per_vb(self, ) -> "float":
-        return _UniffiConverterFloat.lift(
-            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_feerate_as_sat_per_vb,self._uniffi_clone_pointer(),)
+    def to_sat_per_kwu(self, ) -> "int":
+        return _UniffiConverterUInt64.lift(
+            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_feerate_to_sat_per_kwu,self._uniffi_clone_pointer(),)
+        )
+
+
+
+
+
+
+    def to_sat_per_vb_ceil(self, ) -> "int":
+        return _UniffiConverterUInt64.lift(
+            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_feerate_to_sat_per_vb_ceil,self._uniffi_clone_pointer(),)
         )
 
 
 
 
 
 
-    def sat_per_kwu(self, ) -> "float":
-        return _UniffiConverterFloat.lift(
-            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_feerate_sat_per_kwu,self._uniffi_clone_pointer(),)
+    def to_sat_per_vb_floor(self, ) -> "int":
+        return _UniffiConverterUInt64.lift(
+            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_feerate_to_sat_per_vb_floor,self._uniffi_clone_pointer(),)
         )
 
 
 
 
 
 class _UniffiConverterTypeFeeRate:
@@ -3044,93 +3098,94 @@
 
     @classmethod
     def write(cls, value: MnemonicProtocol, buf: _UniffiRustBuffer):
         buf.write_u64(cls.lower(value))
 
 
 
-class PartiallySignedTransactionProtocol(typing.Protocol):
+class PsbtProtocol(typing.Protocol):
     def extract_tx(self, ):
         raise NotImplementedError
     def serialize(self, ):
         raise NotImplementedError
 
-class PartiallySignedTransaction:
+class Psbt:
 
     _pointer: ctypes.c_void_p
     def __init__(self, psbt_base64: "str"):
         _UniffiConverterString.check_lower(psbt_base64)
         
-        self._pointer = _rust_call_with_error(_UniffiConverterTypeAlpha3Error,_UniffiLib.uniffi_bdkffi_fn_constructor_partiallysignedtransaction_new,
+        self._pointer = _rust_call_with_error(_UniffiConverterTypePsbtParseError,_UniffiLib.uniffi_bdkffi_fn_constructor_psbt_new,
         _UniffiConverterString.lower(psbt_base64))
 
     def __del__(self):
         # In case of partial initialization of instances.
         pointer = getattr(self, "_pointer", None)
         if pointer is not None:
-            _rust_call(_UniffiLib.uniffi_bdkffi_fn_free_partiallysignedtransaction, pointer)
+            _rust_call(_UniffiLib.uniffi_bdkffi_fn_free_psbt, pointer)
 
     def _uniffi_clone_pointer(self):
-        return _rust_call(_UniffiLib.uniffi_bdkffi_fn_clone_partiallysignedtransaction, self._pointer)
+        return _rust_call(_UniffiLib.uniffi_bdkffi_fn_clone_psbt, self._pointer)
 
     # Used by alternative constructors or any methods which return this type.
     @classmethod
     def _make_instance_(cls, pointer):
         # Lightly yucky way to bypass the usual __init__ logic
         # and just create a new instance with the required pointer.
         inst = cls.__new__(cls)
         inst._pointer = pointer
         return inst
 
 
     def extract_tx(self, ) -> "Transaction":
         return _UniffiConverterTypeTransaction.lift(
-            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_partiallysignedtransaction_extract_tx,self._uniffi_clone_pointer(),)
+            _rust_call_with_error(
+    _UniffiConverterTypeExtractTxError,_UniffiLib.uniffi_bdkffi_fn_method_psbt_extract_tx,self._uniffi_clone_pointer(),)
         )
 
 
 
 
 
 
     def serialize(self, ) -> "str":
         return _UniffiConverterString.lift(
-            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_partiallysignedtransaction_serialize,self._uniffi_clone_pointer(),)
+            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_psbt_serialize,self._uniffi_clone_pointer(),)
         )
 
 
 
 
 
-class _UniffiConverterTypePartiallySignedTransaction:
+class _UniffiConverterTypePsbt:
 
     @staticmethod
     def lift(value: int):
-        return PartiallySignedTransaction._make_instance_(value)
+        return Psbt._make_instance_(value)
 
     @staticmethod
-    def check_lower(value: PartiallySignedTransaction):
-        if not isinstance(value, PartiallySignedTransaction):
-            raise TypeError("Expected PartiallySignedTransaction instance, {} found".format(type(value).__name__))
+    def check_lower(value: Psbt):
+        if not isinstance(value, Psbt):
+            raise TypeError("Expected Psbt instance, {} found".format(type(value).__name__))
 
     @staticmethod
-    def lower(value: PartiallySignedTransactionProtocol):
-        if not isinstance(value, PartiallySignedTransaction):
-            raise TypeError("Expected PartiallySignedTransaction instance, {} found".format(type(value).__name__))
+    def lower(value: PsbtProtocol):
+        if not isinstance(value, Psbt):
+            raise TypeError("Expected Psbt instance, {} found".format(type(value).__name__))
         return value._uniffi_clone_pointer()
 
     @classmethod
     def read(cls, buf: _UniffiRustBuffer):
         ptr = buf.read_u64()
         if ptr == 0:
             raise InternalError("Raw pointer value was null")
         return cls.lift(ptr)
 
     @classmethod
-    def write(cls, value: PartiallySignedTransactionProtocol, buf: _UniffiRustBuffer):
+    def write(cls, value: PsbtProtocol, buf: _UniffiRustBuffer):
         buf.write_u64(cls.lower(value))
 
 
 
 class ScriptProtocol(typing.Protocol):
     def to_bytes(self, ):
         raise NotImplementedError
@@ -3199,36 +3254,38 @@
     @classmethod
     def write(cls, value: ScriptProtocol, buf: _UniffiRustBuffer):
         buf.write_u64(cls.lower(value))
 
 
 
 class TransactionProtocol(typing.Protocol):
-    def is_coin_base(self, ):
+    def is_coinbase(self, ):
         raise NotImplementedError
     def is_explicitly_rbf(self, ):
         raise NotImplementedError
     def is_lock_time_enabled(self, ):
         raise NotImplementedError
-    def size(self, ):
+    def serialize(self, ):
+        raise NotImplementedError
+    def total_size(self, ):
         raise NotImplementedError
     def txid(self, ):
         raise NotImplementedError
     def version(self, ):
         raise NotImplementedError
     def vsize(self, ):
         raise NotImplementedError
 
 class Transaction:
 
     _pointer: ctypes.c_void_p
     def __init__(self, transaction_bytes: "typing.List[int]"):
         _UniffiConverterSequenceUInt8.check_lower(transaction_bytes)
         
-        self._pointer = _rust_call_with_error(_UniffiConverterTypeAlpha3Error,_UniffiLib.uniffi_bdkffi_fn_constructor_transaction_new,
+        self._pointer = _rust_call_with_error(_UniffiConverterTypeTransactionError,_UniffiLib.uniffi_bdkffi_fn_constructor_transaction_new,
         _UniffiConverterSequenceUInt8.lower(transaction_bytes))
 
     def __del__(self):
         # In case of partial initialization of instances.
         pointer = getattr(self, "_pointer", None)
         if pointer is not None:
             _rust_call(_UniffiLib.uniffi_bdkffi_fn_free_transaction, pointer)
@@ -3242,17 +3299,17 @@
         # Lightly yucky way to bypass the usual __init__ logic
         # and just create a new instance with the required pointer.
         inst = cls.__new__(cls)
         inst._pointer = pointer
         return inst
 
 
-    def is_coin_base(self, ) -> "bool":
+    def is_coinbase(self, ) -> "bool":
         return _UniffiConverterBool.lift(
-            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_transaction_is_coin_base,self._uniffi_clone_pointer(),)
+            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_transaction_is_coinbase,self._uniffi_clone_pointer(),)
         )
 
 
 
 
 
 
@@ -3272,17 +3329,27 @@
         )
 
 
 
 
 
 
-    def size(self, ) -> "int":
+    def serialize(self, ) -> "typing.List[int]":
+        return _UniffiConverterSequenceUInt8.lift(
+            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_transaction_serialize,self._uniffi_clone_pointer(),)
+        )
+
+
+
+
+
+
+    def total_size(self, ) -> "int":
         return _UniffiConverterUInt64.lift(
-            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_transaction_size,self._uniffi_clone_pointer(),)
+            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_transaction_total_size,self._uniffi_clone_pointer(),)
         )
 
 
 
 
 
 
@@ -3537,18 +3604,18 @@
         )
 
 
 
 
 
 
-    def finish(self, wallet: "Wallet") -> "PartiallySignedTransaction":
+    def finish(self, wallet: "Wallet") -> "Psbt":
         _UniffiConverterTypeWallet.check_lower(wallet)
         
-        return _UniffiConverterTypePartiallySignedTransaction.lift(
+        return _UniffiConverterTypePsbt.lift(
             _rust_call_with_error(
     _UniffiConverterTypeAlpha3Error,_UniffiLib.uniffi_bdkffi_fn_method_txbuilder_finish,self._uniffi_clone_pointer(),
         _UniffiConverterTypeWallet.lower(wallet))
         )
 
 
 
@@ -3692,21 +3759,27 @@
         raise NotImplementedError
     def calculate_fee_rate(self, tx: "Transaction"):
         raise NotImplementedError
     def get_address(self, address_index: "AddressIndex"):
         raise NotImplementedError
     def get_balance(self, ):
         raise NotImplementedError
+    def get_tx(self, txid: "str"):
+        raise NotImplementedError
     def is_mine(self, script: "Script"):
         raise NotImplementedError
+    def list_output(self, ):
+        raise NotImplementedError
+    def list_unspent(self, ):
+        raise NotImplementedError
     def network(self, ):
         raise NotImplementedError
     def sent_and_received(self, tx: "Transaction"):
         raise NotImplementedError
-    def sign(self, psbt: "PartiallySignedTransaction"):
+    def sign(self, psbt: "Psbt"):
         raise NotImplementedError
     def transactions(self, ):
         raise NotImplementedError
     def try_get_internal_address(self, address_index: "AddressIndex"):
         raise NotImplementedError
 
 class Wallet:
@@ -3806,27 +3879,61 @@
         )
 
 
 
 
 
 
+    def get_tx(self, txid: "str") -> "typing.Optional[CanonicalTx]":
+        _UniffiConverterString.check_lower(txid)
+        
+        return _UniffiConverterOptionalTypeCanonicalTx.lift(
+            _rust_call_with_error(
+    _UniffiConverterTypeTxidParseError,_UniffiLib.uniffi_bdkffi_fn_method_wallet_get_tx,self._uniffi_clone_pointer(),
+        _UniffiConverterString.lower(txid))
+        )
+
+
+
+
+
+
     def is_mine(self, script: "Script") -> "bool":
         _UniffiConverterTypeScript.check_lower(script)
         
         return _UniffiConverterBool.lift(
             _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_wallet_is_mine,self._uniffi_clone_pointer(),
         _UniffiConverterTypeScript.lower(script))
         )
 
 
 
 
 
 
+    def list_output(self, ) -> "typing.List[LocalOutput]":
+        return _UniffiConverterSequenceTypeLocalOutput.lift(
+            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_wallet_list_output,self._uniffi_clone_pointer(),)
+        )
+
+
+
+
+
+
+    def list_unspent(self, ) -> "typing.List[LocalOutput]":
+        return _UniffiConverterSequenceTypeLocalOutput.lift(
+            _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_wallet_list_unspent,self._uniffi_clone_pointer(),)
+        )
+
+
+
+
+
+
     def network(self, ) -> "Network":
         return _UniffiConverterTypeNetwork.lift(
             _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_wallet_network,self._uniffi_clone_pointer(),)
         )
 
 
 
@@ -3842,44 +3949,44 @@
         )
 
 
 
 
 
 
-    def sign(self, psbt: "PartiallySignedTransaction") -> "bool":
-        _UniffiConverterTypePartiallySignedTransaction.check_lower(psbt)
+    def sign(self, psbt: "Psbt") -> "bool":
+        _UniffiConverterTypePsbt.check_lower(psbt)
         
         return _UniffiConverterBool.lift(
             _rust_call_with_error(
     _UniffiConverterTypeAlpha3Error,_UniffiLib.uniffi_bdkffi_fn_method_wallet_sign,self._uniffi_clone_pointer(),
-        _UniffiConverterTypePartiallySignedTransaction.lower(psbt))
+        _UniffiConverterTypePsbt.lower(psbt))
         )
 
 
 
 
 
 
-    def transactions(self, ) -> "typing.List[Transaction]":
-        return _UniffiConverterSequenceTypeTransaction.lift(
+    def transactions(self, ) -> "typing.List[CanonicalTx]":
+        return _UniffiConverterSequenceTypeCanonicalTx.lift(
             _rust_call(_UniffiLib.uniffi_bdkffi_fn_method_wallet_transactions,self._uniffi_clone_pointer(),)
         )
 
 
 
 
 
 
     def try_get_internal_address(self, address_index: "AddressIndex") -> "AddressInfo":
         _UniffiConverterTypeAddressIndex.check_lower(address_index)
         
         return _UniffiConverterTypeAddressInfo.lift(
             _rust_call_with_error(
-    _UniffiConverterTypeAlpha3Error,_UniffiLib.uniffi_bdkffi_fn_method_wallet_try_get_internal_address,self._uniffi_clone_pointer(),
+    _UniffiConverterTypePersistenceError,_UniffiLib.uniffi_bdkffi_fn_method_wallet_try_get_internal_address,self._uniffi_clone_pointer(),
         _UniffiConverterTypeAddressIndex.lower(address_index))
         )
 
 
 
 
 
@@ -4017,14 +4124,51 @@
         _UniffiConverterUInt64.write(value.trusted_pending, buf)
         _UniffiConverterUInt64.write(value.untrusted_pending, buf)
         _UniffiConverterUInt64.write(value.confirmed, buf)
         _UniffiConverterUInt64.write(value.trusted_spendable, buf)
         _UniffiConverterUInt64.write(value.total, buf)
 
 
+class CanonicalTx:
+    transaction: "Transaction"
+    chain_position: "ChainPosition"
+    @typing.no_type_check
+    def __init__(self, transaction: "Transaction", chain_position: "ChainPosition"):
+        self.transaction = transaction
+        self.chain_position = chain_position
+
+    def __str__(self):
+        return "CanonicalTx(transaction={}, chain_position={})".format(self.transaction, self.chain_position)
+
+    def __eq__(self, other):
+        if self.transaction != other.transaction:
+            return False
+        if self.chain_position != other.chain_position:
+            return False
+        return True
+
+class _UniffiConverterTypeCanonicalTx(_UniffiConverterRustBuffer):
+    @staticmethod
+    def read(buf):
+        return CanonicalTx(
+            transaction=_UniffiConverterTypeTransaction.read(buf),
+            chain_position=_UniffiConverterTypeChainPosition.read(buf),
+        )
+
+    @staticmethod
+    def check_lower(value):
+        _UniffiConverterTypeTransaction.check_lower(value.transaction)
+        _UniffiConverterTypeChainPosition.check_lower(value.chain_position)
+
+    @staticmethod
+    def write(value, buf):
+        _UniffiConverterTypeTransaction.write(value.transaction, buf)
+        _UniffiConverterTypeChainPosition.write(value.chain_position, buf)
+
+
 class LocalOutput:
     outpoint: "OutPoint"
     txout: "TxOut"
     keychain: "KeychainKind"
     is_spent: "bool"
     @typing.no_type_check
     def __init__(self, outpoint: "OutPoint", txout: "TxOut", keychain: "KeychainKind", is_spent: "bool"):
@@ -4216,14 +4360,198 @@
 
     @staticmethod
     def write(value, buf):
         _UniffiConverterUInt64.write(value.value, buf)
         _UniffiConverterTypeScript.write(value.script_pubkey, buf)
 
 
+# AddressError
+# We want to define each variant as a nested class that's also a subclass,
+# which is tricky in Python.  To accomplish this we're going to create each
+# class separately, then manually add the child classes to the base class's
+# __dict__.  All of this happens in dummy class to avoid polluting the module
+# namespace.
+class AddressError(Exception):
+    pass
+
+_UniffiTempAddressError = AddressError
+
+class AddressError:  # type: ignore
+    class Base58(_UniffiTempAddressError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "AddressError.Base58({})".format(str(self))
+    _UniffiTempAddressError.Base58 = Base58 # type: ignore
+    class Bech32(_UniffiTempAddressError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "AddressError.Bech32({})".format(str(self))
+    _UniffiTempAddressError.Bech32 = Bech32 # type: ignore
+    class WitnessVersion(_UniffiTempAddressError):
+
+        def __init__(self, error_message):
+            super().__init__(", ".join([
+                "error_message={!r}".format(error_message),
+            ]))
+            self.error_message = error_message
+        def __repr__(self):
+            return "AddressError.WitnessVersion({})".format(str(self))
+    _UniffiTempAddressError.WitnessVersion = WitnessVersion # type: ignore
+    class WitnessProgram(_UniffiTempAddressError):
+
+        def __init__(self, error_message):
+            super().__init__(", ".join([
+                "error_message={!r}".format(error_message),
+            ]))
+            self.error_message = error_message
+        def __repr__(self):
+            return "AddressError.WitnessProgram({})".format(str(self))
+    _UniffiTempAddressError.WitnessProgram = WitnessProgram # type: ignore
+    class UncompressedPubkey(_UniffiTempAddressError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "AddressError.UncompressedPubkey({})".format(str(self))
+    _UniffiTempAddressError.UncompressedPubkey = UncompressedPubkey # type: ignore
+    class ExcessiveScriptSize(_UniffiTempAddressError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "AddressError.ExcessiveScriptSize({})".format(str(self))
+    _UniffiTempAddressError.ExcessiveScriptSize = ExcessiveScriptSize # type: ignore
+    class UnrecognizedScript(_UniffiTempAddressError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "AddressError.UnrecognizedScript({})".format(str(self))
+    _UniffiTempAddressError.UnrecognizedScript = UnrecognizedScript # type: ignore
+    class NetworkValidation(_UniffiTempAddressError):
+
+        def __init__(self, required, found, address):
+            super().__init__(", ".join([
+                "required={!r}".format(required),
+                "found={!r}".format(found),
+                "address={!r}".format(address),
+            ]))
+            self.required = required
+            self.found = found
+            self.address = address
+        def __repr__(self):
+            return "AddressError.NetworkValidation({})".format(str(self))
+    _UniffiTempAddressError.NetworkValidation = NetworkValidation # type: ignore
+    class OtherAddressErr(_UniffiTempAddressError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "AddressError.OtherAddressErr({})".format(str(self))
+    _UniffiTempAddressError.OtherAddressErr = OtherAddressErr # type: ignore
+
+AddressError = _UniffiTempAddressError # type: ignore
+del _UniffiTempAddressError
+
+
+class _UniffiConverterTypeAddressError(_UniffiConverterRustBuffer):
+    @staticmethod
+    def read(buf):
+        variant = buf.read_i32()
+        if variant == 1:
+            return AddressError.Base58(
+            )
+        if variant == 2:
+            return AddressError.Bech32(
+            )
+        if variant == 3:
+            return AddressError.WitnessVersion(
+                error_message=_UniffiConverterString.read(buf),
+            )
+        if variant == 4:
+            return AddressError.WitnessProgram(
+                error_message=_UniffiConverterString.read(buf),
+            )
+        if variant == 5:
+            return AddressError.UncompressedPubkey(
+            )
+        if variant == 6:
+            return AddressError.ExcessiveScriptSize(
+            )
+        if variant == 7:
+            return AddressError.UnrecognizedScript(
+            )
+        if variant == 8:
+            return AddressError.NetworkValidation(
+                required=_UniffiConverterTypeNetwork.read(buf),
+                found=_UniffiConverterTypeNetwork.read(buf),
+                address=_UniffiConverterString.read(buf),
+            )
+        if variant == 9:
+            return AddressError.OtherAddressErr(
+            )
+        raise InternalError("Raw enum value doesn't match any cases")
+
+    @staticmethod
+    def check_lower(value):
+        if isinstance(value, AddressError.Base58):
+            return
+        if isinstance(value, AddressError.Bech32):
+            return
+        if isinstance(value, AddressError.WitnessVersion):
+            _UniffiConverterString.check_lower(value.error_message)
+            return
+        if isinstance(value, AddressError.WitnessProgram):
+            _UniffiConverterString.check_lower(value.error_message)
+            return
+        if isinstance(value, AddressError.UncompressedPubkey):
+            return
+        if isinstance(value, AddressError.ExcessiveScriptSize):
+            return
+        if isinstance(value, AddressError.UnrecognizedScript):
+            return
+        if isinstance(value, AddressError.NetworkValidation):
+            _UniffiConverterTypeNetwork.check_lower(value.required)
+            _UniffiConverterTypeNetwork.check_lower(value.found)
+            _UniffiConverterString.check_lower(value.address)
+            return
+        if isinstance(value, AddressError.OtherAddressErr):
+            return
+
+    @staticmethod
+    def write(value, buf):
+        if isinstance(value, AddressError.Base58):
+            buf.write_i32(1)
+        if isinstance(value, AddressError.Bech32):
+            buf.write_i32(2)
+        if isinstance(value, AddressError.WitnessVersion):
+            buf.write_i32(3)
+            _UniffiConverterString.write(value.error_message, buf)
+        if isinstance(value, AddressError.WitnessProgram):
+            buf.write_i32(4)
+            _UniffiConverterString.write(value.error_message, buf)
+        if isinstance(value, AddressError.UncompressedPubkey):
+            buf.write_i32(5)
+        if isinstance(value, AddressError.ExcessiveScriptSize):
+            buf.write_i32(6)
+        if isinstance(value, AddressError.UnrecognizedScript):
+            buf.write_i32(7)
+        if isinstance(value, AddressError.NetworkValidation):
+            buf.write_i32(8)
+            _UniffiConverterTypeNetwork.write(value.required, buf)
+            _UniffiConverterTypeNetwork.write(value.found, buf)
+            _UniffiConverterString.write(value.address, buf)
+        if isinstance(value, AddressError.OtherAddressErr):
+            buf.write_i32(9)
+
+
 
 
 
 class AddressIndex:
     def __init__(self):
         raise RuntimeError("AddressIndex cannot be instantiated directly")
 
@@ -4449,14 +4777,119 @@
             buf.write_i32(2)
             _UniffiConverterInt64.write(value.fee, buf)
 
 
 
 
 
+class ChainPosition:
+    def __init__(self):
+        raise RuntimeError("ChainPosition cannot be instantiated directly")
+
+    # Each enum variant is a nested class of the enum itself.
+    class CONFIRMED:
+        height: "int"
+        timestamp: "int"
+
+        @typing.no_type_check
+        def __init__(self,height: "int", timestamp: "int"):
+            
+            self.height = height
+            self.timestamp = timestamp
+            
+
+        def __str__(self):
+            return "ChainPosition.CONFIRMED(height={}, timestamp={})".format(self.height, self.timestamp)
+
+        def __eq__(self, other):
+            if not other.is_confirmed():
+                return False
+            if self.height != other.height:
+                return False
+            if self.timestamp != other.timestamp:
+                return False
+            return True
+    class UNCONFIRMED:
+        timestamp: "int"
+
+        @typing.no_type_check
+        def __init__(self,timestamp: "int"):
+            
+            self.timestamp = timestamp
+            
+
+        def __str__(self):
+            return "ChainPosition.UNCONFIRMED(timestamp={})".format(self.timestamp)
+
+        def __eq__(self, other):
+            if not other.is_unconfirmed():
+                return False
+            if self.timestamp != other.timestamp:
+                return False
+            return True
+    
+
+    # For each variant, we have an `is_NAME` method for easily checking
+    # whether an instance is that variant.
+    def is_confirmed(self) -> bool:
+        return isinstance(self, ChainPosition.CONFIRMED)
+    def is_unconfirmed(self) -> bool:
+        return isinstance(self, ChainPosition.UNCONFIRMED)
+    
+
+# Now, a little trick - we make each nested variant class be a subclass of the main
+# enum class, so that method calls and instance checks etc will work intuitively.
+# We might be able to do this a little more neatly with a metaclass, but this'll do.
+ChainPosition.CONFIRMED = type("ChainPosition.CONFIRMED", (ChainPosition.CONFIRMED, ChainPosition,), {})  # type: ignore
+ChainPosition.UNCONFIRMED = type("ChainPosition.UNCONFIRMED", (ChainPosition.UNCONFIRMED, ChainPosition,), {})  # type: ignore
+
+
+
+
+class _UniffiConverterTypeChainPosition(_UniffiConverterRustBuffer):
+    @staticmethod
+    def read(buf):
+        variant = buf.read_i32()
+        if variant == 1:
+            return ChainPosition.CONFIRMED(
+                _UniffiConverterUInt32.read(buf),
+                _UniffiConverterUInt64.read(buf),
+            )
+        if variant == 2:
+            return ChainPosition.UNCONFIRMED(
+                _UniffiConverterUInt64.read(buf),
+            )
+        raise InternalError("Raw enum value doesn't match any cases")
+
+    @staticmethod
+    def check_lower(value):
+        if value.is_confirmed():
+            _UniffiConverterUInt32.check_lower(value.height)
+            _UniffiConverterUInt64.check_lower(value.timestamp)
+            return
+        if value.is_unconfirmed():
+            _UniffiConverterUInt64.check_lower(value.timestamp)
+            return
+
+    @staticmethod
+    def write(value, buf):
+        if value.is_confirmed():
+            buf.write_i32(1)
+            _UniffiConverterUInt32.write(value.height, buf)
+            _UniffiConverterUInt64.write(value.timestamp, buf)
+        if value.is_unconfirmed():
+            buf.write_i32(2)
+            _UniffiConverterUInt64.write(value.timestamp, buf)
+
+
+
+
+
+
+
 class ChangeSpendPolicy(enum.Enum):
     CHANGE_ALLOWED = 0
     
     ONLY_CHANGE = 1
     
     CHANGE_FORBIDDEN = 2
     
@@ -4491,103 +4924,344 @@
             buf.write_i32(2)
         if value == ChangeSpendPolicy.CHANGE_FORBIDDEN:
             buf.write_i32(3)
 
 
 
 
+# DescriptorError
+# We want to define each variant as a nested class that's also a subclass,
+# which is tricky in Python.  To accomplish this we're going to create each
+# class separately, then manually add the child classes to the base class's
+# __dict__.  All of this happens in dummy class to avoid polluting the module
+# namespace.
+class DescriptorError(Exception):
+    pass
+
+_UniffiTempDescriptorError = DescriptorError
+
+class DescriptorError:  # type: ignore
+    class InvalidHdKeyPath(_UniffiTempDescriptorError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "DescriptorError.InvalidHdKeyPath({})".format(str(self))
+    _UniffiTempDescriptorError.InvalidHdKeyPath = InvalidHdKeyPath # type: ignore
+    class InvalidDescriptorChecksum(_UniffiTempDescriptorError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "DescriptorError.InvalidDescriptorChecksum({})".format(str(self))
+    _UniffiTempDescriptorError.InvalidDescriptorChecksum = InvalidDescriptorChecksum # type: ignore
+    class HardenedDerivationXpub(_UniffiTempDescriptorError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "DescriptorError.HardenedDerivationXpub({})".format(str(self))
+    _UniffiTempDescriptorError.HardenedDerivationXpub = HardenedDerivationXpub # type: ignore
+    class MultiPath(_UniffiTempDescriptorError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "DescriptorError.MultiPath({})".format(str(self))
+    _UniffiTempDescriptorError.MultiPath = MultiPath # type: ignore
+    class Key(_UniffiTempDescriptorError):
+
+        def __init__(self, e):
+            super().__init__(", ".join([
+                "e={!r}".format(e),
+            ]))
+            self.e = e
+        def __repr__(self):
+            return "DescriptorError.Key({})".format(str(self))
+    _UniffiTempDescriptorError.Key = Key # type: ignore
+    class Policy(_UniffiTempDescriptorError):
+
+        def __init__(self, e):
+            super().__init__(", ".join([
+                "e={!r}".format(e),
+            ]))
+            self.e = e
+        def __repr__(self):
+            return "DescriptorError.Policy({})".format(str(self))
+    _UniffiTempDescriptorError.Policy = Policy # type: ignore
+    class InvalidDescriptorCharacter(_UniffiTempDescriptorError):
+
+        def __init__(self, char):
+            super().__init__(", ".join([
+                "char={!r}".format(char),
+            ]))
+            self.char = char
+        def __repr__(self):
+            return "DescriptorError.InvalidDescriptorCharacter({})".format(str(self))
+    _UniffiTempDescriptorError.InvalidDescriptorCharacter = InvalidDescriptorCharacter # type: ignore
+    class Bip32(_UniffiTempDescriptorError):
+
+        def __init__(self, e):
+            super().__init__(", ".join([
+                "e={!r}".format(e),
+            ]))
+            self.e = e
+        def __repr__(self):
+            return "DescriptorError.Bip32({})".format(str(self))
+    _UniffiTempDescriptorError.Bip32 = Bip32 # type: ignore
+    class Base58(_UniffiTempDescriptorError):
+
+        def __init__(self, e):
+            super().__init__(", ".join([
+                "e={!r}".format(e),
+            ]))
+            self.e = e
+        def __repr__(self):
+            return "DescriptorError.Base58({})".format(str(self))
+    _UniffiTempDescriptorError.Base58 = Base58 # type: ignore
+    class Pk(_UniffiTempDescriptorError):
+
+        def __init__(self, e):
+            super().__init__(", ".join([
+                "e={!r}".format(e),
+            ]))
+            self.e = e
+        def __repr__(self):
+            return "DescriptorError.Pk({})".format(str(self))
+    _UniffiTempDescriptorError.Pk = Pk # type: ignore
+    class Miniscript(_UniffiTempDescriptorError):
+
+        def __init__(self, e):
+            super().__init__(", ".join([
+                "e={!r}".format(e),
+            ]))
+            self.e = e
+        def __repr__(self):
+            return "DescriptorError.Miniscript({})".format(str(self))
+    _UniffiTempDescriptorError.Miniscript = Miniscript # type: ignore
+    class Hex(_UniffiTempDescriptorError):
+
+        def __init__(self, e):
+            super().__init__(", ".join([
+                "e={!r}".format(e),
+            ]))
+            self.e = e
+        def __repr__(self):
+            return "DescriptorError.Hex({})".format(str(self))
+    _UniffiTempDescriptorError.Hex = Hex # type: ignore
+
+DescriptorError = _UniffiTempDescriptorError # type: ignore
+del _UniffiTempDescriptorError
+
+
+class _UniffiConverterTypeDescriptorError(_UniffiConverterRustBuffer):
+    @staticmethod
+    def read(buf):
+        variant = buf.read_i32()
+        if variant == 1:
+            return DescriptorError.InvalidHdKeyPath(
+            )
+        if variant == 2:
+            return DescriptorError.InvalidDescriptorChecksum(
+            )
+        if variant == 3:
+            return DescriptorError.HardenedDerivationXpub(
+            )
+        if variant == 4:
+            return DescriptorError.MultiPath(
+            )
+        if variant == 5:
+            return DescriptorError.Key(
+                e=_UniffiConverterString.read(buf),
+            )
+        if variant == 6:
+            return DescriptorError.Policy(
+                e=_UniffiConverterString.read(buf),
+            )
+        if variant == 7:
+            return DescriptorError.InvalidDescriptorCharacter(
+                char=_UniffiConverterString.read(buf),
+            )
+        if variant == 8:
+            return DescriptorError.Bip32(
+                e=_UniffiConverterString.read(buf),
+            )
+        if variant == 9:
+            return DescriptorError.Base58(
+                e=_UniffiConverterString.read(buf),
+            )
+        if variant == 10:
+            return DescriptorError.Pk(
+                e=_UniffiConverterString.read(buf),
+            )
+        if variant == 11:
+            return DescriptorError.Miniscript(
+                e=_UniffiConverterString.read(buf),
+            )
+        if variant == 12:
+            return DescriptorError.Hex(
+                e=_UniffiConverterString.read(buf),
+            )
+        raise InternalError("Raw enum value doesn't match any cases")
+
+    @staticmethod
+    def check_lower(value):
+        if isinstance(value, DescriptorError.InvalidHdKeyPath):
+            return
+        if isinstance(value, DescriptorError.InvalidDescriptorChecksum):
+            return
+        if isinstance(value, DescriptorError.HardenedDerivationXpub):
+            return
+        if isinstance(value, DescriptorError.MultiPath):
+            return
+        if isinstance(value, DescriptorError.Key):
+            _UniffiConverterString.check_lower(value.e)
+            return
+        if isinstance(value, DescriptorError.Policy):
+            _UniffiConverterString.check_lower(value.e)
+            return
+        if isinstance(value, DescriptorError.InvalidDescriptorCharacter):
+            _UniffiConverterString.check_lower(value.char)
+            return
+        if isinstance(value, DescriptorError.Bip32):
+            _UniffiConverterString.check_lower(value.e)
+            return
+        if isinstance(value, DescriptorError.Base58):
+            _UniffiConverterString.check_lower(value.e)
+            return
+        if isinstance(value, DescriptorError.Pk):
+            _UniffiConverterString.check_lower(value.e)
+            return
+        if isinstance(value, DescriptorError.Miniscript):
+            _UniffiConverterString.check_lower(value.e)
+            return
+        if isinstance(value, DescriptorError.Hex):
+            _UniffiConverterString.check_lower(value.e)
+            return
+
+    @staticmethod
+    def write(value, buf):
+        if isinstance(value, DescriptorError.InvalidHdKeyPath):
+            buf.write_i32(1)
+        if isinstance(value, DescriptorError.InvalidDescriptorChecksum):
+            buf.write_i32(2)
+        if isinstance(value, DescriptorError.HardenedDerivationXpub):
+            buf.write_i32(3)
+        if isinstance(value, DescriptorError.MultiPath):
+            buf.write_i32(4)
+        if isinstance(value, DescriptorError.Key):
+            buf.write_i32(5)
+            _UniffiConverterString.write(value.e, buf)
+        if isinstance(value, DescriptorError.Policy):
+            buf.write_i32(6)
+            _UniffiConverterString.write(value.e, buf)
+        if isinstance(value, DescriptorError.InvalidDescriptorCharacter):
+            buf.write_i32(7)
+            _UniffiConverterString.write(value.char, buf)
+        if isinstance(value, DescriptorError.Bip32):
+            buf.write_i32(8)
+            _UniffiConverterString.write(value.e, buf)
+        if isinstance(value, DescriptorError.Base58):
+            buf.write_i32(9)
+            _UniffiConverterString.write(value.e, buf)
+        if isinstance(value, DescriptorError.Pk):
+            buf.write_i32(10)
+            _UniffiConverterString.write(value.e, buf)
+        if isinstance(value, DescriptorError.Miniscript):
+            buf.write_i32(11)
+            _UniffiConverterString.write(value.e, buf)
+        if isinstance(value, DescriptorError.Hex):
+            buf.write_i32(12)
+            _UniffiConverterString.write(value.e, buf)
+
+
 # EsploraError
 # We want to define each variant as a nested class that's also a subclass,
 # which is tricky in Python.  To accomplish this we're going to create each
 # class separately, then manually add the child classes to the base class's
 # __dict__.  All of this happens in dummy class to avoid polluting the module
 # namespace.
 class EsploraError(Exception):
     pass
 
 _UniffiTempEsploraError = EsploraError
 
 class EsploraError:  # type: ignore
-    class Ureq(_UniffiTempEsploraError):
+    class Minreq(_UniffiTempEsploraError):
 
         def __init__(self, error_message):
             super().__init__(", ".join([
                 "error_message={!r}".format(error_message),
             ]))
             self.error_message = error_message
         def __repr__(self):
-            return "EsploraError.Ureq({})".format(str(self))
-    _UniffiTempEsploraError.Ureq = Ureq # type: ignore
-    class UreqTransport(_UniffiTempEsploraError):
+            return "EsploraError.Minreq({})".format(str(self))
+    _UniffiTempEsploraError.Minreq = Minreq # type: ignore
+    class HttpResponse(_UniffiTempEsploraError):
 
-        def __init__(self, error_message):
+        def __init__(self, status, error_message):
             super().__init__(", ".join([
+                "status={!r}".format(status),
                 "error_message={!r}".format(error_message),
             ]))
+            self.status = status
             self.error_message = error_message
         def __repr__(self):
-            return "EsploraError.UreqTransport({})".format(str(self))
-    _UniffiTempEsploraError.UreqTransport = UreqTransport # type: ignore
-    class Http(_UniffiTempEsploraError):
+            return "EsploraError.HttpResponse({})".format(str(self))
+    _UniffiTempEsploraError.HttpResponse = HttpResponse # type: ignore
+    class Parsing(_UniffiTempEsploraError):
 
-        def __init__(self, status_code):
+        def __init__(self, error_message):
             super().__init__(", ".join([
-                "status_code={!r}".format(status_code),
+                "error_message={!r}".format(error_message),
             ]))
-            self.status_code = status_code
+            self.error_message = error_message
         def __repr__(self):
-            return "EsploraError.Http({})".format(str(self))
-    _UniffiTempEsploraError.Http = Http # type: ignore
-    class Io(_UniffiTempEsploraError):
+            return "EsploraError.Parsing({})".format(str(self))
+    _UniffiTempEsploraError.Parsing = Parsing # type: ignore
+    class StatusCode(_UniffiTempEsploraError):
 
         def __init__(self, error_message):
             super().__init__(", ".join([
                 "error_message={!r}".format(error_message),
             ]))
             self.error_message = error_message
         def __repr__(self):
-            return "EsploraError.Io({})".format(str(self))
-    _UniffiTempEsploraError.Io = Io # type: ignore
-    class NoHeader(_UniffiTempEsploraError):
-
-        def __init__(self):
-            pass
-        def __repr__(self):
-            return "EsploraError.NoHeader({})".format(str(self))
-    _UniffiTempEsploraError.NoHeader = NoHeader # type: ignore
-    class Parsing(_UniffiTempEsploraError):
+            return "EsploraError.StatusCode({})".format(str(self))
+    _UniffiTempEsploraError.StatusCode = StatusCode # type: ignore
+    class BitcoinEncoding(_UniffiTempEsploraError):
 
         def __init__(self, error_message):
             super().__init__(", ".join([
                 "error_message={!r}".format(error_message),
             ]))
             self.error_message = error_message
         def __repr__(self):
-            return "EsploraError.Parsing({})".format(str(self))
-    _UniffiTempEsploraError.Parsing = Parsing # type: ignore
-    class BitcoinEncoding(_UniffiTempEsploraError):
+            return "EsploraError.BitcoinEncoding({})".format(str(self))
+    _UniffiTempEsploraError.BitcoinEncoding = BitcoinEncoding # type: ignore
+    class HexToArray(_UniffiTempEsploraError):
 
         def __init__(self, error_message):
             super().__init__(", ".join([
                 "error_message={!r}".format(error_message),
             ]))
             self.error_message = error_message
         def __repr__(self):
-            return "EsploraError.BitcoinEncoding({})".format(str(self))
-    _UniffiTempEsploraError.BitcoinEncoding = BitcoinEncoding # type: ignore
-    class Hex(_UniffiTempEsploraError):
+            return "EsploraError.HexToArray({})".format(str(self))
+    _UniffiTempEsploraError.HexToArray = HexToArray # type: ignore
+    class HexToBytes(_UniffiTempEsploraError):
 
         def __init__(self, error_message):
             super().__init__(", ".join([
                 "error_message={!r}".format(error_message),
             ]))
             self.error_message = error_message
         def __repr__(self):
-            return "EsploraError.Hex({})".format(str(self))
-    _UniffiTempEsploraError.Hex = Hex # type: ignore
+            return "EsploraError.HexToBytes({})".format(str(self))
+    _UniffiTempEsploraError.HexToBytes = HexToBytes # type: ignore
     class TransactionNotFound(_UniffiTempEsploraError):
 
         def __init__(self):
             pass
         def __repr__(self):
             return "EsploraError.TransactionNotFound({})".format(str(self))
     _UniffiTempEsploraError.TransactionNotFound = TransactionNotFound # type: ignore
@@ -4604,131 +5278,302 @@
     class HeaderHashNotFound(_UniffiTempEsploraError):
 
         def __init__(self):
             pass
         def __repr__(self):
             return "EsploraError.HeaderHashNotFound({})".format(str(self))
     _UniffiTempEsploraError.HeaderHashNotFound = HeaderHashNotFound # type: ignore
+    class InvalidHttpHeaderName(_UniffiTempEsploraError):
+
+        def __init__(self, name):
+            super().__init__(", ".join([
+                "name={!r}".format(name),
+            ]))
+            self.name = name
+        def __repr__(self):
+            return "EsploraError.InvalidHttpHeaderName({})".format(str(self))
+    _UniffiTempEsploraError.InvalidHttpHeaderName = InvalidHttpHeaderName # type: ignore
+    class InvalidHttpHeaderValue(_UniffiTempEsploraError):
+
+        def __init__(self, value):
+            super().__init__(", ".join([
+                "value={!r}".format(value),
+            ]))
+            self.value = value
+        def __repr__(self):
+            return "EsploraError.InvalidHttpHeaderValue({})".format(str(self))
+    _UniffiTempEsploraError.InvalidHttpHeaderValue = InvalidHttpHeaderValue # type: ignore
 
 EsploraError = _UniffiTempEsploraError # type: ignore
 del _UniffiTempEsploraError
 
 
 class _UniffiConverterTypeEsploraError(_UniffiConverterRustBuffer):
     @staticmethod
     def read(buf):
         variant = buf.read_i32()
         if variant == 1:
-            return EsploraError.Ureq(
+            return EsploraError.Minreq(
                 error_message=_UniffiConverterString.read(buf),
             )
         if variant == 2:
-            return EsploraError.UreqTransport(
+            return EsploraError.HttpResponse(
+                status=_UniffiConverterUInt16.read(buf),
                 error_message=_UniffiConverterString.read(buf),
             )
         if variant == 3:
-            return EsploraError.Http(
-                status_code=_UniffiConverterUInt16.read(buf),
+            return EsploraError.Parsing(
+                error_message=_UniffiConverterString.read(buf),
             )
         if variant == 4:
-            return EsploraError.Io(
+            return EsploraError.StatusCode(
                 error_message=_UniffiConverterString.read(buf),
             )
         if variant == 5:
-            return EsploraError.NoHeader(
+            return EsploraError.BitcoinEncoding(
+                error_message=_UniffiConverterString.read(buf),
             )
         if variant == 6:
-            return EsploraError.Parsing(
+            return EsploraError.HexToArray(
                 error_message=_UniffiConverterString.read(buf),
             )
         if variant == 7:
-            return EsploraError.BitcoinEncoding(
+            return EsploraError.HexToBytes(
                 error_message=_UniffiConverterString.read(buf),
             )
         if variant == 8:
-            return EsploraError.Hex(
-                error_message=_UniffiConverterString.read(buf),
-            )
-        if variant == 9:
             return EsploraError.TransactionNotFound(
             )
-        if variant == 10:
+        if variant == 9:
             return EsploraError.HeaderHeightNotFound(
                 height=_UniffiConverterUInt32.read(buf),
             )
-        if variant == 11:
+        if variant == 10:
             return EsploraError.HeaderHashNotFound(
             )
+        if variant == 11:
+            return EsploraError.InvalidHttpHeaderName(
+                name=_UniffiConverterString.read(buf),
+            )
+        if variant == 12:
+            return EsploraError.InvalidHttpHeaderValue(
+                value=_UniffiConverterString.read(buf),
+            )
         raise InternalError("Raw enum value doesn't match any cases")
 
     @staticmethod
     def check_lower(value):
-        if isinstance(value, EsploraError.Ureq):
+        if isinstance(value, EsploraError.Minreq):
             _UniffiConverterString.check_lower(value.error_message)
             return
-        if isinstance(value, EsploraError.UreqTransport):
+        if isinstance(value, EsploraError.HttpResponse):
+            _UniffiConverterUInt16.check_lower(value.status)
             _UniffiConverterString.check_lower(value.error_message)
             return
-        if isinstance(value, EsploraError.Http):
-            _UniffiConverterUInt16.check_lower(value.status_code)
-            return
-        if isinstance(value, EsploraError.Io):
+        if isinstance(value, EsploraError.Parsing):
             _UniffiConverterString.check_lower(value.error_message)
             return
-        if isinstance(value, EsploraError.NoHeader):
-            return
-        if isinstance(value, EsploraError.Parsing):
+        if isinstance(value, EsploraError.StatusCode):
             _UniffiConverterString.check_lower(value.error_message)
             return
         if isinstance(value, EsploraError.BitcoinEncoding):
             _UniffiConverterString.check_lower(value.error_message)
             return
-        if isinstance(value, EsploraError.Hex):
+        if isinstance(value, EsploraError.HexToArray):
+            _UniffiConverterString.check_lower(value.error_message)
+            return
+        if isinstance(value, EsploraError.HexToBytes):
             _UniffiConverterString.check_lower(value.error_message)
             return
         if isinstance(value, EsploraError.TransactionNotFound):
             return
         if isinstance(value, EsploraError.HeaderHeightNotFound):
             _UniffiConverterUInt32.check_lower(value.height)
             return
         if isinstance(value, EsploraError.HeaderHashNotFound):
             return
+        if isinstance(value, EsploraError.InvalidHttpHeaderName):
+            _UniffiConverterString.check_lower(value.name)
+            return
+        if isinstance(value, EsploraError.InvalidHttpHeaderValue):
+            _UniffiConverterString.check_lower(value.value)
+            return
 
     @staticmethod
     def write(value, buf):
-        if isinstance(value, EsploraError.Ureq):
+        if isinstance(value, EsploraError.Minreq):
             buf.write_i32(1)
             _UniffiConverterString.write(value.error_message, buf)
-        if isinstance(value, EsploraError.UreqTransport):
+        if isinstance(value, EsploraError.HttpResponse):
             buf.write_i32(2)
+            _UniffiConverterUInt16.write(value.status, buf)
             _UniffiConverterString.write(value.error_message, buf)
-        if isinstance(value, EsploraError.Http):
+        if isinstance(value, EsploraError.Parsing):
             buf.write_i32(3)
-            _UniffiConverterUInt16.write(value.status_code, buf)
-        if isinstance(value, EsploraError.Io):
+            _UniffiConverterString.write(value.error_message, buf)
+        if isinstance(value, EsploraError.StatusCode):
             buf.write_i32(4)
             _UniffiConverterString.write(value.error_message, buf)
-        if isinstance(value, EsploraError.NoHeader):
+        if isinstance(value, EsploraError.BitcoinEncoding):
             buf.write_i32(5)
-        if isinstance(value, EsploraError.Parsing):
+            _UniffiConverterString.write(value.error_message, buf)
+        if isinstance(value, EsploraError.HexToArray):
             buf.write_i32(6)
             _UniffiConverterString.write(value.error_message, buf)
-        if isinstance(value, EsploraError.BitcoinEncoding):
+        if isinstance(value, EsploraError.HexToBytes):
             buf.write_i32(7)
             _UniffiConverterString.write(value.error_message, buf)
-        if isinstance(value, EsploraError.Hex):
-            buf.write_i32(8)
-            _UniffiConverterString.write(value.error_message, buf)
         if isinstance(value, EsploraError.TransactionNotFound):
-            buf.write_i32(9)
+            buf.write_i32(8)
         if isinstance(value, EsploraError.HeaderHeightNotFound):
-            buf.write_i32(10)
+            buf.write_i32(9)
             _UniffiConverterUInt32.write(value.height, buf)
         if isinstance(value, EsploraError.HeaderHashNotFound):
+            buf.write_i32(10)
+        if isinstance(value, EsploraError.InvalidHttpHeaderName):
             buf.write_i32(11)
+            _UniffiConverterString.write(value.name, buf)
+        if isinstance(value, EsploraError.InvalidHttpHeaderValue):
+            buf.write_i32(12)
+            _UniffiConverterString.write(value.value, buf)
+
+
+# ExtractTxError
+# We want to define each variant as a nested class that's also a subclass,
+# which is tricky in Python.  To accomplish this we're going to create each
+# class separately, then manually add the child classes to the base class's
+# __dict__.  All of this happens in dummy class to avoid polluting the module
+# namespace.
+class ExtractTxError(Exception):
+    pass
+
+_UniffiTempExtractTxError = ExtractTxError
+
+class ExtractTxError:  # type: ignore
+    class AbsurdFeeRate(_UniffiTempExtractTxError):
+
+        def __init__(self, fee_rate):
+            super().__init__(", ".join([
+                "fee_rate={!r}".format(fee_rate),
+            ]))
+            self.fee_rate = fee_rate
+        def __repr__(self):
+            return "ExtractTxError.AbsurdFeeRate({})".format(str(self))
+    _UniffiTempExtractTxError.AbsurdFeeRate = AbsurdFeeRate # type: ignore
+    class MissingInputValue(_UniffiTempExtractTxError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "ExtractTxError.MissingInputValue({})".format(str(self))
+    _UniffiTempExtractTxError.MissingInputValue = MissingInputValue # type: ignore
+    class SendingTooMuch(_UniffiTempExtractTxError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "ExtractTxError.SendingTooMuch({})".format(str(self))
+    _UniffiTempExtractTxError.SendingTooMuch = SendingTooMuch # type: ignore
+    class OtherExtractTxErr(_UniffiTempExtractTxError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "ExtractTxError.OtherExtractTxErr({})".format(str(self))
+    _UniffiTempExtractTxError.OtherExtractTxErr = OtherExtractTxErr # type: ignore
+
+ExtractTxError = _UniffiTempExtractTxError # type: ignore
+del _UniffiTempExtractTxError
+
+
+class _UniffiConverterTypeExtractTxError(_UniffiConverterRustBuffer):
+    @staticmethod
+    def read(buf):
+        variant = buf.read_i32()
+        if variant == 1:
+            return ExtractTxError.AbsurdFeeRate(
+                fee_rate=_UniffiConverterUInt64.read(buf),
+            )
+        if variant == 2:
+            return ExtractTxError.MissingInputValue(
+            )
+        if variant == 3:
+            return ExtractTxError.SendingTooMuch(
+            )
+        if variant == 4:
+            return ExtractTxError.OtherExtractTxErr(
+            )
+        raise InternalError("Raw enum value doesn't match any cases")
+
+    @staticmethod
+    def check_lower(value):
+        if isinstance(value, ExtractTxError.AbsurdFeeRate):
+            _UniffiConverterUInt64.check_lower(value.fee_rate)
+            return
+        if isinstance(value, ExtractTxError.MissingInputValue):
+            return
+        if isinstance(value, ExtractTxError.SendingTooMuch):
+            return
+        if isinstance(value, ExtractTxError.OtherExtractTxErr):
+            return
+
+    @staticmethod
+    def write(value, buf):
+        if isinstance(value, ExtractTxError.AbsurdFeeRate):
+            buf.write_i32(1)
+            _UniffiConverterUInt64.write(value.fee_rate, buf)
+        if isinstance(value, ExtractTxError.MissingInputValue):
+            buf.write_i32(2)
+        if isinstance(value, ExtractTxError.SendingTooMuch):
+            buf.write_i32(3)
+        if isinstance(value, ExtractTxError.OtherExtractTxErr):
+            buf.write_i32(4)
+
+
+# FeeRateError
+# We want to define each variant as a nested class that's also a subclass,
+# which is tricky in Python.  To accomplish this we're going to create each
+# class separately, then manually add the child classes to the base class's
+# __dict__.  All of this happens in dummy class to avoid polluting the module
+# namespace.
+class FeeRateError(Exception):
+    pass
+
+_UniffiTempFeeRateError = FeeRateError
+
+class FeeRateError:  # type: ignore
+    class ArithmeticOverflow(_UniffiTempFeeRateError):
+
+        def __repr__(self):
+            return "FeeRateError.ArithmeticOverflow({})".format(repr(str(self)))
+    _UniffiTempFeeRateError.ArithmeticOverflow = ArithmeticOverflow # type: ignore
+
+FeeRateError = _UniffiTempFeeRateError # type: ignore
+del _UniffiTempFeeRateError
+
+
+class _UniffiConverterTypeFeeRateError(_UniffiConverterRustBuffer):
+    @staticmethod
+    def read(buf):
+        variant = buf.read_i32()
+        if variant == 1:
+            return FeeRateError.ArithmeticOverflow(
+                _UniffiConverterString.read(buf),
+            )
+        raise InternalError("Raw enum value doesn't match any cases")
+
+    @staticmethod
+    def check_lower(value):
+        if isinstance(value, FeeRateError.ArithmeticOverflow):
+            return
+
+    @staticmethod
+    def write(value, buf):
+        if isinstance(value, FeeRateError.ArithmeticOverflow):
+            buf.write_i32(1)
 
 
 
 
 
 class KeychainKind(enum.Enum):
     EXTERNAL = 0
@@ -4813,14 +5658,329 @@
             buf.write_i32(3)
         if value == Network.REGTEST:
             buf.write_i32(4)
 
 
 
 
+# PersistenceError
+# We want to define each variant as a nested class that's also a subclass,
+# which is tricky in Python.  To accomplish this we're going to create each
+# class separately, then manually add the child classes to the base class's
+# __dict__.  All of this happens in dummy class to avoid polluting the module
+# namespace.
+class PersistenceError(Exception):
+    pass
+
+_UniffiTempPersistenceError = PersistenceError
+
+class PersistenceError:  # type: ignore
+    class Write(_UniffiTempPersistenceError):
+
+        def __init__(self, e):
+            super().__init__(", ".join([
+                "e={!r}".format(e),
+            ]))
+            self.e = e
+        def __repr__(self):
+            return "PersistenceError.Write({})".format(str(self))
+    _UniffiTempPersistenceError.Write = Write # type: ignore
+
+PersistenceError = _UniffiTempPersistenceError # type: ignore
+del _UniffiTempPersistenceError
+
+
+class _UniffiConverterTypePersistenceError(_UniffiConverterRustBuffer):
+    @staticmethod
+    def read(buf):
+        variant = buf.read_i32()
+        if variant == 1:
+            return PersistenceError.Write(
+                e=_UniffiConverterString.read(buf),
+            )
+        raise InternalError("Raw enum value doesn't match any cases")
+
+    @staticmethod
+    def check_lower(value):
+        if isinstance(value, PersistenceError.Write):
+            _UniffiConverterString.check_lower(value.e)
+            return
+
+    @staticmethod
+    def write(value, buf):
+        if isinstance(value, PersistenceError.Write):
+            buf.write_i32(1)
+            _UniffiConverterString.write(value.e, buf)
+
+
+# PsbtParseError
+# We want to define each variant as a nested class that's also a subclass,
+# which is tricky in Python.  To accomplish this we're going to create each
+# class separately, then manually add the child classes to the base class's
+# __dict__.  All of this happens in dummy class to avoid polluting the module
+# namespace.
+class PsbtParseError(Exception):
+    pass
+
+_UniffiTempPsbtParseError = PsbtParseError
+
+class PsbtParseError:  # type: ignore
+    class PsbtEncoding(_UniffiTempPsbtParseError):
+
+        def __init__(self, e):
+            super().__init__(", ".join([
+                "e={!r}".format(e),
+            ]))
+            self.e = e
+        def __repr__(self):
+            return "PsbtParseError.PsbtEncoding({})".format(str(self))
+    _UniffiTempPsbtParseError.PsbtEncoding = PsbtEncoding # type: ignore
+    class Base64Encoding(_UniffiTempPsbtParseError):
+
+        def __init__(self, e):
+            super().__init__(", ".join([
+                "e={!r}".format(e),
+            ]))
+            self.e = e
+        def __repr__(self):
+            return "PsbtParseError.Base64Encoding({})".format(str(self))
+    _UniffiTempPsbtParseError.Base64Encoding = Base64Encoding # type: ignore
+
+PsbtParseError = _UniffiTempPsbtParseError # type: ignore
+del _UniffiTempPsbtParseError
+
+
+class _UniffiConverterTypePsbtParseError(_UniffiConverterRustBuffer):
+    @staticmethod
+    def read(buf):
+        variant = buf.read_i32()
+        if variant == 1:
+            return PsbtParseError.PsbtEncoding(
+                e=_UniffiConverterString.read(buf),
+            )
+        if variant == 2:
+            return PsbtParseError.Base64Encoding(
+                e=_UniffiConverterString.read(buf),
+            )
+        raise InternalError("Raw enum value doesn't match any cases")
+
+    @staticmethod
+    def check_lower(value):
+        if isinstance(value, PsbtParseError.PsbtEncoding):
+            _UniffiConverterString.check_lower(value.e)
+            return
+        if isinstance(value, PsbtParseError.Base64Encoding):
+            _UniffiConverterString.check_lower(value.e)
+            return
+
+    @staticmethod
+    def write(value, buf):
+        if isinstance(value, PsbtParseError.PsbtEncoding):
+            buf.write_i32(1)
+            _UniffiConverterString.write(value.e, buf)
+        if isinstance(value, PsbtParseError.Base64Encoding):
+            buf.write_i32(2)
+            _UniffiConverterString.write(value.e, buf)
+
+
+# TransactionError
+# We want to define each variant as a nested class that's also a subclass,
+# which is tricky in Python.  To accomplish this we're going to create each
+# class separately, then manually add the child classes to the base class's
+# __dict__.  All of this happens in dummy class to avoid polluting the module
+# namespace.
+class TransactionError(Exception):
+    pass
+
+_UniffiTempTransactionError = TransactionError
+
+class TransactionError:  # type: ignore
+    class Io(_UniffiTempTransactionError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "TransactionError.Io({})".format(str(self))
+    _UniffiTempTransactionError.Io = Io # type: ignore
+    class OversizedVectorAllocation(_UniffiTempTransactionError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "TransactionError.OversizedVectorAllocation({})".format(str(self))
+    _UniffiTempTransactionError.OversizedVectorAllocation = OversizedVectorAllocation # type: ignore
+    class InvalidChecksum(_UniffiTempTransactionError):
+
+        def __init__(self, expected, actual):
+            super().__init__(", ".join([
+                "expected={!r}".format(expected),
+                "actual={!r}".format(actual),
+            ]))
+            self.expected = expected
+            self.actual = actual
+        def __repr__(self):
+            return "TransactionError.InvalidChecksum({})".format(str(self))
+    _UniffiTempTransactionError.InvalidChecksum = InvalidChecksum # type: ignore
+    class NonMinimalVarInt(_UniffiTempTransactionError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "TransactionError.NonMinimalVarInt({})".format(str(self))
+    _UniffiTempTransactionError.NonMinimalVarInt = NonMinimalVarInt # type: ignore
+    class ParseFailed(_UniffiTempTransactionError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "TransactionError.ParseFailed({})".format(str(self))
+    _UniffiTempTransactionError.ParseFailed = ParseFailed # type: ignore
+    class UnsupportedSegwitFlag(_UniffiTempTransactionError):
+
+        def __init__(self, flag):
+            super().__init__(", ".join([
+                "flag={!r}".format(flag),
+            ]))
+            self.flag = flag
+        def __repr__(self):
+            return "TransactionError.UnsupportedSegwitFlag({})".format(str(self))
+    _UniffiTempTransactionError.UnsupportedSegwitFlag = UnsupportedSegwitFlag # type: ignore
+    class OtherTransactionErr(_UniffiTempTransactionError):
+
+        def __init__(self):
+            pass
+        def __repr__(self):
+            return "TransactionError.OtherTransactionErr({})".format(str(self))
+    _UniffiTempTransactionError.OtherTransactionErr = OtherTransactionErr # type: ignore
+
+TransactionError = _UniffiTempTransactionError # type: ignore
+del _UniffiTempTransactionError
+
+
+class _UniffiConverterTypeTransactionError(_UniffiConverterRustBuffer):
+    @staticmethod
+    def read(buf):
+        variant = buf.read_i32()
+        if variant == 1:
+            return TransactionError.Io(
+            )
+        if variant == 2:
+            return TransactionError.OversizedVectorAllocation(
+            )
+        if variant == 3:
+            return TransactionError.InvalidChecksum(
+                expected=_UniffiConverterString.read(buf),
+                actual=_UniffiConverterString.read(buf),
+            )
+        if variant == 4:
+            return TransactionError.NonMinimalVarInt(
+            )
+        if variant == 5:
+            return TransactionError.ParseFailed(
+            )
+        if variant == 6:
+            return TransactionError.UnsupportedSegwitFlag(
+                flag=_UniffiConverterUInt8.read(buf),
+            )
+        if variant == 7:
+            return TransactionError.OtherTransactionErr(
+            )
+        raise InternalError("Raw enum value doesn't match any cases")
+
+    @staticmethod
+    def check_lower(value):
+        if isinstance(value, TransactionError.Io):
+            return
+        if isinstance(value, TransactionError.OversizedVectorAllocation):
+            return
+        if isinstance(value, TransactionError.InvalidChecksum):
+            _UniffiConverterString.check_lower(value.expected)
+            _UniffiConverterString.check_lower(value.actual)
+            return
+        if isinstance(value, TransactionError.NonMinimalVarInt):
+            return
+        if isinstance(value, TransactionError.ParseFailed):
+            return
+        if isinstance(value, TransactionError.UnsupportedSegwitFlag):
+            _UniffiConverterUInt8.check_lower(value.flag)
+            return
+        if isinstance(value, TransactionError.OtherTransactionErr):
+            return
+
+    @staticmethod
+    def write(value, buf):
+        if isinstance(value, TransactionError.Io):
+            buf.write_i32(1)
+        if isinstance(value, TransactionError.OversizedVectorAllocation):
+            buf.write_i32(2)
+        if isinstance(value, TransactionError.InvalidChecksum):
+            buf.write_i32(3)
+            _UniffiConverterString.write(value.expected, buf)
+            _UniffiConverterString.write(value.actual, buf)
+        if isinstance(value, TransactionError.NonMinimalVarInt):
+            buf.write_i32(4)
+        if isinstance(value, TransactionError.ParseFailed):
+            buf.write_i32(5)
+        if isinstance(value, TransactionError.UnsupportedSegwitFlag):
+            buf.write_i32(6)
+            _UniffiConverterUInt8.write(value.flag, buf)
+        if isinstance(value, TransactionError.OtherTransactionErr):
+            buf.write_i32(7)
+
+
+# TxidParseError
+# We want to define each variant as a nested class that's also a subclass,
+# which is tricky in Python.  To accomplish this we're going to create each
+# class separately, then manually add the child classes to the base class's
+# __dict__.  All of this happens in dummy class to avoid polluting the module
+# namespace.
+class TxidParseError(Exception):
+    pass
+
+_UniffiTempTxidParseError = TxidParseError
+
+class TxidParseError:  # type: ignore
+    class InvalidTxid(_UniffiTempTxidParseError):
+
+        def __init__(self, txid):
+            super().__init__(", ".join([
+                "txid={!r}".format(txid),
+            ]))
+            self.txid = txid
+        def __repr__(self):
+            return "TxidParseError.InvalidTxid({})".format(str(self))
+    _UniffiTempTxidParseError.InvalidTxid = InvalidTxid # type: ignore
+
+TxidParseError = _UniffiTempTxidParseError # type: ignore
+del _UniffiTempTxidParseError
+
+
+class _UniffiConverterTypeTxidParseError(_UniffiConverterRustBuffer):
+    @staticmethod
+    def read(buf):
+        variant = buf.read_i32()
+        if variant == 1:
+            return TxidParseError.InvalidTxid(
+                txid=_UniffiConverterString.read(buf),
+            )
+        raise InternalError("Raw enum value doesn't match any cases")
+
+    @staticmethod
+    def check_lower(value):
+        if isinstance(value, TxidParseError.InvalidTxid):
+            _UniffiConverterString.check_lower(value.txid)
+            return
+
+    @staticmethod
+    def write(value, buf):
+        if isinstance(value, TxidParseError.InvalidTxid):
+            buf.write_i32(1)
+            _UniffiConverterString.write(value.txid, buf)
+
+
 # WalletCreationError
 # We want to define each variant as a nested class that's also a subclass,
 # which is tricky in Python.  To accomplish this we're going to create each
 # class separately, then manually add the child classes to the base class's
 # __dict__.  All of this happens in dummy class to avoid polluting the module
 # namespace.
 class WalletCreationError(Exception):
@@ -5099,14 +6259,41 @@
         elif flag == 1:
             return _UniffiConverterTypeDescriptor.read(buf)
         else:
             raise InternalError("Unexpected flag byte for optional type")
 
 
 
+class _UniffiConverterOptionalTypeCanonicalTx(_UniffiConverterRustBuffer):
+    @classmethod
+    def check_lower(cls, value):
+        if value is not None:
+            _UniffiConverterTypeCanonicalTx.check_lower(value)
+
+    @classmethod
+    def write(cls, value, buf):
+        if value is None:
+            buf.write_u8(0)
+            return
+
+        buf.write_u8(1)
+        _UniffiConverterTypeCanonicalTx.write(value, buf)
+
+    @classmethod
+    def read(cls, buf):
+        flag = buf.read_u8()
+        if flag == 0:
+            return None
+        elif flag == 1:
+            return _UniffiConverterTypeCanonicalTx.read(buf)
+        else:
+            raise InternalError("Unexpected flag byte for optional type")
+
+
+
 class _UniffiConverterOptionalTypeNetwork(_UniffiConverterRustBuffer):
     @classmethod
     def check_lower(cls, value):
         if value is not None:
             _UniffiConverterTypeNetwork.check_lower(value)
 
     @classmethod
@@ -5151,35 +6338,60 @@
 
         return [
             _UniffiConverterUInt8.read(buf) for i in range(count)
         ]
 
 
 
-class _UniffiConverterSequenceTypeTransaction(_UniffiConverterRustBuffer):
+class _UniffiConverterSequenceTypeCanonicalTx(_UniffiConverterRustBuffer):
+    @classmethod
+    def check_lower(cls, value):
+        for item in value:
+            _UniffiConverterTypeCanonicalTx.check_lower(item)
+
+    @classmethod
+    def write(cls, value, buf):
+        items = len(value)
+        buf.write_i32(items)
+        for item in value:
+            _UniffiConverterTypeCanonicalTx.write(item, buf)
+
+    @classmethod
+    def read(cls, buf):
+        count = buf.read_i32()
+        if count < 0:
+            raise InternalError("Unexpected negative sequence length")
+
+        return [
+            _UniffiConverterTypeCanonicalTx.read(buf) for i in range(count)
+        ]
+
+
+
+class _UniffiConverterSequenceTypeLocalOutput(_UniffiConverterRustBuffer):
     @classmethod
     def check_lower(cls, value):
         for item in value:
-            _UniffiConverterTypeTransaction.check_lower(item)
+            _UniffiConverterTypeLocalOutput.check_lower(item)
 
     @classmethod
     def write(cls, value, buf):
         items = len(value)
         buf.write_i32(items)
         for item in value:
-            _UniffiConverterTypeTransaction.write(item, buf)
+            _UniffiConverterTypeLocalOutput.write(item, buf)
 
     @classmethod
     def read(cls, buf):
         count = buf.read_i32()
         if count < 0:
             raise InternalError("Unexpected negative sequence length")
 
         return [
-            _UniffiConverterTypeTransaction.read(buf) for i in range(count)
+            _UniffiConverterTypeLocalOutput.read(buf) for i in range(count)
         ]
 
 
 
 class _UniffiConverterSequenceTypeOutPoint(_UniffiConverterRustBuffer):
     @classmethod
     def check_lower(cls, value):
@@ -5226,40 +6438,50 @@
 
         return [
             _UniffiConverterTypeScriptAmount.read(buf) for i in range(count)
         ]
 
 __all__ = [
     "InternalError",
+    "AddressError",
     "AddressIndex",
     "Alpha3Error",
     "CalculateFeeError",
+    "ChainPosition",
     "ChangeSpendPolicy",
+    "DescriptorError",
     "EsploraError",
+    "ExtractTxError",
+    "FeeRateError",
     "KeychainKind",
     "Network",
+    "PersistenceError",
+    "PsbtParseError",
+    "TransactionError",
+    "TxidParseError",
     "WalletCreationError",
     "WordCount",
     "AddressInfo",
     "Balance",
+    "CanonicalTx",
     "LocalOutput",
     "OutPoint",
     "ScriptAmount",
     "SentAndReceivedValues",
     "TxOut",
     "Address",
     "BumpFeeTxBuilder",
     "DerivationPath",
     "Descriptor",
     "DescriptorPublicKey",
     "DescriptorSecretKey",
     "EsploraClient",
     "FeeRate",
     "Mnemonic",
-    "PartiallySignedTransaction",
+    "Psbt",
     "Script",
     "Transaction",
     "TxBuilder",
     "Update",
     "Wallet",
 ]
```

