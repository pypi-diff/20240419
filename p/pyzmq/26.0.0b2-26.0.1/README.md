# Comparing `tmp/pyzmq-26.0.0b2.tar.gz` & `tmp/pyzmq-26.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzmq-26.0.0b2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pyzmq-26.0.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pyzmq-26.0.0b2.tar` & `pyzmq-26.0.1.tar`

### file list

```diff
@@ -1,284 +1,286 @@
--rw-r--r--   0        0        0     1853 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.circleci/config.yml
--rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.coveragerc
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.flake8
--rw-r--r--   0        0        0     2697 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/dependabot.yml
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/workflows/test-docs.yml
--rw-r--r--   0        0        0     5095 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/workflows/test.yml
--rw-r--r--   0        0        0     6029 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.github/workflows/wheels.yml
--rw-r--r--   0        0        0      552 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.gitignore
--rw-r--r--   0        0        0      733 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.mailmap
--rw-r--r--   0        0        0      128 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.obs/workflows.yml
--rw-r--r--   0        0        0     2067 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.prettierignore
--rw-r--r--   0        0        0      337 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/.readthedocs.yml
--rw-r--r--   0        0        0     4810 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/AUTHORS.md
--rw-r--r--   0        0        0    13427 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/CMakeLists.txt
--rw-r--r--   0        0        0     2251 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1545 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/LICENSE.md
--rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/MANIFEST.in
--rw-r--r--   0        0        0     2964 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/README.md
--rw-r--r--   0        0        0     2116 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/README.md
--rw-r--r--   0        0        0     2751 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/authors.py
--rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/chrislaws.md
--rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/ellisonbg.md
--rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/frankwiles.md
--rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/juliantaylor.md
--rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/ledgerx.md
--rw-r--r--   0        0        0      731 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/lothiraldan.md
--rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/minrk.md
--rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/takluyver.md
--rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-bsd.txt
--rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-mplv2-any-osi.txt
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-mplv2.txt
--rw-r--r--   0        0        0     1541 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/SECURITY.md
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/Vagrantfile
--rw-r--r--   0        0        0      692 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/buildutils/build_cffi.py
--rw-r--r--   0        0        0      437 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/buildutils/bundle.py
--rw-r--r--   0        0        0     3634 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/buildutils/constants.py
--rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/buildutils/templates/constant_enums.pxi
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/buildutils/templates/constants.py
--rw-r--r--   0        0        0    11525 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/cmake/FindVcvars.cmake
--rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/cmake/Findsodium.cmake
--rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/codecov.yml
--rw-r--r--   0        0        0     3639 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/Makefile
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/requirements.txt
--rw-r--r--   0        0        0     8686 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/_static/logo.png
--rw-r--r--   0        0        0     1150 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/_static/zeromq.ico
--rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/index.md
--rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.asyncio.md
--rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.auth.asyncio.md
--rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.auth.ioloop.md
--rw-r--r--   0        0        0      420 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.auth.md
--rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.auth.thread.md
--rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.decorators.md
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.devices.md
--rw-r--r--   0        0        0     1807 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.eventloop.future.md
--rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.eventloop.ioloop.md
--rw-r--r--   0        0        0      330 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.eventloop.zmqstream.md
--rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.green.md
--rw-r--r--   0        0        0      442 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.log.handlers.md
--rw-r--r--   0        0        0     4381 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.md
--rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.ssh.tunnel.md
--rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.utils.jsonapi.md
--rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.utils.monitor.md
--rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.utils.win32.md
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/api/zmq.utils.z85.md
--rw-r--r--   0        0        0    41718 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/changelog.md
--rw-r--r--   0        0        0     8271 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/conf.py
--rw-r--r--   0        0        0    10786 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/build.md
--rw-r--r--   0        0        0     3980 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/devices.md
--rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/draft.md
--rw-r--r--   0        0        0     5732 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/eventloop.md
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/index.md
--rw-r--r--   0        0        0     9610 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/logging.md
--rw-r--r--   0        0        0     6548 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/morethanbindings.md
--rw-r--r--   0        0        0     3569 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/serialization.md
--rw-r--r--   0        0        0     2877 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/howto/ssh.md
--rw-r--r--   0        0        0     2025 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/docs/source/index.md
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/LICENSE
--rw-r--r--   0        0        0      326 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/README.md
--rw-r--r--   0        0        0     1206 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/asyncio/coroutines.py
--rw-r--r--   0        0        0     7089 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/asyncio/helloworld_pubsub_dealerrouter.py
--rw-r--r--   0        0        0     2290 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/asyncio/router_router.py
--rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/asyncio/tornado_asyncio.py
--rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/cython/.gitignore
--rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/cython/README.md
--rw-r--r--   0        0        0     1680 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/cython/cyzmq.pyx
--rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/cython/example.py
--rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/cython/setup.py
--rw-r--r--   0        0        0     1598 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/device/device.py
--rw-r--r--   0        0        0      550 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/draft/client-server.py
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/draft/install.sh
--rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/draft/radio-dish.py
--rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/eventloop/asyncweb.py
--rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/eventloop/coroutines.py
--rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/eventloop/echo.py
--rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/eventloop/echofuture.py
--rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/eventloop/echostream.py
--rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/gevent/poll.py
--rw-r--r--   0        0        0     1109 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/gevent/reqrep.py
--rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/gevent/simple.py
--rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/heartbeat/heart.py
--rw-r--r--   0        0        0     2775 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/heartbeat/heartbeater.py
--rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/heartbeat/ping.py
--rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/heartbeat/pong.py
--rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/logger/zmqlogger.py
--rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/mongodb/client.py
--rw-r--r--   0        0        0     3256 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/mongodb/controller.py
--rw-r--r--   0        0        0     2341 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/monitoring/simple_monitor.py
--rw-r--r--   0        0        0     5001 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/monitoring/zmq_monitor_class.py
--rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/poll/pair.py
--rw-r--r--   0        0        0     1401 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/poll/pubsub.py
--rw-r--r--   0        0        0     1767 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/poll/reqrep.py
--rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/pubsub/publisher.py
--rw-r--r--   0        0        0     1849 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/pubsub/subscriber.py
--rwxr-xr-x   0        0        0     2033 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/pubsub/topics_pub.py
--rwxr-xr-x   0        0        0     1773 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/pubsub/topics_sub.py
--rw-r--r--   0        0        0     3746 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/asyncio-ironhouse.py
--rw-r--r--   0        0        0     2007 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/generate_certificates.py
--rw-r--r--   0        0        0      569 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/grasslands.py
--rw-r--r--   0        0        0     4265 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/ioloop-ironhouse.py
--rw-r--r--   0        0        0     3172 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/ironhouse.py
--rw-r--r--   0        0        0     3181 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/stonehouse.py
--rw-r--r--   0        0        0     2215 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/strawhouse.py
--rw-r--r--   0        0        0     2353 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/security/woodhouse.py
--rw-r--r--   0        0        0     2575 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/serialization/serialsocket.py
--rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/examples/win32-interrupt/display.py
--rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/mypy.ini
--rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/mypy_tests/test_context.py
--rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/mypy_tests/test_socket.py
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/mypy_tests/test_toplevel.py
--rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/README.md
--rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/changelog
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/compat
--rw-r--r--   0        0        0     2298 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/control
--rw-r--r--   0        0        0     6045 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/copyright
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/pyzmq.dsc.obs
--rwxr-xr-x   0        0        0     1708 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/rules
--rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/debian/source/format
--rw-r--r--   0        0        0     2338 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/obs/_service
--rw-r--r--   0        0        0     7812 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/packaging/redhat/python-pyzmq.spec
--rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/perf/Dockerfile
--rw-r--r--   0        0        0      707 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/perf/Makefile
--rw-r--r--   0        0        0     4538 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/perf/collect.py
--rw-r--r--   0        0        0   167790 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/perf/perf.ipynb
--rw-r--r--   0        0        0     6333 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/perf/perf.py
--rw-r--r--   0        0        0     4665 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/pytest.ini
--rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/test-requirements.txt
--rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/backend_imports.py
--rw-r--r--   0        0        0     1668 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/collect_cmake.py
--rw-r--r--   0        0        0     1655 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/find_vcredist.py
--rw-r--r--   0        0        0     1959 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/install_libzmq.sh
--rw-r--r--   0        0        0     3786 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/run_with_env.cmd
--rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/showvcvars.py
--rw-r--r--   0        0        0     1521 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/test_sdist.py
--rw-r--r--   0        0        0     1340 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/test_wheel.py
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/tools/wheel-requirements.txt
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/__init__.pxd
--rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/__init__.py
--rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/__init__.pyi
--rw-r--r--   0        0        0    24516 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/_future.py
--rw-r--r--   0        0        0      525 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/_typing.py
--rw-r--r--   0        0        0     6306 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/asyncio.py
--rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/__init__.py
--rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/asyncio.py
--rw-r--r--   0        0        0    16337 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/base.py
--rw-r--r--   0        0        0     4331 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/certs.py
--rw-r--r--   0        0        0     1298 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/ioloop.py
--rw-r--r--   0        0        0     4103 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/auth/thread.py
--rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/__init__.py
--rw-r--r--   0        0        0     3483 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/__init__.pyi
--rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/README.md
--rw-r--r--   0        0        0      833 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/__init__.py
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/_cdefs.h
--rw-r--r--   0        0        0     1314 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/_cffi_src.c
--rw-r--r--   0        0        0     2886 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/_poll.py
--rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/context.py
--rw-r--r--   0        0        0     1572 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/devices.py
--rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/error.py
--rw-r--r--   0        0        0     6488 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/message.py
--rw-r--r--   0        0        0    11450 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/socket.py
--rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cffi/utils.py
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/__init__.pxd
--rw-r--r--   0        0        0      322 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/__init__.py
--rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/_externs.pxd
--rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/_zmq.pxd
--rw-r--r--   0        0        0    57809 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/_zmq.py
--rw-r--r--   0        0        0     7562 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/constant_enums.pxi
--rw-r--r--   0        0        0     4564 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/cython/libzmq.pxd
--rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/backend/select.py
--rw-r--r--   0        0        0    28341 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/constants.py
--rw-r--r--   0        0        0     5112 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/decorators.py
--rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/__init__.py
--rw-r--r--   0        0        0     9581 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/basedevice.py
--rw-r--r--   0        0        0     1294 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/monitoredqueue.py
--rw-r--r--   0        0        0     1930 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/monitoredqueuedevice.py
--rw-r--r--   0        0        0     2849 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/proxydevice.py
--rw-r--r--   0        0        0     3212 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/devices/proxysteerabledevice.py
--rw-r--r--   0        0        0     5368 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/error.py
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/eventloop/__init__.py
--rw-r--r--   0        0        0     6444 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/eventloop/_deprecated.py
--rw-r--r--   0        0        0     2596 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/eventloop/future.py
--rw-r--r--   0        0        0      767 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/eventloop/ioloop.py
--rw-r--r--   0        0        0    23439 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/eventloop/zmqstream.py
--rw-r--r--   0        0        0     1366 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/__init__.py
--rw-r--r--   0        0        0    10836 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/core.py
--rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/device.py
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/eventloop/__init__.py
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/eventloop/ioloop.py
--rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/eventloop/zmqstream.py
--rw-r--r--   0        0        0     2986 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/green/poll.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/log/__init__.py
--rw-r--r--   0        0        0     4008 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/log/__main__.py
--rw-r--r--   0        0        0     7101 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/log/handlers.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/py.typed
--rw-r--r--   0        0        0       29 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/ssh/__init__.py
--rw-r--r--   0        0        0     3358 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/ssh/forward.py
--rw-r--r--   0        0        0    13534 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/ssh/tunnel.py
--rw-r--r--   0        0        0      722 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/__init__.py
--rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/__init__.pyi
--rw-r--r--   0        0        0     2638 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/attrsettr.py
--rw-r--r--   0        0        0    14552 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/context.py
--rw-r--r--   0        0        0     4259 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/frame.py
--rw-r--r--   0        0        0     5752 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/poll.py
--rw-r--r--   0        0        0    34639 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/socket.py
--rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/stopwatch.py
--rw-r--r--   0        0        0     3605 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/tracker.py
--rw-r--r--   0        0        0     1615 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/sugar/version.py
--rw-r--r--   0        0        0     8169 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/__init__.py
--rw-r--r--   0        0        0     5564 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/conftest.py
--rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/cython_ext.pyx
--rw-r--r--   0        0        0     9993 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_asyncio.py
--rw-r--r--   0        0        0    14750 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_auth.py
--rw-r--r--   0        0        0     8945 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_cffi_backend.py
--rw-r--r--   0        0        0      962 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_constants.py
--rw-r--r--   0        0        0    12600 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_context.py
--rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_cython.py
--rw-r--r--   0        0        0     9623 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_decorators.py
--rw-r--r--   0        0        0     6004 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_device.py
--rw-r--r--   0        0        0     1371 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_draft.py
--rw-r--r--   0        0        0     1125 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_error.py
--rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_etc.py
--rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_ext.py
--rw-r--r--   0        0        0    10608 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_future.py
--rw-r--r--   0        0        0     1973 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_imports.py
--rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_includes.py
--rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_ioloop.py
--rw-r--r--   0        0        0     6948 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_log.py
--rw-r--r--   0        0        0    11320 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_message.py
--rw-r--r--   0        0        0     3059 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_monitor.py
--rw-r--r--   0        0        0     8285 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_monqueue.py
--rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_multipart.py
--rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_mypy.py
--rw-r--r--   0        0        0     1232 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_pair.py
--rw-r--r--   0        0        0     7106 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_poll.py
--rw-r--r--   0        0        0     4004 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_proxy_steerable.py
--rw-r--r--   0        0        0     1015 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_pubsub.py
--rw-r--r--   0        0        0     1764 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_reqrep.py
--rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_retry_eintr.py
--rw-r--r--   0        0        0     7805 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_security.py
--rw-r--r--   0        0        0    24126 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_socket.py
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_ssh.py
--rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_version.py
--rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_win32_shim.py
--rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_z85.py
--rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/tests/test_zmqstream.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/__init__.py
--rw-r--r--   0        0        0     7031 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/buffers.pxd
--rw-r--r--   0        0        0     6125 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/garbage.py
--rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/getpid_compat.h
--rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/interop.py
--rw-r--r--   0        0        0      522 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/ipcmaxlen.h
--rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/jsonapi.py
--rw-r--r--   0        0        0     3312 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/monitor.py
--rw-r--r--   0        0        0     1625 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/mutex.h
--rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/pyversion_compat.h
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/strtypes.py
--rw-r--r--   0        0        0     4918 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/win32.py
--rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/z85.py
--rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmq/utils/zmq_compat.h
--rw-r--r--   0        0        0     4103 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/zmqversion.py
--rw-r--r--   0        0        0     6126 2022-11-09 12:37:21.000000 pyzmq-26.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1853 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.circleci/config.yml
+-rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.coveragerc
+-rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.flake8
+-rw-r--r--   0        0        0     2697 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/workflows/test-docs.yml
+-rw-r--r--   0        0        0     5095 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     6029 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0      580 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.gitignore
+-rw-r--r--   0        0        0      733 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.mailmap
+-rw-r--r--   0        0        0      128 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.obs/workflows.yml
+-rw-r--r--   0        0        0     1637 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.prettierignore
+-rw-r--r--   0        0        0      337 2022-11-09 12:37:21.000000 pyzmq-26.0.1/.readthedocs.yml
+-rw-r--r--   0        0        0     4810 2022-11-09 12:37:21.000000 pyzmq-26.0.1/AUTHORS.md
+-rw-r--r--   0        0        0    13745 2022-11-09 12:37:21.000000 pyzmq-26.0.1/CMakeLists.txt
+-rw-r--r--   0        0        0     2251 2022-11-09 12:37:21.000000 pyzmq-26.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1545 2022-11-09 12:37:21.000000 pyzmq-26.0.1/LICENSE.md
+-rw-r--r--   0        0        0      257 2022-11-09 12:37:21.000000 pyzmq-26.0.1/MANIFEST.in
+-rw-r--r--   0        0        0     2964 2022-11-09 12:37:21.000000 pyzmq-26.0.1/README.md
+-rw-r--r--   0        0        0     2116 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/README.md
+-rw-r--r--   0        0        0     2559 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/authors.py
+-rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/chrislaws.md
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/ellisonbg.md
+-rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/frankwiles.md
+-rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/juliantaylor.md
+-rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/ledgerx.md
+-rw-r--r--   0        0        0      731 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/lothiraldan.md
+-rw-r--r--   0        0        0      723 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/minrk.md
+-rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/takluyver.md
+-rw-r--r--   0        0        0      616 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/templates/relicense-template-bsd.txt
+-rw-r--r--   0        0        0      809 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/templates/relicense-template-mplv2-any-osi.txt
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 pyzmq-26.0.1/RELICENSE/templates/relicense-template-mplv2.txt
+-rw-r--r--   0        0        0     1541 2022-11-09 12:37:21.000000 pyzmq-26.0.1/SECURITY.md
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pyzmq-26.0.1/Vagrantfile
+-rw-r--r--   0        0        0      692 2022-11-09 12:37:21.000000 pyzmq-26.0.1/buildutils/build_cffi.py
+-rw-r--r--   0        0        0     1657 2022-11-09 12:37:21.000000 pyzmq-26.0.1/buildutils/bundle.py
+-rw-r--r--   0        0        0     3629 2022-11-09 12:37:21.000000 pyzmq-26.0.1/buildutils/constants.py
+-rw-r--r--   0        0        0      180 2022-11-09 12:37:21.000000 pyzmq-26.0.1/buildutils/templates/constant_enums.pxi
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 pyzmq-26.0.1/buildutils/templates/constants.py
+-rw-r--r--   0        0        0    11525 2022-11-09 12:37:21.000000 pyzmq-26.0.1/cmake/FindVcvars.cmake
+-rw-r--r--   0        0        0     1381 2022-11-09 12:37:21.000000 pyzmq-26.0.1/cmake/Findsodium.cmake
+-rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 pyzmq-26.0.1/codecov.yml
+-rw-r--r--   0        0        0     3639 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/Makefile
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0     8686 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/_static/logo.png
+-rw-r--r--   0        0        0     1150 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/_static/zeromq.ico
+-rw-r--r--   0        0        0      377 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/index.md
+-rw-r--r--   0        0        0     1561 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.asyncio.md
+-rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.auth.asyncio.md
+-rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.auth.ioloop.md
+-rw-r--r--   0        0        0      420 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.auth.md
+-rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.auth.thread.md
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.decorators.md
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.devices.md
+-rw-r--r--   0        0        0     1807 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.eventloop.future.md
+-rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.eventloop.ioloop.md
+-rw-r--r--   0        0        0      330 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.eventloop.zmqstream.md
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.green.md
+-rw-r--r--   0        0        0      442 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.log.handlers.md
+-rw-r--r--   0        0        0     4993 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.md
+-rw-r--r--   0        0        0      471 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.ssh.tunnel.md
+-rw-r--r--   0        0        0      324 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.utils.jsonapi.md
+-rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.utils.monitor.md
+-rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.utils.win32.md
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/api/zmq.utils.z85.md
+-rw-r--r--   0        0        0    42125 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/changelog.md
+-rw-r--r--   0        0        0     8279 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0    12342 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/build.md
+-rw-r--r--   0        0        0     3450 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/cross-android.Dockerfile
+-rw-r--r--   0        0        0     3250 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/cross.Dockerfile
+-rw-r--r--   0        0        0     3980 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/devices.md
+-rw-r--r--   0        0        0     1475 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/draft.md
+-rw-r--r--   0        0        0     5732 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/eventloop.md
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/index.md
+-rw-r--r--   0        0        0     9610 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/logging.md
+-rw-r--r--   0        0        0     6548 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/morethanbindings.md
+-rw-r--r--   0        0        0     3569 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/serialization.md
+-rw-r--r--   0        0        0     2877 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/howto/ssh.md
+-rw-r--r--   0        0        0     2025 2022-11-09 12:37:21.000000 pyzmq-26.0.1/docs/source/index.md
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/LICENSE
+-rw-r--r--   0        0        0      326 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/README.md
+-rw-r--r--   0        0        0     1206 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/asyncio/coroutines.py
+-rw-r--r--   0        0        0     6997 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/asyncio/helloworld_pubsub_dealerrouter.py
+-rw-r--r--   0        0        0     2290 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/asyncio/router_router.py
+-rw-r--r--   0        0        0      813 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/asyncio/tornado_asyncio.py
+-rw-r--r--   0        0        0       11 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/cython/.gitignore
+-rw-r--r--   0        0        0      892 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/cython/README.md
+-rw-r--r--   0        0        0     1680 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/cython/cyzmq.pyx
+-rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/cython/example.py
+-rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/cython/setup.py
+-rw-r--r--   0        0        0     1597 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/device/device.py
+-rw-r--r--   0        0        0      550 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/draft/client-server.py
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/draft/install.sh
+-rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/draft/radio-dish.py
+-rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/eventloop/asyncweb.py
+-rw-r--r--   0        0        0     1388 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/eventloop/coroutines.py
+-rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/eventloop/echo.py
+-rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/eventloop/echofuture.py
+-rw-r--r--   0        0        0      475 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/eventloop/echostream.py
+-rw-r--r--   0        0        0     1154 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/gevent/poll.py
+-rw-r--r--   0        0        0     1109 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/gevent/reqrep.py
+-rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/gevent/simple.py
+-rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/heartbeat/heart.py
+-rw-r--r--   0        0        0     2775 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/heartbeat/heartbeater.py
+-rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/heartbeat/ping.py
+-rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/heartbeat/pong.py
+-rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/logger/zmqlogger.py
+-rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/mongodb/client.py
+-rw-r--r--   0        0        0     3256 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/mongodb/controller.py
+-rw-r--r--   0        0        0     2341 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/monitoring/simple_monitor.py
+-rw-r--r--   0        0        0     5001 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/monitoring/zmq_monitor_class.py
+-rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/poll/pair.py
+-rw-r--r--   0        0        0     1401 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/poll/pubsub.py
+-rw-r--r--   0        0        0     1767 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/poll/reqrep.py
+-rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/pubsub/publisher.py
+-rw-r--r--   0        0        0     1848 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/pubsub/subscriber.py
+-rwxr-xr-x   0        0        0     2033 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/pubsub/topics_pub.py
+-rwxr-xr-x   0        0        0     1773 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/pubsub/topics_sub.py
+-rw-r--r--   0        0        0     3708 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/asyncio-ironhouse.py
+-rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/generate_certificates.py
+-rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/grasslands.py
+-rw-r--r--   0        0        0     4227 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/ioloop-ironhouse.py
+-rw-r--r--   0        0        0     3134 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/ironhouse.py
+-rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/stonehouse.py
+-rw-r--r--   0        0        0     2177 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/strawhouse.py
+-rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/security/woodhouse.py
+-rw-r--r--   0        0        0     2575 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/serialization/serialsocket.py
+-rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 pyzmq-26.0.1/examples/win32-interrupt/display.py
+-rw-r--r--   0        0        0      333 2022-11-09 12:37:21.000000 pyzmq-26.0.1/mypy.ini
+-rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 pyzmq-26.0.1/mypy_tests/test_context.py
+-rw-r--r--   0        0        0      408 2022-11-09 12:37:21.000000 pyzmq-26.0.1/mypy_tests/test_socket.py
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.1/mypy_tests/test_toplevel.py
+-rw-r--r--   0        0        0      218 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/README.md
+-rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/changelog
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/compat
+-rw-r--r--   0        0        0     2298 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/control
+-rw-r--r--   0        0        0     6045 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/copyright
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/pyzmq.dsc.obs
+-rwxr-xr-x   0        0        0     1708 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/rules
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/debian/source/format
+-rw-r--r--   0        0        0     2338 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/obs/_service
+-rw-r--r--   0        0        0     7812 2022-11-09 12:37:21.000000 pyzmq-26.0.1/packaging/redhat/python-pyzmq.spec
+-rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 pyzmq-26.0.1/perf/Dockerfile
+-rw-r--r--   0        0        0      710 2022-11-09 12:37:21.000000 pyzmq-26.0.1/perf/Makefile
+-rw-r--r--   0        0        0     4538 2022-11-09 12:37:21.000000 pyzmq-26.0.1/perf/collect.py
+-rw-r--r--   0        0        0    35487 2022-11-09 12:37:21.000000 pyzmq-26.0.1/perf/perf.ipynb
+-rw-r--r--   0        0        0     6333 2022-11-09 12:37:21.000000 pyzmq-26.0.1/perf/perf.py
+-rw-r--r--   0        0        0     5129 2022-11-09 12:37:21.000000 pyzmq-26.0.1/pyproject.toml
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 pyzmq-26.0.1/pytest.ini
+-rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 pyzmq-26.0.1/test-requirements.txt
+-rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/backend_imports.py
+-rw-r--r--   0        0        0     1668 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/collect_cmake.py
+-rw-r--r--   0        0        0     1655 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/find_vcredist.py
+-rw-r--r--   0        0        0     2154 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/install_libzmq.sh
+-rw-r--r--   0        0        0     3786 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/run_with_env.cmd
+-rw-r--r--   0        0        0      247 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/showvcvars.py
+-rw-r--r--   0        0        0     1521 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/test_sdist.py
+-rw-r--r--   0        0        0     1999 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/test_wheel.py
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 pyzmq-26.0.1/tools/wheel-requirements.txt
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/__init__.pxd
+-rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/__init__.py
+-rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/__init__.pyi
+-rw-r--r--   0        0        0    24919 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/_future.py
+-rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/_typing.py
+-rw-r--r--   0        0        0     6266 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/asyncio.py
+-rw-r--r--   0        0        0      346 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/__init__.py
+-rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/asyncio.py
+-rw-r--r--   0        0        0    16337 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/base.py
+-rw-r--r--   0        0        0     4331 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/certs.py
+-rw-r--r--   0        0        0     1298 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/ioloop.py
+-rw-r--r--   0        0        0     4103 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/auth/thread.py
+-rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/__init__.py
+-rw-r--r--   0        0        0     3379 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/__init__.pyi
+-rw-r--r--   0        0        0       95 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/README.md
+-rw-r--r--   0        0        0      833 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/__init__.py
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/_cdefs.h
+-rw-r--r--   0        0        0     1314 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/_cffi_src.c
+-rw-r--r--   0        0        0     2886 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/_poll.py
+-rw-r--r--   0        0        0     1899 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/context.py
+-rw-r--r--   0        0        0     1572 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/devices.py
+-rw-r--r--   0        0        0      380 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/error.py
+-rw-r--r--   0        0        0     6488 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/message.py
+-rw-r--r--   0        0        0    11427 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/socket.py
+-rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cffi/utils.py
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/__init__.pxd
+-rw-r--r--   0        0        0      322 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/__init__.py
+-rw-r--r--   0        0        0      339 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/_externs.pxd
+-rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/_zmq.pxd
+-rw-r--r--   0        0        0    57647 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/_zmq.py
+-rw-r--r--   0        0        0     7562 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/constant_enums.pxi
+-rw-r--r--   0        0        0     4564 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/cython/libzmq.pxd
+-rw-r--r--   0        0        0      902 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/backend/select.py
+-rw-r--r--   0        0        0    28341 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/constants.py
+-rw-r--r--   0        0        0     5099 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/decorators.py
+-rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/__init__.py
+-rw-r--r--   0        0        0     9580 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/basedevice.py
+-rw-r--r--   0        0        0     1294 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/monitoredqueue.py
+-rw-r--r--   0        0        0     1929 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/monitoredqueuedevice.py
+-rw-r--r--   0        0        0     2849 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/proxydevice.py
+-rw-r--r--   0        0        0     3212 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/devices/proxysteerabledevice.py
+-rw-r--r--   0        0        0     5309 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/error.py
+-rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/eventloop/__init__.py
+-rw-r--r--   0        0        0     6437 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/eventloop/_deprecated.py
+-rw-r--r--   0        0        0     2612 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/eventloop/future.py
+-rw-r--r--   0        0        0      766 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/eventloop/ioloop.py
+-rw-r--r--   0        0        0    23439 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/eventloop/zmqstream.py
+-rw-r--r--   0        0        0     1367 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/__init__.py
+-rw-r--r--   0        0        0    10812 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/core.py
+-rw-r--r--   0        0        0      978 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/device.py
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/eventloop/__init__.py
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/eventloop/ioloop.py
+-rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/eventloop/zmqstream.py
+-rw-r--r--   0        0        0     2996 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/green/poll.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/log/__init__.py
+-rw-r--r--   0        0        0     4005 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/log/__main__.py
+-rw-r--r--   0        0        0     7228 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/log/handlers.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/py.typed
+-rw-r--r--   0        0        0       29 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/ssh/__init__.py
+-rw-r--r--   0        0        0     3280 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/ssh/forward.py
+-rw-r--r--   0        0        0    13533 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/ssh/tunnel.py
+-rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/__init__.py
+-rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/__init__.pyi
+-rw-r--r--   0        0        0     2638 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/attrsettr.py
+-rw-r--r--   0        0        0    14644 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/context.py
+-rw-r--r--   0        0        0     4259 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/frame.py
+-rw-r--r--   0        0        0     5752 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/poll.py
+-rw-r--r--   0        0        0    34703 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/socket.py
+-rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/stopwatch.py
+-rw-r--r--   0        0        0     3605 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/tracker.py
+-rw-r--r--   0        0        0     1613 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/sugar/version.py
+-rw-r--r--   0        0        0     8134 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/__init__.py
+-rw-r--r--   0        0        0     5564 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/conftest.py
+-rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/cython_ext.pyx
+-rw-r--r--   0        0        0     9993 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_asyncio.py
+-rw-r--r--   0        0        0    14750 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_auth.py
+-rw-r--r--   0        0        0     8945 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_cffi_backend.py
+-rw-r--r--   0        0        0      962 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_constants.py
+-rw-r--r--   0        0        0    12600 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_context.py
+-rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_cython.py
+-rw-r--r--   0        0        0     9623 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_decorators.py
+-rw-r--r--   0        0        0     6004 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_device.py
+-rw-r--r--   0        0        0     1371 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_draft.py
+-rw-r--r--   0        0        0     1125 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_error.py
+-rw-r--r--   0        0        0      533 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_etc.py
+-rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_ext.py
+-rw-r--r--   0        0        0    10608 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_future.py
+-rw-r--r--   0        0        0     1973 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_imports.py
+-rw-r--r--   0        0        0      883 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_includes.py
+-rw-r--r--   0        0        0      641 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_ioloop.py
+-rw-r--r--   0        0        0     6948 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_log.py
+-rw-r--r--   0        0        0    11320 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_message.py
+-rw-r--r--   0        0        0     3059 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_monitor.py
+-rw-r--r--   0        0        0     8285 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_monqueue.py
+-rw-r--r--   0        0        0      852 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_multipart.py
+-rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_mypy.py
+-rw-r--r--   0        0        0     1232 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_pair.py
+-rw-r--r--   0        0        0     7106 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_poll.py
+-rw-r--r--   0        0        0     4004 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_proxy_steerable.py
+-rw-r--r--   0        0        0     1015 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_pubsub.py
+-rw-r--r--   0        0        0     1764 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_reqrep.py
+-rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_retry_eintr.py
+-rw-r--r--   0        0        0     7792 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_security.py
+-rw-r--r--   0        0        0    24126 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_socket.py
+-rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_ssh.py
+-rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_version.py
+-rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_win32_shim.py
+-rw-r--r--   0        0        0     2108 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_z85.py
+-rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/tests/test_zmqstream.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/__init__.py
+-rw-r--r--   0        0        0     7031 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/buffers.pxd
+-rw-r--r--   0        0        0     6124 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/garbage.py
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/getpid_compat.h
+-rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/interop.py
+-rw-r--r--   0        0        0      522 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/ipcmaxlen.h
+-rw-r--r--   0        0        0     1025 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/jsonapi.py
+-rw-r--r--   0        0        0     3312 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/monitor.py
+-rw-r--r--   0        0        0     1625 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/mutex.h
+-rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/pyversion_compat.h
+-rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/strtypes.py
+-rw-r--r--   0        0        0     4940 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/win32.py
+-rw-r--r--   0        0        0     1841 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/z85.py
+-rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmq/utils/zmq_compat.h
+-rw-r--r--   0        0        0     4042 2022-11-09 12:37:21.000000 pyzmq-26.0.1/zmqversion.py
+-rw-r--r--   0        0        0     6124 2022-11-09 12:37:21.000000 pyzmq-26.0.1/PKG-INFO
```

