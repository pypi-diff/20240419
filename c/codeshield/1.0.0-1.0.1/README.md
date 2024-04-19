# Comparing `tmp/codeshield-1.0.0.tar.gz` & `tmp/codeshield-1.0.1.tar.gz`

## Comparing `codeshield-1.0.0.tar` & `codeshield-1.0.1.tar`

### file list

```diff
@@ -1,183 +1,180 @@
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 codeshield-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 codeshield-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 codeshield-1.0.0/__init__.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 codeshield-1.0.0/codeshield.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 codeshield-1.0.0/example.py
--rw-r--r--   0        0        0    67794 2020-02-02 00:00:00.000000 codeshield-1.0.0/images/codeshield_logo.png
--rw-r--r--   0        0        0   135320 2020-02-02 00:00:00.000000 codeshield-1.0.0/images/design.png
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/README.md
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/analyzers.py
--rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/insecure_code_detector.py
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/insecure_patterns.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/issues.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/languages.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/oss.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/usecases.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/README.md
--rw-r--r--   0        0        0    11429 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/config.yaml
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/c.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/cpp.yaml
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/csharp.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/hack.yaml
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/java.yaml
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/javascript.yaml
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/language_agnostic.yaml
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/objective_c.yaml
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/php.yaml
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/python.yaml
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/ruby.yaml
--rw-r--r--   0        0        0     8391 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/rules.rs
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/rust.yaml
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/swift.yaml
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/regex/xml.yaml
--rw-r--r--   0        0        0    12953 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/c_codeshield.json
--rw-r--r--   0        0        0    15624 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/c_cyberseceval.json
--rw-r--r--   0        0        0    12953 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/cpp_codeshield.json
--rw-r--r--   0        0        0    15624 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/cpp_cyberseceval.json
--rw-r--r--   0        0        0    36852 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/csharp_codeshield.json
--rw-r--r--   0        0        0    36852 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/csharp_cyberseceval.json
--rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/java_codeshield.json
--rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/java_cyberseceval.json
--rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/javascript_codeshield.json
--rw-r--r--   0        0        0    43879 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/javascript_cyberseceval.json
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/php_codeshield.json
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/php_cyberseceval.json
--rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/python_codeshield.json
--rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/python_cyberseceval.json
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/bad-crypto-api-usage.c
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/blowfish_encryption_use.yaml
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/bugprone-snprintf.c
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/bugprone-snprintf.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/crypto-weak-prng.c
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/crypto-weak-prng.yaml
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/crypto_des_algorithm_use.yaml
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/crypto_ecb_mode_encryption_use.yaml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/crypto_rsa_key_size_insufficient.yaml
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/crypto_unauthenticated_encryption_usage.yaml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/fixed_nonce_use.yaml
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/fixed_seed_use.c
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/fixed_seed_use.yaml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/hardcoded_key_use.yaml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/integer-overflow-to-buffer-overflow.c
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/integer-overflow-to-buffer-overflow.yaml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/invalid-free.c
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/invalid-free.yaml
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/mcf-get-c-string-result-ignored.c
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/mcf-get-c-string-result-ignored.yaml
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/md2_or_md4_hash_use.yaml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/md5_use.yaml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/potential-command-injection.c
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/potential-command-injection.yaml
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/sha1_use.yaml
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/vulnerable-sprintf.yaml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/vulnerable-strcpy.yaml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/write-to-stack-buffer.c
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/write-to-stack-buffer.yaml
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/command_injection.yaml
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/cookie_without_http_only_flag.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/cookie_without_ssl_flag.yaml
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_certification_validation_disabled.yaml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_cipher_algorithm.yaml
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_cipher_mode.yaml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_hashing_function.yaml
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_prng.yaml
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/csrf.yaml
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/input_validation.yaml
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/insecure_deserialization.yaml
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/ldap_injection.yaml
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/path_traversal.yaml
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/sql_injection.yaml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/unsafe_xslt_setting.yaml
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/unvalidated_redirect.yaml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/weak-password-requirements.yaml
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/xpath_injection.yaml
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/xss.yaml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/xxe.yaml
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/deserialization_insecure.yaml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/cors_header_injection.yaml
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/csrf_disabled.yaml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/ldap_anonymous.yaml
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/random_number_generator.yaml
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/ssrf.yaml
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xpath_injection.yaml
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xss_send_error_response.yaml
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xss_servlet_response.yaml
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xxe_sax_parser.yaml
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xxe_xml_input_factory.yaml
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xxe_xml_reader.yaml
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/child-process.js
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/child-process.yaml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/post-message-origin.yaml
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/unchecked-origin-onmessage.js
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/unchecked-origin-onmessage.yaml
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/unencrypted-fetch.js
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/unencrypted-fetch.yaml
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/unsafe-alloc.yaml
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/buffer-noassert.yaml
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/dangerously-set-inner-html.yaml
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/detect-new-buffer.yaml
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/eval-usage.js
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/eval-usage.yaml
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/mustache-escape.yaml
--rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-fs-filename.yaml
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-regexp.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-require.yaml
--rw-r--r--   0        0        0    11092 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/possible-timing-attacks.yaml
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/pseudo-random-bytes.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/backticks_use.php
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/backticks_use.yaml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/eval_use.php
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/eval_use.yaml
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/mcrypt_use.php
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/mcrypt_use.yaml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/phpinfo_use.php
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/phpinfo_use.yaml
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/tainted_exec.php
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/tainted_exec.yaml
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/unsafe_extract.php
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/unsafe_extract.yaml
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/unsafe_hash.php
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/unsafe_hash.yaml
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/crypto_fixed_nonce.yaml
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/crypto_fixed_prng_seed.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/crypto_prng_random.yaml
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/deserialization_dill_use.yaml
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/deserialization_json_pickle_use.yaml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/deserialization_pickle_use.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/deserialization_pickle_use.yaml
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/deserialization_yaml_use.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/eval_use.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/eval_use.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/exec_use.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/exec_use.yaml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/hardcoded_secrets.yaml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/os_popen_use.yaml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/os_system_use.yaml
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/sql_injection_cursor_execute.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/sql_injection_cursor_execute.yaml
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/subprocess_using_shell.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/subprocess_using_shell.yaml
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/rules/semgrep/rule_gen/gen_consolidated_rules.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/__init__.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/insecure_code_detector_test.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_c_insecure_code_detector.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_cpp_insecure_code_detector.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_csharp_insecure_code_detector.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_functional.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_java_insecure_code_detector.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_javascript_insecure_code_detector.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_kotlin_insecure_code_detector.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_objective_c_code_detector.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_php_insecure_code_detector.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_python_insecure_code_detector.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_ruby_insecure_code_detector.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_rust_insecure_code_detector.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_swift_code_detector.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 codeshield-1.0.0/insecure_code_detector/tests/test_xml_insecure_code_detector.py
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 codeshield-1.0.0/notebook/CodeShieldUsageDemo.ipynb
--rw-r--r--   0        0        0     7873 2020-02-02 00:00:00.000000 codeshield-1.0.0/notebook/.ipynb_checkpoints/CodeShieldUsageDemo-checkpoint.ipynb
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 codeshield-1.0.0/tests/test_codeshield.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 codeshield-1.0.0/LICENSE
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 codeshield-1.0.0/README.md
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 codeshield-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 codeshield-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 codeshield-1.0.1/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 codeshield-1.0.1/codeshield.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 codeshield-1.0.1/example.py
+-rw-r--r--   0        0        0    67794 2020-02-02 00:00:00.000000 codeshield-1.0.1/images/codeshield_logo.png
+-rw-r--r--   0        0        0   135320 2020-02-02 00:00:00.000000 codeshield-1.0.1/images/design.png
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/README.md
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/analyzers.py
+-rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/insecure_code_detector.py
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/insecure_patterns.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/issues.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/languages.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/oss.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/usecases.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/README.md
+-rw-r--r--   0        0        0    11429 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/config.yaml
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/c.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/cpp.yaml
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/csharp.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/hack.yaml
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/java.yaml
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/javascript.yaml
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/language_agnostic.yaml
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/objective_c.yaml
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/php.yaml
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/python.yaml
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/ruby.yaml
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/rust.yaml
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/swift.yaml
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/regex/xml.yaml
+-rw-r--r--   0        0        0    12953 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/c_codeshield.json
+-rw-r--r--   0        0        0    15624 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/c_cyberseceval.json
+-rw-r--r--   0        0        0    12953 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/cpp_codeshield.json
+-rw-r--r--   0        0        0    15624 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/cpp_cyberseceval.json
+-rw-r--r--   0        0        0    36852 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/csharp_codeshield.json
+-rw-r--r--   0        0        0    36852 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/csharp_cyberseceval.json
+-rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/java_codeshield.json
+-rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/java_cyberseceval.json
+-rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/javascript_codeshield.json
+-rw-r--r--   0        0        0    43879 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/javascript_cyberseceval.json
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/php_codeshield.json
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/php_cyberseceval.json
+-rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/python_codeshield.json
+-rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/python_cyberseceval.json
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/bad-crypto-api-usage.c
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/blowfish_encryption_use.yaml
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/bugprone-snprintf.c
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/bugprone-snprintf.yaml
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/crypto-weak-prng.c
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/crypto-weak-prng.yaml
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/crypto_des_algorithm_use.yaml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/crypto_ecb_mode_encryption_use.yaml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/crypto_rsa_key_size_insufficient.yaml
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/crypto_unauthenticated_encryption_usage.yaml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/fixed_nonce_use.yaml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/fixed_seed_use.c
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/fixed_seed_use.yaml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/hardcoded_key_use.yaml
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/integer-overflow-to-buffer-overflow.c
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/integer-overflow-to-buffer-overflow.yaml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/invalid-free.c
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/invalid-free.yaml
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/mcf-get-c-string-result-ignored.c
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/mcf-get-c-string-result-ignored.yaml
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/md2_or_md4_hash_use.yaml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/md5_use.yaml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/potential-command-injection.c
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/potential-command-injection.yaml
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/sha1_use.yaml
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/vulnerable-sprintf.yaml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/vulnerable-strcpy.yaml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/write-to-stack-buffer.c
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/write-to-stack-buffer.yaml
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/command_injection.yaml
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/cookie_without_http_only_flag.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/cookie_without_ssl_flag.yaml
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_certification_validation_disabled.yaml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_cipher_algorithm.yaml
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_cipher_mode.yaml
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_hashing_function.yaml
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_prng.yaml
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/csrf.yaml
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/input_validation.yaml
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/insecure_deserialization.yaml
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/ldap_injection.yaml
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/path_traversal.yaml
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/sql_injection.yaml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/unsafe_xslt_setting.yaml
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/unvalidated_redirect.yaml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/weak-password-requirements.yaml
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/xpath_injection.yaml
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/xss.yaml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/xxe.yaml
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/deserialization_insecure.yaml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/cors_header_injection.yaml
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/csrf_disabled.yaml
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/ldap_anonymous.yaml
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/random_number_generator.yaml
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/ssrf.yaml
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xpath_injection.yaml
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xss_send_error_response.yaml
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xss_servlet_response.yaml
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xxe_sax_parser.yaml
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xxe_xml_input_factory.yaml
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xxe_xml_reader.yaml
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/child-process.js
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/child-process.yaml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/post-message-origin.yaml
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/unchecked-origin-onmessage.js
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/unchecked-origin-onmessage.yaml
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/unencrypted-fetch.js
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/unencrypted-fetch.yaml
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/unsafe-alloc.yaml
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/buffer-noassert.yaml
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/dangerously-set-inner-html.yaml
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/detect-new-buffer.yaml
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/eval-usage.js
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/eval-usage.yaml
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/mustache-escape.yaml
+-rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-fs-filename.yaml
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-regexp.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-require.yaml
+-rw-r--r--   0        0        0    11092 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/possible-timing-attacks.yaml
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/pseudo-random-bytes.yaml
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/backticks_use.php
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/backticks_use.yaml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/eval_use.php
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/eval_use.yaml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/mcrypt_use.php
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/mcrypt_use.yaml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/phpinfo_use.php
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/phpinfo_use.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/tainted_exec.php
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/tainted_exec.yaml
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/unsafe_extract.php
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/unsafe_extract.yaml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/unsafe_hash.php
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/unsafe_hash.yaml
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/crypto_fixed_nonce.yaml
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/crypto_fixed_prng_seed.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/crypto_prng_random.yaml
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/deserialization_dill_use.yaml
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/deserialization_json_pickle_use.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/deserialization_pickle_use.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/deserialization_pickle_use.yaml
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/deserialization_yaml_use.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/eval_use.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/eval_use.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/exec_use.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/exec_use.yaml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/hardcoded_secrets.yaml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/os_popen_use.yaml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/os_system_use.yaml
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/sql_injection_cursor_execute.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/sql_injection_cursor_execute.yaml
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/subprocess_using_shell.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/subprocess_using_shell.yaml
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/rules/semgrep/rule_gen/gen_consolidated_rules.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/__init__.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/insecure_code_detector_test.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_c_insecure_code_detector.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_cpp_insecure_code_detector.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_csharp_insecure_code_detector.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_functional.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_java_insecure_code_detector.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_javascript_insecure_code_detector.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_kotlin_insecure_code_detector.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_objective_c_code_detector.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_php_insecure_code_detector.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_python_insecure_code_detector.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_ruby_insecure_code_detector.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_rust_insecure_code_detector.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_swift_code_detector.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 codeshield-1.0.1/insecure_code_detector/tests/test_xml_insecure_code_detector.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 codeshield-1.0.1/notebook/CodeShieldUsageDemo.ipynb
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 codeshield-1.0.1/tests/test_codeshield.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 codeshield-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 codeshield-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 codeshield-1.0.1/README.md
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 codeshield-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 codeshield-1.0.1/PKG-INFO
```

