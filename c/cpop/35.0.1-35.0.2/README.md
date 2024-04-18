# Comparing `tmp/cpop-35.0.1.tar.gz` & `tmp/cpop-35.0.2.tar.gz`

## Comparing `cpop-35.0.1.tar` & `cpop-35.0.2.tar`

### file list

```diff
@@ -1,175 +1,175 @@
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 cpop-35.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/Makefile
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/make.bat
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/outline.rst
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/index.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/releases/32.rst
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/app_merging.rst
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/conf.rst
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/conf_integrate.rst
--rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/contracts.rst
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/dyne_name.rst
--rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/func_alias.rst
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/glossary.rst
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/hub_overview.rst
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/ideas_that_were_not_used.rst
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/learning.rst
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/pop.rst
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/pre_contract_returns.rst
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/story.rst
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/sub_patterns.rst
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/subs_overview.rst
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/topics/virtual.rst
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-35.0.1/docs/source/tutorial/quickstart.rst
--rw-r--r--   0        0        0     9581 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/data.pyx
--rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/dirs.pyx
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/exc.pyx
--rw-r--r--   0        0        0    26676 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/hub.pyx
--rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/loader.pyx
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/ref.pyx
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/scanner.pyx
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-35.0.1/src/cpop/verify.pyx
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/config.yaml
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/log/basic.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/log/init.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/log/timed_rolling.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/log/contracts/init.py
--rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/config.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/contract.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/task.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-35.0.1/src/pop/mods/test.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/contracts/test.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/coro/contracts/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/__init__.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_cli.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_config.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_coro.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_cpop.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_dyne.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_fail.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_hub.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_log.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_ref.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/func/test_sub.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/bad.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/falias_func.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/proc.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/vtrue.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/README.rst
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/unit/__init__.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-35.0.1/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-35.0.1/.gitignore
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 cpop-35.0.1/README.rst
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 cpop-35.0.1/pyproject.toml
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cpop-35.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 cpop-35.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/Makefile
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/make.bat
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/outline.rst
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/releases/32.rst
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/app_merging.rst
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/conf.rst
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/conf_integrate.rst
+-rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/contracts.rst
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/dyne_name.rst
+-rw-r--r--   0        0        0     8191 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/func_alias.rst
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/glossary.rst
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/hub_overview.rst
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/ideas_that_were_not_used.rst
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/learning.rst
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/pop.rst
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/pre_contract_returns.rst
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/story.rst
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/sub_patterns.rst
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/subs_overview.rst
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/topics/virtual.rst
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 cpop-35.0.2/docs/source/tutorial/quickstart.rst
+-rw-r--r--   0        0        0     9581 2020-02-02 00:00:00.000000 cpop-35.0.2/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 cpop-35.0.2/src/cpop/data.pyx
+-rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 cpop-35.0.2/src/cpop/dirs.pyx
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 cpop-35.0.2/src/cpop/exc.pyx
+-rw-r--r--   0        0        0    26963 2020-02-02 00:00:00.000000 cpop-35.0.2/src/cpop/hub.pyx
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 cpop-35.0.2/src/cpop/loader.pyx
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 cpop-35.0.2/src/cpop/ref.pyx
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.2/src/cpop/scanner.pyx
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 cpop-35.0.2/src/cpop/verify.pyx
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/config.yaml
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/log/basic.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/log/init.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/log/timed_rolling.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/log/contracts/init.py
+-rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/mods/config.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/mods/task.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-35.0.2/src/pop/mods/test.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/contracts/test.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/__init__.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_cli.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_config.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_coro.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_cpop.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_dyne.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_fail.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_hub.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_log.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_ref.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/func/test_sub.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/bad.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/falias_func.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/proc.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/vtrue.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/README.rst
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 cpop-35.0.2/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-35.0.2/.gitignore
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 cpop-35.0.2/README.rst
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 cpop-35.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cpop-35.0.2/PKG-INFO
```