### Comparing `pyzmq-26.0.0b2/.circleci/config.yml` & `pyzmq-26.0.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/.github/ISSUE_TEMPLATE/bug.yml` & `pyzmq-26.0.1/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/.github/ISSUE_TEMPLATE/config.yml` & `pyzmq-26.0.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/.github/workflows/test-docs.yml` & `pyzmq-26.0.1/.github/workflows/test-docs.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/.github/workflows/test.yml` & `pyzmq-26.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/.github/workflows/wheels.yml` & `pyzmq-26.0.1/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/.gitignore` & `pyzmq-26.0.1/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -43,7 +43,9 @@
 
 CMakeFiles
 CMakeCache.txt
 cmake_install.cmake
 _deps
 /Makefile
 _src
+licenses
+.virtual_documents
```

### Comparing `pyzmq-26.0.0b2/.mailmap` & `pyzmq-26.0.1/.mailmap`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/.pre-commit-config.yaml` & `pyzmq-26.0.1/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -9,72 +9,54 @@
         name: constants
         files: "^.*/constants.py"
         description: Generate constants files
         entry: python -m buildutils.constants
         language: python
         pass_filenames: false
         additional_dependencies:
-          - black
+          - ruff
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17  # Use the ref you want to point at
     hooks:
       - id: mdformat
         # Optionally add plugins
         additional_dependencies:
           - mdformat-black
           - mdformat-myst
         exclude: LICENSE.md
 
-  - repo: https://github.com/PyCQA/autoflake
-    rev: v2.2.1
-    hooks:
-      - id: autoflake
-        args:
-          - --in-place
-        exclude: zmq/tests/test_imports.py
+  # autoformat and lint Python code
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.2
+    hooks:
+      - id: ruff
+        types_or:
+          - python
+          - jupyter
+          - pyi
+        args: ["--fix", "--show-fixes"]
+      - id: ruff-format
+        types_or:
+          - python
+          - jupyter
+          - pyi
+        # don't format zmq/constants.py twice
+        exclude: zmq/constants.py
 
-  - repo: https://github.com/PyCQA/flake8
-    rev: 7.0.0
-    hooks:
-      - id: flake8
-        exclude: ^buildutils/templates/
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         files: zmq/.*
         # mypy gets the wrong results
         # if we pass specific files instead of the zmq dir
         # no idea why
         pass_filenames: false
         args: [zmq]
         additional_dependencies:
           - types-paramiko
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
-    hooks:
-      - id: pyupgrade
-        args:
-          - --py36-plus
-  - repo: https://github.com/pycqa/isort
-    rev: 5.13.2
-    hooks:
-      - id: isort
-        name: isort (python)
-      - id: isort
-        name: isort (cython)
-        types: [cython]
-      - id: isort
-        name: isort (pyi)
-        types: [pyi]
-  - repo: https://github.com/psf/black
-    rev: 24.1.1
-    hooks:
-      - id: black
-        # don't run black twice on constants.py
-        exclude: zmq/constants.py
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
       - id: end-of-file-fixer
       - id: check-executables-have-shebangs
       - id: requirements-txt-fixer
```