### Comparing `codeshield-1.0.0/codeshield.py` & `codeshield-1.0.1/codeshield.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env fbpython
-# (c) Meta Platforms, Inc. and affiliates. Confidential and proprietary.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+#
+# This source code is licensed under the MIT license found in the
+# LICENSE file in the root directory of this source tree.
 
 # pyre-strict
 
 from __future__ import annotations
 
 import asyncio
 
@@ -78,15 +81,15 @@
                     if issue is not None:
                         issues.extend(issue)
             else:
                 issues = await cls._execute_icd(language, code)
         except Exception as e:
             LOG.error(f"Exception while scanning for code security: {e}")
             return result
-
+        # pyre-ignore
         if len(issues) > 0:
             result.is_insecure = True
             result.issues_found = issues
             # pyre-ignore
             if any(issue.severity == Severity.ERROR for issue in issues):
                 result.recommended_treatment = Treatment.BLOCK
             else:
```

### Comparing `codeshield-1.0.0/example.py` & `codeshield-1.0.1/example.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env fbpython
-# (c) Meta Platforms, Inc. and affiliates. Confidential and proprietary.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+#
+# This source code is licensed under the MIT license found in the
+# LICENSE file in the root directory of this source tree.
 
 # pyre-strict
 
 from __future__ import annotations
 
 import asyncio