### Comparing `cpop-35.0.1/.pre-commit-config.yaml` & `cpop-35.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/Makefile` & `cpop-35.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/make.bat` & `cpop-35.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/outline.rst` & `cpop-35.0.2/docs/outline.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/conf.py` & `cpop-35.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/index.rst` & `cpop-35.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/app_merging.rst` & `cpop-35.0.2/docs/source/topics/app_merging.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/conf.rst` & `cpop-35.0.2/docs/source/topics/conf.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/conf_integrate.rst` & `cpop-35.0.2/docs/source/topics/conf_integrate.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/contracts.rst` & `cpop-35.0.2/docs/source/topics/contracts.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/dyne_name.rst` & `cpop-35.0.2/docs/source/topics/dyne_name.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/func_alias.rst` & `cpop-35.0.2/docs/source/topics/func_alias.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/glossary.rst` & `cpop-35.0.2/docs/source/topics/glossary.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/hub_overview.rst` & `cpop-35.0.2/docs/source/topics/hub_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/ideas_that_were_not_used.rst` & `cpop-35.0.2/docs/source/topics/ideas_that_were_not_used.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/learning.rst` & `cpop-35.0.2/docs/source/topics/learning.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/pop.rst` & `cpop-35.0.2/docs/source/topics/pop.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/pre_contract_returns.rst` & `cpop-35.0.2/docs/source/topics/pre_contract_returns.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/story.rst` & `cpop-35.0.2/docs/source/topics/story.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/sub_patterns.rst` & `cpop-35.0.2/docs/source/topics/sub_patterns.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/subs_overview.rst` & `cpop-35.0.2/docs/source/topics/subs_overview.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/topics/virtual.rst` & `cpop-35.0.2/docs/source/topics/virtual.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/docs/source/tutorial/quickstart.rst` & `cpop-35.0.2/docs/source/tutorial/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/cpop/contract.pyx` & `cpop-35.0.2/src/cpop/contract.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/cpop/data.pyx` & `cpop-35.0.2/src/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/cpop/dirs.pyx` & `cpop-35.0.2/src/cpop/dirs.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/cpop/exc.pyx` & `cpop-35.0.2/src/cpop/exc.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/cpop/hub.pyx` & `cpop-35.0.2/src/cpop/hub.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             pop_mods: list[str] = None,
             cli: str = None,
             logs: bool = True,
             load_config: bool = True,
             sigint = None,
             sigterm = None
             ):