### Comparing `pyzmq-26.0.0b2/AUTHORS.md` & `pyzmq-26.0.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/CMakeLists.txt` & `pyzmq-26.0.1/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -170,27 +170,31 @@
   include(FetchContent)
   add_compile_definitions(ZMQ_STATIC=1)
   set(BUNDLE_DIR "${CMAKE_CURRENT_BINARY_DIR}/bundled")
   file(MAKE_DIRECTORY "${BUNDLE_DIR}/lib")
   include_directories(${BUNDLE_DIR}/include)
   list(PREPEND CMAKE_PREFIX_PATH ${BUNDLE_DIR})
 
+  set(LICENSE_DIR "${CMAKE_CURRENT_SOURCE_DIR}/licenses")
+  file(MAKE_DIRECTORY "${LICENSE_DIR}")
+
   # libsodium
 
   if (MSVC)
     set(libsodium_lib "${BUNDLE_DIR}/lib/libsodium.lib")
   else()
     set(libsodium_lib "${BUNDLE_DIR}/lib/libsodium.a")
   endif()
 
   FetchContent_Declare(bundled_libsodium
     URL ${PYZMQ_LIBSODIUM_URL}
     PREFIX ${BUNDLE_DIR}
   )
   FetchContent_MakeAvailable(bundled_libsodium)
+  configure_file("${bundled_libsodium_SOURCE_DIR}/LICENSE" "${LICENSE_DIR}/LICENSE.libsodium.txt" COPYONLY)
   # run libsodium build explicitly here, so it's available to libzmq next
   set(bundled_libsodium_include "${bundled_libsodium_SOURCE_DIR}/src/libsodium/include")
 
   if(${bundled_libsodium_POPULATED} AND NOT EXISTS "${libsodium_lib}")
     message(STATUS "building bundled libsodium")
     if (MSVC)
       # select vs build solution by msvc version number
@@ -229,15 +233,15 @@
         RESULT_VARIABLE _status
       )
       if (_status) 
         message(FATAL_ERROR "failed to build libsodium")
       endif()
       file(GLOB_RECURSE BUILT_LIB "${bundled_libsodium_SOURCE_DIR}/**/libsodium.lib")
       message(STATUS "copy ${BUILT_LIB} ${libsodium_lib}")