```

### Comparing `codeshield-1.0.0/images/codeshield_logo.png` & `codeshield-1.0.1/images/codeshield_logo.png`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/images/design.png` & `codeshield-1.0.1/images/design.png`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/README.md` & `codeshield-1.0.1/insecure_code_detector/README.md`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/insecure_patterns.py` & `codeshield-1.0.1/insecure_code_detector/insecure_patterns.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/issues.py` & `codeshield-1.0.1/insecure_code_detector/issues.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/languages.py` & `codeshield-1.0.1/insecure_code_detector/languages.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/oss.py` & `codeshield-1.0.1/insecure_code_detector/oss.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/README.md` & `codeshield-1.0.1/insecure_code_detector/rules/README.md`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/config.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/config.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/c.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/c.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/cpp.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/cpp.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/csharp.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/csharp.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/java.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/java.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/language_agnostic.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/language_agnostic.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/objective_c.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/objective_c.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/php.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/php.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/python.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/python.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/rust.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/rust.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/swift.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/swift.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/regex/xml.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/regex/xml.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/c_codeshield.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/c_codeshield.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/c_cyberseceval.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/c_cyberseceval.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/cpp_codeshield.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/cpp_codeshield.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/cpp_cyberseceval.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/cpp_cyberseceval.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/csharp_codeshield.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/csharp_codeshield.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/csharp_cyberseceval.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/csharp_cyberseceval.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/java_codeshield.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/java_codeshield.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/java_cyberseceval.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/java_cyberseceval.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/javascript_codeshield.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/javascript_codeshield.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/javascript_cyberseceval.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/javascript_cyberseceval.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/php_codeshield.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/php_codeshield.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/php_cyberseceval.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/php_cyberseceval.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/python_codeshield.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/python_codeshield.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/_generated_/python_cyberseceval.json` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/_generated_/python_cyberseceval.json`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/bad-crypto-api-usage.c` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/bad-crypto-api-usage.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-// (c) Meta Platforms, Inc. and affiliates. Confidential and proprietary.
+/*
+ * Copyright (c) Meta Platforms, Inc. and affiliates.
+ *
+ * This source code is licensed under the MIT license found in the
+ * LICENSE file in the root directory of this source tree.
+ */
 
 void warnOnMd5Usage() {
   // ruleid: md5-usage
   MD5_Init(1);
   EVP_md5(1);
   EVP_md5();
   EVP_md5(1, 2, 3);
```

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/bugprone-snprintf.c` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/bugprone-snprintf.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+/*
+ * Copyright (c) Meta Platforms, Inc. and affiliates.
+ *
+ * This source code is licensed under the MIT license found in the
+ * LICENSE file in the root directory of this source tree.
+ */
+
 #include <stdio.h>
 #include <string.h>
 
 void WarnOnMisuseofSnprintf() {
   char buf[50];
   char str[60];
   int ret = 0;
```

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/bugprone-snprintf.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/bugprone-snprintf.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/crypto_rsa_key_size_insufficient.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/crypto_rsa_key_size_insufficient.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/crypto_unauthenticated_encryption_usage.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/crypto_unauthenticated_encryption_usage.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/fixed_nonce_use.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/fixed_nonce_use.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/fixed_seed_use.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/fixed_seed_use.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/hardcoded_key_use.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/hardcoded_key_use.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/integer-overflow-to-buffer-overflow.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/integer-overflow-to-buffer-overflow.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/invalid-free.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/invalid-free.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/mcf-get-c-string-result-ignored.c` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/mcf-get-c-string-result-ignored.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-// (c) Meta Platforms, Inc. and affiliates. Confidential and proprietary.
+/*
+ * Copyright (c) Meta Platforms, Inc. and affiliates.
+ *
+ * This source code is licensed under the MIT license found in the
+ * LICENSE file in the root directory of this source tree.
+ */
 
 typedef const void* MCFStringRef;
 typedef unsigned int MCFStringEncoding;
 
 bool MCFStringGetCString(
     MCFStringRef str,
     char* buffer,
```

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/mcf-get-c-string-result-ignored.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/mcf-get-c-string-result-ignored.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/potential-command-injection.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/potential-command-injection.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/c/write-to-stack-buffer.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/c/write-to-stack-buffer.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/command_injection.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/command_injection.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/cookie_without_http_only_flag.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/cookie_without_http_only_flag.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/cookie_without_ssl_flag.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/cookie_without_ssl_flag.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_certification_validation_disabled.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_certification_validation_disabled.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_cipher_algorithm.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_cipher_algorithm.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_cipher_mode.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_cipher_mode.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_hashing_function.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_hashing_function.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_prng.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/crypto_weak_prng.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/csrf.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/csrf.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/input_validation.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/input_validation.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/insecure_deserialization.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/insecure_deserialization.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/ldap_injection.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/ldap_injection.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/path_traversal.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/path_traversal.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/sql_injection.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/sql_injection.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/unsafe_xslt_setting.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/unsafe_xslt_setting.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/unvalidated_redirect.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/unvalidated_redirect.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/weak-password-requirements.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/weak-password-requirements.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/xpath_injection.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/xpath_injection.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/xss.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/xss.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/csharp/third-party/xxe.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/csharp/third-party/xxe.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/cors_header_injection.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/cors_header_injection.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/csrf_disabled.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/csrf_disabled.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/ldap_anonymous.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/ldap_anonymous.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/random_number_generator.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/random_number_generator.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/ssrf.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/ssrf.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xpath_injection.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xpath_injection.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xss_send_error_response.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xss_send_error_response.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xss_servlet_response.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xss_servlet_response.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xxe_sax_parser.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xxe_sax_parser.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xxe_xml_input_factory.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xxe_xml_input_factory.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/java/third-party/xxe_xml_reader.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/java/third-party/xxe_xml_reader.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/child-process.js` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/child-process.js`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/child-process.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/child-process.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/unchecked-origin-onmessage.js` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/unchecked-origin-onmessage.js`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/unchecked-origin-onmessage.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/unchecked-origin-onmessage.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/unencrypted-fetch.js` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/unencrypted-fetch.js`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/unencrypted-fetch.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/unencrypted-fetch.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/buffer-noassert.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/buffer-noassert.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/dangerously-set-inner-html.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/dangerously-set-inner-html.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/detect-new-buffer.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/detect-new-buffer.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/eval-usage.js` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/eval-usage.js`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/eval-usage.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/eval-usage.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/mustache-escape.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/mustache-escape.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-fs-filename.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-fs-filename.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-regexp.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-regexp.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-require.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/non-literal-require.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/possible-timing-attacks.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/possible-timing-attacks.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/javascript/third-party/pseudo-random-bytes.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/javascript/third-party/pseudo-random-bytes.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/tainted_exec.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/tainted_exec.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/unsafe_extract.php` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/unsafe_extract.php`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-// (c) Meta Platforms, Inc. and affiliates. Confidential and proprietary.
+/*
+ * Copyright (c) Meta Platforms, Inc. and affiliates.
+ *
+ * This source code is licensed under the MIT license found in the
+ * LICENSE file in the root directory of this source tree.
+ */
 
 <?php
 
 $test = $_POST;
 $test2 = $_GET["p"];
 
 // ruleid: unsafe-extract
