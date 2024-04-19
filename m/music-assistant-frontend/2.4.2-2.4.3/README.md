# Comparing `tmp/music-assistant-frontend-2.4.2.tar.gz` & `tmp/music-assistant-frontend-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "music-assistant-frontend-2.4.2.tar", last modified: Tue Apr 16 00:06:50 2024, max compression
+gzip compressed data, was "music-assistant-frontend-2.4.3.tar", last modified: Fri Apr 19 10:43:12 2024, max compression
```

## Comparing `music-assistant-frontend-2.4.2.tar` & `music-assistant-frontend-2.4.3.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:06:50.924275 music-assistant-frontend-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 00:05:53.000000 music-assistant-frontend-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 00:05:53.000000 music-assistant-frontend-2.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-16 00:06:50.924275 music-assistant-frontend-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-16 00:05:53.000000 music-assistant-frontend-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:06:50.888275 music-assistant-frontend-2.4.2/music_assistant_frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-16 00:06:42.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-16 00:06:42.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/apple-touch-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:06:50.924275 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/AddGroupPlayer-f291ae3b.js
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/AddProvider-b867b6d9.js
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/AlbumDetails-25e2fe83.js
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Alert-0c4ec871.js
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Alert-3971d760.css
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ArtistDetails-159c8f35.js
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/BrowseView-15d25af1.js
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Container-127b1d7c.css
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Container-ba274a7a.js
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/CoreConfigs-1f56aa74.js
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/CoreConfigs-75569bfe.css
--rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Default-abfbb155.css
--rw-r--r--   0 runner    (1001) docker     (127)    63193 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Default-bd92f6cd.js
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/EditConfig-f2bca5b1.css
--rw-r--r--   0 runner    (1001) docker     (127)    47426 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-658131e8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/EditCoreConfig-db86c453.js
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/EditPlayer-293a9fdd.js
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/EditProvider-b281ecba.js
--rw-r--r--   0 runner    (1001) docker     (127)     8824 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/HomeView-aa005854.js
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/HomeView-f9b96eef.css
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ItemsListing-5372ff4e.css
--rw-r--r--   0 runner    (1001) docker     (127)    23624 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js
--rw-r--r--   0 runner    (1001) docker     (127)    93824 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/JetBrainsMono-Medium-086c48df.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14688 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15764 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15752 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/LibraryAlbums-532f0c88.js
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/LibraryArtists-17fa3e93.js
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/LibraryPlaylists-a41d818d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/LibraryRadios-e4468a3f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/LibraryTracks-a533acbe.js
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ListviewItem-20f54197.css
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ListviewItem-e896b2dc.js
--rw-r--r--   0 runner    (1001) docker     (127)   160576 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
--rw-r--r--   0 runner    (1001) docker     (127)   347588 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   125116 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   143452 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/PanelviewItem-cbf7c595.css
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js
--rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/PlayerQueue-42cde633.js
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Players-0c4ce7a2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/PlaylistDetails-9db516b0.js
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ProviderDetails-2713c080.css
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Providers-ca2eea9e.js
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Providers-e2f60749.css
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/RadioDetails-87373ab9.js
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Search-abd54e1f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Settings-170b9c4c.js
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/TrackDetails-6c6c6bec.js
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VAlert-1c823677.css
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VAlert-f74a2b4b.js
--rw-r--r--   0 runner    (1001) docker     (127)    30209 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VBadge-76d9c3a5.js
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VBadge-bc81f416.css
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VCard-257d0eab.css
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VCard-bfc4071a.js
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VCardText-00c669eb.js
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VDialog-5309eac2.css
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VDialog-82ed2e80.js
--rw-r--r--   0 runner    (1001) docker     (127)    21125 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VExpansionPanel-00a7e4f4.css
--rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VExpansionPanel-9f82eed8.js
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VForm-a7262390.js
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VGrid-37b0738d.css
--rw-r--r--   0 runner    (1001) docker     (127)    18433 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VInput-91b2e758.js
--rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VInput-b16e222c.css
--rw-r--r--   0 runner    (1001) docker     (127)    45661 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VMenu-9506155f.js
--rw-r--r--   0 runner    (1001) docker     (127)    22490 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VMenu-a46f5e7a.css
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VSelect-7df244e0.css
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VSelect-ea96d901.js
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VSlideGroup-5dd0c6f2.js
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VSlideGroup-c5ba1538.css
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTabs-11e16be1.css
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTabs-4c128c89.js
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTextField-8883f272.js
--rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTextField-d31117f3.css
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VToolbar-4ad3b045.js
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VToolbar-78a5e824.css
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTooltip-3a8fb95f.css
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTooltip-a8719c72.js
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VVirtualScroll-29c92c23.css
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VVirtualScroll-5f35af5d.js
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/contextmenu-c4231154.js
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/cover_dark-75402cd0.png
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/cover_light-b832ae9e.png
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/fallback-d0ff2800.png
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/folder-6b5595ac.svg
--rw-r--r--   0 runner    (1001) docker     (127)    40039 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/forwardRefs-70e877d2.js
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/forwardRefs-e5b3781d.css
--rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/hires-438c7046.png
--rw-r--r--   0 runner    (1001) docker     (127)   699901 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/index-52c10419.css
--rw-r--r--   0 runner    (1001) docker     (127)   677473 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/index-6ff57e4c.js
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/index.browser-342e672c.js
--rw-r--r--   0 runner    (1001) docker     (127)    28226 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/layout-bdc1c8bd.js
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/logo-9391b78c.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/m4a-45331b05.png
--rw-r--r--   0 runner    (1001) docker     (127)   155276 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
--rw-r--r--   0 runner    (1001) docker     (127)  1307880 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/materialdesignicons-webfont-0b183104.eot
--rw-r--r--   0 runner    (1001) docker     (127)  1307660 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/materialdesignicons-webfont-61e8aba5.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   403216 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/materialdesignicons-webfont-662fefa8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   587984 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/materialdesignicons-webfont-a5928a0d.woff
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-16 00:06:42.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-16 00:06:44.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-16 00:06:42.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/pwa-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-16 00:06:42.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/pwa-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 00:06:42.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 00:06:42.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-16 00:06:46.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/sw.js
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-16 00:06:46.000000 music-assistant-frontend-2.4.2/music_assistant_frontend/workbox-27b29e6f.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:06:50.888275 music-assistant-frontend-2.4.2/music_assistant_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-16 00:06:50.000000 music-assistant-frontend-2.4.2/music_assistant_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-16 00:06:50.000000 music-assistant-frontend-2.4.2/music_assistant_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:06:50.000000 music-assistant-frontend-2.4.2/music_assistant_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:06:49.000000 music-assistant-frontend-2.4.2/music_assistant_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 00:06:50.000000 music-assistant-frontend-2.4.2/music_assistant_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-16 00:06:17.000000 music-assistant-frontend-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 00:06:50.924275 music-assistant-frontend-2.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:12.245503 music-assistant-frontend-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 10:42:17.000000 music-assistant-frontend-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 10:42:17.000000 music-assistant-frontend-2.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-19 10:43:12.245503 music-assistant-frontend-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-19 10:42:17.000000 music-assistant-frontend-2.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:12.217503 music-assistant-frontend-2.4.3/music_assistant_frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/apple-touch-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:12.245503 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AddGroupPlayer-8a4f0893.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AddProvider-f756ebc3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AlbumDetails-0b4de4f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Alert-19e36349.js
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Alert-3971d760.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ArtistDetails-53ff83d9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/BrowseView-a95cb7cc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Container-127b1d7c.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Container-dc894acd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/CoreConfigs-75569bfe.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/CoreConfigs-f0329745.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Default-2157b447.css
+-rw-r--r--   0 runner    (1001) docker     (127)    64005 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Default-c7088a94.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditConfig-f2bca5b1.css
+-rw-r--r--   0 runner    (1001) docker     (127)    47426 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditCoreConfig-d27a9b35.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditPlayer-6e04043d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditProvider-e046ee5d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8824 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/HomeView-8f9e6181.js
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/HomeView-f9b96eef.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ItemsListing-5372ff4e.css
+-rw-r--r--   0 runner    (1001) docker     (127)    23624 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js
+-rw-r--r--   0 runner    (1001) docker     (127)    93824 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/JetBrainsMono-Medium-086c48df.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14688 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15764 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15752 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryAlbums-7cfa0763.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryArtists-9924ed14.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryPlaylists-95e35cdd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryRadios-4a033696.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryTracks-eeccb967.js
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ListviewItem-20f54197.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ListviewItem-8b992256.js
+-rw-r--r--   0 runner    (1001) docker     (127)   160576 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   347588 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   125116 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   143452 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PanelviewItem-cbf7c595.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PlayerQueue-9f89c917.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Players-0e31a251.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PlaylistDetails-2fe134b1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ProviderDetails-2713c080.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Providers-58a591e0.js
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Providers-e2f60749.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/RadioDetails-54e9e340.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Search-00ee9dd8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Settings-bbdb2168.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/TrackDetails-72029d5e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VAlert-1c823677.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VAlert-56af8987.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30407 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VBadge-84e3406b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VBadge-8b8b8a6d.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VCard-257d0eab.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VCard-b98fe47e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VCardText-6774ea5e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VDialog-5309eac2.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VDialog-d7e50927.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21125 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VExpansionPanel-00a7e4f4.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VExpansionPanel-58c5fe02.js
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VForm-fc99b4aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VGrid-37b0738d.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18433 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VInput-5b197ccd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VInput-b16e222c.css
+-rw-r--r--   0 runner    (1001) docker     (127)    22490 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VMenu-a46f5e7a.css
+-rw-r--r--   0 runner    (1001) docker     (127)    45661 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VMenu-b634019c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSelect-7df244e0.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSelect-d10e917f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSlideGroup-b576aa37.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSlideGroup-c5ba1538.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTabs-11e16be1.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTabs-8ad24bfd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTextField-0c2ec62d.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTextField-d31117f3.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VToolbar-78a5e824.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VToolbar-b7f10b15.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTooltip-3a8fb95f.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTooltip-3ef94159.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VVirtualScroll-29c92c23.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VVirtualScroll-84259ceb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/contextmenu-521b5304.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/cover_dark-75402cd0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/cover_light-b832ae9e.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/fallback-d0ff2800.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/folder-6b5595ac.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    40039 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/forwardRefs-7be90dc2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/forwardRefs-e5b3781d.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/hires-438c7046.png
+-rw-r--r--   0 runner    (1001) docker     (127)   699901 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/index-52c10419.css
+-rw-r--r--   0 runner    (1001) docker     (127)   703850 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/index-b687f95a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/index.browser-342e672c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28226 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/layout-42b7d22e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/logo-9391b78c.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/m4a-45331b05.png
+-rw-r--r--   0 runner    (1001) docker     (127)   155276 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)  1307880 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-0b183104.eot
+-rw-r--r--   0 runner    (1001) docker     (127)  1307660 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-61e8aba5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   403216 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-662fefa8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   587984 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-a5928a0d.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/pwa-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/pwa-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-19 10:43:08.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/sw.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-19 10:43:08.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/workbox-27b29e6f.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:12.217503 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-19 10:43:11.000000 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-19 10:43:12.000000 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:43:11.000000 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:43:10.000000 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 10:43:12.000000 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-19 10:42:38.000000 music-assistant-frontend-2.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:43:12.249503 music-assistant-frontend-2.4.3/setup.cfg
```

### Comparing `music-assistant-frontend-2.4.2/LICENSE` & `music-assistant-frontend-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/PKG-INFO` & `music-assistant-frontend-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-assistant-frontend
-Version: 2.4.2
+Version: 2.4.3
 Summary: The Music Assistant frontend
 Author-email: The Music Assistant Authors <m.vanderveldt@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/music-assistant/frontend
 Platform: any
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `music-assistant-frontend-2.4.2/README.md` & `music-assistant-frontend-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/apple-touch-icon.png` & `music-assistant-frontend-2.4.3/music_assistant_frontend/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/AddGroupPlayer-f291ae3b.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AddGroupPlayer-8a4f0893.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -10,36 +10,36 @@
     l as a,
     A as o,
     x as v,
     Q as c,
     N as p,
     I as N,
     B as s
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     a as U,
     V as w
-} from "./VCardText-00c669eb.js";
+} from "./VCardText-6774ea5e.js";
 import {
     k as P,
     l as b
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     V as T
-} from "./VForm-a7262390.js";
+} from "./VForm-fc99b4aa.js";
 import {
     V as S
-} from "./VTextField-8883f272.js";
+} from "./VTextField-0c2ec62d.js";
 import {
     V as q
-} from "./VSelect-ea96d901.js";
-import "./VMenu-9506155f.js";
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VVirtualScroll-5f35af5d.js";
+} from "./VSelect-d10e917f.js";
+import "./VMenu-b634019c.js";
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VVirtualScroll-84259ceb.js";
 const A = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/AddProvider-b867b6d9.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AddProvider-f756ebc3.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -16,41 +16,41 @@
     A as l,
     x as a,
     Q as p,
     N as d,
     z as y,
     B as r,
     I as v
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     _ as T
-} from "./EditConfig.vue_vue_type_style_index_0_lang-658131e8.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js";
 import {
     a as $,
     V as A
-} from "./VCardText-00c669eb.js";
+} from "./VCardText-6774ea5e.js";
 import {
     a as _
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 import {
     k as j,
     x as I
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     f as U
-} from "./VMenu-9506155f.js";
-import "./VExpansionPanel-9f82eed8.js";
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VForm-a7262390.js"; /* empty css              */
-import "./VDialog-82ed2e80.js";
-import "./VAlert-f74a2b4b.js";
-import "./VTextField-8883f272.js";
-import "./VSelect-ea96d901.js";
-import "./VVirtualScroll-5f35af5d.js";
+} from "./VMenu-b634019c.js";
+import "./VExpansionPanel-58c5fe02.js";
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VForm-fc99b4aa.js"; /* empty css              */
+import "./VDialog-d7e50927.js";
+import "./VAlert-56af8987.js";
+import "./VTextField-0c2ec62d.js";
+import "./VSelect-d10e917f.js";
+import "./VVirtualScroll-84259ceb.js";
 const z = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/AlbumDetails-25e2fe83.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AlbumDetails-0b4de4f6.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     _ as v
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
 import {
     _ as h,
     a as w
-} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js";
+} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js";
 import {
     v as A,
     r as d,
     c as g,
     ap as c,
     w as I,
     o as D,
@@ -17,34 +17,34 @@
     b as E,
     y as l,
     E as M,
     l as V,
     z as n,
     I as u,
     B as f
-} from "./index-6ff57e4c.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VToolbar-4ad3b045.js";
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
-import "./layout-bdc1c8bd.js";
-import "./VDialog-82ed2e80.js";
+} from "./index-b687f95a.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VToolbar-b7f10b15.js";
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
+import "./layout-42b7d22e.js";
+import "./VDialog-d7e50927.js";
 const T = f("br", null, null, -1),
     $ = f("br", null, null, -1),
     te = A({
         __name: "AlbumDetails",
         props: {
             itemId: {},
             provider: {},
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ArtistDetails-159c8f35.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ArtistDetails-53ff83d9.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     _ as b
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
 import {
     _ as A,
     a as h
-} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js";
+} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js";
 import {
     v as g,
     r as p,
     w as I,
     o as D,
     L as l,
     an as F,
@@ -17,34 +17,34 @@
     ap as v,
     y as o,
     E as B,
     l as E,
     z as m,
     I as d,
     B as _
-} from "./index-6ff57e4c.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VToolbar-4ad3b045.js";
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
-import "./layout-bdc1c8bd.js";
-import "./VDialog-82ed2e80.js";
+} from "./index-b687f95a.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VToolbar-b7f10b15.js";
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
+import "./layout-42b7d22e.js";
+import "./VDialog-d7e50927.js";
 const $ = _("br", null, null, -1),
     N = _("br", null, null, -1),
     re = g({
         __name: "ArtistDetails",
         props: {
             itemId: {},
             provider: {}
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/BrowseView-15d25af1.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/BrowseView-a95cb7cc.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -4,35 +4,35 @@
     aa as c,
     c as u,
     K as a,
     y as h,
     E as f,
     l as w,
     L as b
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     _ as d
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VToolbar-4ad3b045.js";
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VToolbar-b7f10b15.js";
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
 const A = n({
     __name: "BrowseView",
     props: {
         path: {}
     },
     setup(s) {
         const t = s,
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Container-127b1d7c.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Container-127b1d7c.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Container-ba274a7a.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Container-dc894acd.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -16,28 +16,28 @@
     l as f,
     F as C,
     I as P,
     a6 as L,
     p as w,
     g as B,
     u as A
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     l as x,
     n as b,
     a as D,
     d as S,
     i as T
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     e as H,
     b as R,
     d as F,
     V as E
-} from "./VMenu-9506155f.js"; /* empty css              */
+} from "./VMenu-b634019c.js"; /* empty css              */
 const N = {
     props: {
         variant: {
             type: String,
             default: "default",
             validator: t => ["plain", "default", "responsive", "icon", "list"].includes(t)
         }
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/CoreConfigs-1f56aa74.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/CoreConfigs-f0329745.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -20,32 +20,32 @@
     N as t,
     F as w,
     G,
     x as s,
     I as T,
     af as Q,
     z as V
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     C as B,
     L as j,
     _ as J
-} from "./Container-ba274a7a.js";
+} from "./Container-dc894acd.js";
 import {
     V as I
-} from "./VToolbar-4ad3b045.js";
+} from "./VToolbar-b7f10b15.js";
 import {
     a as K,
     o as O,
     d as W,
     q as X,
     i as Y,
     n as A
-} from "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
+} from "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
 const Z = D({
         fixedHeader: Boolean,
         fixedFooter: Boolean,
         height: [Number, String],
         hover: Boolean,
         ...K(),
         ...O(),
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/CoreConfigs-75569bfe.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/CoreConfigs-75569bfe.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Default-abfbb155.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Default-2157b447.css`

 * *Files 7% similar despite different names*

```diff
@@ -1 +1 @@
-@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.v-navigation-drawer{-webkit-overflow-scrolling:touch;display:flex;flex-direction:column;height:100%;max-width:100%;pointer-events:auto;transition-duration:.2s;transition-property:box-shadow,transform,visibility,width,height,left,right,top,bottom;transition-timing-function:cubic-bezier(.4,0,.2,1);position:absolute;border-color:rgba(var(--v-border-color),var(--v-border-opacity));border-style:solid;border-width:0;box-shadow:0 0 0 0 var(--v-shadow-key-umbra-opacity, rgba(0, 0, 0, .2)),0 0 0 0 var(--v-shadow-key-penumbra-opacity, rgba(0, 0, 0, .14)),0 0 0 0 var(--v-shadow-key-ambient-opacity, rgba(0, 0, 0, .12));background:rgb(var(--v-theme-surface));color:rgba(var(--v-theme-on-surface),var(--v-high-emphasis-opacity))}.v-navigation-drawer--border{border-width:thin;box-shadow:none}.v-navigation-drawer--rounded{border-radius:4px}.v-navigation-drawer--top{top:0;border-bottom-width:thin}.v-navigation-drawer--bottom{left:0;border-top-width:thin}.v-navigation-drawer--left{top:0;left:0;right:auto;border-right-width:thin}.v-navigation-drawer--right{top:0;left:auto;right:0;border-left-width:thin}.v-navigation-drawer--floating{border:none}.v-navigation-drawer--temporary{box-shadow:0 8px 10px -5px var(--v-shadow-key-umbra-opacity, rgba(0, 0, 0, .2)),0 16px 24px 2px var(--v-shadow-key-penumbra-opacity, rgba(0, 0, 0, .14)),0 6px 30px 5px var(--v-shadow-key-ambient-opacity, rgba(0, 0, 0, .12))}.v-navigation-drawer--sticky{height:auto;transition:box-shadow,transform,visibility,width,height,left,right}.v-navigation-drawer .v-list{overflow:hidden}.v-navigation-drawer__content{flex:0 1 auto;height:100%;max-width:100%;overflow-x:hidden;overflow-y:auto}.v-navigation-drawer__img{height:100%;left:0;position:absolute;top:0;width:100%;z-index:-1}.v-navigation-drawer__img img:not(.v-img__img){height:inherit;object-fit:cover;width:inherit}.v-navigation-drawer__scrim{position:absolute;top:0;left:0;width:100%;height:100%;background:black;opacity:.2;transition:opacity .2s cubic-bezier(.4,0,.2,1);z-index:1}.v-navigation-drawer__prepend,.v-navigation-drawer__append{flex:none;overflow:hidden}.logo_text{margin-left:25px;font-family:JetBrains Mono Medium;font-size:55;font-weight:500}.logo_icon{margin-left:-5px;border-radius:4px}.fullscreen-menu .v-overlay__content{left:0;right:0;top:0;bottom:0}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.v-main{flex:1 0 auto;max-width:100%;transition:.2s cubic-bezier(.4,0,.2,1);padding-left:var(--v-layout-left);padding-right:var(--v-layout-right);padding-top:var(--v-layout-top);padding-bottom:var(--v-layout-bottom)}.v-main__scroller{max-width:100%;position:relative}.v-main--scrollable{display:flex;position:absolute;top:0;left:0;width:100%;height:100%}.v-main--scrollable>.v-main__scroller{flex:1 1 auto;overflow-y:auto;--v-layout-left: 0px;--v-layout-right: 0px;--v-layout-top: 0px;--v-layout-bottom: 0px}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.v-bottom-navigation{display:flex;max-width:100%;overflow:hidden;position:absolute;transition:transform,color .2s,.2s cubic-bezier(.4,0,.2,1);border-color:rgba(var(--v-border-color),var(--v-border-opacity));border-style:solid;border-width:0;border-radius:0;background:rgb(var(--v-theme-surface));color:rgba(var(--v-theme-on-surface),var(--v-high-emphasis-opacity))}.v-bottom-navigation--border{border-width:thin;box-shadow:none}.v-bottom-navigation--active{box-shadow:0 2px 4px -1px var(--v-shadow-key-umbra-opacity, rgba(0, 0, 0, .2)),0 4px 5px 0 var(--v-shadow-key-penumbra-opacity, rgba(0, 0, 0, .14)),0 1px 10px 0 var(--v-shadow-key-ambient-opacity, rgba(0, 0, 0, .12))}.v-bottom-navigation__content{display:flex;flex:none;font-size:.75rem;justify-content:center;transition:inherit;width:100%}.v-bottom-navigation .v-bottom-navigation__content>.v-btn{font-size:inherit;height:100%;max-width:168px;min-width:80px;text-transform:none;transition:inherit;width:auto;border-radius:0}.v-bottom-navigation .v-bottom-navigation__content>.v-btn .v-btn__content,.v-bottom-navigation .v-bottom-navigation__content>.v-btn .v-btn__icon{transition:inherit}.v-bottom-navigation .v-bottom-navigation__content>.v-btn .v-btn__icon{font-size:1.5rem}.v-bottom-navigation--grow .v-bottom-navigation__content>.v-btn{flex-grow:1}.v-bottom-navigation--shift .v-bottom-navigation__content .v-btn:not(.v-btn--selected) .v-btn__content>span{transition:inherit;opacity:0}.v-bottom-navigation--shift .v-bottom-navigation__content .v-btn:not(.v-btn--selected) .v-btn__content{transform:translateY(.5rem)}.menuButton{font-weight:300;font-size:x-small;font-stretch:condensed;text-transform:none;margin-top:5px}.v-slide-group-item--active{opacity:100%}.responsive-icon-holder[data-v-5ed57264]{display:flex;align-items:center;justify-content:center}.responsive-icon-holder-btn[data-v-5ed57264]{display:flex;align-items:center;justify-content:center;opacity:.62;cursor:pointer!important}.responsive-icon-holder-btn[data-v-5ed57264]:focus,.responsive-icon-holder-btn[data-v-5ed57264]:hover{opacity:1}.responsive-icon-holder-btn[data-v-5ed57264]:focus{outline:none;color:#0f0}.responsive-icon-holder-btn[data-v-5ed57264]:active{opacity:1}.responsive-icon-holder-btn.disabled[data-v-5ed57264]{opacity:.5;cursor:not-allowed}.responsive-icon[data-v-5ed57264]{line-height:1}.player-controls-elements{width:46px;height:46px;display:flex;justify-content:center;align-items:center}.no_transform{text-transform:none}.vc-slider{padding-top:13px;margin-inline-start:0px!important;margin-inline-end:0px!important}.volume-control-dialog>.v-overlay__content{bottom:135px!important;right:5px!important;left:unset!important;top:unset!important}.fullscreen-container[data-v-1ba8c187]{display:flex;flex-flow:column;height:100%;padding-bottom:5px}.fullscreen-track-info[data-v-1ba8c187]{margin-top:10px;margin-bottom:10px;padding-top:2vh;padding-bottom:2vh;text-align:center}.fullscreen-track-info-subtitle[data-v-1ba8c187]{opacity:.5}.media-controls-item[data-v-1ba8c187]{margin:0 10px;width:100%;height:100%}@media (max-width: 768px){.media-controls-item[data-v-1ba8c187]{margin:0 5px;width:100%;height:100%}}.fullscreen-row[data-v-1ba8c187]{display:grid;flex:0 1 auto;align-content:center}.fullscreen-row-centered[data-v-1ba8c187]{display:grid;flex:0 1 auto;justify-content:center}.fullscreen-media-controls[data-v-1ba8c187]{display:flex;flex:1 1 auto;align-items:center}.fullscreen-media-controls>button[data-v-1ba8c187]{flex:1 1 auto}.fullscreen-media-controls-bottom[data-v-1ba8c187]{display:flex;flex:0 1 auto;justify-content:center;align-items:center}.fullscreen-media-controls-bottom>div[data-v-1ba8c187]{flex-basis:0;flex-grow:1;max-width:100%}.fullscreen-media-controls>div[data-v-1ba8c187]{width:calc(100% / 3)}.fullscreen-mediacontrols-right[data-v-1ba8c187]{display:table-cell;text-align:right;vertical-align:middle}.fullscreen-mediacontrols-right>div[data-v-1ba8c187]{display:inline-flex;align-items:center}.player-media-thumb{margin-right:10px}.player-track-content-type{height:20px!important;padding:5px 9px!important;font-weight:500;font-size:10px!important;letter-spacing:.1em;border-radius:2px;margin-right:30px}.mediadetails-streamdetails .icon[data-v-de35313d]{opacity:100}.mediacontrols[data-v-de35313d]{display:table;width:100%}.mediacontrols-bg-1[data-v-de35313d]{position:absolute;width:20%;height:100%;left:0;top:0}.mediacontrols-bg-2[data-v-de35313d]{position:absolute;width:40%;height:100%;left:0;top:0;border-radius:10px}.mediacontrols-top-right[data-v-de35313d]{display:table-row}.mediacontrols-left-1[data-v-de35313d]{display:table-cell;vertical-align:middle;width:25%}.mediacontrols-left-2[data-v-de35313d]{display:table-cell;vertical-align:middle}.mediacontrols-left-1>div[data-v-de35313d]{padding:0!important}.mediacontrols-left-2>div[data-v-de35313d]{padding:0!important}.mediacontrols-bottom-center-1[data-v-de35313d]{display:table-cell;text-align:center;width:40%;vertical-align:middle}.mediacontrols-bottom-center-2[data-v-de35313d]{display:none;width:25%}.mediacontrols-bottom-right[data-v-de35313d]{display:table-cell;text-align:right;vertical-align:middle}.mediacontrols-bottom-right>div[data-v-de35313d]{display:inline-flex;align-items:center}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.v-footer{align-items:center;display:flex;flex:1 1 auto;padding:8px 16px;position:relative;transition:.2s cubic-bezier(.4,0,.2,1);transition-property:height,width,transform,max-width,left,right,top,bottom;border-color:rgba(var(--v-border-color),var(--v-border-opacity));border-style:solid;border-width:0;box-shadow:0 0 0 0 var(--v-shadow-key-umbra-opacity, rgba(0, 0, 0, .2)),0 0 0 0 var(--v-shadow-key-penumbra-opacity, rgba(0, 0, 0, .14)),0 0 0 0 var(--v-shadow-key-ambient-opacity, rgba(0, 0, 0, .12));border-radius:0;background:rgb(var(--v-theme-surface));color:rgba(var(--v-theme-on-surface),var(--v-high-emphasis-opacity))}.v-footer--border{border-width:thin;box-shadow:none}.v-footer--absolute{position:absolute}.v-footer--fixed{position:fixed}.v-footer--rounded{border-radius:4px}.mediacontrols-player-float{width:100%;border-top-style:ridge;padding:0!important;left:5px!important;width:calc(100% - 10px)!important;border-radius:10px!important}.mediacontrols-player-default{width:100%;border-top-style:ridge;padding:0}.playerrow{height:60px;margin-right:15px}div.v-expansion-panel-text__wrapper{padding:0}div.v-expansion-panel--active:not(:first-child),.v-expansion-panel--active+.v-expansion-panel{margin-top:0}div.v-expansion-panel__shadow{box-shadow:none}.v-expansion-panel-title__icon{display:inline-flex;margin-bottom:-4px;margin-top:-4px;-webkit-user-select:none;user-select:none;margin-inline-start:auto;margin-right:5px}.v-list-item__prepend{display:unset}.pwa-toast{position:fixed;right:0;bottom:0;margin:16px;padding:12px;border:1px solid #8885;border-radius:4px;z-index:1;text-align:left;box-shadow:3px 4px 5px #8885;background-color:#fff}.pwa-toast .message{margin-bottom:8px}.pwa-toast button{border:1px solid #8885;outline:none;margin-right:5px;border-radius:2px;padding:3px 10px}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.material-icons-outlined{font-family:Material Icons Outlined;font-weight:400;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:"liga";-webkit-font-smoothing:antialiased}html{overflow:hidden}*{-webkit-user-drag:none;-khtml-user-drag:none;-moz-user-drag:none;-o-user-drag:none;user-drag:none;-webkit-touch-callout:none;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}a{cursor:pointer}.v-btn--size-default{padding:0 8px}.vertical-btn{display:flex;flex-direction:column;align-items:center}.right{float:right}.left{float:left}.listitem-media-thumb{height:50px;width:50px;margin-right:10px}.v-slider.v-input--horizontal .v-input__control{min-height:5px}div.v-navigation-drawer__scrim{opacity:.8;background:grey}.v-card--variant-elevated{box-shadow:none;border-width:1px;border-style:solid;font-size:smaller}.line-clamp-2{white-space:pre-line;overflow:hidden;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.v-card-text{padding-right:0}.v-expansion-panel--active>.v-expansion-panel-title{min-height:48px}.v-toolbar>.v-toolbar__content>.v-toolbar-title{margin-inline-start:25px}.v-toolbar>.v-toolbar__content>.v-toolbar__prepend{margin-inline-start:6px}.v-toolbar>.v-toolbar__content>.v-toolbar__append{margin-inline-end:21px}.v-toolbar-default>.v-toolbar__content>.v-toolbar-title{margin-inline-start:16px}.v-toolbar-default>.v-toolbar__content>.v-toolbar__prepend{margin-inline-start:10px}.v-toolbar-default>.v-toolbar__content>.v-toolbar__append{margin-inline-end:10px}.v-toolbar{height:55px}.v-toolbar-title{font-family:JetBrains Mono Medium}.col-2{width:50%;max-width:50%;flex-basis:50%}.col-3{width:33.3%;max-width:33.3%;flex-basis:33.3%}.col-4{width:25%;max-width:25%;flex-basis:25%}.col-5{width:20%;max-width:20%;flex-basis:20%}.col-6{width:16.6%;max-width:16.6%;flex-basis:16.6%}.col-7{width:14.2%;max-width:14.2%;flex-basis:14.2%}.col-8{width:12.5%;max-width:12.5%;flex-basis:12.5%}.col-9{width:11.1%;max-width:11.1%;flex-basis:11.1%}.line-clamp-1{white-space:nowrap;text-overflow:ellipsis;overflow:hidden}.line-clamp-2{white-space:pre-line;overflow:hidden;line-height:1.5em;height:3em;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.small-icon{font-size:22px;height:22px;width:22px}.small-btn,.large-icon{font-size:40px;height:40px;width:40px}.large-btn{font-size:50px;height:50px;width:50px}.v-expansion-panel-title{border-radius:0}.v-input--horizontal .v-input__prepend{margin-inline-end:8px}.v-toolbar__content{height:100%!important}.padded-overlay .v-overlay__content{padding:50px}.v-overlay__scrim{opacity:65%}.v-expansion-panel-title{padding:10px}.flicking-camera{display:flex!important}.v-list-item-subtitle{font-size:.75rem;line-height:1rem;font-weight:400;margin-top:0;margin-bottom:0}.v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}.v-toolbar-title{font-size:1.25rem;line-height:1.75rem;font-weight:500}.v-list-item--nav .v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}h1{font-size:1.5rem;line-height:2rem;font-weight:500}h2{font-size:1.25rem;line-height:1.75rem;font-weight:500}h3{font-size:1.125rem;line-height:1.5rem;font-weight:500}h4{font-size:1rem;line-height:1.25rem;font-weight:700}h5{font-size:.875rem;line-height:1.25rem;font-weight:500}h6{font-size:.75rem;line-height:1rem;font-weight:400}.mh1{margin-top:1.5rem;margin-bottom:1rem}.mh2{margin-top:1.5rem;margin-bottom:.75rem}.mh3{margin-top:1.5rem;margin-bottom:.5rem}.mh4{margin-top:1.25rem;margin-bottom:.5rem}.mh5{margin-top:1rem;margin-bottom:.25rem}.mh6{margin-top:1rem;margin-bottom:0}.v-application{display:flex;background:rgb(var(--v-theme-background));color:rgba(var(--v-theme-on-background),var(--v-high-emphasis-opacity))}.v-application__wrap{backface-visibility:hidden;display:flex;flex-direction:column;flex:1 1 auto;max-width:100%;min-height:100vh;min-height:100dvh;position:relative}
+@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.v-navigation-drawer{-webkit-overflow-scrolling:touch;display:flex;flex-direction:column;height:100%;max-width:100%;pointer-events:auto;transition-duration:.2s;transition-property:box-shadow,transform,visibility,width,height,left,right,top,bottom;transition-timing-function:cubic-bezier(.4,0,.2,1);position:absolute;border-color:rgba(var(--v-border-color),var(--v-border-opacity));border-style:solid;border-width:0;box-shadow:0 0 0 0 var(--v-shadow-key-umbra-opacity, rgba(0, 0, 0, .2)),0 0 0 0 var(--v-shadow-key-penumbra-opacity, rgba(0, 0, 0, .14)),0 0 0 0 var(--v-shadow-key-ambient-opacity, rgba(0, 0, 0, .12));background:rgb(var(--v-theme-surface));color:rgba(var(--v-theme-on-surface),var(--v-high-emphasis-opacity))}.v-navigation-drawer--border{border-width:thin;box-shadow:none}.v-navigation-drawer--rounded{border-radius:4px}.v-navigation-drawer--top{top:0;border-bottom-width:thin}.v-navigation-drawer--bottom{left:0;border-top-width:thin}.v-navigation-drawer--left{top:0;left:0;right:auto;border-right-width:thin}.v-navigation-drawer--right{top:0;left:auto;right:0;border-left-width:thin}.v-navigation-drawer--floating{border:none}.v-navigation-drawer--temporary{box-shadow:0 8px 10px -5px var(--v-shadow-key-umbra-opacity, rgba(0, 0, 0, .2)),0 16px 24px 2px var(--v-shadow-key-penumbra-opacity, rgba(0, 0, 0, .14)),0 6px 30px 5px var(--v-shadow-key-ambient-opacity, rgba(0, 0, 0, .12))}.v-navigation-drawer--sticky{height:auto;transition:box-shadow,transform,visibility,width,height,left,right}.v-navigation-drawer .v-list{overflow:hidden}.v-navigation-drawer__content{flex:0 1 auto;height:100%;max-width:100%;overflow-x:hidden;overflow-y:auto}.v-navigation-drawer__img{height:100%;left:0;position:absolute;top:0;width:100%;z-index:-1}.v-navigation-drawer__img img:not(.v-img__img){height:inherit;object-fit:cover;width:inherit}.v-navigation-drawer__scrim{position:absolute;top:0;left:0;width:100%;height:100%;background:black;opacity:.2;transition:opacity .2s cubic-bezier(.4,0,.2,1);z-index:1}.v-navigation-drawer__prepend,.v-navigation-drawer__append{flex:none;overflow:hidden}.logo_text{margin-left:25px;font-family:JetBrains Mono Medium;font-size:55;font-weight:500}.logo_icon{margin-left:-5px;border-radius:4px}.fullscreen-menu .v-overlay__content{left:0;right:0;top:0;bottom:0}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.v-main{flex:1 0 auto;max-width:100%;transition:.2s cubic-bezier(.4,0,.2,1);padding-left:var(--v-layout-left);padding-right:var(--v-layout-right);padding-top:var(--v-layout-top);padding-bottom:var(--v-layout-bottom)}.v-main__scroller{max-width:100%;position:relative}.v-main--scrollable{display:flex;position:absolute;top:0;left:0;width:100%;height:100%}.v-main--scrollable>.v-main__scroller{flex:1 1 auto;overflow-y:auto;--v-layout-left: 0px;--v-layout-right: 0px;--v-layout-top: 0px;--v-layout-bottom: 0px}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.v-bottom-navigation{display:flex;max-width:100%;overflow:hidden;position:absolute;transition:transform,color .2s,.2s cubic-bezier(.4,0,.2,1);border-color:rgba(var(--v-border-color),var(--v-border-opacity));border-style:solid;border-width:0;border-radius:0;background:rgb(var(--v-theme-surface));color:rgba(var(--v-theme-on-surface),var(--v-high-emphasis-opacity))}.v-bottom-navigation--border{border-width:thin;box-shadow:none}.v-bottom-navigation--active{box-shadow:0 2px 4px -1px var(--v-shadow-key-umbra-opacity, rgba(0, 0, 0, .2)),0 4px 5px 0 var(--v-shadow-key-penumbra-opacity, rgba(0, 0, 0, .14)),0 1px 10px 0 var(--v-shadow-key-ambient-opacity, rgba(0, 0, 0, .12))}.v-bottom-navigation__content{display:flex;flex:none;font-size:.75rem;justify-content:center;transition:inherit;width:100%}.v-bottom-navigation .v-bottom-navigation__content>.v-btn{font-size:inherit;height:100%;max-width:168px;min-width:80px;text-transform:none;transition:inherit;width:auto;border-radius:0}.v-bottom-navigation .v-bottom-navigation__content>.v-btn .v-btn__content,.v-bottom-navigation .v-bottom-navigation__content>.v-btn .v-btn__icon{transition:inherit}.v-bottom-navigation .v-bottom-navigation__content>.v-btn .v-btn__icon{font-size:1.5rem}.v-bottom-navigation--grow .v-bottom-navigation__content>.v-btn{flex-grow:1}.v-bottom-navigation--shift .v-bottom-navigation__content .v-btn:not(.v-btn--selected) .v-btn__content>span{transition:inherit;opacity:0}.v-bottom-navigation--shift .v-bottom-navigation__content .v-btn:not(.v-btn--selected) .v-btn__content{transform:translateY(.5rem)}.menuButton{font-weight:300;font-size:x-small;font-stretch:condensed;text-transform:none;margin-top:5px}.v-slide-group-item--active{opacity:100%}.responsive-icon-holder[data-v-5ed57264]{display:flex;align-items:center;justify-content:center}.responsive-icon-holder-btn[data-v-5ed57264]{display:flex;align-items:center;justify-content:center;opacity:.62;cursor:pointer!important}.responsive-icon-holder-btn[data-v-5ed57264]:focus,.responsive-icon-holder-btn[data-v-5ed57264]:hover{opacity:1}.responsive-icon-holder-btn[data-v-5ed57264]:focus{outline:none;color:#0f0}.responsive-icon-holder-btn[data-v-5ed57264]:active{opacity:1}.responsive-icon-holder-btn.disabled[data-v-5ed57264]{opacity:.5;cursor:not-allowed}.responsive-icon[data-v-5ed57264]{line-height:1}.player-controls-elements{width:46px;height:46px;display:flex;justify-content:center;align-items:center}.no_transform{text-transform:none}.vc-slider{padding-top:13px;margin-inline-start:0px!important;margin-inline-end:0px!important}.volume-control-dialog>.v-overlay__content{bottom:135px!important;right:5px!important;left:unset!important;top:unset!important}.fullscreen-container[data-v-ce8419ef]{display:flex;flex-flow:column;height:100%;padding-bottom:5px}.fullscreen-track-info[data-v-ce8419ef]{margin-top:10px;margin-bottom:10px;padding-top:2vh;padding-bottom:2vh;text-align:center}.fullscreen-track-info-subtitle[data-v-ce8419ef]{opacity:.5}.media-controls-item[data-v-ce8419ef]{margin:0 10px;width:100%;height:100%}@media (max-width: 768px){.media-controls-item[data-v-ce8419ef]{margin:0 5px;width:100%;height:100%}}.fullscreen-row[data-v-ce8419ef]{display:grid;flex:0 1 auto;align-content:center}.fullscreen-row-centered[data-v-ce8419ef]{display:grid;flex:0 1 auto;justify-content:center}.fullscreen-media-controls[data-v-ce8419ef]{display:flex;flex:1 1 auto;align-items:center}.fullscreen-media-controls>button[data-v-ce8419ef]{flex:1 1 auto}.fullscreen-media-controls-bottom[data-v-ce8419ef]{display:flex;flex:0 1 auto;justify-content:center;align-items:center}.fullscreen-media-controls-bottom>div[data-v-ce8419ef]{flex-basis:0;flex-grow:1;max-width:100%}.fullscreen-media-controls>div[data-v-ce8419ef]{width:calc(100% / 3)}.fullscreen-mediacontrols-right[data-v-ce8419ef]{display:table-cell;text-align:right;vertical-align:middle}.fullscreen-mediacontrols-right>div[data-v-ce8419ef]{display:inline-flex;align-items:center}.player-media-thumb{margin-right:10px}.player-track-content-type{height:20px!important;padding:5px 9px!important;font-weight:500;font-size:10px!important;letter-spacing:.1em;border-radius:2px;margin-right:30px}.mediadetails-streamdetails .icon[data-v-b841e61d]{opacity:100}.mediacontrols[data-v-b841e61d]{display:table;width:100%}.mediacontrols-bg-1[data-v-b841e61d]{position:absolute;width:20%;height:100%;left:0;top:0}.mediacontrols-bg-2[data-v-b841e61d]{position:absolute;width:40%;height:100%;left:0;top:0;border-radius:10px}.mediacontrols-top-right[data-v-b841e61d]{display:table-row}.mediacontrols-left-1[data-v-b841e61d]{display:table-cell;vertical-align:middle;width:25%}.mediacontrols-left-2[data-v-b841e61d]{display:table-cell;vertical-align:middle}.mediacontrols-left-1>div[data-v-b841e61d]{padding:0!important}.mediacontrols-left-2>div[data-v-b841e61d]{padding:0!important}.mediacontrols-bottom-center-1[data-v-b841e61d]{display:table-cell;text-align:center;width:40%;vertical-align:middle}.mediacontrols-bottom-center-2[data-v-b841e61d]{display:none;width:25%}.mediacontrols-bottom-right[data-v-b841e61d]{display:table-cell;text-align:right;vertical-align:middle}.mediacontrols-bottom-right>div[data-v-b841e61d]{display:inline-flex;align-items:center}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.v-footer{align-items:center;display:flex;flex:1 1 auto;padding:8px 16px;position:relative;transition:.2s cubic-bezier(.4,0,.2,1);transition-property:height,width,transform,max-width,left,right,top,bottom;border-color:rgba(var(--v-border-color),var(--v-border-opacity));border-style:solid;border-width:0;box-shadow:0 0 0 0 var(--v-shadow-key-umbra-opacity, rgba(0, 0, 0, .2)),0 0 0 0 var(--v-shadow-key-penumbra-opacity, rgba(0, 0, 0, .14)),0 0 0 0 var(--v-shadow-key-ambient-opacity, rgba(0, 0, 0, .12));border-radius:0;background:rgb(var(--v-theme-surface));color:rgba(var(--v-theme-on-surface),var(--v-high-emphasis-opacity))}.v-footer--border{border-width:thin;box-shadow:none}.v-footer--absolute{position:absolute}.v-footer--fixed{position:fixed}.v-footer--rounded{border-radius:4px}.mediacontrols-player-float{width:100%;border-top-style:ridge;padding:0!important;left:5px!important;width:calc(100% - 10px)!important;border-radius:10px!important}.mediacontrols-player-default{width:100%;border-top-style:ridge;padding:0}.playerrow{height:60px;margin-right:15px}div.v-expansion-panel-text__wrapper{padding:0}div.v-expansion-panel--active:not(:first-child),.v-expansion-panel--active+.v-expansion-panel{margin-top:0}div.v-expansion-panel__shadow{box-shadow:none}.v-expansion-panel-title__icon{display:inline-flex;margin-bottom:-4px;margin-top:-4px;-webkit-user-select:none;user-select:none;margin-inline-start:auto;margin-right:5px}.v-list-item__prepend{display:unset}.pwa-toast{position:fixed;right:0;bottom:0;margin:16px;padding:12px;border:1px solid #8885;border-radius:4px;z-index:1;text-align:left;box-shadow:3px 4px 5px #8885;background-color:#fff}.pwa-toast .message{margin-bottom:8px}.pwa-toast button{border:1px solid #8885;outline:none;margin-right:5px;border-radius:2px;padding:3px 10px}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.material-icons-outlined{font-family:Material Icons Outlined;font-weight:400;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:"liga";-webkit-font-smoothing:antialiased}html{overflow:hidden}*{-webkit-user-drag:none;-khtml-user-drag:none;-moz-user-drag:none;-o-user-drag:none;user-drag:none;-webkit-touch-callout:none;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}a{cursor:pointer}.v-btn--size-default{padding:0 8px}.vertical-btn{display:flex;flex-direction:column;align-items:center}.right{float:right}.left{float:left}.listitem-media-thumb{height:50px;width:50px;margin-right:10px}.v-slider.v-input--horizontal .v-input__control{min-height:5px}div.v-navigation-drawer__scrim{opacity:.8;background:grey}.v-card--variant-elevated{box-shadow:none;border-width:1px;border-style:solid;font-size:smaller}.line-clamp-2{white-space:pre-line;overflow:hidden;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.v-card-text{padding-right:0}.v-expansion-panel--active>.v-expansion-panel-title{min-height:48px}.v-toolbar>.v-toolbar__content>.v-toolbar-title{margin-inline-start:25px}.v-toolbar>.v-toolbar__content>.v-toolbar__prepend{margin-inline-start:6px}.v-toolbar>.v-toolbar__content>.v-toolbar__append{margin-inline-end:21px}.v-toolbar-default>.v-toolbar__content>.v-toolbar-title{margin-inline-start:16px}.v-toolbar-default>.v-toolbar__content>.v-toolbar__prepend{margin-inline-start:10px}.v-toolbar-default>.v-toolbar__content>.v-toolbar__append{margin-inline-end:10px}.v-toolbar{height:55px}.v-toolbar-title{font-family:JetBrains Mono Medium}.col-2{width:50%;max-width:50%;flex-basis:50%}.col-3{width:33.3%;max-width:33.3%;flex-basis:33.3%}.col-4{width:25%;max-width:25%;flex-basis:25%}.col-5{width:20%;max-width:20%;flex-basis:20%}.col-6{width:16.6%;max-width:16.6%;flex-basis:16.6%}.col-7{width:14.2%;max-width:14.2%;flex-basis:14.2%}.col-8{width:12.5%;max-width:12.5%;flex-basis:12.5%}.col-9{width:11.1%;max-width:11.1%;flex-basis:11.1%}.line-clamp-1{white-space:nowrap;text-overflow:ellipsis;overflow:hidden}.line-clamp-2{white-space:pre-line;overflow:hidden;line-height:1.5em;height:3em;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.small-icon{font-size:22px;height:22px;width:22px}.small-btn,.large-icon{font-size:40px;height:40px;width:40px}.large-btn{font-size:50px;height:50px;width:50px}.v-expansion-panel-title{border-radius:0}.v-input--horizontal .v-input__prepend{margin-inline-end:8px}.v-toolbar__content{height:100%!important}.padded-overlay .v-overlay__content{padding:50px}.v-overlay__scrim{opacity:65%}.v-expansion-panel-title{padding:10px}.flicking-camera{display:flex!important}.v-list-item-subtitle{font-size:.75rem;line-height:1rem;font-weight:400;margin-top:0;margin-bottom:0}.v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}.v-toolbar-title{font-size:1.25rem;line-height:1.75rem;font-weight:500}.v-list-item--nav .v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}h1{font-size:1.5rem;line-height:2rem;font-weight:500}h2{font-size:1.25rem;line-height:1.75rem;font-weight:500}h3{font-size:1.125rem;line-height:1.5rem;font-weight:500}h4{font-size:1rem;line-height:1.25rem;font-weight:700}h5{font-size:.875rem;line-height:1.25rem;font-weight:500}h6{font-size:.75rem;line-height:1rem;font-weight:400}.mh1{margin-top:1.5rem;margin-bottom:1rem}.mh2{margin-top:1.5rem;margin-bottom:.75rem}.mh3{margin-top:1.5rem;margin-bottom:.5rem}.mh4{margin-top:1.25rem;margin-bottom:.5rem}.mh5{margin-top:1rem;margin-bottom:.25rem}.mh6{margin-top:1rem;margin-bottom:0}.v-application{display:flex;background:rgb(var(--v-theme-background));color:rgba(var(--v-theme-on-background),var(--v-high-emphasis-opacity))}.v-application__wrap{backface-visibility:hidden;display:flex;flex-direction:column;flex:1 1 auto;max-width:100%;min-height:100vh;min-height:100dvh;position:relative}
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Default-bd92f6cd.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Default-c7088a94.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,405 +1,405 @@
 import {
     s as ae,
-    c as S,
-    a as we,
-    o as re,
+    c as x,
+    a as Pe,
+    o as ue,
     w as W,
-    b as ve,
-    C as Wt,
-    p as pe,
+    b as pe,
+    C as Rt,
+    p as ye,
     m as Ht,
     d as Ie,
-    g as ye,
-    u as yt,
-    e as Re,
-    t as X,
-    f as Rt,
-    h as At,
-    r as T,
+    g as fe,
+    u as ft,
+    e as He,
+    t as K,
+    f as At,
+    h as qt,
+    r as S,
     i as Te,
-    j as qt,
-    k as ft,
+    j as Ut,
+    k as ht,
     l as r,
-    n as H,
-    T as ht,
-    F as R,
-    q as Ut,
-    v as M,
+    n as R,
+    T as _t,
+    F as H,
+    q as Ft,
+    v as D,
     x as e,
     y as d,
     z as V,
-    A as y,
+    A as f,
     B as k,
     D as L,
     E as b,
     G as U,
-    H as Ft,
+    H as Ot,
     I,
     J as t,
-    K as C,
+    K as P,
     L as w,
-    M as te,
+    M as Z,
     P as Be,
     N as $,
-    $ as _e,
-    O as Ot,
-    Q as j,
-    R as Yt,
-    S as Gt,
-    U as _t,
-    V as Pe,
+    $ as ge,
+    O as Yt,
+    Q as G,
+    R as Gt,
+    S as jt,
+    U as gt,
+    V as ne,
     W as Me,
-    X as jt,
+    X as Xt,
     Y as De,
-    Z as ce,
+    Z as de,
     _ as Ne,
-    a0 as de,
+    a0 as me,
     a1 as q,
-    a2 as gt,
+    a2 as bt,
     a3 as Ae,
-    a4 as ge,
-    a5 as bt,
-    a6 as ee,
+    a4 as be,
+    a5 as kt,
+    a6 as te,
     a7 as Kt,
-    a8 as Xt,
-    a9 as Zt,
-    aa as Jt,
-    ab as el,
-    ac as tl,
-    ad as be,
-    ae as ll,
-    af as rt,
-    ag as ut,
-    ah as al,
-    ai as kt,
-    aj as ol
-} from "./index-6ff57e4c.js";
+    a8 as Zt,
+    a9 as Jt,
+    aa as el,
+    ab as tl,
+    ac as ll,
+    ad as ke,
+    ae as al,
+    af as ut,
+    ag as ct,
+    ah as ol,
+    ai as wt,
+    aj as il
+} from "./index-b687f95a.js";
 import {
     B as Y,
-    L as K,
+    L as X,
     _ as ze,
     a as xe,
-    C as il
-} from "./Container-ba274a7a.js";
+    C as sl
+} from "./Container-dc894acd.js";
 import {
     u as qe,
-    a as sl,
-    V as ct,
+    a as nl,
+    V as dt,
     b as ie,
-    c as nl,
-    d as dt,
-    e as wt,
-    f as rl
-} from "./VMenu-9506155f.js";
+    c as rl,
+    d as mt,
+    e as Pt,
+    f as ul
+} from "./VMenu-b634019c.js";
 import {
     m as Ue,
-    a as fe,
+    a as he,
     b as Fe,
     c as Oe,
-    d as Se,
+    d as Qe,
     u as Ye,
     e as Ce,
     f as Ge,
     g as je,
-    h as ul,
-    t as cl,
-    i as he,
-    V as Pt,
-    j as dl,
+    h as cl,
+    t as dl,
+    i as _e,
+    V as Ct,
+    j as ml,
     k as le,
-    l as me,
-    n as N,
-    o as ml,
-    p as vl,
-    q as pl,
-    r as yl,
-    s as fl,
-    v as hl,
-    w as _l,
-    x as gl
-} from "./forwardRefs-70e877d2.js";
+    l as ve,
+    n as E,
+    o as vl,
+    p as pl,
+    q as yl,
+    r as fl,
+    s as hl,
+    v as _l,
+    w as gl,
+    x as bl
+} from "./forwardRefs-7be90dc2.js";
 import {
-    m as Ke,
-    u as Xe,
-    a as bl,
-    b as kl,
-    c as wl
-} from "./layout-bdc1c8bd.js";
+    m as Xe,
+    u as Ke,
+    a as kl,
+    b as wl,
+    c as Pl
+} from "./layout-42b7d22e.js";
 import {
     M as Ze,
-    V as Ct,
-    i as ne,
-    a as ue,
-    _ as Pl,
-    g as mt
-} from "./VBadge-76d9c3a5.js";
+    V as Vt,
+    i as re,
+    a as ce,
+    _ as Cl,
+    g as vt
+} from "./VBadge-84e3406b.js";
 import {
     e as Ve,
-    g as Cl,
-    a as Vl
-} from "./contextmenu-c4231154.js";
+    g as Vl,
+    a as $l
+} from "./contextmenu-521b5304.js";
 import {
     V as Je,
-    a as Vt
-} from "./VToolbar-4ad3b045.js";
+    a as $t
+} from "./VToolbar-b7f10b15.js";
 import {
     V as Ee,
-    a as $l
-} from "./VCardText-00c669eb.js";
-import {
-    V as Qe,
     a as Il
-} from "./VCard-bfc4071a.js";
+} from "./VCardText-6774ea5e.js";
+import {
+    V as Se,
+    a as xl
+} from "./VCard-b98fe47e.js";
 import {
     V as et
-} from "./VDialog-82ed2e80.js";
+} from "./VDialog-d7e50927.js";
 import {
-    V as xl
-} from "./VSelect-ea96d901.js";
+    V as Ql
+} from "./VSelect-d10e917f.js";
 import {
     V as Sl,
-    a as Ql
-} from "./VTabs-4c128c89.js";
+    a as Tl
+} from "./VTabs-8ad24bfd.js";
 import {
-    V as $t,
-    a as Tl,
-    b as Bl,
-    c as Ml,
-    d as zl
-} from "./VExpansionPanel-9f82eed8.js";
+    V as It,
+    a as Bl,
+    b as Ml,
+    c as zl,
+    d as Dl
+} from "./VExpansionPanel-58c5fe02.js";
 import {
-    V as Dl
-} from "./VInput-91b2e758.js"; /* empty css              */
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
-import "./VSlideGroup-5dd0c6f2.js";
-const Nl = "" + new URL("logo-9391b78c.svg", import.meta.url).href;
+    V as Nl
+} from "./VInput-5b197ccd.js"; /* empty css              */
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
+import "./VSlideGroup-b576aa37.js";
+const El = "" + new URL("logo-9391b78c.svg", import.meta.url).href;
 
-function El(a) {
+function Ll(a) {
     let {
         rootEl: l,
         isSticky: u,
         layoutItemStyles: o
     } = a;
     const i = ae(!1),
         s = ae(0),
-        n = S(() => {
-            const c = typeof i.value == "boolean" ? "top" : i.value;
+        n = x(() => {
+            const y = typeof i.value == "boolean" ? "top" : i.value;
             return [u.value ? {
                 top: "auto",
                 bottom: "auto",
                 height: void 0
             } : void 0, i.value ? {
-                [c]: we(s.value)
+                [y]: Pe(s.value)
             } : {
                 top: o.value.top
             }]
         });
-    re(() => {
-        W(u, c => {
-            c ? window.addEventListener("scroll", f, {
+    ue(() => {
+        W(u, y => {
+            y ? window.addEventListener("scroll", _, {
                 passive: !0
-            }) : window.removeEventListener("scroll", f)
+            }) : window.removeEventListener("scroll", _)
         }, {
             immediate: !0
         })
-    }), ve(() => {
-        window.removeEventListener("scroll", f)
+    }), pe(() => {
+        window.removeEventListener("scroll", _)
     });
-    let v = 0;
+    let p = 0;
 
-    function f() {
-        const c = v > window.scrollY ? "up" : "down",
-            _ = l.value.getBoundingClientRect(),
-            p = parseFloat(o.value.top ?? 0),
-            m = window.scrollY - Math.max(0, s.value - p),
-            h = _.height + Math.max(s.value, p) - window.scrollY - window.innerHeight,
+    function _() {
+        const y = p > window.scrollY ? "up" : "down",
+            m = l.value.getBoundingClientRect(),
+            c = parseFloat(o.value.top ?? 0),
+            v = window.scrollY - Math.max(0, s.value - c),
+            h = m.height + Math.max(s.value, c) - window.scrollY - window.innerHeight,
             g = parseFloat(getComputedStyle(l.value).getPropertyValue("--v-body-scroll-y")) || 0;
-        _.height < window.innerHeight - p ? (i.value = "top", s.value = p) : c === "up" && i.value === "bottom" || c === "down" && i.value === "top" ? (s.value = window.scrollY + _.top - g, i.value = !0) : c === "down" && h <= 0 ? (s.value = 0, i.value = "bottom") : c === "up" && m <= 0 && (g ? i.value !== "top" && (s.value = -m + g + p, i.value = "top") : (s.value = _.top + m, i.value = "top")), v = window.scrollY
+        m.height < window.innerHeight - c ? (i.value = "top", s.value = c) : y === "up" && i.value === "bottom" || y === "down" && i.value === "top" ? (s.value = window.scrollY + m.top - g, i.value = !0) : y === "down" && h <= 0 ? (s.value = 0, i.value = "bottom") : y === "up" && v <= 0 && (g ? i.value !== "top" && (s.value = -v + g + c, i.value = "top") : (s.value = m.top + v, i.value = "top")), p = window.scrollY
     }
     return {
         isStuck: i,
         stickyStyles: n
     }
 }
-const Ll = 100,
-    Wl = 20;
+const Wl = 100,
+    Rl = 20;
 
-function vt(a) {
+function pt(a) {
     const l = 1.41421356237;
     return (a < 0 ? -1 : 1) * Math.sqrt(Math.abs(a)) * l
 }
 
-function pt(a) {
+function yt(a) {
     if (a.length < 2) return 0;
     if (a.length === 2) return a[1].t === a[0].t ? 0 : (a[1].d - a[0].d) / (a[1].t - a[0].t);
     let l = 0;
     for (let u = a.length - 1; u > 0; u--) {
         if (a[u].t === a[u - 1].t) continue;
-        const o = vt(l),
+        const o = pt(l),
             i = (a[u].d - a[u - 1].d) / (a[u].t - a[u - 1].t);
         l += (i - o) * Math.abs(i), u === a.length - 1 && (l *= .5)
     }
-    return vt(l) * 1e3
+    return pt(l) * 1e3
 }
 
 function Hl() {
     const a = {};
 
     function l(i) {
         Array.from(i.changedTouches).forEach(s => {
-            (a[s.identifier] ?? (a[s.identifier] = new Wt(Wl))).push([i.timeStamp, s])
+            (a[s.identifier] ?? (a[s.identifier] = new Rt(Rl))).push([i.timeStamp, s])
         })
     }
 
     function u(i) {
         Array.from(i.changedTouches).forEach(s => {
             delete a[s.identifier]
         })
     }
 
     function o(i) {
-        var c;
-        const s = (c = a[i]) == null ? void 0 : c.values().reverse();
+        var y;
+        const s = (y = a[i]) == null ? void 0 : y.values().reverse();
         if (!s) throw new Error(`No samples for touch id ${i}`);
         const n = s[0],
-            v = [],
-            f = [];
-        for (const _ of s) {
-            if (n[0] - _[0] > Ll) break;
-            v.push({
-                t: _[0],
-                d: _[1].clientX
-            }), f.push({
-                t: _[0],
-                d: _[1].clientY
+            p = [],
+            _ = [];
+        for (const m of s) {
+            if (n[0] - m[0] > Wl) break;
+            p.push({
+                t: m[0],
+                d: m[1].clientX
+            }), _.push({
+                t: m[0],
+                d: m[1].clientY
             })
         }
         return {
-            x: pt(v),
-            y: pt(f),
+            x: yt(p),
+            y: yt(_),
             get direction() {
                 const {
-                    x: _,
-                    y: p
-                } = this, [m, h] = [Math.abs(_), Math.abs(p)];
-                return m > h && _ >= 0 ? "right" : m > h && _ <= 0 ? "left" : h > m && p >= 0 ? "down" : h > m && p <= 0 ? "up" : Rl()
+                    x: m,
+                    y: c
+                } = this, [v, h] = [Math.abs(m), Math.abs(c)];
+                return v > h && m >= 0 ? "right" : v > h && m <= 0 ? "left" : h > v && c >= 0 ? "down" : h > v && c <= 0 ? "up" : Al()
             }
         }
     }
     return {
         addMovement: l,
         endTouch: u,
         getVelocity: o
     }
 }
 
-function Rl() {
+function Al() {
     throw new Error
 }
 
-function Al(a) {
+function ql(a) {
     let {
         isActive: l,
         isTemporary: u,
         width: o,
         touchless: i,
         position: s
     } = a;
-    re(() => {
-        window.addEventListener("touchstart", B, {
+    ue(() => {
+        window.addEventListener("touchstart", z, {
             passive: !0
         }), window.addEventListener("touchmove", F, {
             passive: !1
         }), window.addEventListener("touchend", O, {
             passive: !0
         })
-    }), ve(() => {
-        window.removeEventListener("touchstart", B), window.removeEventListener("touchmove", F), window.removeEventListener("touchend", O)
+    }), pe(() => {
+        window.removeEventListener("touchstart", z), window.removeEventListener("touchmove", F), window.removeEventListener("touchend", O)
     });
-    const n = S(() => ["left", "right"].includes(s.value)),
+    const n = x(() => ["left", "right"].includes(s.value)),
         {
-            addMovement: v,
-            endTouch: f,
-            getVelocity: c
+            addMovement: p,
+            endTouch: _,
+            getVelocity: y
         } = Hl();
-    let _ = !1;
-    const p = ae(!1),
-        m = ae(0),
+    let m = !1;
+    const c = ae(!1),
+        v = ae(0),
         h = ae(0);
     let g;
 
-    function P(Q, x) {
-        return (s.value === "left" ? Q : s.value === "right" ? document.documentElement.clientWidth - Q : s.value === "top" ? Q : s.value === "bottom" ? document.documentElement.clientHeight - Q : se()) - (x ? o.value : 0)
+    function C(T, Q) {
+        return (s.value === "left" ? T : s.value === "right" ? document.documentElement.clientWidth - T : s.value === "top" ? T : s.value === "bottom" ? document.documentElement.clientHeight - T : se()) - (Q ? o.value : 0)
     }
 
-    function D(Q) {
-        let x = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0;
-        const z = s.value === "left" ? (Q - h.value) / o.value : s.value === "right" ? (document.documentElement.clientWidth - Q - h.value) / o.value : s.value === "top" ? (Q - h.value) / o.value : s.value === "bottom" ? (document.documentElement.clientHeight - Q - h.value) / o.value : se();
-        return x ? Math.max(0, Math.min(1, z)) : z
+    function N(T) {
+        let Q = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0;
+        const B = s.value === "left" ? (T - h.value) / o.value : s.value === "right" ? (document.documentElement.clientWidth - T - h.value) / o.value : s.value === "top" ? (T - h.value) / o.value : s.value === "bottom" ? (document.documentElement.clientHeight - T - h.value) / o.value : se();
+        return Q ? Math.max(0, Math.min(1, B)) : B
     }
 
-    function B(Q) {
+    function z(T) {
         if (i.value) return;
-        const x = Q.changedTouches[0].clientX,
-            z = Q.changedTouches[0].clientY,
-            E = 25,
-            G = s.value === "left" ? x < E : s.value === "right" ? x > document.documentElement.clientWidth - E : s.value === "top" ? z < E : s.value === "bottom" ? z > document.documentElement.clientHeight - E : se(),
-            J = l.value && (s.value === "left" ? x < o.value : s.value === "right" ? x > document.documentElement.clientWidth - o.value : s.value === "top" ? z < o.value : s.value === "bottom" ? z > document.documentElement.clientHeight - o.value : se());
-        (G || J || l.value && u.value) && (_ = !0, g = [x, z], h.value = P(n.value ? x : z, l.value), m.value = D(n.value ? x : z), f(Q), v(Q))
+        const Q = T.changedTouches[0].clientX,
+            B = T.changedTouches[0].clientY,
+            M = 25,
+            j = s.value === "left" ? Q < M : s.value === "right" ? Q > document.documentElement.clientWidth - M : s.value === "top" ? B < M : s.value === "bottom" ? B > document.documentElement.clientHeight - M : se(),
+            ee = l.value && (s.value === "left" ? Q < o.value : s.value === "right" ? Q > document.documentElement.clientWidth - o.value : s.value === "top" ? B < o.value : s.value === "bottom" ? B > document.documentElement.clientHeight - o.value : se());
+        (j || ee || l.value && u.value) && (m = !0, g = [Q, B], h.value = C(n.value ? Q : B, l.value), v.value = N(n.value ? Q : B), _(T), p(T))
     }
 
-    function F(Q) {
-        const x = Q.changedTouches[0].clientX,
-            z = Q.changedTouches[0].clientY;
-        if (_) {
-            if (!Q.cancelable) {
-                _ = !1;
+    function F(T) {
+        const Q = T.changedTouches[0].clientX,
+            B = T.changedTouches[0].clientY;
+        if (m) {
+            if (!T.cancelable) {
+                m = !1;
                 return
             }
-            const G = Math.abs(x - g[0]),
-                J = Math.abs(z - g[1]);
-            (n.value ? G > J && G > 3 : J > G && J > 3) ? (p.value = !0, _ = !1) : (n.value ? J : G) > 3 && (_ = !1)
-        }
-        if (!p.value) return;
-        Q.preventDefault(), v(Q);
-        const E = D(n.value ? x : z, !1);
-        m.value = Math.max(0, Math.min(1, E)), E > 1 ? h.value = P(n.value ? x : z, !0) : E < 0 && (h.value = P(n.value ? x : z, !1))
+            const j = Math.abs(Q - g[0]),
+                ee = Math.abs(B - g[1]);
+            (n.value ? j > ee && j > 3 : ee > j && ee > 3) ? (c.value = !0, m = !1) : (n.value ? ee : j) > 3 && (m = !1)
+        }
+        if (!c.value) return;
+        T.preventDefault(), p(T);
+        const M = N(n.value ? Q : B, !1);
+        v.value = Math.max(0, Math.min(1, M)), M > 1 ? h.value = C(n.value ? Q : B, !0) : M < 0 && (h.value = C(n.value ? Q : B, !1))
     }
 
-    function O(Q) {
-        if (_ = !1, !p.value) return;
-        v(Q), p.value = !1;
-        const x = c(Q.changedTouches[0].identifier),
-            z = Math.abs(x.x),
-            E = Math.abs(x.y);
-        (n.value ? z > E && z > 400 : E > z && E > 3) ? l.value = x.direction === ({
+    function O(T) {
+        if (m = !1, !c.value) return;
+        p(T), c.value = !1;
+        const Q = y(T.changedTouches[0].identifier),
+            B = Math.abs(Q.x),
+            M = Math.abs(Q.y);
+        (n.value ? B > M && B > 400 : M > B && M > 3) ? l.value = Q.direction === ({
             left: "right",
             right: "left",
             top: "down",
             bottom: "up"
-        } [s.value] || se()): l.value = m.value > .5
+        } [s.value] || se()): l.value = v.value > .5
     }
-    const Z = S(() => p.value ? {
-        transform: s.value === "left" ? `translateX(calc(-100% + ${m.value*o.value}px))` : s.value === "right" ? `translateX(calc(100% - ${m.value*o.value}px))` : s.value === "top" ? `translateY(calc(-100% + ${m.value*o.value}px))` : s.value === "bottom" ? `translateY(calc(100% - ${m.value*o.value}px))` : se(),
+    const J = x(() => c.value ? {
+        transform: s.value === "left" ? `translateX(calc(-100% + ${v.value*o.value}px))` : s.value === "right" ? `translateX(calc(100% - ${v.value*o.value}px))` : s.value === "top" ? `translateY(calc(-100% + ${v.value*o.value}px))` : s.value === "bottom" ? `translateY(calc(100% - ${v.value*o.value}px))` : se(),
         transition: "none"
     } : void 0);
     return {
-        isDragging: p,
-        dragProgress: m,
-        dragStyles: Z
+        isDragging: c,
+        dragProgress: v,
+        dragStyles: J
     }
 }
 
 function se() {
     throw new Error
 }
-const ql = ["start", "end", "left", "right", "top", "bottom"],
-    Ul = pe({
+const Ul = ["start", "end", "left", "right", "top", "bottom"],
+    Fl = ye({
         color: String,
         disableResizeWatcher: Boolean,
         disableRouteWatcher: Boolean,
         expandOnHover: Boolean,
         floating: Boolean,
         modelValue: {
             type: Boolean,
@@ -424,187 +424,187 @@
         width: {
             type: [Number, String],
             default: 256
         },
         location: {
             type: String,
             default: "start",
-            validator: a => ql.includes(a)
+            validator: a => Ul.includes(a)
         },
         sticky: Boolean,
         ...Ue(),
-        ...fe(),
+        ...he(),
         ...Ht(),
         ...Fe(),
-        ...Ke(),
+        ...Xe(),
         ...Oe(),
-        ...Se({
+        ...Qe({
             tag: "nav"
         }),
         ...Ie()
     }, "VNavigationDrawer"),
-    It = ye()({
+    xt = fe()({
         name: "VNavigationDrawer",
-        props: Ul(),
+        props: Fl(),
         emits: {
             "update:modelValue": a => !0,
             "update:rail": a => !0
         },
         setup(a, l) {
             let {
                 attrs: u,
                 emit: o,
                 slots: i
             } = l;
             const {
                 isRtl: s
-            } = yt(), {
+            } = ft(), {
                 themeClasses: n
-            } = Re(a), {
-                borderClasses: v
+            } = He(a), {
+                borderClasses: p
             } = Ye(a), {
-                backgroundColorClasses: f,
-                backgroundColorStyles: c
-            } = Ce(X(a, "color")), {
-                elevationClasses: _
+                backgroundColorClasses: _,
+                backgroundColorStyles: y
+            } = Ce(K(a, "color")), {
+                elevationClasses: m
             } = Ge(a), {
-                displayClasses: p,
-                mobile: m
-            } = Rt(a), {
+                displayClasses: c,
+                mobile: v
+            } = At(a), {
                 roundedClasses: h
-            } = je(a), g = ul(), P = At(a, "modelValue", null, A => !!A), {
-                ssrBootStyles: D
+            } = je(a), g = cl(), C = qt(a, "modelValue", null, A => !!A), {
+                ssrBootStyles: N
             } = qe(), {
-                scopeId: B
-            } = sl(), F = T(), O = ae(!1), Z = S(() => a.rail && a.expandOnHover && O.value ? Number(a.width) : Number(a.rail ? a.railWidth : a.width)), Q = S(() => cl(a.location, s.value)), x = S(() => !a.permanent && (m.value || a.temporary)), z = S(() => a.sticky && !x.value && Q.value !== "bottom");
+                scopeId: z
+            } = nl(), F = S(), O = ae(!1), J = x(() => a.rail && a.expandOnHover && O.value ? Number(a.width) : Number(a.rail ? a.railWidth : a.width)), T = x(() => dl(a.location, s.value)), Q = x(() => !a.permanent && (v.value || a.temporary)), B = x(() => a.sticky && !Q.value && T.value !== "bottom");
             Te(() => a.expandOnHover && a.rail != null, () => {
                 W(O, A => o("update:rail", !A))
             }), Te(() => !a.disableResizeWatcher, () => {
-                W(x, A => !a.permanent && Ut(() => P.value = !A))
+                W(Q, A => !a.permanent && Ft(() => C.value = !A))
             }), Te(() => !a.disableRouteWatcher && !!g, () => {
-                W(g.currentRoute, () => x.value && (P.value = !1))
+                W(g.currentRoute, () => Q.value && (C.value = !1))
             }), W(() => a.permanent, A => {
-                A && (P.value = !0)
-            }), qt(() => {
-                a.modelValue != null || x.value || (P.value = a.permanent || !m.value)
+                A && (C.value = !0)
+            }), Ut(() => {
+                a.modelValue != null || Q.value || (C.value = a.permanent || !v.value)
             });
             const {
-                isDragging: E,
-                dragProgress: G,
-                dragStyles: J
-            } = Al({
-                isActive: P,
-                isTemporary: x,
-                width: Z,
-                touchless: X(a, "touchless"),
-                position: Q
-            }), tt = S(() => {
-                const A = x.value ? 0 : a.rail && a.expandOnHover ? Number(a.railWidth) : Z.value;
-                return E.value ? A * G.value : A
+                isDragging: M,
+                dragProgress: j,
+                dragStyles: ee
+            } = ql({
+                isActive: C,
+                isTemporary: Q,
+                width: J,
+                touchless: K(a, "touchless"),
+                position: T
+            }), lt = x(() => {
+                const A = Q.value ? 0 : a.rail && a.expandOnHover ? Number(a.railWidth) : J.value;
+                return M.value ? A * j.value : A
             }), {
-                layoutItemStyles: lt,
-                layoutItemScrimStyles: zt
-            } = Xe({
+                layoutItemStyles: at,
+                layoutItemScrimStyles: Dt
+            } = Ke({
                 id: a.name,
-                order: S(() => parseInt(a.order, 10)),
-                position: Q,
-                layoutSize: tt,
-                elementSize: Z,
-                active: S(() => P.value || E.value),
-                disableTransitions: S(() => E.value),
-                absolute: S(() => a.absolute || z.value && typeof at.value != "string")
+                order: x(() => parseInt(a.order, 10)),
+                position: T,
+                layoutSize: lt,
+                elementSize: J,
+                active: x(() => C.value || M.value),
+                disableTransitions: x(() => M.value),
+                absolute: x(() => a.absolute || B.value && typeof ot.value != "string")
             }), {
-                isStuck: at,
-                stickyStyles: Dt
-            } = El({
+                isStuck: ot,
+                stickyStyles: Nt
+            } = Ll({
                 rootEl: F,
-                isSticky: z,
-                layoutItemStyles: lt
-            }), ot = Ce(S(() => typeof a.scrim == "string" ? a.scrim : null)), Nt = S(() => ({
-                ...E.value ? {
-                    opacity: G.value * .2,
+                isSticky: B,
+                layoutItemStyles: at
+            }), it = Ce(x(() => typeof a.scrim == "string" ? a.scrim : null)), Et = x(() => ({
+                ...M.value ? {
+                    opacity: j.value * .2,
                     transition: "none"
                 } : void 0,
-                ...zt.value
+                ...Dt.value
             }));
-            ft({
+            ht({
                 VList: {
                     bgColor: "transparent"
                 }
             });
 
-            function Et() {
+            function Lt() {
                 O.value = !0
             }
 
-            function Lt() {
+            function Wt() {
                 O.value = !1
             }
-            return he(() => {
+            return _e(() => {
                 const A = i.image || a.image;
-                return r(R, null, [r(a.tag, H({
+                return r(H, null, [r(a.tag, R({
                     ref: F,
-                    onMouseenter: Et,
-                    onMouseleave: Lt,
-                    class: ["v-navigation-drawer", `v-navigation-drawer--${Q.value}`, {
+                    onMouseenter: Lt,
+                    onMouseleave: Wt,
+                    class: ["v-navigation-drawer", `v-navigation-drawer--${T.value}`, {
                         "v-navigation-drawer--expand-on-hover": a.expandOnHover,
                         "v-navigation-drawer--floating": a.floating,
                         "v-navigation-drawer--is-hovering": O.value,
                         "v-navigation-drawer--rail": a.rail,
-                        "v-navigation-drawer--temporary": x.value,
-                        "v-navigation-drawer--active": P.value,
-                        "v-navigation-drawer--sticky": z.value
-                    }, n.value, f.value, v.value, p.value, _.value, h.value, a.class],
-                    style: [c.value, lt.value, J.value, D.value, Dt.value, a.style]
-                }, B, u), {
+                        "v-navigation-drawer--temporary": Q.value,
+                        "v-navigation-drawer--active": C.value,
+                        "v-navigation-drawer--sticky": B.value
+                    }, n.value, _.value, p.value, c.value, m.value, h.value, a.class],
+                    style: [y.value, at.value, ee.value, N.value, Nt.value, a.style]
+                }, z, u), {
                     default: () => {
-                        var it, st, nt;
+                        var st, nt, rt;
                         return [A && r("div", {
                             key: "image",
                             class: "v-navigation-drawer__img"
-                        }, [i.image ? r(dl, {
+                        }, [i.image ? r(ml, {
                             key: "image-defaults",
                             disabled: !a.image,
                             defaults: {
                                 VImg: {
                                     alt: "",
                                     cover: !0,
                                     height: "inherit",
                                     src: a.image
                                 }
                             }
-                        }, i.image) : r(Pt, {
+                        }, i.image) : r(Ct, {
                             key: "image-img",
                             alt: "",
                             cover: !0,
                             height: "inherit",
                             src: a.image
                         }, null)]), i.prepend && r("div", {
                             class: "v-navigation-drawer__prepend"
-                        }, [(it = i.prepend) == null ? void 0 : it.call(i)]), r("div", {
+                        }, [(st = i.prepend) == null ? void 0 : st.call(i)]), r("div", {
                             class: "v-navigation-drawer__content"
-                        }, [(st = i.default) == null ? void 0 : st.call(i)]), i.append && r("div", {
+                        }, [(nt = i.default) == null ? void 0 : nt.call(i)]), i.append && r("div", {
                             class: "v-navigation-drawer__append"
-                        }, [(nt = i.append) == null ? void 0 : nt.call(i)])]
+                        }, [(rt = i.append) == null ? void 0 : rt.call(i)])]
                     }
-                }), r(ht, {
+                }), r(_t, {
                     name: "fade-transition"
                 }, {
-                    default: () => [x.value && (E.value || P.value) && !!a.scrim && r("div", H({
-                        class: ["v-navigation-drawer__scrim", ot.backgroundColorClasses.value],
-                        style: [Nt.value, ot.backgroundColorStyles.value],
-                        onClick: () => P.value = !1
-                    }, B), null)]
+                    default: () => [Q.value && (M.value || C.value) && !!a.scrim && r("div", R({
+                        class: ["v-navigation-drawer__scrim", it.backgroundColorClasses.value],
+                        style: [Et.value, it.backgroundColorStyles.value],
+                        onClick: () => C.value = !1
+                    }, z), null)]
                 })])
             }), {
-                isStuck: at
+                isStuck: ot
             }
         }
     }),
-    Fl = k("div", {
+    Ol = k("div", {
         class: "logo_text"
     }, "Music Assistant", -1),
     Le = [{
         label: "home",
         icon: "mdi-home-outline",
         path: "/home"
     }, {
@@ -636,55 +636,55 @@
         icon: "mdi-magnify",
         path: "/search"
     }, {
         label: "settings.settings",
         icon: "mdi-cog-outline",
         path: "/settings"
     }],
-    Ol = M({
+    Yl = D({
         __name: "DrawerNavigation",
         setup(a) {
-            const l = T(!1);
+            const l = S(!1);
             return W(() => l.value, u => {
-                u ? t.navigationMenuSize = C("mobile") ? 250 : 200 : t.navigationMenuSize = 55
-            }), (u, o) => e(C)({
+                u ? t.navigationMenuSize = P("mobile") ? 250 : 200 : t.navigationMenuSize = 55
+            }), (u, o) => e(P)({
                 breakpoint: "bp3"
-            }) ? (d(), V(It, {
+            }) ? (d(), V(xt, {
                 key: 0,
                 ref: "resizeComponent",
                 app: "",
                 permanent: !u.$vuetify.display.mobile,
                 rail: !u.$vuetify.display.mobile && !l.value,
                 "model-value": u.$vuetify.display.mobile && l.value || !u.$vuetify.display.mobile,
-                width: e(C)("mobile") ? 250 : 200,
+                width: e(P)("mobile") ? 250 : 200,
                 "onUpdate:modelValue": o[1] || (o[1] = i => {
                     u.$vuetify.display.mobile && (l.value = i)
                 })
             }, {
-                default: y(() => [r(ct, {
+                default: f(() => [r(dt, {
                     dark: "",
                     style: {
                         height: "55px"
                     },
                     active: !1
                 }, {
-                    prepend: y(() => [k("img", {
+                    prepend: f(() => [k("img", {
                         class: "logo_icon",
                         style: L(u.$vuetify.theme.current.dark ? "filter: invert(100%);" : ""),
                         width: "35",
-                        src: Nl
+                        src: El
                     }, null, 4)]),
-                    title: y(() => [Fl]),
+                    title: f(() => [Ol]),
                     _: 1
                 }), r(le), r(ie, {
                     lines: "one",
                     density: "compact",
                     nav: ""
                 }, {
-                    default: y(() => [(d(), b(R, null, U(Le, i => r(ct, {
+                    default: f(() => [(d(), b(H, null, U(Le, i => r(dt, {
                         key: i.path,
                         nav: "",
                         density: "compact",
                         height: 15,
                         title: u.$t(i.label),
                         "prepend-icon": i.icon,
                         to: i.path
@@ -699,268 +699,268 @@
                         float: "right",
                         right: "10px",
                         top: "20px"
                     },
                     ripple: !1,
                     icon: l.value ? "mdi-chevron-left" : "mdi-chevron-right",
                     title: u.$t("tooltip.show_menu"),
-                    onClick: o[0] || (o[0] = Ft(i => l.value = !l.value, ["stop"]))
+                    onClick: o[0] || (o[0] = Ot(i => l.value = !l.value, ["stop"]))
                 }, null, 8, ["icon", "title"])]),
                 _: 1
             }, 8, ["permanent", "rail", "model-value", "width"])) : I("", !0)
         }
     });
-const Yl = {
+const Gl = {
         class: "media-thumb"
     },
-    Gl = k("div", {
+    jl = k("div", {
         style: {
             height: "30px"
         }
     }, null, -1),
-    jl = k("div", {
+    Xl = k("div", {
         style: {
             height: "10px"
         }
     }, null, -1),
     Kl = {
         style: {
             width: "50px",
             height: "50px",
             "flex-flow": "column"
         }
     },
-    Xl = M({
+    Zl = D({
         __name: "AddToPlaylistDialog",
         setup(a) {
-            const l = T(!1),
-                u = T([]),
-                o = T([]),
-                i = T(),
-                s = T([]);
-            re(() => {
-                Ve.on("playlistdialog", async _ => {
-                    await n(), s.value = _.items, i.value = _.parentItem, l.value = !0
-                }), ve(() => {
+            const l = S(!1),
+                u = S([]),
+                o = S([]),
+                i = S(),
+                s = S([]);
+            ue(() => {
+                Ve.on("playlistdialog", async m => {
+                    await n(), s.value = m.items, i.value = m.parentItem, l.value = !0
+                }), pe(() => {
                     Ve.off("playlistdialog")
                 })
             });
             const n = async function() {
                 u.value = [], o.value = [];
-                const _ = await w.getLibraryPlaylists(),
-                    p = s.value.length ? s.value[0] : void 0;
-                for (const m of _.items) {
-                    if (!m.provider_mappings.filter(g => g.available).length || !m.is_editable || i.value && i.value.media_type === te.PLAYLIST && m.item_id === i.value.item_id) continue;
-                    const h = w.providers[m.provider_mappings[0].provider_instance];
-                    h.supported_features.includes(Be.PLAYLIST_TRACKS_EDIT) && (h.domain == "builtin" || p != null && p.provider_mappings.filter(g => g.provider_instance == h.instance_id).length) && u.value.push(m)
+                const m = await w.getLibraryPlaylists(),
+                    c = s.value.length ? s.value[0] : void 0;
+                for (const v of m.items) {
+                    if (!v.provider_mappings.filter(g => g.available).length || !v.is_editable || i.value && i.value.media_type === Z.PLAYLIST && v.item_id === i.value.item_id) continue;
+                    const h = w.providers[v.provider_mappings[0].provider_instance];
+                    h.supported_features.includes(Be.PLAYLIST_TRACKS_EDIT) && (h.domain == "builtin" || c != null && c.provider_mappings.filter(g => g.provider_instance == h.instance_id).length) && u.value.push(v)
                 }
-                for (const m of Object.values(w.providers)) m.supported_features.includes(Be.PLAYLIST_CREATE) && m.supported_features.includes(Be.PLAYLIST_TRACKS_EDIT) && (m.domain == "builtin" || p != null && p.provider_mappings.filter(h => h.provider_instance == m.instance_id).length) && o.value.push(m.instance_id)
-            }, v = function(_) {
-                if (s.value[0].media_type === te.TRACK) w.addPlaylistTracks(_.item_id, s.value.map(m => m.uri));
-                else if (s.value[0].media_type === te.ALBUM) {
-                    var p = [];
-                    w.getAlbumTracks(s.value[0].item_id, s.value[0].provider).then(m => {
-                        p = m, w.addPlaylistTracks(_.item_id, p.map(h => h.uri))
+                for (const v of Object.values(w.providers)) v.supported_features.includes(Be.PLAYLIST_CREATE) && v.supported_features.includes(Be.PLAYLIST_TRACKS_EDIT) && (v.domain == "builtin" || c != null && c.provider_mappings.filter(h => h.provider_instance == v.instance_id).length) && o.value.push(v.instance_id)
+            }, p = function(m) {
+                if (s.value[0].media_type === Z.TRACK) w.addPlaylistTracks(m.item_id, s.value.map(v => v.uri));
+                else if (s.value[0].media_type === Z.ALBUM) {
+                    var c = [];
+                    w.getAlbumTracks(s.value[0].item_id, s.value[0].provider).then(v => {
+                        c = v, w.addPlaylistTracks(m.item_id, c.map(h => h.uri))
                     })
                 }
-                c()
-            }, f = async function(_) {
-                const p = prompt(_e("new_playlist_name"));
-                if (!p) return;
-                const m = await w.createPlaylist(p, _);
-                v(m)
-            }, c = function() {
+                y()
+            }, _ = async function(m) {
+                const c = prompt(ge("new_playlist_name"));
+                if (!c) return;
+                const v = await w.createPlaylist(c, m);
+                p(v)
+            }, y = function() {
                 l.value = !1
             };
-            return (_, p) => (d(), V(et, {
+            return (m, c) => (d(), V(et, {
                 modelValue: l.value,
-                "onUpdate:modelValue": [p[1] || (p[1] = m => l.value = m), p[2] || (p[2] = m => {
-                    e(t).dialogActive = m
+                "onUpdate:modelValue": [c[1] || (c[1] = v => l.value = v), c[2] || (c[2] = v => {
+                    e(t).dialogActive = v
                 })],
-                fullscreen: _.$vuetify.display.mobile,
+                fullscreen: m.$vuetify.display.mobile,
                 "min-height": "80%",
                 scrim: !0
             }, {
-                default: y(() => [r(Qe, null, {
-                    default: y(() => [r(Je, {
+                default: f(() => [r(Se, null, {
+                    default: f(() => [r(Je, {
                         color: "transparent",
                         style: {
                             padding: "10px 0px"
                         },
                         density: "compact",
                         class: "titlebar"
                     }, {
-                        default: y(() => [r(me, {
+                        default: f(() => [r(ve, {
                             icon: "mdi-play-circle-outline"
-                        }), r(Vt, {
+                        }), r($t, {
                             style: {
                                 "padding-left": "10px"
                             }
                         }, {
-                            default: y(() => [k("b", null, $(e(_e)("add_playlist")), 1)]),
+                            default: f(() => [k("b", null, $(e(ge)("add_playlist")), 1)]),
                             _: 1
-                        }), r(me, {
+                        }), r(ve, {
                             icon: "mdi-close",
                             dark: "",
-                            onClick: p[0] || (p[0] = m => c())
+                            onClick: c[0] || (c[0] = v => y())
                         })]),
                         _: 1
                     }), r(le), r(Ee, null, {
-                        default: y(() => [r(ie, null, {
-                            default: y(() => [(d(!0), b(R, null, U(u.value, m => (d(), b("div", {
-                                key: m.item_id
-                            }, [r(K, {
+                        default: f(() => [r(ie, null, {
+                            default: f(() => [(d(!0), b(H, null, U(u.value, v => (d(), b("div", {
+                                key: v.item_id
+                            }, [r(X, {
                                 ripple: "",
                                 density: "default",
-                                onClick: h => v(m)
+                                onClick: h => p(v)
                             }, {
-                                prepend: y(() => [k("div", Yl, [r(Ze, {
-                                    item: m,
+                                prepend: f(() => [k("div", Gl, [r(Ze, {
+                                    item: v,
                                     size: 50,
                                     width: "50px",
                                     height: "50px"
                                 }, null, 8, ["item"])])]),
-                                title: y(() => [k("div", null, $(m.name), 1)]),
-                                subtitle: y(() => [k("div", null, $(m.owner), 1)]),
-                                append: y(() => [m.provider_mappings ? (d(), V(ze, {
+                                title: f(() => [k("div", null, $(v.name), 1)]),
+                                subtitle: f(() => [k("div", null, $(v.owner), 1)]),
+                                append: f(() => [v.provider_mappings ? (d(), V(ze, {
                                     key: 0,
-                                    domain: m.provider_mappings[0].provider_domain,
+                                    domain: v.provider_mappings[0].provider_domain,
                                     size: 20
                                 }, null, 8, ["domain"])) : I("", !0)]),
                                 _: 2
-                            }, 1032, ["onClick"])]))), 128)), Gl, r(le), jl, (d(!0), b(R, null, U(o.value, m => (d(), b("div", {
-                                key: m
-                            }, [r(K, {
+                            }, 1032, ["onClick"])]))), 128)), jl, r(le), Xl, (d(!0), b(H, null, U(o.value, v => (d(), b("div", {
+                                key: v
+                            }, [r(X, {
                                 ripple: "",
-                                onClick: h => f(m)
+                                onClick: h => _(v)
                             }, {
-                                prepend: y(() => [k("div", Kl, [r(ze, {
-                                    domain: e(w).providers[m].domain,
+                                prepend: f(() => [k("div", Kl, [r(ze, {
+                                    domain: e(w).providers[v].domain,
                                     size: 45,
                                     class: "media-thumb"
                                 }, null, 8, ["domain"])])]),
-                                title: y(() => [k("div", null, $(e(_e)("new_playlist")), 1)]),
-                                subtitle: y(() => [k("div", null, $(e(_e)("create_playlist_on", [e(w).providers[m].name])), 1)]),
-                                append: y(() => [r(ze, {
-                                    domain: e(w).providers[m].domain,
+                                title: f(() => [k("div", null, $(e(ge)("new_playlist")), 1)]),
+                                subtitle: f(() => [k("div", null, $(e(ge)("create_playlist_on", [e(w).providers[v].name])), 1)]),
+                                append: f(() => [r(ze, {
+                                    domain: e(w).providers[v].domain,
                                     size: 20
                                 }, null, 8, ["domain"])]),
                                 _: 2
                             }, 1032, ["onClick"])]))), 128))]),
                             _: 1
                         })]),
                         _: 1
                     })]),
                     _: 1
                 })]),
                 _: 1
             }, 8, ["modelValue", "fullscreen"]))
         }
     });
-const Zl = {
+const Jl = {
         class: "font-weight-bold"
     },
-    Jl = M({
+    ea = D({
         __name: "PlayItemDialog",
         setup(a) {
             const {
                 t: l
-            } = Ot(), u = T(!1), o = T(), i = T([]), s = T(!1), n = T([]), v = T([]), f = T("");
-            re(() => {
+            } = Yt(), u = S(!1), o = S(), i = S([]), s = S(!1), n = S([]), p = S([]), _ = S("");
+            ue(() => {
                 Ve.on("playdialog", async h => {
-                    i.value = h.items, o.value = h.parentItem, s.value = h.showContextMenuItems || !1, c()
-                }), ve(() => {
+                    i.value = h.items, o.value = h.parentItem, s.value = h.showContextMenuItems || !1, y()
+                }), pe(() => {
                     Ve.off("playdialog")
                 })
             });
-            const c = async function() {
+            const y = async function() {
                 if (u.value = !0, !i.value) return;
-                i.value.length === 1 ? f.value = i.value[0].name : f.value = l("items_selected", [i.value.length]).toString(), t.selectedPlayer && t.selectedPlayer.available ? v.value = Cl(i.value, o.value) : v.value = [];
+                i.value.length === 1 ? _.value = i.value[0].name : _.value = l("items_selected", [i.value.length]).toString(), t.selectedPlayer && t.selectedPlayer.available ? p.value = Vl(i.value, o.value) : p.value = [];
                 let h = i.value[0];
                 if ("position" in h && h.position, h.provider !== "library") try {
                     h = await w.getItemByUri(i.value[0].uri)
                 } catch {
                     h = i.value[0]
                 }
-                s.value ? n.value = Vl(i.value, o.value) : n.value = []
-            }, _ = async function(h) {
-                p(), h.action && h.action()
-            }, p = function() {
+                s.value ? n.value = $l(i.value, o.value) : n.value = []
+            }, m = async function(h) {
+                c(), h.action && h.action()
+            }, c = function() {
                 u.value = !1
-            }, m = S(() => {
-                var g, P;
+            }, v = x(() => {
+                var g, C;
                 const h = [];
-                for (const D in (g = w) == null ? void 0 : g.players) {
-                    const B = (P = w) == null ? void 0 : P.players[D];
-                    B.synced_to || h.push({
-                        title: B.display_name,
-                        value: B.player_id
+                for (const N in (g = w) == null ? void 0 : g.players) {
+                    const z = (C = w) == null ? void 0 : C.players[N];
+                    z.synced_to || h.push({
+                        title: z.display_name,
+                        value: z.player_id
                     })
                 }
-                return h.slice().sort((D, B) => D.title.toUpperCase() > B.title.toUpperCase() ? 1 : -1)
+                return h.slice().sort((N, z) => N.title.toUpperCase() > z.title.toUpperCase() ? 1 : -1)
             });
             return (h, g) => (d(), V(et, {
                 modelValue: u.value,
-                "onUpdate:modelValue": [g[2] || (g[2] = P => u.value = P), g[3] || (g[3] = P => {
-                    e(t).dialogActive = P
+                "onUpdate:modelValue": [g[2] || (g[2] = C => u.value = C), g[3] || (g[3] = C => {
+                    e(t).dialogActive = C
                 })],
                 fullscreen: h.$vuetify.display.mobile,
                 transition: "dialog-bottom-transition",
                 scrim: !0
             }, {
-                default: y(() => [r(Qe, null, {
-                    default: y(() => [r(Je, {
+                default: f(() => [r(Se, null, {
+                    default: f(() => [r(Je, {
                         color: "transparent",
                         density: "compact",
                         class: "titlebar"
                     }, {
-                        prepend: y(() => [r(N, {
+                        prepend: f(() => [r(E, {
                             size: "large",
                             class: "ml-4 d-none d-sm-block",
                             style: {
                                 "vertical-align": "initial"
                             },
                             icon: "mdi-play-circle-outline",
                             "aria-hidden": "true"
                         })]),
-                        default: y(() => [r(Vt, null, {
-                            default: y(() => [k("h2", Zl, $(f.value), 1)]),
+                        default: f(() => [r($t, null, {
+                            default: f(() => [k("h2", Jl, $(_.value), 1)]),
                             _: 1
-                        }), r(me, {
+                        }), r(ve, {
                             icon: "mdi-close",
                             dark: "",
-                            onClick: g[0] || (g[0] = P => p())
+                            onClick: g[0] || (g[0] = C => c())
                         })]),
                         _: 1
-                    }), r(le), v.value.length > 0 ? (d(), V(Ee, {
+                    }), r(le), p.value.length > 0 ? (d(), V(Ee, {
                         key: 0
                     }, {
-                        default: y(() => [r(xl, {
+                        default: f(() => [r(Ql, {
                             label: h.$t("play_on"),
                             "model-value": e(t).selectedPlayerId,
-                            items: m.value,
+                            items: v.value,
                             "hide-details": "",
-                            "onUpdate:modelValue": g[1] || (g[1] = P => {
-                                e(t).selectedPlayerId = P
+                            "onUpdate:modelValue": g[1] || (g[1] = C => {
+                                e(t).selectedPlayerId = C
                             })
                         }, null, 8, ["label", "model-value", "items"]), r(ie, null, {
-                            default: y(() => [(d(!0), b(R, null, U(v.value, P => (d(), b("div", {
-                                key: P.label
-                            }, [r(K, {
-                                title: h.$t(P.label, P.labelArgs),
+                            default: f(() => [(d(!0), b(H, null, U(p.value, C => (d(), b("div", {
+                                key: C.label
+                            }, [r(X, {
+                                title: h.$t(C.label, C.labelArgs),
                                 density: "default",
-                                onClick: D => _(P)
+                                onClick: N => m(C)
                             }, {
-                                prepend: y(() => [r(dt, {
+                                prepend: f(() => [r(mt, {
                                     style: {
                                         "padding-right": "10px"
                                     }
                                 }, {
-                                    default: y(() => [r(N, {
-                                        icon: P.icon
+                                    default: f(() => [r(E, {
+                                        icon: C.icon
                                     }, null, 8, ["icon"])]),
                                     _: 2
                                 }, 1024)]),
                                 _: 2
                             }, 1032, ["title", "onClick"])]))), 128))]),
                             _: 1
                         })]),
@@ -969,36 +969,36 @@
                         key: 1,
                         style: {
                             "padding-top": "0",
                             "margin-top": "-10px",
                             "padding-bottom": "0"
                         }
                     }, {
-                        default: y(() => [r(nl, {
+                        default: f(() => [r(rl, {
                             style: {
                                 "margin-left": "10px"
                             }
                         }, {
-                            default: y(() => [j($(h.$t("actions")), 1)]),
+                            default: f(() => [G($(h.$t("actions")), 1)]),
                             _: 1
                         }), r(ie, null, {
-                            default: y(() => [(d(!0), b(R, null, U(n.value, P => (d(), b("div", {
-                                key: P.label
-                            }, [r(K, {
-                                title: h.$t(P.label, P.labelArgs),
+                            default: f(() => [(d(!0), b(H, null, U(n.value, C => (d(), b("div", {
+                                key: C.label
+                            }, [r(X, {
+                                title: h.$t(C.label, C.labelArgs),
                                 density: "default",
-                                onClick: D => _(P)
+                                onClick: N => m(C)
                             }, {
-                                prepend: y(() => [r(dt, {
+                                prepend: f(() => [r(mt, {
                                     style: {
                                         "padding-right": "10px"
                                     }
                                 }, {
-                                    default: y(() => [r(N, {
-                                        icon: P.icon
+                                    default: f(() => [r(E, {
+                                        icon: C.icon
                                     }, null, 8, ["icon"])]),
                                     _: 2
                                 }, 1024)]),
                                 _: 2
                             }, 1032, ["title", "onClick"])]))), 128))]),
                             _: 1
                         })]),
@@ -1006,80 +1006,80 @@
                     })) : I("", !0)]),
                     _: 1
                 })]),
                 _: 1
             }, 8, ["modelValue", "fullscreen"]))
         }
     });
-const ea = pe({
+const ta = ye({
         scrollable: Boolean,
-        ...fe(),
-        ...Se({
+        ...he(),
+        ...Qe({
             tag: "main"
         })
     }, "VMain"),
-    ta = ye()({
+    la = fe()({
         name: "VMain",
-        props: ea(),
+        props: ta(),
         setup(a, l) {
             let {
                 slots: u
             } = l;
             const {
                 mainStyles: o
-            } = bl(), {
+            } = kl(), {
                 ssrBootStyles: i
             } = qe();
-            return he(() => r(a.tag, {
+            return _e(() => r(a.tag, {
                 class: ["v-main", {
                     "v-main--scrollable": a.scrollable
                 }, a.class],
                 style: [o.value, i.value, a.style]
             }, {
                 default: () => {
                     var s, n;
                     return [a.scrollable ? r("div", {
                         class: "v-main__scroller"
                     }, [(s = u.default) == null ? void 0 : s.call(u)]) : (n = u.default) == null ? void 0 : n.call(u)]
                 }
             })), {}
         }
     }),
-    la = M({
+    aa = D({
         __name: "View",
         setup(a) {
             return (l, u) => {
-                const o = Yt("router-view");
-                return d(), V(ta, {
+                const o = Gt("router-view");
+                return d(), V(la, {
                     id: "cont",
                     class: "overflow-y-auto",
                     style: {
                         height: "0px"
                     }
                 }, {
-                    default: y(() => [r(Ol), r(Xl), r(Jl), r(o, {
+                    default: f(() => [r(Yl), r(Zl), r(ea), r(o, {
                         app: ""
                     }, {
-                        default: y(({
+                        default: f(({
                             Component: i
-                        }) => [r(ht, {
+                        }) => [r(_t, {
                             name: "fade",
                             mode: "out-in"
                         }, {
-                            default: y(() => [(d(), V(Gt(i)))]),
+                            default: f(() => [(d(), V(jt(i)))]),
                             _: 2
                         }, 1024)]),
                         _: 1
                     })]),
                     _: 1
                 })
             }
         }
     });
-const aa = pe({
+const oa = ye({
         bgColor: String,
         color: String,
         grow: Boolean,
         mode: {
             type: String,
             validator: a => !a || ["horizontal", "shift"].includes(a)
         },
@@ -1088,248 +1088,248 @@
             default: 56
         },
         active: {
             type: Boolean,
             default: !0
         },
         ...Ue(),
-        ...fe(),
-        ...ml(),
+        ...he(),
+        ...vl(),
         ...Fe(),
         ...Oe(),
-        ...Ke({
+        ...Xe({
             name: "bottom-navigation"
         }),
-        ...Se({
+        ...Qe({
             tag: "header"
         }),
-        ...vl({
+        ...pl({
             modelValue: !0,
             selectedClass: "v-btn--selected"
         }),
         ...Ie()
     }, "VBottomNavigation"),
-    oa = ye()({
+    ia = fe()({
         name: "VBottomNavigation",
-        props: aa(),
+        props: oa(),
         emits: {
             "update:modelValue": a => !0
         },
         setup(a, l) {
             let {
                 slots: u
             } = l;
             const {
                 themeClasses: o
-            } = _t(), {
+            } = gt(), {
                 borderClasses: i
             } = Ye(a), {
                 backgroundColorClasses: s,
                 backgroundColorStyles: n
-            } = Ce(X(a, "bgColor")), {
-                densityClasses: v
-            } = pl(a), {
-                elevationClasses: f
+            } = Ce(K(a, "bgColor")), {
+                densityClasses: p
+            } = yl(a), {
+                elevationClasses: _
             } = Ge(a), {
-                roundedClasses: c
+                roundedClasses: y
             } = je(a), {
-                ssrBootStyles: _
-            } = qe(), p = S(() => Number(a.height) - (a.density === "comfortable" ? 8 : 0) - (a.density === "compact" ? 16 : 0)), m = X(a, "active"), {
+                ssrBootStyles: m
+            } = qe(), c = x(() => Number(a.height) - (a.density === "comfortable" ? 8 : 0) - (a.density === "compact" ? 16 : 0)), v = K(a, "active"), {
                 layoutItemStyles: h
-            } = Xe({
+            } = Ke({
                 id: a.name,
-                order: S(() => parseInt(a.order, 10)),
-                position: S(() => "bottom"),
-                layoutSize: S(() => m.value ? p.value : 0),
-                elementSize: p,
-                active: m,
-                absolute: X(a, "absolute")
+                order: x(() => parseInt(a.order, 10)),
+                position: x(() => "bottom"),
+                layoutSize: x(() => v.value ? c.value : 0),
+                elementSize: c,
+                active: v,
+                absolute: K(a, "absolute")
             });
-            return yl(a, fl), ft({
+            return fl(a, hl), ht({
                 VBtn: {
-                    color: X(a, "color"),
-                    density: X(a, "density"),
-                    stacked: S(() => a.mode !== "horizontal"),
+                    color: K(a, "color"),
+                    density: K(a, "density"),
+                    stacked: x(() => a.mode !== "horizontal"),
                     variant: "text"
                 }
             }, {
                 scoped: !0
-            }), he(() => r(a.tag, {
+            }), _e(() => r(a.tag, {
                 class: ["v-bottom-navigation", {
-                    "v-bottom-navigation--active": m.value,
+                    "v-bottom-navigation--active": v.value,
                     "v-bottom-navigation--grow": a.grow,
                     "v-bottom-navigation--shift": a.mode === "shift"
-                }, o.value, s.value, i.value, v.value, f.value, c.value, a.class],
+                }, o.value, s.value, i.value, p.value, _.value, y.value, a.class],
                 style: [n.value, h.value, {
-                    height: we(p.value),
-                    transform: `translateY(${we(m.value?0:100,"%")})`
-                }, _.value, a.style]
+                    height: Pe(c.value),
+                    transform: `translateY(${Pe(v.value?0:100,"%")})`
+                }, m.value, a.style]
             }, {
                 default: () => [u.default && r("div", {
                     class: "v-bottom-navigation__content"
                 }, [u.default()])]
             })), {}
         }
     }),
-    ia = {
+    sa = {
         class: "menuButton"
     },
-    sa = M({
+    na = D({
         __name: "BottomNavigation",
         props: {
             height: {}
         },
         setup(a) {
-            const l = S(() => {
+            const l = x(() => {
                 for (const u of Le)
-                    if (Pe.currentRoute.value.path.startsWith(u.path)) return u.path;
+                    if (ne.currentRoute.value.path.startsWith(u.path)) return u.path;
                 return ""
             });
-            return (u, o) => (d(), V(oa, {
+            return (u, o) => (d(), V(ia, {
                 height: "80",
                 grow: ""
             }, {
-                default: y(() => [r(Sl, {
+                default: f(() => [r(Sl, {
                     stacked: "",
                     "show-arrows": !1,
                     "model-value": l.value,
                     "center-active": "",
                     nav: "",
                     color: "accent"
                 }, {
-                    default: y(() => [(d(!0), b(R, null, U(e(Le), i => (d(), V(Ql, {
+                    default: f(() => [(d(!0), b(H, null, U(e(Le), i => (d(), V(Tl, {
                         key: i.path,
                         to: i.path,
                         value: i.path
                     }, {
-                        default: y(() => [r(N, {
+                        default: f(() => [r(E, {
                             size: "xx-large"
                         }, {
-                            default: y(() => [j($(i.icon), 1)]),
+                            default: f(() => [G($(i.icon), 1)]),
                             _: 2
-                        }, 1024), k("span", ia, $(u.$t(i.label)), 1)]),
+                        }, 1024), k("span", sa, $(u.$t(i.label)), 1)]),
                         _: 2
                     }, 1032, ["to", "value"]))), 128))]),
                     _: 1
                 }, 8, ["model-value"])]),
                 _: 1
             }))
         }
     });
-const na = {
+const ra = {
         style: {
             width: "100%"
         }
     },
-    ra = {
+    ua = {
         key: 0,
         style: {
             display: "flex",
             flex: "1 1 auto",
             "align-items": "center"
         }
     },
-    ua = {
+    ca = {
         style: {
             "z-index": "1"
         },
         class: "text-caption"
     },
-    ca = {
+    da = {
         key: 1,
         style: {
             width: "100%",
             "padding-bottom": "0px"
         }
     },
-    We = M({
+    We = D({
         __name: "PlayerTimeline",
         props: {
             isProgressBar: {
                 type: Boolean,
                 default: !1
             },
             color: {
                 default: "accent"
             }
         },
         setup(a) {
             const l = a,
-                u = T(!1),
-                o = T(!0),
-                i = T(!1),
-                s = T(0),
-                n = T(0),
-                v = S(() => t.curQueueItem ? u.value ? `-${Me(t.curQueueItem.duration-c.value)}` : `${Me(c.value)}` : "0:00"),
-                f = S(() => {
+                u = S(!1),
+                o = S(!0),
+                i = S(!1),
+                s = S(0),
+                n = S(0),
+                p = x(() => t.curQueueItem ? u.value ? `-${Me(t.curQueueItem.duration-y.value)}` : `${Me(y.value)}` : "0:00"),
+                _ = x(() => {
                     if (!t.curQueueItem) return "0:00";
                     const h = t.curQueueItem.duration;
                     return Me(h)
                 }),
-                c = S(() => i.value ? (n.value = s.value, s.value) : t.activePlayerQueue ? t.activePlayerQueue.elapsed_time : 0);
-            W(c, h => {
+                y = x(() => i.value ? (n.value = s.value, s.value) : t.activePlayerQueue ? t.activePlayerQueue.elapsed_time : 0);
+            W(y, h => {
                 i.value || (s.value = h)
             });
-            const _ = function() {
+            const m = function() {
                     i.value = !0
                 },
-                p = () => {
-                    i.value = !1, m(n.value)
+                c = () => {
+                    i.value = !1, v(n.value)
                 },
-                m = h => {
+                v = h => {
                     var g;
                     i.value || w.queueCommandSeek(((g = t.activePlayerQueue) == null ? void 0 : g.queue_id) || "", Math.round(h))
                 };
             return (h, g) => {
-                var P, D;
-                return d(), b("div", na, [e(t).activePlayerQueue && !h.isProgressBar ? (d(), b("div", ra, [k("div", {
+                var C, N;
+                return d(), b("div", ra, [e(t).activePlayerQueue && !h.isProgressBar ? (d(), b("div", ua, [k("div", {
                     class: "text-caption",
                     style: {
                         cursor: "pointer",
                         "z-index": "1"
                     },
-                    onClick: g[0] || (g[0] = B => u.value ? u.value = !1 : u.value = !0)
-                }, $(v.value), 1), r($t, {
+                    onClick: g[0] || (g[0] = z => u.value ? u.value = !1 : u.value = !0)
+                }, $(p.value), 1), r(It, {
                     modelValue: s.value,
-                    "onUpdate:modelValue": g[1] || (g[1] = B => s.value = B),
-                    disabled: !e(t).curQueueItem || ((P = e(t).curQueueItem.media_item) == null ? void 0 : P.media_type) != e(te).TRACK,
+                    "onUpdate:modelValue": g[1] || (g[1] = z => s.value = z),
+                    disabled: !e(t).curQueueItem || ((C = e(t).curQueueItem.media_item) == null ? void 0 : C.media_type) != e(Z).TRACK,
                     color: l.color,
                     style: {
                         width: "100%"
                     },
                     min: 0,
                     max: e(t).curQueueItem && e(t).curQueueItem.duration,
                     "hide-details": "",
                     "track-size": 2,
                     "thumb-size": o.value ? 0 : 10,
-                    onTouchstart: g[2] || (g[2] = B => o.value = !1),
-                    onTouchend: g[3] || (g[3] = B => o.value = !0),
-                    onMouseenter: g[4] || (g[4] = B => o.value = !1),
-                    onMouseleave: g[5] || (g[5] = B => o.value = !0),
-                    onMousedown: _,
-                    onMouseup: p
-                }, null, 8, ["modelValue", "disabled", "color", "max", "thumb-size"]), k("div", ua, $(f.value), 1)])) : e(t).activePlayerQueue && h.isProgressBar ? (d(), b("div", ca, [r(hl, {
+                    onTouchstart: g[2] || (g[2] = z => o.value = !1),
+                    onTouchend: g[3] || (g[3] = z => o.value = !0),
+                    onMouseenter: g[4] || (g[4] = z => o.value = !1),
+                    onMouseleave: g[5] || (g[5] = z => o.value = !0),
+                    onMousedown: m,
+                    onMouseup: c
+                }, null, 8, ["modelValue", "disabled", "color", "max", "thumb-size"]), k("div", ca, $(_.value), 1)])) : e(t).activePlayerQueue && h.isProgressBar ? (d(), b("div", da, [r(_l, {
                     modelValue: s.value,
-                    "onUpdate:modelValue": g[6] || (g[6] = B => s.value = B),
-                    disabled: !e(t).activePlayerQueue || !e(t).curQueueItem || ((D = e(t).activePlayerQueue) == null ? void 0 : D.items) == 0,
+                    "onUpdate:modelValue": g[6] || (g[6] = z => s.value = z),
+                    disabled: !e(t).activePlayerQueue || !e(t).curQueueItem || ((N = e(t).activePlayerQueue) == null ? void 0 : N.items) == 0,
                     height: "70",
-                    color: e(jt)(l.color, .15),
+                    color: e(Xt)(l.color, .15),
                     "bg-color": l.color,
                     "bg-opacity": 1,
                     style: {
                         position: "absolute",
                         "border-radius": "10px"
                     },
                     min: 0,
                     max: e(t).curQueueItem && e(t).curQueueItem.duration
                 }, null, 8, ["modelValue", "disabled", "color", "bg-color", "max"])])) : I("", !0)])
             }
         }
     }),
-    da = M({
+    ma = D({
         __name: "ResponsiveIcon",
         props: {
             width: {
                 default: void 0
             },
             height: {
                 default: void 0
@@ -1367,156 +1367,156 @@
         },
         setup(a) {
             const l = a,
                 u = () => {
                     if (o.value) {
                         const s = o.value.offsetWidth,
                             n = o.value.offsetHeight,
-                            v = Math.min(s, n);
-                        i.value.$el.style.fontSize = `${v}px`
+                            p = Math.min(s, n);
+                        i.value.$el.style.fontSize = `${p}px`
                     }
                 },
-                o = T(),
-                i = T();
-            return re(() => {
+                o = S(),
+                i = S();
+            return ue(() => {
                 u(), window.addEventListener("resize", u)
-            }), ve(() => {
+            }), pe(() => {
                 window.removeEventListener("resize", u)
             }), (s, n) => (d(), b("div", {
                 ref_key: "responsiveIconHolder",
                 ref: o,
-                class: ce([l.type == "btn" ? "responsive-icon-holder-btn" : "responsive-icon-holder", {
+                class: de([l.type == "btn" ? "responsive-icon-holder-btn" : "responsive-icon-holder", {
                     disabled: s.disabled
                 }]),
                 style: L({
                     width: l.staticWidth ? l.staticWidth : l.width,
                     height: l.staticWidth ? l.staticWidth : l.height,
                     maxHeight: l.staticHeight ? l.staticHeight : l.maxHeight,
                     maxWidth: l.staticWidth ? l.staticWidth : l.maxWidth,
                     minHeight: l.staticHeight ? l.staticHeight : l.minHeight,
                     minWidth: l.staticWidth ? l.staticWidth : l.minWidth
                 })
-            }, [s.type === "icon" ? (d(), V(N, {
+            }, [s.type === "icon" ? (d(), V(E, {
                 key: 0,
                 ref_key: "responsiveIcon",
                 ref: i,
                 class: "responsive-icon",
                 color: s.color ? s.color : "",
                 icon: l.icon ? l.icon : "mdi-check",
                 width: l.staticWidth ? l.staticWidth : null,
                 height: l.staticHeight ? l.staticHeight : null
             }, De({
                 _: 2
-            }, [U(s.$slots, (v, f) => ({
-                name: f,
-                fn: y(() => [Ne(s.$slots, f, {}, void 0, !0)])
-            }))]), 1032, ["color", "icon", "width", "height"])) : s.type === "btn" ? (d(), V(N, {
+            }, [U(s.$slots, (p, _) => ({
+                name: _,
+                fn: f(() => [Ne(s.$slots, _, {}, void 0, !0)])
+            }))]), 1032, ["color", "icon", "width", "height"])) : s.type === "btn" ? (d(), V(E, {
                 key: 1,
                 ref_key: "responsiveIcon",
                 ref: i,
                 class: "responsive-icon",
                 style: {
                     cursor: "pointer"
                 },
                 color: s.color ? s.color : "",
                 icon: l.icon ? l.icon : "mdi-check",
                 width: l.staticWidth ? l.staticWidth : null,
                 height: l.staticHeight ? l.staticHeight : null,
                 disabled: s.disabled
             }, De({
                 _: 2
-            }, [U(s.$slots, (v, f) => ({
-                name: f,
-                fn: y(() => [Ne(s.$slots, f, {}, void 0, !0)])
+            }, [U(s.$slots, (p, _) => ({
+                name: _,
+                fn: f(() => [Ne(s.$slots, _, {}, void 0, !0)])
             }))]), 1032, ["color", "icon", "width", "height", "disabled"])) : I("", !0)], 6))
         }
     });
-const oe = xe(da, [
+const oe = xe(ma, [
         ["__scopeId", "data-v-5ed57264"]
     ]),
-    xt = M({
+    Qt = D({
         __name: "RepeatBtn",
         props: {
             isVisible: {
                 type: Boolean,
                 default: !0
             },
             icon: {
                 default: void 0
             }
         },
         setup(a) {
             const l = a;
             return (u, o) => {
-                var i, s, n, v, f, c, _, p, m, h;
-                return l.isVisible ? (d(), V(oe, H({
+                var i, s, n, p, _, y, m, c, v, h;
+                return l.isVisible ? (d(), V(oe, R({
                     key: 0
                 }, l.icon, {
                     disabled: !e(t).activePlayerQueue || !((i = e(t).activePlayerQueue) != null && i.active) || ((s = e(t).activePlayerQueue) == null ? void 0 : s.items) == 0,
-                    color: e(de)((n = l.icon) == null ? void 0 : n.color, [
-                        [((v = e(t).activePlayerQueue) == null ? void 0 : v.repeat_mode) == e(q).OFF, null],
-                        [((f = e(t).activePlayerQueue) == null ? void 0 : f.repeat_mode) == e(q).ALL, "secondary"],
-                        [((c = e(t).activePlayerQueue) == null ? void 0 : c.repeat_mode) == e(q).ONE, "secondary"]
+                    color: e(me)((n = l.icon) == null ? void 0 : n.color, [
+                        [((p = e(t).activePlayerQueue) == null ? void 0 : p.repeat_mode) == e(q).OFF, null],
+                        [((_ = e(t).activePlayerQueue) == null ? void 0 : _.repeat_mode) == e(q).ALL, "secondary"],
+                        [((y = e(t).activePlayerQueue) == null ? void 0 : y.repeat_mode) == e(q).ONE, "secondary"]
                     ]),
-                    icon: e(de)((_ = l.icon) == null ? void 0 : _.icon, [
-                        [((p = e(t).activePlayerQueue) == null ? void 0 : p.repeat_mode) == e(q).OFF, "mdi-repeat-off"],
-                        [((m = e(t).activePlayerQueue) == null ? void 0 : m.repeat_mode) == e(q).ALL, "mdi-repeat"],
+                    icon: e(me)((m = l.icon) == null ? void 0 : m.icon, [
+                        [((c = e(t).activePlayerQueue) == null ? void 0 : c.repeat_mode) == e(q).OFF, "mdi-repeat-off"],
+                        [((v = e(t).activePlayerQueue) == null ? void 0 : v.repeat_mode) == e(q).ALL, "mdi-repeat"],
                         [((h = e(t).activePlayerQueue) == null ? void 0 : h.repeat_mode) == e(q).ONE, "mdi-repeat-once"],
                         [!0, "mdi-repeat-off"]
                     ]),
                     type: "btn",
                     onClick: o[0] || (o[0] = g => {
-                        var P, D, B, F;
-                        return e(w).queueCommandRepeat(((P = e(t).activePlayerQueue) == null ? void 0 : P.queue_id) || "", e(de)(null, [
-                            [((D = e(t).activePlayerQueue) == null ? void 0 : D.repeat_mode) == e(q).OFF, e(q).ONE],
-                            [((B = e(t).activePlayerQueue) == null ? void 0 : B.repeat_mode) == e(q).ALL, e(q).OFF],
+                        var C, N, z, F;
+                        return e(w).queueCommandRepeat(((C = e(t).activePlayerQueue) == null ? void 0 : C.queue_id) || "", e(me)(null, [
+                            [((N = e(t).activePlayerQueue) == null ? void 0 : N.repeat_mode) == e(q).OFF, e(q).ONE],
+                            [((z = e(t).activePlayerQueue) == null ? void 0 : z.repeat_mode) == e(q).ALL, e(q).OFF],
                             [((F = e(t).activePlayerQueue) == null ? void 0 : F.repeat_mode) == e(q).ONE, e(q).ALL]
                         ]))
                     })
                 }), null, 16, ["disabled", "color", "icon"])) : I("", !0)
             }
         }
     }),
-    St = M({
+    St = D({
         __name: "ShuffleBtn",
         props: {
             isVisible: {
                 type: Boolean,
                 default: !0
             },
             icon: {
                 default: void 0
             }
         },
         setup(a) {
             const l = a;
             return (u, o) => {
-                var i, s, n, v, f, c, _;
-                return l.isVisible ? (d(), V(oe, H({
+                var i, s, n, p, _, y, m;
+                return l.isVisible ? (d(), V(oe, R({
                     key: 0
                 }, l.icon, {
                     disabled: !e(t).activePlayerQueue || !((i = e(t).activePlayerQueue) != null && i.active) || ((s = e(t).activePlayerQueue) == null ? void 0 : s.items) == 0,
-                    color: e(de)((n = l.icon) == null ? void 0 : n.color, [
-                        [(v = e(t).activePlayerQueue) == null ? void 0 : v.shuffle_enabled, "secondary", ""]
+                    color: e(me)((n = l.icon) == null ? void 0 : n.color, [
+                        [(p = e(t).activePlayerQueue) == null ? void 0 : p.shuffle_enabled, "secondary", ""]
                     ]),
-                    icon: e(de)((f = l.icon) == null ? void 0 : f.icon, [
-                        [(c = e(t).activePlayerQueue) == null ? void 0 : c.shuffle_enabled, "mdi-shuffle"],
-                        [((_ = e(t).activePlayerQueue) == null ? void 0 : _.shuffle_enabled) == !1, "mdi-shuffle-disabled"],
+                    icon: e(me)((_ = l.icon) == null ? void 0 : _.icon, [
+                        [(y = e(t).activePlayerQueue) == null ? void 0 : y.shuffle_enabled, "mdi-shuffle"],
+                        [((m = e(t).activePlayerQueue) == null ? void 0 : m.shuffle_enabled) == !1, "mdi-shuffle-disabled"],
                         [!0, "mdi-shuffle"]
                     ]),
                     type: "btn",
-                    onClick: o[0] || (o[0] = p => {
-                        var m, h;
-                        return e(w).queueCommandShuffle(((m = e(t).activePlayerQueue) == null ? void 0 : m.queue_id) || "", !((h = e(t).activePlayerQueue) != null && h.shuffle_enabled))
+                    onClick: o[0] || (o[0] = c => {
+                        var v, h;
+                        return e(w).queueCommandShuffle(((v = e(t).activePlayerQueue) == null ? void 0 : v.queue_id) || "", !((h = e(t).activePlayerQueue) != null && h.shuffle_enabled))
                     })
                 }), null, 16, ["disabled", "color", "icon"])) : I("", !0)
             }
         }
     }),
-    Qt = M({
+    Tt = D({
         __name: "PlayBtn",
         props: {
             isVisible: {
                 type: Boolean,
                 default: !0
             },
             withCircle: {
@@ -1526,120 +1526,120 @@
             icon: {
                 default: void 0
             }
         },
         setup(a) {
             const l = a;
             return (u, o) => {
-                var i, s, n, v, f, c;
-                return e(t).activePlayerQueue && ((i = e(t).activePlayerQueue) != null && i.active) && l.isVisible ? (d(), V(oe, H({
+                var i, s, n, p, _, y;
+                return e(t).activePlayerQueue && ((i = e(t).activePlayerQueue) != null && i.active) && l.isVisible ? (d(), V(oe, R({
                     key: 0
                 }, l.icon, {
                     disabled: e(t).activePlayerQueue && !((s = e(t).activePlayerQueue) != null && s.active) && ((n = e(t).activePlayerQueue) == null ? void 0 : n.items) == 0,
-                    icon: ((v = e(t).activePlayerQueue) == null ? void 0 : v.state) == "playing" ? l.withCircle ? "mdi-pause-circle" : "mdi-pause" : l.withCircle ? "mdi-play-circle" : "mdi-play",
+                    icon: ((p = e(t).activePlayerQueue) == null ? void 0 : p.state) == "playing" ? l.withCircle ? "mdi-pause-circle" : "mdi-pause" : l.withCircle ? "mdi-play-circle" : "mdi-play",
                     type: "btn",
-                    onClick: o[0] || (o[0] = _ => e(w).queueCommandPlayPause(e(t).activePlayerQueue.queue_id))
-                }), null, 16, ["disabled", "icon"])) : ((f = e(t).selectedPlayer) == null ? void 0 : f.state) == e(gt).PLAYING && l.isVisible ? (d(), V(oe, H({
+                    onClick: o[0] || (o[0] = m => e(w).queueCommandPlayPause(e(t).activePlayerQueue.queue_id))
+                }), null, 16, ["disabled", "icon"])) : ((_ = e(t).selectedPlayer) == null ? void 0 : _.state) == e(bt).PLAYING && l.isVisible ? (d(), V(oe, R({
                     key: 1
                 }, l.icon, {
                     icon: "mdi-stop",
                     type: "btn",
-                    onClick: o[1] || (o[1] = _ => e(w).queueCommandStop(e(t).selectedPlayer.player_id))
-                }), null, 16)) : l.isVisible ? (d(), V(oe, H({
+                    onClick: o[1] || (o[1] = m => e(w).queueCommandStop(e(t).selectedPlayer.player_id))
+                }), null, 16)) : l.isVisible ? (d(), V(oe, R({
                     key: 2
                 }, l.icon, {
-                    disabled: !e(t).activePlayerQueue || ((c = e(t).activePlayerQueue) == null ? void 0 : c.items) == 0,
+                    disabled: !e(t).activePlayerQueue || ((y = e(t).activePlayerQueue) == null ? void 0 : y.items) == 0,
                     icon: l.withCircle ? "mdi-play-circle" : "mdi-play",
                     type: "btn",
-                    onClick: o[2] || (o[2] = _ => {
-                        var p;
-                        return e(w).queueCommandPlay(((p = e(t).activePlayerQueue) == null ? void 0 : p.queue_id) || e(t).selectedPlayer.player_id)
+                    onClick: o[2] || (o[2] = m => {
+                        var c;
+                        return e(w).queueCommandPlay(((c = e(t).activePlayerQueue) == null ? void 0 : c.queue_id) || e(t).selectedPlayer.player_id)
                     })
                 }), null, 16, ["disabled", "icon"])) : I("", !0)
             }
         }
     }),
-    Tt = M({
+    Bt = D({
         __name: "PreviousBtn",
         props: {
             isVisible: {
                 type: Boolean,
                 default: !0
             },
             icon: {
                 default: void 0
             }
         },
         setup(a) {
             const l = a;
             return (u, o) => {
                 var i, s;
-                return l.isVisible ? (d(), V(oe, H({
+                return l.isVisible ? (d(), V(oe, R({
                     key: 0
                 }, l.icon, {
                     disabled: !e(t).activePlayerQueue || !((i = e(t).activePlayerQueue) != null && i.active) || ((s = e(t).activePlayerQueue) == null ? void 0 : s.items) == 0,
                     icon: "mdi-skip-previous-outline",
                     type: "btn",
                     onClick: o[0] || (o[0] = n => e(w).queueCommandPrevious(e(t).activePlayerQueue.queue_id))
                 }), null, 16, ["disabled"])) : I("", !0)
             }
         }
     }),
-    Bt = M({
+    Mt = D({
         __name: "NextBtn",
         props: {
             isVisible: {
                 type: Boolean,
                 default: !0
             },
             icon: {
                 default: void 0
             }
         },
         setup(a) {
             const l = a;
             return (u, o) => {
                 var i, s;
-                return l.isVisible ? (d(), V(oe, H({
+                return l.isVisible ? (d(), V(oe, R({
                     key: 0
                 }, l.icon, {
                     disabled: !e(t).activePlayerQueue || !((i = e(t).activePlayerQueue) != null && i.active) || ((s = e(t).activePlayerQueue) == null ? void 0 : s.items) == 0,
                     icon: "mdi-skip-next-outline",
                     type: "btn",
                     onClick: o[0] || (o[0] = n => e(w).queueCommandNext(e(t).activePlayerQueue.queue_id))
                 }), null, 16, ["disabled"])) : I("", !0)
             }
         }
     }),
-    ma = {
+    va = {
         key: 0,
         style: {
             display: "inline-flex"
         }
     },
-    va = {
+    pa = {
         key: 0,
         class: "player-controls-elements"
     },
-    pa = {
+    ya = {
         key: 1,
         class: "player-controls-elements"
     },
-    ya = {
+    fa = {
         key: 2
     },
-    fa = {
+    ha = {
         key: 3,
         class: "player-controls-elements"
     },
-    ha = {
+    _a = {
         key: 4,
         class: "player-controls-elements"
     },
-    $e = M({
+    $e = D({
         __name: "PlayerControls",
         props: {
             visibleComponents: {
                 default: () => ({
                     repeat: {
                         isVisible: !0
                     },
@@ -1657,342 +1657,342 @@
                     }
                 })
             }
         },
         setup(a) {
             const l = a;
             return (u, o) => {
-                var i, s, n, v, f;
-                return l.visibleComponents ? (d(), b("div", ma, [l.visibleComponents && ((i = l.visibleComponents.shuffle) != null && i.isVisible) ? (d(), b("div", va, [r(St, {
+                var i, s, n, p, _;
+                return l.visibleComponents ? (d(), b("div", va, [l.visibleComponents && ((i = l.visibleComponents.shuffle) != null && i.isVisible) ? (d(), b("div", pa, [r(St, {
                     class: "media-controls-item",
                     icon: l.visibleComponents.shuffle.icon
-                }, null, 8, ["icon"])])) : I("", !0), l.visibleComponents && ((s = l.visibleComponents.previous) != null && s.isVisible) ? (d(), b("div", pa, [r(Tt, {
+                }, null, 8, ["icon"])])) : I("", !0), l.visibleComponents && ((s = l.visibleComponents.previous) != null && s.isVisible) ? (d(), b("div", ya, [r(Bt, {
                     class: "media-controls-item",
                     icon: l.visibleComponents.previous.icon
-                }, null, 8, ["icon"])])) : I("", !0), l.visibleComponents && ((n = l.visibleComponents.play) != null && n.isVisible) ? (d(), b("div", ya, [r(Qt, {
+                }, null, 8, ["icon"])])) : I("", !0), l.visibleComponents && ((n = l.visibleComponents.play) != null && n.isVisible) ? (d(), b("div", fa, [r(Tt, {
                     class: "media-controls-item",
                     "with-circle": l.visibleComponents.play.withCircle,
                     icon: l.visibleComponents.play.icon
-                }, null, 8, ["with-circle", "icon"])])) : I("", !0), l.visibleComponents && ((v = l.visibleComponents.next) != null && v.isVisible) ? (d(), b("div", fa, [r(Bt, {
+                }, null, 8, ["with-circle", "icon"])])) : I("", !0), l.visibleComponents && ((p = l.visibleComponents.next) != null && p.isVisible) ? (d(), b("div", ha, [r(Mt, {
                     icon: l.visibleComponents.next.icon,
                     "static-height": "24px",
                     "static-width": "24px"
-                }, null, 8, ["icon"])])) : I("", !0), l.visibleComponents && ((f = l.visibleComponents.repeat) != null && f.isVisible) ? (d(), b("div", ha, [r(xt, {
+                }, null, 8, ["icon"])])) : I("", !0), l.visibleComponents && ((_ = l.visibleComponents.repeat) != null && _.isVisible) ? (d(), b("div", _a, [r(Qt, {
                     icon: l.visibleComponents.repeat.icon,
                     "static-height": "24px",
                     "static-width": "24px"
                 }, null, 8, ["icon"])])) : I("", !0)])) : I("", !0)
             }
         }
     });
-const _a = M({
+const ga = D({
         __name: "QueueBtn",
         props: {
             color: {}
         },
         setup(a) {
             const l = a;
             return (u, o) => (d(), V(Y, {
                 variant: "icon",
                 icon: "mdi-playlist-play",
                 color: l.color ? u.color : "",
                 onClick: o[0] || (o[0] = i => {
-                    e(t).showFullscreenPlayer = !1, e(Pe).push("/playerqueue/")
+                    e(t).showFullscreenPlayer = !1, e(ne).push("/playerqueue/")
                 })
             }, null, 8, ["color"]))
         }
     }),
-    ga = {
+    ba = {
         key: 2,
         class: "line-clamp-1 no_transform"
     },
-    ba = M({
+    ka = D({
         __name: "SpeakerBtn",
         props: {
             color: {}
         },
         setup(a) {
             const l = a,
-                u = S(() => {
+                u = x(() => {
                     var i;
                     if (!t.selectedPlayer) return 0;
                     let o = 0;
                     for (const s of t.selectedPlayer.group_childs) {
                         const n = (i = w) == null ? void 0 : i.players[s];
                         n && n.available && n.powered && o++
                     }
                     return o
                 });
             return (o, i) => (d(), V(Y, {
                 variant: "icon",
                 ripple: !1,
-                icon: !e(C)("bp6"),
+                icon: !e(P)("bp6"),
                 onClick: i[0] || (i[0] = s => e(t).showPlayersMenu = !0)
             }, {
-                default: y(() => {
+                default: f(() => {
                     var s, n;
-                    return [(s = e(t).selectedPlayer) != null && s.group_childs.length ? (d(), V(Ct, {
+                    return [(s = e(t).selectedPlayer) != null && s.group_childs.length ? (d(), V(Vt, {
                         key: 0,
                         size: "small",
                         content: u.value
                     }, {
-                        default: y(() => [r(N, {
+                        default: f(() => [r(E, {
                             color: l.color ? o.color : "",
                             size: 24
                         }, {
-                            default: y(() => [j("mdi-speaker-multiple")]),
+                            default: f(() => [G("mdi-speaker-multiple")]),
                             _: 1
                         }, 8, ["color"])]),
                         _: 1
-                    }, 8, ["content"])) : (d(), V(N, {
+                    }, 8, ["content"])) : (d(), V(E, {
                         key: 1,
                         color: l.color ? o.color : "",
                         size: 24
                     }, {
-                        default: y(() => [j("mdi-speaker")]),
+                        default: f(() => [G("mdi-speaker")]),
                         _: 1
-                    }, 8, ["color"])), e(t).activePlayerQueue && e(C)("bp6") ? (d(), b("span", ga, $(e(Ae)((n = e(t).activePlayerQueue) == null ? void 0 : n.display_name, e(C)("bp7") ? 16 : 8)), 1)) : I("", !0)]
+                    }, 8, ["color"])), e(t).activePlayerQueue && e(P)("bp6") ? (d(), b("span", ba, $(e(Ae)((n = e(t).activePlayerQueue) == null ? void 0 : n.display_name, e(P)("bp7") ? 16 : 8)), 1)) : I("", !0)]
                 }),
                 _: 1
             }, 8, ["icon"]))
         }
     });
-const ka = {
+const wa = {
     props: {
         width: String,
         height: String,
         style: String,
         isPowered: Boolean
     },
     emits: ["update:model-value"],
     setup(a, l) {
-        const u = T(!0),
-            o = S(() => ({
+        const u = S(!0),
+            o = x(() => ({
                 class: "player-volume",
                 hideDetails: !0,
                 trackSize: 2,
                 thumbSize: u.value ? 0 : 10,
                 step: 2,
                 elevation: 0,
                 disabled: !a.isPowered,
                 style: `width: ${a.width}; height:${a.height}; display: inline-grid; ${a.style}`
             })),
-            i = S(() => ({
+            i = x(() => ({
                 ...o.value,
                 ...l
             }));
         return {
             isThumbHidden: u,
             playerVolumeProps: i,
             onWheel: ({
                 deltaY: n
             }) => {
-                const v = i.value.step,
-                    f = l.attrs["model-value"],
-                    c = n < 0 ? v : -v;
-                l.emit("update:model-value", f + c)
+                const p = i.value.step,
+                    _ = l.attrs["model-value"],
+                    y = n < 0 ? p : -p;
+                l.emit("update:model-value", _ + y)
             }
         }
     }
 };
 
-function wa(a, l, u, o, i, s) {
-    return d(), V($t, H(o.playerVolumeProps, {
+function Pa(a, l, u, o, i, s) {
+    return d(), V(It, R(o.playerVolumeProps, {
         onTouchstart: l[0] || (l[0] = n => o.isThumbHidden = !1),
         onTouchend: l[1] || (l[1] = n => o.isThumbHidden = !0),
         onMouseenter: l[2] || (l[2] = n => o.isThumbHidden = !1),
         onMouseleave: l[3] || (l[3] = n => o.isThumbHidden = !0),
         onWheel: o.onWheel,
         "onUpdate:modelValue": l[4] || (l[4] = n => a.$emit("update:model-value", n))
     }), De({
         _: 2
-    }, [U(a.$slots, (n, v) => ({
-        name: v,
-        fn: y(() => [Ne(a.$slots, v)])
+    }, [U(a.$slots, (n, p) => ({
+        name: p,
+        fn: f(() => [Ne(a.$slots, p)])
     }))]), 1040, ["onWheel"])
 }
-const He = xe(ka, [
-        ["render", wa]
+const Re = xe(wa, [
+        ["render", Pa]
     ]),
-    Pa = {
+    Ca = {
         class: "text-center",
         style: {
             "padding-right": "5px"
         }
     },
-    Ca = {
+    Va = {
         class: "text-caption"
     },
-    Va = {
+    $a = {
         class: "text-center"
     },
-    $a = {
+    Ia = {
         key: 0,
         class: "text-caption"
     },
-    Ia = {
+    xa = {
         key: 1,
         class: "text-caption"
     },
-    xa = {
+    Qa = {
         key: 0
     },
     Sa = {
         key: 1,
         class: "syncbtn"
     },
-    Mt = M({
+    zt = D({
         __name: "VolumeControl",
         props: {
             player: {}
         },
         setup(a) {
             const l = function(o) {
                     var s;
                     const i = [];
-                    o.type != ge.GROUP && o.type != ge.SYNC_GROUP && i.push(o);
+                    o.type != be.GROUP && o.type != be.SYNC_GROUP && i.push(o);
                     for (const n of o.group_childs) {
-                        const v = (s = w) == null ? void 0 : s.players[n];
-                        v && v.available && !i.includes(v) && i.push(v)
+                        const p = (s = w) == null ? void 0 : s.players[n];
+                        p && p.available && !i.includes(p) && i.push(p)
                     }
-                    return i.sort((n, v) => n.display_name.toUpperCase() > v.display_name.toUpperCase() ? 1 : -1), i
+                    return i.sort((n, p) => n.display_name.toUpperCase() > p.display_name.toUpperCase() ? 1 : -1), i
                 },
                 u = function(o, i) {
-                    o.type == ge.GROUP || o.type == ge.SYNC_GROUP || o.group_childs.length > 0 ? w.playerCommandGroupPower(o.player_id, i) : w.playerCommandPower(o.player_id, i)
+                    o.type == be.GROUP || o.type == be.SYNC_GROUP || o.group_childs.length > 0 ? w.playerCommandGroupPower(o.player_id, i) : w.playerCommandPower(o.player_id, i)
                 };
             return (o, i) => (d(), V(ie, {
                 style: {
                     overflow: "hidden"
                 },
                 lines: "two"
             }, {
-                default: y(() => [o.player.group_childs.length > 0 ? (d(), V(K, {
+                default: f(() => [o.player.group_childs.length > 0 ? (d(), V(X, {
                     key: 0
                 }, {
-                    prepend: y(() => [k("div", {
+                    prepend: f(() => [k("div", {
                         style: L(o.player.powered ? "opacity: 0.75" : "opacity: 0.5")
-                    }, [k("div", Pa, [r(Y, {
+                    }, [k("div", Ca, [r(Y, {
                         icon: "",
                         style: {
                             height: "25px !important"
                         },
                         onClick: i[0] || (i[0] = s => u(o.player, !o.player.powered))
                     }, {
-                        default: y(() => [r(N, {
+                        default: f(() => [r(E, {
                             size: 25,
                             icon: o.player.volume_muted ? "mdi-volume-off" : "mdi-power"
                         }, null, 8, ["icon"])]),
                         _: 1
-                    }), k("div", Ca, $(o.player.group_volume), 1)])], 4)]),
-                    default: y(() => [k("div", {
+                    }), k("div", Va, $(o.player.group_volume), 1)])], 4)]),
+                    default: f(() => [k("div", {
                         style: L(o.player.powered ? "opacity: 0.75" : "opacity: 0.5")
-                    }, [k("h6", null, $(e(bt)(o.player, 27)), 1), r(He, {
+                    }, [k("h6", null, $(e(kt)(o.player, 27)), 1), r(Re, {
                         class: "vc-slider",
                         width: "100%",
                         color: "secondary",
                         "is-powered": o.player.powered,
                         "model-value": Math.round(o.player.group_volume),
                         "onUpdate:modelValue": i[1] || (i[1] = s => e(w).playerCommandGroupVolume(o.player.player_id, s))
                     }, null, 8, ["is-powered", "model-value"])], 4)]),
                     _: 1
                 })) : I("", !0), o.player.group_childs.length > 0 ? (d(), V(le, {
                     key: 1,
                     style: {
                         "margin-top": "10px",
                         "margin-bottom": "10px"
                     }
-                })) : I("", !0), (d(!0), b(R, null, U(l(o.player), s => (d(), V(K, {
+                })) : I("", !0), (d(!0), b(H, null, U(l(o.player), s => (d(), V(X, {
                     key: s.player_id,
                     style: L(s.powered ? "opacity: 0.75" : "opacity: 0.5")
                 }, {
-                    prepend: y(() => [k("div", {
+                    prepend: f(() => [k("div", {
                         style: L(s.powered ? "opacity: 0.75" : "opacity: 0.5")
-                    }, [k("div", Va, [r(Y, {
+                    }, [k("div", $a, [r(Y, {
                         icon: "",
                         style: {
                             height: "25px !important"
                         },
                         onClick: n => e(w).playerCommandPowerToggle(s.player_id)
                     }, {
-                        default: y(() => [r(N, {
+                        default: f(() => [r(E, {
                             size: 25,
                             icon: "mdi-power"
                         })]),
                         _: 2
-                    }, 1032, ["onClick"]), s.volume_muted ? (d(), b("div", $a, $(o.$t("muted")), 1)) : (d(), b("div", Ia, $(s.volume_level), 1))])], 4)]),
-                    default: y(() => [k("div", {
+                    }, 1032, ["onClick"]), s.volume_muted ? (d(), b("div", Ia, $(o.$t("muted")), 1)) : (d(), b("div", xa, $(s.volume_level), 1))])], 4)]),
+                    default: f(() => [k("div", {
                         style: L(s.powered ? "opacity: 0.75" : "opacity: 0.5")
-                    }, [k("h6", null, $(e(Ae)(s.display_name, 27)), 1), r(He, {
+                    }, [k("h6", null, $(e(Ae)(s.display_name, 27)), 1), r(Re, {
                         class: "vc-slider",
                         width: "100%",
                         color: "secondary",
                         "is-powered": s.powered,
                         "model-value": Math.round(s.volume_level),
                         "onUpdate:modelValue": n => e(w).playerCommandVolumeSet(s.player_id, n)
                     }, null, 8, ["is-powered", "model-value", "onUpdate:modelValue"])], 4)]),
-                    append: y(() => [k("div", {
+                    append: f(() => [k("div", {
                         style: L(s.powered ? "margin-right:-10px;opacity: 0.75" : "margin-right:-10px;opacity: 0.5")
-                    }, [!s.synced_to && s.can_sync_with.length && Object.values(e(w).players).filter(n => !n.synced_to && n.can_sync_with.includes(s.player_id)).length > 0 ? (d(), b("div", xa, [r(wt, {
+                    }, [!s.synced_to && s.can_sync_with.length && Object.values(e(w).players).filter(n => !n.synced_to && n.can_sync_with.includes(s.player_id)).length > 0 ? (d(), b("div", Qa, [r(Pt, {
                         location: "bottom end",
                         style: {
                             "z-index": "999999"
                         }
                     }, {
-                        activator: y(({
+                        activator: f(({
                             props: n
-                        }) => [r(Y, H({
+                        }) => [r(Y, R({
                             icon: ""
                         }, n), {
-                            default: y(() => [r(N, null, {
-                                default: y(() => [j("mdi-link-variant")]),
+                            default: f(() => [r(E, null, {
+                                default: f(() => [G("mdi-link-variant")]),
                                 _: 1
                             })]),
                             _: 2
                         }, 1040)]),
-                        default: y(() => [r(ie, null, {
-                            default: y(() => [r(Il, null, {
-                                default: y(() => [j($(o.$t("sync_player_to")), 1)]),
+                        default: f(() => [r(ie, null, {
+                            default: f(() => [r(xl, null, {
+                                default: f(() => [G($(o.$t("sync_player_to")), 1)]),
                                 _: 1
-                            }), (d(!0), b(R, null, U(Object.values(e(w).players).filter(n => !n.synced_to && n.can_sync_with.includes(s.player_id)), n => (d(), V(K, {
+                            }), (d(!0), b(H, null, U(Object.values(e(w).players).filter(n => !n.synced_to && n.can_sync_with.includes(s.player_id)), n => (d(), V(X, {
                                 key: n.player_id,
                                 title: n.display_name,
-                                onClick: v => e(w).playerCommandSync(s.player_id, n.player_id)
+                                onClick: p => e(w).playerCommandSync(s.player_id, n.player_id)
                             }, null, 8, ["title", "onClick"]))), 128)), r(le)]),
                             _: 2
                         }, 1024)]),
                         _: 2
                     }, 1024)])) : I("", !0), s.synced_to ? (d(), b("div", Sa, [r(Y, {
                         icon: "",
                         onClick: n => e(w).playerCommandUnSync(s.player_id)
                     }, {
-                        default: y(() => [r(N, null, {
-                            default: y(() => [j("mdi-link-variant-off")]),
+                        default: f(() => [r(E, null, {
+                            default: f(() => [G("mdi-link-variant-off")]),
                             _: 1
                         })]),
                         _: 2
                     }, 1032, ["onClick"])])) : I("", !0)], 4)]),
                     _: 2
                 }, 1032, ["style"]))), 128))]),
                 _: 1
             }))
         }
     });
-const Qa = {
+const Ta = {
         key: 0
     },
-    Ta = {
+    Ba = {
         key: 0
     },
-    Ba = {
+    Ma = {
         class: "text-caption"
     },
-    Ma = {
+    za = {
         key: 1
     },
-    za = M({
+    Da = D({
         __name: "VolumeBtn",
         props: {
             volumeSize: {
                 default: "150px"
             },
             responsiveVolumeSize: {
                 type: Boolean,
@@ -2004,122 +2004,122 @@
             },
             color: {
                 default: ""
             }
         },
         setup(a) {
             const l = a,
-                u = T(!1);
-            return (o, i) => l.isVisible && e(t).selectedPlayer ? (d(), b("div", Qa, [r(wt, {
+                u = S(!1);
+            return (o, i) => l.isVisible && e(t).selectedPlayer ? (d(), b("div", Ta, [r(Pt, {
                 modelValue: u.value,
                 "onUpdate:modelValue": i[2] || (i[2] = s => u.value = s),
                 class: "volume-control-dialog",
                 "close-on-content-click": !1
             }, {
-                activator: y(({
+                activator: f(({
                     props: s
                 }) => {
-                    var n, v;
-                    return [e(C)("bp5") || !o.responsiveVolumeSize ? (d(), b("div", Ta, [r(He, {
+                    var n, p;
+                    return [e(P)("bp5") || !o.responsiveVolumeSize ? (d(), b("div", Ba, [r(Re, {
                         style: "margin-right: 0px; margin-left: 0px;",
                         width: o.volumeSize,
                         "is-powered": !0,
-                        "model-value": e(t).selectedPlayer.group_childs.length > 0 ? Math.round(((n = e(t).selectedPlayer) == null ? void 0 : n.group_volume) || 0) : Math.round(((v = e(t).selectedPlayer) == null ? void 0 : v.volume_level) || 0),
-                        "onUpdate:modelValue": i[0] || (i[0] = f => {
-                            var c, _;
-                            return e(t).selectedPlayer.group_childs.length > 0 ? e(w).playerCommandGroupVolume(((c = e(t).selectedPlayer) == null ? void 0 : c.player_id) || "", f) : e(w).playerCommandVolumeSet(((_ = e(t).selectedPlayer) == null ? void 0 : _.player_id) || "", f)
+                        "model-value": e(t).selectedPlayer.group_childs.length > 0 ? Math.round(((n = e(t).selectedPlayer) == null ? void 0 : n.group_volume) || 0) : Math.round(((p = e(t).selectedPlayer) == null ? void 0 : p.volume_level) || 0),
+                        "onUpdate:modelValue": i[0] || (i[0] = _ => {
+                            var y, m;
+                            return e(t).selectedPlayer.group_childs.length > 0 ? e(w).playerCommandGroupVolume(((y = e(t).selectedPlayer) == null ? void 0 : y.player_id) || "", _) : e(w).playerCommandVolumeSet(((m = e(t).selectedPlayer) == null ? void 0 : m.player_id) || "", _)
                         })
                     }, {
-                        prepend: y(() => [r(Y, H({
+                        prepend: f(() => [r(Y, R({
                             variant: "icon",
                             size: "48",
                             ripple: !1
                         }, {
                             ...s
                         }), {
-                            default: y(() => {
-                                var f, c;
-                                return [r(N, {
+                            default: f(() => {
+                                var _, y;
+                                return [r(E, {
                                     color: l.color ? o.color : "",
                                     size: 24,
                                     icon: "mdi-volume-high"
-                                }, null, 8, ["color"]), k("div", Ba, $(e(t).selectedPlayer.group_childs.length > 0 ? Math.round(((f = e(t).selectedPlayer) == null ? void 0 : f.group_volume) || 0) : Math.round(((c = e(t).selectedPlayer) == null ? void 0 : c.volume_level) || 0)), 1)]
+                                }, null, 8, ["color"]), k("div", Ma, $(e(t).selectedPlayer.group_childs.length > 0 ? Math.round(((_ = e(t).selectedPlayer) == null ? void 0 : _.group_volume) || 0) : Math.round(((y = e(t).selectedPlayer) == null ? void 0 : y.volume_level) || 0)), 1)]
                             }),
                             _: 2
                         }, 1040)]),
                         _: 2
-                    }, 1032, ["width", "model-value"])])) : (d(), b("div", Ma, [r(Y, H({
+                    }, 1032, ["width", "model-value"])])) : (d(), b("div", za, [r(Y, R({
                         ...s
                     }, {
                         size: "48",
                         variant: "icon"
                     }), {
-                        default: y(() => {
-                            var f, c;
-                            return [r(N, {
+                        default: f(() => {
+                            var _, y;
+                            return [r(E, {
                                 color: l.color ? o.color : "",
                                 icon: "mdi-volume-high"
                             }, null, 8, ["color"]), k("div", {
                                 class: "text-caption",
                                 style: L({
                                     color: l.color ? o.color : ""
                                 })
-                            }, $(e(t).selectedPlayer.group_childs.length > 0 ? Math.round(((f = e(t).selectedPlayer) == null ? void 0 : f.group_volume) || 0) : Math.round(((c = e(t).selectedPlayer) == null ? void 0 : c.volume_level) || 0)), 5)]
+                            }, $(e(t).selectedPlayer.group_childs.length > 0 ? Math.round(((_ = e(t).selectedPlayer) == null ? void 0 : _.group_volume) || 0) : Math.round(((y = e(t).selectedPlayer) == null ? void 0 : y.volume_level) || 0)), 5)]
                         }),
                         _: 2
                     }, 1040)]))]
                 }),
-                default: y(() => [r(Qe, {
+                default: f(() => [r(Se, {
                     "min-width": 300
                 }, {
-                    default: y(() => [r(ie, {
+                    default: f(() => [r(ie, {
                         style: {
                             overflow: "hidden"
                         },
                         lines: "two"
                     }, {
-                        default: y(() => {
-                            var s, n, v;
-                            return [r(K, {
+                        default: f(() => {
+                            var s, n, p;
+                            return [r(X, {
                                 density: "compact",
                                 "two-line": "",
                                 title: (s = e(t).selectedPlayer) == null ? void 0 : s.display_name.substring(0, 25),
-                                subtitle: (n = e(t).selectedPlayer) != null && n.powered ? o.$t("state." + ((v = e(t).selectedPlayer) == null ? void 0 : v.state)) : o.$t("state.off")
+                                subtitle: (n = e(t).selectedPlayer) != null && n.powered ? o.$t("state." + ((p = e(t).selectedPlayer) == null ? void 0 : p.state)) : o.$t("state.off")
                             }, {
-                                prepend: y(() => [r(N, {
+                                prepend: f(() => [r(E, {
                                     size: "50",
                                     icon: e(t).selectedPlayer.icon,
                                     color: "primary"
                                 }, null, 8, ["icon"])]),
-                                default: y(() => [r(me, {
+                                default: f(() => [r(ve, {
                                     variant: "plain",
                                     style: {
                                         position: "absolute",
                                         right: "0px",
                                         top: "0px"
                                     },
                                     icon: "mdi-close",
                                     dark: "",
-                                    onClick: i[1] || (i[1] = f => u.value = !u.value)
+                                    onClick: i[1] || (i[1] = _ => u.value = !u.value)
                                 })]),
                                 _: 1
-                            }, 8, ["title", "subtitle"]), r(le), e(t).selectedPlayer ? (d(), V(Mt, {
+                            }, 8, ["title", "subtitle"]), r(le), e(t).selectedPlayer ? (d(), V(zt, {
                                 key: 0,
                                 player: e(t).selectedPlayer
                             }, null, 8, ["player"])) : I("", !0)]
                         }),
                         _: 1
                     })]),
                     _: 1
                 })]),
                 _: 1
             }, 8, ["modelValue"])])) : I("", !0)
         }
     });
-const ke = M({
+const we = D({
         __name: "PlayerExtendedControls",
         props: {
             queue: {
                 default: () => ({
                     isVisible: !0,
                     showQueueDialog: !1
                 })
@@ -2135,358 +2135,393 @@
                     volumeSize: "150px",
                     responsiveVolumeSize: !1
                 })
             }
         },
         setup(a) {
             const l = a;
-            return (u, o) => (d(), b(R, null, [l.player && l.player.isVisible ? (d(), V(ba, {
+            return (u, o) => (d(), b(H, null, [l.player && l.player.isVisible ? (d(), V(ka, {
                 key: 0,
                 color: l.player.color
-            }, null, 8, ["color"])) : I("", !0), l.queue && l.queue.isVisible ? (d(), V(_a, {
+            }, null, 8, ["color"])) : I("", !0), l.queue && l.queue.isVisible ? (d(), V(ga, {
                 key: 1,
                 color: l.queue.color
-            }, null, 8, ["color"])) : I("", !0), l.volume && l.volume.isVisible ? (d(), V(za, {
+            }, null, 8, ["color"])) : I("", !0), l.volume && l.volume.isVisible ? (d(), V(Da, {
                 key: 2,
                 color: l.volume.color,
                 "volume-size": l.volume.volumeSize,
                 "responsive-volume-size": l.volume.responsiveVolumeSize
             }, null, 8, ["color", "volume-size", "responsive-volume-size"])) : I("", !0)], 64))
         }
     }),
-    Da = a => (Xt("data-v-1ba8c187"), a = a(), Zt(), a),
-    Na = Da(() => k("div", {
+    tt = a => (Zt("data-v-ce8419ef"), a = a(), Jt(), a),
+    Na = tt(() => k("div", {
         class: "fullscreen-media-space"
     }, null, -1)),
     Ea = {
         class: "fullscreen-row-centered"
     },
     La = {
         class: "fullscreen-row"
     },
     Wa = {
         key: 0,
         class: "fullscreen-track-info"
     },
-    Ha = {
-        key: 0,
-        class: "fullscreen-track-info-subtitle"
-    },
     Ra = {
-        key: 1,
+        key: 2
+    },
+    Ha = {
         class: "fullscreen-track-info-subtitle"
     },
     Aa = {
-        key: 2,
+        key: 3,
+        style: {
+            cursor: "pointer"
+        },
+        class: "line-clamp-1"
+    },
+    qa = tt(() => k("br", null, null, -1)),
+    Ua = tt(() => k("br", null, null, -1)),
+    Fa = {
+        key: 4,
         class: "fullscreen-track-info-subtitle"
     },
-    qa = {
-        key: 3,
+    Oa = {
+        key: 5,
         class: "fullscreen-track-info-subtitle"
     },
-    Ua = {
-        key: 4,
+    Ya = {
+        key: 6,
         class: "fullscreen-track-info-subtitle"
     },
-    Fa = {
+    Ga = {
         class: "fullscreen-row",
         style: {
             margin: "0 10px"
         }
     };
-const Oa = {
+const ja = {
         class: "fullscreen-row"
     },
-    Ya = {
+    Xa = {
         key: 1,
         class: "fullscreen-media-controls"
     },
-    Ga = {
+    Ka = {
         class: "media-controls-item",
         style: {
             display: "grid",
             "align-content": "center"
         }
     },
-    ja = {
+    Za = {
         class: "media-controls-item fullscreen-row-centered"
     },
-    Ka = {
+    Ja = {
         style: {
             width: "100%"
         }
     },
-    Xa = {
+    eo = {
         class: "fullscreen-mediacontrols-right media-controls-item"
     },
-    Za = {
+    to = {
         class: "fullscreen-media-controls-bottom",
         if: "store.activePlayerQueue"
     },
-    Ja = {
+    lo = {
         key: 0
     },
-    eo = {
+    ao = {
         class: "line-clamp-1"
     },
-    to = {
+    oo = {
         style: {
             "text-align": "end"
         }
     },
-    lo = M({
+    io = D({
         __name: "PlayerFullscreen",
         props: {
             colorPalette: {}
         },
         setup(a) {
             const l = a,
-                u = T(""),
-                o = T(),
-                i = S(() => {
+                u = S(""),
+                o = S(),
+                i = x(() => {
                     if (t.selectedPlayer) return t.selectedPlayer.group_childs
                 }),
-                s = S(() => ee.theme.current.value.dark ? ne : ue),
-                n = function(f) {
-                    Pe.push({
+                s = x(() => te.theme.current.value.dark ? re : ce),
+                n = function(m) {
+                    ne.push({
                         name: "track",
                         params: {
-                            itemId: f.item_id,
-                            provider: f.provider
+                            itemId: m.item_id,
+                            provider: m.provider
                         }
                     }), t.showFullscreenPlayer = !1
                 },
-                v = function(f) {
-                    Pe.push({
+                p = function(m) {
+                    ne.push({
                         name: "artist",
                         params: {
-                            itemId: f.item_id,
-                            provider: f.provider
+                            itemId: m.item_id,
+                            provider: m.provider
+                        }
+                    }), t.showFullscreenPlayer = !1
+                },
+                _ = function(m) {
+                    ne.push({
+                        name: "album",
+                        params: {
+                            itemId: m.item_id,
+                            provider: m.provider
+                        }
+                    }), t.showFullscreenPlayer = !1
+                },
+                y = function(m) {
+                    ne.push({
+                        name: "radio",
+                        params: {
+                            itemId: m.item_id,
+                            provider: m.provider
                         }
                     }), t.showFullscreenPlayer = !1
                 };
-            return W(() => t.curQueueItem, async f => {
-                f && f.media_item && f.media_item.media_type === te.TRACK && (o.value = await w.getItemByUri(f.media_item.uri))
-            }), W(() => l.colorPalette, f => {
-                !f.darkColor || !f.lightColor ? u.value = ee.theme.current.value.dark ? "#000" : "#fff" : u.value = ee.theme.current.value.dark ? f.darkColor : f.lightColor
-            }), (f, c) => (d(), V(et, {
+            return W(() => t.curQueueItem, async m => {
+                m && m.media_item && m.media_item.media_type === Z.TRACK && (o.value = await w.getItemByUri(m.media_item.uri))
+            }), W(() => l.colorPalette, m => {
+                !m.darkColor || !m.lightColor ? u.value = te.theme.current.value.dark ? "#000" : "#fff" : u.value = te.theme.current.value.dark ? m.darkColor : m.lightColor
+            }), (m, c) => (d(), V(et, {
                 modelValue: e(t).showFullscreenPlayer,
-                "onUpdate:modelValue": c[4] || (c[4] = _ => e(t).showFullscreenPlayer = _),
+                "onUpdate:modelValue": c[6] || (c[6] = v => e(t).showFullscreenPlayer = v),
                 fullscreen: "",
                 scrim: !1,
                 style: {
                     overflow: "hidden"
                 },
                 transition: "dialog-bottom-transition"
             }, {
-                default: y(() => [r(Qe, {
+                default: f(() => [r(Se, {
                     color: e(Kt)(u.value, 77, 40)
                 }, {
-                    default: y(() => [r(Je, {
+                    default: f(() => [r(Je, {
                         class: "v-toolbar-default",
                         color: "transparent"
                     }, {
-                        prepend: y(() => [r(Y, {
+                        prepend: f(() => [r(Y, {
                             icon: "",
-                            onClick: c[0] || (c[0] = _ => e(t).showFullscreenPlayer = !1)
+                            onClick: c[0] || (c[0] = v => e(t).showFullscreenPlayer = !1)
                         }, {
-                            default: y(() => [r(N, {
+                            default: f(() => [r(E, {
                                 icon: "mdi-chevron-down"
                             })]),
                             _: 1
                         })]),
                         _: 1
-                    }), r(il, {
+                    }), r(sl, {
                         class: "fullscreen-container"
                     }, {
-                        default: y(() => {
-                            var p, m, h, g, P, D, B, F, O, Z;
-                            return [Na, k("div", Ea, [(e(t).curQueueItem && e(C)({
+                        default: f(() => {
+                            var h, g, C, N, z, F, O, J, T, Q;
+                            return [Na, k("div", Ea, [(e(t).curQueueItem && e(P)({
                                 breakpoint: "mobile"
-                            }) && e(C)({
+                            }) && e(P)({
                                 breakpoint: "bp3",
                                 condition: "lt"
                             }), e(t).curQueueItem ? (d(), V(Ze, {
                                 key: 1,
                                 item: e(t).curQueueItem.media_item || e(t).curQueueItem,
-                                width: e(C)({
+                                width: e(P)({
                                     breakpoint: "bp3",
                                     condition: "lt"
                                 }) ? 512 : 1024,
-                                height: e(C)({
+                                height: e(P)({
                                     breakpoint: "bp3",
                                     condition: "lt"
                                 }) ? 512 : 1024,
                                 style: {
                                     height: "min(calc(100vw - 40px), calc(100vh - 340px))",
                                     width: "min(calc(100vw - 40px), calc(100vh - 340px))"
                                 }
-                            }, null, 8, ["item", "width", "height"])) : (d(), V(Pt, {
+                            }, null, 8, ["item", "width", "height"])) : (d(), V(Ct, {
                                 key: 2,
                                 src: s.value,
                                 style: {
                                     height: "min(calc(100vw - 40px), calc(100vh - 340px))",
                                     width: "min(calc(100vw - 40px), calc(100vh - 340px))"
                                 }
-                            }, null, 8, ["src"])))]), k("div", La, [e(t).curQueueItem && e(t).curQueueItem.media_item ? (d(), b("div", Wa, [k("h2", {
+                            }, null, 8, ["src"])))]), k("div", La, [e(t).curQueueItem && e(t).curQueueItem.media_item ? (d(), b("div", Wa, [(h = e(t).curQueueItem) != null && h.media_item && ((g = e(t).curQueueItem.media_item) == null ? void 0 : g.media_type) == e(Z).RADIO ? (d(), b("h2", {
+                                key: 0,
                                 style: {
                                     cursor: "pointer",
                                     width: "fit-content",
                                     display: "inline"
                                 },
                                 class: "title line-clamp-1",
-                                onClick: c[1] || (c[1] = Q => {
-                                    var x;
-                                    return (x = e(t).curQueueItem) != null && x.media_item ? n(e(t).curQueueItem.media_item) : ""
+                                onClick: c[1] || (c[1] = B => {
+                                    var M;
+                                    return (M = e(t).curQueueItem) != null && M.media_item ? y(e(t).curQueueItem.media_item) : ""
                                 })
-                            }, $(`${e(t).curQueueItem.media_item.name} ${"version"in e(t).curQueueItem.media_item&&e(t).curQueueItem.media_item.version?"("+e(t).curQueueItem.media_item.version+")":""}`), 1), ((p = e(t).curQueueItem.media_item) == null ? void 0 : p.media_type) == e(te).TRACK && "album" in e(t).curQueueItem.media_item && e(t).curQueueItem.media_item.album ? (d(), b("div", {
-                                key: 0,
+                            }, $(e(t).curQueueItem.media_item.name), 1)) : (d(), b("h2", {
+                                key: 1,
                                 style: {
-                                    cursor: "pointer"
+                                    cursor: "pointer",
+                                    width: "fit-content",
+                                    display: "inline"
                                 },
-                                class: "line-clamp-1",
-                                onClick: c[2] || (c[2] = Q => {
-                                    var x;
-                                    return (x = e(t).curQueueItem) != null && x.media_item ? v(e(t).curQueueItem.media_item.artists[0]) : ""
+                                class: "title line-clamp-1",
+                                onClick: c[2] || (c[2] = B => {
+                                    var M;
+                                    return (M = e(t).curQueueItem) != null && M.media_item ? n(e(t).curQueueItem.media_item) : ""
                                 })
-                            }, [e(t).curQueueItem.media_item && ((m = e(t).curQueueItem.media_item) == null ? void 0 : m.media_type) == e(te).TRACK && e(t).curQueueItem.media_item.artists.length > 0 ? (d(), b("h4", Ha, $(e(t).curQueueItem.media_item.artists[0].name), 1)) : (g = (h = e(t).curQueueItem) == null ? void 0 : h.streamdetails) != null && g.stream_title ? (d(), b("h4", Ra, $((D = (P = e(t).curQueueItem) == null ? void 0 : P.streamdetails) == null ? void 0 : D.stream_title), 1)) : e(t).curQueueItem && ((B = e(t).curQueueItem.media_item) != null && B.metadata.description) ? (d(), b("h4", Aa, $(e(t).curQueueItem.media_item.metadata.description), 1)) : e(t).activePlayerQueue && e(t).activePlayerQueue.items == 0 ? (d(), b("h4", qa, $(f.$t("queue_empty")), 1)) : ((F = e(t).selectedPlayer) == null ? void 0 : F.active_source) != ((O = e(t).selectedPlayer) == null ? void 0 : O.player_id) ? (d(), b("h4", Ua, $(f.$t("external_source_active", [(Z = e(t).selectedPlayer) == null ? void 0 : Z.active_source])), 1)) : I("", !0)])) : I("", !0)])) : I("", !0)]), k("div", Fa, [r(We, {
+                            }, $(`${e(t).curQueueItem.media_item.name} ${"version"in e(t).curQueueItem.media_item&&e(t).curQueueItem.media_item.version?"("+e(t).curQueueItem.media_item.version+")":""}`), 1)), ((C = e(t).curQueueItem.media_item) == null ? void 0 : C.media_type) == e(Z).RADIO && ((z = (N = e(t).curQueueItem) == null ? void 0 : N.streamdetails) != null && z.stream_title) ? (d(), b("div", Ra, [k("h4", Ha, $(e(t).curQueueItem.streamdetails.stream_title), 1)])) : ((F = e(t).curQueueItem.media_item) == null ? void 0 : F.media_type) == e(Z).TRACK && "artists" in e(t).curQueueItem.media_item && e(t).curQueueItem.media_item.artists ? (d(), b("div", Aa, [k("h4", null, ["album" in e(t).curQueueItem.media_item && e(t).curQueueItem.media_item.album ? (d(), b("span", {
+                                key: 0,
+                                class: "fullscreen-track-info-subtitle",
+                                onClick: c[3] || (c[3] = B => _(e(t).curQueueItem.media_item.album))
+                            }, $(e(t).curQueueItem.media_item.album.name), 1)) : I("", !0), k("span", {
+                                class: "fullscreen-track-info",
+                                onClick: c[4] || (c[4] = B => p(e(t).curQueueItem.media_item.artists[0]))
+                            }, [qa, Ua, G($(e(t).curQueueItem.media_item.artists[0].name), 1)])])])) : e(t).curQueueItem && ((O = e(t).curQueueItem.media_item) != null && O.metadata.description) ? (d(), b("h4", Fa, $(e(t).curQueueItem.media_item.metadata.description), 1)) : e(t).activePlayerQueue && e(t).activePlayerQueue.items == 0 ? (d(), b("h4", Oa, $(m.$t("queue_empty")), 1)) : ((J = e(t).selectedPlayer) == null ? void 0 : J.active_source) != ((T = e(t).selectedPlayer) == null ? void 0 : T.player_id) ? (d(), b("h4", Ya, $(m.$t("external_source_active", [(Q = e(t).selectedPlayer) == null ? void 0 : Q.active_source])), 1)) : I("", !0)])) : I("", !0)]), k("div", Ga, [r(We, {
                                 "is-progress-bar": !1,
-                                color: f.$vuetify.theme.current.dark ? l.colorPalette.lightColor : l.colorPalette.darkColor
-                            }, null, 8, ["color"])]), I("", !0), k("div", Oa, [e(C)({
+                                color: m.$vuetify.theme.current.dark ? l.colorPalette.lightColor : l.colorPalette.darkColor
+                            }, null, 8, ["color"])]), I("", !0), k("div", ja, [e(P)({
                                 breakpoint: "bp3",
                                 condition: "lt"
-                            }) ? (d(), V(ke, {
+                            }) ? (d(), V(we, {
                                 key: 0,
                                 queue: {
                                     isVisible: !1
                                 },
                                 player: {
                                     isVisible: !1
                                 },
                                 volume: {
                                     isVisible: !0,
                                     volumeSize: "100%",
                                     responsiveVolumeSize: !1
                                 }
-                            })) : I("", !0)]), e(C)({
+                            })) : I("", !0)]), e(P)({
                                 breakpoint: "bp3",
                                 condition: "lt"
-                            }) ? (d(), b("div", Ya, [r(St, {
+                            }) ? (d(), b("div", Xa, [r(St, {
                                 class: "media-controls-item",
                                 "max-height": "24px"
-                            }), r(Tt, {
+                            }), r(Bt, {
                                 class: "media-controls-item",
                                 "max-height": "35px"
-                            }), r(Qt, {
+                            }), r(Tt, {
                                 class: "media-controls-item",
                                 "max-height": "80px"
-                            }), r(Bt, {
+                            }), r(Mt, {
                                 class: "media-controls-item",
                                 "max-height": "35px"
-                            }), r(xt, {
+                            }), r(Qt, {
                                 class: "media-controls-item",
                                 "max-height": "24px"
                             })])) : (d(), b("div", {
                                 key: 2,
                                 class: "fullscreen-media-controls",
                                 style: L({
                                     paddingTop: "1vh",
-                                    flex: e(C)({
+                                    flex: e(P)({
                                         breakpoint: "bp3",
                                         condition: "lt"
                                     }) ? "1 1 auto" : "0 1 auto"
                                 })
-                            }, [k("div", Ga, [r(Pl)]), k("div", ja, [k("div", Ka, [r($e, {
+                            }, [k("div", Ka, [r(Cl)]), k("div", Za, [k("div", Ja, [r($e, {
                                 "visible-components": {
                                     repeat: {
-                                        isVisible: e(C)("bp3")
+                                        isVisible: e(P)("bp3")
                                     },
                                     shuffle: {
-                                        isVisible: e(C)("bp3")
+                                        isVisible: e(P)("bp3")
                                     },
                                     play: {
                                         isVisible: !0,
                                         icon: {
                                             staticWidth: "50px",
                                             staticHeight: "50px"
                                         }
                                     },
                                     previous: {
-                                        isVisible: e(C)("bp3")
+                                        isVisible: e(P)("bp3")
                                     },
                                     next: {
-                                        isVisible: e(C)("bp3")
+                                        isVisible: e(P)("bp3")
                                     }
                                 }
-                            }, null, 8, ["visible-components"])])]), k("div", Xa, [k("div", null, [r($e, {
+                            }, null, 8, ["visible-components"])])]), k("div", eo, [k("div", null, [r($e, {
                                 style: {
                                     "padding-right": "5px"
                                 },
                                 "visible-components": {
                                     repeat: {
                                         isVisible: !1
                                     },
                                     shuffle: {
                                         isVisible: !1
                                     },
                                     play: {
-                                        isVisible: e(C)({
+                                        isVisible: e(P)({
                                             breakpoint: "bp3",
                                             condition: "lt"
                                         })
                                     },
                                     previous: {
                                         isVisible: !1
                                     },
                                     next: {
                                         isVisible: !1
                                     }
                                 }
-                            }, null, 8, ["visible-components"]), r(ke, {
+                            }, null, 8, ["visible-components"]), r(we, {
                                 queue: {
-                                    isVisible: e(C)("bp3")
+                                    isVisible: e(P)("bp3")
                                 },
                                 player: {
                                     isVisible: !0
                                 },
                                 volume: {
-                                    isVisible: e(C)("bp0")
+                                    isVisible: e(P)("bp0")
                                 }
-                            }, null, 8, ["queue", "volume"])])])], 4)), k("div", Za, [e(C)({
+                            }, null, 8, ["queue", "volume"])])])], 4)), k("div", to, [e(P)({
                                 breakpoint: "bp3",
                                 condition: "lt"
-                            }) ? (d(), b("div", Ja, [r(Y, {
-                                onClick: c[3] || (c[3] = Q => e(t).showPlayersMenu = !0)
+                            }) ? (d(), b("div", lo, [r(Y, {
+                                onClick: c[5] || (c[5] = B => e(t).showPlayersMenu = !0)
                             }, {
-                                default: y(() => {
-                                    var Q, x;
-                                    return [i.value && i.value.length > 0 ? (d(), V(Ct, {
+                                default: f(() => {
+                                    var B, M;
+                                    return [i.value && i.value.length > 0 ? (d(), V(Vt, {
                                         key: 0,
-                                        content: (Q = e(t).selectedPlayer) == null ? void 0 : Q.group_childs.length,
-                                        color: f.$vuetify.theme.current.dark ? l.colorPalette.lightColor : l.colorPalette.darkColor
+                                        content: (B = e(t).selectedPlayer) == null ? void 0 : B.group_childs.length,
+                                        color: m.$vuetify.theme.current.dark ? l.colorPalette.lightColor : l.colorPalette.darkColor
                                     }, {
-                                        default: y(() => [r(N, {
+                                        default: f(() => [r(E, {
                                             size: 30
                                         }, {
-                                            default: y(() => [j("mdi-speaker")]),
+                                            default: f(() => [G("mdi-speaker")]),
                                             _: 1
                                         })]),
                                         _: 1
-                                    }, 8, ["content", "color"])) : (d(), V(N, {
+                                    }, 8, ["content", "color"])) : (d(), V(E, {
                                         key: 1,
                                         size: 30
                                     }, {
-                                        default: y(() => [j("mdi-speaker")]),
+                                        default: f(() => [G("mdi-speaker")]),
                                         _: 1
-                                    })), k("div", eo, $((x = e(t).activePlayerQueue) == null ? void 0 : x.display_name), 1)]
+                                    })), k("div", ao, $((M = e(t).activePlayerQueue) == null ? void 0 : M.display_name), 1)]
                                 }),
                                 _: 1
-                            })])) : I("", !0), k("div", to, [r(ke, {
+                            })])) : I("", !0), k("div", oo, [r(we, {
                                 queue: {
-                                    isVisible: e(C)({
+                                    isVisible: e(P)({
                                         breakpoint: "bp3",
                                         condition: "lt"
                                     })
                                 },
                                 player: {
                                     isVisible: !1
                                 },
@@ -2499,55 +2534,55 @@
                     })]),
                     _: 1
                 }, 8, ["color"])]),
                 _: 1
             }, 8, ["modelValue"]))
         }
     });
-const ao = xe(lo, [
-        ["__scopeId", "data-v-1ba8c187"]
+const so = xe(io, [
+        ["__scopeId", "data-v-ce8419ef"]
     ]),
-    oo = {
+    no = {
         key: 0
     },
-    io = {
+    ro = {
         key: 1
     },
-    so = {
+    uo = {
         key: 2
     },
-    no = {
+    co = {
         class: "d-flex justify-center",
         style: {
             width: "100%"
         }
     },
-    ro = {
+    mo = {
         key: 0
     },
-    uo = {
+    vo = {
         key: 1
     },
-    co = {
+    po = {
         key: 2,
         class: "line-clamp-1"
     },
-    mo = {
+    yo = {
         key: 3,
         class: "line-clamp-1"
     },
-    vo = {
+    fo = {
         key: 4,
         class: "line-clamp-1"
     },
-    po = {
+    ho = {
         key: 5,
         class: "line-clamp-1"
     },
-    yo = M({
+    _o = D({
         __name: "PlayerTrackDetails",
         props: {
             showOnlyArtist: {
                 type: Boolean,
                 default: !1
             },
             showQualityDetailsBtn: {
@@ -2556,209 +2591,209 @@
             },
             colorPalette: {},
             primaryColor: {
                 default: ""
             }
         },
         setup(a) {
-            Jt();
+            el();
             const l = a,
-                u = S(() => {
+                u = x(() => {
                     var o, i;
                     return (i = (o = t.activePlayerQueue) == null ? void 0 : o.current_item) == null ? void 0 : i.streamdetails
                 });
-            return (o, i) => (d(), V(K, {
+            return (o, i) => (d(), V(X, {
                 style: {
                     height: "auto",
                     width: "fit-content",
                     margin: "0px",
                     padding: "0px"
                 },
                 lines: "two"
             }, {
-                prepend: y(() => {
+                prepend: f(() => {
                     var s;
                     return [k("div", {
                         class: "media-thumb player-media-thumb",
-                        style: L(`height: ${e(C)({breakpoint:"phone"})?50:64}px; width: ${e(C)({breakpoint:"phone"})?50:64}px; `)
-                    }, [r(ao, {
+                        style: L(`height: ${e(P)({breakpoint:"phone"})?50:64}px; width: ${e(P)({breakpoint:"phone"})?50:64}px; `)
+                    }, [r(so, {
                         "show-fullscreen": e(t).showFullscreenPlayer,
                         "color-palette": o.colorPalette
                     }, null, 8, ["show-fullscreen", "color-palette"]), r(Ze, {
                         item: ((s = e(t).curQueueItem) == null ? void 0 : s.media_item) || e(t).curQueueItem,
-                        fallback: e(ne),
+                        fallback: e(re),
                         style: {
                             cursor: "pointer"
                         },
                         onClick: i[0] || (i[0] = n => e(t).showFullscreenPlayer = !0)
                     }, null, 8, ["item", "fallback"])], 4)]
                 }),
-                title: y(() => {
+                title: f(() => {
                     var s;
                     return [k("div", {
                         style: L({
                             cursor: "pointer",
                             color: o.primaryColor
                         })
                     }, [e(t).curQueueItem && e(t).curQueueItem.media_item ? (d(), b("div", {
                         key: 0,
                         onClick: i[1] || (i[1] = n => e(t).showFullscreenPlayer = !0)
-                    }, [j($(e(t).curQueueItem.media_item.name) + " ", 1), "version" in e(t).curQueueItem.media_item && e(t).curQueueItem.media_item.version ? (d(), b("span", oo, "(" + $(e(t).curQueueItem.media_item.version) + ")", 1)) : I("", !0)])) : e(t).curQueueItem ? (d(), b("div", io, $(e(t).curQueueItem.name), 1)) : (d(), b("div", so, $((s = e(t).activePlayerQueue) == null ? void 0 : s.display_name), 1))], 4)]
+                    }, [G($(e(t).curQueueItem.media_item.name) + " ", 1), "version" in e(t).curQueueItem.media_item && e(t).curQueueItem.media_item.version ? (d(), b("span", no, "(" + $(e(t).curQueueItem.media_item.version) + ")", 1)) : I("", !0)])) : e(t).curQueueItem ? (d(), b("div", ro, $(e(t).curQueueItem.name), 1)) : (d(), b("div", uo, $((s = e(t).activePlayerQueue) == null ? void 0 : s.display_name), 1))], 4)]
                 }),
-                append: y(() => {
-                    var s, n, v;
-                    return [(s = u.value) != null && s.audio_format.content_type && !e(C)({
+                append: f(() => {
+                    var s, n, p;
+                    return [(s = u.value) != null && s.audio_format.content_type && !e(P)({
                         breakpoint: "phone"
-                    }) && o.showQualityDetailsBtn ? (d(), V(Dl, H({
+                    }) && o.showQualityDetailsBtn ? (d(), V(Nl, R({
                         key: 0,
-                        disabled: !e(t).activePlayerQueue || !((n = e(t).activePlayerQueue) != null && n.active) || ((v = e(t).activePlayerQueue) == null ? void 0 : v.items) == 0,
+                        disabled: !e(t).activePlayerQueue || !((n = e(t).activePlayerQueue) != null && n.active) || ((p = e(t).activePlayerQueue) == null ? void 0 : p.items) == 0,
                         class: "player-track-content-type",
                         style: o.$vuetify.theme.current.dark ? "color: #000; background: #fff; margin-left: 15px;" : "color: #fff; background: #000; margin-left: 15px;",
                         label: "",
                         ripple: !1
                     }, l), {
-                        default: y(() => [k("div", no, $(u.value.audio_format.content_type.toUpperCase()), 1)]),
+                        default: f(() => [k("div", co, $(u.value.audio_format.content_type.toUpperCase()), 1)]),
                         _: 1
                     }, 16, ["disabled", "style"])) : I("", !0)]
                 }),
-                subtitle: y(() => {
-                    var s, n, v, f, c, _, p, m, h;
+                subtitle: f(() => {
+                    var s, n, p, _, y, m, c, v, h;
                     return [k("div", {
                         style: L({
                             cursor: "pointer",
                             color: o.primaryColor
                         }),
                         class: "line-clamp-1",
                         onClick: i[2] || (i[2] = g => e(t).showFullscreenPlayer = !0)
-                    }, [e(t).curQueueItem && ((s = e(t).curQueueItem.media_item) == null ? void 0 : s.media_type) == e(te).TRACK && "album" in e(t).curQueueItem.media_item && e(t).curQueueItem.media_item.album && !l.showOnlyArtist ? (d(), b("div", ro, $(e(el)(e(t).curQueueItem.media_item.artists)) + " • " + $(e(t).curQueueItem.media_item.album.name), 1)) : e(t).curQueueItem && e(t).curQueueItem.media_item && "artists" in e(t).curQueueItem.media_item && e(t).curQueueItem.media_item.artists.length > 0 ? (d(), b("div", uo, $(e(t).curQueueItem.media_item.artists[0].name), 1)) : (v = (n = e(t).curQueueItem) == null ? void 0 : n.streamdetails) != null && v.stream_title ? (d(), b("div", co, $((c = (f = e(t).curQueueItem) == null ? void 0 : f.streamdetails) == null ? void 0 : c.stream_title), 1)) : e(t).curQueueItem && ((_ = e(t).curQueueItem.media_item) != null && _.metadata.description) ? (d(), b("div", mo, $(e(t).curQueueItem.media_item.metadata.description), 1)) : e(t).activePlayerQueue && e(t).activePlayerQueue.items == 0 ? (d(), b("div", vo, $(o.$t("queue_empty")), 1)) : ((p = e(t).selectedPlayer) == null ? void 0 : p.active_source) != ((m = e(t).selectedPlayer) == null ? void 0 : m.player_id) ? (d(), b("div", po, $(o.$t("external_source_active", [(h = e(t).selectedPlayer) == null ? void 0 : h.active_source])), 1)) : I("", !0)], 4)]
+                    }, [e(t).curQueueItem && ((s = e(t).curQueueItem.media_item) == null ? void 0 : s.media_type) == e(Z).TRACK && "album" in e(t).curQueueItem.media_item && e(t).curQueueItem.media_item.album && !l.showOnlyArtist ? (d(), b("div", mo, $(e(tl)(e(t).curQueueItem.media_item.artists)) + " • " + $(e(t).curQueueItem.media_item.album.name), 1)) : e(t).curQueueItem && e(t).curQueueItem.media_item && "artists" in e(t).curQueueItem.media_item && e(t).curQueueItem.media_item.artists.length > 0 ? (d(), b("div", vo, $(e(t).curQueueItem.media_item.artists[0].name), 1)) : (p = (n = e(t).curQueueItem) == null ? void 0 : n.streamdetails) != null && p.stream_title ? (d(), b("div", po, $((y = (_ = e(t).curQueueItem) == null ? void 0 : _.streamdetails) == null ? void 0 : y.stream_title), 1)) : e(t).curQueueItem && ((m = e(t).curQueueItem.media_item) != null && m.metadata.description) ? (d(), b("div", yo, $(e(t).curQueueItem.media_item.metadata.description), 1)) : e(t).activePlayerQueue && e(t).activePlayerQueue.items == 0 ? (d(), b("div", fo, $(o.$t("queue_empty")), 1)) : ((c = e(t).selectedPlayer) == null ? void 0 : c.active_source) != ((v = e(t).selectedPlayer) == null ? void 0 : v.player_id) ? (d(), b("div", ho, $(o.$t("external_source_active", [(h = e(t).selectedPlayer) == null ? void 0 : h.active_source])), 1)) : I("", !0)], 4)]
                 }),
                 _: 1
             }))
         }
     });
-const fo = {
+const go = {
         style: {
             width: "100%"
         }
     },
-    ho = {
+    bo = {
         class: "mediacontrols-bottom-right"
     },
-    _o = M({
+    ko = D({
         __name: "Player",
         setup(a) {
-            const l = _t(),
-                u = T(),
-                o = T({
+            const l = gt(),
+                u = S(),
+                o = S({
                     0: "",
                     1: "",
                     2: "",
                     3: "",
                     4: "",
                     5: "",
                     lightColor: "",
                     darkColor: ""
                 }),
                 i = new Image;
-            i.src = ee.theme.current.value.dark ? ue : ne, i.crossOrigin = "Anonymous", i.addEventListener("load", function() {
-                o.value = tl(i), s(), u.value = ee.theme.current.value.dark ? o.value.darkColor : o.value.lightColor
+            i.src = te.theme.current.value.dark ? ce : re, i.crossOrigin = "Anonymous", i.addEventListener("load", function() {
+                o.value = ll(i), s(), u.value = te.theme.current.value.dark ? o.value.darkColor : o.value.lightColor
             }), W(() => {
                 var n;
                 return (n = t.curQueueItem) == null ? void 0 : n.queue_item_id
             }, () => {
                 var n;
-                (n = t.curQueueItem) != null && n.media_item ? i.src = mt(t.curQueueItem.media_item, ut.THUMB) || ee.theme.current.value.dark ? ue : ne : t.curQueueItem ? i.src = mt(t.curQueueItem, ut.THUMB) || ee.theme.current.value.dark ? ue : ne : i.src = ee.theme.current.value.dark ? ue : ne
+                (n = t.curQueueItem) != null && n.media_item ? i.src = vt(t.curQueueItem.media_item, ct.THUMB) || te.theme.current.value.dark ? ce : re : t.curQueueItem ? i.src = vt(t.curQueueItem, ct.THUMB) || te.theme.current.value.dark ? ce : re : i.src = te.theme.current.value.dark ? ce : re
             });
             const s = function() {
                 let n = l.themes.value.light,
-                    v = l.themes.value.dark;
-                n.colors["osd-primary"] = o.value.lightColor || n.colors.primary, n.colors["osd-on-primary"] = be(o.value.lightColor) || n.colors["on-primary"], n.colors["osd-secondary"] = o.value.darkColor || n.colors.secondary, n.colors["osd-on-secondary"] = be(o.value.darkColor) || n.colors["on-secondary"], v.colors["osd-primary"] = o.value.darkColor || v.colors.primary, v.colors["osd-on-primary"] = be(o.value.darkColor) || v.colors["on-primary"], v.colors["osd-secondary"] = o.value.lightColor || v.colors.secondary, v.colors["osd-on-secondary"] = be(o.value.lightColor) || v.colors["on-secondary"]
+                    p = l.themes.value.dark;
+                n.colors["osd-primary"] = o.value.lightColor || n.colors.primary, n.colors["osd-on-primary"] = ke(o.value.lightColor) || n.colors["on-primary"], n.colors["osd-secondary"] = o.value.darkColor || n.colors.secondary, n.colors["osd-on-secondary"] = ke(o.value.darkColor) || n.colors["on-secondary"], p.colors["osd-primary"] = o.value.darkColor || p.colors.primary, p.colors["osd-on-primary"] = ke(o.value.darkColor) || p.colors["on-primary"], p.colors["osd-secondary"] = o.value.lightColor || p.colors.secondary, p.colors["osd-on-secondary"] = ke(o.value.lightColor) || p.colors["on-secondary"]
             };
-            return (n, v) => {
-                const f = ll("breakpoint");
-                return d(), b(R, null, [u.value ? (d(), b("div", {
+            return (n, p) => {
+                const _ = al("breakpoint");
+                return d(), b(H, null, [u.value ? (d(), b("div", {
                     key: 0,
-                    class: ce(`mediacontrols-bg-${e(C)("bp3")?"1":"2"}`),
+                    class: de(`mediacontrols-bg-${e(P)("bp3")?"1":"2"}`),
                     style: L(`background: linear-gradient(90deg, ${u.value}${n.$vuetify.theme.current.dark?"4D":"B3"} 0%, ${u.value}00 100%);`)
-                }, null, 6)) : I("", !0), rt(r(We, {
+                }, null, 6)) : I("", !0), ut(r(We, {
                     color: n.$vuetify.theme.current.dark ? o.value.lightColor : o.value.darkColor,
                     "is-progress-bar": !0
                 }, null, 8, ["color"]), [
-                    [f, {
+                    [_, {
                         breakpoint: "bp3",
                         condition: "lt"
                     }]
                 ]), k("div", {
                     class: "mediacontrols",
-                    style: L(`padding: ${e(C)({breakpoint:"phone"})?3:10}px ${e(C)({breakpoint:"phone"}),10}px;`)
+                    style: L(`padding: ${e(P)({breakpoint:"phone"})?3:10}px ${e(P)({breakpoint:"phone"}),10}px;`)
                 }, [k("div", {
-                    class: ce(`mediacontrols-left-${e(C)("bp3")?"1":"2"}`)
-                }, [r(yo, {
-                    "show-quality-details-btn": !!e(C)("bp7"),
-                    "show-only-artist": !0,
+                    class: de(`mediacontrols-left-${e(P)("bp3")?"1":"2"}`)
+                }, [r(_o, {
+                    "show-quality-details-btn": !!e(P)("bp7"),
+                    "show-only-artist": !e(P)("bp7"),
                     "color-palette": o.value,
-                    "primary-color": !n.$vuetify.theme.current.dark && e(C)({
+                    "primary-color": !n.$vuetify.theme.current.dark && e(P)({
                         breakpoint: "bp3",
                         condition: "lt"
-                    }) || n.$vuetify.theme.current.dark && e(C)({
+                    }) || n.$vuetify.theme.current.dark && e(P)({
                         breakpoint: "bp3",
                         condition: "gt"
                     }) ? "#fff" : "#000"
-                }, null, 8, ["show-quality-details-btn", "color-palette", "primary-color"])], 2), k("div", {
-                    class: ce(`mediacontrols-bottom-center-${e(C)("bp3")?"1":"2"}`)
-                }, [k("div", fo, [r($e, {
+                }, null, 8, ["show-quality-details-btn", "show-only-artist", "color-palette", "primary-color"])], 2), k("div", {
+                    class: de(`mediacontrols-bottom-center-${e(P)("bp3")?"1":"2"}`)
+                }, [k("div", go, [r($e, {
                     "visible-components": {
                         repeat: {
-                            isVisible: e(C)("bp3")
+                            isVisible: e(P)("bp3")
                         },
                         shuffle: {
-                            isVisible: e(C)("bp3")
+                            isVisible: e(P)("bp3")
                         },
                         play: {
                             isVisible: !0,
                             icon: {
                                 staticWidth: "50px",
                                 staticHeight: "50px"
                             }
                         },
                         previous: {
-                            isVisible: e(C)("bp3")
+                            isVisible: e(P)("bp3")
                         },
                         next: {
-                            isVisible: e(C)("bp3")
+                            isVisible: e(P)("bp3")
                         }
                     }
-                }, null, 8, ["visible-components"]), rt(r(We, {
+                }, null, 8, ["visible-components"]), ut(r(We, {
                     color: n.$vuetify.theme.current.dark ? o.value.darkColor : o.value.lightColor,
                     "is-progress-bar": !1
                 }, null, 8, ["color"]), [
-                    [f, {
+                    [_, {
                         breakpoint: "mobile",
                         condition: "gt"
                     }]
-                ])])], 2), k("div", ho, [k("div", null, [r(ke, {
+                ])])], 2), k("div", bo, [k("div", null, [r(we, {
                     queue: {
-                        isVisible: e(C)("bp3")
+                        isVisible: e(P)("bp3")
                     },
                     player: {
                         isVisible: !0,
-                        color: !n.$vuetify.theme.current.dark && e(C)({
+                        color: !n.$vuetify.theme.current.dark && e(P)({
                             breakpoint: "bp3",
                             condition: "lt"
-                        }) || n.$vuetify.theme.current.dark && e(C)({
+                        }) || n.$vuetify.theme.current.dark && e(P)({
                             breakpoint: "bp3",
                             condition: "gt"
                         }) ? "#fff" : "#000"
                     },
                     volume: {
                         isVisible: !0,
-                        color: !n.$vuetify.theme.current.dark && e(C)({
+                        color: !n.$vuetify.theme.current.dark && e(P)({
                             breakpoint: "bp3",
                             condition: "lt"
-                        }) || n.$vuetify.theme.current.dark && e(C)({
+                        }) || n.$vuetify.theme.current.dark && e(P)({
                             breakpoint: "bp3",
                             condition: "gt"
                         }) ? "#fff" : "#000"
                     }
                 }, null, 8, ["queue", "player", "volume"]), r($e, {
                     style: {
                         "padding-right": "5px"
@@ -2767,26 +2802,26 @@
                         repeat: {
                             isVisible: !1
                         },
                         shuffle: {
                             isVisible: !1
                         },
                         play: {
-                            isVisible: e(C)({
+                            isVisible: e(P)({
                                 breakpoint: "bp3",
                                 condition: "lt"
                             }),
                             withCircle: !1,
                             icon: {
                                 staticWidth: "48px",
                                 staticHeight: "48px",
-                                color: !n.$vuetify.theme.current.dark && e(C)({
+                                color: !n.$vuetify.theme.current.dark && e(P)({
                                     breakpoint: "bp3",
                                     condition: "lt"
-                                }) || n.$vuetify.theme.current.dark && e(C)({
+                                }) || n.$vuetify.theme.current.dark && e(P)({
                                     breakpoint: "bp3",
                                     condition: "gt"
                                 }) ? "#fff" : "#000"
                             }
                         },
                         previous: {
                             isVisible: !1
@@ -2795,440 +2830,440 @@
                             isVisible: !1
                         }
                     }
                 }, null, 8, ["visible-components"])])])], 4)], 64)
             }
         }
     });
-const go = xe(_o, [
-    ["__scopeId", "data-v-de35313d"]
+const wo = xe(ko, [
+    ["__scopeId", "data-v-b841e61d"]
 ]);
-const bo = pe({
+const Po = ye({
         app: Boolean,
         color: String,
         height: {
             type: [Number, String],
             default: "auto"
         },
         ...Ue(),
-        ...fe(),
+        ...he(),
         ...Fe(),
-        ...Ke(),
+        ...Xe(),
         ...Oe(),
-        ...Se({
+        ...Qe({
             tag: "footer"
         }),
         ...Ie()
     }, "VFooter"),
-    ko = ye()({
+    Co = fe()({
         name: "VFooter",
-        props: bo(),
+        props: Po(),
         setup(a, l) {
             let {
                 slots: u
             } = l;
             const {
                 themeClasses: o
-            } = Re(a), {
+            } = He(a), {
                 backgroundColorClasses: i,
                 backgroundColorStyles: s
-            } = Ce(X(a, "color")), {
+            } = Ce(K(a, "color")), {
                 borderClasses: n
             } = Ye(a), {
-                elevationClasses: v
+                elevationClasses: p
             } = Ge(a), {
-                roundedClasses: f
-            } = je(a), c = ae(32), {
-                resizeRef: _
-            } = _l(h => {
-                h.length && (c.value = h[0].target.clientHeight)
-            }), p = S(() => a.height === "auto" ? c.value : parseInt(a.height, 10)), {
-                layoutItemStyles: m
-            } = Xe({
+                roundedClasses: _
+            } = je(a), y = ae(32), {
+                resizeRef: m
+            } = gl(h => {
+                h.length && (y.value = h[0].target.clientHeight)
+            }), c = x(() => a.height === "auto" ? y.value : parseInt(a.height, 10)), {
+                layoutItemStyles: v
+            } = Ke({
                 id: a.name,
-                order: S(() => parseInt(a.order, 10)),
-                position: S(() => "bottom"),
-                layoutSize: p,
-                elementSize: S(() => a.height === "auto" ? void 0 : p.value),
-                active: S(() => a.app),
-                absolute: X(a, "absolute")
+                order: x(() => parseInt(a.order, 10)),
+                position: x(() => "bottom"),
+                layoutSize: c,
+                elementSize: x(() => a.height === "auto" ? void 0 : c.value),
+                active: x(() => a.app),
+                absolute: K(a, "absolute")
             });
-            return he(() => r(a.tag, {
-                ref: _,
-                class: ["v-footer", o.value, i.value, n.value, v.value, f.value, a.class],
-                style: [s.value, a.app ? m.value : {
-                    height: we(a.height)
+            return _e(() => r(a.tag, {
+                ref: m,
+                class: ["v-footer", o.value, i.value, n.value, p.value, _.value, a.class],
+                style: [s.value, a.app ? v.value : {
+                    height: Pe(a.height)
                 }, a.style]
             }, u)), {}
         }
     }),
-    wo = M({
+    Vo = D({
         __name: "Footer",
         setup(a) {
-            const l = S(() => t.isInStandaloneMode ? 100 : 80),
-                u = S(() => C({
+            const l = x(() => t.isInStandaloneMode ? 100 : 80),
+                u = x(() => P({
                     breakpoint: "bp3",
                     condition: "lt"
                 }) ? l.value + 5 : 0);
-            return (o, i) => (d(), b(R, null, [e(C)({
+            return (o, i) => (d(), b(H, null, [e(P)({
                 breakpoint: "bp3",
                 condition: "lt"
-            }) ? (d(), V(sa, {
+            }) ? (d(), V(na, {
                 key: 0,
                 height: l.value
-            }, null, 8, ["height"])) : I("", !0), r(ko, {
+            }, null, 8, ["height"])) : I("", !0), r(Co, {
                 bottom: "",
                 fixed: "",
-                class: ce(`d-flex flex-column ${e(C)({breakpoint:"bp3",condition:"lt"})?"mediacontrols-player-float":"mediacontrols-player-default"}`),
+                class: de(`d-flex flex-column ${e(P)({breakpoint:"bp3",condition:"lt"})?"mediacontrols-player-float":"mediacontrols-player-default"}`),
                 style: L(`bottom: ${u.value}px;`),
                 elevation: "5",
                 app: "",
                 dark: !0
             }, {
-                default: y(() => [r(go)]),
+                default: f(() => [r(wo)]),
                 _: 1
             }, 8, ["class", "style"])], 64))
         }
     });
-const Po = {
+const $o = {
         key: 0,
         class: "text-body-2",
         style: {
             "line-height": "1em"
         }
     },
-    Co = {
+    Io = {
         key: 1,
         class: "text-body-2",
         style: {
             "line-height": "1em"
         }
     },
-    Vo = {
+    xo = {
         key: 2,
         class: "text-body-2",
         style: {
             "line-height": "1em"
         }
     },
-    $o = M({
+    Qo = D({
         __name: "PlayerSelect",
         setup(a) {
-            const l = T(void 0),
-                u = S(() => {
-                    var _, p;
-                    const c = [];
-                    for (const m in (_ = w) == null ? void 0 : _.players) {
-                        const h = (p = w) == null ? void 0 : p.players[m];
-                        n(h, !0) && c.push(h)
+            const l = S(void 0),
+                u = x(() => {
+                    var m, c;
+                    const y = [];
+                    for (const v in (m = w) == null ? void 0 : m.players) {
+                        const h = (c = w) == null ? void 0 : c.players[v];
+                        n(h, !0) && y.push(h)
                     }
-                    return c.slice().sort((m, h) => {
+                    return y.slice().sort((v, h) => {
                         var g;
-                        return m.display_name.toUpperCase() > ((g = h.display_name) == null ? void 0 : g.toUpperCase()) ? 1 : -1
+                        return v.display_name.toUpperCase() > ((g = h.display_name) == null ? void 0 : g.toUpperCase()) ? 1 : -1
                     })
                 });
-            W(() => t.showPlayersMenu, c => {
-                c || (l.value = void 0)
-            }), W(() => t.selectedPlayer, c => {
-                c && localStorage.setItem("mass.LastPlayerId", c.player_id)
-            }), W(() => w.players, c => {
-                c && v()
+            W(() => t.showPlayersMenu, y => {
+                y || (l.value = void 0)
+            }), W(() => t.selectedPlayer, y => {
+                y && localStorage.setItem("mass.LastPlayerId", y.player_id)
+            }), W(() => w.players, y => {
+                y && p()
             }, {
                 deep: !0
-            }), W(() => w.state, c => {
-                c.value != kt.CONNECTED && (t.selectedPlayerId = void 0)
+            }), W(() => w.state, y => {
+                y.value != wt.CONNECTED && (t.selectedPlayerId = void 0)
             }, {
                 deep: !0
             });
-            const o = T(),
-                i = T();
-            re(() => {
-                var c, _, p;
-                o.value = (p = (_ = (c = al()) == null ? void 0 : c.vnode) == null ? void 0 : _.el) == null ? void 0 : p.getRootNode(), v()
+            const o = S(),
+                i = S();
+            ue(() => {
+                var y, m, c;
+                o.value = (c = (m = (y = ol()) == null ? void 0 : y.vnode) == null ? void 0 : m.el) == null ? void 0 : c.getRootNode(), p()
             });
-            const s = function(c) {
-                    i.value != c && (i.value = c, setTimeout(() => {
-                        var p;
-                        const _ = (p = o.value) == null ? void 0 : p.getElementById(c);
-                        _ == null || _.scrollIntoView({
+            const s = function(y) {
+                    i.value != y && (i.value = y, setTimeout(() => {
+                        var c;
+                        const m = (c = o.value) == null ? void 0 : c.getElementById(y);
+                        m == null || m.scrollIntoView({
                             behavior: "smooth"
                         })
                     }, 0))
                 },
-                n = function(c, _ = !0, p = !1, m = !1) {
-                    return !(!c.enabled || !c.available && !_ || c.synced_to && !p || c.hidden && !m)
+                n = function(y, m = !0, c = !1, v = !1) {
+                    return !(!y.enabled || !y.available && !m || y.synced_to && !c || y.hidden && !v)
                 },
-                v = function() {
+                p = function() {
                     if (t.selectedPlayer && n(t.selectedPlayer, !1, !1, !1)) return;
-                    const c = f();
-                    c && (t.selectedPlayerId = c.player_id, console.log("Selected new default player: ", c.display_name))
+                    const y = _();
+                    y && (t.selectedPlayerId = y.player_id, console.log("Selected new default player: ", y.display_name))
                 },
-                f = function() {
-                    var _, p, m, h;
-                    const c = localStorage.getItem("mass.LastPlayerId");
-                    if (c && c in w.players && n(w.players[c], !1, !1, !1)) return w.players[c];
-                    if ((_ = w) != null && _.players) {
-                        for (const g in (p = w) == null ? void 0 : p.players) {
-                            const P = w.players[g];
-                            if (P.state == gt.PLAYING) return P
+                _ = function() {
+                    var m, c, v, h;
+                    const y = localStorage.getItem("mass.LastPlayerId");
+                    if (y && y in w.players && n(w.players[y], !1, !1, !1)) return w.players[y];
+                    if ((m = w) != null && m.players) {
+                        for (const g in (c = w) == null ? void 0 : c.players) {
+                            const C = w.players[g];
+                            if (C.state == bt.PLAYING) return C
                         }
-                        for (const g in (m = w) == null ? void 0 : m.queues) {
-                            const P = w.queues[g];
-                            if (n(w.players[g], !1, !1, !1) && P.items) return w.players[g]
+                        for (const g in (v = w) == null ? void 0 : v.queues) {
+                            const C = w.queues[g];
+                            if (n(w.players[g], !1, !1, !1) && C.items) return w.players[g]
                         }
                         for (const g in (h = w) == null ? void 0 : h.queues)
                             if (n(w.players[g], !1, !1, !1)) return w.players[g]
                     }
                 };
-            return (c, _) => (d(), V(It, {
+            return (y, m) => (d(), V(xt, {
                 modelValue: e(t).showPlayersMenu,
-                "onUpdate:modelValue": _[2] || (_[2] = p => e(t).showPlayersMenu = p),
+                "onUpdate:modelValue": m[2] || (m[2] = c => e(t).showPlayersMenu = c),
                 location: "right",
                 app: "",
                 clipped: "",
                 temporary: "",
                 touchless: "",
                 width: "290",
                 style: {
                     "z-index": "9999"
                 }
             }, {
-                default: y(() => [r($l, {
+                default: f(() => [r(Il, {
                     class: "headline"
                 }, {
-                    default: y(() => [k("b", null, $(c.$t("players")), 1)]),
+                    default: f(() => [k("b", null, $(y.$t("players")), 1)]),
                     _: 1
-                }), r(me, {
+                }), r(ve, {
                     variant: "plain",
                     style: {
                         position: "absolute",
                         right: "-10px",
                         top: "0px"
                     },
                     icon: "mdi-close",
                     dark: "",
-                    onClick: _[0] || (_[0] = p => e(t).showPlayersMenu = !e(t).showPlayersMenu)
-                }), r(le), r(Tl, {
+                    onClick: m[0] || (m[0] = c => e(t).showPlayersMenu = !e(t).showPlayersMenu)
+                }), r(le), r(Bl, {
                     modelValue: l.value,
-                    "onUpdate:modelValue": _[1] || (_[1] = p => l.value = p),
+                    "onUpdate:modelValue": m[1] || (m[1] = c => l.value = c),
                     focusable: "",
                     accordion: "",
                     flat: ""
                 }, {
-                    default: y(() => [(d(!0), b(R, null, U(u.value, p => (d(), V(Bl, {
-                        id: p.player_id,
-                        key: p.player_id,
-                        disabled: !p.available,
+                    default: f(() => [(d(!0), b(H, null, U(u.value, c => (d(), V(Ml, {
+                        id: c.player_id,
+                        key: c.player_id,
+                        disabled: !c.available,
                         flat: ""
                     }, {
-                        default: y(() => {
-                            var m;
-                            return [r(Ml, {
+                        default: f(() => {
+                            var v;
+                            return [r(zl, {
                                 class: "playerrow",
-                                style: L(((m = e(t).selectedPlayer) == null ? void 0 : m.player_id) == p.player_id ? "padding:0;" : "padding:0"),
+                                style: L(((v = e(t).selectedPlayer) == null ? void 0 : v.player_id) == c.player_id ? "padding:0;" : "padding:0"),
                                 "expand-icon": "mdi-chevron-down",
                                 "collapse-icon": "mdi-chevron-up",
                                 onClick: h => {
-                                    e(t).selectedPlayerId = p.player_id, s(p.player_id)
+                                    e(t).selectedPlayerId = c.player_id, s(c.player_id)
                                 }
                             }, {
-                                default: y(() => [r(K, null, {
-                                    prepend: y(() => [r(N, {
+                                default: f(() => [r(X, null, {
+                                    prepend: f(() => [r(E, {
                                         size: "50",
-                                        icon: p.icon,
+                                        icon: c.icon,
                                         color: "primary"
                                     }, null, 8, ["icon"])]),
-                                    title: y(() => [k("div", null, [k("b", null, $(e(Ae)(e(bt)(p), 20)), 1)])]),
-                                    subtitle: y(() => [p.powered ? p.active_source != p.player_id && e(w).queues[p.active_source] ? (d(), b("div", Co, $(c.$t("state." + p.state)) + " (" + $(e(w).queues[p.active_source].display_name) + ") ", 1)) : (d(), b("div", Vo, $(c.$t("state." + p.state)), 1)) : (d(), b("div", Po, $(c.$t("state.off")), 1))]),
+                                    title: f(() => [k("div", null, [k("b", null, $(e(Ae)(e(kt)(c), 20)), 1)])]),
+                                    subtitle: f(() => [c.powered ? c.active_source != c.player_id && e(w).queues[c.active_source] ? (d(), b("div", Io, $(y.$t("state." + c.state)) + " (" + $(e(w).queues[c.active_source].display_name) + ") ", 1)) : (d(), b("div", xo, $(y.$t("state." + c.state)), 1)) : (d(), b("div", $o, $(y.$t("state.off")), 1))]),
                                     _: 2
                                 }, 1024)]),
                                 _: 2
-                            }, 1032, ["style", "onClick"]), r(zl, {
+                            }, 1032, ["style", "onClick"]), r(Dl, {
                                 variant: "contain"
                             }, {
-                                default: y(() => [r(Mt, {
-                                    player: p
+                                default: f(() => [r(zt, {
+                                    player: c
                                 }, null, 8, ["player"])]),
                                 _: 2
                             }, 1024)]
                         }),
                         _: 2
                     }, 1032, ["id", "disabled"]))), 128))]),
                     _: 1
                 }, 8, ["modelValue"])]),
                 _: 1
             }, 8, ["modelValue"]))
         }
     });
 
-function Io(a = {}) {
+function So(a = {}) {
     const {
         immediate: l = !1,
         onNeedRefresh: u,
         onOfflineReady: o,
         onRegistered: i,
         onRegisteredSW: s,
         onRegisterError: n
     } = a;
-    let v, f, c;
-    const _ = async (m = !0) => {
-        await f, await (c == null ? void 0 : c())
+    let p, _, y;
+    const m = async (v = !0) => {
+        await _, await (y == null ? void 0 : y())
     };
-    async function p() {
+    async function c() {
         if ("serviceWorker" in navigator) {
-            if (v = await ol(() => import("./workbox-window.prod.es5-a7b12eab.js"), [], import.meta.url).then(({
-                    Workbox: m
-                }) => new m("./sw.js", {
+            if (p = await il(() => import("./workbox-window.prod.es5-a7b12eab.js"), [], import.meta.url).then(({
+                    Workbox: v
+                }) => new v("./sw.js", {
                     scope: "./",
                     type: "classic"
-                })).catch(m => {
-                    n == null || n(m)
-                }), !v) return;
-            c = async () => {
-                await (v == null ? void 0 : v.messageSkipWaiting())
+                })).catch(v => {
+                    n == null || n(v)
+                }), !p) return;
+            y = async () => {
+                await (p == null ? void 0 : p.messageSkipWaiting())
             };
             {
-                let m = !1;
+                let v = !1;
                 const h = () => {
-                    m = !0, v == null || v.addEventListener("controlling", g => {
+                    v = !0, p == null || p.addEventListener("controlling", g => {
                         g.isUpdate && window.location.reload()
                     }), u == null || u()
                 };
-                v.addEventListener("installed", g => {
-                    typeof g.isUpdate > "u" ? typeof g.isExternal < "u" ? g.isExternal ? h() : !m && (o == null || o()) : g.isExternal ? window.location.reload() : !m && (o == null || o()) : g.isUpdate || o == null || o()
-                }), v.addEventListener("waiting", h), v.addEventListener("externalwaiting", h)
+                p.addEventListener("installed", g => {
+                    typeof g.isUpdate > "u" ? typeof g.isExternal < "u" ? g.isExternal ? h() : !v && (o == null || o()) : g.isExternal ? window.location.reload() : !v && (o == null || o()) : g.isUpdate || o == null || o()
+                }), p.addEventListener("waiting", h), p.addEventListener("externalwaiting", h)
             }
-            v.register({
+            p.register({
                 immediate: l
-            }).then(m => {
-                s ? s("./sw.js", m) : i == null || i(m)
-            }).catch(m => {
-                n == null || n(m)
+            }).then(v => {
+                s ? s("./sw.js", v) : i == null || i(v)
+            }).catch(v => {
+                n == null || n(v)
             })
         }
     }
-    return f = p(), _
+    return _ = c(), m
 }
 
-function xo(a = {}) {
+function To(a = {}) {
     const {
         immediate: l = !0,
         onNeedRefresh: u,
         onOfflineReady: o,
         onRegistered: i,
         onRegisteredSW: s,
         onRegisterError: n
-    } = a, v = T(!1), f = T(!1);
+    } = a, p = S(!1), _ = S(!1);
     return {
-        updateServiceWorker: Io({
+        updateServiceWorker: So({
             immediate: l,
             onNeedRefresh() {
-                v.value = !0, u == null || u()
+                p.value = !0, u == null || u()
             },
             onOfflineReady() {
-                f.value = !0, o == null || o()
+                _.value = !0, o == null || o()
             },
             onRegistered: i,
             onRegisteredSW: s,
             onRegisterError: n
         }),
-        offlineReady: f,
-        needRefresh: v
+        offlineReady: _,
+        needRefresh: p
     }
 }
-const So = {
+const Bo = {
         key: 0,
         class: "pwa-toast",
         role: "alert"
     },
-    Qo = {
+    Mo = {
         class: "message"
     },
-    To = {
+    zo = {
         key: 0
     },
-    Bo = {
+    Do = {
         key: 1
     },
-    Mo = M({
+    No = D({
         __name: "ReloadPrompt",
         setup(a) {
             const {
                 offlineReady: l,
                 needRefresh: u,
                 updateServiceWorker: o
-            } = xo(), i = async () => {
+            } = To(), i = async () => {
                 l.value = !1, u.value = !1
             };
-            return (s, n) => e(l) || e(u) ? (d(), b("div", So, [k("div", Qo, [e(l) ? (d(), b("span", To, " App ready to work offline ")) : (d(), b("span", Bo, " New content available, click on reload button to update. "))]), e(u) ? (d(), b("button", {
+            return (s, n) => e(l) || e(u) ? (d(), b("div", Bo, [k("div", Mo, [e(l) ? (d(), b("span", zo, " App ready to work offline ")) : (d(), b("span", Do, " New content available, click on reload button to update. "))]), e(u) ? (d(), b("button", {
                 key: 0,
-                onClick: n[0] || (n[0] = v => e(o)())
+                onClick: n[0] || (n[0] = p => e(o)())
             }, "Reload")) : I("", !0), k("button", {
                 onClick: i
             }, "Close")])) : I("", !0)
         }
     });
-const zo = pe({
-        ...fe(),
-        ...kl({
+const Eo = ye({
+        ...he(),
+        ...wl({
             fullHeight: !0
         }),
         ...Ie()
     }, "VApp"),
-    Do = ye()({
+    Lo = fe()({
         name: "VApp",
-        props: zo(),
+        props: Eo(),
         setup(a, l) {
             let {
                 slots: u
             } = l;
-            const o = Re(a),
+            const o = He(a),
                 {
                     layoutClasses: i,
                     getLayoutItem: s,
                     items: n,
-                    layoutRef: v
-                } = wl(a),
+                    layoutRef: p
+                } = Pl(a),
                 {
-                    rtlClasses: f
-                } = yt();
-            return he(() => {
-                var c;
+                    rtlClasses: _
+                } = ft();
+            return _e(() => {
+                var y;
                 return r("div", {
-                    ref: v,
-                    class: ["v-application", o.themeClasses.value, i.value, f.value, a.class],
+                    ref: p,
+                    class: ["v-application", o.themeClasses.value, i.value, _.value, a.class],
                     style: [a.style]
                 }, [r("div", {
                     class: "v-application__wrap"
-                }, [(c = u.default) == null ? void 0 : c.call(u)])])
+                }, [(y = u.default) == null ? void 0 : y.call(u)])])
             }), {
                 getLayoutItem: s,
                 items: n,
                 theme: o
             }
         }
     }),
-    ti = M({
+    oi = D({
         __name: "Default",
         setup(a) {
-            return (l, u) => (d(), V(Do, null, {
-                default: y(() => [r($o), r(wo), e(w).state.value == e(kt).CONNECTED ? (d(), V(la, {
+            return (l, u) => (d(), V(Lo, null, {
+                default: f(() => [r(Qo), r(Vo), e(w).state.value == e(wt).CONNECTED ? (d(), V(aa, {
                     key: 0
-                })) : (d(), V(rl, {
+                })) : (d(), V(ul, {
                     key: 1
                 }, {
-                    default: y(() => [r(gl, {
+                    default: f(() => [r(bl, {
                         indeterminate: "",
                         size: "64"
                     })]),
                     _: 1
-                })), e(t).isInStandaloneMode ? (d(), V(Mo, {
+                })), e(t).isInStandaloneMode ? (d(), V(No, {
                     key: 2
                 })) : I("", !0)]),
                 _: 1
             }))
         }
     });
 export {
-    ti as
+    oi as
     default
 };
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/EditConfig-f2bca5b1.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditConfig-f2bca5b1.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-658131e8.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -37,66 +37,66 @@
     G as Ee,
     Q as H,
     N as O,
     x as f,
     I as ae,
     B as I,
     $ as T
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     a as ot,
     b as ut,
     c as ct,
     d as pt,
     V as ht
-} from "./VExpansionPanel-9f82eed8.js";
+} from "./VExpansionPanel-58c5fe02.js";
 import {
     P as dt,
     i as gt,
     j as kt,
     Q as ft,
     n as mt,
     R as bt,
     x as xt,
     l as X,
     k as wt
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     V as vt
-} from "./VForm-a7262390.js";
+} from "./VForm-fc99b4aa.js";
 import {
     V as $t,
     b as yt
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 import {
     V as Ae
-} from "./VCardText-00c669eb.js"; /* empty css              */
+} from "./VCardText-6774ea5e.js"; /* empty css              */
 import {
     h as Tt
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 import {
     V as Vt
-} from "./VDialog-82ed2e80.js";
+} from "./VDialog-d7e50927.js";
 import {
     m as Rt,
     d as zt,
     u as Ct,
     b as Le,
     e as qe,
     f as Pe
-} from "./VInput-91b2e758.js";
+} from "./VInput-5b197ccd.js";
 import {
     V as St
-} from "./VAlert-f74a2b4b.js";
+} from "./VAlert-56af8987.js";
 import {
     V as W
-} from "./VTextField-8883f272.js";
+} from "./VTextField-0c2ec62d.js";
 import {
     V as It
-} from "./VSelect-ea96d901.js";
+} from "./VSelect-d10e917f.js";
 const Et = Tt("v-spacer", "div", "VSpacer");
 const At = tt({
         indeterminate: Boolean,
         inset: Boolean,
         flat: Boolean,
         loading: {
             type: [Boolean, String],
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/EditCoreConfig-db86c453.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditCoreConfig-d27a9b35.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -10,44 +10,44 @@
     Q as c,
     N as u,
     x as d,
     z as p,
     B as i,
     I as f,
     L as n
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     _ as $
-} from "./EditConfig.vue_vue_type_style_index_0_lang-658131e8.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js";
 import {
     n as j
 } from "./index.browser-342e672c.js";
 import {
     a as E,
     V as O
-} from "./VCardText-00c669eb.js";
+} from "./VCardText-6774ea5e.js";
 import {
     a as v
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 import {
     k as h,
     x as S
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     f as T
-} from "./VMenu-9506155f.js";
-import "./VExpansionPanel-9f82eed8.js";
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VForm-a7262390.js"; /* empty css              */
-import "./VDialog-82ed2e80.js";
-import "./VAlert-f74a2b4b.js";
-import "./VTextField-8883f272.js";
-import "./VSelect-ea96d901.js";
-import "./VVirtualScroll-5f35af5d.js";
+} from "./VMenu-b634019c.js";
+import "./VExpansionPanel-58c5fe02.js";
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VForm-fc99b4aa.js"; /* empty css              */
+import "./VDialog-d7e50927.js";
+import "./VAlert-56af8987.js";
+import "./VTextField-0c2ec62d.js";
+import "./VSelect-d10e917f.js";
+import "./VVirtualScroll-84259ceb.js";
 const z = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/EditPlayer-293a9fdd.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditPlayer-6e04043d.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -10,41 +10,41 @@
     x as t,
     Q as p,
     N as r,
     B as i,
     I as d,
     z as m,
     L as l
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     V as I,
     _ as S
-} from "./EditConfig.vue_vue_type_style_index_0_lang-658131e8.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js";
 import {
     a as T,
     V as E
-} from "./VCardText-00c669eb.js";
+} from "./VCardText-6774ea5e.js";
 import {
     a as v
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 import {
     k
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     V as D
-} from "./VTextField-8883f272.js";
-import "./VExpansionPanel-9f82eed8.js";
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VMenu-9506155f.js";
-import "./VForm-a7262390.js"; /* empty css              */
-import "./VDialog-82ed2e80.js";
-import "./VAlert-f74a2b4b.js";
-import "./VSelect-ea96d901.js";
-import "./VVirtualScroll-5f35af5d.js";
+} from "./VTextField-0c2ec62d.js";
+import "./VExpansionPanel-58c5fe02.js";
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VMenu-b634019c.js";
+import "./VForm-fc99b4aa.js"; /* empty css              */
+import "./VDialog-d7e50927.js";
+import "./VAlert-56af8987.js";
+import "./VSelect-d10e917f.js";
+import "./VVirtualScroll-84259ceb.js";
 const U = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/EditProvider-b281ecba.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditProvider-e046ee5d.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -13,47 +13,47 @@
     A as d,
     x as i,
     Q as f,
     N as m,
     z as p,
     B as u,
     I as v
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     V as x,
     _ as I
-} from "./EditConfig.vue_vue_type_style_index_0_lang-658131e8.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js";
 import {
     n as P
 } from "./index.browser-342e672c.js";
 import {
     a as U,
     V as O
-} from "./VCardText-00c669eb.js";
+} from "./VCardText-6774ea5e.js";
 import {
     a as _
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 import {
     k as h,
     x as A
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     V as z
-} from "./VTextField-8883f272.js";
+} from "./VTextField-0c2ec62d.js";
 import {
     f as D
-} from "./VMenu-9506155f.js";
-import "./VExpansionPanel-9f82eed8.js";
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VForm-a7262390.js"; /* empty css              */
-import "./VDialog-82ed2e80.js";
-import "./VAlert-f74a2b4b.js";
-import "./VSelect-ea96d901.js";
-import "./VVirtualScroll-5f35af5d.js";
+} from "./VMenu-b634019c.js";
+import "./VExpansionPanel-58c5fe02.js";
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VForm-fc99b4aa.js"; /* empty css              */
+import "./VDialog-d7e50927.js";
+import "./VAlert-56af8987.js";
+import "./VSelect-d10e917f.js";
+import "./VVirtualScroll-84259ceb.js";
 const F = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/HomeView-aa005854.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/HomeView-8f9e6181.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     L as J,
     a as K,
     C as U
-} from "./Container-ba274a7a.js";
+} from "./Container-dc894acd.js";
 import {
     v as h,
     o as Z,
     R as I,
     y as a,
     z as v,
     A as r,
@@ -30,43 +30,43 @@
     Q as C,
     ab as ie,
     J as k,
     a2 as q,
     Z as ae,
     c as se,
     am as re
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     _ as oe
-} from "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
+} from "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
 import {
     i as ne,
     e as le
-} from "./contextmenu-c4231154.js";
+} from "./contextmenu-521b5304.js";
 import {
     n as R,
     l as ue,
     x as de
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     V as me,
     M as _e,
     i as ce
-} from "./VBadge-76d9c3a5.js";
+} from "./VBadge-84e3406b.js";
 import {
     V as Y
-} from "./VToolbar-4ad3b045.js";
+} from "./VToolbar-b7f10b15.js";
 import {
     V as pe
-} from "./VCard-bfc4071a.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VTooltip-a8719c72.js";
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCardText-00c669eb.js";
+} from "./VCard-b98fe47e.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VTooltip-3ef94159.js";
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCardText-6774ea5e.js";
 const j = h({
         __name: "Carousel",
         setup(b) {
             return Z(() => {
                 document.documentElement.style.setProperty("--swiper-navigation-color", "primary")
             }), (e, t) => {
                 const i = I("swiper");
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/HomeView-f9b96eef.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/HomeView-f9b96eef.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ItemsListing-5372ff4e.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ItemsListing-5372ff4e.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -40,44 +40,44 @@
     x as T,
     F as W,
     G as Q,
     M as yt,
     K as H,
     Z as ht,
     ak as gt
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     L as bt
-} from "./ListviewItem-e896b2dc.js";
+} from "./ListviewItem-8b992256.js";
 import {
     C as kt,
     B as E,
     _ as $e,
     L as te
-} from "./Container-ba274a7a.js";
+} from "./Container-dc894acd.js";
 import {
     _ as wt
-} from "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
+} from "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
 import {
     e as St,
     i as Ct,
     a as Bt
-} from "./contextmenu-c4231154.js";
+} from "./contextmenu-521b5304.js";
 import {
     A as _e
-} from "./Alert-0c4ec871.js";
+} from "./Alert-19e36349.js";
 import {
     V as Vt
-} from "./VToolbar-4ad3b045.js";
+} from "./VToolbar-b7f10b15.js";
 import {
     V as $t
-} from "./VTextField-8883f272.js";
+} from "./VTextField-0c2ec62d.js";
 import {
     V as ae
-} from "./VBadge-76d9c3a5.js";
+} from "./VBadge-84e3406b.js";
 import {
     a as Ee,
     d as Me,
     y as _t,
     z as It,
     c as Ft,
     A as At,
@@ -89,29 +89,29 @@
     E as Mt,
     v as Te,
     j as Tt,
     F as jt,
     n as P,
     k as le,
     l as oe
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     V as Ie
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 import {
     m as Rt,
     a as Dt,
     f as Fe,
     b as ne,
     e as se,
     d as Kt
-} from "./VMenu-9506155f.js"; /* empty css              */
+} from "./VMenu-b634019c.js"; /* empty css              */
 import {
     V as Ut
-} from "./VVirtualScroll-5f35af5d.js";
+} from "./VVirtualScroll-84259ceb.js";
 const je = (() => Y.reduce((t, r) => (t[r] = {
         type: [Boolean, String, Number],
         default: !1
     }, t), {}))(),
     Re = (() => Y.reduce((t, r) => {
         const a = "offset" + ie(r);
         return t[a] = {
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/JetBrainsMono-Medium-086c48df.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/JetBrainsMono-Medium-086c48df.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/LibraryAlbums-532f0c88.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryAlbums-7cfa0763.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,41 +1,41 @@
 import {
     _ as p
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
 import {
     v as u,
     r as c,
     o as y,
     L as e,
     an as s,
     b as _,
     y as f,
     z as d,
     x as b,
     M as n,
     ao as o,
     K as v
-} from "./index-6ff57e4c.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VToolbar-4ad3b045.js";
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
+} from "./index-b687f95a.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VToolbar-b7f10b15.js";
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
 const P = u({
     __name: "LibraryAlbums",
     setup(E) {
         const r = c(!1),
             i = {
                 name: "sort_name",
                 recent: "timestamp_added DESC",
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/LibraryArtists-17fa3e93.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PlaylistDetails-2fe134b1.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,75 +1,97 @@
 import {
-    _ as c
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
+    _ as v
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
 import {
-    v as f,
+    _ as y,
+    a as _
+} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js";
+import {
+    v as k,
     r as n,
-    o as y,
-    L as e,
-    an as i,
-    b as _,
-    y as d,
-    z as b,
-    x as v,
-    M as m,
-    ao as r,
-    K as h
-} from "./index-6ff57e4c.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VToolbar-4ad3b045.js";
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
-const F = f({
-    __name: "LibraryArtists",
-    setup(E) {
-        const p = n([]),
-            s = n(!1),
-            o = {
-                name: "sort_name",
-                recent: "timestamp_added DESC"
-            },
-            u = async function(t) {
-                if (t.refresh && !s.value) {
-                    for (e.startSync([m.ARTIST]), await r(250); e.syncTasks.value.length > 0 && e.syncTasks.value.filter(a => a.media_types.includes(m.ARTIST)).length != 0;) await r(500);
-                    await r(500)
-                }
-                return s.value = !1, await e.getLibraryArtists(t.favoritesOnly || void 0, t.search, t.limit, t.offset, o[t.sortBy], t.albumArtistsFilter)
+    w as b,
+    o as h,
+    L as r,
+    an as w,
+    b as I,
+    y as l,
+    E as D,
+    l as E,
+    z as p,
+    I as u,
+    ao as T
+} from "./index-b687f95a.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VToolbar-b7f10b15.js";
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
+import "./layout-42b7d22e.js";
+import "./VDialog-d7e50927.js";
+const S = k({
+    __name: "PlaylistDetails",
+    props: {
+        itemId: {},
+        provider: {}
+    },
+    setup(c) {
+        const a = c,
+            o = n(!1),
+            e = n(),
+            d = async function() {
+                e.value = await r.getPlaylist(a.itemId, a.provider)
             };
-        return y(() => {
-            const t = e.subscribe_multi([i.MEDIA_ITEM_ADDED, i.MEDIA_ITEM_UPDATED, i.MEDIA_ITEM_DELETED], a => {
-                var l;
-                (l = a.object_id) != null && l.startsWith("library://artist") && (s.value = !0)
+        b(() => a.itemId, t => {
+            t && d()
+        }, {
+            immediate: !0
+        }), h(() => {
+            const t = r.subscribe(w.MEDIA_ITEM_ADDED, i => {
+                var m;
+                const s = i.data;
+                ((m = e.value) == null ? void 0 : m.uri) == s.uri && (o.value = !0)
             });
-            _(t)
-        }), (t, a) => (d(), b(c, {
-            itemtype: "artists",
-            items: p.value,
+            I(t)
+        });
+        const f = async function(t) {
+            const i = [];
+            return await r.getPlaylistTracks(a.itemId, a.provider, s => {
+                i.push(...s)
+            }, t.refresh && !o.value), t.refresh && await T(100), o.value = !1, i
+        };
+        return (t, i) => (l(), D("section", null, [E(y, {
+            item: e.value
+        }, null, 8, ["item"]), e.value ? (l(), p(v, {
+            key: 0,
+            itemtype: "playlisttracks",
+            "parent-item": e.value,
             "show-provider": !1,
-            "show-favorites-only-filter": !0,
-            "load-paged-data": u,
-            "show-album-artists-only-filter": !0,
-            "update-available": s.value,
-            title: v(h)("bp4") ? t.$t("artists") : "",
-            "allow-key-hooks": !0,
-            "show-search-button": !0,
-            "sort-keys": Object.keys(o)
-        }, null, 8, ["items", "update-available", "title", "sort-keys"]))
+            "show-library": !1,
+            "show-favorites-only-filter": !1,
+            "show-track-number": !1,
+            "load-items": f,
+            "sort-keys": ["position", "position_desc", "name", "artist", "album", "duration", "duration_desc"],
+            "update-available": o.value,
+            title: t.$t("playlist_tracks"),
+            "allow-key-hooks": !0
+        }, null, 8, ["parent-item", "update-available", "title"])) : u("", !0), e.value ? (l(), p(_, {
+            key: 1,
+            "item-details": e.value
+        }, null, 8, ["item-details"])) : u("", !0)]))
     }
 });
 export {
-    F as
+    S as
     default
 };
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/LibraryPlaylists-a41d818d.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryPlaylists-95e35cdd.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
 import {
     v as d,
     O as v,
     r as o,
     o as b,
     L as s,
     P as h,
@@ -12,32 +12,32 @@
     b as E,
     y as w,
     z as T,
     x as I,
     M as u,
     ao as l,
     K as k
-} from "./index-6ff57e4c.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VToolbar-4ad3b045.js";
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
+} from "./index-b687f95a.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VToolbar-b7f10b15.js";
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
 const q = d({
     __name: "LibraryPlaylists",
     setup(A) {
         const {
             t: c
         } = v(), m = o([]), i = o(!1), n = o([]), p = {
             name: "sort_name",
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/LibraryRadios-e4468a3f.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryRadios-4a033696.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as y
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
 import {
     v as b,
     O as h,
     r as c,
     o as v,
     L as a,
     an as s,
@@ -13,32 +13,32 @@
     z as I,
     x as E,
     M as n,
     ao as l,
     ag as k,
     V as T,
     K as w
-} from "./index-6ff57e4c.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VToolbar-4ad3b045.js";
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
+} from "./index-b687f95a.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VToolbar-b7f10b15.js";
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
 const J = b({
     __name: "LibraryRadios",
     setup(A) {
         const {
             t: o
         } = h(), d = c([]), r = c(!1), m = {
             name: "sort_name",
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/LibraryTracks-a533acbe.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryTracks-eeccb967.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,42 +1,42 @@
 import {
     _
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
 import {
     v as f,
     O as y,
     r as m,
     o as b,
     L as a,
     an as s,
     b as k,
     y as v,
     z as h,
     x as T,
     M as i,
     ao as n,
     K as E
-} from "./index-6ff57e4c.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VToolbar-4ad3b045.js";
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
+} from "./index-b687f95a.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VToolbar-b7f10b15.js";
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
 const q = f({
     __name: "LibraryTracks",
     setup(D) {
         const {
             t: l
         } = y(), c = m([]), r = m(!1), u = {
             name: "sort_name",
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ListviewItem-e896b2dc.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ListviewItem-8b992256.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -21,35 +21,35 @@
     M as d,
     L as P,
     aI as S,
     aq as H,
     ab as k,
     K as B,
     W as z
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     M as E,
     b as O
-} from "./VBadge-76d9c3a5.js";
+} from "./VBadge-84e3406b.js";
 import {
     _ as K,
     L as U,
     a as W
-} from "./Container-ba274a7a.js";
+} from "./Container-dc894acd.js";
 import {
     a as q,
     c as y,
     b as G,
     _ as Q,
     V as _
-} from "./VTooltip-a8719c72.js";
+} from "./VTooltip-3ef94159.js";
 import {
     n as w,
     V as Y
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 const Z = {
         key: 0,
         class: "media-thumb listitem-media-thumb"
     },
     j = {
         key: 1,
         class: "media-thumb listitem-media-thumb"
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -18,40 +18,40 @@
     aI as M,
     Q as r,
     ab as N,
     aq as S,
     Z as D,
     K as L,
     H as z
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     M as A,
     b as H
-} from "./VBadge-76d9c3a5.js";
+} from "./VBadge-84e3406b.js";
 import {
     L as E
-} from "./Container-ba274a7a.js";
+} from "./Container-dc894acd.js";
 import {
     a as R,
     b as O,
     c as u,
     V as P,
     _ as q
-} from "./VTooltip-a8719c72.js";
+} from "./VTooltip-3ef94159.js";
 import {
     f as G,
     g as K,
     c as v
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 import {
     n as k
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     V as Q
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 const W = {
         key: 0
     },
     Z = {
         key: 1
     },
     j = {
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/PlayerQueue-42cde633.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PlayerQueue-9f89c917.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -23,63 +23,63 @@
     F as ie,
     G as ne,
     B as k,
     H as h,
     K as B,
     a3 as oe,
     M as re
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     L as se
-} from "./ListviewItem-e896b2dc.js";
+} from "./ListviewItem-8b992256.js";
 import {
     B as de,
     L as _,
     C as me
-} from "./Container-ba274a7a.js";
+} from "./Container-dc894acd.js";
 import {
     A as z
-} from "./Alert-0c4ec871.js";
+} from "./Alert-19e36349.js";
 import {
     V as D
-} from "./VBadge-76d9c3a5.js";
+} from "./VBadge-84e3406b.js";
 import {
     a as G,
     V as pe
-} from "./VTabs-4c128c89.js";
+} from "./VTabs-8ad24bfd.js";
 import {
     n as g,
     l as I,
     k as P
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     b as H,
     e as ve,
     d as b
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 import {
     V as J,
     a as O
-} from "./VToolbar-4ad3b045.js";
+} from "./VToolbar-b7f10b15.js";
 import {
     V as ce
-} from "./VVirtualScroll-5f35af5d.js";
+} from "./VVirtualScroll-84259ceb.js";
 import {
     V as fe
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 import {
     V as _e
-} from "./VCardText-00c669eb.js";
+} from "./VCardText-6774ea5e.js";
 import {
     V as ye
-} from "./VDialog-82ed2e80.js";
-import "./VTooltip-a8719c72.js";
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js"; /* empty css              */
-import "./VAlert-f74a2b4b.js";
+} from "./VDialog-d7e50927.js";
+import "./VTooltip-3ef94159.js";
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js"; /* empty css              */
+import "./VAlert-56af8987.js";
 const ge = k("br", null, null, -1),
     be = {
         key: 0
     },
     Se = Y({
         __name: "PlayerQueue",
         setup(qe) {
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Players-0c4ce7a2.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Players-0e31a251.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -19,35 +19,35 @@
     n as O,
     F as C,
     G as h,
     I as k,
     af as S,
     x as d,
     B as V
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     C as j,
     L as A,
     _ as E,
     B
-} from "./Container-ba274a7a.js";
+} from "./Container-dc894acd.js";
 import {
     l as Q,
     n as N
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     V as W
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 import {
     e as q
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 import {
     V as H
-} from "./VToolbar-4ad3b045.js"; /* empty css              */
-import "./VCardText-00c669eb.js";
+} from "./VToolbar-b7f10b15.js"; /* empty css              */
+import "./VCardText-6774ea5e.js";
 const J = {
         style: {
             "margin-bottom": "10px"
         }
     },
     K = {
         class: "line-clamp-1"
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/PlaylistDetails-9db516b0.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/RadioDetails-54e9e340.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,97 +1,95 @@
 import {
-    _ as v
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
+    _ as u
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
 import {
-    _ as y,
-    a as _
-} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js";
+    _ as f,
+    a as v
+} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js";
 import {
-    v as k,
-    r as n,
-    w as b,
-    o as h,
-    L as r,
-    an as w,
-    b as I,
-    y as l,
-    E as D,
-    l as E,
-    z as p,
-    I as u,
-    ao as T
-} from "./index-6ff57e4c.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VToolbar-4ad3b045.js";
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
-import "./layout-bdc1c8bd.js";
-import "./VDialog-82ed2e80.js";
-const S = k({
-    __name: "PlaylistDetails",
-    props: {
-        itemId: {},
-        provider: {}
-    },
-    setup(c) {
-        const a = c,
-            o = n(!1),
-            e = n(),
-            d = async function() {
-                e.value = await r.getPlaylist(a.itemId, a.provider)
-            };
-        b(() => a.itemId, t => {
-            t && d()
-        }, {
-            immediate: !0
-        }), h(() => {
-            const t = r.subscribe(w.MEDIA_ITEM_ADDED, i => {
-                var m;
-                const s = i.data;
-                ((m = e.value) == null ? void 0 : m.uri) == s.uri && (o.value = !0)
+    v as _,
+    r as h,
+    w as y,
+    y as a,
+    E as w,
+    l as V,
+    z as m,
+    I as n,
+    B as k,
+    L as s,
+    ap as g
+} from "./index-b687f95a.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VToolbar-b7f10b15.js";
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
+import "./layout-42b7d22e.js";
+import "./VDialog-d7e50927.js";
+const I = k("br", null, null, -1),
+    T = _({
+        __name: "RadioDetails",
+        props: {
+            itemId: {},
+            provider: {}
+        },
+        setup(p) {
+            const t = p,
+                e = h(),
+                l = async function() {
+                    e.value = await s.getRadio(t.itemId, t.provider)
+                };
+            y(() => t.itemId, i => {
+                i && l()
+            }, {
+                immediate: !0
             });
-            I(t)
-        });
-        const f = async function(t) {
-            const i = [];
-            return await r.getPlaylistTracks(a.itemId, a.provider, s => {
-                i.push(...s)
-            }, t.refresh && !o.value), t.refresh && await T(100), o.value = !1, i
-        };
-        return (t, i) => (l(), D("section", null, [E(y, {
-            item: e.value
-        }, null, 8, ["item"]), e.value ? (l(), p(v, {
-            key: 0,
-            itemtype: "playlisttracks",
-            "parent-item": e.value,
-            "show-provider": !1,
-            "show-library": !1,
-            "show-favorites-only-filter": !1,
-            "show-track-number": !1,
-            "load-items": f,
-            "sort-keys": ["position", "position_desc", "name", "artist", "album", "duration", "duration_desc"],
-            "update-available": o.value,
-            title: t.$t("playlist_tracks"),
-            "allow-key-hooks": !0
-        }, null, 8, ["parent-item", "update-available", "title"])) : u("", !0), e.value ? (l(), p(_, {
-            key: 1,
-            "item-details": e.value
-        }, null, 8, ["item-details"])) : u("", !0)]))
-    }
-});
+            const d = async function(i) {
+                const o = [];
+                if (t.provider == "library") {
+                    const r = await s.getRadioVersions(t.itemId, t.provider);
+                    o.push(...r)
+                }
+                for (const r of g(e.value)) {
+                    const c = await s.getRadioVersions(r.item_id, r.provider_instance);
+                    o.push(...c)
+                }
+                return o
+            };
+            return (i, o) => (a(), w("section", null, [V(f, {
+                item: e.value
+            }, null, 8, ["item"]), e.value ? (a(), m(u, {
+                key: 0,
+                itemtype: "radioversions",
+                "parent-item": e.value,
+                "show-provider": !0,
+                "show-favorites-only-filter": !1,
+                "show-library": !1,
+                "show-radio-number": !1,
+                "show-duration": !1,
+                "load-items": d,
+                "sort-keys": ["provider", "sort_name"],
+                title: i.$t("other_versions"),
+                "hide-on-empty": !0,
+                checksum: i.provider + i.itemId
+            }, null, 8, ["parent-item", "title", "checksum"])) : n("", !0), I, e.value ? (a(), m(v, {
+                key: 1,
+                "item-details": e.value
+            }, null, 8, ["item-details"])) : n("", !0)]))
+        }
+    });
 export {
-    S as
+    T as
     default
 };
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ProviderDetails-2713c080.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ProviderDetails-2713c080.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -26,69 +26,69 @@
     J as U,
     M as R,
     aq as ie,
     L as A,
     ar as ae,
     Z as oe,
     K as le
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     B as x,
     _ as Y,
     L as q,
     C as se
-} from "./Container-ba274a7a.js";
+} from "./Container-dc894acd.js";
 import {
     M as S,
     g as j,
     b as ne
-} from "./VBadge-76d9c3a5.js";
+} from "./VBadge-84e3406b.js";
 import {
     e as re,
     a as me
-} from "./contextmenu-c4231154.js";
+} from "./contextmenu-521b5304.js";
 import {
     a as de,
     i as ue,
     V as J,
     n as $,
     l as D,
     v as pe,
     k as ce
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     d as E,
     e as ye,
     b as O
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 import {
     a as fe,
     V as ge
-} from "./VCardText-00c669eb.js";
+} from "./VCardText-6774ea5e.js";
 import {
     a as V,
     V as K,
     b as ve
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 import {
     V as be
-} from "./VTooltip-a8719c72.js";
+} from "./VTooltip-3ef94159.js";
 import {
     b as he,
     c as ke
-} from "./layout-bdc1c8bd.js";
+} from "./layout-42b7d22e.js";
 import {
     V as Ce
-} from "./VDialog-82ed2e80.js";
+} from "./VDialog-d7e50927.js";
 import {
     V as _e
-} from "./VInput-91b2e758.js";
+} from "./VInput-5b197ccd.js";
 import {
     V as $e
-} from "./VToolbar-4ad3b045.js";
+} from "./VToolbar-b7f10b15.js";
 const Ve = W({
         ...de(),
         ...he()
     }, "VLayout"),
     we = Z()({
         name: "VLayout",
         props: Ve(),
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Providers-ca2eea9e.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Providers-58a591e0.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,40 +22,40 @@
     n as J,
     I as v,
     aQ as b,
     B as h,
     af as K,
     a8 as T,
     a9 as W
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     L as B,
     _ as S,
     B as g,
     C as X,
     a as Y
-} from "./Container-ba274a7a.js";
+} from "./Container-dc894acd.js";
 import {
     A as Z
-} from "./Alert-0c4ec871.js";
+} from "./Alert-19e36349.js";
 import {
     e as ee
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 import {
     l as ne,
     n as y
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     V as te
-} from "./VCard-bfc4071a.js";
+} from "./VCard-b98fe47e.js";
 import {
     V as ae
-} from "./VToolbar-4ad3b045.js"; /* empty css              */
-import "./VAlert-f74a2b4b.js";
-import "./VCardText-00c669eb.js";
+} from "./VToolbar-b7f10b15.js"; /* empty css              */
+import "./VAlert-56af8987.js";
+import "./VCardText-6774ea5e.js";
 const ie = p => (T("data-v-15cfe784"), p = p(), W(), p),
     se = ie(() => h("br", null, null, -1)),
     oe = {
         class: "line-clamp-1"
     },
     de = {
         class: "line-clamp-1"
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Search-abd54e1f.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Search-00ee9dd8.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,72 +1,73 @@
 import {
     V as $,
-    _ as S,
-    a as B
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
+    _ as B,
+    a as I
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
 import {
-    v as I,
+    v as F,
     r as o,
-    w as F,
-    o as L,
-    b as _,
+    w as L,
+    o as _,
+    b as C,
     y as i,
     E as f,
     l as c,
     A as v,
-    Q as C,
-    N as E,
-    F as y,
-    G as b,
-    L as N,
-    z as V,
-    I as R
-} from "./index-6ff57e4c.js";
+    Q as E,
+    N,
+    F as b,
+    G as V,
+    L as R,
+    z as g,
+    I as x
+} from "./index-b687f95a.js";
 import {
-    V as x
-} from "./VToolbar-4ad3b045.js";
+    V as D
+} from "./VToolbar-b7f10b15.js";
 import {
-    k as D
-} from "./forwardRefs-70e877d2.js";
+    k as P
+} from "./forwardRefs-7be90dc2.js";
 import {
-    V as P
-} from "./VTextField-8883f272.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VVirtualScroll-5f35af5d.js";
-const re = I({
+    V as U
+} from "./VTextField-0c2ec62d.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VVirtualScroll-84259ceb.js";
+const le = F({
     __name: "Search",
     props: {
         initSearch: {}
     },
-    setup(g) {
-        const p = g,
+    setup(w) {
+        const p = w,
             a = o(""),
+            d = o(""),
             n = o(!1),
             t = o(),
-            d = o(!1),
-            h = o();
-        F(() => a.value, () => {
-            clearTimeout(h.value), h.value = setTimeout(() => {
-                w()
+            h = o(!1),
+            k = o();
+        L(() => a.value, () => {
+            clearTimeout(k.value), k.value = setTimeout(() => {
+                S()
             }, 200)
         });
-        const w = async function() {
-            d.value = !0, localStorage.setItem("globalsearch", a.value), a.value ? t.value = await N.search(a.value) : t.value = void 0, d.value = !1
+        const S = async function() {
+            h.value = !0, localStorage.setItem("globalsearch", a.value), a.value ? t.value = await R.search(a.value) : t.value = void 0, h.value = !1, d.value = a.value
         }, m = function(e) {
             if (!t.value) return [];
             if (e == "artists") return t.value.artists;
             if (e == "albums") return t.value.albums;
             if (e == "tracks") return t.value.tracks;
             if (e == "playlists") return t.value.playlists;
             if (e == "radio") return t.value.radio;
@@ -76,72 +77,72 @@
                     const r = [];
                     for (const u of s) r.includes(u.provider) || (l.push(u), r.push(u.provider))
                 }
                 return l
             }
             return []
         };
-        L(() => {
+        _(() => {
             if (p.initSearch) a.value = p.initSearch;
             else {
                 const e = localStorage.getItem("globalsearch");
                 e && e !== "null" && (a.value = e)
             }
         });
-        const k = function(e) {
+        const y = function(e) {
             !n.value && e.key == "Backspace" ? a.value = a.value.slice(0, -1) : !n.value && e.key.length == 1 && (a.value += e.key)
         };
-        return document.addEventListener("keydown", k), _(() => {
-            document.removeEventListener("keydown", k)
-        }), (e, l) => (i(), f("section", null, [c(x, {
+        return document.addEventListener("keydown", y), C(() => {
+            document.removeEventListener("keydown", y)
+        }), (e, l) => (i(), f("section", null, [c(D, {
             variant: "flat",
             color: "transparent"
         }, {
-            title: v(() => [C(E(e.$t("search")), 1)]),
+            title: v(() => [E(N(e.$t("search")), 1)]),
             _: 1
-        }), c(D), c(P, {
+        }), c(P), c(U, {
             id: "searchInput",
             modelValue: a.value,
             "onUpdate:modelValue": l[0] || (l[0] = s => a.value = s),
             clearable: "",
             "prepend-inner-icon": "mdi-magnify",
             label: e.$t("type_to_search"),
             "hide-details": "",
             variant: "filled",
             onFocus: l[1] || (l[1] = s => n.value = !0),
             onBlur: l[2] || (l[2] = s => n.value = !1)
-        }, null, 8, ["modelValue", "label"]), (i(), f(y, null, b([
+        }, null, 8, ["modelValue", "label"]), (i(), f(b, null, V([
             ["topresult", "tracks"],
             ["artists", "albums"],
             ["playlists", "radio"]
-        ], s => c(B, {
+        ], s => c(I, {
             key: s[0] + s[1]
         }, {
-            default: v(() => [(i(!0), f(y, null, b(s.filter(r => m(r).length), r => (i(), V($, {
+            default: v(() => [(i(!0), f(b, null, V(s.filter(r => m(r).length), r => (i(), g($, {
                 key: r
             }, {
-                default: v(() => [m(r).length ? (i(), V(S, {
+                default: v(() => [m(r).length ? (i(), g(B, {
                     key: 0,
                     itemtype: `search.${r}`,
-                    path: `search.${a.value}`,
+                    path: `search.${d.value}`,
                     "show-provider": !0,
                     "show-favorites-only-filter": !1,
                     "show-select-button": !1,
                     "show-refresh-button": !1,
                     "load-items": async u => m(r),
                     title: e.$t(r),
                     "allow-key-hooks": !1,
                     "show-search-button": !1,
                     limit: 8,
                     "infinite-scroll": !1,
                     "sort-keys": ["original"]
-                }, null, 8, ["itemtype", "path", "load-items", "title"])) : R("", !0)]),
+                }, null, 8, ["itemtype", "path", "load-items", "title"])) : x("", !0)]),
                 _: 2
             }, 1024))), 128))]),
             _: 2
         }, 1024)), 64))]))
     }
 });
 export {
-    re as
+    le as
     default
 };
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/Settings-170b9c4c.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Settings-bbdb2168.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -10,26 +10,26 @@
     Q as o,
     N as s,
     x as _,
     z as V,
     S as y,
     B as h,
     K as b
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     V as B,
     a as n
-} from "./VTabs-4c128c89.js";
+} from "./VTabs-8ad24bfd.js";
 import {
     V as k
-} from "./VToolbar-4ad3b045.js";
+} from "./VToolbar-b7f10b15.js";
 import {
     k as S
-} from "./forwardRefs-70e877d2.js";
-import "./VSlideGroup-5dd0c6f2.js";
+} from "./forwardRefs-7be90dc2.js";
+import "./VSlideGroup-b576aa37.js";
 const T = h("div", {
         style: {
             height: "15px"
         }
     }, null, -1),
     x = d({
         __name: "Settings",
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/TrackDetails-6c6c6bec.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/TrackDetails-72029d5e.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     _ as d
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
 import {
     _ as w,
     a as I
-} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js";
+} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js";
 import {
     v as T,
     r as n,
     c as g,
     ap as c,
     w as D,
     o as A,
@@ -17,34 +17,34 @@
     b as E,
     y as l,
     E as M,
     l as V,
     z as u,
     I as p,
     B as f
-} from "./index-6ff57e4c.js";
-import "./ListviewItem-e896b2dc.js";
-import "./VBadge-76d9c3a5.js";
-import "./Container-ba274a7a.js";
-import "./forwardRefs-70e877d2.js";
-import "./VMenu-9506155f.js"; /* empty css              */
-import "./VInput-91b2e758.js";
-import "./VSlideGroup-5dd0c6f2.js";
-import "./VCard-bfc4071a.js";
-import "./VCardText-00c669eb.js";
-import "./VTooltip-a8719c72.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js";
-import "./contextmenu-c4231154.js";
-import "./Alert-0c4ec871.js";
-import "./VAlert-f74a2b4b.js";
-import "./VToolbar-4ad3b045.js";
-import "./VTextField-8883f272.js";
-import "./VVirtualScroll-5f35af5d.js";
-import "./layout-bdc1c8bd.js";
-import "./VDialog-82ed2e80.js";
+} from "./index-b687f95a.js";
+import "./ListviewItem-8b992256.js";
+import "./VBadge-84e3406b.js";
+import "./Container-dc894acd.js";
+import "./forwardRefs-7be90dc2.js";
+import "./VMenu-b634019c.js"; /* empty css              */
+import "./VInput-5b197ccd.js";
+import "./VSlideGroup-b576aa37.js";
+import "./VCard-b98fe47e.js";
+import "./VCardText-6774ea5e.js";
+import "./VTooltip-3ef94159.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+import "./contextmenu-521b5304.js";
+import "./Alert-19e36349.js";
+import "./VAlert-56af8987.js";
+import "./VToolbar-b7f10b15.js";
+import "./VTextField-0c2ec62d.js";
+import "./VVirtualScroll-84259ceb.js";
+import "./layout-42b7d22e.js";
+import "./VDialog-d7e50927.js";
 const $ = f("br", null, null, -1),
     F = f("br", null, null, -1),
     te = T({
         __name: "TrackDetails",
         props: {
             itemId: {},
             provider: {},
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VAlert-1c823677.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VAlert-1c823677.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VAlert-f74a2b4b.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VAlert-56af8987.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     h as I
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 import {
     a as L,
     o as $,
     T as z,
     b as E,
     y as F,
     z as R,
@@ -19,28 +19,28 @@
     C as U,
     g as G,
     J as H,
     E as K,
     n as Q,
     j as d,
     l as W
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     p as X,
     aL as Y,
     d as Z,
     g as ee,
     h as te,
     c as o,
     e as ae,
     t as le,
     aM as ne,
     l as a,
     n as se
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 const oe = I("v-alert-title"),
     re = ["success", "info", "warning", "error"],
     ie = X({
         border: {
             type: [Boolean, String],
             validator: e => typeof e == "boolean" || ["top", "end", "bottom", "start"].includes(e)
         },
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VBadge-76d9c3a5.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VBadge-84e3406b.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,231 +1,233 @@
 import {
     v as S,
     c as Y,
-    J as k,
-    y as B,
+    J as R,
+    y as v,
     z as M,
     A as c,
-    n as C,
+    n as w,
     x as h,
     B as b,
     N as g,
-    I as F,
+    I as D,
     l as r,
-    Q as R,
+    Q as B,
     D as O,
     E,
     aH as m,
-    L as w,
-    U as X,
-    ag as z,
-    r as L,
-    o as P,
-    Z as U,
-    M as T,
-    p as x,
-    aL as Z,
-    d as V,
-    g as G,
+    L as z,
+    U as L,
+    ag as k,
+    r as U,
+    o as X,
+    Z as T,
+    M as x,
+    p as Z,
+    aL as V,
+    d as G,
+    g as K,
     t as H,
-    aM as K,
-    aN as Q,
-    af as W,
-    aO as j
-} from "./index-6ff57e4c.js";
+    aM as Q,
+    aN as W,
+    af as j,
+    aO as q
+} from "./index-b687f95a.js";
 import {
-    _ as q,
-    a as _
-} from "./Container-ba274a7a.js";
+    _,
+    a as $
+} from "./Container-dc894acd.js";
 import {
-    V as $
-} from "./VInput-91b2e758.js";
+    V as ee
+} from "./VInput-5b197ccd.js";
 import {
-    b as ee,
-    V as te,
-    g as ae,
-    e as ie
-} from "./VMenu-9506155f.js";
+    b as te,
+    V as ae,
+    g as ie,
+    e as ne
+} from "./VMenu-b634019c.js";
 import {
-    k as ne,
-    a as Ae,
+    k as Ae,
+    a as se,
     y as oe,
-    c as se,
-    d as re,
-    I as le,
-    e as ce,
-    g as ue,
-    J as ge,
-    B as me,
+    c as re,
+    d as le,
+    I as ce,
+    e as ue,
+    g as ge,
+    J as me,
+    B as fe,
     i as de,
-    M as fe,
-    n as he
-} from "./forwardRefs-70e877d2.js";
+    M as he,
+    n as be
+} from "./forwardRefs-7be90dc2.js";
 import {
-    V as be
-} from "./VCard-bfc4071a.js";
-const ke = "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACQAAAAkCAYAAADhAJiYAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAABmJLR0QAAAAAAAD5Q7t/AAAACXBIWXMAAABgAAAAYADwa0LPAAAAnElEQVRYw+2UwQ6AMAhDwfjh+OXzZrgslqxjW8K7GWdtRqlIUYyh/qG1Zt8LVYuKzTDUnCGNy41zrfhpGRrhZgn5/HmiWdzuhsrQH7QMicjDENmuGKEbQjaotiwLaGSZeUIzZB2jhnwfAdqyzFAze+gXxPSZxcgaB6JDa+rUDLG2DNFJ3TLkzDlN3bveGWc83ZFlctTIKOVWFCt5AYSDaENMYFhMAAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDIyLTA0LTE1VDEzOjExOjE0KzAwOjAwADepDgAAACV0RVh0ZGF0ZTptb2RpZnkAMjAyMi0wNC0xNVQxMzoxMToxNCswMDowMHFqEbIAAAAASUVORK5CYII=",
-    Re = {
+    V as ke
+} from "./VCard-b98fe47e.js";
+const Re = "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACQAAAAkCAYAAADhAJiYAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAABmJLR0QAAAAAAAD5Q7t/AAAACXBIWXMAAABgAAAAYADwa0LPAAAAnElEQVRYw+2UwQ6AMAhDwfjh+OXzZrgslqxjW8K7GWdtRqlIUYyh/qG1Zt8LVYuKzTDUnCGNy41zrfhpGRrhZgn5/HmiWdzuhsrQH7QMicjDENmuGKEbQjaotiwLaGSZeUIzZB2jhnwfAdqyzFAze+gXxPSZxcgaB6JDa+rUDLG2DNFJ3TLkzDlN3bveGWc83ZFlctTIKOVWFCt5AYSDaENMYFhMAAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDIyLTA0LTE1VDEzOjExOjE0KzAwOjAwADepDgAAACV0RVh0ZGF0ZTptb2RpZnkAMjAyMi0wNC0xNVQxMzoxMToxNCswMDowMHFqEbIAAAAASUVORK5CYII=",
+    Be = {
         class: "d-flex justify-center",
         style: {
             width: "100%"
         }
     },
-    Be = {
+    ve = {
         style: {
             height: "50px",
             display: "flex",
             "align-items": "center"
         }
     },
-    pe = {
+    Fe = {
         style: {
             height: "50px",
             display: "flex",
             "align-items": "center"
         }
     },
-    ve = ["src"],
-    Ie = {
+    pe = ["src"],
+    Ce = {
         key: 0,
         style: {
             height: "50px",
             display: "flex",
             "align-items": "center"
         }
     },
-    Fe = new URL("" + new URL("fallback-d0ff2800.png", import.meta.url).href, self.location).href,
-    Ce = new URL("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAKEAAABtCAYAAADJewF5AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3QwaCisvSBa6TQAACqJJREFUeNrtnXmQFdUVh787MGyirMqgBlDUEAKImkRRqUIxcbfcjcakFDFqlZrSBMtKlf5hSs2uRrOVVuKSGI27FFQlLiHG4AKKKxBBDYICIrtsAvPLH31eqn3Ou91vmHHmvT5fVRfy+p7T3dyft++5fe+54DiO4ziO4ziO4ziO4ziO4ziO4ziO4ziO4ziO4ziO4ziOU3RCkR9eUm9gFDACmGjHeqAn8IUcLlYBa4DtwDpgMfAqsBxYCswPIcx3mbkIy4W3L3AEcLyJby+gsZ0utxpYBLwGPGr/vSCEsN6lV0ARSpoIXAEcBvTtqNsA3gRmAh8C04H/hBBWuQjrW3wDgB8ClwLdOuEtvmWinAk8CSwJIWx1EdaPAI8Ffmr9vh1twTZbX68bsAJ42/4cBAwF9gQ2ADsBO1u5hiqvsxmYBfwdmAa8FkLY7iKs3YDjGuAHrRDCCuCfwPvWh1sCLAPeA9aavy0hhA2p6/UCegHbgK7Wx9wLGAPsBuwBDDShDjXhZrERmAf8BXg8hLDAe4+1I8A+kqapetZKulnS3u14bz0l7SnpQElnSPqlpOclbcy4t48kPSzpBEk9vJY7twD7SXqiFQJ8VNLoDrrnIGmUpPMkTTXBxXhV0hRJw7zGO6cIH61SfEslndvJnmE/SedKuk3SLEmrIq3j7ZLGes13jorrJumPVQrwdUljOvlzBUnDJV0kaXqF1/bLroDOUVmXVCnAZyUNqbFnDJJG2Kv4aUnb7Vne8Oi44yunBzDXotE8vAicGEL4sA3vYXdgpEW9g4Emi4pL45KrbfhmpUXcy2y4Z3kI4aNWXK8rcDBwOTAohDDBRdixIrwM+FXO4i8BJ4QQlrVF343k89+ZwH42/FINa02cq7DvzMACG5b5AFiUZ9Ba0uAQwlJ/H3acAHtKuruKIZhRO3i9LhY0zDB/7cVqSS9KulXSoZJ6em13XhEekOobZXHzDl5rjAUHHcELkn4i6RhJu3rNdy4RXiupOUclbtyRSFjS+ZJWtKGomiVta6XtMkn3Sposaa96qMdQ4yKcA+QZJ5sNHBxCaK7SfyNwPTCllbe4iWR+4UILShaTfAZcTPJZrp8FM03AEAtmmuz3gSRzGmN1tAZ4MIRwYS3XY9ca/59oY85yT7ZCgN2B3wCTWnFfzwD3ADOAxSGELdUMxZB8h+5tQvwScKAdY/n0d+e+JFPTnA5sCf+d8xV2Vit8/64Vr8onJR3Tjs87TNKpkv4gaa5dc6EroTZEeESVfsfl7GuWeFvSBZ/zszdK+oakSa6E2hDhkVX6vb8KAf7VBqudgvYJ20PYhwAn5ix+C3Bltf3NsuuNtP5e/0i/dxkwN4TwjouwGFxNstoui5nA91sR8OwETACOA8ZbVNwnh+lKSfMt6JlHMsl2GfB+COFjr7Y6eR1L6iHptRz+1lQ7hUrSzpIuTQUUbcFKSY95S9ix9Gpjf3uSTMXP4rYQwitVCPBI4OfAAW18v/2BfWpdhA01fv9/Aprb0F9TpG9WYhvwQBUC/DrwWDsIsMQWF2HH8jTJSrgs8q5Yy7N+4wWSqWN5BDgCuItk4NmpUxH2BrrkKDcgp7/uOcpMzznFqhG4lWR+oVPHIlxJsv43izNz+tspR4v6Qk5fk4CjXGJ1LsIQwlzrb2UxQVJTjnKbMs6vADIDElv3fKXLqxgtIcAjOYKTQcDhOXy9A8TG3NbakcV4ktnWThFEGEJ4FngoR9HTc5RZYEcses7TxzvbpVWslhDgqRxlJma9kkMIn2SIsDfJgqYs9nBpFU+E91t/LcZA4PwcvuZFznUhySXjuAg/04KtIVn+mNU3/F6OAGUa8XHFPDNmNru0itcSEkK4z4KUrAAla6r+S8DUyPmxNvs5xnMurYJiq+82ZHz035A1+cCWWW6tYP++Jd6M2X9R0sef00q8mk8D0lBPIgwhzCHJ5xejF3CdpNizPw88EXkdZw1+LyDJcegUtDUcYtm2sjgtw8/pGenZembYT/aWsNhCPC9H5b0Xm5ZvcwtnR+yvyriHpkhaNxdhQYT4SI4KvD3DxwRJn0RSdeybYf97F2GxRbi3pA8yKnCbJVeP+bkmYv9Qhu0+NvvZRVhgIZ6ZI1fNf2O5Cm1pZaUMsNslnZFxD1e5CF2Iv86ZNLMp4mOwpAWR3DCjI7YDJL3hIiy2CPtkBBglZkjaOeLnEEmLKti+JKlbxHa0BUIuwgILcZSk5Tkq9DHLQVPJz0GS1lWwvSlHkLPURVhsIR6WY7+QPBHzBRHbm2Kf9CRNlLTeRVhsIZ5lQytZ3Bv7omIJKytxt+3wVMn2bElbXITFFuJ4CyayeNAWK1Xy87OI7Z0ZLeK32vDbsouwRoU4LhJkpHk4I+C4MWJ7Y4YQT26jvNcuwhoW4khJ89qgRbwo8oq/R9LAiO2xbSBEF2GNC3GYpOdyCrFrxM8BET+vSzo0YvvVnK2yi7COhThA0gM5hdgz4qefpH9EEihdErHd33b7dBEWWIiNkq7PuZXDmIifwZJezkioObSCbX9Jt7gIXYyTc4zjrZf07Ur9REmDJP05Yr9c0jmVhoAknVRl+ri3av3fPbj0PiOCo4HYlgyNJJkabgwhvBrx8x3gpBZOdSdZCHVxCGFlBdu+wBXAl3Pc8rshhClec47jOP46dtqzexBIEnc2AOtDCJtdhMUVw/HA/iQL458JITxXhW1fklRxPUgyvd4RQliVYbM7cCxwMjDObOeRrGl+IITwL6+VYgmwt6R3UhHpHNvsO6/9WWUR7YUZ5YdLejMSEa+TdIrXTLFEeEILQhhXhf3UMtu/RYZoGmxe4//XsUg62o6rUzO8P5Z0uNdOcUT4UGqFXWm7sd/mtN039X24NAa5pdIG4LancekaU8u/0tjXlVKWiRdzpCRx6kCAw1Mimmzfgkv72Q3IYX+llV9kA9GlibU/qlD+mVRLNzIi1POtn+oUQIRTUhMRGiTdkHpVnp1h29VaK0m603571v7+hu3u9KkAxlb/lUTrO265ANUo6RUTxWWp1+Em++3xDPtDU4vnjysTtSQdVVZ+mKQPUyJs9FpwER5lglgiaZfU73fb72tjWRgk/bi0J7GkXSXtIunE1PT+O8vKD00tyFqYkbTJKYgI7zBBbLQZNLMlzSqb/3dRBdtdJL1rZTZJmm92K8rWLA9O2XS3vqasfJcKvi+XNNOO0V5T9SvAXVMpPLbYa3WbHekciLNbEouk01JlNtqcwpX2uv0odW5Smd119vtWSd9swe/u5qvk19MX17EIL7aK/kTSqZb4cqQdI1LDNlsljW/B/r6USA+0KV4Dbd7gcEmL7fwTLbySl9i5pZIOL/UNbafQaSkBX+s1Vb8C7GoDypI0o0KZU1Ji+EXZuSHWWm2XdE4F+1tSrdnYsnMHpV7L22zY5q6y2df3xhbqO7UvwjGpyv5uhTK7pTIqfJBOIZIaG2yW1L+C/ddMYJJ0QwvnR1ifryWmS+pTL//ePtreskD6k+xX0gzMCSFsqlBuFFCKmmeVNl6UtB/JlhXNwMu2P0q5bQPJ9rPdgdUhhHktlOkHfIVkd6geJDNpFgJPhRDWeU05juM4juM4juM4juM4juM4juM4juM4juM4juM4juM4juPUC/8DLSVc5VaBblAAAAAASUVORK5CYII=", self.location).href,
-    we = new URL("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJEAAABfCAYAAADoOiXnAAAPMElEQVR4nO2de7RUVR3HP3Pv9V5eF71eUEBAEQVBufhM0FziE1NRSi1NqaXlI2v5LmtZUlZqrVo+yJKWWCaRWpLio3yh+UjRRJ4higgJIpgooMCFy0x/fPfunDnMzDkzZ98HuL9rzZqZM/vsfc7Z3/3bv9fek8nlcnh4pEFVe1+Ax7YPTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kiNGgd1TAJaECFXANeZ7x6fEmQcpMeGK1gADAO2pK3UY9uBC0kUxnrH9bnALkhKrgM+aedr2S7hmkTtjb7AUOAIoBcwCOiP7vN+4LIy66sCsi4vcHuEaxJVO64vKY4BvgwcB/QrUmY00Ah8YL5XAw3A3kAG6AEMBJrM773N72cBi1vlqrcTuCDRBqQDVQMfO6ivHPQFvgV8E+gWU3YQIpglURMwDehDcSs1C3RJf5nbN1yQqAdSrjOITG2lVPcH7kDSJwmqkMSaZb7XIRKWwkb8dBYLFyT6PiJOFbAS+DXFTfzz0cjPmrYfAV6uoM0dgYkkJ5DFsNDnHAH5PVLABYm+F/r8BiJRMVwM7B/6/g6VkWgccEIF541CkvO/FZzrUQSuPdZxOlHUBbCpgjZ2oXwry6I3sFeF53oUwbYY9hiNrKhKUIv0Ig+HcG3ix5HShf5xSpnlNyAnYwbdb4ODa/AIwQWJmpGinEHTUymi5ELvmZiyhVBNcin0MHArsApYbo5VIYvLwyFckKgvAYmylA6+jkWmdRZ16Ooy2+qNTPs4TAPOpu39Vp9KuCDROQQm/vvAFGQFjQQ2mzZmA38DDgZ6Epj4LwGvl9HWAOR1jsMU2pZA1ei+GoAR5j0b+f1NYC56Rq6vrQfQFT33XgXanmNeyxy3C7gh0U2hzwtRB54MXBk6fg8i0XWISBbnEU+izsCeiKh9ifftbERT7JBQuSrgPdyb9gOBrwEHAcOR17xrifIfIrfGdCQtnyE/C6IcZIDDkXQfjfxvOxcpm0P3/gLwKPAEsKTCdreCa8XajrCo3rGhyPEkJv6xwL0EDztOj9oBuBsRx5bNAKcCjydorxyMIN9PFocG82oCvo6u8+eU36F7AtcApyHHaxwySFKONa+3UR7YLTiQim1t4lcy6oYgadSFZHGsaiQRupjzOgOdKmw7DvukOLcb8A3gAeCAMs47B3gSSfEkBCqEAcBPkFQ6tMI6/g/XJComJdKY9uWGNtoShzuoYzgwGRgcU6478CMkQQY4aBeUMvObtJW4JpGtL5oSYklUGzkeN53WUXyeb29kkJRzgaHAj9FUXAzjgWvZ+hmmxRNpK3ChEw0hMNmtznMTcFfo+Efm+NlIBFvl+O2Yug8gP2jakTCYeOlRDj4PHImmqijORukurvE88Iu0lbggURP5ZFmC/Dn7EOQZLUbWUQ9Eoqw5/gGyWIqhkdKjsz1hk9ZcoQYRaTr5JnoT6ug6h22Bnv145HJIBRckujf0+XUkmcaRb+L/CWUe3kK+Incu8PsSdX/OwfVZuJ66e0W+v4s841uARWiwWKIl9bIfjaZImwueAa4q0JYL3IYImxquTXx781FT3n7fHDke/R5FZ+TfaEFTYC3xzsYcsBZlDNjQSguBm8EVjkc+nz8DzwL/RtNzhuC+apD0HQv8APlySqEb+SQ6GJnxSbESmIFcGcuQz+pA5PgdSaCb/h2FhJygrRP1yzWzL0ESzZ53BPBQzDlrkbNzbqRdlytRqlAnXI880cXQgqbx25GkmgzUlyjfkyDfqQq4kOTpudPQ9DQrcnwK6ufRwM3IUPkuQZpwargmkWsTP7rEZ12Cc7JIB1tTYZtJkAVeixzrjkZ+LSLtx+ZlHarTgHlIIhRDHYHu0xM5WpPgDpRr3lzk9xaURTofSfLZCetNBNcksg+gmCkfHVXlKs1JV5O4NoOLYQ9gDHAUsiLr0T3lEOGXo3DPNCQZn6c0iTYRkO4wkgWbX0OmfzEChbEEh+EOCxckOpLAOrMu9NsR8611tsIcvxCJa4s5DtpvD9QBX0Shh2JmfiMi2eHA1cioiEv6X0MgbRuIl+A5FDZZEVOuVeGCRLnIqxQ2I93EkiuLRu5hBNZTBphJ4FvqaOiCAslXxhUMoR4taEgSp7LP8LMJyi5BSnK7wgWJng19tib+RcC3Q8cnI7P/ThTxthiH4jePEES/c6ZMVOfoKBhPeQQKI25tXFjy7JGgvnfpAEvDXftOrGkbjc6XOp4jX8y35dq1cnEqlRMoCdYRSKskz+BV4t0krQ7XJCo2neVifs8W+dyR0Ih0oNZcKt5MMgXZoo4OsG6urUz8uN8zCcq0N5qAQxKUW4G8+E+iFJSjkLNxtwTnhvPOkwzwgxGp23U/KNeSyEa1O0WOd4r8blGLHlo4G3AH2m9jiEKw0vOkBGXnIk/25UjPux/5b05iaydgMVgSzU9Q1u6C0q5wIYlOJzDxbTD1D8j93mLasLtqXIoWH24xx2cgPeALBL6dLK3gy3CAuHX7m5EFNq/Ab7PRVDiV+ECqJVES0u2K9LR2dZW4kETV5hXOr2lG8bLN5t2O5l4oMNkA7ISslVrkO6o3rwbazllYDuIi9ssoHdB8isIEK4ZVJAsTXUo7J+65juKvQeQ4Dfhp6PijSKRPQJLI4iJkjUyK1DkSBRM7AmxHxiWgxa2jaybekgrnhT+PJHJcFmMjyk68gPio/KEok3ISDi1g1zrRpsi7hbW4opF0a+KHkaNjmfi2U1fFlOuDUjmKYSTxCXZrCZTkNSRfWDAQpdSchQZxFDuiae+PaDeV8xLWmwiurbM4E39bRpwUqUWe7CVsHeAcDPyS0suJQFOiTZvJAX9BOVdJpvd+yKk7H3iMwFVQh5T9oQT9/UOkjzrRpba3PRtbE4sSlGlCU/dU4EFkNBwLnIGmkThErdJ/oNSXpDlFVUjaxUm8PiiWdwrJMiNiG3UJO9KiI8ea+NEofg1b6xGZVriuNLDX91TC8n2QWf8E8CJampOEQFDYo389rRNgHUXlW/TkwdVm6HYtvk10mok2u7Kmv93I6m5klubQqHsLjYTJofrC9XQkzELZi+X4Zcp1nL5b4NhMZKTcgnv/2dVIgX86TSUuSHRD6LNViF9GS6otbKrqdGTG2+i91QEeJtCbqpGC2dHwERoEN8QVbAVMRBmJ43FLpK6m7kFpKnFBorCusBr5fC5BN2zxOErPnEi++/8ClMpwT6TOEcRbQ+2BW1EY4/hWqr/YNN6CpFELeq4uV36kXtfXVrqHHT1R072YKZ8mCOsyKLlDpK71aP3XPyuo60PypXMhlNpwIgvcCHyJ8nZSKYVXgDPTVtJaUfxCvp9Cx0vVUQhxG2i9h0zcJAHJJJtsvVegrkXAV9AUnJTsq9G6+xkx5eJWpOSQ1XccctxW6pBdhFbcnkzhxZJlYVsz8ZvR6FmHLJeX0APZjDp8ofktyW5oWdQJy5Fjz9Zt61tuPheaVt9CI/hEtDp1OIWTyBaj7WN+hZLsDkJ/orOSIJl/PlKo30e77ybBMhTuuBmpCWPRTiHFNjXdhEIuC1C+91M4NF5c/8vQJmTOX4+WpVi8iFJgV5If9rgQ6URLI3WOoPCotUnwLlIfapGSv47KdrENYzfUgTl0fx+ia1yIyG1hXRyt8Uc6jYjM9l8AuiNi5pCEe5X091kQLiTRbQRr6/9jPj9H/vqqmeb3x5EfxZr4K9ADDftg7D8CFYLLLL5NuBuNywn2hSyF1vwXpg9wtKK1XLiQRFEH4nokMcLLgbag6aIXAXGtP6gZLTcOYyUdIO3TIxlcKNarQ683CdaPh49PNWWfRiJ+IbIwjkZTwcLQayalk9T7oGh0JWauTVspB23lQQ+348oXZFN0WhUuHk5d6GWlUk3kuA172B3M7MuGPcLHusVc11XIMuqH9JpiU3KhjhiDNoqySHL/9ShCbvOJ0j4zS5bodY8CfoY84hMi5Qsh7jqGokhAseCts4HheoRZv090jsxGfqdIuUJlwtgZ+CrSvY4B/oXCK6ORFTQRdfoZSC+bQn5GYj2aOnsDf0XK+yiUs3MH8sN0RQsTp6NQQzcUha8FrjD1XmuO34ik63lIsX4ArXgNB0B7mut4BmVwDgK+Y9odj8g0wbwGoryl3iil4zZkMZ4beQ7nI0X5VhRGmmTu5XSkUN+FpP9+iIQXAfehvQxq0VY1r6Ct+1KjIwU6k2ADUsafRg97FzT93YAe3hgUVLwGec7HkJ87k0Vm9QWo0+ejlNbzUaT8RPQnemci8u2PSLUG7a5xBeqEy5Cv5lSk5w03ZY9AS5/3DLXZH9gdWU/j0EDYG0ndQ9CWO59BMSz7h8xZ9Ac4JyDSXkwwfe+EArwvmns8GbkOXkUW8fHmel4y93ogIs0ByCVwFHJYLkD7IUXz4cuGaxLZxXlRfaVL5HeLmgLXUGo624B0qaXIunoFLdluRPG2tWjk1RMsSQ5fi3UwdkfB1KmITG8jqdYJdewcpMv1NNezBeluPZAxYFfxzkCLB3uZa5uLDIJwNuIwcw0bCaYwu/FDMyLUYpQhaqf3KjRI3jDHu4TO7YcGz0MoKNzXnH8nIuHuSDe1i0obEZnsHtq7mvv9nXlPbaG7MPEfI3/7vBxiefj4c6bsfeSP0hXIp/IgwYhYT+kclxr0gD9GD7cK5d3sjTryBeRn6o9GdNgHZTtoHpqy9kWrMjoTbAO4ET14u5F7jalnNuqILsicX4c6cCMiST0imd1LycLmlK8icG8MRyuFF6Jp9S4kLV43bdnrHojIMY/APbAASd+bzf1ejqbJ35r6piPJuh8aSAvN+dYFM9NczwREvnLWuRWECxO/rTEMddwnaFTOQFNEE5JEc1FnDkMdPYsgnNAHSYGlBFPVHHPeQaiD7UMehki+1Jz3FpIwA9DmVm8i4vZBnu01iBg1pk47EDoR/MfbBtRxAxDplqNMyH0R2d5Bg8q2NxhJndnkb0u4BxqMKxGp9kKEttJmiDlvNZK4vU2b80w9Q0wb83CQy74tksijg2FbU6w9OiA8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzX+B1yXSRtpspd4AAAAAElFTkSuQmCC", self.location).href,
+    De = new URL("" + new URL("fallback-d0ff2800.png", import.meta.url).href, self.location).href,
+    we = new URL("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAKEAAABtCAYAAADJewF5AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH3QwaCisvSBa6TQAACqJJREFUeNrtnXmQFdUVh787MGyirMqgBlDUEAKImkRRqUIxcbfcjcakFDFqlZrSBMtKlf5hSs2uRrOVVuKSGI27FFQlLiHG4AKKKxBBDYICIrtsAvPLH31eqn3Ou91vmHHmvT5fVRfy+p7T3dyft++5fe+54DiO4ziO4ziO4ziO4ziO4ziO4ziO4ziO4ziO4ziO4ziOU3RCkR9eUm9gFDACmGjHeqAn8IUcLlYBa4DtwDpgMfAqsBxYCswPIcx3mbkIy4W3L3AEcLyJby+gsZ0utxpYBLwGPGr/vSCEsN6lV0ARSpoIXAEcBvTtqNsA3gRmAh8C04H/hBBWuQjrW3wDgB8ClwLdOuEtvmWinAk8CSwJIWx1EdaPAI8Ffmr9vh1twTZbX68bsAJ42/4cBAwF9gQ2ADsBO1u5hiqvsxmYBfwdmAa8FkLY7iKs3YDjGuAHrRDCCuCfwPvWh1sCLAPeA9aavy0hhA2p6/UCegHbgK7Wx9wLGAPsBuwBDDShDjXhZrERmAf8BXg8hLDAe4+1I8A+kqapetZKulnS3u14bz0l7SnpQElnSPqlpOclbcy4t48kPSzpBEk9vJY7twD7SXqiFQJ8VNLoDrrnIGmUpPMkTTXBxXhV0hRJw7zGO6cIH61SfEslndvJnmE/SedKuk3SLEmrIq3j7ZLGes13jorrJumPVQrwdUljOvlzBUnDJV0kaXqF1/bLroDOUVmXVCnAZyUNqbFnDJJG2Kv4aUnb7Vne8Oi44yunBzDXotE8vAicGEL4sA3vYXdgpEW9g4Emi4pL45KrbfhmpUXcy2y4Z3kI4aNWXK8rcDBwOTAohDDBRdixIrwM+FXO4i8BJ4QQlrVF343k89+ZwH42/FINa02cq7DvzMACG5b5AFiUZ9Ba0uAQwlJ/H3acAHtKuruKIZhRO3i9LhY0zDB/7cVqSS9KulXSoZJ6em13XhEekOobZXHzDl5rjAUHHcELkn4i6RhJu3rNdy4RXiupOUclbtyRSFjS+ZJWtKGomiVta6XtMkn3Sposaa96qMdQ4yKcA+QZJ5sNHBxCaK7SfyNwPTCllbe4iWR+4UILShaTfAZcTPJZrp8FM03AEAtmmuz3gSRzGmN1tAZ4MIRwYS3XY9ca/59oY85yT7ZCgN2B3wCTWnFfzwD3ADOAxSGELdUMxZB8h+5tQvwScKAdY/n0d+e+JFPTnA5sCf+d8xV2Vit8/64Vr8onJR3Tjs87TNKpkv4gaa5dc6EroTZEeESVfsfl7GuWeFvSBZ/zszdK+oakSa6E2hDhkVX6vb8KAf7VBqudgvYJ20PYhwAn5ix+C3Bltf3NsuuNtP5e/0i/dxkwN4TwjouwGFxNstoui5nA91sR8OwETACOA8ZbVNwnh+lKSfMt6JlHMsl2GfB+COFjr7Y6eR1L6iHptRz+1lQ7hUrSzpIuTQUUbcFKSY95S9ix9Gpjf3uSTMXP4rYQwitVCPBI4OfAAW18v/2BfWpdhA01fv9/Aprb0F9TpG9WYhvwQBUC/DrwWDsIsMQWF2HH8jTJSrgs8q5Yy7N+4wWSqWN5BDgCuItk4NmpUxH2BrrkKDcgp7/uOcpMzznFqhG4lWR+oVPHIlxJsv43izNz+tspR4v6Qk5fk4CjXGJ1LsIQwlzrb2UxQVJTjnKbMs6vADIDElv3fKXLqxgtIcAjOYKTQcDhOXy9A8TG3NbakcV4ktnWThFEGEJ4FngoR9HTc5RZYEcses7TxzvbpVWslhDgqRxlJma9kkMIn2SIsDfJgqYs9nBpFU+E91t/LcZA4PwcvuZFznUhySXjuAg/04KtIVn+mNU3/F6OAGUa8XHFPDNmNru0itcSEkK4z4KUrAAla6r+S8DUyPmxNvs5xnMurYJiq+82ZHz035A1+cCWWW6tYP++Jd6M2X9R0sef00q8mk8D0lBPIgwhzCHJ5xejF3CdpNizPw88EXkdZw1+LyDJcegUtDUcYtm2sjgtw8/pGenZembYT/aWsNhCPC9H5b0Xm5ZvcwtnR+yvyriHpkhaNxdhQYT4SI4KvD3DxwRJn0RSdeybYf97F2GxRbi3pA8yKnCbJVeP+bkmYv9Qhu0+NvvZRVhgIZ6ZI1fNf2O5Cm1pZaUMsNslnZFxD1e5CF2Iv86ZNLMp4mOwpAWR3DCjI7YDJL3hIiy2CPtkBBglZkjaOeLnEEmLKti+JKlbxHa0BUIuwgILcZSk5Tkq9DHLQVPJz0GS1lWwvSlHkLPURVhsIR6WY7+QPBHzBRHbm2Kf9CRNlLTeRVhsIZ5lQytZ3Bv7omIJKytxt+3wVMn2bElbXITFFuJ4CyayeNAWK1Xy87OI7Z0ZLeK32vDbsouwRoU4LhJkpHk4I+C4MWJ7Y4YQT26jvNcuwhoW4khJ89qgRbwo8oq/R9LAiO2xbSBEF2GNC3GYpOdyCrFrxM8BET+vSzo0YvvVnK2yi7COhThA0gM5hdgz4qefpH9EEihdErHd33b7dBEWWIiNkq7PuZXDmIifwZJezkioObSCbX9Jt7gIXYyTc4zjrZf07Ur9REmDJP05Yr9c0jmVhoAknVRl+ri3av3fPbj0PiOCo4HYlgyNJJkabgwhvBrx8x3gpBZOdSdZCHVxCGFlBdu+wBXAl3Pc8rshhClec47jOP46dtqzexBIEnc2AOtDCJtdhMUVw/HA/iQL458JITxXhW1fklRxPUgyvd4RQliVYbM7cCxwMjDObOeRrGl+IITwL6+VYgmwt6R3UhHpHNvsO6/9WWUR7YUZ5YdLejMSEa+TdIrXTLFEeEILQhhXhf3UMtu/RYZoGmxe4//XsUg62o6rUzO8P5Z0uNdOcUT4UGqFXWm7sd/mtN039X24NAa5pdIG4LancekaU8u/0tjXlVKWiRdzpCRx6kCAw1Mimmzfgkv72Q3IYX+llV9kA9GlibU/qlD+mVRLNzIi1POtn+oUQIRTUhMRGiTdkHpVnp1h29VaK0m603571v7+hu3u9KkAxlb/lUTrO265ANUo6RUTxWWp1+Em++3xDPtDU4vnjysTtSQdVVZ+mKQPUyJs9FpwER5lglgiaZfU73fb72tjWRgk/bi0J7GkXSXtIunE1PT+O8vKD00tyFqYkbTJKYgI7zBBbLQZNLMlzSqb/3dRBdtdJL1rZTZJmm92K8rWLA9O2XS3vqasfJcKvi+XNNOO0V5T9SvAXVMpPLbYa3WbHekciLNbEouk01JlNtqcwpX2uv0odW5Smd119vtWSd9swe/u5qvk19MX17EIL7aK/kTSqZb4cqQdI1LDNlsljW/B/r6USA+0KV4Dbd7gcEmL7fwTLbySl9i5pZIOL/UNbafQaSkBX+s1Vb8C7GoDypI0o0KZU1Ji+EXZuSHWWm2XdE4F+1tSrdnYsnMHpV7L22zY5q6y2df3xhbqO7UvwjGpyv5uhTK7pTIqfJBOIZIaG2yW1L+C/ddMYJJ0QwvnR1ifryWmS+pTL//ePtreskD6k+xX0gzMCSFsqlBuFFCKmmeVNl6UtB/JlhXNwMu2P0q5bQPJ9rPdgdUhhHktlOkHfIVkd6geJDNpFgJPhRDWeU05juM4juM4juM4juM4juM4juM4juM4juM4juM4juM4juPUC/8DLSVc5VaBblAAAAAASUVORK5CYII=", self.location).href,
+    ze = new URL("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJEAAABfCAYAAADoOiXnAAAPMElEQVR4nO2de7RUVR3HP3Pv9V5eF71eUEBAEQVBufhM0FziE1NRSi1NqaXlI2v5LmtZUlZqrVo+yJKWWCaRWpLio3yh+UjRRJ4higgJIpgooMCFy0x/fPfunDnMzDkzZ98HuL9rzZqZM/vsfc7Z3/3bv9fek8nlcnh4pEFVe1+Ax7YPTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kgNTyKP1PAk8kiNGgd1TAJaECFXANeZ7x6fEmQcpMeGK1gADAO2pK3UY9uBC0kUxnrH9bnALkhKrgM+aedr2S7hmkTtjb7AUOAIoBcwCOiP7vN+4LIy66sCsi4vcHuEaxJVO64vKY4BvgwcB/QrUmY00Ah8YL5XAw3A3kAG6AEMBJrM773N72cBi1vlqrcTuCDRBqQDVQMfO6ivHPQFvgV8E+gWU3YQIpglURMwDehDcSs1C3RJf5nbN1yQqAdSrjOITG2lVPcH7kDSJwmqkMSaZb7XIRKWwkb8dBYLFyT6PiJOFbAS+DXFTfzz0cjPmrYfAV6uoM0dgYkkJ5DFsNDnHAH5PVLABYm+F/r8BiJRMVwM7B/6/g6VkWgccEIF541CkvO/FZzrUQSuPdZxOlHUBbCpgjZ2oXwry6I3sFeF53oUwbYY9hiNrKhKUIv0Ig+HcG3ix5HShf5xSpnlNyAnYwbdb4ODa/AIwQWJmpGinEHTUymi5ELvmZiyhVBNcin0MHArsApYbo5VIYvLwyFckKgvAYmylA6+jkWmdRZ16Ooy2+qNTPs4TAPOpu39Vp9KuCDROQQm/vvAFGQFjQQ2mzZmA38DDgZ6Epj4LwGvl9HWAOR1jsMU2pZA1ei+GoAR5j0b+f1NYC56Rq6vrQfQFT33XgXanmNeyxy3C7gh0U2hzwtRB54MXBk6fg8i0XWISBbnEU+izsCeiKh9ifftbERT7JBQuSrgPdyb9gOBrwEHAcOR17xrifIfIrfGdCQtnyE/C6IcZIDDkXQfjfxvOxcpm0P3/gLwKPAEsKTCdreCa8XajrCo3rGhyPEkJv6xwL0EDztOj9oBuBsRx5bNAKcCjydorxyMIN9PFocG82oCvo6u8+eU36F7AtcApyHHaxwySFKONa+3UR7YLTiQim1t4lcy6oYgadSFZHGsaiQRupjzOgOdKmw7DvukOLcb8A3gAeCAMs47B3gSSfEkBCqEAcBPkFQ6tMI6/g/XJComJdKY9uWGNtoShzuoYzgwGRgcU6478CMkQQY4aBeUMvObtJW4JpGtL5oSYklUGzkeN53WUXyeb29kkJRzgaHAj9FUXAzjgWvZ+hmmxRNpK3ChEw0hMNmtznMTcFfo+Efm+NlIBFvl+O2Yug8gP2jakTCYeOlRDj4PHImmqijORukurvE88Iu0lbggURP5ZFmC/Dn7EOQZLUbWUQ9Eoqw5/gGyWIqhkdKjsz1hk9ZcoQYRaTr5JnoT6ug6h22Bnv145HJIBRckujf0+XUkmcaRb+L/CWUe3kK+Incu8PsSdX/OwfVZuJ66e0W+v4s841uARWiwWKIl9bIfjaZImwueAa4q0JYL3IYImxquTXx781FT3n7fHDke/R5FZ+TfaEFTYC3xzsYcsBZlDNjQSguBm8EVjkc+nz8DzwL/RtNzhuC+apD0HQv8APlySqEb+SQ6GJnxSbESmIFcGcuQz+pA5PgdSaCb/h2FhJygrRP1yzWzL0ESzZ53BPBQzDlrkbNzbqRdlytRqlAnXI880cXQgqbx25GkmgzUlyjfkyDfqQq4kOTpudPQ9DQrcnwK6ufRwM3IUPkuQZpwargmkWsTP7rEZ12Cc7JIB1tTYZtJkAVeixzrjkZ+LSLtx+ZlHarTgHlIIhRDHYHu0xM5WpPgDpRr3lzk9xaURTofSfLZCetNBNcksg+gmCkfHVXlKs1JV5O4NoOLYQ9gDHAUsiLr0T3lEOGXo3DPNCQZn6c0iTYRkO4wkgWbX0OmfzEChbEEh+EOCxckOpLAOrMu9NsR8611tsIcvxCJa4s5DtpvD9QBX0Shh2JmfiMi2eHA1cioiEv6X0MgbRuIl+A5FDZZEVOuVeGCRLnIqxQ2I93EkiuLRu5hBNZTBphJ4FvqaOiCAslXxhUMoR4taEgSp7LP8LMJyi5BSnK7wgWJng19tib+RcC3Q8cnI7P/ThTxthiH4jePEES/c6ZMVOfoKBhPeQQKI25tXFjy7JGgvnfpAEvDXftOrGkbjc6XOp4jX8y35dq1cnEqlRMoCdYRSKskz+BV4t0krQ7XJCo2neVifs8W+dyR0Ih0oNZcKt5MMgXZoo4OsG6urUz8uN8zCcq0N5qAQxKUW4G8+E+iFJSjkLNxtwTnhvPOkwzwgxGp23U/KNeSyEa1O0WOd4r8blGLHlo4G3AH2m9jiEKw0vOkBGXnIk/25UjPux/5b05iaydgMVgSzU9Q1u6C0q5wIYlOJzDxbTD1D8j93mLasLtqXIoWH24xx2cgPeALBL6dLK3gy3CAuHX7m5EFNq/Ab7PRVDiV+ECqJVES0u2K9LR2dZW4kETV5hXOr2lG8bLN5t2O5l4oMNkA7ISslVrkO6o3rwbazllYDuIi9ssoHdB8isIEK4ZVJAsTXUo7J+65juKvQeQ4Dfhp6PijSKRPQJLI4iJkjUyK1DkSBRM7AmxHxiWgxa2jaybekgrnhT+PJHJcFmMjyk68gPio/KEok3ISDi1g1zrRpsi7hbW4opF0a+KHkaNjmfi2U1fFlOuDUjmKYSTxCXZrCZTkNSRfWDAQpdSchQZxFDuiae+PaDeV8xLWmwiurbM4E39bRpwUqUWe7CVsHeAcDPyS0suJQFOiTZvJAX9BOVdJpvd+yKk7H3iMwFVQh5T9oQT9/UOkjzrRpba3PRtbE4sSlGlCU/dU4EFkNBwLnIGmkThErdJ/oNSXpDlFVUjaxUm8PiiWdwrJMiNiG3UJO9KiI8ea+NEofg1b6xGZVriuNLDX91TC8n2QWf8E8CJampOEQFDYo389rRNgHUXlW/TkwdVm6HYtvk10mok2u7Kmv93I6m5klubQqHsLjYTJofrC9XQkzELZi+X4Zcp1nL5b4NhMZKTcgnv/2dVIgX86TSUuSHRD6LNViF9GS6otbKrqdGTG2+i91QEeJtCbqpGC2dHwERoEN8QVbAVMRBmJ43FLpK6m7kFpKnFBorCusBr5fC5BN2zxOErPnEi++/8ClMpwT6TOEcRbQ+2BW1EY4/hWqr/YNN6CpFELeq4uV36kXtfXVrqHHT1R072YKZ8mCOsyKLlDpK71aP3XPyuo60PypXMhlNpwIgvcCHyJ8nZSKYVXgDPTVtJaUfxCvp9Cx0vVUQhxG2i9h0zcJAHJJJtsvVegrkXAV9AUnJTsq9G6+xkx5eJWpOSQ1XccctxW6pBdhFbcnkzhxZJlYVsz8ZvR6FmHLJeX0APZjDp8ofktyW5oWdQJy5Fjz9Zt61tuPheaVt9CI/hEtDp1OIWTyBaj7WN+hZLsDkJ/orOSIJl/PlKo30e77ybBMhTuuBmpCWPRTiHFNjXdhEIuC1C+91M4NF5c/8vQJmTOX4+WpVi8iFJgV5If9rgQ6URLI3WOoPCotUnwLlIfapGSv47KdrENYzfUgTl0fx+ia1yIyG1hXRyt8Uc6jYjM9l8AuiNi5pCEe5X091kQLiTRbQRr6/9jPj9H/vqqmeb3x5EfxZr4K9ADDftg7D8CFYLLLL5NuBuNywn2hSyF1vwXpg9wtKK1XLiQRFEH4nokMcLLgbag6aIXAXGtP6gZLTcOYyUdIO3TIxlcKNarQ683CdaPh49PNWWfRiJ+IbIwjkZTwcLQayalk9T7oGh0JWauTVspB23lQQ+348oXZFN0WhUuHk5d6GWlUk3kuA172B3M7MuGPcLHusVc11XIMuqH9JpiU3KhjhiDNoqySHL/9ShCbvOJ0j4zS5bodY8CfoY84hMi5Qsh7jqGokhAseCts4HheoRZv090jsxGfqdIuUJlwtgZ+CrSvY4B/oXCK6ORFTQRdfoZSC+bQn5GYj2aOnsDf0XK+yiUs3MH8sN0RQsTp6NQQzcUha8FrjD1XmuO34ik63lIsX4ArXgNB0B7mut4BmVwDgK+Y9odj8g0wbwGoryl3iil4zZkMZ4beQ7nI0X5VhRGmmTu5XSkUN+FpP9+iIQXAfehvQxq0VY1r6Ct+1KjIwU6k2ADUsafRg97FzT93YAe3hgUVLwGec7HkJ87k0Vm9QWo0+ejlNbzUaT8RPQnemci8u2PSLUG7a5xBeqEy5Cv5lSk5w03ZY9AS5/3DLXZH9gdWU/j0EDYG0ndQ9CWO59BMSz7h8xZ9Ac4JyDSXkwwfe+EArwvmns8GbkOXkUW8fHmel4y93ogIs0ByCVwFHJYLkD7IUXz4cuGaxLZxXlRfaVL5HeLmgLXUGo624B0qaXIunoFLdluRPG2tWjk1RMsSQ5fi3UwdkfB1KmITG8jqdYJdewcpMv1NNezBeluPZAxYFfxzkCLB3uZa5uLDIJwNuIwcw0bCaYwu/FDMyLUYpQhaqf3KjRI3jDHu4TO7YcGz0MoKNzXnH8nIuHuSDe1i0obEZnsHtq7mvv9nXlPbaG7MPEfI3/7vBxiefj4c6bsfeSP0hXIp/IgwYhYT+kclxr0gD9GD7cK5d3sjTryBeRn6o9GdNgHZTtoHpqy9kWrMjoTbAO4ET14u5F7jalnNuqILsicX4c6cCMiST0imd1LycLmlK8icG8MRyuFF6Jp9S4kLV43bdnrHojIMY/APbAASd+bzf1ejqbJ35r6piPJuh8aSAvN+dYFM9NczwREvnLWuRWECxO/rTEMddwnaFTOQFNEE5JEc1FnDkMdPYsgnNAHSYGlBFPVHHPeQaiD7UMehki+1Jz3FpIwA9DmVm8i4vZBnu01iBg1pk47EDoR/MfbBtRxAxDplqNMyH0R2d5Bg8q2NxhJndnkb0u4BxqMKxGp9kKEttJmiDlvNZK4vU2b80w9Q0wb83CQy74tksijg2FbU6w9OiA8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzU8iTxSw5PIIzX+B1yXSRtpspd4AAAAAElFTkSuQmCC", self.location).href,
     N = new URL("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJEAAABfCAYAAADoOiXnAAALyUlEQVR4nO2debAcVRWHv5eQjRhIIIQEDFRIwCAYFmUTQxJ2TalIQGQRlE3WiBSFsQoiSwWECiIlm8oiSwBBFIMga8BYQFhFCQYhIYIBAoQALxsBkuMfvx6nX8/Sd+Z2z8x7735VXW96+m7T7zd3Oef0nTYzIxDwoUezGxDo/AQRBbwJIgp4E0QU8CaIKOBNEFHAmyCigDdBRAFvgogC3gQRBbwJIgp4E0QU8CaIKOBNEFHAmyCigDdBRAFvgogC3gQRBbwJIgp4s06zG1AnQ4HPAtsAnwdGRucDgH7AIOA94FPgHWA+MBf4O/Bv4M3GN7nr0tZJAvXbgB2BfYGvIfEMqrOsT4EngN8CtwPLM2hft6bVRTQE+DZwJPAlJKYkbwDzgGdQL/Nf1At9HF3vAQwGNkPi2w3YBegNvA1cClwJLMvrQ3R1WlVE2wDHA4cAGyeutaOh6a/An6PX7TWWPxTYG/geMAFYCBwHPFJ3i7sxrSaiMcCZwEFAn8S154DrgJmot8mKkcAU4Nio/JOBjzIsv8vTKiLqA5wN/AhYN3HtAeASYBaaz+TFROBa1CtNIAjJmVYQ0Z7ARWjOE+cR4DLgTw1syzDgNjSfOgBY0cC6Oy3NFFEb8HPgtMT7rwE/Bn7X8BaJNuAeYH1gHPn2fl2CZhkbNwDupFRAM4CdaZ6AAAw4EBgITG9iOzoNzeiJRgO3AtvH3luNep/LGt2YKmyB7El7Ay80uS0tTaNFtAXwKDA89t4i4HBgdiMb4siRwFFISE2fPLYqjRzORgD30lFAC4G9aE0BgYbXTYD9m92QVqZRItoYuAv4XOy9t4BJwMsNakM9rAEuB37Y7Ia0Mo0Yznqi5frY2Hvvo6X983lXngF9kVX8YOTAbVXakOF0u+jvpsghXWA1Wvm+gOZ6S7OquBFe/NPpKCBD7obOICCQ0fE0JPxWZAzwXTRvG41En8Yi4Bpkn/M2qubdE+2M5jtxF8Y04Kw8K+0m7Amcgiztvess417gCDy/IHmKqB/wNHKmFngBWaY/Lpsj4MJQ5AY6rMy114G7gSXAKOTAThttpqAeqW7yHM5+QEcBgXxjQUB+nE+pgNYCF0dHvFcZiHqqamzt26C8VmcDkfEwzi3AwznV1524llKf3s+An1A6LL3nUN4q3wblJaLvoG63wHLkpW8WvaKjXFBbOdaJ0ufZU7ehiIU+1PZ/mEPp8HN1mXS9gN0dyptbQ91lyeMm9URDWZzbgVczKHsAcCrVJ5JLgN8D41FIx44Uw0s+BhagCeWNFJ2rg5HRcw/UvRcC4QytZB5BPcCSCnXuhyImq7EC9cbjgX2Q22e9qA2rUIzUHGTgXJhS1hXImt4TOYvLLdcPREv9aixGgX1+mFnWxzgrZbeMyj6oTNnleNshzW1Ru640szcd0r9sZqPKtKmfmS10bNc7DmmWmNnxZepJHkPMrH+FayPM7HWHug5xqCf1yENENyYaOt/M+mRU9mMONyZPbrfSNh2TU10HlKnL5RhrZgtSyv7IzI6ts/ySI+s50QBk9IpzL7KW+jIO+HIG5fiwCx1tXj2ByTXkfxUtz19ySHtqDeUCbAWciyJBt6iSbh5asV1TY/kVyXpOtB2KDozzUEZlJ2OPKnEPmiyeREezfyXmonnBQci2Uo1P6BikNhFZjF14FLlOlqA5zLSU9CPRXG5lmWu9gAuADVFs1mZoLlfJWv0hEu4dwG+o/cGGqmQtor0S5+3AkxmUuwPwdYd0F1M0LRxBuohmReWuRN/eNBG9hpyyoNVV0oxRiX+icNsPo/MNHPK0UXnVNgE4w7FuQwbIo9GXIHOyHs52SpzPR0+g+jIZDR3VmAdMjV4fhhyQ1ViOequVyByxr0M7/hh7PRa34XUtcCJFAQHs6pBvMZUfrDzBIX+BNvSFmoGbX61msu6JtkycL8A/mGsEGmrSmEZx7vV9h/Qz0cOOAN9EBtJqrELzuwInOtQBMg08HjsfBXzRId+cKtduQr0LyNyxA1rSb1Qlz8HoYc1a51rpZDVDj45liVXAtAzK/GnKSsNMS/TCcnd7M/vEIc9eUfpeZvaiQ/pbYm3a1MzaHfK8b2bDrOPnOc8hn5nZV6y2+7SLma1KKXNV1PZM/+9ZD2fJZ8Z8wyf6oNDZNGZQdAVMJr2HfZbi0677o00hqrEW+EXs/DjcJu0zUfBdgb7ISJjGi9Q+l3yWdDdHXzp6EjIhaxEly1vsWd4kSofIJCspmv03R912GpciYbSheKc0ZgFPRa/XR0/LpmFoKItzTNTGNKZT+yR4U9S2anxEZat73eQdHlvvzh2g3uRMh3Qz0NwLNN5/JiX9POSGAbk5xjvUcXHs9TGkT9pBovtb7Lw/CrtI4zHg5uj1emhDi7RVI6jHTvvsT6BwkWzJeHxMcrZHWfunjO9mmvuMidIPNrkM0jg5VscdDumfNrOeUfq+ZvaKQx4zsynW8fOc6Jiv4CLa2szmRO+tMLNvWOV7NczMFjuUPbFKGXUfeYvoKo+yHnC4KXfH0p/hkH6RmQ2M0m9l6RNRM7PDY3Uc6pC+wIRYvtFm9q5DnnOi9EdY6RciXl78WMfM7nMo+zoza6tQRkuJaE2i4bPrLGd3h5tiJj8RJt/cqw7pL4zVcY5D+tdNvU8hz2zHdpmZ7RHl2cbMXnJIf75phTmjzLVPTT1T8j4NNrO7HMq+tUzelhXR0kTjPzB5m2st5zKHG/Mv07cQq33o62Vu/9hzY236grmZDgo8bmZXmJb5aRRMIftVSXOlmW1kZr3NbHPTsJzmaDXTkJ2VA7whInquzIeYVGMZQ8wtlGNyLM/9DulnxtJPdEi/1MyGxvJc55CnVhaZ2UmxOnqY2SVV0r9rEn/SHleON8zsVKvv/9hUEV1V5sM8WGMZFzncoLfMbECUfh+H9GYdY5oedkh/Xiy96/zJlTfM7CzTcFTuHkw0s6fqLPtJMzulStmZH1m7PWZR6tcZj56Hcgl/ABnnrk9J8xDFPRZ7oE08q7lXFqLlLSiicI+U8t9DT74WOAE3v9OdKBTjaORVXxd5/VegCMnngfuBB6lur7kH+Avy501EbpLhyMDZP0qzBvnWFgOvIDfJo8i00NB9A7J+ZGgw8kclvdQ3oo0RWoE/AN9KSXMOis0BbT76Ivps1ViDYpoLluaC8W818AEK//C52QOQKDeMzj9BYm+n2Xso5dC9VZo7HF5DGXkdkyqPAv/nAzPbMJZnqkMes47mhm515GGx/lWF9y8Hts2hPlc2oqPluRK/puiD6o0e+Xbhl3W0qUuQh4iepBimEGcgGkqG5FBnGoPQxlrVwkZBc6cLYud7olCUNJ4iuwjOTkdevrOplB//t0QPMKZ5zbNkGJrsJqMuy3ESmr9AbZGL1yOHbrckLxE9D9xQ4dq2KAzjgJzqjjMauI/SnWnLcXWUtsCuuDlnl6JVWbclTy/+FIre9SRDUKjpdDrunJYV66Fe5THcAulfprTXcQkRAW2g/q5707oeeW8tMwZtLVMtzmUpsvNchWKyfRiMYpBOR4/QuLAMzX2eib23E8X4obS8o+nmv1rUiJ3Svoo2NO+Vkq4dDSd3IcPgfxzLH4ZijA9GjzMnH1mqxlpkM5qZeH8q2sEkbZ5zE+6PMnVZGrV77FFo6ey6GdNyZLSch8T0FsXdKwZFxwjUC4wkPci+HKtRhOLNZa71p/S3RcrxIcVHiLotjdyCeB80bG3SqAqrsAw4FLkXAp40cgviB9Gj0M+kJcyZf6A5UBBQRjT6ZxnmIyFdgNsGTFmyElnNx9J8IXcpmvkDMcPRKupY0gPMfViO7DjTyWBDp0AprfBTVaPQzmqHkcH+gTHmIvfLDRSfdA3kQCuIqEA/ZFkeh0IqhqNVVz+HvO1oeFyANiyfjew84WemGkAriSjQSWnW750FuhBBRAFvgogC3gQRBbwJIgp4E0QU8CaIKOBNEFHAmyCigDdBRAFvgogC3gQRBbwJIgp4E0QU8CaIKOBNEFHAmyCigDdBRAFvgogC3vwPN7k7QTq1nHAAAAAASUVORK5CYII=", self.location).href,
-    ze = new URL("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJEAAABfCAYAAADoOiXnAAAMUElEQVR4nO2de5RVVR3HP4MSAwgIakqWiqIIkoHVivKxUksx6SE+kwg105VY+ShJzUdWmpWhaWpaLjNExSYN8YEPTNOFL0QFRRHTJYgi4AMUH8z47Y/fOeveObPP495z595zV/uz1ln3ztl7n9+eM985+7dfv9MiCY8nDz0aXQFP8+NF5MmNF5EnN15Entx4EXly40XkyY0XkSc3XkSe3HgReXLjReTJjReRJzdeRJ7ceBF5cuNF5MmNF5EnNxs2ugIVMgDYGxgDDAzOfQgsAe4BFgC1WiA1FNgX2AnoGVx3eWBnLtBeIzvDgH2AHYFewEfAMuBu4FFgfY3sdBstTbIorRX4KvCd4HNgJL0dWAzcANwILMphazBwIDARGAV8LJL+cmDnWuDJHHa2BA7GfqedMaGGKLAzA/gb8HQOO92PpKIfIyXdpeyslXSWpAEV2ukp6RhJyzLaeS+w07tCO70CO69ktPOOpFMltVZop25HwyuQchwo6c2MNzvKg5K2zWhnU0kzqrQzKyifxc4Wkm6u0k6bpIEZ7XgRBcehktqrudtlPCNpaIqdwZLm5rRzr6RNUuxsJWleTjt3KLtg/+9FtJekd1Nu6CpJV6fkkUwgg2Ls9JU0O8M1QmZJWhSTdqPim7b+ku6rwM7Nkp6PSWuTNb2N/hsVWkS9JD2Qfp81X9IQScsz5D0vxtaUDGVDFstENy0hz9kxds6qwM5Cmf/TlpBnSoydhhxFHCc6HNg1Q77HgReBSzLkPQH4YuTccOAUR97ngJWO81OAd0keFjkJ2CVybhhwoiPvImB15JyAnwLvp9g5BRt6KARFFNG4yM8COiLn3gGuCr7/EVgYfF+He/ymFTgscu4gYJAj753YH2gKpTGho4CbgvSke9YvyFvOOGx8K8pMYARwOjAHeAiYBNwepLck2BkEHJGQXl8a/SiMHIMlLY08utslnStpnKTDJR0saftIuWGS9pM50TtLusLRBDyizt3kWY48kvSBpC8n1PGGmHIhT0vauCz/bTH51kkak2BnZoqdeZL6JJSv29HwCkSOXSStd9yw/0raM+M1DpH0muMab6skvk0kPefIE/K0zBl2XX93WW/s9Ziya8vsDJb0YoKd+Yp3xvcK7KyKKbtK0jYxZet6FK056w1s4Dg/BHvk/xWbGnDRAkzFRpM3j7l23+B7X2DjhHqMACbHpP0H2BPYAWsS5zvqETZFaXZGAd+PSZsT2Nkea4oXJNhpKEUT0ft09X/KOQo4PyZtGuZAx1HuWwmbo0oiqR7hNVZi82nR8+Xf0+ykpQO8DrzqsFOIOauiTcCuAFYBWyTk2Sbm/IcZrw2wJsXOXcAFMWkTgaOxXtfHSX4ahHZcDjzALcT3Lo/EnOcdAzuFpWhPomVY1z2JO4PPjYH9saYH4BfAGwnlnqD03/w28HxMvhWYSOKeROOBPbAmM605WUn85OlS4JiEsocGdgotICieiMCeAnG8hXW1twHuB2YBj2FN3EuUBObinsjPc2Py3YR1yc8Nrn8d8C1KgvkgwYaLu2POt2FCPB+4NbDz9bL0Su00jkZ79o5jM9nosIvZsq68a6a9TdIZMeWeDa5bbmeo3D2stZI+dJy/Jig3PcZGefkdyuxsJ2m1I9+aGDtXBuVuSrHje2cJrAR+H5P2aeB6bC1OlAOA43E7qufQdRR6CXChI+9GdF7bEzIxON6LqVscLwB/cpzvF2PnaGydUaV2GkYRRQRwBfAHx/nBQP+YMi2Y/xD9nS4BpseUuRi4r4J6HYaNflfKVODhCvIfSvE6PbEUVUQAPwP+nPMa07G5qDjWAt/DVkVmYRDV/XHfxHpbL2XMPxD3eFkhKbKI1mPN06mkd99dXIg1De+n5HsBc2ifyHDNudj8XDUsCuw8kyHvwzSRY11kEYFNpv4Gm9WfQfqNFdYb2hs4mex+xWJssfy0hDyrMd8mzz1bCHwF+HtCnteAy3H7S4WkWdrdxzB/5LPAXtgyjs2xKZD12B/4eeABzMepZofESqzJuQUb5NuD0jTJPGxW/wW6LtyvlFcDO3cEdnYF+gRpj2Lifxkvom5BmJge60Yb7dgTrw2bs/oktoboqeATqnOso3Rg/tqMwM6WDjtxc4SFo5lEVE86gGeDo5z+wMga2mnHfKXoFqdBlEbiC0/RfaJ6kzaNcSK2qTGJHhmuk5Z+CrBVDezUBS+izoyn6wrIkCOxnmIaK0iewwMbBzooJu1YbJltGq9msFMXfHPWmRHY6PY44GbMYe8PfAP4Ltnu1wO412iXMxw4E9vdOhMTwwBs1H0i2f65H8QmkhuOF1Fnwpn7CcFRDTdmyBP2HicFR6Uoo5264Juz2vIvbIigu5lB8mqHuuJFVDveBs6rg53VdbKTGS+i2nESlU2yVsvp5ItGUnO8iDpTbZf5Akr74LJQ7eTqr8g/KV1zvIg6s6bC/ML+sD+psFylXfMO4IzgKB6NXhVXsKOnpGMlLYlfUChJ6pBtHty3SjsbSJqs5D1poZ1HlH3PXUOOZomUVm/6AmOxjQDDsbGiDmzrzgJsHfZc8ofC6wd8LbA1DNt80I4NWC7AensPUrvQft2CF1E6LZgP44oJ0B12PiLbXrTC4EXkyY13rD258SLy5KYoc2efA/bDfAHfvmanFduUWcmOlZpTFBHtis2ee6qjoSIqSnNW+KjxBabh3f+iiMjTxHgR1ZdXsG1J0YCfTU2ziOh32JLSydhuUhergOOAQ4C/1KFOi7HNla7t3nGcjK1cjIvC1pQ0i4g6sIVYlxIfqmUmcBm24s8VrbXW/BLbzLikgjJhIIrBta9O42gWEY2ltJnvmpg81wafW2O7TGuJ6Or8h1MTlSzrOA8LbhUX9URYDKal2CK3ppj+aBYRjcJ2voIt/IrGL1xKaS/9PnR9lRXYrtKzsddQ7Y+9IupyLCZ2lMexQA9XYZHOJgC7YUE/Q8K1Rz2DOk3GgmFNxMLfuARwG/YEiy6hFba1+ptYMPXhwOexDQMzHdcpFo1eRhAcx6UsiZAsNnWY/+JI2kVlaXMcZe9VKSBUi6QNy/Lvq65hfqcFaZ+StHXwvVX2wpmQCcH5zSX1c/xOpznq8cMg7fjI+Z+XldtR0mdUCoE81XGdcs502K7r0SxPIrAgDWEAzRsiaeHOh6HY6Hc5q4AfYGFdvoSFtnsSuBLbIDgbc3jLCQdhl2L+y2VY5P7tHfVagcUIuB74J/ZE6oGF67sj5rrlTeAyzNcDi2KyCAtr/ARwEZ1D8BWSooxYZ2FbrLm4CrvJz2D7xJ7CAi6AbTzsFyl3DbYduj/mCI8Kzo/A1u8cjK0POhmLxFbOEKw52SyhXiMxUYcBOg/AmqdLsb1rY1N+rw5KS0yWYkEjtgts/yilbCFopicRlHanvgv8I/h+NRZCZgPM34nyUPC5OyUBhYzGFqCtoWtQc7CA50kCAntCRiO8jg8+55G+BmlrSrthZwd13AeLQjInpWwhaDYR7UKpm3wb1lSFTupo3EEQwhhFGznS+lAaDqgmkFYcYbP7BtliJF0M/Br7/dqxPWW/xQRayThUQ2g2EW2CNWlgg31XY70usEFGV+ygMMaja5T4rbLzfR3pWXBtmX4t+OxHthAxvYHTsPhEc7EYj6ODtDPIFl2tYTSbiMDehwY2ch2G4mvFuu0udgs+76Nr83ArFn1tC8zprobpdHb012BOOMAXyBasaj3W7PXAmrMTKG1QXIet7S4szeRYh4zGnNmFlGawx2CvL3AxAeuJzcfeDfJjzGm9n1Jo4ImYb1IJ4bqnPtiY0v2Yb9SGLbIfQPZ3kp2D+U/jgU0xIU4N0jarom51pRlF1Bv4NrYTNGQS8U/V/thA3vHAv+kctqUXJqpzI2VCZzjJTwoHEydhzehFZWk7YL5M9G2PHZFPsMCk87GX5d0eyf+J4LpDEurRcJpRRGD/+cMoCWfvlPw7YWM2d2Fzb8uxZmMsXV+3CdaTuw530PWQE7ExnJHAzthTZAXmB43B/YqqI+j61GzFOgfzsLA0y4NrbItN37heu1UoirLb4zjcUec96ZxFg1eFNqNj7SkYRRFRUerRjDT83hXFJ1qHddnb8bs9KqEfpZDFDaMoPpGniWn4o9DT/HgReXLjReTJjReRJzdeRJ7ceBF5cuNF5MmNF5EnN15Entx4EXly40XkyY0XkSc3XkSe3HgReXLjReTJzf8A7VafuKusJ8IAAAAASUVORK5CYII=", self.location).href;
+    ye = new URL("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJEAAABfCAYAAADoOiXnAAAMUElEQVR4nO2de5RVVR3HP4MSAwgIakqWiqIIkoHVivKxUksx6SE+kwg105VY+ShJzUdWmpWhaWpaLjNExSYN8YEPTNOFL0QFRRHTJYgi4AMUH8z47Y/fOeveObPP495z595zV/uz1ln3ztl7n9+eM985+7dfv9MiCY8nDz0aXQFP8+NF5MmNF5EnN15Entx4EXly40XkyY0XkSc3XkSe3HgReXLjReTJjReRJzdeRJ7ceBF5cuNF5MmNF5EnNxs2ugIVMgDYGxgDDAzOfQgsAe4BFgC1WiA1FNgX2AnoGVx3eWBnLtBeIzvDgH2AHYFewEfAMuBu4FFgfY3sdBstTbIorRX4KvCd4HNgJL0dWAzcANwILMphazBwIDARGAV8LJL+cmDnWuDJHHa2BA7GfqedMaGGKLAzA/gb8HQOO92PpKIfIyXdpeyslXSWpAEV2ukp6RhJyzLaeS+w07tCO70CO69ktPOOpFMltVZop25HwyuQchwo6c2MNzvKg5K2zWhnU0kzqrQzKyifxc4Wkm6u0k6bpIEZ7XgRBcehktqrudtlPCNpaIqdwZLm5rRzr6RNUuxsJWleTjt3KLtg/+9FtJekd1Nu6CpJV6fkkUwgg2Ls9JU0O8M1QmZJWhSTdqPim7b+ku6rwM7Nkp6PSWuTNb2N/hsVWkS9JD2Qfp81X9IQScsz5D0vxtaUDGVDFstENy0hz9kxds6qwM5Cmf/TlpBnSoydhhxFHCc6HNg1Q77HgReBSzLkPQH4YuTccOAUR97ngJWO81OAd0keFjkJ2CVybhhwoiPvImB15JyAnwLvp9g5BRt6KARFFNG4yM8COiLn3gGuCr7/EVgYfF+He/ymFTgscu4gYJAj753YH2gKpTGho4CbgvSke9YvyFvOOGx8K8pMYARwOjAHeAiYBNwepLck2BkEHJGQXl8a/SiMHIMlLY08utslnStpnKTDJR0saftIuWGS9pM50TtLusLRBDyizt3kWY48kvSBpC8n1PGGmHIhT0vauCz/bTH51kkak2BnZoqdeZL6JJSv29HwCkSOXSStd9yw/0raM+M1DpH0muMab6skvk0kPefIE/K0zBl2XX93WW/s9Ziya8vsDJb0YoKd+Yp3xvcK7KyKKbtK0jYxZet6FK056w1s4Dg/BHvk/xWbGnDRAkzFRpM3j7l23+B7X2DjhHqMACbHpP0H2BPYAWsS5zvqETZFaXZGAd+PSZsT2Nkea4oXJNhpKEUT0ft09X/KOQo4PyZtGuZAx1HuWwmbo0oiqR7hNVZi82nR8+Xf0+ykpQO8DrzqsFOIOauiTcCuAFYBWyTk2Sbm/IcZrw2wJsXOXcAFMWkTgaOxXtfHSX4ahHZcDjzALcT3Lo/EnOcdAzuFpWhPomVY1z2JO4PPjYH9saYH4BfAGwnlnqD03/w28HxMvhWYSOKeROOBPbAmM605WUn85OlS4JiEsocGdgotICieiMCeAnG8hXW1twHuB2YBj2FN3EuUBObinsjPc2Py3YR1yc8Nrn8d8C1KgvkgwYaLu2POt2FCPB+4NbDz9bL0Su00jkZ79o5jM9nosIvZsq68a6a9TdIZMeWeDa5bbmeo3D2stZI+dJy/Jig3PcZGefkdyuxsJ2m1I9+aGDtXBuVuSrHje2cJrAR+H5P2aeB6bC1OlAOA43E7qufQdRR6CXChI+9GdF7bEzIxON6LqVscLwB/cpzvF2PnaGydUaV2GkYRRQRwBfAHx/nBQP+YMi2Y/xD9nS4BpseUuRi4r4J6HYaNflfKVODhCvIfSvE6PbEUVUQAPwP+nPMa07G5qDjWAt/DVkVmYRDV/XHfxHpbL2XMPxD3eFkhKbKI1mPN06mkd99dXIg1De+n5HsBc2ifyHDNudj8XDUsCuw8kyHvwzSRY11kEYFNpv4Gm9WfQfqNFdYb2hs4mex+xWJssfy0hDyrMd8mzz1bCHwF+HtCnteAy3H7S4WkWdrdxzB/5LPAXtgyjs2xKZD12B/4eeABzMepZofESqzJuQUb5NuD0jTJPGxW/wW6LtyvlFcDO3cEdnYF+gRpj2Lifxkvom5BmJge60Yb7dgTrw2bs/oktoboqeATqnOso3Rg/tqMwM6WDjtxc4SFo5lEVE86gGeDo5z+wMga2mnHfKXoFqdBlEbiC0/RfaJ6kzaNcSK2qTGJHhmuk5Z+CrBVDezUBS+izoyn6wrIkCOxnmIaK0iewwMbBzooJu1YbJltGq9msFMXfHPWmRHY6PY44GbMYe8PfAP4Ltnu1wO412iXMxw4E9vdOhMTwwBs1H0i2f65H8QmkhuOF1Fnwpn7CcFRDTdmyBP2HicFR6Uoo5264Juz2vIvbIigu5lB8mqHuuJFVDveBs6rg53VdbKTGS+i2nESlU2yVsvp5ItGUnO8iDpTbZf5Akr74LJQ7eTqr8g/KV1zvIg6s6bC/ML+sD+psFylXfMO4IzgKB6NXhVXsKOnpGMlLYlfUChJ6pBtHty3SjsbSJqs5D1poZ1HlH3PXUOOZomUVm/6AmOxjQDDsbGiDmzrzgJsHfZc8ofC6wd8LbA1DNt80I4NWC7AensPUrvQft2CF1E6LZgP44oJ0B12PiLbXrTC4EXkyY13rD258SLy5KYoc2efA/bDfAHfvmanFduUWcmOlZpTFBHtis2ee6qjoSIqSnNW+KjxBabh3f+iiMjTxHgR1ZdXsG1J0YCfTU2ziOh32JLSydhuUhergOOAQ4C/1KFOi7HNla7t3nGcjK1cjIvC1pQ0i4g6sIVYlxIfqmUmcBm24s8VrbXW/BLbzLikgjJhIIrBta9O42gWEY2ltJnvmpg81wafW2O7TGuJ6Or8h1MTlSzrOA8LbhUX9URYDKal2CK3ppj+aBYRjcJ2voIt/IrGL1xKaS/9PnR9lRXYrtKzsddQ7Y+9IupyLCZ2lMexQA9XYZHOJgC7YUE/Q8K1Rz2DOk3GgmFNxMLfuARwG/YEiy6hFba1+ptYMPXhwOexDQMzHdcpFo1eRhAcx6UsiZAsNnWY/+JI2kVlaXMcZe9VKSBUi6QNy/Lvq65hfqcFaZ+StHXwvVX2wpmQCcH5zSX1c/xOpznq8cMg7fjI+Z+XldtR0mdUCoE81XGdcs502K7r0SxPIrAgDWEAzRsiaeHOh6HY6Hc5q4AfYGFdvoSFtnsSuBLbIDgbc3jLCQdhl2L+y2VY5P7tHfVagcUIuB74J/ZE6oGF67sj5rrlTeAyzNcDi2KyCAtr/ARwEZ1D8BWSooxYZ2FbrLm4CrvJz2D7xJ7CAi6AbTzsFyl3DbYduj/mCI8Kzo/A1u8cjK0POhmLxFbOEKw52SyhXiMxUYcBOg/AmqdLsb1rY1N+rw5KS0yWYkEjtgts/yilbCFopicRlHanvgv8I/h+NRZCZgPM34nyUPC5OyUBhYzGFqCtoWtQc7CA50kCAntCRiO8jg8+55G+BmlrSrthZwd13AeLQjInpWwhaDYR7UKpm3wb1lSFTupo3EEQwhhFGznS+lAaDqgmkFYcYbP7BtliJF0M/Br7/dqxPWW/xQRayThUQ2g2EW2CNWlgg31XY70usEFGV+ygMMaja5T4rbLzfR3pWXBtmX4t+OxHthAxvYHTsPhEc7EYj6ODtDPIFl2tYTSbiMDehwY2ch2G4mvFuu0udgs+76Nr83ArFn1tC8zprobpdHb012BOOMAXyBasaj3W7PXAmrMTKG1QXIet7S4szeRYh4zGnNmFlGawx2CvL3AxAeuJzcfeDfJjzGm9n1Jo4ImYb1IJ4bqnPtiY0v2Yb9SGLbIfQPZ3kp2D+U/jgU0xIU4N0jarom51pRlF1Bv4NrYTNGQS8U/V/thA3vHAv+kctqUXJqpzI2VCZzjJTwoHEydhzehFZWk7YL5M9G2PHZFPsMCk87GX5d0eyf+J4LpDEurRcJpRRGD/+cMoCWfvlPw7YWM2d2Fzb8uxZmMsXV+3CdaTuw530PWQE7ExnJHAzthTZAXmB43B/YqqI+j61GzFOgfzsLA0y4NrbItN37heu1UoirLb4zjcUec96ZxFg1eFNqNj7SkYRRFRUerRjDT83hXFJ1qHddnb8bs9KqEfpZDFDaMoPpGniWn4o9DT/HgReXLjReTJjReRJzdeRJ7ceBF5cuNF5MmNF5EnN15Entx4EXly40XkyY0XkSc3XkSe3HgReXLjReTJzf8A7VafuKusJ8IAAAAASUVORK5CYII=", self.location).href;
 new URL("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJEAAABfCAYAAADoOiXnAAAMUElEQVR4nO2de5RVVR3HP4MSAwgIakqWiqIIkoHVivKxUksx6SE+kwg105VY+ShJzUdWmpWhaWpaLjNExSYN8YEPTNOFL0QFRRHTJYgi4AMUH8z47Y/fOeveObPP495z595zV/uz1ln3ztl7n9+eM985+7dfv9MiCY8nDz0aXQFP8+NF5MmNF5EnN15Entx4EXly40XkyY0XkSc3XkSe3HgReXLjReTJjReRJzdeRJ7ceBF5cuNF5MmNF5EnNxs2ugIVMgDYGxgDDAzOfQgsAe4BFgC1WiA1FNgX2AnoGVx3eWBnLtBeIzvDgH2AHYFewEfAMuBu4FFgfY3sdBstTbIorRX4KvCd4HNgJL0dWAzcANwILMphazBwIDARGAV8LJL+cmDnWuDJHHa2BA7GfqedMaGGKLAzA/gb8HQOO92PpKIfIyXdpeyslXSWpAEV2ukp6RhJyzLaeS+w07tCO70CO69ktPOOpFMltVZop25HwyuQchwo6c2MNzvKg5K2zWhnU0kzqrQzKyifxc4Wkm6u0k6bpIEZ7XgRBcehktqrudtlPCNpaIqdwZLm5rRzr6RNUuxsJWleTjt3KLtg/+9FtJekd1Nu6CpJV6fkkUwgg2Ls9JU0O8M1QmZJWhSTdqPim7b+ku6rwM7Nkp6PSWuTNb2N/hsVWkS9JD2Qfp81X9IQScsz5D0vxtaUDGVDFstENy0hz9kxds6qwM5Cmf/TlpBnSoydhhxFHCc6HNg1Q77HgReBSzLkPQH4YuTccOAUR97ngJWO81OAd0keFjkJ2CVybhhwoiPvImB15JyAnwLvp9g5BRt6KARFFNG4yM8COiLn3gGuCr7/EVgYfF+He/ymFTgscu4gYJAj753YH2gKpTGho4CbgvSke9YvyFvOOGx8K8pMYARwOjAHeAiYBNwepLck2BkEHJGQXl8a/SiMHIMlLY08utslnStpnKTDJR0saftIuWGS9pM50TtLusLRBDyizt3kWY48kvSBpC8n1PGGmHIhT0vauCz/bTH51kkak2BnZoqdeZL6JJSv29HwCkSOXSStd9yw/0raM+M1DpH0muMab6skvk0kPefIE/K0zBl2XX93WW/s9Ziya8vsDJb0YoKd+Yp3xvcK7KyKKbtK0jYxZet6FK056w1s4Dg/BHvk/xWbGnDRAkzFRpM3j7l23+B7X2DjhHqMACbHpP0H2BPYAWsS5zvqETZFaXZGAd+PSZsT2Nkea4oXJNhpKEUT0ft09X/KOQo4PyZtGuZAx1HuWwmbo0oiqR7hNVZi82nR8+Xf0+ykpQO8DrzqsFOIOauiTcCuAFYBWyTk2Sbm/IcZrw2wJsXOXcAFMWkTgaOxXtfHSX4ahHZcDjzALcT3Lo/EnOcdAzuFpWhPomVY1z2JO4PPjYH9saYH4BfAGwnlnqD03/w28HxMvhWYSOKeROOBPbAmM605WUn85OlS4JiEsocGdgotICieiMCeAnG8hXW1twHuB2YBj2FN3EuUBObinsjPc2Py3YR1yc8Nrn8d8C1KgvkgwYaLu2POt2FCPB+4NbDz9bL0Su00jkZ79o5jM9nosIvZsq68a6a9TdIZMeWeDa5bbmeo3D2stZI+dJy/Jig3PcZGefkdyuxsJ2m1I9+aGDtXBuVuSrHje2cJrAR+H5P2aeB6bC1OlAOA43E7qufQdRR6CXChI+9GdF7bEzIxON6LqVscLwB/cpzvF2PnaGydUaV2GkYRRQRwBfAHx/nBQP+YMi2Y/xD9nS4BpseUuRi4r4J6HYaNflfKVODhCvIfSvE6PbEUVUQAPwP+nPMa07G5qDjWAt/DVkVmYRDV/XHfxHpbL2XMPxD3eFkhKbKI1mPN06mkd99dXIg1De+n5HsBc2ifyHDNudj8XDUsCuw8kyHvwzSRY11kEYFNpv4Gm9WfQfqNFdYb2hs4mex+xWJssfy0hDyrMd8mzz1bCHwF+HtCnteAy3H7S4WkWdrdxzB/5LPAXtgyjs2xKZD12B/4eeABzMepZofESqzJuQUb5NuD0jTJPGxW/wW6LtyvlFcDO3cEdnYF+gRpj2Lifxkvom5BmJge60Yb7dgTrw2bs/oktoboqeATqnOso3Rg/tqMwM6WDjtxc4SFo5lEVE86gGeDo5z+wMga2mnHfKXoFqdBlEbiC0/RfaJ6kzaNcSK2qTGJHhmuk5Z+CrBVDezUBS+izoyn6wrIkCOxnmIaK0iewwMbBzooJu1YbJltGq9msFMXfHPWmRHY6PY44GbMYe8PfAP4Ltnu1wO412iXMxw4E9vdOhMTwwBs1H0i2f65H8QmkhuOF1Fnwpn7CcFRDTdmyBP2HicFR6Uoo5264Juz2vIvbIigu5lB8mqHuuJFVDveBs6rg53VdbKTGS+i2nESlU2yVsvp5ItGUnO8iDpTbZf5Akr74LJQ7eTqr8g/KV1zvIg6s6bC/ML+sD+psFylXfMO4IzgKB6NXhVXsKOnpGMlLYlfUChJ6pBtHty3SjsbSJqs5D1poZ1HlH3PXUOOZomUVm/6AmOxjQDDsbGiDmzrzgJsHfZc8ofC6wd8LbA1DNt80I4NWC7AensPUrvQft2CF1E6LZgP44oJ0B12PiLbXrTC4EXkyY13rD258SLy5KYoc2efA/bDfAHfvmanFduUWcmOlZpTFBHtis2ee6qjoSIqSnNW+KjxBabh3f+iiMjTxHgR1ZdXsG1J0YCfTU2ziOh32JLSydhuUhergOOAQ4C/1KFOi7HNla7t3nGcjK1cjIvC1pQ0i4g6sIVYlxIfqmUmcBm24s8VrbXW/BLbzLikgjJhIIrBta9O42gWEY2ltJnvmpg81wafW2O7TGuJ6Or8h1MTlSzrOA8LbhUX9URYDKal2CK3ppj+aBYRjcJ2voIt/IrGL1xKaS/9PnR9lRXYrtKzsddQ7Y+9IupyLCZ2lMexQA9XYZHOJgC7YUE/Q8K1Rz2DOk3GgmFNxMLfuARwG/YEiy6hFba1+ptYMPXhwOexDQMzHdcpFo1eRhAcx6UsiZAsNnWY/+JI2kVlaXMcZe9VKSBUi6QNy/Lvq65hfqcFaZ+StHXwvVX2wpmQCcH5zSX1c/xOpznq8cMg7fjI+Z+XldtR0mdUCoE81XGdcs502K7r0SxPIrAgDWEAzRsiaeHOh6HY6Hc5q4AfYGFdvoSFtnsSuBLbIDgbc3jLCQdhl2L+y2VY5P7tHfVagcUIuB74J/ZE6oGF67sj5rrlTeAyzNcDi2KyCAtr/ARwEZ1D8BWSooxYZ2FbrLm4CrvJz2D7xJ7CAi6AbTzsFyl3DbYduj/mCI8Kzo/A1u8cjK0POhmLxFbOEKw52SyhXiMxUYcBOg/AmqdLsb1rY1N+rw5KS0yWYkEjtgts/yilbCFopicRlHanvgv8I/h+NRZCZgPM34nyUPC5OyUBhYzGFqCtoWtQc7CA50kCAntCRiO8jg8+55G+BmlrSrthZwd13AeLQjInpWwhaDYR7UKpm3wb1lSFTupo3EEQwhhFGznS+lAaDqgmkFYcYbP7BtliJF0M/Br7/dqxPWW/xQRayThUQ2g2EW2CNWlgg31XY70usEFGV+ygMMaja5T4rbLzfR3pWXBtmX4t+OxHthAxvYHTsPhEc7EYj6ODtDPIFl2tYTSbiMDehwY2ch2G4mvFuu0udgs+76Nr83ArFn1tC8zprobpdHb012BOOMAXyBasaj3W7PXAmrMTKG1QXIet7S4szeRYh4zGnNmFlGawx2CvL3AxAeuJzcfeDfJjzGm9n1Jo4ImYb1IJ4bqnPtiY0v2Yb9SGLbIfQPZ3kp2D+U/jgU0xIU4N0jarom51pRlF1Bv4NrYTNGQS8U/V/thA3vHAv+kctqUXJqpzI2VCZzjJTwoHEydhzehFZWk7YL5M9G2PHZFPsMCk87GX5d0eyf+J4LpDEurRcJpRRGD/+cMoCWfvlPw7YWM2d2Fzb8uxZmMsXV+3CdaTuw530PWQE7ExnJHAzthTZAXmB43B/YqqI+j61GzFOgfzsLA0y4NrbItN37heu1UoirLb4zjcUec96ZxFg1eFNqNj7SkYRRFRUerRjDT83hXFJ1qHddnb8bs9KqEfpZDFDaMoPpGniWn4o9DT/HgReXLjReTJjReRJzdeRJ7ceBF5cuNF5MmNF5EnN15Entx4EXly40XkyY0XkSc3XkSe3HgReXLjReTJzf8A7VafuKusJ8IAAAAASUVORK5CYII=", self.location).href;
-const De = new URL("" + new URL("m4a-45331b05.png", import.meta.url).href, self.location).href,
+const Ie = new URL("" + new URL("m4a-45331b05.png", import.meta.url).href, self.location).href,
     Ze = new URL("" + new URL("hires-438c7046.png", import.meta.url).href, self.location).href,
-    ye = new URL("" + new URL("cover_dark-75402cd0.png", import.meta.url).href, self.location).href,
-    Je = new URL("" + new URL("cover_light-b832ae9e.png", import.meta.url).href, self.location).href,
-    Me = new URL("" + new URL("folder-6b5595ac.svg", import.meta.url).href, self.location).href,
+    Je = new URL("" + new URL("cover_dark-75402cd0.png", import.meta.url).href, self.location).href,
+    Me = new URL("" + new URL("cover_light-b832ae9e.png", import.meta.url).href, self.location).href,
+    Oe = new URL("" + new URL("folder-6b5595ac.svg", import.meta.url).href, self.location).href,
     Ve = S({
         __name: "QualityDetailsBtn",
         setup(e) {
             const t = Y(() => {
                     var a, A;
-                    return (A = (a = k.activePlayerQueue) == null ? void 0 : a.current_item) == null ? void 0 : A.streamdetails
+                    return (A = (a = R.activePlayerQueue) == null ? void 0 : a.current_item) == null ? void 0 : A.streamdetails
                 }),
                 i = function(a) {
-                    return a == m.AAC ? Ce : a == m.FLAC ? we : a == m.MP3 || a == m.MPEG ? N : a == m.OGG ? ze : a == m.M4A ? De : Fe
+                    return a == m.AAC ? we : a == m.FLAC ? ze : a == m.MP3 || a == m.MPEG ? N : a == m.OGG ? ye : a == m.M4A ? Ie : De
                 };
-            return (a, A) => t.value ? (B(), M(ie, {
+            return (a, A) => t.value ? (v(), M(ne, {
                 key: 0,
                 location: "bottom end",
                 "close-on-content-click": !1
             }, {
                 activator: c(({
-                    props: o
+                    props: s
                 }) => {
-                    var s, l;
-                    return [t.value ? (B(), M($, C({
+                    var o, l;
+                    return [t.value ? (v(), M(ee, w({
                         key: 0,
-                        disabled: !h(k).activePlayerQueue || !((s = h(k).activePlayerQueue) != null && s.active) || ((l = h(k).activePlayerQueue) == null ? void 0 : l.items) == 0,
+                        disabled: !h(R).activePlayerQueue || !((o = h(R).activePlayerQueue) != null && o.active) || ((l = h(R).activePlayerQueue) == null ? void 0 : l.items) == 0,
                         class: "mediadetails-content-type-btn",
                         label: "",
                         ripple: !1
-                    }, o), {
-                        default: c(() => [b("div", Re, g(t.value.audio_format.content_type.toUpperCase()), 1)]),
+                    }, s), {
+                        default: c(() => [b("div", Be, g(t.value.audio_format.content_type.toUpperCase()), 1)]),
                         _: 2
-                    }, 1040, ["disabled"])) : F("", !0)]
+                    }, 1040, ["disabled"])) : D("", !0)]
                 }),
-                default: c(() => [r(be, {
+                default: c(() => [r(ke, {
                     class: "mx-auto",
                     width: "300"
                 }, {
-                    default: c(() => [r(ee, {
+                    default: c(() => [r(te, {
                         style: {
                             overflow: "hidden"
                         }
                     }, {
                         default: c(() => {
-                            var o, s;
-                            return [r(te, {
+                            var s, o;
+                            return [r(ae, {
                                 class: "list-item list-item-main",
                                 "min-height": 5
                             }, {
-                                default: c(() => [r(ae, {
+                                default: c(() => [r(ie, {
                                     class: "text-h5 mb-1"
                                 }, {
-                                    default: c(() => [R(g(a.$t("stream_details")), 1)]),
+                                    default: c(() => [B(g(a.$t("stream_details")), 1)]),
                                     _: 1
                                 })]),
                                 _: 1
-                            }), r(ne), b("div", Be, [r(q, {
+                            }), r(Ae), b("div", ve, [r(_, {
                                 domain: t.value.provider,
                                 size: 35,
                                 style: {
                                     "object-fit": "contain",
                                     "margin-left": "10px",
                                     "margin-right": "5px"
                                 }
-                            }, null, 8, ["domain"]), R(" " + g(((o = h(w).providerManifests[t.value.provider]) == null ? void 0 : o.name) || ((s = h(w).providers[t.value.provider]) == null ? void 0 : s.name)), 1)]), b("div", pe, [b("img", {
+                            }, null, 8, ["domain"]), B(" " + g(((s = h(z).providerManifests[t.value.provider]) == null ? void 0 : s.name) || ((o = h(z).providers[t.value.provider]) == null ? void 0 : o.name)), 1)]), b("div", Fe, [b("img", {
                                 height: "30",
                                 width: "50",
                                 src: i(t.value.audio_format.content_type),
                                 style: O(a.$vuetify.theme.current.dark ? "object-fit: contain;" : "object-fit: contain;filter: invert(100%);")
-                            }, null, 12, ve), R(" " + g(t.value.audio_format.sample_rate / 1e3) + " kHz / " + g(t.value.audio_format.bit_depth) + " bits ", 1)]), t.value.gain_correct ? (B(), E("div", Ie, [b("img", {
+                            }, null, 12, pe), B(" " + g(t.value.audio_format.sample_rate / 1e3) + " kHz / " + g(t.value.audio_format.bit_depth) + " bits ", 1)]), t.value.target_loudness ? (v(), E("div", Ce, [b("img", {
                                 height: "30",
                                 width: "50",
                                 contain: "",
-                                src: ke,
+                                src: Re,
                                 style: O(a.$vuetify.theme.current.dark ? "object-fit: contain;" : "object-fit: contain;filter: invert(100%);")
-                            }, null, 4), R(" " + g(t.value.gain_correct) + " dB ", 1)])) : F("", !0)]
+                            }, null, 4), B(" " + g(t.value.target_loudness) + " dB ", 1)])) : D("", !0)]
                         }),
                         _: 1
                     })]),
                     _: 1
                 })]),
                 _: 1
-            })) : F("", !0)
+            })) : D("", !0)
         }
     });
-const Oe = ["loading", "height", "width", "src"],
-    He = function(e, t = !1, i = 256) {
+const He = ["loading", "height", "width", "src"],
+    Ne = function(e, t = !1, i = 256) {
         return t ? `https://ui-avatars.com/api/?name=${e}&size=${i||256}&bold=true&background=1d1d1d&color=383838` : `https://ui-avatars.com/api/?name=${e}&size=${i||256}&bold=true&background=a0a0a0&color=cccccc`
     },
-    Ne = function(e, t = z.THUMB, i = !1) {
+    P = function(e, t = k.THUMB, i = !1) {
         if (e) {
             if ("image" in e && e.image) return e.image;
             if ("metadata" in e && e.metadata.images) {
                 for (const a of e.metadata.images)
-                    if (!(a.provider == "http" && !i) && a.type == t) return a
+                    if (!(!a.remotely_accessible && !i) && a.type == t) return a
             }
             if ("album" in e && e.album && "metadata" in e.album && e.album.metadata && e.album.metadata.images) {
                 for (const a of e.album.metadata.images)
-                    if (!(a.provider == "http" && !i) && a.type == t) return a
+                    if (!(!a.remotely_accessible && !i) && a.type == t) return a
             }
+            if ("album" in e && e.album && "image" in e.album && e.album.image && e.album.image.type == t && (e.album.image.remotely_accessible || i)) return e.album.image;
             if ("artist" in e && "metadata" in e.artist && e.artist.metadata && e.artist.metadata.images) {
                 for (const a of e.artist.metadata.images)
-                    if (!(a.provider == "http" && !i) && a.type == t) return a
+                    if (!(!a.remotely_accessible && !i) && a.type == t) return a
             }
             if ("artists" in e && e.artists) {
                 for (const a of e.artists)
                     if ("metadata" in a && a.metadata.images) {
                         for (const A of a.metadata.images)
-                            if (!(A.provider == "http" && !i) && A.type == t) return A
+                            if (!(!A.remotely_accessible && !i) && A.type == t) return A
                     }
             }
+            if (t == k.THUMB) return P(e, k.LANDSCAPE, i)
         }
     },
-    Se = function(e, t = z.THUMB, i) {
+    Se = function(e, t = k.THUMB, i) {
         var A;
         if (!e) return;
-        const a = Ne(e, t, !0);
+        const a = P(e, t, !0);
         if (!(!a || !a.path)) {
             if (!a.remotely_accessible || i) {
-                const o = encodeURIComponent(encodeURIComponent(a.path)),
-                    s = "metadata" in e ? (A = e.metadata) == null ? void 0 : A.cache_checksum : "";
-                let l = `${w.baseUrl}/imageproxy?path=${o}&provider=${a.provider}&checksum=${s}`;
+                const s = encodeURIComponent(encodeURIComponent(a.path)),
+                    o = "metadata" in e ? (A = e.metadata) == null ? void 0 : A.cache_checksum : "";
+                let l = `${z.baseUrl}/imageproxy?path=${s}&provider=${a.provider}&checksum=${o}`;
                 return i ? l + `&size=${i}` : l
             }
             return a.path
         }
     },
     Ye = S({
         __name: "MediaItemThumb",
@@ -262,148 +264,148 @@
             rounded: {
                 type: Boolean,
                 default: !0
             }
         },
         setup(e) {
             const t = e,
-                i = X(),
+                i = L(),
                 a = {
-                    backgroundImage: `url(${i.current.value.dark?ye:Je})`
+                    backgroundImage: `url(${i.current.value.dark?Je:Me})`
                 };
 
             function A() {
                 return typeof t.size == "number" ? t.size : typeof t.width == "number" && typeof t.height == "number" ? t.height > t.width ? t.height : t.width : t.thumb ? 256 : 0
             }
-            const o = A();
+            const s = A();
 
-            function s() {
-                return t.fallback ? t.fallback : t.item && "media_type" in t.item && t.item.media_type == T.FOLDER ? Me : !t.item || !t.item.name ? "" : He(t.item.name, i.current.value.dark, o)
+            function o() {
+                return t.fallback ? t.fallback : t.item && "media_type" in t.item && t.item.media_type == x.FOLDER ? Oe : !t.item || !t.item.name ? "" : Ne(t.item.name, i.current.value.dark, s)
             }
-            const l = s(),
-                p = Y(() => t.item && Se(t.item, z.THUMB, o) || l),
-                d = L(null);
-            return P(() => {
-                const n = v => {
-                        v.forEach(I => {
-                            const f = I.target;
-                            f.complete && (f.style.backgroundImage = "", u.disconnect())
+            const l = o(),
+                F = Y(() => t.item && Se(t.item, k.THUMB, s) || l),
+                f = U(null);
+            return X(() => {
+                const n = p => {
+                        p.forEach(C => {
+                            const d = C.target;
+                            d.complete && (d.style.backgroundImage = "", u.disconnect())
                         })
                     },
                     u = new IntersectionObserver(n, {
                         root: null,
                         threshold: 1
                     });
-                d.value && u.observe(d.value)
-            }), (n, u) => (B(), E("img", {
+                f.value && u.observe(f.value)
+            }), (n, u) => (v(), E("img", {
                 ref_key: "imageTag",
-                ref: d,
+                ref: f,
                 loading: n.$props.lazy,
                 height: n.$props.size || n.$props.height || "600px",
                 width: n.$props.size || n.$props.width || "600px",
-                src: p.value,
-                class: U({
+                src: F.value,
+                class: T({
                     rounded: n.rounded
                 }),
                 style: a
-            }, null, 10, Oe))
+            }, null, 10, He))
         }
     });
-const Ge = _(Ye, [
-    ["__scopeId", "data-v-7b262f2c"]
+const Ge = $(Ye, [
+    ["__scopeId", "data-v-0e68fce2"]
 ]);
-const Ee = x({
+const Ee = Z({
         bordered: Boolean,
         color: String,
         content: [Number, String],
         dot: Boolean,
         floating: Boolean,
-        icon: Z,
+        icon: V,
         inline: Boolean,
         label: {
             type: String,
             default: "$vuetify.badge"
         },
         max: [Number, String],
         modelValue: {
             type: Boolean,
             default: !0
         },
         offsetX: [Number, String],
         offsetY: [Number, String],
         textColor: String,
-        ...Ae(),
+        ...se(),
         ...oe({
             location: "top end"
         }),
-        ...se(),
         ...re(),
-        ...V(),
-        ...le({
+        ...le(),
+        ...G(),
+        ...ce({
             transition: "scale-rotate-transition"
         })
     }, "VBadge"),
-    Ke = G()({
+    Ke = K()({
         name: "VBadge",
         inheritAttrs: !1,
         props: Ee(),
         setup(e, t) {
             const {
                 backgroundColorClasses: i,
                 backgroundColorStyles: a
-            } = ce(H(e, "color")), {
+            } = ue(H(e, "color")), {
                 roundedClasses: A
-            } = ue(e), {
-                t: o
-            } = K(), {
-                textColorClasses: s,
+            } = ge(e), {
+                t: s
+            } = Q(), {
+                textColorClasses: o,
                 textColorStyles: l
-            } = ge(H(e, "textColor")), {
-                themeClasses: p
-            } = X(), {
-                locationStyles: d
-            } = me(e, !0, n => (e.floating ? e.dot ? 2 : 4 : e.dot ? 8 : 12) + (["top", "bottom"].includes(n) ? +(e.offsetY ?? 0) : ["left", "right"].includes(n) ? +(e.offsetX ?? 0) : 0));
+            } = me(H(e, "textColor")), {
+                themeClasses: F
+            } = L(), {
+                locationStyles: f
+            } = fe(e, !0, n => (e.floating ? e.dot ? 2 : 4 : e.dot ? 8 : 12) + (["top", "bottom"].includes(n) ? +(e.offsetY ?? 0) : ["left", "right"].includes(n) ? +(e.offsetX ?? 0) : 0));
             return de(() => {
                 const n = Number(e.content),
                     u = !e.max || isNaN(n) ? e.content : n <= +e.max ? n : `${e.max}+`,
-                    [v, I] = Q(t.attrs, ["aria-atomic", "aria-label", "aria-live", "role", "title"]);
-                return r(e.tag, C({
+                    [p, C] = W(t.attrs, ["aria-atomic", "aria-label", "aria-live", "role", "title"]);
+                return r(e.tag, w({
                     class: ["v-badge", {
                         "v-badge--bordered": e.bordered,
                         "v-badge--dot": e.dot,
                         "v-badge--floating": e.floating,
                         "v-badge--inline": e.inline
                     }, e.class]
-                }, I, {
+                }, C, {
                     style: e.style
                 }), {
                     default: () => {
-                        var f, D;
+                        var d, y;
                         return [r("div", {
                             class: "v-badge__wrapper"
-                        }, [(D = (f = t.slots).default) == null ? void 0 : D.call(f), r(fe, {
+                        }, [(y = (d = t.slots).default) == null ? void 0 : y.call(d), r(he, {
                             transition: e.transition
                         }, {
                             default: () => {
-                                var y, J;
-                                return [W(r("span", C({
-                                    class: ["v-badge__badge", p.value, i.value, A.value, s.value],
-                                    style: [a.value, l.value, e.inline ? {} : d.value],
+                                var I, J;
+                                return [j(r("span", w({
+                                    class: ["v-badge__badge", F.value, i.value, A.value, o.value],
+                                    style: [a.value, l.value, e.inline ? {} : f.value],
                                     "aria-atomic": "true",
-                                    "aria-label": o(e.label, n),
+                                    "aria-label": s(e.label, n),
                                     "aria-live": "polite",
                                     role: "status"
-                                }, v), [e.dot ? void 0 : t.slots.badge ? (J = (y = t.slots).badge) == null ? void 0 : J.call(y) : e.icon ? r(he, {
+                                }, p), [e.dot ? void 0 : t.slots.badge ? (J = (I = t.slots).badge) == null ? void 0 : J.call(I) : e.icon ? r(be, {
                                     icon: e.icon
                                 }, null) : u]), [
-                                    [j, e.modelValue]
+                                    [q, e.modelValue]
                                 ])]
                             }
                         })])]
                     }
                 })
             }), {}
         }
     });
 export {
-    Ge as M, Ke as V, Ve as _, Je as a, Ze as b, Se as g, ye as i
+    Ge as M, Ke as V, Ve as _, Me as a, Ze as b, Se as g, Je as i
 };
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VBadge-bc81f416.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VBadge-8b8b8a6d.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-.list-item{padding:0 8px!important}.list-item>div.ListItem__prepend{padding-right:10px}.mediadetails-streamdetails{width:30px;height:14px;border-radius:2px;font-size:x-small;font-weight:800;min-width:55px;padding:0;box-shadow:none}.mediadetails-content-type-btn{height:25px!important;width:50px!important;padding:5px!important;font-weight:500;font-size:10px!important;letter-spacing:.1em;border-radius:2px;flex-flow:column;margin:0}.v-avatar.v-avatar--density-default[data-v-7b262f2c]{height:100%!important;width:100%!important}img[data-v-7b262f2c]{min-width:100%;max-width:100%;height:auto;display:block;background-size:cover}img.rounded[data-v-7b262f2c]{border-radius:4px}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.material-icons-outlined{font-family:Material Icons Outlined;font-weight:400;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:"liga";-webkit-font-smoothing:antialiased}html{overflow:hidden}*{-webkit-user-drag:none;-khtml-user-drag:none;-moz-user-drag:none;-o-user-drag:none;user-drag:none;-webkit-touch-callout:none;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}a{cursor:pointer}.v-btn--size-default{padding:0 8px}.vertical-btn{display:flex;flex-direction:column;align-items:center}.right{float:right}.left{float:left}.listitem-media-thumb{height:50px;width:50px;margin-right:10px}.v-slider.v-input--horizontal .v-input__control{min-height:5px}div.v-navigation-drawer__scrim{opacity:.8;background:grey}.v-card--variant-elevated{box-shadow:none;border-width:1px;border-style:solid;font-size:smaller}.line-clamp-2{white-space:pre-line;overflow:hidden;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.v-card-text{padding-right:0}.v-expansion-panel--active>.v-expansion-panel-title{min-height:48px}.v-toolbar>.v-toolbar__content>.v-toolbar-title{margin-inline-start:25px}.v-toolbar>.v-toolbar__content>.v-toolbar__prepend{margin-inline-start:6px}.v-toolbar>.v-toolbar__content>.v-toolbar__append{margin-inline-end:21px}.v-toolbar-default>.v-toolbar__content>.v-toolbar-title{margin-inline-start:16px}.v-toolbar-default>.v-toolbar__content>.v-toolbar__prepend{margin-inline-start:10px}.v-toolbar-default>.v-toolbar__content>.v-toolbar__append{margin-inline-end:10px}.v-toolbar{height:55px}.v-toolbar-title{font-family:JetBrains Mono Medium}.col-2{width:50%;max-width:50%;flex-basis:50%}.col-3{width:33.3%;max-width:33.3%;flex-basis:33.3%}.col-4{width:25%;max-width:25%;flex-basis:25%}.col-5{width:20%;max-width:20%;flex-basis:20%}.col-6{width:16.6%;max-width:16.6%;flex-basis:16.6%}.col-7{width:14.2%;max-width:14.2%;flex-basis:14.2%}.col-8{width:12.5%;max-width:12.5%;flex-basis:12.5%}.col-9{width:11.1%;max-width:11.1%;flex-basis:11.1%}.line-clamp-1{white-space:nowrap;text-overflow:ellipsis;overflow:hidden}.line-clamp-2{white-space:pre-line;overflow:hidden;line-height:1.5em;height:3em;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.small-icon{font-size:22px;height:22px;width:22px}.small-btn,.large-icon{font-size:40px;height:40px;width:40px}.large-btn{font-size:50px;height:50px;width:50px}.v-expansion-panel-title{border-radius:0}.v-input--horizontal .v-input__prepend{margin-inline-end:8px}.v-toolbar__content{height:100%!important}.padded-overlay .v-overlay__content{padding:50px}.v-overlay__scrim{opacity:65%}.v-expansion-panel-title{padding:10px}.flicking-camera{display:flex!important}.v-list-item-subtitle{font-size:.75rem;line-height:1rem;font-weight:400;margin-top:0;margin-bottom:0}.v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}.v-toolbar-title{font-size:1.25rem;line-height:1.75rem;font-weight:500}.v-list-item--nav .v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}h1{font-size:1.5rem;line-height:2rem;font-weight:500}h2{font-size:1.25rem;line-height:1.75rem;font-weight:500}h3{font-size:1.125rem;line-height:1.5rem;font-weight:500}h4{font-size:1rem;line-height:1.25rem;font-weight:700}h5{font-size:.875rem;line-height:1.25rem;font-weight:500}h6{font-size:.75rem;line-height:1rem;font-weight:400}.mh1{margin-top:1.5rem;margin-bottom:1rem}.mh2{margin-top:1.5rem;margin-bottom:.75rem}.mh3{margin-top:1.5rem;margin-bottom:.5rem}.mh4{margin-top:1.25rem;margin-bottom:.5rem}.mh5{margin-top:1rem;margin-bottom:.25rem}.mh6{margin-top:1rem;margin-bottom:0}.v-badge{display:inline-block;line-height:1}.v-badge__badge{align-items:center;display:inline-flex;border-radius:10px;font-size:.75rem;font-weight:500;height:1.25rem;justify-content:center;min-width:20px;padding:4px 6px;pointer-events:auto;position:absolute;text-align:center;text-indent:0;transition:.225s cubic-bezier(.4,0,.2,1);white-space:nowrap;background:rgb(var(--v-theme-surface-variant));color:rgba(var(--v-theme-on-surface-variant),var(--v-high-emphasis-opacity))}.v-badge--bordered .v-badge__badge:after{border-radius:inherit;border-style:solid;border-width:2px;bottom:0;color:rgb(var(--v-theme-background));content:"";left:0;position:absolute;right:0;top:0;transform:scale(1.05)}.v-badge--dot .v-badge__badge{border-radius:4.5px;height:9px;min-width:0;padding:0;width:9px}.v-badge--dot .v-badge__badge:after{border-width:1.5px}.v-badge--inline .v-badge__badge{position:relative;vertical-align:middle}.v-badge__badge .v-icon{color:inherit;font-size:.75rem;margin:0 -2px}.v-badge__badge img,.v-badge__badge .v-img{height:100%;width:100%}.v-badge__wrapper{display:flex;position:relative}.v-badge--inline .v-badge__wrapper{align-items:center;display:inline-flex;justify-content:center;margin:0 4px}
+.list-item{padding:0 8px!important}.list-item>div.ListItem__prepend{padding-right:10px}.mediadetails-streamdetails{width:30px;height:14px;border-radius:2px;font-size:x-small;font-weight:800;min-width:55px;padding:0;box-shadow:none}.mediadetails-content-type-btn{height:25px!important;width:50px!important;padding:5px!important;font-weight:500;font-size:10px!important;letter-spacing:.1em;border-radius:2px;flex-flow:column;margin:0}.v-avatar.v-avatar--density-default[data-v-0e68fce2]{height:100%!important;width:100%!important}img[data-v-0e68fce2]{min-width:100%;max-width:100%;height:auto;display:block;background-size:cover}img.rounded[data-v-0e68fce2]{border-radius:4px}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}@font-face{font-family:JetBrains Mono Medium;font-weight:400;font-style:normal;font-display:auto;src:url(./JetBrainsMono-Medium-086c48df.woff2) format("woff2")}.material-icons-outlined{font-family:Material Icons Outlined;font-weight:400;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:"liga";-webkit-font-smoothing:antialiased}html{overflow:hidden}*{-webkit-user-drag:none;-khtml-user-drag:none;-moz-user-drag:none;-o-user-drag:none;user-drag:none;-webkit-touch-callout:none;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}a{cursor:pointer}.v-btn--size-default{padding:0 8px}.vertical-btn{display:flex;flex-direction:column;align-items:center}.right{float:right}.left{float:left}.listitem-media-thumb{height:50px;width:50px;margin-right:10px}.v-slider.v-input--horizontal .v-input__control{min-height:5px}div.v-navigation-drawer__scrim{opacity:.8;background:grey}.v-card--variant-elevated{box-shadow:none;border-width:1px;border-style:solid;font-size:smaller}.line-clamp-2{white-space:pre-line;overflow:hidden;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.v-card-text{padding-right:0}.v-expansion-panel--active>.v-expansion-panel-title{min-height:48px}.v-toolbar>.v-toolbar__content>.v-toolbar-title{margin-inline-start:25px}.v-toolbar>.v-toolbar__content>.v-toolbar__prepend{margin-inline-start:6px}.v-toolbar>.v-toolbar__content>.v-toolbar__append{margin-inline-end:21px}.v-toolbar-default>.v-toolbar__content>.v-toolbar-title{margin-inline-start:16px}.v-toolbar-default>.v-toolbar__content>.v-toolbar__prepend{margin-inline-start:10px}.v-toolbar-default>.v-toolbar__content>.v-toolbar__append{margin-inline-end:10px}.v-toolbar{height:55px}.v-toolbar-title{font-family:JetBrains Mono Medium}.col-2{width:50%;max-width:50%;flex-basis:50%}.col-3{width:33.3%;max-width:33.3%;flex-basis:33.3%}.col-4{width:25%;max-width:25%;flex-basis:25%}.col-5{width:20%;max-width:20%;flex-basis:20%}.col-6{width:16.6%;max-width:16.6%;flex-basis:16.6%}.col-7{width:14.2%;max-width:14.2%;flex-basis:14.2%}.col-8{width:12.5%;max-width:12.5%;flex-basis:12.5%}.col-9{width:11.1%;max-width:11.1%;flex-basis:11.1%}.line-clamp-1{white-space:nowrap;text-overflow:ellipsis;overflow:hidden}.line-clamp-2{white-space:pre-line;overflow:hidden;line-height:1.5em;height:3em;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.small-icon{font-size:22px;height:22px;width:22px}.small-btn,.large-icon{font-size:40px;height:40px;width:40px}.large-btn{font-size:50px;height:50px;width:50px}.v-expansion-panel-title{border-radius:0}.v-input--horizontal .v-input__prepend{margin-inline-end:8px}.v-toolbar__content{height:100%!important}.padded-overlay .v-overlay__content{padding:50px}.v-overlay__scrim{opacity:65%}.v-expansion-panel-title{padding:10px}.flicking-camera{display:flex!important}.v-list-item-subtitle{font-size:.75rem;line-height:1rem;font-weight:400;margin-top:0;margin-bottom:0}.v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}.v-toolbar-title{font-size:1.25rem;line-height:1.75rem;font-weight:500}.v-list-item--nav .v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}h1{font-size:1.5rem;line-height:2rem;font-weight:500}h2{font-size:1.25rem;line-height:1.75rem;font-weight:500}h3{font-size:1.125rem;line-height:1.5rem;font-weight:500}h4{font-size:1rem;line-height:1.25rem;font-weight:700}h5{font-size:.875rem;line-height:1.25rem;font-weight:500}h6{font-size:.75rem;line-height:1rem;font-weight:400}.mh1{margin-top:1.5rem;margin-bottom:1rem}.mh2{margin-top:1.5rem;margin-bottom:.75rem}.mh3{margin-top:1.5rem;margin-bottom:.5rem}.mh4{margin-top:1.25rem;margin-bottom:.5rem}.mh5{margin-top:1rem;margin-bottom:.25rem}.mh6{margin-top:1rem;margin-bottom:0}.v-badge{display:inline-block;line-height:1}.v-badge__badge{align-items:center;display:inline-flex;border-radius:10px;font-size:.75rem;font-weight:500;height:1.25rem;justify-content:center;min-width:20px;padding:4px 6px;pointer-events:auto;position:absolute;text-align:center;text-indent:0;transition:.225s cubic-bezier(.4,0,.2,1);white-space:nowrap;background:rgb(var(--v-theme-surface-variant));color:rgba(var(--v-theme-on-surface-variant),var(--v-high-emphasis-opacity))}.v-badge--bordered .v-badge__badge:after{border-radius:inherit;border-style:solid;border-width:2px;bottom:0;color:rgb(var(--v-theme-background));content:"";left:0;position:absolute;right:0;top:0;transform:scale(1.05)}.v-badge--dot .v-badge__badge{border-radius:4.5px;height:9px;min-width:0;padding:0;width:9px}.v-badge--dot .v-badge__badge:after{border-width:1.5px}.v-badge--inline .v-badge__badge{position:relative;vertical-align:middle}.v-badge__badge .v-icon{color:inherit;font-size:.75rem;margin:0 -2px}.v-badge__badge img,.v-badge__badge .v-img{height:100%;width:100%}.v-badge__wrapper{display:flex;position:relative}.v-badge--inline .v-badge__wrapper{align-items:center;display:inline-flex;justify-content:center;margin:0 4px}
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VCard-257d0eab.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VCard-257d0eab.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VCard-bfc4071a.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VCard-b98fe47e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -24,36 +24,36 @@
     B as ie,
     C as le,
     g as se,
     Y as ce,
     V as re,
     R as ue,
     E as oe
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     g as f,
     k as ve,
     l as n,
     p as S,
     aL as u,
     F as A,
     d as me,
     e as ye,
     c as p,
     af as ke,
     ae as ge
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     h as be,
     d as h
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 import {
     a as fe,
     V as Ce
-} from "./VCardText-00c669eb.js";
+} from "./VCardText-6774ea5e.js";
 const Ie = f()({
         name: "VCardActions",
         props: g(),
         setup(e, i) {
             let {
                 slots: t
             } = i;
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VDialog-5309eac2.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VDialog-5309eac2.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VDialog-82ed2e80.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VDialog-d7e50927.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 import {
     m as b,
     k as y,
     a as D,
     f
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 import {
     i as h,
     j as S,
     F as w
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     p as x,
     g as F,
     h as B,
     r as I,
     aX as R,
     w as v,
     q as T,
     c as k,
     n as m,
     l as g,
     aY as L
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 const O = x({
         fullscreen: Boolean,
         retainFocus: {
             type: Boolean,
             default: !0
         },
         scrollable: Boolean,
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VExpansionPanel-00a7e4f4.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VExpansionPanel-00a7e4f4.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VExpansionPanel-9f82eed8.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VExpansionPanel-58c5fe02.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
     h as Be,
     F as Le,
     n as ze,
     d as Me,
     e as Re,
     k as be,
     aL as ue
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     c as pe,
     b as ye,
     a as G,
     S as he,
     f as ke,
     J as Ne,
@@ -39,26 +39,26 @@
     p as $e,
     d as Se,
     r as De,
     O as Oe,
     n as je,
     G as qe,
     H as Ke
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     g as Ge,
     m as Ue,
     u as We,
     b as ce,
     f as Xe
-} from "./VInput-91b2e758.js";
+} from "./VInput-5b197ccd.js";
 import {
     i as ge,
     j as Ye
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 const se = Symbol.for("vuetify:v-slider");
 
 function He(e, a, l) {
     const t = l === "vertical",
         i = a.getBoundingClientRect(),
         m = "touches" in e ? e.touches[0] : e;
     return t ? m.clientY - (i.top + i.height / 2) : m.clientX - (i.left + i.width / 2)
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VForm-a7262390.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VForm-fc99b4aa.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 import {
     a as p,
     i as v,
     F as b
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     h as F,
     i as V
-} from "./VInput-91b2e758.js";
+} from "./VInput-5b197ccd.js";
 import {
     p as h,
     g as y,
     r as R,
     l as P
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 const k = h({
         ...p(),
         ...F()
     }, "VForm"),
     S = y()({
         name: "VForm",
         props: k(),
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VGrid-37b0738d.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VGrid-37b0738d.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VInput-91b2e758.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VInput-5b197ccd.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -32,15 +32,15 @@
     w as j,
     x as Ae,
     j as Me,
     b as $e,
     o as _e,
     i as ae,
     u as De
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     a as E,
     p as Fe,
     d as me,
     A as ye,
     r as we,
     i as z,
@@ -65,22 +65,22 @@
     n as L,
     j as q,
     J as be,
     e as Je,
     I as Ze,
     Z as Qe,
     M as We
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     m as ea,
     V as le
-} from "./VSlideGroup-5dd0c6f2.js";
+} from "./VSlideGroup-b576aa37.js";
 import {
     d as te
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 const Ve = Symbol.for("vuetify:v-chip-group"),
     aa = x({
         column: Boolean,
         filter: Boolean,
         valueComparator: {
             type: Function,
             default: se
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VInput-b16e222c.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VInput-b16e222c.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VMenu-9506155f.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VMenu-b634019c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -53,15 +53,15 @@
     f as mn,
     ar as xt,
     u as yn,
     bk as gn,
     bl as hn,
     aY as at,
     bm as bn
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     a as ae,
     L as ue,
     a4 as Sn,
     N as Ie,
     a5 as wn,
     a6 as Ot,
@@ -101,15 +101,15 @@
     ab as Ee,
     ac as it,
     ad as rt,
     I as Ln,
     h as In,
     ae as Bn,
     F as Tn
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 const ye = new WeakMap;
 
 function Mn(e, n) {
     Object.keys(n).forEach(t => {
         if (St(t)) {
             const a = wt(t),
                 o = ye.get(e);
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VMenu-a46f5e7a.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VMenu-a46f5e7a.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VSelect-7df244e0.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSelect-7df244e0.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VSelect-ea96d901.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSelect-d10e917f.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 import {
     m as re,
     V as N
-} from "./VTextField-8883f272.js";
+} from "./VTextField-0c2ec62d.js";
 import {
     s as Q,
     w as E,
     p as X,
     aL as ce,
     aC as de,
     g as fe,
@@ -18,39 +18,39 @@
     F as O,
     n as x,
     aZ as pe,
     Q as he,
     a_ as ye,
     q as ge,
     a$ as j
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     j as Ve,
     c as ke,
     V as we
-} from "./VInput-91b2e758.js";
+} from "./VInput-5b197ccd.js";
 import {
     I as be,
     i as Ce,
     n as z,
     j as Pe,
     F as xe
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     l as Se,
     k as De,
     n as Te,
     e as Ie,
     b as Ae,
     V as W,
     d as Fe
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 import {
     V as Le
-} from "./VVirtualScroll-5f35af5d.js";
+} from "./VVirtualScroll-84259ceb.js";
 
 function Re(e, B) {
     const n = Q(!1);
     let y;
 
     function m(i) {
         cancelAnimationFrame(y), n.value = !0, y = requestAnimationFrame(() => {
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VSlideGroup-5dd0c6f2.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSlideGroup-b576aa37.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,30 +3,30 @@
     d as ee,
     p as te,
     r as le,
     w as H,
     i as ae,
     a3 as G,
     n as L
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     p as ne,
     aL as $,
     m as se,
     g as ue,
     u as oe,
     f as ie,
     s as x,
     c as S,
     aX as ce,
     w as re,
     l as h,
     aY as ve,
     aV as fe
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 
 function X(a) {
     const s = Math.abs(a);
     return Math.sign(a) * (s / ((1 / .501 - 2) * (1 - s) + 1))
 }
 
 function Y(a) {
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VSlideGroup-c5ba1538.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSlideGroup-c5ba1538.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTabs-11e16be1.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTabs-11e16be1.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTabs-4c128c89.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTabs-8ad24bfd.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -6,34 +6,34 @@
     F as X,
     L as Y,
     N as j,
     o as J,
     d as K,
     q as L,
     e as W
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     p as R,
     aC as p,
     g as F,
     r as E,
     c as V,
     l as f,
     F as Q,
     n as T,
     h as Z,
     t as n,
     k as ee,
     a as te,
     aP as ae
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     m as se,
     V as M
-} from "./VSlideGroup-5dd0c6f2.js";
+} from "./VSlideGroup-b576aa37.js";
 const G = Symbol.for("vuetify:v-tabs"),
     oe = R({
         fixed: Boolean,
         sliderColor: String,
         hideSlider: Boolean,
         direction: {
             type: String,
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTextField-8883f272.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTextField-0c2ec62d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
     b2 as be,
     h as xe,
     aK as Ce,
     ae as ke,
     b3 as Ve,
     q as p,
     b4 as he
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     a as H,
     I as _e,
     Z as Ie,
     i as K,
     M as Pe,
     W as Fe,
@@ -42,23 +42,23 @@
     L as $e,
     R as Ae,
     $ as De,
     j as Ee,
     N as Me,
     a0 as Ne,
     F as Oe
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     f as Ue,
     g as Ke,
     u as te,
     k as je,
     m as We,
     b as ee
-} from "./VInput-91b2e758.js";
+} from "./VInput-5b197ccd.js";
 const qe = O({
         active: Boolean,
         max: [Number, String],
         value: {
             type: [Number, String],
             default: 0
         },
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTextField-d31117f3.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTextField-d31117f3.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VToolbar-4ad3b045.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VToolbar-b7f10b15.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,28 +8,28 @@
     e as D,
     u as w,
     f as $,
     g as j,
     V as F,
     j as u,
     O
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     p as V,
     g as k,
     l as a,
     d as U,
     t as q,
     e as z,
     u as A,
     s as G,
     c as h,
     k as J,
     a as o
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 const K = V({
         text: String,
         ...x(),
         ...y()
     }, "VToolbarTitle"),
     L = k()({
         name: "VToolbarTitle",
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VToolbar-78a5e824.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VToolbar-78a5e824.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTooltip-3a8fb95f.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTooltip-3a8fb95f.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VTooltip-a8719c72.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTooltip-3ef94159.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     m as w,
     a as H,
     u as R,
     b as h,
     c as C
-} from "./VInput-91b2e758.js";
+} from "./VInput-5b197ccd.js";
 import {
     p as y,
     aC as G,
     g,
     h as S,
     at as B,
     c as v,
@@ -20,33 +20,33 @@
     z as K,
     x as L,
     H as I,
     L as N,
     d as W,
     e as j,
     r as q
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     i as T,
     a as E,
     p as J,
     d as Q,
     r as X,
     G as Y,
     H as Z,
     F as _
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     B as ee
-} from "./Container-ba274a7a.js";
+} from "./Container-dc894acd.js";
 import {
     m as te,
     a as oe,
     f as x
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 const ae = y({
         ...w(),
         ...G(H(), ["inline"])
     }, "VCheckbox"),
     de = g()({
         name: "VCheckbox",
         inheritAttrs: !1,
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VVirtualScroll-29c92c23.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VVirtualScroll-29c92c23.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/VVirtualScroll-5f35af5d.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VVirtualScroll-84259ceb.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as L,
     w as W,
     i as X,
     T as re,
     U as oe
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     p as D,
     g as $,
     w as O,
     l as S,
     F as j,
     n as se,
@@ -23,18 +23,18 @@
     q as ie,
     aX as ve,
     au as fe,
     t as de,
     i as me,
     a as F,
     o as he
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 import {
     o as ge
-} from "./VMenu-9506155f.js";
+} from "./VMenu-b634019c.js";
 const pe = D({
         renderless: Boolean,
         ...L()
     }, "VVirtualScrollItem"),
     Se = $()({
         name: "VVirtualScrollItem",
         inheritAttrs: !1,
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/contextmenu-c4231154.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/contextmenu-521b5304.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 import {
     aJ as p,
     M as n,
     L as e,
     V as u,
     $ as c,
     P as t
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 
 function f(i) {
     return {
         all: i = i || new Map,
         on: function(l, r) {
             var a = i.get(l);
             a ? a.push(r) : i.set(l, [r])
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/cover_dark-75402cd0.png` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/cover_dark-75402cd0.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/cover_light-b832ae9e.png` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/cover_light-b832ae9e.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/fallback-d0ff2800.png` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/fallback-d0ff2800.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/folder-6b5595ac.svg` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/folder-6b5595ac.svg`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/forwardRefs-70e877d2.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/forwardRefs-7be90dc2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -54,15 +54,15 @@
     af as he,
     ae as qe,
     bz as Ue,
     aB as pe,
     ba as Dt,
     j as Ft,
     aO as Ht
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 const Xe = ["top", "bottom"],
     Mt = ["start", "end", "left", "right"];
 
 function jt(e, n) {
     let [a, t] = e.split(" ");
     return t || (t = se(Xe, a) ? "start" : se(Mt, a) ? "top" : "center"), {
         side: $e(a, n),
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/forwardRefs-e5b3781d.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/forwardRefs-e5b3781d.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/hires-438c7046.png` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/hires-438c7046.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/index-52c10419.css` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/index-52c10419.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/index-6ff57e4c.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/index-b687f95a.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
-var Ed = Object.defineProperty;
-var kd = (e, n, t) => n in e ? Ed(e, n, {
+var kd = Object.defineProperty;
+var Ed = (e, n, t) => n in e ? kd(e, n, {
     enumerable: !0,
     configurable: !0,
     writable: !0,
     value: t
 }) : e[n] = t;
-var Ye = (e, n, t) => (kd(e, typeof n != "symbol" ? n + "" : n, t), t);
+var Ye = (e, n, t) => (Ed(e, typeof n != "symbol" ? n + "" : n, t), t);
 (function() {
     const n = document.createElement("link").relList;
     if (n && n.supports && n.supports("modulepreload")) return;
     for (const o of document.querySelectorAll('link[rel="modulepreload"]')) r(o);
     new MutationObserver(o => {
         for (const a of o)
             if (a.type === "childList")
@@ -42,15 +42,15 @@
 }
 const Te = {},
     qt = [],
     dn = () => {},
     Ad = () => !1,
     Bo = e => e.charCodeAt(0) === 111 && e.charCodeAt(1) === 110 && (e.charCodeAt(2) > 122 || e.charCodeAt(2) < 97),
     Pa = e => e.startsWith("onUpdate:"),
-    De = Object.assign,
+    Ie = Object.assign,
     Ma = (e, n) => {
         const t = e.indexOf(n);
         t > -1 && e.splice(t, 1)
     },
     Pd = Object.prototype.hasOwnProperty,
     fe = (e, n) => Pd.call(e, n),
     ee = Array.isArray,
@@ -61,54 +61,54 @@
     lr = e => typeof e == "symbol",
     ye = e => e !== null && typeof e == "object",
     Ca = e => (ye(e) || re(e)) && re(e.then) && re(e.catch),
     Nu = Object.prototype.toString,
     Ho = e => Nu.call(e),
     Md = e => Ho(e).slice(8, -1),
     Gu = e => Ho(e) === "[object Object]",
-    Ia = e => Me(e) && e !== "NaN" && e[0] !== "-" && "" + parseInt(e, 10) === e,
+    Da = e => Me(e) && e !== "NaN" && e[0] !== "-" && "" + parseInt(e, 10) === e,
     gr = Aa(",key,ref,ref_for,ref_key,onVnodeBeforeMount,onVnodeMounted,onVnodeBeforeUpdate,onVnodeUpdated,onVnodeBeforeUnmount,onVnodeUnmounted"),
     Fo = e => {
         const n = Object.create(null);
         return t => n[t] || (n[t] = e(t))
     },
     Cd = /-(\w)/g,
     Rn = Fo(e => e.replace(Cd, (n, t) => t ? t.toUpperCase() : "")),
-    Id = /\B([A-Z])/g,
-    sr = Fo(e => e.replace(Id, "-$1").toLowerCase()),
+    Dd = /\B([A-Z])/g,
+    sr = Fo(e => e.replace(Dd, "-$1").toLowerCase()),
     Hr = Fo(e => e.charAt(0).toUpperCase() + e.slice(1)),
     ui = Fo(e => e ? `on${Hr(e)}` : ""),
     mt = (e, n) => !Object.is(e, n),
     ci = (e, n) => {
         for (let t = 0; t < e.length; t++) e[t](n)
     },
     go = (e, n, t) => {
         Object.defineProperty(e, n, {
             configurable: !0,
             enumerable: !1,
             value: t
         })
     },
-    Dd = e => {
+    Id = e => {
         const n = parseFloat(e);
         return isNaN(n) ? e : n
     },
     Bu = e => {
         const n = Me(e) ? Number(e) : NaN;
         return isNaN(n) ? e : n
     };
 let hl;
 const Hu = () => hl || (hl = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {});
 
-function Da(e) {
+function Ia(e) {
     if (ee(e)) {
         const n = {};
         for (let t = 0; t < e.length; t++) {
             const r = e[t],
-                o = Me(r) ? Rd(r) : Da(r);
+                o = Me(r) ? Rd(r) : Ia(r);
             if (o)
                 for (const a in o) n[a] = o[a]
         }
         return n
     } else if (Me(e) || ye(e)) return e
 }
 const Ld = /;(?![^(]*\))/g,
@@ -220,15 +220,15 @@
     get dirty() {
         if (this._dirtyLevel === 2 || this._dirtyLevel === 3) {
             this._dirtyLevel = 1, Ct();
             for (let n = 0; n < this._depsLength; n++) {
                 const t = this.deps[n];
                 if (t.computed && (Vd(t.computed), this._dirtyLevel >= 4)) break
             }
-            this._dirtyLevel === 1 && (this._dirtyLevel = 0), It()
+            this._dirtyLevel === 1 && (this._dirtyLevel = 0), Dt()
         }
         return this._dirtyLevel >= 4
     }
     set dirty(n) {
         this._dirtyLevel = n ? 4 : 0
     }
     run() {
@@ -270,15 +270,15 @@
     Hi = 0;
 const Wu = [];
 
 function Ct() {
     Wu.push(lt), lt = !1
 }
 
-function It() {
+function Dt() {
     const e = Wu.pop();
     lt = e === void 0 ? !0 : e
 }
 
 function xa() {
     Hi++
 }
@@ -305,15 +305,15 @@
     Ra()
 }
 const Xu = (e, n) => {
         const t = new Map;
         return t.cleanup = e, t.computed = n, t
     },
     bo = new WeakMap,
-    Et = Symbol(""),
+    kt = Symbol(""),
     Vi = Symbol("");
 
 function an(e, n, t) {
     if (lt && wt) {
         let r = bo.get(e);
         r || bo.set(e, r = new Map);
         let o = r.get(t);
@@ -329,21 +329,21 @@
     else if (t === "length" && ee(e)) {
         const s = Number(r);
         l.forEach((c, d) => {
             (d === "length" || !lr(d) && d >= s) && u.push(c)
         })
     } else switch (t !== void 0 && u.push(l.get(t)), n) {
         case "add":
-            ee(e) ? Ia(t) && u.push(l.get("length")) : (u.push(l.get(Et)), Wt(e) && u.push(l.get(Vi)));
+            ee(e) ? Da(t) && u.push(l.get("length")) : (u.push(l.get(kt)), Wt(e) && u.push(l.get(Vi)));
             break;
         case "delete":
-            ee(e) || (u.push(l.get(Et)), Wt(e) && u.push(l.get(Vi)));
+            ee(e) || (u.push(l.get(kt)), Wt(e) && u.push(l.get(Vi)));
             break;
         case "set":
-            Wt(e) && u.push(l.get(Et));
+            Wt(e) && u.push(l.get(kt));
             break
     }
     xa();
     for (const s of u) s && Ku(s, 4);
     Ra()
 }
 
@@ -364,15 +364,15 @@
             const o = r[n](...t);
             return o === -1 || o === !1 ? r[n](...t.map(ce)) : o
         }
     }), ["push", "pop", "shift", "unshift", "splice"].forEach(n => {
         e[n] = function(...t) {
             Ct(), xa();
             const r = ce(this)[n].apply(this, t);
-            return Ra(), It(), r
+            return Ra(), Dt(), r
         }
     }), e
 }
 
 function Wd(e) {
     const n = ce(this);
     return an(n, "has", e), n.hasOwnProperty(e)
@@ -390,43 +390,43 @@
         if (t === "__v_raw") return r === (o ? a ? af : nc : a ? ec : Ju).get(n) || Object.getPrototypeOf(n) === Object.getPrototypeOf(r) ? n : void 0;
         const l = ee(n);
         if (!o) {
             if (l && fe(vl, t)) return Reflect.get(vl, t, r);
             if (t === "hasOwnProperty") return Wd
         }
         const u = Reflect.get(n, t, r);
-        return (lr(t) ? Yu.has(t) : Ud(t)) || (o || an(n, "get", t), a) ? u : je(u) ? l && Ia(t) ? u : u.value : ye(u) ? o ? rc(u) : on(u) : u
+        return (lr(t) ? Yu.has(t) : Ud(t)) || (o || an(n, "get", t), a) ? u : je(u) ? l && Da(t) ? u : u.value : ye(u) ? o ? rc(u) : on(u) : u
     }
 }
 class Zu extends Qu {
     constructor(n = !1) {
         super(!1, n)
     }
     set(n, t, r, o) {
         let a = n[t];
         if (!this._isShallow) {
             const s = Zt(a);
             if (!vo(r) && !Zt(r) && (a = ce(a), r = ce(r)), !ee(n) && je(a) && !je(r)) return s ? !1 : (a.value = r, !0)
         }
-        const l = ee(n) && Ia(t) ? Number(t) < n.length : fe(n, t),
+        const l = ee(n) && Da(t) ? Number(t) < n.length : fe(n, t),
             u = Reflect.set(n, t, r, o);
         return n === ce(o) && (l ? mt(r, a) && qn(n, "set", t, r) : qn(n, "add", t, r)), u
     }
     deleteProperty(n, t) {
         const r = fe(n, t);
         n[t];
         const o = Reflect.deleteProperty(n, t);
         return o && r && qn(n, "delete", t, void 0), o
     }
     has(n, t) {
         const r = Reflect.has(n, t);
         return (!lr(t) || !Yu.has(t)) && an(n, "has", t), r
     }
     ownKeys(n) {
-        return an(n, "iterate", ee(n) ? "length" : Et), Reflect.ownKeys(n)
+        return an(n, "iterate", ee(n) ? "length" : kt), Reflect.ownKeys(n)
     }
 }
 class $d extends Qu {
     constructor(n = !1) {
         super(!0, n)
     }
     set(n, t) {
@@ -459,15 +459,15 @@
     const t = this.__v_raw,
         r = ce(t),
         o = ce(e);
     return n || (mt(e, o) && an(r, "has", e), an(r, "has", o)), e === o ? t.has(e) : t.has(e) || t.has(o)
 }
 
 function Xr(e, n = !1) {
-    return e = e.__v_raw, !n && an(ce(e), "iterate", Et), Reflect.get(e, "size", e)
+    return e = e.__v_raw, !n && an(ce(e), "iterate", kt), Reflect.get(e, "size", e)
 }
 
 function yl(e) {
     e = ce(e);
     const n = ce(this);
     return Vo(n).has.call(n, e) || (n.add(e), qn(n, "add", e, e)), this
 }
@@ -506,28 +506,28 @@
 
 function Yr(e, n) {
     return function(r, o) {
         const a = this,
             l = a.__v_raw,
             u = ce(l),
             s = n ? Na : e ? Ha : Ar;
-        return !e && an(u, "iterate", Et), l.forEach((c, d) => r.call(o, s(c), s(d), a))
+        return !e && an(u, "iterate", kt), l.forEach((c, d) => r.call(o, s(c), s(d), a))
     }
 }
 
 function Qr(e, n, t) {
     return function(...r) {
         const o = this.__v_raw,
             a = ce(o),
             l = Wt(a),
             u = e === "entries" || e === Symbol.iterator && l,
             s = e === "keys" && l,
             c = o[e](...r),
             d = t ? Na : n ? Ha : Ar;
-        return !n && an(a, "iterate", s ? Vi : Et), {
+        return !n && an(a, "iterate", s ? Vi : kt), {
             next() {
                 const {
                     value: m,
                     done: f
                 } = c.next();
                 return f ? {
                     value: m,
@@ -868,56 +868,56 @@
 
 function _f(e, n, t, r = !0) {
     console.error(e)
 }
 let Pr = !1,
     ji = !1;
 const $e = [];
-let Dn = 0;
+let In = 0;
 const Kt = [];
 let et = null,
     Tt = 0;
 const mc = Promise.resolve();
 let Va = null;
 
 function Vr(e) {
     const n = Va || mc;
     return e ? n.then(this ? e.bind(this) : e) : n
 }
 
 function pf(e) {
-    let n = Dn + 1,
+    let n = In + 1,
         t = $e.length;
     for (; n < t;) {
         const r = n + t >>> 1,
             o = $e[r],
             a = Mr(o);
         a < e || a === e && o.pre ? n = r + 1 : t = r
     }
     return n
 }
 
 function ja(e) {
-    (!$e.length || !$e.includes(e, Pr && e.allowRecurse ? Dn + 1 : Dn)) && (e.id == null ? $e.push(e) : $e.splice(pf(e.id), 0, e), dc())
+    (!$e.length || !$e.includes(e, Pr && e.allowRecurse ? In + 1 : In)) && (e.id == null ? $e.push(e) : $e.splice(pf(e.id), 0, e), dc())
 }
 
 function dc() {
     !Pr && !ji && (ji = !0, Va = mc.then(_c))
 }
 
 function zf(e) {
     const n = $e.indexOf(e);
-    n > Dn && $e.splice(n, 1)
+    n > In && $e.splice(n, 1)
 }
 
 function Ui(e) {
     ee(e) ? Kt.push(...e) : (!et || !et.includes(e, e.allowRecurse ? Tt + 1 : Tt)) && Kt.push(e), dc()
 }
 
-function El(e, n, t = Pr ? Dn + 1 : 0) {
+function kl(e, n, t = Pr ? In + 1 : 0) {
     for (; t < $e.length; t++) {
         const r = $e[t];
         if (r && r.pre) {
             if (e && r.id !== e.uid) continue;
             $e.splice(t, 1), t--, r()
         }
     }
@@ -944,20 +944,20 @@
         return t
     };
 
 function _c(e) {
     ji = !1, Pr = !0, $e.sort(hf);
     const n = dn;
     try {
-        for (Dn = 0; Dn < $e.length; Dn++) {
-            const t = $e[Dn];
+        for (In = 0; In < $e.length; In++) {
+            const t = $e[In];
             t && t.active !== !1 && ut(t, null, 14)
         }
     } finally {
-        Dn = 0, $e.length = 0, fc(), Pr = !1, Va = null, ($e.length || Kt.length) && _c()
+        In = 0, $e.length = 0, fc(), Pr = !1, Va = null, ($e.length || Kt.length) && _c()
     }
 }
 
 function gf(e, n, ...t) {
     if (e.isUnmounted) return;
     const r = e.vnode.props || Te;
     let o = t;
@@ -965,15 +965,15 @@
         l = a && n.slice(7);
     if (l && l in r) {
         const d = `${l==="modelValue"?"model":l}Modifiers`,
             {
                 number: m,
                 trim: f
             } = r[d] || Te;
-        f && (o = t.map(_ => Me(_) ? _.trim() : _)), m && (o = t.map(Dd))
+        f && (o = t.map(_ => Me(_) ? _.trim() : _)), m && (o = t.map(Id))
     }
     let u, s = r[u = ui(n)] || r[u = ui(Rn(n))];
     !s && a && (s = r[u = ui(sr(n))]), s && yn(s, e, 6, o);
     const c = r[u + "Once"];
     if (c) {
         if (!e.emitted) e.emitted = {};
         else if (e.emitted[u]) return;
@@ -987,37 +987,37 @@
     if (o !== void 0) return o;
     const a = e.emits;
     let l = {},
         u = !1;
     if (!re(e)) {
         const s = c => {
             const d = pc(c, n, !0);
-            d && (u = !0, De(l, d))
+            d && (u = !0, Ie(l, d))
         };
         !t && n.mixins.length && n.mixins.forEach(s), e.extends && s(e.extends), e.mixins && e.mixins.forEach(s)
     }
-    return !a && !u ? (ye(e) && r.set(e, null), null) : (ee(a) ? a.forEach(s => l[s] = null) : De(l, a), ye(e) && r.set(e, l), l)
+    return !a && !u ? (ye(e) && r.set(e, null), null) : (ee(a) ? a.forEach(s => l[s] = null) : Ie(l, a), ye(e) && r.set(e, l), l)
 }
 
 function jo(e, n) {
     return !e || !Bo(n) ? !1 : (n = n.slice(2).replace(/Once$/, ""), fe(e, n[0].toLowerCase() + n.slice(1)) || fe(e, sr(n)) || fe(e, n))
 }
 let Oe = null,
     Uo = null;
 
 function yo(e) {
     const n = Oe;
     return Oe = e, Uo = e && e.type.__scopeId || null, n
 }
 
-function E1(e) {
+function k1(e) {
     Uo = e
 }
 
-function k1() {
+function E1() {
     Uo = null
 }
 
 function bf(e, n = Oe, t) {
     if (!n || e._n) return e;
     const r = (...o) => {
         r._d && Hl(-1);
@@ -1052,34 +1052,34 @@
         inheritAttrs: g
     } = e;
     let y, z;
     const b = yo(e);
     try {
         if (t.shapeFlag & 4) {
             const S = o || r,
-                E = S;
-            y = kn(d.call(E, S, m, a, _, f, p)), z = s
+                k = S;
+            y = En(d.call(k, S, m, a, _, f, p)), z = s
         } else {
             const S = n;
-            y = kn(S.length > 1 ? S(a, {
+            y = En(S.length > 1 ? S(a, {
                 attrs: s,
                 slots: u,
                 emit: c
             }) : S(a, null)), z = n.props ? s : yf(s)
         }
     } catch (S) {
         Sr.length = 0, Fr(S, e, 1), y = ve(en)
     }
     let h = y;
     if (z && g !== !1) {
         const S = Object.keys(z),
             {
-                shapeFlag: E
+                shapeFlag: k
             } = h;
-        S.length && E & 7 && (l && S.some(Pa) && (z = Tf(z, l)), h = dt(h, z))
+        S.length && k & 7 && (l && S.some(Pa) && (z = Tf(z, l)), h = dt(h, z))
     }
     return t.dirs && (h = dt(h), h.dirs = h.dirs ? h.dirs.concat(t.dirs) : t.dirs), t.transition && (h.transition = t.transition), y = h, yo(b), y
 }
 
 function vf(e, n = !0) {
     let t;
     for (let r = 0; r < e.length; r++) {
@@ -1113,27 +1113,27 @@
         props: l,
         children: u,
         patchFlag: s
     } = n, c = a.emitsOptions;
     if (n.dirs || n.transition) return !0;
     if (t && s >= 0) {
         if (s & 1024) return !0;
-        if (s & 16) return r ? kl(r, l, c) : !!l;
+        if (s & 16) return r ? El(r, l, c) : !!l;
         if (s & 8) {
             const d = n.dynamicProps;
             for (let m = 0; m < d.length; m++) {
                 const f = d[m];
                 if (l[f] !== r[f] && !jo(c, f)) return !0
             }
         }
-    } else return (o || u) && (!u || !u.$stable) ? !0 : r === l ? !1 : r ? l ? kl(r, l, c) : !0 : !!l;
+    } else return (o || u) && (!u || !u.$stable) ? !0 : r === l ? !1 : r ? l ? El(r, l, c) : !0 : !!l;
     return !1
 }
 
-function kl(e, n, t) {
+function El(e, n, t) {
     const r = Object.keys(n);
     if (r.length !== Object.keys(e).length) return !0;
     for (let o = 0; o < r.length; o++) {
         const a = r[o];
         if (n[a] !== e[a] && !jo(t, a)) return !0
     }
     return !1
@@ -1148,15 +1148,15 @@
         if (r.suspense && r.suspense.activeBranch === e && (r.el = e.el), r === e)(e = n.vnode).el = t, n = n.parent;
         else break
     }
 }
 const qa = "components",
     wf = "directives";
 
-function Ef(e, n) {
+function kf(e, n) {
     return Wa(qa, e, !0, n) || e
 }
 const zc = Symbol.for("v-ndc");
 
 function A1(e) {
     return Me(e) ? Wa(qa, e, !1) || e : e || zc
 }
@@ -1177,15 +1177,15 @@
         return !l && r ? a : l
     }
 }
 
 function Al(e, n) {
     return e && (e[n] || e[Rn(n)] || e[Hr(Rn(n))])
 }
-const kf = e => e.__isSuspense;
+const Ef = e => e.__isSuspense;
 let qi = 0;
 const Af = {
         name: "Suspense",
         __isSuspense: !0,
         process(e, n, t, r, o, a, l, u, s, c) {
             if (e == null) Pf(n, t, r, o, a, l, u, s, c);
             else {
@@ -1194,15 +1194,15 @@
                     return
                 }
                 Mf(e, n, t, r, o, l, u, s, c)
             }
         },
         hydrate: Cf,
         create: $a,
-        normalize: If
+        normalize: Df
     },
     M1 = Af;
 
 function Cr(e, n) {
     const t = e.props && e.props[n];
     re(t) && t()
 }
@@ -1260,15 +1260,15 @@
         }
     } = c;
     let z;
     const b = Lf(e);
     b && n != null && n.pendingBranch && (z = n.pendingId, n.deps++);
     const h = e.props ? Bu(e.props.timeout) : void 0,
         S = a,
-        E = {
+        k = {
             vnode: e,
             parent: n,
             parentComponent: t,
             namespace: l,
             container: r,
             hiddenContainer: o,
             deps: 0,
@@ -1276,109 +1276,109 @@
             timeout: typeof h == "number" ? h : -1,
             activeBranch: null,
             pendingBranch: null,
             isInFallback: !d,
             isHydrating: d,
             isUnmounted: !1,
             effects: [],
-            resolve(k = !1, D = !1) {
+            resolve(E = !1, I = !1) {
                 const {
                     vnode: P,
                     activeBranch: M,
                     pendingBranch: L,
                     pendingId: F,
                     effects: O,
                     parentComponent: V,
                     container: Z
-                } = E;
+                } = k;
                 let oe = !1;
-                E.isHydrating ? E.isHydrating = !1 : k || (oe = M && L.transition && L.transition.mode === "out-in", oe && (M.transition.afterLeave = () => {
-                    F === E.pendingId && (f(L, Z, a === S ? p(M) : a, 0), Ui(O))
-                }), M && (g(M.el) !== E.hiddenContainer && (a = p(M)), _(M, V, E, !0)), oe || f(L, Z, a, 0)), Xt(E, L), E.pendingBranch = null, E.isInFallback = !1;
-                let ie = E.parent,
+                k.isHydrating ? k.isHydrating = !1 : E || (oe = M && L.transition && L.transition.mode === "out-in", oe && (M.transition.afterLeave = () => {
+                    F === k.pendingId && (f(L, Z, a === S ? p(M) : a, 0), Ui(O))
+                }), M && (g(M.el) !== k.hiddenContainer && (a = p(M)), _(M, V, k, !0)), oe || f(L, Z, a, 0)), Xt(k, L), k.pendingBranch = null, k.isInFallback = !1;
+                let ie = k.parent,
                     se = !1;
                 for (; ie;) {
                     if (ie.pendingBranch) {
                         ie.effects.push(...O), se = !0;
                         break
                     }
                     ie = ie.parent
-                }!se && !oe && Ui(O), E.effects = [], b && n && n.pendingBranch && z === n.pendingId && (n.deps--, n.deps === 0 && !D && n.resolve()), Cr(P, "onResolve")
+                }!se && !oe && Ui(O), k.effects = [], b && n && n.pendingBranch && z === n.pendingId && (n.deps--, n.deps === 0 && !I && n.resolve()), Cr(P, "onResolve")
             },
-            fallback(k) {
-                if (!E.pendingBranch) return;
+            fallback(E) {
+                if (!k.pendingBranch) return;
                 const {
-                    vnode: D,
+                    vnode: I,
                     activeBranch: P,
                     parentComponent: M,
                     container: L,
                     namespace: F
-                } = E;
-                Cr(D, "onFallback");
+                } = k;
+                Cr(I, "onFallback");
                 const O = p(P),
                     V = () => {
-                        E.isInFallback && (m(null, k, L, O, M, null, F, u, s), Xt(E, k))
+                        k.isInFallback && (m(null, E, L, O, M, null, F, u, s), Xt(k, E))
                     },
-                    Z = k.transition && k.transition.mode === "out-in";
-                Z && (P.transition.afterLeave = V), E.isInFallback = !0, _(P, M, null, !0), Z || V()
+                    Z = E.transition && E.transition.mode === "out-in";
+                Z && (P.transition.afterLeave = V), k.isInFallback = !0, _(P, M, null, !0), Z || V()
             },
-            move(k, D, P) {
-                E.activeBranch && f(E.activeBranch, k, D, P), E.container = k
+            move(E, I, P) {
+                k.activeBranch && f(k.activeBranch, E, I, P), k.container = E
             },
             next() {
-                return E.activeBranch && p(E.activeBranch)
+                return k.activeBranch && p(k.activeBranch)
             },
-            registerDep(k, D) {
-                const P = !!E.pendingBranch;
-                P && E.deps++;
-                const M = k.vnode.el;
-                k.asyncDep.catch(L => {
-                    Fr(L, k, 0)
+            registerDep(E, I) {
+                const P = !!k.pendingBranch;
+                P && k.deps++;
+                const M = E.vnode.el;
+                E.asyncDep.catch(L => {
+                    Fr(L, E, 0)
                 }).then(L => {
-                    if (k.isUnmounted || E.isUnmounted || E.pendingId !== k.suspenseId) return;
-                    k.asyncResolved = !0;
+                    if (E.isUnmounted || k.isUnmounted || k.pendingId !== E.suspenseId) return;
+                    E.asyncResolved = !0;
                     const {
                         vnode: F
-                    } = k;
-                    ea(k, L, !1), M && (F.el = M);
-                    const O = !M && k.subTree.el;
-                    D(k, F, g(M || k.subTree.el), M ? null : p(k.subTree), E, l, s), O && y(O), Ua(k, F.el), P && --E.deps === 0 && E.resolve()
+                    } = E;
+                    ea(E, L, !1), M && (F.el = M);
+                    const O = !M && E.subTree.el;
+                    I(E, F, g(M || E.subTree.el), M ? null : p(E.subTree), k, l, s), O && y(O), Ua(E, F.el), P && --k.deps === 0 && k.resolve()
                 })
             },
-            unmount(k, D) {
-                E.isUnmounted = !0, E.activeBranch && _(E.activeBranch, t, k, D), E.pendingBranch && _(E.pendingBranch, t, k, D)
+            unmount(E, I) {
+                k.isUnmounted = !0, k.activeBranch && _(k.activeBranch, t, E, I), k.pendingBranch && _(k.pendingBranch, t, E, I)
             }
         };
-    return E
+    return k
 }
 
 function Cf(e, n, t, r, o, a, l, u, s) {
     const c = n.suspense = $a(n, r, t, e.parentNode, document.createElement("div"), null, o, a, l, u, !0),
         d = s(e, c.pendingBranch = n.ssContent, t, c, a, l);
     return c.deps === 0 && c.resolve(!1, !0), d
 }
 
-function If(e) {
+function Df(e) {
     const {
         shapeFlag: n,
         children: t
     } = e, r = n & 32;
     e.ssContent = Pl(r ? t.default : t), e.ssFallback = r ? Pl(t.fallback) : ve(en)
 }
 
 function Pl(e) {
     let n;
     if (re(e)) {
         const t = Jt && e._c;
         t && (e._d = !1, Yo()), e = e(), t && (e._d = !0, n = vn, Lc())
     }
-    return ee(e) && (e = vf(e)), e = kn(e), n && !e.dynamicChildren && (e.dynamicChildren = n.filter(t => t !== e)), e
+    return ee(e) && (e = vf(e)), e = En(e), n && !e.dynamicChildren && (e.dynamicChildren = n.filter(t => t !== e)), e
 }
 
-function Df(e, n) {
+function If(e, n) {
     n && n.pendingBranch ? ee(e) ? n.effects.push(...e) : n.effects.push(e) : Ui(e)
 }
 
 function Xt(e, n) {
     e.activeBranch = n;
     const {
         vnode: t,
@@ -1410,59 +1410,59 @@
     deep: r,
     flush: o,
     once: a,
     onTrack: l,
     onTrigger: u
 } = Te) {
     if (n && a) {
-        const k = n;
-        n = (...D) => {
-            k(...D), E()
+        const E = n;
+        n = (...I) => {
+            E(...I), k()
         }
     }
     const s = Ve,
-        c = k => r === !0 ? k : St(k, r === !1 ? 1 : void 0);
+        c = E => r === !0 ? E : St(E, r === !1 ? 1 : void 0);
     let d, m = !1,
         f = !1;
-    if (je(e) ? (d = () => e.value, m = vo(e)) : $t(e) ? (d = () => c(e), m = !0) : ee(e) ? (f = !0, m = e.some(k => $t(k) || vo(k)), d = () => e.map(k => {
-            if (je(k)) return k.value;
-            if ($t(k)) return c(k);
-            if (re(k)) return ut(k, s, 2)
+    if (je(e) ? (d = () => e.value, m = vo(e)) : $t(e) ? (d = () => c(e), m = !0) : ee(e) ? (f = !0, m = e.some(E => $t(E) || vo(E)), d = () => e.map(E => {
+            if (je(E)) return E.value;
+            if ($t(E)) return c(E);
+            if (re(E)) return ut(E, s, 2)
         })) : re(e) ? n ? d = () => ut(e, s, 2) : d = () => (_ && _(), yn(e, s, 3, [p])) : d = dn, n && r) {
-        const k = d;
-        d = () => St(k())
+        const E = d;
+        d = () => St(E())
     }
-    let _, p = k => {
+    let _, p = E => {
             _ = h.onStop = () => {
-                ut(k, s, 4), _ = h.onStop = void 0
+                ut(E, s, 4), _ = h.onStop = void 0
             }
         },
         g;
     if (Zo)
         if (p = dn, n ? t && yn(n, s, 3, [d(), f ? [] : void 0, p]) : d(), o === "sync") {
-            const k = xf();
-            g = k.__watcherHandles || (k.__watcherHandles = [])
+            const E = xf();
+            g = E.__watcherHandles || (E.__watcherHandles = [])
         } else return dn;
     let y = f ? new Array(e.length).fill(Zr) : Zr;
     const z = () => {
         if (!(!h.active || !h.dirty))
             if (n) {
-                const k = h.run();
-                (r || m || (f ? k.some((D, P) => mt(D, y[P])) : mt(k, y))) && (_ && _(), yn(n, s, 3, [k, y === Zr ? void 0 : f && y[0] === Zr ? [] : y, p]), y = k)
+                const E = h.run();
+                (r || m || (f ? E.some((I, P) => mt(I, y[P])) : mt(E, y))) && (_ && _(), yn(n, s, 3, [E, y === Zr ? void 0 : f && y[0] === Zr ? [] : y, p]), y = E)
             } else h.run()
     };
     z.allowRecurse = !!n;
     let b;
     o === "sync" ? b = z : o === "post" ? b = () => rn(z, s && s.suspense) : (z.pre = !0, s && (z.id = s.uid), b = () => ja(z));
     const h = new Oa(d, dn, b),
         S = Hd(),
-        E = () => {
+        k = () => {
             h.stop(), S && Ma(S.effects, h)
         };
-    return n ? t ? z() : y = h.run() : o === "post" ? rn(h.run.bind(h), s && s.suspense) : h.run(), g && g.push(E), E
+    return n ? t ? z() : y = h.run() : o === "post" ? rn(h.run.bind(h), s && s.suspense) : h.run(), g && g.push(k), k
 }
 
 function Rf(e, n, t) {
     const r = this.proxy,
         o = Me(e) ? e.includes(".") ? hc(r, e) : () => r[e] : e.bind(r, r);
     let a;
     re(n) ? a = n : (a = n.handler, t = n);
@@ -1522,15 +1522,15 @@
 function pt(e, n, t, r) {
     const o = e.dirs,
         a = n && n.dirs;
     for (let l = 0; l < o.length; l++) {
         const u = o[l];
         a && (u.oldValue = a[l].value);
         let s = u.dir[r];
-        s && (Ct(), yn(s, t, 8, [e.el, u, e, n]), It())
+        s && (Ct(), yn(s, t, 8, [e.el, u, e, n]), Dt())
     }
 }
 const nt = Symbol("_leaveCb"),
     Jr = Symbol("_enterCb");
 
 function gc() {
     const e = {
@@ -1585,21 +1585,21 @@
                 const l = ce(e),
                     {
                         mode: u
                     } = l;
                 if (r.isLeaving) return fi(a);
                 const s = Ml(a);
                 if (!s) return fi(a);
-                const c = Ir(s, l, r, t);
-                Dr(s, c);
+                const c = Dr(s, l, r, t);
+                Ir(s, c);
                 const d = t.subTree,
                     m = d && Ml(d);
                 if (m && m.type !== en && !Ln(s, m)) {
-                    const f = Ir(m, l, r, t);
-                    if (Dr(m, f), u === "out-in") return r.isLeaving = !0, f.afterLeave = () => {
+                    const f = Dr(m, l, r, t);
+                    if (Ir(m, f), u === "out-in") return r.isLeaving = !0, f.afterLeave = () => {
                         r.isLeaving = !1, t.update.active !== !1 && (t.effect.dirty = !0, t.update())
                     }, fi(a);
                     u === "in-out" && s.type !== en && (f.delayLeave = (_, p, g) => {
                         const y = vc(r, m);
                         y[String(m.key)] = m, _[nt] = () => {
                             p(), _[nt] = void 0, delete c.delayedLeave
                         }, c.delayedLeave = g
@@ -1615,15 +1615,15 @@
     const {
         leavingVNodes: t
     } = e;
     let r = t.get(n.type);
     return r || (r = Object.create(null), t.set(n.type, r)), r
 }
 
-function Ir(e, n, t, r) {
+function Dr(e, n, t, r) {
     const {
         appear: o,
         mode: a,
         persisted: l = !1,
         onBeforeEnter: u,
         onEnter: s,
         onAfterEnter: c,
@@ -1632,71 +1632,71 @@
         onLeave: f,
         onAfterLeave: _,
         onLeaveCancelled: p,
         onBeforeAppear: g,
         onAppear: y,
         onAfterAppear: z,
         onAppearCancelled: b
-    } = n, h = String(e.key), S = vc(t, e), E = (P, M) => {
+    } = n, h = String(e.key), S = vc(t, e), k = (P, M) => {
         P && yn(P, r, 9, M)
-    }, k = (P, M) => {
+    }, E = (P, M) => {
         const L = M[1];
-        E(P, M), ee(P) ? P.every(F => F.length <= 1) && L() : P.length <= 1 && L()
-    }, D = {
+        k(P, M), ee(P) ? P.every(F => F.length <= 1) && L() : P.length <= 1 && L()
+    }, I = {
         mode: a,
         persisted: l,
         beforeEnter(P) {
             let M = u;
             if (!t.isMounted)
                 if (o) M = g || u;
                 else return;
             P[nt] && P[nt](!0);
             const L = S[h];
-            L && Ln(e, L) && L.el[nt] && L.el[nt](), E(M, [P])
+            L && Ln(e, L) && L.el[nt] && L.el[nt](), k(M, [P])
         },
         enter(P) {
             let M = s,
                 L = c,
                 F = d;
             if (!t.isMounted)
                 if (o) M = y || s, L = z || c, F = b || d;
                 else return;
             let O = !1;
             const V = P[Jr] = Z => {
-                O || (O = !0, Z ? E(F, [P]) : E(L, [P]), D.delayedLeave && D.delayedLeave(), P[Jr] = void 0)
+                O || (O = !0, Z ? k(F, [P]) : k(L, [P]), I.delayedLeave && I.delayedLeave(), P[Jr] = void 0)
             };
-            M ? k(M, [P, V]) : V()
+            M ? E(M, [P, V]) : V()
         },
         leave(P, M) {
             const L = String(e.key);
             if (P[Jr] && P[Jr](!0), t.isUnmounting) return M();
-            E(m, [P]);
+            k(m, [P]);
             let F = !1;
             const O = P[nt] = V => {
-                F || (F = !0, M(), V ? E(p, [P]) : E(_, [P]), P[nt] = void 0, S[L] === e && delete S[L])
+                F || (F = !0, M(), V ? k(p, [P]) : k(_, [P]), P[nt] = void 0, S[L] === e && delete S[L])
             };
-            S[L] = e, f ? k(f, [P, O]) : O()
+            S[L] = e, f ? E(f, [P, O]) : O()
         },
         clone(P) {
-            return Ir(P, n, t, r)
+            return Dr(P, n, t, r)
         }
     };
-    return D
+    return I
 }
 
 function fi(e) {
     if (Wo(e)) return e = dt(e), e.children = null, e
 }
 
 function Ml(e) {
     return Wo(e) ? e.children ? e.children[0] : void 0 : e
 }
 
-function Dr(e, n) {
-    e.shapeFlag & 6 && e.component ? Dr(e.component.subTree, n) : e.shapeFlag & 128 ? (e.ssContent.transition = n.clone(e.ssContent), e.ssFallback.transition = n.clone(e.ssFallback)) : e.transition = n
+function Ir(e, n) {
+    e.shapeFlag & 6 && e.component ? Ir(e.component.subTree, n) : e.shapeFlag & 128 ? (e.ssContent.transition = n.clone(e.ssContent), e.ssFallback.transition = n.clone(e.ssFallback)) : e.transition = n
 }
 
 function Xa(e, n = !1, t) {
     let r = [],
         o = 0;
     for (let a = 0; a < e.length; a++) {
         let l = e[a];
@@ -1705,16 +1705,16 @@
             key: u
         }) : l)
     }
     if (o > 1)
         for (let a = 0; a < r.length; a++) r[a].patchFlag = -2;
     return r
 } /*! #__NO_SIDE_EFFECTS__ */
-function Dt(e, n) {
-    return re(e) ? (() => De({
+function It(e, n) {
+    return re(e) ? (() => Ie({
         name: e.name
     }, n, {
         setup: e
     }))() : e
 }
 const br = e => !!e.type.__asyncLoader,
     Wo = e => e.type.__isKeepAlive;
@@ -1753,15 +1753,15 @@
     if (t) {
         const o = t[e] || (t[e] = []),
             a = n.__weh || (n.__weh = (...l) => {
                 if (t.isUnmounted) return;
                 Ct();
                 const u = Pt(t),
                     s = yn(n, t, e, l);
-                return u(), It(), s
+                return u(), Dt(), s
             });
         return r ? o.unshift(a) : o.push(a), a
     }
 }
 const $n = e => (n, t = Ve) => (!Zo || e === "sp") && $o(e, (...r) => n(...r), t),
     Vf = $n("bm"),
     ur = $n("m"),
@@ -1773,15 +1773,15 @@
     Uf = $n("rtg"),
     qf = $n("rtc");
 
 function Wf(e, n = Ve) {
     $o("ec", e, n)
 }
 
-function I1(e, n, t, r) {
+function D1(e, n, t, r) {
     let o;
     const a = t && t[r];
     if (ee(e) || Me(e)) {
         o = new Array(e.length);
         for (let l = 0, u = e.length; l < u; l++) o[l] = n(e[l], l, void 0, a && a[l])
     } else if (typeof e == "number") {
         o = new Array(e);
@@ -1796,15 +1796,15 @@
                 o[u] = n(e[c], c, u, a && a[u])
             }
         }
     else o = [];
     return t && (t[r] = o), o
 }
 
-function D1(e, n) {
+function I1(e, n) {
     for (let t = 0; t < n.length; t++) {
         const r = n[t];
         if (ee(r))
             for (let o = 0; o < r.length; o++) e[r[o].name] = r[o].fn;
         else r && (e[r.name] = r.key ? (...o) => {
             const a = r.fn(...o);
             return a && (a.key = r.key), a
@@ -1824,15 +1824,15 @@
     return !o && u.scopeId && (u.slotScopeIds = [u.scopeId + "-s"]), a && a._c && (a._d = !0), u
 }
 
 function Sc(e) {
     return e.some(n => er(n) ? !(n.type === en || n.type === Fe && !Sc(n.children)) : !0) ? e : null
 }
 const Wi = e => e ? Gc(e) ? Jo(e) || e.proxy : Wi(e.parent) : null,
-    vr = De(Object.create(null), {
+    vr = Ie(Object.create(null), {
         $: e => e,
         $el: e => e.vnode.el,
         $data: e => e.data,
         $props: e => e.props,
         $attrs: e => e.attrs,
         $slots: e => e.slots,
         $refs: e => e.refs,
@@ -1928,15 +1928,15 @@
 }
 let $i = !0;
 
 function Kf(e) {
     const n = Qa(e),
         t = e.proxy,
         r = e.ctx;
-    $i = !1, n.beforeCreate && Il(n.beforeCreate, e, "bc");
+    $i = !1, n.beforeCreate && Dl(n.beforeCreate, e, "bc");
     const {
         data: o,
         computed: a,
         methods: l,
         watch: u,
         provide: s,
         inject: c,
@@ -1947,17 +1947,17 @@
         updated: p,
         activated: g,
         deactivated: y,
         beforeDestroy: z,
         beforeUnmount: b,
         destroyed: h,
         unmounted: S,
-        render: E,
-        renderTracked: k,
-        renderTriggered: D,
+        render: k,
+        renderTracked: E,
+        renderTriggered: I,
         errorCaptured: P,
         serverPrefetch: M,
         expose: L,
         inheritAttrs: F,
         components: O,
         directives: V,
         filters: Z
@@ -1972,49 +1972,49 @@
         ye(se) && (e.data = on(se))
     }
     if ($i = !0, a)
         for (const se in a) {
             const ue = a[se],
                 Ue = re(ue) ? ue.bind(t, t) : re(ue.get) ? ue.get.bind(t, t) : dn,
                 Xe = !re(ue) && re(ue.set) ? ue.set.bind(t) : dn,
-                Ee = ae({
+                ke = ae({
                     get: Ue,
                     set: Xe
                 });
             Object.defineProperty(r, se, {
                 enumerable: !0,
                 configurable: !0,
-                get: () => Ee.value,
-                set: ke => Ee.value = ke
+                get: () => ke.value,
+                set: Ee => ke.value = Ee
             })
         }
     if (u)
         for (const se in u) wc(u[se], r, t, se);
     if (s) {
         const se = re(s) ? s.call(t) : s;
         Reflect.ownKeys(se).forEach(ue => {
             Wn(ue, se[ue])
         })
     }
-    d && Il(d, e, "c");
+    d && Dl(d, e, "c");
 
     function ie(se, ue) {
         ee(ue) ? ue.forEach(Ue => se(Ue.bind(t))) : ue && se(ue.bind(t))
     }
-    if (ie(Vf, m), ie(ur, f), ie(Tc, _), ie(Ko, p), ie(Bf, g), ie(Hf, y), ie(Wf, P), ie(qf, k), ie(Uf, D), ie(Xo, b), ie(Ya, S), ie(jf, M), ee(L))
+    if (ie(Vf, m), ie(ur, f), ie(Tc, _), ie(Ko, p), ie(Bf, g), ie(Hf, y), ie(Wf, P), ie(qf, E), ie(Uf, I), ie(Xo, b), ie(Ya, S), ie(jf, M), ee(L))
         if (L.length) {
             const se = e.exposed || (e.exposed = {});
             L.forEach(ue => {
                 Object.defineProperty(se, ue, {
                     get: () => t[ue],
                     set: Ue => t[ue] = Ue
                 })
             })
         } else e.exposed || (e.exposed = {});
-    E && e.render === dn && (e.render = E), F != null && (e.inheritAttrs = F), O && (e.components = O), V && (e.directives = V)
+    k && e.render === dn && (e.render = k), F != null && (e.inheritAttrs = F), O && (e.components = O), V && (e.directives = V)
 }
 
 function Xf(e, n, t = dn) {
     ee(e) && (e = Ki(e));
     for (const r in e) {
         const o = e[r];
         let a;
@@ -2023,15 +2023,15 @@
             configurable: !0,
             get: () => a.value,
             set: l => a.value = l
         }) : n[r] = a
     }
 }
 
-function Il(e, n, t) {
+function Dl(e, n, t) {
     yn(ee(e) ? e.map(r => r.bind(n.proxy)) : e.bind(n.proxy), n, t)
 }
 
 function wc(e, n, t, r) {
     const o = r.includes(".") ? hc(t, r) : () => t[r];
     if (Me(e)) {
         const a = n[e];
@@ -2072,15 +2072,15 @@
     for (const l in n)
         if (!(r && l === "expose")) {
             const u = Yf[l] || t && t[l];
             e[l] = u ? u(e[l], n[l]) : n[l]
         } return e
 }
 const Yf = {
-    data: Dl,
+    data: Il,
     props: Ll,
     emits: Ll,
     methods: hr,
     computed: hr,
     beforeCreate: Qe,
     created: Qe,
     beforeMount: Qe,
@@ -2094,21 +2094,21 @@
     activated: Qe,
     deactivated: Qe,
     errorCaptured: Qe,
     serverPrefetch: Qe,
     components: hr,
     directives: hr,
     watch: Zf,
-    provide: Dl,
+    provide: Il,
     inject: Qf
 };
 
-function Dl(e, n) {
+function Il(e, n) {
     return n ? e ? function() {
-        return De(re(e) ? e.call(this, this) : e, re(n) ? n.call(this, this) : n)
+        return Ie(re(e) ? e.call(this, this) : e, re(n) ? n.call(this, this) : n)
     } : n : e
 }
 
 function Qf(e, n) {
     return hr(Ki(e), Ki(n))
 }
 
@@ -2122,30 +2122,30 @@
 }
 
 function Qe(e, n) {
     return e ? [...new Set([].concat(e, n))] : n
 }
 
 function hr(e, n) {
-    return e ? De(Object.create(null), e, n) : n
+    return e ? Ie(Object.create(null), e, n) : n
 }
 
 function Ll(e, n) {
-    return e ? ee(e) && ee(n) ? [...new Set([...e, ...n])] : De(Object.create(null), Cl(e), Cl(n ?? {})) : n
+    return e ? ee(e) && ee(n) ? [...new Set([...e, ...n])] : Ie(Object.create(null), Cl(e), Cl(n ?? {})) : n
 }
 
 function Zf(e, n) {
     if (!e) return n;
     if (!n) return e;
-    const t = De(Object.create(null), e);
+    const t = Ie(Object.create(null), e);
     for (const r in n) t[r] = Qe(e[r], n[r]);
     return t
 }
 
-function Ec() {
+function kc() {
     return {
         app: null,
         config: {
             isNativeTag: Ad,
             performance: !1,
             globalProperties: {},
             optionMergeStrategies: {},
@@ -2162,26 +2162,26 @@
         emitsCache: new WeakMap
     }
 }
 let Jf = 0;
 
 function e_(e, n) {
     return function(r, o = null) {
-        re(r) || (r = De({}, r)), o != null && !ye(o) && (o = null);
-        const a = Ec(),
+        re(r) || (r = Ie({}, r)), o != null && !ye(o) && (o = null);
+        const a = kc(),
             l = new WeakSet;
         let u = !1;
         const s = a.app = {
             _uid: Jf++,
             _component: r,
             _props: o,
             _container: null,
             _context: a,
             _instance: null,
-            version: E_,
+            version: k_,
             get config() {
                 return a.config
             },
             set config(c) {},
             use(c, ...d) {
                 return l.has(c) || (c && re(c.install) ? (l.add(c), c.install(s, ...d)) : re(c) && (l.add(c), c(s, ...d))), s
             },
@@ -2237,15 +2237,15 @@
         if (arguments.length > 1) return t && re(n) ? n.call(r && r.proxy) : n
     }
 }
 
 function n_(e, n, t, r = !1) {
     const o = {},
         a = {};
-    go(a, Qo, 1), e.propsDefaults = Object.create(null), kc(e, n, o, a);
+    go(a, Qo, 1), e.propsDefaults = Object.create(null), Ec(e, n, o, a);
     for (const l in e.propsOptions[0]) l in o || (o[l] = void 0);
     t ? e.props = r ? o : tc(o) : e.type.props ? e.props = o : e.props = a, e.attrs = a
 }
 
 function t_(e, n, t, r) {
     const {
         props: o,
@@ -2268,24 +2268,24 @@
                         const p = Rn(f);
                         o[p] = Xi(s, u, p, _, e, !1)
                     }
                 else _ !== a[f] && (a[f] = _, c = !0)
             }
         }
     } else {
-        kc(e, n, o, a) && (c = !0);
+        Ec(e, n, o, a) && (c = !0);
         let d;
         for (const m in u)(!n || !fe(n, m) && ((d = sr(m)) === m || !fe(n, d))) && (s ? t && (t[m] !== void 0 || t[d] !== void 0) && (o[m] = Xi(s, u, m, void 0, e, !0)) : delete o[m]);
         if (a !== u)
             for (const m in a)(!n || !fe(n, m)) && (delete a[m], c = !0)
     }
     c && qn(e, "set", "$attrs")
 }
 
-function kc(e, n, t, r) {
+function Ec(e, n, t, r) {
     const [o, a] = e.propsOptions;
     let l = !1,
         u;
     if (n)
         for (let s in n) {
             if (gr(s)) continue;
             const c = n[s];
@@ -2333,15 +2333,15 @@
         l = {},
         u = [];
     let s = !1;
     if (!re(e)) {
         const d = m => {
             s = !0;
             const [f, _] = Ac(m, n, !0);
-            De(l, f), _ && u.push(..._)
+            Ie(l, f), _ && u.push(..._)
         };
         !t && n.mixins.length && n.mixins.forEach(d), e.extends && d(e.extends), e.mixins && e.mixins.forEach(d)
     }
     if (!a && !s) return ye(e) && r.set(e, qt), qt;
     if (ee(a))
         for (let d = 0; d < a.length; d++) {
             const m = Rn(a[d]);
@@ -2349,15 +2349,15 @@
         } else if (a)
             for (const d in a) {
                 const m = Rn(d);
                 if (Ol(m)) {
                     const f = a[d],
                         _ = l[m] = ee(f) || re(f) ? {
                             type: f
-                        } : De({}, f);
+                        } : Ie({}, f);
                     if (_) {
                         const p = Nl(Boolean, _.type),
                             g = Nl(String, _.type);
                         _[0] = p > -1, _[1] = g < 0 || p < g, (p > -1 || fe(_, "default")) && u.push(m)
                     }
                 }
             }
@@ -2377,15 +2377,15 @@
     return xl(e) === xl(n)
 }
 
 function Nl(e, n) {
     return ee(n) ? n.findIndex(t => Rl(t, e)) : re(n) && Rl(n, e) ? 0 : -1
 }
 const Pc = e => e[0] === "_" || e === "$stable",
-    Za = e => ee(e) ? e.map(kn) : [kn(e)],
+    Za = e => ee(e) ? e.map(En) : [En(e)],
     r_ = (e, n, t) => {
         if (n._n) return n;
         const r = bf((...o) => Za(n(...o)), t);
         return r._c = !1, r
     },
     Mc = (e, n, t) => {
         const r = e._ctx;
@@ -2415,15 +2415,15 @@
             vnode: r,
             slots: o
         } = e;
         let a = !0,
             l = Te;
         if (r.shapeFlag & 32) {
             const u = n._;
-            u ? t && u === 1 ? a = !1 : (De(o, n), !t && u === 1 && delete o._) : (a = !n.$stable, Mc(n, o)), l = n
+            u ? t && u === 1 ? a = !1 : (Ie(o, n), !t && u === 1 && delete o._) : (a = !n.$stable, Mc(n, o)), l = n
         } else n && (Cc(e, n), l = {
             default: 1
         });
         if (a)
             for (const u in o) !Pc(u) && l[u] == null && delete o[u]
     };
 
@@ -2453,15 +2453,15 @@
                     o ? ee(g) && Ma(g, a) : ee(g) ? g.includes(a) || g.push(a) : f ? (d[s] = [a], fe(m, s) && (m[s] = d[s])) : (s.value = [a], e.k && (d[e.k] = s.value))
                 } else f ? (d[s] = l, fe(m, s) && (m[s] = l)) : _ && (s.value = l, e.k && (d[e.k] = l))
             };
             l ? (p.id = -1, rn(p, t)) : p()
         }
     }
 }
-const rn = Df;
+const rn = If;
 
 function a_(e) {
     return l_(e)
 }
 
 function l_(e, n) {
     const t = Hu();
@@ -2477,15 +2477,15 @@
         setElementText: d,
         parentNode: m,
         nextSibling: f,
         setScopeId: _ = dn,
         insertStaticContent: p
     } = e, g = (w, A, x, H = null, N = null, U = null, $ = void 0, v = null, T = !!A.dynamicChildren) => {
         if (w === A) return;
-        w && !Ln(w, A) && (H = B(w), ke(w, N, U, !0), w = null), A.patchFlag === -2 && (T = !1, A.dynamicChildren = null);
+        w && !Ln(w, A) && (H = B(w), Ee(w, N, U, !0), w = null), A.patchFlag === -2 && (T = !1, A.dynamicChildren = null);
         const {
             type: C,
             ref: G,
             shapeFlag: q
         } = A;
         switch (C) {
             case jr:
@@ -2497,15 +2497,15 @@
             case zi:
                 w == null && b(A, x, H, $);
                 break;
             case Fe:
                 O(w, A, x, H, N, U, $, v, T);
                 break;
             default:
-                q & 1 ? E(w, A, x, H, N, U, $, v, T) : q & 6 ? V(w, A, x, H, N, U, $, v, T) : (q & 64 || q & 128) && C.process(w, A, x, H, N, U, $, v, T, X)
+                q & 1 ? k(w, A, x, H, N, U, $, v, T) : q & 6 ? V(w, A, x, H, N, U, $, v, T) : (q & 64 || q & 128) && C.process(w, A, x, H, N, U, $, v, T, X)
         }
         G != null && N && Yi(G, w && w.ref, U, A || w, !A)
     }, y = (w, A, x, H) => {
         if (w == null) r(A.el = u(A.children), x, H);
         else {
             const N = A.el = w.el;
             A.children !== w.children && c(N, A.children)
@@ -2524,74 +2524,74 @@
     }, S = ({
         el: w,
         anchor: A
     }) => {
         let x;
         for (; w && w !== A;) x = f(w), o(w), w = x;
         o(A)
-    }, E = (w, A, x, H, N, U, $, v, T) => {
-        A.type === "svg" ? $ = "svg" : A.type === "math" && ($ = "mathml"), w == null ? k(A, x, H, N, U, $, v, T) : M(w, A, N, U, $, v, T)
-    }, k = (w, A, x, H, N, U, $, v) => {
+    }, k = (w, A, x, H, N, U, $, v, T) => {
+        A.type === "svg" ? $ = "svg" : A.type === "math" && ($ = "mathml"), w == null ? E(A, x, H, N, U, $, v, T) : M(w, A, N, U, $, v, T)
+    }, E = (w, A, x, H, N, U, $, v) => {
         let T, C;
         const {
             props: G,
             shapeFlag: q,
             transition: j,
-            dirs: I
+            dirs: D
         } = w;
-        if (T = w.el = l(w.type, U, G && G.is, G), q & 8 ? d(T, w.children) : q & 16 && P(w.children, T, null, H, N, pi(w, U), $, v), I && pt(w, null, H, "created"), D(T, w, w.scopeId, $, H), G) {
+        if (T = w.el = l(w.type, U, G && G.is, G), q & 8 ? d(T, w.children) : q & 16 && P(w.children, T, null, H, N, pi(w, U), $, v), D && pt(w, null, H, "created"), I(T, w, w.scopeId, $, H), G) {
             for (const J in G) J !== "value" && !gr(J) && a(T, J, null, G[J], U, w.children, H, N, Ce);
-            "value" in G && a(T, "value", null, G.value, U), (C = G.onVnodeBeforeMount) && In(C, H, w)
+            "value" in G && a(T, "value", null, G.value, U), (C = G.onVnodeBeforeMount) && Dn(C, H, w)
         }
-        I && pt(w, null, H, "beforeMount");
+        D && pt(w, null, H, "beforeMount");
         const R = s_(N, j);
-        R && j.beforeEnter(T), r(T, A, x), ((C = G && G.onVnodeMounted) || R || I) && rn(() => {
-            C && In(C, H, w), R && j.enter(T), I && pt(w, null, H, "mounted")
+        R && j.beforeEnter(T), r(T, A, x), ((C = G && G.onVnodeMounted) || R || D) && rn(() => {
+            C && Dn(C, H, w), R && j.enter(T), D && pt(w, null, H, "mounted")
         }, N)
-    }, D = (w, A, x, H, N) => {
+    }, I = (w, A, x, H, N) => {
         if (x && _(w, x), H)
             for (let U = 0; U < H.length; U++) _(w, H[U]);
         if (N) {
             let U = N.subTree;
             if (A === U) {
                 const $ = N.vnode;
-                D(w, $, $.scopeId, $.slotScopeIds, N.parent)
+                I(w, $, $.scopeId, $.slotScopeIds, N.parent)
             }
         }
     }, P = (w, A, x, H, N, U, $, v, T = 0) => {
         for (let C = T; C < w.length; C++) {
-            const G = w[C] = v ? tt(w[C]) : kn(w[C]);
+            const G = w[C] = v ? tt(w[C]) : En(w[C]);
             g(null, G, A, x, H, N, U, $, v)
         }
     }, M = (w, A, x, H, N, U, $) => {
         const v = A.el = w.el;
         let {
             patchFlag: T,
             dynamicChildren: C,
             dirs: G
         } = A;
         T |= w.patchFlag & 16;
         const q = w.props || Te,
             j = A.props || Te;
-        let I;
-        if (x && zt(x, !1), (I = j.onVnodeBeforeUpdate) && In(I, x, A, w), G && pt(A, w, x, "beforeUpdate"), x && zt(x, !0), C ? L(w.dynamicChildren, C, v, x, H, pi(A, N), U) : $ || ue(w, A, v, null, x, H, pi(A, N), U, !1), T > 0) {
+        let D;
+        if (x && zt(x, !1), (D = j.onVnodeBeforeUpdate) && Dn(D, x, A, w), G && pt(A, w, x, "beforeUpdate"), x && zt(x, !0), C ? L(w.dynamicChildren, C, v, x, H, pi(A, N), U) : $ || ue(w, A, v, null, x, H, pi(A, N), U, !1), T > 0) {
             if (T & 16) F(v, A, q, j, x, H, N);
             else if (T & 2 && q.class !== j.class && a(v, "class", null, j.class, N), T & 4 && a(v, "style", q.style, j.style, N), T & 8) {
                 const R = A.dynamicProps;
                 for (let J = 0; J < R.length; J++) {
                     const te = R[J],
                         ge = q[te],
                         qe = j[te];
                     (qe !== ge || te === "value") && a(v, te, ge, qe, N, w.children, x, H, Ce)
                 }
             }
             T & 1 && w.children !== A.children && d(v, A.children)
         } else !$ && C == null && F(v, A, q, j, x, H, N);
-        ((I = j.onVnodeUpdated) || G) && rn(() => {
-            I && In(I, x, A, w), G && pt(A, w, x, "updated")
+        ((D = j.onVnodeUpdated) || G) && rn(() => {
+            D && Dn(D, x, A, w), G && pt(A, w, x, "updated")
         }, H)
     }, L = (w, A, x, H, N, U, $) => {
         for (let v = 0; v < A.length; v++) {
             const T = w[v],
                 C = A[v],
                 G = T.el && (T.type === Fe || !Ln(T, C) || T.shapeFlag & 70) ? m(T.el) : x;
             g(T, C, G, null, H, N, U, $, !0)
@@ -2610,17 +2610,17 @@
         }
     }, O = (w, A, x, H, N, U, $, v, T) => {
         const C = A.el = w ? w.el : u(""),
             G = A.anchor = w ? w.anchor : u("");
         let {
             patchFlag: q,
             dynamicChildren: j,
-            slotScopeIds: I
+            slotScopeIds: D
         } = A;
-        I && (v = v ? v.concat(I) : I), w == null ? (r(C, x, H), r(G, x, H), P(A.children || [], x, G, N, U, $, v, T)) : q > 0 && q & 64 && j && w.dynamicChildren ? (L(w.dynamicChildren, j, x, N, U, $, v), (A.key != null || N && A === N.subTree) && Ja(w, A, !0)) : ue(w, A, x, G, N, U, $, v, T)
+        D && (v = v ? v.concat(D) : D), w == null ? (r(C, x, H), r(G, x, H), P(A.children || [], x, G, N, U, $, v, T)) : q > 0 && q & 64 && j && w.dynamicChildren ? (L(w.dynamicChildren, j, x, N, U, $, v), (A.key != null || N && A === N.subTree) && Ja(w, A, !0)) : ue(w, A, x, G, N, U, $, v, T)
     }, V = (w, A, x, H, N, U, $, v, T) => {
         A.slotScopeIds = v, w == null ? A.shapeFlag & 512 ? N.ctx.activate(A, x, H, $, T) : Z(A, x, H, N, U, $, T) : oe(w, A, T)
     }, Z = (w, A, x, H, N, U, $) => {
         const v = w.component = g_(w, H, N);
         if (Wo(w) && (v.ctx.renderer = X), b_(v), v.asyncDep) {
             if (N && N.registerDep(v, ie), !w.el) {
                 const T = v.subTree = ve(en);
@@ -2638,231 +2638,231 @@
     }, ie = (w, A, x, H, N, U, $) => {
         const v = () => {
                 if (w.isMounted) {
                     let {
                         next: G,
                         bu: q,
                         u: j,
-                        parent: I,
+                        parent: D,
                         vnode: R
                     } = w;
                     {
-                        const ln = Ic(w);
+                        const ln = Dc(w);
                         if (ln) {
                             G && (G.el = R.el, se(w, G, $)), ln.asyncDep.then(() => {
                                 w.isUnmounted || v()
                             });
                             return
                         }
                     }
                     let J = G,
                         te;
-                    zt(w, !1), G ? (G.el = R.el, se(w, G, $)) : G = R, q && ci(q), (te = G.props && G.props.onVnodeBeforeUpdate) && In(te, I, G, R), zt(w, !0);
+                    zt(w, !1), G ? (G.el = R.el, se(w, G, $)) : G = R, q && ci(q), (te = G.props && G.props.onVnodeBeforeUpdate) && Dn(te, D, G, R), zt(w, !0);
                     const ge = di(w),
                         qe = w.subTree;
-                    w.subTree = ge, g(qe, ge, m(qe.el), B(qe), w, N, U), G.el = ge.el, J === null && Ua(w, ge.el), j && rn(j, N), (te = G.props && G.props.onVnodeUpdated) && rn(() => In(te, I, G, R), N)
+                    w.subTree = ge, g(qe, ge, m(qe.el), B(qe), w, N, U), G.el = ge.el, J === null && Ua(w, ge.el), j && rn(j, N), (te = G.props && G.props.onVnodeUpdated) && rn(() => Dn(te, D, G, R), N)
                 } else {
                     let G;
                     const {
                         el: q,
                         props: j
                     } = A, {
-                        bm: I,
+                        bm: D,
                         m: R,
                         parent: J
                     } = w, te = br(A);
-                    if (zt(w, !1), I && ci(I), !te && (G = j && j.onVnodeBeforeMount) && In(G, J, A), zt(w, !0), q && ze) {
+                    if (zt(w, !1), D && ci(D), !te && (G = j && j.onVnodeBeforeMount) && Dn(G, J, A), zt(w, !0), q && ze) {
                         const ge = () => {
                             w.subTree = di(w), ze(q, w.subTree, w, N, null)
                         };
                         te ? A.type.__asyncLoader().then(() => !w.isUnmounted && ge()) : ge()
                     } else {
                         const ge = w.subTree = di(w);
                         g(null, ge, x, H, w, N, U), A.el = ge.el
                     }
                     if (R && rn(R, N), !te && (G = j && j.onVnodeMounted)) {
                         const ge = A;
-                        rn(() => In(G, J, ge), N)
+                        rn(() => Dn(G, J, ge), N)
                     }(A.shapeFlag & 256 || J && br(J.vnode) && J.vnode.shapeFlag & 256) && w.a && rn(w.a, N), w.isMounted = !0, A = x = H = null
                 }
             },
             T = w.effect = new Oa(v, dn, () => ja(C), w.scope),
             C = w.update = () => {
                 T.dirty && T.run()
             };
         C.id = w.uid, zt(w, !0), C()
     }, se = (w, A, x) => {
         A.component = w;
         const H = w.vnode.props;
-        w.vnode = A, w.next = null, t_(w, A.props, H, x), i_(w, A.children, x), Ct(), El(w), It()
+        w.vnode = A, w.next = null, t_(w, A.props, H, x), i_(w, A.children, x), Ct(), kl(w), Dt()
     }, ue = (w, A, x, H, N, U, $, v, T = !1) => {
         const C = w && w.children,
             G = w ? w.shapeFlag : 0,
             q = A.children,
             {
                 patchFlag: j,
-                shapeFlag: I
+                shapeFlag: D
             } = A;
         if (j > 0) {
             if (j & 128) {
                 Xe(C, q, x, H, N, U, $, v, T);
                 return
             } else if (j & 256) {
                 Ue(C, q, x, H, N, U, $, v, T);
                 return
             }
         }
-        I & 8 ? (G & 16 && Ce(C, N, U), q !== C && d(x, q)) : G & 16 ? I & 16 ? Xe(C, q, x, H, N, U, $, v, T) : Ce(C, N, U, !0) : (G & 8 && d(x, ""), I & 16 && P(q, x, H, N, U, $, v, T))
+        D & 8 ? (G & 16 && Ce(C, N, U), q !== C && d(x, q)) : G & 16 ? D & 16 ? Xe(C, q, x, H, N, U, $, v, T) : Ce(C, N, U, !0) : (G & 8 && d(x, ""), D & 16 && P(q, x, H, N, U, $, v, T))
     }, Ue = (w, A, x, H, N, U, $, v, T) => {
         w = w || qt, A = A || qt;
         const C = w.length,
             G = A.length,
             q = Math.min(C, G);
         let j;
         for (j = 0; j < q; j++) {
-            const I = A[j] = T ? tt(A[j]) : kn(A[j]);
-            g(w[j], I, x, null, N, U, $, v, T)
+            const D = A[j] = T ? tt(A[j]) : En(A[j]);
+            g(w[j], D, x, null, N, U, $, v, T)
         }
         C > G ? Ce(w, N, U, !0, !1, q) : P(A, x, H, N, U, $, v, T, q)
     }, Xe = (w, A, x, H, N, U, $, v, T) => {
         let C = 0;
         const G = A.length;
         let q = w.length - 1,
             j = G - 1;
         for (; C <= q && C <= j;) {
-            const I = w[C],
-                R = A[C] = T ? tt(A[C]) : kn(A[C]);
-            if (Ln(I, R)) g(I, R, x, null, N, U, $, v, T);
+            const D = w[C],
+                R = A[C] = T ? tt(A[C]) : En(A[C]);
+            if (Ln(D, R)) g(D, R, x, null, N, U, $, v, T);
             else break;
             C++
         }
         for (; C <= q && C <= j;) {
-            const I = w[q],
-                R = A[j] = T ? tt(A[j]) : kn(A[j]);
-            if (Ln(I, R)) g(I, R, x, null, N, U, $, v, T);
+            const D = w[q],
+                R = A[j] = T ? tt(A[j]) : En(A[j]);
+            if (Ln(D, R)) g(D, R, x, null, N, U, $, v, T);
             else break;
             q--, j--
         }
         if (C > q) {
             if (C <= j) {
-                const I = j + 1,
-                    R = I < G ? A[I].el : H;
-                for (; C <= j;) g(null, A[C] = T ? tt(A[C]) : kn(A[C]), x, R, N, U, $, v, T), C++
+                const D = j + 1,
+                    R = D < G ? A[D].el : H;
+                for (; C <= j;) g(null, A[C] = T ? tt(A[C]) : En(A[C]), x, R, N, U, $, v, T), C++
             }
         } else if (C > j)
-            for (; C <= q;) ke(w[C], N, U, !0), C++;
+            for (; C <= q;) Ee(w[C], N, U, !0), C++;
         else {
-            const I = C,
+            const D = C,
                 R = C,
                 J = new Map;
             for (C = R; C <= j; C++) {
-                const sn = A[C] = T ? tt(A[C]) : kn(A[C]);
+                const sn = A[C] = T ? tt(A[C]) : En(A[C]);
                 sn.key != null && J.set(sn.key, C)
             }
             let te, ge = 0;
             const qe = j - R + 1;
             let ln = !1,
                 Wr = 0;
             const xt = new Array(qe);
             for (C = 0; C < qe; C++) xt[C] = 0;
-            for (C = I; C <= q; C++) {
+            for (C = D; C <= q; C++) {
                 const sn = w[C];
                 if (ge >= qe) {
-                    ke(sn, N, U, !0);
+                    Ee(sn, N, U, !0);
                     continue
                 }
                 let Cn;
                 if (sn.key != null) Cn = J.get(sn.key);
                 else
                     for (te = R; te <= j; te++)
                         if (xt[te - R] === 0 && Ln(sn, A[te])) {
                             Cn = te;
                             break
-                        } Cn === void 0 ? ke(sn, N, U, !0) : (xt[Cn - R] = C + 1, Cn >= Wr ? Wr = Cn : ln = !0, g(sn, A[Cn], x, null, N, U, $, v, T), ge++)
+                        } Cn === void 0 ? Ee(sn, N, U, !0) : (xt[Cn - R] = C + 1, Cn >= Wr ? Wr = Cn : ln = !0, g(sn, A[Cn], x, null, N, U, $, v, T), ge++)
             }
             const pl = ln ? u_(xt) : qt;
             for (te = pl.length - 1, C = qe - 1; C >= 0; C--) {
                 const sn = R + C,
                     Cn = A[sn],
                     zl = sn + 1 < G ? A[sn + 1].el : H;
-                xt[C] === 0 ? g(null, Cn, x, zl, N, U, $, v, T) : ln && (te < 0 || C !== pl[te] ? Ee(Cn, x, zl, 2) : te--)
+                xt[C] === 0 ? g(null, Cn, x, zl, N, U, $, v, T) : ln && (te < 0 || C !== pl[te] ? ke(Cn, x, zl, 2) : te--)
             }
         }
-    }, Ee = (w, A, x, H, N = null) => {
+    }, ke = (w, A, x, H, N = null) => {
         const {
             el: U,
             type: $,
             transition: v,
             children: T,
             shapeFlag: C
         } = w;
         if (C & 6) {
-            Ee(w.component.subTree, A, x, H);
+            ke(w.component.subTree, A, x, H);
             return
         }
         if (C & 128) {
             w.suspense.move(A, x, H);
             return
         }
         if (C & 64) {
             $.move(w, A, x, X);
             return
         }
         if ($ === Fe) {
             r(U, A, x);
-            for (let q = 0; q < T.length; q++) Ee(T[q], A, x, H);
+            for (let q = 0; q < T.length; q++) ke(T[q], A, x, H);
             r(w.anchor, A, x);
             return
         }
         if ($ === zi) {
             h(w, A, x);
             return
         }
         if (H !== 2 && C & 1 && v)
             if (H === 0) v.beforeEnter(U), r(U, A, x), rn(() => v.enter(U), N);
             else {
                 const {
                     leave: q,
                     delayLeave: j,
-                    afterLeave: I
+                    afterLeave: D
                 } = v, R = () => r(U, A, x), J = () => {
                     q(U, () => {
-                        R(), I && I()
+                        R(), D && D()
                     })
                 };
                 j ? j(U, R, J) : J()
             }
         else r(U, A, x)
-    }, ke = (w, A, x, H = !1, N = !1) => {
+    }, Ee = (w, A, x, H = !1, N = !1) => {
         const {
             type: U,
             props: $,
             ref: v,
             children: T,
             dynamicChildren: C,
             shapeFlag: G,
             patchFlag: q,
             dirs: j
         } = w;
         if (v != null && Yi(v, null, x, w, !0), G & 256) {
             A.ctx.deactivate(w);
             return
         }
-        const I = G & 1 && j,
+        const D = G & 1 && j,
             R = !br(w);
         let J;
-        if (R && (J = $ && $.onVnodeBeforeUnmount) && In(J, A, w), G & 6) Kn(w.component, x, H);
+        if (R && (J = $ && $.onVnodeBeforeUnmount) && Dn(J, A, w), G & 6) Kn(w.component, x, H);
         else {
             if (G & 128) {
                 w.suspense.unmount(x, H);
                 return
             }
-            I && pt(w, null, A, "beforeUnmount"), G & 64 ? w.type.remove(w, A, x, N, X, H) : C && (U !== Fe || q > 0 && q & 64) ? Ce(C, A, x, !1, !0) : (U === Fe && q & 384 || !N && G & 16) && Ce(T, A, x), H && Mn(w)
-        }(R && (J = $ && $.onVnodeUnmounted) || I) && rn(() => {
-            J && In(J, A, w), I && pt(w, null, A, "unmounted")
+            D && pt(w, null, A, "beforeUnmount"), G & 64 ? w.type.remove(w, A, x, N, X, H) : C && (U !== Fe || q > 0 && q & 64) ? Ce(C, A, x, !1, !0) : (U === Fe && q & 384 || !N && G & 16) && Ce(T, A, x), H && Mn(w)
+        }(R && (J = $ && $.onVnodeUnmounted) || D) && rn(() => {
+            J && Dn(J, A, w), D && pt(w, null, A, "unmounted")
         }, x)
     }, Mn = w => {
         const {
             type: A,
             el: x,
             anchor: H,
             transition: N
@@ -2893,28 +2893,28 @@
         const {
             bum: H,
             scope: N,
             update: U,
             subTree: $,
             um: v
         } = w;
-        H && ci(H), N.stop(), U && (U.active = !1, ke($, w, A, x)), v && rn(v, A), rn(() => {
+        H && ci(H), N.stop(), U && (U.active = !1, Ee($, w, A, x)), v && rn(v, A), rn(() => {
             w.isUnmounted = !0
         }, A), A && A.pendingBranch && !A.isUnmounted && w.asyncDep && !w.asyncResolved && w.suspenseId === A.pendingId && (A.deps--, A.deps === 0 && A.resolve())
     }, Ce = (w, A, x, H = !1, N = !1, U = 0) => {
-        for (let $ = U; $ < w.length; $++) ke(w[$], A, x, H, N)
+        for (let $ = U; $ < w.length; $++) Ee(w[$], A, x, H, N)
     }, B = w => w.shapeFlag & 6 ? B(w.component.subTree) : w.shapeFlag & 128 ? w.suspense.next() : f(w.anchor || w.el);
     let K = !1;
     const W = (w, A, x) => {
-            w == null ? A._vnode && ke(A._vnode, null, null, !0) : g(A._vnode || null, w, A, null, null, null, x), K || (K = !0, El(), fc(), K = !1), A._vnode = w
+            w == null ? A._vnode && Ee(A._vnode, null, null, !0) : g(A._vnode || null, w, A, null, null, null, x), K || (K = !0, kl(), fc(), K = !1), A._vnode = w
         },
         X = {
             p: g,
-            um: ke,
-            m: Ee,
+            um: Ee,
+            m: ke,
             r: Mn,
             mt: Z,
             mc: P,
             pc: ue,
             pbc: L,
             n: B,
             o: e
@@ -2972,17 +2972,17 @@
             c < e[t[a]] && (a > 0 && (n[r] = t[a - 1]), t[a] = r)
         }
     }
     for (a = t.length, l = t[a - 1]; a-- > 0;) t[a] = l, l = n[l];
     return t
 }
 
-function Ic(e) {
+function Dc(e) {
     const n = e.subTree.component;
-    if (n) return n.asyncDep && !n.asyncResolved ? n : Ic(n)
+    if (n) return n.asyncDep && !n.asyncResolved ? n : Dc(n)
 }
 const c_ = e => e.__isTeleport,
     Tr = e => e && (e.disabled || e.disabled === ""),
     Gl = e => typeof SVGElement < "u" && e instanceof SVGElement,
     Bl = e => typeof MathMLElement == "function" && e instanceof MathMLElement,
     Qi = (e, n) => {
         const t = e && e.to;
@@ -3005,39 +3005,39 @@
             } = c, z = Tr(n.props);
             let {
                 shapeFlag: b,
                 children: h,
                 dynamicChildren: S
             } = n;
             if (e == null) {
-                const E = n.el = g(""),
-                    k = n.anchor = g("");
-                _(E, t, r), _(k, t, r);
-                const D = n.target = Qi(n.props, p),
+                const k = n.el = g(""),
+                    E = n.anchor = g("");
+                _(k, t, r), _(E, t, r);
+                const I = n.target = Qi(n.props, p),
                     P = n.targetAnchor = g("");
-                D && (_(P, D), l === "svg" || Gl(D) ? l = "svg" : (l === "mathml" || Bl(D)) && (l = "mathml"));
+                I && (_(P, I), l === "svg" || Gl(I) ? l = "svg" : (l === "mathml" || Bl(I)) && (l = "mathml"));
                 const M = (L, F) => {
                     b & 16 && d(h, L, F, o, a, l, u, s)
                 };
-                z ? M(t, k) : D && M(D, P)
+                z ? M(t, E) : I && M(I, P)
             } else {
                 n.el = e.el;
-                const E = n.anchor = e.anchor,
-                    k = n.target = e.target,
-                    D = n.targetAnchor = e.targetAnchor,
+                const k = n.anchor = e.anchor,
+                    E = n.target = e.target,
+                    I = n.targetAnchor = e.targetAnchor,
                     P = Tr(e.props),
-                    M = P ? t : k,
-                    L = P ? E : D;
-                if (l === "svg" || Gl(k) ? l = "svg" : (l === "mathml" || Bl(k)) && (l = "mathml"), S ? (f(e.dynamicChildren, S, M, o, a, l, u), Ja(e, n, !0)) : s || m(e, n, M, L, o, a, l, u, !1), z) P ? n.props && e.props && n.props.to !== e.props.to && (n.props.to = e.props.to) : eo(n, t, E, c, 1);
+                    M = P ? t : E,
+                    L = P ? k : I;
+                if (l === "svg" || Gl(E) ? l = "svg" : (l === "mathml" || Bl(E)) && (l = "mathml"), S ? (f(e.dynamicChildren, S, M, o, a, l, u), Ja(e, n, !0)) : s || m(e, n, M, L, o, a, l, u, !1), z) P ? n.props && e.props && n.props.to !== e.props.to && (n.props.to = e.props.to) : eo(n, t, k, c, 1);
                 else if ((n.props && n.props.to) !== (e.props && e.props.to)) {
                     const F = n.target = Qi(n.props, p);
                     F && eo(n, F, null, c, 0)
-                } else P && eo(n, k, D, c, 1)
+                } else P && eo(n, E, I, c, 1)
             }
-            Dc(n)
+            Ic(n)
         },
         remove(e, n, t, r, {
             um: o,
             o: {
                 remove: a
             }
         }, l) {
@@ -3096,21 +3096,21 @@
                 n.anchor = l(e);
                 let f = m;
                 for (; f;)
                     if (f = l(f), f && f.nodeType === 8 && f.data === "teleport anchor") {
                         n.targetAnchor = f, d._lpa = n.targetAnchor && l(n.targetAnchor);
                         break
                     } c(m, n, d, t, r, o, a)
-            } Dc(n)
+            } Ic(n)
     }
     return n.anchor && l(n.anchor)
 }
 const x1 = m_;
 
-function Dc(e) {
+function Ic(e) {
     const n = e.ctx;
     if (n && n.ut) {
         let t = e.children[0].el;
         for (; t && t !== e.targetAnchor;) t.nodeType === 1 && t.setAttribute("data-v-owner", n.uid), t = t.nextSibling;
         n.ut()
     }
 }
@@ -3208,22 +3208,22 @@
     }
     if (w_(e) && (e = e.__vccOpts), n) {
         n = __(n);
         let {
             class: u,
             style: s
         } = n;
-        u && !Me(u) && (n.class = La(u)), ye(s) && (oc(s) && !ee(s) && (s = De({}, s)), n.style = Da(s))
+        u && !Me(u) && (n.class = La(u)), ye(s) && (oc(s) && !ee(s) && (s = Ie({}, s)), n.style = Ia(s))
     }
-    const l = Me(e) ? 1 : kf(e) ? 128 : c_(e) ? 64 : ye(e) ? 4 : re(e) ? 2 : 0;
+    const l = Me(e) ? 1 : Ef(e) ? 128 : c_(e) ? 64 : ye(e) ? 4 : re(e) ? 2 : 0;
     return Rc(e, n, t, r, o, l, a, !0)
 }
 
 function __(e) {
-    return e ? oc(e) || Qo in e ? De({}, e) : e : null
+    return e ? oc(e) || Qo in e ? Ie({}, e) : e : null
 }
 
 function dt(e, n, t = !1) {
     const {
         props: r,
         ref: o,
         patchFlag: a,
@@ -3264,15 +3264,15 @@
     return ve(jr, null, e, n)
 }
 
 function N1(e = "", n = !1) {
     return n ? (Yo(), el(en, null, e)) : ve(en, null, e)
 }
 
-function kn(e) {
+function En(e) {
     return e == null || typeof e == "boolean" ? ve(en) : ee(e) ? ve(Fe, null, e.slice()) : typeof e == "object" ? tt(e) : ve(jr, null, String(e))
 }
 
 function tt(e) {
     return e.el === null && e.patchFlag !== -1 || e.memo ? e : dt(e)
 }
 
@@ -3302,28 +3302,28 @@
 
 function Nc(...e) {
     const n = {};
     for (let t = 0; t < e.length; t++) {
         const r = e[t];
         for (const o in r)
             if (o === "class") n.class !== r.class && (n.class = La([n.class, r.class]));
-            else if (o === "style") n.style = Da([n.style, r.style]);
+            else if (o === "style") n.style = Ia([n.style, r.style]);
         else if (Bo(o)) {
             const a = n[o],
                 l = r[o];
             l && a !== l && !(ee(a) && a.includes(l)) && (n[o] = a ? [].concat(a, l) : l)
         } else o !== "" && (n[o] = r[o])
     }
     return n
 }
 
-function In(e, n, t, r = null) {
+function Dn(e, n, t, r = null) {
     yn(e, n, 7, [t, r])
 }
-const z_ = Ec();
+const z_ = kc();
 let h_ = 0;
 
 function g_(e, n, t) {
     const r = e.type,
         o = (n ? n.appContext : e.appContext) || z_,
         a = {
             uid: h_++,
@@ -3435,15 +3435,15 @@
         setup: r
     } = t;
     if (r) {
         const o = e.setupContext = r.length > 1 ? T_(e) : null,
             a = Pt(e);
         Ct();
         const l = ut(r, e, 0, [e.props, o]);
-        if (It(), a(), Ca(l)) {
+        if (Dt(), a(), Ca(l)) {
             if (l.then(Ji, Ji), n) return l.then(u => {
                 ea(e, u, n)
             }).catch(u => {
                 Fr(u, e, 0)
             });
             e.asyncDep = l
         } else ea(e, l, n)
@@ -3463,29 +3463,29 @@
             if (o) {
                 const {
                     isCustomElement: a,
                     compilerOptions: l
                 } = e.appContext.config, {
                     delimiters: u,
                     compilerOptions: s
-                } = r, c = De(De({
+                } = r, c = Ie(Ie({
                     isCustomElement: a,
                     delimiters: u
                 }, l), s);
                 r.render = Fl(o, c)
             }
         }
         e.render = r.render || dn
     } {
         const o = Pt(e);
         Ct();
         try {
             Kf(e)
         } finally {
-            It(), o()
+            Dt(), o()
         }
     }
 }
 
 function y_(e) {
     return e.attrsProxy || (e.attrsProxy = new Proxy(e.attrs, {
         get(n, t) {
@@ -3529,34 +3529,34 @@
 }
 const ae = (e, n) => uf(e, n, Zo);
 
 function Ge(e, n, t) {
     const r = arguments.length;
     return r === 2 ? ye(n) && !ee(n) ? er(n) ? ve(e, null, [n]) : ve(e, n) : ve(e, null, n) : (r > 3 ? t = Array.prototype.slice.call(arguments, 2) : r === 3 && er(t) && (t = [t]), ve(e, n, t))
 }
-const E_ = "3.4.21";
+const k_ = "3.4.21";
 /**
  * @vue/runtime-dom v3.4.21
  * (c) 2018-present Yuxi (Evan) You and Vue contributors
  * @license MIT
  **/
-const k_ = "http://www.w3.org/2000/svg",
+const E_ = "http://www.w3.org/2000/svg",
     A_ = "http://www.w3.org/1998/Math/MathML",
     rt = typeof document < "u" ? document : null,
     Vl = rt && rt.createElement("template"),
     P_ = {
         insert: (e, n, t) => {
             n.insertBefore(e, t || null)
         },
         remove: e => {
             const n = e.parentNode;
             n && n.removeChild(e)
         },
         createElement: (e, n, t, r) => {
-            const o = n === "svg" ? rt.createElementNS(k_, e) : n === "mathml" ? rt.createElementNS(A_, e) : rt.createElement(e, t ? {
+            const o = n === "svg" ? rt.createElementNS(E_, e) : n === "mathml" ? rt.createElementNS(A_, e) : rt.createElement(e, t ? {
                 is: t
             } : void 0);
             return e === "select" && r && r.multiple != null && o.setAttribute("multiple", r.multiple), o
         },
         createText: e => rt.createTextNode(e),
         createComment: e => rt.createComment(e),
         setText: (e, n) => {
@@ -3609,15 +3609,15 @@
         appearFromClass: String,
         appearActiveClass: String,
         appearToClass: String,
         leaveFromClass: String,
         leaveActiveClass: String,
         leaveToClass: String
     },
-    M_ = Hc.props = De({}, bc, Fc),
+    M_ = Hc.props = Ie({}, bc, Fc),
     ht = (e, n = []) => {
         ee(e) ? e.forEach(t => t(...n)) : e && e(...n)
     },
     jl = e => e ? ee(e) ? e.some(n => n.length > 1) : e.length > 1 : !1;
 
 function Vc(e) {
     const n = {};
@@ -3637,35 +3637,35 @@
         leaveActiveClass: f = `${t}-leave-active`,
         leaveToClass: _ = `${t}-leave-to`
     } = e, p = C_(o), g = p && p[0], y = p && p[1], {
         onBeforeEnter: z,
         onEnter: b,
         onEnterCancelled: h,
         onLeave: S,
-        onLeaveCancelled: E,
-        onBeforeAppear: k = z,
-        onAppear: D = b,
+        onLeaveCancelled: k,
+        onBeforeAppear: E = z,
+        onAppear: I = b,
         onAppearCancelled: P = h
     } = n, M = (O, V, Z) => {
         Jn(O, V ? d : u), Jn(O, V ? c : l), Z && Z()
     }, L = (O, V) => {
         O._isLeaving = !1, Jn(O, m), Jn(O, _), Jn(O, f), V && V()
     }, F = O => (V, Z) => {
-        const oe = O ? D : b,
+        const oe = O ? I : b,
             ie = () => M(V, O, Z);
         ht(oe, [V, ie]), Ul(() => {
             Jn(V, O ? s : a), Hn(V, O ? d : u), jl(oe) || ql(V, r, g, ie)
         })
     };
-    return De(n, {
+    return Ie(n, {
         onBeforeEnter(O) {
             ht(z, [O]), Hn(O, a), Hn(O, l)
         },
         onBeforeAppear(O) {
-            ht(k, [O]), Hn(O, s), Hn(O, c)
+            ht(E, [O]), Hn(O, s), Hn(O, c)
         },
         onEnter: F(!1),
         onAppear: F(!0),
         onLeave(O, V) {
             O._isLeaving = !0;
             const Z = () => L(O, V);
             Hn(O, m), Uc(), Hn(O, f), Ul(() => {
@@ -3675,15 +3675,15 @@
         onEnterCancelled(O) {
             M(O, !1), ht(h, [O])
         },
         onAppearCancelled(O) {
             M(O, !0), ht(P, [O])
         },
         onLeaveCancelled(O) {
-            L(O), ht(E, [O])
+            L(O), ht(k, [O])
         }
     })
 }
 
 function C_(e) {
     if (e == null) return null;
     if (ye(e)) return [hi(e.enter), hi(e.leave)];
@@ -3708,18 +3708,18 @@
 }
 
 function Ul(e) {
     requestAnimationFrame(() => {
         requestAnimationFrame(e)
     })
 }
-let I_ = 0;
+let D_ = 0;
 
 function ql(e, n, t, r) {
-    const o = e._endId = ++I_,
+    const o = e._endId = ++D_,
         a = () => {
             o === e._endId && r()
         };
     if (t) return setTimeout(a, t);
     const {
         type: l,
         timeout: u,
@@ -3770,15 +3770,15 @@
     return e === "auto" ? 0 : Number(e.slice(0, -1).replace(",", ".")) * 1e3
 }
 
 function Uc() {
     return document.body.offsetHeight
 }
 
-function D_(e, n, t) {
+function I_(e, n, t) {
     const r = e[nr];
     r && (n = (n ? [n, ...r] : [...r]).join(" ")), n == null ? e.removeAttribute("class") : t ? e.setAttribute("class", n) : e.className = n
 }
 const wo = Symbol("_vod"),
     qc = Symbol("_vsh"),
     G1 = {
         beforeMount(e, {
@@ -3949,33 +3949,33 @@
             t.call(e), e._stopped = !0
         }, n.map(r => o => !o._stopped && r && r(o))
     } else return n
 }
 const Jl = e => e.charCodeAt(0) === 111 && e.charCodeAt(1) === 110 && e.charCodeAt(2) > 96 && e.charCodeAt(2) < 123,
     $_ = (e, n, t, r, o, a, l, u, s) => {
         const c = o === "svg";
-        n === "class" ? D_(e, r, c) : n === "style" ? x_(e, t, r) : Bo(n) ? Pa(n) || F_(e, n, t, r, l) : (n[0] === "." ? (n = n.slice(1), !0) : n[0] === "^" ? (n = n.slice(1), !1) : K_(e, n, r, c)) ? G_(e, n, r, a, l, u, s) : (n === "true-value" ? e._trueValue = r : n === "false-value" && (e._falseValue = r), N_(e, n, r, c))
+        n === "class" ? I_(e, r, c) : n === "style" ? x_(e, t, r) : Bo(n) ? Pa(n) || F_(e, n, t, r, l) : (n[0] === "." ? (n = n.slice(1), !0) : n[0] === "^" ? (n = n.slice(1), !1) : K_(e, n, r, c)) ? G_(e, n, r, a, l, u, s) : (n === "true-value" ? e._trueValue = r : n === "false-value" && (e._falseValue = r), N_(e, n, r, c))
     };
 
 function K_(e, n, t, r) {
     if (r) return !!(n === "innerHTML" || n === "textContent" || n in e && Jl(n) && re(t));
     if (n === "spellcheck" || n === "draggable" || n === "translate" || n === "form" || n === "list" && e.tagName === "INPUT" || n === "type" && e.tagName === "TEXTAREA") return !1;
     if (n === "width" || n === "height") {
         const o = e.tagName;
         if (o === "IMG" || o === "VIDEO" || o === "CANVAS" || o === "SOURCE") return !1
     }
     return Jl(n) && Me(t) ? !1 : n in e
 }
 const Wc = new WeakMap,
     $c = new WeakMap,
-    Eo = Symbol("_moveCb"),
+    ko = Symbol("_moveCb"),
     es = Symbol("_enterCb"),
     Kc = {
         name: "TransitionGroup",
-        props: De({}, M_, {
+        props: Ie({}, M_, {
             tag: String,
             moveClass: String
         }),
         setup(e, {
             slots: n
         }) {
             const t = Lt(),
@@ -3987,44 +3987,44 @@
                 if (!J_(o[0].el, t.vnode.el, l)) return;
                 o.forEach(Y_), o.forEach(Q_);
                 const u = o.filter(Z_);
                 Uc(), u.forEach(s => {
                     const c = s.el,
                         d = c.style;
                     Hn(c, l), d.transform = d.webkitTransform = d.transitionDuration = "";
-                    const m = c[Eo] = f => {
-                        f && f.target !== c || (!f || /transform$/.test(f.propertyName)) && (c.removeEventListener("transitionend", m), c[Eo] = null, Jn(c, l))
+                    const m = c[ko] = f => {
+                        f && f.target !== c || (!f || /transform$/.test(f.propertyName)) && (c.removeEventListener("transitionend", m), c[ko] = null, Jn(c, l))
                     };
                     c.addEventListener("transitionend", m)
                 })
             }), () => {
                 const l = ce(e),
                     u = Vc(l);
                 let s = l.tag || Fe;
                 o = a, a = n.default ? Xa(n.default()) : [];
                 for (let c = 0; c < a.length; c++) {
                     const d = a[c];
-                    d.key != null && Dr(d, Ir(d, u, r, t))
+                    d.key != null && Ir(d, Dr(d, u, r, t))
                 }
                 if (o)
                     for (let c = 0; c < o.length; c++) {
                         const d = o[c];
-                        Dr(d, Ir(d, u, r, t)), Wc.set(d, d.el.getBoundingClientRect())
+                        Ir(d, Dr(d, u, r, t)), Wc.set(d, d.el.getBoundingClientRect())
                     }
                 return ve(s, null, a)
             }
         }
     },
     X_ = e => delete e.mode;
 Kc.props;
 const B1 = Kc;
 
 function Y_(e) {
     const n = e.el;
-    n[Eo] && n[Eo](), n[es] && n[es]()
+    n[ko] && n[ko](), n[es] && n[es]()
 }
 
 function Q_(e) {
     $c.set(e, e.el.getBoundingClientRect())
 }
 
 function Z_(e) {
@@ -4072,15 +4072,15 @@
             for (let l = 0; l < n.length; l++) {
                 const u = np[n[l]];
                 if (u && u(o, n)) return
             }
             return e(o, ...a)
         })
     },
-    tp = De({
+    tp = Ie({
         patchProp: $_
     }, P_);
 let ns;
 
 function rp() {
     return ns || (ns = a_(tp))
 }
@@ -4376,33 +4376,33 @@
     onReconnect(n, t) {
         return this.addListener(be.reconnect, n, t), this
     }
     build() {
         return new sp(this._url, this._protocols, this._options)
     }
     addListener(n, t, r) {
-        var o, a, l, u, s, c, d, m, f, _, p, g, y, z, b, h, S, E, k, D, P;
+        var o, a, l, u, s, c, d, m, f, _, p, g, y, z, b, h, S, k, E, I, P;
         return this._options = Object.assign(Object.assign({}, this._options), {
             listeners: {
                 open: (l = (a = (o = this._options) === null || o === void 0 ? void 0 : o.listeners) === null || a === void 0 ? void 0 : a.open) !== null && l !== void 0 ? l : [],
                 close: (c = (s = (u = this._options) === null || u === void 0 ? void 0 : u.listeners) === null || s === void 0 ? void 0 : s.close) !== null && c !== void 0 ? c : [],
                 error: (f = (m = (d = this._options) === null || d === void 0 ? void 0 : d.listeners) === null || m === void 0 ? void 0 : m.error) !== null && f !== void 0 ? f : [],
                 message: (g = (p = (_ = this._options) === null || _ === void 0 ? void 0 : _.listeners) === null || p === void 0 ? void 0 : p.message) !== null && g !== void 0 ? g : [],
                 retry: (b = (z = (y = this._options) === null || y === void 0 ? void 0 : y.listeners) === null || z === void 0 ? void 0 : z.retry) !== null && b !== void 0 ? b : [],
-                reconnect: (E = (S = (h = this._options) === null || h === void 0 ? void 0 : h.listeners) === null || S === void 0 ? void 0 : S.reconnect) !== null && E !== void 0 ? E : [],
-                [n]: [...(P = (D = (k = this._options) === null || k === void 0 ? void 0 : k.listeners) === null || D === void 0 ? void 0 : D[n]) !== null && P !== void 0 ? P : [], {
+                reconnect: (k = (S = (h = this._options) === null || h === void 0 ? void 0 : h.listeners) === null || S === void 0 ? void 0 : S.reconnect) !== null && k !== void 0 ? k : [],
+                [n]: [...(P = (I = (E = this._options) === null || E === void 0 ? void 0 : E.listeners) === null || I === void 0 ? void 0 : I[n]) !== null && P !== void 0 ? P : [], {
                     listener: t,
                     options: r
                 }]
             }
         }), this
     }
 }
 const cp = 1,
-    ko = 2,
+    Eo = 2,
     vi = 3,
     tl = 4,
     mp = 5,
     dp = 6;
 
 function fp(e) {
     return {
@@ -4481,29 +4481,29 @@
     const r = n.wsUrl;
 
     function o(a, l, u) {
         const s = new WebSocket(r);
         let c = !1;
         const d = () => {
                 if (s.removeEventListener("close", d), c) {
-                    u(ko);
+                    u(Eo);
                     return
                 }
                 if (a === 0) {
                     u(cp);
                     return
                 }
                 const _ = a === -1 ? -1 : a - 1;
                 setTimeout(() => o(_, l, u), 1e3)
             },
             m = async _ => {
                 try {
                     n.expired && await (t || n.refreshAccessToken()), s.send(JSON.stringify(fp(n.accessToken)))
                 } catch (p) {
-                    c = p === ko, s.close()
+                    c = p === Eo, s.close()
                 }
             }, f = async _ => {
                 const p = JSON.parse(_.data);
                 switch (p.type) {
                     case vp:
                         c = !0, s.close();
                         break;
@@ -4550,15 +4550,15 @@
                             this._setSocket(u)
                         } catch (u) {
                             if (this._queuedMessages) {
                                 const s = this._queuedMessages;
                                 this._queuedMessages = void 0;
                                 for (const c of s) c.reject && c.reject(vi)
                             }
-                            u === ko ? this.fireEvent("reconnect-error", u) : a(l + 1)
+                            u === Eo ? this.fireEvent("reconnect-error", u) : a(l + 1)
                         }
                     }, Math.min(l, 5) * 1e3)
                 };
             this.suspendReconnectPromise && (await this.suspendReconnectPromise, this.suspendReconnectPromise = void 0, this._queuedMessages = []), a(0)
         }, this.options = t, this.commandId = 2, this.commands = new Map, this.eventListeners = new Map, this.closeRequested = !1, this._setSocket(n)
     }
     get connected() {
@@ -4675,17 +4675,17 @@
         }), () => o.unsubscribe()
     }
     _genCmdId() {
         return ++this.commandId
     }
 }
 const wp = () => `${location.protocol}//${location.host}/`,
-    Ep = e => e * 1e3 + Date.now();
+    kp = e => e * 1e3 + Date.now();
 
-function kp() {
+function Ep() {
     const {
         protocol: e,
         host: n,
         pathname: t,
         search: r
     } = location;
     return `${e}//${n}${t}${r}`
@@ -4710,17 +4710,17 @@
         o.append(u, t[u])
     });
     const a = await fetch(`${e}/auth/token`, {
         method: "POST",
         credentials: "same-origin",
         body: o
     });
-    if (!a.ok) throw a.status === 400 || a.status === 403 ? ko : new Error("Unable to fetch tokens");
+    if (!a.ok) throw a.status === 400 || a.status === 403 ? Eo : new Error("Unable to fetch tokens");
     const l = await a.json();
-    return l.hassUrl = e, l.clientId = n, l.expires = Ep(l.expires_in), l
+    return l.hassUrl = e, l.clientId = n, l.expires = kp(l.expires_in), l
 }
 
 function rs(e, n, t) {
     return Xc(e, n, {
         code: t,
         grant_type: "authorization_code"
     })
@@ -4729,15 +4729,15 @@
 function Mp(e) {
     return btoa(JSON.stringify(e))
 }
 
 function Cp(e) {
     return JSON.parse(atob(e))
 }
-class Ip {
+class Dp {
     constructor(n, t) {
         this.data = n, this._saveTokens = t
     }
     get wsUrl() {
         return `ws${this.data.hassUrl.substr(4)}/api/websocket`
     }
     get accessToken() {
@@ -4773,38 +4773,38 @@
         const a = gp(location.search.substr(1));
         if ("auth_callback" in a) {
             const l = Cp(a.state);
             if (o && (l.hassUrl !== t || l.clientId !== r)) throw dp;
             n = await rs(l.hassUrl, l.clientId, a.code), e.saveTokens && e.saveTokens(n)
         }
     }
-    if (!n && e.loadTokens && (n = await e.loadTokens()), n) return new Ip(n, e.saveTokens);
+    if (!n && e.loadTokens && (n = await e.loadTokens()), n) return new Dp(n, e.saveTokens);
     if (t === void 0) throw tl;
-    return Pp(t, r, e.redirectUrl || kp(), Mp({
+    return Pp(t, r, e.redirectUrl || Ep(), Mp({
         hassUrl: t,
         clientId: r
     })), new Promise(() => {})
 }
-async function Dp(e) {
+async function Ip(e) {
     const n = Object.assign({
             setupRetry: 0,
             createSocket: Tp
         }, e),
         t = await n.createSocket(n);
     return new Sp(t, n)
 }
 const F1 = "this_value_is_encrypted";
 var na = (e => (e.ARTIST = "artist", e.ALBUM = "album", e.TRACK = "track", e.PLAYLIST = "playlist", e.RADIO = "radio", e.FOLDER = "folder", e.UNKNOWN = "unknown", e))(na || {}),
-    Lp = (e => (e.THUMB = "thumb", e.WIDE_THUMB = "wide_thumb", e.FANART = "fanart", e.LOGO = "logo", e.CLEARART = "clearart", e.BANNER = "banner", e.CUTOUT = "cutout", e.BACK = "back", e.CDART = "cdart", e.EMBEDDED_THUMB = "embedded_thumb", e.OTHER = "other", e))(Lp || {}),
+    Lp = (e => (e.THUMB = "thumb", e.LANDSCAPE = "landscape", e.FANART = "fanart", e.LOGO = "logo", e.CLEARART = "clearart", e.BANNER = "banner", e.CUTOUT = "cutout", e.BACK = "back", e.CDART = "cdart", e.EMBEDDED_THUMB = "embedded_thumb", e.OTHER = "other", e))(Lp || {}),
     Op = (e => (e.OGG = "ogg", e.FLAC = "flac", e.MP3 = "mp3", e.AAC = "aac", e.MPEG = "mpeg", e.ALAC = "alac", e.WAV = "wav", e.AIFF = "aiff", e.WMA = "wma", e.M4B = "m4b", e.M4A = "m4a", e.DSF = "dsf", e.WAVPACK = "wv", e.PCM_S16LE = "s16le", e.PCM_S24LE = "s24le", e.PCM_S32LE = "s32le", e.PCM_F32LE = "f32le", e.PCM_F64LE = "f64le", e.MPEG_DASH = "dash", e.UNKNOWN = "?", e))(Op || {}),
     xp = (e => (e.PLAY = "play", e.REPLACE = "replace", e.NEXT = "next", e.REPLACE_NEXT = "replace_next", e.ADD = "add", e))(xp || {}),
     Bt = (e => (e.OFF = "off", e.ONE = "one", e.ALL = "all", e))(Bt || {}),
     Rp = (e => (e.IDLE = "idle", e.PAUSED = "paused", e.PLAYING = "playing", e))(Rp || {}),
     ta = (e => (e.PLAYER = "player", e.GROUP = "group", e.SYNC_GROUP = "sync_group", e))(ta || {}),
-    En = (e => (e.PLAYER_ADDED = "player_added", e.PLAYER_UPDATED = "player_updated", e.PLAYER_REMOVED = "player_removed", e.PLAYER_SETTINGS_UPDATED = "player_settings_updated", e.QUEUE_ADDED = "queue_added", e.QUEUE_UPDATED = "queue_updated", e.QUEUE_ITEMS_UPDATED = "queue_items_updated", e.QUEUE_TIME_UPDATED = "queue_time_updated", e.QUEUE_SETTINGS_UPDATED = "queue_settings_updated", e.SHUTDOWN = "application_shutdown", e.MEDIA_ITEM_ADDED = "media_item_added", e.MEDIA_ITEM_UPDATED = "media_item_updated", e.MEDIA_ITEM_DELETED = "media_item_deleted", e.PROVIDERS_UPDATED = "providers_updated", e.PLAYER_CONFIG_UPDATED = "player_config_updated", e.SYNC_TASKS_UPDATED = "sync_tasks_updated", e.AUTH_SESSION = "auth_session", e.ALL = "*", e))(En || {}),
+    kn = (e => (e.PLAYER_ADDED = "player_added", e.PLAYER_UPDATED = "player_updated", e.PLAYER_REMOVED = "player_removed", e.PLAYER_SETTINGS_UPDATED = "player_settings_updated", e.QUEUE_ADDED = "queue_added", e.QUEUE_UPDATED = "queue_updated", e.QUEUE_ITEMS_UPDATED = "queue_items_updated", e.QUEUE_TIME_UPDATED = "queue_time_updated", e.QUEUE_SETTINGS_UPDATED = "queue_settings_updated", e.SHUTDOWN = "application_shutdown", e.MEDIA_ITEM_ADDED = "media_item_added", e.MEDIA_ITEM_UPDATED = "media_item_updated", e.MEDIA_ITEM_DELETED = "media_item_deleted", e.PROVIDERS_UPDATED = "providers_updated", e.PLAYER_CONFIG_UPDATED = "player_config_updated", e.SYNC_TASKS_UPDATED = "sync_tasks_updated", e.AUTH_SESSION = "auth_session", e.ALL = "*", e))(kn || {}),
     Np = (e => (e.BROWSE = "browse", e.SEARCH = "search", e.RECOMMENDATIONS = "recommendations", e.LIBRARY_ARTISTS = "library_artists", e.LIBRARY_ALBUMS = "library_albums", e.LIBRARY_TRACKS = "library_tracks", e.LIBRARY_PLAYLISTS = "library_playlists", e.LIBRARY_RADIOS = "library_radios", e.ARTIST_ALBUMS = "artist_albums", e.ARTIST_TOPTRACKS = "artist_toptracks", e.LIBRARY_ARTISTS_EDIT = "library_artists_edit", e.LIBRARY_ALBUMS_EDIT = "library_albums_edit", e.LIBRARY_TRACKS_EDIT = "library_tracks_edit", e.LIBRARY_PLAYLISTS_EDIT = "library_playlists_edit", e.LIBRARY_RADIOS_EDIT = "library_radios_edit", e.SIMILAR_TRACKS = "similar_tracks", e.PLAYLIST_TRACKS_EDIT = "playlist_tracks_edit", e.PLAYLIST_CREATE = "playlist_create", e.PLAYER_GROUP_CREATE = "player_group_create", e.SYNC_PLAYERS = "sync_players", e.ARTIST_METADATA = "artist_metadata", e.ALBUM_METADATA = "album_metadata", e.TRACK_METADATA = "track_metadata", e))(Np || {}),
     Gp = (e => (e.MUSIC = "music", e.PLAYER = "player", e.METADATA = "metadata", e.PLUGIN = "plugin", e))(Gp || {}),
     Bp = (e => (e.BOOLEAN = "boolean", e.STRING = "string", e.SECURE_STRING = "secure_string", e.INTEGER = "integer", e.FLOAT = "float", e.LABEL = "label", e.DIVIDER = "divider", e.ACTION = "action", e.ICON = "icon", e.ALERT = "alert", e))(Bp || {}),
     Hp = (e => (e[e.DISCONNECTED = 0] = "DISCONNECTED", e[e.CONNECTING = 1] = "CONNECTING", e[e.CONNECTED = 2] = "CONNECTED", e))(Hp || {});
 class Fp {
     constructor() {
         Ye(this, "ws");
@@ -5367,43 +5367,43 @@
                 if (t.hassUrl = prompt("Please enter the URL to Home Assistant", "http://homeassistant.local:8123") || "", !t.hassUrl) return;
                 n = await os(t)
             } else {
                 alert(`Unknown error: ${o}`);
                 return
             }
         }
-        const r = await Dp({
+        const r = await Ip({
             auth: n
         });
         return r.addEventListener("ready", () => window.history.back()), r
     }
     handleEventMessage(n) {
-        if (n.event == En.QUEUE_ADDED) {
+        if (n.event == kn.QUEUE_ADDED) {
             const t = n.data;
             this.queues[t.queue_id] = t
-        } else if (n.event == En.QUEUE_UPDATED) {
+        } else if (n.event == kn.QUEUE_UPDATED) {
             const t = n.data;
             t.queue_id in this.queues ? Object.assign(this.queues[t.queue_id], t) : this.queues[t.queue_id] = t
-        } else if (n.event == En.QUEUE_TIME_UPDATED) {
+        } else if (n.event == kn.QUEUE_TIME_UPDATED) {
             const t = n.object_id;
             t in this.queues && (this.queues[t].elapsed_time = n.data)
-        } else if (n.event == En.PLAYER_ADDED) {
+        } else if (n.event == kn.PLAYER_ADDED) {
             const t = n.data;
             this.players[t.player_id] = t
-        } else if (n.event == En.PLAYER_UPDATED) {
+        } else if (n.event == kn.PLAYER_UPDATED) {
             const t = n.data;
             t.player_id in this.players ? Object.assign(this.players[t.player_id], t) : this.players[t.player_id] = t
-        } else if (n.event == En.PLAYER_REMOVED) delete this.players[n.object_id];
-        else if (n.event == En.SYNC_TASKS_UPDATED) this.syncTasks.value = n.data;
-        else if (n.event == En.PROVIDERS_UPDATED) {
+        } else if (n.event == kn.PLAYER_REMOVED) delete this.players[n.object_id];
+        else if (n.event == kn.SYNC_TASKS_UPDATED) this.syncTasks.value = n.data;
+        else if (n.event == kn.PROVIDERS_UPDATED) {
             const t = {};
             for (const r of n.data) t[r.instance_id] = r;
             this.providers = t
         }
-        n.event !== En.QUEUE_TIME_UPDATED && console.log("[event]", n), this.signalEvent(n)
+        n.event !== kn.QUEUE_TIME_UPDATED && console.log("[event]", n), this.signalEvent(n)
     }
     handleResultMessage(n) {
         const t = this.commands.get(n.message_id);
         t && (console.log("[resultMessage]", n), this.commands.delete(n.message_id), this.fetchesInProgress.value = this.fetchesInProgress.value.filter(r => r != n.message_id), "error_code" in n ? (n = n, t.reject(n.details || n.error_code)) : (n = n, t.resolve(n.result)))
     }
     handleChunkedResultMessage(n) {
         const t = this.commands.get(n.message_id);
@@ -5412,15 +5412,15 @@
             o = "error_code" in n;
         console.log("[chunkedResultMessage]", n), (o || r) && (this.commands.delete(n.message_id), this.fetchesInProgress.value = this.fetchesInProgress.value.filter(a => a != n.message_id)), "error_code" in n ? (n = n, t.reject(n.details || n.error_code)) : (t.chunkCallback && t.chunkCallback(n.result), r && t.resolve([]))
     }
     handleServerInfoMessage(n) {
         console.log("[serverInfo]", n), this.state.value = 2, this.serverInfo.value = n, this._fetchState()
     }
     signalEvent(n) {
-        for (const t of this.eventCallbacks)(t[0] === En.ALL || t[0] === n.event) && t[1](n)
+        for (const t of this.eventCallbacks)(t[0] === kn.ALL || t[0] === n.event) && t[1](n)
     }
     getData(n, t, r) {
         const o = this._genCmdId();
         return new Promise((a, l) => {
             this.commands.set(o, {
                 resolve: a,
                 reject: l,
@@ -5702,21 +5702,21 @@
     return r
 }
 
 function ez(e) {
     return e.map(n => n.type === Fe ? ez(n.children) : n).flat()
 }
 
-function kt() {
+function Et() {
     let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : "";
-    if (kt.cache.has(e)) return kt.cache.get(e);
+    if (Et.cache.has(e)) return Et.cache.get(e);
     const n = e.replace(/[^a-z]/gi, "-").replace(/\B([A-Z])/g, "-$1").toLowerCase();
-    return kt.cache.set(e, n), n
+    return Et.cache.set(e, n), n
 }
-kt.cache = new Map;
+Et.cache = new Map;
 
 function Ti(e, n) {
     if (!n || typeof n != "object") return [];
     if (Array.isArray(n)) return n.map(t => Ti(e, t)).flat(1);
     if (Array.isArray(n.children)) return n.children.map(t => Ti(e, t)).flat(1);
     if (n.component) {
         if (Object.getOwnPropertySymbols(n.component.provides).includes(e)) return [n.component];
@@ -6071,20 +6071,20 @@
 }
 
 function wz(e, n) {
     const t = em(rl(e));
     return t[0] = t[0] - n * 10, tm(nm(t))
 }
 
-function Ez(e) {
+function kz(e) {
     const n = jn(e);
     return rl(n)[1]
 }
 
-function kz(e) {
+function Ez(e) {
     const n = Math.abs(hs(jn(0), jn(e)));
     return Math.abs(hs(jn(16777215), jn(e))) > Math.min(n, 50) ? "#fff" : "#000"
 }
 
 function ei(e, n) {
     return t => Object.keys(e).reduce((r, o) => {
         const l = typeof e[o] == "object" && e[o] != null && !Array.isArray(e[o]) ? e[o] : {
@@ -6131,15 +6131,15 @@
             return c.prev ? _n(c.prev, c) : c
         });
     return Wn(tr, o), o
 }
 
 function Pz(e, n) {
     var t, r;
-    return typeof((t = e.props) == null ? void 0 : t[n]) < "u" || typeof((r = e.props) == null ? void 0 : r[kt(n)]) < "u"
+    return typeof((t = e.props) == null ? void 0 : t[n]) < "u" || typeof((r = e.props) == null ? void 0 : r[Et(n)]) < "u"
 }
 
 function Mz() {
     let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
         n = arguments.length > 1 ? arguments[1] : void 0,
         t = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : ol();
     const r = Ot("useDefaults");
@@ -6163,15 +6163,15 @@
                 return d.startsWith(d[0].toUpperCase())
             });
             l.value = s.length ? Object.fromEntries(s) : void 0
         } else l.value = void 0
     });
 
     function u() {
-        const s = Dz(tr, r);
+        const s = Iz(tr, r);
         Wn(tr, ae(() => l.value ? _n((s == null ? void 0 : s.value) ?? {}, l.value) : s == null ? void 0 : s.value))
     }
     return {
         props: a,
         provideSubDefaults: u
     }
 }
@@ -6194,27 +6194,27 @@
         }
     }
     return e
 }
 
 function Cz() {
     let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : !0;
-    return n => (e ? Ur : Dt)(n)
+    return n => (e ? Ur : It)(n)
 }
 
 function Ot(e, n) {
     const t = Lt();
     if (!t) throw new Error(`[Vuetify] ${e} ${n||"must be called from inside a setup function"}`);
     return t
 }
 
-function Iz() {
+function Dz() {
     let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : "composables";
     const n = Ot(e).type;
-    return kt((n == null ? void 0 : n.aliasName) || (n == null ? void 0 : n.name))
+    return Et((n == null ? void 0 : n.aliasName) || (n == null ? void 0 : n.name))
 }
 let om = 0,
     po = new WeakMap;
 
 function im() {
     const e = Ot("getUid");
     if (po.has(e)) return po.get(e);
@@ -6223,28 +6223,28 @@
         return po.set(e, n), n
     }
 }
 im.reset = () => {
     om = 0, po = new WeakMap
 };
 
-function Dz(e) {
+function Iz(e) {
     let n = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : Ot("injectSelf");
     const {
         provides: t
     } = n;
     if (t && e in t) return t[e]
 }
 
 function Lz(e, n, t) {
     let r = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : m => m,
         o = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : m => m;
     const a = Ot("useProxiedModel"),
         l = he(e[n] !== void 0 ? e[n] : t),
-        u = kt(n),
+        u = Et(n),
         c = ae(u !== n ? () => {
             var m, f, _, p;
             return e[n], !!(((m = a.vnode.props) != null && m.hasOwnProperty(n) || (f = a.vnode.props) != null && f.hasOwnProperty(u)) && ((_ = a.vnode.props) != null && _.hasOwnProperty(`onUpdate:${n}`) || (p = a.vnode.props) != null && p.hasOwnProperty(`onUpdate:${u}`)))
         } : () => {
             var m, f;
             return e[n], !!((m = a.vnode.props) != null && m.hasOwnProperty(n) && ((f = a.vnode.props) != null && f.hasOwnProperty(`onUpdate:${n}`)))
         });
@@ -7166,31 +7166,31 @@
     }) : e.adapter);
     return Je(n.current, r => {
         t.locale = e.locale[r] ?? r ?? t.locale
     }), t
 }
 const _T = ["sm", "md", "lg", "xl", "xxl"],
     aa = Symbol.for("vuetify:display"),
-    Es = {
+    ks = {
         mobileBreakpoint: "lg",
         thresholds: {
             xs: 0,
             sm: 600,
             md: 960,
             lg: 1280,
             xl: 1920,
             xxl: 2560
         }
     },
-    Eh = function() {
-        let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : Es;
-        return _n(Es, e)
+    kh = function() {
+        let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : ks;
+        return _n(ks, e)
     };
 
-function ks(e) {
+function Es(e) {
     return fn && !e ? window.innerWidth : typeof e == "object" && e.clientWidth || 0
 }
 
 function As(e) {
     return fn && !e ? window.innerHeight : typeof e == "object" && e.clientHeight || 0
 }
 
@@ -7224,22 +7224,22 @@
         mac: f,
         linux: _,
         touch: jp,
         ssr: n === "ssr"
     }
 }
 
-function kh(e, n) {
+function Eh(e, n) {
     const {
         thresholds: t,
         mobileBreakpoint: r
-    } = Eh(e), o = st(As(n)), a = st(Ps(n)), l = on({}), u = st(ks(n));
+    } = kh(e), o = st(As(n)), a = st(Ps(n)), l = on({}), u = st(Es(n));
 
     function s() {
-        o.value = As(), u.value = ks()
+        o.value = As(), u.value = Es()
     }
 
     function c() {
         s(), a.value = Ps()
     }
     return qo(() => {
         const d = u.value < t.sm,
@@ -7262,15 +7262,15 @@
 }
 const pT = ei({
     mobileBreakpoint: [Number, String]
 }, "display");
 
 function zT() {
     let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
-        n = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : Iz();
+        n = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : Dz();
     const t = He(aa);
     if (!t) throw new Error("Could not find Vuetify display injection");
     const r = ae(() => {
             if (!e.mobileBreakpoint) return t.mobile.value;
             const a = typeof e.mobileBreakpoint == "number" ? e.mobileBreakpoint : t.thresholds.value[e.mobileBreakpoint];
             return t.width.value < a
         }),
@@ -7416,15 +7416,15 @@
                     d: r
                 }, null)) : ve("path", {
                     d: e.icon
                 }, null)])]
             })
         }
     }),
-    Ih = Ur({
+    Dh = Ur({
         name: "VLigatureIcon",
         props: ni(),
         setup(e) {
             return () => ve(e.tag, null, {
                 default: () => [e.icon]
             })
         }
@@ -7435,27 +7435,27 @@
         setup(e) {
             return () => ve(e.tag, {
                 class: e.icon
             }, null)
         }
     });
 
-function Dh() {
+function Ih() {
     return {
         svg: {
             component: _m
         },
         class: {
             component: pm
         }
     }
 }
 
 function Lh(e) {
-    const n = Dh(),
+    const n = Ih(),
         t = (e == null ? void 0 : e.defaultSet) ?? "mdi";
     return t === "mdi" && !n.mdi && (n.mdi = fm), _n({
         defaultSet: t,
         sets: n,
         aliases: {
             ...dm,
             vuetify: ["M8.2241 14.2009L12 21L22 3H14.4459L8.2241 14.2009Z", ["M7.26303 12.4733L7.00113 12L2 3H12.5261C12.5261 3 12.5261 3 12.5261 3L7.26303 12.4733Z", .6]],
@@ -7625,25 +7625,25 @@
                                 for (const b of Zc(n.variations[y], 1)) _.colors[`${p}-${y}-${b}`] = vz(z(jn(g), b))
                             }
                     }
                 for (const p of Object.keys(_.colors)) {
                     if (/^on-[a-z]/.test(p) || _.colors[`on-${p}`]) continue;
                     const g = `on-${p}`,
                         y = jn(_.colors[p]);
-                    _.colors[g] = kz(y)
+                    _.colors[g] = Ez(y)
                 }
             }
             return d
         }),
         a = ae(() => o.value[t.value]),
         l = ae(() => {
             var p;
             const d = [];
-            (p = a.value) != null && p.dark && bt(d, ":root", ["color-scheme: dark"]), bt(d, ":root", Is(a.value));
-            for (const [g, y] of Object.entries(o.value)) bt(d, `.v-theme--${g}`, [`color-scheme: ${y.dark?"dark":"normal"}`, ...Is(y)]);
+            (p = a.value) != null && p.dark && bt(d, ":root", ["color-scheme: dark"]), bt(d, ":root", Ds(a.value));
+            for (const [g, y] of Object.entries(o.value)) bt(d, `.v-theme--${g}`, [`color-scheme: ${y.dark?"dark":"normal"}`, ...Ds(y)]);
             const m = [],
                 f = [],
                 _ = new Set(Object.values(o.value).flatMap(g => Object.keys(g.colors)));
             for (const g of _) /^on-[a-z]/.test(g) ? bt(f, `.${g}`, [`color: rgb(var(--v-theme-${g})) !important`]) : (bt(m, `.bg-${g}`, [`--v-theme-overlay-multiplier: var(--v-theme-${g}-overlay-multiplier)`, `background-color: rgb(var(--v-theme-${g})) !important`, `color: rgb(var(--v-theme-on-${g})) !important`]), bt(f, `.text-${g}`, [`color: rgb(var(--v-theme-${g})) !important`]), bt(f, `.border-${g}`, [`--v-border-color: var(--v-theme-${g})`]));
             return d.push(...m, ...f), d.map((g, y) => y === 0 ? g : `    ${g}`).join("")
         });
 
@@ -7724,21 +7724,21 @@
 function bt(e, n, t) {
     e.push(`${n} {
 `, ...t.map(r => `  ${r};
 `), `}
 `)
 }
 
-function Is(e) {
+function Ds(e) {
     const n = e.dark ? 2 : 1,
         t = e.dark ? 1 : 2,
         r = [];
     for (const [o, a] of Object.entries(e.colors)) {
         const l = jn(a);
-        r.push(`--v-theme-${o}: ${l.r},${l.g},${l.b}`), o.startsWith("on-") || r.push(`--v-theme-${o}-overlay-multiplier: ${Ez(a)>.18?n:t}`)
+        r.push(`--v-theme-${o}: ${l.r},${l.g},${l.b}`), o.startsWith("on-") || r.push(`--v-theme-${o}-overlay-multiplier: ${kz(a)>.18?n:t}`)
     }
     for (const [o, a] of Object.entries(e.variables)) {
         const l = typeof a == "string" && a.startsWith("#") ? jn(a) : void 0,
             u = l ? `${l.r}, ${l.g}, ${l.b}` : void 0;
         r.push(`--v-${o}: ${u??a}`)
     }
     return r
@@ -7749,15 +7749,15 @@
     const {
         blueprint: n,
         ...t
     } = e, r = _n(n, t), {
         aliases: o = {},
         components: a = {},
         directives: l = {}
-    } = r, u = Az(r.defaults), s = kh(r.display, r.ssr), c = xh(r.theme), d = Lh(r.icons), m = Nz(r.locale), f = Sh(r.date, m), _ = Mh(r.goTo, m);
+    } = r, u = Az(r.defaults), s = Eh(r.display, r.ssr), c = xh(r.theme), d = Lh(r.icons), m = Nz(r.locale), f = Sh(r.date, m), _ = Mh(r.goTo, m);
     return {
         install: g => {
             for (const y in l) g.directive(y, l[y]);
             for (const y in a) g.component(y, a[y]);
             for (const y in o) g.component(y, Ur({
                 ...o[y],
                 name: y,
@@ -7804,15 +7804,15 @@
 
 function Gt(e) {
     var r, o;
     const n = this.$,
         t = ((r = n.parent) == null ? void 0 : r.provides) ?? ((o = n.vnode.appContext) == null ? void 0 : o.provides);
     if (t && e in t) return t[e]
 }
-const Gh = Dt({
+const Gh = It({
     __name: "App",
     setup(e) {
         const n = Rh();
         return ur(() => {
             le.isInStandaloneMode = window.navigator.standalone || !1, window.matchMedia("(prefers-color-scheme: dark)").addEventListener("change", r => {
                 const o = r.matches ? "dark" : "light";
                 n.global.name.value = o
@@ -7820,15 +7820,15 @@
             let t = "";
             {
                 const r = window.location;
                 t = r.origin + r.pathname
             }
             ot.initialize(t)
         }), (t, r) => {
-            const o = Ef("router-view");
+            const o = kf("router-view");
             return Yo(), el(o)
         }
     }
 });
 const Bh = {
         base: "#f44336",
         lighten5: "#ffebee",
@@ -8065,15 +8065,15 @@
         darken3: "#ef6c00",
         darken4: "#e65100",
         accent1: "#ffd180",
         accent2: "#ffab40",
         accent3: "#ff9100",
         accent4: "#ff6d00"
     },
-    e0 = {
+    eg = {
         base: "#ff5722",
         lighten5: "#fbe9e7",
         lighten4: "#ffccbc",
         lighten3: "#ffab91",
         lighten2: "#ff8a65",
         lighten1: "#ff7043",
         darken1: "#f4511e",
@@ -8081,51 +8081,51 @@
         darken3: "#d84315",
         darken4: "#bf360c",
         accent1: "#ff9e80",
         accent2: "#ff6e40",
         accent3: "#ff3d00",
         accent4: "#dd2c00"
     },
-    n0 = {
+    ng = {
         base: "#795548",
         lighten5: "#efebe9",
         lighten4: "#d7ccc8",
         lighten3: "#bcaaa4",
         lighten2: "#a1887f",
         lighten1: "#8d6e63",
         darken1: "#6d4c41",
         darken2: "#5d4037",
         darken3: "#4e342e",
         darken4: "#3e2723"
     },
-    t0 = {
+    tg = {
         base: "#607d8b",
         lighten5: "#eceff1",
         lighten4: "#cfd8dc",
         lighten3: "#b0bec5",
         lighten2: "#90a4ae",
         lighten1: "#78909c",
         darken1: "#546e7a",
         darken2: "#455a64",
         darken3: "#37474f",
         darken4: "#263238"
     },
-    r0 = {
+    rg = {
         base: "#9e9e9e",
         lighten5: "#fafafa",
         lighten4: "#f5f5f5",
         lighten3: "#eeeeee",
         lighten2: "#e0e0e0",
         lighten1: "#bdbdbd",
         darken1: "#757575",
         darken2: "#616161",
         darken3: "#424242",
         darken4: "#212121"
     },
-    o0 = {
+    og = {
         black: "#000000",
         white: "#ffffff",
         transparent: "#ffffff00"
     },
     io = {
         red: Bh,
         pink: Hh,
@@ -8138,32 +8138,32 @@
         teal: $h,
         green: Kh,
         lightGreen: Xh,
         lime: Yh,
         yellow: Qh,
         amber: Zh,
         orange: Jh,
-        deepOrange: e0,
-        brown: n0,
-        blueGrey: t0,
-        grey: r0,
-        shades: o0
+        deepOrange: eg,
+        brown: ng,
+        blueGrey: tg,
+        grey: rg,
+        shades: og
     },
-    i0 = {
-        component: e => Ge(Ih, {
+    ig = {
+        component: e => Ge(Dh, {
             ...e,
             class: "material-icons"
         })
     },
-    a0 = zm({
+    ag = zm({
         icons: {
             defaultSet: "mdi",
             aliases: dm,
             sets: {
-                md: i0,
+                md: ig,
                 mdi: fm
             }
         },
         display: {
             mobileBreakpoint: "md",
             thresholds: {
                 xs: 0,
@@ -8189,34 +8189,34 @@
                         primary: io.blue.darken4,
                         accent: io.blue.lighten2
                     }
                 }
             }
         }
     }),
-    l0 = "modulepreload",
-    s0 = function(e, n) {
+    lg = "modulepreload",
+    sg = function(e, n) {
         return new URL(e, n).href
     },
-    Ds = {},
+    Is = {},
     Se = function(n, t, r) {
         if (!t || t.length === 0) return n();
         const o = document.getElementsByTagName("link");
         return Promise.all(t.map(a => {
-            if (a = s0(a, r), a in Ds) return;
-            Ds[a] = !0;
+            if (a = sg(a, r), a in Is) return;
+            Is[a] = !0;
             const l = a.endsWith(".css"),
                 u = l ? '[rel="stylesheet"]' : "";
             if (!!r)
                 for (let d = o.length - 1; d >= 0; d--) {
                     const m = o[d];
                     if (m.href === a && (!l || m.rel === "stylesheet")) return
                 } else if (document.querySelector(`link[href="${a}"]${u}`)) return;
             const c = document.createElement("link");
-            if (c.rel = l ? "stylesheet" : l0, l || (c.as = "script", c.crossOrigin = ""), c.href = a, document.head.appendChild(c), l) return new Promise((d, m) => {
+            if (c.rel = l ? "stylesheet" : lg, l || (c.as = "script", c.crossOrigin = ""), c.href = a, document.head.appendChild(c), l) return new Promise((d, m) => {
                 c.addEventListener("load", d), c.addEventListener("error", () => m(new Error(`Unable to preload CSS for ${a}`)))
             })
         })).then(() => n()).catch(a => {
             const l = new Event("vite:preloadError", {
                 cancelable: !0
             });
             if (l.payload = a, window.dispatchEvent(l), !l.defaultPrevented) throw a
@@ -8225,15 +8225,15 @@
 /*!
  * vue-router v4.3.0
  * (c) 2024 Eduardo San Martin Morote
  * @license MIT
  */
 const Ht = typeof document < "u";
 
-function u0(e) {
+function ug(e) {
     return e.__esModule || e[Symbol.toStringTag] === "Module"
 }
 const pe = Object.assign;
 
 function wi(e, n) {
     const t = {};
     for (const r in n) {
@@ -8241,110 +8241,110 @@
         t[r] = An(o) ? o.map(e) : e(o)
     }
     return t
 }
 const wr = () => {},
     An = Array.isArray,
     hm = /#/g,
-    c0 = /&/g,
-    m0 = /\//g,
-    d0 = /=/g,
-    f0 = /\?/g,
+    cg = /&/g,
+    mg = /\//g,
+    dg = /=/g,
+    fg = /\?/g,
     gm = /\+/g,
-    _0 = /%5B/g,
-    p0 = /%5D/g,
+    _g = /%5B/g,
+    pg = /%5D/g,
     bm = /%5E/g,
-    z0 = /%60/g,
+    zg = /%60/g,
     vm = /%7B/g,
-    h0 = /%7C/g,
+    hg = /%7C/g,
     ym = /%7D/g,
-    g0 = /%20/g;
+    gg = /%20/g;
 
 function il(e) {
-    return encodeURI("" + e).replace(h0, "|").replace(_0, "[").replace(p0, "]")
+    return encodeURI("" + e).replace(hg, "|").replace(_g, "[").replace(pg, "]")
 }
 
-function b0(e) {
+function bg(e) {
     return il(e).replace(vm, "{").replace(ym, "}").replace(bm, "^")
 }
 
 function sa(e) {
-    return il(e).replace(gm, "%2B").replace(g0, "+").replace(hm, "%23").replace(c0, "%26").replace(z0, "`").replace(vm, "{").replace(ym, "}").replace(bm, "^")
+    return il(e).replace(gm, "%2B").replace(gg, "+").replace(hm, "%23").replace(cg, "%26").replace(zg, "`").replace(vm, "{").replace(ym, "}").replace(bm, "^")
 }
 
-function v0(e) {
-    return sa(e).replace(d0, "%3D")
+function vg(e) {
+    return sa(e).replace(dg, "%3D")
 }
 
-function y0(e) {
-    return il(e).replace(hm, "%23").replace(f0, "%3F")
+function yg(e) {
+    return il(e).replace(hm, "%23").replace(fg, "%3F")
 }
 
-function T0(e) {
-    return e == null ? "" : y0(e).replace(m0, "%2F")
+function Tg(e) {
+    return e == null ? "" : yg(e).replace(mg, "%2F")
 }
 
 function xr(e) {
     try {
         return decodeURIComponent("" + e)
     } catch {}
     return "" + e
 }
-const S0 = /\/$/,
-    w0 = e => e.replace(S0, "");
+const Sg = /\/$/,
+    wg = e => e.replace(Sg, "");
 
-function Ei(e, n, t = "/") {
+function ki(e, n, t = "/") {
     let r, o = {},
         a = "",
         l = "";
     const u = n.indexOf("#");
     let s = n.indexOf("?");
-    return u < s && u >= 0 && (s = -1), s > -1 && (r = n.slice(0, s), a = n.slice(s + 1, u > -1 ? u : n.length), o = e(a)), u > -1 && (r = r || n.slice(0, u), l = n.slice(u, n.length)), r = P0(r ?? n, t), {
+    return u < s && u >= 0 && (s = -1), s > -1 && (r = n.slice(0, s), a = n.slice(s + 1, u > -1 ? u : n.length), o = e(a)), u > -1 && (r = r || n.slice(0, u), l = n.slice(u, n.length)), r = Pg(r ?? n, t), {
         fullPath: r + (a && "?") + a + l,
         path: r,
         query: o,
         hash: xr(l)
     }
 }
 
-function E0(e, n) {
+function kg(e, n) {
     const t = n.query ? e(n.query) : "";
     return n.path + (t && "?") + t + (n.hash || "")
 }
 
 function Ls(e, n) {
     return !n || !e.toLowerCase().startsWith(n.toLowerCase()) ? e : e.slice(n.length) || "/"
 }
 
-function k0(e, n, t) {
+function Eg(e, n, t) {
     const r = n.matched.length - 1,
         o = t.matched.length - 1;
     return r > -1 && r === o && rr(n.matched[r], t.matched[o]) && Tm(n.params, t.params) && e(n.query) === e(t.query) && n.hash === t.hash
 }
 
 function rr(e, n) {
     return (e.aliasOf || e) === (n.aliasOf || n)
 }
 
 function Tm(e, n) {
     if (Object.keys(e).length !== Object.keys(n).length) return !1;
     for (const t in e)
-        if (!A0(e[t], n[t])) return !1;
+        if (!Ag(e[t], n[t])) return !1;
     return !0
 }
 
-function A0(e, n) {
+function Ag(e, n) {
     return An(e) ? Os(e, n) : An(n) ? Os(n, e) : e === n
 }
 
 function Os(e, n) {
     return An(n) ? e.length === n.length && e.every((t, r) => t === n[r]) : e.length === 1 && e[0] === n
 }
 
-function P0(e, n) {
+function Pg(e, n) {
     if (e.startsWith("/")) return e;
     if (!e) return n;
     const t = n.split("/"),
         r = e.split("/"),
         o = r[r.length - 1];
     (o === ".." || o === ".") && r.push("");
     let a = t.length - 1,
@@ -8355,73 +8355,73 @@
             else break;
     return t.slice(0, a).join("/") + "/" + r.slice(l).join("/")
 }
 var Rr;
 (function(e) {
     e.pop = "pop", e.push = "push"
 })(Rr || (Rr = {}));
-var Er;
+var kr;
 (function(e) {
     e.back = "back", e.forward = "forward", e.unknown = ""
-})(Er || (Er = {}));
+})(kr || (kr = {}));
 
-function M0(e) {
+function Mg(e) {
     if (!e)
         if (Ht) {
             const n = document.querySelector("base");
             e = n && n.getAttribute("href") || "/", e = e.replace(/^\w+:\/\/[^\/]+/, "")
         } else e = "/";
-    return e[0] !== "/" && e[0] !== "#" && (e = "/" + e), w0(e)
+    return e[0] !== "/" && e[0] !== "#" && (e = "/" + e), wg(e)
 }
-const C0 = /^[^#]+#/;
+const Cg = /^[^#]+#/;
 
-function I0(e, n) {
-    return e.replace(C0, "#") + n
+function Dg(e, n) {
+    return e.replace(Cg, "#") + n
 }
 
-function D0(e, n) {
+function Ig(e, n) {
     const t = document.documentElement.getBoundingClientRect(),
         r = e.getBoundingClientRect();
     return {
         behavior: n.behavior,
         left: r.left - t.left - (n.left || 0),
         top: r.top - t.top - (n.top || 0)
     }
 }
 const ti = () => ({
     left: window.scrollX,
     top: window.scrollY
 });
 
-function L0(e) {
+function Lg(e) {
     let n;
     if ("el" in e) {
         const t = e.el,
             r = typeof t == "string" && t.startsWith("#"),
             o = typeof t == "string" ? r ? document.getElementById(t.slice(1)) : document.querySelector(t) : t;
         if (!o) return;
-        n = D0(o, e)
+        n = Ig(o, e)
     } else n = e;
     "scrollBehavior" in document.documentElement.style ? window.scrollTo(n) : window.scrollTo(n.left != null ? n.left : window.scrollX, n.top != null ? n.top : window.scrollY)
 }
 
 function xs(e, n) {
     return (history.state ? history.state.position - n : -1) + e
 }
 const ua = new Map;
 
-function O0(e, n) {
+function Og(e, n) {
     ua.set(e, n)
 }
 
-function x0(e) {
+function xg(e) {
     const n = ua.get(e);
     return ua.delete(e), n
 }
-let R0 = () => location.protocol + "//" + location.host;
+let Rg = () => location.protocol + "//" + location.host;
 
 function Sm(e, n) {
     const {
         pathname: t,
         search: r,
         hash: o
     } = n, a = e.indexOf("#");
@@ -8429,15 +8429,15 @@
         let u = o.includes(e.slice(a)) ? e.slice(a).length : 1,
             s = o.slice(u);
         return s[0] !== "/" && (s = "/" + s), Ls(s, "")
     }
     return Ls(t, e) + r + o
 }
 
-function N0(e, n, t, r) {
+function Ng(e, n, t, r) {
     let o = [],
         a = [],
         l = null;
     const u = ({
         state: f
     }) => {
         const _ = Sm(e, location),
@@ -8451,15 +8451,15 @@
             }
             y = g ? f.position - g.position : 0
         } else r(_);
         o.forEach(z => {
             z(t.value, p, {
                 delta: y,
                 type: Rr.pop,
-                direction: y ? y > 0 ? Er.forward : Er.back : Er.unknown
+                direction: y ? y > 0 ? kr.forward : kr.back : kr.unknown
             })
         })
     };
 
     function s() {
         l = t.value
     }
@@ -8502,15 +8502,15 @@
         forward: t,
         replaced: r,
         position: window.history.length,
         scroll: o ? ti() : null
     }
 }
 
-function G0(e) {
+function Gg(e) {
     const {
         history: n,
         location: t
     } = window, r = {
         value: Sm(e, t)
     }, o = {
         value: n.state
@@ -8522,15 +8522,15 @@
         position: n.length - 1,
         replaced: !0,
         scroll: null
     }, !0);
 
     function a(s, c, d) {
         const m = e.indexOf("#"),
-            f = m > -1 ? (t.host && document.querySelector("base") ? e : e.slice(m)) + s : R0() + e + s;
+            f = m > -1 ? (t.host && document.querySelector("base") ? e : e.slice(m)) + s : Rg() + e + s;
         try {
             n[d ? "replaceState" : "pushState"](c, "", f), o.value = c
         } catch (_) {
             console.error(_), t[d ? "replace" : "assign"](f)
         }
     }
 
@@ -8556,42 +8556,42 @@
         location: r,
         state: o,
         push: u,
         replace: l
     }
 }
 
-function B0(e) {
-    e = M0(e);
-    const n = G0(e),
-        t = N0(e, n.state, n.location, n.replace);
+function Bg(e) {
+    e = Mg(e);
+    const n = Gg(e),
+        t = Ng(e, n.state, n.location, n.replace);
 
     function r(a, l = !0) {
         l || t.pauseListeners(), history.go(a)
     }
     const o = pe({
         location: "",
         base: e,
         go: r,
-        createHref: I0.bind(null, e)
+        createHref: Dg.bind(null, e)
     }, n, t);
     return Object.defineProperty(o, "location", {
         enumerable: !0,
         get: () => n.location.value
     }), Object.defineProperty(o, "state", {
         enumerable: !0,
         get: () => n.state.value
     }), o
 }
 
-function H0(e) {
-    return e = location.host ? e || location.pathname + location.search : "", e.includes("#") || (e += "#"), B0(e)
+function Hg(e) {
+    return e = location.host ? e || location.pathname + location.search : "", e.includes("#") || (e += "#"), Bg(e)
 }
 
-function F0(e) {
+function Fg(e) {
     return typeof e == "string" || e && typeof e == "object"
 }
 
 function wm(e) {
     return typeof e == "string" || typeof e == "symbol"
 }
 const Qn = {
@@ -8601,51 +8601,51 @@
         query: {},
         hash: "",
         fullPath: "/",
         matched: [],
         meta: {},
         redirectedFrom: void 0
     },
-    Em = Symbol("");
+    km = Symbol("");
 var Ns;
 (function(e) {
     e[e.aborted = 4] = "aborted", e[e.cancelled = 8] = "cancelled", e[e.duplicated = 16] = "duplicated"
 })(Ns || (Ns = {}));
 
 function or(e, n) {
     return pe(new Error, {
         type: e,
-        [Em]: !0
+        [km]: !0
     }, n)
 }
 
 function Nn(e, n) {
-    return e instanceof Error && Em in e && (n == null || !!(e.type & n))
+    return e instanceof Error && km in e && (n == null || !!(e.type & n))
 }
 const Gs = "[^/]+?",
-    V0 = {
+    Vg = {
         sensitive: !1,
         strict: !1,
         start: !0,
         end: !0
     },
-    j0 = /[.+*?^${}()[\]/\\]/g;
+    jg = /[.+*?^${}()[\]/\\]/g;
 
-function U0(e, n) {
-    const t = pe({}, V0, n),
+function Ug(e, n) {
+    const t = pe({}, Vg, n),
         r = [];
     let o = t.start ? "^" : "";
     const a = [];
     for (const c of e) {
         const d = c.length ? [] : [90];
         t.strict && !c.length && (o += "/");
         for (let m = 0; m < c.length; m++) {
             const f = c[m];
             let _ = 40 + (t.sensitive ? .25 : 0);
-            if (f.type === 0) m || (o += "/"), o += f.value.replace(j0, "\\$&"), _ += 40;
+            if (f.type === 0) m || (o += "/"), o += f.value.replace(jg, "\\$&"), _ += 40;
             else if (f.type === 1) {
                 const {
                     value: p,
                     repeatable: g,
                     optional: y,
                     regexp: z
                 } = f;
@@ -8717,56 +8717,56 @@
         score: r,
         keys: a,
         parse: u,
         stringify: s
     }
 }
 
-function q0(e, n) {
+function qg(e, n) {
     let t = 0;
     for (; t < e.length && t < n.length;) {
         const r = n[t] - e[t];
         if (r) return r;
         t++
     }
     return e.length < n.length ? e.length === 1 && e[0] === 40 + 40 ? -1 : 1 : e.length > n.length ? n.length === 1 && n[0] === 40 + 40 ? 1 : -1 : 0
 }
 
-function W0(e, n) {
+function Wg(e, n) {
     let t = 0;
     const r = e.score,
         o = n.score;
     for (; t < r.length && t < o.length;) {
-        const a = q0(r[t], o[t]);
+        const a = qg(r[t], o[t]);
         if (a) return a;
         t++
     }
     if (Math.abs(o.length - r.length) === 1) {
         if (Bs(r)) return 1;
         if (Bs(o)) return -1
     }
     return o.length - r.length
 }
 
 function Bs(e) {
     const n = e[e.length - 1];
     return e.length > 0 && n[n.length - 1] < 0
 }
-const $0 = {
+const $g = {
         type: 0,
         value: ""
     },
-    K0 = /[a-zA-Z0-9_]/;
+    Kg = /[a-zA-Z0-9_]/;
 
-function X0(e) {
+function Xg(e) {
     if (!e) return [
         []
     ];
     if (e === "/") return [
-        [$0]
+        [$g]
     ];
     if (!e.startsWith("/")) throw new Error(`Invalid path "${e}"`);
 
     function n(_) {
         throw new Error(`ERR (${t})/"${c}": ${_}`)
     }
     let t = 0,
@@ -8806,15 +8806,15 @@
             case 0:
                 s === "/" ? (c && m(), l()) : s === ":" ? (m(), t = 1) : f();
                 break;
             case 4:
                 f(), t = r;
                 break;
             case 1:
-                s === "(" ? t = 2 : K0.test(s) ? f() : (m(), t = 0, s !== "*" && s !== "?" && s !== "+" && u--);
+                s === "(" ? t = 2 : Kg.test(s) ? f() : (m(), t = 0, s !== "*" && s !== "?" && s !== "+" && u--);
                 break;
             case 2:
                 s === ")" ? d[d.length - 1] == "\\" ? d = d.slice(0, -1) + s : t = 3 : d += s;
                 break;
             case 3:
                 m(), t = 0, s !== "*" && s !== "?" && s !== "+" && u--, d = "";
                 break;
@@ -8822,41 +8822,41 @@
                 n("Unknown state");
                 break
         }
     }
     return t === 2 && n(`Unfinished custom RegExp for param "${c}"`), m(), l(), o
 }
 
-function Y0(e, n, t) {
-    const r = U0(X0(e.path), t),
+function Yg(e, n, t) {
+    const r = Ug(Xg(e.path), t),
         o = pe(r, {
             record: e,
             parent: n,
             children: [],
             alias: []
         });
     return n && !o.record.aliasOf == !n.record.aliasOf && n.children.push(o), o
 }
 
-function Q0(e, n) {
+function Qg(e, n) {
     const t = [],
         r = new Map;
     n = Vs({
         strict: !1,
         end: !0,
         sensitive: !1
     }, n);
 
     function o(d) {
         return r.get(d)
     }
 
     function a(d, m, f) {
         const _ = !f,
-            p = Z0(d);
+            p = Zg(d);
         p.aliasOf = f && f.record;
         const g = Vs(n, d),
             y = [p];
         if ("alias" in d) {
             const h = typeof d.alias == "string" ? [d.alias] : d.alias;
             for (const S of h) y.push(pe({}, p, {
                 components: f ? f.record.components : p.components,
@@ -8866,21 +8866,21 @@
         }
         let z, b;
         for (const h of y) {
             const {
                 path: S
             } = h;
             if (m && S[0] !== "/") {
-                const E = m.record.path,
-                    k = E[E.length - 1] === "/" ? "" : "/";
-                h.path = m.record.path + (S && k + S)
-            }
-            if (z = Y0(h, m, g), f ? f.alias.push(z) : (b = b || z, b !== z && b.alias.push(z), _ && d.name && !Fs(z) && l(d.name)), p.children) {
-                const E = p.children;
-                for (let k = 0; k < E.length; k++) a(E[k], z, f && f.children[k])
+                const k = m.record.path,
+                    E = k[k.length - 1] === "/" ? "" : "/";
+                h.path = m.record.path + (S && E + S)
+            }
+            if (z = Yg(h, m, g), f ? f.alias.push(z) : (b = b || z, b !== z && b.alias.push(z), _ && d.name && !Fs(z) && l(d.name)), p.children) {
+                const k = p.children;
+                for (let E = 0; E < k.length; E++) a(k[E], z, f && f.children[E])
             }
             f = f || z, (z.record.components && Object.keys(z.record.components).length || z.record.name || z.record.redirect) && s(z)
         }
         return b ? () => {
             l(b)
         } : wr
     }
@@ -8897,15 +8897,15 @@
 
     function u() {
         return t
     }
 
     function s(d) {
         let m = 0;
-        for (; m < t.length && W0(d, t[m]) >= 0 && (d.record.path !== t[m].record.path || !km(d, t[m]));) m++;
+        for (; m < t.length && Wg(d, t[m]) >= 0 && (d.record.path !== t[m].record.path || !Em(d, t[m]));) m++;
         t.splice(m, 0, d), d.record.name && !Fs(d) && r.set(d.record.name, d)
     }
 
     function c(d, m) {
         let f, _ = {},
             p, g;
         if ("name" in d && d.name) {
@@ -8925,15 +8925,15 @@
         let z = f;
         for (; z;) y.unshift(z.record), z = z.parent;
         return {
             name: g,
             path: p,
             params: _,
             matched: y,
-            meta: eg(y)
+            meta: e0(y)
         }
     }
     return e.forEach(d => a(d)), {
         addRoute: a,
         resolve: c,
         removeRoute: l,
         getRoutes: u,
@@ -8943,35 +8943,35 @@
 
 function Hs(e, n) {
     const t = {};
     for (const r of n) r in e && (t[r] = e[r]);
     return t
 }
 
-function Z0(e) {
+function Zg(e) {
     return {
         path: e.path,
         redirect: e.redirect,
         name: e.name,
         meta: e.meta || {},
         aliasOf: void 0,
         beforeEnter: e.beforeEnter,
-        props: J0(e),
+        props: Jg(e),
         children: e.children || [],
         instances: {},
         leaveGuards: new Set,
         updateGuards: new Set,
         enterCallbacks: {},
         components: "components" in e ? e.components || null : e.component && {
             default: e.component
         }
     }
 }
 
-function J0(e) {
+function Jg(e) {
     const n = {},
         t = e.props || !1;
     if ("component" in e) n.default = t;
     else
         for (const r in e.components) n[r] = typeof t == "object" ? t[r] : t;
     return n
 }
@@ -8980,29 +8980,29 @@
     for (; e;) {
         if (e.record.aliasOf) return !0;
         e = e.parent
     }
     return !1
 }
 
-function eg(e) {
+function e0(e) {
     return e.reduce((n, t) => pe(n, t.meta), {})
 }
 
 function Vs(e, n) {
     const t = {};
     for (const r in e) t[r] = r in n ? n[r] : e[r];
     return t
 }
 
-function km(e, n) {
-    return n.children.some(t => t === e || km(e, t))
+function Em(e, n) {
+    return n.children.some(t => t === e || Em(e, t))
 }
 
-function ng(e) {
+function n0(e) {
     const n = {};
     if (e === "" || e === "?") return n;
     const r = (e[0] === "?" ? e.slice(1) : e).split("&");
     for (let o = 0; o < r.length; ++o) {
         const a = r[o].replace(gm, " "),
             l = a.indexOf("="),
             u = xr(l < 0 ? a : a.slice(0, l)),
@@ -9015,33 +9015,33 @@
     return n
 }
 
 function js(e) {
     let n = "";
     for (let t in e) {
         const r = e[t];
-        if (t = v0(t), r == null) {
+        if (t = vg(t), r == null) {
             r !== void 0 && (n += (n.length ? "&" : "") + t);
             continue
         }(An(r) ? r.map(a => a && sa(a)) : [r && sa(r)]).forEach(a => {
             a !== void 0 && (n += (n.length ? "&" : "") + t, a != null && (n += "=" + a))
         })
     }
     return n
 }
 
-function tg(e) {
+function t0(e) {
     const n = {};
     for (const t in e) {
         const r = e[t];
         r !== void 0 && (n[t] = An(r) ? r.map(o => o == null ? null : "" + o) : r == null ? r : "" + r)
     }
     return n
 }
-const rg = Symbol(""),
+const r0 = Symbol(""),
     Us = Symbol(""),
     ri = Symbol(""),
     Am = Symbol(""),
     ca = Symbol("");
 
 function _r() {
     let e = [];
@@ -9066,49 +9066,49 @@
 function it(e, n, t, r, o, a = l => l()) {
     const l = r && (r.enterCallbacks[o] = r.enterCallbacks[o] || []);
     return () => new Promise((u, s) => {
         const c = f => {
                 f === !1 ? s(or(4, {
                     from: t,
                     to: n
-                })) : f instanceof Error ? s(f) : F0(f) ? s(or(2, {
+                })) : f instanceof Error ? s(f) : Fg(f) ? s(or(2, {
                     from: n,
                     to: f
                 })) : (l && r.enterCallbacks[o] === l && typeof f == "function" && l.push(f), u())
             },
             d = a(() => e.call(r && r.instances[o], n, t, c));
         let m = Promise.resolve(d);
         e.length < 3 && (m = m.then(c)), m.catch(f => s(f))
     })
 }
 
-function ki(e, n, t, r, o = a => a()) {
+function Ei(e, n, t, r, o = a => a()) {
     const a = [];
     for (const l of e)
         for (const u in l.components) {
             let s = l.components[u];
             if (!(n !== "beforeRouteEnter" && !l.instances[u]))
-                if (og(s)) {
+                if (o0(s)) {
                     const d = (s.__vccOpts || s)[n];
                     d && a.push(it(d, t, r, l, u, o))
                 } else {
                     let c = s();
                     a.push(() => c.then(d => {
                         if (!d) return Promise.reject(new Error(`Couldn't resolve component "${u}" at "${l.path}"`));
-                        const m = u0(d) ? d.default : d;
+                        const m = ug(d) ? d.default : d;
                         l.components[u] = m;
                         const _ = (m.__vccOpts || m)[n];
                         return _ && it(_, t, r, l, u, o)()
                     }))
                 }
         }
     return a
 }
 
-function og(e) {
+function o0(e) {
     return typeof e == "object" || "displayName" in e || "props" in e || "__vccOpts" in e
 }
 
 function qs(e) {
     const n = He(ri),
         t = He(Am),
         r = ae(() => n.resolve(bn(e.to))),
@@ -9120,29 +9120,29 @@
             } = s, d = s[c - 1], m = t.matched;
             if (!d || !m.length) return -1;
             const f = m.findIndex(rr.bind(null, d));
             if (f > -1) return f;
             const _ = Ws(s[c - 2]);
             return c > 1 && Ws(d) === _ && m[m.length - 1].path !== _ ? m.findIndex(rr.bind(null, s[c - 2])) : f
         }),
-        a = ae(() => o.value > -1 && sg(t.params, r.value.params)),
+        a = ae(() => o.value > -1 && s0(t.params, r.value.params)),
         l = ae(() => o.value > -1 && o.value === t.matched.length - 1 && Tm(t.params, r.value.params));
 
     function u(s = {}) {
-        return lg(s) ? n[bn(e.replace) ? "replace" : "push"](bn(e.to)).catch(wr) : Promise.resolve()
+        return l0(s) ? n[bn(e.replace) ? "replace" : "push"](bn(e.to)).catch(wr) : Promise.resolve()
     }
     return {
         route: r,
         href: ae(() => r.value.href),
         isActive: a,
         isExactActive: l,
         navigate: u
     }
 }
-const ig = Dt({
+const i0 = It({
         name: "RouterLink",
         compatConfig: {
             MODE: 3
         },
         props: {
             to: {
                 type: [String, Object],
@@ -9176,42 +9176,42 @@
                     href: t.href,
                     onClick: t.navigate,
                     class: o.value
                 }, a)
             }
         }
     }),
-    ag = ig;
+    a0 = i0;
 
-function lg(e) {
+function l0(e) {
     if (!(e.metaKey || e.altKey || e.ctrlKey || e.shiftKey) && !e.defaultPrevented && !(e.button !== void 0 && e.button !== 0)) {
         if (e.currentTarget && e.currentTarget.getAttribute) {
             const n = e.currentTarget.getAttribute("target");
             if (/\b_blank\b/i.test(n)) return
         }
         return e.preventDefault && e.preventDefault(), !0
     }
 }
 
-function sg(e, n) {
+function s0(e, n) {
     for (const t in n) {
         const r = n[t],
             o = e[t];
         if (typeof r == "string") {
             if (r !== o) return !1
         } else if (!An(o) || o.length !== r.length || r.some((a, l) => a !== o[l])) return !1
     }
     return !0
 }
 
 function Ws(e) {
     return e ? e.aliasOf ? e.aliasOf.path : e.path : ""
 }
 const $s = (e, n, t) => e ?? n ?? t,
-    ug = Dt({
+    u0 = It({
         name: "RouterView",
         inheritAttrs: !1,
         props: {
             name: {
                 type: String,
                 default: "default"
             },
@@ -9234,15 +9234,15 @@
                     } = o.value;
                     let m;
                     for (;
                         (m = d[c]) && !m.components;) c++;
                     return c
                 }),
                 u = ae(() => o.value.matched[l.value]);
-            Wn(Us, ae(() => l.value + 1)), Wn(rg, u), Wn(ca, o);
+            Wn(Us, ae(() => l.value + 1)), Wn(r0, u), Wn(ca, o);
             const s = he();
             return Je(() => [s.value, u.value, e.name], ([c, d, m], [f, _, p]) => {
                 d && (d.instances[m] = c, _ && _ !== d && c && c === f && (d.leaveGuards.size || (d.leaveGuards = _.leaveGuards), d.updateGuards.size || (d.updateGuards = _.updateGuards))), c && d && (!_ || !rr(d, _) || !f) && (d.enterCallbacks[m] || []).forEach(g => g(c))
             }, {
                 flush: "post"
             }), () => {
                 const c = o.value,
@@ -9270,29 +9270,29 @@
     });
 
 function Ks(e, n) {
     if (!e) return null;
     const t = e(n);
     return t.length === 1 ? t[0] : t
 }
-const cg = ug;
+const c0 = u0;
 
-function mg(e) {
-    const n = Q0(e.routes, e),
-        t = e.parseQuery || ng,
+function m0(e) {
+    const n = Qg(e.routes, e),
+        t = e.parseQuery || n0,
         r = e.stringifyQuery || js,
         o = e.history,
         a = _r(),
         l = _r(),
         u = _r(),
         s = st(Qn);
     let c = Qn;
     Ht && e.scrollBehavior && "scrollRestoration" in history && (history.scrollRestoration = "manual");
     const d = wi.bind(null, B => "" + B),
-        m = wi.bind(null, T0),
+        m = wi.bind(null, Tg),
         f = wi.bind(null, xr);
 
     function _(B, K) {
         let W, X;
         return wm(B) ? (W = n.getRecordMatcher(B), X = K) : X = B, n.addRoute(X, W)
     }
 
@@ -9307,77 +9307,77 @@
 
     function y(B) {
         return !!n.getRecordMatcher(B)
     }
 
     function z(B, K) {
         if (K = pe({}, K || s.value), typeof B == "string") {
-            const A = Ei(t, B, K.path),
+            const A = ki(t, B, K.path),
                 x = n.resolve({
                     path: A.path
                 }, K),
                 H = o.createHref(A.fullPath);
             return pe(A, x, {
                 params: f(x.params),
                 hash: xr(A.hash),
                 redirectedFrom: void 0,
                 href: H
             })
         }
         let W;
         if (B.path != null) W = pe({}, B, {
-            path: Ei(t, B.path, K.path).path
+            path: ki(t, B.path, K.path).path
         });
         else {
             const A = pe({}, B.params);
             for (const x in A) A[x] == null && delete A[x];
             W = pe({}, B, {
                 params: m(A)
             }), K.params = m(K.params)
         }
         const X = n.resolve(W, K),
             me = B.hash || "";
         X.params = d(f(X.params));
-        const ze = E0(r, pe({}, B, {
-                hash: b0(me),
+        const ze = kg(r, pe({}, B, {
+                hash: bg(me),
                 path: X.path
             })),
             w = o.createHref(ze);
         return pe({
             fullPath: ze,
             hash: me,
-            query: r === js ? tg(B.query) : B.query || {}
+            query: r === js ? t0(B.query) : B.query || {}
         }, X, {
             redirectedFrom: void 0,
             href: w
         })
     }
 
     function b(B) {
-        return typeof B == "string" ? Ei(t, B, s.value.path) : pe({}, B)
+        return typeof B == "string" ? ki(t, B, s.value.path) : pe({}, B)
     }
 
     function h(B, K) {
         if (c !== B) return or(8, {
             from: K,
             to: B
         })
     }
 
     function S(B) {
-        return D(B)
+        return I(B)
     }
 
-    function E(B) {
+    function k(B) {
         return S(pe(b(B), {
             replace: !0
         }))
     }
 
-    function k(B) {
+    function E(B) {
         const K = B.matched[B.matched.length - 1];
         if (K && K.redirect) {
             const {
                 redirect: W
             } = K;
             let X = typeof W == "function" ? W(B) : W;
             return typeof X == "string" && (X = X.includes("?") || X.includes("#") ? X = b(X) : {
@@ -9386,35 +9386,35 @@
                 query: B.query,
                 hash: B.hash,
                 params: X.path != null ? {} : B.params
             }, X)
         }
     }
 
-    function D(B, K) {
+    function I(B, K) {
         const W = c = z(B),
             X = s.value,
             me = B.state,
             ze = B.force,
             w = B.replace === !0,
-            A = k(W);
-        if (A) return D(pe(b(A), {
+            A = E(W);
+        if (A) return I(pe(b(A), {
             state: typeof A == "object" ? pe({}, me, A.state) : me,
             force: ze,
             replace: w
         }), K || W);
         const x = W;
         x.redirectedFrom = K;
         let H;
-        return !ze && k0(r, X, W) && (H = or(16, {
+        return !ze && Eg(r, X, W) && (H = or(16, {
             to: x,
             from: X
-        }), Ee(X, X, !0, !1)), (H ? Promise.resolve(H) : L(x, X)).catch(N => Nn(N) ? Nn(N, 2) ? N : Xe(N) : ue(N, x, X)).then(N => {
+        }), ke(X, X, !0, !1)), (H ? Promise.resolve(H) : L(x, X)).catch(N => Nn(N) ? Nn(N, 2) ? N : Xe(N) : ue(N, x, X)).then(N => {
             if (N) {
-                if (Nn(N, 2)) return D(pe({
+                if (Nn(N, 2)) return I(pe({
                     replace: w
                 }, b(N.to), {
                     state: typeof N.to == "object" ? pe({}, me, N.to.state) : me,
                     force: ze
                 }), K || x)
             } else N = O(x, X, !0, w, me);
             return F(x, X, N), N
@@ -9429,39 +9429,39 @@
     function M(B) {
         const K = Sn.values().next().value;
         return K && typeof K.runWithContext == "function" ? K.runWithContext(B) : B()
     }
 
     function L(B, K) {
         let W;
-        const [X, me, ze] = dg(B, K);
-        W = ki(X.reverse(), "beforeRouteLeave", B, K);
+        const [X, me, ze] = d0(B, K);
+        W = Ei(X.reverse(), "beforeRouteLeave", B, K);
         for (const A of X) A.leaveGuards.forEach(x => {
             W.push(it(x, B, K))
         });
         const w = P.bind(null, B, K);
         return W.push(w), Ce(W).then(() => {
             W = [];
             for (const A of a.list()) W.push(it(A, B, K));
             return W.push(w), Ce(W)
         }).then(() => {
-            W = ki(me, "beforeRouteUpdate", B, K);
+            W = Ei(me, "beforeRouteUpdate", B, K);
             for (const A of me) A.updateGuards.forEach(x => {
                 W.push(it(x, B, K))
             });
             return W.push(w), Ce(W)
         }).then(() => {
             W = [];
             for (const A of ze)
                 if (A.beforeEnter)
                     if (An(A.beforeEnter))
                         for (const x of A.beforeEnter) W.push(it(x, B, K));
                     else W.push(it(A.beforeEnter, B, K));
             return W.push(w), Ce(W)
-        }).then(() => (B.matched.forEach(A => A.enterCallbacks = {}), W = ki(ze, "beforeRouteEnter", B, K, M), W.push(w), Ce(W))).then(() => {
+        }).then(() => (B.matched.forEach(A => A.enterCallbacks = {}), W = Ei(ze, "beforeRouteEnter", B, K, M), W.push(w), Ce(W))).then(() => {
             W = [];
             for (const A of l.list()) W.push(it(A, B, K));
             return W.push(w), Ce(W)
         }).catch(A => Nn(A, 8) ? A : Promise.reject(A))
     }
 
     function F(B, K, W) {
@@ -9471,32 +9471,32 @@
     function O(B, K, W, X, me) {
         const ze = h(B, K);
         if (ze) return ze;
         const w = K === Qn,
             A = Ht ? history.state : {};
         W && (X || w ? o.replace(B.fullPath, pe({
             scroll: w && A && A.scroll
-        }, me)) : o.push(B.fullPath, me)), s.value = B, Ee(B, K, W, w), Xe()
+        }, me)) : o.push(B.fullPath, me)), s.value = B, ke(B, K, W, w), Xe()
     }
     let V;
 
     function Z() {
         V || (V = o.listen((B, K, W) => {
             if (!Kn.listening) return;
             const X = z(B),
-                me = k(X);
+                me = E(X);
             if (me) {
-                D(pe(me, {
+                I(pe(me, {
                     replace: !0
                 }), X).catch(wr);
                 return
             }
             c = X;
             const ze = s.value;
-            Ht && O0(xs(ze.fullPath, W.delta), ti()), L(X, ze).catch(w => Nn(w, 12) ? w : Nn(w, 2) ? (D(w.to, X).then(A => {
+            Ht && Og(xs(ze.fullPath, W.delta), ti()), L(X, ze).catch(w => Nn(w, 12) ? w : Nn(w, 2) ? (I(w.to, X).then(A => {
                 Nn(A, 20) && !W.delta && W.type === Rr.pop && o.go(-1, !1)
             }).catch(wr), Promise.reject()) : (W.delta && o.go(-W.delta, !1), ue(w, X, ze))).then(w => {
                 w = w || O(X, ze, !1), w && (W.delta && !Nn(w, 8) ? o.go(-W.delta, !1) : W.type === Rr.pop && Nn(w, 20) && o.go(-1, !1)), F(X, ze, w)
             }).catch(wr)
         }))
     }
     let oe = _r(),
@@ -9515,47 +9515,47 @@
         })
     }
 
     function Xe(B) {
         return se || (se = !B, Z(), oe.list().forEach(([K, W]) => B ? W(B) : K()), oe.reset()), B
     }
 
-    function Ee(B, K, W, X) {
+    function ke(B, K, W, X) {
         const {
             scrollBehavior: me
         } = e;
         if (!Ht || !me) return Promise.resolve();
-        const ze = !W && x0(xs(B.fullPath, 0)) || (X || !W) && history.state && history.state.scroll || null;
-        return Vr().then(() => me(B, K, ze)).then(w => w && L0(w)).catch(w => ue(w, B, K))
+        const ze = !W && xg(xs(B.fullPath, 0)) || (X || !W) && history.state && history.state.scroll || null;
+        return Vr().then(() => me(B, K, ze)).then(w => w && Lg(w)).catch(w => ue(w, B, K))
     }
-    const ke = B => o.go(B);
+    const Ee = B => o.go(B);
     let Mn;
     const Sn = new Set,
         Kn = {
             currentRoute: s,
             listening: !0,
             addRoute: _,
             removeRoute: p,
             hasRoute: y,
             getRoutes: g,
             resolve: z,
             options: e,
             push: S,
-            replace: E,
-            go: ke,
-            back: () => ke(-1),
-            forward: () => ke(1),
+            replace: k,
+            go: Ee,
+            back: () => Ee(-1),
+            forward: () => Ee(1),
             beforeEach: a.add,
             beforeResolve: l.add,
             afterEach: u.add,
             onError: ie.add,
             isReady: Ue,
             install(B) {
                 const K = this;
-                B.component("RouterLink", ag), B.component("RouterView", cg), B.config.globalProperties.$router = K, Object.defineProperty(B.config.globalProperties, "$route", {
+                B.component("RouterLink", a0), B.component("RouterView", c0), B.config.globalProperties.$router = K, Object.defineProperty(B.config.globalProperties, "$route", {
                     enumerable: !0,
                     get: () => bn(s)
                 }), Ht && !Mn && s.value === Qn && (Mn = !0, S(o.location).catch(me => {}));
                 const W = {};
                 for (const me in Qn) Object.defineProperty(W, me, {
                     get: () => s.value[me],
                     enumerable: !0
@@ -9570,15 +9570,15 @@
 
     function Ce(B) {
         return B.reduce((K, W) => K.then(() => M(W)), Promise.resolve())
     }
     return Kn
 }
 
-function dg(e, n) {
+function d0(e, n) {
     const t = [],
         r = [],
         o = [],
         a = Math.max(n.matched.length, e.matched.length);
     for (let l = 0; l < a; l++) {
         const u = n.matched[l];
         u && (e.matched.find(c => rr(c, u)) ? r.push(u) : t.push(u));
@@ -9993,85 +9993,85 @@
         if (typeof n == "function" && n.amd) return n;
         if (typeof window < "u") return function(t) {
             window.MobileDetect = t()
         };
         throw new Error("unknown environment")
     }())
 })(Mm);
-var fg = Mm.exports;
-const _g = Pm(fg),
-    Yt = new _g(window.navigator.userAgent),
+var f0 = Mm.exports;
+const _0 = Pm(f0),
+    Yt = new _0(window.navigator.userAgent),
     We = {
         bp0: 375,
         bp1: 500,
         bp2: 540,
         bp3: 575,
         bp4: 715,
         bp5: 800,
         bp6: 960,
         bp7: 1100,
         bp8: 1500,
         bp9: 1700,
         bp10: 1900,
         bp11: 415
     },
-    Ie = on({
+    De = on({
         width: window.innerWidth
     });
 window.addEventListener("resize", () => {
-    Ie.width = window.innerWidth
+    De.width = window.innerWidth
 });
 const nn = e => {
         let n = "bp1",
             t = "gt",
             r = 0;
         if (typeof e == "object" ? (n = e.breakpoint, t = e.condition || "gt", r = e.offset || 0) : n = e, Object.values(["mobile", "phone", "tablet"]).includes(n)) switch (typeof e == "object" && (t = e.condition || "lt"), n) {
             case "mobile":
-                return Yt.mobile() ? !0 : t === "lt" ? Ie.width < We.bp3 : Ie.width >= We.bp3;
+                return Yt.mobile() ? !0 : t === "lt" ? De.width < We.bp3 : De.width >= We.bp3;
             case "phone":
-                return Yt.phone() ? !0 : t === "lt" ? Ie.width < We.bp3 : Ie.width >= We.bp3;
+                return Yt.phone() ? !0 : t === "lt" ? De.width < We.bp3 : De.width >= We.bp3;
             case "tablet":
-                return Yt.tablet() ? !0 : t === "lt" ? Ie.width < We.bp3 : Ie.width >= We.bp3
-        } else return t === "lt" ? Ie.width < We[n] + r : Ie.width >= We[n] + r;
+                return Yt.tablet() ? !0 : t === "lt" ? De.width < We.bp3 : De.width >= We.bp3
+        } else return t === "lt" ? De.width < We[n] + r : De.width >= We[n] + r;
         return !1
     },
     Xs = () => {
-        Ie.width = window.innerWidth
+        De.width = window.innerWidth
     },
-    pg = {
+    p0 = {
         beforeMount(e, n) {
             let t = "gt",
                 r = "bp1",
                 o = 0;
             typeof n.value == "object" ? (t = n.value.condition, r = n.value.breakpoint, o = n.value.offset || 0) : r = n.value, Object.values(["mobile", "phone", "tablet"]).includes(r) && (t = n.value.condition || "lt");
             const a = u => {
-                    if (u === "mobile") return !!Yt.mobile() ? !0 : t === "lt" ? Ie.width < We.bp3 : Ie.width >= We.bp3;
-                    if (u === "phone") return !!Yt.phone() ? !0 : t === "lt" ? Ie.width < We.bp3 : Ie.width >= We.bp3;
-                    if (u === "tablet") return !!Yt.tablet() ? !0 : t === "lt" ? Ie.width < We.bp3 : Ie.width >= We.bp3
+                    if (u === "mobile") return !!Yt.mobile() ? !0 : t === "lt" ? De.width < We.bp3 : De.width >= We.bp3;
+                    if (u === "phone") return !!Yt.phone() ? !0 : t === "lt" ? De.width < We.bp3 : De.width >= We.bp3;
+                    if (u === "tablet") return !!Yt.tablet() ? !0 : t === "lt" ? De.width < We.bp3 : De.width >= We.bp3
                 },
                 l = () => {
-                    Object.values(["mobile", "phone", "tablet"]).includes(r) ? a(r) ? e.style.display = "" : e.style.display = "none" : (t === "lt" ? Ie.width < We[r] + o : Ie.width >= We[r] + o) ? e.style.display = "" : e.style.display = "none"
+                    Object.values(["mobile", "phone", "tablet"]).includes(r) ? a(r) ? e.style.display = "" : e.style.display = "none" : (t === "lt" ? De.width < We[r] + o : De.width >= We[r] + o) ? e.style.display = "" : e.style.display = "none"
                 };
-            window.addEventListener("resize", Xs), Je(() => Ie.width, l), l(), e._onDestroy = () => {
+            window.addEventListener("resize", Xs), Je(() => De.width, l), l(), e._onDestroy = () => {
                 window.removeEventListener("resize", Xs)
             }
         },
         unmounted(e) {
             e._onDestroy()
         }
     },
-    zg = {
+    z0 = {
         install(e) {
-            e.config.globalProperties.$screenSize = Fa(Ie), e.directive("breakpoint", pg)
+            e.config.globalProperties.$screenSize = Fa(De), e.directive("breakpoint", p0)
         }
     };
 var Cm = {
         exports: {}
     },
-    Im = {
+    Dm = {
         aliceblue: [240, 248, 255],
         antiquewhite: [250, 235, 215],
         aqua: [0, 255, 255],
         aquamarine: [127, 255, 212],
         azure: [240, 255, 255],
         beige: [245, 245, 220],
         bisque: [255, 228, 196],
@@ -10213,41 +10213,41 @@
         violet: [238, 130, 238],
         wheat: [245, 222, 179],
         white: [255, 255, 255],
         whitesmoke: [245, 245, 245],
         yellow: [255, 255, 0],
         yellowgreen: [154, 205, 50]
     },
-    Dm = {
+    Im = {
         exports: {}
     },
-    hg = function(n) {
+    h0 = function(n) {
         return !n || typeof n == "string" ? !1 : n instanceof Array || Array.isArray(n) || n.length >= 0 && (n.splice instanceof Function || Object.getOwnPropertyDescriptor(n, n.length - 1) && n.constructor.name !== "String")
     },
-    gg = hg,
-    bg = Array.prototype.concat,
-    vg = Array.prototype.slice,
-    Ys = Dm.exports = function(n) {
+    g0 = h0,
+    b0 = Array.prototype.concat,
+    v0 = Array.prototype.slice,
+    Ys = Im.exports = function(n) {
         for (var t = [], r = 0, o = n.length; r < o; r++) {
             var a = n[r];
-            gg(a) ? t = bg.call(t, vg.call(a)) : t.push(a)
+            g0(a) ? t = b0.call(t, v0.call(a)) : t.push(a)
         }
         return t
     };
 Ys.wrap = function(e) {
     return function() {
         return e(Ys(arguments))
     }
 };
-var yg = Dm.exports,
-    kr = Im,
-    qr = yg,
+var y0 = Im.exports,
+    Er = Dm,
+    qr = y0,
     Lm = Object.hasOwnProperty,
     Om = Object.create(null);
-for (var Ai in kr) Lm.call(kr, Ai) && (Om[kr[Ai]] = Ai);
+for (var Ai in Er) Lm.call(Er, Ai) && (Om[Er[Ai]] = Ai);
 var pn = Cm.exports = {
     to: {},
     get: {}
 };
 pn.get = function(e) {
     var n = e.substring(0, 3).toLowerCase(),
         t, r;
@@ -10287,15 +10287,15 @@
         c && (l[3] = parseInt(c + c, 16) / 255)
     } else if (u = e.match(r)) {
         for (s = 0; s < 3; s++) l[s] = parseInt(u[s + 1], 0);
         u[4] && (u[5] ? l[3] = parseFloat(u[4]) * .01 : l[3] = parseFloat(u[4]))
     } else if (u = e.match(o)) {
         for (s = 0; s < 3; s++) l[s] = Math.round(parseFloat(u[s + 1]) * 2.55);
         u[4] && (u[5] ? l[3] = parseFloat(u[4]) * .01 : l[3] = parseFloat(u[4]))
-    } else return (u = e.match(a)) ? u[1] === "transparent" ? [0, 0, 0, 0] : Lm.call(kr, u[1]) ? (l = kr[u[1]], l[3] = 1, l) : null : null;
+    } else return (u = e.match(a)) ? u[1] === "transparent" ? [0, 0, 0, 0] : Lm.call(Er, u[1]) ? (l = Er[u[1]], l[3] = 1, l) : null : null;
     for (s = 0; s < 3; s++) l[s] = ct(l[s], 0, 255);
     return l[3] = ct(l[3], 0, 1), l
 };
 pn.get.hsl = function(e) {
     if (!e) return null;
     var n = /^hsla?\(\s*([+-]?(?:\d{0,3}\.)?\d+)(?:deg)?\s*,?\s*([+-]?[\d\.]+)%\s*,?\s*([+-]?[\d\.]+)%\s*(?:[,|\/]\s*([+-]?(?=\.\d|\d)(?:0|[1-9]\d*)?(?:\.\d*)?(?:[eE][+-]?\d+)?)\s*)?\)$/,
         t = e.match(n);
@@ -10355,16 +10355,16 @@
     return Math.min(Math.max(n, e), t)
 }
 
 function ao(e) {
     var n = Math.round(e).toString(16).toUpperCase();
     return n.length < 2 ? "0" + n : n
 }
-var Tg = Cm.exports;
-const Nr = Im,
+var T0 = Cm.exports;
+const Nr = Dm,
     xm = {};
 for (const e of Object.keys(Nr)) xm[Nr[e]] = e;
 const Y = {
     rgb: {
         channels: 3,
         labels: "rgb"
     },
@@ -10479,25 +10479,25 @@
         o = Math.min(1 - n, 1 - t, 1 - r),
         a = (1 - n - o) / (1 - o) || 0,
         l = (1 - t - o) / (1 - o) || 0,
         u = (1 - r - o) / (1 - o) || 0;
     return [a * 100, l * 100, u * 100, o * 100]
 };
 
-function Sg(e, n) {
+function S0(e, n) {
     return (e[0] - n[0]) ** 2 + (e[1] - n[1]) ** 2 + (e[2] - n[2]) ** 2
 }
 Y.rgb.keyword = function(e) {
     const n = xm[e];
     if (n) return n;
     let t = 1 / 0,
         r;
     for (const o of Object.keys(Nr)) {
         const a = Nr[o],
-            l = Sg(e, a);
+            l = S0(e, a);
         l < t && (t = l, r = o)
     }
     return r
 };
 Y.keyword.rgb = function(e) {
     return Nr[e]
 };
@@ -10831,102 +10831,102 @@
     return "000000".substring(r.length) + r
 };
 Y.rgb.gray = function(e) {
     return [(e[0] + e[1] + e[2]) / 3 / 255 * 100]
 };
 const Mo = Rm;
 
-function wg() {
+function w0() {
     const e = {},
         n = Object.keys(Mo);
     for (let t = n.length, r = 0; r < t; r++) e[n[r]] = {
         distance: -1,
         parent: null
     };
     return e
 }
 
-function Eg(e) {
-    const n = wg(),
+function k0(e) {
+    const n = w0(),
         t = [e];
     for (n[e].distance = 0; t.length;) {
         const r = t.pop(),
             o = Object.keys(Mo[r]);
         for (let a = o.length, l = 0; l < a; l++) {
             const u = o[l],
                 s = n[u];
             s.distance === -1 && (s.distance = n[r].distance + 1, s.parent = r, t.unshift(u))
         }
     }
     return n
 }
 
-function kg(e, n) {
+function E0(e, n) {
     return function(t) {
         return n(e(t))
     }
 }
 
-function Ag(e, n) {
+function A0(e, n) {
     const t = [n[e].parent, e];
     let r = Mo[n[e].parent][e],
         o = n[e].parent;
-    for (; n[o].parent;) t.unshift(n[o].parent), r = kg(Mo[n[o].parent][o], r), o = n[o].parent;
+    for (; n[o].parent;) t.unshift(n[o].parent), r = E0(Mo[n[o].parent][o], r), o = n[o].parent;
     return r.conversion = t, r
 }
-var Pg = function(e) {
-    const n = Eg(e),
+var P0 = function(e) {
+    const n = k0(e),
         t = {},
         r = Object.keys(n);
     for (let o = r.length, a = 0; a < o; a++) {
         const l = r[a];
-        n[l].parent !== null && (t[l] = Ag(l, n))
+        n[l].parent !== null && (t[l] = A0(l, n))
     }
     return t
 };
 const ma = Rm,
-    Mg = Pg,
+    M0 = P0,
     Ft = {},
-    Cg = Object.keys(ma);
+    C0 = Object.keys(ma);
 
-function Ig(e) {
+function D0(e) {
     const n = function(...t) {
         const r = t[0];
         return r == null ? r : (r.length > 1 && (t = r), e(t))
     };
     return "conversion" in e && (n.conversion = e.conversion), n
 }
 
-function Dg(e) {
+function I0(e) {
     const n = function(...t) {
         const r = t[0];
         if (r == null) return r;
         r.length > 1 && (t = r);
         const o = e(t);
         if (typeof o == "object")
             for (let a = o.length, l = 0; l < a; l++) o[l] = Math.round(o[l]);
         return o
     };
     return "conversion" in e && (n.conversion = e.conversion), n
 }
-Cg.forEach(e => {
+C0.forEach(e => {
     Ft[e] = {}, Object.defineProperty(Ft[e], "channels", {
         value: ma[e].channels
     }), Object.defineProperty(Ft[e], "labels", {
         value: ma[e].labels
     });
-    const n = Mg(e);
+    const n = M0(e);
     Object.keys(n).forEach(r => {
         const o = n[r];
-        Ft[e][r] = Dg(o), Ft[e][r].raw = Ig(o)
+        Ft[e][r] = I0(o), Ft[e][r].raw = D0(o)
     })
 });
-var Lg = Ft;
-const Vt = Tg,
-    mn = Lg,
+var L0 = Ft;
+const Vt = T0,
+    mn = L0,
     Nm = ["keyword", "gray", "hex"],
     da = {};
 for (const e of Object.keys(mn)) da[[...mn[e].labels].sort().join("")] = e;
 const Co = {};
 
 function Ne(e, n) {
     if (!(this instanceof Ne)) return new Ne(e, n);
@@ -11000,15 +11000,15 @@
         return e[0] /= 255, e[1] /= 255, e[2] /= 255, this.valpha !== 1 && e.push(this.valpha), e
     },
     unitObject() {
         const e = this.rgb().object();
         return e.r /= 255, e.g /= 255, e.b /= 255, this.valpha !== 1 && (e.alpha = this.valpha), e
     },
     round(e) {
-        return e = Math.max(e || 0, 0), new Ne([...this.color.map(xg(e)), this.valpha], this.model)
+        return e = Math.max(e || 0, 0), new Ne([...this.color.map(x0(e)), this.valpha], this.model)
     },
     alpha(e) {
         return e !== void 0 ? new Ne([...this.color, Math.max(0, Math.min(1, e))], this.model) : this.valpha
     },
     red: Ae("rgb", 0, Le(255)),
     green: Ae("rgb", 1, Le(255)),
     blue: Ae("rgb", 2, Le(255)),
@@ -11131,28 +11131,28 @@
 };
 for (const e of Object.keys(mn)) {
     if (Nm.includes(e)) continue;
     const {
         channels: n
     } = mn[e];
     Ne.prototype[e] = function(...t) {
-        return this.model === e ? new Ne(this) : t.length > 0 ? new Ne(t, e) : new Ne([...Rg(mn[this.model][e].raw(this.color)), this.valpha], e)
+        return this.model === e ? new Ne(this) : t.length > 0 ? new Ne(t, e) : new Ne([...R0(mn[this.model][e].raw(this.color)), this.valpha], e)
     }, Ne[e] = function(...t) {
         let r = t[0];
         return typeof r == "number" && (r = fa(t, n)), new Ne(r, e)
     }
 }
 
-function Og(e, n) {
+function O0(e, n) {
     return Number(e.toFixed(n))
 }
 
-function xg(e) {
+function x0(e) {
     return function(n) {
-        return Og(n, e)
+        return O0(n, e)
     }
 }
 
 function Ae(e, n, t) {
     e = Array.isArray(e) ? e : [e];
     for (const r of e)(Co[r] || (Co[r] = []))[n] = t;
     return e = e[0],
@@ -11164,24 +11164,24 @@
 
 function Le(e) {
     return function(n) {
         return Math.max(0, Math.min(e, n))
     }
 }
 
-function Rg(e) {
+function R0(e) {
     return Array.isArray(e) ? e : [e]
 }
 
 function fa(e, n) {
     for (let t = 0; t < n; t++) typeof e[t] != "number" && (e[t] = 0);
     return e
 }
-var Ng = Ne;
-const Qs = Pm(Ng);
+var N0 = Ne;
+const Qs = Pm(N0);
 if (!Vn) var Vn = {
     map: function(e, n) {
         var t = {};
         return n ? e.map(function(r, o) {
             return t.index = o, n.call(t, r)
         }) : e.slice()
     },
@@ -11196,15 +11196,15 @@
             return r + o
         }, 0)
     },
     max: function(e, n) {
         return Math.max.apply(null, n ? Vn.map(e, n) : e)
     }
 };
-var Gg = function() {
+var G0 = function() {
         var e = 5,
             n = 8 - e,
             t = 1e3;
 
         function r(s, c, d) {
             return (s << 2 * e) + (c << e) + d
         }
@@ -11270,26 +11270,26 @@
                             b[_] = z += y
                         } else
                             for (_ = c.b1; _ <= c.b2; _++) {
                                 for (y = 0, p = c.r1; p <= c.r2; p++)
                                     for (g = c.g1; g <= c.g2; g++) y += s[r(p, g, _)] || 0;
                                 b[_] = z += y
                             }
-                return b.forEach(function(S, E) {
-                        h[E] = z - S
+                return b.forEach(function(S, k) {
+                        h[k] = z - S
                     }),
                     function(S) {
-                        var E, k, D, P, M, L = S + "1",
+                        var k, E, I, P, M, L = S + "1",
                             F = S + "2",
                             O = 0;
                         for (_ = c[L]; _ <= c[F]; _++)
                             if (b[_] > z / 2) {
-                                for (D = c.copy(), P = c.copy(), M = (E = _ - c[L]) <= (k = c[F] - _) ? Math.min(c[F] - 1, ~~(_ + k / 2)) : Math.max(c[L], ~~(_ - 1 - E / 2)); !b[M];) M++;
+                                for (I = c.copy(), P = c.copy(), M = (k = _ - c[L]) <= (E = c[F] - _) ? Math.min(c[F] - 1, ~~(_ + E / 2)) : Math.max(c[L], ~~(_ - 1 - k / 2)); !b[M];) M++;
                                 for (O = h[M]; !O && b[M - 1];) O = h[--M];
-                                return D[F] = M, P[L] = D[F] + 1, [D, P]
+                                return I[F] = M, P[L] = I[F] + 1, [I, P]
                             }
                     }(f == d ? "r" : f == m ? "g" : "b")
             }
         }
         return a.prototype = {
             volume: function(s) {
                 var c = this;
@@ -11374,37 +11374,37 @@
                     var z, b = new Array(1 << 3 * e);
                     return y.forEach(function(h) {
                         z = r(h[0] >> n, h[1] >> n, h[2] >> n), b[z] = (b[z] || 0) + 1
                     }), b
                 }(s);
                 d.forEach(function() {});
                 var m = function(y, z) {
-                        var b, h, S, E = 1e6,
-                            k = 0,
-                            D = 1e6,
+                        var b, h, S, k = 1e6,
+                            E = 0,
+                            I = 1e6,
                             P = 0,
                             M = 1e6,
                             L = 0;
                         return y.forEach(function(F) {
-                            (b = F[0] >> n) < E ? E = b : b > k && (k = b), (h = F[1] >> n) < D ? D = h : h > P && (P = h), (S = F[2] >> n) < M ? M = S : S > L && (L = S)
-                        }), new a(E, k, D, P, M, L, z)
+                            (b = F[0] >> n) < k ? k = b : b > E && (E = b), (h = F[1] >> n) < I ? I = h : h > P && (P = h), (S = F[2] >> n) < M ? M = S : S > L && (L = S)
+                        }), new a(k, E, I, P, M, L, z)
                     }(s, d),
                     f = new o(function(y, z) {
                         return Vn.naturalOrder(y.count(), z.count())
                     });
 
                 function _(y, z) {
                     for (var b, h = y.size(), S = 0; S < t;) {
                         if (h >= z || S++ > t) return;
                         if ((b = y.pop()).count()) {
-                            var E = u(d, b),
-                                k = E[0],
-                                D = E[1];
-                            if (!k) return;
-                            y.push(k), D && (y.push(D), h++)
+                            var k = u(d, b),
+                                E = k[0],
+                                I = k[1];
+                            if (!E) return;
+                            y.push(E), I && (y.push(I), h++)
                         } else y.push(b), S++
                     }
                 }
                 f.push(m), _(f, .75 * c);
                 for (var p = new o(function(y, z) {
                         return Vn.naturalOrder(y.count() * y.volume(), z.count() * z.volume())
                     }); f.size();) p.push(f.pop());
@@ -11440,15 +11440,15 @@
             quality: t
         }),
         o = new Gm(e),
         a = function(u, s, c) {
             for (var d, m, f, _, p, g = u, y = [], z = 0; z < s; z += c) m = g[0 + (d = 4 * z)], f = g[d + 1], _ = g[d + 2], ((p = g[d + 3]) === void 0 || p >= 125) && (m > 250 && f > 250 && _ > 250 || y.push([m, f, _]));
             return y
         }(o.getImageData().data, o.width * o.height, r.quality),
-        l = Gg(a, r.colorCount);
+        l = G0(a, r.colorCount);
     return l ? l.palette() : null
 }, jt.prototype.getColorFromUrl = function(e, n, t) {
     var r = this,
         o = document.createElement("img");
     o.addEventListener("load", function() {
         var a = r.getPalette(o, 5, t);
         n(a[0], e)
@@ -11492,18 +11492,18 @@
     ST = function(e, n) {
         return e ? n ? e.slice(0, n).map(t => t.name).join(" | ") : e.map(t => t.name).join(" | ") : ""
     },
     wT = function(e, n) {
         let t = "";
         return e != null && e.name && (e != null && e.label) ? t = `${e.name}: ${n(e==null?void 0:e.label)}` : e != null && e.name ? t = e.name : e != null && e.label ? t = n(e == null ? void 0 : e.label) : t = e.path || "", t
     },
-    ET = function(e, n = 26) {
+    kT = function(e, n = 26) {
         return e ? e.type != ta.GROUP && e.type != ta.SYNC_GROUP && e.group_childs.length > 1 ? `${Zs(e.display_name,n-3)} +${e.group_childs.length-1}` : Zs(e.display_name, n) : ""
     },
-    kT = function(e) {
+    ET = function(e) {
         const n = [];
         for (const t of (e == null ? void 0 : e.provider_mappings) || []) t.provider_domain.startsWith("filesystem") || t.provider_domain != "plex" && (n.filter(r => r.provider_domain == t.provider_domain).length || n.push(t));
         return n
     },
     AT = e => new Promise(n => setTimeout(n, e));
 
 function PT(e) {
@@ -11518,43 +11518,43 @@
     const t = Qs(e),
         r = Qs(n);
     return t.contrast(r)
 }
 
 function MT(e, n) {
     if (n <= 0 || n > 1) throw new Error("Faktor muss im Bereich von 0 (ausschließlich) bis 1 liegen.");
-    const t = Bg(e),
+    const t = B0(e),
         r = [Math.min(255, Math.round(t[0] + (255 - t[0]) * n)), Math.min(255, Math.round(t[1] + (255 - t[1]) * n)), Math.min(255, Math.round(t[2] + (255 - t[2]) * n))];
     return oi(r)
 }
 
-function Bg(e) {
+function B0(e) {
     const n = parseInt(e.startsWith("#") ? e.slice(1) : e, 16),
         t = n >> 16 & 255,
         r = n >> 8 & 255,
         o = n & 255;
     return [t, r, o]
 }
 
 function oi(e) {
     const [n, t, r] = e;
     return `#${n.toString(16).padStart(2,"0")}${t.toString(16).padStart(2,"0")}${r.toString(16).padStart(2,"0")}`
 }
 
-function Hg(e) {
+function H0(e) {
     let n = "",
         t = 0;
     return e.forEach(r => {
         const o = oi(r),
             a = Bm("#000000", o);
         (a > t && a >= 7 || a > t && a >= t * .7) && (t = a, n = o)
     }), n
 }
 
-function Fg(e) {
+function F0(e) {
     let n = "",
         t = 0;
     const r = 17.35;
     return e.forEach(o => {
         const a = oi(o),
             l = Bm("#fff", a);
         r >= l && (l > t && l >= 7 || l > t && l >= t * .7) && (t = l, n = a)
@@ -11571,41 +11571,41 @@
             c = Math.max(0, a - t),
             d = Math.max(0, l - t);
         return `#${s.toString(16).padStart(2,"0")}${c.toString(16).padStart(2,"0")}${d.toString(16).padStart(2,"0")}`
     }
     return e
 }
 
-function IT(e) {
+function DT(e) {
     const t = new jt().getPalette(e, 5),
         r = t.map(o => oi(o));
     return {
         0: r[0],
         1: r[1],
         2: r[2],
         3: r[3],
         4: r[4],
-        lightColor: Hg(t),
-        darkColor: Fg(t)
+        lightColor: H0(t),
+        darkColor: F0(t)
     }
 }
 
-function DT(e, n) {
+function IT(e, n) {
     if (e) return e;
     for (const t of n) {
         const r = t,
             o = r[0],
             a = r[1],
             l = r[2];
         if (o) return a;
         if (l !== void 0) return l
     }
 }
 
-function Vg(e, n, t) {
+function V0(e, n, t) {
     const r = e.scrollTop,
         o = n - r,
         a = new Date().getTime(),
         l = (s, c, d, m) => (s /= m / 2, s < 1 ? d / 2 * s * s + c : (s--, -d / 2 * (s * (s - 2) - 1) + c)),
         u = () => {
             const c = new Date().getTime() - a;
             e.scrollTop = l(c, r, o, t), c < t ? requestAnimationFrame(u) : e.scrollTop = n
@@ -11667,235 +11667,235 @@
             offset: le.navigationMenuSize
         }) ? 8 : nn({
             breakpoint: "bp10",
             condition: "gt",
             offset: le.navigationMenuSize
         }) ? 9 : 0
     },
-    jg = ["artists", "albums", "tracks", "playlists", "browse"],
-    Ug = [{
+    j0 = ["artists", "albums", "tracks", "playlists", "browse"],
+    U0 = [{
         path: "/",
-        component: () => Se(() => import("./Default-bd92f6cd.js"), ["./Default-bd92f6cd.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./layout-bdc1c8bd.js", "./VBadge-76d9c3a5.js", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./contextmenu-c4231154.js", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css", "./VSelect-ea96d901.js", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./VTabs-4c128c89.js", "./VTabs-11e16be1.css", "./VExpansionPanel-9f82eed8.js", "./VExpansionPanel-00a7e4f4.css", "./Default-abfbb155.css"], import.meta.url),
+        component: () => Se(() => import("./Default-c7088a94.js"), ["./Default-c7088a94.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./layout-42b7d22e.js", "./VBadge-84e3406b.js", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./contextmenu-521b5304.js", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./VSelect-d10e917f.js", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./VTabs-8ad24bfd.js", "./VTabs-11e16be1.css", "./VExpansionPanel-58c5fe02.js", "./VExpansionPanel-00a7e4f4.css", "./Default-2157b447.css"], import.meta.url),
         children: [{
             path: "",
             redirect: "/home",
             name: "homeredirect"
         }, {
             path: "/home",
             name: "home",
-            component: () => Se(() => import("./HomeView-aa005854.js"), ["./HomeView-aa005854.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./VBadge-76d9c3a5.js", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./HomeView-f9b96eef.css"], import.meta.url),
+            component: () => Se(() => import("./HomeView-8f9e6181.js"), ["./HomeView-8f9e6181.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./VBadge-84e3406b.js", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./HomeView-f9b96eef.css"], import.meta.url),
             props: !0
         }, {
             path: "/search",
             name: "search",
-            component: () => Se(() => import("./Search-abd54e1f.js"), ["./Search-abd54e1f.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+            component: () => Se(() => import("./Search-00ee9dd8.js"), ["./Search-00ee9dd8.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
             props: !0
         }, {
             path: "/browse",
             name: "browse",
-            component: () => Se(() => import("./BrowseView-15d25af1.js"), ["./BrowseView-15d25af1.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+            component: () => Se(() => import("./BrowseView-a95cb7cc.js"), ["./BrowseView-a95cb7cc.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
             props: e => ({
                 ...e.query
             })
         }, {
             path: "/artists",
             children: [{
                 path: "",
                 name: "artists",
-                component: () => Se(() => import("./LibraryArtists-17fa3e93.js"), ["./LibraryArtists-17fa3e93.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+                component: () => Se(() => import("./LibraryArtists-9924ed14.js"), ["./LibraryArtists-9924ed14.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
                 props: !0
             }, {
                 path: ":provider/:itemId",
                 name: "artist",
-                component: () => Se(() => import("./ArtistDetails-159c8f35.js"), ["./ArtistDetails-159c8f35.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js", "./layout-bdc1c8bd.js", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
+                component: () => Se(() => import("./ArtistDetails-53ff83d9.js"), ["./ArtistDetails-53ff83d9.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js", "./layout-42b7d22e.js", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
                 props: !0
             }]
         }, {
             path: "/albums",
             children: [{
                 path: "",
                 name: "albums",
-                component: () => Se(() => import("./LibraryAlbums-532f0c88.js"), ["./LibraryAlbums-532f0c88.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+                component: () => Se(() => import("./LibraryAlbums-7cfa0763.js"), ["./LibraryAlbums-7cfa0763.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
                 props: !0
             }, {
                 path: ":provider/:itemId",
                 name: "album",
-                component: () => Se(() => import("./AlbumDetails-25e2fe83.js"), ["./AlbumDetails-25e2fe83.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js", "./layout-bdc1c8bd.js", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
+                component: () => Se(() => import("./AlbumDetails-0b4de4f6.js"), ["./AlbumDetails-0b4de4f6.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js", "./layout-42b7d22e.js", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
                 props: !0
             }]
         }, {
             path: "/tracks",
             children: [{
                 path: "",
                 name: "tracks",
-                component: () => Se(() => import("./LibraryTracks-a533acbe.js"), ["./LibraryTracks-a533acbe.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+                component: () => Se(() => import("./LibraryTracks-eeccb967.js"), ["./LibraryTracks-eeccb967.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
                 props: !0
             }, {
                 path: ":provider/:itemId",
                 name: "track",
-                component: () => Se(() => import("./TrackDetails-6c6c6bec.js"), ["./TrackDetails-6c6c6bec.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js", "./layout-bdc1c8bd.js", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
+                component: () => Se(() => import("./TrackDetails-72029d5e.js"), ["./TrackDetails-72029d5e.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js", "./layout-42b7d22e.js", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
                 props: e => ({
                     ...e.params,
                     ...e.query
                 })
             }]
         }, {
             path: "/playlists",
             children: [{
                 path: "",
                 name: "playlists",
-                component: () => Se(() => import("./LibraryPlaylists-a41d818d.js"), ["./LibraryPlaylists-a41d818d.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+                component: () => Se(() => import("./LibraryPlaylists-95e35cdd.js"), ["./LibraryPlaylists-95e35cdd.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
                 props: !0
             }, {
                 path: ":provider/:itemId",
                 name: "playlist",
-                component: () => Se(() => import("./PlaylistDetails-9db516b0.js"), ["./PlaylistDetails-9db516b0.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js", "./layout-bdc1c8bd.js", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
+                component: () => Se(() => import("./PlaylistDetails-2fe134b1.js"), ["./PlaylistDetails-2fe134b1.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js", "./layout-42b7d22e.js", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
                 props: !0
             }]
         }, {
             path: "/radios",
             children: [{
                 path: "",
                 name: "radios",
-                component: () => Se(() => import("./LibraryRadios-e4468a3f.js"), ["./LibraryRadios-e4468a3f.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+                component: () => Se(() => import("./LibraryRadios-4a033696.js"), ["./LibraryRadios-4a033696.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
                 props: !0
             }, {
                 path: ":provider/:itemId",
                 name: "radio",
-                component: () => Se(() => import("./RadioDetails-87373ab9.js"), ["./RadioDetails-87373ab9.js", "./ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c4231154.js", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js", "./layout-bdc1c8bd.js", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
+                component: () => Se(() => import("./RadioDetails-54e9e340.js"), ["./RadioDetails-54e9e340.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js", "./layout-42b7d22e.js", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
                 props: !0
             }]
         }, {
             path: "/playerqueue",
             name: "playerqueue",
-            component: () => Se(() => import("./PlayerQueue-42cde633.js"), ["./PlayerQueue-42cde633.js", "./ListviewItem-e896b2dc.js", "./VBadge-76d9c3a5.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VBadge-bc81f416.css", "./VTooltip-a8719c72.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VTabs-4c128c89.js", "./VTabs-11e16be1.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css"], import.meta.url),
+            component: () => Se(() => import("./PlayerQueue-9f89c917.js"), ["./PlayerQueue-9f89c917.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VTabs-8ad24bfd.js", "./VTabs-11e16be1.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css"], import.meta.url),
             props: !0
         }, {
             path: "/settings",
             name: "settings",
-            component: () => Se(() => import("./Settings-170b9c4c.js"), ["./Settings-170b9c4c.js", "./VTabs-4c128c89.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VTabs-11e16be1.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css"], import.meta.url),
+            component: () => Se(() => import("./Settings-bbdb2168.js"), ["./Settings-bbdb2168.js", "./VTabs-8ad24bfd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VTabs-11e16be1.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css"], import.meta.url),
             props: !0,
             children: [{
                 path: "providers",
                 name: "providersettings",
-                component: () => Se(() => import("./Providers-ca2eea9e.js"), ["./Providers-ca2eea9e.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./Alert-0c4ec871.js", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./Providers-e2f60749.css"], import.meta.url),
+                component: () => Se(() => import("./Providers-58a591e0.js"), ["./Providers-58a591e0.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./Providers-e2f60749.css"], import.meta.url),
                 props: !0
             }, {
                 path: "players",
                 name: "playersettings",
-                component: () => Se(() => import("./Players-0c4ce7a2.js"), ["./Players-0c4ce7a2.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css"], import.meta.url),
+                component: () => Se(() => import("./Players-0e31a251.js"), ["./Players-0e31a251.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css"], import.meta.url),
                 props: !0
             }, {
                 path: "core",
                 name: "coresettings",
-                component: () => Se(() => import("./CoreConfigs-1f56aa74.js"), ["./CoreConfigs-1f56aa74.js", "./Container-ba274a7a.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VToolbar-4ad3b045.js", "./VToolbar-78a5e824.css", "./CoreConfigs-75569bfe.css"], import.meta.url),
+                component: () => Se(() => import("./CoreConfigs-f0329745.js"), ["./CoreConfigs-f0329745.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./CoreConfigs-75569bfe.css"], import.meta.url),
                 props: !0
             }, {
                 path: "addprovider/:domain",
                 name: "addprovider",
-                component: () => Se(() => import("./AddProvider-b867b6d9.js"), ["./AddProvider-b867b6d9.js", "./index.browser-342e672c.js", "./EditConfig.vue_vue_type_style_index_0_lang-658131e8.js", "./VExpansionPanel-9f82eed8.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-a7262390.js", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VSelect-ea96d901.js", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css"], import.meta.url),
+                component: () => Se(() => import("./AddProvider-f756ebc3.js"), ["./AddProvider-f756ebc3.js", "./index.browser-342e672c.js", "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js", "./VExpansionPanel-58c5fe02.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-fc99b4aa.js", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VSelect-d10e917f.js", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css"], import.meta.url),
                 props: !0
             }, {
                 path: "editprovider/:instanceId",
                 name: "editprovider",
-                component: () => Se(() => import("./EditProvider-b281ecba.js"), ["./EditProvider-b281ecba.js", "./EditConfig.vue_vue_type_style_index_0_lang-658131e8.js", "./VExpansionPanel-9f82eed8.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-a7262390.js", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VSelect-ea96d901.js", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css", "./index.browser-342e672c.js"], import.meta.url),
+                component: () => Se(() => import("./EditProvider-e046ee5d.js"), ["./EditProvider-e046ee5d.js", "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js", "./VExpansionPanel-58c5fe02.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-fc99b4aa.js", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VSelect-d10e917f.js", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css", "./index.browser-342e672c.js"], import.meta.url),
                 props: !0
             }, {
                 path: "editplayer/:playerId",
                 name: "editplayer",
-                component: () => Se(() => import("./EditPlayer-293a9fdd.js"), ["./EditPlayer-293a9fdd.js", "./EditConfig.vue_vue_type_style_index_0_lang-658131e8.js", "./VExpansionPanel-9f82eed8.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-a7262390.js", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VSelect-ea96d901.js", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css"], import.meta.url),
+                component: () => Se(() => import("./EditPlayer-6e04043d.js"), ["./EditPlayer-6e04043d.js", "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js", "./VExpansionPanel-58c5fe02.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-fc99b4aa.js", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VSelect-d10e917f.js", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css"], import.meta.url),
                 props: !0
             }, {
                 path: "editcore/:domain",
                 name: "editcore",
-                component: () => Se(() => import("./EditCoreConfig-db86c453.js"), ["./EditCoreConfig-db86c453.js", "./EditConfig.vue_vue_type_style_index_0_lang-658131e8.js", "./VExpansionPanel-9f82eed8.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VMenu-9506155f.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-a7262390.js", "./VCard-bfc4071a.js", "./VCardText-00c669eb.js", "./VCard-257d0eab.css", "./VDialog-82ed2e80.js", "./VDialog-5309eac2.css", "./VAlert-f74a2b4b.js", "./VAlert-1c823677.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VSelect-ea96d901.js", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css", "./index.browser-342e672c.js"], import.meta.url),
+                component: () => Se(() => import("./EditCoreConfig-d27a9b35.js"), ["./EditCoreConfig-d27a9b35.js", "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js", "./VExpansionPanel-58c5fe02.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-fc99b4aa.js", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VSelect-d10e917f.js", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css", "./index.browser-342e672c.js"], import.meta.url),
                 props: !0
             }, {
                 path: "addgroup/:provider",
                 name: "addgroup",
-                component: () => Se(() => import("./AddGroupPlayer-f291ae3b.js"), ["./AddGroupPlayer-f291ae3b.js", "./VCardText-00c669eb.js", "./VMenu-9506155f.js", "./forwardRefs-70e877d2.js", "./forwardRefs-e5b3781d.css", "./VMenu-a46f5e7a.css", "./VForm-a7262390.js", "./VInput-91b2e758.js", "./VSlideGroup-5dd0c6f2.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VTextField-8883f272.js", "./VTextField-d31117f3.css", "./VSelect-ea96d901.js", "./VVirtualScroll-5f35af5d.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css"], import.meta.url),
+                component: () => Se(() => import("./AddGroupPlayer-8a4f0893.js"), ["./AddGroupPlayer-8a4f0893.js", "./VCardText-6774ea5e.js", "./VMenu-b634019c.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-a46f5e7a.css", "./VForm-fc99b4aa.js", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VSelect-d10e917f.js", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css"], import.meta.url),
                 props: !0
             }, {
                 path: "",
                 redirect: "/settings/providers",
                 name: "settingsredirect"
             }]
         }]
     }],
-    al = mg({
-        history: H0(),
-        routes: Ug
+    al = m0({
+        history: Hg(),
+        routes: U0
     });
 al.beforeEach((e, n) => {
-    if (!(n != null && n.name) || !jg.includes(n.name.toString())) return;
+    if (!(n != null && n.name) || !j0.includes(n.name.toString())) return;
     const t = document.querySelector("#cont");
     t && (le.prevScrollPos = t.scrollTop), le.prevScrollName = n.name.toString()
 });
 al.afterEach((e, n) => {
     n != null && n.name && e != null && e.name && le.prevScrollName && le.prevScrollName == e.name && Vr(() => {
         const t = document.getElementById("cont");
         setTimeout(() => {
-            t && le.prevScrollPos && Vg(t, le.prevScrollPos, 1e3), le.prevScrollName = void 0, le.prevScrollPos = void 0
+            t && le.prevScrollPos && V0(t, le.prevScrollPos, 1e3), le.prevScrollName = void 0, le.prevScrollPos = void 0
         }, 400)
     })
 });
 /*!
  * shared v9.12.1
  * (c) 2024 kazuya kawaguchi
  * Released under the MIT License.
  */
-const Io = typeof window < "u",
+const Do = typeof window < "u",
     ft = (e, n = !1) => n ? Symbol.for(e) : Symbol(e),
-    qg = (e, n, t) => Wg({
+    q0 = (e, n, t) => W0({
         l: e,
         k: n,
         s: t
     }),
-    Wg = e => JSON.stringify(e).replace(/\u2028/g, "\\u2028").replace(/\u2029/g, "\\u2029").replace(/\u0027/g, "\\u0027"),
+    W0 = e => JSON.stringify(e).replace(/\u2028/g, "\\u2028").replace(/\u2029/g, "\\u2029").replace(/\u0027/g, "\\u0027"),
     Be = e => typeof e == "number" && isFinite(e),
-    $g = e => Fm(e) === "[object Date]",
-    Do = e => Fm(e) === "[object RegExp]",
+    $0 = e => Fm(e) === "[object Date]",
+    Io = e => Fm(e) === "[object RegExp]",
     ii = e => de(e) && Object.keys(e).length === 0,
     Ke = Object.assign;
 let Js;
 const ll = () => Js || (Js = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {});
 
 function eu(e) {
     return e.replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;").replace(/'/g, "&apos;")
 }
-const Kg = Object.prototype.hasOwnProperty;
+const K0 = Object.prototype.hasOwnProperty;
 
 function Lo(e, n) {
-    return Kg.call(e, n)
+    return K0.call(e, n)
 }
 const xe = Array.isArray,
     Pe = e => typeof e == "function",
     Q = e => typeof e == "string",
     we = e => typeof e == "boolean",
     _e = e => e !== null && typeof e == "object",
-    Xg = e => _e(e) && Pe(e.then) && Pe(e.catch),
+    X0 = e => _e(e) && Pe(e.then) && Pe(e.catch),
     Hm = Object.prototype.toString,
     Fm = e => Hm.call(e),
     de = e => {
         if (!_e(e)) return !1;
         const n = Object.getPrototypeOf(e);
         return n === null || n.constructor === Object
     },
-    Yg = e => e == null ? "" : xe(e) || de(e) && e.toString === Hm ? JSON.stringify(e, null, 2) : String(e);
+    Y0 = e => e == null ? "" : xe(e) || de(e) && e.toString === Hm ? JSON.stringify(e, null, 2) : String(e);
 
-function Qg(e, n = "") {
+function Q0(e, n = "") {
     return e.reduce((t, r, o) => o === 0 ? t + r : t + n + r, "")
 }
 
 function ai(e) {
     let n = e;
     return () => ++n
 }
 
-function Zg(e, n) {
+function Z0(e, n) {
     typeof console < "u" && (console.warn("[intlify] " + e), n && console.warn(n.stack))
 }
 const lo = e => !_e(e) || xe(e);
 
 function zo(e, n) {
     if (lo(e) || lo(n)) throw new Error("Invalid value");
     const t = [{
@@ -11916,15 +11916,15 @@
     }
 }
 /*!
  * message-compiler v9.12.1
  * (c) 2024 kazuya kawaguchi
  * Released under the MIT License.
  */
-function Jg(e, n, t) {
+function J0(e, n, t) {
     return {
         line: e,
         column: n,
         offset: t
     }
 }
 
@@ -12022,24 +12022,24 @@
 
 function ub(e) {
     const n = e;
     let t = 0,
         r = 1,
         o = 1,
         a = 0;
-    const l = D => n[D] === ab && n[D + 1] === Ze,
-        u = D => n[D] === Ze,
-        s = D => n[D] === sb,
-        c = D => n[D] === lb,
-        d = D => l(D) || u(D) || s(D) || c(D),
+    const l = I => n[I] === ab && n[I + 1] === Ze,
+        u = I => n[I] === Ze,
+        s = I => n[I] === sb,
+        c = I => n[I] === lb,
+        d = I => l(I) || u(I) || s(I) || c(I),
         m = () => t,
         f = () => r,
         _ = () => o,
         p = () => a,
-        g = D => l(D) || s(D) || c(D) ? Ze : n[D],
+        g = I => l(I) || s(I) || c(I) ? Ze : n[I],
         y = () => g(t),
         z = () => g(t + a);
 
     function b() {
         return a = 0, d(t) && (r++, o = 0), l(t) && t++, t++, o++, n[t]
     }
 
@@ -12047,48 +12047,48 @@
         return l(t + a) && a++, a++, n[t + a]
     }
 
     function S() {
         t = 0, r = 1, o = 1, a = 0
     }
 
-    function E(D = 0) {
-        a = D
+    function k(I = 0) {
+        a = I
     }
 
-    function k() {
-        const D = t + a;
-        for (; D !== t;) b();
+    function E() {
+        const I = t + a;
+        for (; I !== t;) b();
         a = 0
     }
     return {
         index: m,
         line: f,
         column: _,
         peekOffset: p,
         charAt: g,
         currentChar: y,
         currentPeek: z,
         next: b,
         peek: h,
         reset: S,
-        resetPeek: E,
-        skipToPeek: k
+        resetPeek: k,
+        skipToPeek: E
     }
 }
 const Zn = void 0,
     cb = ".",
     tu = "'",
     mb = "tokenizer";
 
 function db(e, n = {}) {
     const t = n.location !== !1,
         r = ub(e),
         o = () => r.index(),
-        a = () => Jg(r.line(), r.column(), r.index()),
+        a = () => J0(r.line(), r.column(), r.index()),
         l = a(),
         u = o(),
         s = {
             currentType: 14,
             offset: u,
             startLoc: l,
             endLoc: l,
@@ -12105,19 +12105,19 @@
             onError: d
         } = n;
 
     function m(v, T, C, ...G) {
         const q = c();
         if (T.column += C, T.offset += C, d) {
             const j = t ? Oo(q.startLoc, T) : null,
-                I = cr(v, j, {
+                D = cr(v, j, {
                     domain: mb,
                     args: G
                 });
-            d(I)
+            d(D)
         }
     }
 
     function f(v, T, C) {
         v.endLoc = a(), v.currentType = T;
         const G = {
             type: T
@@ -12170,35 +12170,35 @@
         if (C !== 2) return !1;
         g(v);
         const G = v.currentPeek() === "-" ? v.peek() : v.currentPeek(),
             q = b(G);
         return v.resetPeek(), q
     }
 
-    function E(v, T) {
+    function k(v, T) {
         const {
             currentType: C
         } = T;
         if (C !== 2) return !1;
         g(v);
         const G = v.currentPeek() === tu;
         return v.resetPeek(), G
     }
 
-    function k(v, T) {
+    function E(v, T) {
         const {
             currentType: C
         } = T;
         if (C !== 8) return !1;
         g(v);
         const G = v.currentPeek() === ".";
         return v.resetPeek(), G
     }
 
-    function D(v, T) {
+    function I(v, T) {
         const {
             currentType: C
         } = T;
         if (C !== 9) return !1;
         g(v);
         const G = z(v.currentPeek());
         return v.resetPeek(), G
@@ -12239,17 +12239,17 @@
         return v.resetPeek(), {
             isModulo: C,
             hasSpace: T.length > 0
         }
     }
 
     function O(v, T = !0) {
-        const C = (q = !1, j = "", I = !1) => {
+        const C = (q = !1, j = "", D = !1) => {
                 const R = v.currentPeek();
-                return R === "{" ? j === "%" ? !1 : q : R === "@" || !R ? j === "%" ? !0 : q : R === "%" ? (v.peek(), C(q, "%", !0)) : R === "|" ? j === "%" || I ? !0 : !(j === Gn || j === Ze) : R === Gn ? (v.peek(), C(!0, Gn, I)) : R === Ze ? (v.peek(), C(!0, Ze, I)) : !0
+                return R === "{" ? j === "%" ? !1 : q : R === "@" || !R ? j === "%" ? !0 : q : R === "%" ? (v.peek(), C(q, "%", !0)) : R === "|" ? j === "%" || D ? !0 : !(j === Gn || j === Ze) : R === Gn ? (v.peek(), C(!0, Gn, D)) : R === Ze ? (v.peek(), C(!0, Ze, D)) : !0
             },
             G = C();
         return T && v.resetPeek(), G
     }
 
     function V(v, T) {
         const C = v.currentChar();
@@ -12284,19 +12284,19 @@
     }
 
     function Xe(v) {
         const T = v.charCodeAt(0);
         return T >= 48 && T <= 57 || T >= 65 && T <= 70 || T >= 97 && T <= 102
     }
 
-    function Ee(v) {
+    function ke(v) {
         return V(v, Xe)
     }
 
-    function ke(v) {
+    function Ee(v) {
         let T = "",
             C = "";
         for (; T = Ue(v);) C += T;
         return C
     }
 
     function Mn(v) {
@@ -12331,15 +12331,15 @@
         for (; T = se(v);) C += T;
         return v.currentChar() === Zn && m(ne.UNTERMINATED_CLOSING_BRACE, a(), 0), C
     }
 
     function Ce(v) {
         y(v);
         let T = "";
-        return v.currentChar() === "-" ? (v.next(), T += `-${ke(v)}`) : T += ke(v), v.currentChar() === Zn && m(ne.UNTERMINATED_CLOSING_BRACE, a(), 0), T
+        return v.currentChar() === "-" ? (v.next(), T += `-${Ee(v)}`) : T += Ee(v), v.currentChar() === Zn && m(ne.UNTERMINATED_CLOSING_BRACE, a(), 0), T
     }
 
     function B(v) {
         return v !== tu && v !== Ze
     }
 
     function K(v) {
@@ -12366,15 +12366,15 @@
         }
     }
 
     function X(v, T, C) {
         p(v, T);
         let G = "";
         for (let q = 0; q < C; q++) {
-            const j = Ee(v);
+            const j = ke(v);
             if (!j) {
                 m(ne.INVALID_UNICODE_ESCAPE_SEQUENCE, a(), 0, `\\${T}${G}${v.currentChar()}`);
                 break
             }
             G += j
         }
         return `\\${T}${G}`
@@ -12421,21 +12421,21 @@
             case "}":
                 return T.braceNest > 0 && T.currentType === 2 && m(ne.EMPTY_PLACEHOLDER, a(), 0), v.next(), C = f(T, 3, "}"), T.braceNest--, T.braceNest > 0 && y(v), T.inLinked && T.braceNest === 0 && (T.inLinked = !1), C;
             case "@":
                 return T.braceNest > 0 && m(ne.UNTERMINATED_CLOSING_BRACE, a(), 0), C = N(v, T) || _(T), T.braceNest = 0, C;
             default: {
                 let q = !0,
                     j = !0,
-                    I = !0;
+                    D = !0;
                 if (L(v)) return T.braceNest > 0 && m(ne.UNTERMINATED_CLOSING_BRACE, a(), 0), C = f(T, 1, x(v)), T.braceNest = 0, T.inLinked = !1, C;
                 if (T.braceNest > 0 && (T.currentType === 5 || T.currentType === 6 || T.currentType === 7)) return m(ne.UNTERMINATED_CLOSING_BRACE, a(), 0), T.braceNest = 0, U(v, T);
                 if (q = h(v, T)) return C = f(T, 5, Kn(v)), y(v), C;
                 if (j = S(v, T)) return C = f(T, 6, Ce(v)), y(v), C;
-                if (I = E(v, T)) return C = f(T, 7, K(v)), y(v), C;
-                if (!q && !j && !I) return C = f(T, 13, ze(v)), m(ne.INVALID_TOKEN_IN_PLACEHOLDER, a(), 0, C.value), y(v), C;
+                if (D = k(v, T)) return C = f(T, 7, K(v)), y(v), C;
+                if (!q && !j && !D) return C = f(T, 13, ze(v)), m(ne.INVALID_TOKEN_IN_PLACEHOLDER, a(), 0, C.value), y(v), C;
                 break
             }
         }
         return C
     }
 
     function N(v, T) {
@@ -12448,15 +12448,15 @@
             case "@":
                 return v.next(), G = f(T, 8, "@"), T.inLinked = !0, G;
             case ".":
                 return y(v), v.next(), f(T, 9, ".");
             case ":":
                 return y(v), v.next(), f(T, 10, ":");
             default:
-                return L(v) ? (G = f(T, 1, x(v)), T.braceNest = 0, T.inLinked = !1, G) : k(v, T) || P(v, T) ? (y(v), N(v, T)) : D(v, T) ? (y(v), f(T, 12, w(v))) : M(v, T) ? (y(v), q === "{" ? H(v, T) || G : f(T, 11, A(v))) : (C === 8 && m(ne.INVALID_LINKED_FORMAT, a(), 0), T.braceNest = 0, T.inLinked = !1, U(v, T))
+                return L(v) ? (G = f(T, 1, x(v)), T.braceNest = 0, T.inLinked = !1, G) : E(v, T) || P(v, T) ? (y(v), N(v, T)) : I(v, T) ? (y(v), f(T, 12, w(v))) : M(v, T) ? (y(v), q === "{" ? H(v, T) || G : f(T, 11, A(v))) : (C === 8 && m(ne.INVALID_LINKED_FORMAT, a(), 0), T.braceNest = 0, T.inLinked = !1, U(v, T))
         }
     }
 
     function U(v, T) {
         let C = {
             type: 14
         };
@@ -12518,207 +12518,207 @@
 function zb(e = {}) {
     const n = e.location !== !1,
         {
             onError: t,
             onWarn: r
         } = e;
 
-    function o(h, S, E, k, ...D) {
+    function o(h, S, k, E, ...I) {
         const P = h.currentPosition();
-        if (P.offset += k, P.column += k, t) {
-            const M = n ? Oo(E, P) : null,
+        if (P.offset += E, P.column += E, t) {
+            const M = n ? Oo(k, P) : null,
                 L = cr(S, M, {
                     domain: fb,
-                    args: D
+                    args: I
                 });
             t(L)
         }
     }
 
-    function a(h, S, E, k, ...D) {
+    function a(h, S, k, E, ...I) {
         const P = h.currentPosition();
-        if (P.offset += k, P.column += k, r) {
-            const M = n ? Oo(E, P) : null;
-            r(rb(S, M, D))
+        if (P.offset += E, P.column += E, r) {
+            const M = n ? Oo(k, P) : null;
+            r(rb(S, M, I))
         }
     }
 
-    function l(h, S, E) {
-        const k = {
+    function l(h, S, k) {
+        const E = {
             type: h
         };
-        return n && (k.start = S, k.end = S, k.loc = {
-            start: E,
-            end: E
-        }), k
+        return n && (E.start = S, E.end = S, E.loc = {
+            start: k,
+            end: k
+        }), E
     }
 
-    function u(h, S, E, k) {
-        k && (h.type = k), n && (h.end = S, h.loc && (h.loc.end = E))
+    function u(h, S, k, E) {
+        E && (h.type = E), n && (h.end = S, h.loc && (h.loc.end = k))
     }
 
     function s(h, S) {
-        const E = h.context(),
-            k = l(3, E.offset, E.startLoc);
-        return k.value = S, u(k, h.currentOffset(), h.currentPosition()), k
+        const k = h.context(),
+            E = l(3, k.offset, k.startLoc);
+        return E.value = S, u(E, h.currentOffset(), h.currentPosition()), E
     }
 
     function c(h, S) {
-        const E = h.context(),
+        const k = h.context(),
             {
-                lastOffset: k,
-                lastStartLoc: D
-            } = E,
-            P = l(5, k, D);
+                lastOffset: E,
+                lastStartLoc: I
+            } = k,
+            P = l(5, E, I);
         return P.index = parseInt(S, 10), h.nextToken(), u(P, h.currentOffset(), h.currentPosition()), P
     }
 
-    function d(h, S, E) {
-        const k = h.context(),
+    function d(h, S, k) {
+        const E = h.context(),
             {
-                lastOffset: D,
+                lastOffset: I,
                 lastStartLoc: P
-            } = k,
-            M = l(4, D, P);
-        return M.key = S, E === !0 && (M.modulo = !0), h.nextToken(), u(M, h.currentOffset(), h.currentPosition()), M
+            } = E,
+            M = l(4, I, P);
+        return M.key = S, k === !0 && (M.modulo = !0), h.nextToken(), u(M, h.currentOffset(), h.currentPosition()), M
     }
 
     function m(h, S) {
-        const E = h.context(),
+        const k = h.context(),
             {
-                lastOffset: k,
-                lastStartLoc: D
-            } = E,
-            P = l(9, k, D);
+                lastOffset: E,
+                lastStartLoc: I
+            } = k,
+            P = l(9, E, I);
         return P.value = S.replace(_b, pb), h.nextToken(), u(P, h.currentOffset(), h.currentPosition()), P
     }
 
     function f(h) {
         const S = h.nextToken(),
-            E = h.context(),
+            k = h.context(),
             {
-                lastOffset: k,
-                lastStartLoc: D
-            } = E,
-            P = l(8, k, D);
-        return S.type !== 12 ? (o(h, ne.UNEXPECTED_EMPTY_LINKED_MODIFIER, E.lastStartLoc, 0), P.value = "", u(P, k, D), {
+                lastOffset: E,
+                lastStartLoc: I
+            } = k,
+            P = l(8, E, I);
+        return S.type !== 12 ? (o(h, ne.UNEXPECTED_EMPTY_LINKED_MODIFIER, k.lastStartLoc, 0), P.value = "", u(P, E, I), {
             nextConsumeToken: S,
             node: P
-        }) : (S.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, E.lastStartLoc, 0, wn(S)), P.value = S.value || "", u(P, h.currentOffset(), h.currentPosition()), {
+        }) : (S.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, k.lastStartLoc, 0, wn(S)), P.value = S.value || "", u(P, h.currentOffset(), h.currentPosition()), {
             node: P
         })
     }
 
     function _(h, S) {
-        const E = h.context(),
-            k = l(7, E.offset, E.startLoc);
-        return k.value = S, u(k, h.currentOffset(), h.currentPosition()), k
+        const k = h.context(),
+            E = l(7, k.offset, k.startLoc);
+        return E.value = S, u(E, h.currentOffset(), h.currentPosition()), E
     }
 
     function p(h) {
         const S = h.context(),
-            E = l(6, S.offset, S.startLoc);
-        let k = h.nextToken();
-        if (k.type === 9) {
-            const D = f(h);
-            E.modifier = D.node, k = D.nextConsumeToken || h.nextToken()
+            k = l(6, S.offset, S.startLoc);
+        let E = h.nextToken();
+        if (E.type === 9) {
+            const I = f(h);
+            k.modifier = I.node, E = I.nextConsumeToken || h.nextToken()
         }
-        switch (k.type !== 10 && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(k)), k = h.nextToken(), k.type === 2 && (k = h.nextToken()), k.type) {
+        switch (E.type !== 10 && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(E)), E = h.nextToken(), E.type === 2 && (E = h.nextToken()), E.type) {
             case 11:
-                k.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(k)), E.key = _(h, k.value || "");
+                E.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(E)), k.key = _(h, E.value || "");
                 break;
             case 5:
-                k.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(k)), E.key = d(h, k.value || "");
+                E.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(E)), k.key = d(h, E.value || "");
                 break;
             case 6:
-                k.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(k)), E.key = c(h, k.value || "");
+                E.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(E)), k.key = c(h, E.value || "");
                 break;
             case 7:
-                k.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(k)), E.key = m(h, k.value || "");
+                E.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(E)), k.key = m(h, E.value || "");
                 break;
             default: {
                 o(h, ne.UNEXPECTED_EMPTY_LINKED_KEY, S.lastStartLoc, 0);
-                const D = h.context(),
-                    P = l(7, D.offset, D.startLoc);
-                return P.value = "", u(P, D.offset, D.startLoc), E.key = P, u(E, D.offset, D.startLoc), {
-                    nextConsumeToken: k,
-                    node: E
+                const I = h.context(),
+                    P = l(7, I.offset, I.startLoc);
+                return P.value = "", u(P, I.offset, I.startLoc), k.key = P, u(k, I.offset, I.startLoc), {
+                    nextConsumeToken: E,
+                    node: k
                 }
             }
         }
-        return u(E, h.currentOffset(), h.currentPosition()), {
-            node: E
+        return u(k, h.currentOffset(), h.currentPosition()), {
+            node: k
         }
     }
 
     function g(h) {
         const S = h.context(),
-            E = S.currentType === 1 ? h.currentOffset() : S.offset,
-            k = S.currentType === 1 ? S.endLoc : S.startLoc,
-            D = l(2, E, k);
-        D.items = [];
+            k = S.currentType === 1 ? h.currentOffset() : S.offset,
+            E = S.currentType === 1 ? S.endLoc : S.startLoc,
+            I = l(2, k, E);
+        I.items = [];
         let P = null,
             M = null;
         do {
             const O = P || h.nextToken();
             switch (P = null, O.type) {
                 case 0:
-                    O.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(O)), D.items.push(s(h, O.value || ""));
+                    O.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(O)), I.items.push(s(h, O.value || ""));
                     break;
                 case 6:
-                    O.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(O)), D.items.push(c(h, O.value || ""));
+                    O.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(O)), I.items.push(c(h, O.value || ""));
                     break;
                 case 4:
                     M = !0;
                     break;
                 case 5:
-                    O.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(O)), D.items.push(d(h, O.value || "", !!M)), M && (a(h, sl.USE_MODULO_SYNTAX, S.lastStartLoc, 0, wn(O)), M = null);
+                    O.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(O)), I.items.push(d(h, O.value || "", !!M)), M && (a(h, sl.USE_MODULO_SYNTAX, S.lastStartLoc, 0, wn(O)), M = null);
                     break;
                 case 7:
-                    O.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(O)), D.items.push(m(h, O.value || ""));
+                    O.value == null && o(h, ne.UNEXPECTED_LEXICAL_ANALYSIS, S.lastStartLoc, 0, wn(O)), I.items.push(m(h, O.value || ""));
                     break;
                 case 8: {
                     const V = p(h);
-                    D.items.push(V.node), P = V.nextConsumeToken || null;
+                    I.items.push(V.node), P = V.nextConsumeToken || null;
                     break
                 }
             }
         } while (S.currentType !== 14 && S.currentType !== 1);
         const L = S.currentType === 1 ? S.lastOffset : h.currentOffset(),
             F = S.currentType === 1 ? S.lastEndLoc : h.currentPosition();
-        return u(D, L, F), D
+        return u(I, L, F), I
     }
 
-    function y(h, S, E, k) {
-        const D = h.context();
-        let P = k.items.length === 0;
-        const M = l(1, S, E);
-        M.cases = [], M.cases.push(k);
+    function y(h, S, k, E) {
+        const I = h.context();
+        let P = E.items.length === 0;
+        const M = l(1, S, k);
+        M.cases = [], M.cases.push(E);
         do {
             const L = g(h);
             P || (P = L.items.length === 0), M.cases.push(L)
-        } while (D.currentType !== 14);
-        return P && o(h, ne.MUST_HAVE_MESSAGES_IN_PLURAL, E, 0), u(M, h.currentOffset(), h.currentPosition()), M
+        } while (I.currentType !== 14);
+        return P && o(h, ne.MUST_HAVE_MESSAGES_IN_PLURAL, k, 0), u(M, h.currentOffset(), h.currentPosition()), M
     }
 
     function z(h) {
         const S = h.context(),
             {
-                offset: E,
-                startLoc: k
+                offset: k,
+                startLoc: E
             } = S,
-            D = g(h);
-        return S.currentType === 14 ? D : y(h, E, k, D)
+            I = g(h);
+        return S.currentType === 14 ? I : y(h, k, E, I)
     }
 
     function b(h) {
         const S = db(h, jm({}, e)),
-            E = S.context(),
-            k = l(0, E.offset, E.startLoc);
-        return n && k.loc && (k.loc.source = h), k.body = z(S), e.onCacheKey && (k.cacheKey = e.onCacheKey(h)), E.currentType !== 14 && o(S, ne.UNEXPECTED_LEXICAL_ANALYSIS, E.lastStartLoc, 0, h[E.offset] || ""), u(k, S.currentOffset(), S.currentPosition()), k
+            k = S.context(),
+            E = l(0, k.offset, k.startLoc);
+        return n && E.loc && (E.loc.source = h), E.body = z(S), e.onCacheKey && (E.cacheKey = e.onCacheKey(h)), k.currentType !== 14 && o(S, ne.UNEXPECTED_LEXICAL_ANALYSIS, k.lastStartLoc, 0, h[k.offset] || ""), u(E, S.currentOffset(), S.currentPosition()), E
     }
     return {
         parse: b
     }
 }
 
 function wn(e) {
@@ -12918,41 +12918,41 @@
     } = e;
     e.push(`${t("normalize")}([`), e.indent(r());
     const o = n.items.length;
     for (let a = 0; a < o && (ir(e, n.items[a]), a !== o - 1); a++) e.push(", ");
     e.deindent(r()), e.push("])")
 }
 
-function Eb(e, n) {
+function kb(e, n) {
     const {
         helper: t,
         needIndent: r
     } = e;
     if (n.cases.length > 1) {
         e.push(`${t("plural")}([`), e.indent(r());
         const o = n.cases.length;
         for (let a = 0; a < o && (ir(e, n.cases[a]), a !== o - 1); a++) e.push(", ");
         e.deindent(r()), e.push("])")
     }
 }
 
-function kb(e, n) {
+function Eb(e, n) {
     n.body ? ir(e, n.body) : e.push("null")
 }
 
 function ir(e, n) {
     const {
         helper: t
     } = e;
     switch (n.type) {
         case 0:
-            kb(e, n);
+            Eb(e, n);
             break;
         case 1:
-            Eb(e, n);
+            kb(e, n);
             break;
         case 2:
             wb(e, n);
             break;
         case 6:
             Sb(e, n);
             break;
@@ -13069,19 +13069,19 @@
 _t[6] = {
     '"': [4, 0],
     o: 8,
     l: [6, 0]
 };
 const Cb = /^\s?(?:true|false|-?[\d.]+|'[^']*'|"[^"]*")\s?$/;
 
-function Ib(e) {
+function Db(e) {
     return Cb.test(e)
 }
 
-function Db(e) {
+function Ib(e) {
     const n = e.charCodeAt(0),
         t = e.charCodeAt(e.length - 1);
     return n === t && (n === 34 || n === 39) ? e.slice(1, -1) : e
 }
 
 function Lb(e) {
     if (e == null) return "o";
@@ -13106,15 +13106,15 @@
             return "w"
     }
     return "i"
 }
 
 function Ob(e) {
     const n = e.trim();
-    return e.charAt(0) === "0" && isNaN(parseInt(e)) ? !1 : Ib(n) ? Db(n) : "*" + n
+    return e.charAt(0) === "0" && isNaN(parseInt(e)) ? !1 : Db(n) ? Ib(n) : "*" + n
 }
 
 function xb(e) {
     const n = [];
     let t = -1,
         r = 0,
         o = 0,
@@ -13163,16 +13163,16 @@
         o = l, a++
     }
     return o
 }
 const Gb = e => e,
     Bb = e => "",
     Hb = "text",
-    Fb = e => e.length === 0 ? "" : Qg(e),
-    Vb = Yg;
+    Fb = e => e.length === 0 ? "" : Q0(e),
+    Vb = Y0;
 
 function au(e, n) {
     return e = Math.abs(e), n === 2 ? e ? e > 1 ? 1 : 0 : 1 : e ? Math.min(e, 2) : 0
 }
 
 function jb(e) {
     const n = Be(e.pluralIndex) ? e.pluralIndex : -1;
@@ -13205,20 +13205,20 @@
         p = de(e.processor) && Q(e.processor.type) ? e.processor.type : Hb,
         y = {
             list: u,
             named: c,
             plural: a,
             linked: (z, ...b) => {
                 const [h, S] = b;
-                let E = "text",
-                    k = "";
-                b.length === 1 ? _e(h) ? (k = h.modifier || k, E = h.type || E) : Q(h) && (k = h || k) : b.length === 2 && (Q(h) && (k = h || k), Q(S) && (E = S || E));
-                const D = d(z)(y),
-                    P = E === "vnode" && xe(D) && k ? D[0] : D;
-                return k ? m(k)(P, E) : P
+                let k = "text",
+                    E = "";
+                b.length === 1 ? _e(h) ? (E = h.modifier || E, k = h.type || k) : Q(h) && (E = h || E) : b.length === 2 && (Q(h) && (E = h || E), Q(S) && (k = S || k));
+                const I = d(z)(y),
+                    P = k === "vnode" && xe(I) && E ? I[0] : I;
+                return E ? m(E)(P, k) : P
             },
             message: d,
             type: p,
             interpolate: _,
             normalize: f,
             values: Ke({}, l, s)
         };
@@ -13279,15 +13279,15 @@
 
 function lu(e) {
     if (Q(e)) return e;
     if (Pe(e)) {
         if (e.resolvedOnce && Pi != null) return Pi;
         if (e.constructor.name === "Function") {
             const n = e();
-            if (Xg(n)) throw Un(On.NOT_SUPPORT_LOCALE_PROMISE_VALUE);
+            if (X0(n)) throw Un(On.NOT_SUPPORT_LOCALE_PROMISE_VALUE);
             return Pi = n
         } else throw Un(On.NOT_SUPPORT_LOCALE_ASYNC_FUNCTION)
     } else throw Un(On.NOT_SUPPORT_LOCALE_TYPE)
 }
 
 function Qb(e, n, t) {
     return [...new Set([t, ...xe(n) ? n : _e(n) ? Object.keys(n) : Q(n) ? [n] : [t]])]
@@ -13373,15 +13373,15 @@
 const mu = e => {
         Zm = e
     },
     lv = () => Zm;
 let du = 0;
 
 function sv(e = {}) {
-    const n = Pe(e.onWarn) ? e.onWarn : Zg,
+    const n = Pe(e.onWarn) ? e.onWarn : Z0,
         t = Q(e.version) ? e.version : ev,
         r = Q(e.locale) || Pe(e.locale) ? e.locale : xo,
         o = Pe(r) ? xo : r,
         a = xe(e.fallbackLocale) || de(e.fallbackLocale) || Q(e.fallbackLocale) || e.fallbackLocale === !1 ? e.fallbackLocale : o,
         l = de(e.messages) ? e.messages : {
             [o]: {}
         },
@@ -13390,26 +13390,26 @@
         },
         s = de(e.numberFormats) ? e.numberFormats : {
             [o]: {}
         },
         c = Ke({}, e.modifiers || {}, nv()),
         d = e.pluralRules || {},
         m = Pe(e.missing) ? e.missing : null,
-        f = we(e.missingWarn) || Do(e.missingWarn) ? e.missingWarn : !0,
-        _ = we(e.fallbackWarn) || Do(e.fallbackWarn) ? e.fallbackWarn : !0,
+        f = we(e.missingWarn) || Io(e.missingWarn) ? e.missingWarn : !0,
+        _ = we(e.fallbackWarn) || Io(e.fallbackWarn) ? e.fallbackWarn : !0,
         p = !!e.fallbackFormat,
         g = !!e.unresolving,
         y = Pe(e.postTranslation) ? e.postTranslation : null,
         z = de(e.processor) ? e.processor : null,
         b = we(e.warnHtmlMessage) ? e.warnHtmlMessage : !0,
         h = !!e.escapeParameter,
         S = Pe(e.messageCompiler) ? e.messageCompiler : Km,
-        E = Pe(e.messageResolver) ? e.messageResolver : Xm || Rb,
-        k = Pe(e.localeFallbacker) ? e.localeFallbacker : Ym || Qb,
-        D = _e(e.fallbackContext) ? e.fallbackContext : void 0,
+        k = Pe(e.messageResolver) ? e.messageResolver : Xm || Rb,
+        E = Pe(e.localeFallbacker) ? e.localeFallbacker : Ym || Qb,
+        I = _e(e.fallbackContext) ? e.fallbackContext : void 0,
         P = e,
         M = _e(P.__datetimeFormatters) ? P.__datetimeFormatters : new Map,
         L = _e(P.__numberFormatters) ? P.__numberFormatters : new Map,
         F = _e(P.__meta) ? P.__meta : {};
     du++;
     const O = {
         version: t,
@@ -13425,17 +13425,17 @@
         fallbackFormat: p,
         unresolving: g,
         postTranslation: y,
         processor: z,
         warnHtmlMessage: b,
         escapeParameter: h,
         messageCompiler: S,
-        messageResolver: E,
-        localeFallbacker: k,
-        fallbackContext: D,
+        messageResolver: k,
+        localeFallbacker: E,
+        fallbackContext: I,
         onWarn: n,
         __meta: F
     };
     return O.datetimeFormats = u, O.numberFormats = s, O.__datetimeFormatters = M, O.__numberFormatters = L, __INTLIFY_PROD_DEVTOOLS__ && $b(O, t, F), O
 }
 
 function ml(e, n, t, r, o) {
@@ -13559,22 +13559,22 @@
         postTranslation: r,
         unresolving: o,
         messageCompiler: a,
         fallbackLocale: l,
         messages: u
     } = e, [s, c] = pa(...n), d = we(c.missingWarn) ? c.missingWarn : e.missingWarn, m = we(c.fallbackWarn) ? c.fallbackWarn : e.fallbackWarn, f = we(c.escapeParameter) ? c.escapeParameter : e.escapeParameter, _ = !!c.resolvedMessage, p = Q(c.default) || we(c.default) ? we(c.default) ? a ? s : () => s : c.default : t ? a ? s : () => s : "", g = t || p !== "", y = cl(e, c);
     f && fv(c);
-    let [z, b, h] = _ ? [s, y, u[y] || {}] : Jm(e, s, y, l, m, d), S = z, E = s;
-    if (!_ && !(Q(S) || ar(S) || gn(S)) && g && (S = p, E = S), !_ && (!(Q(S) || ar(S) || gn(S)) || !Q(b))) return o ? li : s;
-    let k = !1;
-    const D = () => {
-            k = !0
+    let [z, b, h] = _ ? [s, y, u[y] || {}] : Jm(e, s, y, l, m, d), S = z, k = s;
+    if (!_ && !(Q(S) || ar(S) || gn(S)) && g && (S = p, k = S), !_ && (!(Q(S) || ar(S) || gn(S)) || !Q(b))) return o ? li : s;
+    let E = !1;
+    const I = () => {
+            E = !0
         },
-        P = gn(S) ? S : ed(e, s, b, S, E, D);
-    if (k) return S;
+        P = gn(S) ? S : ed(e, s, b, S, k, I);
+    if (E) return S;
     const M = zv(e, b, h, c),
         L = qb(M),
         F = _v(e, P, L),
         O = r ? r(F, s) : F;
     if (__INTLIFY_PROD_DEVTOOLS__) {
         const V = {
             timestamp: Date.now(),
@@ -13643,15 +13643,15 @@
     return {
         locale: n,
         key: t,
         warnHtmlMessage: o,
         onError: l => {
             throw a && a(l), l
         },
-        onCacheKey: l => qg(n, t, l)
+        onCacheKey: l => q0(n, t, l)
     }
 }
 
 function zv(e, n, t, r) {
     const {
         modifiers: o,
         pluralRules: a,
@@ -13696,20 +13696,20 @@
     const _ = !!d.part,
         p = cl(e, d),
         g = l(e, o, p);
     if (!Q(s) || s === "") return new Intl.DateTimeFormat(p, m).format(c);
     let y = {},
         z, b = null;
     const h = "datetime format";
-    for (let k = 0; k < g.length && (z = g[k], y = t[z] || {}, b = y[s], !de(b)); k++) ml(e, s, z, f, h);
+    for (let E = 0; E < g.length && (z = g[E], y = t[z] || {}, b = y[s], !de(b)); E++) ml(e, s, z, f, h);
     if (!de(b) || !Q(z)) return r ? li : s;
     let S = `${z}__${s}`;
     ii(m) || (S = `${S}__${JSON.stringify(m)}`);
-    let E = u.get(S);
-    return E || (E = new Intl.DateTimeFormat(z, Ke({}, b, m)), u.set(S, E)), _ ? E.formatToParts(c) : E.format(c)
+    let k = u.get(S);
+    return k || (k = new Intl.DateTimeFormat(z, Ke({}, b, m)), u.set(S, k)), _ ? k.formatToParts(c) : k.format(c)
 }
 const nd = ["localeMatcher", "weekday", "era", "year", "month", "day", "hour", "minute", "second", "timeZoneName", "formatMatcher", "hour12", "timeZone", "dateStyle", "timeStyle", "calendar", "dayPeriod", "numberingSystem", "hourCycle", "fractionalSecondDigits"];
 
 function za(...e) {
     const [n, t, r, o] = e, a = {};
     let l = {},
         u;
@@ -13719,15 +13719,15 @@
         const c = s[3] ? s[3].trim().startsWith("T") ? `${s[1].trim()}${s[3].trim()}` : `${s[1].trim()}T${s[3].trim()}` : s[1].trim();
         u = new Date(c);
         try {
             u.toISOString()
         } catch {
             throw Un(On.INVALID_ISO_DATE_ARGUMENT)
         }
-    } else if ($g(n)) {
+    } else if ($0(n)) {
         if (isNaN(n.getTime())) throw Un(On.INVALID_DATE_ARGUMENT);
         u = n
     } else if (Be(n)) u = n;
     else throw Un(On.INVALID_ARGUMENT);
     return Q(t) ? a.key = t : de(t) && Object.keys(t).forEach(s => {
         nd.includes(s) ? l[s] = t[s] : a[s] = t[s]
     }), Q(r) ? a.locale = r : de(r) && (l = r), de(o) && (l = o), [a.key || "", u, a, l]
@@ -13755,20 +13755,20 @@
     const _ = !!d.part,
         p = cl(e, d),
         g = l(e, o, p);
     if (!Q(s) || s === "") return new Intl.NumberFormat(p, m).format(c);
     let y = {},
         z, b = null;
     const h = "number format";
-    for (let k = 0; k < g.length && (z = g[k], y = t[z] || {}, b = y[s], !de(b)); k++) ml(e, s, z, f, h);
+    for (let E = 0; E < g.length && (z = g[E], y = t[z] || {}, b = y[s], !de(b)); E++) ml(e, s, z, f, h);
     if (!de(b) || !Q(z)) return r ? li : s;
     let S = `${z}__${s}`;
     ii(m) || (S = `${S}__${JSON.stringify(m)}`);
-    let E = u.get(S);
-    return E || (E = new Intl.NumberFormat(z, Ke({}, b, m)), u.set(S, E)), _ ? E.formatToParts(c) : E.format(c)
+    let k = u.get(S);
+    return k || (k = new Intl.NumberFormat(z, Ke({}, b, m)), u.set(S, k)), _ ? k.formatToParts(c) : k.format(c)
 }
 const td = ["localeMatcher", "style", "currency", "currencyDisplay", "currencySign", "useGrouping", "minimumIntegerDigits", "minimumFractionDigits", "maximumFractionDigits", "minimumSignificantDigits", "maximumSignificantDigits", "compactDisplay", "notation", "signDisplay", "unit", "unitDisplay", "roundingMode", "roundingPriority", "roundingIncrement", "trailingZeroDisplay"];
 
 function ha(...e) {
     const [n, t, r, o] = e, a = {};
     let l = {};
     if (!Be(n)) throw Un(On.INVALID_ARGUMENT);
@@ -13921,316 +13921,316 @@
     } : null
 };
 
 function ld(e = {}, n) {
     const {
         __root: t,
         __injectWithOption: r
-    } = e, o = t === void 0, a = e.flatJson, l = Io ? he : st, u = !!e.translateExistCompatible;
+    } = e, o = t === void 0, a = e.flatJson, l = Do ? he : st, u = !!e.translateExistCompatible;
     let s = we(e.inheritLocale) ? e.inheritLocale : !0;
     const c = l(t && s ? t.locale.value : Q(e.locale) ? e.locale : xo),
         d = l(t && s ? t.fallbackLocale.value : Q(e.fallbackLocale) || xe(e.fallbackLocale) || de(e.fallbackLocale) || e.fallbackLocale === !1 ? e.fallbackLocale : c.value),
         m = l(id(c.value, e)),
         f = l(de(e.datetimeFormats) ? e.datetimeFormats : {
             [c.value]: {}
         }),
         _ = l(de(e.numberFormats) ? e.numberFormats : {
             [c.value]: {}
         });
-    let p = t ? t.missingWarn : we(e.missingWarn) || Do(e.missingWarn) ? e.missingWarn : !0,
-        g = t ? t.fallbackWarn : we(e.fallbackWarn) || Do(e.fallbackWarn) ? e.fallbackWarn : !0,
+    let p = t ? t.missingWarn : we(e.missingWarn) || Io(e.missingWarn) ? e.missingWarn : !0,
+        g = t ? t.fallbackWarn : we(e.fallbackWarn) || Io(e.fallbackWarn) ? e.fallbackWarn : !0,
         y = t ? t.fallbackRoot : we(e.fallbackRoot) ? e.fallbackRoot : !0,
         z = !!e.fallbackFormat,
         b = Pe(e.missing) ? e.missing : null,
         h = Pe(e.missing) ? wu(e.missing) : null,
         S = Pe(e.postTranslation) ? e.postTranslation : null,
-        E = t ? t.warnHtmlMessage : we(e.warnHtmlMessage) ? e.warnHtmlMessage : !0,
-        k = !!e.escapeParameter;
-    const D = t ? t.modifiers : de(e.modifiers) ? e.modifiers : {};
+        k = t ? t.warnHtmlMessage : we(e.warnHtmlMessage) ? e.warnHtmlMessage : !0,
+        E = !!e.escapeParameter;
+    const I = t ? t.modifiers : de(e.modifiers) ? e.modifiers : {};
     let P = e.pluralRules || t && t.pluralRules,
         M;
     M = (() => {
         o && mu(null);
-        const I = {
+        const D = {
             version: hv,
             locale: c.value,
             fallbackLocale: d.value,
             messages: m.value,
-            modifiers: D,
+            modifiers: I,
             pluralRules: P,
             missing: h === null ? void 0 : h,
             missingWarn: p,
             fallbackWarn: g,
             fallbackFormat: z,
             unresolving: !0,
             postTranslation: S === null ? void 0 : S,
-            warnHtmlMessage: E,
-            escapeParameter: k,
+            warnHtmlMessage: k,
+            escapeParameter: E,
             messageResolver: e.messageResolver,
             messageCompiler: e.messageCompiler,
             __meta: {
                 framework: "vue"
             }
         };
-        I.datetimeFormats = f.value, I.numberFormats = _.value, I.__datetimeFormatters = de(M) ? M.__datetimeFormatters : void 0, I.__numberFormatters = de(M) ? M.__numberFormatters : void 0;
-        const R = sv(I);
+        D.datetimeFormats = f.value, D.numberFormats = _.value, D.__datetimeFormatters = de(M) ? M.__datetimeFormatters : void 0, D.__numberFormatters = de(M) ? M.__numberFormatters : void 0;
+        const R = sv(D);
         return o && mu(R), R
     })(), pr(M, c.value, d.value);
 
     function F() {
         return [c.value, d.value, m.value, f.value, _.value]
     }
     const O = ae({
             get: () => c.value,
-            set: I => {
-                c.value = I, M.locale = c.value
+            set: D => {
+                c.value = D, M.locale = c.value
             }
         }),
         V = ae({
             get: () => d.value,
-            set: I => {
-                d.value = I, M.fallbackLocale = d.value, pr(M, c.value, I)
+            set: D => {
+                d.value = D, M.fallbackLocale = d.value, pr(M, c.value, D)
             }
         }),
         Z = ae(() => m.value),
         oe = ae(() => f.value),
         ie = ae(() => _.value);
 
     function se() {
         return Pe(S) ? S : null
     }
 
-    function ue(I) {
-        S = I, M.postTranslation = I
+    function ue(D) {
+        S = D, M.postTranslation = D
     }
 
     function Ue() {
         return b
     }
 
-    function Xe(I) {
-        I !== null && (h = wu(I)), b = I, M.missing = h
+    function Xe(D) {
+        D !== null && (h = wu(D)), b = D, M.missing = h
     }
-    const Ee = (I, R, J, te, ge, qe) => {
+    const ke = (D, R, J, te, ge, qe) => {
         F();
         let ln;
         try {
             __INTLIFY_PROD_DEVTOOLS__,
             o || (M.fallbackContext = t ? lv() : void 0),
-            ln = I(M)
+            ln = D(M)
         }
         finally {
             __INTLIFY_PROD_DEVTOOLS__,
             o || (M.fallbackContext = void 0)
         }
         if (J !== "translate exists" && Be(ln) && ln === li || J === "translate exists" && !ln) {
             const [Wr, xt] = R();
             return t && y ? te(t) : ge(Wr)
         } else {
             if (qe(ln)) return ln;
             throw Pn(Tn.UNEXPECTED_RETURN_TYPE)
         }
     };
 
-    function ke(...I) {
-        return Ee(R => Reflect.apply(pu, null, [R, ...I]), () => pa(...I), "translate", R => Reflect.apply(R.t, R, [...I]), R => R, R => Q(R))
+    function Ee(...D) {
+        return ke(R => Reflect.apply(pu, null, [R, ...D]), () => pa(...D), "translate", R => Reflect.apply(R.t, R, [...D]), R => R, R => Q(R))
     }
 
-    function Mn(...I) {
-        const [R, J, te] = I;
+    function Mn(...D) {
+        const [R, J, te] = D;
         if (te && !_e(te)) throw Pn(Tn.INVALID_ARGUMENT);
-        return ke(R, J, Ke({
+        return Ee(R, J, Ke({
             resolvedMessage: !0
         }, te || {}))
     }
 
-    function Sn(...I) {
-        return Ee(R => Reflect.apply(zu, null, [R, ...I]), () => za(...I), "datetime format", R => Reflect.apply(R.d, R, [...I]), () => uu, R => Q(R))
+    function Sn(...D) {
+        return ke(R => Reflect.apply(zu, null, [R, ...D]), () => za(...D), "datetime format", R => Reflect.apply(R.d, R, [...D]), () => uu, R => Q(R))
     }
 
-    function Kn(...I) {
-        return Ee(R => Reflect.apply(gu, null, [R, ...I]), () => ha(...I), "number format", R => Reflect.apply(R.n, R, [...I]), () => uu, R => Q(R))
+    function Kn(...D) {
+        return ke(R => Reflect.apply(gu, null, [R, ...D]), () => ha(...D), "number format", R => Reflect.apply(R.n, R, [...D]), () => uu, R => Q(R))
     }
 
-    function Ce(I) {
-        return I.map(R => Q(R) || Be(R) || we(R) ? vu(String(R)) : R)
+    function Ce(D) {
+        return D.map(R => Q(R) || Be(R) || we(R) ? vu(String(R)) : R)
     }
     const K = {
         normalize: Ce,
-        interpolate: I => I,
+        interpolate: D => D,
         type: "vnode"
     };
 
-    function W(...I) {
-        return Ee(R => {
+    function W(...D) {
+        return ke(R => {
             let J;
             const te = R;
             try {
-                te.processor = K, J = Reflect.apply(pu, null, [te, ...I])
+                te.processor = K, J = Reflect.apply(pu, null, [te, ...D])
             } finally {
                 te.processor = null
             }
             return J
-        }, () => pa(...I), "translate", R => R[ga](...I), R => [vu(R)], R => xe(R))
+        }, () => pa(...D), "translate", R => R[ga](...D), R => [vu(R)], R => xe(R))
     }
 
-    function X(...I) {
-        return Ee(R => Reflect.apply(gu, null, [R, ...I]), () => ha(...I), "number format", R => R[va](...I), Tu, R => Q(R) || xe(R))
+    function X(...D) {
+        return ke(R => Reflect.apply(gu, null, [R, ...D]), () => ha(...D), "number format", R => R[va](...D), Tu, R => Q(R) || xe(R))
     }
 
-    function me(...I) {
-        return Ee(R => Reflect.apply(zu, null, [R, ...I]), () => za(...I), "datetime format", R => R[ba](...I), Tu, R => Q(R) || xe(R))
+    function me(...D) {
+        return ke(R => Reflect.apply(zu, null, [R, ...D]), () => za(...D), "datetime format", R => R[ba](...D), Tu, R => Q(R) || xe(R))
     }
 
-    function ze(I) {
-        P = I, M.pluralRules = P
+    function ze(D) {
+        P = D, M.pluralRules = P
     }
 
-    function w(I, R) {
-        return Ee(() => {
-            if (!I) return !1;
+    function w(D, R) {
+        return ke(() => {
+            if (!D) return !1;
             const J = Q(R) ? R : c.value,
                 te = H(J),
-                ge = M.messageResolver(te, I);
+                ge = M.messageResolver(te, D);
             return u ? ge != null : ar(ge) || gn(ge) || Q(ge)
-        }, () => [I], "translate exists", J => Reflect.apply(J.te, J, [I, R]), Tv, J => we(J))
+        }, () => [D], "translate exists", J => Reflect.apply(J.te, J, [D, R]), Tv, J => we(J))
     }
 
-    function A(I) {
+    function A(D) {
         let R = null;
         const J = $m(M, d.value, c.value);
         for (let te = 0; te < J.length; te++) {
             const ge = m.value[J[te]] || {},
-                qe = M.messageResolver(ge, I);
+                qe = M.messageResolver(ge, D);
             if (qe != null) {
                 R = qe;
                 break
             }
         }
         return R
     }
 
-    function x(I) {
-        const R = A(I);
-        return R ?? (t ? t.tm(I) || {} : {})
+    function x(D) {
+        const R = A(D);
+        return R ?? (t ? t.tm(D) || {} : {})
     }
 
-    function H(I) {
-        return m.value[I] || {}
+    function H(D) {
+        return m.value[D] || {}
     }
 
-    function N(I, R) {
+    function N(D, R) {
         if (a) {
             const J = {
-                [I]: R
+                [D]: R
             };
             for (const te in J) Lo(J, te) && Br(J[te]);
-            R = J[I]
+            R = J[D]
         }
-        m.value[I] = R, M.messages = m.value
+        m.value[D] = R, M.messages = m.value
     }
 
-    function U(I, R) {
-        m.value[I] = m.value[I] || {};
+    function U(D, R) {
+        m.value[D] = m.value[D] || {};
         const J = {
-            [I]: R
+            [D]: R
         };
         if (a)
             for (const te in J) Lo(J, te) && Br(J[te]);
-        R = J[I], zo(R, m.value[I]), M.messages = m.value
+        R = J[D], zo(R, m.value[D]), M.messages = m.value
     }
 
-    function $(I) {
-        return f.value[I] || {}
+    function $(D) {
+        return f.value[D] || {}
     }
 
-    function v(I, R) {
-        f.value[I] = R, M.datetimeFormats = f.value, hu(M, I, R)
+    function v(D, R) {
+        f.value[D] = R, M.datetimeFormats = f.value, hu(M, D, R)
     }
 
-    function T(I, R) {
-        f.value[I] = Ke(f.value[I] || {}, R), M.datetimeFormats = f.value, hu(M, I, R)
+    function T(D, R) {
+        f.value[D] = Ke(f.value[D] || {}, R), M.datetimeFormats = f.value, hu(M, D, R)
     }
 
-    function C(I) {
-        return _.value[I] || {}
+    function C(D) {
+        return _.value[D] || {}
     }
 
-    function G(I, R) {
-        _.value[I] = R, M.numberFormats = _.value, bu(M, I, R)
+    function G(D, R) {
+        _.value[D] = R, M.numberFormats = _.value, bu(M, D, R)
     }
 
-    function q(I, R) {
-        _.value[I] = Ke(_.value[I] || {}, R), M.numberFormats = _.value, bu(M, I, R)
+    function q(D, R) {
+        _.value[D] = Ke(_.value[D] || {}, R), M.numberFormats = _.value, bu(M, D, R)
     }
-    Su++, t && Io && (Je(t.locale, I => {
-        s && (c.value = I, M.locale = I, pr(M, c.value, d.value))
-    }), Je(t.fallbackLocale, I => {
-        s && (d.value = I, M.fallbackLocale = I, pr(M, c.value, d.value))
+    Su++, t && Do && (Je(t.locale, D => {
+        s && (c.value = D, M.locale = D, pr(M, c.value, d.value))
+    }), Je(t.fallbackLocale, D => {
+        s && (d.value = D, M.fallbackLocale = D, pr(M, c.value, d.value))
     }));
     const j = {
         id: Su,
         locale: O,
         fallbackLocale: V,
         get inheritLocale() {
             return s
         },
-        set inheritLocale(I) {
-            s = I, I && t && (c.value = t.locale.value, d.value = t.fallbackLocale.value, pr(M, c.value, d.value))
+        set inheritLocale(D) {
+            s = D, D && t && (c.value = t.locale.value, d.value = t.fallbackLocale.value, pr(M, c.value, d.value))
         },
         get availableLocales() {
             return Object.keys(m.value).sort()
         },
         messages: Z,
         get modifiers() {
-            return D
+            return I
         },
         get pluralRules() {
             return P || {}
         },
         get isGlobal() {
             return o
         },
         get missingWarn() {
             return p
         },
-        set missingWarn(I) {
-            p = I, M.missingWarn = p
+        set missingWarn(D) {
+            p = D, M.missingWarn = p
         },
         get fallbackWarn() {
             return g
         },
-        set fallbackWarn(I) {
-            g = I, M.fallbackWarn = g
+        set fallbackWarn(D) {
+            g = D, M.fallbackWarn = g
         },
         get fallbackRoot() {
             return y
         },
-        set fallbackRoot(I) {
-            y = I
+        set fallbackRoot(D) {
+            y = D
         },
         get fallbackFormat() {
             return z
         },
-        set fallbackFormat(I) {
-            z = I, M.fallbackFormat = z
+        set fallbackFormat(D) {
+            z = D, M.fallbackFormat = z
         },
         get warnHtmlMessage() {
-            return E
+            return k
         },
-        set warnHtmlMessage(I) {
-            E = I, M.warnHtmlMessage = I
+        set warnHtmlMessage(D) {
+            k = D, M.warnHtmlMessage = D
         },
         get escapeParameter() {
-            return k
+            return E
         },
-        set escapeParameter(I) {
-            k = I, M.escapeParameter = I
+        set escapeParameter(D) {
+            E = D, M.escapeParameter = D
         },
-        t: ke,
+        t: Ee,
         getLocaleMessage: H,
         setLocaleMessage: N,
         mergeLocaleMessage: U,
         getPostTranslationHandler: se,
         setPostTranslationHandler: ue,
         getMissingHandler: Ue,
         setMissingHandler: Xe,
@@ -14263,15 +14263,15 @@
         return o && (t[r] = o()), t
     }, {})
 }
 
 function sd(e) {
     return Fe
 }
-const Ev = Dt({
+const kv = It({
         name: "i18n-t",
         props: Ke({
             keypath: {
                 type: String,
                 required: !0
             },
             plural: {
@@ -14295,17 +14295,17 @@
                     s = o[ga](e.keypath, u, l),
                     c = Ke({}, r),
                     d = Q(e.tag) || _e(e.tag) ? e.tag : sd();
                 return Ge(d, c, s)
             }
         }
     }),
-    Eu = Ev;
+    ku = kv;
 
-function kv(e) {
+function Ev(e) {
     return xe(e) && !Q(e[0])
 }
 
 function ud(e, n, t, r) {
     const {
         slots: o,
         attrs: a
@@ -14323,22 +14323,22 @@
         xe(s) ? c = s.map((f, _) => {
             const p = o[f.type],
                 g = p ? p({
                     [f.type]: f.value,
                     index: _,
                     parts: s
                 }) : [f.value];
-            return kv(g) && (g[0].key = `${f.type}-${_}`), g
+            return Ev(g) && (g[0].key = `${f.type}-${_}`), g
         }) : Q(s) && (c = [s]);
         const d = Ke({}, a),
             m = Q(e.tag) || _e(e.tag) ? e.tag : sd();
         return Ge(m, d, c)
     }
 }
-const Av = Dt({
+const Av = It({
         name: "i18n-n",
         props: Ke({
             value: {
                 type: Number,
                 required: !0
             },
             format: {
@@ -14349,16 +14349,16 @@
             const t = e.i18n || fl({
                 useScope: e.scope,
                 __useComponent: !0
             });
             return ud(e, n, td, (...r) => t[va](...r))
         }
     }),
-    ku = Av,
-    Pv = Dt({
+    Eu = Av,
+    Pv = It({
         name: "i18n-d",
         props: Ke({
             value: {
                 type: [Number, Date],
                 required: !0
             },
             format: {
@@ -14395,20 +14395,20 @@
         const d = Mv(e, u.$),
             m = Pu(c);
         return [Reflect.apply(d.t, d, [...Mu(m)]), d]
     };
     return {
         created: (l, u) => {
             const [s, c] = n(u);
-            Io && e.global === c && (l.__i18nWatcher = Je(c.locale, () => {
+            Do && e.global === c && (l.__i18nWatcher = Je(c.locale, () => {
                 u.instance && u.instance.$forceUpdate()
             })), l.__composer = c, l.textContent = s
         },
         unmounted: l => {
-            Io && l.__i18nWatcher && (l.__i18nWatcher(), l.__i18nWatcher = void 0, delete l.__i18nWatcher), l.__composer && (l.__composer = void 0, delete l.__composer)
+            Do && l.__i18nWatcher && (l.__i18nWatcher(), l.__i18nWatcher = void 0, delete l.__i18nWatcher), l.__composer && (l.__composer = void 0, delete l.__composer)
         },
         beforeUpdate: (l, {
             value: u
         }) => {
             if (l.__composer) {
                 const s = l.__composer,
                     c = Pu(u);
@@ -14441,20 +14441,20 @@
         args: r,
         choice: o,
         plural: a
     } = e, l = {}, u = r || {};
     return Q(t) && (l.locale = t), Be(o) && (l.plural = o), Be(a) && (l.plural = a), [n, u, l]
 }
 
-function Iv(e, n, ...t) {
+function Dv(e, n, ...t) {
     const r = de(t[0]) ? t[0] : {},
         o = !!r.useI18nComponentName;
-    (we(r.globalInstall) ? r.globalInstall : !0) && ([o ? "i18n" : Eu.name, "I18nT"].forEach(l => e.component(l, Eu)), [ku.name, "I18nN"].forEach(l => e.component(l, ku)), [Au.name, "I18nD"].forEach(l => e.component(l, Au))), e.directive("t", Cv(n))
+    (we(r.globalInstall) ? r.globalInstall : !0) && ([o ? "i18n" : ku.name, "I18nT"].forEach(l => e.component(l, ku)), [Eu.name, "I18nN"].forEach(l => e.component(l, Eu)), [Au.name, "I18nD"].forEach(l => e.component(l, Au))), e.directive("t", Cv(n))
 }
-const Dv = ft("global-vue-i18n");
+const Iv = ft("global-vue-i18n");
 
 function Lv(e = {}, n) {
     const t = we(e.globalInjection) ? e.globalInjection : !0,
         r = !0,
         o = new Map,
         [a, l] = Ov(e),
         u = ft("");
@@ -14479,15 +14479,15 @@
             },
             async install(f, ..._) {
                 if (f.__VUE_I18N_SYMBOL__ = u, f.provide(f.__VUE_I18N_SYMBOL__, m), de(_[0])) {
                     const y = _[0];
                     m.__composerExtend = y.__composerExtend, m.__vueI18nExtend = y.__vueI18nExtend
                 }
                 let p = null;
-                t && (p = Vv(f, m.global)), Iv(f, m, ..._);
+                t && (p = Vv(f, m.global)), Dv(f, m, ..._);
                 const g = f.unmount;
                 f.unmount = () => {
                     p && p(), m.dispose(), g()
                 }
             },
             get global() {
                 return l
@@ -14533,15 +14533,15 @@
         if (o == null) throw Pn(Tn.UNEXPECTED_ERROR);
         return [r, o]
     }
 }
 
 function xv(e) {
     {
-        const n = He(e.isCE ? Dv : e.appContext.app.__VUE_I18N_SYMBOL__);
+        const n = He(e.isCE ? Iv : e.appContext.app.__VUE_I18N_SYMBOL__);
         if (!n) throw Pn(e.isCE ? Tn.NOT_INSTALLED_WITH_PROVIDE : Tn.UNEXPECTED_ERROR);
         return n
     }
 }
 
 function Rv(e, n) {
     return ii(e) ? "__i18n" in n ? "local" : "global" : e.useScope ? e.useScope : "local"
@@ -16720,15 +16720,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Luk"])
             },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["Opret ny afspilningsliste på ", t(r(0))])
             },
@@ -17579,15 +17579,15 @@
                     }
                 },
                 auto_play: {
                     label: e => {
                         const {
                             normalize: n
                         } = e;
-                        return n(["Start afspilning"])
+                        return n(["Start automatisk afspilning"])
                     },
                     description: e => {
                         const {
                             normalize: n
                         } = e;
                         return n(["Når denne afspiller tændes, starter afspilningen automatisk (hvis der er elementer i køen)."])
                     }
@@ -18055,14 +18055,158 @@
                 provider_depends_on_confirm: e => {
                     const {
                         normalize: n,
                         interpolate: t,
                         list: r
                     } = e;
                     return n(["Før du kan opsætte ", t(r(0)), ", skal du have konfigureret ", t(r(1)), " udbyderen, vil du gøre det nu?"])
+                },
+                category: {
+                    audio: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lyd"])
+                    },
+                    advanced: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Avancerede indstillinger"])
+                    },
+                    generic: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Generelle indstillinger"])
+                    },
+                    announcements: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Konfiguration af meddelelser"])
+                    },
+                    airplay: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Airplay-specifikke indstillinger"])
+                    }
+                },
+                tts_pre_announce: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Forhåndsannoncering af TTS-meddelelser"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Når en TTS-besked (tekst-til-tale) sendes til Announce-funktionen, tilføjes en kort lyd (klokke) før meddelelsen."])
+                    }
+                },
+                announce_volume_strategy: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lydstyrkestrategi for meddelelser"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Når der sendes en meddelelse til denne afspiller, hvordan skal lydstyrken så justeres midlertidigt (brug i kombination med lydstyrken nedenfor)."])
+                    },
+                    options: {
+                        absolute: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Bestemt lydstyrke"])
+                        },
+                        relative: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Relativ lydstyrkeforøgelse"])
+                        },
+                        percentual: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lydstyrkeforøgelse med fast procentsats"])
+                        },
+                        none: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Juster ikke lydstyrken"])
+                        }
+                    }
+                },
+                announce_volume: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lydstyrke for meddelelser"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Det procentuelle, relative eller absolutte, lydstyrkeniveau, der bruges med strategien til meddelelser."])
+                    }
+                },
+                announce_volume_min: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Minimum lydstyrke for meddelelser"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lydstyrken af meddelelser bør ikke gå under dette niveau."])
+                    }
+                },
+                announce_volume_max: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Maksimal lydstyrke for meddelelser"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lydstyrken af meddelelser bør ikke overstige dette niveau."])
+                    }
+                },
+                icon: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Ikon"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n([`Material design ikon for denne afspiller. 
+
+ Se https://pictogrammers.com/library/mdi/.`])
+                    }
                 }
             },
             show_info: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Vis info"])
@@ -18375,14 +18519,20 @@
                     return n(["Vis/skjul menu"])
                 },
                 search_filter_active: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Søgningen filtrerer i øjeblikket resultater"])
+                },
+                play_sample: e => {
+                    const {
+                        normalize: n
+                    } = e;
+                    return n(["Afspil prøve"])
                 }
             },
             topresult: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Bedste resultat"])
@@ -18532,14 +18682,46 @@
                 return n(["Radio"])
             },
             muted: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["dæmpet"])
+            },
+            enter_name: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Indtast et nyt (brugerdefineret) navn"])
+            },
+            image_url: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Indtast URL'en til et billede eller ikon (valgfrit)"])
+            },
+            invalid_input: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Input var ugyldigt"])
+            },
+            new_playlist: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Ny playliste"])
+            },
+            create_playlist_on: e => {
+                const {
+                    normalize: n,
+                    interpolate: t,
+                    list: r
+                } = e;
+                return n(["Opret ny playliste på ", t(r(0))])
             }
         }
     }, {
         de: {
             actions: e => {
                 const {
                     normalize: n
@@ -18676,15 +18858,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Schließen"])
             },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["Erstelle eine neue Playlist auf ", t(r(0))])
             },
@@ -18718,15 +18900,15 @@
                 } = e;
                 return n(["Details"])
             },
             enter_url: e => {
                 const {
                     normalize: n
                 } = e;
-                return n(["Geben Sie die URL ein, die Sie manuell zur Datenbank hinzufügen möchten"])
+                return n(["URL eingeben, die manuell zur Datenbank hinzugefügt werden soll"])
             },
             external_source_active: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
@@ -18870,15 +19052,15 @@
                 } = e;
                 return n(["Wiedergeben auf: ", t(r(0))])
             },
             play_playlist_from: e => {
                 const {
                     normalize: n
                 } = e;
-                return n(["Playliste von hier abspielen"])
+                return n(["Playlist von hier abspielen"])
             },
             play_radio: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Radio starten"])
             },
@@ -18908,15 +19090,15 @@
                 } = e;
                 return n(["Mediaplayer"])
             },
             playlist: e => {
                 const {
                     normalize: n
                 } = e;
-                return n(["Playliste"])
+                return n(["Playlist"])
             },
             playlist_tracks: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Playlisten Tracks"])
             },
@@ -19083,15 +19265,15 @@
                     } = e;
                     return n(["Erweiterte Einstellungen"])
                 },
                 check_docs: e => {
                     const {
                         normalize: n
                     } = e;
-                    return n(["Schauen Sie sich die Dokumentation an"])
+                    return n(["Dokumentation ansehen"])
                 },
                 codeowners: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Autoren/Credits"])
                 },
@@ -19169,15 +19351,15 @@
                     } = e;
                     return n(["Musikanbieter"])
                 },
                 need_help_setup_provider: e => {
                     const {
                         normalize: n
                     } = e;
-                    return n(["Benötigen Sie Hilfe bei der Einrichtung dieses Anbieters?"])
+                    return n(["Benötigst du Hilfe bei der Einrichtung dieses Anbieters?"])
                 },
                 no_providers: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Keine Musikanbieter konfiguriert"])
                 },
@@ -19425,15 +19607,15 @@
                 },
                 add_new_provider_button: e => {
                     const {
                         normalize: n,
                         interpolate: t,
                         list: r
                     } = e;
-                    return n(["Anbieter ", t(r(0)), " hinzufügen"])
+                    return n([t(r(0)), "-Anbieter hinzufügen"])
                 },
                 add_group_player: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Wiedergabegruppen hinzufügen"])
                 },
@@ -19526,16 +19708,16 @@
                         } = e;
                         return n(['Warteschlangen-"Flow"-Modus aktivieren'])
                     },
                     description: e => {
                         const {
                             normalize: n
                         } = e;
-                        return n([`Aktiviere den "Flow"-Modus, bei dem alle Warteschlangentitel als kontinuierlicher Audiostrom gesendet werden. 
-Verwenden Sie diesen Modus für Player, die keine native lückenlose Überblendung unterstützen, oder wenn der Player Probleme beim Übergang zwischen den Titeln hat.`])
+                        return n([`Aktiviere den "Flow"-Modus, bei dem alle Warteschlangentitel als kontinuierlicher Audiostream gesendet werden. 
+Verwende diesen Modus für Player, die keine native lückenlose Überblendung unterstützen, oder wenn der Player Probleme beim Übergang zwischen Titeln hat.`])
                     }
                 },
                 auto_play: {
                     label: e => {
                         const {
                             normalize: n
                         } = e;
@@ -19719,19 +19901,175 @@
                     },
                     options: {
                         library_tracks: e => {
                             const {
                                 normalize: n
                             } = e;
                             return n(["Nur Titel in der Bibliothek"])
+                        },
+                        library_album_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Alle Titel aus allen Alben in der Bibliothek"])
+                        },
+                        all_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Alle (Top) Titel von allen Anbietern"])
+                        },
+                        all_album_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Alle Titel aller Alben von allen Anbietern"])
+                        }
+                    }
+                },
+                default_enqueue_select_album: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Elemente, die bei der Wiedergabe eines Albums (aus der Bibliothek) ausgewählt werden sollen."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Wenn Du einen Künstler abspielen möchtest, welche Elemente sollten in die Warteschlange gestellt werden?"])
+                    },
+                    options: {
+                        library_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Nur Titel in der Bibliothek"])
+                        },
+                        all_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Alle Titel für das Album beim Anbieter"])
+                        }
+                    }
+                },
+                default_enqueue_action_artist: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Standard-Warteschlangenoption für Künstlerartikel."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Definiere die Standard-Warteschlangenaktion für diesen Medientyp (falls keine bestimmte Aktion gewählt wurde)."])
+                    },
+                    options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Spiele jetzt die Titel des Künstlers und behalte die verbleibenden Elemente in der Warteschlange."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lösche die Warteschlange und spiele den/die Künstler-Titel ab."])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Spiele den/die Titel direkt nach dem derzeit abgespielten/gepufferten Titel ab."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Warteschlange leeren und den/die Titel direkt nach dem aktuell gespielten/gepufferten Element abspielen."])
+                        },
+                        add: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Füge den/die Titel des Künstlers am Ende der Warteschlange hinzu."])
+                        }
+                    }
+                },
+                default_enqueue_action_album: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Standard-Warteschlangenoption für Künstlerartikel."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Definiere die Standard-Warteschlangenaktion für diesen Medientyp (falls keine bestimmte Aktion gewählt wurde)."])
+                    },
+                    options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Albumtitel jetzt abspielen und die verbleibenden Warteschlangenelemente beibehalten."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lösche die Warteschlange und spiele den/die Album-Titel ab."])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Spiele den/die Titel direkt nach dem derzeit abgespielten/gepufferten Titel ab."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Warteschlange leeren und Albumtitel direkt nach dem aktuell abgespielten/gepufferten Titel abspielen."])
+                        },
+                        add: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Füge den/die Album-Titel am Ende der Warteschlange hinzu."])
                         }
                     }
                 },
                 default_enqueue_action_track: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Standardmäßige Warteschlangenoption für Titel."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Definiere die Standardaktion zum Einreihen in die Warteschlange für diesen Medientyp (falls keine Aktion definiert wurde)."])
+                    },
                     options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Spiele jetzt den/die Titel ab und behalte die verbleibenden Warteschlangenelemente."])
+                        },
                         replace: e => {
                             const {
                                 normalize: n
                             } = e;
                             return n(["Lösche die Warteschlange und spiele den/die Titel ab."])
                         },
                         next: e => {
@@ -19751,15 +20089,51 @@
                                 normalize: n
                             } = e;
                             return n(["Füge den/die Titel am Ende der Warteschlange hinzu."])
                         }
                     }
                 },
                 default_enqueue_action_playlist: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Standardmäßige Warteschlangenoption für Playlist-Elemente."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Definiere die Standardaktion zum Einreihen in die Warteschlange für diesen Medientyp (falls keine Aktion definiert wurde)."])
+                    },
                     options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Playlist jetzt abspielen und die verbleibenden Warteschlangenelemente beibehalten."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lösche die Warteschlange und spiele die Playlist-Titel ab."])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Spiele den/die Titel direkt nach dem derzeit abgespielten/gepufferten Titel ab."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lösche die Warteschlange und spiele den/die Titel direkt nach dem aktuell gespielten/gepufferten Element der Playlist ab."])
+                        },
                         add: e => {
                             const {
                                 normalize: n
                             } = e;
                             return n(["Füge den/die Playlist-Titel am Ende der Warteschlange hinzu."])
                         }
                     }
@@ -19784,15 +20158,15 @@
                             } = e;
                             return n(["Spiele jetzt den Radiosender ab und behalte die verbleibenden Warteschlangenelemente."])
                         },
                         replace: e => {
                             const {
                                 normalize: n
                             } = e;
-                            return n(["Lösche die Warteschlange und spiele den Radiosender ab [Standard]"])
+                            return n(["Lösche die Warteschlange und spiele den Radiosender ab"])
                         },
                         next: e => {
                             const {
                                 normalize: n
                             } = e;
                             return n(["Spiele das/die Element(e) direkt nach dem aktuell gespielten/gepufferten Element ab."])
                         },
@@ -19811,14 +20185,166 @@
                     }
                 },
                 default: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Standard"])
+                },
+                provider_depends_on_confirm: e => {
+                    const {
+                        normalize: n,
+                        interpolate: t,
+                        list: r
+                    } = e;
+                    return n(["Bevor du ", t(r(0)), " einrichten kannst, musst du den Anbieter ", t(r(1)), " konfigurieren. Willst du das jetzt tun?"])
+                },
+                category: {
+                    audio: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Audio"])
+                    },
+                    advanced: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Erweiterte Einstellungen "])
+                    },
+                    generic: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Allgemeine Einstellungen"])
+                    },
+                    announcements: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Einstellungen für Durchsagen"])
+                    },
+                    airplay: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Airplay-spezifische Einstellungen"])
+                    }
+                },
+                tts_pre_announce: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["TTS-Durchsagen vorankündigen"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Wenn eine TTS (Text-zu-Sprache) Nachricht an die Durchsagefunktion gesendet wird, füge der Durchsage einen kurzen Ankündigungston (Glockenpfeife) hinzu."])
+                    }
+                },
+                announce_volume_strategy: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lautstärkestrategie für Durchsagen"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Wie soll die Lautstärke vorübergehend angepasst werden, wenn eine Ansage an diesen Player gesendet wird (in Kombination mit dem unten stehenden Lautstärkewert verwenden)."])
+                    },
+                    options: {
+                        absolute: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Absolute Lautstärke"])
+                        },
+                        relative: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Relative Lautstärkezunahme"])
+                        },
+                        percentual: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lautstärke erhöhen um festen Prozentsatz"])
+                        },
+                        none: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lautstärke nicht anpassen"])
+                        }
+                    }
+                },
+                announce_volume: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lautstärke für Durchsagen"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Der prozentuale, relative oder absolute Lautstärkepegel, der mit der Strategie für Durchsagen verwendet wird."])
+                    }
+                },
+                announce_volume_min: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Mindestlautstärke für Durchsagen"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Die Lautstärke (Anpassung) der Durchsagen sollte nicht unter dieses Niveau fallen."])
+                    }
+                },
+                announce_volume_max: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Maximale Lautstärke für Durchsagen"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Die Lautstärke (Anpassung) der Durchsagen sollte nicht über dieses Niveau hinausgehen."])
+                    }
+                },
+                icon: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Icon"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n([`Material Design Icon für diesen Player. 
+
+Siehe https://pictogrammers.com/library/mdi/.`])
+                    }
                 }
             },
             show_info: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Zeige Informationen"])
@@ -20131,14 +20657,20 @@
                     return n(["Menü anzeigen/verbergen"])
                 },
                 search_filter_active: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Die Suche filtert aktuell die Ergebnisse"])
+                },
+                play_sample: e => {
+                    const {
+                        normalize: n
+                    } = e;
+                    return n(["Beispiel wiedergeben"])
                 }
             },
             topresult: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Top-Ergebnis"])
@@ -20187,15 +20719,15 @@
                 } = e;
                 return n(["Jetzt wiedergeben (Warteschlange leeren)"])
             },
             currently_playing: e => {
                 const {
                     normalize: n
                 } = e;
-                return n(["Wird grade abgespielt"])
+                return n(["Wird gerade abgespielt"])
             },
             favorites_add: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Zu Favoriten hinzufügen"])
             },
@@ -20205,15 +20737,15 @@
                 } = e;
                 return n(["Aus Favoriten entfernen"])
             },
             confirm_library_remove: e => {
                 const {
                     normalize: n
                 } = e;
-                return n(["Sind Sie sicher, dass Sie dieses Element aus der Bibliothek entfernen möchten? Alle von diesem Element abhängigen Daten werden ebenfalls rekursiv entfernt. Beachten Sie, dass dadurch nur dieses Element aus der Bibliothek entfernt wird. Falls es sich um eine Musikdatei auf der Festplatte handelt wird diese nicht gelöscht und bei der nächsten Synchronisierung möglicherweise wieder angezeigt."])
+                return n(["Dieses Element wirklich aus der Bibliothek entfernen? Alle von diesem Element abhängigen Daten werden ebenfalls rekursive entfernt. Beachte, dass dieses Element dadurch nur aus der Bibliothek entfernt wird. Falls es sich um eine Musikdatei auf der Festplatte handelt wird diese nicht gelöscht und bei der nächsten Synchronisierung möglicherweise wieder angezeigt."])
             },
             check_item_on_provider: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
@@ -20288,14 +20820,46 @@
                 return n(["Radio"])
             },
             muted: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["stumm"])
+            },
+            enter_name: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Neuen (benutzerdefinierten) Namen eingeben"])
+            },
+            image_url: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["URL zu einem Bild oder Icon eingeben (optional)"])
+            },
+            invalid_input: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Die Eingabe ist ungültig"])
+            },
+            new_playlist: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Neue Playlist"])
+            },
+            create_playlist_on: e => {
+                const {
+                    normalize: n,
+                    interpolate: t,
+                    list: r
+                } = e;
+                return n(["Erstelle eine neue Playlist auf ", t(r(0))])
             }
         }
     }, {
         en: {
             actions: e => {
                 const {
                     normalize: n
@@ -20432,21 +20996,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Close"])
             },
-            new_playlist: e => {
-                const {
-                    normalize: n
-                } = e;
-                return n(["New playlist"])
-            },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["Create new playlist on ", t(r(0))])
             },
@@ -20512,20 +21070,14 @@
             },
             home: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Home"])
             },
-            invalid_input: e => {
-                const {
-                    normalize: n
-                } = e;
-                return n(["The input was invalid"])
-            },
             items_selected: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n([t(r(0)), " item(s) selected"])
@@ -20558,26 +21110,14 @@
             },
             new_playlist_name: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Enter a new for the new playlist"])
             },
-            enter_name: e => {
-                const {
-                    normalize: n
-                } = e;
-                return n(["Enter a new (custom) name"])
-            },
-            image_url: e => {
-                const {
-                    normalize: n
-                } = e;
-                return n(["Input the URL to an image or icon (optional)"])
-            },
             no_content: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["No items found."])
             },
             no_content_filter: e => {
@@ -21219,46 +21759,14 @@
                 },
                 group_members: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Group members"])
                 },
-                category: {
-                    audio: e => {
-                        const {
-                            normalize: n
-                        } = e;
-                        return n(["Audio"])
-                    },
-                    advanced: e => {
-                        const {
-                            normalize: n
-                        } = e;
-                        return n(["Advanced settings"])
-                    },
-                    generic: e => {
-                        const {
-                            normalize: n
-                        } = e;
-                        return n(["Generic Settings"])
-                    },
-                    announcements: e => {
-                        const {
-                            normalize: n
-                        } = e;
-                        return n(["Announcements configuration"])
-                    },
-                    airplay: e => {
-                        const {
-                            normalize: n
-                        } = e;
-                        return n(["Airplay specific settings"])
-                    }
-                },
                 log_level: {
                     label: e => {
                         const {
                             normalize: n
                         } = e;
                         return n(["Log level"])
                     },
@@ -21794,14 +22302,46 @@
                     const {
                         normalize: n,
                         interpolate: t,
                         list: r
                     } = e;
                     return n(["Before you can setup ", t(r(0)), ", you need to have the ", t(r(1)), " provider configured, do you want to do that now?"])
                 },
+                category: {
+                    audio: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Audio"])
+                    },
+                    advanced: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Advanced settings"])
+                    },
+                    generic: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Generic Settings"])
+                    },
+                    announcements: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Announcements configuration"])
+                    },
+                    airplay: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Airplay specific settings"])
+                    }
+                },
                 tts_pre_announce: {
                     label: e => {
                         const {
                             normalize: n
                         } = e;
                         return n(["Pre-announce TTS announcements"])
                     },
@@ -22382,14 +22922,46 @@
                 return n(["Radio"])
             },
             muted: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["muted"])
+            },
+            enter_name: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Enter a new (custom) name"])
+            },
+            image_url: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Input the URL to an image or icon (optional)"])
+            },
+            invalid_input: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["The input was invalid"])
+            },
+            new_playlist: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["New playlist"])
+            },
+            create_playlist_on: e => {
+                const {
+                    normalize: n,
+                    interpolate: t,
+                    list: r
+                } = e;
+                return n(["Create new playlist on ", t(r(0))])
             }
         }
     }, {
         es: {
             actions: e => {
                 const {
                     normalize: n
@@ -22526,15 +23098,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Cerrar"])
             },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["Crear nueva lista de reproducción en ", t(r(0))])
             },
@@ -23747,14 +24319,22 @@
                 return n(["Cargar más elementos..."])
             },
             radio: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Radio"])
+            },
+            create_playlist_on: e => {
+                const {
+                    normalize: n,
+                    interpolate: t,
+                    list: r
+                } = e;
+                return n(["Crear nueva lista de reproducción en ", t(r(0))])
             }
         }
     }, {
         fr: {
             actions: e => {
                 const {
                     normalize: n
@@ -23891,15 +24471,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Close"])
             },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["Créer une nouvelle Playlist sur ", t(r(0))])
             },
@@ -24655,14 +25235,26 @@
                 group_members: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Membres du groupe"])
                 },
                 log_level: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Niveau des logs"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Définit le niveau de détail des logs pour ce fournisseur."])
+                    },
                     options: {
                         global: e => {
                             const {
                                 normalize: n
                             } = e;
                             return n(["Global"])
                         },
@@ -24680,14 +25272,20 @@
                         },
                         error: e => {
                             const {
                                 normalize: n
                             } = e;
                             return n(["Erreur"])
                         },
+                        debug: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Déboguer"])
+                        },
                         GLOBAL: e => {
                             const {
                                 normalize: n
                             } = e;
                             return n(["Vide"])
                         },
                         INFO: e => {
@@ -24712,15 +25310,56 @@
                             const {
                                 normalize: n
                             } = e;
                             return n(["Vide"])
                         }
                     }
                 },
+                flow_mode: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n([`Activer le mode "flow" pour la file d'attente`])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n([`Active le mode "flow" dans lequel toutes les pistes de la file d'attente sont envoyées comme un flux audio continu. 
+À utiliser pour les lecteurs qui ne prennent pas en charge le gapless et/ou le crossfading ou si le lecteur a du mal à faire la transition entre les pistes.`])
+                    }
+                },
+                auto_play: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lecture automatique (reprise à la mise sous tension)"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lorsque ce lecteur est mis en marche, la lecture commence automatiquement (s'il y a des éléments dans la file d'attente)."])
+                    }
+                },
                 output_channels: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Mode du canal de sortie"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Vous pouvez configurer ce lecteur pour qu'il ne joue que le canal gauche ou droit, par exemple pour créer une paire stéréo avec 2 lecteurs."])
+                    },
                     options: {
                         stereo: e => {
                             const {
                                 normalize: n
                             } = e;
                             return n(["Stéréo (les deux canaux)"])
                         },
@@ -24740,36 +25379,84 @@
                             const {
                                 normalize: n
                             } = e;
                             return n(["Mono (les deux canaux)"])
                         }
                     }
                 },
+                volume_normalization: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Activer la normalisation du volume (basée sur l'EBU-R128)"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Activer la normalisation du volume basée sur la norme EBU-R128 sans affecter la plage dynamique"])
+                    }
+                },
+                volume_normalization_target: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Niveau cible pour la normalisation du volume"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n([`Ajuster l'intensité sonore moyenne (perçue) à ce niveau cible, la valeur par défaut étant de -17 LUFS. 
+
+ **AVERTISSEMENT:** Un niveau trop élevé peut entraîner un écrêtage !`])
+                    }
+                },
                 eq_bass: {
                     label: e => {
                         const {
                             normalize: n
                         } = e;
                         return n(["Égaliseur : graves"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Utilisez l'égaliseur de base intégré pour régler le niveau de basses du son."])
                     }
                 },
                 eq_mid: {
                     label: e => {
                         const {
                             normalize: n
                         } = e;
                         return n(["Égaliseur : mediums"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Utilisez l'égaliseur de base intégré pour régler le niveau des médiums du son."])
                     }
                 },
                 eq_treble: {
                     label: e => {
                         const {
                             normalize: n
                         } = e;
                         return n(["Égaliseur : aigus"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Utilisez l'égaliseur de base intégré pour régler le niveau des aigus du son."])
                     }
                 },
                 crossfade: {
                     label: e => {
                         const {
                             normalize: n
                         } = e;
@@ -24792,19 +25479,485 @@
                     description: e => {
                         const {
                             normalize: n
                         } = e;
                         return n(["Durée en secondes du fondu enchaîné entre les pistes (si activé)"])
                     }
                 },
+                hide_player: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Masquer ce lecteur dans l'interface utilisateur"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n([`Masquez ce lecteur dans l’interface utilisateur. 
+
+Notez qu’il peut toujours être contrôlé et qu’il apparaîtra également dans tous les groupes de synchronisation auxquels ce lecteur appartient.`])
+                    }
+                },
+                default_enqueue_select_artist: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Éléments à sélectionner lors de la lecture d'un artiste (de la bibliothèque)."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Si vous voulez jouer un artiste, quels éléments doivent être mis en file d'attente ?"])
+                    },
+                    options: {
+                        library_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Uniquement les titres en bibliothèque"])
+                        },
+                        library_album_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Toutes les pistes de tous les albums de la bibliothèque"])
+                        },
+                        all_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Tous les (meilleurs) titres de (tous) les fournisseurs"])
+                        },
+                        all_album_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Toutes les pistes de tous les albums de (tous) les fournisseurs"])
+                        }
+                    }
+                },
+                default_enqueue_select_album: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Éléments à sélectionner lors de la lecture d'un album (de la bibliothèque)."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Si vous voulez jouer un artiste, quels éléments doivent être mis en file d'attente ?"])
+                    },
+                    options: {
+                        library_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Uniquement les pistes de la bibliothèque"])
+                        },
+                        all_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Toutes les pistes de l'album sur le fournisseur"])
+                        }
+                    }
+                },
+                default_enqueue_action_artist: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Option de mise en file d'attente par défaut pour le(s) élément(s) Artiste(s)."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Définit l'action de mise en file d'attente par défaut pour ce type de média (si vous n'avez pas spécifié d'action)."])
+                    },
+                    options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Jouez le(s) titre(s) de l’artiste maintenant et conservez le(s) élément(s) restant(s) dans la file d’attente."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Vider la file d’attente et jouer le(s) titre(s) de l’artiste"])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Jouez le(s) élément(s) juste après l'élément actuellement joué/mis en mémoire tampon."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Effacer la file d'attente et lire le(s) morceau(x) de l'artiste juste après l'élément actuellement lu/mis en mémoire tampon."])
+                        },
+                        add: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Ajouter la ou les pistes de l'artiste à la fin de la file d'attente."])
+                        }
+                    }
+                },
+                default_enqueue_action_album: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Option de mise en file d'attente par défaut pour les éléments de l'album."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Définit l'action de mise en file d'attente par défaut pour ce type de média (si vous n'avez pas spécifié d'action)."])
+                    },
+                    options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lire les pistes de l'album maintenant et conserver les autres éléments de la file d'attente."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Effacer la file d'attente et lire le(s) titre(s) de l'album"])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Jouer le(s) piste(s) juste après l'élément actuellement joué/mis en mémoire tampon."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Effacer la file d'attente et lire le(s) titre(s) de l'album juste après l'élément en cours de lecture ou de mise en mémoire tampon."])
+                        },
+                        add: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Ajouter la ou les pistes de l'album à la fin de la file d'attente."])
+                        }
+                    }
+                },
+                default_enqueue_action_track: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Option de mise en file d'attente par défaut pour les pistes."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Définit l'action de mise en file d'attente par défaut pour ce type de média (si vous n'avez pas spécifié d'action)."])
+                    },
+                    options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lire le(s) morceau(x) maintenant et conserver le(s) morceau(x) restant(s) dans la file d'attente."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Effacer la file d'attente et lire la ou les pistes."])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lit le(s) morceau(s) juste après l'élément actuellement lu/mis en mémoire tampon."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Efface la file d'attente et lit la (les) piste(s) juste après l'élément actuellement lu/mis en mémoire tampon."])
+                        },
+                        add: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Ajouter la ou les pistes à la fin de la file d'attente."])
+                        }
+                    }
+                },
+                default_enqueue_action_playlist: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Option de mise en file d'attente par défaut pour les éléments d'une playlist."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Définit l'action de mise en file d'attente par défaut pour ce type de média (si vous n'avez pas spécifié d'action)."])
+                    },
+                    options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Lire la ou les pistes de la liste de lecture maintenant et conserver les éléments restants dans la file d'attente."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Effacer la file d'attente et lire la ou les pistes de la liste de lecture"])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Jouer le(s) élément(s) juste après l'élément actuellement joué/mis en mémoire tampon."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Effacer la file d'attente et lit la (les) piste(s) de la playlist de lecture juste après l'élément actuellement lu/mis en mémoire tampon."])
+                        },
+                        add: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Ajoutez le(s) titre(s) de la playlist à la fin de la file d’attente."])
+                        }
+                    }
+                },
+                default_enqueue_action_radio: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Option de mise en file d'attente par défaut pour les éléments Radio."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Définit l'action de mise en file d'attente par défaut pour ce type de média (si vous n'avez pas spécifié d'action)."])
+                    },
+                    options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Écouter la station de radio maintenant et conserver le(s) élément(s) restant(s) dans la file d'attente."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Effacer la file d'attente et diffuser la station de radio"])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Jouer le(s) élément(s) juste après l'élément actuellement joué/mis en mémoire tampon."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Efface la file d'attente et joue la ou les stations de radio juste après l'élément actuellement joué/mis en mémoire tampon."])
+                        },
+                        add: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Ajouter la ou les stations de radio à la fin de la file d'attente."])
+                        }
+                    }
+                },
                 default: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Par défaut"])
+                },
+                provider_depends_on_confirm: e => {
+                    const {
+                        normalize: n,
+                        interpolate: t,
+                        list: r
+                    } = e;
+                    return n(["Avant de pouvoir configurer ", t(r(0)), ", vous devez avoir configuré le fournisseur ", t(r(1)), ". Voulez-vous le faire maintenant ?"])
+                },
+                category: {
+                    audio: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Son"])
+                    },
+                    advanced: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Paramètres avancés"])
+                    },
+                    generic: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Paramètres par défaut"])
+                    },
+                    announcements: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Configuration des annonces"])
+                    },
+                    airplay: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Paramètres spécifiques à Airplay"])
+                    }
+                },
+                tts_pre_announce: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Pré-annoncer les annonces TTS"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lorsqu'un message TTS (text-to-speech) est envoyé à la fonction d'annonce, l'annonce est précédée d'un court son de pré-annonce (son de cloche)."])
+                    }
+                },
+                announce_volume_strategy: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Stratégie de volume pour les annonces"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Lorsqu'une annonce est diffusée sur ce lecteur, comment le volume doit-il être réglé temporairement (à utiliser en combinaison avec la valeur du volume ci-dessous)."])
+                    },
+                    options: {
+                        absolute: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Volume absolu"])
+                        },
+                        relative: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Augmentation du volume relatif"])
+                        },
+                        percentual: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Augmentation du volume par un pourcentage définit"])
+                        },
+                        none: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Ne pas régler le volume"])
+                        }
+                    }
+                },
+                announce_volume: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Volume pour les annonces"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Le niveau de volume en pourcentage, relatif ou absolu, utilisé avec la stratégie pour les annonces."])
+                    }
+                },
+                announce_volume_min: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Volume minimum pour les annonces"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Le volume (réglage) des annonces ne doit pas être inférieur à ce niveau."])
+                    }
+                },
+                announce_volume_max: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Volume maximum pour les annonces"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Le volume (réglage) des annonces ne doit pas dépasser ce niveau."])
+                    }
+                },
+                icon: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Icône"])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n([`Icône utilisée pour ce lecteur. 
+
+Voir https://pictogrammers.com/library/mdi/.`])
+                    }
                 }
             },
             show_info: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Montrer les infos"])
@@ -25268,14 +26421,46 @@
                 return n(["Charger plus d'éléments..."])
             },
             radio: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Radio"])
+            },
+            muted: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["en sourdine"])
+            },
+            enter_name: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Saisir un nouveau nom (personnalisé)"])
+            },
+            image_url: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["Saisir l'URL d'une image ou d'une icône (facultatif)"])
+            },
+            invalid_input: e => {
+                const {
+                    normalize: n
+                } = e;
+                return n(["L'entrée n'était pas valide"])
+            },
+            create_playlist_on: e => {
+                const {
+                    normalize: n,
+                    interpolate: t,
+                    list: r
+                } = e;
+                return n(["Créer une nouvelle Playlist sur ", t(r(0))])
             }
         }
     }, {
         he: {
             actions: e => {
                 const {
                     normalize: n
@@ -25412,15 +26597,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["סגור"])
             },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["צור רשימת השמעה חדשה על ", t(r(0))])
             },
@@ -26765,15 +27950,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Chiudi"])
             },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["Crea nuova playlist su ", t(r(0))])
             },
@@ -27824,15 +29009,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Lukk"])
             },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["Opprett ny spilleliste på ", t(r(0))])
             },
@@ -29189,15 +30374,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Close"])
             },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["Maak een nieuwe playlist aan op ", t(r(0))])
             },
@@ -29888,21 +31073,21 @@
                     } = e;
                     return n(["Home Assistant-add-on"])
                 },
                 artists_in_library: e => {
                     const {
                         normalize: n
                     } = e;
-                    return n(["Artietsen in de bibltioheek"])
+                    return n(["Artiesten in de bibliotheek"])
                 },
                 albums_in_library: e => {
                     const {
                         normalize: n
                     } = e;
-                    return n(["Albums in de bibltioheek"])
+                    return n(["Albums in de bibliotheek"])
                 },
                 tracks_in_library: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Nummers in de bibliotheek"])
                 },
@@ -30213,21 +31398,251 @@
                             normalize: n
                         } = e;
                         return n([`Verberg deze speler in de gebruikersinterface. 
 
 Merk op dat het nog steeds kan worden bestuurd en het zal ook verschijnen in alle synchronisatiegroepen waartoe de speler behoort.`])
                     }
                 },
+                default_enqueue_select_artist: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Te selecteren items wanneer je een artiest (uit de bibliotheek) afspeelt."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Wanneer je een artiest wilt afspelen, welke items zouden dan in de wachtrij moeten?"])
+                    },
+                    options: {
+                        library_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Uitsluitend nummers uit de bibliotheek"])
+                        },
+                        library_album_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Alle nummers van alle albums in de bibliotheek."])
+                        },
+                        all_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Alle (top) nummers van (alle) aanbieders."])
+                        },
+                        all_album_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Alle nummers van alle albums van (alle) aanbieders."])
+                        }
+                    }
+                },
+                default_enqueue_select_album: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Te selecteren items wanneer je een album uit de bibliotheek wilt afspelen."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Wanneer je een artiest wilt afspelen, welke items moet dan op de wachtrij worden geplaatst?"])
+                    },
+                    options: {
+                        library_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Alleen nummers in de bibliotheek."])
+                        },
+                        all_tracks: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Alle nummers voor het album op aanbieder."])
+                        }
+                    }
+                },
+                default_enqueue_action_artist: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Standaard wachtrij-optie voor de items van de artiest."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Definieer de standaard actie voor dit mediatype (wanneer je nog geen actie hebt gespecificeerd)."])
+                    },
+                    options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Speel nu het nummer(s) van de artiest en bewaar de resterende items van de wachtrij."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Wis de wachtrij en speel het nummer(s) van de artiest."])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Speel het item(s) direct na het huidig spelende of gebufferde item."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Wis de wachtrij en speel het nummer(s) van de artiest direct na het huidig spelende of gebufferde nummer."])
+                        },
+                        add: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Voeg de nummers van de artiest toe aan het einde van de wachtrij."])
+                        }
+                    }
+                },
+                default_enqueue_action_album: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Standaard wachtrij-optie voor album item(s)."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Definieer de standaard actie voor dit mediatype (wanneer je nog geen actie hebt gespecificeerd)."])
+                    },
+                    options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Speel het album nummer nu en behoudt de resterende wachtlijst items."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Wis de wachtrij en speel het album nummer."])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Speel het item direct na het huidig afspelende of gebufferde item."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Wis de wachtrij en speel het album nummer(s) direct na het huidig spelende of gebufferde item."])
+                        },
+                        add: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Voeg het album nummer(s) toe aan het einde van de wachtrij."])
+                        }
+                    }
+                },
+                default_enqueue_action_track: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Standaard wachrij-optie voor afspeel items."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Definieer de standaard wachtrij-actie voor dit mediatype (wanneer je geen actie gespecificeerd hebt)."])
+                    },
+                    options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Speel het nummer(s) nu en hou de overblijvende wachtrij items."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Wis de wachtrij en speel het nummer(s)."])
+                        },
+                        next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Speel het nummer(s) meteen na het huidige afgespeelde of gebufferde item."])
+                        },
+                        replace_next: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Wis de wachtrij en speel het nummer(s) direct na het huidig afgespeelde of gebufferde item."])
+                        },
+                        add: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Voeg het nummer(s) toe aan het einde van de wachtrij."])
+                        }
+                    }
+                },
                 default_enqueue_action_playlist: {
+                    label: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["Standaard wachtrij-actie voor items op de afspeellijst."])
+                    },
+                    description: e => {
+                        const {
+                            normalize: n
+                        } = e;
+                        return n(["definieer de standaard  wachtrij-actie voor dit mediatype (wanneer je geen actie gespecificeerd hebt)."])
+                    },
                     options: {
+                        play: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Speel nu de afspeellijst en hou de overige nummers in de wachtrij."])
+                        },
+                        replace: e => {
+                            const {
+                                normalize: n
+                            } = e;
+                            return n(["Wis de wachtrij en speel de nummers van de afspeellijst"])
+                        },
                         next: e => {
                             const {
                                 normalize: n
                             } = e;
-                            return n(["Speel de item(s) direct na het momenteel afgespeelde/gebufferde item af."])
+                            return n(["Speel het item(s) direct na het nu afgespeelde/gebufferde item af."])
                         },
                         replace_next: e => {
                             const {
                                 normalize: n
                             } = e;
                             return n(["Wis de wachtrij en speel de afspeellijsttrack(s) af direct na het huidige afgespeelde/gebufferde item."])
                         },
@@ -30240,15 +31655,15 @@
                     }
                 },
                 default_enqueue_action_radio: {
                     label: e => {
                         const {
                             normalize: n
                         } = e;
-                        return n(["Standaard enqueue optie voor Radio item(s)."])
+                        return n(["Standaard wachtrij-optie voor Radio item(s)."])
                     },
                     description: e => {
                         const {
                             normalize: n
                         } = e;
                         return n(["Definieer de standaardactie voor het in de wachtrij plaatsen voor dit mediatype (als je geen actie hebt opgegeven)."])
                     },
@@ -30286,14 +31701,20 @@
                     }
                 },
                 default: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["standaard"])
+                },
+                provider_depends_on_confirm: e => {
+                    const {
+                        normalize: n
+                    } = e;
+                    return n(["Voordat je verder kunt met de set-up, moet je de provider configureren. Wil je dat nu doen?"])
                 }
             },
             show_info: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Bekijk informatie"])
@@ -30600,14 +32021,20 @@
                     return n(["Terug"])
                 },
                 show_menu: e => {
                     const {
                         normalize: n
                     } = e;
                     return n(["Toon of verberg menu"])
+                },
+                search_filter_active: e => {
+                    const {
+                        normalize: n
+                    } = e;
+                    return n(["De zoekactie toont nu gefilterde resultaten."])
                 }
             },
             topresult: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Top resultaat"])
@@ -30757,14 +32184,22 @@
                 return n(["Radio"])
             },
             muted: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["gedempt"])
+            },
+            create_playlist_on: e => {
+                const {
+                    normalize: n,
+                    interpolate: t,
+                    list: r
+                } = e;
+                return n(["Maak een nieuwe playlist aan op ", t(r(0))])
             }
         }
     }, {
         pl: {
             actions: e => {
                 const {
                     normalize: n
@@ -30901,15 +32336,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Zamknij"])
             },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["Utwórz nową listę odtwarzania na ", t(r(0))])
             },
@@ -32122,14 +33557,22 @@
                 return n(["Załaduj więcej pozycji..."])
             },
             radio: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Radio"])
+            },
+            create_playlist_on: e => {
+                const {
+                    normalize: n,
+                    interpolate: t,
+                    list: r
+                } = e;
+                return n(["Utwórz nową listę odtwarzania na ", t(r(0))])
             }
         }
     }, {
         uk_UA: {
             actions: e => {
                 const {
                     normalize: n
@@ -32266,15 +33709,15 @@
             },
             close: e => {
                 const {
                     normalize: n
                 } = e;
                 return n(["Закрити"])
             },
-            create_playlist_on: e => {
+            create_playlist: e => {
                 const {
                     normalize: n,
                     interpolate: t,
                     list: r
                 } = e;
                 return n(["Створити новий список відтворення на ", t(r(0))])
             },
@@ -33525,17 +34968,17 @@
                     const z = S => {
                             S.touches && (g = S.touches[0].clientX, y = S.touches[0].clientY, p = window.setTimeout(() => {
                                 d.value(S), p = null
                             }, t))
                         },
                         b = S => {
                             if (!g || !y || !p || !S.touches) return;
-                            const E = S.touches[0].clientX,
-                                k = S.touches[0].clientY;
-                            (Math.abs(E - g) > a || Math.abs(k - y) > a) && (window.clearTimeout(p), p = null)
+                            const k = S.touches[0].clientX,
+                                E = S.touches[0].clientY;
+                            (Math.abs(k - g) > a || Math.abs(E - y) > a) && (window.clearTimeout(p), p = null)
                         },
                         h = () => {
                             p && (window.clearTimeout(p), p = null)
                         };
                     c.addEventListener(m, z), c.addEventListener(f, h), c.addEventListener(_, b), c._hold = {
                         handleTouchStart: z,
                         handleTouchEnd: h,
@@ -33571,19 +35014,19 @@
                     const g = z => {
                             z.touches && (_ = z.touches[0].clientX, p = z.touches[0].clientY)
                         },
                         y = z => {
                             const b = z.changedTouches[0].clientX,
                                 h = z.changedTouches[0].clientY,
                                 S = b - (_ || 0),
-                                E = h - (p || 0),
-                                k = Math.abs(S),
-                                D = Math.abs(E);
+                                k = h - (p || 0),
+                                E = Math.abs(S),
+                                I = Math.abs(k);
                             let P = null;
-                            (k > r || D > r) && (k >= D ? P = S > 0 ? "right" : "left" : P = E > 0 ? "down" : "up"), P && (d.modifiers.right && P === "right" || d.modifiers.left && P === "left" || d.modifiers.up && P === "up" || d.modifiers.down && P === "down" || !d.modifiers.right && !d.modifiers.left && !d.modifiers.up && !d.modifiers.down) && d.value(P)
+                            (E > r || I > r) && (E >= I ? P = S > 0 ? "right" : "left" : P = k > 0 ? "down" : "up"), P && (d.modifiers.right && P === "right" || d.modifiers.left && P === "left" || d.modifiers.up && P === "up" || d.modifiers.down && P === "down" || !d.modifiers.right && !d.modifiers.left && !d.modifiers.up && !d.modifiers.down) && d.value(P)
                         };
                     c.addEventListener(m, g), c.addEventListener(f, y), c._swipe = {
                         handleTouchStart: g,
                         handleTouchEnd: y
                     }
                 },
                 unmounted(c) {
@@ -33598,20 +35041,20 @@
                         g = !1;
                     const y = h => {
                             h.touches && (h.preventDefault(), m = h.touches[0].clientX, f = h.touches[0].clientY, _ = c.offsetLeft, p = c.offsetTop, g = !0)
                         },
                         z = h => {
                             if (!g || !h.touches) return;
                             const S = h.touches[0].clientX,
-                                E = h.touches[0].clientY,
-                                k = S - (m || 0),
-                                D = E - (f || 0);
+                                k = h.touches[0].clientY,
+                                E = S - (m || 0),
+                                I = k - (f || 0);
                             d.value({
-                                offsetX: _ + k,
-                                offsetY: p + D
+                                offsetX: _ + E,
+                                offsetY: p + I
                             })
                         },
                         b = () => {
                             g = !1
                         };
                     c.addEventListener(l, y), c.addEventListener(s, z), c.addEventListener(u, b), c._drag = {
                         handleTouchStart: y,
@@ -33664,21 +35107,21 @@
                 unmounted(c) {
                     c._doubletap && c.removeEventListener(l, c._doubletap.handleTouchEnd)
                 }
             })
         }
     };
 
-function Iu(e) {
+function Du(e) {
     return e !== null && typeof e == "object" && "constructor" in e && e.constructor === Object
 }
 
 function _l(e, n) {
     e === void 0 && (e = {}), n === void 0 && (n = {}), Object.keys(n).forEach(t => {
-        typeof e[t] > "u" ? e[t] = n[t] : Iu(n[t]) && Iu(e[t]) && Object.keys(n[t]).length > 0 && _l(e[t], n[t])
+        typeof e[t] > "u" ? e[t] = n[t] : Du(n[t]) && Du(e[t]) && Object.keys(n[t]).length > 0 && _l(e[t], n[t])
     })
 }
 const md = {
     body: {},
     addEventListener() {},
     removeEventListener() {},
     activeElement: {
@@ -33939,42 +35382,42 @@
 function fd(e, n) {
     const t = [];
     let r = e.parentElement;
     for (; r;) n ? r.matches(n) && t.push(r) : t.push(r), r = r.parentElement;
     return t
 }
 
-function Ii(e, n) {
+function Di(e, n) {
     function t(r) {
         r.target === e && (n.call(e, r), e.removeEventListener("transitionend", t))
     }
     n && e.addEventListener("transitionend", t)
 }
 
 function wa(e, n, t) {
     const r = zn();
     return t ? e[n === "width" ? "offsetWidth" : "offsetHeight"] + parseFloat(r.getComputedStyle(e, null).getPropertyValue(n === "width" ? "margin-right" : "margin-top")) + parseFloat(r.getComputedStyle(e, null).getPropertyValue(n === "width" ? "margin-left" : "margin-bottom")) : e.offsetWidth
 }
 
 function Re(e) {
     return (Array.isArray(e) ? e : [e]).filter(n => !!n)
 }
-let Di;
+let Ii;
 
 function Jv() {
     const e = zn(),
         n = mr();
     return {
         smoothScroll: n.documentElement && n.documentElement.style && "scrollBehavior" in n.documentElement.style,
         touch: !!("ontouchstart" in e || e.DocumentTouch && n instanceof e.DocumentTouch)
     }
 }
 
 function _d() {
-    return Di || (Di = Jv()), Di
+    return Ii || (Ii = Jv()), Ii
 }
 let Li;
 
 function ey(e) {
     let {
         userAgent: n
     } = e === void 0 ? {} : e;
@@ -34227,28 +35670,28 @@
     typeof g == "function" && (g = t.slidesOffsetBefore.call(e));
     let y = t.slidesOffsetAfter;
     typeof y == "function" && (y = t.slidesOffsetAfter.call(e));
     const z = e.snapGrid.length,
         b = e.slidesGrid.length;
     let h = t.spaceBetween,
         S = -g,
-        E = 0,
-        k = 0;
+        k = 0,
+        E = 0;
     if (typeof a > "u") return;
     typeof h == "string" && h.indexOf("%") >= 0 ? h = parseFloat(h.replace("%", "")) / 100 * a : typeof h == "string" && (h = parseFloat(h)), e.virtualSize = -h, d.forEach(L => {
         l ? L.style.marginLeft = "" : L.style.marginRight = "", L.style.marginBottom = "", L.style.marginTop = ""
     }), t.centeredSlides && t.cssMode && (co(r, "--swiper-centered-offset-before", ""), co(r, "--swiper-centered-offset-after", ""));
-    const D = t.grid && t.grid.rows > 1 && e.grid;
-    D ? e.grid.initSlides(d) : e.grid && e.grid.unsetSlides();
+    const I = t.grid && t.grid.rows > 1 && e.grid;
+    I ? e.grid.initSlides(d) : e.grid && e.grid.unsetSlides();
     let P;
     const M = t.slidesPerView === "auto" && t.breakpoints && Object.keys(t.breakpoints).filter(L => typeof t.breakpoints[L].slidesPerView < "u").length > 0;
     for (let L = 0; L < m; L += 1) {
         P = 0;
         let F;
-        if (d[L] && (F = d[L]), D && e.grid.updateSlide(L, F, d), !(d[L] && at(F, "display") === "none")) {
+        if (d[L] && (F = d[L]), I && e.grid.updateSlide(L, F, d), !(d[L] && at(F, "display") === "none")) {
             if (t.slidesPerView === "auto") {
                 M && (d[L].style[e.getDirectionLabel("width")] = "");
                 const O = getComputedStyle(F),
                     V = F.style.transform,
                     Z = F.style.webkitTransform;
                 if (V && (F.style.transform = "none"), Z && (F.style.webkitTransform = "none"), t.roundLengths) P = e.isHorizontal() ? wa(F, "width", !0) : wa(F, "height", !0);
                 else {
@@ -34257,26 +35700,26 @@
                         se = n(O, "padding-right"),
                         ue = n(O, "margin-left"),
                         Ue = n(O, "margin-right"),
                         Xe = O.getPropertyValue("box-sizing");
                     if (Xe && Xe === "border-box") P = oe + ue + Ue;
                     else {
                         const {
-                            clientWidth: Ee,
-                            offsetWidth: ke
+                            clientWidth: ke,
+                            offsetWidth: Ee
                         } = F;
-                        P = oe + ie + se + ue + Ue + (ke - Ee)
+                        P = oe + ie + se + ue + Ue + (Ee - ke)
                     }
                 }
                 V && (F.style.transform = V), Z && (F.style.webkitTransform = Z), t.roundLengths && (P = Math.floor(P))
             } else P = (a - (t.slidesPerView - 1) * h) / t.slidesPerView, t.roundLengths && (P = Math.floor(P)), d[L] && (d[L].style[e.getDirectionLabel("width")] = `${P}px`);
-            d[L] && (d[L].swiperSlideSize = P), p.push(P), t.centeredSlides ? (S = S + P / 2 + E / 2 + h, E === 0 && L !== 0 && (S = S - a / 2 - h), L === 0 && (S = S - a / 2 - h), Math.abs(S) < 1 / 1e3 && (S = 0), t.roundLengths && (S = Math.floor(S)), k % t.slidesPerGroup === 0 && f.push(S), _.push(S)) : (t.roundLengths && (S = Math.floor(S)), (k - Math.min(e.params.slidesPerGroupSkip, k)) % e.params.slidesPerGroup === 0 && f.push(S), _.push(S), S = S + P + h), e.virtualSize += P + h, E = P, k += 1
+            d[L] && (d[L].swiperSlideSize = P), p.push(P), t.centeredSlides ? (S = S + P / 2 + k / 2 + h, k === 0 && L !== 0 && (S = S - a / 2 - h), L === 0 && (S = S - a / 2 - h), Math.abs(S) < 1 / 1e3 && (S = 0), t.roundLengths && (S = Math.floor(S)), E % t.slidesPerGroup === 0 && f.push(S), _.push(S)) : (t.roundLengths && (S = Math.floor(S)), (E - Math.min(e.params.slidesPerGroupSkip, E)) % e.params.slidesPerGroup === 0 && f.push(S), _.push(S), S = S + P + h), e.virtualSize += P + h, k = P, E += 1
         }
     }
-    if (e.virtualSize = Math.max(e.virtualSize, a) + y, l && u && (t.effect === "slide" || t.effect === "coverflow") && (r.style.width = `${e.virtualSize+h}px`), t.setWrapperSize && (r.style[e.getDirectionLabel("width")] = `${e.virtualSize+h}px`), D && e.grid.updateWrapperSize(P, f), !t.centeredSlides) {
+    if (e.virtualSize = Math.max(e.virtualSize, a) + y, l && u && (t.effect === "slide" || t.effect === "coverflow") && (r.style.width = `${e.virtualSize+h}px`), t.setWrapperSize && (r.style[e.getDirectionLabel("width")] = `${e.virtualSize+h}px`), I && e.grid.updateWrapperSize(P, f), !t.centeredSlides) {
         const L = [];
         for (let F = 0; F < f.length; F += 1) {
             let O = f[F];
             t.roundLengths && (O = Math.floor(O)), f[F] <= e.virtualSize - a && L.push(O)
         }
         f = L, Math.floor(e.virtualSize - a) - Math.floor(f[f.length - 1]) > 1 && f.push(e.virtualSize - a)
     }
@@ -34473,15 +35916,15 @@
         }
     },
     Ri = (e, n) => {
         if (!e.slides[n]) return;
         const t = e.slides[n].querySelector('[loading="lazy"]');
         t && t.removeAttribute("loading")
     },
-    Ea = e => {
+    ka = e => {
         if (!e || e.destroyed || !e.params) return;
         let n = e.params.lazyPreloadPrevNext;
         const t = e.slides.length;
         if (!t || !n || n < 0) return;
         n = Math.min(n, t);
         const r = e.params.slidesPerView === "auto" ? e.slidesPerViewDynamic() : Math.ceil(e.params.slidesPerView),
             o = e.activeIndex;
@@ -34557,15 +36000,15 @@
     Object.assign(n, {
         previousSnapIndex: u,
         snapIndex: c,
         previousRealIndex: l,
         realIndex: f,
         previousIndex: a,
         activeIndex: s
-    }), n.initialized && Ea(n), n.emit("activeIndexChange"), n.emit("snapIndexChange"), (n.initialized || n.params.runCallbacksOnInit) && (l !== f && n.emit("realIndexChange"), n.emit("slideChange"))
+    }), n.initialized && ka(n), n.emit("activeIndexChange"), n.emit("snapIndexChange"), (n.initialized || n.params.runCallbacksOnInit) && (l !== f && n.emit("realIndexChange"), n.emit("slideChange"))
 }
 
 function py(e, n) {
     const t = this,
         r = t.params;
     let o = e.closest(`.${r.slideClass}, swiper-slide`);
     !o && t.isElement && n && n.length > 1 && n.includes(e) && [...n.slice(n.indexOf(e) + 1, n.length)].forEach(u => {
@@ -34714,31 +36157,31 @@
         swiper: t,
         runCallbacks: e,
         direction: n,
         step: "Start"
     }))
 }
 
-function Ey(e, n) {
+function ky(e, n) {
     e === void 0 && (e = !0);
     const t = this,
         {
             params: r
         } = t;
     t.animating = !1, !r.cssMode && (t.setTransition(0), zd({
         swiper: t,
         runCallbacks: e,
         direction: n,
         step: "End"
     }))
 }
-var ky = {
+var Ey = {
     setTransition: Sy,
     transitionStart: wy,
-    transitionEnd: Ey
+    transitionEnd: ky
 };
 
 function Ay(e, n, t, r, o) {
     e === void 0 && (e = 0), t === void 0 && (t = !0), typeof e == "string" && (e = parseInt(e, 10));
     const a = this;
     let l = e;
     l < 0 && (l = 0);
@@ -34757,30 +36200,30 @@
     const g = Math.min(a.params.slidesPerGroupSkip, l);
     let y = g + Math.floor((l - g) / a.params.slidesPerGroup);
     y >= s.length && (y = s.length - 1);
     const z = -s[y];
     if (u.normalizeSlideIndex)
         for (let h = 0; h < c.length; h += 1) {
             const S = -Math.floor(z * 100),
-                E = Math.floor(c[h] * 100),
-                k = Math.floor(c[h + 1] * 100);
-            typeof c[h + 1] < "u" ? S >= E && S < k - (k - E) / 2 ? l = h : S >= E && S < k && (l = h + 1) : S >= E && (l = h)
+                k = Math.floor(c[h] * 100),
+                E = Math.floor(c[h + 1] * 100);
+            typeof c[h + 1] < "u" ? S >= k && S < E - (E - k) / 2 ? l = h : S >= k && S < E && (l = h + 1) : S >= k && (l = h)
         }
     if (a.initialized && l !== m && (!a.allowSlideNext && (f ? z > a.translate && z > a.minTranslate() : z < a.translate && z < a.minTranslate()) || !a.allowSlidePrev && z > a.translate && z > a.maxTranslate() && (m || 0) !== l)) return !1;
     l !== (d || 0) && t && a.emit("beforeSlideChangeStart"), a.updateProgress(z);
     let b;
     if (l > m ? b = "next" : l < m ? b = "prev" : b = "reset", f && -z === a.translate || !f && z === a.translate) return a.updateActiveIndex(l), u.autoHeight && a.updateAutoHeight(), a.updateSlidesClasses(), u.effect !== "slide" && a.setTranslate(z), b !== "reset" && (a.transitionStart(t, b), a.transitionEnd(t, b)), !1;
     if (u.cssMode) {
         const h = a.isHorizontal(),
             S = f ? z : -z;
         if (n === 0) {
-            const E = a.virtual && a.params.virtual.enabled;
-            E && (a.wrapperEl.style.scrollSnapType = "none", a._immediateVirtual = !0), E && !a._cssModeVirtualInitialSet && a.params.initialSlide > 0 ? (a._cssModeVirtualInitialSet = !0, requestAnimationFrame(() => {
+            const k = a.virtual && a.params.virtual.enabled;
+            k && (a.wrapperEl.style.scrollSnapType = "none", a._immediateVirtual = !0), k && !a._cssModeVirtualInitialSet && a.params.initialSlide > 0 ? (a._cssModeVirtualInitialSet = !0, requestAnimationFrame(() => {
                 _[h ? "scrollLeft" : "scrollTop"] = S
-            })) : _[h ? "scrollLeft" : "scrollTop"] = S, E && requestAnimationFrame(() => {
+            })) : _[h ? "scrollLeft" : "scrollTop"] = S, k && requestAnimationFrame(() => {
                 a.wrapperEl.style.scrollSnapType = "", a._immediateVirtual = !1
             })
         } else {
             if (!a.support.smoothScroll) return dd({
                 swiper: a,
                 targetPosition: S,
                 side: h ? "left" : "top"
@@ -34902,21 +36345,21 @@
         return r.slideTo(z, e, n, t)
     } else if (o.loop && r.activeIndex === 0 && o.cssMode) return requestAnimationFrame(() => {
         r.slideTo(y, e, n, t)
     }), !0;
     return r.slideTo(y, e, n, t)
 }
 
-function Iy(e, n, t) {
+function Dy(e, n, t) {
     n === void 0 && (n = !0);
     const r = this;
     if (!r.destroyed) return typeof e > "u" && (e = r.params.speed), r.slideTo(r.activeIndex, e, n, t)
 }
 
-function Dy(e, n, t, r) {
+function Iy(e, n, t, r) {
     n === void 0 && (n = !0), r === void 0 && (r = .5);
     const o = this;
     if (o.destroyed) return;
     typeof e > "u" && (e = o.params.speed);
     let a = o.activeIndex;
     const l = Math.min(o.params.slidesPerGroupSkip, a),
         u = l + Math.floor((a - l) / o.params.slidesPerGroup),
@@ -34953,16 +36396,16 @@
     } else e.slideTo(o)
 }
 var Oy = {
     slideTo: Ay,
     slideToLoop: Py,
     slideNext: My,
     slidePrev: Cy,
-    slideReset: Iy,
-    slideToClosest: Dy,
+    slideReset: Dy,
+    slideToClosest: Iy,
     slideToClickedSlide: Ly
 };
 
 function xy(e) {
     const n = this,
         {
             params: t,
@@ -35034,18 +36477,18 @@
     const y = _.slidesPerGroupAuto ? g : _.slidesPerGroup;
     let z = y;
     z % y !== 0 && (z += y - z % y), z += _.loopAdditionalSlides, s.loopedSlides = z;
     const b = s.grid && _.grid && _.grid.rows > 1;
     c.length < g + z ? Ro("Swiper Loop Warning: The number of slides is not enough for loop mode, it will be disabled and not function properly. You need to add more slides (or make duplicates) or lower the values of slidesPerView and slidesPerGroup parameters") : b && _.grid.fill === "row" && Ro("Swiper Loop Warning: Loop mode is not compatible with grid.fill = `row`");
     const h = [],
         S = [];
-    let E = s.activeIndex;
-    typeof a > "u" ? a = s.getSlideIndex(c.filter(V => V.classList.contains(_.slideActiveClass))[0]) : E = a;
-    const k = r === "next" || !r,
-        D = r === "prev" || !r;
+    let k = s.activeIndex;
+    typeof a > "u" ? a = s.getSlideIndex(c.filter(V => V.classList.contains(_.slideActiveClass))[0]) : k = a;
+    const E = r === "next" || !r,
+        I = r === "prev" || !r;
     let P = 0,
         M = 0;
     const L = b ? Math.ceil(c.length / _.grid.rows) : c.length,
         O = (b ? c[a].column : a) + (p && typeof o > "u" ? -g / 2 + .5 : 0);
     if (O < z) {
         P = Math.max(z - O, y);
         for (let V = 0; V < z - O; V += 1) {
@@ -35062,35 +36505,35 @@
             b ? c.forEach((oe, ie) => {
                 oe.column === Z && S.push(ie)
             }) : S.push(Z)
         }
     }
     if (s.__preventObserver__ = !0, requestAnimationFrame(() => {
             s.__preventObserver__ = !1
-        }), D && h.forEach(V => {
+        }), I && h.forEach(V => {
             c[V].swiperLoopMoveDOM = !0, f.prepend(c[V]), c[V].swiperLoopMoveDOM = !1
-        }), k && S.forEach(V => {
+        }), E && S.forEach(V => {
             c[V].swiperLoopMoveDOM = !0, f.append(c[V]), c[V].swiperLoopMoveDOM = !1
-        }), s.recalcSlides(), _.slidesPerView === "auto" ? s.updateSlides() : b && (h.length > 0 && D || S.length > 0 && k) && s.slides.forEach((V, Z) => {
+        }), s.recalcSlides(), _.slidesPerView === "auto" ? s.updateSlides() : b && (h.length > 0 && I || S.length > 0 && E) && s.slides.forEach((V, Z) => {
             s.grid.updateSlide(Z, V, s.slides)
         }), _.watchSlidesProgress && s.updateSlidesOffset(), t) {
-        if (h.length > 0 && D) {
+        if (h.length > 0 && I) {
             if (typeof n > "u") {
-                const V = s.slidesGrid[E],
-                    oe = s.slidesGrid[E + P] - V;
-                u ? s.setTranslate(s.translate - oe) : (s.slideTo(E + Math.ceil(P), 0, !1, !0), o && (s.touchEventsData.startTranslate = s.touchEventsData.startTranslate - oe, s.touchEventsData.currentTranslate = s.touchEventsData.currentTranslate - oe))
+                const V = s.slidesGrid[k],
+                    oe = s.slidesGrid[k + P] - V;
+                u ? s.setTranslate(s.translate - oe) : (s.slideTo(k + Math.ceil(P), 0, !1, !0), o && (s.touchEventsData.startTranslate = s.touchEventsData.startTranslate - oe, s.touchEventsData.currentTranslate = s.touchEventsData.currentTranslate - oe))
             } else if (o) {
                 const V = b ? h.length / _.grid.rows : h.length;
                 s.slideTo(s.activeIndex + V, 0, !1, !0), s.touchEventsData.currentTranslate = s.translate
             }
-        } else if (S.length > 0 && k)
+        } else if (S.length > 0 && E)
             if (typeof n > "u") {
-                const V = s.slidesGrid[E],
-                    oe = s.slidesGrid[E - M] - V;
-                u ? s.setTranslate(s.translate - oe) : (s.slideTo(E - M, 0, !1, !0), o && (s.touchEventsData.startTranslate = s.touchEventsData.startTranslate - oe, s.touchEventsData.currentTranslate = s.touchEventsData.currentTranslate - oe))
+                const V = s.slidesGrid[k],
+                    oe = s.slidesGrid[k - M] - V;
+                u ? s.setTranslate(s.translate - oe) : (s.slideTo(k - M, 0, !1, !0), o && (s.touchEventsData.startTranslate = s.touchEventsData.startTranslate - oe, s.touchEventsData.currentTranslate = s.touchEventsData.currentTranslate - oe))
             } else {
                 const V = b ? S.length / _.grid.rows : S.length;
                 s.slideTo(s.activeIndex - V, 0, !1, !0)
             }
     }
     if (s.allowSlidePrev = d, s.allowSlideNext = m, s.controller && s.controller.control && !l) {
         const V = {
@@ -35165,15 +36608,15 @@
         r.assignedSlot && (r = r.assignedSlot);
         const o = r.closest(e);
         return !o && !r.getRootNode ? null : o || t(r.getRootNode().host)
     }
     return t(n)
 }
 
-function Du(e, n, t) {
+function Iu(e, n, t) {
     const r = zn(),
         {
             params: o
         } = e,
         a = o.edgeSwipeDetection,
         l = o.edgeSwipeThreshold;
     return a && (t <= l || t >= r.innerWidth - l) ? a === "prevent" ? (n.preventDefault(), !0) : !1 : !0
@@ -35186,15 +36629,15 @@
     r.originalEvent && (r = r.originalEvent);
     const o = n.touchEventsData;
     if (r.type === "pointerdown") {
         if (o.pointerId !== null && o.pointerId !== r.pointerId) return;
         o.pointerId = r.pointerId
     } else r.type === "touchstart" && r.targetTouches.length === 1 && (o.touchId = r.targetTouches[0].identifier);
     if (r.type === "touchstart") {
-        Du(n, r, r.targetTouches[0].pageX);
+        Iu(n, r, r.targetTouches[0].pageX);
         return
     }
     const {
         params: a,
         touches: l,
         enabled: u
     } = n;
@@ -35211,15 +36654,15 @@
         n.allowClick = !0;
         return
     }
     if (a.swipeHandler && !s.closest(a.swipeHandler)) return;
     l.currentX = r.pageX, l.currentY = r.pageY;
     const _ = l.currentX,
         p = l.currentY;
-    if (!Du(n, r, _)) return;
+    if (!Iu(n, r, _)) return;
     Object.assign(o, {
         isTouched: !0,
         isMoved: !1,
         allowTouchCallbacks: !0,
         isScrolling: void 0,
         startMoving: void 0
     }), l.startX = _, l.startY = p, o.touchStartTime = At(), n.allowClick = !0, n.updateSize(), n.swipeDirection = void 0, a.threshold > 0 && (o.allowThresholdMove = !1);
@@ -35240,15 +36683,15 @@
             enabled: u
         } = t;
     if (!u || !o.simulateTouch && e.pointerType === "mouse") return;
     let s = e;
     if (s.originalEvent && (s = s.originalEvent), s.type === "pointermove" && (r.touchId !== null || s.pointerId !== r.pointerId)) return;
     let c;
     if (s.type === "touchmove") {
-        if (c = [...s.changedTouches].filter(k => k.identifier === r.touchId)[0], !c || c.identifier !== r.touchId) return
+        if (c = [...s.changedTouches].filter(E => E.identifier === r.touchId)[0], !c || c.identifier !== r.touchId) return
     } else c = s;
     if (!r.isTouched) {
         r.startMoving && r.isScrolling && t.emit("touchMoveOpposite", s);
         return
     }
     const d = c.pageX,
         m = c.pageY;
@@ -35278,16 +36721,16 @@
         return
     }
     r.allowTouchCallbacks && t.emit("touchMove", s), a.previousX = a.currentX, a.previousY = a.currentY, a.currentX = d, a.currentY = m;
     const f = a.currentX - a.startX,
         _ = a.currentY - a.startY;
     if (t.params.threshold && Math.sqrt(f ** 2 + _ ** 2) < t.params.threshold) return;
     if (typeof r.isScrolling > "u") {
-        let k;
-        t.isHorizontal() && a.currentY === a.startY || t.isVertical() && a.currentX === a.startX ? r.isScrolling = !1 : f * f + _ * _ >= 25 && (k = Math.atan2(Math.abs(_), Math.abs(f)) * 180 / Math.PI, r.isScrolling = t.isHorizontal() ? k > o.touchAngle : 90 - k > o.touchAngle)
+        let E;
+        t.isHorizontal() && a.currentY === a.startY || t.isVertical() && a.currentX === a.startX ? r.isScrolling = !1 : f * f + _ * _ >= 25 && (E = Math.atan2(Math.abs(_), Math.abs(f)) * 180 / Math.PI, r.isScrolling = t.isHorizontal() ? E > o.touchAngle : 90 - E > o.touchAngle)
     }
     if (r.isScrolling && t.emit("touchMoveOpposite", s), typeof r.startMoving > "u" && (a.currentX !== a.startX || a.currentY !== a.startY) && (r.startMoving = !0), r.isScrolling) {
         r.isTouched = !1;
         return
     }
     if (!r.startMoving) return;
     t.allowClick = !1, !o.cssMode && s.cancelable && s.preventDefault(), o.touchMoveStopPropagation && !o.nested && s.stopPropagation();
@@ -35298,19 +36741,19 @@
     t.swipeDirection = p > 0 ? "prev" : "next", t.touchesDirection = g > 0 ? "prev" : "next";
     const z = t.params.loop && !o.cssMode,
         b = t.touchesDirection === "next" && t.allowSlideNext || t.touchesDirection === "prev" && t.allowSlidePrev;
     if (!r.isMoved) {
         if (z && b && t.loopFix({
                 direction: t.swipeDirection
             }), r.startTranslate = t.getTranslate(), t.setTransition(0), t.animating) {
-            const k = new window.CustomEvent("transitionend", {
+            const E = new window.CustomEvent("transitionend", {
                 bubbles: !0,
                 cancelable: !0
             });
-            t.wrapperEl.dispatchEvent(k)
+            t.wrapperEl.dispatchEvent(E)
         }
         r.allowMomentumBounce = !1, o.grabCursor && (t.allowSlideNext === !0 || t.allowSlidePrev === !0) && t.setGrabCursor(!0), t.emit("sliderFirstMove", s)
     }
     let h;
     if (new Date().getTime(), r.isMoved && r.allowThresholdMove && y !== t.touchesDirection && z && b && Math.abs(p) >= 1) {
         Object.assign(a, {
             startX: d,
@@ -35319,24 +36762,24 @@
             currentY: m,
             startTranslate: r.currentTranslate
         }), r.loopSwapReset = !0, r.startTranslate = r.currentTranslate;
         return
     }
     t.emit("sliderMove", s), r.isMoved = !0, r.currentTranslate = p + r.startTranslate;
     let S = !0,
-        E = o.resistanceRatio;
-    if (o.touchReleaseOnEdges && (E = 0), p > 0 ? (z && b && !h && r.allowThresholdMove && r.currentTranslate > (o.centeredSlides ? t.minTranslate() - t.slidesSizesGrid[t.activeIndex + 1] : t.minTranslate()) && t.loopFix({
+        k = o.resistanceRatio;
+    if (o.touchReleaseOnEdges && (k = 0), p > 0 ? (z && b && !h && r.allowThresholdMove && r.currentTranslate > (o.centeredSlides ? t.minTranslate() - t.slidesSizesGrid[t.activeIndex + 1] : t.minTranslate()) && t.loopFix({
             direction: "prev",
             setTranslate: !0,
             activeSlideIndex: 0
-        }), r.currentTranslate > t.minTranslate() && (S = !1, o.resistance && (r.currentTranslate = t.minTranslate() - 1 + (-t.minTranslate() + r.startTranslate + p) ** E))) : p < 0 && (z && b && !h && r.allowThresholdMove && r.currentTranslate < (o.centeredSlides ? t.maxTranslate() + t.slidesSizesGrid[t.slidesSizesGrid.length - 1] : t.maxTranslate()) && t.loopFix({
+        }), r.currentTranslate > t.minTranslate() && (S = !1, o.resistance && (r.currentTranslate = t.minTranslate() - 1 + (-t.minTranslate() + r.startTranslate + p) ** k))) : p < 0 && (z && b && !h && r.allowThresholdMove && r.currentTranslate < (o.centeredSlides ? t.maxTranslate() + t.slidesSizesGrid[t.slidesSizesGrid.length - 1] : t.maxTranslate()) && t.loopFix({
             direction: "next",
             setTranslate: !0,
             activeSlideIndex: t.slides.length - (o.slidesPerView === "auto" ? t.slidesPerViewDynamic() : Math.ceil(parseFloat(o.slidesPerView, 10)))
-        }), r.currentTranslate < t.maxTranslate() && (S = !1, o.resistance && (r.currentTranslate = t.maxTranslate() + 1 - (t.maxTranslate() - r.startTranslate - p) ** E))), S && (s.preventedByNestedSwiper = !0), !t.allowSlideNext && t.swipeDirection === "next" && r.currentTranslate < r.startTranslate && (r.currentTranslate = r.startTranslate), !t.allowSlidePrev && t.swipeDirection === "prev" && r.currentTranslate > r.startTranslate && (r.currentTranslate = r.startTranslate), !t.allowSlidePrev && !t.allowSlideNext && (r.currentTranslate = r.startTranslate), o.threshold > 0)
+        }), r.currentTranslate < t.maxTranslate() && (S = !1, o.resistance && (r.currentTranslate = t.maxTranslate() + 1 - (t.maxTranslate() - r.startTranslate - p) ** k))), S && (s.preventedByNestedSwiper = !0), !t.allowSlideNext && t.swipeDirection === "next" && r.currentTranslate < r.startTranslate && (r.currentTranslate = r.startTranslate), !t.allowSlidePrev && t.swipeDirection === "prev" && r.currentTranslate > r.startTranslate && (r.currentTranslate = r.startTranslate), !t.allowSlidePrev && !t.allowSlideNext && (r.currentTranslate = r.startTranslate), o.threshold > 0)
         if (Math.abs(p) > o.threshold || r.allowThresholdMove) {
             if (!r.allowThresholdMove) {
                 r.allowThresholdMove = !0, a.startX = a.currentX, a.startY = a.currentY, r.currentTranslate = r.startTranslate, a.diff = t.isHorizontal() ? a.currentX - a.startX : a.currentY - a.startY;
                 return
             }
         } else {
             r.currentTranslate = r.startTranslate;
@@ -35347,15 +36790,15 @@
 function qy(e) {
     const n = this,
         t = n.touchEventsData;
     let r = e;
     r.originalEvent && (r = r.originalEvent);
     let o;
     if (r.type === "touchend" || r.type === "touchcancel") {
-        if (o = [...r.changedTouches].filter(E => E.identifier === t.touchId)[0], !o || o.identifier !== t.touchId) return
+        if (o = [...r.changedTouches].filter(k => k.identifier === t.touchId)[0], !o || o.identifier !== t.touchId) return
     } else {
         if (t.touchId !== null || r.pointerId !== t.pointerId) return;
         o = r
     }
     if (["pointercancel", "pointerout", "pointerleave", "contextmenu"].includes(r.type) && !(["pointercancel", "contextmenu"].includes(r.type) && (n.browser.isSafari || n.browser.isWebView))) return;
     t.pointerId = null, t.touchId = null;
     const {
@@ -35370,16 +36813,16 @@
         t.isMoved && l.grabCursor && n.setGrabCursor(!1), t.isMoved = !1, t.startMoving = !1;
         return
     }
     l.grabCursor && t.isMoved && t.isTouched && (n.allowSlideNext === !0 || n.allowSlidePrev === !0) && n.setGrabCursor(!1);
     const m = At(),
         f = m - t.touchStartTime;
     if (n.allowClick) {
-        const E = r.path || r.composedPath && r.composedPath();
-        n.updateClickedSlide(E && E[0] || r.target, E), n.emit("tap click", r), f < 300 && m - t.lastClickTime < 300 && n.emit("doubleTap doubleClick", r)
+        const k = r.path || r.composedPath && r.composedPath();
+        n.updateClickedSlide(k && k[0] || r.target, k), n.emit("tap click", r), f < 300 && m - t.lastClickTime < 300 && n.emit("doubleTap doubleClick", r)
     }
     if (t.lastClickTime = At(), Sa(() => {
             n.destroyed || (n.allowClick = !0)
         }), !t.isTouched || !t.isMoved || !n.swipeDirection || u.diff === 0 && !t.loopSwapReset || t.currentTranslate === t.startTranslate && !t.loopSwapReset) {
         t.isTouched = !1, t.isMoved = !1, t.startMoving = !1;
         return
     }
@@ -35391,17 +36834,17 @@
             currentPos: _
         });
         return
     }
     const p = _ >= -n.maxTranslate() && !n.params.loop;
     let g = 0,
         y = n.slidesSizesGrid[0];
-    for (let E = 0; E < c.length; E += E < l.slidesPerGroupSkip ? 1 : l.slidesPerGroup) {
-        const k = E < l.slidesPerGroupSkip - 1 ? 1 : l.slidesPerGroup;
-        typeof c[E + k] < "u" ? (p || _ >= c[E] && _ < c[E + k]) && (g = E, y = c[E + k] - c[E]) : (p || _ >= c[E]) && (g = E, y = c[c.length - 1] - c[c.length - 2])
+    for (let k = 0; k < c.length; k += k < l.slidesPerGroupSkip ? 1 : l.slidesPerGroup) {
+        const E = k < l.slidesPerGroupSkip - 1 ? 1 : l.slidesPerGroup;
+        typeof c[k + E] < "u" ? (p || _ >= c[k] && _ < c[k + E]) && (g = k, y = c[k + E] - c[k]) : (p || _ >= c[k]) && (g = k, y = c[c.length - 1] - c[c.length - 2])
     }
     let z = null,
         b = null;
     l.rewind && (n.isBeginning ? b = l.virtual && l.virtual.enabled && n.virtual ? n.virtual.slides.length - 1 : n.slides.length - 1 : n.isEnd && (z = 0));
     const h = (_ - c[g]) / y,
         S = g < l.slidesPerGroupSkip - 1 ? 1 : l.slidesPerGroup;
     if (f > l.longSwipesMs) {
@@ -35544,16 +36987,16 @@
         d = Ou(e, s),
         m = e.params.grabCursor,
         f = s.grabCursor,
         _ = r.enabled;
     c && !d ? (o.classList.remove(`${r.containerModifierClass}grid`, `${r.containerModifierClass}grid-column`), e.emitContainerClasses()) : !c && d && (o.classList.add(`${r.containerModifierClass}grid`), (s.grid.fill && s.grid.fill === "column" || !s.grid.fill && r.grid.fill === "column") && o.classList.add(`${r.containerModifierClass}grid-column`), e.emitContainerClasses()), m && !f ? e.unsetGrabCursor() : !m && f && e.setGrabCursor(), ["navigation", "pagination", "scrollbar"].forEach(h => {
         if (typeof s[h] > "u") return;
         const S = r[h] && r[h].enabled,
-            E = s[h] && s[h].enabled;
-        S && !E && e[h].disable(), !S && E && e[h].enable()
+            k = s[h] && s[h].enabled;
+        S && !k && e[h].disable(), !S && k && e[h].enable()
     });
     const p = s.direction && s.direction !== r.direction,
         g = r.loop && (s.slidesPerView !== r.slidesPerView || p),
         y = r.loop;
     p && t && e.changeDirection(), cn(e.params, s);
     const z = e.params.enabled,
         b = e.params.loop;
@@ -35667,15 +37110,15 @@
         e.isLocked = e.size > a
     } else e.isLocked = e.snapGrid.length === 1;
     t.allowSlideNext === !0 && (e.allowSlideNext = !e.isLocked), t.allowSlidePrev === !0 && (e.allowSlidePrev = !e.isLocked), n && n !== e.isLocked && (e.isEnd = !1), n !== e.isLocked && e.emit(e.isLocked ? "lock" : "unlock")
 }
 var l1 = {
         checkOverflow: a1
     },
-    ka = {
+    Ea = {
         init: !0,
         direction: "horizontal",
         oneWayMovement: !1,
         swiperElementNodeName: "SWIPER-CONTAINER",
         touchEventsTarget: "wrapper",
         initialSlide: 0,
         speed: 300,
@@ -35783,15 +37226,15 @@
         }), cn(n, r)
     }
 }
 const Ni = {
         eventsEmitter: iy,
         update: zy,
         translate: Ty,
-        transition: ky,
+        transition: Ey,
         slide: Oy,
         loop: Gy,
         grabCursor: Fy,
         events: Zy,
         breakpoints: n1,
         checkOverflow: l1,
         classes: i1
@@ -35824,15 +37267,15 @@
                 extendParams: s1(t, s),
                 on: u.on.bind(u),
                 once: u.once.bind(u),
                 off: u.off.bind(u),
                 emit: u.emit.bind(u)
             })
         });
-        const c = cn({}, ka, s);
+        const c = cn({}, Ea, s);
         return u.params = cn({}, c, Gi, t), u.originalParams = cn({}, u.params), u.passedParams = cn({}, t), u.params && u.params.on && Object.keys(u.params.on).forEach(d => {
             u.on(d, u.params.on[d])
         }), u.params && u.params.onAny && u.onAny(u.params.onAny), Object.assign(u, {
             enabled: u.params.enabled,
             el: n,
             classNames: [],
             slides: [],
@@ -36046,15 +37489,15 @@
         if (t.initialized || t.mount(n) === !1) return t;
         t.emit("beforeInit"), t.params.breakpoints && t.setBreakpoint(), t.addClasses(), t.updateSize(), t.updateSlides(), t.params.watchOverflow && t.checkOverflow(), t.params.grabCursor && t.enabled && t.setGrabCursor(), t.params.loop && t.virtual && t.params.virtual.enabled ? t.slideTo(t.params.initialSlide + t.virtual.slidesBefore, 0, t.params.runCallbacksOnInit, !1, !0) : t.slideTo(t.params.initialSlide, 0, t.params.runCallbacksOnInit, !1, !0), t.params.loop && t.loopCreate(), t.attachEvents();
         const o = [...t.el.querySelectorAll('[loading="lazy"]')];
         return t.isElement && o.push(...t.hostEl.querySelectorAll('[loading="lazy"]')), o.forEach(a => {
             a.complete ? ho(t, a) : a.addEventListener("load", l => {
                 ho(t, l.target)
             })
-        }), Ea(t), t.initialized = !0, Ea(t), t.emit("init"), t.emit("afterInit"), t
+        }), ka(t), t.initialized = !0, ka(t), t.emit("init"), t.emit("afterInit"), t
     }
     destroy(n, t) {
         n === void 0 && (n = !0), t === void 0 && (t = !0);
         const r = this,
             {
                 params: o,
                 el: a,
@@ -36070,15 +37513,15 @@
     static extendDefaults(n) {
         cn(Gi, n)
     }
     static get extendedDefaults() {
         return Gi
     }
     static get defaults() {
-        return ka
+        return Ea
     }
     static installModule(n) {
         Fn.prototype.__modules__ || (Fn.prototype.__modules__ = []);
         const t = Fn.prototype.__modules__;
         typeof n == "function" && t.indexOf(n) < 0 && t.push(n)
     }
     static use(n) {
@@ -36145,36 +37588,36 @@
             params: d,
             pagination: m,
             navigation: f,
             scrollbar: _,
             virtual: p,
             thumbs: g
         } = n;
-    let y, z, b, h, S, E, k, D;
+    let y, z, b, h, S, k, E, I;
     o.includes("thumbs") && r.thumbs && r.thumbs.swiper && d.thumbs && !d.thumbs.swiper && (y = !0), o.includes("controller") && r.controller && r.controller.control && d.controller && !d.controller.control && (z = !0), o.includes("pagination") && r.pagination && (r.pagination.el || s) && (d.pagination || d.pagination === !1) && m && !m.el && (b = !0), o.includes("scrollbar") && r.scrollbar && (r.scrollbar.el || u) && (d.scrollbar || d.scrollbar === !1) && _ && !_.el && (h = !0), o.includes("navigation") && r.navigation && (r.navigation.prevEl || l) && (r.navigation.nextEl || a) && (d.navigation || d.navigation === !1) && f && !f.prevEl && !f.nextEl && (S = !0);
     const P = M => {
         n[M] && (n[M].destroy(), M === "navigation" ? (n.isElement && (n[M].prevEl.remove(), n[M].nextEl.remove()), d[M].prevEl = void 0, d[M].nextEl = void 0, n[M].prevEl = void 0, n[M].nextEl = void 0) : (n.isElement && n[M].el.remove(), d[M].el = void 0, n[M].el = void 0))
     };
-    o.includes("loop") && n.isElement && (d.loop && !r.loop ? E = !0 : !d.loop && r.loop ? k = !0 : D = !0), c.forEach(M => {
+    o.includes("loop") && n.isElement && (d.loop && !r.loop ? k = !0 : !d.loop && r.loop ? E = !0 : I = !0), c.forEach(M => {
         if (Mt(d[M]) && Mt(r[M])) Object.assign(d[M], r[M]), (M === "navigation" || M === "pagination" || M === "scrollbar") && "enabled" in r[M] && !r[M].enabled && P(M);
         else {
             const L = r[M];
             (L === !0 || L === !1) && (M === "navigation" || M === "pagination" || M === "scrollbar") ? L === !1 && P(M): d[M] = r[M]
         }
-    }), c.includes("controller") && !z && n.controller && n.controller.control && d.controller && d.controller.control && (n.controller.control = d.controller.control), o.includes("children") && t && p && d.virtual.enabled ? (p.slides = t, p.update(!0)) : o.includes("virtual") && p && d.virtual.enabled && (t && (p.slides = t), p.update(!0)), o.includes("children") && t && d.loop && (D = !0), y && g.init() && g.update(!0), z && (n.controller.control = d.controller.control), b && (n.isElement && (!s || typeof s == "string") && (s = document.createElement("div"), s.classList.add("swiper-pagination"), s.part.add("pagination"), n.el.appendChild(s)), s && (d.pagination.el = s), m.init(), m.render(), m.update()), h && (n.isElement && (!u || typeof u == "string") && (u = document.createElement("div"), u.classList.add("swiper-scrollbar"), u.part.add("scrollbar"), n.el.appendChild(u)), u && (d.scrollbar.el = u), _.init(), _.updateSize(), _.setTranslate()), S && (n.isElement && ((!a || typeof a == "string") && (a = document.createElement("div"), a.classList.add("swiper-button-next"), a.innerHTML = n.hostEl.constructor.nextButtonSvg, a.part.add("button-next"), n.el.appendChild(a)), (!l || typeof l == "string") && (l = document.createElement("div"), l.classList.add("swiper-button-prev"), l.innerHTML = n.hostEl.constructor.prevButtonSvg, l.part.add("button-prev"), n.el.appendChild(l))), a && (d.navigation.nextEl = a), l && (d.navigation.prevEl = l), f.init(), f.update()), o.includes("allowSlideNext") && (n.allowSlideNext = r.allowSlideNext), o.includes("allowSlidePrev") && (n.allowSlidePrev = r.allowSlidePrev), o.includes("direction") && n.changeDirection(r.direction, !1), (E || D) && n.loopDestroy(), (k || D) && n.loopCreate(), n.update()
+    }), c.includes("controller") && !z && n.controller && n.controller.control && d.controller && d.controller.control && (n.controller.control = d.controller.control), o.includes("children") && t && p && d.virtual.enabled ? (p.slides = t, p.update(!0)) : o.includes("virtual") && p && d.virtual.enabled && (t && (p.slides = t), p.update(!0)), o.includes("children") && t && d.loop && (I = !0), y && g.init() && g.update(!0), z && (n.controller.control = d.controller.control), b && (n.isElement && (!s || typeof s == "string") && (s = document.createElement("div"), s.classList.add("swiper-pagination"), s.part.add("pagination"), n.el.appendChild(s)), s && (d.pagination.el = s), m.init(), m.render(), m.update()), h && (n.isElement && (!u || typeof u == "string") && (u = document.createElement("div"), u.classList.add("swiper-scrollbar"), u.part.add("scrollbar"), n.el.appendChild(u)), u && (d.scrollbar.el = u), _.init(), _.updateSize(), _.setTranslate()), S && (n.isElement && ((!a || typeof a == "string") && (a = document.createElement("div"), a.classList.add("swiper-button-next"), a.innerHTML = n.hostEl.constructor.nextButtonSvg, a.part.add("button-next"), n.el.appendChild(a)), (!l || typeof l == "string") && (l = document.createElement("div"), l.classList.add("swiper-button-prev"), l.innerHTML = n.hostEl.constructor.prevButtonSvg, l.part.add("button-prev"), n.el.appendChild(l))), a && (d.navigation.nextEl = a), l && (d.navigation.prevEl = l), f.init(), f.update()), o.includes("allowSlideNext") && (n.allowSlideNext = r.allowSlideNext), o.includes("allowSlidePrev") && (n.allowSlidePrev = r.allowSlidePrev), o.includes("direction") && n.changeDirection(r.direction, !1), (k || I) && n.loopDestroy(), (E || I) && n.loopCreate(), n.update()
 }
 
 function xu(e, n) {
     e === void 0 && (e = {}), n === void 0 && (n = !0);
     const t = {
             on: {}
         },
         r = {},
         o = {};
-    Qt(t, ka), t._emitClasses = !0, t.init = !1;
+    Qt(t, Ea), t._emitClasses = !0, t.init = !1;
     const a = {},
         l = gd.map(s => s.replace(/_/, "")),
         u = Object.assign({}, e);
     return Object.keys(u).forEach(s => {
         typeof e[s] > "u" || (l.indexOf(s) >= 0 ? Mt(e[s]) ? (t[s] = {}, o[s] = {}, Qt(t[s], e[s]), Qt(o[s], e[s])) : (t[s] = e[s], o[s] = e[s]) : s.search(/on[A-Z]/) === 0 && typeof e[s] == "function" ? n ? r[`${s[2].toLowerCase()}${s.substr(3)}`] = e[s] : t.on[`${s[2].toLowerCase()}${s.substr(3)}`] = e[s] : a[s] = e[s])
     }), ["navigation", "pagination", "scrollbar"].forEach(s => {
         t[s] === !0 && (t[s] = {}), t[s] === !1 && delete t[s]
@@ -36740,30 +38183,30 @@
             }, p = {
                 value: []
             }, g = he(null), y = he(null), z = he(null), b = he(null), {
                 params: h,
                 passedParams: S
             } = xu(e, !1);
             Bi(t, _, p), f.value = S, p.value = _.value;
-            const E = () => {
+            const k = () => {
                 Bi(t, _, p), s.value = !0
             };
             h.onAny = function(P) {
                 for (var M = arguments.length, L = new Array(M > 1 ? M - 1 : 0), F = 1; F < M; F++) L[F - 1] = arguments[F];
                 r(P, ...L)
             }, Object.assign(h.on, {
-                _beforeBreakpoint: E,
+                _beforeBreakpoint: k,
                 _containerClasses(P, M) {
                     l.value = M
                 }
             });
-            const k = {
+            const E = {
                 ...h
             };
-            if (delete k.wrapperClass, m.value = new si(k), m.value.virtual && m.value.params.virtual.enabled) {
+            if (delete E.wrapperClass, m.value = new si(E), m.value.virtual && m.value.params.virtual.enabled) {
                 m.value.virtual.slides = _.value;
                 const P = {
                     cache: !1,
                     slides: _.value,
                     renderExternal: M => {
                         u.value = M
                     },
@@ -36799,30 +38242,30 @@
                     scrollbarEl: b.value,
                     swiper: m.value
                 }, h), r("swiper", m.value))
             }), Xo(() => {
                 m.value && !m.value.destroyed && m.value.destroy(!0, !1)
             });
 
-            function D(P) {
+            function I(P) {
                 return h.virtual ? _1(m, P, u.value) : (P.forEach((M, L) => {
                     M.props || (M.props = {}), M.props.swiperRef = m, M.props.swiperSlideIndex = L
                 }), P)
             }
             return () => {
                 const {
                     slides: P,
                     slots: M
                 } = Bi(t, _, p);
                 return Ge(o, {
                     ref: d,
                     class: Td(l.value)
                 }, [M["container-start"], Ge(a, {
                     class: u1(h.wrapperClass)
-                }, [M["wrapper-start"], D(P), M["wrapper-end"]]), bd(e) && [Ge("div", {
+                }, [M["wrapper-start"], I(P), M["wrapper-end"]]), bd(e) && [Ge("div", {
                     ref: y,
                     class: "swiper-button-prev"
                 }), Ge("div", {
                     ref: g,
                     class: "swiper-button-next"
                 })], yd(e) && Ge("div", {
                     ref: b,
@@ -37118,23 +38561,23 @@
 
     function m() {
         const z = n.rtl,
             b = n.params.pagination;
         if (s()) return;
         let h = n.pagination.el;
         h = Re(h);
-        let S, E;
-        const k = n.virtual && n.params.virtual.enabled ? n.virtual.slides.length : n.slides.length,
-            D = n.params.loop ? Math.ceil(k / n.params.slidesPerGroup) : n.snapGrid.length;
-        if (n.params.loop ? (E = n.previousRealIndex || 0, S = n.params.slidesPerGroup > 1 ? Math.floor(n.realIndex / n.params.slidesPerGroup) : n.realIndex) : typeof n.snapIndex < "u" ? (S = n.snapIndex, E = n.previousSnapIndex) : (E = n.previousIndex || 0, S = n.activeIndex || 0), b.type === "bullets" && n.pagination.bullets && n.pagination.bullets.length > 0) {
+        let S, k;
+        const E = n.virtual && n.params.virtual.enabled ? n.virtual.slides.length : n.slides.length,
+            I = n.params.loop ? Math.ceil(E / n.params.slidesPerGroup) : n.snapGrid.length;
+        if (n.params.loop ? (k = n.previousRealIndex || 0, S = n.params.slidesPerGroup > 1 ? Math.floor(n.realIndex / n.params.slidesPerGroup) : n.realIndex) : typeof n.snapIndex < "u" ? (S = n.snapIndex, k = n.previousSnapIndex) : (k = n.previousIndex || 0, S = n.activeIndex || 0), b.type === "bullets" && n.pagination.bullets && n.pagination.bullets.length > 0) {
             const P = n.pagination.bullets;
             let M, L, F;
             if (b.dynamicBullets && (l = wa(P[0], n.isHorizontal() ? "width" : "height", !0), h.forEach(O => {
                     O.style[n.isHorizontal() ? "width" : "height"] = `${l*(b.dynamicMainBullets+4)}px`
-                }), b.dynamicMainBullets > 1 && E !== void 0 && (u += S - (E || 0), u > b.dynamicMainBullets - 1 ? u = b.dynamicMainBullets - 1 : u < 0 && (u = 0)), M = Math.max(S - u, 0), L = M + (Math.min(P.length, b.dynamicMainBullets) - 1), F = (L + M) / 2), P.forEach(O => {
+                }), b.dynamicMainBullets > 1 && k !== void 0 && (u += S - (k || 0), u > b.dynamicMainBullets - 1 ? u = b.dynamicMainBullets - 1 : u < 0 && (u = 0)), M = Math.max(S - u, 0), L = M + (Math.min(P.length, b.dynamicMainBullets) - 1), F = (L + M) / 2), P.forEach(O => {
                     const V = [...["", "-next", "-next-next", "-prev", "-prev-prev", "-main"].map(Z => `${b.bulletActiveClass}${Z}`)].map(Z => typeof Z == "string" && Z.includes(" ") ? Z.split(" ") : Z).flat();
                     O.classList.remove(...V)
                 }), h.length > 1) P.forEach(O => {
                 const V = Go(O);
                 V === S ? O.classList.add(...b.bulletActiveClass.split(" ")) : n.isElement && O.setAttribute("part", "bullet"), b.dynamicBullets && (V >= M && V <= L && O.classList.add(...`${b.bulletActiveClass}-main`.split(" ")), V === M && c(O, "prev"), V === L && c(O, "next"))
             });
             else {
@@ -37157,43 +38600,43 @@
                 })
             }
         }
         h.forEach((P, M) => {
             if (b.type === "fraction" && (P.querySelectorAll(zr(b.currentClass)).forEach(L => {
                     L.textContent = b.formatFractionCurrent(S + 1)
                 }), P.querySelectorAll(zr(b.totalClass)).forEach(L => {
-                    L.textContent = b.formatFractionTotal(D)
+                    L.textContent = b.formatFractionTotal(I)
                 })), b.type === "progressbar") {
                 let L;
                 b.progressbarOpposite ? L = n.isHorizontal() ? "vertical" : "horizontal" : L = n.isHorizontal() ? "horizontal" : "vertical";
-                const F = (S + 1) / D;
+                const F = (S + 1) / I;
                 let O = 1,
                     V = 1;
                 L === "horizontal" ? O = F : V = F, P.querySelectorAll(zr(b.progressbarFillClass)).forEach(Z => {
                     Z.style.transform = `translate3d(0,0,0) scaleX(${O}) scaleY(${V})`, Z.style.transitionDuration = `${n.params.speed}ms`
                 })
             }
-            b.type === "custom" && b.renderCustom ? (P.innerHTML = b.renderCustom(n, S + 1, D), M === 0 && o("paginationRender", P)) : (M === 0 && o("paginationRender", P), o("paginationUpdate", P)), n.params.watchOverflow && n.enabled && P.classList[n.isLocked ? "add" : "remove"](b.lockClass)
+            b.type === "custom" && b.renderCustom ? (P.innerHTML = b.renderCustom(n, S + 1, I), M === 0 && o("paginationRender", P)) : (M === 0 && o("paginationRender", P), o("paginationUpdate", P)), n.params.watchOverflow && n.enabled && P.classList[n.isLocked ? "add" : "remove"](b.lockClass)
         })
     }
 
     function f() {
         const z = n.params.pagination;
         if (s()) return;
         const b = n.virtual && n.params.virtual.enabled ? n.virtual.slides.length : n.grid && n.params.grid.rows > 1 ? n.slides.length / Math.ceil(n.params.grid.rows) : n.slides.length;
         let h = n.pagination.el;
         h = Re(h);
         let S = "";
         if (z.type === "bullets") {
-            let E = n.params.loop ? Math.ceil(b / n.params.slidesPerGroup) : n.snapGrid.length;
-            n.params.freeMode && n.params.freeMode.enabled && E > b && (E = b);
-            for (let k = 0; k < E; k += 1) z.renderBullet ? S += z.renderBullet.call(n, k, z.bulletClass) : S += `<${z.bulletElement} ${n.isElement?'part="bullet"':""} class="${z.bulletClass}"></${z.bulletElement}>`
+            let k = n.params.loop ? Math.ceil(b / n.params.slidesPerGroup) : n.snapGrid.length;
+            n.params.freeMode && n.params.freeMode.enabled && k > b && (k = b);
+            for (let E = 0; E < k; E += 1) z.renderBullet ? S += z.renderBullet.call(n, E, z.bulletClass) : S += `<${z.bulletElement} ${n.isElement?'part="bullet"':""} class="${z.bulletClass}"></${z.bulletElement}>`
         }
-        z.type === "fraction" && (z.renderFraction ? S = z.renderFraction.call(n, z.currentClass, z.totalClass) : S = `<span class="${z.currentClass}"></span> / <span class="${z.totalClass}"></span>`), z.type === "progressbar" && (z.renderProgressbar ? S = z.renderProgressbar.call(n, z.progressbarFillClass) : S = `<span class="${z.progressbarFillClass}"></span>`), n.pagination.bullets = [], h.forEach(E => {
-            z.type !== "custom" && (E.innerHTML = S || ""), z.type === "bullets" && n.pagination.bullets.push(...E.querySelectorAll(zr(z.bulletClass)))
+        z.type === "fraction" && (z.renderFraction ? S = z.renderFraction.call(n, z.currentClass, z.totalClass) : S = `<span class="${z.currentClass}"></span> / <span class="${z.totalClass}"></span>`), z.type === "progressbar" && (z.renderProgressbar ? S = z.renderProgressbar.call(n, z.progressbarFillClass) : S = `<span class="${z.progressbarFillClass}"></span>`), n.pagination.bullets = [], h.forEach(k => {
+            z.type !== "custom" && (k.innerHTML = S || ""), z.type === "bullets" && n.pagination.bullets.push(...k.querySelectorAll(zr(z.bulletClass)))
         }), z.type !== "custom" && o("paginationRender", h[0])
     }
 
     function _() {
         n.params.pagination = Sd(n, n.originalParams.pagination, n.params.pagination, {
             el: "swiper-pagination"
         });
@@ -37242,16 +38685,16 @@
     }), r("lock unlock", () => {
         m()
     }), r("click", (z, b) => {
         const h = b.target,
             S = Re(n.pagination.el);
         if (n.params.pagination.el && n.params.pagination.hideOnClick && S && S.length > 0 && !h.classList.contains(n.params.pagination.bulletClass)) {
             if (n.navigation && (n.navigation.nextEl && h === n.navigation.nextEl || n.navigation.prevEl && h === n.navigation.prevEl)) return;
-            const E = S[0].classList.contains(n.params.pagination.hiddenClass);
-            o(E === !0 ? "paginationShow" : "paginationHide"), S.forEach(k => k.classList.toggle(n.params.pagination.hiddenClass))
+            const k = S[0].classList.contains(n.params.pagination.hiddenClass);
+            o(k === !0 ? "paginationShow" : "paginationHide"), S.forEach(E => E.classList.toggle(n.params.pagination.hiddenClass))
         }
     });
     const g = () => {
             n.el.classList.remove(n.params.pagination.paginationDisabledClass);
             let {
                 el: z
             } = n.pagination;
@@ -37347,46 +38790,46 @@
             } else n.velocity = 0;
             n.velocity *= d.freeMode.momentumVelocityRatio, p.velocities.length = 0;
             let z = 1e3 * d.freeMode.momentumRatio;
             const b = n.velocity * z;
             let h = n.translate + b;
             f && (h = -h);
             let S = !1,
-                E;
-            const k = Math.abs(n.velocity) * 20 * d.freeMode.momentumBounceRatio;
-            let D;
-            if (h < n.maxTranslate()) d.freeMode.momentumBounce ? (h + n.maxTranslate() < -k && (h = n.maxTranslate() - k), E = n.maxTranslate(), S = !0, p.allowMomentumBounce = !0) : h = n.maxTranslate(), d.loop && d.centeredSlides && (D = !0);
-            else if (h > n.minTranslate()) d.freeMode.momentumBounce ? (h - n.minTranslate() > k && (h = n.minTranslate() + k), E = n.minTranslate(), S = !0, p.allowMomentumBounce = !0) : h = n.minTranslate(), d.loop && d.centeredSlides && (D = !0);
+                k;
+            const E = Math.abs(n.velocity) * 20 * d.freeMode.momentumBounceRatio;
+            let I;
+            if (h < n.maxTranslate()) d.freeMode.momentumBounce ? (h + n.maxTranslate() < -E && (h = n.maxTranslate() - E), k = n.maxTranslate(), S = !0, p.allowMomentumBounce = !0) : h = n.maxTranslate(), d.loop && d.centeredSlides && (I = !0);
+            else if (h > n.minTranslate()) d.freeMode.momentumBounce ? (h - n.minTranslate() > E && (h = n.minTranslate() + E), k = n.minTranslate(), S = !0, p.allowMomentumBounce = !0) : h = n.minTranslate(), d.loop && d.centeredSlides && (I = !0);
             else if (d.freeMode.sticky) {
                 let P;
                 for (let M = 0; M < _.length; M += 1)
                     if (_[M] > -h) {
                         P = M;
                         break
                     } Math.abs(_[P] - h) < Math.abs(_[P - 1] - h) || n.swipeDirection === "next" ? h = _[P] : h = _[P - 1], h = -h
             }
-            if (D && o("transitionEnd", () => {
+            if (I && o("transitionEnd", () => {
                     n.loopFix()
                 }), n.velocity !== 0) {
                 if (f ? z = Math.abs((-h - n.translate) / n.velocity) : z = Math.abs((h - n.translate) / n.velocity), d.freeMode.sticky) {
                     const P = Math.abs((f ? -h : h) - n.translate),
                         M = n.slidesSizesGrid[n.activeIndex];
                     P < M ? z = d.speed : P < 2 * M ? z = d.speed * 1.5 : z = d.speed * 2.5
                 }
             } else if (d.freeMode.sticky) {
                 n.slideToClosest();
                 return
             }
-            d.freeMode.momentumBounce && S ? (n.updateProgress(E), n.setTransition(z), n.setTranslate(h), n.transitionStart(!0, n.swipeDirection), n.animating = !0, Ii(m, () => {
+            d.freeMode.momentumBounce && S ? (n.updateProgress(k), n.setTransition(z), n.setTranslate(h), n.transitionStart(!0, n.swipeDirection), n.animating = !0, Di(m, () => {
                 !n || n.destroyed || !p.allowMomentumBounce || (r("momentumBounce"), n.setTransition(d.speed), setTimeout(() => {
-                    n.setTranslate(E), Ii(m, () => {
+                    n.setTranslate(k), Di(m, () => {
                         !n || n.destroyed || n.transitionEnd()
                     })
                 }, 0))
-            })) : n.velocity ? (r("_freeModeNoMomentumRelease"), n.updateProgress(h), n.setTransition(z), n.setTranslate(h), n.transitionStart(!0, n.swipeDirection), n.animating || (n.animating = !0, Ii(m, () => {
+            })) : n.velocity ? (r("_freeModeNoMomentumRelease"), n.updateProgress(h), n.setTransition(z), n.setTranslate(h), n.transitionStart(!0, n.swipeDirection), n.animating || (n.animating = !0, Di(m, () => {
                 !n || n.destroyed || n.transitionEnd()
             }))) : n.updateProgress(h), n.updateActiveIndex(), n.updateSlidesClasses()
         } else if (d.freeMode.sticky) {
             n.slideToClosest();
             return
         } else d.freeMode && r("_freeModeNoMomentumRelease");
         (!d.freeMode.momentum || y >= d.longSwipesMs) && (r("_freeModeStaticRelease"), n.updateProgress(), n.updateActiveIndex(), n.updateSlidesClasses())
@@ -37402,15 +38845,15 @@
 const v1 = {
     install(e) {
         si.use([g1, h1, b1]), e.component("Swiper", p1).component("SwiperSlide", z1)
     }
 };
 
 function y1(e) {
-    e.use(a0).use(al).use(cd).use(Uv).use(zg).use(v1)
+    e.use(ag).use(al).use(cd).use(Uv).use(z0).use(v1)
 }
 const wd = op(Gh);
 y1(wd);
 wd.mount("#app");
 export {
-    OT as $, bf as A, Rc as B, J1 as C, Da as D, R1 as E, Fe as F, I1 as G, H1 as H, N1 as I, le as J, nn as K, ot as L, na as M, S1 as N, fl as O, Np as P, p_ as Q, Ef as R, A1 as S, Hc as T, Rh as U, al as V, TT as W, MT as X, D1 as Y, La as Z, L1 as _, U1 as a, aT as a$, DT as a0, Bt as a1, Rp as a2, Zs as a3, ta as a4, ET as a5, a0 as a6, CT as a7, E1 as a8, k1 as a9, Hr as aA, Ge as aB, Yp as aC, q1 as aD, Fd as aE, Fa as aF, Ya as aG, Op as aH, wT as aI, xp as aJ, X1 as aK, Ch as aL, dT as aM, ls as aN, G1 as aO, as as aP, Gp as aQ, Bp as aR, F1 as aS, Z1 as aT, Zc as aU, Zp as aV, $1 as aW, fn as aX, nz as aY, oz as aZ, Y1 as a_, vT as aa, ST as ab, IT as ac, PT as ad, P1 as ae, C1 as af, Lp as ag, Lt as ah, Hp as ai, Se as aj, LT as ak, O1 as al, M1 as am, En as an, AT as ao, kT as ap, yT as aq, on as ar, He as as, im as at, Ot as au, Wn as av, Hf as aw, Bf as ax, Ti as ay, _T as az, Xo as b, rT as b0, K1 as b1, Xp as b2, dt as b3, iT as b4, qo as b5, Q1 as b6, Kp as b7, Iz as b8, tT as b9, Rn as ba, ce as bb, rc as bc, Ur as bd, uT as be, j1 as bf, rz as bg, eT as bh, Uu as bi, lT as bj, x1 as bk, sT as bl, tz as bm, nT as bn, je as bo, gz as bp, cT as bq, jn as br, kz as bs, hT as bt, ez as bu, jr as bv, V1 as bw, oT as bx, W1 as by, B1 as bz, ae as c, gT as d, bT as e, zT as f, Cz as g, Lz as h, Vp as i, Vf as j, mT as k, ve as l, pT as m, Nc as n, ur as o, ei as p, Vr as q, he as r, st as s, w1 as t, fT as u, Dt as v, Je as w, bn as x, Yo as y, el as z
+    OT as $, bf as A, Rc as B, J1 as C, Ia as D, R1 as E, Fe as F, D1 as G, H1 as H, N1 as I, le as J, nn as K, ot as L, na as M, S1 as N, fl as O, Np as P, p_ as Q, kf as R, A1 as S, Hc as T, Rh as U, al as V, TT as W, MT as X, I1 as Y, La as Z, L1 as _, U1 as a, aT as a$, IT as a0, Bt as a1, Rp as a2, Zs as a3, ta as a4, kT as a5, ag as a6, CT as a7, k1 as a8, E1 as a9, Hr as aA, Ge as aB, Yp as aC, q1 as aD, Fd as aE, Fa as aF, Ya as aG, Op as aH, wT as aI, xp as aJ, X1 as aK, Ch as aL, dT as aM, ls as aN, G1 as aO, as as aP, Gp as aQ, Bp as aR, F1 as aS, Z1 as aT, Zc as aU, Zp as aV, $1 as aW, fn as aX, nz as aY, oz as aZ, Y1 as a_, vT as aa, ST as ab, DT as ac, PT as ad, P1 as ae, C1 as af, Lp as ag, Lt as ah, Hp as ai, Se as aj, LT as ak, O1 as al, M1 as am, kn as an, AT as ao, ET as ap, yT as aq, on as ar, He as as, im as at, Ot as au, Wn as av, Hf as aw, Bf as ax, Ti as ay, _T as az, Xo as b, rT as b0, K1 as b1, Xp as b2, dt as b3, iT as b4, qo as b5, Q1 as b6, Kp as b7, Dz as b8, tT as b9, Rn as ba, ce as bb, rc as bc, Ur as bd, uT as be, j1 as bf, rz as bg, eT as bh, Uu as bi, lT as bj, x1 as bk, sT as bl, tz as bm, nT as bn, je as bo, gz as bp, cT as bq, jn as br, Ez as bs, hT as bt, ez as bu, jr as bv, V1 as bw, oT as bx, W1 as by, B1 as bz, ae as c, gT as d, bT as e, zT as f, Cz as g, Lz as h, Vp as i, Vf as j, mT as k, ve as l, pT as m, Nc as n, ur as o, ei as p, Vr as q, he as r, st as s, w1 as t, fT as u, It as v, Je as w, bn as x, Yo as y, el as z
 };
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/layout-bdc1c8bd.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/layout-42b7d22e.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     w as ee
-} from "./forwardRefs-70e877d2.js";
+} from "./forwardRefs-7be90dc2.js";
 import {
     p as U,
     as as E,
     at as te,
     au as Z,
     av as k,
     s as D,
@@ -13,15 +13,15 @@
     c as s,
     b as ae,
     r as se,
     ar as $,
     a as R,
     o as ue,
     ay as le
-} from "./index-6ff57e4c.js";
+} from "./index-b687f95a.js";
 const M = Symbol.for("vuetify:layout"),
     X = Symbol.for("vuetify:layout-item"),
     N = 1e3,
     de = U({
         overlaps: {
             type: Array,
             default: () => []
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/logo-9391b78c.svg` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/logo-9391b78c.svg`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/m4a-45331b05.png` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/m4a-45331b05.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/materialdesignicons-webfont-0b183104.eot` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-0b183104.eot`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/materialdesignicons-webfont-61e8aba5.ttf` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-61e8aba5.ttf`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/materialdesignicons-webfont-662fefa8.woff2` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-662fefa8.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/materialdesignicons-webfont-a5928a0d.woff` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-a5928a0d.woff`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/favicon.ico` & `music-assistant-frontend-2.4.3/music_assistant_frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/index.html` & `music-assistant-frontend-2.4.3/music_assistant_frontend/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     <link rel="mask-icon" href="favicon.svg" color="#FFFFFF">
     <link rel="manifest" href="manifest.webmanifest">
     <meta name="theme-color" media="(prefers-color-scheme: light)" content="#ffffff">
     <meta name="theme-color" media="(prefers-color-scheme: dark)"  content="#121212">
     <link rel="icon" href="favicon.ico" />
     <title>Music Assistant</title>
     <meta name="description" content="Music Assistant - Music library manager for Home Assistant">
-    <script type="module" crossorigin src="./assets/index-6ff57e4c.js"></script>
+    <script type="module" crossorigin src="./assets/index-b687f95a.js"></script>
     <link rel="stylesheet" href="./assets/index-52c10419.css">
   <link rel="manifest" href="./manifest.webmanifest"><style>@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}</style></head>
   <body>
     <noscript>
       <strong
         >We're sorry but musicassistant-frontend doesn't work properly without
         JavaScript enabled. Please enable it to continue.</strong
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/manifest.webmanifest` & `music-assistant-frontend-2.4.3/music_assistant_frontend/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/pwa-192x192.png` & `music-assistant-frontend-2.4.3/music_assistant_frontend/pwa-192x192.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/pwa-512x512.png` & `music-assistant-frontend-2.4.3/music_assistant_frontend/pwa-512x512.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/sw.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/sw.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -26,259 +26,259 @@
     }
 }
 define(["./workbox-27b29e6f"], (function(s) {
     "use strict";
     self.addEventListener("message", (s => {
         s.data && "SKIP_WAITING" === s.data.type && self.skipWaiting()
     })), s.precacheAndRoute([{
-        url: "assets/AddGroupPlayer-f291ae3b.js",
+        url: "assets/AddGroupPlayer-8a4f0893.js",
         revision: null
     }, {
-        url: "assets/AddProvider-b867b6d9.js",
+        url: "assets/AddProvider-f756ebc3.js",
         revision: null
     }, {
-        url: "assets/AlbumDetails-25e2fe83.js",
+        url: "assets/AlbumDetails-0b4de4f6.js",
         revision: null
     }, {
-        url: "assets/Alert-0c4ec871.js",
+        url: "assets/Alert-19e36349.js",
         revision: null
     }, {
         url: "assets/Alert-3971d760.css",
         revision: null
     }, {
-        url: "assets/ArtistDetails-159c8f35.js",
+        url: "assets/ArtistDetails-53ff83d9.js",
         revision: null
     }, {
-        url: "assets/BrowseView-15d25af1.js",
+        url: "assets/BrowseView-a95cb7cc.js",
         revision: null
     }, {
         url: "assets/Container-127b1d7c.css",
         revision: null
     }, {
-        url: "assets/Container-ba274a7a.js",
+        url: "assets/Container-dc894acd.js",
         revision: null
     }, {
-        url: "assets/contextmenu-c4231154.js",
+        url: "assets/contextmenu-521b5304.js",
         revision: null
     }, {
-        url: "assets/CoreConfigs-1f56aa74.js",
+        url: "assets/CoreConfigs-75569bfe.css",
         revision: null
     }, {
-        url: "assets/CoreConfigs-75569bfe.css",
+        url: "assets/CoreConfigs-f0329745.js",
         revision: null
     }, {
-        url: "assets/Default-abfbb155.css",
+        url: "assets/Default-2157b447.css",
         revision: null
     }, {
-        url: "assets/Default-bd92f6cd.js",
+        url: "assets/Default-c7088a94.js",
         revision: null
     }, {
         url: "assets/EditConfig-f2bca5b1.css",
         revision: null
     }, {
-        url: "assets/EditConfig.vue_vue_type_style_index_0_lang-658131e8.js",
+        url: "assets/EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js",
         revision: null
     }, {
-        url: "assets/EditCoreConfig-db86c453.js",
+        url: "assets/EditCoreConfig-d27a9b35.js",
         revision: null
     }, {
-        url: "assets/EditPlayer-293a9fdd.js",
+        url: "assets/EditPlayer-6e04043d.js",
         revision: null
     }, {
-        url: "assets/EditProvider-b281ecba.js",
+        url: "assets/EditProvider-e046ee5d.js",
         revision: null
     }, {
-        url: "assets/forwardRefs-70e877d2.js",
+        url: "assets/forwardRefs-7be90dc2.js",
         revision: null
     }, {
         url: "assets/forwardRefs-e5b3781d.css",
         revision: null
     }, {
-        url: "assets/HomeView-aa005854.js",
+        url: "assets/HomeView-8f9e6181.js",
         revision: null
     }, {
         url: "assets/HomeView-f9b96eef.css",
         revision: null
     }, {
         url: "assets/index-52c10419.css",
         revision: null
     }, {
-        url: "assets/index-6ff57e4c.js",
+        url: "assets/index-b687f95a.js",
         revision: null
     }, {
         url: "assets/index.browser-342e672c.js",
         revision: null
     }, {
         url: "assets/ItemsListing-5372ff4e.css",
         revision: null
     }, {
-        url: "assets/ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js",
+        url: "assets/ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js",
         revision: null
     }, {
-        url: "assets/layout-bdc1c8bd.js",
+        url: "assets/layout-42b7d22e.js",
         revision: null
     }, {
-        url: "assets/LibraryAlbums-532f0c88.js",
+        url: "assets/LibraryAlbums-7cfa0763.js",
         revision: null
     }, {
-        url: "assets/LibraryArtists-17fa3e93.js",
+        url: "assets/LibraryArtists-9924ed14.js",
         revision: null
     }, {
-        url: "assets/LibraryPlaylists-a41d818d.js",
+        url: "assets/LibraryPlaylists-95e35cdd.js",
         revision: null
     }, {
-        url: "assets/LibraryRadios-e4468a3f.js",
+        url: "assets/LibraryRadios-4a033696.js",
         revision: null
     }, {
-        url: "assets/LibraryTracks-a533acbe.js",
+        url: "assets/LibraryTracks-eeccb967.js",
         revision: null
     }, {
         url: "assets/ListviewItem-20f54197.css",
         revision: null
     }, {
-        url: "assets/ListviewItem-e896b2dc.js",
+        url: "assets/ListviewItem-8b992256.js",
         revision: null
     }, {
         url: "assets/PanelviewItem-cbf7c595.css",
         revision: null
     }, {
-        url: "assets/PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js",
+        url: "assets/PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js",
         revision: null
     }, {
-        url: "assets/PlayerQueue-42cde633.js",
+        url: "assets/PlayerQueue-9f89c917.js",
         revision: null
     }, {
-        url: "assets/Players-0c4ce7a2.js",
+        url: "assets/Players-0e31a251.js",
         revision: null
     }, {
-        url: "assets/PlaylistDetails-9db516b0.js",
+        url: "assets/PlaylistDetails-2fe134b1.js",
         revision: null
     }, {
         url: "assets/ProviderDetails-2713c080.css",
         revision: null
     }, {
-        url: "assets/ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js",
+        url: "assets/ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js",
         revision: null
     }, {
-        url: "assets/Providers-ca2eea9e.js",
+        url: "assets/Providers-58a591e0.js",
         revision: null
     }, {
         url: "assets/Providers-e2f60749.css",
         revision: null
     }, {
-        url: "assets/RadioDetails-87373ab9.js",
+        url: "assets/RadioDetails-54e9e340.js",
         revision: null
     }, {
-        url: "assets/Search-abd54e1f.js",
+        url: "assets/Search-00ee9dd8.js",
         revision: null
     }, {
-        url: "assets/Settings-170b9c4c.js",
+        url: "assets/Settings-bbdb2168.js",
         revision: null
     }, {
-        url: "assets/TrackDetails-6c6c6bec.js",
+        url: "assets/TrackDetails-72029d5e.js",
         revision: null
     }, {
         url: "assets/VAlert-1c823677.css",
         revision: null
     }, {
-        url: "assets/VAlert-f74a2b4b.js",
+        url: "assets/VAlert-56af8987.js",
         revision: null
     }, {
-        url: "assets/VBadge-76d9c3a5.js",
+        url: "assets/VBadge-84e3406b.js",
         revision: null
     }, {
-        url: "assets/VBadge-bc81f416.css",
+        url: "assets/VBadge-8b8b8a6d.css",
         revision: null
     }, {
         url: "assets/VCard-257d0eab.css",
         revision: null
     }, {
-        url: "assets/VCard-bfc4071a.js",
+        url: "assets/VCard-b98fe47e.js",
         revision: null
     }, {
-        url: "assets/VCardText-00c669eb.js",
+        url: "assets/VCardText-6774ea5e.js",
         revision: null
     }, {
         url: "assets/VDialog-5309eac2.css",
         revision: null
     }, {
-        url: "assets/VDialog-82ed2e80.js",
+        url: "assets/VDialog-d7e50927.js",
         revision: null
     }, {
         url: "assets/VExpansionPanel-00a7e4f4.css",
         revision: null
     }, {
-        url: "assets/VExpansionPanel-9f82eed8.js",
+        url: "assets/VExpansionPanel-58c5fe02.js",
         revision: null
     }, {
-        url: "assets/VForm-a7262390.js",
+        url: "assets/VForm-fc99b4aa.js",
         revision: null
     }, {
         url: "assets/VGrid-37b0738d.css",
         revision: null
     }, {
-        url: "assets/VInput-91b2e758.js",
+        url: "assets/VInput-5b197ccd.js",
         revision: null
     }, {
         url: "assets/VInput-b16e222c.css",
         revision: null
     }, {
-        url: "assets/VMenu-9506155f.js",
+        url: "assets/VMenu-a46f5e7a.css",
         revision: null
     }, {
-        url: "assets/VMenu-a46f5e7a.css",
+        url: "assets/VMenu-b634019c.js",
         revision: null
     }, {
         url: "assets/VSelect-7df244e0.css",
         revision: null
     }, {
-        url: "assets/VSelect-ea96d901.js",
+        url: "assets/VSelect-d10e917f.js",
         revision: null
     }, {
-        url: "assets/VSlideGroup-5dd0c6f2.js",
+        url: "assets/VSlideGroup-b576aa37.js",
         revision: null
     }, {
         url: "assets/VSlideGroup-c5ba1538.css",
         revision: null
     }, {
         url: "assets/VTabs-11e16be1.css",
         revision: null
     }, {
-        url: "assets/VTabs-4c128c89.js",
+        url: "assets/VTabs-8ad24bfd.js",
         revision: null
     }, {
-        url: "assets/VTextField-8883f272.js",
+        url: "assets/VTextField-0c2ec62d.js",
         revision: null
     }, {
         url: "assets/VTextField-d31117f3.css",
         revision: null
     }, {
-        url: "assets/VToolbar-4ad3b045.js",
+        url: "assets/VToolbar-78a5e824.css",
         revision: null
     }, {
-        url: "assets/VToolbar-78a5e824.css",
+        url: "assets/VToolbar-b7f10b15.js",
         revision: null
     }, {
         url: "assets/VTooltip-3a8fb95f.css",
         revision: null
     }, {
-        url: "assets/VTooltip-a8719c72.js",
+        url: "assets/VTooltip-3ef94159.js",
         revision: null
     }, {
         url: "assets/VVirtualScroll-29c92c23.css",
         revision: null
     }, {
-        url: "assets/VVirtualScroll-5f35af5d.js",
+        url: "assets/VVirtualScroll-84259ceb.js",
         revision: null
     }, {
         url: "assets/workbox-window.prod.es5-a7b12eab.js",
         revision: null
     }, {
         url: "index.html",
-        revision: "5a54d06173e7073b887c571bd710bb6d"
+        revision: "9316d7db7067601d034630c21a631d4d"
     }, {
         url: "favicon.ico",
         revision: "60d77c1713c2255be3f6de69c4de24d9"
     }, {
         url: "robots.txt",
         revision: "5e0bd1c281a62a380d7a948085bfe2d1"
     }, {
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend/workbox-27b29e6f.js` & `music-assistant-frontend-2.4.3/music_assistant_frontend/workbox-27b29e6f.js`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend.egg-info/PKG-INFO` & `music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-assistant-frontend
-Version: 2.4.2
+Version: 2.4.3
 Summary: The Music Assistant frontend
 Author-email: The Music Assistant Authors <m.vanderveldt@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/music-assistant/frontend
 Platform: any
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `music-assistant-frontend-2.4.2/music_assistant_frontend.egg-info/SOURCES.txt` & `music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 music_assistant_frontend/sw.js
 music_assistant_frontend/workbox-27b29e6f.js
 music_assistant_frontend.egg-info/PKG-INFO
 music_assistant_frontend.egg-info/SOURCES.txt
 music_assistant_frontend.egg-info/dependency_links.txt
 music_assistant_frontend.egg-info/not-zip-safe
 music_assistant_frontend.egg-info/top_level.txt
-music_assistant_frontend/assets/AddGroupPlayer-f291ae3b.js
-music_assistant_frontend/assets/AddProvider-b867b6d9.js
-music_assistant_frontend/assets/AlbumDetails-25e2fe83.js
-music_assistant_frontend/assets/Alert-0c4ec871.js
+music_assistant_frontend/assets/AddGroupPlayer-8a4f0893.js
+music_assistant_frontend/assets/AddProvider-f756ebc3.js
+music_assistant_frontend/assets/AlbumDetails-0b4de4f6.js
+music_assistant_frontend/assets/Alert-19e36349.js
 music_assistant_frontend/assets/Alert-3971d760.css
-music_assistant_frontend/assets/ArtistDetails-159c8f35.js
-music_assistant_frontend/assets/BrowseView-15d25af1.js
+music_assistant_frontend/assets/ArtistDetails-53ff83d9.js
+music_assistant_frontend/assets/BrowseView-a95cb7cc.js
 music_assistant_frontend/assets/Container-127b1d7c.css
-music_assistant_frontend/assets/Container-ba274a7a.js
-music_assistant_frontend/assets/CoreConfigs-1f56aa74.js
+music_assistant_frontend/assets/Container-dc894acd.js
 music_assistant_frontend/assets/CoreConfigs-75569bfe.css
-music_assistant_frontend/assets/Default-abfbb155.css
-music_assistant_frontend/assets/Default-bd92f6cd.js
+music_assistant_frontend/assets/CoreConfigs-f0329745.js
+music_assistant_frontend/assets/Default-2157b447.css
+music_assistant_frontend/assets/Default-c7088a94.js
 music_assistant_frontend/assets/EditConfig-f2bca5b1.css
-music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-658131e8.js
-music_assistant_frontend/assets/EditCoreConfig-db86c453.js
-music_assistant_frontend/assets/EditPlayer-293a9fdd.js
-music_assistant_frontend/assets/EditProvider-b281ecba.js
-music_assistant_frontend/assets/HomeView-aa005854.js
+music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js
+music_assistant_frontend/assets/EditCoreConfig-d27a9b35.js
+music_assistant_frontend/assets/EditPlayer-6e04043d.js
+music_assistant_frontend/assets/EditProvider-e046ee5d.js
+music_assistant_frontend/assets/HomeView-8f9e6181.js
 music_assistant_frontend/assets/HomeView-f9b96eef.css
 music_assistant_frontend/assets/ItemsListing-5372ff4e.css
-music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-a2bccead.js
+music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js
 music_assistant_frontend/assets/JetBrainsMono-Medium-086c48df.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
@@ -80,82 +80,82 @@
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
-music_assistant_frontend/assets/LibraryAlbums-532f0c88.js
-music_assistant_frontend/assets/LibraryArtists-17fa3e93.js
-music_assistant_frontend/assets/LibraryPlaylists-a41d818d.js
-music_assistant_frontend/assets/LibraryRadios-e4468a3f.js
-music_assistant_frontend/assets/LibraryTracks-a533acbe.js
+music_assistant_frontend/assets/LibraryAlbums-7cfa0763.js
+music_assistant_frontend/assets/LibraryArtists-9924ed14.js
+music_assistant_frontend/assets/LibraryPlaylists-95e35cdd.js
+music_assistant_frontend/assets/LibraryRadios-4a033696.js
+music_assistant_frontend/assets/LibraryTracks-eeccb967.js
 music_assistant_frontend/assets/ListviewItem-20f54197.css
-music_assistant_frontend/assets/ListviewItem-e896b2dc.js
+music_assistant_frontend/assets/ListviewItem-8b992256.js
 music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
 music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
 music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
 music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
 music_assistant_frontend/assets/PanelviewItem-cbf7c595.css
-music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-7a8dba32.js
-music_assistant_frontend/assets/PlayerQueue-42cde633.js
-music_assistant_frontend/assets/Players-0c4ce7a2.js
-music_assistant_frontend/assets/PlaylistDetails-9db516b0.js
+music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js
+music_assistant_frontend/assets/PlayerQueue-9f89c917.js
+music_assistant_frontend/assets/Players-0e31a251.js
+music_assistant_frontend/assets/PlaylistDetails-2fe134b1.js
 music_assistant_frontend/assets/ProviderDetails-2713c080.css
-music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-37eb5b13.js
-music_assistant_frontend/assets/Providers-ca2eea9e.js
+music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js
+music_assistant_frontend/assets/Providers-58a591e0.js
 music_assistant_frontend/assets/Providers-e2f60749.css
-music_assistant_frontend/assets/RadioDetails-87373ab9.js
-music_assistant_frontend/assets/Search-abd54e1f.js
-music_assistant_frontend/assets/Settings-170b9c4c.js
-music_assistant_frontend/assets/TrackDetails-6c6c6bec.js
+music_assistant_frontend/assets/RadioDetails-54e9e340.js
+music_assistant_frontend/assets/Search-00ee9dd8.js
+music_assistant_frontend/assets/Settings-bbdb2168.js
+music_assistant_frontend/assets/TrackDetails-72029d5e.js
 music_assistant_frontend/assets/VAlert-1c823677.css
-music_assistant_frontend/assets/VAlert-f74a2b4b.js
-music_assistant_frontend/assets/VBadge-76d9c3a5.js
-music_assistant_frontend/assets/VBadge-bc81f416.css
+music_assistant_frontend/assets/VAlert-56af8987.js
+music_assistant_frontend/assets/VBadge-84e3406b.js
+music_assistant_frontend/assets/VBadge-8b8b8a6d.css
 music_assistant_frontend/assets/VCard-257d0eab.css
-music_assistant_frontend/assets/VCard-bfc4071a.js
-music_assistant_frontend/assets/VCardText-00c669eb.js
+music_assistant_frontend/assets/VCard-b98fe47e.js
+music_assistant_frontend/assets/VCardText-6774ea5e.js
 music_assistant_frontend/assets/VDialog-5309eac2.css
-music_assistant_frontend/assets/VDialog-82ed2e80.js
+music_assistant_frontend/assets/VDialog-d7e50927.js
 music_assistant_frontend/assets/VExpansionPanel-00a7e4f4.css
-music_assistant_frontend/assets/VExpansionPanel-9f82eed8.js
-music_assistant_frontend/assets/VForm-a7262390.js
+music_assistant_frontend/assets/VExpansionPanel-58c5fe02.js
+music_assistant_frontend/assets/VForm-fc99b4aa.js
 music_assistant_frontend/assets/VGrid-37b0738d.css
-music_assistant_frontend/assets/VInput-91b2e758.js
+music_assistant_frontend/assets/VInput-5b197ccd.js
 music_assistant_frontend/assets/VInput-b16e222c.css
-music_assistant_frontend/assets/VMenu-9506155f.js
 music_assistant_frontend/assets/VMenu-a46f5e7a.css
+music_assistant_frontend/assets/VMenu-b634019c.js
 music_assistant_frontend/assets/VSelect-7df244e0.css
-music_assistant_frontend/assets/VSelect-ea96d901.js
-music_assistant_frontend/assets/VSlideGroup-5dd0c6f2.js
+music_assistant_frontend/assets/VSelect-d10e917f.js
+music_assistant_frontend/assets/VSlideGroup-b576aa37.js
 music_assistant_frontend/assets/VSlideGroup-c5ba1538.css
 music_assistant_frontend/assets/VTabs-11e16be1.css
-music_assistant_frontend/assets/VTabs-4c128c89.js
-music_assistant_frontend/assets/VTextField-8883f272.js
+music_assistant_frontend/assets/VTabs-8ad24bfd.js
+music_assistant_frontend/assets/VTextField-0c2ec62d.js
 music_assistant_frontend/assets/VTextField-d31117f3.css
-music_assistant_frontend/assets/VToolbar-4ad3b045.js
 music_assistant_frontend/assets/VToolbar-78a5e824.css
+music_assistant_frontend/assets/VToolbar-b7f10b15.js
 music_assistant_frontend/assets/VTooltip-3a8fb95f.css
-music_assistant_frontend/assets/VTooltip-a8719c72.js
+music_assistant_frontend/assets/VTooltip-3ef94159.js
 music_assistant_frontend/assets/VVirtualScroll-29c92c23.css
-music_assistant_frontend/assets/VVirtualScroll-5f35af5d.js
-music_assistant_frontend/assets/contextmenu-c4231154.js
+music_assistant_frontend/assets/VVirtualScroll-84259ceb.js
+music_assistant_frontend/assets/contextmenu-521b5304.js
 music_assistant_frontend/assets/cover_dark-75402cd0.png
 music_assistant_frontend/assets/cover_light-b832ae9e.png
 music_assistant_frontend/assets/fallback-d0ff2800.png
 music_assistant_frontend/assets/folder-6b5595ac.svg
-music_assistant_frontend/assets/forwardRefs-70e877d2.js
+music_assistant_frontend/assets/forwardRefs-7be90dc2.js
 music_assistant_frontend/assets/forwardRefs-e5b3781d.css
 music_assistant_frontend/assets/hires-438c7046.png
 music_assistant_frontend/assets/index-52c10419.css
-music_assistant_frontend/assets/index-6ff57e4c.js
+music_assistant_frontend/assets/index-b687f95a.js
 music_assistant_frontend/assets/index.browser-342e672c.js
 music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
-music_assistant_frontend/assets/layout-bdc1c8bd.js
+music_assistant_frontend/assets/layout-42b7d22e.js
 music_assistant_frontend/assets/logo-9391b78c.svg
 music_assistant_frontend/assets/m4a-45331b05.png
 music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
 music_assistant_frontend/assets/materialdesignicons-webfont-0b183104.eot
 music_assistant_frontend/assets/materialdesignicons-webfont-61e8aba5.ttf
 music_assistant_frontend/assets/materialdesignicons-webfont-662fefa8.woff2
 music_assistant_frontend/assets/materialdesignicons-webfont-a5928a0d.woff
```

### Comparing `music-assistant-frontend-2.4.2/pyproject.toml` & `music-assistant-frontend-2.4.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools~=62.3",
     "wheel~=0.37.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "music-assistant-frontend"
-version = "2.4.2"
+version = "2.4.3"
 description = "The Music Assistant frontend"
 readme = "README.md"
 authors = [
     { name = "The Music Assistant Authors", email = "m.vanderveldt@outlook.com" },
 ]
 requires-python = ">=3.9.0"
```

