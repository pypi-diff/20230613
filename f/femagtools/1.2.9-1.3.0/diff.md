# Comparing `tmp/femagtools-1.2.9.tar.gz` & `tmp/femagtools-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femagtools-1.2.9.tar", last modified: Fri May 26 13:42:30 2023, max compression
+gzip compressed data, was "femagtools-1.3.0.tar", last modified: Tue Jun 13 07:53:59 2023, max compression
```

## Comparing `femagtools-1.2.9.tar` & `femagtools-1.3.0.tar`

### file list

```diff
@@ -1,185 +1,188 @@
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.290895 femagtools-1.2.9/
--rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.2.9/LICENSE
--rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.2.9/MANIFEST.in
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-05-26 13:42:30.289895 femagtools-1.2.9/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.2.9/README.md
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.271895 femagtools-1.2.9/femagtools/
--rw-r--r--   0 tar        (210) tar        (210)     1630 2023-05-26 13:39:54.000000 femagtools-1.2.9/femagtools/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/airgap.py
--rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/amazon.py
--rw-r--r--   0 tar        (210) tar        (210)     9741 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/amela.py
--rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    68684 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/bch.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/bchxml.py
--rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/condor.py
--rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/config.py
--rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/convert.py
--rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dakota.py
--rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dakota_femag.py
--rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dakotaout.py
--rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.2.9/femagtools/docker.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.274895 femagtools-1.2.9/femagtools/dxfsl/
--rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    52503 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/area.py
--rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/conv.py
--rw-r--r--   0 tar        (210) tar        (210)    18787 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/converter.py
--rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/corner.py
--rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/dumprenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    23233 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/fslrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)     9835 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/functions.py
--rw-r--r--   0 tar        (210) tar        (210)   132506 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/geom.py
--rw-r--r--   0 tar        (210) tar        (210)    27661 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/machine.py
--rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/plotrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    43088 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/dxfsl/shape.py
--rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/erg.py
--rw-r--r--   0 tar        (210) tar        (210)    40675 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/femag.py
--rw-r--r--   0 tar        (210) tar        (210)     7415 2023-05-17 15:12:10.000000 femagtools-1.2.9/femagtools/forcedens.py
--rw-r--r--   0 tar        (210) tar        (210)    28180 2023-02-21 19:53:03.000000 femagtools-1.2.9/femagtools/fsl.py
--rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/getset.py
--rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/gmsh.py
--rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/google.py
--rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/grid.py
--rw-r--r--   0 tar        (210) tar        (210)    41556 2023-04-13 07:48:25.000000 femagtools-1.2.9/femagtools/isa7.py
--rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/jcf2msh.py
--rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/jhb.py
--rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/job.py
--rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.2.9/femagtools/losscoeffs.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.275895 femagtools-1.2.9/femagtools/machine/
--rw-r--r--   0 tar        (210) tar        (210)     7392 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/machine/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5680 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/machine/effloss.py
--rw-r--r--   0 tar        (210) tar        (210)    34847 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/machine/im.py
--rwxr-xr-x   0 tar        (210) tar        (210)    30721 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/machine/pm.py
--rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/machine/sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    26367 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/machine/sm.py
--rw-r--r--   0 tar        (210) tar        (210)    16188 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/machine/utils.py
--rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.2.9/femagtools/magnet.py
--rw-r--r--   0 tar        (210) tar        (210)    38043 2023-02-16 09:09:33.000000 femagtools-1.2.9/femagtools/mcv.py
--rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/me.py
--rw-r--r--   0 tar        (210) tar        (210)    14106 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/model.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.276895 femagtools-1.2.9/femagtools/moo/
--rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/moo/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/moo/algorithm.py
--rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/moo/population.py
--rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/moo/problem.py
--rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/moproblem.py
--rw-r--r--   0 tar        (210) tar        (210)     8265 2023-04-05 06:37:05.000000 femagtools-1.2.9/femagtools/multiproc.py
--rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/mxw2msh.py
--rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/nc.py
--rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/netlist.py
--rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/ntib.py
--rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.2.9/femagtools/opt.py
--rw-r--r--   0 tar        (210) tar        (210)    18733 2023-04-05 06:37:05.000000 femagtools-1.2.9/femagtools/parstudy.py
--rw-r--r--   0 tar        (210) tar        (210)    58201 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/plot.py
--rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/poc.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.283895 femagtools-1.2.9/femagtools/templates/
--rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/FE-losses.mako
--rw-r--r--   0 tar        (210) tar        (210)      242 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/airgapinduc.mako
--rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.2.9/femagtools/templates/asyn_motor.mako
--rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.2.9/femagtools/templates/basic_modpar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/calc_field_ts.mako
--rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/cogg_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/colorgrad.mako
--rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/com_motor_sim.mako
--rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/conduct-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      437 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/connect_models.mako
--rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/cu_losses.mako
--rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/ec-rotorbar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/fe-contr.mako
--rw-r--r--   0 tar        (210) tar        (210)     4289 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/gen_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/inductances.mako
--rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/ld_lq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/leak_dist_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/leak_evol_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/leak_tooth_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnet-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetFC2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1372 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIron.mako
--rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIron2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIron3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIron4.mako
--rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIron5.mako
--rw-r--r--   0 tar        (210) tar        (210)     2208 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetIronV.mako
--rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetSector.mako
--rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetSectorLinear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetShell.mako
--rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/magnetShell2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/mesh-airgap.mako
--rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/modal_analysis.mako
--rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/mult_cal_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/new_model.mako
--rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/noloadflux-rot.mako
--rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/noloadflux.mako
--rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/noloadfluxdc.mako
--rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/open.mako
--rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/plots.mako
--rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/pm_sym_f_cur.mako
--rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/pm_sym_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/pm_sym_loss.mako
--rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/psd_psq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/ring.mako
--rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.2.9/femagtools/templates/rot_hsm.mako
--rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.2.9/femagtools/templates/rotorAsyn.mako
--rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/rotorKs2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/rotor_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.2.9/femagtools/templates/rotor_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/shortcircuit.mako
--rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/srm.mako
--rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/stator1.mako
--rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/stator2.mako
--rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/stator3Linear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/stator4.mako
--rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/statorBG.mako
--rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/statorRing.mako
--rw-r--r--   0 tar        (210) tar        (210)     4073 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/templates/statorRotor3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/templates/stator_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)     1716 2023-05-26 13:39:42.000000 femagtools-1.2.9/femagtools/templates/torq_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.2.9/femagtools/tks.py
--rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.2.9/femagtools/ts.py
--rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/vbf.py
--rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.2.9/femagtools/vtu.py
--rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.2.9/femagtools/windings.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.272895 femagtools-1.2.9/femagtools.egg-info/
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     4861 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/SOURCES.txt
--rw-r--r--   0 tar        (210) tar        (210)        1 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/dependency_links.txt
--rw-r--r--   0 tar        (210) tar        (210)      191 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/entry_points.txt
--rw-r--r--   0 tar        (210) tar        (210)      144 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/requires.txt
--rw-r--r--   0 tar        (210) tar        (210)       11 2023-05-26 13:42:30.000000 femagtools-1.2.9/femagtools.egg-info/top_level.txt
--rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.2.9/pyproject.toml
--rw-r--r--   0 tar        (210) tar        (210)       38 2023-05-26 13:42:30.290895 femagtools-1.2.9/setup.cfg
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-26 13:42:30.289895 femagtools-1.2.9/tests/
--rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_airgap_induction.py
--rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_amela.py
--rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_bchreader.py
--rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_convert.py
--rw-r--r--   0 tar        (210) tar        (210)     1142 2023-05-26 13:39:42.000000 femagtools-1.2.9/tests/test_effloss.py
--rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_erg.py
--rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.2.9/tests/test_femag.py
--rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_forcedens.py
--rwxr-xr-x   0 tar        (210) tar        (210)    16079 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_fsl.py
--rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_im.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_isa7.py
--rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_jhb.py
--rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_job.py
--rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.2.9/tests/test_losscoeffs.py
--rwxr-xr-x   0 tar        (210) tar        (210)    12906 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_machine.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_magncurv.py
--rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_magnet.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_mcvreader.py
--rwxr-xr-x   0 tar        (210) tar        (210)     3922 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_mcvwriter.py
--rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_me.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_model.py
--rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_nc.py
--rw-r--r--   0 tar        (210) tar        (210)     1323 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_parident.py
--rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.2.9/tests/test_parstudy.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_pocfile.py
--rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.2.9/tests/test_sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    83524 2023-05-26 13:39:42.000000 femagtools-1.2.9/tests/test_sm.py
--rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.2.9/tests/test_tksreader.py
--rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_ts.py
--rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_vbfreader.py
--rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.2.9/tests/test_vtu.py
--rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.2.9/tests/test_windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.619754 femagtools-1.3.0/
+-rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.3.0/LICENSE
+-rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.3.0/MANIFEST.in
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-06-13 07:53:59.619754 femagtools-1.3.0/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.3.0/README.md
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.604755 femagtools-1.3.0/femagtools/
+-rw-r--r--   0 tar        (210) tar        (210)     1630 2023-06-13 07:52:35.000000 femagtools-1.3.0/femagtools/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/airgap.py
+-rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/amazon.py
+-rw-r--r--   0 tar        (210) tar        (210)     9741 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    68745 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/bch.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/bchxml.py
+-rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/condor.py
+-rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/config.py
+-rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dakota.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dakota_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dakotaout.py
+-rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.3.0/femagtools/docker.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.605754 femagtools-1.3.0/femagtools/dxfsl/
+-rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    52503 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/area.py
+-rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/conv.py
+-rw-r--r--   0 tar        (210) tar        (210)    18787 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/converter.py
+-rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/corner.py
+-rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/dumprenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    23233 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/fslrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)     9835 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/functions.py
+-rw-r--r--   0 tar        (210) tar        (210)   132506 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/geom.py
+-rw-r--r--   0 tar        (210) tar        (210)    27661 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/machine.py
+-rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/plotrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    43088 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/dxfsl/shape.py
+-rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/erg.py
+-rw-r--r--   0 tar        (210) tar        (210)    41410 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     7415 2023-05-17 15:12:10.000000 femagtools-1.3.0/femagtools/forcedens.py
+-rw-r--r--   0 tar        (210) tar        (210)    30964 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/getset.py
+-rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/gmsh.py
+-rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/google.py
+-rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/grid.py
+-rw-r--r--   0 tar        (210) tar        (210)    41556 2023-04-13 07:48:25.000000 femagtools-1.3.0/femagtools/isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/jcf2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.3.0/femagtools/losscoeffs.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.606754 femagtools-1.3.0/femagtools/machine/
+-rw-r--r--   0 tar        (210) tar        (210)     7392 2023-05-26 13:39:42.000000 femagtools-1.3.0/femagtools/machine/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     6387 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/machine/effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)    34847 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/machine/im.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    35696 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/machine/pm.py
+-rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/machine/sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    26608 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/machine/sm.py
+-rw-r--r--   0 tar        (210) tar        (210)    16617 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/machine/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.3.0/femagtools/magnet.py
+-rw-r--r--   0 tar        (210) tar        (210)    39691 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/mcv.py
+-rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/me.py
+-rw-r--r--   0 tar        (210) tar        (210)    14068 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/model.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.606754 femagtools-1.3.0/femagtools/moo/
+-rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/moo/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/moo/algorithm.py
+-rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/moo/population.py
+-rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/moo/problem.py
+-rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/moproblem.py
+-rw-r--r--   0 tar        (210) tar        (210)     8506 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/multiproc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/mxw2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/netlist.py
+-rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/ntib.py
+-rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.3.0/femagtools/opt.py
+-rw-r--r--   0 tar        (210) tar        (210)    18714 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/parstudy.py
+-rw-r--r--   0 tar        (210) tar        (210)    58203 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/plot.py
+-rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/poc.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.616754 femagtools-1.3.0/femagtools/templates/
+-rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/FE-losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)      242 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/airgapinduc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.3.0/femagtools/templates/asyn_motor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.3.0/femagtools/templates/basic_modpar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/calc_field_ts.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1600 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/calc_therm_field.mako
+-rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/cogg_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/colorgrad.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/com_motor_sim.mako
+-rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/conduct-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      663 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/connect_models.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/cu_losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/ec-rotorbar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/fe-contr.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4820 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/gen_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/inductances.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/ld_lq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/leak_dist_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/leak_evol_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/leak_tooth_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnet-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetFC2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2268 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/magnetIron.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetIron2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetIron3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetIron4.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetIron5.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3960 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/magnetIronV.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetSector.mako
+-rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetSectorLinear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetShell.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/magnetShell2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/mesh-airgap.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/modal_analysis.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/mult_cal_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/new_model.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/noloadflux-rot.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/noloadflux.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/noloadfluxdc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/open.mako
+-rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/plots.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/pm_sym_f_cur.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/pm_sym_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/pm_sym_loss.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/psd_psq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/ring.mako
+-rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.3.0/femagtools/templates/rot_hsm.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.3.0/femagtools/templates/rotorAsyn.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/rotorKs2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/rotor_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.3.0/femagtools/templates/rotor_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/shortcircuit.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/srm.mako
+-rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/stator1.mako
+-rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/stator2.mako
+-rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/stator3Linear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/stator4.mako
+-rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/statorBG.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/templates/statorRing.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4942 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/statorRotor3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/templates/stator_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2906 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/therm-dynamic.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1002 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/therm-static.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1782 2023-06-13 07:51:56.000000 femagtools-1.3.0/femagtools/templates/torq_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.3.0/femagtools/tks.py
+-rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.3.0/femagtools/ts.py
+-rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/vbf.py
+-rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.3.0/femagtools/vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.3.0/femagtools/windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.604755 femagtools-1.3.0/femagtools.egg-info/
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     4983 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tar        (210) tar        (210)        1 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tar        (210) tar        (210)      191 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/entry_points.txt
+-rw-r--r--   0 tar        (210) tar        (210)      144 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/requires.txt
+-rw-r--r--   0 tar        (210) tar        (210)       11 2023-06-13 07:53:59.000000 femagtools-1.3.0/femagtools.egg-info/top_level.txt
+-rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.3.0/pyproject.toml
+-rw-r--r--   0 tar        (210) tar        (210)       38 2023-06-13 07:53:59.619754 femagtools-1.3.0/setup.cfg
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-06-13 07:53:59.618754 femagtools-1.3.0/tests/
+-rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_airgap_induction.py
+-rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_bchreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     1142 2023-06-13 07:51:56.000000 femagtools-1.3.0/tests/test_effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_erg.py
+-rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.3.0/tests/test_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_forcedens.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    16099 2023-06-13 07:51:56.000000 femagtools-1.3.0/tests/test_fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_im.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.3.0/tests/test_losscoeffs.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    12906 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_machine.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_magncurv.py
+-rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_magnet.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_mcvreader.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     3986 2023-06-13 07:51:56.000000 femagtools-1.3.0/tests/test_mcvwriter.py
+-rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_me.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_model.py
+-rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1323 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_parident.py
+-rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.3.0/tests/test_parstudy.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_pocfile.py
+-rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.3.0/tests/test_sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    83524 2023-05-26 13:39:42.000000 femagtools-1.3.0/tests/test_sm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.3.0/tests/test_tksreader.py
+-rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_ts.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_vbfreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.3.0/tests/test_vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.3.0/tests/test_windings.py
```

### Comparing `femagtools-1.2.9/LICENSE` & `femagtools-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/PKG-INFO` & `femagtools-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.2.9
+Version: 1.3.0
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.2.9/README.md` & `femagtools-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/__init__.py` & `femagtools-1.3.0/femagtools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     Python bindings for FEMAG
 
 
 
 """
 __title__ = 'femagtools'
-__version__ = '1.2.9'
+__version__ = '1.3.0'
 __author__ = 'Ronald Tanner'
 __license__ = 'BSD'
 __copyright__ = 'Copyright 2016-2022 SEMAFOR Informatik & Energie AG'
 
 from .asm import read
 from .bch import Reader
 from .model import MachineModel
```

### Comparing `femagtools-1.2.9/femagtools/airgap.py` & `femagtools-1.3.0/femagtools/airgap.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/amazon.py` & `femagtools-1.3.0/femagtools/amazon.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/amela.py` & `femagtools-1.3.0/femagtools/amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/asm.py` & `femagtools-1.3.0/femagtools/asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/bch.py` & `femagtools-1.3.0/femagtools/bch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1642,14 +1642,15 @@
     def items(self):
         return [(k, self.get(k)) for k in ('version',
                                            'type',
                                            'filename',
                                            'date',
                                            'areas',
                                            'inertia',
+                                           'current_angles',
                                            'torque',
                                            'torque_fft',
                                            'psidq',
                                            'psidq_ldq',
                                            'machine',
                                            'lossPar',
                                            'weights',
```

### Comparing `femagtools-1.2.9/femagtools/bchxml.py` & `femagtools-1.3.0/femagtools/bchxml.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/condor.py` & `femagtools-1.3.0/femagtools/condor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/conductor.py` & `femagtools-1.3.0/femagtools/conductor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/config.py` & `femagtools-1.3.0/femagtools/config.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/convert.py` & `femagtools-1.3.0/femagtools/convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dakota.py` & `femagtools-1.3.0/femagtools/dakota.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dakota_femag.py` & `femagtools-1.3.0/femagtools/dakota_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dakotaout.py` & `femagtools-1.3.0/femagtools/dakotaout.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/docker.py` & `femagtools-1.3.0/femagtools/docker.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/area.py` & `femagtools-1.3.0/femagtools/dxfsl/area.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/conv.py` & `femagtools-1.3.0/femagtools/dxfsl/conv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/converter.py` & `femagtools-1.3.0/femagtools/dxfsl/converter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/corner.py` & `femagtools-1.3.0/femagtools/dxfsl/corner.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/dumprenderer.py` & `femagtools-1.3.0/femagtools/dxfsl/dumprenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/fslrenderer.py` & `femagtools-1.3.0/femagtools/dxfsl/fslrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/functions.py` & `femagtools-1.3.0/femagtools/dxfsl/functions.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/geom.py` & `femagtools-1.3.0/femagtools/dxfsl/geom.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/machine.py` & `femagtools-1.3.0/femagtools/dxfsl/machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/plotrenderer.py` & `femagtools-1.3.0/femagtools/dxfsl/plotrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/dxfsl/shape.py` & `femagtools-1.3.0/femagtools/dxfsl/shape.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/erg.py` & `femagtools-1.3.0/femagtools/erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/femag.py` & `femagtools-1.3.0/femagtools/femag.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     ~~~~~~~~~~~~~~~~
 
     Running FEMAG
 
 
 """
 import subprocess
