# Comparing `tmp/gwcelery-2.1.1.tar.gz` & `tmp/gwcelery-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwcelery-2.1.1.tar", max compression
+gzip compressed data, was "gwcelery-2.1.2.tar", max compression
```

## Comparing `gwcelery-2.1.1.tar` & `gwcelery-2.1.2.tar`

### file list

```diff
@@ -1,232 +1,233 @@
--rw-r--r--   0        0        0    95189 2023-05-29 15:18:35.905637 gwcelery-2.1.1/CHANGES.rst
--rw-r--r--   0        0        0       64 2023-05-29 15:18:35.906637 gwcelery-2.1.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0    19716 2023-05-29 15:18:35.906637 gwcelery-2.1.1/LICENSE.rst
--rw-r--r--   0        0        0     1351 2023-05-29 15:18:35.906637 gwcelery-2.1.1/README.rst
--rw-r--r--   0        0        0      634 2023-05-29 15:18:35.906637 gwcelery-2.1.1/doc/Makefile
--rw-r--r--   0        0        0   191486 2023-05-29 15:18:35.908637 gwcelery-2.1.1/doc/_static/acceptance-tests-checklist.png
--rw-r--r--   0        0        0   241593 2023-05-29 15:18:35.910637 gwcelery-2.1.1/doc/_static/celeryevent-screenshot.png
--rw-r--r--   0        0        0   206465 2023-05-29 15:18:35.911637 gwcelery-2.1.1/doc/_static/deployment-screenshot.png
--rw-r--r--   0        0        0   161306 2023-05-29 15:18:35.912637 gwcelery-2.1.1/doc/_static/flask-screenshot.png
--rw-r--r--   0        0        0   328056 2023-05-29 15:18:35.913637 gwcelery-2.1.1/doc/_static/flower-screenshot.png
--rw-r--r--   0        0        0   114719 2023-05-29 15:18:35.914637 gwcelery-2.1.1/doc/_static/logo-0.5x.png
--rw-r--r--   0        0        0   351955 2023-05-29 15:18:35.917637 gwcelery-2.1.1/doc/_static/logo.png
--rw-r--r--   0        0        0   230777 2023-05-29 15:18:35.918637 gwcelery-2.1.1/doc/_static/sentry-screenshot.png
--rwxr-xr-x   0        0        0     7356 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/conf.py
--rw-r--r--   0        0        0     4346 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/configuration.rst
--rw-r--r--   0        0        0     5698 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/contributing.rst
--rw-r--r--   0        0        0     7202 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/deployment.rst
--rw-r--r--   0        0        0    10176 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/design.rst
--rw-r--r--   0        0        0      486 2023-05-29 15:18:35.919637 gwcelery-2.1.1/doc/gwcelery.conf.rst
--rw-r--r--   0        0        0      284 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.email.rst
--rw-r--r--   0        0        0      329 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.igwn_alert.rst
--rw-r--r--   0        0        0      227 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.rst
--rw-r--r--   0        0        0       79 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.sentry.rst
--rw-r--r--   0        0        0       97 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.alerts.rst
--rw-r--r--   0        0        0      103 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.bayestar.rst
--rw-r--r--   0        0        0      107 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.circulars.rst
--rw-r--r--   0        0        0       98 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.condor.rst
--rw-r--r--   0        0        0     2404 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.detchar.rst
--rw-r--r--   0        0        0     1110 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.em_bright.rst
--rw-r--r--   0        0        0      129 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.external_skymaps.rst
--rw-r--r--   0        0        0     6738 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.external_triggers.rst
--rw-r--r--   0        0        0      112 2023-05-29 15:18:35.920637 gwcelery-2.1.1/doc/gwcelery.tasks.first2years.rst
--rw-r--r--   0        0        0       88 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.gcn.rst
--rw-r--r--   0        0        0      100 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.gracedb.rst
--rw-r--r--   0        0        0      109 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.igwn_alert.rst
--rw-r--r--   0        0        0      109 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.inference.rst
--rw-r--r--   0        0        0     8111 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.orchestrator.rst
--rw-r--r--   0        0        0      100 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.p_astro.rst
--rw-r--r--   0        0        0       94 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.raven.rst
--rw-r--r--   0        0        0      628 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.rst
--rw-r--r--   0        0        0      100 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.skymaps.rst
--rw-r--r--   0        0        0     7161 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tasks.superevents.rst
--rw-r--r--   0        0        0       97 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tools.condor.rst
--rw-r--r--   0        0        0       94 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tools.flask.rst
--rw-r--r--   0        0        0       97 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tools.nagios.rst
--rw-r--r--   0        0        0      185 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.tools.rst
--rw-r--r--   0        0        0       73 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.util.rst
--rw-r--r--   0        0        0      507 2023-05-29 15:18:35.921637 gwcelery-2.1.1/doc/gwcelery.voevent.rst
--rw-r--r--   0        0        0     3564 2023-05-29 15:18:35.922637 gwcelery-2.1.1/doc/htcondor.rst
--rw-r--r--   0        0        0     1576 2023-05-29 15:18:35.922637 gwcelery-2.1.1/doc/index.rst
--rw-r--r--   0        0        0      800 2023-05-29 15:18:35.922637 gwcelery-2.1.1/doc/make.bat
--rw-r--r--   0        0        0     4416 2023-05-29 15:18:35.922637 gwcelery-2.1.1/doc/monitoring.rst
--rw-r--r--   0        0        0     5312 2023-05-29 15:18:35.922637 gwcelery-2.1.1/doc/quickstart.rst
--rw-r--r--   0        0        0     1149 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/__init__.py
--rw-r--r--   0        0        0    18447 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/_version.py
--rw-r--r--   0        0        0    15596 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/conf/__init__.py
--rw-r--r--   0        0        0     1014 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/conf/dev.py
--rw-r--r--   0        0        0      403 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/conf/development.py
--rw-r--r--   0        0        0     1026 2023-05-29 15:18:35.922637 gwcelery-2.1.1/gwcelery/conf/minikube.py
--rw-r--r--   0        0        0     1722 2023-05-29 15:18:35.923637 gwcelery-2.1.1/gwcelery/conf/playground.py
--rw-r--r--   0        0        0     3541 2023-05-29 15:18:35.923637 gwcelery-2.1.1/gwcelery/conf/production.py
--rw-r--r--   0        0        0     2040 2023-05-29 15:18:35.923637 gwcelery-2.1.1/gwcelery/conf/test.py
--rw-r--r--   0        0        0        0 2023-05-29 15:18:36.000637 gwcelery-2.1.1/gwcelery/data/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 15:18:36.001637 gwcelery-2.1.1/gwcelery/data/first2years/__init__.py
--rw-r--r--   0        0        0   731421 2023-05-29 15:18:35.925637 gwcelery-2.1.1/gwcelery/data/first2years/gstlal.xml.gz
--rwxr-xr-x   0        0        0     2785 2023-05-29 15:18:35.925637 gwcelery-2.1.1/gwcelery/data/gwcelery.sub
--rw-r--r--   0        0        0      505 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/email/__init__.py
--rw-r--r--   0        0        0     3317 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/email/bootsteps.py
--rw-r--r--   0        0        0      995 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/email/signals.py
--rw-r--r--   0        0        0     1457 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/flask.py
--rw-r--r--   0        0        0      529 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/igwn_alert/__init__.py
--rw-r--r--   0        0        0     4484 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/igwn_alert/bootsteps.py
--rw-r--r--   0        0        0      608 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/igwn_alert/signals.py
--rw-r--r--   0        0        0      275 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/jinja.py
--rw-r--r--   0        0        0      305 2023-05-29 15:18:35.926637 gwcelery-2.1.1/gwcelery/kafka/__init__.py
--rw-r--r--   0        0        0    10431 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/kafka/bootsteps.py
--rw-r--r--   0        0        0      522 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/kafka/signals.py
--rw-r--r--   0        0        0     2567 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/sentry/__init__.py
--rw-r--r--   0        0        0       34 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/sentry/integrations/__init__.py
--rw-r--r--   0        0        0      832 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/sentry/integrations/condor.py
--rw-r--r--   0        0        0      836 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/sentry/integrations/requests.py
--rw-r--r--   0        0        0      939 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/sentry/integrations/subprocess.py
--rw-r--r--   0        0        0     1302 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/static/typeahead.css
--rw-r--r--   0        0        0     4124 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/static/vega/index.html
--rw-r--r--   0        0        0      515 2023-05-29 15:18:35.927637 gwcelery-2.1.1/gwcelery/tasks/__init__.py
--rw-r--r--   0        0        0    13597 2023-05-29 15:18:35.928637 gwcelery-2.1.1/gwcelery/tasks/alerts.py
--rw-r--r--   0        0        0     2672 2023-05-29 15:18:35.928637 gwcelery-2.1.1/gwcelery/tasks/bayestar.py
--rw-r--r--   0        0        0     1535 2023-05-29 15:18:35.928637 gwcelery-2.1.1/gwcelery/tasks/circulars.py
--rw-r--r--   0        0        0     7502 2023-05-29 15:18:35.928637 gwcelery-2.1.1/gwcelery/tasks/condor.py
--rw-r--r--   0        0        0     2692 2023-05-29 15:18:35.928637 gwcelery-2.1.1/gwcelery/tasks/core.py
--rw-r--r--   0        0        0    21515 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/detchar.py
--rw-r--r--   0        0        0     4863 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/em_bright.py
--rw-r--r--   0        0        0    21951 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/external_skymaps.py
--rw-r--r--   0        0        0    23806 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/external_triggers.py
--rw-r--r--   0        0        0     6832 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/first2years.py
--rw-r--r--   0        0        0     6384 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/first2years_external.py
--rw-r--r--   0        0        0     4831 2023-05-29 15:18:35.929637 gwcelery-2.1.1/gwcelery/tasks/gcn.py
--rw-r--r--   0        0        0    11079 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/gracedb.py
--rw-r--r--   0        0        0     6105 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/gwskynet.py
--rw-r--r--   0        0        0     2453 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/igwn_alert.py
--rw-r--r--   0        0        0    41859 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/inference.py
--rw-r--r--   0        0        0     1406 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/legacy_gracedb.py
--rw-r--r--   0        0        0     7772 2023-05-29 15:18:35.930637 gwcelery-2.1.1/gwcelery/tasks/notice_text.py
--rw-r--r--   0        0        0    46819 2023-05-29 15:18:35.931637 gwcelery-2.1.1/gwcelery/tasks/orchestrator.py
--rw-r--r--   0        0        0     5796 2023-05-29 15:18:35.931637 gwcelery-2.1.1/gwcelery/tasks/p_astro.py
--rw-r--r--   0        0        0    20999 2023-05-29 15:18:35.931637 gwcelery-2.1.1/gwcelery/tasks/raven.py
--rw-r--r--   0        0        0     2242 2023-05-29 15:18:35.931637 gwcelery-2.1.1/gwcelery/tasks/rrt_utils.py
--rw-r--r--   0        0        0    12528 2023-05-29 15:18:35.932637 gwcelery-2.1.1/gwcelery/tasks/skymaps.py
--rw-r--r--   0        0        0    23631 2023-05-29 15:18:35.932637 gwcelery-2.1.1/gwcelery/tasks/superevents.py
--rw-r--r--   0        0        0     1084 2023-05-29 15:18:35.932637 gwcelery-2.1.1/gwcelery/templates/fits_header.jinja2
--rw-r--r--   0        0        0    35556 2023-05-29 15:18:35.932637 gwcelery-2.1.1/gwcelery/templates/index.jinja2
--rw-r--r--   0        0        0     8505 2023-05-29 15:18:35.932637 gwcelery-2.1.1/gwcelery/templates/lalinference.jinja2
--rw-r--r--   0        0        0     9496 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/templates/rapidpe.jinja2
--rw-r--r--   0        0        0      806 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/templates/vector_table.jinja2
--rw-r--r--   0        0        0        0 2023-05-29 15:18:36.003637 gwcelery-2.1.1/gwcelery/tests/__init__.py
--rw-r--r--   0        0        0     4388 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/conftest.py
--rw-r--r--   0        0        0      976 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/G000012_S0040_preferred.json
--rw-r--r--   0        0        0     6258 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/G298048-1-Initial.xml
--rw-r--r--   0        0        0      599 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/G298048_log.json
--rw-r--r--   0        0        0      150 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
--rw-r--r--   0        0        0      974 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
--rw-r--r--   0        0        0    17572 2023-05-29 15:18:35.933637 gwcelery-2.1.1/gwcelery/tests/data/MS220722v.xml
--rw-r--r--   0        0        0   777600 2023-05-29 15:18:35.938637 gwcelery-2.1.1/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
--rw-r--r--   0        0        0     8220 2023-05-29 15:18:35.938637 gwcelery-2.1.1/gwcelery/tests/data/S230413b.json
--rw-r--r--   0        0        0     7255 2023-05-29 15:18:35.938637 gwcelery-2.1.1/gwcelery/tests/data/S230413g.json
--rw-r--r--   0        0        0     7721 2023-05-29 15:18:35.938637 gwcelery-2.1.1/gwcelery/tests/data/S230413h.json
--rw-r--r--   0        0        0     3387 2023-05-29 15:18:35.939637 gwcelery-2.1.1/gwcelery/tests/data/T0212_S0039_preferred.json
--rw-r--r--   0        0        0     3384 2023-05-29 15:18:35.939637 gwcelery-2.1.1/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
--rw-r--r--   0        0        0     5210 2023-05-29 15:18:35.939637 gwcelery-2.1.1/gwcelery/tests/data/T0219_S0041_nopreferred.json
--rw-r--r--   0        0        0        0 2023-05-29 15:18:36.003637 gwcelery-2.1.1/gwcelery/tests/data/__init__.py
--rw-r--r--   0        0        0     2290 2023-05-29 15:18:35.939637 gwcelery-2.1.1/gwcelery/tests/data/agile_grb_gcn.xml
--rw-r--r--   0        0        0   854036 2023-05-29 15:18:35.943637 gwcelery-2.1.1/gwcelery/tests/data/coinc.xml
--rw-r--r--   0        0        0     6175 2023-05-29 15:18:35.943637 gwcelery-2.1.1/gwcelery/tests/data/externaltrigger_original_data.xml
--rw-r--r--   0        0        0     5482 2023-05-29 15:18:35.943637 gwcelery-2.1.1/gwcelery/tests/data/fermi_grb_gcn.xml
--rw-r--r--   0        0        0     5469 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fermi_initial_grb_gcn.xml
--rw-r--r--   0        0        0     5865 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fermi_noise_gcn.xml
--rw-r--r--   0        0        0     5864 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fermi_noise_gcn_2.xml
--rw-r--r--   0        0        0     4914 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
--rw-r--r--   0        0        0     4914 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
--rw-r--r--   0        0        0     3407 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/fits_header_result.html
--rw-r--r--   0        0        0      882 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/gracedb_externaltrigger_log.json
--rw-r--r--   0        0        0      446 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/gracedb_setrigger_log.json
--rw-r--r--   0        0        0      870 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_detchar.json
--rw-r--r--   0        0        0     2025 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_exttrig_creation.json
--rw-r--r--   0        0        0     2007 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
--rw-r--r--   0        0        0      166 2023-05-29 15:18:35.944637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_fits.json
--rw-r--r--   0        0        0      101 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_label_dqv.json
--rw-r--r--   0        0        0      743 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_psd.json
--rw-r--r--   0        0        0     2020 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_snews_creation.json
--rw-r--r--   0        0        0     2012 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_snews_test_creation.json
--rw-r--r--   0        0        0     2028 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_subgrb_creation.json
--rw-r--r--   0        0        0     1235 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_superevent_creation.json
--rw-r--r--   0        0        0      107 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_superevent_label.json
--rw-r--r--   0        0        0     5021 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_voevent.json
--rw-r--r--   0        0        0     4429 2023-05-29 15:18:35.945637 gwcelery-2.1.1/gwcelery/tests/data/integral_grb_gcn.xml
--rw-r--r--   0        0        0     4295 2023-05-29 15:18:35.946637 gwcelery-2.1.1/gwcelery/tests/data/integral_mdc_gcn.xml
--rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/__init__.py
--rw-r--r--   0        0        0    14614 2023-05-29 15:18:35.946637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/fail/L1/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/fail/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/omegascan/__init__.py
--rw-r--r--   0        0        0   516419 2023-05-29 15:18:35.948637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
--rw-r--r--   0        0        0    14630 2023-05-29 15:18:35.949637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/pass/H1/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 15:18:36.004637 gwcelery-2.1.1/gwcelery/tests/data/llhoft/pass/__init__.py
--rw-r--r--   0        0        0    13099 2023-05-29 15:18:35.949637 gwcelery-2.1.1/gwcelery/tests/data/lvalert_event_creation.json
--rw-r--r--   0        0        0     9060 2023-05-29 15:18:35.949637 gwcelery-2.1.1/gwcelery/tests/data/lvalert_xmpp.xml
--rw-r--r--   0        0        0      864 2023-05-29 15:18:35.949637 gwcelery-2.1.1/gwcelery/tests/data/mock_superevent_object.json
--rw-r--r--   0        0        0   445440 2023-05-29 15:18:35.951637 gwcelery-2.1.1/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
--rw-r--r--   0        0        0   294426 2023-05-29 15:18:35.952637 gwcelery-2.1.1/gwcelery/tests/data/psd.xml.gz
--rw-r--r--   0        0        0    11520 2023-05-29 15:18:35.952637 gwcelery-2.1.1/gwcelery/tests/data/rrt_small_area.fits
--rw-r--r--   0        0        0     2964 2023-05-29 15:18:35.952637 gwcelery-2.1.1/gwcelery/tests/data/sample_events.json
--rw-r--r--   0        0        0     3648 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/samples.hdf5
--rw-r--r--   0        0        0      616 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/scaler_set_all.pickle
--rw-r--r--   0        0        0     6169 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/snews_gcn.xml
--rw-r--r--   0        0        0     6161 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/snews_gcn_test.xml
--rw-r--r--   0        0        0     9583 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/superevents.json
--rw-r--r--   0        0        0     7713 2023-05-29 15:18:35.953637 gwcelery-2.1.1/gwcelery/tests/data/swift_grb_gcn.xml
--rw-r--r--   0        0        0   581918 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/data/test_classifier.pickle
--rw-r--r--   0        0        0     4042 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/process.py
--rw-r--r--   0        0        0     2307 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/test_sentry.py
--rw-r--r--   0        0        0     1705 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/test_tasks_alerts.py
--rw-r--r--   0        0        0     4916 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/test_tasks_alerts_validate.py
--rw-r--r--   0        0        0     1439 2023-05-29 15:18:35.955637 gwcelery-2.1.1/gwcelery/tests/test_tasks_bayestar.py
--rw-r--r--   0        0        0     3007 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_circulars.py
--rw-r--r--   0        0        0     4550 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_condor.py
--rw-r--r--   0        0        0    15811 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_detchar.py
--rw-r--r--   0        0        0     2317 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_em_bright.py
--rw-r--r--   0        0        0    12322 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_external_skymaps.py
--rw-r--r--   0        0        0    34773 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_external_triggers.py
--rw-r--r--   0        0        0     1816 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_first2years.py
--rw-r--r--   0        0        0     4555 2023-05-29 15:18:35.956637 gwcelery-2.1.1/gwcelery/tests/test_tasks_first2years_external.py
--rw-r--r--   0        0        0     1826 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_gcn.py
--rw-r--r--   0        0        0     1655 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_gcn_validate.py
--rw-r--r--   0        0        0     5739 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_gracedb.py
--rw-r--r--   0        0        0     9591 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_gwskynet.py
--rw-r--r--   0        0        0     3662 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_igwn_alert.py
--rw-r--r--   0        0        0    22955 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_inference.py
--rw-r--r--   0        0        0    33299 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_orchestrator.py
--rw-r--r--   0        0        0     1647 2023-05-29 15:18:35.957637 gwcelery-2.1.1/gwcelery/tests/test_tasks_p_astro.py
--rw-r--r--   0        0        0    25523 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tasks_raven.py
--rw-r--r--   0        0        0     4724 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tasks_rrt_utils.py
--rw-r--r--   0        0        0     5035 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tasks_skymaps.py
--rw-r--r--   0        0        0    40127 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tasks_superevents.py
--rw-r--r--   0        0        0      637 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tempfile.py
--rw-r--r--   0        0        0     3520 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tools_condor.py
--rw-r--r--   0        0        0     1098 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tools_condor_submit_helper.py
--rw-r--r--   0        0        0      633 2023-05-29 15:18:35.958637 gwcelery-2.1.1/gwcelery/tests/test_tools_flask.py
--rw-r--r--   0        0        0     9668 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tests/test_tools_nagios.py
--rw-r--r--   0        0        0      269 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tests/test_util.py
--rw-r--r--   0        0        0    22392 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tests/test_views.py
--rw-r--r--   0        0        0      216 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tools/__init__.py
--rw-r--r--   0        0        0     2948 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tools/condor.py
--rw-r--r--   0        0        0     1120 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tools/condor_submit_helper.py
--rw-r--r--   0        0        0     1938 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tools/flask.py
--rw-r--r--   0        0        0     6624 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/tools/nagios.py
--rw-r--r--   0        0        0      413 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/__init__.py
--rw-r--r--   0        0        0     1007 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/cmdline.py
--rw-r--r--   0        0        0      453 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/matplotlib.py
--rw-r--r--   0        0        0      390 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/proxy.py
--rw-r--r--   0        0        0      514 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/resources.py
--rw-r--r--   0        0        0      253 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/sphinx.py
--rw-r--r--   0        0        0      941 2023-05-29 15:18:35.959637 gwcelery-2.1.1/gwcelery/util/tempfile.py
--rw-r--r--   0        0        0    19058 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/views.py
--rw-r--r--   0        0        0      365 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/__init__.py
--rw-r--r--   0        0        0     6387 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/bootsteps.py
--rw-r--r--   0        0        0     1063 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/logging.py
--rw-r--r--   0        0        0      779 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/signals.py
--rw-r--r--   0        0        0      852 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/subscriber.py
--rw-r--r--   0        0        0     1454 2023-05-29 15:18:35.960637 gwcelery-2.1.1/gwcelery/voevent/util.py
--rw-r--r--   0        0        0     6099 2023-05-29 15:18:46.862686 gwcelery-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     4525 1970-01-01 00:00:00.000000 gwcelery-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    96823 2023-06-09 18:39:41.376572 gwcelery-2.1.2/CHANGES.rst
+-rw-r--r--   0        0        0       64 2023-06-09 18:39:41.376572 gwcelery-2.1.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    19716 2023-06-09 18:39:41.377572 gwcelery-2.1.2/LICENSE.rst
+-rw-r--r--   0        0        0     1351 2023-06-09 18:39:41.377572 gwcelery-2.1.2/README.rst
+-rw-r--r--   0        0        0      634 2023-06-09 18:39:41.377572 gwcelery-2.1.2/doc/Makefile
+-rw-r--r--   0        0        0   191486 2023-06-09 18:39:41.379572 gwcelery-2.1.2/doc/_static/acceptance-tests-checklist.png
+-rw-r--r--   0        0        0   241593 2023-06-09 18:39:41.380572 gwcelery-2.1.2/doc/_static/celeryevent-screenshot.png
+-rw-r--r--   0        0        0   206465 2023-06-09 18:39:41.382572 gwcelery-2.1.2/doc/_static/deployment-screenshot.png
+-rw-r--r--   0        0        0   161306 2023-06-09 18:39:41.383572 gwcelery-2.1.2/doc/_static/flask-screenshot.png
+-rw-r--r--   0        0        0   328056 2023-06-09 18:39:41.386572 gwcelery-2.1.2/doc/_static/flower-screenshot.png
+-rw-r--r--   0        0        0   114719 2023-06-09 18:39:41.387572 gwcelery-2.1.2/doc/_static/logo-0.5x.png
+-rw-r--r--   0        0        0   351955 2023-06-09 18:39:41.390572 gwcelery-2.1.2/doc/_static/logo.png
+-rw-r--r--   0        0        0   230777 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/_static/sentry-screenshot.png
+-rwxr-xr-x   0        0        0     7356 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/conf.py
+-rw-r--r--   0        0        0     4346 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/configuration.rst
+-rw-r--r--   0        0        0     5698 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/contributing.rst
+-rw-r--r--   0        0        0     7202 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/deployment.rst
+-rw-r--r--   0        0        0    10176 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/design.rst
+-rw-r--r--   0        0        0      486 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/gwcelery.conf.rst
+-rw-r--r--   0        0        0      284 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.email.rst
+-rw-r--r--   0        0        0      329 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.igwn_alert.rst
+-rw-r--r--   0        0        0      227 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.rst
+-rw-r--r--   0        0        0       79 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.sentry.rst
+-rw-r--r--   0        0        0       97 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.alerts.rst
+-rw-r--r--   0        0        0      103 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.bayestar.rst
+-rw-r--r--   0        0        0      107 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.circulars.rst
+-rw-r--r--   0        0        0       98 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.condor.rst
+-rw-r--r--   0        0        0     2404 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.detchar.rst
+-rw-r--r--   0        0        0     1110 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.em_bright.rst
+-rw-r--r--   0        0        0      129 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.external_skymaps.rst
+-rw-r--r--   0        0        0     6738 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.external_triggers.rst
+-rw-r--r--   0        0        0      112 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.first2years.rst
+-rw-r--r--   0        0        0       88 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.gcn.rst
+-rw-r--r--   0        0        0      100 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.gracedb.rst
+-rw-r--r--   0        0        0      109 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.igwn_alert.rst
+-rw-r--r--   0        0        0      109 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.inference.rst
+-rw-r--r--   0        0        0     8111 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.orchestrator.rst
+-rw-r--r--   0        0        0      100 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.p_astro.rst
+-rw-r--r--   0        0        0       94 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.raven.rst
+-rw-r--r--   0        0        0      628 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.rst
+-rw-r--r--   0        0        0      100 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.skymaps.rst
+-rw-r--r--   0        0        0     7161 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.superevents.rst
+-rw-r--r--   0        0        0       97 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tools.condor.rst
+-rw-r--r--   0        0        0       94 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tools.flask.rst
+-rw-r--r--   0        0        0       97 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/gwcelery.tools.nagios.rst
+-rw-r--r--   0        0        0      185 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/gwcelery.tools.rst
+-rw-r--r--   0        0        0       73 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/gwcelery.util.rst
+-rw-r--r--   0        0        0      507 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/gwcelery.voevent.rst
+-rw-r--r--   0        0        0     3564 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/htcondor.rst
+-rw-r--r--   0        0        0     1576 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/index.rst
+-rw-r--r--   0        0        0      800 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/make.bat
+-rw-r--r--   0        0        0     4416 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/monitoring.rst
+-rw-r--r--   0        0        0     5312 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/quickstart.rst
+-rw-r--r--   0        0        0     1149 2023-06-09 18:39:41.395572 gwcelery-2.1.2/gwcelery/__init__.py
+-rw-r--r--   0        0        0    18447 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/_version.py
+-rw-r--r--   0        0        0    16230 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/__init__.py
+-rw-r--r--   0        0        0     1014 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/dev.py
+-rw-r--r--   0        0        0      403 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/development.py
+-rw-r--r--   0        0        0     1289 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/minikube.py
+-rw-r--r--   0        0        0     1865 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/playground.py
+-rw-r--r--   0        0        0     3541 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/production.py
+-rw-r--r--   0        0        0     2040 2023-06-09 18:39:41.397572 gwcelery-2.1.2/gwcelery/conf/test.py
+-rw-r--r--   0        0        0        0 2023-06-09 18:39:41.477573 gwcelery-2.1.2/gwcelery/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 18:39:41.478573 gwcelery-2.1.2/gwcelery/data/first2years/__init__.py
+-rw-r--r--   0        0        0   731421 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/data/first2years/gstlal.xml.gz
+-rwxr-xr-x   0        0        0     2809 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/data/gwcelery.sub
+-rw-r--r--   0        0        0      505 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/email/__init__.py
+-rw-r--r--   0        0        0     3317 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/email/bootsteps.py
+-rw-r--r--   0        0        0      995 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/email/signals.py
+-rw-r--r--   0        0        0     1457 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/flask.py
+-rw-r--r--   0        0        0      529 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/igwn_alert/__init__.py
+-rw-r--r--   0        0        0     4484 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/igwn_alert/bootsteps.py
+-rw-r--r--   0        0        0      608 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/igwn_alert/signals.py
+-rw-r--r--   0        0        0      275 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/jinja.py
+-rw-r--r--   0        0        0      305 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/kafka/__init__.py
+-rw-r--r--   0        0        0    10652 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/kafka/bootsteps.py
+-rw-r--r--   0        0        0      522 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/kafka/signals.py
+-rw-r--r--   0        0        0     2567 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/sentry/__init__.py
+-rw-r--r--   0        0        0       34 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/sentry/integrations/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/sentry/integrations/condor.py
+-rw-r--r--   0        0        0      836 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/sentry/integrations/requests.py
+-rw-r--r--   0        0        0      939 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/sentry/integrations/subprocess.py
+-rw-r--r--   0        0        0     1302 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/static/typeahead.css
+-rw-r--r--   0        0        0     4124 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/static/vega/index.html
+-rw-r--r--   0        0        0      515 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/tasks/__init__.py
+-rw-r--r--   0        0        0    13597 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/tasks/alerts.py
+-rw-r--r--   0        0        0     2672 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/tasks/bayestar.py
+-rw-r--r--   0        0        0     1535 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/tasks/circulars.py
+-rw-r--r--   0        0        0     7502 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/tasks/condor.py
+-rw-r--r--   0        0        0     2692 2023-06-09 18:39:41.403572 gwcelery-2.1.2/gwcelery/tasks/core.py
+-rw-r--r--   0        0        0    23014 2023-06-09 18:39:41.403572 gwcelery-2.1.2/gwcelery/tasks/detchar.py
+-rw-r--r--   0        0        0     4863 2023-06-09 18:39:41.403572 gwcelery-2.1.2/gwcelery/tasks/em_bright.py
+-rw-r--r--   0        0        0    21775 2023-06-09 18:39:41.403572 gwcelery-2.1.2/gwcelery/tasks/external_skymaps.py
+-rw-r--r--   0        0        0    23705 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/external_triggers.py
+-rw-r--r--   0        0        0     6832 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/first2years.py
+-rw-r--r--   0        0        0     6320 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/first2years_external.py
+-rw-r--r--   0        0        0     4831 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/gcn.py
+-rw-r--r--   0        0        0    11079 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/gracedb.py
+-rw-r--r--   0        0        0     6105 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/gwskynet.py
+-rw-r--r--   0        0        0     2453 2023-06-09 18:39:41.405572 gwcelery-2.1.2/gwcelery/tasks/igwn_alert.py
+-rw-r--r--   0        0        0    33507 2023-06-09 18:39:41.405572 gwcelery-2.1.2/gwcelery/tasks/inference.py
+-rw-r--r--   0        0        0     1406 2023-06-09 18:39:41.405572 gwcelery-2.1.2/gwcelery/tasks/legacy_gracedb.py
+-rw-r--r--   0        0        0     7772 2023-06-09 18:39:41.405572 gwcelery-2.1.2/gwcelery/tasks/notice_text.py
+-rw-r--r--   0        0        0    47203 2023-06-09 18:39:41.406572 gwcelery-2.1.2/gwcelery/tasks/orchestrator.py
+-rw-r--r--   0        0        0     5796 2023-06-09 18:39:41.406572 gwcelery-2.1.2/gwcelery/tasks/p_astro.py
+-rw-r--r--   0        0        0    20783 2023-06-09 18:39:41.406572 gwcelery-2.1.2/gwcelery/tasks/raven.py
+-rw-r--r--   0        0        0     2242 2023-06-09 18:39:41.406572 gwcelery-2.1.2/gwcelery/tasks/rrt_utils.py
+-rw-r--r--   0        0        0    12528 2023-06-09 18:39:41.407572 gwcelery-2.1.2/gwcelery/tasks/skymaps.py
+-rw-r--r--   0        0        0    23631 2023-06-09 18:39:41.407572 gwcelery-2.1.2/gwcelery/tasks/superevents.py
+-rw-r--r--   0        0        0     1084 2023-06-09 18:39:41.407572 gwcelery-2.1.2/gwcelery/templates/fits_header.jinja2
+-rw-r--r--   0        0        0    35556 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/templates/index.jinja2
+-rw-r--r--   0        0        0     8505 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/templates/lalinference.jinja2
+-rw-r--r--   0        0        0     9511 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/templates/rapidpe.jinja2
+-rw-r--r--   0        0        0      472 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/templates/vector_table.jinja2
+-rw-r--r--   0        0        0        0 2023-06-09 18:39:41.480573 gwcelery-2.1.2/gwcelery/tests/__init__.py
+-rw-r--r--   0        0        0     4388 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/tests/conftest.py
+-rw-r--r--   0        0        0      976 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/tests/data/G000012_S0040_preferred.json
+-rw-r--r--   0        0        0     6258 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/tests/data/G298048-1-Initial.xml
+-rw-r--r--   0        0        0      599 2023-06-09 18:39:41.409572 gwcelery-2.1.2/gwcelery/tests/data/G298048_log.json
+-rw-r--r--   0        0        0      150 2023-06-09 18:39:41.409572 gwcelery-2.1.2/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
+-rw-r--r--   0        0        0      974 2023-06-09 18:39:41.409572 gwcelery-2.1.2/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
+-rw-r--r--   0        0        0    17572 2023-06-09 18:39:41.409572 gwcelery-2.1.2/gwcelery/tests/data/MS220722v.xml
+-rw-r--r--   0        0        0   777600 2023-06-09 18:39:41.415572 gwcelery-2.1.2/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
+-rw-r--r--   0        0        0     8220 2023-06-09 18:39:41.415572 gwcelery-2.1.2/gwcelery/tests/data/S230413b.json
+-rw-r--r--   0        0        0     7255 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/S230413g.json
+-rw-r--r--   0        0        0     7721 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/S230413h.json
+-rw-r--r--   0        0        0     3387 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/T0212_S0039_preferred.json
+-rw-r--r--   0        0        0     3384 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
+-rw-r--r--   0        0        0     5210 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/T0219_S0041_nopreferred.json
+-rw-r--r--   0        0        0        0 2023-06-09 18:39:41.481573 gwcelery-2.1.2/gwcelery/tests/data/__init__.py
+-rw-r--r--   0        0        0     2290 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/agile_grb_gcn.xml
+-rw-r--r--   0        0        0   854036 2023-06-09 18:39:41.422572 gwcelery-2.1.2/gwcelery/tests/data/coinc.xml
+-rw-r--r--   0        0        0     6175 2023-06-09 18:39:41.422572 gwcelery-2.1.2/gwcelery/tests/data/externaltrigger_original_data.xml
+-rw-r--r--   0        0        0     5482 2023-06-09 18:39:41.422572 gwcelery-2.1.2/gwcelery/tests/data/fermi_grb_gcn.xml
+-rw-r--r--   0        0        0     5469 2023-06-09 18:39:41.422572 gwcelery-2.1.2/gwcelery/tests/data/fermi_initial_grb_gcn.xml
+-rw-r--r--   0        0        0     5865 2023-06-09 18:39:41.422572 gwcelery-2.1.2/gwcelery/tests/data/fermi_noise_gcn.xml
+-rw-r--r--   0        0        0     5864 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/fermi_noise_gcn_2.xml
+-rw-r--r--   0        0        0     4914 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
+-rw-r--r--   0        0        0     4914 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
+-rw-r--r--   0        0        0     3407 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/fits_header_result.html
+-rw-r--r--   0        0        0      882 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/gracedb_externaltrigger_log.json
+-rw-r--r--   0        0        0      446 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/gracedb_setrigger_log.json
+-rw-r--r--   0        0        0      870 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_detchar.json
+-rw-r--r--   0        0        0     2025 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_exttrig_creation.json
+-rw-r--r--   0        0        0     2007 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
+-rw-r--r--   0        0        0      166 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_fits.json
+-rw-r--r--   0        0        0      101 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_label_dqv.json
+-rw-r--r--   0        0        0      743 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_psd.json
+-rw-r--r--   0        0        0     2020 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_snews_creation.json
+-rw-r--r--   0        0        0     2012 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_snews_test_creation.json
+-rw-r--r--   0        0        0     2028 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_subgrb_creation.json
+-rw-r--r--   0        0        0     1235 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_superevent_creation.json
+-rw-r--r--   0        0        0      107 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_superevent_label.json
+-rw-r--r--   0        0        0     5021 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_voevent.json
+-rw-r--r--   0        0        0     4429 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/integral_grb_gcn.xml
+-rw-r--r--   0        0        0     4295 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/integral_mdc_gcn.xml
+-rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/__init__.py
+-rw-r--r--   0        0        0     8267 2023-06-09 18:39:41.425572 gwcelery-2.1.2/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/fail/L1/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/fail/__init__.py
+-rw-r--r--   0        0        0    14942 2023-06-09 18:39:41.425572 gwcelery-2.1.2/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/omegascan/__init__.py
+-rw-r--r--   0        0        0   516419 2023-06-09 18:39:41.426572 gwcelery-2.1.2/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
+-rw-r--r--   0        0        0    14950 2023-06-09 18:39:41.427572 gwcelery-2.1.2/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/pass/H1/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/pass/__init__.py
+-rw-r--r--   0        0        0    13099 2023-06-09 18:39:41.427572 gwcelery-2.1.2/gwcelery/tests/data/lvalert_event_creation.json
+-rw-r--r--   0        0        0     9060 2023-06-09 18:39:41.427572 gwcelery-2.1.2/gwcelery/tests/data/lvalert_xmpp.xml
+-rw-r--r--   0        0        0      864 2023-06-09 18:39:41.427572 gwcelery-2.1.2/gwcelery/tests/data/mock_superevent_object.json
+-rw-r--r--   0        0        0   445440 2023-06-09 18:39:41.429572 gwcelery-2.1.2/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
+-rw-r--r--   0        0        0   294426 2023-06-09 18:39:41.430572 gwcelery-2.1.2/gwcelery/tests/data/psd.xml.gz
+-rw-r--r--   0        0        0    11520 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/rrt_small_area.fits
+-rw-r--r--   0        0        0     2964 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/sample_events.json
+-rw-r--r--   0        0        0     3648 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/samples.hdf5
+-rw-r--r--   0        0        0      616 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/scaler_set_all.pickle
+-rw-r--r--   0        0        0     6169 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/snews_gcn.xml
+-rw-r--r--   0        0        0     6161 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/snews_gcn_test.xml
+-rw-r--r--   0        0        0     9583 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/superevents.json
+-rw-r--r--   0        0        0     7713 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/swift_grb_gcn.xml
+-rw-r--r--   0        0        0   581918 2023-06-09 18:39:41.434573 gwcelery-2.1.2/gwcelery/tests/data/test_classifier.pickle
+-rw-r--r--   0        0        0     4042 2023-06-09 18:39:41.434573 gwcelery-2.1.2/gwcelery/tests/process.py
+-rw-r--r--   0        0        0     2307 2023-06-09 18:39:41.434573 gwcelery-2.1.2/gwcelery/tests/test_sentry.py
+-rw-r--r--   0        0        0     1705 2023-06-09 18:39:41.434573 gwcelery-2.1.2/gwcelery/tests/test_tasks_alerts.py
+-rw-r--r--   0        0        0     4916 2023-06-09 18:39:41.434573 gwcelery-2.1.2/gwcelery/tests/test_tasks_alerts_validate.py
+-rw-r--r--   0        0        0     1439 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_bayestar.py
+-rw-r--r--   0        0        0     3007 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_circulars.py
+-rw-r--r--   0        0        0     4550 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_condor.py
+-rw-r--r--   0        0        0    16937 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_detchar.py
+-rw-r--r--   0        0        0     2317 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_em_bright.py
+-rw-r--r--   0        0        0    12322 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_external_skymaps.py
+-rw-r--r--   0        0        0    34773 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_external_triggers.py
+-rw-r--r--   0        0        0     1816 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_first2years.py
+-rw-r--r--   0        0        0     4555 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_first2years_external.py
+-rw-r--r--   0        0        0     1826 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_gcn.py
+-rw-r--r--   0        0        0     1655 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_gcn_validate.py
+-rw-r--r--   0        0        0     5739 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_gracedb.py
+-rw-r--r--   0        0        0     9591 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_gwskynet.py
+-rw-r--r--   0        0        0     3662 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_igwn_alert.py
+-rw-r--r--   0        0        0    24398 2023-06-09 18:39:41.437573 gwcelery-2.1.2/gwcelery/tests/test_tasks_inference.py
+-rw-r--r--   0        0        0    33486 2023-06-09 18:39:41.437573 gwcelery-2.1.2/gwcelery/tests/test_tasks_orchestrator.py
+-rw-r--r--   0        0        0     1647 2023-06-09 18:39:41.437573 gwcelery-2.1.2/gwcelery/tests/test_tasks_p_astro.py
+-rw-r--r--   0        0        0    25523 2023-06-09 18:39:41.437573 gwcelery-2.1.2/gwcelery/tests/test_tasks_raven.py
+-rw-r--r--   0        0        0     4724 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tasks_rrt_utils.py
+-rw-r--r--   0        0        0     5035 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tasks_skymaps.py
+-rw-r--r--   0        0        0    40274 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tasks_superevents.py
+-rw-r--r--   0        0        0      637 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tempfile.py
+-rw-r--r--   0        0        0     3520 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tools_condor.py
+-rw-r--r--   0        0        0     1098 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tools_condor_submit_helper.py
+-rw-r--r--   0        0        0      633 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tools_flask.py
+-rw-r--r--   0        0        0     9668 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tests/test_tools_nagios.py
+-rw-r--r--   0        0        0      269 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tests/test_util.py
+-rw-r--r--   0        0        0    22656 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tests/test_views.py
+-rw-r--r--   0        0        0      216 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tools/__init__.py
+-rw-r--r--   0        0        0     2948 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tools/condor.py
+-rw-r--r--   0        0        0     1120 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tools/condor_submit_helper.py
+-rw-r--r--   0        0        0     1938 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tools/flask.py
+-rw-r--r--   0        0        0     6624 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tools/nagios.py
+-rw-r--r--   0        0        0      413 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/util/__init__.py
+-rw-r--r--   0        0        0     1007 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/util/cmdline.py
+-rw-r--r--   0        0        0      453 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/util/matplotlib.py
+-rw-r--r--   0        0        0      390 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/util/proxy.py
+-rw-r--r--   0        0        0      514 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/util/resources.py
+-rw-r--r--   0        0        0      253 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/util/sphinx.py
+-rw-r--r--   0        0        0      941 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/util/tempfile.py
+-rw-r--r--   0        0        0    19407 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/views.py
+-rw-r--r--   0        0        0      365 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/voevent/__init__.py
+-rw-r--r--   0        0        0     6387 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/voevent/bootsteps.py
+-rw-r--r--   0        0        0     1063 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/voevent/logging.py
+-rw-r--r--   0        0        0      779 2023-06-09 18:39:41.441573 gwcelery-2.1.2/gwcelery/voevent/signals.py
+-rw-r--r--   0        0        0      852 2023-06-09 18:39:41.441573 gwcelery-2.1.2/gwcelery/voevent/subscriber.py
+-rw-r--r--   0        0        0     1454 2023-06-09 18:39:41.441573 gwcelery-2.1.2/gwcelery/voevent/util.py
+-rw-r--r--   0        0        0     6107 2023-06-09 18:39:53.695639 gwcelery-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4524 1970-01-01 00:00:00.000000 gwcelery-2.1.2/PKG-INFO
```

### Comparing `gwcelery-2.1.1/CHANGES.rst` & `gwcelery-2.1.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,56 @@
 Changelog
 =========
 
+2.1.2 "Ogopogo" (2023-06-09)
+----------------------------
+
+-   Update the low-significance threshold to be 2/day pre-trials factor. Update
+    low-siginificance trials factors to 7.
+
+-   Do not apply HIGH_PROFILE label to less-significant alerts.
+
+-   Do not make pe skymap public automatically before approved.
+
+-   Make image created when omegascan fails smaller.
+
+-   Remove "overall state of detectors" line from detchar vector table,
+    since without Virgo being online it will always be "bad".
+
+-   Check the iDQ OK vector before checking the value of iDQ timeseries.
+
+-   Upgrade bilby_pipe to v1.1.1.
+
+-   Enable SCiMMA kafka on minikube.
+
+-   Use real KafkaError methods in delivery callback.
+
+-   Use production accounting tag for bilby running on real events.
+
+-   Disable querying data before starting PE as bilby now uses kafka data
+    stream and PE timeout is long enough for low-latency frame data to be
+    produced.
+
+-   Move RAVEN tasks to main worker and make GCN ingestion sequential.
+
+-   Update low-significance FAR threshold and trials factors to ensure these
+    will go out at a rate of 2/day pre-trials factors.
+
+-   Limit the number of MDC BBH bilby jobs to less than 5 to save disk usage.
+
+-   Upgrade lalsuite to v7.15.
+
+-   Updated rapidpe-rift-pipe version to 0.5.1. rapidpe will be
+    submitted on superevents with gstlal/non-gstlal preferred event.
+    Launching rapidpe 30s after merger. `query_shm=True` will run on lower
+    latency data on `/dev/shm/kafka/` if it is available, if not it will
+    default to `/ifocache/llcache/kafka/`.
+
+-   When updating the preferred event, also update t_0.
+
 2.1.1 "Lone Island Mountain Devil" (2023-05-29)
 -----------------------------------------------
 
 -   Upgrade ligo-followup-advocate to v1.2.3
 
 -   Bump ligo.em-bright to v1.1.3 to be compatible with schema of online PE
     files with spinning waveforms.
```

### Comparing `gwcelery-2.1.1/LICENSE.rst` & `gwcelery-2.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/README.rst` & `gwcelery-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/Makefile` & `gwcelery-2.1.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/_static/acceptance-tests-checklist.png` & `gwcelery-2.1.2/doc/_static/acceptance-tests-checklist.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/_static/celeryevent-screenshot.png` & `gwcelery-2.1.2/doc/_static/celeryevent-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/_static/deployment-screenshot.png` & `gwcelery-2.1.2/doc/_static/deployment-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/_static/flask-screenshot.png` & `gwcelery-2.1.2/doc/_static/flask-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/_static/flower-screenshot.png` & `gwcelery-2.1.2/doc/_static/flower-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/_static/logo-0.5x.png` & `gwcelery-2.1.2/doc/_static/logo-0.5x.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/_static/logo.png` & `gwcelery-2.1.2/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/_static/sentry-screenshot.png` & `gwcelery-2.1.2/doc/_static/sentry-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/conf.py` & `gwcelery-2.1.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/configuration.rst` & `gwcelery-2.1.2/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/contributing.rst` & `gwcelery-2.1.2/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/deployment.rst` & `gwcelery-2.1.2/doc/deployment.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/design.rst` & `gwcelery-2.1.2/doc/design.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/gwcelery.tasks.detchar.rst` & `gwcelery-2.1.2/doc/gwcelery.tasks.detchar.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/gwcelery.tasks.em_bright.rst` & `gwcelery-2.1.2/doc/gwcelery.tasks.em_bright.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/gwcelery.tasks.external_triggers.rst` & `gwcelery-2.1.2/doc/gwcelery.tasks.external_triggers.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/gwcelery.tasks.orchestrator.rst` & `gwcelery-2.1.2/doc/gwcelery.tasks.orchestrator.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/gwcelery.tasks.rst` & `gwcelery-2.1.2/doc/gwcelery.tasks.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/gwcelery.tasks.superevents.rst` & `gwcelery-2.1.2/doc/gwcelery.tasks.superevents.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/htcondor.rst` & `gwcelery-2.1.2/doc/htcondor.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/index.rst` & `gwcelery-2.1.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/make.bat` & `gwcelery-2.1.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/monitoring.rst` & `gwcelery-2.1.2/doc/monitoring.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/doc/quickstart.rst` & `gwcelery-2.1.2/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/__init__.py` & `gwcelery-2.1.2/gwcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/_version.py` & `gwcelery-2.1.2/gwcelery/_version.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/conf/__init__.py` & `gwcelery-2.1.2/gwcelery/conf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,35 +145,39 @@
 
 significant_alert_far_threshold = {'cbc': 1 / (30 * 86400),
                                    'burst': 1 / (365 * 86400),
                                    'test': 1 / (30 * 86400)}
 """Group specific maximum false alarm rate to consider
 sending significant alerts."""
 
-preliminary_alert_far_threshold = {'cbc': 2 / (1 * 86400),
-                                   'burst': 2 / (1 * 86400),
-                                   'test': 2 / (1 * 86400)}
-"""Group specific maximum false alarm rate to consider
-sending less significant alerts."""
-
 early_warning_alert_trials_factor = 4.0
 """Trials factor for early warning alerts. There are two pipelines that are
 producing early warning events: gstlal and spiir."""
 
 early_warning_alert_far_threshold = 1 / (30 * 86400)
 """False alarm rate threshold for significant early warning alerts."""
 
 significant_alert_trials_factor = dict(cbc=5.0, burst=4.0)
 """Trials factor corresponding to trigger categories. For CBC and Burst, trials
 factor is the number of pipelines. CBC pipelines are gstlal, pycbc, mbta and
 spiir. Burst searches are cwb.allsky, cwb.imbh, and olib."""
 
-preliminary_alert_trials_factor = dict(cbc=8.0, burst=8.0)
+preliminary_alert_trials_factor = dict(cbc=7.0, burst=7.0)
 """Trials factor for less significant alerts."""
 
+preliminary_alert_far_threshold = {
+    'cbc': 2 / (1 * 86400) * preliminary_alert_trials_factor['cbc'],
+    'burst': 2 / (1 * 86400) * preliminary_alert_trials_factor['burst'],
+    'test': 2 / (1 * 86400) * preliminary_alert_trials_factor['cbc']
+}
+"""Group specific maximum false alarm rate to consider sending less significant
+alerts. Trials factors are included here to ensure events are sent with the
+false alarm rate initially listed and removing trials factors are from the
+threshold calculation."""
+
 snews_gw_far_threshold = 1 / (3600 * 24)
 """Maximum false alarm rate for a superevent to send out a coincidence alert
 between an external SNEWS alert and the superevent."""
 
 sog_paper_far_threshold = {'gw': 1 / (10 * 365 * 86400),
                            'joint': 1 / (10000 * 365 * 86400)}
 """False alarm rate thresholds for producing a manuscript of speed of gravity
@@ -185,14 +189,20 @@
 event out of the accumulated events."""
 
 pe_timeout = 345.0
 """The orchestrator will wait this many seconds from the time of the
 creation of a new superevent to the time that parameter estimation begins, in
 case the preferred event is updated with high latency."""
 
+rapidpe_timeout = 30.0
+"""The orchestrator will wait this many seconds from the time of the
+creation of a new superevent to the time rapidpe parameter estimation begins,
+in case the preferred event is updated with high latency."""
+
+
 check_vector_prepost = {'gstlal': [2, 2],
                         'spiir': [2, 2],
                         'pycbc': [2, 2],
                         'MBTA': [2, 2],
                         'oLIB': [1.5, 1.5],
                         'LIB': [1.5, 1.5],
                         'CWB': [1.5, 1.5],
@@ -233,14 +243,18 @@
     'L1:DMT-DQ_VECTOR': 'dmt_dq_vector_bits',
     'H1:GDS-CALIB_STATE_VECTOR': 'ligo_state_vector_bits',
     'L1:GDS-CALIB_STATE_VECTOR': 'ligo_state_vector_bits',
     'V1:DQ_ANALYSIS_STATE_VECTOR': 'virgo_state_vector_bits'}
 """Low-latency h(t) state vector configuration. This is a dictionary consisting
 of a channel and its bitmask, as defined in :mod:`gwcelery.tasks.detchar`."""
 
+idq_ok_channels = ['H1:IDQ-OK_OVL_10_2048',
+                   'L1:IDQ-OK_OVL_10_2048']
+"""Low-latency iDQ OK channel names for O4. High bit indicates iDQ is ok."""
+
 idq_channels = ['H1:IDQ-FAP_OVL_10_2048',
                 'L1:IDQ-FAP_OVL_10_2048']
 """Low-latency iDQ false alarm probability channel names for O4."""
 
 idq_fap_thresh = 0.01
 """If FAP is below this threshold, and
 :obj:`~gwcelery.conf.idq_veto` for the pipeline is true, DQV will be labeled
```

### Comparing `gwcelery-2.1.1/gwcelery/conf/dev.py` & `gwcelery-2.1.2/gwcelery/conf/dev.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/conf/minikube.py` & `gwcelery-2.1.2/gwcelery/conf/minikube.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,12 +21,19 @@
 early_warning_alert_far_threshold = float('inf')
 """False alarm rate threshold for early warning alerts."""
 
 mock_events_simulate_multiple_uploads = False
 """If True, then upload each mock event several times in rapid succession with
 random jitter in order to simulate multiple pipeline uploads."""
 
+kafka_consumer_config = {
+}
+"""Kafka consumer configuration details. The keys describe the senders of the
+messages to be consumed. The values are a dictionary of the URL to listen to
+and information about the message serializer."""
+
 kafka_alert_config = {
     'scimma': {'url': 'kafka://hopskotch-server/igwn.gwalert-minikube',
-               'suffix': 'avro', 'skymap_encoder': lambda _: _}
+               'suffix': 'avro', 'skymap_encoder': lambda _: _,
+               'auth': False}
 }
 """Kafka broker configuration details"""
```

### Comparing `gwcelery-2.1.1/gwcelery/conf/playground.py` & `gwcelery-2.1.2/gwcelery/conf/playground.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,10 +33,14 @@
 
 voevent_receiver_address = '50.116.49.68:8094'
 """The VOEvent listener will connect to this address to receive GCNs. For
 options, see `GCN's list of available VOEvent servers
 <https://gcn.gsfc.nasa.gov/voevent.html#tc2>`_. If this is an empty string,
 then completely disable the GCN listener."""
 
+idq_ok_channels = ['H1:IDQ-OK_OVL_16_4096',
+                   'L1:IDQ-OK_OVL_16_4096']
+"""Low-latency iDQ OK channel names for O3 replay."""
+
 idq_channels = ['H1:IDQ-FAP_OVL_16_4096',
                 'L1:IDQ-FAP_OVL_16_4096']
 """Low-latency iDQ false alarm probability channel names for O3 replay."""
```

### Comparing `gwcelery-2.1.1/gwcelery/conf/production.py` & `gwcelery-2.1.2/gwcelery/conf/production.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/conf/test.py` & `gwcelery-2.1.2/gwcelery/conf/test.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/data/first2years/gstlal.xml.gz` & `gwcelery-2.1.2/gwcelery/data/first2years/gstlal.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/data/gwcelery.sub` & `gwcelery-2.1.2/gwcelery/data/gwcelery.sub`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # FIXME: The GraceDB tasks are not very computationally intensive, but take a
 # very long time to execute. Manually bump up the concurrency well past the
 # number of hardware threads until the GraceDB API throughput is improved.
 arguments = "gwcelery worker -l info -n gwcelery-worker@%h -f %n.log -Q celery --igwn-alert --email --concurrency 64"
 description = gwcelery-worker
 queue
 
-arguments = "gwcelery worker -l info -n gwcelery-exttrig-worker@%h -f %n.log -Q exttrig -c 1"
+arguments = "gwcelery worker -l info -n gwcelery-exttrig-worker@%h -f %n.log -Q exttrig -c 1 --prefetch-multiplier 1"
 description = gwcelery-exttrig-worker
 queue
 
 arguments = "gwcelery worker -l info -n gwcelery-superevent-worker@%h -f %n.log -Q superevent -c 1 --prefetch-multiplier 1"
 description = gwcelery-superevent-worker
 queue
```

### Comparing `gwcelery-2.1.1/gwcelery/email/bootsteps.py` & `gwcelery-2.1.2/gwcelery/email/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/email/signals.py` & `gwcelery-2.1.2/gwcelery/email/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/flask.py` & `gwcelery-2.1.2/gwcelery/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/igwn_alert/__init__.py` & `gwcelery-2.1.2/gwcelery/igwn_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/igwn_alert/bootsteps.py` & `gwcelery-2.1.2/gwcelery/igwn_alert/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/igwn_alert/signals.py` & `gwcelery-2.1.2/gwcelery/igwn_alert/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/kafka/bootsteps.py` & `gwcelery-2.1.2/gwcelery/kafka/bootsteps.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,20 @@
 
 
 class KafkaBase:
 
     def __init__(self, name, config, prefix):
         self.name = name
         self._config = config
-        self._credential = self.get_auth(prefix)
+        if config.get('auth') is not False:
+            # Users only add auth to config to disable authentication
+            self._credential = self.get_auth(prefix)
+        else:
+            # Dont use credentials
+            self._credential = False
         self._hop_stream = Stream(self._credential)
 
         # FIXME Drop get_payload_content method once
         # https://github.com/scimma/hop-client/pull/190 is merged
         if config['suffix'] == 'avro':
             self.serialization_model = AvroBlobWrapper
             self.get_payload_content = lambda payload: payload.content[0]
@@ -167,17 +172,17 @@
             record = AvroBlob.deserialize(message.value()).content[0]
         else:
             record = JSONBlob.deserialize(message.value()).content
         kafka_url = self._config['url']
         if kafka_error is None:
             self.kafka_delivery_failures = False
         else:
-            log.error(f'Received error code {kafka_error.error_code} '
-                      f'({kafka_error.reason}) when delivering '
-                      f'{record["superevent_id"]} '
+            log.error(f'Received error code {kafka_error.code()} '
+                      f'({kafka_error.name()}, {kafka_error.str()}) '
+                      f'when delivering {record["superevent_id"]} '
                       f'{record["alert_type"]} alert to {kafka_url}')
             self.kafka_delivery_failures = True
 
     def write(self, payload):
         self._open_hop_stream.write(payload,
                                     delivery_callback=self._delivery_cb)
         self._open_hop_stream.flush()
```

### Comparing `gwcelery-2.1.1/gwcelery/kafka/signals.py` & `gwcelery-2.1.2/gwcelery/kafka/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/sentry/__init__.py` & `gwcelery-2.1.2/gwcelery/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/sentry/integrations/condor.py` & `gwcelery-2.1.2/gwcelery/sentry/integrations/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/sentry/integrations/requests.py` & `gwcelery-2.1.2/gwcelery/sentry/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/sentry/integrations/subprocess.py` & `gwcelery-2.1.2/gwcelery/sentry/integrations/subprocess.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/static/typeahead.css` & `gwcelery-2.1.2/gwcelery/static/typeahead.css`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/static/vega/index.html` & `gwcelery-2.1.2/gwcelery/static/vega/index.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/__init__.py` & `gwcelery-2.1.2/gwcelery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/alerts.py` & `gwcelery-2.1.2/gwcelery/tasks/alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/bayestar.py` & `gwcelery-2.1.2/gwcelery/tasks/bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/circulars.py` & `gwcelery-2.1.2/gwcelery/tasks/circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/condor.py` & `gwcelery-2.1.2/gwcelery/tasks/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/core.py` & `gwcelery-2.1.2/gwcelery/tasks/core.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/detchar.py` & `gwcelery-2.1.2/gwcelery/tasks/detchar.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,17 +136,19 @@
         # Do q_transforms for the different durations
         qgrams = [ts.q_transform(
             frange=(20, 4096), gps=t0,
             outseg=(t0 - before, t0 + after), logf=True)
             for before, after in durs]
     except (IndexError, FloatingPointError, ValueError):
         # data from cache can't be properly read, or data is weird
-        fig = plt.figure()
+        fig = plt.figure(figsize=(4, 1))
         plt.axis("off")
-        plt.text(0.1, 0.45, f"Failed to create {ifo} omegascan", fontsize=17)
+        plt.text(0.5, 0.5, "Failed to create V1 omegascan",
+                 horizontalalignment='center', verticalalignment='center',
+                 fontsize=17)
     else:
         fig = Plot(*qgrams,
                    figsize=(12 * len(durs), 6),
                    geometry=(1, len(durs)),
                    yscale='log',
                    method='pcolormesh',
                    cmap='viridis')
@@ -263,14 +265,32 @@
         figures=[],
         tables=[],
         links=links,
         extra=[],
     )
 
 
+def ifo_from_channel(channel):
+    '''Get detector prefix from a channel.
+
+    Parameters
+    ----------
+    channel : str
+        Channel, e.g., H1:GDS-CALIB_STRAIN.
+
+    Returns
+    -------
+    str
+        Detector prefix, e.g., H1.
+    '''
+    ifo = channel.split(':')[0]
+    assert len(ifo) == 2, "Detector name should be two letters"
+    return ifo
+
+
 def check_idq(cache, channel, start, end):
     """Looks for iDQ frame and reads them.
 
     Parameters
     ----------
     cache : :class:`glue.lal.Cache`
         Cache from which to check.
@@ -359,22 +379,22 @@
             log.warning('Failed to read from low-latency frame files')
         else:
             # FIXME: In the playground environment, the Virgo state vector
             # channel is stored as a float. Is this also the case in the
             # production environment?
             statevector = statevector.astype(np.uint32)
             if len(statevector) > 0:  # statevector must not be empty
-                return {bitname.format(channel.split(':')[0], key):
+                return {bitname.format(ifo_from_channel(channel), key):
                         bool(logic_map[logic_type](
                             value.value if len(value.value) > 0 else None))
                         for key, value in statevector.get_bit_series().items()}
     # FIXME: figure out how to get access to low-latency frames outside
     # of the cluster. Until we figure that out, actual I/O errors have
     # to be non-fatal.
-    return {bitname.format(channel.split(':')[0], key):
+    return {bitname.format(ifo_from_channel(channel), key):
             None for key in bits if key is not None}
 
 
 @app.task(shared=False, bind=True, default_retry_delay=5)
 def check_vectors(self, event, graceid, start, end):
     """Perform data quality checks for an event and labels/logs results to
     GraceDB.
@@ -432,15 +452,15 @@
     instruments = event['instruments'].split(',')
     pipeline = event['pipeline']
     pre, post = app.conf['check_vector_prepost'][pipeline]
     start, end = start - pre, end + post
     prepost_msg = "Check looked within -{}/+{} seconds of superevent. ".format(
         pre, post)
 
-    ifos = {key.split(':')[0] for key, val in
+    ifos = {ifo_from_channel(key) for key, val in
             app.conf['llhoft_channels'].items()}
     caches = {ifo: create_cache(ifo, start, end) for ifo in ifos}
     bit_defs = {channel_type: Bits(channel=bitdef['channel'],
                                    bits=bitdef['bits'])
                 for channel_type, bitdef
                 in app.conf['detchar_bit_definitions'].items()}
 
@@ -450,37 +470,58 @@
     analysis_channels = app.conf['llhoft_channels'].items()
     if app.conf['uses_gatedhoft'][pipeline]:
         analysis_channels = {k: v for k, v in analysis_channels
                              if k[3:] != 'DMT-DQ_VECTOR'}.items()
     for channel, bits in analysis_channels:
         try:
             states.update(check_vector(
-                caches[channel.split(':')[0]], channel,
+                caches[ifo_from_channel(channel)], channel,
                 start, end, bit_defs[bits]))
         except ValueError as exc:
             # check_vector likely failed to find the requested data
             # in the cache because it has yet to arrive
             raise self.retry(exc=exc, max_retries=4)
     # Pick out DQ and injection states, then filter for active detectors
     dq_states = {key: value for key, value in states.items()
                  if key.split('_')[-1] != 'INJ'}
     inj_states = {key: value for key, value in states.items()
                   if key.split('_')[-1] == 'INJ'}
     active_dq_states = {key: value for key, value in dq_states.items()
-                        if key.split(':')[0] in instruments}
+                        if ifo_from_channel(key) in instruments}
     active_inj_states = {key: value for key, value in inj_states.items()
-                         if key.split(':')[0] in instruments}
+                         if ifo_from_channel(channel) in instruments}
 
     # Check iDQ states and filter for active instruments
-    idq_faps = dict(check_idq(caches[channel.split(':')[0]],
+    idq_faps = dict(check_idq(caches[ifo_from_channel(channel)],
                     channel, start, end)
                     for channel in app.conf['idq_channels']
-                    if channel.split(':')[0] in instruments)
+                    if ifo_from_channel(channel) in instruments)
+    idq_oks = dict(check_idq(caches[ifo_from_channel(channel)],
+                   channel, start, end)
+                   for channel in app.conf['idq_ok_channels']
+                   if ifo_from_channel(channel) in instruments)
 
     # Logging iDQ to GraceDB
+    # Checking the IDQ-OK vector
+    idq_not_ok_ifos = [
+        ifo_from_channel(ok_channel)
+        for ok_channel, min_value in idq_oks.items()
+        if min_value == 0 or min_value is None]
+    idq_not_ok_fap_chans = [
+        chan for chan in idq_faps.keys()
+        if ifo_from_channel(chan) in idq_not_ok_ifos]
+    # Remove iDQ FAP channels if their IDQ_OK values are bad
+    for idq_not_ok_chan in idq_not_ok_fap_chans:
+        del idq_faps[idq_not_ok_chan]
+    if len(idq_not_ok_ifos) > 0:
+        idq_ok_msg = (f"Not checking iDQ for {', '.join(idq_not_ok_ifos)} "
+                      "because it has times where IDQ_OK = 0. ")
+    else:
+        idq_ok_msg = ''
+
     if None not in idq_faps.values() and len(idq_faps) > 0:
         idq_faps_readable = {k: round(v, 3) for k, v in idq_faps.items()}
         if min(idq_faps.values()) <= app.conf['idq_fap_thresh']:
             idq_msg = ("iDQ false alarm probability is low "
                        "(below {} threshold), "
                        "i.e., there could be a data quality issue: "
                        "minimum FAP is {}. ").format(
@@ -498,18 +539,21 @@
                     pass
         else:
             idq_msg = ("iDQ false alarm probabilities for active detectors "
                        "are good (above {} threshold). "
                        "Minimum FAP is {}. ").format(
                            app.conf['idq_fap_thresh'],
                            json.dumps(idq_faps_readable)[1:-1])
-    else:
+    elif None in idq_faps.values():
         idq_msg = "iDQ false alarm probabilities unknown. "
+    else:
+        idq_msg = ''
     gracedb.upload.delay(
-        None, None, graceid, idq_msg + prepost_msg, ['data_quality'])
+        None, None, graceid,
+        idq_ok_msg + idq_msg + prepost_msg, ['data_quality'])
 
     # Labeling INJ to GraceDB
     if False in active_inj_states.values():
         # Label 'INJ' if injection found in active IFOs
         gracedb.create_label('INJ', graceid)
         # Add labels to return value to avoid querying GraceDB again.
         event = dict(event, labels=event.get('labels', []) + ['INJ'])
@@ -577,15 +621,16 @@
             event['labels'].remove('DQOK')
         except ValueError:  # not in list
             pass
     else:
         state = "unknown"
 
     # Create and upload DQR-compatible json
-    state_summary = '{} {} {}'.format(inj_msg, idq_msg, msg)
+    state_summary = '{} {} {}'.format(
+        inj_msg, idq_ok_msg + idq_msg, msg)
     if state == "unknown":
         json_state = "error"
     else:
         json_state = state
     file = dqr_json(json_state, state_summary)
     filename = 'gwcelerydetcharcheckvectors-{}.json'.format(graceid)
     message = "DQR-compatible json generated from check_vectors results"
```

### Comparing `gwcelery-2.1.1/gwcelery/tasks/em_bright.py` & `gwcelery-2.1.2/gwcelery/tasks/em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/external_skymaps.py` & `gwcelery-2.1.2/gwcelery/tasks/external_skymaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 COMBINED_SKYMAP_FILENAME_FLAT = 'combined-ext.fits.gz'
 """Filename of combined sky map in a flattened format"""
 
 COMBINED_SKYMAP_FILENAME_PNG = 'combined-ext.png'
 """Filename of combined sky map plot"""
 
 
-@app.task(shared=False,
-          queue='exttrig')
+@app.task(shared=False)
 def create_combined_skymap(se_id, ext_id, preferred_event=None):
     """Creates and uploads the combined LVK-external skymap, uploading to the
     external trigger GraceDB page. The filename used for the combined sky map
     will be 'combined-ext.multiorder.fits' if the GW sky map is multi-ordered
     or 'combined-ext.fits.gz' if the GW sky map is not. Will use the GW sky map
     in from the preferred event if given.
 
@@ -93,15 +92,14 @@
             gracedb.upload.s(COMBINED_SKYMAP_FILENAME_PNG, ext_id,
                              message_png, ['sky_loc', 'ext_coinc'])
         )
     ).delay()
 
 
 @app.task(autoretry_for=(ValueError,), retry_backoff=10,
-          queue='exttrig',
           retry_backoff_max=600)
 def get_skymap_filename(graceid, is_gw):
     """Get the skymap fits filename.
 
     If not available, will try again 10 seconds later, then 20, then 40, etc.
     until up to 10 minutes after initial attempt.
 
@@ -140,15 +138,15 @@
             if (filename.endswith('.fits') or filename.endswith('.fit') or
                     filename.endswith('.fits.gz')) and \
                     "combined-ext." not in filename:
                 return fv
     raise ValueError('No skymap available for {0} yet.'.format(graceid))
 
 
-@app.task(shared=False, queue='exttrig')
+@app.task(shared=False)
 def _download_skymaps(gw_filename, ext_filename, gw_id, ext_id):
     """Download both superevent and external sky map to be combined."""
     gw_skymap = gracedb.download(gw_filename, gw_id)
     ext_skymap = gracedb.download(ext_filename, ext_id)
     return gw_skymap, ext_skymap
 
 
@@ -190,15 +188,15 @@
             '', 'The values were reweighted by using data from {0}{1}'.format(
                 ('an ' if ext_instrument == 'external instrument'
                  else ''),
                 ext_instrument)])
     return gw_sky
 
 
-@app.task(shared=False, queue='exttrig')
+@app.task(shared=False)
 def combine_skymaps(skymapsbytes, gw_moc=True):
     """This task combines the two input skymaps, in this case the external
     trigger skymap and the LVK skymap and writes to a temporary output file. It
     then returns the contents of the file as a byte array.
 
     There are separate methods in case the GW sky map is multiordered (we just
     reweight using the external sky map) or flattened (use standard
@@ -240,15 +238,15 @@
     if len(em_events):
         for exttrig in em_events:
             if gracedb.get_event(exttrig)['search'] == 'GRB':
                 return exttrig
     raise ValueError('No associated GRB EM event(s) for {0}.'.format(graceid))
 
 
-@app.task(shared=False, queue='exttrig')
+@app.task(shared=False)
 def external_trigger_heasarc(external_id):
     """Returns the HEASARC fits file link."""
     gracedb_log = gracedb.get_log(external_id)
     for message in gracedb_log:
         if 'Original Data' in message['comment']:
             filename = message['filename']
             xmlfile = gracedb.download(urllib.parse.quote(filename),
@@ -258,15 +256,14 @@
                                     ).attrib['value']
             return re.sub(r'quicklook(.*)', 'current/', heasarc_url)
     raise ValueError('Not able to retrieve HEASARC link for {0}.'.format(
         external_id))
 
 
 @app.task(autoretry_for=(urllib.error.HTTPError,), retry_backoff=10,
-          queue='exttrig',
           retry_backoff_max=600)
 def get_external_skymap(link, search):
     """Download the Fermi sky map fits file and return the contents as a byte
     array. If GRB, will construct a HEASARC url, while if SubGRB, will use the
     link directly.
 
     If not available, will try again 10 seconds later, then 20, then 40, etc.
@@ -286,15 +283,14 @@
     context.options |= ssl.OP_NO_TLSv1_3
     #  return astropy.utils.data.get_file_contents(
     #      (skymap_link), encoding='binary', cache=False)
     return urllib.request.urlopen(skymap_link, context=context).read()
 
 
 @app.task(autoretry_for=(urllib.error.HTTPError, urllib.error.URLError,),
-          queue='exttrig',
           retry_backoff=10, retry_backoff_max=1200)
 def get_upload_external_skymap(event, skymap_link=None):
     """If a Fermi sky map is not uploaded yet, tries to download one and upload
     to external event. If sky map is not available, passes so that this can be
     re-run the next time an update GCN notice is received. If GRB, will
     construct a HEASARC url, while if SubGRB, will use the link directly.
     If SubGRB or FromURL, downloads a skymap using the provided URL rather
@@ -482,15 +478,15 @@
                            origin='LIGO-VIRGO-KAGRA',
                            vcs_version=_version.get_versions()['version'],
                            history='file only for internal use')
         with open(f.name, 'rb') as file:
             return file.read()
 
 
-@app.task(shared=False, queue='exttrig')
+@app.task(shared=False)
 def create_upload_external_skymap(event, notice_type, notice_date):
     """Create and upload external sky map using
     RA, dec, and error radius information.
 
     Parameters
     ----------
     event : dict
```

### Comparing `gwcelery-2.1.1/gwcelery/tasks/external_triggers.py` & `gwcelery-2.1.2/gwcelery/tasks/external_triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,14 @@
 
 @igwn_alert.handler('superevent',
                     'mdc_superevent',
                     'external_fermi',
                     'external_swift',
                     'external_integral',
                     'external_agile',
-                    queue='exttrig',
                     shared=False)
 def handle_grb_igwn_alert(alert):
     """Parse an IGWN alert message related to superevents/GRB external triggers
     and dispatch it to other tasks.
 
     Notes
     -----
@@ -428,15 +427,14 @@
             raven.trigger_raven_alert(coinc_far_dict, superevent, graceid,
                                       alert['object'], gw_group)
 
 
 @igwn_alert.handler('superevent',
                     'mdc_superevent',
                     'external_snews',
-                    queue='exttrig',
                     shared=False)
 def handle_snews_igwn_alert(alert):
     """Parse an IGWN alert message related to superevents/SN external triggers
     and dispatch it to other tasks.
 
     Notes
     -----
@@ -489,16 +487,15 @@
         ext_id = event['em_type']
     else:
         se_id = event['superevent']
         ext_id = event['graceid']
     return se_id, ext_id
 
 
-@app.task(queue='exttrig',
-          shared=False)
+@app.task(shared=False)
 def _launch_external_detchar(event):
     start = event['gpstime']
     if event['pipeline'] == 'SNEWS':
         start, end = event['gpstime'], event['gpstime']
     else:
         integration_time = \
             event['extra_attributes']['GRB']['trigger_duration'] or 4.0
```

### Comparing `gwcelery-2.1.1/gwcelery/tasks/first2years.py` & `gwcelery-2.1.2/gwcelery/tasks/first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/first2years_external.py` & `gwcelery-2.1.2/gwcelery/tasks/first2years_external.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,14 @@
         val += (ord(end_string[i]) - 96) * 26 ** (len(end_string) - i - 1)
     return val % int(app.conf['joint_mdc_freq']) == 0 if se_search == 'MDC' \
         else val % int(app.conf['joint_O3_replay_freq']) == 0
 
 
 @igwn_alert.handler('mdc_superevent',
                     'superevent',
-                    queue='exttrig',
                     shared=False)
 def upload_external_event(alert):
     """Upload a random GRB event for a certain percentage of MDC
     or O3-replay superevents.
 
     Notes
     -----
@@ -164,16 +163,15 @@
         external_triggers.handle_grb_gcn(ext_event)
 
         events.append(ext_event), pipelines.append(pipeline)
 
     return events, pipelines
 
 
-@app.task(queue='exttrig',
-          ignore_result=True,
+@app.task(ignore_result=True,
           shared=False)
 def upload_snews_event():
     """Create and upload a SNEWS-like MDC external event."""
     current_time = Time(Time.now(), format='gps').value
     ext_event = create_external_event(current_time, 'SNEWS', 'MDC')
     external_triggers.handle_snews_gcn(ext_event)
     return ext_event
```

### Comparing `gwcelery-2.1.1/gwcelery/tasks/gcn.py` & `gwcelery-2.1.2/gwcelery/tasks/gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/gracedb.py` & `gwcelery-2.1.2/gwcelery/tasks/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/gwskynet.py` & `gwcelery-2.1.2/gwcelery/tasks/gwskynet.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/igwn_alert.py` & `gwcelery-2.1.2/gwcelery/tasks/igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/inference.py` & `gwcelery-2.1.2/gwcelery/tasks/inference.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,82 +6,22 @@
 import os
 import subprocess
 import urllib
 
 from bilby_pipe.utils import convert_string_to_dict
 from bilby_pipe.bilbyargparser import BilbyConfigFileParser
 from celery import group
-from gwdatafind import find_urls
 import numpy as np
 
 from .. import app
 from ..jinja import env
 from . import condor
 from . import gracedb
 
 
-def _data_exists(gpstime, frametype_dict):
-    """Check whether data at input GPS time can be found with gwdatafind and
-    return true if it is found.
-    """
-    return min(
-        len(
-            find_urls(ifo[0], frametype_dict[ifo], gpstime, gpstime + 1)
-        ) for ifo in frametype_dict.keys()
-    ) > 0
-
-
-class NotEnoughData(Exception):
-    """Raised if found data is not enough due to the latency of data
-    transfer
-    """
-
-
-@app.task(bind=True, autoretry_for=(NotEnoughData, ),
-          retry_backoff=True, retry_backoff_max=600, max_retries=16)
-def query_data(self, trigtime):
-    """Continues to query data until it is found with gwdatafind and return
-    frametypes for the data. This query will be retried for ~4600 seconds,
-    which is longer than the expected latency of transfer of high-latency data
-    with length of ~4000 seconds.
-    """
-    end = trigtime + 2
-    if _data_exists(end, app.conf['low_latency_frame_types']):
-        return app.conf['low_latency_frame_types']
-    elif _data_exists(end, app.conf['high_latency_frame_types']):
-        return app.conf['high_latency_frame_types']
-    else:
-        raise NotEnoughData
-
-
-@app.task(ignore_result=True, shared=False)
-def upload_no_frame_files(request, exc, traceback, superevent_id):
-    """Upload notification when no frame files are found.
-
-    Parameters
-    ----------
-    request : Context (placeholder)
-        Task request variables
-    exc : Exception
-        Exception raised by query_data
-    traceback : str (placeholder)
-        Traceback message from a task
-    superevent_id : str
-        The GraceDB ID of a target superevent
-
-    """
-    if isinstance(exc, NotEnoughData):
-        gracedb.upload.delay(
-            filecontents=None, filename=None,
-            graceid=superevent_id,
-            message='Frame files have not been found.',
-            tags='pe'
-        )
-
-
 def _find_appropriate_cal_env(trigtime, dir_name):
     """Return the path to the calibration uncertainties estimated at the time
     before and closest to the trigger time. If there are no calibration
     uncertainties estimated before the trigger time, return the oldest one. The
     gpstimes at which the calibration uncertainties were estimated and the
     names of the files containing the uncertaintes are saved in
     [HLV]_CalEnvs.txt.
@@ -111,21 +51,19 @@
         idx = np.argmax(gpstimes * candidate_gpstimes)
         appropriate_cal = calibration_index['filename'][idx]
     else:
         appropriate_cal = calibration_index['filename'][np.argmin(gpstimes)]
     return os.path.join(dir_name, appropriate_cal.decode('utf-8'))
 
 
-def prepare_lalinference_ini(frametype_dict, event, superevent_id):
+def prepare_lalinference_ini(event, superevent_id):
     """Determine LALInference configurations and return ini file content
 
     Parameters
     ----------
-    frametype_dict : dict
-        Dictionary whose keys are ifos and values are frame types
     event : dict
         The json contents of a target G event retrieved from
         gracedb.get_event(), whose mass and spin information are used to
         determine analysis settings.
     superevent_id : str
         The GraceDB ID of a target superevent
 
@@ -160,15 +98,15 @@
                    'gracedb': 'gracedb',
                    'ppanalysis': 'cbcBayesPPAnalysis',
                    'pos_to_sim_inspiral': 'cbcBayesPosToSimInspiral',
                    'bayeswave': 'BayesWave',
                    'bayeswavepost': 'BayesWavePost'}
     ini_settings = {
         'gracedb_host': app.conf['gracedb_host'],
-        'types': frametype_dict,
+        'types': app.conf['low_latency_frame_types'],
         'channels': app.conf['strain_channel_names'],
         'state_vector_channels': app.conf['state_vector_channel_names'],
         'webdir': os.path.join(
             app.conf['pe_results_path'], superevent_id, 'lalinference'
         ),
         'paths': [{'name': name, 'path': find_executable(executable)}
                   for name, executable in executables.items()],
@@ -189,47 +127,43 @@
                   for sngl in singleinspiraltable]),
         'mpirun': find_executable('mpirun')
     }
     return ini_template.render(ini_settings)
 
 
 @app.task(shared=False)
-def _setup_dag_for_lalinference(coinc, rundir, event, superevent_id,
-                                frametype_dict):
+def _setup_dag_for_lalinference(coinc, rundir, event, superevent_id):
     """Create DAG for a lalinference run and return the path to DAG.
 
     Parameters
     ----------
     coinc : byte contents
         Byte contents of ``coinc.xml``. The PSD is expected to be embedded.
     rundir : str
         The path to a run directory where the DAG file is created.
     event : dict
         The json contents of a target G event retrieved from
         gracedb.get_event(), whose mass and spin information are used to
         determine analysis settings.
     superevent_id : str
         The GraceDB ID of a target superevent
-    frametype_dict : dict
-        Dictionary whose keys are ifos and values are frame types
 
     Returns
     -------
     path_to_dag : str
         The path to the .dag file
 
     """
     # write down coinc.xml in the run directory
     path_to_coinc = os.path.join(rundir, 'coinc.xml')
     with open(path_to_coinc, 'wb') as f:
         f.write(coinc)
 
     # write down and upload ini file
-    ini_contents = prepare_lalinference_ini(
-        frametype_dict, event, superevent_id)
+    ini_contents = prepare_lalinference_ini(event, superevent_id)
     path_to_ini = os.path.join(rundir, 'online_lalinference_pe.ini')
     with open(path_to_ini, 'w') as f:
         f.write(ini_contents)
     gracedb.upload.delay(
         ini_contents, filename=os.path.basename(path_to_ini),
         graceid=superevent_id,
         message=('Automatically generated LALInference configuration file'
@@ -250,202 +184,14 @@
             message='Failed to prepare DAG for lalinference', tags='pe'
         )
         raise
 
     return os.path.join(rundir, 'multidag.dag')
 
 
-def _dump_phenomd_settings(path):
-    settings = {
-        "likelihood_args": {
-            "likelihood_type": "ROQGravitationalWaveTransient",
-            "minimum_frequency": 20,
-            "maximum_frequency": 1024,
-            "roq_scale_factor": 1,
-            "waveform_approximant": "IMRPhenomD",
-        },
-        "likelihood_parameter_bounds": {
-            "mass_ratio_min": 0.125,
-            "a_1_max": 0.05,
-            "a_2_max": 0.05,
-            "spin_template": "aligned",
-        },
-        "trigger_dependent": {
-            "range": {
-                "chirp_mass": [
-                    [0.6, 1.012], [1.012, 1.54], [1.54, 2.31], [2.31, 4.0]
-                ],
-            },
-            "likelihood_args": [
-                {"roq_linear_matrix":
-                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_512s.hdf5",
-                 "roq_quadratic_matrix":
-                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_512s.hdf5",
-                 "duration": 512},
-                {"roq_linear_matrix":
-                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_256s.hdf5",
-                 "roq_quadratic_matrix":
-                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_256s.hdf5",
-                 "duration": 256},
-                {"roq_linear_matrix":
-                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_128s.hdf5",
-                 "roq_quadratic_matrix":
-                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_128s.hdf5",
-                 "duration": 128},
-                {"roq_linear_matrix":
-                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_64s.hdf5",
-                 "roq_quadratic_matrix":
-                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_64s.hdf5",
-                 "duration": 64}
-            ],
-            "likelihood_parameter_bounds": [
-                {"chirp_mass_min": 0.6, "chirp_mass_max": 1.1},
-                {"chirp_mass_min": 0.92, "chirp_mass_max": 1.7},
-                {"chirp_mass_min": 1.4, "chirp_mass_max": 2.6},
-                {"chirp_mass_min": 2.1, "chirp_mass_max": 4.0}
-            ],
-        },
-    }
-    with open(path, 'w') as f:
-        json.dump(settings, f, indent=2)
-
-
-def _dump_high_mass_ratio_pv2_settings(path):
-    settings = {
-        "likelihood_args": {
-            "likelihood_type": "ROQGravitationalWaveTransient",
-            "minimum_frequency": 20,
-            "maximum_frequency": 1024,
-            "roq_scale_factor": 1,
-            "waveform_approximant": "IMRPhenomPv2",
-        },
-        "likelihood_parameter_bounds": {
-            "mass_ratio_min": 0.05,
-            "a_1_max": 0.99,
-            "a_2_max": 0.99,
-            "spin_template": "precessing",
-        },
-        "trigger_dependent": {
-            "range": {
-                "chirp_mass": [[1.4, 2.31], [2.31, 3.63], [3.63, 5.72],
-                               [5.72, 9.57], [9.57, 21]],
-            },
-            "likelihood_args": [
-                {"roq_linear_matrix":
-                    "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_128s.hdf5",
-                 "roq_quadratic_matrix":
-                    "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_128s.hdf5",
-                 "duration": 128},
-                {
-                    "roq_linear_matrix":
-                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_64s.hdf5",
-                    "roq_quadratic_matrix":
-                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_64s.hdf5",
-                    "duration": 64,
-                },
-                {
-                    "roq_linear_matrix":
-                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_32s.hdf5",
-                    "roq_quadratic_matrix":
-                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_32s.hdf5",
-                    "duration": 32,
-                },
-                {
-                    "roq_linear_matrix":
-                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_16s.hdf5",
-                    "roq_quadratic_matrix":
-                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_16s.hdf5",
-                    "duration": 16,
-                },
-                {
-                    "roq_linear_matrix":
-                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_8s.hdf5",
-                    "roq_quadratic_matrix":
-                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_8s.hdf5",
-                    "duration": 8,
-                },
-            ],
-            "likelihood_parameter_bounds": [
-                {"chirp_mass_min": 1.4, "chirp_mass_max": 2.6},
-                {"chirp_mass_min": 2.1, "chirp_mass_max": 4.0},
-                {"chirp_mass_min": 3.3, "chirp_mass_max": 6.3},
-                {"chirp_mass_min": 5.2, "chirp_mass_max": 11.0},
-                {"chirp_mass_min": 8.7, "chirp_mass_max": 21.0},
-            ],
-        },
-    }
-    with open(path, 'w') as f:
-        json.dump(settings, f, indent=2)
-
-
-def _dump_xphm_settings(path):
-    settings = {
-        "likelihood_args": {
-            "likelihood_type": "ROQGravitationalWaveTransient",
-            "minimum_frequency": 20,
-            "maximum_frequency": 4096,
-            "reference_frequency": 20,
-            "roq_scale_factor": 1,
-            "waveform_approximant": "IMRPhenomXPHM",
-            "waveform_arguments_dict": {"PhenomXHMReleaseVersion": 122019},
-            "phase_marginalization": False,
-        },
-        "likelihood_parameter_bounds": {
-            "mass_ratio_min": 0.05,
-            "a_1_max": 0.99,
-            "a_2_max": 0.99,
-            "spin_template": "precessing",
-        },
-        "trigger_dependent": {
-            "range": {
-                "chirp_mass": [[10.03, 16], [16, 25],
-                               [25, 45], [45, np.inf]],
-            },
-            "likelihood_args": [
-                {
-                    "roq_linear_matrix":
-                        "/home/roq/IMRPhenomXPHM/basis_32s.hdf5",
-                    "roq_quadratic_matrix":
-                        "/home/roq/IMRPhenomXPHM/basis_32s.hdf5",
-                    "duration": 32,
-                },
-                {
-                    "roq_linear_matrix":
-                        "/home/roq/IMRPhenomXPHM/basis_16s.hdf5",
-                    "roq_quadratic_matrix":
-                        "/home/roq/IMRPhenomXPHM/basis_16s.hdf5",
-                    "duration": 16,
-                },
-                {
-                    "roq_linear_matrix":
-                        "/home/roq/IMRPhenomXPHM/basis_8s.hdf5",
-                    "roq_quadratic_matrix":
-                        "/home/roq/IMRPhenomXPHM/basis_8s.hdf5",
-                    "duration": 8,
-                },
-                {
-                    "roq_linear_matrix":
-                        "/home/roq/IMRPhenomXPHM/basis_4s.hdf5",
-                    "roq_quadratic_matrix":
-                        "/home/roq/IMRPhenomXPHM/basis_4s.hdf5",
-                    "duration": 4,
-                },
-            ],
-            "likelihood_parameter_bounds": [
-                {"chirp_mass_min": 10.03, "chirp_mass_max": 19.04},
-                {"chirp_mass_min": 13, "chirp_mass_max": 31.85},
-                {"chirp_mass_min": 20, "chirp_mass_max": 62.86},
-                {"chirp_mass_min": 30, "chirp_mass_max": 200},
-            ],
-        },
-    }
-    with open(path, 'w') as f:
-        json.dump(settings, f, indent=2)
-
-
 @app.task(shared=False)
 def _setup_dag_for_bilby(
     coinc, rundir, event, superevent_id, mode="production"
 ):
     """Create DAG for a bilby run and return the path to DAG.
 
     Parameters
@@ -491,20 +237,20 @@
 
     path_to_settings = os.path.join(rundir, 'settings.json')
     setup_arg = ['bilby_pipe_gracedb', '--webdir', path_to_webdir,
                  '--outdir', rundir, '--json', path_to_json,
                  '--psd-file', path_to_psd, '--settings', path_to_settings]
     settings = {'summarypages_arguments': {'gracedb': event['graceid'],
                                            'no_ligo_skymap': True},
-                'accounting_user': 'soichiro.morisaki',
-                'enforce_signal_duration': False}
+                'accounting_user': 'soichiro.morisaki'}
     if app.conf['gracedb_host'] != 'gracedb.ligo.org':
         settings['queue'] = 'Online_PE_MDC'
     else:
         settings['queue'] = 'Online_PE'
+        settings['accounting'] = 'ligo.prod.o4.cbc.pe.bilby'
     # FIXME: using live data for gracedb-test events should be reconsidered
     # when we have a better idea to differentiate MDC and real events.
     if app.conf['gracedb_host'] not in [
         'gracedb.ligo.org', 'gracedb-test.ligo.org'
     ]:
         setup_arg += ['--channel-dict', 'o3replay']
 
@@ -524,29 +270,26 @@
                 'spline_calibration_nodes': 10,
                 'request_memory_generation': 8.0
             }
         )
         # use low-spin IMRPhenomD below chirp mass of m1=3Msun, m2=1Msun
         # assuming binary neutron star
         if trigger_chirp_mass < 1.465:
-            likelihood_mode = os.path.join(rundir, "likelihood_mode.json")
-            _dump_phenomd_settings(likelihood_mode)
+            likelihood_mode = 'lowspin_phenomd_fhigh1024_roq'
             settings['sampler_kwargs']['naccept'] = 10
         # use IMRPhenomPv2 with mass ratio upper bound of 8 below chirp mass of
         # m1=8Msun, m2=1Msun
         elif trigger_chirp_mass < 2.243:
             likelihood_mode = 'phenompv2_bns_roq'
         # use IMRPhenomPv2 with mass ratio upper bound of 20 in chirp-mass
         # range where IMRPhenomXPHM ROQ bases are not available
         elif trigger_chirp_mass < 12:
-            likelihood_mode = os.path.join(rundir, "likelihood_mode.json")
-            _dump_high_mass_ratio_pv2_settings(likelihood_mode)
+            likelihood_mode = 'low_q_phenompv2_roq'
         else:
-            likelihood_mode = os.path.join(rundir, "likelihood_mode.json")
-            _dump_xphm_settings(likelihood_mode)
+            likelihood_mode = 'phenomxphm_roq'
             settings['request_memory_generation'] = 36.0
             settings['request_memory'] = 16.0
         setup_arg += ['--cbc-likelihood-mode', likelihood_mode]
     elif mode == 'fast_test':
         setup_arg += ["--sampler-kwargs", "FastTest"]
         if trigger_chirp_mass < 3.9:
             setup_arg += ['--cbc-likelihood-mode', 'phenompv2_bns_roq']
@@ -583,25 +326,23 @@
             tags='pe')
 
     path_to_dag, = glob.glob(os.path.join(rundir, 'submit/dag*.submit'))
     return path_to_dag
 
 
 @app.task(shared=False)
-def _setup_dag_for_rapidpe(rundir, superevent_id, frametype_dict):
+def _setup_dag_for_rapidpe(rundir, superevent_id):
     """Create DAG for a rapidpe run and return the path to DAG.
 
     Parameters
     ----------
     rundir : str
         The path to a run directory where the DAG file is created
     superevent_id : str
         The GraceDB ID of a target superevent
-    frametype_dict : dict
-        Dictionary whose keys are ifos and values are frame types
 
     Returns
     -------
     path_to_dag : str
         The path to the .dag file
 
     """
@@ -618,15 +359,15 @@
         {'rundir': rundir,
          'webdir': os.path.join(
              app.conf['pe_results_path'], superevent_id, 'rapidpe'
          ),
          'gracedb_url': f'https://{app.conf["gracedb_host"]}/api',
          'superevent_id': superevent_id,
          'run_mode': run_mode,
-         'frame_data_types': frametype_dict})
+         'frame_data_types': app.conf['low_latency_frame_types']})
     path_to_ini = os.path.join(rundir, 'rapidpe.ini')
     with open(path_to_ini, 'w') as f:
         f.write(ini_contents)
     gracedb.upload.delay(
         ini_contents, filename=os.path.basename(path_to_ini),
         graceid=superevent_id,
         message=('Automatically generated RapidPE-RIFT configuration file'
@@ -656,16 +397,15 @@
 def _condor_no_submit(path_to_dag):
     """Run 'condor_submit_dag -no_submit' and return the path to .sub file."""
     subprocess.run(['condor_submit_dag', '-no_submit', path_to_dag],
                    capture_output=True, check=True)
     return '{}.condor.sub'.format(path_to_dag)
 
 
-def dag_prepare_task(rundir, event, superevent_id, pe_pipeline,
-                     frametype_dict=None, **kwargs):
+def dag_prepare_task(rundir, event, superevent_id, pe_pipeline, **kwargs):
     """Return a canvas of tasks to prepare DAG.
 
     Parameters
     ----------
     rundir : str
         The path to a run directory where the DAG file is created
     event : dict
@@ -673,34 +413,30 @@
         gracedb.get_event(), whose mass and spin information are used to
         determine analysis settings.
     superevent_id : str
         The GraceDB ID of a target superevent
     pe_pipeline : str
         The parameter estimation pipeline used,
         lalinference, bilby, or rapidpe.
-    frametype_dict : dict
-        Dictionary whose keys are ifos and values are frame types
 
     Returns
     -------
     canvas : canvas of tasks
         The canvas of tasks to prepare DAG
 
     """
     if pe_pipeline == 'lalinference':
         canvas = gracedb.download.si('coinc.xml', event['graceid']) | \
-            _setup_dag_for_lalinference.s(rundir, event, superevent_id,
-                                          frametype_dict)
+            _setup_dag_for_lalinference.s(rundir, event, superevent_id)
     elif pe_pipeline == 'bilby':
         canvas = gracedb.download.si('coinc.xml', event['graceid']) | \
             _setup_dag_for_bilby.s(
                 rundir, event, superevent_id, kwargs['bilby_mode'])
     elif pe_pipeline == 'rapidpe':
-        canvas = _setup_dag_for_rapidpe.s(
-            rundir, superevent_id, frametype_dict)
+        canvas = _setup_dag_for_rapidpe.s(rundir, superevent_id)
     else:
         raise NotImplementedError(f'Unknown PE pipeline {pe_pipeline}.')
     canvas |= _condor_no_submit.s()
     return canvas
 
 
 def _find_paths_from_name(directory, name):
@@ -990,25 +726,33 @@
         app.conf['pe_results_url'],
         os.path.join(superevent_id, 'rapidpe', 'summarypage.html')
     )
     canvas = gracedb.upload.si(
         None, None, superevent_id,
         f'Summary page for RapidPE-RIFT is available <a href={url}>here</a>',
         ('pe',))
-
+    pipeline = gracedb.get_superevent(superevent_id)[
+            'preferred_event_data']['pipeline']
+    if pipeline == 'gstlal':
+        pastro_tags = (
+            "pe", "lvem",
+            "public", "p_astro"
+        )
+    else:
+        pastro_tags = ("pe", "p_astro")
     to_upload = [
         (
             "p_astro.json", "RapidPE_RIFT.p_astro.json",
             "RapidPE-RIFT Pastro results",
-            ("pe", "lvem", "public", "p_astro"),
+            pastro_tags,
         ),
         (
             "p_astro.png", "RapidPE_RIFT.p_astro.png",
             "RapidPE-RIFT Pastro results",
-            ("pe", "lvem", "public", "p_astro"),
+            pastro_tags,
         ),
     ]
     tasks = []
     for src_basename, dst_filename, description, tags in to_upload:
         src_filename = os.path.join(summary_path, src_basename)
         if os.path.isfile(src_filename):
             with open(src_filename, "rb") as f:
@@ -1104,21 +848,19 @@
         condor_kwargs['requirements'] = '((TARGET.Online_PE =?= True))'
         condor_kwargs['+Online_PE'] = True
         args += ["--redshift_method", "exact", "--evolve_spins_forwards"]
     return condor.check_output.si(args, **condor_kwargs)
 
 
 @app.task(ignore_result=True, shared=False)
-def start_pe(frametype_dict, event, superevent_id, pe_pipeline):
+def start_pe(event, superevent_id, pe_pipeline):
     """Run Parameter Estimation on a given event.
 
     Parameters
     ----------
-    frametype_dict : dict
-        Dictionary whose keys are ifos and values are frame types
     event : dict
         The json contents of a target G event retrieved from
         gracedb.get_event(), whose mass and spin information are used to
         determine analysis settings.
     superevent_id : str
         The GraceDB ID of a target superevent
     pe_pipeline : str
@@ -1126,40 +868,75 @@
         lalinference, bilby, or rapidpe.
 
     """
     # make an event directory
     pipeline_dir = os.path.expanduser('~/.cache/{}'.format(pe_pipeline))
     mkpath(pipeline_dir)
     event_dir = os.path.join(pipeline_dir, superevent_id)
-    os.mkdir(event_dir)
 
     if pe_pipeline == 'bilby':
+        if (
+            app.conf['gracedb_host'] == 'gracedb-playground.ligo.org' and
+            event['extra_attributes']['CoincInspiral']['mchirp'] >= 12
+        ):
+            # Count the number of BBH jobs and do not start a run if it exceeds
+            # 5 so that we do not use up disk space. We assume that the job is
+            # running if a data dump pickle file exists under the run
+            # directory, which is the largest file produced by PE and removed
+            # when the run completes.
+            number_of_bbh_running = 0
+            for p in glob.glob(
+                os.path.join(
+                    pipeline_dir,
+                    "*/*/data/*_generation_data_dump.pickle"
+                )
+            ):
+                path_to_ev = os.path.join(os.path.dirname(p), "../event.json")
+                if os.path.exists(path_to_ev):
+                    with open(path_to_ev, "r") as f:
+                        ev = json.load(f)
+                        mc = ev['extra_attributes']['CoincInspiral']['mchirp']
+                    if mc >= 12:
+                        number_of_bbh_running += 1
+            if number_of_bbh_running > 5:
+                gracedb.upload.delay(
+                    filecontents=None, filename=None, graceid=superevent_id,
+                    message='Parameter estimation will not start to save disk '
+                            f'space (There are {number_of_bbh_running} BBH '
+                            'jobs running).',
+                    tags='pe'
+                )
+                return
         modes = ["production"]
         rundirs = [os.path.join(event_dir, m) for m in modes]
         kwargs_list = [{'bilby_mode': m} for m in modes]
         analyses = [f'{m}-mode bilby' for m in modes]
+    elif pe_pipeline == 'rapidpe':
+        rundirs = [event_dir]
+        kwargs_list = [{'event_pipeline': event["pipeline"]}]
+        analyses = [pe_pipeline]
     else:
         rundirs = [event_dir]
         kwargs_list = [{}]
         analyses = [pe_pipeline]
 
+    os.mkdir(event_dir)
     for rundir, kwargs, analysis in zip(rundirs, kwargs_list, analyses):
         mkpath(rundir)
 
         gracedb.upload.delay(
             filecontents=None, filename=None, graceid=superevent_id,
             message=(f'Starting {analysis} parameter estimation '
                      f'for {event["graceid"]}'),
             tags='pe'
         )
 
         (
             dag_prepare_task(
-                rundir, event, superevent_id, pe_pipeline, frametype_dict,
-                **kwargs
+                rundir, event, superevent_id, pe_pipeline, **kwargs
             )
             |
             condor.submit.s().on_error(
                 job_error_notification.s(superevent_id, rundir, analysis)
             )
             |
             dag_finished.si(rundir, superevent_id, pe_pipeline, **kwargs)
```

### Comparing `gwcelery-2.1.1/gwcelery/tasks/legacy_gracedb.py` & `gwcelery-2.1.2/gwcelery/tasks/legacy_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/notice_text.py` & `gwcelery-2.1.2/gwcelery/tasks/notice_text.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/orchestrator.py` & `gwcelery-2.1.2/gwcelery/tasks/orchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from . import igwn_alert
 from . import p_astro
 from . import rrt_utils
 from . import skymaps
 from . import superevents
 
 from ligo.rrt_chat import channel_creation
+from astropy.time import Time
 
 
 @igwn_alert.handler('superevent',
                     'mdc_superevent',
                     shared=False)
 def handle_superevent(alert):
     """Schedule annotations for new superevents.
@@ -41,25 +42,43 @@
     checks with :meth:`gwcelery.tasks.detchar.check_vectors` and calls
     :meth:`~gwcelery.tasks.orchestrator.earlywarning_preliminary_alert` to send
     a preliminary notice.
     """
     superevent_id = alert['uid']
     # launch PE and detchar based on new type superevents
     if alert['alert_type'] == 'new':
+        # launching rapidpe 30s after merger.
+        timeout = max(
+            alert['object']['t_0'] - Time.now().gps +
+            app.conf['rapidpe_timeout'], 0
+        )
+        (
+            _get_preferred_event.si(superevent_id).set(
+                countdown=timeout
+            )
+            |
+            group(
+                _get_lowest_far.si(superevent_id),
+                gracedb.get_event.s()
+            )
+            |
+            parameter_estimation.s(superevent_id, 'rapidpe')
+        ).apply_async()
+
         (
             _get_preferred_event.si(superevent_id).set(
                 countdown=app.conf['pe_timeout']
             )
             |
             group(
                 _get_lowest_far.si(superevent_id),
                 gracedb.get_event.s()
             )
             |
-            parameter_estimation.s(superevent_id)
+            parameter_estimation.s(superevent_id, 'bilby')
         ).apply_async()
 
         # run check_vectors. Create and upload omegascans
         group(
             detchar.omegascan.si(alert['object']['t_0'], superevent_id),
 
             detchar.check_vectors.si(
@@ -409,15 +428,15 @@
             not alert['data']['filename'].endswith('.posterior_samples.hdf5'):
         return
     superevent_id = alert['uid']
     filename = alert['data']['filename']
     info = '{} {}'.format(alert['data']['comment'], filename)
     prefix, _ = filename.rsplit('.posterior_samples.')
     skymap_filename = f'{prefix}.multiorder.fits'
-    labels = ['pe', 'sky_loc', 'public']
+    labels = ['pe', 'sky_loc']
 
     (
         gracedb.download.si(filename, superevent_id)
         |
         skymaps.skymap_from_samples.s()
         |
         group(
@@ -572,28 +591,29 @@
     gracedb.create_label.delay(label, graceid)
     return filename
 
 
 @app.task(shared=False)
 def _leave_log_message_and_return_event_dict(event, superevent_id,
                                              message, **kwargs):
-    """Wrapper around :meth:`gracedb.update_superevent`
+    """Wrapper around :meth:`gracedb.upload`
     that returns the event dictionary.
     """
     gracedb.upload.delay(None, None, superevent_id, message, **kwargs)
     return event
 
 
 @gracedb.task(shared=False)
 def _update_superevent_and_return_event_dict(event, superevent_id):
     """Wrapper around :meth:`gracedb.update_superevent`
     that returns the event dictionary.
     """
     gracedb.update_superevent(superevent_id,
-                              preferred_event=event['graceid'])
+                              preferred_event=event['graceid'],
+                              t_0=event['gpstime'])
     return event
 
 
 @gracedb.task(shared=False)
 def _proceed_if_not_blocked_by(files, superevent_id, block_by):
     """Return files in case the superevent does not have labels `block_by`
 
@@ -674,15 +694,15 @@
         superevent_id,
         ['sky_loc', 'public']
     )
 
     return input_list
 
 
-@app.task(shared=False)
+@gracedb.task(shared=False)
 def _unpack_args_and_send_earlywarning_preliminary_alert(input_list, alert,
                                                          alert_type):
     """Unpack the output of the skymap, embright, p-astro download group in the
     beginning of the
     :meth:`~gwcelery.tasks.orchestartor.earlywarning_preliminary_alert` canvas
     and call
     :meth:`gwcelery.tasks.orchestrator.earlywarning_preliminary_initial_update_alert`.
@@ -872,15 +892,15 @@
     # FIXME: remove ._orig_run when this bug is fixed:
     # https://github.com/getsentry/sentry-python/issues/370
     return min(gracedb.get_event._orig_run(gid)['far'] for gid in
                gracedb.get_superevent._orig_run(superevent_id)["gw_events"])
 
 
 @app.task(ignore_result=True, shared=False)
-def parameter_estimation(far_event, superevent_id):
+def parameter_estimation(far_event, superevent_id, pe_pipeline):
     """Parameter Estimation with Bilby and RapidPE-RIFT. Parameter estimation
     runs are triggered for CBC triggers which pass the FAR threshold and are
     not mock uploads. For those which do not pass these criteria, this task
     uploads messages explaining why parameter estimation is not started.
     """
     far, event = far_event
     threshold = (app.conf['significant_alert_far_threshold']['cbc'] /
@@ -906,25 +926,15 @@
             filecontents=None, filename=None,
             graceid=superevent_id,
             message='Parameter estimation will not start since parameter '
                     'estimation is disabled for mock uploads.',
             tags='pe'
         )
     else:
-        canvas = inference.query_data.s(event['gpstime']).on_error(
-            inference.upload_no_frame_files.s(superevent_id)
-        )
-        pe_pipelines = ['bilby']
-        # Currently rapidpe works only for gstlal triggers
-        if event['pipeline'] == 'gstlal':
-            pe_pipelines += ['rapidpe']
-        canvas |= group(
-            inference.start_pe.s(event, superevent_id, p)
-            for p in pe_pipelines)
-        canvas.apply_async()
+        inference.start_pe.delay(event, superevent_id, pe_pipeline)
 
 
 @gracedb.task(shared=False)
 def earlywarning_preliminary_initial_update_alert(
     filenames,
     superevent,
     alert_type,
@@ -990,14 +1000,15 @@
                     and 'combined' not in f:
                 skymap_filename = fv
             if em_bright_needed \
                     and 'em_bright' in t \
                     and f.endswith('.json'):
                 em_bright_filename = fv
             if p_astro_needed \
+                    and {'public'}.issubset(t) \
                     and 'p_astro' in t \
                     and f.endswith('.json'):
                 p_astro_filename = fv
             if combined_skymap_needed \
                     and {'sky_loc', 'ext_coinc'}.issubset(t) \
                     and f.startswith('combined-ext.') \
                     and 'fit' in f:
@@ -1084,17 +1095,20 @@
     # (see comment before defining kafka_alert_canvas)
     voevent_significance = 0 if alert_type == 'less-significant' else 1
 
     if filecontents and not combined_skymap_filename:
         skymap, em_bright, p_astro = filecontents
 
         # check high profile and apply label if true
-        high_profile_canvas = rrt_utils.check_high_profile.si(
-            skymap, em_bright, p_astro, superevent
-        )
+        if alert_type == 'preliminary':
+            high_profile_canvas = rrt_utils.check_high_profile.si(
+                skymap, em_bright, p_astro, superevent
+            )
+        else:
+            high_profile_canvas = identity.si()
 
         download_andor_expose_group = []
 
         voevent_canvas = _create_voevent.si(
             (em_bright, p_astro),
             superevent_id,
             alert_type_voevent,
```

### Comparing `gwcelery-2.1.1/gwcelery/tasks/p_astro.py` & `gwcelery-2.1.2/gwcelery/tasks/p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/raven.py` & `gwcelery-2.1.2/gwcelery/tasks/raven.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from .core import identity
 from . import external_skymaps
 from . import gracedb
 
 log = get_task_logger(__name__)
 
 
-@app.task(queue='exttrig',
-          shared=False)
+@app.task(shared=False)
 def calculate_coincidence_far(superevent, exttrig, tl, th,
                               use_superevent_skymap=None):
     """Compute coincidence FAR for external trigger and superevent
     coincidence by calling ligo.raven.search.calc_signif_gracedb,
     using sky map info if available.
 
     Parameters
@@ -69,16 +68,15 @@
                    superevent_id, exttrig_id, tl, th,
                    se_dict=superevent, ext_dict=exttrig,
                    grb_search=exttrig['search'],
                    incl_sky=False, gracedb=gracedb.client,
                    far_grb=exttrig['far'])
 
 
-@app.task(queue='exttrig',
-          shared=False)
+@app.task(shared=False)
 def coincidence_search(gracedb_id, alert_object, group=None, pipelines=[],
                        searches=[], se_searches=[]):
     """Perform ligo-raven search for coincidences. Determines time window to
     use. If events found, launches raven pipeline.
 
     Parameters
     ----------
@@ -149,16 +147,15 @@
     if 'S' in gracedb_id:
         # If triggering on a superevent, need to reverse the time window
         tl, th = -th, -tl
 
     return tl, th
 
 
-@app.task(queue='exttrig',
-          shared=False)
+@app.task(shared=False)
 def search(gracedb_id, alert_object, tl=-5, th=5, group=None,
            pipelines=[], searches=[], se_searches=[]):
     """Perform ligo-raven search for coincidences.
 
     Parameters
     ----------
     gracedb_id: str
@@ -188,16 +185,15 @@
                                     event_dict=alert_object,
                                     gracedb=gracedb.client,
                                     group=group, pipelines=pipelines,
                                     searches=searches,
                                     se_searches=se_searches)
 
 
-@app.task(queue='exttrig',
-          shared=False)
+@app.task(shared=False)
 def raven_pipeline(raven_search_results, gracedb_id, alert_object, tl, th,
                    gw_group, use_superevent_skymap=None):
     """Executes much of the full raven pipeline, including adding
     the external trigger to the superevent, calculating the
     coincidence false alarm rate, and applying 'EM_COINC' to the
     appropriate events. Also a preimlinary alert will be triggered
     if the coincidence passes threshold.
@@ -249,16 +245,15 @@
                   gracedb.create_label.si('EM_COINC', exttrig_id),
                   trigger_raven_alert.s(superevent, gracedb_id,
                                         ext_event, gw_group))
         )
         canvas.delay()
 
 
-@app.task(queue='exttrig',
-          shared=False)
+@app.task(shared=False)
 def preferred_superevent(raven_search_results):
     """Chooses the superevent with the lowest far for an external
     event to be added to. This is to prevent errors from trying to
     add one external event to multiple superevents.
 
     Parameters
     ----------
@@ -267,16 +262,15 @@
 
     """
     minfar, idx = min((result['far'], idx) for (idx, result) in
                       enumerate(raven_search_results))
     return [raven_search_results[idx]]
 
 
-@app.task(queue='exttrig',
-          shared=False)
+@app.task(shared=False)
 def update_coinc_far(coinc_far_dict, superevent, ext_event):
     """Update joint info in superevent based on the current preferred
     coincidence. This prefers a spacetime joint FAR over a time-only joint
     FAR. A SNEWS coincidence is preferred over either.
 
       Parameters
     ----------
@@ -346,16 +340,15 @@
     if is_event_improved and not snews_to_grb:
         gracedb.update_superevent(superevent_id, em_type=ext_id,
                                   time_coinc_far=new_time_far,
                                   space_coinc_far=new_space_far)
     return coinc_far_dict
 
 
-@app.task(queue='exttrig',
-          shared=False)
+@app.task(shared=False)
 def trigger_raven_alert(coinc_far_dict, superevent, gracedb_id,
                         ext_event, gw_group):
     """Determine whether an event should be published as a preliminary alert.
     If yes, then triggers an alert by applying `RAVEN_ALERT` to the preferred
     event.
 
     All of the following conditions must be true for a preliminary alert:
@@ -497,16 +490,15 @@
             alert_canvas,
             external_skymaps.plot_overlap_integral.s(superevent, ext_event),
             *messages
         )
     ).delay()
 
 
-@app.task(queue='exttrig',
-          shared=False)
+@app.task(shared=False)
 def sog_paper_pipeline(ext_event, superevent):
     """Determine whether an a speed of gravity measurment manuscript should be
     triggered for a given coincidence.
     This is denoted by applying the SOG_READY label to a superevent.
 
     All of the following conditions must be true for a SoG paper:
```

### Comparing `gwcelery-2.1.1/gwcelery/tasks/rrt_utils.py` & `gwcelery-2.1.2/gwcelery/tasks/rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/skymaps.py` & `gwcelery-2.1.2/gwcelery/tasks/skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tasks/superevents.py` & `gwcelery-2.1.2/gwcelery/tasks/superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/templates/fits_header.jinja2` & `gwcelery-2.1.2/gwcelery/templates/fits_header.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/templates/index.jinja2` & `gwcelery-2.1.2/gwcelery/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/templates/lalinference.jinja2` & `gwcelery-2.1.2/gwcelery/templates/lalinference.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/templates/rapidpe.jinja2` & `gwcelery-2.1.2/gwcelery/templates/rapidpe.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 web_dir={{ webdir }}
 
 [Event]
 superevent_id={{ superevent_id }}
 run_mode={{ run_mode }}
 frame_data_types={{ frame_data_types | tojson }}
+query_shm=True
 mdc_event_injection_file =/home/vinaya.valsan/rapidPE/RapidPE_RIFT_Developments/RapidPE-RIFT_fork/gracedb_playground_events/injection_campaign_studies/lowlatency-replay-distributions/minSNR-4/injections-minSNR-4.xml.gz
 mdc_time_offset=101760000
 #Anything specified in this section is passed verbatim to rapidpe_compute_intrinsic_grid in generate_initial_grid_based_of_gstlal_O2_overlaps.py
 [InitialGridOnly]
 #mc-min = 5
 #mc-max = 61
 points-per-side=10
```

### Comparing `gwcelery-2.1.1/gwcelery/tests/conftest.py` & `gwcelery-2.1.2/gwcelery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/G000012_S0040_preferred.json` & `gwcelery-2.1.2/gwcelery/tests/data/G000012_S0040_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/G298048-1-Initial.xml` & `gwcelery-2.1.2/gwcelery/tests/data/G298048-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/G298048_log.json` & `gwcelery-2.1.2/gwcelery/tests/data/G298048_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json` & `gwcelery-2.1.2/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/MS220722v.xml` & `gwcelery-2.1.2/gwcelery/tests/data/MS220722v.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits` & `gwcelery-2.1.2/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/S230413b.json` & `gwcelery-2.1.2/gwcelery/tests/data/S230413b.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/S230413g.json` & `gwcelery-2.1.2/gwcelery/tests/data/S230413g.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/S230413h.json` & `gwcelery-2.1.2/gwcelery/tests/data/S230413h.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/T0212_S0039_preferred.json` & `gwcelery-2.1.2/gwcelery/tests/data/T0212_S0039_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json` & `gwcelery-2.1.2/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/T0219_S0041_nopreferred.json` & `gwcelery-2.1.2/gwcelery/tests/data/T0219_S0041_nopreferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/agile_grb_gcn.xml` & `gwcelery-2.1.2/gwcelery/tests/data/agile_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/coinc.xml` & `gwcelery-2.1.2/gwcelery/tests/data/coinc.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/externaltrigger_original_data.xml` & `gwcelery-2.1.2/gwcelery/tests/data/externaltrigger_original_data.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/fermi_grb_gcn.xml` & `gwcelery-2.1.2/gwcelery/tests/data/fermi_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/fermi_initial_grb_gcn.xml` & `gwcelery-2.1.2/gwcelery/tests/data/fermi_initial_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/fermi_noise_gcn.xml` & `gwcelery-2.1.2/gwcelery/tests/data/fermi_noise_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/fermi_noise_gcn_2.xml` & `gwcelery-2.1.2/gwcelery/tests/data/fermi_noise_gcn_2.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml` & `gwcelery-2.1.2/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml` & `gwcelery-2.1.2/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/fits_header_result.html` & `gwcelery-2.1.2/gwcelery/tests/data/fits_header_result.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/gracedb_externaltrigger_log.json` & `gwcelery-2.1.2/gwcelery/tests/data/gracedb_externaltrigger_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_detchar.json` & `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_detchar.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_exttrig_creation.json` & `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_exttrig_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json` & `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_psd.json` & `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_psd.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_snews_creation.json` & `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_snews_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_snews_test_creation.json` & `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_snews_test_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_subgrb_creation.json` & `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_subgrb_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_superevent_creation.json` & `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_superevent_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/igwn_alert_voevent.json` & `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_voevent.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/integral_grb_gcn.xml` & `gwcelery-2.1.2/gwcelery/tests/data/integral_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/integral_mdc_gcn.xml` & `gwcelery-2.1.2/gwcelery/tests/data/integral_mdc_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.2/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files 9% similar despite different names*

```diff
@@ -146,22 +146,22 @@
 00000910: 2066 6f72 2074 6865 2066 6972 7374 2061   for the first a
 00000920: 7578 696c 6961 7279 2074 6162 6c65 2064  uxiliary table d
 00000930: 6174 6100 209f 3edd 3600 0000 0000 0000  ata. .>.6.......
 00000940: 0102 1500 0000 0700 6368 6b53 756d 0007  ........chkSum..
 00000950: 0049 4e54 5f34 5500 1000 5374 7275 6374  .INT_4U...Struct
 00000960: 2063 6865 636b 7375 6d00 bccb b902 8500   checksum.......
 00000970: 0000 0000 0000 0103 0000 0000 0500 6777  ..............gw
-00000980: 7079 0000 0000 0000 0000 0000 0000 00b8  py..............
+00000980: 7079 0000 0000 002c 203c 5469 6d65 53b8  py....., <TimeS.
 00000990: 8183 4800 0000 0025 0000 0000 0000 0010  ..H....%........
 000009a0: 4000 0000 0000 0000 0000 0000 0000 0000  @...............
 000009b0: 0000 0005 0000 0000 0000 0000 0000 0000  ................
 000009c0: 0000 0000 000b 0000 0000 0000 0000 0000  ................
 000009d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000009e0: 0000 0000 0000 0000 0000 0000 0000 0047  ...............G
-000009f0: 6661 b63b 0000 0000 0000 0001 0101 0000  fa.;............
+000009e0: 0000 0000 0000 0000 0000 0000 0000 00be  ................
+000009f0: 448c 8c3b 0000 0000 0000 0001 0101 0000  D..;............
 00000a00: 000b 0046 7244 6574 6563 746f 7200 0500  ...FrDetector...
 00000a10: 1800 4465 7465 6374 6f72 2044 6174 6120  ..Detector Data 
 00000a20: 5374 7275 6374 7572 6500 94bd 3e10 2500  Structure...>.%.
 00000a30: 0000 0000 0000 0102 1600 0000 0500 6e61  ..............na
 00000a40: 6d65 0007 0053 5452 494e 4700 0100 006c  me...STRING....l
 00000a50: ebf8 8528 0000 0000 0000 0001 0217 0000  ...(............
 00000a60: 0007 0070 7265 6669 7800 0800 4348 4152  ...prefix...CHAR
@@ -203,20 +203,20 @@
 00000ca0: 0000 0005 006e 6578 7400 1900 5054 525f  .....next...PTR_
 00000cb0: 5354 5255 4354 2846 7244 6574 6563 746f  STRUCT(FrDetecto
 00000cc0: 7220 2a29 0001 0000 9c02 f62a 3600 0000  r *).......*6...
 00000cd0: 0000 0000 0102 2500 0000 0700 6368 6b53  ......%.....chkS
 00000ce0: 756d 0007 0049 4e54 5f34 5500 1000 5374  um...INT_4U...St
 00000cf0: 7275 6374 2063 6865 636b 7375 6d00 60e8  ruct checksum.`.
 00000d00: f252 5f00 0000 0000 0000 0105 0000 0000  .R_.............
-00000d10: 0700 4c4c 4f5f 346b 004c 31b7 9c4b 7155  ..LLO_4k.L1..KqU
-00000d20: 59f9 bf08 e57d 1ccd 11e1 3f35 5ed2 c0da  Y....}....?5^...
-00000d30: e68c 40b7 4535 405a a1a3 b962 1720 ba3d  ..@.E5@Z...b. .=
-00000d40: b2f9 443d b2f9 4400 0000 0000 0000 0000  ..D=..D.........
-00000d50: 0000 0000 0000 0000 0000 0000 00a3 1c37  ...............7
-00000d60: 8541 0000 0000 0000 0001 0102 0000 000b  .A..............
+00000d10: 0700 4c48 4f5f 346b 0048 31ce 3637 a627  ..LHO_4k.H1.67.'
+00000d20: ac00 c08b 5418 5b08 f2e9 3fd3 8d0e 43c7  ....T.[...?...C.
+00000d30: f4b4 40bf b682 40f1 6522 ba17 b751 3748  ..@...@.e"...Q7H
+00000d40: b1f9 44a4 b0f9 4400 0000 0000 0000 0000  ..D...D.........
+00000d50: 0000 0000 0000 0000 0000 0000 00db 6303  ..............c.
+00000d60: e441 0000 0000 0000 0001 0102 0000 000b  .A..............
 00000d70: 0046 7250 726f 6344 6174 6100 0b00 1e00  .FrProcData.....
 00000d80: 506f 7374 2d50 726f 6365 7373 6564 2044  Post-Processed D
 00000d90: 6174 6120 5374 7275 6374 7572 6500 1cf9  ata Structure...
 00000da0: 1b5b 3900 0000 0000 0000 0102 2600 0000  .[9.........&...
 00000db0: 0500 6e61 6d65 0007 0053 5452 494e 4700  ..name...STRING.
 00000dc0: 1500 4461 7461 206f 7220 6368 616e 6e65  ..Data or channe
 00000dd0: 6c20 6e61 6d65 0064 4e94 5e2f 0000 0000  l name.dN.^/....
@@ -314,601 +314,622 @@
 00001390: 7469 6669 6572 2066 6f72 206e 6578 7420  tifier for next 
 000013a0: 4672 5072 6f63 4461 7461 2073 7472 7563  FrProcData struc
 000013b0: 7475 7265 2069 6e20 7468 6520 6c69 6e6b  ture in the link
 000013c0: 6564 206c 6973 7400 e888 67b1 3600 0000  ed list...g.6...
 000013d0: 0000 0000 0102 3800 0000 0700 6368 6b53  ......8.....chkS
 000013e0: 756d 0007 0049 4e54 5f34 5500 1000 5374  um...INT_4U...St
 000013f0: 7275 6374 2063 6865 636b 7375 6d00 7e66  ruct checksum.~f
-00001400: 8ab6 8800 0000 0000 0000 010b 0000 0000  ................
-00001410: 1100 4c31 3a44 4d54 2d44 515f 5645 4354  ..L1:DMT-DQ_VECT
-00001420: 4f52 0011 004c 313a 444d 542d 4451 5f56  OR...L1:DMT-DQ_V
-00001430: 4543 544f 5200 0100 0000 0000 0000 0000  ECTOR...........
-00001440: 0000 0000 0000 0000 1040 0000 0000 0000  .........@......
-00001450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001460: 0000 0000 0000 0000 1400 0000 0000 0000  ................
-00001470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001480: 0b00 0100 0000 cdee 28c4 3500 0000 0000  ........(.5.....
-00001490: 0000 0101 0300 0000 0700 4672 5665 6374  ..........FrVect
-000014a0: 0014 0016 0056 6563 746f 7220 4461 7461  .....Vector Data
-000014b0: 2053 7472 7563 7475 7265 00af a279 264e   Structure...y&N
-000014c0: 0000 0000 0000 0001 0239 0000 0005 006e  .........9.....n
-000014d0: 616d 6500 0700 5354 5249 4e47 002a 0043  ame...STRING.*.C
-000014e0: 6861 6e6e 656c 206e 616d 6520 2d2d 206e  hannel name -- n
-000014f0: 6f74 2072 6571 7569 7265 6420 746f 2062  ot required to b
-00001500: 6520 756e 6971 7565 0023 3580 8545 0000  e unique.#5..E..
-00001510: 0000 0000 0001 023a 0000 0009 0063 6f6d  .......:.....com
-00001520: 7072 6573 7300 0700 494e 545f 3255 001d  press...INT_2U..
-00001530: 0043 6f6d 7072 6573 7369 6f6e 2061 6c67  .Compression alg
-00001540: 6f72 6974 686d 206e 756d 6265 7200 b1fa  orithm number...
-00001550: 026c 3100 0000 0000 0000 0102 3b00 0000  .l1.........;...
-00001560: 0500 7479 7065 0007 0049 4e54 5f32 5500  ..type...INT_2U.
-00001570: 0d00 5665 6374 6f72 2063 6c61 7373 0013  ..Vector class..
-00001580: fdab ae4e 0000 0000 0000 0001 023c 0000  ...N.........<..
-00001590: 0006 006e 4461 7461 0007 0049 4e54 5f38  ...nData...INT_8
-000015a0: 5500 2900 4e75 6d62 6572 206f 6620 7361  U.).Number of sa
-000015b0: 6d70 6c65 2065 6c65 6d65 6e74 7320 696e  mple elements in
-000015c0: 2064 6174 6120 7365 7269 6573 0092 220f   data series..".
-000015d0: 634f 0000 0000 0000 0001 023d 0000 0007  cO.........=....
-000015e0: 006e 4279 7465 7300 0700 494e 545f 3855  .nBytes...INT_8U
-000015f0: 0029 004e 756d 6265 7220 6f66 2062 7974  .).Number of byt
-00001600: 6573 2069 6e20 7468 6520 636f 6d70 7265  es in the compre
-00001610: 7373 6564 2076 6563 746f 7200 fe47 a552  ssed vector..G.R
-00001620: 4c00 0000 0000 0000 0102 3e00 0000 0500  L.........>.....
-00001630: 6461 7461 000d 0043 4841 525b 6e42 7974  data...CHAR[nByt
-00001640: 6573 5d00 2200 6e44 6174 6120 656c 656d  es].".nData elem
-00001650: 656e 7473 206f 6620 7370 6563 6966 6965  ents of specifie
-00001660: 6420 636c 6173 7300 d461 1f2e 4200 0000  d class..a..B...
-00001670: 0000 0000 0102 3f00 0000 0500 6e44 696d  ......?.....nDim
-00001680: 0007 0049 4e54 5f34 5500 1e00 4469 6d65  ...INT_4U...Dime
-00001690: 6e73 696f 6e61 6c69 7479 206f 6620 6461  nsionality of da
-000016a0: 7461 2076 6563 746f 7200 cd27 6340 3a00  ta vector..'c@:.
-000016b0: 0000 0000 0000 0102 4000 0000 0300 6e78  ........@.....nx
-000016c0: 000d 0049 4e54 5f38 555b 6e44 696d 5d00  ...INT_8U[nDim].
-000016d0: 1200 6469 6d65 6e73 696f 6e20 6c65 6e67  ..dimension leng
-000016e0: 7468 7300 403d c725 4d00 0000 0000 0000  ths.@=.%M.......
-000016f0: 0102 4100 0000 0300 6478 000d 0052 4541  ..A.....dx...REA
-00001700: 4c5f 385b 6e44 696d 5d00 2500 7361 6d70  L_8[nDim].%.samp
-00001710: 6c65 2073 7061 6369 6e67 2061 6c6f 6e67  le spacing along
-00001720: 2065 6163 6820 636f 6f72 6469 6e61 7465   each coordinate
-00001730: 00ac b934 e445 0000 0000 0000 0001 0242  ...4.E.........B
-00001740: 0000 0007 0073 7461 7274 5800 0d00 5245  .....startX...RE
-00001750: 414c 5f38 5b6e 4469 6d5d 0019 004f 7269  AL_8[nDim]...Ori
-00001760: 6769 6e20 666f 7220 6561 6368 2064 6174  gin for each dat
-00001770: 6120 7365 7400 d235 5772 4200 0000 0000  a set..5WrB.....
-00001780: 0000 0102 4300 0000 0600 756e 6974 5800  ....C.....unitX.
-00001790: 0d00 5354 5249 4e47 5b6e 4469 6d5d 0017  ..STRING[nDim]..
-000017a0: 0073 6361 6c65 2066 6163 746f 7273 2069  .scale factors i
-000017b0: 6e20 4153 4349 4900 5d23 1276 6200 0000  n ASCII.]#.vb...
-000017c0: 0000 0000 0102 4400 0000 0600 756e 6974  ......D.....unit
-000017d0: 5900 0700 5354 5249 4e47 003d 0053 7472  Y...STRING.=.Str
-000017e0: 696e 6720 6465 7363 7269 6269 6e67 2068  ing describing h
-000017f0: 6f77 2074 6f20 696e 7465 7270 7265 7420  ow to interpret 
-00001800: 7468 6520 7661 6c75 6520 6f66 2065 6163  the value of eac
-00001810: 6820 656c 656d 656e 7400 bc2b a817 5200  h element..+..R.
-00001820: 0000 0000 0000 0102 4500 0000 0500 6e65  ........E.....ne
-00001830: 7874 0015 0050 5452 5f53 5452 5543 5428  xt...PTR_STRUCT(
-00001840: 4672 5665 6374 202a 2900 2000 4964 656e  FrVect *). .Iden
-00001850: 7469 6669 6572 2066 6f72 2061 6464 6974  tifier for addit
-00001860: 696f 6e61 6c20 6461 7461 2e00 bb79 c453  ional data...y.S
-00001870: 3600 0000 0000 0000 0102 4600 0000 0700  6.........F.....
-00001880: 6368 6b53 756d 0007 0049 4e54 5f34 5500  chkSum...INT_4U.
-00001890: 1000 5374 7275 6374 2063 6865 636b 7375  ..Struct checksu
-000018a0: 6d00 885a 50b6 7000 0000 0000 0000 0114  m..ZP.p.........
-000018b0: 0000 0000 1100 4c31 3a44 4d54 2d44 515f  ......L1:DMT-DQ_
-000018c0: 5645 4354 4f52 0001 0105 0040 0000 0000  VECTOR.....@....
-000018d0: 0000 000e 0000 0000 0000 0078 9c63 6018  ...........x.c`.
-000018e0: 0523 1900 0002 0000 0101 0000 0040 0000  .#...........@..
-000018f0: 0000 0000 0000 0000 0000 00b0 3f00 0000  ............?...
-00001900: 0000 0000 0002 0073 0001 0000 0000 0000  .......s........
-00001910: 0000 8488 0b13 9a00 0000 0000 0000 010b  ................
-00001920: 0100 0000 1a00 4c31 3a47 4453 2d43 414c  ......L1:GDS-CAL
-00001930: 4942 5f53 5441 5445 5f56 4543 544f 5200  IB_STATE_VECTOR.
-00001940: 1a00 4c31 3a47 4453 2d43 414c 4942 5f53  ..L1:GDS-CALIB_S
-00001950: 5441 5445 5f56 4543 544f 5200 0100 0000  TATE_VECTOR.....
-00001960: 0000 0000 0000 0000 0000 0000 0000 1040  ...............@
-00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001980: 0000 0000 0000 0000 0000 0000 0000 1400  ................
-00001990: 0100 0000 0000 0000 0000 0000 0000 0000  ................
-000019a0: 0000 0000 0000 0b00 0200 0000 7d7b 0ea0  ............}{..
-000019b0: 7900 0000 0000 0000 0114 0100 0000 1a00  y...............
-000019c0: 4c31 3a47 4453 2d43 414c 4942 5f53 5441  L1:GDS-CALIB_STA
-000019d0: 5445 5f56 4543 544f 5200 0101 0500 4000  TE_VECTOR.....@.
-000019e0: 0000 0000 0000 0e00 0000 0000 0000 789c  ..............x.
-000019f0: 6360 1805 2319 0000 0200 0001 0100 0000  c`..#...........
-00001a00: 4000 0000 0000 0000 0000 0000 0000 b03f  @..............?
-00001a10: 0000 0000 0000 0000 0200 7300 0100 0000  ..........s.....
-00001a20: 0000 0000 000d 1572 bf94 0000 0000 0000  .......r........
-00001a30: 0001 0b02 0000 0017 004c 313a 4944 512d  .........L1:IDQ-
-00001a40: 4641 505f 4f56 4c5f 3332 5f32 3034 3800  FAP_OVL_32_2048.
-00001a50: 1700 4c31 3a49 4451 2d46 4150 5f4f 564c  ..L1:IDQ-FAP_OVL
-00001a60: 5f33 325f 3230 3438 0001 0000 0000 0000  _32_2048........
-00001a70: 0000 0000 0000 0000 0000 0010 4000 0000  ............@...
-00001a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001a90: 0000 0000 0000 0000 0000 0014 0002 0000  ................
-00001aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ab0: 0000 0000 0000 0000 0017 3b04 fb87 0000  ..........;.....
-00001ac0: 0000 0000 0001 1402 0000 0017 004c 313a  .............L1:
-00001ad0: 4944 512d 4641 505f 4f56 4c5f 3332 5f32  IDQ-FAP_OVL_32_2
-00001ae0: 3034 3800 0101 0500 0004 0000 0000 0000  048.............
-00001af0: 1f00 0000 0000 0000 789c edc1 010d 0000  ........x.......
-00001b00: 00c2 a0f7 4f6d 0e37 a000 0000 0000 0000  ....Om.7........
-00001b10: 8077 0320 0000 0101 0000 0000 0400 0000  .w. ............
-00001b20: 0000 0000 0000 0000 0070 3f00 0000 0000  .........p?.....
-00001b30: 0000 0002 0073 0001 0000 0000 0000 0000  .....s..........
-00001b40: 913f 116f 4100 0000 0000 0000 0101 0400  .?.oA...........
-00001b50: 0000 0d00 4672 456e 644f 6646 7261 6d65  ....FrEndOfFrame
-00001b60: 0007 001c 0045 6e64 206f 6620 4672 616d  .....End of Fram
-00001b70: 6520 4461 7461 2053 7472 7563 7475 7265  e Data Structure
-00001b80: 009c ab33 e258 0000 0000 0000 0001 0247  ...3.X.........G
-00001b90: 0000 0004 0072 756e 0007 0049 4e54 5f34  .....run...INT_4
-00001ba0: 5300 3500 5275 6e20 6e75 6d62 6572 3b20  S.5.Run number; 
-00001bb0: 7361 6d65 2061 7320 696e 2046 7261 6d65  same as in Frame
-00001bc0: 4865 6164 6572 2072 756e 206e 756d 6265  Header run numbe
-00001bd0: 7220 6461 7475 6d2e 000b 9641 5b87 0000  r datum....A[...
-00001be0: 0000 0000 0001 0248 0000 0006 0066 7261  .......H.....fra
-00001bf0: 6d65 0007 0049 4e54 5f34 5500 6200 4672  me...INT_4U.b.Fr
-00001c00: 616d 6520 6e75 6d62 6572 2c20 6d6f 6e6f  ame number, mono
-00001c10: 746f 6e69 6361 6c6c 7920 696e 6372 6561  tonically increa
-00001c20: 7369 6e67 2075 6e74 696c 2065 6e64 206f  sing until end o
-00001c30: 6620 7275 6e3b 2073 616d 6520 6173 2069  f run; same as i
-00001c40: 6e20 4672 616d 6520 4865 6164 6572 2072  n Frame Header r
-00001c50: 756e 206e 756d 6265 7220 6461 7475 6d00  un number datum.
-00001c60: ba5a b3d1 4700 0000 0000 0000 0102 4900  .Z..G.........I.
-00001c70: 0000 0700 4754 696d 6553 0007 0049 4e54  ....GTimeS...INT
-00001c80: 5f34 5500 2100 4672 616d 6520 7374 6172  _4U.!.Frame star
-00001c90: 7420 7469 6d65 2069 6e20 4750 5320 5365  t time in GPS Se
-00001ca0: 636f 6e64 732e 0018 add0 ff56 0000 0000  conds......V....
-00001cb0: 0000 0001 024a 0000 0007 0047 5469 6d65  .....J.....GTime
-00001cc0: 4e00 0700 494e 545f 3455 0030 0046 7261  N...INT_4U.0.Fra
-00001cd0: 6d65 2073 7461 7274 2074 696d 6520 7265  me start time re
-00001ce0: 7369 6475 616c 2c20 696e 7465 6765 7220  sidual, integer 
-00001cf0: 6e61 6e6f 7365 636f 6e64 732e 0064 338f  nanoseconds..d3.
-00001d00: ba36 0000 0000 0000 0001 024b 0000 0007  .6.........K....
-00001d10: 0063 686b 5375 6d00 0700 494e 545f 3455  .chkSum...INT_4U
-00001d20: 0010 0053 7472 7563 7420 6368 6563 6b73  ...Struct checks
-00001d30: 756d 0022 ca11 6222 0000 0000 0000 0001  um."..b"........
-00001d40: 0700 0000 0000 0000 0000 0000 0000 0000  ................
-00001d50: 0000 0000 00c9 70fa 3b37 0000 0000 0000  ......p.;7......
-00001d60: 0001 0100 0000 0006 0046 7254 4f43 0013  .........FrTOC..
-00001d70: 0019 0053 696d 756c 6174 6564 2044 6174  ...Simulated Dat
-00001d80: 6120 5374 7275 6374 7572 6500 7c69 656b  a Structure.|iek
-00001d90: 4800 0000 0000 0000 0102 0000 0000 0700  H...............
-00001da0: 554c 6561 7053 0007 0049 4e54 5f32 5300  ULeapS...INT_2S.
-00001db0: 2200 4672 6f6d 2074 6865 2066 6972 7374  ".From the first
-00001dc0: 2046 7261 6d65 4820 696e 2074 6865 2066   FrameH in the f
-00001dd0: 696c 6500 0087 5256 4300 0000 0000 0000  ile...RVC.......
-00001de0: 0102 0100 0000 0700 6e46 7261 6d65 0007  ........nFrame..
-00001df0: 0049 4e54 5f34 5500 1d00 4e75 6d62 6572  .INT_4U...Number
-00001e00: 206f 6620 6672 616d 6573 2069 6e20 7468   of frames in th
-00001e10: 6520 6669 6c65 00cc 3d5f 7370 0000 0000  e file..=_sp....
-00001e20: 0000 0001 0202 0000 000c 0064 6174 6151  ...........dataQ
-00001e30: 7561 6c69 7479 000f 0049 4e54 5f34 555b  uality...INT_4U[
-00001e40: 6e46 7261 6d65 5d00 3d00 4172 7261 7920  nFrame].=.Array 
-00001e50: 6f66 2069 6e74 6567 6572 2051 4120 776f  of integer QA wo
-00001e60: 7264 7320 6672 6f6d 2065 6163 6820 4672  rds from each Fr
-00001e70: 616d 6548 2028 7369 7a65 206f 6620 6e46  ameH (size of nF
-00001e80: 7261 6d65 7329 0088 6738 c05f 0000 0000  rames)..g8._....
-00001e90: 0000 0001 0203 0000 0007 0047 5469 6d65  ...........GTime
-00001ea0: 5300 0f00 494e 545f 3455 5b6e 4672 616d  S...INT_4U[nFram
-00001eb0: 655d 0031 0041 7272 6179 206f 6620 696e  e].1.Array of in
-00001ec0: 7465 6765 7220 4750 5320 6672 6165 2074  teger GPS frae t
-00001ed0: 696d 6573 2028 7369 7a65 206f 6620 6e46  imes (size of nF
-00001ee0: 7261 6d65 7300 d5b2 6755 7600 0000 0000  rames...gUv.....
-00001ef0: 0000 0102 0400 0000 0700 4754 696d 654e  ..........GTimeN
-00001f00: 000f 0049 4e54 5f34 555b 6e46 7261 6d65  ...INT_4U[nFrame
-00001f10: 5d00 4800 4172 7261 7920 6f66 2069 6e74  ].H.Array of int
-00001f20: 6567 6572 2047 5053 2072 6573 6964 7561  eger GPS residua
-00001f30: 6c20 6e61 6e6f 7365 636f 6e64 7320 666f  l nanoseconds fo
-00001f40: 7220 7468 6520 6672 616d 6520 2873 697a  r the frame (siz
-00001f50: 6520 6f66 206e 4672 616d 6500 154d fabb  e of nFrame..M..
-00001f60: 6000 0000 0000 0000 0102 0500 0000 0300  `...............
-00001f70: 6474 000f 0052 4541 4c5f 385b 6e46 7261  dt...REAL_8[nFra
-00001f80: 6d65 5d00 3600 4172 7261 7920 6f66 2066  me].6.Array of f
-00001f90: 7261 6d65 2064 7572 6174 696f 6e73 2069  rame durations i
-00001fa0: 6e20 7365 636f 6e64 7328 2073 697a 6520  n seconds( size 
-00001fb0: 6f66 206e 4672 616d 6573 2900 0d06 b877  of nFrames)....w
-00001fc0: 5200 0000 0000 0000 0102 0600 0000 0500  R...............
-00001fd0: 7275 6e73 000f 0049 4e54 5f34 535b 6e46  runs...INT_4S[nF
-00001fe0: 7261 6d65 5d00 2600 4172 7261 7920 6f66  rame].&.Array of
-00001ff0: 2072 756e 206e 756d 6265 7273 2028 7369   run numbers (si
-00002000: 7a65 206f 6620 6e46 7261 6d65 2900 ca0b  ze of nFrame)...
-00002010: 9f5c 5500 0000 0000 0000 0102 0700 0000  .\U.............
-00002020: 0600 6672 616d 6500 0f00 494e 545f 3455  ..frame...INT_4U
-00002030: 5b6e 4672 616d 655d 0028 0041 7272 6179  [nFrame].(.Array
-00002040: 206f 6620 6672 616d 6520 6e75 6d62 6572   of frame number
-00002050: 7320 2873 697a 6520 6f66 206e 4672 616d  s (size of nFram
-00002060: 6529 0031 285d 2581 0000 0000 0000 0001  e).1(]%.........
-00002070: 0208 0000 000a 0070 6f73 6974 696f 6e48  .......positionH
-00002080: 000f 0049 4e54 5f38 555b 6e46 7261 6d65  ...INT_8U[nFrame
-00002090: 5d00 5000 4172 7261 7920 6f66 2046 7261  ].P.Array of Fra
-000020a0: 6d65 4820 706f 7369 7469 6f6e 732c 2069  meH positions, i
-000020b0: 6e20 6279 7465 732c 2066 726f 6d20 7468  n bytes, from th
-000020c0: 6520 6267 696e 6e69 6e67 206f 6620 6669  e bginning of fi
-000020d0: 6c65 2028 7369 7a65 206f 6620 6e46 7261  le (size of nFra
-000020e0: 6d65 2900 db18 22e8 8700 0000 0000 0000  me)...".........
-000020f0: 0102 0900 0000 0a00 6e46 6972 7374 4144  ........nFirstAD
-00002100: 4300 0f00 494e 545f 3855 5b6e 4672 616d  C...INT_8U[nFram
-00002110: 655d 0056 0041 7272 6179 206f 6620 6669  e].V.Array of fi
-00002120: 7273 7420 4672 4144 4344 6174 6120 706f  rst FrADCData po
-00002130: 7369 7469 6f6e 732c 2069 6e20 6279 7465  sitions, in byte
-00002140: 732c 2066 726f 6d20 6265 6769 6e6e 696e  s, from beginnin
-00002150: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
-00002160: 6f66 206e 4672 616d 6529 00b7 d5cd 8b86  of nFrame)......
-00002170: 0000 0000 0000 0001 020a 0000 000a 006e  ...............n
-00002180: 4669 7273 7453 6572 000f 0049 4e54 5f38  FirstSer...INT_8
-00002190: 555b 6e46 7261 6d65 5d00 5500 4172 7261  U[nFrame].U.Arra
-000021a0: 7920 6f66 2066 6972 7374 2046 7253 6572  y of first FrSer
-000021b0: 4461 7461 2070 6f73 6974 696f 6e73 2069  Data positions i
-000021c0: 6e20 6279 7465 732c 2066 726f 6d20 6265  n bytes, from be
-000021d0: 6769 6e6e 696e 6720 6f66 2066 696c 6520  ginning of file 
-000021e0: 2873 697a 6520 6f66 206e 4672 616d 6529  (size of nFrame)
-000021f0: 00fa c761 6b87 0000 0000 0000 0001 020b  ...ak...........
-00002200: 0000 000c 006e 4669 7273 7454 6162 6c65  .....nFirstTable
-00002210: 000f 0049 4e54 5f38 555b 6e46 7261 6d65  ...INT_8U[nFrame
-00002220: 5d00 5400 4172 7261 7920 6f66 2066 6972  ].T.Array of fir
-00002230: 7374 2046 7254 6162 6c65 2070 6f73 6974  st FrTable posit
-00002240: 696f 6e73 2c20 696e 2062 7974 6573 2c20  ions, in bytes, 
-00002250: 6672 6f6d 2062 6567 696e 6e69 6e67 206f  from beginning o
-00002260: 6620 6669 6c65 2028 7369 7a65 206f 6620  f file (size of 
-00002270: 6e46 7261 6d65 2900 1016 52a6 8300 0000  nFrame)...R.....
-00002280: 0000 0000 0102 0c00 0000 0a00 6e46 6972  ............nFir
-00002290: 7374 4d73 6700 0f00 494e 545f 3855 5b6e  stMsg...INT_8U[n
-000022a0: 4672 616d 655d 0052 0041 7272 6179 206f  Frame].R.Array o
-000022b0: 6620 6669 7273 7420 4672 4d73 6720 706f  f first FrMsg po
-000022c0: 7369 7469 6f6e 732c 2069 6e20 6279 7465  sitions, in byte
-000022d0: 732c 2066 726f 6d20 6265 6769 6e6e 696e  s, from beginnin
-000022e0: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
-000022f0: 6f66 206e 4672 616d 6529 00b9 e1c6 f949  of nFrame).....I
-00002300: 0000 0000 0000 0001 020d 0000 0004 006e  ...............n
-00002310: 5348 0007 0049 4e54 5f34 5500 2600 4e75  SH...INT_4U.&.Nu
-00002320: 6d62 6572 206f 6620 4672 5348 2073 7472  mber of FrSH str
-00002330: 7563 7475 7265 7320 696e 2074 6865 2066  uctures in the f
-00002340: 696c 6500 f46c 0bb0 4900 0000 0000 0000  ile..l..I.......
-00002350: 0102 0e00 0000 0500 5348 6964 000c 0049  ........SHid...I
-00002360: 4e54 5f32 555b 6e53 485d 0020 0041 7272  NT_2U[nSH]. .Arr
-00002370: 6179 206f 6620 4672 5348 2049 4473 2028  ay of FrSH IDs (
-00002380: 7369 7a65 206f 6620 6e53 4829 0010 5b23  size of nSH)..[#
-00002390: 074d 0000 0000 0000 0001 020f 0000 0007  .M..............
-000023a0: 0053 486e 616d 6500 0c00 5354 5249 4e47  .SHname...STRING
-000023b0: 5b6e 5348 5d00 2200 4172 7261 7920 6f66  [nSH].".Array of
-000023c0: 2046 7253 4820 6e61 6d65 7320 2873 697a   FrSH names (siz
-000023d0: 6520 6f66 206e 5348 2900 a664 b4df 5c00  e of nSH)..d..\.
-000023e0: 0000 0000 0000 0102 1000 0000 0a00 6e44  ..............nD
-000023f0: 6574 6563 746f 7200 0700 494e 545f 3455  etector...INT_4U
-00002400: 0033 004e 756d 6265 7220 6f66 2064 6973  .3.Number of dis
-00002410: 7469 6e63 7420 7479 7065 7320 6f66 2046  tinct types of F
-00002420: 7244 6574 6563 746f 7220 696e 2074 6865  rDetector in the
-00002430: 2066 696c 6500 fa46 0067 8100 0000 0000   file..F.g......
-00002440: 0000 0102 1100 0000 0d00 6e61 6d65 4465  ..........nameDe
-00002450: 7465 6374 6f72 0012 0053 5452 494e 475b  tector...STRING[
-00002460: 6e44 6574 6563 746f 725d 004a 0041 7272  nDetector].J.Arr
-00002470: 6179 206f 6620 4672 4465 7465 6374 6f72  ay of FrDetector
-00002480: 206e 616d 6573 2028 7369 7a65 206f 6620   names (size of 
-00002490: 6e44 6574 6563 746f 7229 2e20 5468 6579  nDetector). They
-000024a0: 2061 7070 6561 7220 616c 7068 6162 6574   appear alphabet
-000024b0: 6963 616c 6c79 0011 11d2 a589 0000 0000  ically..........
-000024c0: 0000 0001 0212 0000 0011 0070 6f73 6974  ...........posit
-000024d0: 696f 6e44 6574 6563 746f 7200 1200 494e  ionDetector...IN
-000024e0: 545f 3855 5b6e 4465 7465 6374 6f72 5d00  T_8U[nDetector].
-000024f0: 4e00 4172 7261 7920 6f66 2046 7244 6574  N.Array of FrDet
-00002500: 6563 746f 7220 706f 7369 7469 6f6e 7320  ector positions 
-00002510: 6672 6f6d 2074 6865 2062 6567 696e 6e69  from the beginni
-00002520: 6e67 206f 6620 6669 6c65 2028 7369 7a65  ng of file (size
-00002530: 206f 6620 6e44 6574 6563 746f 7229 2e00   of nDetector)..
-00002540: 8345 9ff0 5800 0000 0000 0000 0102 1300  .E..X...........
-00002550: 0000 0a00 6e53 7461 7454 7970 6500 0700  ....nStatType...
-00002560: 494e 545f 3455 002f 004e 756d 6265 7220  INT_4U./.Number 
-00002570: 6f66 2073 7461 7469 6320 6461 7461 2062  of static data b
-00002580: 6c6f 636b 2074 7970 6573 2069 6e20 7468  lock types in th
-00002590: 6520 6669 6c65 2e00 0f05 6246 6000 0000  e file....bF`...
-000025a0: 0000 0000 0102 1400 0000 0900 6e61 6d65  ............name
-000025b0: 5374 6174 0012 0053 5452 494e 475b 6e53  Stat...STRING[nS
-000025c0: 7461 7454 7970 655d 002d 0041 7272 6179  tatType].-.Array
-000025d0: 206f 6620 4672 5374 6174 4461 7461 206e   of FrStatData n
-000025e0: 616d 6520 2873 697a 6520 6f66 206e 5374  ame (size of nSt
-000025f0: 6174 5479 7065 2900 a3bf 4547 5d00 0000  atType)...EG]...
-00002600: 0000 0000 0102 1500 0000 0900 6465 7465  ............dete
-00002610: 6374 6f72 0012 0053 5452 494e 475b 6e53  ctor...STRING[nS
-00002620: 7461 7454 7970 655d 002a 0041 7272 6179  tatType].*.Array
-00002630: 206f 6620 4465 7465 6374 6f72 206e 616d   of Detector nam
-00002640: 6528 7369 7a65 206f 6620 6e53 7461 7454  e(size of nStatT
-00002650: 7970 6529 0041 b642 9d7b 0000 0000 0000  ype).A.B.{......
-00002660: 0001 0216 0000 000e 006e 5374 6174 496e  .........nStatIn
-00002670: 7374 616e 6365 0012 0049 4e54 5f34 555b  stance...INT_4U[
-00002680: 6e53 7461 7454 7970 655d 0043 0041 7272  nStatType].C.Arr
-00002690: 6179 206f 6620 6e75 6d62 6572 206f 6620  ay of number of 
-000026a0: 696e 7374 616e 6365 2066 6f72 2065 6163  instance for eac
-000026b0: 6820 4672 5374 6174 4461 7461 2873 697a  h FrStatData(siz
-000026c0: 6520 6f66 206e 5374 6174 5479 7065 2900  e of nStatType).
-000026d0: 66b8 774f 4b00 0000 0000 0000 0102 1700  f.wOK...........
-000026e0: 0000 0b00 6e54 6f74 616c 5374 6174 0007  ....nTotalStat..
-000026f0: 0049 4e54 5f34 5500 2100 5375 6d6d 6174  .INT_4U.!.Summat
-00002700: 696f 6e20 6f66 206e 5374 6174 496e 7374  ion of nStatInst
-00002710: 616e 6365 2061 7272 6179 0089 b4e7 f874  ance array.....t
-00002720: 0000 0000 0000 0001 0218 0000 0007 0074  ...............t
-00002730: 5374 6172 7400 1300 494e 545f 3455 5b6e  Start...INT_4U[n
-00002740: 546f 7461 6c53 7461 745d 0042 0041 7272  TotalStat].B.Arr
-00002750: 6179 206f 6620 4750 5320 696e 7465 6765  ay of GPS intege
-00002760: 7220 7374 6172 7420 7469 6d65 732c 2069  r start times, i
-00002770: 6e20 7365 636f 6e64 7320 2873 697a 6520  n seconds (size 
-00002780: 6f66 206e 546f 7461 6c53 7461 7429 001a  of nTotalStat)..
-00002790: 531d 0970 0000 0000 0000 0001 0219 0000  S..p............
-000027a0: 0005 0074 456e 6400 1300 494e 545f 3455  ...tEnd...INT_4U
-000027b0: 5b6e 546f 7461 6c53 7461 745d 0040 0041  [nTotalStat].@.A
-000027c0: 7272 6179 206f 6620 4750 5320 696e 7465  rray of GPS inte
-000027d0: 6765 7220 656e 6420 7469 6d65 732c 2069  ger end times, i
-000027e0: 6e20 7365 636f 6e64 7320 2873 697a 6520  n seconds (size 
-000027f0: 6f66 206e 546f 7461 6c53 7461 7429 0045  of nTotalStat).E
-00002800: 668b 4d5e 0000 0000 0000 0001 021a 0000  f.M^............
-00002810: 0008 0076 6572 7369 6f6e 0013 0049 4e54  ...version...INT
-00002820: 5f34 555b 6e54 6f74 616c 5374 6174 5d00  _4U[nTotalStat].
-00002830: 2b00 4172 7261 7920 6f66 2076 6572 7369  +.Array of versi
-00002840: 6f6e 2074 696d 6520 2873 697a 6520 6f66  on time (size of
-00002850: 206e 546f 7461 6c53 7461 7429 0093 e259   nTotalStat)...Y
-00002860: 1d82 0000 0000 0000 0001 021b 0000 000d  ................
-00002870: 0070 6f73 6974 696f 6e53 7461 7400 1300  .positionStat...
-00002880: 494e 545f 3855 5b6e 546f 7461 6c53 7461  INT_8U[nTotalSta
-00002890: 745d 004a 0041 7272 6179 206f 6620 4672  t].J.Array of Fr
-000028a0: 5374 6174 4461 7461 2070 6f73 6974 696f  StatData positio
-000028b0: 6e73 2066 726f 6d20 6265 6769 6e6e 696e  ns from beginnin
-000028c0: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
-000028d0: 6f66 206e 546f 7461 6c53 7461 7429 002e  of nTotalStat)..
-000028e0: 51de 564e 0000 0000 0000 0001 021c 0000  Q.VN............
-000028f0: 0005 006e 4144 4300 0700 494e 545f 3455  ...nADC...INT_4U
-00002900: 002a 004e 756d 6265 7220 6f66 2075 6e69  .*.Number of uni
-00002910: 7175 6520 4672 4164 6344 6174 6120 6e61  que FrAdcData na
-00002920: 6d65 7320 696e 2066 696c 652e 0007 54ee  mes in file...T.
-00002930: e143 0000 0000 0000 0001 021d 0000 0005  .C..............
-00002940: 006e 616d 6500 0d00 5354 5249 4e47 5b6e  .name...STRING[n
-00002950: 4144 435d 0019 0041 7272 6179 206f 6620  ADC]...Array of 
-00002960: 4672 4164 6344 6174 6120 6e61 6d65 7300  FrAdcData names.
-00002970: 89b1 c3ad 4800 0000 0000 0000 0102 1e00  ....H...........
-00002980: 0000 0a00 6368 616e 6e65 6c49 4400 0d00  ....channelID...
-00002990: 494e 545f 3455 5b6e 4144 435d 0019 0041  INT_4U[nADC]...A
-000029a0: 7272 6179 206f 6620 4144 4320 6368 616e  rray of ADC chan
-000029b0: 6e65 6c20 4944 7300 251b 8f78 4400 0000  nel IDs.%..xD...
-000029c0: 0000 0000 0102 1f00 0000 0800 6772 6f75  ............grou
-000029d0: 7049 4400 0d00 494e 545f 3455 5b6e 4144  pID...INT_4U[nAD
-000029e0: 435d 0017 0041 7272 6179 206f 6620 4144  C]...Array of AD
-000029f0: 4320 6772 6f75 7020 4944 7300 ec33 7c9e  C group IDs..3|.
-00002a00: 9e00 0000 0000 0000 0102 2000 0000 0c00  .......... .....
-00002a10: 706f 7369 7469 6f6e 4144 4300 1500 494e  positionADC...IN
-00002a20: 545f 3855 5b6e 4144 435d 5b6e 4672 616d  T_8U[nADC][nFram
-00002a30: 655d 0065 0041 7272 6179 206f 6620 6c69  e].e.Array of li
-00002a40: 7374 7320 6f66 2046 7241 6463 4461 7461  sts of FrAdcData
-00002a50: 206f 6666 7365 7420 706f 7369 7469 6f6e   offset position
-00002a60: 732c 2069 6e20 6279 7465 732c 2066 726f  s, in bytes, fro
-00002a70: 6d20 6265 6769 6e6e 696e 6720 6f66 2066  m beginning of f
-00002a80: 696c 6520 2873 697a 6520 6f66 206e 4672  ile (size of nFr
-00002a90: 616d 652a 6e41 4443 2900 6d54 ccf2 5000  ame*nADC).mT..P.
-00002aa0: 0000 0000 0000 0102 2100 0000 0600 6e50  ........!.....nP
-00002ab0: 726f 6300 0700 494e 545f 3455 002b 004e  roc...INT_4U.+.N
-00002ac0: 756d 6265 7220 6f66 2075 6e69 7175 6520  umber of unique 
-00002ad0: 4672 5072 6f63 4461 7461 206e 616d 6573  FrProcData names
-00002ae0: 2069 6e20 6669 6c65 2e00 feef 7499 4900   in file....t.I.
-00002af0: 0000 0000 0000 0102 2200 0000 0900 6e61  ........".....na
-00002b00: 6d65 5072 6f63 000e 0053 5452 494e 475b  meProc...STRING[
-00002b10: 6e50 726f 635d 001a 0041 7272 6179 206f  nProc]...Array o
-00002b20: 6620 4672 5072 6f63 4461 7461 206e 616d  f FrProcData nam
-00002b30: 6573 0092 f0ec 64a2 0000 0000 0000 0001  es....d.........
-00002b40: 0223 0000 000d 0070 6f73 6974 696f 6e50  .#.....positionP
-00002b50: 726f 6300 1600 494e 545f 3855 5b6e 5072  roc...INT_8U[nPr
-00002b60: 6f63 5d5b 6e46 7261 6d65 5d00 6700 4172  oc][nFrame].g.Ar
-00002b70: 7261 7920 6f66 206c 6973 7473 206f 6620  ray of lists of 
-00002b80: 4672 5072 6f63 4461 7461 206f 6666 7365  FrProcData offse
-00002b90: 7420 706f 7369 7469 6f6e 732c 2069 6e20  t positions, in 
-00002ba0: 6279 7465 732c 2066 726f 6d20 6265 6769  bytes, from begi
-00002bb0: 6e6e 696e 6720 6f66 2066 696c 6520 2873  nning of file (s
-00002bc0: 697a 6520 6f66 206e 4672 616d 652a 6e50  ize of nFrame*nP
-00002bd0: 726f 6329 00f2 b9e4 a64e 0000 0000 0000  roc).....N......
-00002be0: 0001 0224 0000 0005 006e 5369 6d00 0700  ...$.....nSim...
-00002bf0: 494e 545f 3455 002a 004e 756d 6265 7220  INT_4U.*.Number 
-00002c00: 6f66 2075 6e69 7175 6520 4672 5369 6d44  of unique FrSimD
-00002c10: 6174 6120 6e61 6d65 7320 696e 2066 696c  ata names in fil
-00002c20: 652e 0008 01bc 3746 0000 0000 0000 0001  e.....7F........
-00002c30: 0225 0000 0008 006e 616d 6553 696d 000d  .%.....nameSim..
-00002c40: 0053 5452 494e 475b 6e53 696d 5d00 1900  .STRING[nSim]...
-00002c50: 4172 7261 7920 6f66 2046 7253 696d 4461  Array of FrSimDa
-00002c60: 7461 206e 616d 6573 00c4 a72b f69e 0000  ta names...+....
-00002c70: 0000 0000 0001 0226 0000 000c 0070 6f73  .......&.....pos
-00002c80: 6974 696f 6e53 696d 0015 0049 4e54 5f38  itionSim...INT_8
-00002c90: 555b 6e53 696d 5d5b 6e46 7261 6d65 5d00  U[nSim][nFrame].
-00002ca0: 6500 4172 7261 7920 6f66 206c 6973 7473  e.Array of lists
-00002cb0: 206f 6620 4672 5369 6d44 6174 6120 6f66   of FrSimData of
-00002cc0: 6673 6574 2070 6f73 6974 696f 6e73 2c20  fset positions, 
-00002cd0: 696e 2062 7974 6573 2c20 6672 6f6d 2062  in bytes, from b
-00002ce0: 6567 696e 6e69 6e67 206f 6620 6669 6c65  eginning of file
-00002cf0: 2028 7369 7a65 206f 6620 6e46 7261 6d65   (size of nFrame
-00002d00: 2a6e 5369 6d29 00d3 40ba c14e 0000 0000  *nSim)..@..N....
-00002d10: 0000 0001 0227 0000 0005 006e 5365 7200  .....'.....nSer.
-00002d20: 0700 494e 545f 3455 002a 004e 756d 6265  ..INT_4U.*.Numbe
-00002d30: 7220 6f66 2075 6e69 7175 6520 4672 5365  r of unique FrSe
-00002d40: 7244 6174 6120 6e61 6d65 7320 696e 2066  rData names in f
-00002d50: 696c 652e 000f 814d 9046 0000 0000 0000  ile....M.F......
-00002d60: 0001 0228 0000 0008 006e 616d 6553 6572  ...(.....nameSer
-00002d70: 000d 0053 5452 494e 475b 6e53 6572 5d00  ...STRING[nSer].
-00002d80: 1900 4172 7261 7920 6f66 2046 7253 6572  ..Array of FrSer
-00002d90: 4461 7461 206e 616d 6573 00bd 2d79 109e  Data names..-y..
-00002da0: 0000 0000 0000 0001 0229 0000 000c 0070  .........).....p
-00002db0: 6f73 6974 696f 6e53 6572 0015 0049 4e54  ositionSer...INT
-00002dc0: 5f38 555b 6e53 6572 5d5b 6e46 7261 6d65  _8U[nSer][nFrame
-00002dd0: 5d00 6500 4172 7261 7920 6f66 206c 6973  ].e.Array of lis
-00002de0: 7473 206f 6620 4672 5365 7244 6174 6120  ts of FrSerData 
-00002df0: 6f66 6673 6574 2070 6f73 6974 696f 6e73  offset positions
-00002e00: 2c20 696e 2062 7974 6573 2c20 6672 6f6d  , in bytes, from
-00002e10: 2062 6567 696e 6e69 6e67 206f 6620 6669   beginning of fi
-00002e20: 6c65 2028 7369 7a65 206f 6620 6e46 7261  le (size of nFra
-00002e30: 6d65 2a6e 5365 7229 001c 5003 fb52 0000  me*nSer)..P..R..
-00002e40: 0000 0000 0001 022a 0000 0009 006e 5375  .......*.....nSu
-00002e50: 6d6d 6172 7900 0700 494e 545f 3455 002a  mmary...INT_4U.*
-00002e60: 004e 756d 6265 7220 6f66 2075 6e69 7175  .Number of uniqu
-00002e70: 6520 4672 5375 6d6d 6172 7920 6e61 6d65  e FrSummary name
-00002e80: 7320 696e 2066 696c 652e 0034 77a5 e94b  s in file..4w..K
-00002e90: 0000 0000 0000 0001 022b 0000 0009 006e  .........+.....n
-00002ea0: 616d 6553 5375 6d00 1100 5354 5249 4e47  ameSSum...STRING
-00002eb0: 5b6e 5375 6d6d 6172 795d 0019 0041 7272  [nSummary]...Arr
-00002ec0: 6179 206f 6620 4672 5375 6d6d 6172 7920  ay of FrSummary 
-00002ed0: 6e61 6d65 7300 0684 574e a200 0000 0000  names...WN......
-00002ee0: 0000 0102 2c00 0000 0c00 706f 7369 7469  ....,.....positi
-00002ef0: 6f6e 5365 7200 1900 494e 545f 3855 5b6e  onSer...INT_8U[n
-00002f00: 5375 6d6d 6172 795d 5b6e 4672 616d 655d  Summary][nFrame]
-00002f10: 0065 0041 7272 6179 206f 6620 6c69 7374  .e.Array of list
-00002f20: 7320 6f66 2046 7253 756d 6d61 7279 206f  s of FrSummary o
-00002f30: 6666 7365 7420 706f 7369 7469 6f6e 732c  ffset positions,
-00002f40: 2069 6e20 6279 7465 732c 2066 726f 6d20   in bytes, from 
-00002f50: 6265 6769 6e6e 696e 6720 6f66 2066 696c  beginning of fil
-00002f60: 6520 2873 697a 6520 6f66 206e 4672 616d  e (size of nFram
-00002f70: 652a 6e53 6572 2900 c376 da95 4800 0000  e*nSer)..v..H...
-00002f80: 0000 0000 0102 2d00 0000 0b00 6e45 7665  ......-.....nEve
-00002f90: 6e74 5479 7065 0007 0049 4e54 5f34 5500  ntType...INT_4U.
-00002fa0: 1e00 4e75 6d62 6572 206f 6620 4672 4576  ..Number of FrEv
-00002fb0: 656e 7420 696e 2074 6865 2066 696c 6500  ent in the file.
-00002fc0: cb0b 34f7 4c00 0000 0000 0000 0102 2e00  ..4.L...........
-00002fd0: 0000 0a00 6e61 6d65 4576 656e 7400 1300  ....nameEvent...
-00002fe0: 5354 5249 4e47 5b6e 4576 656e 7454 7970  STRING[nEventTyp
-00002ff0: 655d 0017 0041 7272 6179 206f 6620 4672  e]...Array of Fr
-00003000: 4576 656e 7420 6e61 6d65 7300 8aec 7442  Event names...tB
-00003010: 7200 0000 0000 0000 0102 2f00 0000 0700  r........./.....
-00003020: 6e45 7665 6e74 0013 0049 4e54 5f34 555b  nEvent...INT_4U[
-00003030: 6e45 7665 6e74 5479 7065 5d00 4000 4e75  nEventType].@.Nu
-00003040: 6d62 6572 206f 6620 4672 4576 656e 7420  mber of FrEvent 
-00003050: 666f 7220 6561 6368 2074 7970 6520 6f66  for each type of
-00003060: 2046 7245 7665 6e74 2028 7369 7a65 206f   FrEvent (size o
-00003070: 6620 6e45 7665 6e74 5479 7065 2900 aebb  f nEventType)...
-00003080: 6fd3 4300 0000 0000 0000 0102 3000 0000  o.C.........0...
-00003090: 0c00 6e54 6f74 616c 4576 656e 7400 0700  ..nTotalEvent...
-000030a0: 494e 545f 3455 0018 0054 6f74 616c 206e  INT_4U...Total n
-000030b0: 756d 6265 7220 6f66 2046 7245 7665 6e74  umber of FrEvent
-000030c0: 0074 8af4 4a54 0000 0000 0000 0001 0231  .t..JT.........1
-000030d0: 0000 000c 0047 5469 6d65 5345 7665 6e74  .....GTimeSEvent
-000030e0: 0014 0049 4e54 5f34 555b 6e54 6f74 616c  ...INT_4U[nTotal
-000030f0: 4576 656e 745d 001c 0047 5053 2074 696d  Event]...GPS tim
-00003100: 6520 696e 2069 6e74 6567 6572 2073 6563  e in integer sec
-00003110: 6f6e 6473 0015 3513 2961 0000 0000 0000  onds..5.)a......
-00003120: 0001 0232 0000 000c 0047 5469 6d65 4e45  ...2.....GTimeNE
-00003130: 7665 6e74 0014 0049 4e54 5f34 555b 6e54  vent...INT_4U[nT
-00003140: 6f74 616c 4576 656e 745d 0029 0052 6573  otalEvent].).Res
-00003150: 6964 7561 6c20 4750 5320 7469 6d65 2069  idual GPS time i
-00003160: 6e20 696e 7465 6765 7220 6e61 6e6f 7365  n integer nanose
-00003170: 636f 6e64 7300 157d 335d 4b00 0000 0000  conds..}3]K.....
-00003180: 0000 0102 3300 0000 0f00 616d 706c 6974  ....3.....amplit
-00003190: 7564 6545 7665 6e74 0014 0052 4541 4c5f  udeEvent...REAL_
-000031a0: 345b 6e54 6f74 616c 4576 656e 745d 0010  4[nTotalEvent]..
-000031b0: 0045 7665 6e74 2061 6d70 6c69 7475 6465  .Event amplitude
-000031c0: 00c2 ba16 4177 0000 0000 0000 0001 0234  ....Aw.........4
-000031d0: 0000 000e 0070 6f73 6974 696f 6e45 7665  .....positionEve
-000031e0: 6e74 0014 0049 4e54 5f38 555b 6e54 6f74  nt...INT_8U[nTot
-000031f0: 616c 4576 656e 745d 003d 0041 7272 6179  alEvent].=.Array
-00003200: 206f 6620 4672 4576 656e 7420 706f 7369   of FrEvent posi
-00003210: 7469 6f6e 732c 2069 6e20 6279 7465 732c  tions, in bytes,
-00003220: 2066 726f 6d20 6265 6769 6e6e 696e 6720   from beginning 
-00003230: 6f66 2066 696c 6500 46be 4b47 4e00 0000  of file.F.KGN...
-00003240: 0000 0000 0102 3500 0000 0e00 6e53 696d  ......5.....nSim
-00003250: 4576 656e 7454 7970 6500 0700 494e 545f  EventType...INT_
-00003260: 3455 0021 004e 756d 6265 7220 6f66 2046  4U.!.Number of F
-00003270: 7253 696d 4576 656e 7420 696e 2074 6865  rSimEvent in the
-00003280: 2066 696c 6500 d601 de2b 5500 0000 0000   file....+U.....
-00003290: 0000 0102 3600 0000 0d00 6e61 6d65 5369  ....6.....nameSi
-000032a0: 6d45 7665 6e74 0016 0053 5452 494e 475b  mEvent...STRING[
-000032b0: 6e53 696d 4576 656e 7454 7970 655d 001a  nSimEventType]..
-000032c0: 0041 7272 6179 206f 6620 4672 5369 6d45  .Array of FrSimE
-000032d0: 7665 6e74 206e 616d 6573 00c3 e4da a081  vent names......
-000032e0: 0000 0000 0000 0001 0237 0000 000a 006e  .........7.....n
-000032f0: 5369 6d45 7665 6e74 0016 0049 4e54 5f34  SimEvent...INT_4
-00003300: 555b 6e53 696d 4576 656e 7454 7970 655d  U[nSimEventType]
-00003310: 0049 004e 756d 6265 7220 6f66 2046 7253  .I.Number of FrS
-00003320: 696d 4576 656e 7420 666f 7220 6561 6368  imEvent for each
-00003330: 2074 7970 6520 6f66 2046 7253 696d 4576   type of FrSimEv
-00003340: 656e 7420 2873 697a 6520 6f66 206e 5369  ent (size of nSi
-00003350: 6d45 7665 6e74 5479 7065 2900 4e11 c946  mEventType).N..F
-00003360: 4700 0000 0000 0000 0102 3800 0000 0d00  G.........8.....
-00003370: 6e54 6f74 616c 5345 7665 6e74 0007 0049  nTotalSEvent...I
-00003380: 4e54 5f34 5500 1b00 546f 7461 6c20 6e75  NT_4U...Total nu
-00003390: 6d62 6572 206f 6620 4672 5369 6d45 7665  mber of FrSimEve
-000033a0: 6e74 00de 86a5 7e53 0000 0000 0000 0001  nt....~S........
-000033b0: 0239 0000 000a 0047 5469 6d65 5353 696d  .9.....GTimeSSim
-000033c0: 0015 0049 4e54 5f34 555b 6e54 6f74 616c  ...INT_4U[nTotal
-000033d0: 5345 7665 6e74 5d00 1c00 4750 5320 7469  SEvent]...GPS ti
-000033e0: 6d65 2069 6e20 696e 7465 6765 7220 7365  me in integer se
-000033f0: 636f 6e64 7300 8b64 9181 6000 0000 0000  conds..d..`.....
-00003400: 0000 0102 3a00 0000 0a00 4754 696d 654e  ....:.....GTimeN
-00003410: 5369 6d00 1500 494e 545f 3455 5b6e 546f  Sim...INT_4U[nTo
-00003420: 7461 6c53 4576 656e 745d 0029 0052 6573  talSEvent].).Res
-00003430: 6964 7561 6c20 4750 5320 7469 6d65 2069  idual GPS time i
-00003440: 6e20 696e 7465 6765 7220 6e61 6e6f 7365  n integer nanose
-00003450: 636f 6e64 7300 6127 db26 5200 0000 0000  conds.a'.&R.....
-00003460: 0000 0102 3b00 0000 1200 616d 706c 6974  ....;.....amplit
-00003470: 7564 6553 696d 4576 656e 7400 1500 5245  udeSimEvent...RE
-00003480: 414c 5f34 5b6e 546f 7461 6c53 4576 656e  AL_4[nTotalSEven
-00003490: 745d 0013 0053 696d 4576 656e 7420 616d  t]...SimEvent am
-000034a0: 706c 6974 7564 6500 2410 90c2 7e00 0000  plitude.$...~...
-000034b0: 0000 0000 0102 3c00 0000 1100 706f 7369  ......<.....posi
-000034c0: 7469 6f6e 5369 6d45 7665 6e74 0015 0049  tionSimEvent...I
-000034d0: 4e54 5f38 555b 6e54 6f74 616c 5345 7665  NT_8U[nTotalSEve
-000034e0: 6e74 5d00 4000 4172 7261 7920 6f66 2046  nt].@.Array of F
-000034f0: 7253 696d 4576 656e 7420 706f 7369 7469  rSimEvent positi
-00003500: 6f6e 732c 2069 6e20 6279 7465 732c 2066  ons, in bytes, f
-00003510: 726f 6d20 6265 6769 6e6e 696e 6720 6f66  rom beginning of
-00003520: 2066 696c 6500 9f96 37f5 3600 0000 0000   file...7.6.....
-00003530: 0000 0102 3d00 0000 0700 6368 6b53 756d  ....=.....chkSum
-00003540: 0007 0049 4e54 5f34 5500 1000 5374 7275  ...INT_4U...Stru
-00003550: 6374 2063 6865 636b 7375 6d00 8e79 d77a  ct checksum..y.z
-00003560: 5001 0000 0000 0000 0113 0000 0000 2500  P.............%.
-00003570: 0100 0000 0000 0000 b881 8348 0000 0000  ...........H....
-00003580: 0000 0000 0000 1040 0000 0000 0000 0000  .......@........
-00003590: 6e09 0000 0000 0000 0000 0000 0000 0000  n...............
-000035a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000035b0: 0000 0000 0000 0000 0600 0000 0300 0500  ................
-000035c0: 0b00 1400 0700 1300 0700 4672 616d 6548  ..........FrameH
-000035d0: 000b 0046 7244 6574 6563 746f 7200 0b00  ...FrDetector...
-000035e0: 4672 5072 6f63 4461 7461 0007 0046 7256  FrProcData...FrV
-000035f0: 6563 7400 0d00 4672 456e 644f 6646 7261  ect...FrEndOfFra
-00003600: 6d65 0006 0046 7254 4f43 0001 0000 0007  me...FrTOC......
-00003610: 004c 4c4f 5f34 6b00 020d 0000 0000 0000  .LLO_4k.........
-00003620: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00003630: 1100 4c31 3a44 4d54 2d44 515f 5645 4354  ..L1:DMT-DQ_VECT
-00003640: 4f52 001a 004c 313a 4744 532d 4341 4c49  OR...L1:GDS-CALI
-00003650: 425f 5354 4154 455f 5645 4354 4f52 0017  B_STATE_VECTOR..
-00003660: 004c 313a 4944 512d 4641 505f 4f56 4c5f  .L1:IDQ-FAP_OVL_
-00003670: 3332 5f32 3034 3800 0214 0000 0000 0000  32_2048.........
-00003680: 1619 0000 0000 0000 291a 0000 0000 0000  ........).......
-00003690: ffff ffff ffff ffff ffff ffff 0000 0000  ................
-000036a0: 0000 0000 0000 0000 0000 0000 5a2d 2ead  ............Z-..
-000036b0: 3f00 0000 0000 0000 0101 0100 0000 0c00  ?...............
-000036c0: 4672 456e 644f 6646 696c 6500 0600 1b00  FrEndOfFile.....
-000036d0: 456e 6420 6f66 2046 696c 6520 4461 7461  End of File Data
-000036e0: 2053 7472 7563 7475 7265 00a8 da1b ec45   Structure.....E
-000036f0: 0000 0000 0000 0001 023e 0000 0008 006e  .........>.....n
-00003700: 4672 616d 6573 0007 0049 4e54 5f34 5500  Frames...INT_4U.
-00003710: 1e00 4e75 6d62 6572 206f 6620 6672 616d  ..Number of fram
-00003720: 6573 2069 6e20 7468 6973 2066 696c 6500  es in this file.
-00003730: c01d f442 5f00 0000 0000 0000 0102 3f00  ...B_.........?.
-00003740: 0000 0700 6e42 7974 6573 0007 0049 4e54  ....nBytes...INT
-00003750: 5f38 5500 3900 546f 7461 6c20 6e75 6d62  _8U.9.Total numb
-00003760: 6572 206f 6620 6279 7465 7320 696e 2074  er of bytes in t
-00003770: 6869 7320 6669 6c65 2028 2030 2069 6620  his file ( 0 if 
-00003780: 4e4f 5420 636f 6d70 7574 6564 2029 0082  NOT computed )..
-00003790: 8d13 02a1 0000 0000 0000 0001 0240 0000  .............@..
-000037a0: 0008 0073 6565 6b54 4f43 0007 0049 4e54  ...seekTOC...INT
-000037b0: 5f38 5500 7a00 4279 6573 2074 6f20 6261  _8U.z.Byes to ba
-000037c0: 636b 2075 7020 746f 2074 6865 2062 6567  ck up to the beg
-000037d0: 696e 6e69 6e67 206f 6620 7468 6520 7461  inning of the ta
-000037e0: 626c 6520 6f66 2063 6f6e 7465 6e74 7320  ble of contents 
-000037f0: 7374 7275 6374 7572 652e 2049 6620 7365  structure. If se
-00003800: 656b 544f 4320 3d3d 2030 2c20 7468 656e  ekTOC == 0, then
-00003810: 2074 6865 7265 2069 7320 6e6f 2054 4f43   there is no TOC
-00003820: 2066 6f72 2074 6869 7320 6669 6c65 2e00   for this file..
-00003830: c8d4 6535 4100 0000 0000 0000 0102 4100  ..e5A.........A.
-00003840: 0000 0f00 6368 6b53 756d 4672 4865 6164  ....chkSumFrHead
-00003850: 6572 0007 0049 4e54 5f34 5500 1300 4672  er...INT_4U...Fr
-00003860: 4865 6164 6572 2063 6865 636b 7375 6d2e  Header checksum.
-00003870: 0009 9135 933a 0000 0000 0000 0001 0242  ...5.:.........B
-00003880: 0000 0007 0063 686b 5375 6d00 0700 494e  .....chkSum...IN
-00003890: 545f 3455 0014 0053 7472 7563 7475 7265  T_4U...Structure
-000038a0: 2063 6865 636b 7375 6d2e 00d0 97d1 a839   checksum......9
-000038b0: 0000 0000 0000 0001 0243 0000 000b 0063  .........C.....c
-000038c0: 686b 5375 6d46 696c 6500 0700 494e 545f  hkSumFile...INT_
-000038d0: 3455 000f 0046 696c 6520 6368 6563 6b73  4U...File checks
-000038e0: 756d 2e00 16df ff60 2e00 0000 0000 0000  um.....`........
-000038f0: 0106 0000 0000 0100 0000 1639 0000 0000  ...........9....
-00003900: 0000 b603 0000 0000 0000 bac1 b663 8668  .............c.h
-00003910: 785b bd0c 3ba0                           x[..;.
+00001400: 8ab6 9a00 0000 0000 0000 010b 0000 0000  ................
+00001410: 1a00 4831 3a47 4453 2d43 414c 4942 5f53  ..H1:GDS-CALIB_S
+00001420: 5441 5445 5f56 4543 544f 5200 1a00 4831  TATE_VECTOR...H1
+00001430: 3a47 4453 2d43 414c 4942 5f53 5441 5445  :GDS-CALIB_STATE
+00001440: 5f56 4543 544f 5200 0100 0000 0000 0000  _VECTOR.........
+00001450: 0000 0000 0000 0000 0000 1040 0000 0000  ...........@....
+00001460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001470: 0000 0000 0000 0000 0000 1400 0000 0000  ................
+00001480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001490: 0000 0b00 0100 0000 d2e3 49c6 3500 0000  ..........I.5...
+000014a0: 0000 0000 0101 0300 0000 0700 4672 5665  ............FrVe
+000014b0: 6374 0014 0016 0056 6563 746f 7220 4461  ct.....Vector Da
+000014c0: 7461 2053 7472 7563 7475 7265 00af a279  ta Structure...y
+000014d0: 264e 0000 0000 0000 0001 0239 0000 0005  &N.........9....
+000014e0: 006e 616d 6500 0700 5354 5249 4e47 002a  .name...STRING.*
+000014f0: 0043 6861 6e6e 656c 206e 616d 6520 2d2d  .Channel name --
+00001500: 206e 6f74 2072 6571 7569 7265 6420 746f   not required to
+00001510: 2062 6520 756e 6971 7565 0023 3580 8545   be unique.#5..E
+00001520: 0000 0000 0000 0001 023a 0000 0009 0063  .........:.....c
+00001530: 6f6d 7072 6573 7300 0700 494e 545f 3255  ompress...INT_2U
+00001540: 001d 0043 6f6d 7072 6573 7369 6f6e 2061  ...Compression a
+00001550: 6c67 6f72 6974 686d 206e 756d 6265 7200  lgorithm number.
+00001560: b1fa 026c 3100 0000 0000 0000 0102 3b00  ...l1.........;.
+00001570: 0000 0500 7479 7065 0007 0049 4e54 5f32  ....type...INT_2
+00001580: 5500 0d00 5665 6374 6f72 2063 6c61 7373  U...Vector class
+00001590: 0013 fdab ae4e 0000 0000 0000 0001 023c  .....N.........<
+000015a0: 0000 0006 006e 4461 7461 0007 0049 4e54  .....nData...INT
+000015b0: 5f38 5500 2900 4e75 6d62 6572 206f 6620  _8U.).Number of 
+000015c0: 7361 6d70 6c65 2065 6c65 6d65 6e74 7320  sample elements 
+000015d0: 696e 2064 6174 6120 7365 7269 6573 0092  in data series..
+000015e0: 220f 634f 0000 0000 0000 0001 023d 0000  ".cO.........=..
+000015f0: 0007 006e 4279 7465 7300 0700 494e 545f  ...nBytes...INT_
+00001600: 3855 0029 004e 756d 6265 7220 6f66 2062  8U.).Number of b
+00001610: 7974 6573 2069 6e20 7468 6520 636f 6d70  ytes in the comp
+00001620: 7265 7373 6564 2076 6563 746f 7200 fe47  ressed vector..G
+00001630: a552 4c00 0000 0000 0000 0102 3e00 0000  .RL.........>...
+00001640: 0500 6461 7461 000d 0043 4841 525b 6e42  ..data...CHAR[nB
+00001650: 7974 6573 5d00 2200 6e44 6174 6120 656c  ytes].".nData el
+00001660: 656d 656e 7473 206f 6620 7370 6563 6966  ements of specif
+00001670: 6965 6420 636c 6173 7300 d461 1f2e 4200  ied class..a..B.
+00001680: 0000 0000 0000 0102 3f00 0000 0500 6e44  ........?.....nD
+00001690: 696d 0007 0049 4e54 5f34 5500 1e00 4469  im...INT_4U...Di
+000016a0: 6d65 6e73 696f 6e61 6c69 7479 206f 6620  mensionality of 
+000016b0: 6461 7461 2076 6563 746f 7200 cd27 6340  data vector..'c@
+000016c0: 3a00 0000 0000 0000 0102 4000 0000 0300  :.........@.....
+000016d0: 6e78 000d 0049 4e54 5f38 555b 6e44 696d  nx...INT_8U[nDim
+000016e0: 5d00 1200 6469 6d65 6e73 696f 6e20 6c65  ]...dimension le
+000016f0: 6e67 7468 7300 403d c725 4d00 0000 0000  ngths.@=.%M.....
+00001700: 0000 0102 4100 0000 0300 6478 000d 0052  ....A.....dx...R
+00001710: 4541 4c5f 385b 6e44 696d 5d00 2500 7361  EAL_8[nDim].%.sa
+00001720: 6d70 6c65 2073 7061 6369 6e67 2061 6c6f  mple spacing alo
+00001730: 6e67 2065 6163 6820 636f 6f72 6469 6e61  ng each coordina
+00001740: 7465 00ac b934 e445 0000 0000 0000 0001  te...4.E........
+00001750: 0242 0000 0007 0073 7461 7274 5800 0d00  .B.....startX...
+00001760: 5245 414c 5f38 5b6e 4469 6d5d 0019 004f  REAL_8[nDim]...O
+00001770: 7269 6769 6e20 666f 7220 6561 6368 2064  rigin for each d
+00001780: 6174 6120 7365 7400 d235 5772 4200 0000  ata set..5WrB...
+00001790: 0000 0000 0102 4300 0000 0600 756e 6974  ......C.....unit
+000017a0: 5800 0d00 5354 5249 4e47 5b6e 4469 6d5d  X...STRING[nDim]
+000017b0: 0017 0073 6361 6c65 2066 6163 746f 7273  ...scale factors
+000017c0: 2069 6e20 4153 4349 4900 5d23 1276 6200   in ASCII.]#.vb.
+000017d0: 0000 0000 0000 0102 4400 0000 0600 756e  ........D.....un
+000017e0: 6974 5900 0700 5354 5249 4e47 003d 0053  itY...STRING.=.S
+000017f0: 7472 696e 6720 6465 7363 7269 6269 6e67  tring describing
+00001800: 2068 6f77 2074 6f20 696e 7465 7270 7265   how to interpre
+00001810: 7420 7468 6520 7661 6c75 6520 6f66 2065  t the value of e
+00001820: 6163 6820 656c 656d 656e 7400 bc2b a817  ach element..+..
+00001830: 5200 0000 0000 0000 0102 4500 0000 0500  R.........E.....
+00001840: 6e65 7874 0015 0050 5452 5f53 5452 5543  next...PTR_STRUC
+00001850: 5428 4672 5665 6374 202a 2900 2000 4964  T(FrVect *). .Id
+00001860: 656e 7469 6669 6572 2066 6f72 2061 6464  entifier for add
+00001870: 6974 696f 6e61 6c20 6461 7461 2e00 bb79  itional data...y
+00001880: c453 3600 0000 0000 0000 0102 4600 0000  .S6.........F...
+00001890: 0700 6368 6b53 756d 0007 0049 4e54 5f34  ..chkSum...INT_4
+000018a0: 5500 1000 5374 7275 6374 2063 6865 636b  U...Struct check
+000018b0: 7375 6d00 885a 50b6 7f00 0000 0000 0000  sum..ZP.........
+000018c0: 0114 0000 0000 1a00 4831 3a47 4453 2d43  ........H1:GDS-C
+000018d0: 414c 4942 5f53 5441 5445 5f56 4543 544f  ALIB_STATE_VECTO
+000018e0: 5200 0101 0500 4000 0000 0000 0000 1400  R.....@.........
+000018f0: 0000 0000 0000 789c fb5f ff4f 9f01 08fe  ......x.._.O....
+00001900: 8fd2 2392 0600 b514 aac1 0100 0000 4000  ..#...........@.
+00001910: 0000 0000 0000 0000 0000 0000 b03f 0000  .............?..
+00001920: 0000 0000 0000 0200 7300 0100 0000 0000  ........s.......
+00001930: 0000 00e8 2243 6488 0000 0000 0000 0001  ...."Cd.........
+00001940: 0b01 0000 0011 0048 313a 444d 542d 4451  .......H1:DMT-DQ
+00001950: 5f56 4543 544f 5200 1100 4831 3a44 4d54  _VECTOR...H1:DMT
+00001960: 2d44 515f 5645 4354 4f52 0001 0000 0000  -DQ_VECTOR......
+00001970: 0000 0000 0000 0000 0000 0000 0010 4000  ..............@.
+00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001990: 0000 0000 0000 0000 0000 0000 0014 0001  ................
+000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019b0: 0000 0000 000b 0002 0000 0013 42a3 7b72  ............B.{r
+000019c0: 0000 0000 0000 0001 1401 0000 0011 0048  ...............H
+000019d0: 313a 444d 542d 4451 5f56 4543 544f 5200  1:DMT-DQ_VECTOR.
+000019e0: 0101 0500 4000 0000 0000 0000 1000 0000  ....@...........
+000019f0: 0000 0000 789c 6367 8000 f651 7a44 d200  ....x.cg...QzD..
+00001a00: c90f 01c1 0100 0000 4000 0000 0000 0000  ........@.......
+00001a10: 0000 0000 0000 b03f 0000 0000 0000 0000  .......?........
+00001a20: 0200 7300 0100 0000 0000 0000 00ba 2642  ..s...........&B
+00001a30: ad94 0000 0000 0000 0001 0b02 0000 0017  ................
+00001a40: 0048 313a 4944 512d 4641 505f 4f56 4c5f  .H1:IDQ-FAP_OVL_
+00001a50: 3332 5f32 3034 3800 1700 4831 3a49 4451  32_2048...H1:IDQ
+00001a60: 2d46 4150 5f4f 564c 5f33 325f 3230 3438  -FAP_OVL_32_2048
+00001a70: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+00001a80: 0000 0010 4000 0000 0000 0000 0000 0000  ....@...........
+00001a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001aa0: 0000 0014 0002 0000 0000 0000 0000 0000  ................
+00001ab0: 0000 0000 0000 0000 0000 000b 0003 0000  ................
+00001ac0: 00b5 76f2 7a8f 0000 0000 0000 0001 1402  ..v.z...........
+00001ad0: 0000 0017 0048 313a 4944 512d 4641 505f  .....H1:IDQ-FAP_
+00001ae0: 4f56 4c5f 3332 5f32 3034 3800 0101 0500  OVL_32_2048.....
+00001af0: 0004 0000 0000 0000 2700 0000 0000 0000  ........'.......
+00001b00: 789c edc5 310d 0000 0c03 a0d5 bfe9 1d55  x...1..........U
+00001b10: d104 1e72 15db b66d dbb6 6ddb b66d dbb6  ...r...m..m..m..
+00001b20: 3dfb 0333 c004 0101 0000 0000 0400 0000  =..3............
+00001b30: 0000 0000 0000 0000 0070 3f00 0000 0000  .........p?.....
+00001b40: 0000 0002 0073 0001 0000 0000 0000 0000  .....s..........
+00001b50: aeb3 7f50 9200 0000 0000 0000 010b 0300  ...P............
+00001b60: 0000 1600 4831 3a49 4451 2d4f 4b5f 4f56  ....H1:IDQ-OK_OV
+00001b70: 4c5f 3332 5f32 3034 3800 1600 4831 3a49  L_32_2048...H1:I
+00001b80: 4451 2d4f 4b5f 4f56 4c5f 3332 5f32 3034  DQ-OK_OVL_32_204
+00001b90: 3800 0100 0000 0000 0000 0000 0000 0000  8...............
+00001ba0: 0000 0000 1040 0000 0000 0000 0000 0000  .....@..........
+00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bc0: 0000 0000 1400 0300 0000 0000 0000 0000  ................
+00001bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001be0: 0000 58c0 43d5 8e00 0000 0000 0000 0114  ..X.C...........
+00001bf0: 0300 0000 1600 4831 3a49 4451 2d4f 4b5f  ......H1:IDQ-OK_
+00001c00: 4f56 4c5f 3332 5f32 3034 3800 0101 0500  OVL_32_2048.....
+00001c10: 0004 0000 0000 0000 2700 0000 0000 0000  ........'.......
+00001c20: 789c edc5 310d 0000 0c03 a0d5 bfe9 1d55  x...1..........U
+00001c30: d104 1e72 15db b66d dbb6 6ddb b66d dbb6  ...r...m..m..m..
+00001c40: 3dfb 0333 c004 0101 0000 0000 0400 0000  =..3............
+00001c50: 0000 0000 0000 0000 0070 3f00 0000 0000  .........p?.....
+00001c60: 0000 0002 0073 0001 0000 0000 0000 0000  .....s..........
+00001c70: 1fbb ac07 4100 0000 0000 0000 0101 0400  ....A...........
+00001c80: 0000 0d00 4672 456e 644f 6646 7261 6d65  ....FrEndOfFrame
+00001c90: 0007 001c 0045 6e64 206f 6620 4672 616d  .....End of Fram
+00001ca0: 6520 4461 7461 2053 7472 7563 7475 7265  e Data Structure
+00001cb0: 009c ab33 e258 0000 0000 0000 0001 0247  ...3.X.........G
+00001cc0: 0000 0004 0072 756e 0007 0049 4e54 5f34  .....run...INT_4
+00001cd0: 5300 3500 5275 6e20 6e75 6d62 6572 3b20  S.5.Run number; 
+00001ce0: 7361 6d65 2061 7320 696e 2046 7261 6d65  same as in Frame
+00001cf0: 4865 6164 6572 2072 756e 206e 756d 6265  Header run numbe
+00001d00: 7220 6461 7475 6d2e 000b 9641 5b87 0000  r datum....A[...
+00001d10: 0000 0000 0001 0248 0000 0006 0066 7261  .......H.....fra
+00001d20: 6d65 0007 0049 4e54 5f34 5500 6200 4672  me...INT_4U.b.Fr
+00001d30: 616d 6520 6e75 6d62 6572 2c20 6d6f 6e6f  ame number, mono
+00001d40: 746f 6e69 6361 6c6c 7920 696e 6372 6561  tonically increa
+00001d50: 7369 6e67 2075 6e74 696c 2065 6e64 206f  sing until end o
+00001d60: 6620 7275 6e3b 2073 616d 6520 6173 2069  f run; same as i
+00001d70: 6e20 4672 616d 6520 4865 6164 6572 2072  n Frame Header r
+00001d80: 756e 206e 756d 6265 7220 6461 7475 6d00  un number datum.
+00001d90: ba5a b3d1 4700 0000 0000 0000 0102 4900  .Z..G.........I.
+00001da0: 0000 0700 4754 696d 6553 0007 0049 4e54  ....GTimeS...INT
+00001db0: 5f34 5500 2100 4672 616d 6520 7374 6172  _4U.!.Frame star
+00001dc0: 7420 7469 6d65 2069 6e20 4750 5320 5365  t time in GPS Se
+00001dd0: 636f 6e64 732e 0018 add0 ff56 0000 0000  conds......V....
+00001de0: 0000 0001 024a 0000 0007 0047 5469 6d65  .....J.....GTime
+00001df0: 4e00 0700 494e 545f 3455 0030 0046 7261  N...INT_4U.0.Fra
+00001e00: 6d65 2073 7461 7274 2074 696d 6520 7265  me start time re
+00001e10: 7369 6475 616c 2c20 696e 7465 6765 7220  sidual, integer 
+00001e20: 6e61 6e6f 7365 636f 6e64 732e 0064 338f  nanoseconds..d3.
+00001e30: ba36 0000 0000 0000 0001 024b 0000 0007  .6.........K....
+00001e40: 0063 686b 5375 6d00 0700 494e 545f 3455  .chkSum...INT_4U
+00001e50: 0010 0053 7472 7563 7420 6368 6563 6b73  ...Struct checks
+00001e60: 756d 0022 ca11 6222 0000 0000 0000 0001  um."..b"........
+00001e70: 0700 0000 0000 0000 002c 203c 5400 0000  ........., <T...
+00001e80: 0000 0000 00b4 e395 1b37 0000 0000 0000  .........7......
+00001e90: 0001 0100 0000 0006 0046 7254 4f43 0013  .........FrTOC..
+00001ea0: 0019 0053 696d 756c 6174 6564 2044 6174  ...Simulated Dat
+00001eb0: 6120 5374 7275 6374 7572 6500 7c69 656b  a Structure.|iek
+00001ec0: 4800 0000 0000 0000 0102 0000 0000 0700  H...............
+00001ed0: 554c 6561 7053 0007 0049 4e54 5f32 5300  ULeapS...INT_2S.
+00001ee0: 2200 4672 6f6d 2074 6865 2066 6972 7374  ".From the first
+00001ef0: 2046 7261 6d65 4820 696e 2074 6865 2066   FrameH in the f
+00001f00: 696c 6500 0087 5256 4300 0000 0000 0000  ile...RVC.......
+00001f10: 0102 0100 0000 0700 6e46 7261 6d65 0007  ........nFrame..
+00001f20: 0049 4e54 5f34 5500 1d00 4e75 6d62 6572  .INT_4U...Number
+00001f30: 206f 6620 6672 616d 6573 2069 6e20 7468   of frames in th
+00001f40: 6520 6669 6c65 00cc 3d5f 7370 0000 0000  e file..=_sp....
+00001f50: 0000 0001 0202 0000 000c 0064 6174 6151  ...........dataQ
+00001f60: 7561 6c69 7479 000f 0049 4e54 5f34 555b  uality...INT_4U[
+00001f70: 6e46 7261 6d65 5d00 3d00 4172 7261 7920  nFrame].=.Array 
+00001f80: 6f66 2069 6e74 6567 6572 2051 4120 776f  of integer QA wo
+00001f90: 7264 7320 6672 6f6d 2065 6163 6820 4672  rds from each Fr
+00001fa0: 616d 6548 2028 7369 7a65 206f 6620 6e46  ameH (size of nF
+00001fb0: 7261 6d65 7329 0088 6738 c05f 0000 0000  rames)..g8._....
+00001fc0: 0000 0001 0203 0000 0007 0047 5469 6d65  ...........GTime
+00001fd0: 5300 0f00 494e 545f 3455 5b6e 4672 616d  S...INT_4U[nFram
+00001fe0: 655d 0031 0041 7272 6179 206f 6620 696e  e].1.Array of in
+00001ff0: 7465 6765 7220 4750 5320 6672 6165 2074  teger GPS frae t
+00002000: 696d 6573 2028 7369 7a65 206f 6620 6e46  imes (size of nF
+00002010: 7261 6d65 7300 d5b2 6755 7600 0000 0000  rames...gUv.....
+00002020: 0000 0102 0400 0000 0700 4754 696d 654e  ..........GTimeN
+00002030: 000f 0049 4e54 5f34 555b 6e46 7261 6d65  ...INT_4U[nFrame
+00002040: 5d00 4800 4172 7261 7920 6f66 2069 6e74  ].H.Array of int
+00002050: 6567 6572 2047 5053 2072 6573 6964 7561  eger GPS residua
+00002060: 6c20 6e61 6e6f 7365 636f 6e64 7320 666f  l nanoseconds fo
+00002070: 7220 7468 6520 6672 616d 6520 2873 697a  r the frame (siz
+00002080: 6520 6f66 206e 4672 616d 6500 154d fabb  e of nFrame..M..
+00002090: 6000 0000 0000 0000 0102 0500 0000 0300  `...............
+000020a0: 6474 000f 0052 4541 4c5f 385b 6e46 7261  dt...REAL_8[nFra
+000020b0: 6d65 5d00 3600 4172 7261 7920 6f66 2066  me].6.Array of f
+000020c0: 7261 6d65 2064 7572 6174 696f 6e73 2069  rame durations i
+000020d0: 6e20 7365 636f 6e64 7328 2073 697a 6520  n seconds( size 
+000020e0: 6f66 206e 4672 616d 6573 2900 0d06 b877  of nFrames)....w
+000020f0: 5200 0000 0000 0000 0102 0600 0000 0500  R...............
+00002100: 7275 6e73 000f 0049 4e54 5f34 535b 6e46  runs...INT_4S[nF
+00002110: 7261 6d65 5d00 2600 4172 7261 7920 6f66  rame].&.Array of
+00002120: 2072 756e 206e 756d 6265 7273 2028 7369   run numbers (si
+00002130: 7a65 206f 6620 6e46 7261 6d65 2900 ca0b  ze of nFrame)...
+00002140: 9f5c 5500 0000 0000 0000 0102 0700 0000  .\U.............
+00002150: 0600 6672 616d 6500 0f00 494e 545f 3455  ..frame...INT_4U
+00002160: 5b6e 4672 616d 655d 0028 0041 7272 6179  [nFrame].(.Array
+00002170: 206f 6620 6672 616d 6520 6e75 6d62 6572   of frame number
+00002180: 7320 2873 697a 6520 6f66 206e 4672 616d  s (size of nFram
+00002190: 6529 0031 285d 2581 0000 0000 0000 0001  e).1(]%.........
+000021a0: 0208 0000 000a 0070 6f73 6974 696f 6e48  .......positionH
+000021b0: 000f 0049 4e54 5f38 555b 6e46 7261 6d65  ...INT_8U[nFrame
+000021c0: 5d00 5000 4172 7261 7920 6f66 2046 7261  ].P.Array of Fra
+000021d0: 6d65 4820 706f 7369 7469 6f6e 732c 2069  meH positions, i
+000021e0: 6e20 6279 7465 732c 2066 726f 6d20 7468  n bytes, from th
+000021f0: 6520 6267 696e 6e69 6e67 206f 6620 6669  e bginning of fi
+00002200: 6c65 2028 7369 7a65 206f 6620 6e46 7261  le (size of nFra
+00002210: 6d65 2900 db18 22e8 8700 0000 0000 0000  me)...".........
+00002220: 0102 0900 0000 0a00 6e46 6972 7374 4144  ........nFirstAD
+00002230: 4300 0f00 494e 545f 3855 5b6e 4672 616d  C...INT_8U[nFram
+00002240: 655d 0056 0041 7272 6179 206f 6620 6669  e].V.Array of fi
+00002250: 7273 7420 4672 4144 4344 6174 6120 706f  rst FrADCData po
+00002260: 7369 7469 6f6e 732c 2069 6e20 6279 7465  sitions, in byte
+00002270: 732c 2066 726f 6d20 6265 6769 6e6e 696e  s, from beginnin
+00002280: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
+00002290: 6f66 206e 4672 616d 6529 00b7 d5cd 8b86  of nFrame)......
+000022a0: 0000 0000 0000 0001 020a 0000 000a 006e  ...............n
+000022b0: 4669 7273 7453 6572 000f 0049 4e54 5f38  FirstSer...INT_8
+000022c0: 555b 6e46 7261 6d65 5d00 5500 4172 7261  U[nFrame].U.Arra
+000022d0: 7920 6f66 2066 6972 7374 2046 7253 6572  y of first FrSer
+000022e0: 4461 7461 2070 6f73 6974 696f 6e73 2069  Data positions i
+000022f0: 6e20 6279 7465 732c 2066 726f 6d20 6265  n bytes, from be
+00002300: 6769 6e6e 696e 6720 6f66 2066 696c 6520  ginning of file 
+00002310: 2873 697a 6520 6f66 206e 4672 616d 6529  (size of nFrame)
+00002320: 00fa c761 6b87 0000 0000 0000 0001 020b  ...ak...........
+00002330: 0000 000c 006e 4669 7273 7454 6162 6c65  .....nFirstTable
+00002340: 000f 0049 4e54 5f38 555b 6e46 7261 6d65  ...INT_8U[nFrame
+00002350: 5d00 5400 4172 7261 7920 6f66 2066 6972  ].T.Array of fir
+00002360: 7374 2046 7254 6162 6c65 2070 6f73 6974  st FrTable posit
+00002370: 696f 6e73 2c20 696e 2062 7974 6573 2c20  ions, in bytes, 
+00002380: 6672 6f6d 2062 6567 696e 6e69 6e67 206f  from beginning o
+00002390: 6620 6669 6c65 2028 7369 7a65 206f 6620  f file (size of 
+000023a0: 6e46 7261 6d65 2900 1016 52a6 8300 0000  nFrame)...R.....
+000023b0: 0000 0000 0102 0c00 0000 0a00 6e46 6972  ............nFir
+000023c0: 7374 4d73 6700 0f00 494e 545f 3855 5b6e  stMsg...INT_8U[n
+000023d0: 4672 616d 655d 0052 0041 7272 6179 206f  Frame].R.Array o
+000023e0: 6620 6669 7273 7420 4672 4d73 6720 706f  f first FrMsg po
+000023f0: 7369 7469 6f6e 732c 2069 6e20 6279 7465  sitions, in byte
+00002400: 732c 2066 726f 6d20 6265 6769 6e6e 696e  s, from beginnin
+00002410: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
+00002420: 6f66 206e 4672 616d 6529 00b9 e1c6 f949  of nFrame).....I
+00002430: 0000 0000 0000 0001 020d 0000 0004 006e  ...............n
+00002440: 5348 0007 0049 4e54 5f34 5500 2600 4e75  SH...INT_4U.&.Nu
+00002450: 6d62 6572 206f 6620 4672 5348 2073 7472  mber of FrSH str
+00002460: 7563 7475 7265 7320 696e 2074 6865 2066  uctures in the f
+00002470: 696c 6500 f46c 0bb0 4900 0000 0000 0000  ile..l..I.......
+00002480: 0102 0e00 0000 0500 5348 6964 000c 0049  ........SHid...I
+00002490: 4e54 5f32 555b 6e53 485d 0020 0041 7272  NT_2U[nSH]. .Arr
+000024a0: 6179 206f 6620 4672 5348 2049 4473 2028  ay of FrSH IDs (
+000024b0: 7369 7a65 206f 6620 6e53 4829 0010 5b23  size of nSH)..[#
+000024c0: 074d 0000 0000 0000 0001 020f 0000 0007  .M..............
+000024d0: 0053 486e 616d 6500 0c00 5354 5249 4e47  .SHname...STRING
+000024e0: 5b6e 5348 5d00 2200 4172 7261 7920 6f66  [nSH].".Array of
+000024f0: 2046 7253 4820 6e61 6d65 7320 2873 697a   FrSH names (siz
+00002500: 6520 6f66 206e 5348 2900 a664 b4df 5c00  e of nSH)..d..\.
+00002510: 0000 0000 0000 0102 1000 0000 0a00 6e44  ..............nD
+00002520: 6574 6563 746f 7200 0700 494e 545f 3455  etector...INT_4U
+00002530: 0033 004e 756d 6265 7220 6f66 2064 6973  .3.Number of dis
+00002540: 7469 6e63 7420 7479 7065 7320 6f66 2046  tinct types of F
+00002550: 7244 6574 6563 746f 7220 696e 2074 6865  rDetector in the
+00002560: 2066 696c 6500 fa46 0067 8100 0000 0000   file..F.g......
+00002570: 0000 0102 1100 0000 0d00 6e61 6d65 4465  ..........nameDe
+00002580: 7465 6374 6f72 0012 0053 5452 494e 475b  tector...STRING[
+00002590: 6e44 6574 6563 746f 725d 004a 0041 7272  nDetector].J.Arr
+000025a0: 6179 206f 6620 4672 4465 7465 6374 6f72  ay of FrDetector
+000025b0: 206e 616d 6573 2028 7369 7a65 206f 6620   names (size of 
+000025c0: 6e44 6574 6563 746f 7229 2e20 5468 6579  nDetector). They
+000025d0: 2061 7070 6561 7220 616c 7068 6162 6574   appear alphabet
+000025e0: 6963 616c 6c79 0011 11d2 a589 0000 0000  ically..........
+000025f0: 0000 0001 0212 0000 0011 0070 6f73 6974  ...........posit
+00002600: 696f 6e44 6574 6563 746f 7200 1200 494e  ionDetector...IN
+00002610: 545f 3855 5b6e 4465 7465 6374 6f72 5d00  T_8U[nDetector].
+00002620: 4e00 4172 7261 7920 6f66 2046 7244 6574  N.Array of FrDet
+00002630: 6563 746f 7220 706f 7369 7469 6f6e 7320  ector positions 
+00002640: 6672 6f6d 2074 6865 2062 6567 696e 6e69  from the beginni
+00002650: 6e67 206f 6620 6669 6c65 2028 7369 7a65  ng of file (size
+00002660: 206f 6620 6e44 6574 6563 746f 7229 2e00   of nDetector)..
+00002670: 8345 9ff0 5800 0000 0000 0000 0102 1300  .E..X...........
+00002680: 0000 0a00 6e53 7461 7454 7970 6500 0700  ....nStatType...
+00002690: 494e 545f 3455 002f 004e 756d 6265 7220  INT_4U./.Number 
+000026a0: 6f66 2073 7461 7469 6320 6461 7461 2062  of static data b
+000026b0: 6c6f 636b 2074 7970 6573 2069 6e20 7468  lock types in th
+000026c0: 6520 6669 6c65 2e00 0f05 6246 6000 0000  e file....bF`...
+000026d0: 0000 0000 0102 1400 0000 0900 6e61 6d65  ............name
+000026e0: 5374 6174 0012 0053 5452 494e 475b 6e53  Stat...STRING[nS
+000026f0: 7461 7454 7970 655d 002d 0041 7272 6179  tatType].-.Array
+00002700: 206f 6620 4672 5374 6174 4461 7461 206e   of FrStatData n
+00002710: 616d 6520 2873 697a 6520 6f66 206e 5374  ame (size of nSt
+00002720: 6174 5479 7065 2900 a3bf 4547 5d00 0000  atType)...EG]...
+00002730: 0000 0000 0102 1500 0000 0900 6465 7465  ............dete
+00002740: 6374 6f72 0012 0053 5452 494e 475b 6e53  ctor...STRING[nS
+00002750: 7461 7454 7970 655d 002a 0041 7272 6179  tatType].*.Array
+00002760: 206f 6620 4465 7465 6374 6f72 206e 616d   of Detector nam
+00002770: 6528 7369 7a65 206f 6620 6e53 7461 7454  e(size of nStatT
+00002780: 7970 6529 0041 b642 9d7b 0000 0000 0000  ype).A.B.{......
+00002790: 0001 0216 0000 000e 006e 5374 6174 496e  .........nStatIn
+000027a0: 7374 616e 6365 0012 0049 4e54 5f34 555b  stance...INT_4U[
+000027b0: 6e53 7461 7454 7970 655d 0043 0041 7272  nStatType].C.Arr
+000027c0: 6179 206f 6620 6e75 6d62 6572 206f 6620  ay of number of 
+000027d0: 696e 7374 616e 6365 2066 6f72 2065 6163  instance for eac
+000027e0: 6820 4672 5374 6174 4461 7461 2873 697a  h FrStatData(siz
+000027f0: 6520 6f66 206e 5374 6174 5479 7065 2900  e of nStatType).
+00002800: 66b8 774f 4b00 0000 0000 0000 0102 1700  f.wOK...........
+00002810: 0000 0b00 6e54 6f74 616c 5374 6174 0007  ....nTotalStat..
+00002820: 0049 4e54 5f34 5500 2100 5375 6d6d 6174  .INT_4U.!.Summat
+00002830: 696f 6e20 6f66 206e 5374 6174 496e 7374  ion of nStatInst
+00002840: 616e 6365 2061 7272 6179 0089 b4e7 f874  ance array.....t
+00002850: 0000 0000 0000 0001 0218 0000 0007 0074  ...............t
+00002860: 5374 6172 7400 1300 494e 545f 3455 5b6e  Start...INT_4U[n
+00002870: 546f 7461 6c53 7461 745d 0042 0041 7272  TotalStat].B.Arr
+00002880: 6179 206f 6620 4750 5320 696e 7465 6765  ay of GPS intege
+00002890: 7220 7374 6172 7420 7469 6d65 732c 2069  r start times, i
+000028a0: 6e20 7365 636f 6e64 7320 2873 697a 6520  n seconds (size 
+000028b0: 6f66 206e 546f 7461 6c53 7461 7429 001a  of nTotalStat)..
+000028c0: 531d 0970 0000 0000 0000 0001 0219 0000  S..p............
+000028d0: 0005 0074 456e 6400 1300 494e 545f 3455  ...tEnd...INT_4U
+000028e0: 5b6e 546f 7461 6c53 7461 745d 0040 0041  [nTotalStat].@.A
+000028f0: 7272 6179 206f 6620 4750 5320 696e 7465  rray of GPS inte
+00002900: 6765 7220 656e 6420 7469 6d65 732c 2069  ger end times, i
+00002910: 6e20 7365 636f 6e64 7320 2873 697a 6520  n seconds (size 
+00002920: 6f66 206e 546f 7461 6c53 7461 7429 0045  of nTotalStat).E
+00002930: 668b 4d5e 0000 0000 0000 0001 021a 0000  f.M^............
+00002940: 0008 0076 6572 7369 6f6e 0013 0049 4e54  ...version...INT
+00002950: 5f34 555b 6e54 6f74 616c 5374 6174 5d00  _4U[nTotalStat].
+00002960: 2b00 4172 7261 7920 6f66 2076 6572 7369  +.Array of versi
+00002970: 6f6e 2074 696d 6520 2873 697a 6520 6f66  on time (size of
+00002980: 206e 546f 7461 6c53 7461 7429 0093 e259   nTotalStat)...Y
+00002990: 1d82 0000 0000 0000 0001 021b 0000 000d  ................
+000029a0: 0070 6f73 6974 696f 6e53 7461 7400 1300  .positionStat...
+000029b0: 494e 545f 3855 5b6e 546f 7461 6c53 7461  INT_8U[nTotalSta
+000029c0: 745d 004a 0041 7272 6179 206f 6620 4672  t].J.Array of Fr
+000029d0: 5374 6174 4461 7461 2070 6f73 6974 696f  StatData positio
+000029e0: 6e73 2066 726f 6d20 6265 6769 6e6e 696e  ns from beginnin
+000029f0: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
+00002a00: 6f66 206e 546f 7461 6c53 7461 7429 002e  of nTotalStat)..
+00002a10: 51de 564e 0000 0000 0000 0001 021c 0000  Q.VN............
+00002a20: 0005 006e 4144 4300 0700 494e 545f 3455  ...nADC...INT_4U
+00002a30: 002a 004e 756d 6265 7220 6f66 2075 6e69  .*.Number of uni
+00002a40: 7175 6520 4672 4164 6344 6174 6120 6e61  que FrAdcData na
+00002a50: 6d65 7320 696e 2066 696c 652e 0007 54ee  mes in file...T.
+00002a60: e143 0000 0000 0000 0001 021d 0000 0005  .C..............
+00002a70: 006e 616d 6500 0d00 5354 5249 4e47 5b6e  .name...STRING[n
+00002a80: 4144 435d 0019 0041 7272 6179 206f 6620  ADC]...Array of 
+00002a90: 4672 4164 6344 6174 6120 6e61 6d65 7300  FrAdcData names.
+00002aa0: 89b1 c3ad 4800 0000 0000 0000 0102 1e00  ....H...........
+00002ab0: 0000 0a00 6368 616e 6e65 6c49 4400 0d00  ....channelID...
+00002ac0: 494e 545f 3455 5b6e 4144 435d 0019 0041  INT_4U[nADC]...A
+00002ad0: 7272 6179 206f 6620 4144 4320 6368 616e  rray of ADC chan
+00002ae0: 6e65 6c20 4944 7300 251b 8f78 4400 0000  nel IDs.%..xD...
+00002af0: 0000 0000 0102 1f00 0000 0800 6772 6f75  ............grou
+00002b00: 7049 4400 0d00 494e 545f 3455 5b6e 4144  pID...INT_4U[nAD
+00002b10: 435d 0017 0041 7272 6179 206f 6620 4144  C]...Array of AD
+00002b20: 4320 6772 6f75 7020 4944 7300 ec33 7c9e  C group IDs..3|.
+00002b30: 9e00 0000 0000 0000 0102 2000 0000 0c00  .......... .....
+00002b40: 706f 7369 7469 6f6e 4144 4300 1500 494e  positionADC...IN
+00002b50: 545f 3855 5b6e 4144 435d 5b6e 4672 616d  T_8U[nADC][nFram
+00002b60: 655d 0065 0041 7272 6179 206f 6620 6c69  e].e.Array of li
+00002b70: 7374 7320 6f66 2046 7241 6463 4461 7461  sts of FrAdcData
+00002b80: 206f 6666 7365 7420 706f 7369 7469 6f6e   offset position
+00002b90: 732c 2069 6e20 6279 7465 732c 2066 726f  s, in bytes, fro
+00002ba0: 6d20 6265 6769 6e6e 696e 6720 6f66 2066  m beginning of f
+00002bb0: 696c 6520 2873 697a 6520 6f66 206e 4672  ile (size of nFr
+00002bc0: 616d 652a 6e41 4443 2900 6d54 ccf2 5000  ame*nADC).mT..P.
+00002bd0: 0000 0000 0000 0102 2100 0000 0600 6e50  ........!.....nP
+00002be0: 726f 6300 0700 494e 545f 3455 002b 004e  roc...INT_4U.+.N
+00002bf0: 756d 6265 7220 6f66 2075 6e69 7175 6520  umber of unique 
+00002c00: 4672 5072 6f63 4461 7461 206e 616d 6573  FrProcData names
+00002c10: 2069 6e20 6669 6c65 2e00 feef 7499 4900   in file....t.I.
+00002c20: 0000 0000 0000 0102 2200 0000 0900 6e61  ........".....na
+00002c30: 6d65 5072 6f63 000e 0053 5452 494e 475b  meProc...STRING[
+00002c40: 6e50 726f 635d 001a 0041 7272 6179 206f  nProc]...Array o
+00002c50: 6620 4672 5072 6f63 4461 7461 206e 616d  f FrProcData nam
+00002c60: 6573 0092 f0ec 64a2 0000 0000 0000 0001  es....d.........
+00002c70: 0223 0000 000d 0070 6f73 6974 696f 6e50  .#.....positionP
+00002c80: 726f 6300 1600 494e 545f 3855 5b6e 5072  roc...INT_8U[nPr
+00002c90: 6f63 5d5b 6e46 7261 6d65 5d00 6700 4172  oc][nFrame].g.Ar
+00002ca0: 7261 7920 6f66 206c 6973 7473 206f 6620  ray of lists of 
+00002cb0: 4672 5072 6f63 4461 7461 206f 6666 7365  FrProcData offse
+00002cc0: 7420 706f 7369 7469 6f6e 732c 2069 6e20  t positions, in 
+00002cd0: 6279 7465 732c 2066 726f 6d20 6265 6769  bytes, from begi
+00002ce0: 6e6e 696e 6720 6f66 2066 696c 6520 2873  nning of file (s
+00002cf0: 697a 6520 6f66 206e 4672 616d 652a 6e50  ize of nFrame*nP
+00002d00: 726f 6329 00f2 b9e4 a64e 0000 0000 0000  roc).....N......
+00002d10: 0001 0224 0000 0005 006e 5369 6d00 0700  ...$.....nSim...
+00002d20: 494e 545f 3455 002a 004e 756d 6265 7220  INT_4U.*.Number 
+00002d30: 6f66 2075 6e69 7175 6520 4672 5369 6d44  of unique FrSimD
+00002d40: 6174 6120 6e61 6d65 7320 696e 2066 696c  ata names in fil
+00002d50: 652e 0008 01bc 3746 0000 0000 0000 0001  e.....7F........
+00002d60: 0225 0000 0008 006e 616d 6553 696d 000d  .%.....nameSim..
+00002d70: 0053 5452 494e 475b 6e53 696d 5d00 1900  .STRING[nSim]...
+00002d80: 4172 7261 7920 6f66 2046 7253 696d 4461  Array of FrSimDa
+00002d90: 7461 206e 616d 6573 00c4 a72b f69e 0000  ta names...+....
+00002da0: 0000 0000 0001 0226 0000 000c 0070 6f73  .......&.....pos
+00002db0: 6974 696f 6e53 696d 0015 0049 4e54 5f38  itionSim...INT_8
+00002dc0: 555b 6e53 696d 5d5b 6e46 7261 6d65 5d00  U[nSim][nFrame].
+00002dd0: 6500 4172 7261 7920 6f66 206c 6973 7473  e.Array of lists
+00002de0: 206f 6620 4672 5369 6d44 6174 6120 6f66   of FrSimData of
+00002df0: 6673 6574 2070 6f73 6974 696f 6e73 2c20  fset positions, 
+00002e00: 696e 2062 7974 6573 2c20 6672 6f6d 2062  in bytes, from b
+00002e10: 6567 696e 6e69 6e67 206f 6620 6669 6c65  eginning of file
+00002e20: 2028 7369 7a65 206f 6620 6e46 7261 6d65   (size of nFrame
+00002e30: 2a6e 5369 6d29 00d3 40ba c14e 0000 0000  *nSim)..@..N....
+00002e40: 0000 0001 0227 0000 0005 006e 5365 7200  .....'.....nSer.
+00002e50: 0700 494e 545f 3455 002a 004e 756d 6265  ..INT_4U.*.Numbe
+00002e60: 7220 6f66 2075 6e69 7175 6520 4672 5365  r of unique FrSe
+00002e70: 7244 6174 6120 6e61 6d65 7320 696e 2066  rData names in f
+00002e80: 696c 652e 000f 814d 9046 0000 0000 0000  ile....M.F......
+00002e90: 0001 0228 0000 0008 006e 616d 6553 6572  ...(.....nameSer
+00002ea0: 000d 0053 5452 494e 475b 6e53 6572 5d00  ...STRING[nSer].
+00002eb0: 1900 4172 7261 7920 6f66 2046 7253 6572  ..Array of FrSer
+00002ec0: 4461 7461 206e 616d 6573 00bd 2d79 109e  Data names..-y..
+00002ed0: 0000 0000 0000 0001 0229 0000 000c 0070  .........).....p
+00002ee0: 6f73 6974 696f 6e53 6572 0015 0049 4e54  ositionSer...INT
+00002ef0: 5f38 555b 6e53 6572 5d5b 6e46 7261 6d65  _8U[nSer][nFrame
+00002f00: 5d00 6500 4172 7261 7920 6f66 206c 6973  ].e.Array of lis
+00002f10: 7473 206f 6620 4672 5365 7244 6174 6120  ts of FrSerData 
+00002f20: 6f66 6673 6574 2070 6f73 6974 696f 6e73  offset positions
+00002f30: 2c20 696e 2062 7974 6573 2c20 6672 6f6d  , in bytes, from
+00002f40: 2062 6567 696e 6e69 6e67 206f 6620 6669   beginning of fi
+00002f50: 6c65 2028 7369 7a65 206f 6620 6e46 7261  le (size of nFra
+00002f60: 6d65 2a6e 5365 7229 001c 5003 fb52 0000  me*nSer)..P..R..
+00002f70: 0000 0000 0001 022a 0000 0009 006e 5375  .......*.....nSu
+00002f80: 6d6d 6172 7900 0700 494e 545f 3455 002a  mmary...INT_4U.*
+00002f90: 004e 756d 6265 7220 6f66 2075 6e69 7175  .Number of uniqu
+00002fa0: 6520 4672 5375 6d6d 6172 7920 6e61 6d65  e FrSummary name
+00002fb0: 7320 696e 2066 696c 652e 0034 77a5 e94b  s in file..4w..K
+00002fc0: 0000 0000 0000 0001 022b 0000 0009 006e  .........+.....n
+00002fd0: 616d 6553 5375 6d00 1100 5354 5249 4e47  ameSSum...STRING
+00002fe0: 5b6e 5375 6d6d 6172 795d 0019 0041 7272  [nSummary]...Arr
+00002ff0: 6179 206f 6620 4672 5375 6d6d 6172 7920  ay of FrSummary 
+00003000: 6e61 6d65 7300 0684 574e a200 0000 0000  names...WN......
+00003010: 0000 0102 2c00 0000 0c00 706f 7369 7469  ....,.....positi
+00003020: 6f6e 5365 7200 1900 494e 545f 3855 5b6e  onSer...INT_8U[n
+00003030: 5375 6d6d 6172 795d 5b6e 4672 616d 655d  Summary][nFrame]
+00003040: 0065 0041 7272 6179 206f 6620 6c69 7374  .e.Array of list
+00003050: 7320 6f66 2046 7253 756d 6d61 7279 206f  s of FrSummary o
+00003060: 6666 7365 7420 706f 7369 7469 6f6e 732c  ffset positions,
+00003070: 2069 6e20 6279 7465 732c 2066 726f 6d20   in bytes, from 
+00003080: 6265 6769 6e6e 696e 6720 6f66 2066 696c  beginning of fil
+00003090: 6520 2873 697a 6520 6f66 206e 4672 616d  e (size of nFram
+000030a0: 652a 6e53 6572 2900 c376 da95 4800 0000  e*nSer)..v..H...
+000030b0: 0000 0000 0102 2d00 0000 0b00 6e45 7665  ......-.....nEve
+000030c0: 6e74 5479 7065 0007 0049 4e54 5f34 5500  ntType...INT_4U.
+000030d0: 1e00 4e75 6d62 6572 206f 6620 4672 4576  ..Number of FrEv
+000030e0: 656e 7420 696e 2074 6865 2066 696c 6500  ent in the file.
+000030f0: cb0b 34f7 4c00 0000 0000 0000 0102 2e00  ..4.L...........
+00003100: 0000 0a00 6e61 6d65 4576 656e 7400 1300  ....nameEvent...
+00003110: 5354 5249 4e47 5b6e 4576 656e 7454 7970  STRING[nEventTyp
+00003120: 655d 0017 0041 7272 6179 206f 6620 4672  e]...Array of Fr
+00003130: 4576 656e 7420 6e61 6d65 7300 8aec 7442  Event names...tB
+00003140: 7200 0000 0000 0000 0102 2f00 0000 0700  r........./.....
+00003150: 6e45 7665 6e74 0013 0049 4e54 5f34 555b  nEvent...INT_4U[
+00003160: 6e45 7665 6e74 5479 7065 5d00 4000 4e75  nEventType].@.Nu
+00003170: 6d62 6572 206f 6620 4672 4576 656e 7420  mber of FrEvent 
+00003180: 666f 7220 6561 6368 2074 7970 6520 6f66  for each type of
+00003190: 2046 7245 7665 6e74 2028 7369 7a65 206f   FrEvent (size o
+000031a0: 6620 6e45 7665 6e74 5479 7065 2900 aebb  f nEventType)...
+000031b0: 6fd3 4300 0000 0000 0000 0102 3000 0000  o.C.........0...
+000031c0: 0c00 6e54 6f74 616c 4576 656e 7400 0700  ..nTotalEvent...
+000031d0: 494e 545f 3455 0018 0054 6f74 616c 206e  INT_4U...Total n
+000031e0: 756d 6265 7220 6f66 2046 7245 7665 6e74  umber of FrEvent
+000031f0: 0074 8af4 4a54 0000 0000 0000 0001 0231  .t..JT.........1
+00003200: 0000 000c 0047 5469 6d65 5345 7665 6e74  .....GTimeSEvent
+00003210: 0014 0049 4e54 5f34 555b 6e54 6f74 616c  ...INT_4U[nTotal
+00003220: 4576 656e 745d 001c 0047 5053 2074 696d  Event]...GPS tim
+00003230: 6520 696e 2069 6e74 6567 6572 2073 6563  e in integer sec
+00003240: 6f6e 6473 0015 3513 2961 0000 0000 0000  onds..5.)a......
+00003250: 0001 0232 0000 000c 0047 5469 6d65 4e45  ...2.....GTimeNE
+00003260: 7665 6e74 0014 0049 4e54 5f34 555b 6e54  vent...INT_4U[nT
+00003270: 6f74 616c 4576 656e 745d 0029 0052 6573  otalEvent].).Res
+00003280: 6964 7561 6c20 4750 5320 7469 6d65 2069  idual GPS time i
+00003290: 6e20 696e 7465 6765 7220 6e61 6e6f 7365  n integer nanose
+000032a0: 636f 6e64 7300 157d 335d 4b00 0000 0000  conds..}3]K.....
+000032b0: 0000 0102 3300 0000 0f00 616d 706c 6974  ....3.....amplit
+000032c0: 7564 6545 7665 6e74 0014 0052 4541 4c5f  udeEvent...REAL_
+000032d0: 345b 6e54 6f74 616c 4576 656e 745d 0010  4[nTotalEvent]..
+000032e0: 0045 7665 6e74 2061 6d70 6c69 7475 6465  .Event amplitude
+000032f0: 00c2 ba16 4177 0000 0000 0000 0001 0234  ....Aw.........4
+00003300: 0000 000e 0070 6f73 6974 696f 6e45 7665  .....positionEve
+00003310: 6e74 0014 0049 4e54 5f38 555b 6e54 6f74  nt...INT_8U[nTot
+00003320: 616c 4576 656e 745d 003d 0041 7272 6179  alEvent].=.Array
+00003330: 206f 6620 4672 4576 656e 7420 706f 7369   of FrEvent posi
+00003340: 7469 6f6e 732c 2069 6e20 6279 7465 732c  tions, in bytes,
+00003350: 2066 726f 6d20 6265 6769 6e6e 696e 6720   from beginning 
+00003360: 6f66 2066 696c 6500 46be 4b47 4e00 0000  of file.F.KGN...
+00003370: 0000 0000 0102 3500 0000 0e00 6e53 696d  ......5.....nSim
+00003380: 4576 656e 7454 7970 6500 0700 494e 545f  EventType...INT_
+00003390: 3455 0021 004e 756d 6265 7220 6f66 2046  4U.!.Number of F
+000033a0: 7253 696d 4576 656e 7420 696e 2074 6865  rSimEvent in the
+000033b0: 2066 696c 6500 d601 de2b 5500 0000 0000   file....+U.....
+000033c0: 0000 0102 3600 0000 0d00 6e61 6d65 5369  ....6.....nameSi
+000033d0: 6d45 7665 6e74 0016 0053 5452 494e 475b  mEvent...STRING[
+000033e0: 6e53 696d 4576 656e 7454 7970 655d 001a  nSimEventType]..
+000033f0: 0041 7272 6179 206f 6620 4672 5369 6d45  .Array of FrSimE
+00003400: 7665 6e74 206e 616d 6573 00c3 e4da a081  vent names......
+00003410: 0000 0000 0000 0001 0237 0000 000a 006e  .........7.....n
+00003420: 5369 6d45 7665 6e74 0016 0049 4e54 5f34  SimEvent...INT_4
+00003430: 555b 6e53 696d 4576 656e 7454 7970 655d  U[nSimEventType]
+00003440: 0049 004e 756d 6265 7220 6f66 2046 7253  .I.Number of FrS
+00003450: 696d 4576 656e 7420 666f 7220 6561 6368  imEvent for each
+00003460: 2074 7970 6520 6f66 2046 7253 696d 4576   type of FrSimEv
+00003470: 656e 7420 2873 697a 6520 6f66 206e 5369  ent (size of nSi
+00003480: 6d45 7665 6e74 5479 7065 2900 4e11 c946  mEventType).N..F
+00003490: 4700 0000 0000 0000 0102 3800 0000 0d00  G.........8.....
+000034a0: 6e54 6f74 616c 5345 7665 6e74 0007 0049  nTotalSEvent...I
+000034b0: 4e54 5f34 5500 1b00 546f 7461 6c20 6e75  NT_4U...Total nu
+000034c0: 6d62 6572 206f 6620 4672 5369 6d45 7665  mber of FrSimEve
+000034d0: 6e74 00de 86a5 7e53 0000 0000 0000 0001  nt....~S........
+000034e0: 0239 0000 000a 0047 5469 6d65 5353 696d  .9.....GTimeSSim
+000034f0: 0015 0049 4e54 5f34 555b 6e54 6f74 616c  ...INT_4U[nTotal
+00003500: 5345 7665 6e74 5d00 1c00 4750 5320 7469  SEvent]...GPS ti
+00003510: 6d65 2069 6e20 696e 7465 6765 7220 7365  me in integer se
+00003520: 636f 6e64 7300 8b64 9181 6000 0000 0000  conds..d..`.....
+00003530: 0000 0102 3a00 0000 0a00 4754 696d 654e  ....:.....GTimeN
+00003540: 5369 6d00 1500 494e 545f 3455 5b6e 546f  Sim...INT_4U[nTo
+00003550: 7461 6c53 4576 656e 745d 0029 0052 6573  talSEvent].).Res
+00003560: 6964 7561 6c20 4750 5320 7469 6d65 2069  idual GPS time i
+00003570: 6e20 696e 7465 6765 7220 6e61 6e6f 7365  n integer nanose
+00003580: 636f 6e64 7300 6127 db26 5200 0000 0000  conds.a'.&R.....
+00003590: 0000 0102 3b00 0000 1200 616d 706c 6974  ....;.....amplit
+000035a0: 7564 6553 696d 4576 656e 7400 1500 5245  udeSimEvent...RE
+000035b0: 414c 5f34 5b6e 546f 7461 6c53 4576 656e  AL_4[nTotalSEven
+000035c0: 745d 0013 0053 696d 4576 656e 7420 616d  t]...SimEvent am
+000035d0: 706c 6974 7564 6500 2410 90c2 7e00 0000  plitude.$...~...
+000035e0: 0000 0000 0102 3c00 0000 1100 706f 7369  ......<.....posi
+000035f0: 7469 6f6e 5369 6d45 7665 6e74 0015 0049  tionSimEvent...I
+00003600: 4e54 5f38 555b 6e54 6f74 616c 5345 7665  NT_8U[nTotalSEve
+00003610: 6e74 5d00 4000 4172 7261 7920 6f66 2046  nt].@.Array of F
+00003620: 7253 696d 4576 656e 7420 706f 7369 7469  rSimEvent positi
+00003630: 6f6e 732c 2069 6e20 6279 7465 732c 2066  ons, in bytes, f
+00003640: 726f 6d20 6265 6769 6e6e 696e 6720 6f66  rom beginning of
+00003650: 2066 696c 6500 9f96 37f5 3600 0000 0000   file...7.6.....
+00003660: 0000 0102 3d00 0000 0700 6368 6b53 756d  ....=.....chkSum
+00003670: 0007 0049 4e54 5f34 5500 1000 5374 7275  ...INT_4U...Stru
+00003680: 6374 2063 6865 636b 7375 6d00 8e79 d77a  ct checksum..y.z
+00003690: 7001 0000 0000 0000 0113 0000 0000 2500  p.............%.
+000036a0: 0100 0000 696d 6553 b881 8348 0000 0000  ....imeS...H....
+000036b0: 0000 0000 0000 1040 0000 0000 2c20 3c54  .......@...., <T
+000036c0: 6e09 0000 0000 0000 0000 0000 0000 0000  n...............
+000036d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000036e0: 0000 0000 0000 0000 0600 0000 0300 0500  ................
+000036f0: 0b00 1400 0700 1300 0700 4672 616d 6548  ..........FrameH
+00003700: 000b 0046 7244 6574 6563 746f 7200 0b00  ...FrDetector...
+00003710: 4672 5072 6f63 4461 7461 0007 0046 7256  FrProcData...FrV
+00003720: 6563 7400 0d00 4672 456e 644f 6646 7261  ect...FrEndOfFra
+00003730: 6d65 0006 0046 7254 4f43 0001 0000 0007  me...FrTOC......
+00003740: 004c 484f 5f34 6b00 020d 0000 0000 0000  .LHO_4k.........
+00003750: 0000 0000 0000 0000 0000 0000 0400 0000  ................
+00003760: 1100 4831 3a44 4d54 2d44 515f 5645 4354  ..H1:DMT-DQ_VECT
+00003770: 4f52 001a 0048 313a 4744 532d 4341 4c49  OR...H1:GDS-CALI
+00003780: 425f 5354 4154 455f 5645 4354 4f52 0017  B_STATE_VECTOR..
+00003790: 0048 313a 4944 512d 4641 505f 4f56 4c5f  .H1:IDQ-FAP_OVL_
+000037a0: 3332 5f32 3034 3800 1600 4831 3a49 4451  32_2048...H1:IDQ
+000037b0: 2d4f 4b5f 4f56 4c5f 3332 5f32 3034 3800  -OK_OVL_32_2048.
+000037c0: 3719 0000 0000 0000 0214 0000 0000 0000  7...............
+000037d0: 311a 0000 0000 0000 541b 0000 0000 0000  1.......T.......
+000037e0: ffff ffff ffff ffff ffff ffff 0000 0000  ................
+000037f0: 0000 0000 0000 0000 0000 0000 58fe 5def  ............X.].
+00003800: 3f00 0000 0000 0000 0101 0100 0000 0c00  ?...............
+00003810: 4672 456e 644f 6646 696c 6500 0600 1b00  FrEndOfFile.....
+00003820: 456e 6420 6f66 2046 696c 6520 4461 7461  End of File Data
+00003830: 2053 7472 7563 7475 7265 00a8 da1b ec45   Structure.....E
+00003840: 0000 0000 0000 0001 023e 0000 0008 006e  .........>.....n
+00003850: 4672 616d 6573 0007 0049 4e54 5f34 5500  Frames...INT_4U.
+00003860: 1e00 4e75 6d62 6572 206f 6620 6672 616d  ..Number of fram
+00003870: 6573 2069 6e20 7468 6973 2066 696c 6500  es in this file.
+00003880: c01d f442 5f00 0000 0000 0000 0102 3f00  ...B_.........?.
+00003890: 0000 0700 6e42 7974 6573 0007 0049 4e54  ....nBytes...INT
+000038a0: 5f38 5500 3900 546f 7461 6c20 6e75 6d62  _8U.9.Total numb
+000038b0: 6572 206f 6620 6279 7465 7320 696e 2074  er of bytes in t
+000038c0: 6869 7320 6669 6c65 2028 2030 2069 6620  his file ( 0 if 
+000038d0: 4e4f 5420 636f 6d70 7574 6564 2029 0082  NOT computed )..
+000038e0: 8d13 02a1 0000 0000 0000 0001 0240 0000  .............@..
+000038f0: 0008 0073 6565 6b54 4f43 0007 0049 4e54  ...seekTOC...INT
+00003900: 5f38 5500 7a00 4279 6573 2074 6f20 6261  _8U.z.Byes to ba
+00003910: 636b 2075 7020 746f 2074 6865 2062 6567  ck up to the beg
+00003920: 696e 6e69 6e67 206f 6620 7468 6520 7461  inning of the ta
+00003930: 626c 6520 6f66 2063 6f6e 7465 6e74 7320  ble of contents 
+00003940: 7374 7275 6374 7572 652e 2049 6620 7365  structure. If se
+00003950: 656b 544f 4320 3d3d 2030 2c20 7468 656e  ekTOC == 0, then
+00003960: 2074 6865 7265 2069 7320 6e6f 2054 4f43   there is no TOC
+00003970: 2066 6f72 2074 6869 7320 6669 6c65 2e00   for this file..
+00003980: c8d4 6535 4100 0000 0000 0000 0102 4100  ..e5A.........A.
+00003990: 0000 0f00 6368 6b53 756d 4672 4865 6164  ....chkSumFrHead
+000039a0: 6572 0007 0049 4e54 5f34 5500 1300 4672  er...INT_4U...Fr
+000039b0: 4865 6164 6572 2063 6865 636b 7375 6d2e  Header checksum.
+000039c0: 0009 9135 933a 0000 0000 0000 0001 0242  ...5.:.........B
+000039d0: 0000 0007 0063 686b 5375 6d00 0700 494e  .....chkSum...IN
+000039e0: 545f 3455 0014 0053 7472 7563 7475 7265  T_4U...Structure
+000039f0: 2063 6865 636b 7375 6d2e 00d0 97d1 a839   checksum......9
+00003a00: 0000 0000 0000 0001 0243 0000 000b 0063  .........C.....c
+00003a10: 686b 5375 6d46 696c 6500 0700 494e 545f  hkSumFile...INT_
+00003a20: 3455 000f 0046 696c 6520 6368 6563 6b73  4U...File checks
+00003a30: 756d 2e00 16df ff60 2e00 0000 0000 0000  um.....`........
+00003a40: 0106 0000 0000 0100 0000 663a 0000 0000  ..........f:....
+00003a50: 0000 d603 0000 0000 0000 bac1 b663 32ac  .............c2.
+00003a60: b4b1 95fc 6c9c                           ....l.
```

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/llhoft/omegascan/scanme.gwf` & `gwcelery-2.1.2/gwcelery/tests/data/llhoft/omegascan/scanme.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.2/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files 3% similar despite different names*

```diff
@@ -146,22 +146,22 @@
 00000910: 2066 6f72 2074 6865 2066 6972 7374 2061   for the first a
 00000920: 7578 696c 6961 7279 2074 6162 6c65 2064  uxiliary table d
 00000930: 6174 6100 209f 3edd 3600 0000 0000 0000  ata. .>.6.......
 00000940: 0102 1500 0000 0700 6368 6b53 756d 0007  ........chkSum..
 00000950: 0049 4e54 5f34 5500 1000 5374 7275 6374  .INT_4U...Struct
 00000960: 2063 6865 636b 7375 6d00 bccb b902 8500   checksum.......
 00000970: 0000 0000 0000 0103 0000 0000 0500 6777  ..............gw
-00000980: 7079 0000 0000 002c 203c 5469 6d65 53b8  py....., <TimeS.
+00000980: 7079 0000 0000 0000 0000 0000 0000 00b8  py..............
 00000990: 8183 4800 0000 0025 0000 0000 0000 0010  ..H....%........
 000009a0: 4000 0000 0000 0000 0000 0000 0000 0000  @...............
 000009b0: 0000 0005 0000 0000 0000 0000 0000 0000  ................
 000009c0: 0000 0000 000b 0000 0000 0000 0000 0000  ................
 000009d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000009e0: 0000 0000 0000 0000 0000 0000 0000 00be  ................
-000009f0: 448c 8c3b 0000 0000 0000 0001 0101 0000  D..;............
+000009e0: 0000 0000 0000 0000 0000 0000 0000 0047  ...............G
+000009f0: 6661 b63b 0000 0000 0000 0001 0101 0000  fa.;............
 00000a00: 000b 0046 7244 6574 6563 746f 7200 0500  ...FrDetector...
 00000a10: 1800 4465 7465 6374 6f72 2044 6174 6120  ..Detector Data 
 00000a20: 5374 7275 6374 7572 6500 94bd 3e10 2500  Structure...>.%.
 00000a30: 0000 0000 0000 0102 1600 0000 0500 6e61  ..............na
 00000a40: 6d65 0007 0053 5452 494e 4700 0100 006c  me...STRING....l
 00000a50: ebf8 8528 0000 0000 0000 0001 0217 0000  ...(............
 00000a60: 0007 0070 7265 6669 7800 0800 4348 4152  ...prefix...CHAR
@@ -421,495 +421,514 @@
 00001a40: 0048 313a 4944 512d 4641 505f 4f56 4c5f  .H1:IDQ-FAP_OVL_
 00001a50: 3332 5f32 3034 3800 1700 4831 3a49 4451  32_2048...H1:IDQ
 00001a60: 2d46 4150 5f4f 564c 5f33 325f 3230 3438  -FAP_OVL_32_2048
 00001a70: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00001a80: 0000 0010 4000 0000 0000 0000 0000 0000  ....@...........
 00001a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001aa0: 0000 0014 0002 0000 0000 0000 0000 0000  ................
-00001ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ac0: 00f7 1d25 038f 0000 0000 0000 0001 1402  ...%............
+00001ab0: 0000 0000 0000 0000 0000 000b 0003 0000  ................
+00001ac0: 00b5 76f2 7a8f 0000 0000 0000 0001 1402  ..v.z...........
 00001ad0: 0000 0017 0048 313a 4944 512d 4641 505f  .....H1:IDQ-FAP_
 00001ae0: 4f56 4c5f 3332 5f32 3034 3800 0101 0500  OVL_32_2048.....
 00001af0: 0004 0000 0000 0000 2700 0000 0000 0000  ........'.......
 00001b00: 789c edc5 310d 0000 0c03 a0d5 bfe9 1d55  x...1..........U
 00001b10: d104 1e72 15db b66d dbb6 6ddb b66d dbb6  ...r...m..m..m..
 00001b20: 3dfb 0333 c004 0101 0000 0000 0400 0000  =..3............
 00001b30: 0000 0000 0000 0000 0070 3f00 0000 0000  .........p?.....
 00001b40: 0000 0002 0073 0001 0000 0000 0000 0000  .....s..........
-00001b50: aeb3 7f50 4100 0000 0000 0000 0101 0400  ...PA...........
-00001b60: 0000 0d00 4672 456e 644f 6646 7261 6d65  ....FrEndOfFrame
-00001b70: 0007 001c 0045 6e64 206f 6620 4672 616d  .....End of Fram
-00001b80: 6520 4461 7461 2053 7472 7563 7475 7265  e Data Structure
-00001b90: 009c ab33 e258 0000 0000 0000 0001 0247  ...3.X.........G
-00001ba0: 0000 0004 0072 756e 0007 0049 4e54 5f34  .....run...INT_4
-00001bb0: 5300 3500 5275 6e20 6e75 6d62 6572 3b20  S.5.Run number; 
-00001bc0: 7361 6d65 2061 7320 696e 2046 7261 6d65  same as in Frame
-00001bd0: 4865 6164 6572 2072 756e 206e 756d 6265  Header run numbe
-00001be0: 7220 6461 7475 6d2e 000b 9641 5b87 0000  r datum....A[...
-00001bf0: 0000 0000 0001 0248 0000 0006 0066 7261  .......H.....fra
-00001c00: 6d65 0007 0049 4e54 5f34 5500 6200 4672  me...INT_4U.b.Fr
-00001c10: 616d 6520 6e75 6d62 6572 2c20 6d6f 6e6f  ame number, mono
-00001c20: 746f 6e69 6361 6c6c 7920 696e 6372 6561  tonically increa
-00001c30: 7369 6e67 2075 6e74 696c 2065 6e64 206f  sing until end o
-00001c40: 6620 7275 6e3b 2073 616d 6520 6173 2069  f run; same as i
-00001c50: 6e20 4672 616d 6520 4865 6164 6572 2072  n Frame Header r
-00001c60: 756e 206e 756d 6265 7220 6461 7475 6d00  un number datum.
-00001c70: ba5a b3d1 4700 0000 0000 0000 0102 4900  .Z..G.........I.
-00001c80: 0000 0700 4754 696d 6553 0007 0049 4e54  ....GTimeS...INT
-00001c90: 5f34 5500 2100 4672 616d 6520 7374 6172  _4U.!.Frame star
-00001ca0: 7420 7469 6d65 2069 6e20 4750 5320 5365  t time in GPS Se
-00001cb0: 636f 6e64 732e 0018 add0 ff56 0000 0000  conds......V....
-00001cc0: 0000 0001 024a 0000 0007 0047 5469 6d65  .....J.....GTime
-00001cd0: 4e00 0700 494e 545f 3455 0030 0046 7261  N...INT_4U.0.Fra
-00001ce0: 6d65 2073 7461 7274 2074 696d 6520 7265  me start time re
-00001cf0: 7369 6475 616c 2c20 696e 7465 6765 7220  sidual, integer 
-00001d00: 6e61 6e6f 7365 636f 6e64 732e 0064 338f  nanoseconds..d3.
-00001d10: ba36 0000 0000 0000 0001 024b 0000 0007  .6.........K....
-00001d20: 0063 686b 5375 6d00 0700 494e 545f 3455  .chkSum...INT_4U
-00001d30: 0010 0053 7472 7563 7420 6368 6563 6b73  ...Struct checks
-00001d40: 756d 0022 ca11 6222 0000 0000 0000 0001  um."..b"........
-00001d50: 0700 0000 0000 0000 002c 203c 5400 0000  ........., <T...
-00001d60: 0000 0000 00b4 e395 1b37 0000 0000 0000  .........7......
-00001d70: 0001 0100 0000 0006 0046 7254 4f43 0013  .........FrTOC..
-00001d80: 0019 0053 696d 756c 6174 6564 2044 6174  ...Simulated Dat
-00001d90: 6120 5374 7275 6374 7572 6500 7c69 656b  a Structure.|iek
-00001da0: 4800 0000 0000 0000 0102 0000 0000 0700  H...............
-00001db0: 554c 6561 7053 0007 0049 4e54 5f32 5300  ULeapS...INT_2S.
-00001dc0: 2200 4672 6f6d 2074 6865 2066 6972 7374  ".From the first
-00001dd0: 2046 7261 6d65 4820 696e 2074 6865 2066   FrameH in the f
-00001de0: 696c 6500 0087 5256 4300 0000 0000 0000  ile...RVC.......
-00001df0: 0102 0100 0000 0700 6e46 7261 6d65 0007  ........nFrame..
-00001e00: 0049 4e54 5f34 5500 1d00 4e75 6d62 6572  .INT_4U...Number
-00001e10: 206f 6620 6672 616d 6573 2069 6e20 7468   of frames in th
-00001e20: 6520 6669 6c65 00cc 3d5f 7370 0000 0000  e file..=_sp....
-00001e30: 0000 0001 0202 0000 000c 0064 6174 6151  ...........dataQ
-00001e40: 7561 6c69 7479 000f 0049 4e54 5f34 555b  uality...INT_4U[
-00001e50: 6e46 7261 6d65 5d00 3d00 4172 7261 7920  nFrame].=.Array 
-00001e60: 6f66 2069 6e74 6567 6572 2051 4120 776f  of integer QA wo
-00001e70: 7264 7320 6672 6f6d 2065 6163 6820 4672  rds from each Fr
-00001e80: 616d 6548 2028 7369 7a65 206f 6620 6e46  ameH (size of nF
-00001e90: 7261 6d65 7329 0088 6738 c05f 0000 0000  rames)..g8._....
-00001ea0: 0000 0001 0203 0000 0007 0047 5469 6d65  ...........GTime
-00001eb0: 5300 0f00 494e 545f 3455 5b6e 4672 616d  S...INT_4U[nFram
-00001ec0: 655d 0031 0041 7272 6179 206f 6620 696e  e].1.Array of in
-00001ed0: 7465 6765 7220 4750 5320 6672 6165 2074  teger GPS frae t
-00001ee0: 696d 6573 2028 7369 7a65 206f 6620 6e46  imes (size of nF
-00001ef0: 7261 6d65 7300 d5b2 6755 7600 0000 0000  rames...gUv.....
-00001f00: 0000 0102 0400 0000 0700 4754 696d 654e  ..........GTimeN
-00001f10: 000f 0049 4e54 5f34 555b 6e46 7261 6d65  ...INT_4U[nFrame
-00001f20: 5d00 4800 4172 7261 7920 6f66 2069 6e74  ].H.Array of int
-00001f30: 6567 6572 2047 5053 2072 6573 6964 7561  eger GPS residua
-00001f40: 6c20 6e61 6e6f 7365 636f 6e64 7320 666f  l nanoseconds fo
-00001f50: 7220 7468 6520 6672 616d 6520 2873 697a  r the frame (siz
-00001f60: 6520 6f66 206e 4672 616d 6500 154d fabb  e of nFrame..M..
-00001f70: 6000 0000 0000 0000 0102 0500 0000 0300  `...............
-00001f80: 6474 000f 0052 4541 4c5f 385b 6e46 7261  dt...REAL_8[nFra
-00001f90: 6d65 5d00 3600 4172 7261 7920 6f66 2066  me].6.Array of f
-00001fa0: 7261 6d65 2064 7572 6174 696f 6e73 2069  rame durations i
-00001fb0: 6e20 7365 636f 6e64 7328 2073 697a 6520  n seconds( size 
-00001fc0: 6f66 206e 4672 616d 6573 2900 0d06 b877  of nFrames)....w
-00001fd0: 5200 0000 0000 0000 0102 0600 0000 0500  R...............
-00001fe0: 7275 6e73 000f 0049 4e54 5f34 535b 6e46  runs...INT_4S[nF
-00001ff0: 7261 6d65 5d00 2600 4172 7261 7920 6f66  rame].&.Array of
-00002000: 2072 756e 206e 756d 6265 7273 2028 7369   run numbers (si
-00002010: 7a65 206f 6620 6e46 7261 6d65 2900 ca0b  ze of nFrame)...
-00002020: 9f5c 5500 0000 0000 0000 0102 0700 0000  .\U.............
-00002030: 0600 6672 616d 6500 0f00 494e 545f 3455  ..frame...INT_4U
-00002040: 5b6e 4672 616d 655d 0028 0041 7272 6179  [nFrame].(.Array
-00002050: 206f 6620 6672 616d 6520 6e75 6d62 6572   of frame number
-00002060: 7320 2873 697a 6520 6f66 206e 4672 616d  s (size of nFram
-00002070: 6529 0031 285d 2581 0000 0000 0000 0001  e).1(]%.........
-00002080: 0208 0000 000a 0070 6f73 6974 696f 6e48  .......positionH
-00002090: 000f 0049 4e54 5f38 555b 6e46 7261 6d65  ...INT_8U[nFrame
-000020a0: 5d00 5000 4172 7261 7920 6f66 2046 7261  ].P.Array of Fra
-000020b0: 6d65 4820 706f 7369 7469 6f6e 732c 2069  meH positions, i
-000020c0: 6e20 6279 7465 732c 2066 726f 6d20 7468  n bytes, from th
-000020d0: 6520 6267 696e 6e69 6e67 206f 6620 6669  e bginning of fi
-000020e0: 6c65 2028 7369 7a65 206f 6620 6e46 7261  le (size of nFra
-000020f0: 6d65 2900 db18 22e8 8700 0000 0000 0000  me)...".........
-00002100: 0102 0900 0000 0a00 6e46 6972 7374 4144  ........nFirstAD
-00002110: 4300 0f00 494e 545f 3855 5b6e 4672 616d  C...INT_8U[nFram
-00002120: 655d 0056 0041 7272 6179 206f 6620 6669  e].V.Array of fi
-00002130: 7273 7420 4672 4144 4344 6174 6120 706f  rst FrADCData po
-00002140: 7369 7469 6f6e 732c 2069 6e20 6279 7465  sitions, in byte
-00002150: 732c 2066 726f 6d20 6265 6769 6e6e 696e  s, from beginnin
-00002160: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
-00002170: 6f66 206e 4672 616d 6529 00b7 d5cd 8b86  of nFrame)......
-00002180: 0000 0000 0000 0001 020a 0000 000a 006e  ...............n
-00002190: 4669 7273 7453 6572 000f 0049 4e54 5f38  FirstSer...INT_8
-000021a0: 555b 6e46 7261 6d65 5d00 5500 4172 7261  U[nFrame].U.Arra
-000021b0: 7920 6f66 2066 6972 7374 2046 7253 6572  y of first FrSer
-000021c0: 4461 7461 2070 6f73 6974 696f 6e73 2069  Data positions i
-000021d0: 6e20 6279 7465 732c 2066 726f 6d20 6265  n bytes, from be
-000021e0: 6769 6e6e 696e 6720 6f66 2066 696c 6520  ginning of file 
-000021f0: 2873 697a 6520 6f66 206e 4672 616d 6529  (size of nFrame)
-00002200: 00fa c761 6b87 0000 0000 0000 0001 020b  ...ak...........
-00002210: 0000 000c 006e 4669 7273 7454 6162 6c65  .....nFirstTable
-00002220: 000f 0049 4e54 5f38 555b 6e46 7261 6d65  ...INT_8U[nFrame
-00002230: 5d00 5400 4172 7261 7920 6f66 2066 6972  ].T.Array of fir
-00002240: 7374 2046 7254 6162 6c65 2070 6f73 6974  st FrTable posit
-00002250: 696f 6e73 2c20 696e 2062 7974 6573 2c20  ions, in bytes, 
-00002260: 6672 6f6d 2062 6567 696e 6e69 6e67 206f  from beginning o
-00002270: 6620 6669 6c65 2028 7369 7a65 206f 6620  f file (size of 
-00002280: 6e46 7261 6d65 2900 1016 52a6 8300 0000  nFrame)...R.....
-00002290: 0000 0000 0102 0c00 0000 0a00 6e46 6972  ............nFir
-000022a0: 7374 4d73 6700 0f00 494e 545f 3855 5b6e  stMsg...INT_8U[n
-000022b0: 4672 616d 655d 0052 0041 7272 6179 206f  Frame].R.Array o
-000022c0: 6620 6669 7273 7420 4672 4d73 6720 706f  f first FrMsg po
-000022d0: 7369 7469 6f6e 732c 2069 6e20 6279 7465  sitions, in byte
-000022e0: 732c 2066 726f 6d20 6265 6769 6e6e 696e  s, from beginnin
-000022f0: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
-00002300: 6f66 206e 4672 616d 6529 00b9 e1c6 f949  of nFrame).....I
-00002310: 0000 0000 0000 0001 020d 0000 0004 006e  ...............n
-00002320: 5348 0007 0049 4e54 5f34 5500 2600 4e75  SH...INT_4U.&.Nu
-00002330: 6d62 6572 206f 6620 4672 5348 2073 7472  mber of FrSH str
-00002340: 7563 7475 7265 7320 696e 2074 6865 2066  uctures in the f
-00002350: 696c 6500 f46c 0bb0 4900 0000 0000 0000  ile..l..I.......
-00002360: 0102 0e00 0000 0500 5348 6964 000c 0049  ........SHid...I
-00002370: 4e54 5f32 555b 6e53 485d 0020 0041 7272  NT_2U[nSH]. .Arr
-00002380: 6179 206f 6620 4672 5348 2049 4473 2028  ay of FrSH IDs (
-00002390: 7369 7a65 206f 6620 6e53 4829 0010 5b23  size of nSH)..[#
-000023a0: 074d 0000 0000 0000 0001 020f 0000 0007  .M..............
-000023b0: 0053 486e 616d 6500 0c00 5354 5249 4e47  .SHname...STRING
-000023c0: 5b6e 5348 5d00 2200 4172 7261 7920 6f66  [nSH].".Array of
-000023d0: 2046 7253 4820 6e61 6d65 7320 2873 697a   FrSH names (siz
-000023e0: 6520 6f66 206e 5348 2900 a664 b4df 5c00  e of nSH)..d..\.
-000023f0: 0000 0000 0000 0102 1000 0000 0a00 6e44  ..............nD
-00002400: 6574 6563 746f 7200 0700 494e 545f 3455  etector...INT_4U
-00002410: 0033 004e 756d 6265 7220 6f66 2064 6973  .3.Number of dis
-00002420: 7469 6e63 7420 7479 7065 7320 6f66 2046  tinct types of F
-00002430: 7244 6574 6563 746f 7220 696e 2074 6865  rDetector in the
-00002440: 2066 696c 6500 fa46 0067 8100 0000 0000   file..F.g......
-00002450: 0000 0102 1100 0000 0d00 6e61 6d65 4465  ..........nameDe
-00002460: 7465 6374 6f72 0012 0053 5452 494e 475b  tector...STRING[
-00002470: 6e44 6574 6563 746f 725d 004a 0041 7272  nDetector].J.Arr
-00002480: 6179 206f 6620 4672 4465 7465 6374 6f72  ay of FrDetector
-00002490: 206e 616d 6573 2028 7369 7a65 206f 6620   names (size of 
-000024a0: 6e44 6574 6563 746f 7229 2e20 5468 6579  nDetector). They
-000024b0: 2061 7070 6561 7220 616c 7068 6162 6574   appear alphabet
-000024c0: 6963 616c 6c79 0011 11d2 a589 0000 0000  ically..........
-000024d0: 0000 0001 0212 0000 0011 0070 6f73 6974  ...........posit
-000024e0: 696f 6e44 6574 6563 746f 7200 1200 494e  ionDetector...IN
-000024f0: 545f 3855 5b6e 4465 7465 6374 6f72 5d00  T_8U[nDetector].
-00002500: 4e00 4172 7261 7920 6f66 2046 7244 6574  N.Array of FrDet
-00002510: 6563 746f 7220 706f 7369 7469 6f6e 7320  ector positions 
-00002520: 6672 6f6d 2074 6865 2062 6567 696e 6e69  from the beginni
-00002530: 6e67 206f 6620 6669 6c65 2028 7369 7a65  ng of file (size
-00002540: 206f 6620 6e44 6574 6563 746f 7229 2e00   of nDetector)..
-00002550: 8345 9ff0 5800 0000 0000 0000 0102 1300  .E..X...........
-00002560: 0000 0a00 6e53 7461 7454 7970 6500 0700  ....nStatType...
-00002570: 494e 545f 3455 002f 004e 756d 6265 7220  INT_4U./.Number 
-00002580: 6f66 2073 7461 7469 6320 6461 7461 2062  of static data b
-00002590: 6c6f 636b 2074 7970 6573 2069 6e20 7468  lock types in th
-000025a0: 6520 6669 6c65 2e00 0f05 6246 6000 0000  e file....bF`...
-000025b0: 0000 0000 0102 1400 0000 0900 6e61 6d65  ............name
-000025c0: 5374 6174 0012 0053 5452 494e 475b 6e53  Stat...STRING[nS
-000025d0: 7461 7454 7970 655d 002d 0041 7272 6179  tatType].-.Array
-000025e0: 206f 6620 4672 5374 6174 4461 7461 206e   of FrStatData n
-000025f0: 616d 6520 2873 697a 6520 6f66 206e 5374  ame (size of nSt
-00002600: 6174 5479 7065 2900 a3bf 4547 5d00 0000  atType)...EG]...
-00002610: 0000 0000 0102 1500 0000 0900 6465 7465  ............dete
-00002620: 6374 6f72 0012 0053 5452 494e 475b 6e53  ctor...STRING[nS
-00002630: 7461 7454 7970 655d 002a 0041 7272 6179  tatType].*.Array
-00002640: 206f 6620 4465 7465 6374 6f72 206e 616d   of Detector nam
-00002650: 6528 7369 7a65 206f 6620 6e53 7461 7454  e(size of nStatT
-00002660: 7970 6529 0041 b642 9d7b 0000 0000 0000  ype).A.B.{......
-00002670: 0001 0216 0000 000e 006e 5374 6174 496e  .........nStatIn
-00002680: 7374 616e 6365 0012 0049 4e54 5f34 555b  stance...INT_4U[
-00002690: 6e53 7461 7454 7970 655d 0043 0041 7272  nStatType].C.Arr
-000026a0: 6179 206f 6620 6e75 6d62 6572 206f 6620  ay of number of 
-000026b0: 696e 7374 616e 6365 2066 6f72 2065 6163  instance for eac
-000026c0: 6820 4672 5374 6174 4461 7461 2873 697a  h FrStatData(siz
-000026d0: 6520 6f66 206e 5374 6174 5479 7065 2900  e of nStatType).
-000026e0: 66b8 774f 4b00 0000 0000 0000 0102 1700  f.wOK...........
-000026f0: 0000 0b00 6e54 6f74 616c 5374 6174 0007  ....nTotalStat..
-00002700: 0049 4e54 5f34 5500 2100 5375 6d6d 6174  .INT_4U.!.Summat
-00002710: 696f 6e20 6f66 206e 5374 6174 496e 7374  ion of nStatInst
-00002720: 616e 6365 2061 7272 6179 0089 b4e7 f874  ance array.....t
-00002730: 0000 0000 0000 0001 0218 0000 0007 0074  ...............t
-00002740: 5374 6172 7400 1300 494e 545f 3455 5b6e  Start...INT_4U[n
-00002750: 546f 7461 6c53 7461 745d 0042 0041 7272  TotalStat].B.Arr
-00002760: 6179 206f 6620 4750 5320 696e 7465 6765  ay of GPS intege
-00002770: 7220 7374 6172 7420 7469 6d65 732c 2069  r start times, i
-00002780: 6e20 7365 636f 6e64 7320 2873 697a 6520  n seconds (size 
-00002790: 6f66 206e 546f 7461 6c53 7461 7429 001a  of nTotalStat)..
-000027a0: 531d 0970 0000 0000 0000 0001 0219 0000  S..p............
-000027b0: 0005 0074 456e 6400 1300 494e 545f 3455  ...tEnd...INT_4U
-000027c0: 5b6e 546f 7461 6c53 7461 745d 0040 0041  [nTotalStat].@.A
-000027d0: 7272 6179 206f 6620 4750 5320 696e 7465  rray of GPS inte
-000027e0: 6765 7220 656e 6420 7469 6d65 732c 2069  ger end times, i
-000027f0: 6e20 7365 636f 6e64 7320 2873 697a 6520  n seconds (size 
-00002800: 6f66 206e 546f 7461 6c53 7461 7429 0045  of nTotalStat).E
-00002810: 668b 4d5e 0000 0000 0000 0001 021a 0000  f.M^............
-00002820: 0008 0076 6572 7369 6f6e 0013 0049 4e54  ...version...INT
-00002830: 5f34 555b 6e54 6f74 616c 5374 6174 5d00  _4U[nTotalStat].
-00002840: 2b00 4172 7261 7920 6f66 2076 6572 7369  +.Array of versi
-00002850: 6f6e 2074 696d 6520 2873 697a 6520 6f66  on time (size of
-00002860: 206e 546f 7461 6c53 7461 7429 0093 e259   nTotalStat)...Y
-00002870: 1d82 0000 0000 0000 0001 021b 0000 000d  ................
-00002880: 0070 6f73 6974 696f 6e53 7461 7400 1300  .positionStat...
-00002890: 494e 545f 3855 5b6e 546f 7461 6c53 7461  INT_8U[nTotalSta
-000028a0: 745d 004a 0041 7272 6179 206f 6620 4672  t].J.Array of Fr
-000028b0: 5374 6174 4461 7461 2070 6f73 6974 696f  StatData positio
-000028c0: 6e73 2066 726f 6d20 6265 6769 6e6e 696e  ns from beginnin
-000028d0: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
-000028e0: 6f66 206e 546f 7461 6c53 7461 7429 002e  of nTotalStat)..
-000028f0: 51de 564e 0000 0000 0000 0001 021c 0000  Q.VN............
-00002900: 0005 006e 4144 4300 0700 494e 545f 3455  ...nADC...INT_4U
-00002910: 002a 004e 756d 6265 7220 6f66 2075 6e69  .*.Number of uni
-00002920: 7175 6520 4672 4164 6344 6174 6120 6e61  que FrAdcData na
-00002930: 6d65 7320 696e 2066 696c 652e 0007 54ee  mes in file...T.
-00002940: e143 0000 0000 0000 0001 021d 0000 0005  .C..............
-00002950: 006e 616d 6500 0d00 5354 5249 4e47 5b6e  .name...STRING[n
-00002960: 4144 435d 0019 0041 7272 6179 206f 6620  ADC]...Array of 
-00002970: 4672 4164 6344 6174 6120 6e61 6d65 7300  FrAdcData names.
-00002980: 89b1 c3ad 4800 0000 0000 0000 0102 1e00  ....H...........
-00002990: 0000 0a00 6368 616e 6e65 6c49 4400 0d00  ....channelID...
-000029a0: 494e 545f 3455 5b6e 4144 435d 0019 0041  INT_4U[nADC]...A
-000029b0: 7272 6179 206f 6620 4144 4320 6368 616e  rray of ADC chan
-000029c0: 6e65 6c20 4944 7300 251b 8f78 4400 0000  nel IDs.%..xD...
-000029d0: 0000 0000 0102 1f00 0000 0800 6772 6f75  ............grou
-000029e0: 7049 4400 0d00 494e 545f 3455 5b6e 4144  pID...INT_4U[nAD
-000029f0: 435d 0017 0041 7272 6179 206f 6620 4144  C]...Array of AD
-00002a00: 4320 6772 6f75 7020 4944 7300 ec33 7c9e  C group IDs..3|.
-00002a10: 9e00 0000 0000 0000 0102 2000 0000 0c00  .......... .....
-00002a20: 706f 7369 7469 6f6e 4144 4300 1500 494e  positionADC...IN
-00002a30: 545f 3855 5b6e 4144 435d 5b6e 4672 616d  T_8U[nADC][nFram
-00002a40: 655d 0065 0041 7272 6179 206f 6620 6c69  e].e.Array of li
-00002a50: 7374 7320 6f66 2046 7241 6463 4461 7461  sts of FrAdcData
-00002a60: 206f 6666 7365 7420 706f 7369 7469 6f6e   offset position
-00002a70: 732c 2069 6e20 6279 7465 732c 2066 726f  s, in bytes, fro
-00002a80: 6d20 6265 6769 6e6e 696e 6720 6f66 2066  m beginning of f
-00002a90: 696c 6520 2873 697a 6520 6f66 206e 4672  ile (size of nFr
-00002aa0: 616d 652a 6e41 4443 2900 6d54 ccf2 5000  ame*nADC).mT..P.
-00002ab0: 0000 0000 0000 0102 2100 0000 0600 6e50  ........!.....nP
-00002ac0: 726f 6300 0700 494e 545f 3455 002b 004e  roc...INT_4U.+.N
-00002ad0: 756d 6265 7220 6f66 2075 6e69 7175 6520  umber of unique 
-00002ae0: 4672 5072 6f63 4461 7461 206e 616d 6573  FrProcData names
-00002af0: 2069 6e20 6669 6c65 2e00 feef 7499 4900   in file....t.I.
-00002b00: 0000 0000 0000 0102 2200 0000 0900 6e61  ........".....na
-00002b10: 6d65 5072 6f63 000e 0053 5452 494e 475b  meProc...STRING[
-00002b20: 6e50 726f 635d 001a 0041 7272 6179 206f  nProc]...Array o
-00002b30: 6620 4672 5072 6f63 4461 7461 206e 616d  f FrProcData nam
-00002b40: 6573 0092 f0ec 64a2 0000 0000 0000 0001  es....d.........
-00002b50: 0223 0000 000d 0070 6f73 6974 696f 6e50  .#.....positionP
-00002b60: 726f 6300 1600 494e 545f 3855 5b6e 5072  roc...INT_8U[nPr
-00002b70: 6f63 5d5b 6e46 7261 6d65 5d00 6700 4172  oc][nFrame].g.Ar
-00002b80: 7261 7920 6f66 206c 6973 7473 206f 6620  ray of lists of 
-00002b90: 4672 5072 6f63 4461 7461 206f 6666 7365  FrProcData offse
-00002ba0: 7420 706f 7369 7469 6f6e 732c 2069 6e20  t positions, in 
-00002bb0: 6279 7465 732c 2066 726f 6d20 6265 6769  bytes, from begi
-00002bc0: 6e6e 696e 6720 6f66 2066 696c 6520 2873  nning of file (s
-00002bd0: 697a 6520 6f66 206e 4672 616d 652a 6e50  ize of nFrame*nP
-00002be0: 726f 6329 00f2 b9e4 a64e 0000 0000 0000  roc).....N......
-00002bf0: 0001 0224 0000 0005 006e 5369 6d00 0700  ...$.....nSim...
-00002c00: 494e 545f 3455 002a 004e 756d 6265 7220  INT_4U.*.Number 
-00002c10: 6f66 2075 6e69 7175 6520 4672 5369 6d44  of unique FrSimD
-00002c20: 6174 6120 6e61 6d65 7320 696e 2066 696c  ata names in fil
-00002c30: 652e 0008 01bc 3746 0000 0000 0000 0001  e.....7F........
-00002c40: 0225 0000 0008 006e 616d 6553 696d 000d  .%.....nameSim..
-00002c50: 0053 5452 494e 475b 6e53 696d 5d00 1900  .STRING[nSim]...
-00002c60: 4172 7261 7920 6f66 2046 7253 696d 4461  Array of FrSimDa
-00002c70: 7461 206e 616d 6573 00c4 a72b f69e 0000  ta names...+....
-00002c80: 0000 0000 0001 0226 0000 000c 0070 6f73  .......&.....pos
-00002c90: 6974 696f 6e53 696d 0015 0049 4e54 5f38  itionSim...INT_8
-00002ca0: 555b 6e53 696d 5d5b 6e46 7261 6d65 5d00  U[nSim][nFrame].
-00002cb0: 6500 4172 7261 7920 6f66 206c 6973 7473  e.Array of lists
-00002cc0: 206f 6620 4672 5369 6d44 6174 6120 6f66   of FrSimData of
-00002cd0: 6673 6574 2070 6f73 6974 696f 6e73 2c20  fset positions, 
-00002ce0: 696e 2062 7974 6573 2c20 6672 6f6d 2062  in bytes, from b
-00002cf0: 6567 696e 6e69 6e67 206f 6620 6669 6c65  eginning of file
-00002d00: 2028 7369 7a65 206f 6620 6e46 7261 6d65   (size of nFrame
-00002d10: 2a6e 5369 6d29 00d3 40ba c14e 0000 0000  *nSim)..@..N....
-00002d20: 0000 0001 0227 0000 0005 006e 5365 7200  .....'.....nSer.
-00002d30: 0700 494e 545f 3455 002a 004e 756d 6265  ..INT_4U.*.Numbe
-00002d40: 7220 6f66 2075 6e69 7175 6520 4672 5365  r of unique FrSe
-00002d50: 7244 6174 6120 6e61 6d65 7320 696e 2066  rData names in f
-00002d60: 696c 652e 000f 814d 9046 0000 0000 0000  ile....M.F......
-00002d70: 0001 0228 0000 0008 006e 616d 6553 6572  ...(.....nameSer
-00002d80: 000d 0053 5452 494e 475b 6e53 6572 5d00  ...STRING[nSer].
-00002d90: 1900 4172 7261 7920 6f66 2046 7253 6572  ..Array of FrSer
-00002da0: 4461 7461 206e 616d 6573 00bd 2d79 109e  Data names..-y..
-00002db0: 0000 0000 0000 0001 0229 0000 000c 0070  .........).....p
-00002dc0: 6f73 6974 696f 6e53 6572 0015 0049 4e54  ositionSer...INT
-00002dd0: 5f38 555b 6e53 6572 5d5b 6e46 7261 6d65  _8U[nSer][nFrame
-00002de0: 5d00 6500 4172 7261 7920 6f66 206c 6973  ].e.Array of lis
-00002df0: 7473 206f 6620 4672 5365 7244 6174 6120  ts of FrSerData 
-00002e00: 6f66 6673 6574 2070 6f73 6974 696f 6e73  offset positions
-00002e10: 2c20 696e 2062 7974 6573 2c20 6672 6f6d  , in bytes, from
-00002e20: 2062 6567 696e 6e69 6e67 206f 6620 6669   beginning of fi
-00002e30: 6c65 2028 7369 7a65 206f 6620 6e46 7261  le (size of nFra
-00002e40: 6d65 2a6e 5365 7229 001c 5003 fb52 0000  me*nSer)..P..R..
-00002e50: 0000 0000 0001 022a 0000 0009 006e 5375  .......*.....nSu
-00002e60: 6d6d 6172 7900 0700 494e 545f 3455 002a  mmary...INT_4U.*
-00002e70: 004e 756d 6265 7220 6f66 2075 6e69 7175  .Number of uniqu
-00002e80: 6520 4672 5375 6d6d 6172 7920 6e61 6d65  e FrSummary name
-00002e90: 7320 696e 2066 696c 652e 0034 77a5 e94b  s in file..4w..K
-00002ea0: 0000 0000 0000 0001 022b 0000 0009 006e  .........+.....n
-00002eb0: 616d 6553 5375 6d00 1100 5354 5249 4e47  ameSSum...STRING
-00002ec0: 5b6e 5375 6d6d 6172 795d 0019 0041 7272  [nSummary]...Arr
-00002ed0: 6179 206f 6620 4672 5375 6d6d 6172 7920  ay of FrSummary 
-00002ee0: 6e61 6d65 7300 0684 574e a200 0000 0000  names...WN......
-00002ef0: 0000 0102 2c00 0000 0c00 706f 7369 7469  ....,.....positi
-00002f00: 6f6e 5365 7200 1900 494e 545f 3855 5b6e  onSer...INT_8U[n
-00002f10: 5375 6d6d 6172 795d 5b6e 4672 616d 655d  Summary][nFrame]
-00002f20: 0065 0041 7272 6179 206f 6620 6c69 7374  .e.Array of list
-00002f30: 7320 6f66 2046 7253 756d 6d61 7279 206f  s of FrSummary o
-00002f40: 6666 7365 7420 706f 7369 7469 6f6e 732c  ffset positions,
-00002f50: 2069 6e20 6279 7465 732c 2066 726f 6d20   in bytes, from 
-00002f60: 6265 6769 6e6e 696e 6720 6f66 2066 696c  beginning of fil
-00002f70: 6520 2873 697a 6520 6f66 206e 4672 616d  e (size of nFram
-00002f80: 652a 6e53 6572 2900 c376 da95 4800 0000  e*nSer)..v..H...
-00002f90: 0000 0000 0102 2d00 0000 0b00 6e45 7665  ......-.....nEve
-00002fa0: 6e74 5479 7065 0007 0049 4e54 5f34 5500  ntType...INT_4U.
-00002fb0: 1e00 4e75 6d62 6572 206f 6620 4672 4576  ..Number of FrEv
-00002fc0: 656e 7420 696e 2074 6865 2066 696c 6500  ent in the file.
-00002fd0: cb0b 34f7 4c00 0000 0000 0000 0102 2e00  ..4.L...........
-00002fe0: 0000 0a00 6e61 6d65 4576 656e 7400 1300  ....nameEvent...
-00002ff0: 5354 5249 4e47 5b6e 4576 656e 7454 7970  STRING[nEventTyp
-00003000: 655d 0017 0041 7272 6179 206f 6620 4672  e]...Array of Fr
-00003010: 4576 656e 7420 6e61 6d65 7300 8aec 7442  Event names...tB
-00003020: 7200 0000 0000 0000 0102 2f00 0000 0700  r........./.....
-00003030: 6e45 7665 6e74 0013 0049 4e54 5f34 555b  nEvent...INT_4U[
-00003040: 6e45 7665 6e74 5479 7065 5d00 4000 4e75  nEventType].@.Nu
-00003050: 6d62 6572 206f 6620 4672 4576 656e 7420  mber of FrEvent 
-00003060: 666f 7220 6561 6368 2074 7970 6520 6f66  for each type of
-00003070: 2046 7245 7665 6e74 2028 7369 7a65 206f   FrEvent (size o
-00003080: 6620 6e45 7665 6e74 5479 7065 2900 aebb  f nEventType)...
-00003090: 6fd3 4300 0000 0000 0000 0102 3000 0000  o.C.........0...
-000030a0: 0c00 6e54 6f74 616c 4576 656e 7400 0700  ..nTotalEvent...
-000030b0: 494e 545f 3455 0018 0054 6f74 616c 206e  INT_4U...Total n
-000030c0: 756d 6265 7220 6f66 2046 7245 7665 6e74  umber of FrEvent
-000030d0: 0074 8af4 4a54 0000 0000 0000 0001 0231  .t..JT.........1
-000030e0: 0000 000c 0047 5469 6d65 5345 7665 6e74  .....GTimeSEvent
-000030f0: 0014 0049 4e54 5f34 555b 6e54 6f74 616c  ...INT_4U[nTotal
-00003100: 4576 656e 745d 001c 0047 5053 2074 696d  Event]...GPS tim
-00003110: 6520 696e 2069 6e74 6567 6572 2073 6563  e in integer sec
-00003120: 6f6e 6473 0015 3513 2961 0000 0000 0000  onds..5.)a......
-00003130: 0001 0232 0000 000c 0047 5469 6d65 4e45  ...2.....GTimeNE
-00003140: 7665 6e74 0014 0049 4e54 5f34 555b 6e54  vent...INT_4U[nT
-00003150: 6f74 616c 4576 656e 745d 0029 0052 6573  otalEvent].).Res
-00003160: 6964 7561 6c20 4750 5320 7469 6d65 2069  idual GPS time i
-00003170: 6e20 696e 7465 6765 7220 6e61 6e6f 7365  n integer nanose
-00003180: 636f 6e64 7300 157d 335d 4b00 0000 0000  conds..}3]K.....
-00003190: 0000 0102 3300 0000 0f00 616d 706c 6974  ....3.....amplit
-000031a0: 7564 6545 7665 6e74 0014 0052 4541 4c5f  udeEvent...REAL_
-000031b0: 345b 6e54 6f74 616c 4576 656e 745d 0010  4[nTotalEvent]..
-000031c0: 0045 7665 6e74 2061 6d70 6c69 7475 6465  .Event amplitude
-000031d0: 00c2 ba16 4177 0000 0000 0000 0001 0234  ....Aw.........4
-000031e0: 0000 000e 0070 6f73 6974 696f 6e45 7665  .....positionEve
-000031f0: 6e74 0014 0049 4e54 5f38 555b 6e54 6f74  nt...INT_8U[nTot
-00003200: 616c 4576 656e 745d 003d 0041 7272 6179  alEvent].=.Array
-00003210: 206f 6620 4672 4576 656e 7420 706f 7369   of FrEvent posi
-00003220: 7469 6f6e 732c 2069 6e20 6279 7465 732c  tions, in bytes,
-00003230: 2066 726f 6d20 6265 6769 6e6e 696e 6720   from beginning 
-00003240: 6f66 2066 696c 6500 46be 4b47 4e00 0000  of file.F.KGN...
-00003250: 0000 0000 0102 3500 0000 0e00 6e53 696d  ......5.....nSim
-00003260: 4576 656e 7454 7970 6500 0700 494e 545f  EventType...INT_
-00003270: 3455 0021 004e 756d 6265 7220 6f66 2046  4U.!.Number of F
-00003280: 7253 696d 4576 656e 7420 696e 2074 6865  rSimEvent in the
-00003290: 2066 696c 6500 d601 de2b 5500 0000 0000   file....+U.....
-000032a0: 0000 0102 3600 0000 0d00 6e61 6d65 5369  ....6.....nameSi
-000032b0: 6d45 7665 6e74 0016 0053 5452 494e 475b  mEvent...STRING[
-000032c0: 6e53 696d 4576 656e 7454 7970 655d 001a  nSimEventType]..
-000032d0: 0041 7272 6179 206f 6620 4672 5369 6d45  .Array of FrSimE
-000032e0: 7665 6e74 206e 616d 6573 00c3 e4da a081  vent names......
-000032f0: 0000 0000 0000 0001 0237 0000 000a 006e  .........7.....n
-00003300: 5369 6d45 7665 6e74 0016 0049 4e54 5f34  SimEvent...INT_4
-00003310: 555b 6e53 696d 4576 656e 7454 7970 655d  U[nSimEventType]
-00003320: 0049 004e 756d 6265 7220 6f66 2046 7253  .I.Number of FrS
-00003330: 696d 4576 656e 7420 666f 7220 6561 6368  imEvent for each
-00003340: 2074 7970 6520 6f66 2046 7253 696d 4576   type of FrSimEv
-00003350: 656e 7420 2873 697a 6520 6f66 206e 5369  ent (size of nSi
-00003360: 6d45 7665 6e74 5479 7065 2900 4e11 c946  mEventType).N..F
-00003370: 4700 0000 0000 0000 0102 3800 0000 0d00  G.........8.....
-00003380: 6e54 6f74 616c 5345 7665 6e74 0007 0049  nTotalSEvent...I
-00003390: 4e54 5f34 5500 1b00 546f 7461 6c20 6e75  NT_4U...Total nu
-000033a0: 6d62 6572 206f 6620 4672 5369 6d45 7665  mber of FrSimEve
-000033b0: 6e74 00de 86a5 7e53 0000 0000 0000 0001  nt....~S........
-000033c0: 0239 0000 000a 0047 5469 6d65 5353 696d  .9.....GTimeSSim
-000033d0: 0015 0049 4e54 5f34 555b 6e54 6f74 616c  ...INT_4U[nTotal
-000033e0: 5345 7665 6e74 5d00 1c00 4750 5320 7469  SEvent]...GPS ti
-000033f0: 6d65 2069 6e20 696e 7465 6765 7220 7365  me in integer se
-00003400: 636f 6e64 7300 8b64 9181 6000 0000 0000  conds..d..`.....
-00003410: 0000 0102 3a00 0000 0a00 4754 696d 654e  ....:.....GTimeN
-00003420: 5369 6d00 1500 494e 545f 3455 5b6e 546f  Sim...INT_4U[nTo
-00003430: 7461 6c53 4576 656e 745d 0029 0052 6573  talSEvent].).Res
-00003440: 6964 7561 6c20 4750 5320 7469 6d65 2069  idual GPS time i
-00003450: 6e20 696e 7465 6765 7220 6e61 6e6f 7365  n integer nanose
-00003460: 636f 6e64 7300 6127 db26 5200 0000 0000  conds.a'.&R.....
-00003470: 0000 0102 3b00 0000 1200 616d 706c 6974  ....;.....amplit
-00003480: 7564 6553 696d 4576 656e 7400 1500 5245  udeSimEvent...RE
-00003490: 414c 5f34 5b6e 546f 7461 6c53 4576 656e  AL_4[nTotalSEven
-000034a0: 745d 0013 0053 696d 4576 656e 7420 616d  t]...SimEvent am
-000034b0: 706c 6974 7564 6500 2410 90c2 7e00 0000  plitude.$...~...
-000034c0: 0000 0000 0102 3c00 0000 1100 706f 7369  ......<.....posi
-000034d0: 7469 6f6e 5369 6d45 7665 6e74 0015 0049  tionSimEvent...I
-000034e0: 4e54 5f38 555b 6e54 6f74 616c 5345 7665  NT_8U[nTotalSEve
-000034f0: 6e74 5d00 4000 4172 7261 7920 6f66 2046  nt].@.Array of F
-00003500: 7253 696d 4576 656e 7420 706f 7369 7469  rSimEvent positi
-00003510: 6f6e 732c 2069 6e20 6279 7465 732c 2066  ons, in bytes, f
-00003520: 726f 6d20 6265 6769 6e6e 696e 6720 6f66  rom beginning of
-00003530: 2066 696c 6500 9f96 37f5 3600 0000 0000   file...7.6.....
-00003540: 0000 0102 3d00 0000 0700 6368 6b53 756d  ....=.....chkSum
-00003550: 0007 0049 4e54 5f34 5500 1000 5374 7275  ...INT_4U...Stru
-00003560: 6374 2063 6865 636b 7375 6d00 8e79 d77a  ct checksum..y.z
-00003570: 5001 0000 0000 0000 0113 0000 0000 2500  P.............%.
-00003580: 0100 0000 696d 6553 b881 8348 0000 0000  ....imeS...H....
-00003590: 0000 0000 0000 1040 0000 0000 2c20 3c54  .......@...., <T
-000035a0: 6e09 0000 0000 0000 0000 0000 0000 0000  n...............
-000035b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000035c0: 0000 0000 0000 0000 0600 0000 0300 0500  ................
-000035d0: 0b00 1400 0700 1300 0700 4672 616d 6548  ..........FrameH
-000035e0: 000b 0046 7244 6574 6563 746f 7200 0b00  ...FrDetector...
-000035f0: 4672 5072 6f63 4461 7461 0007 0046 7256  FrProcData...FrV
-00003600: 6563 7400 0d00 4672 456e 644f 6646 7261  ect...FrEndOfFra
-00003610: 6d65 0006 0046 7254 4f43 0001 0000 0007  me...FrTOC......
-00003620: 004c 484f 5f34 6b00 020d 0000 0000 0000  .LHO_4k.........
-00003630: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00003640: 1100 4831 3a44 4d54 2d44 515f 5645 4354  ..H1:DMT-DQ_VECT
-00003650: 4f52 001a 0048 313a 4744 532d 4341 4c49  OR...H1:GDS-CALI
-00003660: 425f 5354 4154 455f 5645 4354 4f52 0017  B_STATE_VECTOR..
-00003670: 0048 313a 4944 512d 4641 505f 4f56 4c5f  .H1:IDQ-FAP_OVL_
-00003680: 3332 5f32 3034 3800 3719 0000 0000 0000  32_2048.7.......
-00003690: 0214 0000 0000 0000 311a 0000 0000 0000  ........1.......
-000036a0: ffff ffff ffff ffff ffff ffff 0000 0000  ................
-000036b0: 0000 0000 0000 0000 0000 0000 a770 c544  .............p.D
-000036c0: 3f00 0000 0000 0000 0101 0100 0000 0c00  ?...............
-000036d0: 4672 456e 644f 6646 696c 6500 0600 1b00  FrEndOfFile.....
-000036e0: 456e 6420 6f66 2046 696c 6520 4461 7461  End of File Data
-000036f0: 2053 7472 7563 7475 7265 00a8 da1b ec45   Structure.....E
-00003700: 0000 0000 0000 0001 023e 0000 0008 006e  .........>.....n
-00003710: 4672 616d 6573 0007 0049 4e54 5f34 5500  Frames...INT_4U.
-00003720: 1e00 4e75 6d62 6572 206f 6620 6672 616d  ..Number of fram
-00003730: 6573 2069 6e20 7468 6973 2066 696c 6500  es in this file.
-00003740: c01d f442 5f00 0000 0000 0000 0102 3f00  ...B_.........?.
-00003750: 0000 0700 6e42 7974 6573 0007 0049 4e54  ....nBytes...INT
-00003760: 5f38 5500 3900 546f 7461 6c20 6e75 6d62  _8U.9.Total numb
-00003770: 6572 206f 6620 6279 7465 7320 696e 2074  er of bytes in t
-00003780: 6869 7320 6669 6c65 2028 2030 2069 6620  his file ( 0 if 
-00003790: 4e4f 5420 636f 6d70 7574 6564 2029 0082  NOT computed )..
-000037a0: 8d13 02a1 0000 0000 0000 0001 0240 0000  .............@..
-000037b0: 0008 0073 6565 6b54 4f43 0007 0049 4e54  ...seekTOC...INT
-000037c0: 5f38 5500 7a00 4279 6573 2074 6f20 6261  _8U.z.Byes to ba
-000037d0: 636b 2075 7020 746f 2074 6865 2062 6567  ck up to the beg
-000037e0: 696e 6e69 6e67 206f 6620 7468 6520 7461  inning of the ta
-000037f0: 626c 6520 6f66 2063 6f6e 7465 6e74 7320  ble of contents 
-00003800: 7374 7275 6374 7572 652e 2049 6620 7365  structure. If se
-00003810: 656b 544f 4320 3d3d 2030 2c20 7468 656e  ekTOC == 0, then
-00003820: 2074 6865 7265 2069 7320 6e6f 2054 4f43   there is no TOC
-00003830: 2066 6f72 2074 6869 7320 6669 6c65 2e00   for this file..
-00003840: c8d4 6535 4100 0000 0000 0000 0102 4100  ..e5A.........A.
-00003850: 0000 0f00 6368 6b53 756d 4672 4865 6164  ....chkSumFrHead
-00003860: 6572 0007 0049 4e54 5f34 5500 1300 4672  er...INT_4U...Fr
-00003870: 4865 6164 6572 2063 6865 636b 7375 6d2e  Header checksum.
-00003880: 0009 9135 933a 0000 0000 0000 0001 0242  ...5.:.........B
-00003890: 0000 0007 0063 686b 5375 6d00 0700 494e  .....chkSum...IN
-000038a0: 545f 3455 0014 0053 7472 7563 7475 7265  T_4U...Structure
-000038b0: 2063 6865 636b 7375 6d2e 00d0 97d1 a839   checksum......9
-000038c0: 0000 0000 0000 0001 0243 0000 000b 0063  .........C.....c
-000038d0: 686b 5375 6d46 696c 6500 0700 494e 545f  hkSumFile...INT_
-000038e0: 3455 000f 0046 696c 6520 6368 6563 6b73  4U...File checks
-000038f0: 756d 2e00 16df ff60 2e00 0000 0000 0000  um.....`........
-00003900: 0106 0000 0000 0100 0000 2639 0000 0000  ..........&9....
-00003910: 0000 b603 0000 0000 0000 bac1 b663 6ab8  .............cj.
-00003920: c8e8 71c7 ed04                           ..q...
+00001b50: aeb3 7f50 9200 0000 0000 0000 010b 0300  ...P............
+00001b60: 0000 1600 4831 3a49 4451 2d4f 4b5f 4f56  ....H1:IDQ-OK_OV
+00001b70: 4c5f 3332 5f32 3034 3800 1600 4831 3a49  L_32_2048...H1:I
+00001b80: 4451 2d4f 4b5f 4f56 4c5f 3332 5f32 3034  DQ-OK_OVL_32_204
+00001b90: 3800 0100 0000 0000 0000 0000 0000 0000  8...............
+00001ba0: 0000 0000 1040 0000 0000 0000 0000 0000  .....@..........
+00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bc0: 0000 0000 1400 0300 0000 0000 0000 0000  ................
+00001bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001be0: 0000 58c0 43d5 8600 0000 0000 0000 0114  ..X.C...........
+00001bf0: 0300 0000 1600 4831 3a49 4451 2d4f 4b5f  ......H1:IDQ-OK_
+00001c00: 4f56 4c5f 3332 5f32 3034 3800 0101 0200  OVL_32_2048.....
+00001c10: 0004 0000 0000 0000 1f00 0000 0000 0000  ................
+00001c20: 789c edc1 010d 0000 00c2 a0f7 4f6d 0e37  x...........Om.7
+00001c30: a000 0000 0000 0000 8077 0320 0000 0101  .........w. ....
+00001c40: 0000 0000 0400 0000 0000 0000 0000 0000  ................
+00001c50: 0070 3f00 0000 0000 0000 0002 0073 0001  .p?..........s..
+00001c60: 0000 0000 0000 0000 9a71 fcec 4100 0000  .........q..A...
+00001c70: 0000 0000 0101 0400 0000 0d00 4672 456e  ............FrEn
+00001c80: 644f 6646 7261 6d65 0007 001c 0045 6e64  dOfFrame.....End
+00001c90: 206f 6620 4672 616d 6520 4461 7461 2053   of Frame Data S
+00001ca0: 7472 7563 7475 7265 009c ab33 e258 0000  tructure...3.X..
+00001cb0: 0000 0000 0001 0247 0000 0004 0072 756e  .......G.....run
+00001cc0: 0007 0049 4e54 5f34 5300 3500 5275 6e20  ...INT_4S.5.Run 
+00001cd0: 6e75 6d62 6572 3b20 7361 6d65 2061 7320  number; same as 
+00001ce0: 696e 2046 7261 6d65 4865 6164 6572 2072  in FrameHeader r
+00001cf0: 756e 206e 756d 6265 7220 6461 7475 6d2e  un number datum.
+00001d00: 000b 9641 5b87 0000 0000 0000 0001 0248  ...A[..........H
+00001d10: 0000 0006 0066 7261 6d65 0007 0049 4e54  .....frame...INT
+00001d20: 5f34 5500 6200 4672 616d 6520 6e75 6d62  _4U.b.Frame numb
+00001d30: 6572 2c20 6d6f 6e6f 746f 6e69 6361 6c6c  er, monotonicall
+00001d40: 7920 696e 6372 6561 7369 6e67 2075 6e74  y increasing unt
+00001d50: 696c 2065 6e64 206f 6620 7275 6e3b 2073  il end of run; s
+00001d60: 616d 6520 6173 2069 6e20 4672 616d 6520  ame as in Frame 
+00001d70: 4865 6164 6572 2072 756e 206e 756d 6265  Header run numbe
+00001d80: 7220 6461 7475 6d00 ba5a b3d1 4700 0000  r datum..Z..G...
+00001d90: 0000 0000 0102 4900 0000 0700 4754 696d  ......I.....GTim
+00001da0: 6553 0007 0049 4e54 5f34 5500 2100 4672  eS...INT_4U.!.Fr
+00001db0: 616d 6520 7374 6172 7420 7469 6d65 2069  ame start time i
+00001dc0: 6e20 4750 5320 5365 636f 6e64 732e 0018  n GPS Seconds...
+00001dd0: add0 ff56 0000 0000 0000 0001 024a 0000  ...V.........J..
+00001de0: 0007 0047 5469 6d65 4e00 0700 494e 545f  ...GTimeN...INT_
+00001df0: 3455 0030 0046 7261 6d65 2073 7461 7274  4U.0.Frame start
+00001e00: 2074 696d 6520 7265 7369 6475 616c 2c20   time residual, 
+00001e10: 696e 7465 6765 7220 6e61 6e6f 7365 636f  integer nanoseco
+00001e20: 6e64 732e 0064 338f ba36 0000 0000 0000  nds..d3..6......
+00001e30: 0001 024b 0000 0007 0063 686b 5375 6d00  ...K.....chkSum.
+00001e40: 0700 494e 545f 3455 0010 0053 7472 7563  ..INT_4U...Struc
+00001e50: 7420 6368 6563 6b73 756d 0022 ca11 6222  t checksum."..b"
+00001e60: 0000 0000 0000 0001 0700 0000 0000 0000  ................
+00001e70: 0000 0000 0000 0000 0000 0000 00c9 70fa  ..............p.
+00001e80: 3b37 0000 0000 0000 0001 0100 0000 0006  ;7..............
+00001e90: 0046 7254 4f43 0013 0019 0053 696d 756c  .FrTOC.....Simul
+00001ea0: 6174 6564 2044 6174 6120 5374 7275 6374  ated Data Struct
+00001eb0: 7572 6500 7c69 656b 4800 0000 0000 0000  ure.|iekH.......
+00001ec0: 0102 0000 0000 0700 554c 6561 7053 0007  ........ULeapS..
+00001ed0: 0049 4e54 5f32 5300 2200 4672 6f6d 2074  .INT_2S.".From t
+00001ee0: 6865 2066 6972 7374 2046 7261 6d65 4820  he first FrameH 
+00001ef0: 696e 2074 6865 2066 696c 6500 0087 5256  in the file...RV
+00001f00: 4300 0000 0000 0000 0102 0100 0000 0700  C...............
+00001f10: 6e46 7261 6d65 0007 0049 4e54 5f34 5500  nFrame...INT_4U.
+00001f20: 1d00 4e75 6d62 6572 206f 6620 6672 616d  ..Number of fram
+00001f30: 6573 2069 6e20 7468 6520 6669 6c65 00cc  es in the file..
+00001f40: 3d5f 7370 0000 0000 0000 0001 0202 0000  =_sp............
+00001f50: 000c 0064 6174 6151 7561 6c69 7479 000f  ...dataQuality..
+00001f60: 0049 4e54 5f34 555b 6e46 7261 6d65 5d00  .INT_4U[nFrame].
+00001f70: 3d00 4172 7261 7920 6f66 2069 6e74 6567  =.Array of integ
+00001f80: 6572 2051 4120 776f 7264 7320 6672 6f6d  er QA words from
+00001f90: 2065 6163 6820 4672 616d 6548 2028 7369   each FrameH (si
+00001fa0: 7a65 206f 6620 6e46 7261 6d65 7329 0088  ze of nFrames)..
+00001fb0: 6738 c05f 0000 0000 0000 0001 0203 0000  g8._............
+00001fc0: 0007 0047 5469 6d65 5300 0f00 494e 545f  ...GTimeS...INT_
+00001fd0: 3455 5b6e 4672 616d 655d 0031 0041 7272  4U[nFrame].1.Arr
+00001fe0: 6179 206f 6620 696e 7465 6765 7220 4750  ay of integer GP
+00001ff0: 5320 6672 6165 2074 696d 6573 2028 7369  S frae times (si
+00002000: 7a65 206f 6620 6e46 7261 6d65 7300 d5b2  ze of nFrames...
+00002010: 6755 7600 0000 0000 0000 0102 0400 0000  gUv.............
+00002020: 0700 4754 696d 654e 000f 0049 4e54 5f34  ..GTimeN...INT_4
+00002030: 555b 6e46 7261 6d65 5d00 4800 4172 7261  U[nFrame].H.Arra
+00002040: 7920 6f66 2069 6e74 6567 6572 2047 5053  y of integer GPS
+00002050: 2072 6573 6964 7561 6c20 6e61 6e6f 7365   residual nanose
+00002060: 636f 6e64 7320 666f 7220 7468 6520 6672  conds for the fr
+00002070: 616d 6520 2873 697a 6520 6f66 206e 4672  ame (size of nFr
+00002080: 616d 6500 154d fabb 6000 0000 0000 0000  ame..M..`.......
+00002090: 0102 0500 0000 0300 6474 000f 0052 4541  ........dt...REA
+000020a0: 4c5f 385b 6e46 7261 6d65 5d00 3600 4172  L_8[nFrame].6.Ar
+000020b0: 7261 7920 6f66 2066 7261 6d65 2064 7572  ray of frame dur
+000020c0: 6174 696f 6e73 2069 6e20 7365 636f 6e64  ations in second
+000020d0: 7328 2073 697a 6520 6f66 206e 4672 616d  s( size of nFram
+000020e0: 6573 2900 0d06 b877 5200 0000 0000 0000  es)....wR.......
+000020f0: 0102 0600 0000 0500 7275 6e73 000f 0049  ........runs...I
+00002100: 4e54 5f34 535b 6e46 7261 6d65 5d00 2600  NT_4S[nFrame].&.
+00002110: 4172 7261 7920 6f66 2072 756e 206e 756d  Array of run num
+00002120: 6265 7273 2028 7369 7a65 206f 6620 6e46  bers (size of nF
+00002130: 7261 6d65 2900 ca0b 9f5c 5500 0000 0000  rame)....\U.....
+00002140: 0000 0102 0700 0000 0600 6672 616d 6500  ..........frame.
+00002150: 0f00 494e 545f 3455 5b6e 4672 616d 655d  ..INT_4U[nFrame]
+00002160: 0028 0041 7272 6179 206f 6620 6672 616d  .(.Array of fram
+00002170: 6520 6e75 6d62 6572 7320 2873 697a 6520  e numbers (size 
+00002180: 6f66 206e 4672 616d 6529 0031 285d 2581  of nFrame).1(]%.
+00002190: 0000 0000 0000 0001 0208 0000 000a 0070  ...............p
+000021a0: 6f73 6974 696f 6e48 000f 0049 4e54 5f38  ositionH...INT_8
+000021b0: 555b 6e46 7261 6d65 5d00 5000 4172 7261  U[nFrame].P.Arra
+000021c0: 7920 6f66 2046 7261 6d65 4820 706f 7369  y of FrameH posi
+000021d0: 7469 6f6e 732c 2069 6e20 6279 7465 732c  tions, in bytes,
+000021e0: 2066 726f 6d20 7468 6520 6267 696e 6e69   from the bginni
+000021f0: 6e67 206f 6620 6669 6c65 2028 7369 7a65  ng of file (size
+00002200: 206f 6620 6e46 7261 6d65 2900 db18 22e8   of nFrame)...".
+00002210: 8700 0000 0000 0000 0102 0900 0000 0a00  ................
+00002220: 6e46 6972 7374 4144 4300 0f00 494e 545f  nFirstADC...INT_
+00002230: 3855 5b6e 4672 616d 655d 0056 0041 7272  8U[nFrame].V.Arr
+00002240: 6179 206f 6620 6669 7273 7420 4672 4144  ay of first FrAD
+00002250: 4344 6174 6120 706f 7369 7469 6f6e 732c  CData positions,
+00002260: 2069 6e20 6279 7465 732c 2066 726f 6d20   in bytes, from 
+00002270: 6265 6769 6e6e 696e 6720 6f66 2066 696c  beginning of fil
+00002280: 6520 2873 697a 6520 6f66 206e 4672 616d  e (size of nFram
+00002290: 6529 00b7 d5cd 8b86 0000 0000 0000 0001  e)..............
+000022a0: 020a 0000 000a 006e 4669 7273 7453 6572  .......nFirstSer
+000022b0: 000f 0049 4e54 5f38 555b 6e46 7261 6d65  ...INT_8U[nFrame
+000022c0: 5d00 5500 4172 7261 7920 6f66 2066 6972  ].U.Array of fir
+000022d0: 7374 2046 7253 6572 4461 7461 2070 6f73  st FrSerData pos
+000022e0: 6974 696f 6e73 2069 6e20 6279 7465 732c  itions in bytes,
+000022f0: 2066 726f 6d20 6265 6769 6e6e 696e 6720   from beginning 
+00002300: 6f66 2066 696c 6520 2873 697a 6520 6f66  of file (size of
+00002310: 206e 4672 616d 6529 00fa c761 6b87 0000   nFrame)...ak...
+00002320: 0000 0000 0001 020b 0000 000c 006e 4669  .............nFi
+00002330: 7273 7454 6162 6c65 000f 0049 4e54 5f38  rstTable...INT_8
+00002340: 555b 6e46 7261 6d65 5d00 5400 4172 7261  U[nFrame].T.Arra
+00002350: 7920 6f66 2066 6972 7374 2046 7254 6162  y of first FrTab
+00002360: 6c65 2070 6f73 6974 696f 6e73 2c20 696e  le positions, in
+00002370: 2062 7974 6573 2c20 6672 6f6d 2062 6567   bytes, from beg
+00002380: 696e 6e69 6e67 206f 6620 6669 6c65 2028  inning of file (
+00002390: 7369 7a65 206f 6620 6e46 7261 6d65 2900  size of nFrame).
+000023a0: 1016 52a6 8300 0000 0000 0000 0102 0c00  ..R.............
+000023b0: 0000 0a00 6e46 6972 7374 4d73 6700 0f00  ....nFirstMsg...
+000023c0: 494e 545f 3855 5b6e 4672 616d 655d 0052  INT_8U[nFrame].R
+000023d0: 0041 7272 6179 206f 6620 6669 7273 7420  .Array of first 
+000023e0: 4672 4d73 6720 706f 7369 7469 6f6e 732c  FrMsg positions,
+000023f0: 2069 6e20 6279 7465 732c 2066 726f 6d20   in bytes, from 
+00002400: 6265 6769 6e6e 696e 6720 6f66 2066 696c  beginning of fil
+00002410: 6520 2873 697a 6520 6f66 206e 4672 616d  e (size of nFram
+00002420: 6529 00b9 e1c6 f949 0000 0000 0000 0001  e).....I........
+00002430: 020d 0000 0004 006e 5348 0007 0049 4e54  .......nSH...INT
+00002440: 5f34 5500 2600 4e75 6d62 6572 206f 6620  _4U.&.Number of 
+00002450: 4672 5348 2073 7472 7563 7475 7265 7320  FrSH structures 
+00002460: 696e 2074 6865 2066 696c 6500 f46c 0bb0  in the file..l..
+00002470: 4900 0000 0000 0000 0102 0e00 0000 0500  I...............
+00002480: 5348 6964 000c 0049 4e54 5f32 555b 6e53  SHid...INT_2U[nS
+00002490: 485d 0020 0041 7272 6179 206f 6620 4672  H]. .Array of Fr
+000024a0: 5348 2049 4473 2028 7369 7a65 206f 6620  SH IDs (size of 
+000024b0: 6e53 4829 0010 5b23 074d 0000 0000 0000  nSH)..[#.M......
+000024c0: 0001 020f 0000 0007 0053 486e 616d 6500  .........SHname.
+000024d0: 0c00 5354 5249 4e47 5b6e 5348 5d00 2200  ..STRING[nSH].".
+000024e0: 4172 7261 7920 6f66 2046 7253 4820 6e61  Array of FrSH na
+000024f0: 6d65 7320 2873 697a 6520 6f66 206e 5348  mes (size of nSH
+00002500: 2900 a664 b4df 5c00 0000 0000 0000 0102  )..d..\.........
+00002510: 1000 0000 0a00 6e44 6574 6563 746f 7200  ......nDetector.
+00002520: 0700 494e 545f 3455 0033 004e 756d 6265  ..INT_4U.3.Numbe
+00002530: 7220 6f66 2064 6973 7469 6e63 7420 7479  r of distinct ty
+00002540: 7065 7320 6f66 2046 7244 6574 6563 746f  pes of FrDetecto
+00002550: 7220 696e 2074 6865 2066 696c 6500 fa46  r in the file..F
+00002560: 0067 8100 0000 0000 0000 0102 1100 0000  .g..............
+00002570: 0d00 6e61 6d65 4465 7465 6374 6f72 0012  ..nameDetector..
+00002580: 0053 5452 494e 475b 6e44 6574 6563 746f  .STRING[nDetecto
+00002590: 725d 004a 0041 7272 6179 206f 6620 4672  r].J.Array of Fr
+000025a0: 4465 7465 6374 6f72 206e 616d 6573 2028  Detector names (
+000025b0: 7369 7a65 206f 6620 6e44 6574 6563 746f  size of nDetecto
+000025c0: 7229 2e20 5468 6579 2061 7070 6561 7220  r). They appear 
+000025d0: 616c 7068 6162 6574 6963 616c 6c79 0011  alphabetically..
+000025e0: 11d2 a589 0000 0000 0000 0001 0212 0000  ................
+000025f0: 0011 0070 6f73 6974 696f 6e44 6574 6563  ...positionDetec
+00002600: 746f 7200 1200 494e 545f 3855 5b6e 4465  tor...INT_8U[nDe
+00002610: 7465 6374 6f72 5d00 4e00 4172 7261 7920  tector].N.Array 
+00002620: 6f66 2046 7244 6574 6563 746f 7220 706f  of FrDetector po
+00002630: 7369 7469 6f6e 7320 6672 6f6d 2074 6865  sitions from the
+00002640: 2062 6567 696e 6e69 6e67 206f 6620 6669   beginning of fi
+00002650: 6c65 2028 7369 7a65 206f 6620 6e44 6574  le (size of nDet
+00002660: 6563 746f 7229 2e00 8345 9ff0 5800 0000  ector)...E..X...
+00002670: 0000 0000 0102 1300 0000 0a00 6e53 7461  ............nSta
+00002680: 7454 7970 6500 0700 494e 545f 3455 002f  tType...INT_4U./
+00002690: 004e 756d 6265 7220 6f66 2073 7461 7469  .Number of stati
+000026a0: 6320 6461 7461 2062 6c6f 636b 2074 7970  c data block typ
+000026b0: 6573 2069 6e20 7468 6520 6669 6c65 2e00  es in the file..
+000026c0: 0f05 6246 6000 0000 0000 0000 0102 1400  ..bF`...........
+000026d0: 0000 0900 6e61 6d65 5374 6174 0012 0053  ....nameStat...S
+000026e0: 5452 494e 475b 6e53 7461 7454 7970 655d  TRING[nStatType]
+000026f0: 002d 0041 7272 6179 206f 6620 4672 5374  .-.Array of FrSt
+00002700: 6174 4461 7461 206e 616d 6520 2873 697a  atData name (siz
+00002710: 6520 6f66 206e 5374 6174 5479 7065 2900  e of nStatType).
+00002720: a3bf 4547 5d00 0000 0000 0000 0102 1500  ..EG]...........
+00002730: 0000 0900 6465 7465 6374 6f72 0012 0053  ....detector...S
+00002740: 5452 494e 475b 6e53 7461 7454 7970 655d  TRING[nStatType]
+00002750: 002a 0041 7272 6179 206f 6620 4465 7465  .*.Array of Dete
+00002760: 6374 6f72 206e 616d 6528 7369 7a65 206f  ctor name(size o
+00002770: 6620 6e53 7461 7454 7970 6529 0041 b642  f nStatType).A.B
+00002780: 9d7b 0000 0000 0000 0001 0216 0000 000e  .{..............
+00002790: 006e 5374 6174 496e 7374 616e 6365 0012  .nStatInstance..
+000027a0: 0049 4e54 5f34 555b 6e53 7461 7454 7970  .INT_4U[nStatTyp
+000027b0: 655d 0043 0041 7272 6179 206f 6620 6e75  e].C.Array of nu
+000027c0: 6d62 6572 206f 6620 696e 7374 616e 6365  mber of instance
+000027d0: 2066 6f72 2065 6163 6820 4672 5374 6174   for each FrStat
+000027e0: 4461 7461 2873 697a 6520 6f66 206e 5374  Data(size of nSt
+000027f0: 6174 5479 7065 2900 66b8 774f 4b00 0000  atType).f.wOK...
+00002800: 0000 0000 0102 1700 0000 0b00 6e54 6f74  ............nTot
+00002810: 616c 5374 6174 0007 0049 4e54 5f34 5500  alStat...INT_4U.
+00002820: 2100 5375 6d6d 6174 696f 6e20 6f66 206e  !.Summation of n
+00002830: 5374 6174 496e 7374 616e 6365 2061 7272  StatInstance arr
+00002840: 6179 0089 b4e7 f874 0000 0000 0000 0001  ay.....t........
+00002850: 0218 0000 0007 0074 5374 6172 7400 1300  .......tStart...
+00002860: 494e 545f 3455 5b6e 546f 7461 6c53 7461  INT_4U[nTotalSta
+00002870: 745d 0042 0041 7272 6179 206f 6620 4750  t].B.Array of GP
+00002880: 5320 696e 7465 6765 7220 7374 6172 7420  S integer start 
+00002890: 7469 6d65 732c 2069 6e20 7365 636f 6e64  times, in second
+000028a0: 7320 2873 697a 6520 6f66 206e 546f 7461  s (size of nTota
+000028b0: 6c53 7461 7429 001a 531d 0970 0000 0000  lStat)..S..p....
+000028c0: 0000 0001 0219 0000 0005 0074 456e 6400  ...........tEnd.
+000028d0: 1300 494e 545f 3455 5b6e 546f 7461 6c53  ..INT_4U[nTotalS
+000028e0: 7461 745d 0040 0041 7272 6179 206f 6620  tat].@.Array of 
+000028f0: 4750 5320 696e 7465 6765 7220 656e 6420  GPS integer end 
+00002900: 7469 6d65 732c 2069 6e20 7365 636f 6e64  times, in second
+00002910: 7320 2873 697a 6520 6f66 206e 546f 7461  s (size of nTota
+00002920: 6c53 7461 7429 0045 668b 4d5e 0000 0000  lStat).Ef.M^....
+00002930: 0000 0001 021a 0000 0008 0076 6572 7369  ...........versi
+00002940: 6f6e 0013 0049 4e54 5f34 555b 6e54 6f74  on...INT_4U[nTot
+00002950: 616c 5374 6174 5d00 2b00 4172 7261 7920  alStat].+.Array 
+00002960: 6f66 2076 6572 7369 6f6e 2074 696d 6520  of version time 
+00002970: 2873 697a 6520 6f66 206e 546f 7461 6c53  (size of nTotalS
+00002980: 7461 7429 0093 e259 1d82 0000 0000 0000  tat)...Y........
+00002990: 0001 021b 0000 000d 0070 6f73 6974 696f  .........positio
+000029a0: 6e53 7461 7400 1300 494e 545f 3855 5b6e  nStat...INT_8U[n
+000029b0: 546f 7461 6c53 7461 745d 004a 0041 7272  TotalStat].J.Arr
+000029c0: 6179 206f 6620 4672 5374 6174 4461 7461  ay of FrStatData
+000029d0: 2070 6f73 6974 696f 6e73 2066 726f 6d20   positions from 
+000029e0: 6265 6769 6e6e 696e 6720 6f66 2066 696c  beginning of fil
+000029f0: 6520 2873 697a 6520 6f66 206e 546f 7461  e (size of nTota
+00002a00: 6c53 7461 7429 002e 51de 564e 0000 0000  lStat)..Q.VN....
+00002a10: 0000 0001 021c 0000 0005 006e 4144 4300  ...........nADC.
+00002a20: 0700 494e 545f 3455 002a 004e 756d 6265  ..INT_4U.*.Numbe
+00002a30: 7220 6f66 2075 6e69 7175 6520 4672 4164  r of unique FrAd
+00002a40: 6344 6174 6120 6e61 6d65 7320 696e 2066  cData names in f
+00002a50: 696c 652e 0007 54ee e143 0000 0000 0000  ile...T..C......
+00002a60: 0001 021d 0000 0005 006e 616d 6500 0d00  .........name...
+00002a70: 5354 5249 4e47 5b6e 4144 435d 0019 0041  STRING[nADC]...A
+00002a80: 7272 6179 206f 6620 4672 4164 6344 6174  rray of FrAdcDat
+00002a90: 6120 6e61 6d65 7300 89b1 c3ad 4800 0000  a names.....H...
+00002aa0: 0000 0000 0102 1e00 0000 0a00 6368 616e  ............chan
+00002ab0: 6e65 6c49 4400 0d00 494e 545f 3455 5b6e  nelID...INT_4U[n
+00002ac0: 4144 435d 0019 0041 7272 6179 206f 6620  ADC]...Array of 
+00002ad0: 4144 4320 6368 616e 6e65 6c20 4944 7300  ADC channel IDs.
+00002ae0: 251b 8f78 4400 0000 0000 0000 0102 1f00  %..xD...........
+00002af0: 0000 0800 6772 6f75 7049 4400 0d00 494e  ....groupID...IN
+00002b00: 545f 3455 5b6e 4144 435d 0017 0041 7272  T_4U[nADC]...Arr
+00002b10: 6179 206f 6620 4144 4320 6772 6f75 7020  ay of ADC group 
+00002b20: 4944 7300 ec33 7c9e 9e00 0000 0000 0000  IDs..3|.........
+00002b30: 0102 2000 0000 0c00 706f 7369 7469 6f6e  .. .....position
+00002b40: 4144 4300 1500 494e 545f 3855 5b6e 4144  ADC...INT_8U[nAD
+00002b50: 435d 5b6e 4672 616d 655d 0065 0041 7272  C][nFrame].e.Arr
+00002b60: 6179 206f 6620 6c69 7374 7320 6f66 2046  ay of lists of F
+00002b70: 7241 6463 4461 7461 206f 6666 7365 7420  rAdcData offset 
+00002b80: 706f 7369 7469 6f6e 732c 2069 6e20 6279  positions, in by
+00002b90: 7465 732c 2066 726f 6d20 6265 6769 6e6e  tes, from beginn
+00002ba0: 696e 6720 6f66 2066 696c 6520 2873 697a  ing of file (siz
+00002bb0: 6520 6f66 206e 4672 616d 652a 6e41 4443  e of nFrame*nADC
+00002bc0: 2900 6d54 ccf2 5000 0000 0000 0000 0102  ).mT..P.........
+00002bd0: 2100 0000 0600 6e50 726f 6300 0700 494e  !.....nProc...IN
+00002be0: 545f 3455 002b 004e 756d 6265 7220 6f66  T_4U.+.Number of
+00002bf0: 2075 6e69 7175 6520 4672 5072 6f63 4461   unique FrProcDa
+00002c00: 7461 206e 616d 6573 2069 6e20 6669 6c65  ta names in file
+00002c10: 2e00 feef 7499 4900 0000 0000 0000 0102  ....t.I.........
+00002c20: 2200 0000 0900 6e61 6d65 5072 6f63 000e  ".....nameProc..
+00002c30: 0053 5452 494e 475b 6e50 726f 635d 001a  .STRING[nProc]..
+00002c40: 0041 7272 6179 206f 6620 4672 5072 6f63  .Array of FrProc
+00002c50: 4461 7461 206e 616d 6573 0092 f0ec 64a2  Data names....d.
+00002c60: 0000 0000 0000 0001 0223 0000 000d 0070  .........#.....p
+00002c70: 6f73 6974 696f 6e50 726f 6300 1600 494e  ositionProc...IN
+00002c80: 545f 3855 5b6e 5072 6f63 5d5b 6e46 7261  T_8U[nProc][nFra
+00002c90: 6d65 5d00 6700 4172 7261 7920 6f66 206c  me].g.Array of l
+00002ca0: 6973 7473 206f 6620 4672 5072 6f63 4461  ists of FrProcDa
+00002cb0: 7461 206f 6666 7365 7420 706f 7369 7469  ta offset positi
+00002cc0: 6f6e 732c 2069 6e20 6279 7465 732c 2066  ons, in bytes, f
+00002cd0: 726f 6d20 6265 6769 6e6e 696e 6720 6f66  rom beginning of
+00002ce0: 2066 696c 6520 2873 697a 6520 6f66 206e   file (size of n
+00002cf0: 4672 616d 652a 6e50 726f 6329 00f2 b9e4  Frame*nProc)....
+00002d00: a64e 0000 0000 0000 0001 0224 0000 0005  .N.........$....
+00002d10: 006e 5369 6d00 0700 494e 545f 3455 002a  .nSim...INT_4U.*
+00002d20: 004e 756d 6265 7220 6f66 2075 6e69 7175  .Number of uniqu
+00002d30: 6520 4672 5369 6d44 6174 6120 6e61 6d65  e FrSimData name
+00002d40: 7320 696e 2066 696c 652e 0008 01bc 3746  s in file.....7F
+00002d50: 0000 0000 0000 0001 0225 0000 0008 006e  .........%.....n
+00002d60: 616d 6553 696d 000d 0053 5452 494e 475b  ameSim...STRING[
+00002d70: 6e53 696d 5d00 1900 4172 7261 7920 6f66  nSim]...Array of
+00002d80: 2046 7253 696d 4461 7461 206e 616d 6573   FrSimData names
+00002d90: 00c4 a72b f69e 0000 0000 0000 0001 0226  ...+...........&
+00002da0: 0000 000c 0070 6f73 6974 696f 6e53 696d  .....positionSim
+00002db0: 0015 0049 4e54 5f38 555b 6e53 696d 5d5b  ...INT_8U[nSim][
+00002dc0: 6e46 7261 6d65 5d00 6500 4172 7261 7920  nFrame].e.Array 
+00002dd0: 6f66 206c 6973 7473 206f 6620 4672 5369  of lists of FrSi
+00002de0: 6d44 6174 6120 6f66 6673 6574 2070 6f73  mData offset pos
+00002df0: 6974 696f 6e73 2c20 696e 2062 7974 6573  itions, in bytes
+00002e00: 2c20 6672 6f6d 2062 6567 696e 6e69 6e67  , from beginning
+00002e10: 206f 6620 6669 6c65 2028 7369 7a65 206f   of file (size o
+00002e20: 6620 6e46 7261 6d65 2a6e 5369 6d29 00d3  f nFrame*nSim)..
+00002e30: 40ba c14e 0000 0000 0000 0001 0227 0000  @..N.........'..
+00002e40: 0005 006e 5365 7200 0700 494e 545f 3455  ...nSer...INT_4U
+00002e50: 002a 004e 756d 6265 7220 6f66 2075 6e69  .*.Number of uni
+00002e60: 7175 6520 4672 5365 7244 6174 6120 6e61  que FrSerData na
+00002e70: 6d65 7320 696e 2066 696c 652e 000f 814d  mes in file....M
+00002e80: 9046 0000 0000 0000 0001 0228 0000 0008  .F.........(....
+00002e90: 006e 616d 6553 6572 000d 0053 5452 494e  .nameSer...STRIN
+00002ea0: 475b 6e53 6572 5d00 1900 4172 7261 7920  G[nSer]...Array 
+00002eb0: 6f66 2046 7253 6572 4461 7461 206e 616d  of FrSerData nam
+00002ec0: 6573 00bd 2d79 109e 0000 0000 0000 0001  es..-y..........
+00002ed0: 0229 0000 000c 0070 6f73 6974 696f 6e53  .).....positionS
+00002ee0: 6572 0015 0049 4e54 5f38 555b 6e53 6572  er...INT_8U[nSer
+00002ef0: 5d5b 6e46 7261 6d65 5d00 6500 4172 7261  ][nFrame].e.Arra
+00002f00: 7920 6f66 206c 6973 7473 206f 6620 4672  y of lists of Fr
+00002f10: 5365 7244 6174 6120 6f66 6673 6574 2070  SerData offset p
+00002f20: 6f73 6974 696f 6e73 2c20 696e 2062 7974  ositions, in byt
+00002f30: 6573 2c20 6672 6f6d 2062 6567 696e 6e69  es, from beginni
+00002f40: 6e67 206f 6620 6669 6c65 2028 7369 7a65  ng of file (size
+00002f50: 206f 6620 6e46 7261 6d65 2a6e 5365 7229   of nFrame*nSer)
+00002f60: 001c 5003 fb52 0000 0000 0000 0001 022a  ..P..R.........*
+00002f70: 0000 0009 006e 5375 6d6d 6172 7900 0700  .....nSummary...
+00002f80: 494e 545f 3455 002a 004e 756d 6265 7220  INT_4U.*.Number 
+00002f90: 6f66 2075 6e69 7175 6520 4672 5375 6d6d  of unique FrSumm
+00002fa0: 6172 7920 6e61 6d65 7320 696e 2066 696c  ary names in fil
+00002fb0: 652e 0034 77a5 e94b 0000 0000 0000 0001  e..4w..K........
+00002fc0: 022b 0000 0009 006e 616d 6553 5375 6d00  .+.....nameSSum.
+00002fd0: 1100 5354 5249 4e47 5b6e 5375 6d6d 6172  ..STRING[nSummar
+00002fe0: 795d 0019 0041 7272 6179 206f 6620 4672  y]...Array of Fr
+00002ff0: 5375 6d6d 6172 7920 6e61 6d65 7300 0684  Summary names...
+00003000: 574e a200 0000 0000 0000 0102 2c00 0000  WN..........,...
+00003010: 0c00 706f 7369 7469 6f6e 5365 7200 1900  ..positionSer...
+00003020: 494e 545f 3855 5b6e 5375 6d6d 6172 795d  INT_8U[nSummary]
+00003030: 5b6e 4672 616d 655d 0065 0041 7272 6179  [nFrame].e.Array
+00003040: 206f 6620 6c69 7374 7320 6f66 2046 7253   of lists of FrS
+00003050: 756d 6d61 7279 206f 6666 7365 7420 706f  ummary offset po
+00003060: 7369 7469 6f6e 732c 2069 6e20 6279 7465  sitions, in byte
+00003070: 732c 2066 726f 6d20 6265 6769 6e6e 696e  s, from beginnin
+00003080: 6720 6f66 2066 696c 6520 2873 697a 6520  g of file (size 
+00003090: 6f66 206e 4672 616d 652a 6e53 6572 2900  of nFrame*nSer).
+000030a0: c376 da95 4800 0000 0000 0000 0102 2d00  .v..H.........-.
+000030b0: 0000 0b00 6e45 7665 6e74 5479 7065 0007  ....nEventType..
+000030c0: 0049 4e54 5f34 5500 1e00 4e75 6d62 6572  .INT_4U...Number
+000030d0: 206f 6620 4672 4576 656e 7420 696e 2074   of FrEvent in t
+000030e0: 6865 2066 696c 6500 cb0b 34f7 4c00 0000  he file...4.L...
+000030f0: 0000 0000 0102 2e00 0000 0a00 6e61 6d65  ............name
+00003100: 4576 656e 7400 1300 5354 5249 4e47 5b6e  Event...STRING[n
+00003110: 4576 656e 7454 7970 655d 0017 0041 7272  EventType]...Arr
+00003120: 6179 206f 6620 4672 4576 656e 7420 6e61  ay of FrEvent na
+00003130: 6d65 7300 8aec 7442 7200 0000 0000 0000  mes...tBr.......
+00003140: 0102 2f00 0000 0700 6e45 7665 6e74 0013  ../.....nEvent..
+00003150: 0049 4e54 5f34 555b 6e45 7665 6e74 5479  .INT_4U[nEventTy
+00003160: 7065 5d00 4000 4e75 6d62 6572 206f 6620  pe].@.Number of 
+00003170: 4672 4576 656e 7420 666f 7220 6561 6368  FrEvent for each
+00003180: 2074 7970 6520 6f66 2046 7245 7665 6e74   type of FrEvent
+00003190: 2028 7369 7a65 206f 6620 6e45 7665 6e74   (size of nEvent
+000031a0: 5479 7065 2900 aebb 6fd3 4300 0000 0000  Type)...o.C.....
+000031b0: 0000 0102 3000 0000 0c00 6e54 6f74 616c  ....0.....nTotal
+000031c0: 4576 656e 7400 0700 494e 545f 3455 0018  Event...INT_4U..
+000031d0: 0054 6f74 616c 206e 756d 6265 7220 6f66  .Total number of
+000031e0: 2046 7245 7665 6e74 0074 8af4 4a54 0000   FrEvent.t..JT..
+000031f0: 0000 0000 0001 0231 0000 000c 0047 5469  .......1.....GTi
+00003200: 6d65 5345 7665 6e74 0014 0049 4e54 5f34  meSEvent...INT_4
+00003210: 555b 6e54 6f74 616c 4576 656e 745d 001c  U[nTotalEvent]..
+00003220: 0047 5053 2074 696d 6520 696e 2069 6e74  .GPS time in int
+00003230: 6567 6572 2073 6563 6f6e 6473 0015 3513  eger seconds..5.
+00003240: 2961 0000 0000 0000 0001 0232 0000 000c  )a.........2....
+00003250: 0047 5469 6d65 4e45 7665 6e74 0014 0049  .GTimeNEvent...I
+00003260: 4e54 5f34 555b 6e54 6f74 616c 4576 656e  NT_4U[nTotalEven
+00003270: 745d 0029 0052 6573 6964 7561 6c20 4750  t].).Residual GP
+00003280: 5320 7469 6d65 2069 6e20 696e 7465 6765  S time in intege
+00003290: 7220 6e61 6e6f 7365 636f 6e64 7300 157d  r nanoseconds..}
+000032a0: 335d 4b00 0000 0000 0000 0102 3300 0000  3]K.........3...
+000032b0: 0f00 616d 706c 6974 7564 6545 7665 6e74  ..amplitudeEvent
+000032c0: 0014 0052 4541 4c5f 345b 6e54 6f74 616c  ...REAL_4[nTotal
+000032d0: 4576 656e 745d 0010 0045 7665 6e74 2061  Event]...Event a
+000032e0: 6d70 6c69 7475 6465 00c2 ba16 4177 0000  mplitude....Aw..
+000032f0: 0000 0000 0001 0234 0000 000e 0070 6f73  .......4.....pos
+00003300: 6974 696f 6e45 7665 6e74 0014 0049 4e54  itionEvent...INT
+00003310: 5f38 555b 6e54 6f74 616c 4576 656e 745d  _8U[nTotalEvent]
+00003320: 003d 0041 7272 6179 206f 6620 4672 4576  .=.Array of FrEv
+00003330: 656e 7420 706f 7369 7469 6f6e 732c 2069  ent positions, i
+00003340: 6e20 6279 7465 732c 2066 726f 6d20 6265  n bytes, from be
+00003350: 6769 6e6e 696e 6720 6f66 2066 696c 6500  ginning of file.
+00003360: 46be 4b47 4e00 0000 0000 0000 0102 3500  F.KGN.........5.
+00003370: 0000 0e00 6e53 696d 4576 656e 7454 7970  ....nSimEventTyp
+00003380: 6500 0700 494e 545f 3455 0021 004e 756d  e...INT_4U.!.Num
+00003390: 6265 7220 6f66 2046 7253 696d 4576 656e  ber of FrSimEven
+000033a0: 7420 696e 2074 6865 2066 696c 6500 d601  t in the file...
+000033b0: de2b 5500 0000 0000 0000 0102 3600 0000  .+U.........6...
+000033c0: 0d00 6e61 6d65 5369 6d45 7665 6e74 0016  ..nameSimEvent..
+000033d0: 0053 5452 494e 475b 6e53 696d 4576 656e  .STRING[nSimEven
+000033e0: 7454 7970 655d 001a 0041 7272 6179 206f  tType]...Array o
+000033f0: 6620 4672 5369 6d45 7665 6e74 206e 616d  f FrSimEvent nam
+00003400: 6573 00c3 e4da a081 0000 0000 0000 0001  es..............
+00003410: 0237 0000 000a 006e 5369 6d45 7665 6e74  .7.....nSimEvent
+00003420: 0016 0049 4e54 5f34 555b 6e53 696d 4576  ...INT_4U[nSimEv
+00003430: 656e 7454 7970 655d 0049 004e 756d 6265  entType].I.Numbe
+00003440: 7220 6f66 2046 7253 696d 4576 656e 7420  r of FrSimEvent 
+00003450: 666f 7220 6561 6368 2074 7970 6520 6f66  for each type of
+00003460: 2046 7253 696d 4576 656e 7420 2873 697a   FrSimEvent (siz
+00003470: 6520 6f66 206e 5369 6d45 7665 6e74 5479  e of nSimEventTy
+00003480: 7065 2900 4e11 c946 4700 0000 0000 0000  pe).N..FG.......
+00003490: 0102 3800 0000 0d00 6e54 6f74 616c 5345  ..8.....nTotalSE
+000034a0: 7665 6e74 0007 0049 4e54 5f34 5500 1b00  vent...INT_4U...
+000034b0: 546f 7461 6c20 6e75 6d62 6572 206f 6620  Total number of 
+000034c0: 4672 5369 6d45 7665 6e74 00de 86a5 7e53  FrSimEvent....~S
+000034d0: 0000 0000 0000 0001 0239 0000 000a 0047  .........9.....G
+000034e0: 5469 6d65 5353 696d 0015 0049 4e54 5f34  TimeSSim...INT_4
+000034f0: 555b 6e54 6f74 616c 5345 7665 6e74 5d00  U[nTotalSEvent].
+00003500: 1c00 4750 5320 7469 6d65 2069 6e20 696e  ..GPS time in in
+00003510: 7465 6765 7220 7365 636f 6e64 7300 8b64  teger seconds..d
+00003520: 9181 6000 0000 0000 0000 0102 3a00 0000  ..`.........:...
+00003530: 0a00 4754 696d 654e 5369 6d00 1500 494e  ..GTimeNSim...IN
+00003540: 545f 3455 5b6e 546f 7461 6c53 4576 656e  T_4U[nTotalSEven
+00003550: 745d 0029 0052 6573 6964 7561 6c20 4750  t].).Residual GP
+00003560: 5320 7469 6d65 2069 6e20 696e 7465 6765  S time in intege
+00003570: 7220 6e61 6e6f 7365 636f 6e64 7300 6127  r nanoseconds.a'
+00003580: db26 5200 0000 0000 0000 0102 3b00 0000  .&R.........;...
+00003590: 1200 616d 706c 6974 7564 6553 696d 4576  ..amplitudeSimEv
+000035a0: 656e 7400 1500 5245 414c 5f34 5b6e 546f  ent...REAL_4[nTo
+000035b0: 7461 6c53 4576 656e 745d 0013 0053 696d  talSEvent]...Sim
+000035c0: 4576 656e 7420 616d 706c 6974 7564 6500  Event amplitude.
+000035d0: 2410 90c2 7e00 0000 0000 0000 0102 3c00  $...~.........<.
+000035e0: 0000 1100 706f 7369 7469 6f6e 5369 6d45  ....positionSimE
+000035f0: 7665 6e74 0015 0049 4e54 5f38 555b 6e54  vent...INT_8U[nT
+00003600: 6f74 616c 5345 7665 6e74 5d00 4000 4172  otalSEvent].@.Ar
+00003610: 7261 7920 6f66 2046 7253 696d 4576 656e  ray of FrSimEven
+00003620: 7420 706f 7369 7469 6f6e 732c 2069 6e20  t positions, in 
+00003630: 6279 7465 732c 2066 726f 6d20 6265 6769  bytes, from begi
+00003640: 6e6e 696e 6720 6f66 2066 696c 6500 9f96  nning of file...
+00003650: 37f5 3600 0000 0000 0000 0102 3d00 0000  7.6.........=...
+00003660: 0700 6368 6b53 756d 0007 0049 4e54 5f34  ..chkSum...INT_4
+00003670: 5500 1000 5374 7275 6374 2063 6865 636b  U...Struct check
+00003680: 7375 6d00 8e79 d77a 7001 0000 0000 0000  sum..y.zp.......
+00003690: 0113 0000 0000 2500 0100 0000 0000 0000  ......%.........
+000036a0: b881 8348 0000 0000 0000 0000 0000 1040  ...H...........@
+000036b0: 0000 0000 0000 0000 6e09 0000 0000 0000  ........n.......
+000036c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000036d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000036e0: 0600 0000 0300 0500 0b00 1400 0700 1300  ................
+000036f0: 0700 4672 616d 6548 000b 0046 7244 6574  ..FrameH...FrDet
+00003700: 6563 746f 7200 0b00 4672 5072 6f63 4461  ector...FrProcDa
+00003710: 7461 0007 0046 7256 6563 7400 0d00 4672  ta...FrVect...Fr
+00003720: 456e 644f 6646 7261 6d65 0006 0046 7254  EndOfFrame...FrT
+00003730: 4f43 0001 0000 0007 004c 484f 5f34 6b00  OC.......LHO_4k.
+00003740: 020d 0000 0000 0000 0000 0000 0000 0000  ................
+00003750: 0000 0000 0400 0000 1100 4831 3a44 4d54  ..........H1:DMT
+00003760: 2d44 515f 5645 4354 4f52 001a 0048 313a  -DQ_VECTOR...H1:
+00003770: 4744 532d 4341 4c49 425f 5354 4154 455f  GDS-CALIB_STATE_
+00003780: 5645 4354 4f52 0017 0048 313a 4944 512d  VECTOR...H1:IDQ-
+00003790: 4641 505f 4f56 4c5f 3332 5f32 3034 3800  FAP_OVL_32_2048.
+000037a0: 1600 4831 3a49 4451 2d4f 4b5f 4f56 4c5f  ..H1:IDQ-OK_OVL_
+000037b0: 3332 5f32 3034 3800 3719 0000 0000 0000  32_2048.7.......
+000037c0: 0214 0000 0000 0000 311a 0000 0000 0000  ........1.......
+000037d0: 541b 0000 0000 0000 ffff ffff ffff ffff  T...............
+000037e0: ffff ffff 0000 0000 0000 0000 0000 0000  ................
+000037f0: 0000 0000 7a7d e364 3f00 0000 0000 0000  ....z}.d?.......
+00003800: 0101 0100 0000 0c00 4672 456e 644f 6646  ........FrEndOfF
+00003810: 696c 6500 0600 1b00 456e 6420 6f66 2046  ile.....End of F
+00003820: 696c 6520 4461 7461 2053 7472 7563 7475  ile Data Structu
+00003830: 7265 00a8 da1b ec45 0000 0000 0000 0001  re.....E........
+00003840: 023e 0000 0008 006e 4672 616d 6573 0007  .>.....nFrames..
+00003850: 0049 4e54 5f34 5500 1e00 4e75 6d62 6572  .INT_4U...Number
+00003860: 206f 6620 6672 616d 6573 2069 6e20 7468   of frames in th
+00003870: 6973 2066 696c 6500 c01d f442 5f00 0000  is file....B_...
+00003880: 0000 0000 0102 3f00 0000 0700 6e42 7974  ......?.....nByt
+00003890: 6573 0007 0049 4e54 5f38 5500 3900 546f  es...INT_8U.9.To
+000038a0: 7461 6c20 6e75 6d62 6572 206f 6620 6279  tal number of by
+000038b0: 7465 7320 696e 2074 6869 7320 6669 6c65  tes in this file
+000038c0: 2028 2030 2069 6620 4e4f 5420 636f 6d70   ( 0 if NOT comp
+000038d0: 7574 6564 2029 0082 8d13 02a1 0000 0000  uted )..........
+000038e0: 0000 0001 0240 0000 0008 0073 6565 6b54  .....@.....seekT
+000038f0: 4f43 0007 0049 4e54 5f38 5500 7a00 4279  OC...INT_8U.z.By
+00003900: 6573 2074 6f20 6261 636b 2075 7020 746f  es to back up to
+00003910: 2074 6865 2062 6567 696e 6e69 6e67 206f   the beginning o
+00003920: 6620 7468 6520 7461 626c 6520 6f66 2063  f the table of c
+00003930: 6f6e 7465 6e74 7320 7374 7275 6374 7572  ontents structur
+00003940: 652e 2049 6620 7365 656b 544f 4320 3d3d  e. If seekTOC ==
+00003950: 2030 2c20 7468 656e 2074 6865 7265 2069   0, then there i
+00003960: 7320 6e6f 2054 4f43 2066 6f72 2074 6869  s no TOC for thi
+00003970: 7320 6669 6c65 2e00 c8d4 6535 4100 0000  s file....e5A...
+00003980: 0000 0000 0102 4100 0000 0f00 6368 6b53  ......A.....chkS
+00003990: 756d 4672 4865 6164 6572 0007 0049 4e54  umFrHeader...INT
+000039a0: 5f34 5500 1300 4672 4865 6164 6572 2063  _4U...FrHeader c
+000039b0: 6865 636b 7375 6d2e 0009 9135 933a 0000  hecksum....5.:..
+000039c0: 0000 0000 0001 0242 0000 0007 0063 686b  .......B.....chk
+000039d0: 5375 6d00 0700 494e 545f 3455 0014 0053  Sum...INT_4U...S
+000039e0: 7472 7563 7475 7265 2063 6865 636b 7375  tructure checksu
+000039f0: 6d2e 00d0 97d1 a839 0000 0000 0000 0001  m......9........
+00003a00: 0243 0000 000b 0063 686b 5375 6d46 696c  .C.....chkSumFil
+00003a10: 6500 0700 494e 545f 3455 000f 0046 696c  e...INT_4U...Fil
+00003a20: 6520 6368 6563 6b73 756d 2e00 16df ff60  e checksum.....`
+00003a30: 2e00 0000 0000 0000 0106 0000 0000 0100  ................
+00003a40: 0000 5e3a 0000 0000 0000 d603 0000 0000  ..^:............
+00003a50: 0000 bac1 b663 0c5b 4c35 b158 d144       .....c.[L5.X.D
```

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/lvalert_event_creation.json` & `gwcelery-2.1.2/gwcelery/tests/data/lvalert_event_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/lvalert_xmpp.xml` & `gwcelery-2.1.2/gwcelery/tests/data/lvalert_xmpp.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/mock_superevent_object.json` & `gwcelery-2.1.2/gwcelery/tests/data/mock_superevent_object.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite` & `gwcelery-2.1.2/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/psd.xml.gz` & `gwcelery-2.1.2/gwcelery/tests/data/psd.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/rrt_small_area.fits` & `gwcelery-2.1.2/gwcelery/tests/data/rrt_small_area.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/sample_events.json` & `gwcelery-2.1.2/gwcelery/tests/data/sample_events.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/samples.hdf5` & `gwcelery-2.1.2/gwcelery/tests/data/samples.hdf5`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/scaler_set_all.pickle` & `gwcelery-2.1.2/gwcelery/tests/data/scaler_set_all.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/snews_gcn.xml` & `gwcelery-2.1.2/gwcelery/tests/data/snews_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/snews_gcn_test.xml` & `gwcelery-2.1.2/gwcelery/tests/data/snews_gcn_test.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/superevents.json` & `gwcelery-2.1.2/gwcelery/tests/data/superevents.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/swift_grb_gcn.xml` & `gwcelery-2.1.2/gwcelery/tests/data/swift_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/data/test_classifier.pickle` & `gwcelery-2.1.2/gwcelery/tests/data/test_classifier.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/process.py` & `gwcelery-2.1.2/gwcelery/tests/process.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_sentry.py` & `gwcelery-2.1.2/gwcelery/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_alerts.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_alerts_validate.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_alerts_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_bayestar.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_circulars.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_condor.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_detchar.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_detchar.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 @pytest.fixture
 def llhoft_glob_fail(monkeypatch):
     path = str(Path(__file__).parent / 'data/llhoft/fail/{detector}/*.gwf')
     yield monkeypatch.setitem(app.conf, 'llhoft_glob', path)
 
 
 @pytest.fixture
+def llhoft_glob_idq_bad(monkeypatch):
+    path = str(Path(__file__).parent / 'data/llhoft/idqbad/{detector}/*.gwf')
+    yield monkeypatch.setitem(app.conf, 'llhoft_glob', path)
+
+
+@pytest.fixture
 def ifo_h1(monkeypatch):
     monkeypatch.setitem(app.conf, 'llhoft_channels', {
         'H1:DMT-DQ_VECTOR': 'dmt_dq_vector_bits',
         'H1:GDS-CALIB_STATE_VECTOR': 'ligo_state_vector_bits'})
 
 
 @pytest.fixture
@@ -41,20 +47,24 @@
         'L1:GDS-CALIB_STATE_VECTOR': 'ligo_state_vector_bits'})
 
 
 @pytest.fixture
 def ifo_h1_idq(monkeypatch):
     monkeypatch.setitem(
         app.conf, 'idq_channels', ['H1:IDQ-FAP_OVL_32_2048'])
+    monkeypatch.setitem(
+        app.conf, 'idq_ok_channels', ['H1:IDQ-OK_OVL_32_2048'])
 
 
 @pytest.fixture
 def ifo_l1_idq(monkeypatch):
     monkeypatch.setitem(
         app.conf, 'idq_channels', ['L1:IDQ-FAP_OVL_32_2048'])
+    monkeypatch.setitem(
+        app.conf, 'idq_ok_channels', ['L1:IDQ-OK_OVL_32_2048'])
 
 
 @pytest.fixture
 def ifo_l1_idq_wrong_channel_name(monkeypatch):
     monkeypatch.setitem(
         app.conf, 'idq_channels', ['L1:IDQ-FAP_OVL_WRONG'])
 
@@ -120,14 +130,22 @@
     detchar.omegascan(t0, gid)
     mock_upload.assert_called_with(
         mock_fig(), "V1_omegascan.png", gid, "V1 omegascan",
         tags=['data_quality']
     )
 
 
+def test_ifo_from_channel():
+    channels = [
+        'H1:GDS-CALIB_STRAIN', 'L1:DMT-DQ_VECTOR',
+        'V1:DQ_ANALYSIS_STATE_VECTOR', 'K1:TEST-CHAN']
+    ifos = [detchar.ifo_from_channel(chan) for chan in channels]
+    assert ifos == ['H1', 'L1', 'V1', 'K1']
+
+
 def test_omegascan_skips_ew(caplog):
     """Test that omegascans are delayed for events in the future."""
     caplog.set_level(logging.INFO)
     detchar.omegascan(Time.now().gps + 99, 'S1234')
     messages = [record.message for record in caplog.records]
     assert 'Delaying omegascan because S1234 is in the future' in messages  # noqa: E501
 
@@ -322,14 +340,30 @@
     ]
     mock_upload.assert_has_calls(calls, any_order=True)
     mock_create_label.assert_called_with('DQV', 'S12345a')
     mock_remove_label.assert_called_with('DQOK', 'S12345a')
 
 
 @patch('gwcelery.tasks.gracedb.upload.run')
+def test_check_vectors_idq_not_ok(
+        mock_upload, llhoft_glob_idq_bad, ifo_h1, ifo_h1_idq):
+    event = {'search': 'AllSky', 'instruments': 'H1', 'pipeline': 'oLIB'}
+    superevent_id = 'S12345a'
+    start, end = 1216577978, 1216577978.1
+    detchar.check_vectors(event, superevent_id, start, end)
+    mock_upload.assert_any_call(
+        None, None, 'S12345a',
+        ('Not checking iDQ for H1 '
+            'because it has times where IDQ_OK = 0. '
+            'Check looked within -1.5/+1.5 seconds of superevent. '),
+        ['data_quality']
+    )
+
+
+@patch('gwcelery.tasks.gracedb.upload.run')
 @patch('celery.app.task.Task.request')
 @patch('gwcelery.tasks.detchar.check_vector', side_effect=ValueError)
 def test_check_vectors_retries_on_valueerror(
         mock_check_vector, mock_request,
         mock_upload, llhoft_glob_pass, ifo_h1, ifo_h1_idq):
     # Mocking this retry https://docs.celeryq.dev/en/stable/_modules/celery/app/task.html#Task.retry  # noqa E501
     event = {'search': 'AllSky', 'instruments': 'L1', 'pipeline': 'oLIB'}
@@ -381,14 +415,12 @@
               '    <tr><td>good_bit_2</td><td bgcolor="#0f0">1</td></tr>\n'
               '    <tr><td>bad_bit_1</td><td bgcolor="red">0</td></tr>\n'
               '    <tr><td>bad_bit_2</td><td bgcolor="red">0</td></tr>\n'
               '    <tr><td>unknown_bit_1</td>'
               '<td bgcolor="yellow">unknown</td></tr>\n'
               '    <tr><td>unknown_bit_2</td>'
               '<td bgcolor="yellow">unknown</td></tr>\n'
-              '    <tr bgcolor="red"><th>Overall state for all '
-              'detectors</th><th>bad</th></tr>\n'
               '</table>')
     assert detchar.generate_table(
         'title', ['good_bit_1', 'good_bit_2'],
         ['bad_bit_1', 'bad_bit_2'], ['unknown_bit_1', 'unknown_bit_2']
     ) == result
```

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_em_bright.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_external_skymaps.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_external_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_external_triggers.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_external_triggers.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_first2years.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_first2years_external.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_gcn.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_gcn_validate.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_gcn_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_gracedb.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_gwskynet.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_gwskynet.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_igwn_alert.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_inference.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,62 +9,14 @@
 from unittest.mock import Mock
 
 from .. import app
 from ..tasks import condor
 from ..tasks import inference
 
 
-def mock_find_urls(available_frametypes):
-    """Return mock gwdatafind.find_urls, which returns 'path_to_data' when
-    input ifo and frametype are in available_frametypes.
-
-    available_frametypes : dictionary
-        Dictionary whose key is ifo and item is frametype
-    """
-    _available_frametypes = dict(
-        (ifo[0], frametype) for ifo, frametype in available_frametypes.items())
-
-    def _mock_find_url(ifo, frametype, start, end):
-        data_exists = (ifo in _available_frametypes.keys() and
-                       frametype == _available_frametypes[ifo])
-        if data_exists:
-            return ['path_to_data']
-        else:
-            return []
-
-    return _mock_find_url
-
-
-@pytest.mark.parametrize(
-    'available_frametypes,answer',
-    [[{}, None],
-     [{'H1': app.conf['low_latency_frame_types']['H1']}, None],
-     [app.conf['low_latency_frame_types'],
-      app.conf['low_latency_frame_types']],
-     [app.conf['high_latency_frame_types'],
-      app.conf['high_latency_frame_types']]]
-)
-def test_query_data(monkeypatch, available_frametypes, answer):
-    monkeypatch.setattr('gwcelery.tasks.inference.find_urls',
-                        mock_find_urls(available_frametypes))
-    if answer is None:
-        with pytest.raises(inference.NotEnoughData):
-            inference.query_data(1187008882)
-    else:
-        assert inference.query_data(1187008882) == answer
-
-
-def test_upload_no_frametypes(monkeypatch):
-    upload = Mock()
-    monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', upload)
-    inference.upload_no_frame_files(
-        None, inference.NotEnoughData(), 'test', 'S1234')
-    upload.assert_called_once()
-
-
 def test_find_appropriate_cal_env(tmp_path):
     filepath = tmp_path / 'H_CalEnvs.txt'
     t1, cal1 = 1126259462, 'O1_calibration.txt'
     t2, cal2 = 1187008882, 'O2_calibration.txt'
     filepath.write_text('{t1} {cal1}\n{t2} {cal2}'.format(
             t1=t1, cal1=cal1, t2=t2, cal2=cal2))
     dir_name = str(tmp_path)
@@ -122,16 +74,15 @@
         'gpstime': 1187008882,
         'graceid': 'G1234',
         'extra_attributes':
             {'SingleInspiral': [{'mass1': m1, 'mass2': m2, 'mchirp': mc}]}
     }
     config = configparser.ConfigParser()
     config.read_string(
-        inference.prepare_lalinference_ini(
-            app.conf['low_latency_frame_types'], event, 'S1234'))
+        inference.prepare_lalinference_ini(event, 'S1234'))
     for section, key, answer in answers:
         assert config[section][key] == answer
 
 
 def test_setup_dag_for_lalinference(monkeypatch, tmp_path):
     coinc = b'coinc'
     rundir = str(tmp_path)
@@ -163,15 +114,15 @@
     monkeypatch.setattr('subprocess.run', _subprocess_run)
     monkeypatch.setattr(
         'gwcelery.tasks.inference.prepare_lalinference_ini',
         Mock(return_value=ini))
     monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', upload)
 
     path_to_dag = inference._setup_dag_for_lalinference(
-        coinc, rundir, {}, 'S1234', {})
+        coinc, rundir, {}, 'S1234')
 
     assert os.path.exists(path_to_dag)
     with open(path_to_dag, 'r') as f:
         assert f.read() == dag
     upload.assert_called_once()
 
 
@@ -218,43 +169,39 @@
         path_to_settings = cmd[10]
         assert os.path.exists(path_to_settings)
         ans = {
             'summarypages_arguments': {'gracedb': event['graceid'],
                                        'no_ligo_skymap': True},
             'queue': 'Online_PE',
             'accounting_user': 'soichiro.morisaki',
-            'enforce_signal_duration': False
         }
         if host != 'gracedb.ligo.org':
             ans['queue'] = 'Online_PE_MDC'
+        else:
+            ans['accounting'] = 'ligo.prod.o4.cbc.pe.bilby'
         if mode == 'production':
             ans.update(
                 {'sampler_kwargs': {'naccept': 60, 'nlive': 500,
                                     'npool': 24, 'sample': 'acceptance-walk'},
                  'n_parallel': 2,
                  'request_cpus': 24,
                  'spline_calibration_nodes': 10,
                  'request_memory_generation': 8.0}
             )
-            if 1.465 < mc < 2.243:
+            if 0.6 < mc < 1.465:
+                assert 'lowspin_phenomd_fhigh1024_roq' in cmd
+                ans['sampler_kwargs']['naccept'] = 10
+            elif mc < 2.243:
                 assert 'phenompv2_bns_roq' in cmd
+            elif mc < 12:
+                assert 'low_q_phenompv2_roq' in cmd
             else:
-                path_to_mode = cmd[cmd.index("--cbc-likelihood-mode") + 1]
-                assert os.path.exists(path_to_mode)
-                with open(path_to_mode, 'r') as f:
-                    w = json.load(f)["likelihood_args"]["waveform_approximant"]
-                if 0.6 < mc < 1.465:
-                    assert w == "IMRPhenomD"
-                    ans['sampler_kwargs']['naccept'] = 10
-                elif mc < 11.033:
-                    assert w == "IMRPhenomPv2"
-                else:
-                    assert w == "IMRPhenomXPHM"
-                    ans['request_memory_generation'] = 36.0
-                    ans['request_memory'] = 16.0
+                assert 'phenomxphm_roq' in cmd
+                ans['request_memory_generation'] = 36.0
+                ans['request_memory'] = 16.0
         elif mode == 'fast_test' and mc < 3.9:
             ans['request_memory_generation'] = 8.0
         with open(path_to_settings, 'r') as f:
             assert json.load(f) == ans
 
         with open(os.path.join(rundir, 'bilby_config.ini'), 'w') as f:
             f.write(ini)
@@ -305,15 +252,15 @@
         with open(os.path.join(rundir, dag_filename), 'w') as f:
             f.write(dag_content)
 
     upload = Mock()
     monkeypatch.setattr('subprocess.run', _subprocess_run)
     monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', upload)
 
-    path_to_dag = inference._setup_dag_for_rapidpe(rundir, 'S1234', {})
+    path_to_dag = inference._setup_dag_for_rapidpe(rundir, 'S1234')
     with open(path_to_dag, 'r') as f:
         assert f.read() == dag_content
     upload.assert_called_once()
 
 
 @pytest.mark.parametrize('pipeline', ['lalinference', 'bilby', 'rapidpe'])
 def test_setup_dag_for_failure(monkeypatch, tmp_path, pipeline):
@@ -333,20 +280,20 @@
         'extra_attributes': {'SingleInspiral':
                              [{'mass1': 1.4, 'mass2': 1.4, 'mchirp': 1.2}],
                              'CoincInspiral': {'mchirp': 1}}
     }
     with pytest.raises(subprocess.CalledProcessError):
         if pipeline == 'lalinference':
             inference._setup_dag_for_lalinference(
-                b'coinc', rundir, event, 'S1234', {})
+                b'coinc', rundir, event, 'S1234')
         elif pipeline == 'bilby':
             inference._setup_dag_for_bilby(
                 (b'psd'), rundir, event, 'S1234', 'production')
         elif pipeline == 'rapidpe':
-            inference._setup_dag_for_rapidpe(rundir, 'S1234', {})
+            inference._setup_dag_for_rapidpe(rundir, 'S1234')
     if pipeline == 'bilby':
         assert upload.call_count == 1
     else:
         # For pipelines except for bilby, an ini file is uploaded before dag
         # generation, and hence the call count is 2.
         assert upload.call_count == 2
 
@@ -354,34 +301,32 @@
 @pytest.mark.parametrize(
     'pipeline', ['lalinference', 'bilby', 'rapidpe', 'my_awesome_pipeline'])
 def test_dag_prepare_task(monkeypatch, pipeline):
     sid = 'S1234'
     coinc = b'coinc'
     event = {'gpstime': 1187008882, 'graceid': 'G1234'}
     rundir = 'rundir'
-    frametype_dict = {'H1': 'H1_llhoft', 'L1': 'L1_llhoft'}
     path_to_dag = os.path.join(rundir, 'parameter_estimation.dag')
     kwargs = {'bilby_mode': 'production'}
 
     def mock_download(filename, gid):
         if filename == 'coinc.xml':
             return coinc
 
-    def _setup_dag_for_lalinference(c, r, e, s, f):
-        assert (c == coinc and r == rundir and e == event and s == sid and
-                f == frametype_dict)
+    def _setup_dag_for_lalinference(c, r, e, s):
+        assert (c == coinc and r == rundir and e == event and s == sid)
         return path_to_dag
 
     def _setup_dag_for_bilby(c, r, e, s, m):
         assert c == coinc and r == rundir and e == event and s == sid and \
             m == kwargs['bilby_mode']
         return path_to_dag
 
-    def _setup_dag_for_rapidpe(r, s, f):
-        assert r == rundir and s == sid and f == frametype_dict
+    def _setup_dag_for_rapidpe(r, s):
+        assert r == rundir and s == sid
         return path_to_dag
 
     def _subprocess_run(cmd, **kwargs):
         assert cmd == ['condor_submit_dag', '-no_submit', path_to_dag]
 
     mock_setup_dag_for_lalinference = \
         Mock(side_effect=_setup_dag_for_lalinference)
@@ -396,25 +341,25 @@
     monkeypatch.setattr('gwcelery.tasks.inference._setup_dag_for_bilby.run',
                         mock_setup_dag_for_bilby)
     monkeypatch.setattr('gwcelery.tasks.inference._setup_dag_for_rapidpe.run',
                         mock_setup_dag_for_rapidpe)
     monkeypatch.setattr('subprocess.run', _subprocess_run)
     if pipeline in ['lalinference', 'bilby', 'rapidpe']:
         inference.dag_prepare_task(
-            rundir, event, sid, pipeline, frametype_dict, **kwargs).delay()
+            rundir, event, sid, pipeline, **kwargs).delay()
         if pipeline == 'lalinference':
             mock_setup_dag_for_lalinference.assert_called_once()
         elif pipeline == 'bilby':
             mock_setup_dag_for_bilby.assert_called_once()
         elif pipeline == 'rapidpe':
             mock_setup_dag_for_rapidpe.assert_called_once()
     else:
         with pytest.raises(NotImplementedError):
             inference.dag_prepare_task(
-                rundir, event, sid, pipeline, frametype_dict).delay()
+                rundir, event, sid, pipeline).delay()
 
 
 @pytest.mark.parametrize(
     'exc,host',
     product(
         [condor.JobAborted(1, 'test'),
          condor.JobFailed(1, 'test'),
@@ -559,19 +504,24 @@
 
         else:
             paths = []
         for path in paths:
             with open(path, 'wb') as f:
                 f.write(b'result')
 
-        inference.dag_finished(rundir, sid, pipeline, **kwargs)
-
         if pipeline == 'rapidpe':
+            for event_pipeline in ['gstlal', 'pycbc']:
+                kwargs['event_pipeline'] = event_pipeline
+                inference.dag_finished(rundir, sid, pipeline, **kwargs)
+        else:
+            inference.dag_finished(rundir, sid, pipeline, **kwargs)
+
+        if pipeline == "rapidpe":
             # +1 corresponds to summary page link
-            assert upload.call_count == len(paths) + 1
+            assert upload.call_count == 2 * (len(paths) + 1)
         elif pipeline == 'bilby':
             # +1 corresponds to pesummary link
             assert upload.call_count == len(paths) + 1
             n = len(glob.glob(os.path.join(datadir, "*")))
             if host == "gracedb.ligo.org":
                 assert n == 2
             else:
@@ -594,14 +544,89 @@
 def test_start_pe(monkeypatch, tmp_path, pipeline):
     path_to_sub = 'pe.dag.condor.sub'
 
     @app.task
     def mock_task():
         return path_to_sub
 
+    def mock_condor_submit(path):
+        assert path == path_to_sub
+
+    if pipeline == 'rapidpe':
+        event_pipeline_info = {
+            'gstlal': {'sid': 'S1234', 'graceid': 'G1234'},
+            'pycbc': {'sid': 'S1235', 'graceid': 'G1235'}}
+        for event_pipeline in event_pipeline_info:
+            dag_prepare_task = Mock(return_value=mock_task.s())
+
+            condor_submit = Mock(side_effect=mock_condor_submit)
+            dag_finished = Mock()
+            monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', Mock())
+            monkeypatch.setattr('os.path.expanduser', Mock(
+                return_value=str(tmp_path)))
+            monkeypatch.setattr('gwcelery.tasks.inference.dag_prepare_task',
+                                dag_prepare_task)
+            monkeypatch.setattr(
+                    'gwcelery.tasks.condor.submit.run', condor_submit)
+            monkeypatch.setattr(
+                    'gwcelery.tasks.inference.dag_finished.run',
+                    dag_finished)
+
+            inference.start_pe({
+                'graceid': event_pipeline_info[event_pipeline]['graceid'],
+                'pipeline': event_pipeline},
+                event_pipeline_info[event_pipeline]['sid'], pipeline)
+            dag_prepare_task.assert_called_once()
+            condor_submit.assert_called_once()
+            dag_finished.assert_called_once()
+    else:
+        dag_prepare_task = Mock(return_value=mock_task.s())
+
+        condor_submit = Mock(side_effect=mock_condor_submit)
+        dag_finished = Mock()
+        monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', Mock())
+        monkeypatch.setattr('distutils.dir_util.mkpath',
+                            Mock(return_value=str(tmp_path)))
+        monkeypatch.setattr('gwcelery.tasks.inference.dag_prepare_task',
+                            dag_prepare_task)
+        monkeypatch.setattr('gwcelery.tasks.condor.submit.run', condor_submit)
+        monkeypatch.setattr(
+                'gwcelery.tasks.inference.dag_finished.run',
+                dag_finished)
+
+        inference.start_pe({'graceid': 'G1234'}, 'S1234', pipeline)
+        dag_prepare_task.assert_called_once()
+        condor_submit.assert_called_once()
+        dag_finished.assert_called_once()
+
+
+@pytest.mark.parametrize(
+    'host', ["gracedb-playground.ligo.org", "gracedb.ligo.org"])
+def test_bbh_rate_limit(monkeypatch, tmp_path, host):
+    monkeypatch.setitem(app.conf, 'gracedb_host', host)
+    monkeypatch.setattr('os.path.expanduser', Mock(return_value=str(tmp_path)))
+    event = {'gpstime': 1187008882, 'graceid': 'G1234',
+             'extra_attributes': {'CoincInspiral': {'mchirp': 20}}}
+    for i in range(6):
+        rundir = os.path.join(str(tmp_path), f"{i}/production")
+        os.makedirs(rundir)
+        os.mkdir(os.path.join(rundir, "data"))
+        with open(
+            os.path.join(rundir, "data/pe_generation_data_dump.pickle"), "wb"
+        ) as f:
+            f.write(b"test")
+        with open(os.path.join(rundir, "event.json"), "w") as f:
+            json.dump(event, f, indent=2)
+
+    path_to_sub = 'pe.dag.condor.sub'
+
+    @app.task
+    def mock_task():
+        return path_to_sub
+
     dag_prepare_task = Mock(return_value=mock_task.s())
 
     def mock_condor_submit(path):
         assert path == path_to_sub
 
     condor_submit = Mock(side_effect=mock_condor_submit)
     dag_finished = Mock()
@@ -610,11 +635,16 @@
                         Mock(return_value=str(tmp_path)))
     monkeypatch.setattr('gwcelery.tasks.inference.dag_prepare_task',
                         dag_prepare_task)
     monkeypatch.setattr('gwcelery.tasks.condor.submit.run', condor_submit)
     monkeypatch.setattr('gwcelery.tasks.inference.dag_finished.run',
                         dag_finished)
 
-    inference.start_pe({}, {'graceid': 'G1234'}, 'S1234', pipeline)
-    dag_prepare_task.assert_called_once()
-    condor_submit.assert_called_once()
-    dag_finished.assert_called_once()
+    inference.start_pe(event, 'S1234', 'bilby')
+    if host == "gracedb-playground.ligo.org":
+        dag_prepare_task.assert_not_called()
+        condor_submit.assert_not_called()
+        dag_finished.assert_not_called()
+    else:
+        dag_prepare_task.assert_called_once()
+        condor_submit.assert_called_once()
+        dag_finished.assert_called_once()
```

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_orchestrator.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_orchestrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
          ['H1', 'L1', 'V1'], 'S1234', ['LOW_SIGNIF_LOCKED']],
      ['label_added', 'GCN_PRELIM_SENT', 'CBC', 'gstlal', False, 1.e-9,
          ['H1', 'L1', 'V1'], 'S1234', ['SIGNIF_LOCKED']],
      ['label_added', 'LOW_SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-9,
          ['H1', 'L1', 'V1'], 'S1234', ['SIGNIF_LOCKED']],
      ['label_added', 'LOW_SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-9,
          ['H1', 'L1', 'V1'], 'S1234', []],
+     ['label_added', 'LOW_SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-5,
+         ['H1', 'L1', 'V1'], 'S1234', []],
      ['label_added', 'LOW_SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-10,
          ['H1', 'L1', 'V1'], 'S1234', ['EARLY_WARNING']],
      ['label_added', 'LOW_SIGNIF_PRELIM_SENT', 'CBC', 'gstlal', False, 1.e-9,
          ['H1', 'L1', 'V1'], 'S1234', ['EM_SelectedConfident']],
      ['label_added', 'LOW_SIGNIF_PRELIM_SENT', 'CBC', 'gstlal', False, 1.e-7,
          ['H1', 'L1', 'V1'], 'S1234', ['EM_Selected']],
      ['new', '', 'CBC', 'gstlal', False, 1.e-9, ['H1', 'L1'], 'S1234',
@@ -73,15 +75,15 @@
             'search': (
                 'EarlyWarning' if alert_label == 'EARLY_WARNING'
                 else 'AllSky'
             ),
             'graceid': 'G1234',
             'offline': offline,
             'far': far,
-            'gpstime': 1234,
+            'gpstime': 1234.,
             'extra_attributes': {},
             'labels': ['PASTRO_READY', 'EMBRIGHT_READY', 'SKYMAP_READY']
         }
         if pipeline == 'gstlal':
             # Simulate subthreshold triggers for gstlal. Subthreshold triggers
             # do not contribute to the significance estimate. The way that we
             # can tell that a subthreshold trigger is present is that the chisq
@@ -151,15 +153,14 @@
         alert_label == 'LOW_SIGNIF_PRELIM_SENT' and \
         'EM_SelectedConfident' in superevent_labels else \
         Mock(return_value=(('skymap', 'skymap-filename'),
                            ('em-bright', 'em-bright-filename'),
                            ('p-astro', 'p-astro-filename')))
     gcn_send = Mock()
     alerts_send = Mock()
-    query_data = Mock()
     setup_dag = Mock()
     start_pe = Mock()
     create_voevent = Mock(return_value='S1234-1-Preliminary.xml')
     create_label = Mock()
     create_tag = Mock()
     select_preferred_event_task = Mock(return_value=get_event('G1234'))
     update_superevent_task = Mock()
@@ -203,16 +204,14 @@
                         create_voevent)
     monkeypatch.setattr('gwcelery.tasks.gracedb.get_superevent._orig_run',
                         get_superevent)
     monkeypatch.setattr('gwcelery.tasks.circulars.create_initial_circular.run',
                         create_initial_circular)
     monkeypatch.setattr('gwcelery.tasks.circulars.create_emcoinc_circular.run',
                         create_emcoinc_circular)
-    monkeypatch.setattr('gwcelery.tasks.inference.query_data.run',
-                        query_data)
     monkeypatch.setattr('gwcelery.tasks.inference._setup_dag_for_bilby.run',
                         setup_dag)
     monkeypatch.setattr('gwcelery.tasks.inference.start_pe.run',
                         start_pe)
     monkeypatch.setattr('gwcelery.tasks.gracedb.create_label._orig_run',
                         create_label)
     monkeypatch.setattr(
@@ -291,15 +290,15 @@
             gcn_send.assert_not_called()
             create_tag.assert_not_called()
             create_initial_circular.assert_not_called()
             check_high_profile.assert_not_called()
         else:
             annotate_fits.assert_called_once()
             update_superevent_task.assert_called_once_with(
-                'S1234', preferred_event='G1234'
+                'S1234', preferred_event='G1234', t_0=1234.
             )
             expose.assert_called_once_with('S1234')
             create_tag.assert_has_calls(
                 [call('S1234-1-Preliminary.xml', 'public', 'S1234'),
                  call('em-bright-filename', 'public', 'S1234'),
                  call('p-astro-filename', 'public', 'S1234'),
                  call('skymap-filename', 'public', 'S1234')],
@@ -313,14 +312,16 @@
                 ('EARLY_WARNING' in superevent_labels):
             expose.assert_not_called()
             alerts_send.assert_not_called()
             gcn_send.assert_not_called()
             create_tag.assert_not_called()
             create_initial_circular.assert_not_called()
             check_high_profile.assert_not_called()
+        elif far > 3.8e-7:
+            check_high_profile.assert_not_called()
         else:
             annotate_fits.assert_called_once()
             # no superevent clean up needed
             update_superevent_task.assert_not_called()
             # no circular creation for less-significant alerts
             create_initial_circular.assert_not_called()
             create_emcoinc_circular.assert_not_called()
@@ -340,23 +341,22 @@
             check_high_profile.assert_not_called()
         else:
             # check alert type is less-significant
             _files, _superevent, _alert_type = alerts_send.call_args.args
             assert _alert_type == 'less-significant'
 
     if alert_type == 'new' and group == 'CBC':
-        query_data.assert_called_once()
         threshold = (
             app.conf['preliminary_alert_far_threshold']['cbc'] /
             app.conf['preliminary_alert_trials_factor']['cbc']
         )
         if far <= threshold:
             assert start_pe.call_count == 2
             call_args = [
-                call_args.args[1:] for call_args in start_pe.call_args_list]
+                call_args.args for call_args in start_pe.call_args_list]
             assert all(
                 [(get_event('G1234'), superevent_id, pipeline) in call_args
                  for pipeline in ('bilby', 'rapidpe')])
         else:
             start_pe.assert_not_called()
 
     if alert_type == 'new':
@@ -418,15 +418,15 @@
 def _mock_get_log(se_id):
     logs = [{'tag_names': ['sky_loc', 'public'],
              'filename': 'foobar.multiorder.fits',
              'file_version': 0},
             {'tag_names': ['em_bright'],
              'filename': 'em_bright.json',
              'file_version': 0},
-            {'tag_names': ['p_astro'],
+            {'tag_names': ['p_astro', 'public'],
              'filename': 'p_astro.json',
              'file_version': 0}]
     if se_id == 'S2468':
         logs.append({'tag_names': ['sky_loc', 'ext_coinc'],
                      'filename': 'combined-ext.multiorder.fits',
                      'file_version': 0})
     return logs
@@ -715,52 +715,55 @@
             superevent_id,
             'preliminary'
         ).get()
         mock_alert.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    'far,event',
-    [[1, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'AllSky'}],
-     [1e-30, {'gpstime': 1187008882, 'group': 'Burst', 'search': 'AllSky'}],
-     [1e-30, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'MDC'}],
+    'far,event,pe_pipeline',
+    [[1, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'AllSky'}, 'bilby'],
+     [1e-30, {'gpstime': 1187008882, 'group': 'Burst', 'search': 'AllSky'},
+         'bilby'],
+     [1e-30, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'MDC'},
+         'bilby'],
+     [1e-30, {'gpstime': 1187008882, 'group': 'CBC',
+              'search': 'AllSky', 'pipeline': 'gstlal'}, 'bilby'],
      [1e-30, {'gpstime': 1187008882, 'group': 'CBC',
-              'search': 'AllSky', 'pipeline': 'gstlal'}],
+              'search': 'AllSky', 'pipeline': 'pycbc'}, 'bilby'],
+     [1, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'AllSky'},
+         'rapidpe'],
+     [1e-30, {'gpstime': 1187008882, 'group': 'Burst', 'search': 'AllSky'},
+         'rapidpe'],
+     [1e-30, {'gpstime': 1187008882, 'group': 'CBC', 'search': 'MDC'},
+         'rapidpe'],
      [1e-30, {'gpstime': 1187008882, 'group': 'CBC',
-              'search': 'AllSky', 'pipeline': 'pycbc'}]]
+              'search': 'AllSky', 'pipeline': 'gstlal'}, 'rapidpe'],
+     [1e-30, {'gpstime': 1187008882, 'group': 'CBC',
+              'search': 'AllSky', 'pipeline': 'pycbc'}, 'rapidpe']]
 )
-def test_parameter_estimation(monkeypatch, far, event):
+def test_parameter_estimation(monkeypatch, far, event, pe_pipeline):
     superevent_id = 'S1234'
-    frametype_dict = {'H1': 'H1_llhoft', 'L1': 'L1_llhoft', 'V1': 'V1_llhoft'}
     mock_upload = Mock()
-    mock_query_data = Mock(return_value=frametype_dict)
     mock_start_pe = Mock()
     monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', mock_upload)
-    monkeypatch.setattr(
-        'gwcelery.tasks.inference.query_data.run', mock_query_data)
     monkeypatch.setattr('gwcelery.tasks.inference.start_pe.run', mock_start_pe)
 
     orchestrator.parameter_estimation.delay(
-        far_event=(far, event), superevent_id=superevent_id)
+        far_event=(far, event), superevent_id=superevent_id,
+        pe_pipeline=pe_pipeline)
 
     threshold = (app.conf['significant_alert_far_threshold']['cbc'] /
                  app.conf['significant_alert_trials_factor']['cbc'])
     if (
         far <= threshold and event['group'] == 'CBC' and
         event['search'] != 'MDC'
     ):
-        mock_query_data.assert_called_once()
         mock_start_pe.assert_any_call(
-            frametype_dict, event, superevent_id, 'bilby')
-        if event['pipeline'] == 'gstlal':
-            mock_start_pe.assert_any_call(
-                frametype_dict, event, superevent_id, 'rapidpe')
-            assert mock_start_pe.call_count == 2
-        else:
-            assert mock_start_pe.call_count == 1
+            event, superevent_id, pe_pipeline)
+        assert mock_start_pe.call_count == 1
     else:
         mock_upload.assert_called_once()
 
 
 @pytest.mark.parametrize(
     "superevent_labels,block_by_labels",
     [
```

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_p_astro.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_raven.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_raven.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_rrt_utils.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_skymaps.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tasks_superevents.py` & `gwcelery-2.1.2/gwcelery/tests/test_tasks_superevents.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,14 +404,16 @@
 @pytest.mark.parametrize(
     'group,pipeline,search,offline,far,instruments,labels,expected_result,'
     'expected_result_less_significant',
     [['CBC', 'gstlal', 'AllSky', False, 1.e-10, 'H1',  # complete significant
         ['PASTRO_READY', 'SKYMAP_READY', 'EMBRIGHT_READY'], True, True],
      ['CBC', 'gstlal', 'AllSky', False, 1.e-6, 'H1',  # complete less-signif
         ['PASTRO_READY', 'SKYMAP_READY', 'EMBRIGHT_READY'], False, True],
+     ['CBC', 'gstlal', 'AllSky', False, 2.5e-5, 'H1',  # complete noise
+        ['PASTRO_READY', 'SKYMAP_READY', 'EMBRIGHT_READY'], False, False],
      ['CBC', 'gstlal', 'AllSky', False, 1.e-6, 'H1',  # incomplete less-signif
         ['PASTRO_READY', 'SKYMAP_READY'], False, False],
      ['CBC', 'gstlal', 'AllSky', False, 1.e-6, 'H1,L1',  # incomplete CBC
         ['EMBRIGHT_READY'], False, False],
      ['Burst', 'cwb', 'AllSky', False, 1e-15, 'H1,L1',  # complete Burst
         ['SKYMAP_READY'], True, True],
      ['Burst', 'cwb', 'AllSky', False, 1e-15, 'H1,L1',  # incomplete Burst
```

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tempfile.py` & `gwcelery-2.1.2/gwcelery/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tools_condor.py` & `gwcelery-2.1.2/gwcelery/tests/test_tools_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tools_condor_submit_helper.py` & `gwcelery-2.1.2/gwcelery/tests/test_tools_condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tools_flask.py` & `gwcelery-2.1.2/gwcelery/tests/test_tools_flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_tools_nagios.py` & `gwcelery-2.1.2/gwcelery/tests/test_tools_nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tests/test_views.py` & `gwcelery-2.1.2/gwcelery/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,20 @@
     mock_get_event.assert_not_called()
     mock_preliminary_alert.assert_not_called()
 
 
 def test_send_preliminary_gcn_post(client, monkeypatch):
     """Test send_update_gcn endpoint with complete form data."""
     mock_update_superevent = Mock()
-    mock_event = Mock()
+    mock_event = MagicMock()
+    event_dict_spoofer = {
+        'pipeline': 'gstlal',
+        'gpstime': 12345.
+    }
+    mock_event.__getitem__.side_effect = event_dict_spoofer.__getitem__
     mock_superevent = Mock()
     mock_get_event = Mock(return_value=mock_event)
     mock_get_superevent = Mock(return_value=mock_superevent)
     mock_preliminary_alert = Mock()
     monkeypatch.setattr(
         'gwcelery.tasks.gracedb.update_superevent.run',
         mock_update_superevent)
@@ -64,16 +69,16 @@
     response = client.post(url_for('send_preliminary_gcn'), data={
         'superevent_id': 'MS190208a',
         'event_id': 'M12345'})
     assert HTTP_STATUS_CODES[response.status_code] == 'Found'
     assert get_flashed_messages() == [
         'Queued preliminary alert for MS190208a.']
     mock_update_superevent.assert_called_once_with(
-        'MS190208a', preferred_event='M12345')
-    mock_get_event.assert_called_once_with('M12345')
+        'MS190208a', preferred_event='M12345', t_0=12345.)
+    mock_get_event.assert_has_calls([call('M12345'), call('M12345')])
     mock_get_superevent.assert_called_once_with('MS190208a')
 
     alert = {
         'uid': 'MS190208a',
         'object': mock_superevent
     }
     mock_preliminary_alert.assert_called_once_with(mock_event, alert,
@@ -85,14 +90,15 @@
     """Test changing preferred event with complete form data."""
     mock_update_superevent = Mock()
     mock_add_pipeline_pref_event = Mock()
     mock_event = MagicMock()
     mock_superevent = MagicMock()
     event_dict_spoofer = {
         'pipeline': 'gstlal',
+        'gpstime': 12345.
     }
     superevent_dict_spoofer = {
         'pipeline_preferred_events': {'gstlal': {'graceid': 'M12345'}}
     }
     mock_event.__getitem__.side_effect = event_dict_spoofer.__getitem__
     mock_superevent.__getitem__.side_effect = \
         superevent_dict_spoofer.__getitem__
@@ -118,15 +124,15 @@
     response = client.post(url_for('change_preferred_event'), data={
         'superevent_id': 'MS190208a',
         'event_id': 'M12345'})
     assert HTTP_STATUS_CODES[response.status_code] == 'Found'
     assert get_flashed_messages() == [
         'Changed preferred event for MS190208a.']
     mock_update_superevent.assert_called_once_with(
-        'MS190208a', preferred_event='M12345')
+        'MS190208a', preferred_event='M12345', t_0=12345.)
     mock_get_event.assert_called_once_with('M12345')
     mock_get_superevent.assert_called_once_with('MS190208a')
     mock_preliminary_alert.assert_called_once_with([mock_superevent,
                                                    mock_event], 'MS190208a',
                                                    initiate_voevent=False)
     # This should only be called if the new preferred event is not already a
     # pipeline preferred event
@@ -137,15 +143,15 @@
                                                               monkeypatch):
     """Test changing preferred event to event that isn't a pipeline preferred
     event with complete form data."""
     mock_update_superevent = Mock()
     mock_add_pipeline_pref_event = Mock()
     mock_event = MagicMock()
     mock_superevent = MagicMock()
-    event_dict_spoofer = {'pipeline': 'gstlal'}
+    event_dict_spoofer = {'pipeline': 'gstlal', 'gpstime': 12345.}
     superevent_dict_spoofer = {
         'pipeline_preferred_events': {'gstlal': {'graceid': 'M12344'}}
     }
     mock_event.__getitem__.side_effect = event_dict_spoofer.__getitem__
     mock_superevent.__getitem__.side_effect = \
         superevent_dict_spoofer.__getitem__
     mock_get_event = Mock(return_value=mock_event)
@@ -170,15 +176,15 @@
     response = client.post(url_for('change_preferred_event'), data={
         'superevent_id': 'MS190208a',
         'event_id': 'M12345'})
     assert HTTP_STATUS_CODES[response.status_code] == 'Found'
     assert get_flashed_messages() == [
         'Changed preferred event for MS190208a.']
     mock_update_superevent.assert_called_once_with(
-        'MS190208a', preferred_event='M12345')
+        'MS190208a', preferred_event='M12345', t_0=12345.)
     mock_get_event.assert_called_once_with('M12345')
     mock_get_superevent.assert_called_once_with('MS190208a')
     mock_preliminary_alert.assert_called_once_with([mock_superevent,
                                                    mock_event], 'MS190208a',
                                                    initiate_voevent=False)
     # This should only be called if the new preferred event is not already a
     # pipeline preferred event
```

### Comparing `gwcelery-2.1.1/gwcelery/tools/condor.py` & `gwcelery-2.1.2/gwcelery/tools/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tools/condor_submit_helper.py` & `gwcelery-2.1.2/gwcelery/tools/condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tools/flask.py` & `gwcelery-2.1.2/gwcelery/tools/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/tools/nagios.py` & `gwcelery-2.1.2/gwcelery/tools/nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/util/cmdline.py` & `gwcelery-2.1.2/gwcelery/util/cmdline.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/util/resources.py` & `gwcelery-2.1.2/gwcelery/util/resources.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/util/tempfile.py` & `gwcelery-2.1.2/gwcelery/util/tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/views.py` & `gwcelery-2.1.2/gwcelery/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,23 +204,30 @@
 
 @app.route('/send_preliminary_gcn', methods=['POST'])
 def send_preliminary_gcn():
     """Handle submission of preliminary alert form."""
     keys = ('superevent_id', 'event_id')
     superevent_id, event_id, *_ = tuple(request.form.get(key) for key in keys)
     if superevent_id and event_id:
+        try:
+            event = gracedb.get_event(event_id)
+        except HTTPError as e:
+            flash(f'No action performed. GraceDB query for {event_id} '
+                  f'returned error code {e.response.status_code}.', 'danger')
+            return redirect(url_for('index'))
+
         (
             gracedb.upload.s(
                 None, None, superevent_id,
                 'User {} queued a Preliminary alert through the dashboard.'
                 .format(request.remote_user or '(unknown)'),
                 tags=['em_follow'])
             |
             gracedb.update_superevent.si(
-                superevent_id, preferred_event=event_id)
+                superevent_id, preferred_event=event_id, t_0=event['gpstime'])
             |
             group(
                 gracedb.get_superevent.si(superevent_id),
 
                 gracedb.get_event.si(event_id)
             )
             |
@@ -256,15 +263,16 @@
             gracedb.upload.s(
                 None, None, superevent_id,
                 celery_app.conf['views_manual_preferred_event_log_message']
                 .format(request.remote_user or '(unknown)', event_id),
                 tags=['em_follow'])
             |
             gracedb.update_superevent.si(
-                superevent_id, preferred_event=event_id)
+                superevent_id, preferred_event=event_id,
+                t_0=event['gpstime'])
             |
             _construct_igwn_alert_and_send_prelim_alert.si(
                 [superevent, event],
                 superevent_id,
                 initiate_voevent=False
             )
         ).delay()
```

### Comparing `gwcelery-2.1.1/gwcelery/voevent/bootsteps.py` & `gwcelery-2.1.2/gwcelery/voevent/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/voevent/logging.py` & `gwcelery-2.1.2/gwcelery/voevent/logging.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/voevent/signals.py` & `gwcelery-2.1.2/gwcelery/voevent/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/voevent/subscriber.py` & `gwcelery-2.1.2/gwcelery/voevent/subscriber.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/gwcelery/voevent/util.py` & `gwcelery-2.1.2/gwcelery/voevent/util.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.1/pyproject.toml` & `gwcelery-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwcelery"
-version = "2.1.1"
+version = "2.1.2"
 description = "Low-latency pipeline for annotating IGWN events"
 readme = "README.rst"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Cody Messick <cody.messick@ligo.org>",
     "Geoffrey Mo <geoffrey.mo@ligo.org>",
     "Leo Singer <leo.singer@ligo.org>"
@@ -50,15 +50,15 @@
 "Bug Tracker" = "https://git.ligo.org/emfollow/gwcelery/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 adc-streaming = ">=2.3.0"  # https://github.com/astronomy-commons/adc-streaming/pull/62
 astropy = ">=4.3.1,!=5.3"  # https://github.com/astropy/astropy/issues/11879, https://github.com/gwpy/gwpy/issues/1629
 bilby = ">=2.1.1"
-bilby_pipe = "==1.0.10"
+bilby_pipe = ">=1.1.1"
 celery = {version = ">=5.1", extras = ["redis"]}
 ciecplib = {version = "*", extras = ["kerberos"]}  # for renew-cert.sh
 click = ">=7"
 comet = "*"
 confluent-kafka = "^1.9.2"
 dnspython = "*"  # silence "DNS: dnspython not found. Can not use SRV lookup." warning from SleekXMPP
 flask = ">=2.2"
@@ -70,15 +70,15 @@
 healpy = "*"
 hop-client = ">=0.7.0"  # https://github.com/scimma/hop-client/pull/176
 igwn-alert = ">=0.2.2"
 igwn-gwalert-schema = "^1.0.0"
 imapclient = "*"
 importlib-metadata = { version = "*"}
 jinja2 = ">=2.11.2"  # https://github.com/pallets/jinja/issues/1168
-lalsuite = ">=6.82"  # https://git.ligo.org/lscsoft/lalsuite/-/issues/414
+lalsuite = ">=7.15"  # https://git.ligo.org/lscsoft/lalsuite/-/merge_requests/2120
 ligo-followup-advocate = ">=1.2.3"
 ligo-gracedb = ">=2.7.5"  # https://git.ligo.org/lscsoft/gracedb-client/-/issues/28
 ligo-raven = ">=3.2"
 ligo-segments = "*"
 "ligo.em-bright" = ">=1.1.3"  # https://git.ligo.org/emfollow/em-properties/em-bright/-/issues/34
 "ligo.skymap" = ">=1.0.4"  # https://git.ligo.org/lscsoft/ligo.skymap/-/merge_requests/299
 lscsoft-glue = "*"
@@ -88,17 +88,17 @@
 numpy = "*"
 p_astro = ">=1.0.1"  # https://git.ligo.org/lscsoft/p-astro/-/merge_requests/40
 pesummary = ">=1.0.0"  # https://git.ligo.org/computing/sccb/-/issues/1182
 pygcn = ">=1.0.1"
 python-ligo-lw = "^1.8.3"
 pyxdg = "*"
 rapid-pe = ">=0.1.0,<0.2.0"  # https://git.ligo.org/computing/sccb/-/issues/1154
-rapidpe-rift-pipe = ">=0.3.0"  # https://git.ligo.org/computing/sccb/-/issues/1214
+rapidpe-rift-pipe = ">=0.5.1"  # https://git.ligo.org/computing/sccb/-/issues/1231
 redis = "!=4.5.2,!=4.5.3"  # https://git.ligo.org/emfollow/gwcelery/-/issues/556
-RIFT = ">=0.0.15.7"
+RIFT = ">=0.0.15.8"
 scipy = "<1.10"  # https://github.com/astropy/astropy/issues/14230
 safe-netrc = "*"
 sentry-sdk = {version = "*", extras = ["flask", "tornado"]}
 service-identity = "*"  # We don't actually use this package, but it silences some annoying warnings from twistd.
 voeventlib = ">=1.2"
 werkzeug = ">=0.15.0"  # for werkzeug.middleware.proxy_fix.ProxyFix
 zstandard = "*"  # for task compression
```

### Comparing `gwcelery-2.1.1/PKG-INFO` & `gwcelery-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwcelery
-Version: 2.1.1
+Version: 2.1.2
 Summary: Low-latency pipeline for annotating IGWN events
 Home-page: https://git.ligo.org/emfollow/gwcelery
 License: GPL-2.0+
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -17,19 +17,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: GWSkyNet (>=2.3.0)
-Requires-Dist: RIFT (>=0.0.15.7)
+Requires-Dist: RIFT (>=0.0.15.8)
 Requires-Dist: adc-streaming (>=2.3.0)
 Requires-Dist: astropy (>=4.3.1,!=5.3)
 Requires-Dist: bilby (>=2.1.1)
-Requires-Dist: bilby_pipe (==1.0.10)
+Requires-Dist: bilby_pipe (>=1.1.1)
 Requires-Dist: celery[redis] (>=5.1)
 Requires-Dist: ciecplib[kerberos]
 Requires-Dist: click (>=7)
 Requires-Dist: comet
 Requires-Dist: confluent-kafka (>=1.9.2,<2.0.0)
 Requires-Dist: dnspython
 Requires-Dist: fastavro (>=1.6.1,<2.0.0) ; extra == "test"
@@ -41,15 +41,15 @@
 Requires-Dist: healpy
 Requires-Dist: hop-client (>=0.7.0)
 Requires-Dist: igwn-alert (>=0.2.2)
 Requires-Dist: igwn-gwalert-schema (>=1.0.0,<2.0.0)
 Requires-Dist: imapclient
 Requires-Dist: importlib-metadata
 Requires-Dist: jinja2 (>=2.11.2)
-Requires-Dist: lalsuite (>=6.82)
+Requires-Dist: lalsuite (>=7.15)
 Requires-Dist: ligo-followup-advocate (>=1.2.3)
 Requires-Dist: ligo-gracedb (>=2.7.5)
 Requires-Dist: ligo-raven (>=3.2)
 Requires-Dist: ligo-rrt-chat (>=0.1.1)
 Requires-Dist: ligo-segments
 Requires-Dist: ligo.em-bright (>=1.1.3)
 Requires-Dist: ligo.skymap (>=1.0.4)
@@ -65,15 +65,15 @@
 Requires-Dist: pytest-celery ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-flask ; extra == "test"
 Requires-Dist: pytest-socket ; extra == "test"
 Requires-Dist: python-ligo-lw (>=1.8.3,<2.0.0)
 Requires-Dist: pyxdg
 Requires-Dist: rapid-pe (>=0.1.0,<0.2.0)
-Requires-Dist: rapidpe-rift-pipe (>=0.3.0)
+Requires-Dist: rapidpe-rift-pipe (>=0.5.1)
 Requires-Dist: redis (!=4.5.2,!=4.5.3)
 Requires-Dist: safe-netrc
 Requires-Dist: scipy (<1.10)
 Requires-Dist: sentry-sdk[flask,tornado]
 Requires-Dist: service-identity
 Requires-Dist: sphinx (>=4.0,<=5.3.0) ; extra == "doc"
 Requires-Dist: voeventlib (>=1.2)
```