-        self._init_kwargs = {
+        self.__init_kwargs = {
             k: v for k, v in locals().items() if k != "self" and not k.startswith("_")
         }
         subs = {}
         sub_alias = {}
         imports = {}
         PopMeta.__init__(self, [subs, sub_alias, imports])
         self._subs = subs
@@ -107,61 +107,57 @@
     async def __aenter__(
         self,
     ):
         self._tasks = asyncio.Queue()
 
         loop = asyncio.get_running_loop()
 
-        sigint = self._init_kwargs["sigint"]
+        sigint = self.__init_kwargs["sigint"]
         if sigint:
             s = signal.SIGINT
             loop.add_signal_handler(s, lambda s=s: loop.create_task(sigint(s)))
-        sigterm = self._init_kwargs["sigterm"]
+        sigterm = self.__init_kwargs["sigterm"]
         if sigterm:
             s = signal.SIGTERM
             loop.add_signal_handler(s, lambda s=s: loop.create_task(sigterm(s)))
 
         # Add the dyne for python imports to live in to the hub
         if "lib" not in self._subs:
             self._subs["lib"] = await AsyncSub(
-                self, subname="lib", dyne_name="lib"
-            )
-            # Load all existing libraries onto hub.lib
-            self._subs["lib"]._imports.update(
-                {
-                    base: mod
-                    for base, mod in sys.modules.items()
-                    if not base.startswith("_") and "." not in base
-                }
+                self,
+                subname="lib",
+                dyne_name="lib",
+                # Allow the sub to find python modules dynamically
+                lookup_paths=[sys.modules]
             )
 
-        pop_mods = self._init_kwargs["pop_mods"]
+        pop_mods = self.__init_kwargs["pop_mods"]
         if pop_mods is None:
             pop_mods = ["pop.mods"]
         if "pop" not in self._subs:
 
             # Add the pop sub to the hub, this should always use pypath and
             # Should never be made dynamic. This is a core system sub and should
             # NOT be app-merged
             self._subs["pop"] = await AsyncSub(self, subname="pop", pypath=pop_mods)
             await self._subs["pop"]._load_all()
 
-        self._load_all_dynes = self._init_kwargs["load_all_dynes"]
-        self._load_all_subdirs = self._init_kwargs["load_all_subdirs"]
-        self._recurse_subdirs = self._init_kwargs["recurse_subdirs"]
+        self._load_all_dynes = self.__init_kwargs["load_all_dynes"]
+        self._load_all_subdirs = self.__init_kwargs["load_all_subdirs"]
+        self._recurse_subdirs = self.__init_kwargs["recurse_subdirs"]
         if self._load_all_dynes:
             await self._scan_dynamic()
             await self._load_all()
 
-            if self._init_kwargs["load_config"]:
+            if self.__init_kwargs["load_config"]:
                 # Overwrite opt with config data
-                self._opt = await self.pop.config.load(cli=self._init_kwargs["cli"], **self._dynamic.config)
+                self._opt = await self.pop.config.load(cli=self.__init_kwargs["cli"], **self._dynamic.config)
 
         # Set up a logger
-        if "log" in self._subs and self._init_kwargs["logs"]:
+        if "log" in self._subs and self.__init_kwargs["logs"]:
             await self.log.init.setup(**self._opt.log.copy())
 
         return self
 
     async def __aexit__(self, exc_type, exc_value, tb):
         if exc_type is not None and exc_value is not None:
             self._traceback(exc_type, exc_value, tb)
@@ -263,15 +259,15 @@
             elif isinstance(v, dict):
                 if all(isinstance(v2, cpop.loader.BASE_TYPES) for v2 in v.values()):
                     attrs[k] = v
             elif isinstance(v, Iterable):
                 if all(isinstance(v2, cpop.loader.BASE_TYPES) for v2 in v):
                     attrs[k] = v
         state = dict(
-            init_kwargs=self._init_kwargs,
+            init_kwargs=self.__init_kwargs,
             subs={name: sub.__getstate__() for name, sub in self._subs.items()},
             aliases=self._sub_alias,
             OPT=cpop.data.unfreeze(self._opt),
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
             attrs=attrs,
         )
         return state
@@ -347,14 +343,15 @@
         mod_basename: str = "",
         stop_on_failures: bool = False,
         init: bool = True,
         is_contract: bool = False,
         sub_virtual: bool = True,
         recursive_contracts_static: list[str] = None,
         default_recursive_contracts: list[str] = None,
+        lookup_paths: list[dict] = None,
     ):
         """
         :param hub: The redistributed pop central hub
         :param subname: The name that the sub is going to take on the hub
             if nothing else is passed, it is used as the pypath
         :param pypath: One or many python paths which will be imported
         :param static: Directories that can be explicitly passed
@@ -375,26 +372,28 @@
             Allow plugins to be loaded into a separate namespace.
         :param stop_on_failures: If any module fails to load for any reason, stacktrace and do not continue
             loading this sub
         :param init: bool: determine whether or not we process __init__ functions
         :param is_contract: Specify whether or not this sub is a contract
         :param sub_virtual: bool: Recursively ignore this sub and it's subs
         """