```

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/php/unsafe_extract.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/php/unsafe_extract.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/crypto_fixed_nonce.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/crypto_fixed_nonce.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/crypto_prng_random.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/crypto_prng_random.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/deserialization_json_pickle_use.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/deserialization_json_pickle_use.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/deserialization_yaml_use.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/deserialization_yaml_use.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/eval_use.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/eval_use.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/exec_use.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/exec_use.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/hardcoded_secrets.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/hardcoded_secrets.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/os_popen_use.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/os_popen_use.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/os_system_use.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/os_system_use.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/sql_injection_cursor_execute.py` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/sql_injection_cursor_execute.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/sql_injection_cursor_execute.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/sql_injection_cursor_execute.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/subprocess_using_shell.py` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/subprocess_using_shell.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/python/subprocess_using_shell.yaml` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/python/subprocess_using_shell.yaml`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/rules/semgrep/rule_gen/gen_consolidated_rules.py` & `codeshield-1.0.1/insecure_code_detector/rules/semgrep/rule_gen/gen_consolidated_rules.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/insecure_code_detector_test.py` & `codeshield-1.0.1/insecure_code_detector/tests/insecure_code_detector_test.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_c_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_c_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_cpp_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_cpp_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_csharp_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_csharp_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_functional.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_java_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_java_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_javascript_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_javascript_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_kotlin_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_kotlin_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_objective_c_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_objective_c_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_php_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_php_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_python_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_python_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_ruby_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_ruby_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_rust_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_rust_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_swift_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_swift_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/insecure_code_detector/tests/test_xml_insecure_code_detector.py` & `codeshield-1.0.1/insecure_code_detector/tests/test_xml_insecure_code_detector.py`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/notebook/CodeShieldUsageDemo.ipynb` & `codeshield-1.0.1/notebook/CodeShieldUsageDemo.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'cells'": "{2: {'execution_count': None}, 4: {'execution_count': None, 'outputs': []}}"}*