+import pathlib
 import os
 import glob
 import logging
 try:
     import zmq
 except ImportError:
     pass
@@ -455,14 +456,20 @@
                 with open(os.path.join(self.workdir,
                                        self.modelname+'.ntib'), 'w') as f:
                     f.write('\n'.join(ntib.create(
                         simulation['speed'],
                         simulation['current'],
                         simulation['angl_i_up'])))
                 # TODO: add r1, m
+            if simulation['calculationMode'] == 'therm-dynamic':
+                load = simulation['load']
+                (pathlib.Path(self.workdir)/'load.csv').write_text(
+                    '\n'.join([','.join([f"{load[k][i]}"
+                                         for k in ('t', 'n', 'T', 'i1', 'beta')])
+                               for i in range(0, len(load['t']))]))
         else:
             stateofproblem = 'mag_static'
 
         self.run(fslfile, options, fsl_args, stateofproblem=stateofproblem)
         if simulation:
             if simulation['calculationMode'] == "pm_sym_loss":
                 return self.read_los(self.modelname)
@@ -472,14 +479,20 @@
 
             if simulation['calculationMode'] == 'calc_field_ts':
                 return self.read_ts(self.modelname)
 
             if simulation['calculationMode'] == 'modal_analysis':
                 return self.read_modal(self.modelname)
 
+            if simulation['calculationMode'] == 'therm-dynamic':
+                temp = [[float(n) for n in l.split()]
+                        for l in (pathlib.Path(self.workdir) / 'temperature.dat').read_text().split('\n') if l]
+                ttemp = list(zip(*temp))
+                return {'t': ttemp[0], 'temperature': ttemp[1]}
+
             bch = self.read_bch(self.modelname)
             if simulation['calculationMode'] == 'pm_sym_fast':
                 if simulation.get('shortCircuit', False):
                     logger.info("short circuit simulation")
                     simulation.update(
                         get_shortCircuit_parameters(bch,
                                                     simulation.get('initial', 2)))
@@ -506,14 +519,15 @@
                         except (KeyError, IndexError):
                             logging.debug(
                                 "No additional flux data in sc simulation")
                             break
 
                     bch.torque += bchsc.torque
                     bch.demag += bchsc.demag
+
             if 'airgap_induc' in simulation:
                 try:
                     pmod = bch.machine['p_sim']
                 except KeyError:
                     pmod = 0
                 bch.airgap = ag.read(os.path.join(self.workdir, 'bag.dat'),
                                      pmod=pmod)
```

### Comparing `femagtools-1.2.9/femagtools/forcedens.py` & `femagtools-1.3.0/femagtools/forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/fsl.py` & `femagtools-1.3.0/femagtools/fsl.py`

 * *Files 3% similar despite different names*

```diff
@@ -332,15 +332,37 @@
     def create_connect_models(self, model):
         """return connect_model if rotating machine and incomplete model
         (Note: femag bug with connect model)"
         """
         if (model.get('move_action') == 0 and (
                 model.connect_full or
                 model.stator['num_slots'] > model.stator['num_slots_gen'])):
-            return ['pre_models("connect_models")\n']
+            fslcmds = ['pre_models("connect_models")\n']
+            if 'thcond' in model.stator:
+                fslcmds += [
+                    '-- thermal properties in airgap',
+                    'ag_cond = 0.063',
+                    'thcap = 1007',
+                    'beta = math.pi*m.npols_gen/m.num_poles + m.zeroangl/180*math.pi',
+                    'xai, yai = pr2c((da1+da2)/4, beta)',
+                    'def_mat_therm(xai,yai,"cyan",1.19,ag_cond,thcap,1)',
+                    'xai, yai = pr2c((da1+da2)/4-ag/4, beta)',
+                    'def_mat_therm(xai,yai,"cyan",1.19,ag_cond,thcap,1)',
+                    'xai, yai = pr2c((da1+da2)/4+ag/4, beta)',
+                    'def_mat_therm(xai,yai,"cyan",1.19,ag_cond,thcap,1)',
+                    '',
+                    'state_of_problem("therm_static") -- thermic boundary conditions',
+                    'x1,y1 = pd2c(dy2/2,m.zeroangl)',
+                    'x2,y2 = pd2c(dy1/2,m.zeroangl)',
+                    'beta = 360*m.npols_gen/m.num_poles',
+                    'x3,y3 = pd2c(dy1/2,beta+m.zeroangl)',
+                    'x4,y4 = pd2c(dy2/2,beta+m.zeroangl)',
+                    'def_bcond_tp(x1,y1,x2,y2,x3,y3,x4,y4, 4)',
+                    'state_of_problem("mag_static")']
+            return fslcmds
         return []
 
     def create_open(self, model):
         return (['-- created by femagtools {}'.format(__version__), ''] +
                 self.__render(model, 'open') +
                 ['global_unit("mm")', cosys(model)] +
                 self.set_modpar(model) +
@@ -375,29 +397,56 @@
             if condMat:
                 cond = condMat.find(windings['material'])
             if not cond:
                 raise FslBuilderError(
                     'conductor material {} not found'.format(
                         windings['material']))
             windings['cuconduct'] = cond['elconduct']
+            for k in ('thcond', 'thcap'):
+                if k in cond:
+                    windings[k] = cond[k]
+
         return self.__render(windings, 'cu_losses')
 
     def create_fe_losses(self, model):
-        if any(model.get(k, 0) for k in ('ffactor', 'cw', 'ch', 'hyscoef',
-                                         'edycof', 'indcof', 'fillfact',
-                                         'basfreq', 'basind')):
-            return self.__render(model, 'FE-losses')
+        for part in ('stator', 'rotor', 'commutator', 'magnet'):
+            if model.get(part, 0):
+                submod = model.get(part)
+                if any(submod.get(k, 0) for k in (
+                        'ffactor', 'cw', 'ch', 'hyscoef',
+                        'edycof', 'indcof', 'fillfact',
+                        'fillfac','basfreq', 'basind',
+                        'ffactor')):
+                    if submod.get('fillfac', 0):
+                        submod['fillfact'] = submod['fillfac']
+                    return self.__render(submod, 'FE-losses')
         return []
 
     def create_gen_winding(self, model):
         genwdg = self.__render(model, 'gen_winding')
         k = list({'leak_dist_wind',
                   'leak_evol_wind',
                   'leak_tooth_wind'}.intersection(model.windings))
         if k:
+            logger.info("LEAK %s ---------------", k)
+            if 'wiredia' not in model.windings[k[0]]:
+                if 'wire_gauge' in model.windings:
+                    import numpy as np
+                    d = 2*np.sqrt(model.windings['wire_gauge']/np.pi)
+                    model.windings[k[0]]['wiredia'] = d
+                elif 'dia_wire' in model.windings:
+                    model.windings[k[0]]['wiredia'] = model.windings['dia_wire']
+                elif 'wire_width' in model.windings:
+                    import numpy as np
+                    w = model.windings['wire_width']
+                    h = model.windings['wire_height']
+                    d = 2*np.sqrt(h*w/np.pi)
+                    model.windings[k[0]]['wiredia'] = d
+                elif 'wire_diam' in model.windings:
+                    model.windings[k[0]]['wiredia'] = model.windings['wire_diam']
             return (genwdg +
                     self.__render(model.windings[k[0]], k[0]) +
                     ['post_models("end_wind_leak","leak")',
                      'file_leak = io.open("end_wind_leak.dat","w")',
                      'file_leak:write(string.format("%g %g %g\\n", leak[1], leak[2], leak[3]))',
                      'file_leak:close()'])
         return genwdg
@@ -485,14 +534,18 @@
                 model.set_num_slots_gen()
             if hasattr(model, 'magnet'):
                 if magnetMat:
                     model['magnet']['remanenc'] = magnetMat.get(
                         'remanenc', 1.2)
                     model['magnet']['relperm'] = magnetMat.get('relperm', 1.05)
                     model['magnet']['rlen'] = magnetMat.get('rlen', 1.0)
+                    for k in ('thcond', 'thcap'):
+                        if k in magnetMat:
+                            model['magnet'][k] = magnetMat[k]
+
                 rotor = (self.create_magnet(model) +
                          self.create_magnet_model(model))
                 if magnetMat:
                     rotor += self.create_magnet(model, magnetMat)
             else:
                 rotor = self.create_rotor_model(
                     model, condMat, ignore_material)
@@ -626,15 +679,18 @@
             if 'num_poles' in model.windings:
                 num_poles = model.windings['num_poles']
         except AttributeError:
             pass
 
         if 'poc' in sim:
             poc = sim['poc']
-            poc.pole_pitch = 2*360/num_poles
+            try:
+                poc.pole_pitch = 2*360/num_poles
+            except UnboundLocalError:
+                pass
             sim['pocfilename'] = poc.filename()
         elif 'pocfilename' not in sim:
             try:
                 poc = Poc(2*360/num_poles)
                 sim['poc'] = poc
                 sim['pocfilename'] = poc.filename()
             except UnboundLocalError:
```

### Comparing `femagtools-1.2.9/femagtools/getset.py` & `femagtools-1.3.0/femagtools/getset.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/gmsh.py` & `femagtools-1.3.0/femagtools/gmsh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/google.py` & `femagtools-1.3.0/femagtools/google.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/grid.py` & `femagtools-1.3.0/femagtools/grid.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/isa7.py` & `femagtools-1.3.0/femagtools/isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/jcf2msh.py` & `femagtools-1.3.0/femagtools/jcf2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/jhb.py` & `femagtools-1.3.0/femagtools/jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/job.py` & `femagtools-1.3.0/femagtools/job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/losscoeffs.py` & `femagtools-1.3.0/femagtools/losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/machine/__init__.py` & `femagtools-1.3.0/femagtools/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/machine/effloss.py` & `femagtools-1.3.0/femagtools/machine/effloss.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import scipy.interpolate as ip
 import logging
 from .utils import betai1
 from .pm import PmRelMachineLdq, PmRelMachinePsidq, PmRelMachine
-from .sm import SynchronousMachine
+from .sm import SynchronousMachine, SynchronousMachineLdq, SynchronousMachinePsidq
 from . import create_from_eecpars
 
 logger = logging.getLogger("femagtools.effloss")
 
 
 def _generate_mesh(n, T, nb, Tb, npoints):
     """return speed and torque list for driving/braking speed range
@@ -34,17 +34,21 @@
         def tbip(x): return 0
 
     nxtx = []
     for nx in np.linspace(1, nmax, npoints[0]):
         t0 = tbip(nx)
         t1 = tip(nx)
         npnts = max(round((t1-t0) / (tmax-tmin) * tnum), 2)
-        for t in np.concatenate(
-                (np.linspace(t0, 0.015*tmin, npnts),
-                 np.linspace(0.015*tmax, t1, npnts))):
+        if nb:
+            a = np.concatenate(
+                        (np.linspace(t0, 0.015*tmin, npnts),
+                         np.linspace(0.015*tmax, t1, npnts)))
+        else:
+            a = np.linspace(0.015*tmax, t1, npnts)
+        for t in a:
             nxtx.append((nx, t))
     return np.array(nxtx).T
 
 
 def efficiency_losses_map(eecpars, u1, T, temp, n, npoints=(60, 40)):
     """return speed, torque efficiency and losses
 
@@ -67,35 +71,48 @@
     else:  # must be an instance of Machine
         m = eecpars
     if isinstance(T, list):
         r = {'T': T, 'n': n}
         rb = {'T': [], 'n': []}
     else:  # calculate speed,torque characteristics
         nmax = n
+        nsamples = npoints[0]
         rb = {}
-        r = m.characteristics(T, nmax, u1)  # driving mode
-        if isinstance(m, PmRelMachineLdq):
+        r = m.characteristics(T, nmax, u1, nsamples=nsamples)  # driving mode
+        if isinstance(m, (PmRelMachineLdq, SynchronousMachineLdq)):
             if min(m.betarange) >= -np.pi/2:  # driving mode only
                 rb['n'] = None
                 rb['T'] = None
-        if isinstance(m, PmRelMachinePsidq):
+        if isinstance(m, (PmRelMachinePsidq, SynchronousMachinePsidq)):
             if min(m.iqrange) >= 0:  # driving mode only
                 rb['n'] = None
                 rb['T'] = None
         if 'n' not in rb:
-            rb = m.characteristics(-T, max(r['n']), u1)  # braking mode
+            rb = m.characteristics(-T, max(r['n']), u1, nsamples=nsamples)  # braking mode
     ntmesh = _generate_mesh(r['n'], r['T'],
                             rb['n'], rb['T'], npoints)
 
-    if isinstance(m, PmRelMachine) or isinstance(m, SynchronousMachine):
+    class ProgressLogger:
+        def __init__(self, nsamples):
+            self.n = 0
+            self.nsamples = nsamples
+            self.num_iv = round(nsamples/15)
+        def __call__(self, iqd):
+            self.n += 1
+            if self.n % self.num_iv == 0:
+                logger.info("Losses/Eff Map: %d%%",
+                            round(100*self.n/self.nsamples))
+
+    if isinstance(m, (PmRelMachine, SynchronousMachine)):
+        progress = ProgressLogger(ntmesh.shape[1])
         iqd = np.array([
             m.iqd_torque_umax(
                 nt[1],
                 2*np.pi*nt[0]*m.p,
-                u1)[:-1]
+                u1, log=progress)[:-1]
             for nt in ntmesh.T]).T
         beta, i1 = betai1(iqd[0], iqd[1])
         uqd = [m.uqd(2*np.pi*n*m.p, *i)
                for n, i in zip(ntmesh[0], iqd.T)]
         u1 = np.linalg.norm(uqd, axis=1)/np.sqrt(2.0)
         f1 = ntmesh[0]*m.p
     else:
@@ -111,16 +128,15 @@
             i1 = m.i1(w1, m.psi, wm)
             r['i1'].append(np.abs(i1))
             r['plfe1'].append(m.m*np.abs(u1)**2/m.rfe(w1, m.psi))
             i2 = m.i2(w1, m.psi, wm)
             r['plcu1'].append(m.m*np.abs(i1)**2*m.rstat(w1))
             r['plcu2'].append(m.m*np.abs(i2)**2*m.rrot(w1-m.p*wm))
 
-
-    if isinstance(m, PmRelMachine) or isinstance(m, SynchronousMachine):
+    if isinstance(m, (PmRelMachine, SynchronousMachine)):
         plfe1 = m.iqd_plfe1(*iqd, f1)
         plfe2 = m.iqd_plfe2(iqd[0], iqd[1], f1)
         plmag = m.iqd_plmag(iqd[0], iqd[1], f1)
         plcu1 = m.iqd_plcu1(iqd[0], iqd[1], 2*np.pi*f1)
         plcu2 = m.iqd_plcu2(*iqd)
         try:
             tfric = m.kfric_b*m.rotor_mass*30e-3/np.pi
@@ -133,15 +149,15 @@
         plcu1 = np.array(r['plcu1'])
         plcu2 = np.array(r['plcu2'])
         iqd = np.zeros(ntmesh.shape)
         u1 = np.array(r['u1'])
         i1 = np.array(r['i1'])
         try:
             tfric = eecpars['kfric_b']*eecpars['rotor_mass']*30e-3/np.pi
-        except:
+        except KeyError:
             tfric = 0
 
     plfric = 2*np.pi*ntmesh[0]*tfric
     ntmesh[1] -= tfric
     pmech = np.array(
         [2*np.pi*nt[0]*nt[1]
          for nt in ntmesh.T])
```

### Comparing `femagtools-1.2.9/femagtools/machine/im.py` & `femagtools-1.3.0/femagtools/machine/im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/machine/pm.py` & `femagtools-1.3.0/femagtools/machine/pm.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,18 +38,20 @@
         self.p = p
         self.m = m
         self.r1 = r1
         self.ls = ls
         self.io = (1, -1)
         self.fo = 50.0
         self.tcu1 = 20
-        self.zeta1 = 0.2
+        self.zeta1 = 0.3
         self.gam = 0.7
         self.kh = 2
         self.kfric_b = 1