-        self._init_kwargs = {
+        self.__init_kwargs = {
             k: v
             for k, v in locals().items()
             if k not in ("self", "hub", "root") and not k.startswith("_")
         }
         subs = {}
         sub_alias = {}
         imports = {}
         loaded = {}
         # tracks what has been setattr-ed on this sub for performance; if something needs to be
         # *removed*, we can delattr everything in _cached, it will be re-set on the next call.
-        super().__init__([loaded, imports, subs, sub_alias])
+        if lookup_paths is None:
+            lookup_paths =  []
+        super().__init__([loaded, imports, subs, sub_alias] + lookup_paths)
         self._subs = subs
         self._sub_alias = sub_alias
         self._imports = imports
         self._loaded = loaded
         self._reload_mods = {}
         self._alias = []
         self._loaded_all = False
@@ -508,24 +507,33 @@
             return self._pypath[0]
         elif self._dirs:
             return secrets.token_hex()
 
     def __getstate__(self):
         attrs = {}
         for k, v in self._attrs.items():
-            if isinstance(v, cpop.loader.BASE_TYPES):
-                attrs[k] = v
-            elif isinstance(v, dict):
+            if isinstance(v, dict):
                 if all(isinstance(v2, cpop.loader.BASE_TYPES) for v2 in v.values()):
                     attrs[k] = v
             elif isinstance(v, Iterable):
                 if all(isinstance(v2, cpop.loader.BASE_TYPES) for v2 in v):
                     attrs[k] = v
+            elif isinstance(v, cpop.loader.BASE_TYPES):
+                attrs[k] = v
+
+        init_kwargs = self.__init_kwargs.copy()
+        lookup_paths = []
+        for dict_ in (init_kwargs.pop("lookup_paths", None) or []):
+            if all(isinstance(v2, cpop.loader.BASE_TYPES) for v2 in dict_.values()):
+                lookup_paths.append(dict_)
+
+        init_kwargs["lookup_paths"] = lookup_paths
+
         return dict(
-            init_kwargs=self._init_kwargs,
+            init_kwargs=lookup_paths,
             loaded={
                 item: dict(
                     iface=iface, bname=bname, state=self._loaded[item].__getstate__()
                 )
                 for item, (iface, bname) in self._reload_mods.items()
             },
             subs={name: sub.__getstate__() for name, sub in self._subs.items()},
```

### Comparing `cpop-35.0.1/src/cpop/loader.pyx` & `cpop-35.0.2/src/cpop/loader.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/cpop/ref.pyx` & `cpop-35.0.2/src/cpop/ref.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/cpop/scanner.pyx` & `cpop-35.0.2/src/cpop/scanner.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/cpop/verify.pyx` & `cpop-35.0.2/src/cpop/verify.pyx`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/pop/config.yaml` & `cpop-35.0.2/src/pop/config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -78,11 +78,13 @@
   - logging
   - os
   - cpop.exc
   - cpop.contract
   - cpop.data
   - cpop.hub
   - msgpack
+  - pickle
   - signal
   - sys
   - traceback
   - yaml
+  - typing
```

### Comparing `cpop-35.0.1/src/pop/log/basic.py` & `cpop-35.0.2/src/pop/log/basic.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/pop/log/init.py` & `cpop-35.0.2/src/pop/log/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/pop/log/timed_rolling.py` & `cpop-35.0.2/src/pop/log/timed_rolling.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/pop/mods/config.py` & `cpop-35.0.2/src/pop/mods/config.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/pop/mods/contract.py` & `cpop-35.0.2/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/pop/mods/sub.py` & `cpop-35.0.2/src/pop/mods/sub.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     omit_vars: bool = False,
     mod_basename: str = "pop.sub",
     stop_on_failures: bool = False,
     init: bool = True,
     recursive_contracts_static: list[str] = None,
     default_recursive_contracts: list[str] = None,
     python_import: str = None,
+    lookup_paths: list[dict] = None,
 ):
     """
     Add a new subsystem to the hub
     :param hub: The redistributed pop central hub
     :param subname: The name that the sub is going to take on the hub
         if nothing else is passed, it is used as the dyne_name
     :param sub: The sub to use as the root to add to
@@ -51,14 +52,15 @@
         Allow plugins to be loaded into a separate namespace.
     :param stop_on_failures: If any module fails to load for any reason, stacktrace and do not continue loading this sub
     :param init: bool: determine whether or not we process __init__ functions
     :param recursive_contracts_static: Load additional recursive contract paths from a specific directory
     :param default_recursive_contracts: Specifies that a specific recursive contract plugin will be applied as a default
         to all plugins
     :param python_import: Load a module from python onto the sub
+    :param lookup_paths: A list of dictionaries where the Sub will resolve getattr from
     """
     if python_import:
         subname = subname if subname else python_import.split(".")[0]
     if pypath:
         pypath = cpop.hub.ex_path(pypath)
         subname = subname if subname else pypath[0].split(".")[-1]
     elif static:
@@ -93,14 +95,15 @@
         omit_vars=omit_vars,
         mod_basename=mod_basename,
         stop_on_failures=stop_on_failures,
         init=init,
         sub_virtual=getattr(root, "_subvirt", True),
         recursive_contracts_static=recursive_contracts_static,
         default_recursive_contracts=default_recursive_contracts,
+        lookup_paths=lookup_paths,
     )
     # init the sub (init.py:__init__) after it can be referenced on the hub!
     await root._subs[subname]._sub_init()
     await root._subs[subname]._load_all()
     for alias in root._subs[subname]._alias:
         root._sub_alias[alias] = root._subs[subname]