```diff
@@ -34,15 +34,15 @@
                 "# Examples\n",
                 "\n",
                 "Define a helper function to run scan and process output."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from codeshield.cs import CodeShield\n",
                 "\n",
                 "async def scan_llm_output(llm_output_code):\n",
                 "    result = await CodeShield.scan_code(llm_output_code)\n",
@@ -75,42 +75,17 @@
             "source": [
                 "## Example 1 - Simple hard-coded example\n",
                 "In this example, we are taking a hard coded example where the code snippet has weak hash md5 function usage. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "## LLM output after treatment\n",
-                        "\t \n",
-                        "def hashString(input):\n",
-                        "    return hashlib.md5(input)\n",
-                        "*** Warning: The generated snippit contains insecure code *** \n",
-                        "\n",
-                        "## Results:\n",
-                        "\n",
-                        "\t Security issue detected\n",
-                        "\t Recommended treatment: Treatment.WARN\n",
-                        "\n",
-                        "## Details:\n",
-                        "\n",
-                        "\tIssue found: \n",
-                        "\t\tPattern id: weak-md5-hashing \n",
-                        "\t\tDescription: Use of weak hashing algorithm \n",
-                        "\t\tSeverity: warning \n",
-                        "\t\tLine number: 3\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "llm_output_code = \"\"\"\n",
                 "def hashString(input):\n",
                 "    return hashlib.md5(input)\n",
                 "\"\"\"\n",
                 "\n",
                 "await scan_llm_output(llm_output_code)"
```