+        # TODO: need this for speedranges and idq_imax_umax mtpv only
+        self.check_extrapolation = True
         for k in kwargs.keys():
             setattr(self, k, kwargs[k])
 
         self.plexp = {'styoke_hyst': 1.0,
                       'stteeth_hyst': 1.0,
                       'styoke_eddy': 2.0,
                       'stteeth_eddy': 2.0,
@@ -72,18 +74,23 @@
         tq = self.m*self.p/2*(psid*iq - psiq*id)
         return tq
 
     def iqd_torque(self, torque):
         """return minimum d-q-current for torque"""
         if np.abs(torque) < 1e-2:
             return (0, 0)
-        res = so.minimize(lambda iqd: la.norm(iqd), self.io, method='SLSQP',
-                          constraints=({'type': 'eq',
-                                        'fun': lambda iqd:
-                                        self.torque_iqd(*iqd) - torque}))
+        if torque > 0:
+            iqd0 = self.i1range[1]/2, 0
+        else:
+            iqd0 = -self.i1range[1]/2, 0
+        res = so.minimize(
+            lambda iqd: la.norm(iqd), self.io, method='SLSQP',
+            constraints=({'type': 'eq',
+                          'fun': lambda iqd:
+                          self.torque_iqd(*iqd) - torque}))
         if not res.success:
             raise ValueError(f'Torque {torque} out of current range')
         return res.x
 
     def tmech_iqd(self, iq, id, n, kpfe, pfw):
         """return shaft torque with given d-q current, iron loss correction factor
           and friction windage losses"""
@@ -95,15 +102,15 @@
         return self.torque_iqd(iq, id) - (plfe + pmag + pfw)/(2*np.pi*n)
 
     def uqd(self, w1, iq, id):
         """return uq, ud of frequency w1 and d-q current"""
         psid, psiq = self.psi(iq, id)
         uqd = (self.r1*iq + w1*(self.ls*id + psid),
                self.r1*id - w1*(self.ls*iq + psiq))
-        logger.debug('beta i1 %s u1 %f', betai1(iq, id), la.norm(uqd))
+        #logger.debug('beta i1 %s u1 %f', betai1(iq, id), la.norm(uqd))
         return uqd
 
     def w1_umax(self, u, iq, id):
         """return frequency w1 at given voltage u and id, iq current
 
         Keyword arguments:
         u -- the maximum voltage (RMS)
@@ -175,96 +182,175 @@
         if ier == 1:
             return i1
         raise ValueError("{} for w1 {}, u1 {}, beta {}".format(
             mesg, w1, u1, beta))
 
     def id_torque(self, torque, iq):
         "return d current with given torque and d-current"
-        id0 = min(self.io[1]/4, iq/np.tan(self.betarange[0]))
+        id0 = self.iqd_torque(torque)[1]
         return so.fsolve(
             lambda id: self.torque_iqd(np.array([iq]), id)-torque, id0)[0]
 
-    def iqd_torque_umax(self, torque, w1, u1max):
-        "return d-q current and torque at stator frequency and max voltage"
+    def iqd_torque_umax(self, torque, w1, u1max, log=0):
+        """return d-q current and torque at stator frequency and max voltage
+        with minmal current"""
         res = so.minimize(lambda iqd: la.norm(iqd), self.io, method='SLSQP',
                           constraints=(
                               {'type': 'eq',
                                'fun': lambda iqd:
                                self.torque_iqd(*iqd) - torque},
                               {'type': 'ineq',
                                'fun': lambda iqd:
                                np.sqrt(2)*u1max - la.norm(self.uqd(w1, *iqd))}))
+        if log:
+            log(res.x)
+        logger.debug("iqd_torque_umax w1=%f torque=%f %f iq=%f id=%f u1 u1 %f %f",
+                    w1, torque, self.torque_iqd(*res.x), res.x[0], res.x[1],
+                    u1max, np.linalg.norm(
+                        self.uqd(w1, *res.x))/np.sqrt(2))
         return res.x[0], res.x[1], self.torque_iqd(*res.x)
 
-    def iqd_torque_imax_umax(self, torque, n, umax):
-        """return iq, id, torque for constant torque or field weakening"""
+    def iqd_torque_imax_umax(self, torque, n, u1max, log=0):
+        """return d-q current and torque at stator frequency w1,
+        max voltage  and current"""
         iq, id = self.iqd_torque(torque)
         w1 = 2*np.pi*n*self.p
         # Constant torque range
-        if np.linalg.norm(self.uqd(w1, iq, id)) <= umax*np.sqrt(2):
+        if np.linalg.norm(self.uqd(w1, iq, id)) <= u1max*np.sqrt(2):
+            if log:
+                log((iq, id, torque))
             return (iq, id, torque)
         # Field weaking range
         imax = betai1(iq, id)[1]
-        iq, id = self.iqd_imax_umax(imax, w1, umax, maxtorque=torque > 0)
-        return iq, id, self.torque_iqd(iq, id)
+        iq, id, tq = self.iqd_imax_umax(imax, w1, u1max, torque, with_mtpv=False)
+        if log:
+            log((iq, id, tq))
+        return iq, id, tq
+
+    def iqd_maxtorque_imax_umax(self, i1max, w1, u1max):
+        """return d-q current and max torque at stator frequency w1,
+        max voltage  and current"""
+        sign = -1 if i1max > 0 else 1
+        res = so.minimize(lambda iqd: sign*self.torque_iqd(*iqd),
+                          self.mtpa(i1max)[:2],
+                          method='SLSQP',
+                          constraints=(
+                              {'type': 'ineq',
+                               'fun': lambda iqd:
+                               np.sqrt(2)*abs(i1max) - betai1(*iqd)[1]},
+                              {'type': 'eq',
+                               'fun': lambda iqd:
+                               np.sqrt(2)*u1max - la.norm(self.uqd(w1, *iqd))}
+                          ))
+        return res.x[0], res.x[1], self.torque_iqd(*res.x)
 
-    def iqd_imax_umax(self, i1max, w1, u1max, maxtorque=True):
-        """return d-q current at stator frequency and max voltage
+    def iqd_imax_umax(self, i1max, w1, u1max, torque, with_mtpv=True):
+        """return d-q current and torque at stator frequency and max voltage
         and max current (for motor operation if maxtorque else generator operation)"""
 
-        if maxtorque:
-            btab = np.linspace(max(-np.pi/2, self.betarange[0]), 0)
+        if torque > 0:
+            # -pi/2 --> 0
+            b0, b1 = max(-np.pi/2, self.betarange[0]), 0
+            if max(self.betarange) < b1:
+                raise ValueError(
+                    f"invalid betarange for maxtorque>0: {self.betarange}")
         else:
-            btab = np.linspace(min(-np.pi/2, self.betarange[1]),
-                               self.betarange[0])
-        u1b = [np.linalg.norm(self.uqd(w1, *iqd(b, i1max)))
-               for b in btab]
-        if np.max(u1b) > np.sqrt(2)*u1max:
-            beta0 = btab[0]
-            for bx, ux in zip(btab, u1b):
-                if ux/np.sqrt(2) > u1max:
+            # -pi/2 --> -pi
+            b0, b1 = -np.pi/2, max(-np.pi, self.betarange[0])
+            if min(self.betarange) > b0:
+                raise ValueError(
+                    f"invalid betarange for maxtorque<0: {self.betarange}")
+
+        deps = 1e-6
+        kmax = 100
+
+        def u1norm(b):
+            return np.linalg.norm(
+                self.uqd(w1, *iqd(b, abs(i1max))))/np.sqrt(2)
+        if u1norm(b1) < u1max:
+            # must reduce current (torque)
+            iq, id, tq = self.iqd_torque_umax_imin(torque, w1, u1max)
+            if not with_mtpv:
+                return iq, id, tq
+            beta, i1 = betai1(iq, id)
+        else:
+            for k in range(kmax):
+                bx = b0 + (b1-b0)/2
+                ux = u1norm(bx)
+                #logger.info("%d: bx %f ux %f", k, bx, ux)
+                if ux > u1max:
+                    b1 = bx
+                else:
+                    b0 = bx
+                if abs(b1-b0) < deps:
                     break
-                beta0 = bx
-            beta, info, ier, mesg = so.fsolve(
-                lambda b: la.norm(
-                    self.uqd(w1, *iqd(b, i1max))) - u1max*np.sqrt(2),
-                beta0,
-                full_output=True)
-            if ier == 1:
-                return iqd(beta[0], i1max)
-        return self.mtpv(w1, u1max, i1max, maxtorque)[:2]
+            beta, i1 = bx, i1max
+            du = ux - u1max
+            logger.debug("iqd_imax_umax n %f beta %f iter=%d du=%f",
+                         w1/2/np.pi/self.p*60, beta/np.pi*180, k, du)
+            if abs(du) < 0.1:
+                iq, id = iqd(beta, abs(i1max))
+            else:
+                iq, id = self.iqd_torque(torque)
+        if with_mtpv:
+            # must check mtpv
+            self.check_extrapolation = False
+            try:
+                def voltw1(wx):
+                    return np.linalg.norm(
+                        self.mtpv(wx, u1max,
+                                  maxtorque=torque>0)[:2]) - np.sqrt(2)*i1,
+                w, _, ier, _ = so.fsolve(voltw1, w1, full_output=True)
+                logger.info("3: ier %d w %f w1 %f", ier, w, w1)
+                if ier in (1,5) and abs(w[0]) <= w1:
+                    self.check_extrapolation = True
+                    return self.mtpv(w1, u1max)
+            except ValueError as e:
+                logger.warning("MTPV w1=%f i1max=%f, u1max %f %s",
+                               w1, i1, u1max, e)
+            self.check_extrapolation = True
+
+        iq, id = iqd(beta, abs(i1))
+        tq = self.torque_iqd(iq, id)
+        logger.debug("iqd_imax_umax w1=%f torque=%f %f iq=%f id=%f u1 %f %f",
+                    w1, torque, tq, iq, id, u1max, np.linalg.norm(
+                            self.uqd(w1, iq, id))/np.sqrt(2))
+        return iq, id, tq
 
     def mtpa(self, i1):
         """return iq, id, torque at maximum torque of current i1"""
         sign = -1 if i1 > 0 else 1
         b0 = 0 if i1 > 0 else -np.pi
         bopt, fopt, iter, funcalls, warnflag = so.fmin(
             lambda x: sign*self.torque_iqd(*iqd(x, abs(i1))), b0,
             full_output=True,
             disp=0)
         iq, id = iqd(bopt[0], abs(i1))
         return [iq, id, sign*fopt]
 
-    def mtpv(self, w1, u1, i1max, maxtorque=True):
+    def mtpv(self, w1, u1, iqd0=0, maxtorque=True):
         """return d-q-current, torque for voltage and frequency
         with maximum (maxtorque=True) or minimum torque """
         sign = -1 if maxtorque else 1
-        i0 = (-sign*self.i1range[1]/10, -self.i1range[1]/10)
+        if np.isscalar(iqd0):
+            i0 = (-sign*self.i1range[1]/20, -self.i1range[1]/np.sqrt(2))
+        else:
+            i0 = iqd0
         res = so.minimize(
             lambda iqd: sign*self.torque_iqd(*iqd),
             i0, method='SLSQP',
+            #bounds=((0, self.i1range[1]),
+            #        (-self.i1range[1], 0)),
             constraints=(
-                {'type': 'ineq',
+                {'type': 'eq',
                  'fun': lambda iqd:
-                 np.sqrt(2)*u1 - la.norm(self.uqd(w1, *iqd))},
-                {'type': 'ineq',
-                 'fun': lambda iqd:
-                 i1max - betai1(*iqd)[1]}))
-
-        return res.x[0], res.x[1], sign*res.fun
+                 np.sqrt(2)*u1 - la.norm(self.uqd(w1, *iqd))},))
+        if res['success']:
+            return res.x[0], res.x[1], sign*res.fun
+        raise ValueError(f"mtpv w1={w1} u1={u1} maxtorque={maxtorque} res: {res['message']}")
 
     def _set_losspar(self, pfe):
         self.fo = pfe['speed']*self.p
         ef = pfe.get('ef', [2.0, 2.0])
         hf = pfe.get('hf', [1.0, 1.0])
         self.plexp = {'styoke_hyst': hf[0],
                       'stteeth_hyst': hf[0],
@@ -294,116 +380,146 @@
 
     def iqd_losses(self, iq, id, f):
         return np.sum([self.iqd_plfe1(iq, id, f),
                        self.iqd_plfe2(iq, id, f),
                        self.iqd_plmag(iq, id, f),
                        self.iqd_plcu(iq, id, 2*np.pi*f)], axis=0)
 
-    def characteristics(self, T, n, u1max, nsamples=30):
+    def speedranges(self, i1max, u1max, speedmax, with_mtpv, weps=1e-4):
+        """calculate speed range intervals:
+        1. const current MTPA (u < u1max)
+        2. const voltage: flux reduction / MTPA and MTPV (if enabled)
+        returns list of speed limit for each interval
+        """
+        iq, id, T = self.mtpa(i1max)
+        logger.debug("speedrange i1 %f T %f", i1max, T)
+        w1max = 2*np.pi*speedmax*self.p
+        w1type = self.w1_umax(u1max, iq, id)
+        wl, wu = [w1type, w1max]
+        if with_mtpv:
+            kmax = 6
+            self.check_extrapolation = False
+        else:
+            kmax = 0
+            k = kmax
+        for k in range(kmax):
+            wx = wl + (wu-wl)/2
+            try:
+                iq, id = self.iqd_imax_umax(i1max, wx, u1max,
+                                            T, with_mtpv=False)[:2]
+                i1 = betai1(iq, id)[1]
+                try:
+                    def voltw1(wx):
+                        return np.linalg.norm(
+                            self.mtpv(wx, u1max,
+                                      maxtorque=T > 0)[:2]) - np.sqrt(2)*i1
+                    w, _, ier, _ = so.fsolve(voltw1, wx, full_output=True)
+                    logger.debug("3: ier %d i1 %f w %f w1 %f", ier, i1, w, wx)
+                    if ier in (1, 4, 5):
+                        self.check_extrapolation = True
+                        if abs(w[0]) <= wx:
+                            return [w/2/np.pi/self.p
+                                    for w in (w1type, w[0], w1max)]  # ['MTPA', 'MTPV']
+                        wl = w[0]
+                except ValueError as e:
+                    logger.debug(e)
+                    wl = wx
+                    pass
+            except ValueError as e:
+                logger.warning(e)
+                wu = wx
+            logger.debug("%d: wx %f wl %f wu %f --> %f",
+                         k, wx, wl, wu, 100*(wu-wl)/wl)
+
+        self.check_extrapolation = True
+        w1max = min(w1max, self.w1_umax(
+            u1max, *iqd(-np.pi/2, abs(i1max))))
+        return [w/2/np.pi/self.p for w in (w1type, w1max)]  # ['MTPA']
+
+
+    def characteristics(self, T, n, u1max, nsamples=60, with_mtpv=True):
         """calculate torque speed characteristics.
         return dict with list values of
         id, iq, n, T, ud, uq, u1, i1,
         beta, gamma, phi, cosphi, pmech, n_type
 
         Keyword arguments:
         T -- the maximum torque or the list of torque values in Nm
         n -- the maximum speed or the list of speed values in 1/s
         u1max -- the maximum voltage in V rms
         nsamples -- (optional) number of speed samples
+        with_mtpv -- (optional) use mtpv if true (default)
         """
         r = dict(id=[], iq=[], uq=[], ud=[], u1=[], i1=[], T=[],
                  beta=[], gamma=[], phi=[], cosphi=[], pmech=[], n=[])
         if np.isscalar(T):
             iq, id = self.iqd_torque(T)
             i1max = betai1(iq, id)[1]
+            if T < 0:
+                i1max = -i1max
             w1 = self.w1_umax(u1max, iq, id)
-            iqmin, idmin = self.iqdmin(i1max)
-            if (iqmin < 0):
-                iqmin = 0
-            w1max = self.w1_umax(u1max, iqmin, idmin)
-            nmax = max(w1, w1max)/2/np.pi/self.p
-            n1 = min(w1/2/np.pi/self.p, nmax)
+            n1 = w1/2/np.pi/self.p
             r['n_type'] = n1
+            nmax = n
             logger.info("Type speed %f n: %f nmax %f",
                         60*n1, 60*n, 60*nmax)
-            try:
-                w1 = self.w2_imax_umax(i1max, u1max, maxtorque=(T > 0))
-                n2 = w1/2/np.pi/self.p
-                iqmtpv, idmtpv, tq = self.mtpv(
-                    w1, u1max, i1max, maxtorque=T > 0)
-                if not self._inrange((iqmtpv, idmtpv)):
-                    if n > 0:
-                        n2 = min(nmax, n)
-                    else:
-                        n2 = nmax
-                logger.info("n1: %f n2: %f ",
-                            60*n1, 60*n2)
-            except ValueError:
-                if n > 0:
-                    n2 = min(nmax, n)
+
+            n1 = min(n1, nmax)
+            if n1 < nmax:
+                speedrange = [0] + self.speedranges(i1max, u1max,
+                                                     nmax, with_mtpv)
+                if len(speedrange) > 3:
+                    interv = 'MTPA', 'MTPV'
                 else:
-                    n2 = nmax
-            if n > 0:
-                nmax = min(nmax, n)
-                speedrange = sorted(
-                    list(set([nx for nx in [n1, n2, n] if nx < 1.01*nmax])))
+                    interv = 'MTPA',
             else:
-                speedrange = sorted(list(set([n1, n2])))
-            logger.info("speedrange %s (T = %s Nm)",
-                        speedrange, T)
-            speedrange.insert(0, 0)
+                speedrange = [0, n1]
+                interv = []
+
+            logger.info("Speedrange T=%g %s", T, speedrange)
             n3 = speedrange[-1]
             nstab = [int(nsamples*(x1-x2)/n3)
                      for x1, x2 in zip(speedrange[1:],
                                        speedrange)]
+            logger.info("sample intervals %s", nstab)
             for nx in np.linspace(0, n1, nstab[0]):
                 r['id'].append(id)
                 r['iq'].append(iq)
                 r['n'].append(nx)
                 r['T'].append(T)
 
-            n1 = speedrange[1]
-            try:
-                n2 = speedrange[2]
-            except IndexError:
-                n2 = n1
-            if n1 < n2:  # find id, iq, torque in fieldweakening range
-                dn = r['n'][-1] - r['n'][-2]
-                for nn in np.linspace(r['n'][-1]+dn, n2, nstab[1]):
-                    w1 = 2*np.pi*nn*self.p
-                    logger.debug("fieldweakening: n %g T %g i1max %g w1 %g u1 %g",
-                                 nn*60, T, i1max, w1, u1max)
-                    iq, id = self.iqd_imax_umax(i1max, w1, u1max,
-                                                maxtorque=T > 0)
-                    tq = self.torque_iqd(iq, id)
-                    if (T > 0 and tq > 0) or (T < 0 and tq < 0):
-                        r['id'].append(id)
-                        r['iq'].append(iq)
-                        r['n'].append(nn)
-                        r['T'].append(tq)
-                    else:
-                        logger.warning("fieldweakening: n %g T %g tq %g i1max %g w1 %g u1 %g",
-                                       nn*60, T, tq, i1max, w1, u1max)
-
-            if n2 < n3:
-                for nn in np.linspace(r['n'][-1]+dn/2, n3, nstab[2]):
-                    w1 = 2*np.pi*nn*self.p
-                    try:
-                        iq, id, tq = self.mtpv(
-                            w1, u1max, i1max, maxtorque=T > 0)
-                        if not self._inrange((iq, id)):
-                            break
-                    except ValueError:
-                        logger.warn("ValueError at speed %f", 60*nx)
-                        break
-                    r['id'].append(id)
-                    r['iq'].append(iq)
-                    r['n'].append(nn)
-                    r['T'].append(tq)
-
+            for ns, nu, iv in zip(nstab[1:], speedrange[2:], interv):
+                # find id, iq, torque in fieldweakening range
+                if ns == 0:
+                    ns = 1
+                dn = (nu - r['n'][-1])/ns
+                logger.info("RANGE %s %d: %f -- %f",
+                            iv, ns, r['n'][-1] + dn, nu)
+                try:
+                    for nn in np.linspace(r['n'][-1]+dn, nu, ns):
+                        w1 = 2*np.pi*nn*self.p
+                        logger.debug("fieldweakening: n %g T %g i1max %g w1 %g u1 %g",
+                                     nn*60, T, i1max, w1, u1max)
+                        if iv == 'MTPA':
+                            iq, id, tq = self.iqd_imax_umax(i1max, w1, u1max, T,
+                                                            with_mtpv=False)
+                        else:
+                            iq, id, tq = self.mtpv(w1, u1max,
+                                                   maxtorque=T > 0)
+                        if (T > 0 and tq > 0) or (T < 0 and tq < 0):
+                            r['id'].append(id)
+                            r['iq'].append(iq)
+                            r['n'].append(nn)
+                            r['T'].append(tq)
+                        else:
+                            logger.warning("fieldweakening: n %g T %g tq %g i1max %g w1 %g u1 %g",
+                                           nn*60, T, tq, i1max, w1, u1max)
+                except ValueError as e:
+                    nmax = r['n'][-1]
+                    logger.warning("%s: adjusted nmax %f", e, nmax)
         else:
             for t, nx in zip(T, n):
                 w1 = 2*np.pi*nx*self.p
                 iq, id, tq = self.iqd_torque_umax(t, w1, u1max)
                 r['id'].append(id)
                 r['iq'].append(iq)
                 r['T'].append(tq)
@@ -613,27 +729,28 @@
         self.lq = lambda x, y: ip.RectBivariateSpline(
             beta, i1, np.asarray(lq)).ev(x, y)
         logger.debug("rectbivariatespline beta %s i1 %s", beta, i1)
 
     def psi(self, iq, id):
         """return psid, psiq of currents iq, id"""
         beta, i1 = betai1(np.asarray(iq), np.asarray(id))
-        logger.debug('beta %f (%f, %f) i1 %f %f',
-                     beta, self.betarange[0], self.betarange[1],
-                     i1, self.i1range[1])
-        if (self.betarange[0] <= beta <= self.betarange[1] and
-                i1 <= 1.01*self.i1range[1]):
-            if self.psid:
-                return (self.psid(beta, i1), self.psiq(beta, i1))
-
-            psid = self.ld(beta, i1)*id + np.sqrt(2)*self.psim(beta, i1)
-            psiq = self.lq(beta, i1)*iq
-            return (psid, psiq)
-
-        return (np.nan, np.nan)
+        #logger.debug('beta %f (%f, %f) i1 %f %f',
+        #             beta, self.betarange[0], self.betarange[1],
+        #             i1, self.i1range[1])
+        if self.check_extrapolation:
+            if (self.betarange[0] > beta or
+                self.betarange[1] < beta or
+                i1 > 1.01*self.i1range[1]):
+                return (np.nan, np.nan)
+        if self.psid:
+            return (self.psid(beta, i1), self.psiq(beta, i1))
+
+        psid = self.ld(beta, i1)*id + np.sqrt(2)*self.psim(beta, i1)
+        psiq = self.lq(beta, i1)*iq
+        return (psid, psiq)
 
     def iqdmin(self, i1):
         """max iq, min id for given current"""
         if self.betarange[0] <= -np.pi/2 <= self.betarange[1]:
             return iqd(-np.pi/2, i1)
         if self.betarange[1] == 0:
             return iqd(self.betarange[0], i1)
```

### Comparing `femagtools-1.2.9/femagtools/machine/sizing.py` & `femagtools-1.3.0/femagtools/machine/sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/machine/sm.py` & `femagtools-1.3.0/femagtools/machine/sm.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .utils import skin_resistance, wdg_resistance
 from .. import parstudy, windings
 import femagtools.bch
 
 EPS = 1e-13
 
 eecdefaults = dict(
-    zeta1=0.2,
+    zeta1=0.3,
     zeta2=0,
     gam=0.7,
     kh=2,
     tcu1=20,
     tcu2=20,
     rotor_mass=0,
     kfric_b=1)
@@ -62,19 +62,19 @@
         i1_max = round(0.28*np.pi*hs*(da1+hs)/Q1/N*Jmax*1e5)*10 * \
             machine['windings'].get('num_par_wdgs', 1)
 
         ifnom = machine['rotor']['ifnom']
         exc_logspace = True
         if exc_logspace:
             excur = np.logspace(np.log(ifnom/10), np.log(1.5*ifnom),
-                                kwargs.get("num_exc_steps", 8),
+                                kwargs.get("num_exc_steps", 6),
                                 base=np.exp(1)).tolist()
         else:
             excur = np.linspace(ifnom/10, 1.5*ifnom,
-                                kwargs.get("num_exc_steps", 8))
+                                kwargs.get("num_exc_steps", 6))
 
         parvardef = {
             "decision_vars": [
                 {"values": excur, "name": "load_ex_cur"}
             ]
         }
 