-      file(COPY_FILE ${BUILT_LIB} ${libsodium_lib})
+      configure_file(${BUILT_LIB} ${libsodium_lib} COPYONLY)
     else()
       list(APPEND libsodium_configure
         ./configure
         --prefix=${BUNDLE_DIR}
         --with-pic
         --disable-dependency-tracking
         --disable-shared
@@ -313,14 +317,15 @@
   endif()
 
   FetchContent_Declare(bundled_libzmq
     URL ${PYZMQ_LIBZMQ_URL}
     PREFIX ${BUNDLE_DIR}
   )
   FetchContent_MakeAvailable(bundled_libzmq)
+  configure_file("${bundled_libzmq_SOURCE_DIR}/LICENSE" "${LICENSE_DIR}/LICENSE.zeromq.txt" COPYONLY)
 
   # target for libzmq static
   if (TARGET libzmq-static)
     set(libzmq_target "libzmq-static")
   else()
     message(FATAL_ERROR "libzmq-static target not found in bundled libzmq")
   endif()
```

### Comparing `pyzmq-26.0.0b2/CONTRIBUTING.md` & `pyzmq-26.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/LICENSE.md` & `pyzmq-26.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/README.md` & `pyzmq-26.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/README.md` & `pyzmq-26.0.1/RELICENSE/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/authors.py` & `pyzmq-26.0.1/RELICENSE/authors.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,19 +78,9 @@
 for email, commits in sorted(author_commits.items(), key=sort_key, reverse=True):
     if len(commits) <= 2:
         msg = '{} ({})'.format(
             ' '.join(c.hexsha[:12] for c in commits),
             commits[0].authored_datetime.year,
         )
     else:
-        msg = "{commits} commits ({start}-{end})".format(
-            commits=len(commits),
-            start=commits[-1].authored_datetime.year,
-            end=commits[0].authored_datetime.year,
-        )
-    print(
-        "- [ ] {name} {email}: {msg}".format(
-            name=email_names[email],
-            email=email,
-            msg=msg,
-        )
-    )
+        msg = f"{len(commits)} commits ({commits[-1].authored_datetime.year}-{commits[0].authored_datetime.year})"
+    print(f"- [ ] {email_names[email]} {email}: {msg}")
```

### Comparing `pyzmq-26.0.0b2/RELICENSE/chrislaws.md` & `pyzmq-26.0.1/RELICENSE/chrislaws.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/ellisonbg.md` & `pyzmq-26.0.1/RELICENSE/ellisonbg.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/frankwiles.md` & `pyzmq-26.0.1/RELICENSE/frankwiles.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/juliantaylor.md` & `pyzmq-26.0.1/RELICENSE/juliantaylor.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/ledgerx.md` & `pyzmq-26.0.1/RELICENSE/ledgerx.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/lothiraldan.md` & `pyzmq-26.0.1/RELICENSE/lothiraldan.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/minrk.md` & `pyzmq-26.0.1/RELICENSE/minrk.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/takluyver.md` & `pyzmq-26.0.1/RELICENSE/takluyver.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-bsd.txt` & `pyzmq-26.0.1/RELICENSE/templates/relicense-template-bsd.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-mplv2-any-osi.txt` & `pyzmq-26.0.1/RELICENSE/templates/relicense-template-mplv2-any-osi.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/RELICENSE/templates/relicense-template-mplv2.txt` & `pyzmq-26.0.1/RELICENSE/templates/relicense-template-mplv2.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/SECURITY.md` & `pyzmq-26.0.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/Vagrantfile` & `pyzmq-26.0.1/Vagrantfile`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/buildutils/build_cffi.py` & `pyzmq-26.0.1/buildutils/build_cffi.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/buildutils/constants.py` & `pyzmq-26.0.1/buildutils/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 pjoin = os.path.join
 
 buildutils = os.path.abspath(os.path.dirname(__file__))
 root = pjoin(buildutils, os.path.pardir)
 
 sys.path.insert(0, pjoin(root, 'zmq'))
-import constants
+import constants  # noqa: E402
 
 all_names = []
 for name in constants.__all__:
     item = getattr(constants, name)
     if isinstance(item, enum.Enum):
         all_names.append(name)
 
@@ -45,15 +45,15 @@
 
 
 def cython_enums():
     """generate `enum: ZMQ_CONST` block for constant_enums.pxi"""
     lines = []
     for name in all_names:
         if no_prefix(name):
-            lines.append('enum: ZMQ_{0} "{0}"'.format(name))
+            lines.append(f'enum: ZMQ_{name} "{name}"')
         else:
             lines.append(f'enum: ZMQ_{name}')
 
     return dict(ZMQ_ENUMS='\n    '.join(lines))
 
 
 def ifndefs():
@@ -108,15 +108,15 @@
         tpl = f.read()
     out = tpl.format(**ns_func())
     dest = pjoin(dest_dir, fname)
     print("generating %s from template" % dest)
     with open(dest, 'w') as f:
         f.write(out)
     if fname.endswith(".py"):
-        run([sys.executable, "-m", "black", dest])
+        run(["ruff", "format", dest])
 
 
 def render_constants():
     """render generated constant files from templates"""
     generate_file(
         "constant_enums.pxi", cython_enums, pjoin(root, 'zmq', 'backend', 'cython')
     )
```

### Comparing `pyzmq-26.0.0b2/cmake/FindVcvars.cmake` & `pyzmq-26.0.1/cmake/FindVcvars.cmake`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/cmake/Findsodium.cmake` & `pyzmq-26.0.1/cmake/Findsodium.cmake`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/Makefile` & `pyzmq-26.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/_static/logo.png` & `pyzmq-26.0.1/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/_static/zeromq.ico` & `pyzmq-26.0.1/docs/source/_static/zeromq.ico`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/api/zmq.asyncio.md` & `pyzmq-26.0.1/docs/source/api/zmq.asyncio.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/api/zmq.devices.md` & `pyzmq-26.0.1/docs/source/api/zmq.devices.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/api/zmq.eventloop.future.md` & `pyzmq-26.0.1/docs/source/api/zmq.eventloop.future.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/api/zmq.md` & `pyzmq-26.0.1/docs/source/api/zmq.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,37 @@
 ```
 
 ```{currentmodule} zmq
 ```
 
 ## Basic Classes
 
+````{note}
+For typing purposes, `zmq.Context` and `zmq.Socket` are Generics,
+which means they will accept any Context or Socket implementation.
+
+The base `zmq.Context()` constructor returns the type
+`zmq.Context[zmq.Socket[bytes]]`.
+If you are using type annotations and want to _exclude_ the async subclasses,
+use the resolved types instead of the base Generics:
+
+```python
+ctx: zmq.Context[zmq.Socket[bytes]] = zmq.Context()
+sock: zmq.Socket[bytes]
+```
+
+in pyzmq 26, these are available as the Type Aliases (not actual classes!):
+
+```python
+ctx: zmq.SyncContext = zmq.Context()
+sock: zmq.SyncSocket
+```
+
+````
+
 ### {class}`Context`
 
 ```{eval-rst}
 .. autoclass:: Context
   :members:
   :inherited-members:
   :exclude-members: sockopts, closed, __del__, __enter__, __exit__, __copy__, __deepcopy__, __delattr__, __getattr__, __setattr__,
```

### Comparing `pyzmq-26.0.0b2/docs/source/changelog.md` & `pyzmq-26.0.1/docs/source/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 # Changes in PyZMQ
 
 This is a coarse summary of changes in pyzmq versions.
 For a full changelog, consult the [git log](https://github.com/zeromq/pyzmq/commits).
 
 ## 26
 
+### 26.0.1
+
+- Fix install from source with cmake \< 3.21
+
+### 26.0.0
+
 pyzmq 26 is a small release, but with some big changes _hopefully_ nobody will notice,
 except for some users (especially on Windows) where pyzmq releases did not work.
 
 The highlights are:
 
 - The Cython backend has been rewritten using Cython 3's pure Python mode.
 - The build system has been rewritten to use CMake via [scikit-build-core] instead of setuptools (setup.py is gone!).
@@ -32,14 +38,17 @@
 See [build docs](building-pyzmq) for more info.
 
 __New__:
 
 - Experimental support for wheels on windows-arm64
 - `Socket.bind('tcp://ip:0')` can be used as a context manager to bind to a random port.
   The resulting URL can be retrieved as `socket.last_endpoint`.
+- Add `SyncSocket` and `SyncContext` type aliases for the default Socket/Context implementations,
+  since the base classes are Generics, type-wise.
+  These are type aliases only to be used in type checking, not actual classes.
 
 __Enhancements__:
 
 - `repr(Frame)` now produces a nice repr, summarizing Frame contents (without getting too large),
   e.g. `<zmq.Frame(b'abcdefghijkl'...52B)>`
 
 __Breaking changes__:
@@ -50,14 +59,19 @@
   `bytes(Frame)` remains unchanged, and utf-8 text strings can still be produced with:
   `bytes(Frame).decode("utf8")`,
   which works in all versions of pyzmq and does the same thing.
 - Stop building Python 3.7 wheels for manylinux1, which reached EOL in January, 2022. The new build system doesn't seem to be able to find cmake in that environment.
 
 ## 25
 
+### 25.1.2
+
+- Fix builds with some recent compilers and bundled libzmq
+- Fix builds with upcoming Cython 3.1
+
 ### 25.1.1
 
 25.1.1 is the first stable release with Python 3.12 wheels.
 
 Changes:
 
 - Allow Cython 0.29.35 to build Python 3.12 wheels (no longer require Cython 3)
```

### Comparing `pyzmq-26.0.0b2/docs/source/conf.py` & `pyzmq-26.0.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # add repo root to sys.path for buildutils import
 here = Path(__file__).parent.absolute()
 repo_root = here.parents[1]
 sys.path.append(str(repo_root))
 
 # set target libzmq version
-from buildutils.bundle import bundled_version
+from buildutils.bundle import bundled_version  # noqa
 
 # remove repo root from sys.path
 sys.path = sys.path[:-1]
 
 target_libzmq = bundled_version
 
 # -- General configuration -----------------------------------------------------
```

### Comparing `pyzmq-26.0.0b2/docs/source/howto/build.md` & `pyzmq-26.0.1/docs/source/howto/build.md`

 * *Files 14% similar despite different names*

```diff
@@ -100,14 +100,18 @@
 
 If pyzmq doesn't find a libzmq to link to, it will fall back on building libzmq itself.
 You can tell pyzmq to skip searching for libzmq and always build the bundled version with `ZMQ_PREFIX=bundled`.
 
 When building a bundled libzmq, pyzmq downloads and builds libzmq and libsodium as static libraries.
 These static libraries are then linked to by the pyzmq extension and discarded.
 
+Bundled libzmq is supported on a best-effort basis, and isn't expected to work everywhere with zero configuration.
+If you have trouble building bundled libzmq, please do [report it](https://github.com/zeromq/pyzmq/issues).
+But the best solution is usually to install libzmq yourself via the appropriate mechanism _before_ building pyzmq.
+
 ### Building bundled libsodium
 
 libsodium is built first, with `configure` most places:
 
 ```bash
 ./configure --enable-static --disable-shared --with-pic
 make
@@ -397,9 +401,52 @@
 
 # Output zmq library base name
 ZMQ_OUTPUT_BASENAME:STRING=zmq
 ```
 
 </details>
 
+## Cross-compiling pyzmq
+
+Cross-compiling Python extensions is tricky!
+
+To cross-compile pyzmq, in general you need:
+
+- Python built for the 'build' machine
+- Python built for the 'host' machine (identical version)
+- cross-compiling toolchain (e.g. `aarch64-linux-gnu-gcc`)
+- Python setup to cross-compile ([crossenv] is the popular tool these days, and includes lots of info for cross-compiling for Python, but pyzmq makes no assumptions)
+
+It is probably a good idea to build libzmq/libsodium separately and link them with ZMQ_PREFIX,
+as cross-compiling bundled libzmq is not guaranteed to work.
+
+I don't have a lot of experience cross-compiling,
+but we have two example Dockerfiles that appear to work to cross-compile pyzmq.
+These aren't official or supported, but they appear to work and may be useful as reference to get you started.
+
+<details>
+
+<summary>Dockerfile for building x86_64 on aarch64</summary>
+
+```{literalinclude} cross.Dockerfile
+---
+language: Dockerfile
+---
+```
+
+</details>
+
+<details>
+
+<summary>Dockerfile for building for android-aarch64 on x86_64</summary>
+
+```{literalinclude} cross-android.Dockerfile
+---
+language: Dockerfile
+---
+```
+
+</details>
+
+[crossenv]: https://crossenv.readthedocs.io/
 [fetchcontent]: https://cmake.org/cmake/help/latest/module/FetchContent.html
 [scikit-build-core]: https://scikit-build-core.readthedocs.io
```

### Comparing `pyzmq-26.0.0b2/docs/source/howto/devices.md` & `pyzmq-26.0.1/docs/source/howto/devices.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/howto/draft.md` & `pyzmq-26.0.1/docs/source/howto/draft.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/howto/eventloop.md` & `pyzmq-26.0.1/docs/source/howto/eventloop.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/howto/logging.md` & `pyzmq-26.0.1/docs/source/howto/logging.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/howto/morethanbindings.md` & `pyzmq-26.0.1/docs/source/howto/morethanbindings.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/howto/serialization.md` & `pyzmq-26.0.1/docs/source/howto/serialization.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/howto/ssh.md` & `pyzmq-26.0.1/docs/source/howto/ssh.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/docs/source/index.md` & `pyzmq-26.0.1/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/asyncio/coroutines.py` & `pyzmq-26.0.1/examples/asyncio/coroutines.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/asyncio/helloworld_pubsub_dealerrouter.py` & `pyzmq-26.0.1/examples/asyncio/helloworld_pubsub_dealerrouter.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,19 +191,15 @@
             while True:
                 [id_dealer, msg] = await rout.recv_multipart()
                 print(
                     f"Command rout; Sender ID: {id_dealer!r};\tmessage: {msg.decode()}"
                 )
 
                 self.hello_world.change_language()
-                print(
-                    "Changed language! New language is: {}\n".format(
-                        self.hello_world.lang
-                    )
-                )
+                print(f"Changed language! New language is: {self.hello_world.lang}\n")
 
         except Exception as e:
             print("Error with sub world")
             # print(e)
             logging.error(traceback.format_exc())
             print()
```

### Comparing `pyzmq-26.0.0b2/examples/asyncio/router_router.py` & `pyzmq-26.0.1/examples/asyncio/router_router.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/asyncio/tornado_asyncio.py` & `pyzmq-26.0.1/examples/asyncio/tornado_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/cython/README.md` & `pyzmq-26.0.1/examples/cython/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/cython/cyzmq.pyx` & `pyzmq-26.0.1/examples/cython/cyzmq.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/cython/example.py` & `pyzmq-26.0.1/examples/cython/example.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/device/device.py` & `pyzmq-26.0.1/examples/device/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Demonstrate using zmq.proxy device for message relay"""
 
 # This example is placed in the Public Domain
 # It may also be used under the Creative Commons CC-0 License, (C) PyZMQ Developers
 
-
 import time
 from threading import Thread
 
 import zmq
 
 MSGS = 10
 PRODUCERS = 2
```

### Comparing `pyzmq-26.0.0b2/examples/draft/client-server.py` & `pyzmq-26.0.1/examples/draft/client-server.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/draft/install.sh` & `pyzmq-26.0.1/examples/draft/install.sh`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/draft/radio-dish.py` & `pyzmq-26.0.1/examples/draft/radio-dish.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/eventloop/asyncweb.py` & `pyzmq-26.0.1/examples/eventloop/asyncweb.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/eventloop/coroutines.py` & `pyzmq-26.0.1/examples/eventloop/coroutines.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/eventloop/echo.py` & `pyzmq-26.0.1/examples/eventloop/echo.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/gevent/poll.py` & `pyzmq-26.0.1/examples/gevent/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/gevent/reqrep.py` & `pyzmq-26.0.1/examples/gevent/reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/gevent/simple.py` & `pyzmq-26.0.1/examples/gevent/simple.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/heartbeat/heart.py` & `pyzmq-26.0.1/examples/heartbeat/heart.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/heartbeat/heartbeater.py` & `pyzmq-26.0.1/examples/heartbeat/heartbeater.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/heartbeat/ping.py` & `pyzmq-26.0.1/examples/heartbeat/ping.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/heartbeat/pong.py` & `pyzmq-26.0.1/examples/heartbeat/pong.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/logger/zmqlogger.py` & `pyzmq-26.0.1/examples/logger/zmqlogger.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/mongodb/client.py` & `pyzmq-26.0.1/examples/mongodb/client.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/mongodb/controller.py` & `pyzmq-26.0.1/examples/mongodb/controller.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/monitoring/simple_monitor.py` & `pyzmq-26.0.1/examples/monitoring/simple_monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/monitoring/zmq_monitor_class.py` & `pyzmq-26.0.1/examples/monitoring/zmq_monitor_class.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/poll/pair.py` & `pyzmq-26.0.1/examples/poll/pair.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/poll/pubsub.py` & `pyzmq-26.0.1/examples/poll/pubsub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/poll/reqrep.py` & `pyzmq-26.0.1/examples/poll/reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/pubsub/publisher.py` & `pyzmq-26.0.1/examples/pubsub/publisher.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/pubsub/subscriber.py` & `pyzmq-26.0.1/examples/pubsub/subscriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # -----------------------------------------------------------------------------
 #  Copyright (c) 2010 Brian Granger
 #
 #  Distributed under the terms of the New BSD License.  The full license is in
 #  the file LICENSE.BSD, distributed as part of this software.
 # -----------------------------------------------------------------------------
 
-
 import sys
 import time
 
 import zmq
 
 
 def sync(connect_to: str) -> None:
```

### Comparing `pyzmq-26.0.0b2/examples/pubsub/topics_pub.py` & `pyzmq-26.0.1/examples/pubsub/topics_pub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/pubsub/topics_sub.py` & `pyzmq-26.0.1/examples/pubsub/topics_sub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/security/asyncio-ironhouse.py` & `pyzmq-26.0.1/examples/security/asyncio-ironhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,17 +94,15 @@
     # stop auth task
     auth.stop()
 
 
 if __name__ == '__main__':
     if zmq.zmq_version_info() < (4, 0):
         raise RuntimeError(
-            "Security is not supported in libzmq version < 4.0. libzmq version {}".format(
-                zmq.zmq_version()
-            )
+            f"Security is not supported in libzmq version < 4.0. libzmq version {zmq.zmq_version()}"
         )
 
     if '-v' in sys.argv:
         level = logging.DEBUG
     else:
         level = logging.INFO
```

### Comparing `pyzmq-26.0.0b2/examples/security/generate_certificates.py` & `pyzmq-26.0.1/examples/security/generate_certificates.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,13 +51,11 @@
                 os.path.join(keys_dir, key_file), os.path.join(secret_keys_dir, '.')
             )
 
 
 if __name__ == '__main__':
     if zmq.zmq_version_info() < (4, 0):
         raise RuntimeError(
-            "Security is not supported in libzmq version < 4.0. libzmq version {}".format(
-                zmq.zmq_version()
-            )
+            f"Security is not supported in libzmq version < 4.0. libzmq version {zmq.zmq_version()}"
         )
 
     generate_certificates(os.path.dirname(__file__))
```

### Comparing `pyzmq-26.0.0b2/examples/security/grasslands.py` & `pyzmq-26.0.1/examples/security/grasslands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 
 '''
 No protection at all.
 
-All connections are accepted, there is no authentication, and no privacy. 
+All connections are accepted, there is no authentication, and no privacy.
 
-This is how ZeroMQ always worked until we built security into the wire 
-protocol in early 2013. Internally, it uses a security mechanism called 
+This is how ZeroMQ always worked until we built security into the wire
+protocol in early 2013. Internally, it uses a security mechanism called
 "NULL".
 
 Author: Chris Laws
 '''
 
 import zmq
```

### Comparing `pyzmq-26.0.0b2/examples/security/ioloop-ironhouse.py` & `pyzmq-26.0.1/examples/security/ioloop-ironhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,15 @@
 
     auth.start()
 
 
 if __name__ == '__main__':
     if zmq.zmq_version_info() < (4, 0):
         raise RuntimeError(
-            "Security is not supported in libzmq version < 4.0. libzmq version {}".format(
-                zmq.zmq_version()
-            )
+            f"Security is not supported in libzmq version < 4.0. libzmq version {zmq.zmq_version()}"
         )
 
     if '-v' in sys.argv:
         level = logging.DEBUG
     else:
         level = logging.INFO
```

### Comparing `pyzmq-26.0.0b2/examples/security/ironhouse.py` & `pyzmq-26.0.1/examples/security/ironhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,15 @@
     # stop auth thread
     auth.stop()
 
 
 if __name__ == '__main__':
     if zmq.zmq_version_info() < (4, 0):
         raise RuntimeError(
-            "Security is not supported in libzmq version < 4.0. libzmq version {}".format(
-                zmq.zmq_version()
-            )
+            f"Security is not supported in libzmq version < 4.0. libzmq version {zmq.zmq_version()}"
         )
 
     if '-v' in sys.argv:
         level = logging.DEBUG
     else:
         level = logging.INFO
```

### Comparing `pyzmq-26.0.0b2/examples/security/stonehouse.py` & `pyzmq-26.0.1/examples/security/stonehouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,15 @@
     # stop auth thread
     auth.stop()
 
 
 if __name__ == '__main__':
     if zmq.zmq_version_info() < (4, 0):
         raise RuntimeError(
-            "Security is not supported in libzmq version < 4.0. libzmq version {}".format(
-                zmq.zmq_version()
-            )
+            f"Security is not supported in libzmq version < 4.0. libzmq version {zmq.zmq_version()}"
         )
 
     if '-v' in sys.argv:
         level = logging.DEBUG
     else:
         level = logging.INFO
```

### Comparing `pyzmq-26.0.0b2/examples/security/strawhouse.py` & `pyzmq-26.0.1/examples/security/strawhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,15 @@
     else:
         logging.error("Strawhouse test FAIL")
 
 
 if __name__ == '__main__':
     if zmq.zmq_version_info() < (4, 0):
         raise RuntimeError(
-            "Security is not supported in libzmq version < 4.0. libzmq version {}".format(
-                zmq.zmq_version()
-            )
+            f"Security is not supported in libzmq version < 4.0. libzmq version {zmq.zmq_version()}"
         )
 
     if '-v' in sys.argv:
         level = logging.DEBUG
     else:
         level = logging.INFO
```

### Comparing `pyzmq-26.0.0b2/examples/security/woodhouse.py` & `pyzmq-26.0.1/examples/security/woodhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,15 @@
     else:
         logging.error("Woodhouse test FAIL")
 
 
 if __name__ == '__main__':
     if zmq.zmq_version_info() < (4, 0):
         raise RuntimeError(
-            "Security is not supported in libzmq version < 4.0. libzmq version {}".format(
-                zmq.zmq_version()
-            )
+            f"Security is not supported in libzmq version < 4.0. libzmq version {zmq.zmq_version()}"
         )
 
     if '-v' in sys.argv:
         level = logging.DEBUG
     else:
         level = logging.INFO
```

### Comparing `pyzmq-26.0.0b2/examples/serialization/serialsocket.py` & `pyzmq-26.0.1/examples/serialization/serialsocket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/examples/win32-interrupt/display.py` & `pyzmq-26.0.1/examples/win32-interrupt/display.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/packaging/debian/control` & `pyzmq-26.0.1/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/packaging/debian/copyright` & `pyzmq-26.0.1/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/packaging/debian/pyzmq.dsc.obs` & `pyzmq-26.0.1/packaging/debian/pyzmq.dsc.obs`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/packaging/debian/rules` & `pyzmq-26.0.1/packaging/debian/rules`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/packaging/obs/_service` & `pyzmq-26.0.1/packaging/obs/_service`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/packaging/redhat/python-pyzmq.spec` & `pyzmq-26.0.1/packaging/redhat/python-pyzmq.spec`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/perf/Makefile` & `pyzmq-26.0.1/perf/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-BASE_IMAGE=python:3.6
+BASE_IMAGE=python:3.11
 IMAGE=pyzmq-perf
 VOLUME=pyzmq-perf
 
-ifeq ($(DOCKER_MACHINE_NAME), "")
+ifeq ("$(DOCKER_MACHINE_NAME)", "")
 	OUT_PATH=$(PWD)
 	FETCH=true
 else
 	OUT_PATH=/tmp/data
 	FETCH=docker-machine scp $(DOCKER_MACHINE_NAME):$(OUT_PATH)/*.pickle ./
 endif
```

### Comparing `pyzmq-26.0.0b2/perf/collect.py` & `pyzmq-26.0.1/perf/collect.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/perf/perf.py` & `pyzmq-26.0.1/perf/perf.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/pyproject.toml` & `pyzmq-26.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # build-backend = "setuptools.build_meta"
 
 # Project metadata
 # ref: https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "pyzmq"
-version = "26.0.0b2"
+version = "26.0.1"
 authors = [
   { name = "PyZMQ Contributors", email = "zeromq-dev@lists.zeromq.org" },
   { name = "Brian E. Granger" },
   { name = "Min Ragan-Kelley" },
 ]
 license = { file = "LICENSE.md" }
 requires-python = ">=3.7"
@@ -49,55 +49,79 @@
 
 [project.urls]
 Homepage = "https://pyzmq.readthedocs.org"
 Documentation = "https://pyzmq.readthedocs.org"
 Source = "https://github.com/zeromq/pyzmq"
 Tracker = "https://github.com/zeromq/pyzmq/issues"
 
-[tool.meson-python.args]
-# avoid installing static libzmq
-install = ['--tags=runtime,python-runtime']
-
-[tool.setuptools]
-zip-safe = false
-license-files = ["LICENSE.md", "bundled/zeromq/COPYING", "bundled/zeromq/COPYING.LESSER"]
-packages = ["zmq"]
-
-[tool.setuptools.dynamic]
-readme = { file = "README.md" }
-
 [tool.scikit-build]
 wheel.packages = ["zmq"]
+wheel.license-files = ["licenses/LICENSE*"]
 # 3.14 for FetchContent_MakeAvailable
 cmake.version = ">=3.14"
 # only build/install the pyzmq component
 cmake.targets = ["pyzmq"]
 install.components = ["pyzmq"]
 
+[tool.ruff]
+
+[tool.ruff.format]
+exclude = [
+    "buildutils/templates/*",
+    "zmq/eventloop/minitornado/*",
+]
+quote-style = "preserve"
+
+[tool.ruff.lint]
+select = [
+    "E",
+    "F",
+    "UP",
+    "I",
+]
+ignore = [
+    "E501", # line length (formatter is responsible)
+    "E721", # compare types
+    "F841", # unused variables
+]
+ignore-init-module-imports = true
+exclude = ["buildutils/templates/*"]
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = ["F4", "E4"]
+"__init__.pyi" = ["F4", "E4"]
+"zmq/tests/*" = ["E4", "F4"]
+"docs/source/conf.py" = ["E4"]
+"zmq/eventloop/*" = ["E402"]
+"zmq/ssh/forward.py" = ["E"]
+
+# no longer used autoformatters, linters:
+
 [tool.autoflake]
 ignore-init-module-imports = true
 remove-all-unused-imports = true
 remove-duplicate-keys = true
 
 # remove-unused-variables = true
+
 [tool.black]
 skip-string-normalization = true
 exclude = "zmq/eventloop/minitornado|docs/source/conf.py"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 skip = ["zmq/__init__.py"]
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/zeromq/pyzmq"
 
 [tool.tbump.version]
-current = "26.0.0b2"
+current = "26.0.1"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?P<pre>((a|b|rc|)\d+)|.dev\d*|)
@@ -116,15 +140,15 @@
 
 [[tool.tbump.file]]
 src = "zmq/sugar/version.py"
 search = '__version__: str = "{current_version}"'
 
 [tool.cibuildwheel]
 build-verbosity = "1"
-test-requires = ["pytest"]
+test-requires = ["pytest", "importlib_metadata"]
 test-command = "pytest -vsx {package}/tools/test_wheel.py"
 
 [tool.cibuildwheel.linux]
 before-all = "bash tools/install_libzmq.sh"
 manylinux-x86_64-image = "manylinux2014"
 manylinux-i686-image = "manylinux2014"
 manylinux-aarch64-image = "manylinux2014"
@@ -141,14 +165,15 @@
 before-all = "bash tools/install_libzmq.sh"
 
 [tool.cibuildwheel.macos.environment]
 ZMQ_PREFIX = "/tmp/zmq"
 MACOSX_DEPLOYMENT_TARGET = "10.9"
 
 [tool.cibuildwheel.windows]
+before-all = "python buildutils/bundle.py licenses"
 repair-wheel-command = """\
     delvewheel repair \
         -v \
         --wheel-dir={dest_dir} \
         {wheel} \
 """
```

### Comparing `pyzmq-26.0.0b2/test-requirements.txt` & `pyzmq-26.0.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/tools/collect_cmake.py` & `pyzmq-26.0.1/tools/collect_cmake.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/tools/find_vcredist.py` & `pyzmq-26.0.1/tools/find_vcredist.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/tools/install_libzmq.sh` & `pyzmq-26.0.1/tools/install_libzmq.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #!/usr/bin/env bash
 # script to install libzmq/libsodium for use in wheels
 set -ex
 LIBSODIUM_VERSION=$(python buildutils/bundle.py libsodium)
 LIBZMQ_VERSION=$(python buildutils/bundle.py)
+PYZMQ_DIR="$PWD"
+LICENSE_DIR="$PYZMQ_DIR/licenses"
+test -d "$LICENSE_DIR" || mkdir "$LICENSE_DIR"
 
 if [[ "$(uname)" == "Darwin" ]]; then
     # need LT_MULTI_MODULE or libtool will strip out
     # all multi-arch symbols at the last step
     export LT_MULTI_MODULE=1
     ARCHS="x86_64"
     case "${CIBW_ARCHS_MACOS:-${CIBW_ARCHS:-auto}}" in
@@ -41,27 +44,29 @@
 
 curl -L -O "https://download.libsodium.org/libsodium/releases/libsodium-${LIBSODIUM_VERSION}.tar.gz"
 
 curl -L -O "https://github.com/zeromq/libzmq/releases/download/v${LIBZMQ_VERSION}/zeromq-${LIBZMQ_VERSION}.tar.gz"
 
 tar -xzf libsodium-${LIBSODIUM_VERSION}.tar.gz
 cd libsodium-*/
+cp LICENSE "${LICENSE_DIR}/LICENSE.libsodium.txt"
 ./configure --prefix="$PREFIX"
 make -j4
 make install
 
 cd ..
 
 which ldconfig && ldconfig || true
 
 # make sure to find our libsodium
 export PKG_CONFIG_PATH=$PREFIX/lib/pkgconfig
 
 tar -xzf zeromq-${LIBZMQ_VERSION}.tar.gz
 cd zeromq-${LIBZMQ_VERSION}
+cp LICENSE "${LICENSE_DIR}/LICENSE.zeromq.txt"
 # avoid error on warning
 export CXXFLAGS="-Wno-error ${CXXFLAGS:-}"
 
 ./configure --prefix="$PREFIX" --disable-perf --without-docs --enable-curve --with-libsodium --disable-drafts --disable-libsodium_randombytes_close
 make -j4
 make install
```

### Comparing `pyzmq-26.0.0b2/tools/run_with_env.cmd` & `pyzmq-26.0.1/tools/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/tools/test_sdist.py` & `pyzmq-26.0.1/tools/test_sdist.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/__init__.py` & `pyzmq-26.0.1/zmq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/__init__.pyi` & `pyzmq-26.0.1/zmq/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,9 +21,9 @@
 from .backend import strerror as strerror
 from .backend import zmq_errno as zmq_errno
 from .backend import zmq_poll as zmq_poll
 from .constants import *
 from .error import *
 from .sugar import *
 
-def get_includes() -> List[str]: ...
-def get_library_dirs() -> List[str]: ...
+def get_includes() -> list[str]: ...
+def get_library_dirs() -> list[str]: ...
```

### Comparing `pyzmq-26.0.0b2/zmq/_future.py` & `pyzmq-26.0.1/zmq/_future.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,27 @@
 
         Returns a Future whose result will be a multipart message.
         """
         return self._add_recv_event(
             'recv_multipart', dict(flags=flags, copy=copy, track=track)
         )
 
+    @overload  # type: ignore
+    def recv(self, flags: int = 0, *, track: bool = False) -> Awaitable[bytes]: ...
+
+    @overload
+    def recv(
+        self, flags: int = 0, *, copy: Literal[True], track: bool = False
+    ) -> Awaitable[bytes]: ...
+
+    @overload
+    def recv(
+        self, flags: int = 0, *, copy: Literal[False], track: bool = False
+    ) -> Awaitable[_zmq.Frame]: ...
+
     def recv(  # type: ignore
         self, flags: int = 0, copy: bool = True, track: bool = False
     ) -> Awaitable[bytes | _zmq.Frame]:
         """Receive a single zmq frame.
 
         Returns a Future, whose result will be the received frame.
 
@@ -427,15 +440,17 @@
 
         return future
 
     # overrides only necessary for updated types
     def recv_string(self, *args, **kwargs) -> Awaitable[str]:  # type: ignore
         return super().recv_string(*args, **kwargs)  # type: ignore
 
-    def send_string(self, s: str, flags: int = 0, encoding: str = 'utf-8') -> Awaitable[None]:  # type: ignore
+    def send_string(  # type: ignore
+        self, s: str, flags: int = 0, encoding: str = 'utf-8'
+    ) -> Awaitable[None]:
         return super().send_string(s, flags=flags, encoding=encoding)  # type: ignore
 
     def _add_timeout(self, future, timeout):
         """Add a timeout for a send or recv Future"""
 
         def future_timeout():
             if future.done():
```

### Comparing `pyzmq-26.0.0b2/zmq/_typing.py` & `pyzmq-26.0.1/zmq/_typing.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,7 +15,16 @@
             def __getitem__(self, key):
                 return Any
 
         Literal = _Literal()  # type: ignore
 
         class TypedDict(Dict):  # type: ignore
             pass
+
+
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias
+else:
+    try:
+        from typing_extensions import TypeAlias
+    except ImportError:
+        TypeAlias = type  # type: ignore
```

### Comparing `pyzmq-26.0.0b2/zmq/asyncio.py` & `pyzmq-26.0.1/zmq/asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,16 @@
     """
 
     if asyncio_loop in _selectors:
         return _selectors[asyncio_loop]
 
     # detect add_reader instead of checking for proactor?
     if hasattr(asyncio, "ProactorEventLoop") and isinstance(
-        asyncio_loop, asyncio.ProactorEventLoop  # type: ignore
+        asyncio_loop,
+        asyncio.ProactorEventLoop,  # type: ignore
     ):
         try:
             from tornado.platform.asyncio import AddThreadSelectorEventLoop
         except ImportError:
             raise RuntimeError(
                 "Proactor event loop does not implement add_reader family of methods required for zmq."
                 " zmq will work with proactor if tornado >= 6.1 can be found."
@@ -62,15 +63,17 @@
             " Use `asyncio.set_event_loop_policy(WindowsSelectorEventLoopPolicy())`"
             " to avoid this warning.",
             RuntimeWarning,
             # stacklevel 5 matches most likely zmq.asyncio.Context().socket()
             stacklevel=5,
         )
 
-        selector_loop = _selectors[asyncio_loop] = AddThreadSelectorEventLoop(asyncio_loop)  # type: ignore
+        selector_loop = _selectors[asyncio_loop] = AddThreadSelectorEventLoop(
+            asyncio_loop
+        )  # type: ignore
 
         # patch loop.close to also close the selector thread
         loop_close = asyncio_loop.close
 
         def _close_selector_and_loop():
             # restore original before calling selector.close,
             # which in turn calls eventloop.close!
@@ -97,23 +100,22 @@
 
 class _AsyncIO:
     _Future = Future
     _WRITE = selectors.EVENT_WRITE
     _READ = selectors.EVENT_READ
 
     def _default_loop(self):
-        if sys.version_info >= (3, 7):
-            try:
-                return asyncio.get_running_loop()
-            except RuntimeError:
-                warnings.warn(
-                    "No running event loop. zmq.asyncio should be used from within an asyncio loop.",
-                    RuntimeWarning,
-                    stacklevel=4,
-                )
+        try:
+            return asyncio.get_running_loop()
+        except RuntimeError:
+            warnings.warn(
+                "No running event loop. zmq.asyncio should be used from within an asyncio loop.",
+                RuntimeWarning,
+                stacklevel=4,
+            )
         # get_event_loop deprecated in 3.10:
         return asyncio.get_event_loop()
 
 
 class Poller(_AsyncIO, _future._AsyncPoller):
     """Poller returning asyncio.Future for poll results."""
```

### Comparing `pyzmq-26.0.0b2/zmq/auth/asyncio.py` & `pyzmq-26.0.1/zmq/auth/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/auth/base.py` & `pyzmq-26.0.1/zmq/auth/base.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/auth/certs.py` & `pyzmq-26.0.1/zmq/auth/certs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """0MQ authentication related functions and classes."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
-
 import datetime
 import glob
 import os
 from typing import Dict, Optional, Tuple, Union
 
 import zmq
 
@@ -84,15 +83,15 @@
         metadata=metadata,
     )
 
     return public_key_file, secret_key_file
 
 
 def load_certificate(
-    filename: Union[str, os.PathLike]
+    filename: Union[str, os.PathLike],
 ) -> Tuple[bytes, Optional[bytes]]:
     """Load public and secret key from a zmq certificate.
 
     Returns (public_key, secret_key)
 
     If the certificate file only contains the public key,
     secret_key will be None.
```

### Comparing `pyzmq-26.0.0b2/zmq/auth/ioloop.py` & `pyzmq-26.0.1/zmq/auth/ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/auth/thread.py` & `pyzmq-26.0.1/zmq/auth/thread.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/__init__.py` & `pyzmq-26.0.1/zmq/backend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Import basic exposure of libzmq C API as a backend"""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
-
 import os
 import platform
 
 from .select import public_api, select_backend
 
 if 'PYZMQ_BACKEND' in os.environ:
     backend = os.environ['PYZMQ_BACKEND']
```

### Comparing `pyzmq-26.0.0b2/zmq/backend/cffi/__init__.py` & `pyzmq-26.0.1/zmq/backend/cffi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/cffi/_cdefs.h` & `pyzmq-26.0.1/zmq/backend/cffi/_cdefs.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/cffi/_cffi_src.c` & `pyzmq-26.0.1/zmq/backend/cffi/_cffi_src.c`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/cffi/_poll.py` & `pyzmq-26.0.1/zmq/backend/cffi/_poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/cffi/context.py` & `pyzmq-26.0.1/zmq/backend/cffi/context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/cffi/devices.py` & `pyzmq-26.0.1/zmq/backend/cffi/devices.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/cffi/message.py` & `pyzmq-26.0.1/zmq/backend/cffi/message.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/cffi/socket.py` & `pyzmq-26.0.1/zmq/backend/cffi/socket.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,61 @@
 """zmq Socket class"""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
 import errno as errno_mod
 
+import zmq
+from zmq.constants import SocketOption, _OptType
+from zmq.error import ZMQError, _check_rc, _check_version
+
 from ._cffi import ffi
 from ._cffi import lib as C
+from .message import Frame
+from .utils import _retry_sys_call
 
 nsp = new_sizet_pointer = lambda length: ffi.new('size_t*', length)
 
-new_uint64_pointer = lambda: (ffi.new('uint64_t*'), nsp(ffi.sizeof('uint64_t')))
-new_int64_pointer = lambda: (ffi.new('int64_t*'), nsp(ffi.sizeof('int64_t')))
-new_int_pointer = lambda: (ffi.new('int*'), nsp(ffi.sizeof('int')))
-new_binary_data = lambda length: (
-    ffi.new('char[%d]' % (length)),
-    nsp(ffi.sizeof('char') * length),
-)
-
-value_uint64_pointer = lambda val: (ffi.new('uint64_t*', val), ffi.sizeof('uint64_t'))
-value_int64_pointer = lambda val: (ffi.new('int64_t*', val), ffi.sizeof('int64_t'))
-value_int_pointer = lambda val: (ffi.new('int*', val), ffi.sizeof('int'))
-value_binary_data = lambda val, length: (
-    ffi.new('char[%d]' % (length + 1), val),
-    ffi.sizeof('char') * length,
-)
 
-ZMQ_FD_64BIT = ffi.sizeof('ZMQ_FD_T') == 8
+def new_uint64_pointer():
+    return ffi.new('uint64_t*'), nsp(ffi.sizeof('uint64_t'))
 
-IPC_PATH_MAX_LEN = C.get_ipc_path_max_len()
 
-import zmq
-from zmq.constants import SocketOption, _OptType
-from zmq.error import ZMQError, _check_rc, _check_version
+def new_int64_pointer():
+    return ffi.new('int64_t*'), nsp(ffi.sizeof('int64_t'))
 
-from .message import Frame
-from .utils import _retry_sys_call
+
+def new_int_pointer():
+    return ffi.new('int*'), nsp(ffi.sizeof('int'))
+
+
+def new_binary_data(length):
+    return ffi.new('char[%d]' % length), nsp(ffi.sizeof('char') * length)
+
+
+def value_uint64_pointer(val):
+    return ffi.new('uint64_t*', val), ffi.sizeof('uint64_t')
+
+
+def value_int64_pointer(val):
+    return ffi.new('int64_t*', val), ffi.sizeof('int64_t')
+
+
+def value_int_pointer(val):
+    return ffi.new('int*', val), ffi.sizeof('int')
+
+
+def value_binary_data(val, length):
+    return ffi.new('char[%d]' % (length + 1), val), ffi.sizeof('char') * length
+
+
+ZMQ_FD_64BIT = ffi.sizeof('ZMQ_FD_T') == 8
+
+IPC_PATH_MAX_LEN = C.get_ipc_path_max_len()
 
 
 def new_pointer_from_opt(option, length=0):
     opt_type = getattr(option, "_opt_type", _OptType.int)
 
     if opt_type == _OptType.int64 or (ZMQ_FD_64BIT and opt_type == _OptType.fd):
         return new_int64_pointer()
@@ -152,18 +168,16 @@
         if isinstance(address, bytes):
             address = address_b.decode('utf8')
         rc = C.zmq_bind(self._zmq_socket, address_b)
         if rc < 0:
             if IPC_PATH_MAX_LEN and C.zmq_errno() == errno_mod.ENAMETOOLONG:
                 path = address.split('://', 1)[-1]
                 msg = (
-                    'ipc path "{}" is longer than {} '
-                    'characters (sizeof(sockaddr_un.sun_path)).'.format(
-                        path, IPC_PATH_MAX_LEN
-                    )
+                    f'ipc path "{path}" is longer than {IPC_PATH_MAX_LEN} '
+                    'characters (sizeof(sockaddr_un.sun_path)).'
                 )
                 raise ZMQError(C.zmq_errno(), msg=msg)
             elif C.zmq_errno() == errno_mod.ENOENT:
                 path = address.split('://', 1)[-1]
                 msg = f'No such file or directory for ipc path "{path}".'
                 raise ZMQError(C.zmq_errno(), msg=msg)
             else:
```

### Comparing `pyzmq-26.0.0b2/zmq/backend/cffi/utils.py` & `pyzmq-26.0.1/zmq/backend/cffi/utils.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/cython/_zmq.pxd` & `pyzmq-26.0.1/zmq/backend/cython/_zmq.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/cython/_zmq.py` & `pyzmq-26.0.1/zmq/backend/cython/_zmq.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,17 +82,14 @@
     zmq_ctx_get,
     zmq_ctx_new,
     zmq_ctx_set,
     zmq_curve_keypair,
     zmq_curve_public,
     zmq_device,
     zmq_disconnect,
-)
-from cython.cimports.zmq.backend.cython.libzmq import zmq_errno as _zmq_errno
-from cython.cimports.zmq.backend.cython.libzmq import (
     zmq_free_fn,
     zmq_getsockopt,
     zmq_has,
     zmq_init,
     zmq_join,
     zmq_leave,
     zmq_msg_close,
@@ -108,26 +105,25 @@
     zmq_msg_routing_id,
     zmq_msg_send,
     zmq_msg_set,
     zmq_msg_set_group,
     zmq_msg_set_routing_id,
     zmq_msg_size,
     zmq_msg_t,
-)
-from cython.cimports.zmq.backend.cython.libzmq import zmq_poll as zmq_poll_c
-from cython.cimports.zmq.backend.cython.libzmq import (
     zmq_pollitem_t,
     zmq_proxy,
     zmq_proxy_steerable,
     zmq_setsockopt,
     zmq_socket,
     zmq_socket_monitor,
     zmq_strerror,
     zmq_unbind,
 )
+from cython.cimports.zmq.backend.cython.libzmq import zmq_errno as _zmq_errno
+from cython.cimports.zmq.backend.cython.libzmq import zmq_poll as zmq_poll_c
 from cython.cimports.zmq.utils.buffers import asbuffer_r
 
 import zmq
 from zmq.constants import SocketOption, _OptType
 from zmq.error import InterruptedSystemCall, ZMQError, _check_version
 
 IPC_PATH_MAX_LEN = get_ipc_path_max_len()
@@ -883,20 +879,18 @@
             raise TypeError('expected str, got: %r' % addr)
         c_addr = addr_b
         rc = zmq_bind(self.handle, c_addr)
         if rc != 0:
             if IPC_PATH_MAX_LEN and zmq_errno() == ENAMETOOLONG:
                 path = addr.split('://', 1)[-1]
                 msg = (
-                    'ipc path "{}" is longer than {} '
+                    f'ipc path "{path}" is longer than {IPC_PATH_MAX_LEN} '
                     'characters (sizeof(sockaddr_un.sun_path)). '
                     'zmq.IPC_PATH_MAX_LEN constant can be used '
-                    'to check addr length (if it is defined).'.format(
-                        path, IPC_PATH_MAX_LEN
-                    )
+                    'to check addr length (if it is defined).'
                 )
                 raise ZMQError(msg=msg)
             elif zmq_errno() == ENOENT:
                 path = addr.split('://', 1)[-1]
                 msg = f'No such file or directory for ipc path "{path}".'
                 raise ZMQError(msg=msg)
         while True:
@@ -1513,15 +1507,15 @@
             pollitems[i].socket = NULL
             pollitems[i].fd = s
             pollitems[i].events = events
             pollitems[i].revents = 0
         elif hasattr(s, 'fileno'):
             try:
                 fileno = int(s.fileno())
-            except:
+            except Exception:
                 free(pollitems)
                 raise ValueError('fileno() must return a valid integer fd')
             else:
                 pollitems[i].socket = NULL
                 pollitems[i].fd = fileno
                 pollitems[i].events = events
                 pollitems[i].revents = 0
```

### Comparing `pyzmq-26.0.0b2/zmq/backend/cython/constant_enums.pxi` & `pyzmq-26.0.1/zmq/backend/cython/constant_enums.pxi`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/cython/libzmq.pxd` & `pyzmq-26.0.1/zmq/backend/cython/libzmq.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/backend/select.py` & `pyzmq-26.0.1/zmq/backend/select.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/constants.py` & `pyzmq-26.0.1/zmq/constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/decorators.py` & `pyzmq-26.0.1/zmq/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Like using Contexts and Sockets as context managers, but with decorator syntax.
 Context and sockets are closed at the end of the function.
 
 For example::
 
     from zmq.decorators import context, socket
-    
+
     @context()
     @socket(zmq.PUSH)
     def work(ctx, push):
         ...
 """
 
 from __future__ import annotations
@@ -65,16 +65,16 @@
 
                 with target(*dec_args, **dec_kwargs) as obj:
                     # insert our object into args
                     if kw_name and kw_name not in kwargs:
                         kwargs[kw_name] = obj
                     elif kw_name and kw_name in kwargs:
                         raise TypeError(
-                            "{}() got multiple values for"
-                            " argument '{}'".format(func.__name__, kw_name)
+                            f"{func.__name__}() got multiple values for"
+                            f" argument '{kw_name}'"
                         )
                     else:
                         args = args + (obj,)
 
                     return func(*args, **kwargs)
 
             return wrapper
```

### Comparing `pyzmq-26.0.0b2/zmq/devices/__init__.py` & `pyzmq-26.0.1/zmq/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/devices/basedevice.py` & `pyzmq-26.0.1/zmq/devices/basedevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Classes for running 0MQ Devices in the background."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
-
 import time
 from multiprocessing import Process
 from threading import Thread
 from typing import Any, Callable, List, Optional, Tuple
 
 import zmq
 from zmq import ENOTSOCK, ETERM, PUSH, QUEUE, Context, ZMQBindError, ZMQError, device
```

### Comparing `pyzmq-26.0.0b2/zmq/devices/monitoredqueue.py` & `pyzmq-26.0.1/zmq/devices/monitoredqueue.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/devices/monitoredqueuedevice.py` & `pyzmq-26.0.1/zmq/devices/monitoredqueuedevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """MonitoredQueue classes and functions."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
-
 from zmq import PUB
 from zmq.devices.monitoredqueue import monitored_queue
 from zmq.devices.proxydevice import ProcessProxy, Proxy, ProxyBase, ThreadProxy
 
 
 class MonitoredQueueBase(ProxyBase):
     """Base class for overriding methods."""
```

### Comparing `pyzmq-26.0.0b2/zmq/devices/proxydevice.py` & `pyzmq-26.0.1/zmq/devices/proxydevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/devices/proxysteerabledevice.py` & `pyzmq-26.0.1/zmq/devices/proxysteerabledevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/error.py` & `pyzmq-26.0.1/zmq/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,19 +171,15 @@
         self.min_version = min_version
         self.version = _zmq_version
 
     def __repr__(self):
         return "ZMQVersionError('%s')" % str(self)
 
     def __str__(self):
-        return "{} requires libzmq >= {}, have {}".format(
-            self.msg,
-            self.min_version,
-            self.version,
-        )
+        return f"{self.msg} requires libzmq >= {self.min_version}, have {self.version}"
 
 
 def _check_version(
     min_version_info: tuple[int] | tuple[int, int] | tuple[int, int, int],
     msg: str = "Feature",
 ):
     """Check for libzmq
```

### Comparing `pyzmq-26.0.0b2/zmq/eventloop/_deprecated.py` & `pyzmq-26.0.1/zmq/eventloop/_deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 support for concurrent futures - this will only be available if you
 have tornado ≥ 3.0.
 """
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
-
 import time
 import warnings
 from typing import Tuple
 
 from zmq import ETERM, POLLERR, POLLIN, POLLOUT, Poller, ZMQError
 
 tornado_version: Tuple = ()
@@ -196,18 +195,17 @@
     prior to calling this function.
     """
     from tornado import ioloop
 
     # check if tornado's IOLoop is already initialized to something other
     # than the pyzmq IOLoop instance:
     assert (
-        not ioloop.IOLoop.initialized()
-    ) or ioloop.IOLoop.instance() is IOLoop.instance(), (
-        "tornado IOLoop already initialized"
-    )
+        (not ioloop.IOLoop.initialized())
+        or ioloop.IOLoop.instance() is IOLoop.instance()
+    ), "tornado IOLoop already initialized"
 
     if tornado_version >= (3,):
         # tornado 3 has an official API for registering new defaults, yay!
         ioloop.IOLoop.configure(ZMQIOLoop)
     else:
         # we have to set the global instance explicitly
         ioloop.IOLoop._instance = IOLoop.instance()
```

### Comparing `pyzmq-26.0.0b2/zmq/eventloop/future.py` & `pyzmq-26.0.1/zmq/eventloop/future.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,8 +97,8 @@
         if io_loop is not None:
             warnings.warn(
                 f"{self.__class__.__name__}(io_loop) argument is deprecated in pyzmq 22.2."
                 " The currently active loop will always be used.",
                 DeprecationWarning,
                 stacklevel=2,
             )
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)  # type: ignore
```

### Comparing `pyzmq-26.0.0b2/zmq/eventloop/ioloop.py` & `pyzmq-26.0.1/zmq/eventloop/ioloop.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 eventloop integration is no longer required
 and tornado itself should be used.
 """
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
-
 import warnings
 
 
 def _deprecated():
     warnings.warn(
         "zmq.eventloop.ioloop is deprecated in pyzmq 17."
         " pyzmq now works with default tornado and asyncio eventloops.",
```

### Comparing `pyzmq-26.0.0b2/zmq/eventloop/zmqstream.py` & `pyzmq-26.0.1/zmq/eventloop/zmqstream.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
-from __future__ import annotations
-
 """A utility class for event-based messaging on a zmq socket using tornado.
 
 .. seealso::
 
     - :mod:`zmq.asyncio`
     - :mod:`zmq.eventloop.future`
 """
 
+from __future__ import annotations
+
 import asyncio
 import pickle
 import warnings
 from queue import Queue
 from typing import Any, Awaitable, Callable, Sequence, cast, overload
 
 from tornado.ioloop import IOLoop
```

### Comparing `pyzmq-26.0.0b2/zmq/green/__init__.py` & `pyzmq-26.0.1/zmq/green/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 Any calls that would have blocked the current thread will now only block the
 current green thread.
 
 This compatibility is accomplished by ensuring the nonblocking flag is set
 before any blocking operation and the ØMQ file descriptor is polled internally
 to trigger needed events.
 """
+
 from __future__ import annotations
 
 from typing import List
 
 import zmq as _zmq
 from zmq import *
 from zmq.green.core import _Context, _Socket
```

### Comparing `pyzmq-26.0.0b2/zmq/green/core.py` & `pyzmq-26.0.1/zmq/green/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 #  This file is part of pyzmq
 #  It is adapted from upstream project zeromq_gevent under the New BSD License
 #
 #  Distributed under the terms of the New BSD License.  The full license is in
 #  the file LICENSE.BSD, distributed as part of this software.
 # -----------------------------------------------------------------------------
 
-"""This module wraps the :class:`Socket` and :class:`Context` found in :mod:`pyzmq <zmq>` to be non blocking
-"""
+"""This module wraps the :class:`Socket` and :class:`Context` found in :mod:`pyzmq <zmq>` to be non blocking"""
+
 from __future__ import annotations
 
 import sys
 import time
 import warnings
 
 import gevent
@@ -214,17 +214,15 @@
                 msg = super().send(data, flags, copy, track, **kwargs)
             finally:
                 if not self.__in_send_multipart:
                     self.__state_changed()
             return msg
         # ensure the zmq.NOBLOCK flag is part of flags
         flags |= zmq.NOBLOCK
-        while (
-            True
-        ):  # Attempt to complete this operation indefinitely, blocking the current greenlet
+        while True:  # Attempt to complete this operation indefinitely, blocking the current greenlet
             try:
                 # attempt the actual call
                 msg = super().send(data, flags, copy, track)
             except zmq.ZMQError as e:
                 # if the raised ZMQError is not EAGAIN, reraise
                 if e.errno != zmq.EAGAIN:
                     if not self.__in_send_multipart:
```

### Comparing `pyzmq-26.0.0b2/zmq/green/device.py` & `pyzmq-26.0.1/zmq/green/device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/green/poll.py` & `pyzmq-26.0.1/zmq/green/poll.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 rlist.append(socket.getsockopt(zmq.FD))
                 continue
             elif isinstance(socket, int):
                 fd = socket
             elif hasattr(socket, 'fileno'):
                 try:
                     fd = int(socket.fileno())
-                except:
+                except Exception:
                     raise ValueError('fileno() must return an valid integer fd')
             else:
                 raise TypeError(
                     'Socket must be a 0MQ socket, an integer fd '
                     'or have a fileno() method: %r' % socket
                 )
```

### Comparing `pyzmq-26.0.0b2/zmq/log/__main__.py` & `pyzmq-26.0.1/zmq/log/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 Easily view log messages published by the PUBHandler in zmq.log.handlers
 
 Designed to be run as an executable module - try this to see options:
     python -m zmq.log -h
 
 Subscribes to the '' (empty string) topic by default which means it will work
-out-of-the-box with a PUBHandler object instantiated with default settings. 
-If you change the root topic with PUBHandler.setRootTopic() you must pass 
+out-of-the-box with a PUBHandler object instantiated with default settings.
+If you change the root topic with PUBHandler.setRootTopic() you must pass
 the value to this script with the --topic argument.
 
 Note that the default formats for the PUBHandler object selectively include
 the log level in the message. This creates redundancy in this script as it
-always prints the topic of the message, which includes the log level. 
+always prints the topic of the message, which includes the log level.
 Consider overriding the default formats with PUBHandler.setFormat() to
 avoid this issue.
 
 """
 
 # encoding: utf-8
```

### Comparing `pyzmq-26.0.0b2/zmq/log/handlers.py` & `pyzmq-26.0.1/zmq/log/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     >>> import logging
     >>> handler = PUBHandler('tcp://127.0.0.1:12345')
     >>> handler.root_topic = 'foo'
     >>> logger = logging.getLogger('foobar')
     >>> logger.setLevel(logging.DEBUG)
     >>> logger.addHandler(handler)
-    
+
 Or using ``dictConfig``, as in::
 
     >>> from logging.config import dictConfig
     >>> socket = Context.instance().socket(PUB)
     >>> socket.connect('tcp://127.0.0.1:12345')
     >>> dictConfig({
     >>>     'version': 1,
@@ -28,15 +28,15 @@
     >>>         }
     >>>     },
     >>>     'root': {
     >>>         'level': 'DEBUG',
     >>>         'handlers': ['zmq'],
     >>>     }
     >>> })
-        
+
 
 After this point, all messages logged by ``logger`` will be published on the
 PUB socket.
 
 Code adapted from StarCluster:
 
     https://github.com/jtriley/StarCluster/blob/StarCluster-0.91/starcluster/logger.py
@@ -214,15 +214,19 @@
         """
         logging.Logger.log(self, level, f'{topic}{TOPIC_DELIM}{msg}', *args, **kwargs)
 
 
 # Generate the methods of TopicLogger, since they are just adding a
 # topic prefix to a message.
 for name in "debug warn warning error critical fatal".split():
-    meth = getattr(logging.Logger, name)
+    try:
+        meth = getattr(logging.Logger, name)
+    except AttributeError:
+        # some methods are missing, e.g. Logger.warn was removed from Python 3.13
+        continue
     setattr(
         TopicLogger,
         name,
         lambda self, level, topic, msg, *args, **kwargs: meth(
             self, level, topic + TOPIC_DELIM + msg, *args, **kwargs
         ),
     )
```

### Comparing `pyzmq-26.0.0b2/zmq/ssh/forward.py` & `pyzmq-26.0.1/zmq/ssh/forward.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 Sample script showing how to do local port forwarding over paramiko.
 
 This script connects to the requested SSH server and sets up local port
 forwarding (the openssh -L option) from a local port through a tunneled
 connection to a destination reachable from the SSH server machine.
 """
 
-
 import logging
 import select
 import socketserver
 
 logger = logging.getLogger('ssh')
 
 
@@ -56,20 +55,15 @@
             logger.debug(
                 'Incoming request to %s:%d was rejected by the SSH server.'
                 % (self.chain_host, self.chain_port)
             )
             return
 
         logger.debug(
-            'Connected!  Tunnel open %r -> %r -> %r'
-            % (
-                self.request.getpeername(),
-                chan.getpeername(),
-                (self.chain_host, self.chain_port),
-            )
+            f'Connected!  Tunnel open {self.request.getpeername()!r} -> {chan.getpeername()!r} -> {(self.chain_host, self.chain_port)!r}'
         )
         while True:
             r, w, x = select.select([self.request, chan], [], [])
             if self.request in r:
                 data = self.request.recv(1024)
                 if len(data) == 0:
                     break
```

### Comparing `pyzmq-26.0.0b2/zmq/ssh/tunnel.py` & `pyzmq-26.0.1/zmq/ssh/tunnel.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 
 # Copyright (C) 2010-2011  IPython Development Team
 # Copyright (C) 2011- PyZMQ Developers
 #
 # Redistributed from IPython under the terms of the BSD License.
 
-
 import atexit
 import os
 import re
 import signal
 import socket
 import sys
 import warnings
```

### Comparing `pyzmq-26.0.0b2/zmq/sugar/__init__.py` & `pyzmq-26.0.1/zmq/sugar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """pure-Python sugar wrappers for core 0MQ objects."""
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
-
 from zmq import error
 from zmq.sugar import context, frame, poll, socket, tracker, version
 
 __all__ = []
 for submod in (context, error, frame, poll, socket, tracker, version):
     __all__.extend(submod.__all__)
```

### Comparing `pyzmq-26.0.0b2/zmq/sugar/attrsettr.py` & `pyzmq-26.0.1/zmq/sugar/attrsettr.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/sugar/context.py` & `pyzmq-26.0.1/zmq/sugar/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 import os
 from threading import Lock
 from typing import Any, Callable, Generic, TypeVar, overload
 from warnings import warn
 from weakref import WeakSet
 
 import zmq
+from zmq._typing import TypeAlias
 from zmq.backend import Context as ContextBase
 from zmq.constants import ContextOption, Errno, SocketOption
 from zmq.error import ZMQError
 from zmq.utils.interop import cast_int_addr
 
 from .attrsettr import AttributeSetter, OptValT
-from .socket import Socket
+from .socket import Socket, SyncSocket
 
 # notice when exiting, to avoid triggering term on exit
 _exiting = False
 
 
 def _notice_atexit() -> None:
     global _exiting
@@ -74,26 +75,26 @@
     _shadow_obj = None
     _warn_destroy_close = False
     _sockets: WeakSet
     # mypy doesn't like a default value here
     _socket_class: type[_SocketType] = Socket  # type: ignore
 
     @overload
-    def __init__(self: Context[Socket], io_threads: int = 1): ...
+    def __init__(self: SyncContext, io_threads: int = 1): ...
 
     @overload
-    def __init__(self: Context[Socket], io_threads: Context):
+    def __init__(self: SyncContext, io_threads: Context):
         # this should be positional-only, but that requires 3.8
         ...
 
     @overload
-    def __init__(self: Context[Socket], *, shadow: Context | int): ...
+    def __init__(self: SyncContext, *, shadow: Context | int): ...
 
     def __init__(
-        self: Context[Socket],
+        self: SyncContext,
         io_threads: int | Context = 1,
         shadow: Context | int = 0,
     ) -> None:
         if isinstance(io_threads, Context):
             # allow positional shadow `zmq.Context(zmq.asyncio.Context())`
             # this s
             shadow = io_threads
@@ -411,8 +412,11 @@
         else:
             if opt not in self.sockopts:
                 raise AttributeError(key)
             else:
                 del self.sockopts[opt]
 
 
-__all__ = ['Context']
+SyncContext: TypeAlias = Context[SyncSocket]
+
+
+__all__ = ['Context', 'SyncContext']
```

### Comparing `pyzmq-26.0.0b2/zmq/sugar/frame.py` & `pyzmq-26.0.1/zmq/sugar/frame.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/sugar/poll.py` & `pyzmq-26.0.1/zmq/sugar/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/sugar/socket.py` & `pyzmq-26.0.1/zmq/sugar/socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Union,
     cast,
     overload,
 )
 from warnings import warn
 
 import zmq
-from zmq._typing import Literal
+from zmq._typing import Literal, TypeAlias
 from zmq.backend import Socket as SocketBase
 from zmq.error import ZMQBindError, ZMQError
 from zmq.utils import jsonapi
 from zmq.utils.interop import cast_int_addr
 
 from ..constants import SocketOption, SocketType, _OptType
 from .attrsettr import AttributeSetter
@@ -1103,8 +1103,10 @@
 
         .. versionadded:: 14.4
         """
         self._monitor_socket = None
         self.monitor(None, 0)
 
 
-__all__ = ['Socket']
+SyncSocket: TypeAlias = Socket[bytes]
+
+__all__ = ['Socket', 'SyncSocket']
```

### Comparing `pyzmq-26.0.0b2/zmq/sugar/stopwatch.py` & `pyzmq-26.0.1/zmq/sugar/stopwatch.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/sugar/tracker.py` & `pyzmq-26.0.1/zmq/sugar/tracker.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/sugar/version.py` & `pyzmq-26.0.1/zmq/sugar/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 import re
 from typing import Match, cast
 
 from zmq.backend import zmq_version_info
 
-__version__: str = "26.0.0b2"
+__version__: str = "26.0.1"
 _version_pat = re.compile(r"(\d+)\.(\d+)\.(\d+)(.*)")
 _match = cast(Match, _version_pat.match(__version__))
 _version_groups = _match.groups()
 
 VERSION_MAJOR = int(_version_groups[0])
 VERSION_MINOR = int(_version_groups[1])
 VERSION_PATCH = int(_version_groups[2])
```

### Comparing `pyzmq-26.0.0b2/zmq/tests/__init__.py` & `pyzmq-26.0.1/zmq/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 
 PYPY = platform.python_implementation() == 'PyPy'
 
 # -----------------------------------------------------------------------------
 # skip decorators (directly from unittest)
 # -----------------------------------------------------------------------------
 
-_id = lambda x: x
+
+def _id(x):
+    return x
+
 
 skip_pypy = mark.skipif(PYPY, reason="Doesn't work on PyPy")
 require_zmq_4 = mark.skipif(zmq.zmq_version_info() < (4,), reason="requires zmq >= 4")
 
 # -----------------------------------------------------------------------------
 # Base test class
 # -----------------------------------------------------------------------------
@@ -168,17 +171,16 @@
     def assertRaisesErrno(self, errno, func, *args, **kwargs):
         try:
             func(*args, **kwargs)
         except zmq.ZMQError as e:
             self.assertEqual(
                 e.errno,
                 errno,
-                "wrong error raised, expected '%s' \
-got '%s'"
-                % (zmq.ZMQError(errno), zmq.ZMQError(e.errno)),
+                f"wrong error raised, expected '{zmq.ZMQError(errno)}' \
+got '{zmq.ZMQError(e.errno)}'",
             )
         else:
             self.fail("Function did not raise any error")
 
     def _select_recv(self, multipart, socket, **kwargs):
         """call recv[_multipart] in a way that raises if there is nothing to receive"""
         if zmq.zmq_version_info() >= (3, 1, 0):
@@ -219,17 +221,16 @@
         try:
             func(*args, **kwargs)
         except zmq.ZMQError:
             e = sys.exc_info()[1]
             self.assertEqual(
                 e.errno,
                 errno,
-                "wrong error raised, expected '%s' \
-got '%s'"
-                % (zmq.ZMQError(errno), zmq.ZMQError(e.errno)),
+                f"wrong error raised, expected '{zmq.ZMQError(errno)}' \
+got '{zmq.ZMQError(e.errno)}'",
             )
         else:
             self.fail("Function did not raise any error")
 
     def tearDown(self):
         if self._should_test_timeout:
             # cancel the timeout alarm, if there was one
```

### Comparing `pyzmq-26.0.0b2/zmq/tests/conftest.py` & `pyzmq-26.0.1/zmq/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/cython_ext.pyx` & `pyzmq-26.0.1/zmq/tests/cython_ext.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_asyncio.py` & `pyzmq-26.0.1/zmq/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_auth.py` & `pyzmq-26.0.1/zmq/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_cffi_backend.py` & `pyzmq-26.0.1/zmq/tests/test_cffi_backend.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_constants.py` & `pyzmq-26.0.1/zmq/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_context.py` & `pyzmq-26.0.1/zmq/tests/test_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def test_instance(self):
         ctx = self.Context.instance()
         c2 = self.Context.instance(io_threads=2)
         assert c2 is ctx
         c2.term()
         c3 = self.Context.instance()
         c4 = self.Context.instance()
-        assert not c3 is c2
+        assert c3 is not c2
         assert not c3.closed
         assert c3 is c4
 
     def test_instance_subclass_first(self):
         self.context.term()
 
         class SubContext(zmq.Context):
```

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_cython.py` & `pyzmq-26.0.1/zmq/tests/test_cython.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_decorators.py` & `pyzmq-26.0.1/zmq/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_device.py` & `pyzmq-26.0.1/zmq/tests/test_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             del dev
 
     def test_device_attributes(self):
         dev = devices.Device(zmq.QUEUE, zmq.SUB, zmq.PUB)
         assert dev.in_type == zmq.SUB
         assert dev.out_type == zmq.PUB
         assert dev.device_type == zmq.QUEUE
-        assert dev.daemon == True
+        assert dev.daemon is True
         del dev
 
     def test_single_socket_forwarder_connect(self):
         if zmq.zmq_version() in ('4.1.1', '4.0.6'):
             raise SkipTest("libzmq-%s broke single-socket devices" % zmq.zmq_version())
         dev = devices.ThreadDevice(zmq.QUEUE, zmq.REP, -1)
         req = self.context.socket(zmq.REQ)
```

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_draft.py` & `pyzmq-26.0.1/zmq/tests/test_draft.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_error.py` & `pyzmq-26.0.1/zmq/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_etc.py` & `pyzmq-26.0.1/zmq/tests/test_etc.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_ext.py` & `pyzmq-26.0.1/zmq/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_future.py` & `pyzmq-26.0.1/zmq/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_imports.py` & `pyzmq-26.0.1/zmq/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_includes.py` & `pyzmq-26.0.1/zmq/tests/test_includes.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_ioloop.py` & `pyzmq-26.0.1/zmq/tests/test_ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_log.py` & `pyzmq-26.0.1/zmq/tests/test_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         time.sleep(0.1)
         return logger, handler, sub
 
     def test_init_iface(self):
         logger = self.logger
         ctx = self.context
         handler = handlers.PUBHandler(self.iface)
-        assert not handler.ctx is ctx
+        assert handler.ctx is not ctx
         self.sockets.append(handler.socket)
         # handler.ctx.term()
         handler = handlers.PUBHandler(self.iface, self.context)
         self.sockets.append(handler.socket)
         assert handler.ctx is ctx
         handler.setLevel(logging.DEBUG)
         handler.root_topic = self.topic
```

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_message.py` & `pyzmq-26.0.1/zmq/tests/test_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,17 @@
             if pm.done:
                 break
             time.sleep(0.1)
         assert pm.done
 
     def test_no_tracker(self):
         m = zmq.Frame(b'asdf', track=False)
-        assert m.tracker == None
+        assert m.tracker is None
         m2 = copy.copy(m)
-        assert m2.tracker == None
+        assert m2.tracker is None
         self.assertRaises(ValueError, zmq.MessageTracker, m)
 
     def test_multi_tracker(self):
         m = zmq.Frame(b'asdf', copy=False, track=True)
         m2 = zmq.Frame(b'whoda', copy=False, track=True)
         mt = zmq.MessageTracker(m, m2)
         assert not m.tracker.done
```

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_monitor.py` & `pyzmq-26.0.1/zmq/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_monqueue.py` & `pyzmq-26.0.1/zmq/tests/test_monqueue.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_multipart.py` & `pyzmq-26.0.1/zmq/tests/test_multipart.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,19 +10,18 @@
     def test_router_dealer(self):
         router, dealer = self.create_bound_pair(zmq.ROUTER, zmq.DEALER)
 
         msg1 = b'message1'
         dealer.send(msg1)
         self.recv(router)
         more = router.rcvmore
-        assert more == True
+        assert more
         msg2 = self.recv(router)
         assert msg1 == msg2
-        more = router.rcvmore
-        assert more == False
+        assert not router.rcvmore
 
     def test_basic_multipart(self):
         a, b = self.create_bound_pair(zmq.PAIR, zmq.PAIR)
         msg = [b'hi', b'there', b'b']
         a.send_multipart(msg)
         recvd = b.recv_multipart()
         assert msg == recvd
```

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_mypy.py` & `pyzmq-26.0.1/zmq/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_pair.py` & `pyzmq-26.0.1/zmq/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_poll.py` & `pyzmq-26.0.1/zmq/tests/test_poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_proxy_steerable.py` & `pyzmq-26.0.1/zmq/tests/test_proxy_steerable.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_pubsub.py` & `pyzmq-26.0.1/zmq/tests/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_reqrep.py` & `pyzmq-26.0.1/zmq/tests/test_reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_retry_eintr.py` & `pyzmq-26.0.1/zmq/tests/test_retry_eintr.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_security.py` & `pyzmq-26.0.1/zmq/tests/test_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         client.curve_serverkey = server_public
         client.curve_publickey = client_public
         client.curve_secretkey = client_secret
 
         assert server.mechanism == zmq.CURVE
         assert client.mechanism == zmq.CURVE
 
-        assert server.get(zmq.CURVE_SERVER) == True
-        assert client.get(zmq.CURVE_SERVER) == False
+        assert server.get(zmq.CURVE_SERVER)
+        assert not client.get(zmq.CURVE_SERVER)
 
         with self.zap():
             iface = 'tcp://127.0.0.1'
             port = server.bind_to_random_port(iface)
             client.connect("%s:%i" % (iface, port))
             self.bounce(server, client)
```

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_socket.py` & `pyzmq-26.0.1/zmq/tests/test_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
                 a.bind(url)
                 with ctx.socket(zmq.PULL) as b:
                     b.connect(url)
                     msg = b'hi'
                     a.send(msg)
                     rcvd = self.recv(b)
                     assert rcvd == msg
-                assert b.closed == True
-            assert a.closed == True
-        assert ctx.closed == True
+                assert b.closed is True
+            assert a.closed is True
+        assert ctx.closed is True
 
     def test_connectbind_context_managers(self):
         url = 'inproc://a'
         msg = b'hi'
         with self.Context() as ctx:
             # Test connect() context manager
             with ctx.socket(zmq.PUSH) as a, ctx.socket(zmq.PULL) as b:
@@ -352,46 +352,46 @@
 
         b.bind(iface)
         msg = self.recv_multipart(b)
         for i in range(10):
             if p1.done:
                 break
             time.sleep(0.1)
-        assert p1.done == True
+        assert p1.done is True
         assert msg == [b'something']
         msg = self.recv_multipart(b)
         for i in range(10):
             if p2.done:
                 break
             time.sleep(0.1)
-        assert p2.done == True
+        assert p2.done is True
         assert msg == [b'something', b'else']
         m = zmq.Frame(b"again", copy=False, track=True)
-        assert m.tracker.done == False
+        assert m.tracker.done is False
         p1 = a.send(m, copy=False)
         p2 = a.send(m, copy=False)
-        assert m.tracker.done == False
-        assert p1.done == False
-        assert p2.done == False
+        assert m.tracker.done is False
+        assert p1.done is False
+        assert p2.done is False
         msg = self.recv_multipart(b)
-        assert m.tracker.done == False
+        assert m.tracker.done is False
         assert msg == [b'again']
         msg = self.recv_multipart(b)
-        assert m.tracker.done == False
+        assert m.tracker.done is False
         assert msg == [b'again']
-        assert p1.done == False
-        assert p2.done == False
+        assert p1.done is False
+        assert p2.done is False
         m.tracker
         del m
         for i in range(10):
             if p1.done:
                 break
             time.sleep(0.1)
-        assert p1.done == True
-        assert p2.done == True
+        assert p1.done is True
+        assert p2.done is True
         m = zmq.Frame(b'something', track=False)
         self.assertRaises(ValueError, a.send, m, copy=False, track=True)
 
     def test_close(self):
         ctx = self.Context()
         s = ctx.socket(zmq.PUB)
         s.close()
```

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_version.py` & `pyzmq-26.0.1/zmq/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_win32_shim.py` & `pyzmq-26.0.1/zmq/tests/test_win32_shim.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_z85.py` & `pyzmq-26.0.1/zmq/tests/test_z85.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,56 +10,56 @@
 
 from zmq.utils import z85
 
 
 class TestZ85(TestCase):
     def test_client_public(self):
         client_public = (
-            b"\xBB\x88\x47\x1D\x65\xE2\x65\x9B"
-            b"\x30\xC5\x5A\x53\x21\xCE\xBB\x5A"
-            b"\xAB\x2B\x70\xA3\x98\x64\x5C\x26"
-            b"\xDC\xA2\xB2\xFC\xB4\x3F\xC5\x18"
+            b"\xbb\x88\x47\x1d\x65\xe2\x65\x9b"
+            b"\x30\xc5\x5a\x53\x21\xce\xbb\x5a"
+            b"\xab\x2b\x70\xa3\x98\x64\x5c\x26"
+            b"\xdc\xa2\xb2\xfc\xb4\x3f\xc5\x18"
         )
         encoded = z85.encode(client_public)
 
         assert encoded == b"Yne@$w-vo<fVvi]a<NY6T1ed:M$fCG*[IaLV{hID"
         decoded = z85.decode(encoded)
         assert decoded == client_public
 
     def test_client_secret(self):
         client_secret = (
-            b"\x7B\xB8\x64\xB4\x89\xAF\xA3\x67"
-            b"\x1F\xBE\x69\x10\x1F\x94\xB3\x89"
-            b"\x72\xF2\x48\x16\xDF\xB0\x1B\x51"
-            b"\x65\x6B\x3F\xEC\x8D\xFD\x08\x88"
+            b"\x7b\xb8\x64\xb4\x89\xaf\xa3\x67"
+            b"\x1f\xbe\x69\x10\x1f\x94\xb3\x89"
+            b"\x72\xf2\x48\x16\xdf\xb0\x1b\x51"
+            b"\x65\x6b\x3f\xec\x8d\xfd\x08\x88"
         )
         encoded = z85.encode(client_secret)
 
         assert encoded == b"D:)Q[IlAW!ahhC2ac:9*A}h:p?([4%wOTJ%JR%cs"
         decoded = z85.decode(encoded)
         assert decoded == client_secret
 
     def test_server_public(self):
         server_public = (
-            b"\x54\xFC\xBA\x24\xE9\x32\x49\x96"
-            b"\x93\x16\xFB\x61\x7C\x87\x2B\xB0"
-            b"\xC1\xD1\xFF\x14\x80\x04\x27\xC5"
-            b"\x94\xCB\xFA\xCF\x1B\xC2\xD6\x52"
+            b"\x54\xfc\xba\x24\xe9\x32\x49\x96"
+            b"\x93\x16\xfb\x61\x7c\x87\x2b\xb0"
+            b"\xc1\xd1\xff\x14\x80\x04\x27\xc5"
+            b"\x94\xcb\xfa\xcf\x1b\xc2\xd6\x52"
         )
         encoded = z85.encode(server_public)
 
         assert encoded == b"rq:rM>}U?@Lns47E1%kR.o@n%FcmmsL/@{H8]yf7"
         decoded = z85.decode(encoded)
         assert decoded == server_public
 
     def test_server_secret(self):
         server_secret = (
-            b"\x8E\x0B\xDD\x69\x76\x28\xB9\x1D"
-            b"\x8F\x24\x55\x87\xEE\x95\xC5\xB0"
-            b"\x4D\x48\x96\x3F\x79\x25\x98\x77"
-            b"\xB4\x9C\xD9\x06\x3A\xEA\xD3\xB7"
+            b"\x8e\x0b\xdd\x69\x76\x28\xb9\x1d"
+            b"\x8f\x24\x55\x87\xee\x95\xc5\xb0"
+            b"\x4d\x48\x96\x3f\x79\x25\x98\x77"
+            b"\xb4\x9c\xd9\x06\x3a\xea\xd3\xb7"
         )
         encoded = z85.encode(server_secret)
 
         assert encoded == b"JTKVSB%%)wK0E.X)V>+}o?pNmC{O&4W4b!Ni{Lh6"
         decoded = z85.decode(encoded)
         assert decoded == server_secret
```

### Comparing `pyzmq-26.0.0b2/zmq/tests/test_zmqstream.py` & `pyzmq-26.0.1/zmq/tests/test_zmqstream.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/utils/buffers.pxd` & `pyzmq-26.0.1/zmq/utils/buffers.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/utils/garbage.py` & `pyzmq-26.0.1/zmq/utils/garbage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Garbage collection thread for representing zmq refcount of Python objects
 used in zero-copy sends.
 """
 
 # Copyright (C) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
-
 import atexit
 import struct
 import warnings
 from collections import namedtuple
 from os import getpid
 from threading import Event, Lock, Thread
```

### Comparing `pyzmq-26.0.0b2/zmq/utils/interop.py` & `pyzmq-26.0.1/zmq/utils/interop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/utils/ipcmaxlen.h` & `pyzmq-26.0.1/zmq/utils/ipcmaxlen.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/utils/jsonapi.py` & `pyzmq-26.0.1/zmq/utils/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/utils/monitor.py` & `pyzmq-26.0.1/zmq/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/utils/mutex.h` & `pyzmq-26.0.1/zmq/utils/mutex.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/utils/strtypes.py` & `pyzmq-26.0.1/zmq/utils/strtypes.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/utils/win32.py` & `pyzmq-26.0.1/zmq/utils/win32.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,18 @@
         SetConsoleCtrlHandler = self._SetConsoleCtrlHandler = (
             kernel32.SetConsoleCtrlHandler
         )
         SetConsoleCtrlHandler.argtypes = (PHANDLER_ROUTINE, BOOL)
         SetConsoleCtrlHandler.restype = BOOL
 
         if action is None:
-            action = lambda: None
+
+            def action():
+                return None
+
         self.action = action
 
         @PHANDLER_ROUTINE
         def handle(event):
             if event == 0:  # CTRL_C_EVENT
                 action()
                 # Typical C implementations would return 1 to indicate that
```

### Comparing `pyzmq-26.0.0b2/zmq/utils/z85.py` & `pyzmq-26.0.1/zmq/utils/z85.py`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmq/utils/zmq_compat.h` & `pyzmq-26.0.1/zmq/utils/zmq_compat.h`

 * *Files identical despite different names*

### Comparing `pyzmq-26.0.0b2/zmqversion.py` & `pyzmq-26.0.1/zmqversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,21 @@
 This is similar to the version.sh script in a zeromq source dir, but
 it searches for an installed header, rather than in the current dir.
 """
 
 # Copyright (c) PyZMQ Developers
 # Distributed under the terms of the Modified BSD License.
 
-
 import os
 import re
 import sys
 import traceback
+from configparser import ConfigParser
 from warnings import warn
 
-try:
-    from configparser import ConfigParser
-except:
-    from ConfigParser import ConfigParser
-
 pjoin = os.path.join
 
 MAJOR_PAT = '^#define +ZMQ_VERSION_MAJOR +[0-9]+$'
 MINOR_PAT = '^#define +ZMQ_VERSION_MINOR +[0-9]+$'
 PATCH_PAT = '^#define +ZMQ_VERSION_PATCH +[0-9]+$'
```

### Comparing `pyzmq-26.0.0b2/PKG-INFO` & `pyzmq-26.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzmq
-Version: 26.0.0b2
+Version: 26.0.1
 Summary: Python bindings for 0MQ
 Author: Brian E. Granger, Min Ragan-Kelley
 Author-Email: PyZMQ Contributors <zeromq-dev@lists.zeromq.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2009-2012, Brian Granger, Min Ragan-Kelley
```