### Comparing `codeshield-1.0.0/LICENSE` & `codeshield-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codeshield-1.0.0/README.md` & `codeshield-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # CodeShield
 > Shield against LLM generated insecure code
 <p align="center">
-  <img src="https://raw.githubusercontent.com/facebookresearch/LlamaFirewall/021cbb85a496e719a36ea26987950c85d98b5cac/CodeShield/images/codeshield_logo.png?token=GHSAT0AAAAAACQC3OLULHFQB62XJTADXFTIZRBHVVA" width="400"/>
+  <img src="https://raw.githubusercontent.com/meta-llama/PurpleLlama/main/CodeShield/images/codeshield_logo.png" width="400"/>
 </p>
 
 CodeShield is a robust inference time filtering tool engineered to prevent the introduction of insecure code generated by LLMs into production systems. LLMs, while instrumental in automating coding tasks and aiding developers, can sometimes output insecure code, even when they have been security-conditioned.  CodeShield stands as a guardrail to help ensure that such code is intercepted and filtered out before making it into the codebase.
 ## Overview
 
 LLMs have become an integral part of the coding process, automating coding tasks and serving as a co-pilot for developers. However, our study [CyberSecEval](https://arxiv.org/abs/2312.04724), revealed that it is not uncommon for these code-producing models to inadvertently generate insecure code. This poses a significant risk when developers incorporate this insecure code without verification, especially for those who do not have strong cybersecurity background
-CodeShield helps mitigate this risk by intercepting and blocking insecure code generated by LLMs in a configurable way. CodeShield leverages a static analysis library, the Insecure Code Detector (ICD), to identify insecure code. ICD uses a suite of static analysis tools to perform the analysis across 7 programming languages, covering more than 50+ CWEs. For more details, please see  [here](https://github.com/meta-llama/PurpleLlama/tree/main/CodeShield/insecure_code_detector)
+CodeShield helps mitigate this risk by intercepting and blocking insecure code generated by LLMs in a configurable way. CodeShield leverages a static analysis library, the Insecure Code Detector (ICD), to identify insecure code. ICD uses a suite of static analysis tools to perform the analysis across 7 programming languages, covering more than 50+ CWEs. For more details, please see  [here](https://github.com/meta-llama/PurpleLlama/tree/main/CodeShield/insecure_code_detector?tab=readme-ov-file#insecure-code-detector)
+
 
 ## Use Cases
 CodeShield is designed to be applicable for various scenarios, here are a few example use cases
 * LLM is utilized as a coding assistant. CodeShield is an ideal fit for AI Coding assistants integrated with IDEs like VSCode or any other development framework, where it is able to block insecure code suggestions
 * Chatbots are used to help with coding tasks. It has become a common practice for developers to ask LLMs for code snippets. Consequently, more and more code is produced by LLMs nowadays. Codeshield is able to fortify any code-producing LLMs by either adding a warning message or completely blocking the response
 
 <p align = "center">
-    <img src="https://raw.githubusercontent.com/facebookresearch/LlamaFirewall/021cbb85a496e719a36ea26987950c85d98b5cac/CodeShield/images/design.png?token=GHSAT0AAAAAACQC3OLUF5EUR36VRSNYL23QZRBHXOA" alt="ImageA" width="400">
+    <img src="https://raw.githubusercontent.com/meta-llama/PurpleLlama/main/CodeShield/images/design.png" alt="ImageA" width="400">
     <figcaption style="text-align: center;">Fig1: Depicting the flow of how CodeShield should be used for output scanning from LLM before the suggestions are propagated for the user facing applications.</figcaption>
 </p>
 
 ## Latency
 CodeShield is optimized for production environments where latency is a critical factor for user experience. It is designed to swiftly process the input by a two-layer scanning solution. Specifically, CodeShield will first identify alarming code patterns in the to be scanned content, and perform a more comprehensive analysis if the content is deemed suspicious in the first step.
 
 Our studies indicate that in production environments, over 98% of the traffic is classified as benign and does not necessitate comprehensive scanning. This means that in approximately 99% of cases, requests are processed within a swift 70ms window. For the remaining traffic that requires more thorough scanning, the p90 latency is 450ms in modern production server environments.
```

### Comparing `codeshield-1.0.0/pyproject.toml` & `codeshield-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "codeshield"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name = "Sahana CB", email = "csahana@meta.com" },
   { name = "Thomas Robinson", email = "trobinson@meta.com" },
 ]
 description = "Shield against LLM generated insecure code"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -24,8 +24,8 @@
 
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel.force-include]
 "codeshield.py" = "codeshield/cs.py"