@@ -308,61 +308,68 @@
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             def sqrtculoss(iqde):
                 pcu = self.culoss(iqde)
                 #logger.info("iqde %s --> pcu %f", iqde, pcu)
                 return pcu
             res = so.minimize(
-                sqrtculoss, startvals, method='SLSQP',  # trust-constr
+                self.culoss, startvals, method='SLSQP',  # trust-constr
                 bounds=self.bounds,
                 #            jac=gradient_respecting_bounds(self.bounds, self.culoss),
                 constraints=[
                     {'type': 'eq',
                      'fun': lambda iqd: self.torque_iqd(*iqd) - torque}],
                 options={'disp': disp, 'maxiter': maxiter})
             if res['success']:
                 return res.x
         logger.warning("%s: torque=%f %f, io=%s",
                        res['message'], torque, self.torque_iqd(*startvals),
                        startvals)
         raise ValueError(res['message'])
 
-    def iqd_torque_umax(self, torque, w1, u1max, io=0,
-                        disp=False, maxiter=500):
+    def iqd_torque_umax(self, torque, w1, u1max,
+                        disp=False, maxiter=500, log=0):
         """return currents for torque with minimal losses"""
         #logger.info(">> torque %g w1 %g u1 %g io %s", torque, w1, u1max, io)
-        if io == 0:
-            iqde = self.iqd_torque(torque, disp, maxiter)
-            if np.linalg.norm(
-                    self.uqd(w1, *iqde)) <= u1max*np.sqrt(2):
+        #if torque > 0:
+        #    io = self.bounds[0][1]/2, 0, sum(self.bounds[-1])/2
+        #else:
+        #    io = -self.bounds[0][1]/2, 0, sum(self.bounds[-1])/2
+        iqde = self.iqd_torque(torque, disp, maxiter)
+        if np.linalg.norm(
+            self.uqd(w1, *iqde)) <= u1max*np.sqrt(2):
+                if log:
+                    log(iqde)
                 return (*iqde, torque)
-            io = iqde[0], 0, iqde[2]
-            logger.debug("--- torque %g io %s", torque, io)
+        io = iqde[0], 0, iqde[2]
+        #    logger.debug("--- torque %g io %s", torque, io)
         #logger.info(">>      io %s", io)
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             def sqrtculoss(iqde):
                 pcu = self.culoss(iqde)
                 #logger.info("iqde %s pcu %g", iqde, pcu)
                 return pcu
 
             res = so.minimize(
-                sqrtculoss, io, method='SLSQP',  # trust-constr
+                self.culoss, io, method='SLSQP',  # trust-constr
                 bounds=self.bounds,
                 options={'disp': disp, 'maxiter': maxiter},
                 #            jac=gradient_respecting_bounds(self.bounds, self.culoss),
                 constraints=[
                     {'type': 'eq',
                      'fun': lambda iqd: self.torque_iqd(*iqd) - torque},
                     {'type': 'eq',
                      'fun': lambda iqd: np.linalg.norm(
                          self.uqd(w1, *iqd)) - u1max*np.sqrt(2)}])
             if res['success']:
-                return (*res.x, self.torque_iqd(*res.x))
+                if log:
+                    log(res.x)
+                return *res.x, self.torque_iqd(*res.x)
         logger.warning("%s: w1=%f torque=%f, u1max=%f, io=%s",
                        res['message'], w1, torque, u1max, io)
         raise ValueError(res['message'])
 
     def w1_umax(self, u, iq, id, iex):
         """return frequency w1 at given voltage u and id, iq current
```

### Comparing `femagtools-1.2.9/femagtools/machine/utils.py` & `femagtools-1.3.0/femagtools/machine/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 def skin_resistance(r0, w, temp, zeta, gam=0, nh=1, kth=KTH):
     """return eddy current resistance of winding or rotor bar
     Arguments:
     r0: (float) dc resistance
     w: (float) current frequency in rad
     temp: (float) conductor temperature in deg Celsius
     zeta: (float) skin effect coefficient (penetration depth)
-    gam: (float) constant coefficient (0..1)
+    gam: (float) ratio of length of end winding and length of slot (0..1)
     nh: (int) number of vertical conductors in slot
     kth: (float) temperature coefficient (Default = 0.0039, Cu)"""
     xi = xiskin(w, temp, zeta)
     if np.isscalar(xi):
         if xi < 1e-12:
             k = 1
         else:
@@ -320,16 +320,14 @@
             for f in ('hf', 'ef'):
                 if f in dqpars[0]['losses']:
                     fpip['losses'][f] = dqpars[0]['losses'][f]
     except KeyError:
         pass
     return x, fpip
 
-    Q2 = machine['rotor']['num_slots']
-
 
 def dqparident(workdir, engine, temp, machine,
                magnetizingCurves, magnetMat=[], condMat=[],
                **kwargs):
     """return list of parameters of equivalent circuit for PM machines
 
     arguments:
@@ -340,18 +338,18 @@
     machine -- dict() with machine parameters
     magnetizingCurves -- list of dict() with BH curves
     magnetMat -- list of dict() with magnet material properties
     condMat -- list of dict() with conductor material properties
 
     optional arguments:
     num_cur_steps: number of current steps (default 5)
-    num_beta_steps: number of current steps (default 13)
+    num_beta_steps: number of current steps (default 7 per quadrant)
     speed: rotor speed in 1/s (default 160/p)
     i1_max: maximum current in A rms (default approx 3*i1nom)
-    use_multiprocessing: (boolean) perfom FE simulations in parallel (default: True)
+    period_frac: fraction of rotating angle (default 6)
     """
     import pathlib
 
     da1 = machine['outer_diam']
     Q1 = machine['stator']['num_slots']
     slotmodel = [k for k in machine['stator'] if isinstance(
         machine['stator'][k], dict)][-1]
@@ -361,31 +359,35 @@
     else:
         hs = machine['stator'][slotmodel].get('slot_height', 0)
     N = machine['windings']['num_wires']
     Jmax = 15  # max current density in A/mm2
 
     i1_max = round(0.28*np.pi*hs*(da1+hs)/Q1/N*Jmax*1e5)*10 * \
         machine['windings'].get('num_par_wdgs', 1)
-    period_frac = 6
+    period_frac = kwargs.get('period_frac', 6)
     if machine.get('external_rotor', False):
         period_frac = 1  # TODO: missing femag support
 
     # winding resistance
     yd = machine['windings'].get('coil_span', Q1/machine['poles'])
     wdg = windings.Winding(
         {'Q': machine['stator']['num_slots'],
          'm': machine['windings']['num_phases'],
          'p': machine['poles']//2,
          'l': machine['windings']['num_layers'],
          'yd': yd})
 
     lfe = machine['lfe']
     g = machine['windings'].get('num_par_wdgs', 1)
-    if 'dia_wire' in machine['windings']:
+    if 'wire_gauge' in machine['windings']:
+        aw = machine['windings']['wire_gauge']
+    elif 'dia_wire' in machine['windings']:
         aw = np.pi*machine['windings'].get('dia_wire', 1e-3)**2/4
+    elif ('wire_width' in machine['windings']) and ('wire_height' in machine['windings']):
+        aw = machine['windings']['wire_width']*machine['windings']['wire_height']
     else:  # wire diameter from slot area
         aw = 0.75 * \
             machine['windings'].get('cufilfact', 0.45)*np.pi*da1*hs/Q1/2/N
     r1 = wdg_resistance(wdg, N, g, aw, da1, hs, lfe)
 
     n = len(temp)
     parvardef = {
@@ -397,14 +399,17 @@
     }
 
     parvar = parstudy.List(
         workdir, condMat=condMat,
         magnetizingCurves=magnetizingCurves,
         magnets=magnetMat)
 
+    leakfile = pathlib.Path(workdir) / 'end_wind_leak.dat'
+    leakfile.unlink(missing_ok=True)
+
     simulation = dict(
         calculationMode='ld_lq_fast',
         i1_max=kwargs.get('i1_max', i1_max),
         magn_temp=20,
         wind_temp=20,
         beta_max=0,
         beta_min=-90,
@@ -414,19 +419,18 @@
         num_beta_steps=kwargs.get('num_beta_steps', 7),
         speed=kwargs.get('speed', 160/machine['poles']),
         period_frac=period_frac)
 
     # TODO: cleanup()  # remove previously created files in workdir
     # start calculation
     results = parvar(parvardef, machine, simulation, engine)
-    import json
-    with open('results.json', 'w') as fp:
-        json.dump(results, fp)
+    #import json
+    #with open('results.json', 'w') as fp:
+    #    json.dump(results, fp)
     ls1 = 0
-    leakfile = pathlib.Path(workdir) / 'end_wind_leak.dat'
     try:
         leakages = [float(x)
                     for x in leakfile.read_text().split()]
         ls1 += leakages[1]  # TODO: np.linalg.norm(leakages[1:])
     except:
         logger.warning("No end winding leakage")
 
@@ -453,13 +457,18 @@
         ldq[j]['losses'] = {k: np.vstack((np.array(results['f'][i+1]['ldq']['losses'][k])[:-1, :],
                                           np.array(results['f'][i]['ldq']['losses'][k]))).tolist()
                             for k in losskeys}
         ldq[j]['losses']['speed'] = results['f'][i]['ldq']['losses']['speed']
         for k in ('hf', 'ef'):
             ldq[j]['losses'][k] = results['f'][i]['lossPar'][k]
 
-    return {'m': machine['windings']['num_phases'],
-            'p': machine['poles']//2,
-            'r1': machine['windings'].get('resistance', r1),
-            'ls1': ls1,
-            "rotor_mass": rotor_mass, "kfric_b": 1,
-            'ldq': ldq}
+    dqpars = {
+        'm': machine['windings']['num_phases'],
+        'p': machine['poles']//2,
+        'r1': machine['windings'].get('resistance', r1),
+        'ls1': ls1,
+        "rotor_mass": rotor_mass, "kfric_b": 1,
+        'ldq': ldq}
+
+    if 'current_angles' in results['f'][0]:
+        dqpars['current_angles'] = results['f'][0]['current_angles']
+    return dqpars
```

### Comparing `femagtools-1.2.9/femagtools/magnet.py` & `femagtools-1.3.0/femagtools/magnet.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/mcv.py` & `femagtools-1.3.0/femagtools/mcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,16 +441,16 @@
 
         # write line, mc1_remz, mc1_bsat, mc1_bref, mc1_fillfac
         if self.version_mc_curve == self.ACT_VERSION_MC_CURVE:
             self.writeBlock([float(self.mc1_remz), float(self.mc1_bsat),
                              float(self.mc1_bref), float(mc1_fillfac)])
         if mc1_type == DEMCRV_BR:
             self.mc1_remz = self.mc1_angle[self.mc1_curves-1]
-        if self.version_mc_curve == self.ORIENTED_VERSION_MC_CURVE or \
-           self.version_mc_curve == self.PARAMETER_PM_CURVE:
+        if self.version_mc_curve in (self.ORIENTED_VERSION_MC_CURVE,
+                                     self.PARAMETER_PM_CURVE):
             logging.debug("write mc1_curves %d", self.mc1_curves)
             self.writeBlock([float(self.mc1_remz), float(self.mc1_bsat),
                              float(self.mc1_bref), float(mc1_fillfac),
                              self.mc1_curves])
 
         if mc1_type == DEMCRV_BR:
             self.mc1_angle[self.mc1_curves-1] = self.mc1_remz
@@ -484,19 +484,38 @@
                  for j in range(self.MC1_NIMAX)],
                 [float(lb[j]) if j < len(lb) else 0.
                  for j in range(self.MC1_NIMAX)],
                 [0.]*50,
                 [0.]*50
             ]))
 
-            #
-            if self.version_mc_curve == self.ORIENTED_VERSION_MC_CURVE or \
-               self.version_mc_curve == self.PARAMETER_PM_CURVE:
+            if self.version_mc_curve in (self.ORIENTED_VERSION_MC_CURVE,
+                                         self.PARAMETER_PM_CURVE):
                 self.writeBlock([self.mc1_angle[K], self.mc1_db2[K]])
 
+        if not (self.mc1_ch_factor or self.mc1_cw_factor) and self.losses:
+            pfe = self.losses['pfe']
+            f = self.losses['f']
+            B = self.losses['B']
+            colsize = len(f)
+            losses = [list(p) + [0]*(colsize-len(p)) for p in pfe]
+            fo = self.mc1_base_frequency
+            Bo = self.mc1_base_induction
+            fit_jordan = False
+            if fit_jordan:
+                ch, alfa, cw, beta, gamma = lc.fitjordan(f, B, losses, Bo, fo)
+                self.mc1_ch_factor = ch
+                self.mc1_ch_freq_factor = alfa
+            else:
+                cw, beta, gamma = lc.fitsteinmetz(f, B, losses, Bo, fo)
+                self.mc1_ch_factor = 0
+                self.mc1_ch_freq_factor = 0
+            self.mc1_cw_factor = cw
+            self.mc1_cw_freq_factor = beta
+            self.mc1_induction_factor = gamma
         self.writeBlock([float(self.mc1_base_frequency),
                          float(self.mc1_base_induction),
                          float(self.mc1_ch_factor),
                          float(self.mc1_cw_factor),
                          float(self.mc1_ch_freq_factor),
                          float(self.mc1_cw_freq_factor),
                          float(self.mc1_induction_factor),
@@ -507,25 +526,30 @@
             return
 
         try:
             nfreq = len([1 for x in self.losses['f'] if x > 0])
             nind = len(self.losses['B'])
             if nind < 1 or nfreq < 1:
                 return
+            fo = self.losses.get('fo',
+                                 self.mc1_base_frequency)
+            Bo = self.losses.get('Bo',
+                                 self.mc1_base_induction)
             if np.isscalar(self.losses['B'][0]):
                 B = self.losses['B']
                 pfe = self.losses['pfe']
-                cw = self.losses['cw']
-                alfa = self.losses['cw_freq']
-                beta = self.losses['b_coeff']
+                if 'cw' not in self.losses:
+                    cw, alfa, beta = lc.fitsteinmetz(
+                        self.losses['f'], self.losses['B'], self.losses['pfe'], Bo, fo)
+                    self.losses['cw'] = cw
+                    self.losses['cw_freq'] = alfa
+                    self.losses['b_coeff'] = beta
+                    self.losses['Bo'] = Bo
+                    self.losses['fo'] = fo
             else:
-                fo = self.losses.get('fo',
-                                     self.mc1_base_frequency)
-                Bo = self.losses.get('Bo',
-                                     self.mc1_base_induction)
                 cw, alfa, beta = lc.fitsteinmetz(
                     self.losses['f'], self.losses['B'], self.losses['pfe'], Bo, fo)
                 B, pfe = norm_pfe(self.losses['B'], self.losses['pfe'])
                 nind = len(B)
                 self.losses['cw'] = cw
                 self.losses['cw_freq'] = alfa
                 self.losses['b_coeff'] = beta
@@ -533,21 +557,29 @@
                 self.losses['fo'] = fo
 
             self.writeBlock([nfreq, nind])
             self.writeBlock(B +
                             [0.0]*(M_LOSS_INDUCT - nind))
 
             for f, p in zip(self.losses['f'], pfe):
-                if f is not None:
-                    pl = [px if px is not None else lc.pfe_steinmetz(
-                        f, b, cw, alfa, beta,
-                        self.losses['fo'],
-                        self.losses['Bo'])
-
-                        for px, b in zip(p, B)]
+                if f > 0:
+                    y = np.array(p)
+                    losses = y[y != np.array(None)].tolist()
+                    if len(losses) == nind:
+                        pl = p
+                    else:
+                        n = len(losses)
+                        cw, alfa, beta = lc.fitsteinmetz(
+                            f, B[:n], losses, Bo, fo)
+                        pl = [lc.pfe_steinmetz(
+                            f, b, cw, alfa, beta,
+                            self.losses['fo'],
+                            self.losses['Bo'])
+                              for b in B]
+                    logger.debug("%s", pl)
                     self.writeBlock(pl +
                                     [0.0]*(M_LOSS_INDUCT - len(pl)))
                     self.writeBlock(f)
             for m in range(M_LOSS_FREQ - len(pfe)):
                 self.writeBlock([0.0]*M_LOSS_INDUCT)
                 self.writeBlock(0.0)
 
@@ -806,17 +838,20 @@
                 self.losses['B'] = self.readBlock(
                     [float]*M_LOSS_INDUCT)[:njind]
                 self.losses['f'] = []
                 self.losses['pfe'] = []
                 for i in range(M_LOSS_FREQ):
                     res = self.readBlock([float]*M_LOSS_INDUCT)
                     f = self.readBlock(float)
-                    if f != None:
+                    if i<nfreq and f != None:
                         self.losses['pfe'].append(res[:njind])
                         self.losses['f'].append(f)
+                    else:
+                        self.losses['f'].append(0)
+                        self.losses['pfe'].append([0]*njind)
                 (cw, alfa, beta, basefreq, baseind) = self.readBlock([float]*5)
                 self.losses['fo'] = basefreq
                 self.losses['Bo'] = baseind
                 self.losses['cw'] = cw
                 self.losses['cw_freq'] = alfa
                 self.losses['b_coeff'] = beta
                 self.losses['ch'] = self.ch
```

### Comparing `femagtools-1.2.9/femagtools/me.py` & `femagtools-1.3.0/femagtools/me.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/model.py` & `femagtools-1.3.0/femagtools/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,19 +176,14 @@
             self.commutator = self.windings['wdgtype'] == 'CMM'
         except AttributeError:
             self.commutator = False
         try:
             self.windings['cufilfact'] = self.windings['fillfac']
         except (KeyError, AttributeError):
             pass
-        try:
-            if 'leak_dist_wind' in self.windings:
-                self.windings['leak_dist_wind']['wiredia'] = self.windings['dia_wire']
-        except:
-            pass
 
     def set_num_slots_gen(self):
         if 'num_slots_gen' not in self.stator:
             try:
                 m = self.windings['num_phases']
             except (KeyError, AttributeError):
                 m = 1
@@ -427,13 +422,16 @@
         if parameters.get('calculationMode', '') == 'asyn_motor':
             self.recsin = 'flux'
 
     def get_num_cur_steps(self):
         """returns number of curSteps (used for progress calc)"""
         try:
             if self.calculationMode == 'psd_psq_fast':
-                return self.round((self.maxiq-self.miniq)/self.delta_iq) + 1
+                return round(
+                    ((self.maxiq-self.minid)/self.delta_id) + 1)
             if self.calculationMode == 'ld_lq_fast':
-                return self.num_cur_steps+1  # must include 0
-        except:
+                return (self.num_cur_steps+1)  # must include 0
+        except AttributeError as e:
+            logger.warning("%s current steps of %s",
+                           e, self.calculationMode)
             pass
         return 1
```

### Comparing `femagtools-1.2.9/femagtools/moo/algorithm.py` & `femagtools-1.3.0/femagtools/moo/algorithm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/moo/population.py` & `femagtools-1.3.0/femagtools/moo/population.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/moo/problem.py` & `femagtools-1.3.0/femagtools/moo/problem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/moproblem.py` & `femagtools-1.3.0/femagtools/moproblem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/multiproc.py` & `femagtools-1.3.0/femagtools/multiproc.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,38 +25,40 @@
     DEVNULL = open(os.devnull, 'wb')
 
 logger = logging.getLogger(__name__)
 
 numpat = re.compile(r'([+-]?\d+(?:\.\d+)?(?:[eE][+-]\d+)?)\s*')
 
 class LicenseError(Exception):
-    pass 
+    pass
 
 class ProtFile:
     def __init__(self, dirname, num_cur_steps):
         self.size = 0
         self.looplen = 0
         self.cur_steps = [1, num_cur_steps]
         self.n = 0
         self.num_loops = 0
         self.dirname = dirname
+        self.name = 'samples'
 
     def percent(self):
         if self.looplen > 0:
             return 100 * self.n / self.looplen
         return 0
 
     def update(self):
         p = list(pathlib.Path(self.dirname).glob('*.PROT'))
         if p:
+            buf = ''
             if self.size < p[0].stat().st_size:
                 with p[0].open() as fp:
                     fp.seek(self.size)
                     buf = fp.read()
-                return self.append(buf)
+            return self.append(buf)
         return ''
 
     def append(self, buf):
         self.size += len(buf)
         for line in [l.strip() for l in buf.split('\n') if l]:
             if line.startswith('Loop'):
                 self.n = 0
@@ -71,14 +73,16 @@
                 self.looplen = cur_steps*beta_steps*move_steps
                 self.num_loops += 1
             elif (line.startswith('Cur') or
                   line.startswith('Id')):
                 self.n += 1
             elif line.startswith('Number movesteps Fe-Losses'):
                 return ''
+            elif line.startswith('begin'):
+                self.name = line.split()[1].strip()
 
         return f'{self.percent():3.1f}%'  # {self.n}/{self.looplen}'
 
 
 class ProgressLogger(threading.Thread):
     def __init__(self, dirs, num_cur_steps, timestep):
         threading.Thread.__init__(self)
@@ -94,15 +98,18 @@
         while self.running:
             time.sleep(self.timestep)
             logmsg = [p.update() for p in protfiles]
             summary = [l  # f'<{i}> {l}'
                        for i, l in enumerate(logmsg)
                        if l]
             if summary:
-                logger.info('Samples %s', ', '.join(summary))
+                labels = set([p.name for p in protfiles])
+                logger.info('%s: %s',
+                            ', '.join(labels),
+                            ', '.join(summary))
             else:
                 logger.info('collecting FE losses ...')
                 return
 
     def stop(self):
         self.running = False
 
@@ -137,22 +144,22 @@
 
             #logger.info("Finished pid: %d return %d",
             #            proc.pid, proc.returncode)
             #return proc.returncode
         except OSError as e:
             logger.error("Starting process failed: %s, Command: %s", e, cmd)
             raise
-        
+
     # raise License Error
-    if proc.returncode != 0: 
-        with open(os.path.join(workdir, "femag.err"), "r") as err: 
-            for line in err: 
-                if 'license' in line: 
+    if proc.returncode != 0:
+        with open(os.path.join(workdir, "femag.err"), "r") as err:
+            for line in err:
+                if 'license' in line:
                     raise LicenseError(line)
-                
+
     logger.info("Finished pid: %d return %d", proc.pid, proc.returncode)
     return proc.returncode
 
 
 class Engine:
     """The MultiProc engine uses a pool of local calculation processes.
 