```

### Comparing `cpop-35.0.1/src/pop/mods/task.py` & `cpop-35.0.2/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/src/pop/mods/test.py` & `cpop-35.0.2/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/conftest.py` & `cpop-35.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/contracts/ctx.py` & `cpop-35.0.2/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/contracts/many.py` & `cpop-35.0.2/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/contracts/test.py` & `cpop-35.0.2/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/func/test_basic.py` & `cpop-35.0.2/tests/func/test_basic.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/func/test_config.py` & `cpop-35.0.2/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/func/test_contract_ctx.py` & `cpop-35.0.2/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/func/test_fail.py` & `cpop-35.0.2/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/func/test_log.py` & `cpop-35.0.2/tests/func/test_log.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/func/test_no_raise_on_pre_failure.py` & `cpop-35.0.2/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/func/test_raise_on_pre_failure.py` & `cpop-35.0.2/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/func/test_ref.py` & `cpop-35.0.2/tests/func/test_ref.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/func/test_serial.py` & `cpop-35.0.2/tests/func/test_serial.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 
 async def test_serialize_hub(hub):
     hub.lib.pickle.dumps(hub)
 
 
 async def test_serialize_sub(hub):
-    hub.lib.pickle.dumps(hub.lib)
+    hub.lib.pickle.dumps(hub.pop)
 
+async def test_serialize_lib(hub):
+    hub.lib.pickle.dumps(hub.lib)
 
 def child_process(hub):
     # Try to access or modify the hub object in the child process
     hub.VAR.value += 1
     return hub.VAR
```

### Comparing `cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-35.0.2/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-35.0.2/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-35.0.2/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-35.0.2/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-35.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-35.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-35.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-35.0.2/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-35.0.2/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-35.0.2/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/mods/proc.py` & `cpop-35.0.2/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/mods/test.py` & `cpop-35.0.2/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/regression/contract_masking/test_contract_masking.py` & `cpop-35.0.2/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-35.0.2/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/tpath/cn/contract/test.py` & `cpop-35.0.2/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/unit/test_contract.py` & `cpop-35.0.2/tests/unit/test_contract.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/tests/unit/test_sigs.py` & `cpop-35.0.2/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/.gitignore` & `cpop-35.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/README.rst` & `cpop-35.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-35.0.1/pyproject.toml` & `cpop-35.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython", "hatch-compile-yaml>=18.0.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "35.0.1"
+version = "35.0.2"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
```

### Comparing `cpop-35.0.1/PKG-INFO` & `cpop-35.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 35.0.1
+Version: 35.0.2
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```
