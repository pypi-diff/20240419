# Comparing `tmp/chainzpy-0.4.tar.gz` & `tmp/chainzpy-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainzpy-0.4.tar", last modified: Tue Apr 16 20:27:19 2024, max compression
+gzip compressed data, was "chainzpy-0.5.tar", last modified: Fri Apr 19 17:02:20 2024, max compression
```

## Comparing `chainzpy-0.4.tar` & `chainzpy-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-16 20:27:19.024042 chainzpy-0.4/
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-16 20:27:19.019750 chainzpy-0.4/Chainzpy/
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      328 2024-04-14 17:14:47.000000 chainzpy-0.4/Chainzpy/__init__.py
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)     3440 2024-04-14 17:15:15.000000 chainzpy-0.4/Chainzpy/main.py
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-16 20:27:19.023168 chainzpy-0.4/Chainzpy.egg-info/
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      251 2024-04-16 20:27:18.000000 chainzpy-0.4/Chainzpy.egg-info/PKG-INFO
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      412 2024-04-16 20:27:18.000000 chainzpy-0.4/Chainzpy.egg-info/SOURCES.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        1 2024-04-16 20:27:18.000000 chainzpy-0.4/Chainzpy.egg-info/dependency_links.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       13 2024-04-16 20:27:18.000000 chainzpy-0.4/Chainzpy.egg-info/requires.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        9 2024-04-16 20:27:18.000000 chainzpy-0.4/Chainzpy.egg-info/top_level.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      251 2024-04-16 20:27:19.023511 chainzpy-0.4/PKG-INFO
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:29:26.000000 chainzpy-0.4/README.md
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       38 2024-04-16 20:27:19.024146 chainzpy-0.4/setup.cfg
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      377 2024-04-16 20:27:16.000000 chainzpy-0.4/setup.py
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-19 17:02:20.760903 chainzpy-0.5/
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-19 17:02:20.758406 chainzpy-0.5/Chainzpy/
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      328 2024-04-14 17:14:47.000000 chainzpy-0.5/Chainzpy/__init__.py
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)     3369 2024-04-19 17:01:39.000000 chainzpy-0.5/Chainzpy/main.py
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-19 17:02:20.760116 chainzpy-0.5/Chainzpy.egg-info/
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      334 2024-04-19 17:02:20.000000 chainzpy-0.5/Chainzpy.egg-info/PKG-INFO
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      412 2024-04-19 17:02:20.000000 chainzpy-0.5/Chainzpy.egg-info/SOURCES.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        1 2024-04-19 17:02:20.000000 chainzpy-0.5/Chainzpy.egg-info/dependency_links.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       13 2024-04-19 17:02:20.000000 chainzpy-0.5/Chainzpy.egg-info/requires.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        9 2024-04-19 17:02:20.000000 chainzpy-0.5/Chainzpy.egg-info/top_level.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      334 2024-04-19 17:02:20.760455 chainzpy-0.5/PKG-INFO
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:29:26.000000 chainzpy-0.5/README.md
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       38 2024-04-19 17:02:20.760971 chainzpy-0.5/setup.cfg
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      462 2024-04-19 17:00:49.000000 chainzpy-0.5/setup.py
```

### Comparing `chainzpy-0.4/Chainzpy/main.py` & `chainzpy-0.5/Chainzpy/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,23 +28,20 @@
     soup = BeautifulSoup(r.text, 'html.parser')
     price_find = soup.find(class_='sc-f70bb44c-0 jxpCgO base-text')
     str_price = str(price_find)
     stripedPrice = str_price.strip('<span class="sc-f70bb44c-0 jxpCgO base-text">')
     striped2Price = stripedPrice.strip('</')
     final_price = striped2Price.replace(",", "").replace("$", "")
     float_price = float(final_price)
-    print(final_price)
-    print(float_price)
 
     
 
     r1 = requests.get(f'https://chainz.cryptoid.info/{cryptoabbr}/api.dws?q=getbalance&a={address}&key{KEY}')
     data = r1.text
     crypto_bal = float(data)
-    print(crypto_bal)
     crypto_to_usd = float_price * crypto_bal
     crypto_in_usd = "${:,.2f}".format(crypto_to_usd)
     print(crypto_in_usd) # prints the amount of money in a users wallet in USD
 
 # getAddressBalanceUSD('litecoin', 'ltc', 'M8T1B2Z97gVdvmfkQcAtYbEepune1tzGua')
     
 
@@ -54,16 +51,15 @@
     data = r.json()
     if DATA_TO_JSON == True:
         print(data)
     elif DATA_TO_JSON == False:
         print(f'Balance: {data['balance']} | Transaction Count: {data['transactionCount']} | First Block: {data['firstBlock']} | Last Block: {data['lastBlock']}')
     
     
-
-# getAddressInfo('ltc', 'M8T1B2Z97gVdvmfkQcAtYbEepune1tzGua')
+getAddressInfo('ltc', 'M8T1B2Z97gVdvmfkQcAtYbEepune1tzGua')
     
 
 def getRichestRank(cryptoabbr, address):
     global KEY
     r = requests.get(f'https://chainz.cryptoid.info/{cryptoabbr}/api.dws?q=richrank&a={address}&key={KEY}')
     print(r.text) # Prints the rank of the users address in terms of amount of crypto being held inside
```