@@ -171,15 +178,15 @@
         cmd = kwargs.get('cmd', '')
         if cmd:
             self.cmd = [cmd]
             if platform.system() == 'Windows':
                 self.cmd.append('-m')
 
         self.progressLogger = 0
-        self.progress_timestep = kwargs.get('timestep', 3)
+        self.progress_timestep = kwargs.get('timestep', 5)
 
     def create_job(self, workdir):
         """Create a FEMAG :py:class:`Job`
 
         Args:
             workdir: The workdir where the calculation files are stored
 
@@ -253,8 +260,7 @@
             self.progressLogger.stop()
         # terminate pool
         try:
             self.pool.terminate()
             self.pool.close()
         except AttributeError:
             logger.warn("%s", e)
-
```

### Comparing `femagtools-1.2.9/femagtools/mxw2msh.py` & `femagtools-1.3.0/femagtools/mxw2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/nc.py` & `femagtools-1.3.0/femagtools/nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/netlist.py` & `femagtools-1.3.0/femagtools/netlist.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/ntib.py` & `femagtools-1.3.0/femagtools/ntib.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/opt.py` & `femagtools-1.3.0/femagtools/opt.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/parstudy.py` & `femagtools-1.3.0/femagtools/parstudy.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,15 +276,15 @@
                         task.add_file(mc)
                     set_magnet_properties(model, fea, self.femag.magnets)
                     task.add_file(
                         'femag.fsl',
                         builder.create_model(model, self.femag.magnets) +
                         builder.create_analysis(fea) +
                         ['save_model("close")'])
-                    
+
                 if hasattr(fea, 'poc'):
                     task.add_file(fea.pocfilename,
                                   fea.poc.content())
                 if hasattr(fea, 'stateofproblem'):
                     task.set_stateofproblem(fea.stateofproblem)
 
             tstart = time.time()
@@ -403,15 +403,15 @@
 
     def _get_names_and_range(self, dvars, num_samples):
         dvarnames = [d['name'] for d in dvars]
         l_bounds = [d['bounds'][0] for d in dvars]
         u_bounds = [d['bounds'][1] for d in dvars]
 
         N = num_samples
-        sampler = sc.stats.qmc.LatinHypercube(d=len(l_bounds), centered=True)
+        sampler = sc.stats.qmc.LatinHypercube(d=len(l_bounds), scramble=False)
         sample = sampler.random(n=N)
         par_range = sc.stats.qmc.scale(sample, l_bounds, u_bounds)
         domain = par_range.T.tolist()
         return dvarnames, domain, par_range
 
 
 class Sobol(ParameterStudy):
```

### Comparing `femagtools-1.2.9/femagtools/plot.py` & `femagtools-1.3.0/femagtools/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1140,26 +1140,26 @@
     """
     import femagtools.losscoeffs as lc
     if ax == 0:
         ax = plt.gca()
 
     fo = losses['fo']
     Bo = losses['Bo']
-    B = plt.np.linspace(0.9*np.min(losses['B']),
+    B = np.linspace(0.9*np.min(losses['B']),
                         1.1*0.9*np.max(losses['B']))
 
     for i, f in enumerate(losses['f']):
         pfe = [p for p in np.array(losses['pfe'])[i] if p]
         if f > 0:
             if len(coeffs) == 5:
                 ax.plot(B, lc.pfe_jordan(f, B, *coeffs, fo=fo, Bo=Bo))
             elif len(coeffs) == 3:
                 ax.plot(B, lc.pfe_steinmetz(f, B, *coeffs, fo=fo, Bo=Bo))
-        plt.plot(losses['B'][:len(pfe)], pfe,
-                 marker='o', label="{} Hz".format(f))
+            ax.plot(losses['B'][:len(pfe)], pfe,
+                    marker='o', label="{} Hz".format(f))
 
     ax.set_title("Fe Losses/(W/kg) " + title)
     if log:
         ax.set_yscale('log')
         ax.set_xscale('log')
     ax.set_xlabel("Flux Density [T]")
     # plt.ylabel("Pfe [W/kg]")
@@ -1730,15 +1730,15 @@
     from matplotlib.patches import PathPatch
     x = [60*n for n in speed]
     y = torque
     if not levels:
         if max(z) <= 1:
             if max(z) > 0.96:
                 levels = [0.5, 0.75, 0.8, 0.84,
-                          0.88, 0.91, 0.93, 0.95, 0.97]
+                          0.89, 0.92, 0.94, 0.96, 0.97]
             else:
                 levels = [0.25, 0.5, 0.75, 0.8, 0.84,
                           0.88, 0.9, 0.92, 0.94, 0.96]
 
             if max(z) > levels[-1]:
                 levels.append(np.ceil(max(z)*100)/100)
         else:
```

### Comparing `femagtools-1.2.9/femagtools/poc.py` & `femagtools-1.3.0/femagtools/poc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/FE-losses.mako` & `femagtools-1.3.0/femagtools/templates/FE-losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/asyn_motor.mako` & `femagtools-1.3.0/femagtools/templates/asyn_motor.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/basic_modpar.mako` & `femagtools-1.3.0/femagtools/templates/basic_modpar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/calc_field_ts.mako` & `femagtools-1.3.0/femagtools/templates/calc_field_ts.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/cogg_calc.mako` & `femagtools-1.3.0/femagtools/templates/cogg_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/com_motor_sim.mako` & `femagtools-1.3.0/femagtools/templates/com_motor_sim.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/cu_losses.mako` & `femagtools-1.3.0/femagtools/templates/cu_losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/ec-rotorbar.mako` & `femagtools-1.3.0/femagtools/templates/ec-rotorbar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/fe-contr.mako` & `femagtools-1.3.0/femagtools/templates/fe-contr.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/gen_winding.mako` & `femagtools-1.3.0/femagtools/templates/gen_winding.mako`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 % if model.windings['wdgtype'] == 'CMM':
 --  GEN_CMM_WDG
 
-m.s_or_w_windg    = ${model.windings.get('s_or_w_windg', 1)} --   Lap/wave/frog-leg winding = 1/2/3       
-m.numpl_sw        = ${model.windings.get('numpl_sw', 1)} --   Number of plex of lap winding: m_l      
-m.numpl_ww        = ${model.windings.get('numpl_ww', 1)} --   Number of plex of wave winding: m_w     
-m.foreward        = ${model.windings.get('foreward', 1)} --   Progressive = 1 / retrogressive = 2     
-m.num_wires       = ${model.windings.get('num_wires', 1)} --   Number of wires per slot side w_sp      
-m.current         =       0     --   Armat.-Wdg-Current[A] or flux[Vs/mm]    
-m.wind_type       =       1     --   Wdg-coil:1=w&cur;2=w&flux;3=bar&cur     
-m.num_layers      = ${model.windings.get('num_layers', 1)} --   Number of coil sides per slot layer:u   
-m.pitch_fact      = ${model.windings.get('pitch_fact', 1)} --   Short pitch factor : beta_v             
-m.dc_ac           = ${model.windings.get('dc_ac', 0)}     --   Current: DC: 0; AC: 1                   
- 
+m.s_or_w_windg    = ${model.windings.get('s_or_w_windg', 1)} --   Lap/wave/frog-leg winding = 1/2/3
+m.numpl_sw        = ${model.windings.get('numpl_sw', 1)} --   Number of plex of lap winding: m_l
+m.numpl_ww        = ${model.windings.get('numpl_ww', 1)} --   Number of plex of wave winding: m_w
+m.foreward        = ${model.windings.get('foreward', 1)} --   Progressive = 1 / retrogressive = 2
+m.num_wires       = ${model.windings.get('num_wires', 1)} --   Number of wires per slot side w_sp
+m.current         =       0     --   Armat.-Wdg-Current[A] or flux[Vs/mm]
+m.wind_type       =       1     --   Wdg-coil:1=w&cur;2=w&flux;3=bar&cur
+m.num_layers      = ${model.windings.get('num_layers', 1)} --   Number of coil sides per slot layer:u
+m.pitch_fact      = ${model.windings.get('pitch_fact', 1)} --   Short pitch factor : beta_v
+m.dc_ac           = ${model.windings.get('dc_ac', 0)}     --   Current: DC: 0; AC: 1
+
  pre_models("GEN_CMM_WDG")
 -- gen cmm
 pre_models("GEN_CMM"); -- autm. generate cmm File (requires femag rel >=9.2)"
 % elif 'wdgfile' in model.windings:
 def_new_wdg('${model.windings.get("wdgfile")}')
-pre_models("gen_pocfile") 
+pre_models("gen_pocfile")
 % else:
 --  Gen_winding
 if m.xcoil_1 ~= nil then
   m.wdg_location = 1 --stator
 end
 
 m.num_phases      =  ${model.get(['windings','num_phases'])}
@@ -29,38 +29,38 @@
 m.num_wires       =  ${model.get(['windings','num_wires'])}
 m.coil_span       =  ${model.get(['windings','coil_span'])}
 % if 'num_poles' in model.windings:
 m.num_poles       =  ${model.get(['windings','num_poles'])}
 % endif
 % if model.get('move_action', 0) == 0:
 m.current         =   0.0
-m.mat_type        =   1.0 -- rotating 
+m.mat_type        =   1.0 -- rotating
 m.wind_type       =   1.0 -- winding & current
 m.win_asym        =   1.0 -- sym
 
 m.curr_inp        =   0.0 -- const
 m.dq_offset       =   0
 
 % if model.get(['stator', 'num_slots_gen']) == 1:
 def_new_wdg(m.xcoil_1, m.ycoil_1, "green", "1", m.num_wires, 0.0, "wi")
 add_to_wdg(m.xcoil_2, m.ycoil_2, "wsamekey", "wo", "wser")
 % else:
 pre_models("Gen_winding")
-pre_models("gen_pocfile") 
+pre_models("gen_pocfile")
 % endif
 % else:
 color={"green", "yellow", "magenta", "lightgrey", "darkred", "skyblue", "violet"}
 wkey={0,0,0,0,0,0}
 --
 bz = m.width_bz
 --
 ys = m.slot_height/2
 
 dirl = 1
-for i=1, m.num_phases do	
+for i=1, m.num_phases do
   wdg = "w"..i
   for g=1, m.num_sl_gen/m.num_phases/2 do
     xs = 2*bz*((i-1) + (g-1)*m.num_phases)
     if g == 1 then
       wkey[i]=def_new_wdg(xs + bz/3, ys, color[i], wdg, m.num_wires, 0, dirl)
     else
       add_to_wdg(xs + bz/3, ys, color[i], wkey[i], dirl, "wser")
@@ -77,15 +77,15 @@
     if m.num_layers > 1 then
       add_to_wdg(xs + bz + bz/3, ys, wkey[i], dirl, "wser")
     end
   end
 end
 
 ----------------------------------------------------------------------
--- create poc-File 
+-- create poc-File
 ----------------------------------------------------------------------
 base_angle = 0.0
 period = 2*m.tot_num_slot*m.width_bz/m.num_poles
 f = assert(io.open(model..'_'..m.num_poles.."p.poc","w"));
   f:write(string.format("          %i\n",m.num_phases));
   for i = 1, m.num_phases do
     if i<10      then f:write(string.format("          %i\n",i));
@@ -108,8 +108,35 @@
   f:write("          0\n");
 io.close(f);
 
 %endif
 % if 'num_poles' in model.windings:
 m.num_poles       =  ${model.poles}
 % endif
-% endif
+% endif
+
+% if 'thcap' in model.windings:
+-- Thermal Material properties
+rw = da1/2 +(m.slot_height-m.slot_h1)/2
+dw = 0
+dr = 0
+if m.middle_line == 1 then
+  dw = 1/60
+elseif m.middle_line == 2 then
+  dr = 1
+end
+lamCu = 400
+capCu = 385
+da = 1.0785
+dCu = 1.0
+lam = lamCu*(dCu/(da-dCu)+(da-dCu)/da)
+cap = capCu*da^2/(dCu^2*math.pi/4)
+for i=1,m.num_sl_gen do
+  a = (2*i-1)*math.pi/m.tot_num_sl + m.zeroangl/180*math.pi
+  xwl,ywl = pr2c(rw+dr,a+dw)
+  def_mat_therm(xwl,ywl,'yellow',8920,lam,cap,1)
+  if m.middle_line > 0 then
+    xwr,ywr = pr2c(rw-dr,a-dw)
+    def_mat_therm(xwr,ywr,'yellow',8920,lam,cap,1)
+  end
+end
+%endif
```

### Comparing `femagtools-1.2.9/femagtools/templates/inductances.mako` & `femagtools-1.3.0/femagtools/templates/inductances.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/ld_lq_fast.mako` & `femagtools-1.3.0/femagtools/templates/ld_lq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/leak_dist_wind.mako` & `femagtools-1.3.0/femagtools/templates/leak_dist_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/leak_evol_wind.mako` & `femagtools-1.3.0/femagtools/templates/leak_evol_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/magnet-data.mako` & `femagtools-1.3.0/femagtools/templates/magnet-data.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/magnetFC2.mako` & `femagtools-1.3.0/femagtools/templates/magnetFC2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/magnetIron.mako` & `femagtools-1.3.0/femagtools/templates/magnetIron4.mako`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 
 m.magn_rad       = da2/2
 m.yoke_rad       = dy2/2
 
 m.magn_height     =    ${model['magn_height']*1e3}
 m.magn_width      =    ${model['magn_width']*1e3}
 m.gap_ma_iron     =    ${model['gap_ma_iron']*1e3}
-m.air_triangle    =    ${model.get('air_triangle', 0)}
-m.iron_height     =    ${model['iron_height']*1e3}
-m.magn_rem        =    ${model['magn_rem']}
-m.shaft_rad      =     ${model['condshaft_r']*1e3}
-m.magn_ori        =    ${model['magn_ori']}
-m.bridge_height   =    ${model['bridge_height']*1e3}
-m.bridge_width    =    ${model['bridge_width']*1e3}
 m.iron_shape      =    ${model['iron_shape']*1e3}
-
+m.air_space_h     =    ${model['air_space_h']*1e3}
+m.iron_bfe        =    ${model['iron_bfe']*1e3}
+m.magn_di_ra      =    ${model['magn_di_ra']*1e3}
+m.corner_r        =    ${model['corner_r']*1e3}
+m.air_sp_ori      =    ${model['air_sp_ori']}
+m.magn_ori        =    ${model['magn_ori']}
+m.magn_num        =    ${model['magn_num']}
+m.cond_shaft      =    0.0 -- ignored
 m.zeroangl        =    ${model.get('zeroangle',0)}
 
 m.mcvkey_yoke     =   mcvkey_yoke
+m.mcvkey_mshaft    =  mcvkey_shaft
 m.nodedist        =   ${model.get('nodedist',1)}
 
- pre_models("Magnet in Iron")
+ pre_models("Magnet Iron 4")
 
 %if model.get('mcvkey_magnet', ''):
 gamma = 0
 for i = 0, m.npols_gen-1 do
     alfa = (2*i+1)*180/m.num_poles
-    x0, y0 = pd2c((m.magn_rad-m.magn_height/2)*math.cos(math.pi/m.num_poles), alfa)
+    x0, y0 = pd2c(m.magn_rad - m.magn_height/2 - m.magn_di_ra, alfa)
     if i < 2 and m.npols_gen > 1 then
         delete_sreg(x0, y0)
     end
     if m.orient == "cartaniso" or m.orient == "cartiso" then
         gamma = alfa
-    end
+    end    
     if i % 2 == 0 then
         def_mat_pm_nlin(x0, y0, "red", m.mcvkey_magnet, gamma, m.orient, m.magncond, m.rlen)
     else
         def_mat_pm_nlin(x0, y0, "green", m.mcvkey_magnet, gamma-180, m.orient, m.magncond, m.rlen)
     end
 end
 %endif
```

### Comparing `femagtools-1.2.9/femagtools/templates/magnetIron2.mako` & `femagtools-1.3.0/femagtools/templates/magnetIron2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/magnetIron3.mako` & `femagtools-1.3.0/femagtools/templates/magnetIron3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/magnetIron4.mako` & `femagtools-1.3.0/femagtools/templates/magnetIron5.mako`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 
 m.magn_rad       = da2/2
 m.yoke_rad       = dy2/2
 
 m.magn_height     =    ${model['magn_height']*1e3}
 m.magn_width      =    ${model['magn_width']*1e3}
 m.gap_ma_iron     =    ${model['gap_ma_iron']*1e3}
-m.iron_shape      =    ${model['iron_shape']*1e3}
-m.air_space_h     =    ${model['air_space_h']*1e3}
 m.iron_bfe        =    ${model['iron_bfe']*1e3}
-m.magn_di_ra      =    ${model['magn_di_ra']*1e3}
+m.air_space_h     =    ${model['air_space_h']*1e3}
 m.corner_r        =    ${model['corner_r']*1e3}
 m.air_sp_ori      =    ${model['air_sp_ori']}
-m.magn_ori        =    ${model['magn_ori']}
 m.magn_num        =    ${model['magn_num']}
-m.cond_shaft      =    0.0 -- ignored
-m.zeroangl        =    ${model.get('zeroangle',0)}
+m.iron_shape      =    ${model['iron_shape']*1e3}
+m.air_space_b     =    ${model['air_space_b']*1e3}
+m.magn_di_ra      =    ${model['magn_di_ra']*1e3}
+
+m.zeroangl        =   ${model.get('zeroangle',0)}
 
 m.mcvkey_yoke     =   mcvkey_yoke
-m.mcvkey_mshaft    =  mcvkey_shaft
+m.mcvkey_mshaft   =   mcvkey_shaft
 m.nodedist        =   ${model.get('nodedist',1)}
 
- pre_models("Magnet Iron 4")
+ pre_models("Magnet Iron 5")
 
 %if model.get('mcvkey_magnet', ''):
 gamma = 0
 for i = 0, m.npols_gen-1 do
     alfa = (2*i+1)*180/m.num_poles
     x0, y0 = pd2c(m.magn_rad - m.magn_height/2 - m.magn_di_ra, alfa)
     if i < 2 and m.npols_gen > 1 then
         delete_sreg(x0, y0)
     end
-    if m.orient == "cartaniso" or m.orient == "cartiso" then
+    if m.orient == mcartaniso or m.orient == mcartiso then
         gamma = alfa
-    end    
+    end
     if i % 2 == 0 then
         def_mat_pm_nlin(x0, y0, "red", m.mcvkey_magnet, gamma, m.orient, m.magncond, m.rlen)
     else
         def_mat_pm_nlin(x0, y0, "green", m.mcvkey_magnet, gamma-180, m.orient, m.magncond, m.rlen)
     end
 end
 %endif
```

### Comparing `femagtools-1.2.9/femagtools/templates/magnetSector.mako` & `femagtools-1.3.0/femagtools/templates/magnetSector.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/magnetSectorLinear.mako` & `femagtools-1.3.0/femagtools/templates/magnetSectorLinear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/magnetShell.mako` & `femagtools-1.3.0/femagtools/templates/magnetShell.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/magnetShell2.mako` & `femagtools-1.3.0/femagtools/templates/magnetShell2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/mesh-airgap.mako` & `femagtools-1.3.0/femagtools/templates/mesh-airgap.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/modal_analysis.mako` & `femagtools-1.3.0/femagtools/templates/modal_analysis.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/mult_cal_fast.mako` & `femagtools-1.3.0/femagtools/templates/mult_cal_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/noloadflux-rot.mako` & `femagtools-1.3.0/femagtools/templates/noloadflux-rot.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/noloadflux.mako` & `femagtools-1.3.0/femagtools/templates/noloadflux.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/noloadfluxdc.mako` & `femagtools-1.3.0/femagtools/templates/noloadfluxdc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/plots.mako` & `femagtools-1.3.0/femagtools/templates/plots.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/pm_sym_f_cur.mako` & `femagtools-1.3.0/femagtools/templates/pm_sym_f_cur.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/pm_sym_fast.mako` & `femagtools-1.3.0/femagtools/templates/pm_sym_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/pm_sym_loss.mako` & `femagtools-1.3.0/femagtools/templates/pm_sym_loss.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/psd_psq_fast.mako` & `femagtools-1.3.0/femagtools/templates/psd_psq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/ring.mako` & `femagtools-1.3.0/femagtools/templates/ring.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/rot_hsm.mako` & `femagtools-1.3.0/femagtools/templates/rot_hsm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/rotorAsyn.mako` & `femagtools-1.3.0/femagtools/templates/rotorAsyn.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/rotorKs2.mako` & `femagtools-1.3.0/femagtools/templates/rotorKs2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/rotor_msh.mako` & `femagtools-1.3.0/femagtools/templates/rotor_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/rotor_winding.mako` & `femagtools-1.3.0/femagtools/templates/rotor_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/shortcircuit.mako` & `femagtools-1.3.0/femagtools/templates/shortcircuit.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/srm.mako` & `femagtools-1.3.0/femagtools/templates/srm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/stator1.mako` & `femagtools-1.3.0/femagtools/templates/stator1.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/stator2.mako` & `femagtools-1.3.0/femagtools/templates/stator2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/stator3Linear.mako` & `femagtools-1.3.0/femagtools/templates/stator3Linear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/stator4.mako` & `femagtools-1.3.0/femagtools/templates/stator4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/statorBG.mako` & `femagtools-1.3.0/femagtools/templates/statorBG.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/statorRing.mako` & `femagtools-1.3.0/femagtools/templates/statorRing.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/statorRotor3.mako` & `femagtools-1.3.0/femagtools/templates/statorRotor3.mako`

 * *Files 22% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 m.slot_h2     = ${model['slot_h2']*1e3}
 m.slot_width  = ${model['slot_width']*1e3}
 m.slot_r1     = ${model['slot_r1']*1e3}
 m.slot_r2     = ${model['slot_r2']*1e3}
 m.wedge_width1= ${model['wedge_width1']*1e3}
 m.wedge_width2= ${model['wedge_width2']*1e3}
 m.middle_line = ${model.get('middle_line',0)}
-m.tooth_width = ${model['tooth_width']*1e3}
+m.tooth_width = ${model.get('tooth_width',0)*1e3}
 m.slot_top_sh = ${model['slot_top_sh']}
 
 m.zeroangl    = ${model.get('zeroangle',0)}
 m.rlength     = ${model.get('rlength',1)*100}
 
 m.mcvkey_yoke = mcvkey_yoke
 
@@ -138,8 +138,33 @@
      r = (m.inside_diam - m.slot_height)/2
   else
      r = (m.inside_diam + m.slot_height)/2
   end
   x0, y0 = pr2c(r, 2*math.pi/m.tot_num_slot + m.zeroangl/180*math.pi)
    def_mat_fm_nlin(x0, y0, "blue", mcvkey_teeth, m.rlength)
 end