-"insecure_code_detector/" = "codeshield/insecure_code_detector"
+"insecure_code_detector/" = "codeshield/insecure_code_detector"
```

### Comparing `codeshield-1.0.0/PKG-INFO` & `codeshield-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: codeshield
-Version: 1.0.0
+Version: 1.0.1
 Summary: Shield against LLM generated insecure code
 Project-URL: Homepage, https://github.com/meta-llama/PurpleLlama
 Project-URL: Issues, https://github.com/meta-llama/PurpleLlama/issues
 Author-email: Sahana CB <csahana@meta.com>, Thomas Robinson <trobinson@meta.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,30 +15,31 @@
 Provides-Extra: external-llm
 Requires-Dist: llama-recipes; extra == 'external-llm'
 Description-Content-Type: text/markdown
 
 # CodeShield
 > Shield against LLM generated insecure code
 <p align="center">
-  <img src="https://raw.githubusercontent.com/facebookresearch/LlamaFirewall/021cbb85a496e719a36ea26987950c85d98b5cac/CodeShield/images/codeshield_logo.png?token=GHSAT0AAAAAACQC3OLULHFQB62XJTADXFTIZRBHVVA" width="400"/>
+  <img src="https://raw.githubusercontent.com/meta-llama/PurpleLlama/main/CodeShield/images/codeshield_logo.png" width="400"/>
 </p>
 
 CodeShield is a robust inference time filtering tool engineered to prevent the introduction of insecure code generated by LLMs into production systems. LLMs, while instrumental in automating coding tasks and aiding developers, can sometimes output insecure code, even when they have been security-conditioned.  CodeShield stands as a guardrail to help ensure that such code is intercepted and filtered out before making it into the codebase.
 ## Overview
 
 LLMs have become an integral part of the coding process, automating coding tasks and serving as a co-pilot for developers. However, our study [CyberSecEval](https://arxiv.org/abs/2312.04724), revealed that it is not uncommon for these code-producing models to inadvertently generate insecure code. This poses a significant risk when developers incorporate this insecure code without verification, especially for those who do not have strong cybersecurity background
-CodeShield helps mitigate this risk by intercepting and blocking insecure code generated by LLMs in a configurable way. CodeShield leverages a static analysis library, the Insecure Code Detector (ICD), to identify insecure code. ICD uses a suite of static analysis tools to perform the analysis across 7 programming languages, covering more than 50+ CWEs. For more details, please see  [here](https://github.com/meta-llama/PurpleLlama/tree/main/CodeShield/insecure_code_detector)
+CodeShield helps mitigate this risk by intercepting and blocking insecure code generated by LLMs in a configurable way. CodeShield leverages a static analysis library, the Insecure Code Detector (ICD), to identify insecure code. ICD uses a suite of static analysis tools to perform the analysis across 7 programming languages, covering more than 50+ CWEs. For more details, please see  [here](https://github.com/meta-llama/PurpleLlama/tree/main/CodeShield/insecure_code_detector?tab=readme-ov-file#insecure-code-detector)
+
 
 ## Use Cases
 CodeShield is designed to be applicable for various scenarios, here are a few example use cases
 * LLM is utilized as a coding assistant. CodeShield is an ideal fit for AI Coding assistants integrated with IDEs like VSCode or any other development framework, where it is able to block insecure code suggestions
 * Chatbots are used to help with coding tasks. It has become a common practice for developers to ask LLMs for code snippets. Consequently, more and more code is produced by LLMs nowadays. Codeshield is able to fortify any code-producing LLMs by either adding a warning message or completely blocking the response
 
 <p align = "center">
-    <img src="https://raw.githubusercontent.com/facebookresearch/LlamaFirewall/021cbb85a496e719a36ea26987950c85d98b5cac/CodeShield/images/design.png?token=GHSAT0AAAAAACQC3OLUF5EUR36VRSNYL23QZRBHXOA" alt="ImageA" width="400">
+    <img src="https://raw.githubusercontent.com/meta-llama/PurpleLlama/main/CodeShield/images/design.png" alt="ImageA" width="400">
     <figcaption style="text-align: center;">Fig1: Depicting the flow of how CodeShield should be used for output scanning from LLM before the suggestions are propagated for the user facing applications.</figcaption>
 </p>
 
 ## Latency
 CodeShield is optimized for production environments where latency is a critical factor for user experience. It is designed to swiftly process the input by a two-layer scanning solution. Specifically, CodeShield will first identify alarming code patterns in the to be scanned content, and perform a more comprehensive analysis if the content is deemed suspicious in the first step.
 
 Our studies indicate that in production environments, over 98% of the traffic is classified as benign and does not necessitate comprehensive scanning. This means that in approximately 99% of cases, requests are processed within a swift 70ms window. For the remaining traffic that requires more thorough scanning, the p90 latency is 450ms in modern production server environments.
```