-%endif
+%endif
+
+%if model.get('thcond', 0) and model.get('thcap', 0):
+
+-- Thermal properties: iron in yoke and tooth
+xst,yst = pd2c(m.inside_diam/2+1,m.zeroangl+0.1)    -- stator tooth
+xsj,ysj = pd2c(m.yoke_diam/2-1,m.zeroangl+0.1)  -- stator yoke
+thcond = 24
+thcap = 480
+def_mat_therm(xst,yst,'darkblue',7700,thcond,thcap,1)
+def_mat_therm(xsj,ysj,'darkblue',7700,thcond,thcap,1)
+-- insulation
+if m.slot_indul > 0 then
+  thickness = 0.25 -- mm
+  thcond = 0.31
+  thcap = 1100
+  xip, yip = pr2c(m.slot_height + m.inside_diam/2-m.slot_indul/2,
+                  math.pi/m.tot_num_slot+m.zeroangl/180*math.pi)
+  def_insulation(xip,yip,'darkred',thickness,1340,thcond,thcap)
+end
+-- air in slot opening
+xnl, ynl = pr2c(m.inside_diam/2+m.slot_h1/2, math.pi/m.tot_num_slot+m.zeroangl/180*math.pi)
+sl_cond = 0.15
+sl_cap = 1007
+def_mat_therm(xnl,ynl,'cyan',1.19,sl_cond,sl_cap,1)
+%endif
```

### Comparing `femagtools-1.2.9/femagtools/templates/stator_msh.mako` & `femagtools-1.3.0/femagtools/templates/stator_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/templates/torq_calc.mako` & `femagtools-1.3.0/femagtools/templates/torq_calc.mako`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 % if model.get('lfe',0):
 m.arm_length      =    ${model.get('lfe')*1e3}
 % endif
 % if model.get('move_action', 0) == 0:
 m.speed           =    ${model.get('speed')*60}
 m.skew_angle      =    ${model.get('skew_angle',0)}
 m.fc_radius2      =    0.0
-m.phi_start       =    ${model.get('phi_start', 0)}
-m.range_phi       =    ${model.get('range_phi', 0)}
+% if model.get('range_start', 0):
+m.phi_start       =    ${model['phi_start']}
+%endif
+% if model.get('range_phi', 0):
+m.range_phi       =    ${model['range_phi']}
+%endif
 % else:
 m.speed_linear    =    ${model.get('speed')}
 m.skew_linear     =    ${model.get('skew_displ',0)}
 m.line            =    0
 m.two_pole_wi     =    2*m.pole_width
 m.range_x         =    m.two_pole_wi
 m.range_y         =    0.0
```

### Comparing `femagtools-1.2.9/femagtools/tks.py` & `femagtools-1.3.0/femagtools/tks.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/ts.py` & `femagtools-1.3.0/femagtools/ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/vbf.py` & `femagtools-1.3.0/femagtools/vbf.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/vtu.py` & `femagtools-1.3.0/femagtools/vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools/windings.py` & `femagtools-1.3.0/femagtools/windings.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/femagtools.egg-info/PKG-INFO` & `femagtools-1.3.0/femagtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.2.9
+Version: 1.3.0
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.2.9/femagtools.egg-info/SOURCES.txt` & `femagtools-1.3.0/femagtools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 femagtools/moo/population.py
 femagtools/moo/problem.py
 femagtools/templates/FE-losses.mako
 femagtools/templates/airgapinduc.mako
 femagtools/templates/asyn_motor.mako
 femagtools/templates/basic_modpar.mako
 femagtools/templates/calc_field_ts.mako
+femagtools/templates/calc_therm_field.mako
 femagtools/templates/cogg_calc.mako
 femagtools/templates/colorgrad.mako
 femagtools/templates/com_motor_sim.mako
 femagtools/templates/conduct-data.mako
 femagtools/templates/connect_models.mako
 femagtools/templates/cu_losses.mako
 femagtools/templates/ec-rotorbar.mako
@@ -134,14 +135,16 @@
 femagtools/templates/stator2.mako
 femagtools/templates/stator3Linear.mako
 femagtools/templates/stator4.mako
 femagtools/templates/statorBG.mako
 femagtools/templates/statorRing.mako
 femagtools/templates/statorRotor3.mako
 femagtools/templates/stator_msh.mako
+femagtools/templates/therm-dynamic.mako
+femagtools/templates/therm-static.mako
 femagtools/templates/torq_calc.mako
 tests/test_airgap_induction.py
 tests/test_amela.py
 tests/test_asm.py
 tests/test_bchreader.py
 tests/test_conductor.py
 tests/test_convert.py
```

### Comparing `femagtools-1.2.9/pyproject.toml` & `femagtools-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_airgap_induction.py` & `femagtools-1.3.0/tests/test_airgap_induction.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_amela.py` & `femagtools-1.3.0/tests/test_amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_asm.py` & `femagtools-1.3.0/tests/test_asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_bchreader.py` & `femagtools-1.3.0/tests/test_bchreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_convert.py` & `femagtools-1.3.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_effloss.py` & `femagtools-1.3.0/tests/test_effloss.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,11 +23,11 @@
     u1 = 230
     temp = (120, 120)
 
     r = femagtools.machine.effloss.efficiency_losses_map(
         impars, u1, T, temp, nmax, npoints=(5, 4))
     assert r['T'] == pytest.approx(
         [-33.1, -0.6, 0.4, 32.7,
-         -25.2, -0.6, 0.4, 23.2,
-         -12.8, -0.6, 0.4, 11.6,
-         -8.7, -0.6, 0.4, 7.7,
+         -27.9, -0.6, 0.4, 25.9,
+         -13.5, -0.6, 0.4, 12.2,
+         -8.9, -0.6, 0.4, 7.8,
          -6.6, -0.6, 0.4, 5.8], abs=1e-1)
```

### Comparing `femagtools-1.2.9/tests/test_erg.py` & `femagtools-1.3.0/tests/test_erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_femag.py` & `femagtools-1.3.0/tests/test_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_forcedens.py` & `femagtools-1.3.0/tests/test_forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_fsl.py` & `femagtools-1.3.0/tests/test_fsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             slot_top_sh=0,
             slot_r2=0.002,
             slot_height=0.02,
             slot_r1=0.003,
             slot_width=0.003)
         model = femagtools.MachineModel(self.m)
         fsl = self.builder.create_stator_model(model)
-        self.assertEqual(len(fsl), 40)
+        self.assertEqual(len(fsl), 41)
 
     def test_stator4(self):
         self.m['stator']['stator4'] = dict(
             slot_height=0.1,
             slot_h1=1e-3,
             slot_h2=0,
             slot_h3=2e-3,
@@ -253,15 +253,15 @@
                 air_triangle=1,
                 iron_height=0.001,
                 condshaft_r=0.006,
                 magn_angle=130,
                 iron_shape=0))
         model = femagtools.MachineModel(self.m)
         fsl = self.builder.create_magnet_model(model)
-        self.assertEqual(len(fsl), 27)
+        self.assertEqual(len(fsl), 28)
 
     def test_magnetFC2(self):
         self.m['magnet'] = dict(
             magnetFC2=dict(
                 magn_height=0.005,
                 magn_width=0.008,
                 yoke_height=5e-3,
@@ -297,21 +297,21 @@
         fsl = self.builder.create_rotor_model(model, condMat=[])
         self.assertEqual(len(fsl), 33)
 
     def test_fe_losses(self):
         model = femagtools.MachineModel(self.m)
         fsl = self.builder.create_fe_losses(model)
         self.assertFalse(fsl)
-        self.m['ffactor'] = 1.1
+        self.m['stator']['ffactor'] = 1.1
         model = femagtools.MachineModel(self.m)
         fsl = self.builder.create_fe_losses(model)
         self.assertEqual(len(fsl), 21)
         ffact = [float(f.split('=')[1])
                  for f in fsl if f.startswith('m.ffactor')][0]
-        self.assertEqual(ffact, self.m['ffactor'])
+        self.assertEqual(ffact, self.m['stator']['ffactor'])
         feloss = [f.split('"')[1]
                   for f in fsl if f.find('pre_models') > 0][0]
         self.assertEqual(feloss, 'FE-Losses-1')
 
     def test_run_models(self):
         feapars['calculationMode'] = "cogg_calc"
         fsl = self.builder.create_analysis(feapars)
@@ -323,15 +323,15 @@
 
         feapars['calculationMode'] = "mult_cal_fast"
         fsl = self.builder.create_analysis(feapars)
         self.assertEqual(len(fsl), 31)
 
         feapars['calculationMode'] = "torq_calc"
         fsl = self.builder.create_analysis(feapars)
-        self.assertEqual(len(fsl), 26)
+        self.assertEqual(len(fsl), 24)
 
     def test_run_existing_model(self):
         model = femagtools.MachineModel('data/magnsec')
         feapars['calculationMode'] = "cogg_calc"
         fsl = self.builder.create(model, feapars)
         self.assertEqual(len(fsl), 65)
 
@@ -386,43 +386,43 @@
         for p in result['parameter']:
             self.assertTrue(p['key'] in ['dshaft', 'hm', 'bm', 'ws'])
 
     def test_gen_winding(self):
         model = femagtools.MachineModel(self.m)
 
         fsl = self.builder.create_gen_winding(model)
-        self.assertEqual(len(fsl), 20)
+        self.assertEqual(len(fsl), 21)
 
         model.windings['leak_dist_wind'] = dict(
             perimrad=1,
             vbendrad=1,
             endheight=1,
             wiredia=1)
         fsl = self.builder.create_gen_winding(model)
-        self.assertEqual(len(fsl), 33)
+        self.assertEqual(len(fsl), 34)
 
         model.windings.pop('leak_dist_wind')
         model.windings['leak_evol_wind'] = dict(
             evol1rad=1,
             evol2rad=1,
             botlevel=1,
             toplevel=1,
             endheight=1,
             evolbend=1,
             wiredia=1)
         fsl = self.builder.create_gen_winding(model)
-        self.assertEqual(len(fsl), 38)
+        self.assertEqual(len(fsl), 39)
 
         model.windings.pop('leak_evol_wind')
         model.windings['leak_tooth_wind'] = dict(
             endheight=1,
             bendrad=1,
             wiredia=1)
         fsl = self.builder.create_gen_winding(model)
-        self.assertEqual(len(fsl), 34)
+        self.assertEqual(len(fsl), 35)
 
     def test_create_model_with_magnet_material(self):
         magnetmat = [dict(
             name='M45',
             rlen=0.9,
             remanenc=1.1,
             relperm=1.04,
@@ -482,15 +482,15 @@
                 coil_span=1,
                 num_layers=2)
         )
         model = femagtools.MachineModel(machine)
         magnets = femagtools.magnet.Magnet(magnetmat)
         condMat = femagtools.magnet.Magnet([dict(name='Cu', elconduct=56e6)])
         fsl = self.builder.create_model(model, magnets, condMat)
-        self.assertEqual(len(fsl), 185)
+        self.assertEqual(len(fsl), 186)
         brem = [l.strip() for l in fsl
                 if l.split('=')[0].strip() == 'm.remanenc']
         self.assertEqual(brem[-1].split('=')[-1].strip(),
                          str(magnetmat[0]['remanenc']))
         rlen = [l.strip() for l in fsl
                 if l.split('=')[0].strip() == 'm.rlen']
         self.assertEqual(rlen[0].split('=')[-1].strip(),
```

### Comparing `femagtools-1.2.9/tests/test_im.py` & `femagtools-1.3.0/tests/test_im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_isa7.py` & `femagtools-1.3.0/tests/test_isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_jhb.py` & `femagtools-1.3.0/tests/test_jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_job.py` & `femagtools-1.3.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_losscoeffs.py` & `femagtools-1.3.0/tests/test_losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_machine.py` & `femagtools-1.3.0/tests/test_machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_magncurv.py` & `femagtools-1.3.0/tests/test_magncurv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_mcvreader.py` & `femagtools-1.3.0/tests/test_mcvreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_mcvwriter.py` & `femagtools-1.3.0/tests/test_mcvwriter.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         writeMcvFile = '{0}/{1}'.format(testPath, filename_out)
         writer.writeMcv(writeMcvFile)
         self.assertNotEqual(writer, None)
 
         # TEST
         reader2 = femagtools.mcv.Reader()
         reader2.readMcv(writeMcvFile)
-        
+
         for attr in ['version_mc_curve', 'mc1_curves', 'mc1_title']:
             self.assertAlmostEqual(getattr(reader, attr),
                                    getattr(reader2, attr))
         for attr in ['mc1_remz', 'mc1_bsat', 'mc1_bref', 'mc1_fillfac',
                      'fo', 'Bo', 'ch', 'ch_freq', 'cw',
                      'cw_freq', 'b_coeff', 'rho', 'fe_sat_mag']:
             self.assertAlmostEqual(getattr(reader, attr),
@@ -71,25 +71,26 @@
         writeMcvFile = '{0}/{1}'.format(testPath, filename_out)
         writer.writeMcv(writeMcvFile)
         self.assertNotEqual(writer, None)
 
         # TEST
         reader2 = femagtools.mcv.Reader()
         reader2.readMcv(writeMcvFile)
-        
+
         for attr in ['version_mc_curve', 'mc1_curves', 'mc1_title']:
             self.assertAlmostEqual(getattr(reader, attr),
                                    getattr(reader2, attr))
         for attr in ['mc1_remz', 'mc1_bsat', 'mc1_bref', 'mc1_fillfac',
                      'fo', 'Bo', 'ch', 'ch_freq', 'cw',
                      'cw_freq', 'b_coeff', 'rho', 'fe_sat_mag']:
             self.assertAlmostEqual(getattr(reader, attr),
                                    getattr(reader2, attr), 3)
         for attr in ['hi', 'bi']:
             self.assertAlmostEqual(reader.curve[0][attr],
                                    reader2.curve[0][attr], 3)
-        for attr in ['f', 'B']:
-            np.testing.assert_almost_equal(reader.losses[attr],
-                                           reader2.losses[attr], 5)
+        np.testing.assert_almost_equal(reader.losses['f'],
+                                       reader2.losses['f'], 5)
+        np.testing.assert_almost_equal(reader.losses['B'],
+                                       reader2.losses['B'], 5)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `femagtools-1.2.9/tests/test_model.py` & `femagtools-1.3.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_nc.py` & `femagtools-1.3.0/tests/test_nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_parident.py` & `femagtools-1.3.0/tests/test_parident.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_parstudy.py` & `femagtools-1.3.0/tests/test_parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_pocfile.py` & `femagtools-1.3.0/tests/test_pocfile.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_sizing.py` & `femagtools-1.3.0/tests/test_sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_sm.py` & `femagtools-1.3.0/tests/test_sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_tksreader.py` & `femagtools-1.3.0/tests/test_tksreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_ts.py` & `femagtools-1.3.0/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_vbfreader.py` & `femagtools-1.3.0/tests/test_vbfreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_vtu.py` & `femagtools-1.3.0/tests/test_vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.9/tests/test_windings.py` & `femagtools-1.3.0/tests/test_windings.py`

 * *Files identical despite different names*

