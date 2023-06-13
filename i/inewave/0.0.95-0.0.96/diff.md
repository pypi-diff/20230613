# Comparing `tmp/inewave-0.0.95.tar.gz` & `tmp/inewave-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inewave-0.0.95.tar", last modified: Tue Apr 25 14:39:48 2023, max compression
+gzip compressed data, was "inewave-0.0.96.tar", last modified: Tue Jun 13 20:15:29 2023, max compression
```

## Comparing `inewave-0.0.95.tar` & `inewave-0.0.96.tar`

### file list

```diff
@@ -1,652 +1,659 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.284622 inewave-0.0.95/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 14:36:08.000000 inewave-0.0.95/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-25 14:39:48.284622 inewave-0.0.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-25 14:36:08.000000 inewave-0.0.95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.136619 inewave-0.0.95/inewave/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.140619 inewave-0.0.95/inewave/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/_utils/leituracsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.148619 inewave-0.0.95/inewave/newave/
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/abertura.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    16024 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/bid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    73214 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/elnino.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/forwardh.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/gee.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/manutt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.160619 inewave-0.0.95/inewave/newave/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/abertura.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/arquivos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.160619 inewave-0.0.95/inewave/newave/modelos/arquivoscsv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/arquivoscsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/arquivoscsv/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/bid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.160619 inewave-0.0.95/inewave/newave/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)   133284 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/elnino.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/gee.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/perda.py
--rw-r--r--   0 runner    (1001) docker     (123)    24454 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/tecno.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modelos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    18834 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12901 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/perda.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/tecno.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/newave/vazpast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.160619 inewave-0.0.95/inewave/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/estados.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.160619 inewave-0.0.95/inewave/nwlistcf/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/modelos/estados.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/modelos/nwlistcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistcf/nwlistcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.172619 inewave-0.0.95/inewave/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/merclsin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/inewave/nwlistop/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivousina.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/inewave/nwlistop/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/parsubmercados.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/submercado.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/usina.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/valoresserie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/def.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dflppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dflpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/modelos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/nwlistop/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/inewave/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.140619 inewave-0.0.95/inewave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-25 14:39:48.000000 inewave-0.0.95/inewave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19993 2023-04-25 14:39:48.000000 inewave-0.0.95/inewave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:39:48.000000 inewave-0.0.95/inewave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-25 14:39:48.000000 inewave-0.0.95/inewave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 14:39:48.000000 inewave-0.0.95/inewave.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:39:48.284622 inewave-0.0.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-25 14:36:08.000000 inewave-0.0.95/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/tests/_arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/_arquivos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.184620 inewave-0.0.95/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.256621 inewave-0.0.95/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)    46951 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    30063 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)   847210 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)   295249 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)   295245 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105146 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)   295190 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)   295196 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   847164 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)   120243 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)   267099 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267152 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)   267153 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267144 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)   291239 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)   291240 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicaconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/estados.py
--rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)   267138 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104654 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104650 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105178 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105179 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105181 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   847144 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105136 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105139 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105141 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105140 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105189 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105190 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)    49768 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105188 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105191 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1087195 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    56692 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/nwlistcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)   378349 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)   267136 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   380918 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/term.py
--rw-r--r--   0 runner    (1001) docker     (123)   271157 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)   283139 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   283209 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)   847200 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267158 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267117 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105173 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105174 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105176 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   847195 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   847135 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/arquivos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.268622 inewave-0.0.95/tests/newave/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    48797 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_exph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_parp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/newave/test_vazpast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.268622 inewave-0.0.95/tests/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistcf/test_estados.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistcf/test_nwlistcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:39:48.284622 inewave-0.0.95/tests/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_coper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_evert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_exces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_geol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_invade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vento.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-25 14:36:08.000000 inewave-0.0.95/tests/nwlistop/test_vturuh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:29.026776 inewave-0.0.96/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 20:08:26.000000 inewave-0.0.96/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-13 20:15:29.026776 inewave-0.0.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-13 20:08:26.000000 inewave-0.0.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.702771 inewave-0.0.96/inewave/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.702771 inewave-0.0.96/inewave/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/_utils/leituracsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.722771 inewave-0.0.96/inewave/newave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75043 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42179 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/gee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/manutt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.790772 inewave-0.0.96/inewave/newave/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/arquivos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.790772 inewave-0.0.96/inewave/newave/modelos/arquivoscsv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/arquivoscsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/arquivoscsv/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/bid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.790772 inewave-0.0.96/inewave/newave/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/blocos/versaomodelo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30466 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135879 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87572 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/gee.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/perda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24454 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/perda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/vazpast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.790772 inewave-0.0.96/inewave/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/estados.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.790772 inewave-0.0.96/inewave/nwlistcf/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/modelos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/modelos/nwlistcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/nwlistcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.830773 inewave-0.0.96/inewave/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/merclsin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.854773 inewave-0.0.96/inewave/nwlistop/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.858773 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivousina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.858773 inewave-0.0.96/inewave/nwlistop/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/parsubmercados.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/submercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/usina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/valoresserie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dflppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dflpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.702771 inewave-0.0.96/inewave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-13 20:15:28.000000 inewave-0.0.96/inewave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20208 2023-06-13 20:15:28.000000 inewave-0.0.96/inewave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:15:28.000000 inewave-0.0.96/inewave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 20:15:28.000000 inewave-0.0.96/inewave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 20:15:28.000000 inewave-0.0.96/inewave.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:15:29.026776 inewave-0.0.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-13 20:08:26.000000 inewave-0.0.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.858773 inewave-0.0.96/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.858773 inewave-0.0.96/tests/_arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/_arquivos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.858773 inewave-0.0.96/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.982775 inewave-0.0.96/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46951 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30063 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847210 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295249 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295245 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105146 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295190 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295196 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847164 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120243 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267099 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267152 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267153 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267144 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291239 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291240 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicaconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267138 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104654 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104650 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105178 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105179 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105181 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847144 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105136 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105139 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105141 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105140 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105189 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105190 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49768 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105188 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105191 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1087195 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56692 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/nwlistcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)   378349 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267136 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   380918 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)   271157 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283139 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283209 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847200 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267158 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267117 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105173 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105174 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105176 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847195 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847135 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:29.002776 inewave-0.0.96/tests/newave/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49743 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_vazpast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:29.006775 inewave-0.0.96/tests/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistcf/test_estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistcf/test_nwlistcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:29.026776 inewave-0.0.96/tests/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vturuh.py
```

### Comparing `inewave-0.0.95/LICENSE.md` & `inewave-0.0.96/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/PKG-INFO` & `inewave-0.0.96/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 0.0.95
+Version: 0.0.96
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-0.0.95/README.md` & `inewave-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/_utils/leituracsv.py` & `inewave-0.0.96/inewave/_utils/leituracsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/config.py` & `inewave-0.0.96/inewave/config.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/__init__.py` & `inewave-0.0.96/inewave/newave/__init__.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/abertura.py` & `inewave-0.0.96/inewave/newave/abertura.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Abertura(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao número de
     aberturas utilizadas por período.
 
     """
@@ -17,11 +21,22 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="abertura.dat"
     ) -> "Abertura":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="abertura.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/newave/adterm.py` & `inewave-0.0.96/inewave/newave/adterm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from inewave.newave.modelos.adterm import BlocoUTEAdTerm
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import Type, TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class AdTerm(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às térmicas de
     despacho antecipado disponíveis.
 
     """
@@ -17,18 +21,29 @@
     SECTIONS = [BlocoUTEAdTerm]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="adterm.dat") -> "AdTerm":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="adterm.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/agrint.py` & `inewave-0.0.96/inewave/newave/agrint.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class AgrInt(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes aos agrupamentos
     livres de intercâmbio.
 
     """
@@ -15,11 +19,22 @@
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="agrint.dat") -> "AgrInt":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="agrint.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/newave/arquivos.py` & `inewave-0.0.96/inewave/newave/arquivos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from inewave.newave.modelos.arquivos import BlocoNomesArquivos
 
 from cfinterface.files.sectionfile import SectionFile
 
 from typing import List, TypeVar, Type, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Arquivos(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao arquivo
     `arquivos.dat`.
 
     Esta classe lida com informações de entrada do NEWAVE e
@@ -21,18 +25,29 @@
 
     SECTIONS = [BlocoNomesArquivos]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="arquivos.dat"
     ) -> "Arquivos":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arquivos.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/avl_cortesfpha_nwv.py` & `inewave-0.0.96/inewave/newave/nwv_avl_evap.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 from inewave.newave.modelos.blocos.versaomodelo import VersaoModelo
-from inewave.newave.modelos.avl_cortesfpha_nwv import TabelaAvlCortesFpha
+from inewave.newave.modelos.nwv_avl_evap import TabelaAvlEvap
 
 from inewave.newave.modelos.arquivoscsv.arquivocsv import ArquivoCSV
 from typing import Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class AvlCortesFpha(ArquivoCSV):
+
+class NwvAvlEvap(ArquivoCSV):
     """
-    Arquivo com os cortes da função de produção para as UHEs
-    do NEWAVE.
+    Arquivo com a avaliação da evaporação linear do NEWAVE.
     """
 
-    BLOCKS = [VersaoModelo, TabelaAvlCortesFpha]
+    BLOCKS = [VersaoModelo, TabelaAvlEvap]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, arquivo: str = "avl_cortesfpha_nwv.csv"
-    ) -> "AvlCortesFpha":
-        return cls.read(diretorio, arquivo)
+        cls, diretorio: str, arquivo: str = "nwv_avl_evap.csv"
+    ) -> "NwvAvlEvap":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, arquivo))
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
-        - indice_usina (`int`)
         - periodo (`int`)
+        - indice_usina (`int`)
         - nome_usina (`str`)
-        - indice_corte (`int`)
-        - fator_correcao (`float`)
-        - rhs_energia (`float`)
-        - coeficiente_volume_util_MW_hm3 (`float`)
-        - coeficiente_vazao_turbinada_MW_m3s (`float`)
-        - coeficiente_vazao_vertida_MW_m3s (`float`)
-        - coeficiente_vazao_lateral_MW_m3s (`float`)
+        - volume_armazenado_hm3 (`float`)
+        - evaporacao_calculada_hm3 (`float`)
+        - evaporacao_modelo_hm3 (`float`)
+        - desvio_absoluto_hm3 (`float`)
+        - desvio_percentual (`float`)
 
         :return: A tabela como um dataframe
         :rtype: pd.DataFrame | None
         """
         return self._tabela()
```

### Comparing `inewave-0.0.95/inewave/newave/avl_desvfpha_s.py` & `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,40 @@
-from inewave.newave.modelos.blocos.versaomodelo import VersaoModelo
-from inewave.newave.modelos.avl_desvfpha_s import TabelaAvlDesvFphaS
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.blocos.valoresserie import (
+    ValoresSerie,
+)
 
 from cfinterface.files.blockfile import BlockFile
-from typing import Optional, TypeVar, Type
 import pandas as pd  # type: ignore
+from typing import Type, TypeVar, Optional
 
 
-class AvlDesvFphaS(BlockFile):
+class ArquivoSubmercado(BlockFile):
     """
-    Arquivo com os desvios da função de produção no plano de
-    vazão vertida (S).
+    Armazena os dados das saídas por submercado.
     """
 
-    BLOCKS = [VersaoModelo, TabelaAvlDesvFphaS]
-    ENCODING = "iso-8859-1"
-
     T = TypeVar("T")
 
+    BLOCKS = [Submercado, ValoresSerie]
+
     def __init__(self, data=...) -> None:
         super().__init__(data)
-        self.__df_completo: Optional[pd.DataFrame] = None
+        self.__valores = None
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, arquivo: str = "avl_desvfpha_s_001.dat"
-    ) -> "AvlDesvFphaS":
-        return cls.read(diretorio, arquivo)
-
-    @property
-    def tabela(self) -> Optional[pd.DataFrame]:
-        """
-        A tabela de dados que está contida no arquivo.
-
-        - indice_usina (`int`)
-        - nome_usina (`str`)
-        - volume_armazenado_percentual (`float`)
-        - vazao_turbinada_m3s (`float`)
-        - vazao_vertida_m3s (`float`)
-        - desvio_percentual (`float`)
+        cls, diretorio: str, nome_arquivo="arq.out"
+    ) -> "ArquivoSubmercado":
+        return cls.read(diretorio, nome_arquivo)
 
-        :return: A tabela como um dataframe
-        :rtype: pd.DataFrame | None
-        """
-        if self.__df_completo is None:
-            tabelas = self.data.of_type(TabelaAvlDesvFphaS)
-            self.__df_completo = pd.DataFrame()
-            for t in tabelas:
-                self.__df_completo = pd.concat(
-                    [self.__df_completo, t.data], ignore_index=True
-                )
-        return self.__df_completo
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
+        self.write(diretorio, nome_arquivo)
 
-    def _bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
+    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
         :param indice: O índice do bloco a ser acessado, dentre os do tipo
         :type indice: int
@@ -67,19 +46,51 @@
                 b
                 for i, b in enumerate(self.data.of_type(bloco))
                 if i == indice
             )
         except StopIteration:
             return None
 
+    def __monta_tabela(self) -> pd.DataFrame:
+        df = None
+        for b in self.data.of_type(ValoresSerie):
+            dados = b.data
+            if dados is None:
+                continue
+            elif df is None:
+                df = b.data
+            else:
+                df = pd.concat([df, b.data], ignore_index=True)
+        return df
+
+    @property
+    def valores(self) -> Optional[pd.DataFrame]:
+        """
+        Tabela com os valores, por série e
+        por mês/ano de estudo.
+
+        - Ano (`int`)
+        - Série (`int`)
+        - Patamar (`str`)
+        - Janeiro (`float`)
+        - ...
+        - Dezembro (`float`)
+
+        :return: A tabela dos valores.
+        :rtype: pd.DataFrame | None
+        """
+        if self.__valores is None:
+            self.__valores = self.__monta_tabela()
+        return self.__valores
+
     @property
-    def versao(self) -> Optional[str]:
+    def submercado(self) -> Optional[str]:
         """
-        A versão do modelo utilizada para executar o caso.
+        O submercado associado ao arquivo lido.
 
-        :return: A versão do modelo
-        :rtype: str | None
+        :return: Os nome do submercado
+        :rtype: str
         """
-        b = self._bloco_por_tipo(VersaoModelo, 0)
+        b = self.__bloco_por_tipo(Submercado, 0)
         if b is not None:
             return b.data
         return None
```

### Comparing `inewave-0.0.95/inewave/newave/avl_desvfpha_v_q.py` & `inewave-0.0.96/inewave/newave/avl_desvfpha_v_q.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from inewave.newave.modelos.blocos.versaomodelo import VersaoModelo
 from inewave.newave.modelos.avl_desvfpha_v_q import TabelaAvlDesvFphaVQ
 
 from cfinterface.files.blockfile import BlockFile
 from typing import Optional, TypeVar, Type
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class AvlDesvFphaVQ(BlockFile):
     """
     Arquivo com os desvios da função de produção nos planos de
     volume armazenado e vazão turbinada (V-Q).
     """
 
@@ -21,15 +25,20 @@
         super().__init__(data)
         self.__df_completo: Optional[pd.DataFrame] = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, arquivo: str = "avl_desvfpha_v_q_001.dat"
     ) -> "AvlDesvFphaVQ":
-        return cls.read(diretorio, arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, arquivo))
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
         - indice_usina (`int`)
```

### Comparing `inewave-0.0.95/inewave/newave/cadic.py` & `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivousina.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-from inewave.newave.modelos.cadic import BlocoCargasAdicionais
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.blocos.valoresserie import (
+    ValoresSerie,
+)
 
-from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
+from typing import Type, TypeVar, Optional
 
 
-class CAdic(SectionFile):
+class ArquivoUsina(BlockFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às cargas
-    adicionais.
-
+    Armazena os dados das saídas por usina.
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoCargasAdicionais]
+    BLOCKS = [Usina, ValoresSerie]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
+        self.__valores = None
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="c_adic.dat") -> "CAdic":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="arq.out"
+    ) -> "ArquivoUsina":
         return cls.read(diretorio, nome_arquivo)
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="c_adic.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
@@ -42,37 +46,51 @@
                 b
                 for i, b in enumerate(self.data.of_type(bloco))
                 if i == indice
             )
         except StopIteration:
             return None
 
+    def __monta_tabela(self) -> pd.DataFrame:
+        df = None
+        for b in self.data.of_type(ValoresSerie):
+            dados = b.data
+            if dados is None:
+                continue
+            elif df is None:
+                df = b.data
+            else:
+                df = pd.concat([df, b.data], ignore_index=True)
+        return df
+
     @property
-    def cargas(self) -> Optional[pd.DataFrame]:
+    def valores(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com as cargas adicionais por mês/ano e por subsistema
-        para cada razão de carga adicional. As colunas são:
+        Tabela com os valores, por série e
+        por mês/ano de estudo.
 
-        - Código Subsistema (`int`)
-        - Nome Subsistema (`str`)
-        - Razão (`str`)
-        - Ano (`str`)
+        - Ano (`int`)
+        - Série (`int`)
+        - Patamar (`str`)
         - Janeiro (`float`)
-        - Fevereiro (`float`)
         - ...
         - Dezembro (`float`)
 
-        :return: A tabela como um DataFrame
+        :return: A tabela dos valores.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoCargasAdicionais, 0)
+        if self.__valores is None:
+            self.__valores = self.__monta_tabela()
+        return self.__valores
+
+    @property
+    def usina(self) -> Optional[str]:
+        """
+        A usina associada ao arquivo lido.
+
+        :return: O nome da usina
+        :rtype: str
+        """
+        b = self.__bloco_por_tipo(Usina, 0)
         if b is not None:
             return b.data
         return None
-
-    @cargas.setter
-    def cargas(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoCargasAdicionais, 0)
-        if b is not None:
-            b.data = valor
-        else:
-            raise ValueError("Campo não lido")
```

### Comparing `inewave-0.0.95/inewave/newave/caso.py` & `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-from inewave.newave.modelos.caso import NomeCaso, CaminhoGerenciadorProcessos
+from inewave.nwlistop.modelos.blocos.parsubmercados import ParSubmercados
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
+)
 
-from cfinterface.files.sectionfile import SectionFile
+from cfinterface.files.blockfile import BlockFile
+import pandas as pd  # type: ignore
 from typing import Type, TypeVar, Optional
 
 
-class Caso(SectionFile):
+class ArquivoParSubmercadoPatamar(BlockFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às
-    configurações das usinas hidrelétricas.
-
-    Esta classe lida com informações de entrada fornecidas ao NEWAVE e
-    que podem ser modificadas através do arquivo `modif.dat`.
-
+    Armazena os dados das saídas por patamar, por par de submercados.
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [NomeCaso, CaminhoGerenciadorProcessos]
+    BLOCKS = [ParSubmercados, ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
+        self.__valores = None
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="caso.dat") -> "Caso":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="arq.out"
+    ) -> "ArquivoParSubmercadoPatamar":
         return cls.read(diretorio, nome_arquivo)
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="caso.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
@@ -44,44 +46,64 @@
                 b
                 for i, b in enumerate(self.data.of_type(bloco))
                 if i == indice
             )
         except StopIteration:
             return None
 
+    def __monta_tabela(self) -> pd.DataFrame:
+        df = None
+        for b in self.data.of_type(ValoresSeriePatamar):
+            dados = b.data
+            if dados is None:
+                continue
+            elif df is None:
+                df = b.data
+            else:
+                df = pd.concat([df, b.data], ignore_index=True)
+        return df
+
     @property
-    def arquivos(self) -> Optional[str]:
+    def valores(self) -> Optional[pd.DataFrame]:
         """
-        Caminho para o arquivo `arquivos.dat` de entrada do NEWAVE.
+        Tabela com os valores por patamar, por série e
+        por mês/ano de estudo.
 
-        :return: O caminho para o arquivo
-        :rtype: str | None
+        - Ano (`int`)
+        - Série (`int`)
+        - Patamar (`str`)
+        - Janeiro (`float`)
+        - ...
+        - Dezembro (`float`)
+
+        :return: A tabela dos valores por patamar.
+        :rtype: pd.DataFrame | None
+        """
+        if self.__valores is None:
+            self.__valores = self.__monta_tabela()
+        return self.__valores
+
+    @property
+    def submercado_de(self) -> Optional[str]:
         """
-        b = self.__bloco_por_tipo(NomeCaso, 0)
-        if b is not None:
-            return b.data
-        return None
+        O submercado de origem associado ao arquivo lido.
 
-    @arquivos.setter
-    def arquivos(self, a: str):
-        b = self.__bloco_por_tipo(NomeCaso, 0)
+        :return: Os nome do submercado
+        :rtype: str
+        """
+        b = self.__bloco_por_tipo(ParSubmercados, 0)
         if b is not None:
-            b.data = a
+            return b.data[0]
+        return None
 
     @property
-    def gerenciador_processos(self) -> Optional[str]:
+    def submercado_para(self) -> Optional[str]:
         """
-        Caminho para o gerenciador de processos do NEWAVE.
+        O submercado de destino associado ao arquivo lido.
 
-        :return: O caminho para o arquivo
-        :rtype: str | None
+        :return: Os nome do submercado
+        :rtype: str
         """
-        b = self.__bloco_por_tipo(CaminhoGerenciadorProcessos, 0)
+        b = self.__bloco_por_tipo(ParSubmercados, 0)
         if b is not None:
-            return b.data
+            return b.data[1]
         return None
-
-    @gerenciador_processos.setter
-    def gerenciador_processos(self, a: str):
-        b = self.__bloco_por_tipo(CaminhoGerenciadorProcessos, 0)
-        if b is not None:
-            b.data = a
```

### Comparing `inewave-0.0.95/inewave/newave/clast.py` & `inewave-0.0.96/inewave/newave/clast.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,18 @@
     BlocoModificacaoUTEClasT,
 )
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import Type, TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class ClasT(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às classes de
     usinas térmicas.
 
     """
@@ -20,18 +24,29 @@
     SECTIONS = [BlocoUTEClasT, BlocoModificacaoUTEClasT]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="clast.dat") -> "ClasT":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="clast.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/confhd.py` & `inewave-0.0.96/inewave/newave/confhd.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from inewave.newave.modelos.confhd import BlocoConfUHE
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import Type, TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Confhd(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às
     configurações das usinas hidrelétricas.
 
     Esta classe lida com informações de entrada fornecidas ao NEWAVE e
@@ -20,18 +24,29 @@
     SECTIONS = [BlocoConfUHE]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="confhd.dat") -> "Confhd":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="confhd.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/conft.py` & `inewave-0.0.96/inewave/newave/conft.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from inewave.newave.modelos.conft import BlocoConfUTE
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import Type, TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class ConfT(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às configurações das
     usinas térmicas.
     """
 
@@ -16,18 +20,29 @@
     SECTIONS = [BlocoConfUTE]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="conft.dat") -> "ConfT":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="conft.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/curva.py` & `inewave-0.0.96/inewave/newave/curva.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     BlocoImpressaoRelatorioProcessoIterativoEtapa2,
 )
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import Type, TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Curva(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes à curva para
     penalização por volume mínimo dos reservatórios.
     """
 
@@ -32,18 +36,29 @@
     ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="curva.dat") -> "Curva":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="curva.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/cvar.py` & `inewave-0.0.96/inewave/newave/cvar.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,18 @@
     BlocoLambdaVariavelNoTempo,
 )
 
 from cfinterface.files.blockfile import BlockFile
 from typing import Type, TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class CVAR(BlockFile):
     """
     Armazena os dados de entrada do NEWAVE referentes à curva para
     penalização por volume mínimo dos reservatórios.
     """
 
@@ -24,18 +28,29 @@
     ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="cvar.dat") -> "CVAR":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="cvar.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/dger.py` & `inewave-0.0.96/inewave/newave/dger.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,20 @@
 from inewave.newave.modelos.dger import BlocoRestricaoLPPTurbinamentoMaximoREE
 from inewave.newave.modelos.dger import BlocoRestricaoLPPDefluenciaMaximaREE
 from inewave.newave.modelos.dger import BlocoRestricaoLPPTurbinamentoMaximoUHE
 from inewave.newave.modelos.dger import BlocoRestricaoLPPDefluenciaMaximaUHE
 from inewave.newave.modelos.dger import BlocoRestricoesEletricasEspeciais
 from inewave.newave.modelos.dger import BlocoFuncaoProducaoUHE
 from inewave.newave.modelos.dger import BlocoFCFPosEstudo
+from inewave.newave.modelos.dger import BlocoEstacoesBombeamento
+from inewave.newave.modelos.dger import BlocoCanalDesvio
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
 class DGer(SectionFile):
     """
     Classe para armazenar dados gerais de uma execução do NEWAVE.
 
     """
@@ -208,25 +214,38 @@
         BlocoRestricaoLPPTurbinamentoMaximoREE,
         BlocoRestricaoLPPDefluenciaMaximaREE,
         BlocoRestricaoLPPTurbinamentoMaximoUHE,
         BlocoRestricaoLPPDefluenciaMaximaUHE,
         BlocoRestricoesEletricasEspeciais,
         BlocoFuncaoProducaoUHE,
         BlocoFCFPosEstudo,
+        BlocoEstacoesBombeamento,
+        BlocoCanalDesvio,
     ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="dger.dat") -> "DGer":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="dger.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
@@ -2371,7 +2390,45 @@
         return None
 
     @fcf_pos_estudo.setter
     def fcf_pos_estudo(self, dado: int):
         b = self.__bloco_por_tipo(BlocoFCFPosEstudo, 0)
         if b is not None:
             b.valor = dado
+
+    @property
+    def estacoes_bombeamento(self) -> Optional[int]:
+        """
+        Configuração da linha número 101 do arquivo `dger.dat`.
+
+        :return: O valor do campo
+        :rtype: int | None
+        """
+        b = self.__bloco_por_tipo(BlocoEstacoesBombeamento, 0)
+        if b is not None:
+            return b.valor
+        return None
+
+    @estacoes_bombeamento.setter
+    def estacoes_bombeamento(self, dado: int):
+        b = self.__bloco_por_tipo(BlocoEstacoesBombeamento, 0)
+        if b is not None:
+            b.valor = dado
+
+    @property
+    def canal_desvio(self) -> Optional[int]:
+        """
+        Configuração da linha número 102 do arquivo `dger.dat`.
+
+        :return: O valor do campo
+        :rtype: int | None
+        """
+        b = self.__bloco_por_tipo(BlocoCanalDesvio, 0)
+        if b is not None:
+            return b.valor
+        return None
+
+    @canal_desvio.setter
+    def canal_desvio(self, dado: int):
+        b = self.__bloco_por_tipo(BlocoCanalDesvio, 0)
+        if b is not None:
+            b.valor = dado
```

### Comparing `inewave-0.0.95/inewave/newave/dsvagua.py` & `inewave-0.0.96/inewave/newave/vazpast.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,54 @@
-from inewave.newave.modelos.dsvagua import BlocoDsvUHE
+from inewave.newave.modelos.vazpast import BlocoVazPast
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import Type, TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class DSVAgua(SectionFile):
+
+class VazPast(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes aos
-    desvios de água por usina.
+    Armazena os dados de entrada do NEWAVE referentes às
+    vazões anteriores ao período de planejamento.
 
     Esta classe lida com informações de entrada fornecidas ao NEWAVE e
-    que podem ser modificadas através do arquivo `dsvagua.dat`.
+    que são usadas juntos das contidas no arquivo `vazoes.dat`.
 
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoDsvUHE]
+    SECTIONS = [BlocoVazPast]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dsvagua.dat"
-    ) -> "DSVAgua":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="dsvagua.dat"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="vazpast.dat"
+    ) -> "VazPast":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
+
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="vazpast.dat"):
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
@@ -48,34 +63,30 @@
                 for i, b in enumerate(self.data.of_type(bloco))
                 if i == indice
             )
         except StopIteration:
             return None
 
     @property
-    def desvios(self) -> Optional[pd.DataFrame]:
+    def tendencia(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com os desvios de água por usina e por estágio.
+        Tabela com a tendência hidrológica por REE.
 
-        - Ano (`int`)
-        - Usina (`int`)
+        - Índice (`int`)
+        - Usina (`str`)
         - Janeiro (`float`)
-        - Fevereiro (`float`)
         - ...
         - Dezembro (`float`)
-        - Flag (`int`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoDsvUHE, 0)
+        b = self.__bloco_por_tipo(BlocoVazPast, 0)
         if b is not None:
             return b.data
         return None
 
-    @desvios.setter
-    def desvios(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoDsvUHE, 0)
+    @tendencia.setter
+    def tendencia(self, df: pd.DataFrame):
+        b = self.__bloco_por_tipo(BlocoVazPast, 0)
         if b is not None:
-            b.data = valor
-        else:
-            raise ValueError("Campo não lido")
+            b.data = df
```

### Comparing `inewave-0.0.95/inewave/newave/eafpast.py` & `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from inewave.newave.modelos.eafpast import BlocoEafPast
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
+)
 
-from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
+from typing import Type, TypeVar, Optional
 
 
-class EafPast(SectionFile):
+class ArquivoUsinaPatamar(BlockFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às
-    vazões anteriores ao período de planejamento por REE.
-
-    Esta classe lida com informações de entrada fornecidas ao NEWAVE e
-    que são usadas junto das contidas no arquivo `vazoes.dat`.
-
+    Armazena os dados das saídas por patamar, por Usina.
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoEafPast]
+    BLOCKS = [Usina, ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
+        self.__valores = None
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="eafpast.dat"
-    ) -> "EafPast":
+        cls, diretorio: str, nome_arquivo="arq.out"
+    ) -> "ArquivoUsinaPatamar":
         return cls.read(diretorio, nome_arquivo)
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="eafpast.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
@@ -47,32 +46,51 @@
                 b
                 for i, b in enumerate(self.data.of_type(bloco))
                 if i == indice
             )
         except StopIteration:
             return None
 
+    def __monta_tabela(self) -> pd.DataFrame:
+        df = None
+        for b in self.data.of_type(ValoresSeriePatamar):
+            dados = b.data
+            if dados is None:
+                continue
+            elif df is None:
+                df = b.data
+            else:
+                df = pd.concat([df, b.data], ignore_index=True)
+        return df
+
     @property
-    def tendencia(self) -> Optional[pd.DataFrame]:
+    def valores(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com a tendência hidrológica por REE.
+        Tabela com os valores por patamar, por série e
+        por mês/ano de estudo.
 
-        - Índice (`int`)
-        - REE (`str`)
+        - Ano (`int`)
+        - Série (`int`)
+        - Patamar (`str`)
         - Janeiro (`float`)
-        - Fevereiro (`float`)
         - ...
         - Dezembro (`float`)
 
-        :return: A tabela como um DataFrame
-        :rtype: Optional[pd.DataFrame]
+        :return: A tabela dos valores por patamar.
+        :rtype: pd.DataFrame | None
+        """
+        if self.__valores is None:
+            self.__valores = self.__monta_tabela()
+        return self.__valores
+
+    @property
+    def usina(self) -> Optional[str]:
+        """
+        A usina associada ao arquivo lido.
+
+        :return: O nome da usina
+        :rtype: str
         """
-        b = self.__bloco_por_tipo(BlocoEafPast, 0)
+        b = self.__bloco_por_tipo(Usina, 0)
         if b is not None:
             return b.data
         return None
-
-    @tendencia.setter
-    def tendencia(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoEafPast, 0)
-        if b is not None:
-            b.data = df
```

### Comparing `inewave-0.0.95/inewave/newave/enavazb.py` & `inewave-0.0.96/inewave/newave/enavazb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from cfinterface.files.sectionfile import SectionFile
 from inewave.newave.modelos.enavazb import SecaoDadosEnavazb
 import pandas as pd  # type: ignore
 
 from typing import TypeVar, Optional
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Enavazb(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às séries sintéticas
     de energia para a etapa backward geradas pelo modelo, formadas
     pela agregação das séries de vazão incrementais das UHEs.
     """
@@ -26,26 +30,27 @@
         diretorio: str,
         nome_arquivo="enavazb.dat",
         numero_forwards: int = 200,
         numero_aberturas: int = 20,
         numero_rees: int = 12,
         numero_estagios: int = 60,
     ) -> "Enavazb":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
         return cls.read(
-            diretorio,
-            nome_arquivo,
+            join(diretorio, nome_arquivo),
+            numero_rees=numero_rees,
             numero_forwards=numero_forwards,
             numero_aberturas=numero_aberturas,
-            numero_rees=numero_rees,
             numero_estagios=numero_estagios,
         )
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="enavazb.dat"):
-        self.write(diretorio, nome_arquivo)
-
     @property
     def series(self) -> Optional[pd.DataFrame]:
         """
         Obtém a tabela com os dados das séries de energia
         afluente por REE, por estágio, série forward e abertura.
 
         - estagio (`int`): estágio do cenário gerado
```

### Comparing `inewave-0.0.95/inewave/newave/enavazf.py` & `inewave-0.0.96/inewave/newave/vazaos.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 from cfinterface.files.sectionfile import SectionFile
-from inewave.newave.modelos.enavazf import SecaoDadosEnavazf
+from inewave.newave.modelos.vazaos import SecaoDadosVazaos
 import pandas as pd  # type: ignore
 
 from typing import TypeVar, Optional
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Enavazf(SectionFile):
+
+class Vazaos(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às séries sintéticas
-    de energia para a etapa forward geradas pelo modelo, formadas
-    pela agregação das séries de vazão incrementais das UHEs.
+    de vazão para a simulação final geradas pelo modelo.
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [SecaoDadosEnavazf]
+    SECTIONS = [SecaoDadosVazaos]
     STORAGE = "BINARY"
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls,
         diretorio: str,
-        nome_arquivo="enavazf.dat",
-        numero_forwards: int = 200,
-        numero_rees: int = 12,
+        nome_arquivo="vazaos.dat",
+        numero_series: int = 2000,
+        numero_uhes: int = 164,
         numero_estagios: int = 60,
         numero_estagios_th: int = 12,
-    ) -> "Enavazf":
+    ) -> "Vazaos":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
         return cls.read(
-            diretorio,
-            nome_arquivo,
-            numero_forwards=numero_forwards,
-            numero_rees=numero_rees,
+            join(diretorio, nome_arquivo),
+            numero_series=numero_series,
+            numero_uhes=numero_uhes,
             numero_estagios=numero_estagios,
             numero_estagios_th=numero_estagios_th,
         )
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="enavazf.dat"):
-        self.write(diretorio, nome_arquivo)
-
     @property
     def series(self) -> Optional[pd.DataFrame]:
         """
-        Obtém a tabela com os dados das séries de energia
-        afluente por REE e por estágio.
+        Obtém a tabela com os dados das séries de vazão
+        afluente por UHE e por estágio.
 
         - estagio (`int`): estágio do cenário gerado
-        - ree (`int`): REE para o qual foi gerado
-        - serie (`int`): índice da série forward
-        - valor (`float`): energia em MWmes
+        - uhe (`int`): UHE para a qual foi gerado
+        - serie (`int`): índice da série sintética
+        - valor (`float`): vazão em hm3
 
         :return: A tabela com os dados das séries
         :rtype: pd.DataFrame | None
         """
-        sections = [r for r in self.data.of_type(SecaoDadosEnavazf)]
+        sections = [r for r in self.data.of_type(SecaoDadosVazaos)]
         if len(sections) > 0:
             return sections[0].data
         else:
             return None
 
     @series.setter
     def series(self, df: pd.DataFrame):
-        sections = [r for r in self.data.of_type(SecaoDadosEnavazf)]
+        sections = [r for r in self.data.of_type(SecaoDadosVazaos)]
         if len(sections) > 0:
             sections[0].data = df
```

### Comparing `inewave-0.0.95/inewave/newave/energiab.py` & `inewave-0.0.96/inewave/newave/energiab.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from cfinterface.files.sectionfile import SectionFile
 from inewave.newave.modelos.energiab import SecaoDadosEnergiab
 import pandas as pd  # type: ignore
 
 from typing import TypeVar, Optional
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Energiab(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às séries sintéticas
     de energia para a etapa backward geradas pelo modelo.
     """
 
@@ -25,26 +29,27 @@
         diretorio: str,
         nome_arquivo="energiab.dat",
         numero_forwards: int = 200,
         numero_aberturas: int = 20,
         numero_rees: int = 12,
         numero_estagios: int = 60,
     ) -> "Energiab":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
         return cls.read(
-            diretorio,
-            nome_arquivo,
+            join(diretorio, nome_arquivo),
+            numero_rees=numero_rees,
             numero_forwards=numero_forwards,
             numero_aberturas=numero_aberturas,
-            numero_rees=numero_rees,
             numero_estagios=numero_estagios,
         )
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="energiab.dat"):
-        self.write(diretorio, nome_arquivo)
-
     @property
     def series(self) -> Optional[pd.DataFrame]:
         """
         Obtém a tabela com os dados das séries de energia
         afluente por REE, por estágio, série forward e abertura.
 
         - estagio (`int`): estágio do cenário gerado
```

### Comparing `inewave-0.0.95/inewave/newave/energiaf.py` & `inewave-0.0.96/inewave/newave/energiaf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from cfinterface.files.sectionfile import SectionFile
 from inewave.newave.modelos.energiaf import SecaoDadosEnergiaf
 import pandas as pd  # type: ignore
 
 from typing import TypeVar, Optional
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Energiaf(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às séries sintéticas
     de energia para a etapa forward geradas pelo modelo.
     """
 
@@ -25,26 +29,27 @@
         diretorio: str,
         nome_arquivo="energiaf.dat",
         numero_forwards: int = 200,
         numero_rees: int = 12,
         numero_estagios: int = 60,
         numero_estagios_th: int = 12,
     ) -> "Energiaf":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
         return cls.read(
-            diretorio,
-            nome_arquivo,
-            numero_forwards=numero_forwards,
+            join(diretorio, nome_arquivo),
             numero_rees=numero_rees,
+            numero_forwards=numero_forwards,
             numero_estagios=numero_estagios,
             numero_estagios_th=numero_estagios_th,
         )
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="energiaf.dat"):
-        self.write(diretorio, nome_arquivo)
-
     @property
     def series(self) -> Optional[pd.DataFrame]:
         """
         Obtém a tabela com os dados das séries de energia
         afluente por REE e por estágio.
 
         - estagio (`int`): estágio do cenário gerado
```

### Comparing `inewave-0.0.95/inewave/newave/energias.py` & `inewave-0.0.96/inewave/newave/energias.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from cfinterface.files.sectionfile import SectionFile
 from inewave.newave.modelos.energias import SecaoDadosEnergias
 import pandas as pd  # type: ignore
 
 from typing import TypeVar, Optional
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Energias(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às séries sintéticas
     de energia para a simulação final geradas pelo modelo.
     """
 
@@ -25,26 +29,27 @@
         diretorio: str,
         nome_arquivo="energias.dat",
         numero_series: int = 2000,
         numero_rees: int = 12,
         numero_estagios: int = 60,
         numero_estagios_th: int = 12,
     ) -> "Energias":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
         return cls.read(
-            diretorio,
-            nome_arquivo,
-            numero_series=numero_series,
+            join(diretorio, nome_arquivo),
             numero_rees=numero_rees,
+            numero_series=numero_series,
             numero_estagios=numero_estagios,
             numero_estagios_th=numero_estagios_th,
         )
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="energias.dat"):
-        self.write(diretorio, nome_arquivo)
-
     @property
     def series(self) -> Optional[pd.DataFrame]:
         """
         Obtém a tabela com os dados das séries de energia
         afluente por REE e por estágio, para a simulação final.
 
         - estagio (`int`): estágio do cenário gerado
```

### Comparing `inewave-0.0.95/inewave/newave/engnat.py` & `inewave-0.0.96/inewave/newave/engnat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from cfinterface.files.sectionfile import SectionFile
 from inewave.newave.modelos.engnat import SecaoDadosEngnat
 import pandas as pd  # type: ignore
 
 from typing import TypeVar, Optional
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Engnat(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às séries históricas
     de energia por configuração, calculadas a partir das séries históricas
     de vazão.
     """
@@ -25,25 +29,26 @@
         cls,
         diretorio: str,
         nome_arquivo="engnat.dat",
         numero_rees: int = 12,
         numero_configuracoes: int = 60,
         ano_inicio_historico: int = 1931,
     ) -> "Engnat":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
         return cls.read(
-            diretorio,
-            nome_arquivo,
+            join(diretorio, nome_arquivo),
             numero_rees=numero_rees,
             numero_configuracoes=numero_configuracoes,
             ano_inicio_historico=ano_inicio_historico,
         )
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="engnat.dat"):
-        self.write(diretorio, nome_arquivo)
-
     @property
     def series(self) -> Optional[pd.DataFrame]:
         """
         Obtém a tabela com os dados das séries de energia
         afluente por REE e por estágio.
 
         - configuracao (`int`): configuração da série histórica
```

### Comparing `inewave-0.0.95/inewave/newave/eolicacadastro.py` & `inewave-0.0.96/inewave/newave/eolicacadastro.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     RegistroEolicaCadastroAerogerador,
     RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo,
     RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva,
     RegistroPEECadastro,
     RegistroPEEPotenciaInstaladaPeriodo,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class EolicaCadastro(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao cadastro
     das usinas eólicas do sistema.
     """
 
@@ -35,20 +39,31 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="eolica-cadastro.csv"
     ) -> "EolicaCadastro":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(
         self, diretorio: str, nome_arquivo="eolica-cadastro.csv"
     ):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
```

### Comparing `inewave-0.0.95/inewave/newave/eolicaconfiguracao.py` & `inewave-0.0.96/inewave/newave/eolicaconfiguracao.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.eolicaconfiguracao import (
     RegistroEolicaConfiguracao,
     RegistroPEEConfiguracaoPeriodo,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class EolicaConfiguracao(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às configurações
     das usinas eólicas.
     """
 
@@ -22,20 +26,31 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="eolica-config.csv"
     ) -> "EolicaConfiguracao":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(
         self, diretorio: str, nome_arquivo="eolica-config.csv"
     ):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
```

### Comparing `inewave-0.0.95/inewave/newave/eolicafte.py` & `inewave-0.0.96/inewave/newave/eolicafte.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import Type, TypeVar, List, Optional, Union
 from datetime import datetime
 
 from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.eolicafte import RegistroEolicaFTE, RegistroPEEFTE
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class EolicaFTE(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às funções de
     transferência vento-potência.
     """
 
@@ -19,18 +23,29 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="eolica-fte.csv"
     ) -> "EolicaFTE":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="eolica-fte.csv"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
```

### Comparing `inewave-0.0.95/inewave/newave/eolicageracao.py` & `inewave-0.0.96/inewave/newave/eolicageracao.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.eolicageracao import (
     RegistroEolicaGeracaoPeriodo,
     RegistroEolicaGeracaoPatamar,
     RegistroPEEGeracaoPatamar,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class EolicaGeracao(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao histórico
     de geração das usinas eólicas.
     """
 
@@ -27,20 +31,31 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="eolica-geracao.csv"
     ) -> "EolicaGeracao":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(
         self, diretorio: str, nome_arquivo="eolica-geracao.csv"
     ):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
```

### Comparing `inewave-0.0.95/inewave/newave/eolicahistorico.py` & `inewave-0.0.96/inewave/newave/eolicahistorico.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from inewave.newave.modelos.eolicahistorico import (
     RegistroEolicaHistoricoVentoHorizonte,
     RegistroEolicaHistoricoVento,
     RegistroHistoricoVentoHorizonte,
     RegistroHistoricoVento,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class EolicaHistorico(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao histórico
     de ventos das usinas eólicas.
     """
 
@@ -29,18 +33,29 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="hist-ventos.csv"
     ) -> "EolicaHistorico":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="hist-ventos.csv"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
```

### Comparing `inewave-0.0.95/inewave/newave/eolicaposto.py` & `inewave-0.0.96/inewave/newave/eolicaposto.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.eolicaposto import (
     RegistroPEEPostoVento,
     RegistroPostoVentoCadastro,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class EolicaPosto(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes aos postos
     de vento e sua associação com os PEE.
     """
 
@@ -25,18 +29,29 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="eolica-posto.csv"
     ) -> "EolicaPosto":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="eolica-posto.csv"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
```

### Comparing `inewave-0.0.95/inewave/newave/eolicasubmercado.py` & `inewave-0.0.96/inewave/newave/eolicasubmercado.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.eolicasubmercado import (
     RegistroEolicaSubmercado,
     RegistroPEESubmercado,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class EolicaSubmercado(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao mapeamento
     de usinas eólicas e submercados.
     """
 
@@ -21,20 +25,31 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="eolica-submercado.csv"
     ) -> "EolicaSubmercado":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(
         self, diretorio: str, nome_arquivo="eolica-submercado.csv"
     ):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
```

### Comparing `inewave-0.0.95/inewave/newave/exph.py` & `inewave-0.0.96/inewave/newave/exph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 from inewave.newave.modelos.exph import BlocoUHEExph
 
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Exph(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes à expansão
     hidraulica do sistema.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = [BlocoUHEExph]
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="exph.dat") -> "Exph":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="exph.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/expt.py` & `inewave-0.0.96/inewave/newave/ensoaux.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Expt(SectionFile):
+
+class ENSOAux(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes à expansão
-    térmica do sistema.
+    Armazena os dados de entrada do NEWAVE referentes ao arquivo ENSO 2.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="expt.dat") -> "Expt":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="expt.dat"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="ensoaux.dat"
+    ) -> "ENSOAux":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
+
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="ensoaux.dat"):
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/newave/ghmin.py` & `inewave-0.0.96/inewave/newave/ghmin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class GHMin(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes à geração hidráulica
     mínima por usina.
 
     """
@@ -15,11 +19,22 @@
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="ghmin.dat") -> "GHMin":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="ghmin.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/newave/gtminpat.py` & `inewave-0.0.96/inewave/newave/tecno.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class GTMinPat(SectionFile):
+
+class Tecno(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes à geração térmica
-    mínima por patamar.
+    Armazena os dados de entrada do NEWAVE referentes às tecnologias
+    disponíveis para geração de energia.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="gtminpat.dat"
-    ) -> "GTMinPat":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="gtminpat.dat"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(cls, diretorio: str, nome_arquivo="tecno.dat") -> "Tecno":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
+
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="tecno.dat"):
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/newave/hidr.py` & `inewave-0.0.96/inewave/newave/hidr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.hidr import RegistroUHEHidr
 from inewave.config import MESES_ABREV
 import pandas as pd  # type: ignore
 
 
-from typing import TypeVar, List, Optional
+from typing import TypeVar, List, Optional, Union, IO
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
 class Hidr(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao cadastro das
     usinas hidroelétricas.
     """
@@ -20,19 +24,33 @@
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__df: Optional[pd.DataFrame] = None
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="hidr.dat") -> "Hidr":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="hidr.dat"):
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
+
+    def write(self, to: Union[str, IO], *args, **kwargs):
         self.__atualiza_registros()
-        self.write(diretorio, nome_arquivo)
+        super().write(to, *args, **kwargs)
 
     def __monta_df_de_registros(self) -> Optional[pd.DataFrame]:
         registros: List[RegistroUHEHidr] = [
             r for r in self.data.of_type(RegistroUHEHidr)
         ]
         if len(registros) == 0:
             return None
```

### Comparing `inewave-0.0.95/inewave/newave/modelos/adterm.py` & `inewave-0.0.96/inewave/newave/modelos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/arquivos.py` & `inewave-0.0.96/inewave/newave/modelos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/arquivoscsv/arquivocsv.py` & `inewave-0.0.96/inewave/newave/modelos/arquivoscsv/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/avl_cortesfpha_nwv.py` & `inewave-0.0.96/inewave/newave/modelos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/avl_desvfpha_s.py` & `inewave-0.0.96/inewave/newave/modelos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/avl_desvfpha_v_q.py` & `inewave-0.0.96/inewave/newave/modelos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/blocos/tabelacsv.py` & `inewave-0.0.96/inewave/newave/modelos/blocos/tabelacsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/blocos/versaomodelo.py` & `inewave-0.0.96/inewave/newave/modelos/blocos/versaomodelo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/cadic.py` & `inewave-0.0.96/inewave/newave/modelos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/caso.py` & `inewave-0.0.96/inewave/newave/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/clast.py` & `inewave-0.0.96/inewave/newave/modelos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/confhd.py` & `inewave-0.0.96/inewave/newave/modelos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/conft.py` & `inewave-0.0.96/inewave/newave/modelos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/curva.py` & `inewave-0.0.96/inewave/newave/modelos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/cvar.py` & `inewave-0.0.96/inewave/newave/modelos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/dger.py` & `inewave-0.0.96/inewave/newave/modelos/dger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1169,15 +1169,15 @@
 
     def __init__(self, previous=None, next=None, data=None) -> None:
         super().__init__(previous, next, data)
         self.__linha = Line(
             [
                 LiteralField(24, 0),
                 IntegerField(1, 24),
-                IntegerField(1, 28),
+                IntegerField(4, 26),
                 LiteralField(76, 31),
             ]
         )
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, BlocoTipoSimFinal):
             return False
@@ -4835,7 +4835,101 @@
         :rtype: int | None
         """
         return self.data[1]
 
     @valor.setter
     def valor(self, v: int):
         self.data[1] = v
+
+
+class BlocoEstacoesBombeamento(Section):
+    """
+    Bloco com a escolha da consideração, ou não, de estações de bombeamento
+    no estudo.
+    """
+
+    def __init__(self, previous=None, next=None, data=None) -> None:
+        super().__init__(previous, next, data)
+        self.__linha = Line(
+            [LiteralField(24, 0), IntegerField(1, 24), LiteralField(14, 28)]
+        )
+
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, BlocoEstacoesBombeamento):
+            return False
+        bloco: BlocoEstacoesBombeamento = o
+        if not all(
+            [
+                isinstance(self.data, list),
+                isinstance(o.data, list),
+            ]
+        ):
+            return False
+        else:
+            return self.data == bloco.data
+
+    def read(self, file: IO, *args, **kwargs):
+        self.data = self.__linha.read(file.readline())
+
+    def write(self, file: IO, *args, **kwargs):
+        file.write(self.__linha.write(self.data))
+
+    @property
+    def valor(self) -> Optional[int]:
+        """
+        O valor da opção configurada
+
+        :return: A consideração ou não de estações de bombeamento
+        :rtype: int | None
+        """
+        return self.data[1]
+
+    @valor.setter
+    def valor(self, v: int):
+        self.data[1] = v
+
+
+class BlocoCanalDesvio(Section):
+    """
+    Bloco com a escolha da consideração, ou não, de canais de desvio entre usinas
+    hidrelétricas e reservatórios.
+    """
+
+    def __init__(self, previous=None, next=None, data=None) -> None:
+        super().__init__(previous, next, data)
+        self.__linha = Line(
+            [LiteralField(24, 0), IntegerField(1, 24), LiteralField(14, 28)]
+        )
+
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, BlocoCanalDesvio):
+            return False
+        bloco: BlocoCanalDesvio = o
+        if not all(
+            [
+                isinstance(self.data, list),
+                isinstance(o.data, list),
+            ]
+        ):
+            return False
+        else:
+            return self.data == bloco.data
+
+    def read(self, file: IO, *args, **kwargs):
+        self.data = self.__linha.read(file.readline())
+
+    def write(self, file: IO, *args, **kwargs):
+        file.write(self.__linha.write(self.data))
+
+    @property
+    def valor(self) -> Optional[int]:
+        """
+        O valor da opção configurada
+
+        :return: A consideração ou não de canais de desvio
+        :rtype: int | None
+        """
+        return self.data[1]
+
+    @valor.setter
+    def valor(self, v: int):
+        self.data[1] = v
```

### Comparing `inewave-0.0.95/inewave/newave/modelos/dsvagua.py` & `inewave-0.0.96/inewave/newave/modelos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/eafpast.py` & `inewave-0.0.96/inewave/newave/modelos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/enavazb.py` & `inewave-0.0.96/inewave/newave/modelos/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/enavazf.py` & `inewave-0.0.96/inewave/newave/modelos/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/energiab.py` & `inewave-0.0.96/inewave/newave/modelos/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/energiaf.py` & `inewave-0.0.96/inewave/newave/modelos/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/energias.py` & `inewave-0.0.96/inewave/newave/modelos/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/engnat.py` & `inewave-0.0.96/inewave/newave/modelos/engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/eolicacadastro.py` & `inewave-0.0.96/inewave/newave/modelos/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/eolicaconfiguracao.py` & `inewave-0.0.96/inewave/newave/modelos/eolicaconfiguracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/eolicafte.py` & `inewave-0.0.96/inewave/newave/modelos/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/eolicageracao.py` & `inewave-0.0.96/inewave/newave/modelos/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/eolicahistorico.py` & `inewave-0.0.96/inewave/newave/modelos/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/eolicaposto.py` & `inewave-0.0.96/inewave/newave/modelos/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/eolicasubmercado.py` & `inewave-0.0.96/inewave/newave/modelos/eolicasubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/exph.py` & `inewave-0.0.96/inewave/newave/modelos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/hidr.py` & `inewave-0.0.96/inewave/newave/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/modif.py` & `inewave-0.0.96/inewave/newave/modelos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/newavetim.py` & `inewave-0.0.96/inewave/newave/modelos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/nwv_avl_evap.py` & `inewave-0.0.96/inewave/newave/modelos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/nwv_cortes_evap.py` & `inewave-0.0.96/inewave/newave/modelos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/nwv_eco_evap.py` & `inewave-0.0.96/inewave/newave/modelos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/parp.py` & `inewave-0.0.96/inewave/newave/modelos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/parpeol.py` & `inewave-0.0.96/inewave/newave/modelos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/parpvaz.py` & `inewave-0.0.96/inewave/newave/modelos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/patamar.py` & `inewave-0.0.96/inewave/newave/modelos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/penalid.py` & `inewave-0.0.96/inewave/newave/modelos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/pmo.py` & `inewave-0.0.96/inewave/newave/modelos/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/re.py` & `inewave-0.0.96/inewave/newave/modelos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/ree.py` & `inewave-0.0.96/inewave/newave/modelos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/restricaoeletrica.py` & `inewave-0.0.96/inewave/newave/modelos/restricaoeletrica.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/restricaoenergia.py` & `inewave-0.0.96/inewave/newave/modelos/restricaoenergia.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/restricaovazao.py` & `inewave-0.0.96/inewave/newave/modelos/restricaovazao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/sistema.py` & `inewave-0.0.96/inewave/newave/modelos/sistema.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
         i = 0
         subsistemas: List[str] = []
         tabela = np.zeros((MAX_SUBMERCADOS, 10))
         while True:
             linha = file.readline()
             # Confere se terminaram
-            if len(linha) < 3 or BlocoCustosDeficit.FIM_BLOCO in linha:
+            if len(linha) < 3 or BlocoCustosDeficit.FIM_BLOCO in linha[:4]:
                 # Converte para df e salva na variável
                 if i > 0:
                     tabela = tabela[:i, :]
                     self.data = converte_tabela_em_df()
                 break
             # Confere se é uma linha de subsistema ou tabela
             else:
```

### Comparing `inewave-0.0.95/inewave/newave/modelos/term.py` & `inewave-0.0.96/inewave/newave/modelos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/vazaob.py` & `inewave-0.0.96/inewave/newave/modelos/vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/vazaof.py` & `inewave-0.0.96/inewave/newave/modelos/vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/vazaos.py` & `inewave-0.0.96/inewave/newave/modelos/vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/vazoes.py` & `inewave-0.0.96/inewave/newave/modelos/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modelos/vazpast.py` & `inewave-0.0.96/inewave/newave/modelos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/newave/modif.py` & `inewave-0.0.96/inewave/newave/modif.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     VMINP,
     VAZMINT,
 )
 
 
 from typing import Type, TypeVar, List, Optional, Union
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Modif(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às alterações nas
     configurações das usinas hidroelétricas.
     """
 
@@ -46,18 +50,29 @@
     ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="modif.dat") -> "Modif":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="modif.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/newavetim.py` & `inewave-0.0.96/inewave/newave/newavetim.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from inewave.newave.modelos.newavetim import BlocoTemposEtapasTim
 
 from cfinterface.components.block import Block
 from cfinterface.files.blockfile import BlockFile
 from typing import Type, TypeVar, Optional, Any
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class NewaveTim(BlockFile):
     """
     Armazena os dados de saída do NEWAVE referentes aos
     tempos de execução do programa.
 
     """
@@ -17,15 +21,20 @@
 
     BLOCKS = [BlocoTemposEtapasTim]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="newave.tim"
     ) -> "NewaveTim":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/nwv_avl_evap.py` & `inewave-0.0.96/inewave/newave/nwv_eco_evap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 from inewave.newave.modelos.blocos.versaomodelo import VersaoModelo
-from inewave.newave.modelos.nwv_avl_evap import TabelaAvlEvap
+from inewave.newave.modelos.nwv_eco_evap import TabelaEcoEvap
 
 from inewave.newave.modelos.arquivoscsv.arquivocsv import ArquivoCSV
 from typing import Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class NwvAvlEvap(ArquivoCSV):
+
+class NwvEcoEvap(ArquivoCSV):
     """
-    Arquivo com a avaliação da evaporação linear do NEWAVE.
+    Arquivo com o eco dos dados da evaporação linear do NEWAVE.
     """
 
-    BLOCKS = [VersaoModelo, TabelaAvlEvap]
+    BLOCKS = [VersaoModelo, TabelaEcoEvap]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, arquivo: str = "nwv_avl_evap.csv"
-    ) -> "NwvAvlEvap":
-        return cls.read(diretorio, arquivo)
+        cls, diretorio: str, arquivo: str = "nwv_eco_evap.csv"
+    ) -> "NwvEcoEvap":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, arquivo))
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
         - periodo (`int`)
         - indice_usina (`int`)
         - nome_usina (`str`)
-        - volume_armazenado_hm3 (`float`)
-        - evaporacao_calculada_hm3 (`float`)
-        - evaporacao_modelo_hm3 (`float`)
-        - desvio_absoluto_hm3 (`float`)
-        - desvio_percentual (`float`)
+        - volume_referencia_hm3 (`float`)
+        - evaporacao_referencia_hm3 (`float`)
+        - coeficiente_evaporacao_mm_mes (`int`)
+        - flag_evaporacao (`int`)
+        - evaporacao_linear (`int`)
+        - tipo_volume_referencia (`int`)
 
         :return: A tabela como um dataframe
         :rtype: pd.DataFrame | None
         """
         return self._tabela()
```

### Comparing `inewave-0.0.95/inewave/newave/parp.py` & `inewave-0.0.96/inewave/newave/parp.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from inewave.newave.modelos.parp import BlocoCorrelEspacialMensalConfig
 
 from cfinterface.components.block import Block
 from cfinterface.files.blockfile import BlockFile
 from typing import Type, TypeVar, Optional, Any, List
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class PARp(BlockFile):
     """
     Armazena os dados de saída do NEWAVE referentes aos modelos e às
     séries sintéticas de energia geradas pelo PAR(p).
 
 
@@ -57,15 +61,20 @@
         self.__ordem_final_modelo = None
         self.__coeficientes = None
         self.__correl_espacial_anual = None
         self.__correl_espacial_mensal = None
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="parp.dat") -> "PARp":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def __rees(self) -> Optional[List[str]]:
         """
         Retorna a lista dos REEs lidos do arquivo.
 
         :return: Os nomes dos REEs
         :rtype: List[str]
```

### Comparing `inewave-0.0.95/inewave/newave/parpeol.py` & `inewave-0.0.96/inewave/newave/parpeol.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from inewave.newave.modelos.parpeol import BlocoCorrelEspacialMensalConfig
 
 from cfinterface.components.block import Block
 from cfinterface.files.blockfile import BlockFile
 from typing import Type, TypeVar, Optional, Any, List
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class PARpeol(BlockFile):
     """
     Armazena os dados de saída do NEWAVE referentes às
     séries sintéticas de ventos geradas pelo PAR(p).
 
     Esta classe lida com informações de saída do NEWAVE e
@@ -42,15 +46,20 @@
         self.__correl_espacial_anual = None
         self.__correl_espacial_mensal = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="parpeol.dat"
     ) -> "PARpeol":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def __uees(self) -> Optional[List[str]]:
         """
         Retorna a lista das UEEs lidos do arquivo.
 
         :return: Os nomes das UEEs
         :rtype: List[str]
```

### Comparing `inewave-0.0.95/inewave/newave/parpvaz.py` & `inewave-0.0.96/inewave/newave/parpvaz.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 from inewave.newave.modelos.parpvaz import BlocoCorrelEspacialAnualMensalUHE
 
 from cfinterface.components.block import Block
 from cfinterface.files.blockfile import BlockFile
 from typing import Type, TypeVar, Optional, Any, List
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class PARpvaz(BlockFile):
     """
     Armazena os dados de saída do NEWAVE referentes aos modelos e às
     séries sintéticas de vazões geradas pelo PAR(p).
 
 
@@ -50,15 +54,20 @@
         self.__coeficientes = None
         self.__correl_espacial_anual_mensal = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="parpvaz.dat"
     ) -> "PARpvaz":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def __uhes(self) -> Optional[List[str]]:
         """
         Retorna a lista das UHEs lidos do arquivo.
 
         :return: Os nomes das UHEs
         :rtype: List[str]
```

### Comparing `inewave-0.0.95/inewave/newave/patamar.py` & `inewave-0.0.96/inewave/newave/patamar.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,18 @@
     BlocoUsinasNaoSimuladas,
 )
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import Type, TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Patamar(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes aos
     patamares de carga por submercado.
 
     """
@@ -31,18 +35,29 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="patamar.dat"
     ) -> "Patamar":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="patamar.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/penalid.py` & `inewave-0.0.96/inewave/newave/penalid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type, Optional
 import pandas as pd  # type: ignore
 
 from inewave.newave.modelos.penalid import BlocoPenalidades
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Penalid(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às penalidades
     aplicadas por desvio.
 
     """
@@ -20,18 +24,29 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="penalid.dat"
     ) -> "Penalid":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="penalid.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/perda.py` & `inewave-0.0.96/inewave/newave/expt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Perda(SectionFile):
+
+class Expt(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes aos fatores de perda
-    das usinas e das interligações.
+    Armazena os dados de entrada do NEWAVE referentes à expansão
+    térmica do sistema.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="perda.dat") -> "Perda":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="perda.dat"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(cls, diretorio: str, nome_arquivo="expt.dat") -> "Expt":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
+
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="expt.dat"):
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/newave/pmo.py` & `inewave-0.0.96/inewave/newave/pmo.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from inewave.newave.modelos.pmo import BlocoProdutibilidadesConfiguracaoPMO
 
 from cfinterface.components.block import Block
 from cfinterface.files.blockfile import BlockFile
 from typing import Type, TypeVar, Optional, Any
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class PMO(BlockFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao
     acompanhamento do programa.
 
     Esta classe lida com as informações de entrada fornecidas ao
@@ -40,15 +44,20 @@
         BlocoCustoOperacaoPMO,
         BlocoCustoOperacaoTotalPMO,
         BlocoProdutibilidadesConfiguracaoPMO,
     ]
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="pmo.dat") -> "PMO":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/re.py` & `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoree.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from inewave.newave.modelos.re import (
-    BlocoUsinasConjuntoRE,
-    BlocoConfiguracaoRestricoesRE,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.blocos.valoresserie import (
+    ValoresSerie,
 )
 
-from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
+from typing import Type, TypeVar, Optional
 
 
-class RE(SectionFile):
+class ArquivoREE(BlockFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às restrições
-    elétricas existentes.
-
+    Armazena os dados das saídas por REE.
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [
-        BlocoUsinasConjuntoRE,
-        BlocoConfiguracaoRestricoesRE,
-    ]
+    BLOCKS = [REE, ValoresSerie]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
+        self.__valores = None
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="re.dat") -> "RE":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="arq.out"
+    ) -> "ArquivoREE":
         return cls.read(diretorio, nome_arquivo)
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="re.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
@@ -48,57 +46,51 @@
                 b
                 for i, b in enumerate(self.data.of_type(bloco))
                 if i == indice
             )
         except StopIteration:
             return None
 
+    def __monta_tabela(self) -> pd.DataFrame:
+        df = None
+        for b in self.data.of_type(ValoresSerie):
+            dados = b.data
+            if dados is None:
+                continue
+            elif df is None:
+                df = b.data
+            else:
+                df = pd.concat([df, b.data], ignore_index=True)
+        return df
+
     @property
-    def usinas_conjuntos(self) -> Optional[pd.DataFrame]:
+    def valores(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com os conjuntos de usinas com restrições elétricas.
+        Tabela com os valores, por série e
+        por mês/ano de estudo.
 
-        - Conjunto (`int`)
-        - Usina 1 (`float`)
-        - Usina 2 (`float`)
+        - Ano (`int`)
+        - Série (`int`)
+        - Patamar (`str`)
+        - Janeiro (`float`)
         - ...
-        - Usina N (`float`)
+        - Dezembro (`float`)
 
-        :return: A tabela como um DataFrame.
+        :return: A tabela dos valores.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoUsinasConjuntoRE, 0)
-        if b is not None:
-            return b.data
-        return None
-
-    @usinas_conjuntos.setter
-    def usinas_conjuntos(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoUsinasConjuntoRE, 0)
-        if b is not None:
-            b.data = df
+        if self.__valores is None:
+            self.__valores = self.__monta_tabela()
+        return self.__valores
 
     @property
-    def restricoes(self) -> Optional[pd.DataFrame]:
+    def ree(self) -> Optional[str]:
         """
-        Tabela com as configurações das restrições elétricas.
-
-        - Conjunto (`int`)
-        - Mês Início (`int`)
-        - Mês Fim (`int`)
-        - Ano Início (`int`)
-        - Ano Fim (`int`)
-        - Flag P (`int`)
+        O REE associado ao arquivo lido.
 
-        :return: A tabela como um DataFrame.
-        :rtype: pd.DataFrame | None
+        :return: O nome do ree
+        :rtype: str
         """
-        b = self.__bloco_por_tipo(BlocoConfiguracaoRestricoesRE, 0)
+        b = self.__bloco_por_tipo(REE, 0)
         if b is not None:
             return b.data
         return None
-
-    @restricoes.setter
-    def restricoes(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoConfiguracaoRestricoesRE, 0)
-        if b is not None:
-            b.data = df
```

### Comparing `inewave-0.0.95/inewave/newave/ree.py` & `inewave-0.0.96/inewave/newave/ree.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import pandas as pd  # type: ignore
 
 from inewave.newave.modelos.ree import (
     BlocoReesSubmercados,
     BlocoFicticiasIndividualizado,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class REE(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às configurações
     dos REEs.
 
     """
@@ -25,18 +29,29 @@
     ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="ree.dat") -> "REE":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="ree.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/restricaoeletrica.py` & `inewave-0.0.96/inewave/newave/restricaoeletrica.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.restricaoeletrica import (
     RegistroRE,
     RegistroREHorizPer,
     RegistroRELimFormPer,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class RestricaoEletrica(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao cadastro
     das restrições lineares por partes no domínio de energia (REE).
     """
 
@@ -27,20 +31,31 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="restricao-eletrica.csv"
     ) -> "RestricaoEletrica":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(
         self, diretorio: str, nome_arquivo="restricao-eletrica.csv"
     ):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
```

### Comparing `inewave-0.0.95/inewave/newave/restricaoenergia.py` & `inewave-0.0.96/inewave/newave/restricaoenergia.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.restricaoenergia import (
     RegistroRHE,
     RegistroRHEHorizPer,
     RegistroRHELsLPPEarmi,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class RestricaoEnergia(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao cadastro
     das restrições lineares por partes no domínio de energia (REE).
     """
 
@@ -27,20 +31,31 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="restricao-energia.csv"
     ) -> "RestricaoEnergia":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(
         self, diretorio: str, nome_arquivo="restricao-energia.csv"
     ):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
```

### Comparing `inewave-0.0.95/inewave/newave/restricaovazao.py` & `inewave-0.0.96/inewave/newave/restricaovazao.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.restricaovazao import (
     RegistroRHQ,
     RegistroRHQHorizPer,
     RegistroRHQLsLPPVoli,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class RestricaoVazao(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao cadastro
     das restrições lineares por partes no domínio de vazão (RHQ).
     """
 
@@ -27,20 +31,31 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="restricao-vazao.csv"
     ) -> "RestricaoVazao":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(
         self, diretorio: str, nome_arquivo="restricao-vazao.csv"
     ):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
         """
         Obtém os registro de um tipo, se houver algum no arquivo.
 
         :param registro: Um tipo de registro para ser lido
         :type registro: T
```

### Comparing `inewave-0.0.95/inewave/newave/shist.py` & `inewave-0.0.96/inewave/newave/perda.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Shist(SectionFile):
+
+class Perda(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes à varredura
-    das séries históricas para simulação.
+    Armazena os dados de entrada do NEWAVE referentes aos fatores de perda
+    das usinas e das interligações.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="shist.dat") -> "Shist":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="shist.dat"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(cls, diretorio: str, nome_arquivo="perda.dat") -> "Perda":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
+
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="perda.dat"):
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/newave/sistema.py` & `inewave-0.0.96/inewave/newave/sistema.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 )
 
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import Type, TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Sistema(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às configurações
     dos subsistemas (submercados).
 
     """
@@ -32,18 +36,29 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="sistema.dat"
     ) -> "Sistema":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="sistema.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/tecno.py` & `inewave-0.0.96/inewave/newave/itaipu.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Tecno(SectionFile):
+
+class Itaipu(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às tecnologias
-    disponíveis para geração de energia.
+    Armazena os dados de entrada do NEWAVE referentes às restrições
+    de Itaipu.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="tecno.dat") -> "Tecno":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="tecno.dat"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(cls, diretorio: str, nome_arquivo="itaipu.dat") -> "Itaipu":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
+
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="itaipu.dat"):
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/newave/term.py` & `inewave-0.0.96/inewave/newave/term.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from inewave.newave.modelos.term import BlocoTermUTE
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import Type, TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Term(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes aos dados das
     usinas térmicas.
     """
 
@@ -16,18 +20,29 @@
     SECTIONS = [BlocoTermUTE]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="term.dat") -> "Term":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="term.dat"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
```

### Comparing `inewave-0.0.95/inewave/newave/vazaob.py` & `inewave-0.0.96/inewave/newave/vazaob.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from cfinterface.files.sectionfile import SectionFile
 from inewave.newave.modelos.vazaob import SecaoDadosVazaob
 import pandas as pd  # type: ignore
 
 from typing import TypeVar, Optional
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Vazaob(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às séries sintéticas
     de vazão para a etapa backward geradas pelo modelo.
     """
 
@@ -25,26 +29,27 @@
         diretorio: str,
         nome_arquivo="vazaob.dat",
         numero_forwards: int = 200,
         numero_aberturas: int = 20,
         numero_uhes: int = 164,
         numero_estagios: int = 60,
     ) -> "Vazaob":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
         return cls.read(
-            diretorio,
-            nome_arquivo,
+            join(diretorio, nome_arquivo),
             numero_forwards=numero_forwards,
             numero_aberturas=numero_aberturas,
             numero_uhes=numero_uhes,
             numero_estagios=numero_estagios,
         )
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vazaob.dat"):
-        self.write(diretorio, nome_arquivo)
-
     @property
     def series(self) -> Optional[pd.DataFrame]:
         """
         Obtém a tabela com os dados das séries de vazão
         afluente por UHE, por estágio, série forward e abertura.
 
         - estagio (`int`): estágio do cenário gerado
```

### Comparing `inewave-0.0.95/inewave/newave/vazaof.py` & `inewave-0.0.96/inewave/newave/vazaof.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from cfinterface.files.sectionfile import SectionFile
 from inewave.newave.modelos.vazaof import SecaoDadosVazaof
 import pandas as pd  # type: ignore
 
 from typing import TypeVar, Optional
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Vazaof(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às séries sintéticas
     de vazão para a etapa forward geradas pelo modelo.
     """
 
@@ -25,26 +29,27 @@
         diretorio: str,
         nome_arquivo="vazaof.dat",
         numero_forwards: int = 200,
         numero_uhes: int = 164,
         numero_estagios: int = 60,
         numero_estagios_th: int = 12,
     ) -> "Vazaof":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
         return cls.read(
-            diretorio,
-            nome_arquivo,
+            join(diretorio, nome_arquivo),
             numero_forwards=numero_forwards,
             numero_uhes=numero_uhes,
             numero_estagios=numero_estagios,
             numero_estagios_th=numero_estagios_th,
         )
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vazaof.dat"):
-        self.write(diretorio, nome_arquivo)
-
     @property
     def series(self) -> Optional[pd.DataFrame]:
         """
         Obtém a tabela com os dados das séries de vazão
         afluente por UHE e por estágio.
 
         - estagio (`int`): estágio do cenário gerado
```

### Comparing `inewave-0.0.95/inewave/newave/vazoes.py` & `inewave-0.0.96/inewave/newave/vazoes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.vazoes import RegistroVazoesPostos
 import pandas as pd  # type: ignore
 
 
-from typing import TypeVar, List, Optional
+from typing import TypeVar, List, Optional, Union, IO
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
 class Vazoes(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao cadastro das
     usinas hidroelétricas.
     """
@@ -21,19 +25,33 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__df: Optional[pd.DataFrame] = None
         RegistroVazoesPostos.set_postos(self.POSTOS)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="vazoes.dat") -> "Vazoes":
-        return cls.read(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="vazoes.dat"):
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
+
+    def write(self, to: Union[str, IO], *args, **kwargs):
         self.__atualiza_registros()
-        self.write(diretorio, nome_arquivo)
+        super().write(to, *args, **kwargs)
 
     def __monta_df_de_registros(self) -> Optional[pd.DataFrame]:
         registros: List[RegistroVazoesPostos] = [
             r for r in self.data.of_type(RegistroVazoesPostos)
         ]
         if len(registros) == 0:
             return None
```

### Comparing `inewave-0.0.95/inewave/newave/vazpast.py` & `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from inewave.newave.modelos.vazpast import BlocoVazPast
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
+)
 
-from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
+from typing import Type, TypeVar, Optional
 
 
-class VazPast(SectionFile):
+class ArquivoREEPatamar(BlockFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às
-    vazões anteriores ao período de planejamento.
-
-    Esta classe lida com informações de entrada fornecidas ao NEWAVE e
-    que são usadas juntos das contidas no arquivo `vazoes.dat`.
-
+    Armazena os dados das saídas por patamar, por REE.
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoVazPast]
+    BLOCKS = [REE, ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
+        self.__valores = None
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vazpast.dat"
-    ) -> "VazPast":
+        cls, diretorio: str, nome_arquivo="arq.out"
+    ) -> "ArquivoREEPatamar":
         return cls.read(diretorio, nome_arquivo)
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vazpast.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
@@ -47,31 +46,51 @@
                 b
                 for i, b in enumerate(self.data.of_type(bloco))
                 if i == indice
             )
         except StopIteration:
             return None
 
+    def __monta_tabela(self) -> pd.DataFrame:
+        df = None
+        for b in self.data.of_type(ValoresSeriePatamar):
+            dados = b.data
+            if dados is None:
+                continue
+            elif df is None:
+                df = b.data
+            else:
+                df = pd.concat([df, b.data], ignore_index=True)
+        return df
+
     @property
-    def tendencia(self) -> Optional[pd.DataFrame]:
+    def valores(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com a tendência hidrológica por REE.
+        Tabela com os valores por patamar, por série e
+        por mês/ano de estudo.
 
-        - Índice (`int`)
-        - Usina (`str`)
+        - Ano (`int`)
+        - Série (`int`)
+        - Patamar (`str`)
         - Janeiro (`float`)
         - ...
         - Dezembro (`float`)
 
-        :return: A tabela como um DataFrame
+        :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoVazPast, 0)
+        if self.__valores is None:
+            self.__valores = self.__monta_tabela()
+        return self.__valores
+
+    @property
+    def ree(self) -> Optional[str]:
+        """
+        O REE associado ao arquivo lido.
+
+        :return: O nome do REE
+        :rtype: str
+        """
+        b = self.__bloco_por_tipo(REE, 0)
         if b is not None:
             return b.data
         return None
-
-    @tendencia.setter
-    def tendencia(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoVazPast, 0)
-        if b is not None:
-            b.data = df
```

### Comparing `inewave-0.0.95/inewave/nwlistcf/estados.py` & `inewave-0.0.96/inewave/nwlistcf/estados.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from inewave.nwlistcf.modelos.estados import EstadosPeriodoNwlistcf
 
 from cfinterface.files.blockfile import BlockFile
 from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Estados(BlockFile):
     """
     Armazena os dados dos estados visitados pelo NEWAVE existentes
     no arquivo `estados.rel` do NWLISTCF.
 
     Esta classe armazena os estados de cada uma das variáveis envolvidas
@@ -24,18 +28,20 @@
         super().__init__(data)
         self.__estados_periodos = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="estados.rel"
     ) -> "Estados":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="estados.rel"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def __monta_tabela_estados(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(EstadosPeriodoNwlistcf):
             dados = b.data
             if dados is None:
                 continue
```

### Comparing `inewave-0.0.95/inewave/nwlistcf/modelos/estados.py` & `inewave-0.0.96/inewave/nwlistcf/modelos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistcf/modelos/nwlistcf.py` & `inewave-0.0.96/inewave/nwlistcf/modelos/nwlistcf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistcf/nwlistcf.py` & `inewave-0.0.96/inewave/nwlistcf/nwlistcf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from inewave.nwlistcf.modelos.nwlistcf import CortesPeriodoNwlistcf
 
 from cfinterface.files.blockfile import BlockFile
 from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Nwlistcf(BlockFile):
     """
     Armazena os dados dos cortes construídos pelo NEWAVE existentes
     no arquivo `nwlistcf.rel` do NWLISTCF.
 
     Esta classe armazena os cortes da FCF de cada uma das variáveis,
@@ -23,18 +27,20 @@
         super().__init__(data)
         self.__cortes_periodos = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="nwlistcf.rel"
     ) -> "Nwlistcf":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="nwlistcf.rel"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
 
     def __monta_tabela_cortes(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(CortesPeriodoNwlistcf):
             dados = b.data
             if dados is None:
                 continue
```

### Comparing `inewave-0.0.95/inewave/nwlistop/__init__.py` & `inewave-0.0.96/inewave/nwlistop/__init__.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/cdef.py` & `inewave-0.0.96/inewave/nwlistop/cdef.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from inewave.nwlistop.modelos.cdef import CdefAnos
 
 from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
     ArquivoSubmercado,
     Submercado,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Cdef(ArquivoSubmercado):
     """
     Armazena os dados das saídas referentes ao custo de déficit
     de cada estágio em cada série.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `cdef00x.out`.
     """
 
     BLOCKS = [CdefAnos, Submercado]
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="cdef001.out") -> "Cdef":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="cdef001.out"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/cdefsin.py` & `inewave-0.0.96/inewave/nwlistop/fteolm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,37 @@
-from inewave.nwlistop.modelos.cdefsin import CdefAnos
-
-from inewave.nwlistop.modelos.arquivos.arquivosin import (
-    ArquivoSIN,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
+    ArquivoSubmercadoPatamar,
 )
+from inewave.nwlistop.modelos.exces import ExcesAnos
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
-class CdefSIN(ArquivoSIN):
+class Fteolm(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes ao custo de déficit
-    de cada estágio em cada série.
+    Armazena os dados das saídas referentes à folga da variável de
+    geração eólica por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `cdefsin.out`.
+    NWLISTOP e reproduzidas nos `fteolm00x.out`, onde x varia conforme o
+    submercado em questão.
+
     """
 
     BLOCKS = [
-        CdefAnos,
+        Submercado,
+        ExcesAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="cdefsin.out"
-    ) -> "CdefSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="cdefsin.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="fteolm001.out"
+    ) -> "Fteolm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/cmarg.py` & `inewave-0.0.96/inewave/nwlistop/cmarg.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.cmarg import CmargsAnos
 from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
     ArquivoSubmercadoPatamar,
 )
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Cmarg(ArquivoSubmercadoPatamar):
     """
     Armazena os dados das saídas referentes aos custos marginais de operação
     por patamar, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
@@ -21,11 +25,13 @@
         CmargsAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="cmarg001.out"
     ) -> "Cmarg":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="cmarg001.out"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/coper.py` & `inewave-0.0.96/inewave/nwlistop/gttot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,37 @@
-from inewave.nwlistop.modelos.coper import CoperAnos
-
-from inewave.nwlistop.modelos.arquivos.arquivosin import (
-    ArquivoSIN,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
+    ArquivoSubmercadoPatamar,
 )
+from inewave.nwlistop.modelos.gttot import GTAnos
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
-class Coper(ArquivoSIN):
+class Gttot(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes ao custo total de operação
-    de cada estágio em cada série.
+    Armazena os dados das saídas referentes à geração térmica total
+    por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `coper.out`.
+    NWLISTOP e reproduzidas nos `gttot00x.out`, onde x varia conforme o
+    REE em questão.
+
     """
 
     BLOCKS = [
-        CoperAnos,
+        Submercado,
+        GTAnos,
     ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="coper.out") -> "Coper":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="coper.out"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="gttot001.out"
+    ) -> "Gttot":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/corteolm.py` & `inewave-0.0.96/inewave/nwlistop/ghmaxm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
     ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.corteolm import CorteolmAnos
+from inewave.nwlistop.modelos.ghmaxm import GHAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Corteolm(ArquivoSubmercadoPatamar):
+
+class Ghmaxm(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes ao corte de geração eólica.
+    Armazena os dados das saídas referentes à geração hidraulica máxima
+    por patamar, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `corteolm00x.out`, onde x varia conforme
-    a usina em questão.
+    NWLISTOP e reproduzidas nos `ghmax00x.out`, onde x varia conforme o
+    Submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        CorteolmAnos,
+        GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="corteolm001.out"
-    ) -> "Corteolm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="corteolm001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="ghmaxm001.out"
+    ) -> "Ghmaxm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/cterm.py` & `inewave-0.0.96/inewave/nwlistop/invadem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.cterm import CtermsAnos
 from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
     ArquivoSubmercado,
 )
+from inewave.nwlistop.modelos.invade import InvadeAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Cterm(ArquivoSubmercado):
+
+class Invadem(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes aos custos de geração térmica
-    por patamar, por submercado.
+    Armazena os dados das saídas referentes às violações da CAR
+    , por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `cterm00x.out`, onde x varia conforme o
-    submercado em questão.
+    NWLISTOP e reproduzidas nos `invadem00x.out`, onde x varia conforme o
+    REE em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        CtermsAnos,
+        InvadeAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="cterm001.out"
-    ) -> "Cterm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="cterm001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="invadem001.out"
+    ) -> "Invadem":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/ctermsin.py` & `inewave-0.0.96/inewave/nwlistop/varmuh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-from inewave.nwlistop.modelos.ctermsin import CtermsAnos
-from inewave.nwlistop.modelos.arquivos.arquivosin import (
-    ArquivoSIN,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousina import (
+    ArquivoUsina,
 )
+from inewave.nwlistop.modelos.varmuh import VarmAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class CtermSIN(ArquivoSIN):
+
+class VarmUH(ArquivoUsina):
     """
-    Armazena os dados das saídas referentes aos custos de geração térmica
-    para o SIN.
+    Armazena os dados das saídas referentes aos armazenamentos por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ctermsin.out`.
+    NWLISTOP e reproduzidas nos `varmuh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
-        CtermsAnos,
+        Usina,
+        VarmAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ctermsin.out"
-    ) -> "CtermSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ctermsin.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="varmuh001.out"
+    ) -> "VarmUH":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/deficit.py` & `inewave-0.0.96/inewave/nwlistop/evertm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
-    ArquivoSubmercadoPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.defsin import DefAnos
+from inewave.nwlistop.modelos.evertm import EvertAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Def(ArquivoSubmercadoPatamar):
+
+class Evertm(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes à geração hidraulica total
-    por patamar, por submercado.
+    Armazena os dados das saídas referentes ao vertimento de reservatórios
+    , por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghtotm00x.out`, onde x varia conforme o
-    submercado em questão.
+    NWLISTOP e reproduzidas nos `evertm00x.out`, onde x varia conforme o
+    Submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        DefAnos,
+        EvertAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="def001p001.out"
-    ) -> "Def":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="def001p001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="evertm001.out"
+    ) -> "Evertm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/defsin.py` & `inewave-0.0.96/inewave/nwlistop/defsin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
     ArquivoSINPatamar,
 )
 from inewave.nwlistop.modelos.defsin import DefAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class DefSIN(ArquivoSINPatamar):
     """
     Armazena os dados das saídas referentes ao déficit
     por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
@@ -17,11 +21,13 @@
         DefAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="defsinp001.out"
     ) -> "DefSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="defsinp001.out"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/depminuh.py` & `inewave-0.0.96/inewave/nwlistop/dlppdfmax.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
+    ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.depminuh import DepminAnos
+from inewave.nwlistop.modelos.dlppdfmax import DLPPdfmaxAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Depminuh(ArquivoUsinaPatamar):
+
+class DLPPdfmax(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes À violação de defluência
-    mínima da usina.
+    Armazena os dados das saídas referentes à violação das restrições LPP
+    de defluência máxima por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `depminuh00x.out`, onde x varia conforme
-    a usina em questão.
+    NWLISTOP e reproduzidas nos `dlppdfmax00x.out`, onde x varia conforme o
+    REE em questão.
 
     """
 
     BLOCKS = [
-        Usina,
-        DepminAnos,
+        REE,
+        DLPPdfmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="depminuh001.out"
-    ) -> "Depminuh":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="depminuh001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="dlppdfmax001.out"
+    ) -> "DLPPdfmax":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/dfphauh.py` & `inewave-0.0.96/inewave/nwlistop/varmpuh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivousina import (
+    ArquivoUsina,
 )
-from inewave.nwlistop.modelos.dfphauh import DfphauhAnos
+from inewave.nwlistop.modelos.varmpuh import VarmAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Dfphauh(ArquivoUsinaPatamar):
+
+class VarmpUH(ArquivoUsina):
     """
-    Armazena os dados das saídas referentes à variável de folga da
-    FPHA da usina.
+    Armazena os dados das saídas referentes aos armazenamentos em
+    percentual por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dfphauh00x.out`, onde x varia conforme
-    a usina em questão.
+    NWLISTOP e reproduzidas nos `varmpuh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        DfphauhAnos,
+        VarmAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dfphauh001.out"
-    ) -> "Dfphauh":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="dfphauh001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="varmpuh001.out"
+    ) -> "VarmpUH":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/dlppdfmaxm.py` & `inewave-0.0.96/inewave/nwlistop/mercl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
-    ArquivoSubmercadoPatamar,
+from inewave.nwlistop.modelos.merclsin import MerclAnos
+
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.dlppdfmax import DLPPdfmaxAnos
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
-class DLPPdfmaxm(ArquivoSubmercadoPatamar):
+class Mercl(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes à violação das restrições LPP
-    de defluência máxima por patamar, por Submercado.
+    Armazena os dados das saídas referentes ao mercado líquido
+    de cada estágio em cada série por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dlppdfmax00x.out`, onde x varia conforme o
-    Submercado em questão.
-
+    NWLISTOP e reproduzidas nos `mercl001.out`.
     """
 
     BLOCKS = [
         Submercado,
-        DLPPdfmaxAnos,
+        MerclAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dlppdfmaxm001.out"
-    ) -> "DLPPdfmaxm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(
-        self, diretorio: str, nome_arquivo="dlppdfmaxm001.out"
-    ):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="mercl001.out"
+    ) -> "Mercl":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/dlppdfmaxs.py` & `inewave-0.0.96/inewave/nwlistop/vertuh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,36 @@
-from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
-    ArquivoSINPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.dlppdfmaxs import DLPPdfmaxAnos
+from inewave.nwlistop.modelos.vertuh import VertAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class DLPPdfmaxs(ArquivoSINPatamar):
+
+class VertUH(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à violação das restrições
-    LPP de defluência máxima por patamar para o SIN.
+    Armazena os dados das saídas referentes aos vertimentos por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dlppdfmaxs.out`.
+    NWLISTOP e reproduzidas nos `vertuh00x.out`, onde x varia conforme a
+    usina em questão.
+
     """
 
     BLOCKS = [
-        DLPPdfmaxAnos,
+        Usina,
+        VertAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dlppdfmaxs.out"
-    ) -> "DLPPdfmaxs":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="dlppdfmaxs.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="vertuh001.out"
+    ) -> "VertUH":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/dlpptbmax.py` & `inewave-0.0.96/inewave/nwlistop/depminuh.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
-    ArquivoREEPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.dlpptbmax import DLPPtbmaxAnos
+from inewave.nwlistop.modelos.depminuh import DepminAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class DLPPtbmax(ArquivoREEPatamar):
+
+class Depminuh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à violação das restrições LPP
-    de turbinamento máximo por patamar, por REE.
+    Armazena os dados das saídas referentes À violação de defluência
+    mínima da usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dlpptbmax00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `depminuh00x.out`, onde x varia conforme
+    a usina em questão.
 
     """
 
     BLOCKS = [
-        REE,
-        DLPPtbmaxAnos,
+        Usina,
+        DepminAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dlpptbmax001.out"
-    ) -> "DLPPtbmax":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="dlpptbmax001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="depminuh001.out"
+    ) -> "Depminuh":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/dlpptbmaxm.py` & `inewave-0.0.96/inewave/nwlistop/exces.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
     ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.dlppdfmax import DLPPdfmaxAnos
+from inewave.nwlistop.modelos.exces import ExcesAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class DLPPtbmaxm(ArquivoSubmercadoPatamar):
+
+class Exces(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes à violação das restrições LPP
-    de turbinamento máximo por patamar, por Submercado.
+    Armazena os dados das saídas referentes ao excesso de energia
+    por patamar, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dlpptbmax00x.out`, onde x varia conforme o
-    Submercado em questão.
+    NWLISTOP e reproduzidas nos `exces00x.out`, onde x varia conforme o
+    submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        DLPPdfmaxAnos,
+        ExcesAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dlpptbmaxm001.out"
-    ) -> "DLPPtbmaxm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(
-        self, diretorio: str, nome_arquivo="dlpptbmaxm001.out"
-    ):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="exces001.out"
+    ) -> "Exces":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/dlpptbmaxs.py` & `inewave-0.0.96/inewave/nwlistop/dlpptbmaxs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
     ArquivoSINPatamar,
 )
 from inewave.nwlistop.modelos.dlpptbmaxs import DLPPtbmaxAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class DLPPtbmaxs(ArquivoSINPatamar):
     """
     Armazena os dados das saídas referentes à violação das restrições
     LPP de turbinamento máximo por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
@@ -17,11 +21,13 @@
         DLPPtbmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="dlpptbmaxs.out"
     ) -> "DLPPtbmaxs":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="dlpptbmaxs.out"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/dtbmax.py` & `inewave-0.0.96/inewave/nwlistop/qincruh.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivousina import (
+    ArquivoUsina,
 )
-from inewave.nwlistop.modelos.dtbmax import DtbmaxAnos
+from inewave.nwlistop.modelos.qincruh import QincrAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Dtbmax(ArquivoUsinaPatamar):
+
+class QincrUH(ArquivoUsina):
     """
-    Armazena os dados das saídas referentes à violação de restrição de
-    turbinamento máximo por usina.
+    Armazena os dados das saídas referentes às vazões incrementais por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dtbmax00x.out`, onde x varia conforme
-    a usina em questão.
+    NWLISTOP e reproduzidas nos `qincruh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        DtbmaxAnos,
+        QincrAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dtbmax001.out"
-    ) -> "Dtbmax":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="dtbmax001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="qincruh001.out"
+    ) -> "QincrUH":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/dtbmin.py` & `inewave-0.0.96/inewave/nwlistop/vturuh.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.dtbmin import DtbminAnos
+from inewave.nwlistop.modelos.vturuh import VturAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Dtbmin(ArquivoUsinaPatamar):
+
+class VturUH(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à violação de restrição de
-    turbinamento mínimo por usina.
+    Armazena os dados das saídas referentes às vazões turbinadas por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dtbmin00x.out`, onde x varia conforme
-    a usina em questão.
+    NWLISTOP e reproduzidas nos `vturuh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        DtbminAnos,
+        VturAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dtbmin001.out"
-    ) -> "Dtbmin":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="dtbmin001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="vturuh001.out"
+    ) -> "VturUH":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/dvazmax.py` & `inewave-0.0.96/inewave/nwlistop/deficit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
+    ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.dvazmax import DvazmaxAnos
+from inewave.nwlistop.modelos.defsin import DefAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Dvazmax(ArquivoUsinaPatamar):
+
+class Def(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes à violação de restrição de
-    vazão máxima por usina.
+    Armazena os dados das saídas referentes à geração hidraulica total
+    por patamar, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dvazmax00x.out`, onde x varia conforme
-    a usina em questão.
+    NWLISTOP e reproduzidas nos `ghtotm00x.out`, onde x varia conforme o
+    submercado em questão.
 
     """
 
     BLOCKS = [
-        Usina,
-        DvazmaxAnos,
+        Submercado,
+        DefAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dvazmax001.out"
-    ) -> "Dvazmax":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="dvazmax001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="def001p001.out"
+    ) -> "Def":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/eaf.py` & `inewave-0.0.96/inewave/nwlistop/verturbm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,37 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
-from inewave.nwlistop.modelos.eaf import EafsAnos
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
+)
+from inewave.nwlistop.modelos.verturbm import VertAnos
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
-class Eaf(ArquivoREE):
+class Verturbm(ArquivoSubmercado):
     """
     Armazena os dados das saídas referentes às energias
-    afluentes, por REE.
+    vertidas, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `eaf00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `vertub00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
-        REE,
-        EafsAnos,
+        Submercado,
+        VertAnos,
     ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="eaf001.out") -> "Eaf":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="eaf001.out"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="verturbm001.out"
+    ) -> "Verturbm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/eafb.py` & `inewave-0.0.96/inewave/nwlistop/eafbm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,37 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
-from inewave.nwlistop.modelos.eafb import EafsAnos
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
+)
+from inewave.nwlistop.modelos.eafbm import EafsAnos
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
-class Eafb(ArquivoREE):
+class Eafbm(ArquivoSubmercado):
     """
     Armazena os dados das saídas referentes às energias
-    afluentes brutas, por REE.
+    afluentes brutas, por submercado em valores absolutos.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `eafb00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `eafbm00x.out`, onde x varia conforme o
+    submercado em questão.
 
     """
 
     BLOCKS = [
-        REE,
+        Submercado,
         EafsAnos,
     ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="eafb001.out") -> "Eafb":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="eafb001.out"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="eafbm001.out"
+    ) -> "Eafbm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/eafbsin.py` & `inewave-0.0.96/inewave/nwlistop/evertsin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-from inewave.nwlistop.modelos.eafbsin import EafsAnos
-
 from inewave.nwlistop.modelos.arquivos.arquivosin import (
     ArquivoSIN,
 )
+from inewave.nwlistop.modelos.evertsin import EvertAnos
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
-class EafbSIN(ArquivoSIN):
+class EvertSIN(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes à energia natural
-    afluente para o SIN.
+    Armazena os dados das saídas referentes ao vertimento de reservatórios
+    , para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `eafbsin.out`.
+    NWLISTOP e reproduzidas no `evertsin.out`.
+
     """
 
     BLOCKS = [
-        EafsAnos,
+        EvertAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="eafbsin.out"
-    ) -> "EafbSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="eafbsin.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="evertsin.out"
+    ) -> "EvertSIN":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/earmfpm.py` & `inewave-0.0.96/inewave/nwlistop/earmfm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from inewave.nwlistop.modelos.earmfpm import EarmsAnos
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
     ArquivoSubmercado,
 )
+from inewave.nwlistop.modelos.earmfm import EarmsAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Earmfpm(ArquivoSubmercado):
+
+class Earmfm(ArquivoSubmercado):
     """
     Armazena os dados das saídas referentes às energias
-    armazenadas finais, por submercado e em % da energia armazenável máxima.
+    armazenadas finais, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `earmfpm00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `earmfm00x.out`, onde x varia conforme o
     submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
         EarmsAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="earmfpm001.out"
-    ) -> "Earmfpm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="earmfpm001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="earmfm001.out"
+    ) -> "Earmfm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/evertm.py` & `inewave-0.0.96/inewave/nwlistop/earmfpsin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
-    ArquivoSubmercado,
+from inewave.nwlistop.modelos.earmfpsin import EarmsAnos
+
+from inewave.nwlistop.modelos.arquivos.arquivosin import (
+    ArquivoSIN,
 )
-from inewave.nwlistop.modelos.evertm import EvertAnos
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
-class Evertm(ArquivoSubmercado):
+class EarmfpSIN(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes ao vertimento de reservatórios
-    , por Submercado.
+    Armazena os dados das saídas referentes às energias
+    armazenadas finais para o SIN e em % da energia armazenável máxima.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `evertm00x.out`, onde x varia conforme o
-    Submercado em questão.
-
+    NWLISTOP e reproduzidas nos `earmfpsin.out`, onde x varia conforme o
+    submercado em questão.
     """
 
     BLOCKS = [
-        Submercado,
-        EvertAnos,
+        EarmsAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="evertm001.out"
-    ) -> "Evertm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="evertm001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="earmfpsin.out"
+    ) -> "EarmfpSIN":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/excessin.py` & `inewave-0.0.96/inewave/nwlistop/perdfsin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
-    ArquivoSINPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosin import (
+    ArquivoSIN,
 )
-from inewave.nwlistop.modelos.exces import ExcesAnos
+from inewave.nwlistop.modelos.perdfsin import PerdfAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class ExcesSIN(ArquivoSINPatamar):
+
+class PerdfSIN(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes ao excesso de energia
-    por patamar, para o SIN.
+    Armazena os dados das saídas referentes ao vertimento fio d'água
+    , para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas no `excessin.out`
+    NWLISTOP e reproduzidas no `perdfsin.out`.
 
     """
 
     BLOCKS = [
-        ExcesAnos,
+        PerdfAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="excessin.out"
-    ) -> "ExcesSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="excessin.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="perdfsin.out"
+    ) -> "PerdfSIN":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/fteolsin.py` & `inewave-0.0.96/inewave/nwlistop/vevmin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
-    ArquivoSINPatamar,
-)
-from inewave.nwlistop.modelos.exces import ExcesAnos
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
+from inewave.nwlistop.modelos.vevmin import VevminAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class FteolSIN(ArquivoSINPatamar):
+
+class Vevmin(ArquivoREE):
     """
-    Armazena os dados das saídas referentes à folga da variável de
-    geração eólica para o SIN.
+    Armazena os dados das saídas referentes às violações da meta
+    de energia da vazão mínima, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas no `fteolsin.out`
+    NWLISTOP e reproduzidas nos `vevmin00x.out`, onde x varia conforme o
+    REE em questão.
 
     """
 
     BLOCKS = [
-        ExcesAnos,
+        REE,
+        VevminAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="fteolsin.out"
-    ) -> "FteolSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="fteolsin.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="vevmin001.out"
+    ) -> "Vevmin":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/geol.py` & `inewave-0.0.96/inewave/nwlistop/ghiduh.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.geol import GEAnos
+from inewave.nwlistop.modelos.ghiduh import GhidAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Geol(ArquivoUsinaPatamar):
+
+class GhidUH(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à geração eólica total
-    por patamar, por usina.
+    Armazena os dados das saídas referentes à geração hidráulica por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `geol00x.out`, onde x varia conforme o
-    PEE em questão.
+    NWLISTOP e reproduzidas nos `ghiduh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        GEAnos,
+        GhidAnos,
     ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="geol001.out") -> "Geol":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="geol001.out"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="ghiduh001.out"
+    ) -> "GhidUH":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/ghiduh.py` & `inewave-0.0.96/inewave/nwlistop/geol.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.ghiduh import GhidAnos
+from inewave.nwlistop.modelos.geol import GEAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class GhidUH(ArquivoUsinaPatamar):
+
+class Geol(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidráulica por usina.
+    Armazena os dados das saídas referentes à geração eólica total
+    por patamar, por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghiduh00x.out`, onde x varia conforme a
-    usina em questão.
+    NWLISTOP e reproduzidas nos `geol00x.out`, onde x varia conforme o
+    PEE em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        GhidAnos,
+        GEAnos,
     ]
 
     @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghiduh001.out"
-    ) -> "GhidUH":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghiduh001.out"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(cls, diretorio: str, nome_arquivo="geol001.out") -> "Geol":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/ghmax.py` & `inewave-0.0.96/inewave/nwlistop/geolsin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
-    ArquivoREEPatamar,
+from inewave.nwlistop.modelos.geolsin import GEAnos
+
+from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
+    ArquivoSINPatamar,
 )
-from inewave.nwlistop.modelos.ghmax import GHAnos
+
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
-class Ghmax(ArquivoREEPatamar):
+class GeolSIN(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidraulica máxima
-    por patamar, por REE.
+    Armazena os dados das saídas referentes à geração eólica total
+    para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghmax00x.out`, onde x varia conforme o
-    REE em questão.
-
+    NWLISTOP e reproduzidas nos `geolsin.out`.
     """
 
     BLOCKS = [
-        REE,
-        GHAnos,
+        GEAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghmax001.out"
-    ) -> "Ghmax":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghmax001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="geolsin.out"
+    ) -> "GeolSIN":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/ghmaxm.py` & `inewave-0.0.96/inewave/nwlistop/vevminm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
-    ArquivoSubmercadoPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.ghmaxm import GHAnos
+from inewave.nwlistop.modelos.vevminm import VevminAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Ghmaxm(ArquivoSubmercadoPatamar):
+
+class Vevminm(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes à geração hidraulica máxima
-    por patamar, por Submercado.
+    Armazena os dados das saídas referentes às violações da meta
+    de energia da vazão mínima, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghmax00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `vevminm00x.out`, onde x varia conforme o
     Submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        GHAnos,
+        VevminAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghmaxm001.out"
-    ) -> "Ghmaxm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghmaxm001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="vevminm001.out"
+    ) -> "Vevminm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/ghmaxmr.py` & `inewave-0.0.96/inewave/nwlistop/ghtotm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
     ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.ghmaxmr import GHAnos
+from inewave.nwlistop.modelos.ghtotm import GHAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Ghmaxmr(ArquivoSubmercadoPatamar):
+
+class Ghtotm(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidraulica máxima
-    considerando restrições elétricas por patamar, por Submercado.
+    Armazena os dados das saídas referentes à geração hidraulica total
+    por patamar, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghmaxmr00x.out`, onde x varia conforme o
-    Submercado em questão.
+    NWLISTOP e reproduzidas nos `ghtotm00x.out`, onde x varia conforme o
+    submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
         GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghmaxmr001.out"
-    ) -> "Ghmaxmr":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghmaxmr001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="ghtotm001.out"
+    ) -> "Ghtotm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/ghmaxr.py` & `inewave-0.0.96/inewave/nwlistop/vento.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
-    ArquivoREEPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousina import (
+    ArquivoUsina,
 )
-from inewave.nwlistop.modelos.ghmaxr import GHAnos
+from inewave.nwlistop.modelos.vento import VentoAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Ghmaxr(ArquivoREEPatamar):
+
+class Vento(ArquivoUsina):
     """
-    Armazena os dados das saídas referentes à geração hidraulica máxima
-    considerando restrições elétricas por patamar, por REE.
+    Armazena os dados das saídas referentes às velocidades do
+    vento por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghmax00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `vento00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
-        REE,
-        GHAnos,
+        Usina,
+        VentoAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghmaxr001.out"
-    ) -> "Ghmaxr":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghmaxr001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="vento001.out"
+    ) -> "Vento":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/ghmaxrsin.py` & `inewave-0.0.96/inewave/nwlistop/perdfm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,37 @@
-from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
-    ArquivoSINPatamar,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.ghmaxrsin import GHAnos
+from inewave.nwlistop.modelos.perdfm import PerdfAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class GhmaxrSIN(ArquivoSINPatamar):
+
+class Perdfm(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes à geração hidraulica máxima
-    considerando restrições elétricas por patamar para o SIN.
+    Armazena os dados das saídas referentes ao vertimento fio d'água
+    , por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghmaxsin.out`.
+    NWLISTOP e reproduzidas nos `perdfm00x.out`, onde x varia conforme o
+    Submercado em questão.
+
     """
 
     BLOCKS = [
-        GHAnos,
+        Submercado,
+        PerdfAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghmaxrsin.out"
-    ) -> "GhmaxrSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghmaxrsin.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="perdfm001.out"
+    ) -> "Perdfm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/ghmaxsin.py` & `inewave-0.0.96/inewave/nwlistop/vghminsin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
     ArquivoSINPatamar,
 )
-from inewave.nwlistop.modelos.ghmaxsin import GHAnos
+from inewave.nwlistop.modelos.vghmin import VghminAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class GhmaxSIN(ArquivoSINPatamar):
+
+class VghminSIN(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidraulica máxima
-    por patamar para o SIN.
+    Armazena os dados das saídas referentes à violação da meta de geração
+    hidraulica mínima por patamar, para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghmaxsin.out`.
+    NWLISTOP e reproduzidas no `vghminsin.out`.
+
     """
 
     BLOCKS = [
-        GHAnos,
+        VghminAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghmaxsin.out"
-    ) -> "GhmaxSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghmaxsin.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="vghminsin.out"
+    ) -> "VghminSIN":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/ghtot.py` & `inewave-0.0.96/inewave/nwlistop/ghmax.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
     ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.ghtot import GHAnos
+from inewave.nwlistop.modelos.ghmax import GHAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Ghtot(ArquivoREEPatamar):
+
+class Ghmax(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidraulica total
+    Armazena os dados das saídas referentes à geração hidraulica máxima
     por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghtot00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `ghmax00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
         GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghtot001.out"
-    ) -> "Ghtot":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghtot001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="ghmax001.out"
+    ) -> "Ghmax":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/ghtotm.py` & `inewave-0.0.96/inewave/nwlistop/geolm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
     ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.ghtotm import GHAnos
+from inewave.nwlistop.modelos.geolm import GEAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Ghtotm(ArquivoSubmercadoPatamar):
+
+class Geolm(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidraulica total
+    Armazena os dados das saídas referentes à geração eólica total
     por patamar, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghtotm00x.out`, onde x varia conforme o
-    submercado em questão.
+    NWLISTOP e reproduzidas nos `geol00x.out`, onde x varia conforme o
+    PEE em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        GHAnos,
+        GEAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghtotm001.out"
-    ) -> "Ghtotm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghtotm001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="geolm001.out"
+    ) -> "Geolm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/gttot.py` & `inewave-0.0.96/inewave/nwlistop/cterm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
-    ArquivoSubmercadoPatamar,
+from inewave.nwlistop.modelos.cterm import CtermsAnos
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.gttot import GTAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Gttot(ArquivoSubmercadoPatamar):
+
+class Cterm(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes à geração térmica total
-    por patamar, por REE.
+    Armazena os dados das saídas referentes aos custos de geração térmica
+    por patamar, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `gttot00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `cterm00x.out`, onde x varia conforme o
+    submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        GTAnos,
+        CtermsAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="gttot001.out"
-    ) -> "Gttot":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="gttot001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="cterm001.out"
+    ) -> "Cterm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/gttotsin.py` & `inewave-0.0.96/inewave/nwlistop/ghmaxsin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from inewave.nwlistop.modelos.gttotsin import GTAnos
 from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
     ArquivoSINPatamar,
 )
+from inewave.nwlistop.modelos.ghmaxsin import GHAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class GttotSIN(ArquivoSINPatamar):
+
+class GhmaxSIN(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes à geração térmica total
-    por patamar, para o SIN.
+    Armazena os dados das saídas referentes à geração hidraulica máxima
+    por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `gttotsin.out`.
+    NWLISTOP e reproduzidas nos `ghmaxsin.out`.
     """
 
     BLOCKS = [
-        GTAnos,
+        GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="gttotsin.out"
-    ) -> "GttotSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="gttotsin.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="ghmaxsin.out"
+    ) -> "GhmaxSIN":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/intercambio.py` & `inewave-0.0.96/inewave/nwlistop/dlpptbmaxm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from inewave.nwlistop.modelos.blocos.parsubmercados import ParSubmercados
-from inewave.nwlistop.modelos.arquivos.arquivoparsubmercadopatamar import (
-    ArquivoParSubmercadoPatamar,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
+    ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.intercambio import IntercambioAnos
+from inewave.nwlistop.modelos.dlppdfmax import DLPPdfmaxAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Intercambio(ArquivoParSubmercadoPatamar):
+
+class DLPPtbmaxm(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes ao intercâmbio
-    por patamar, por submercado.
+    Armazena os dados das saídas referentes à violação das restrições LPP
+    de turbinamento máximo por patamar, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `int00x00y.out`, onde x e y variam
-    conforme os submercados em questão.
+    NWLISTOP e reproduzidas nos `dlpptbmax00x.out`, onde x varia conforme o
+    Submercado em questão.
 
     """
 
     BLOCKS = [
-        ParSubmercados,
-        IntercambioAnos,
+        Submercado,
+        DLPPdfmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="int001002.out"
-    ) -> "Intercambio":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghtotm001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="dlpptbmaxm001.out"
+    ) -> "DLPPtbmaxm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/invade.py` & `inewave-0.0.96/inewave/nwlistop/vagua.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
-from inewave.nwlistop.modelos.invade import InvadeAnos
 
+from inewave.nwlistop.modelos.vagua import VAAnos
 
-class Invade(ArquivoREE):
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
+
+class Vagua(ArquivoREE):
     """
-    Armazena os dados das saídas referentes às violações da CAR
-    , por REE.
+    Armazena os dados das saídas referentes aos valores da água
+    por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `invade00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `vagua00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
-        InvadeAnos,
+        VAAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="invade001.out"
-    ) -> "Invade":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="invade001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="vagua001.out"
+    ) -> "Vagua":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/mediasmerc.py` & `inewave-0.0.96/inewave/nwlistop/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/mediassin.py` & `inewave-0.0.96/inewave/nwlistop/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py` & `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from inewave.nwlistop.modelos.blocos.parsubmercados import ParSubmercados
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
 from typing import Type, TypeVar, Optional
 
 
-class ArquivoParSubmercadoPatamar(BlockFile):
+class ArquivoSubmercadoPatamar(BlockFile):
     """
-    Armazena os dados das saídas por patamar, por par de submercados.
+    Armazena os dados das saídas por patamar, por submercado.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [ParSubmercados, ValoresSeriePatamar]
+    BLOCKS = [Submercado, ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoParSubmercadoPatamar":
+    ) -> "ArquivoSubmercadoPatamar":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
@@ -79,31 +79,18 @@
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
 
     @property
-    def submercado_de(self) -> Optional[str]:
+    def submercado(self) -> Optional[str]:
         """
-        O submercado de origem associado ao arquivo lido.
+        O submercado associado ao arquivo lido.
 
         :return: Os nome do submercado
         :rtype: str
         """
-        b = self.__bloco_por_tipo(ParSubmercados, 0)
+        b = self.__bloco_por_tipo(Submercado, 0)
         if b is not None:
-            return b.data[0]
-        return None
-
-    @property
-    def submercado_para(self) -> Optional[str]:
-        """
-        O submercado de destino associado ao arquivo lido.
-
-        :return: Os nome do submercado
-        :rtype: str
-        """
-        b = self.__bloco_por_tipo(ParSubmercados, 0)
-        if b is not None:
-            return b.data[1]
+            return b.data
         return None
```

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py` & `inewave-0.0.96/inewave/newave/caso.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,51 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
-    ValoresSeriePatamar,
-)
+from inewave.newave.modelos.caso import NomeCaso, CaminhoGerenciadorProcessos
 
-from cfinterface.files.blockfile import BlockFile
-import pandas as pd  # type: ignore
+from cfinterface.files.sectionfile import SectionFile
 from typing import Type, TypeVar, Optional
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class ArquivoREEPatamar(BlockFile):
+
+class Caso(SectionFile):
     """
-    Armazena os dados das saídas por patamar, por REE.
+    Armazena os dados de entrada do NEWAVE referentes às
+    configurações das usinas hidrelétricas.
+
+    Esta classe lida com informações de entrada fornecidas ao NEWAVE e
+    que podem ser modificadas através do arquivo `modif.dat`.
+
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [REE, ValoresSeriePatamar]
+    SECTIONS = [NomeCaso, CaminhoGerenciadorProcessos]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
-        self.__valores = None
 
     @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoREEPatamar":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(cls, diretorio: str, nome_arquivo="caso.dat") -> "Caso":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
+
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="caso.dat"):
+        msg = (
+            "O método escreve_arquivo(diretorio, nome_arquivo) será"
+            + " descontinuado na versão 1.0.0 -"
+            + " use o método write(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        self.write(join(diretorio, nome_arquivo))
 
     def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
         """
         Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
 
         :param bloco: Um tipo de bloco para ser lido
         :type bloco: T
@@ -46,51 +59,44 @@
                 b
                 for i, b in enumerate(self.data.of_type(bloco))
                 if i == indice
             )
         except StopIteration:
             return None
 
-    def __monta_tabela(self) -> pd.DataFrame:
-        df = None
-        for b in self.data.of_type(ValoresSeriePatamar):
-            dados = b.data
-            if dados is None:
-                continue
-            elif df is None:
-                df = b.data
-            else:
-                df = pd.concat([df, b.data], ignore_index=True)
-        return df
-
     @property
-    def valores(self) -> Optional[pd.DataFrame]:
+    def arquivos(self) -> Optional[str]:
         """
-        Tabela com os valores por patamar, por série e
-        por mês/ano de estudo.
+        Caminho para o arquivo `arquivos.dat` de entrada do NEWAVE.
 
-        - Ano (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
-
-        :return: A tabela dos valores por patamar.
-        :rtype: pd.DataFrame | None
-        """
-        if self.__valores is None:
-            self.__valores = self.__monta_tabela()
-        return self.__valores
+        :return: O caminho para o arquivo
+        :rtype: str | None
+        """
+        b = self.__bloco_por_tipo(NomeCaso, 0)
+        if b is not None:
+            return b.data
+        return None
+
+    @arquivos.setter
+    def arquivos(self, a: str):
+        b = self.__bloco_por_tipo(NomeCaso, 0)
+        if b is not None:
+            b.data = a
 
     @property
-    def ree(self) -> Optional[str]:
+    def gerenciador_processos(self) -> Optional[str]:
         """
-        O REE associado ao arquivo lido.
+        Caminho para o gerenciador de processos do NEWAVE.
 
-        :return: O nome do REE
-        :rtype: str
+        :return: O caminho para o arquivo
+        :rtype: str | None
         """
-        b = self.__bloco_por_tipo(REE, 0)
+        b = self.__bloco_por_tipo(CaminhoGerenciadorProcessos, 0)
         if b is not None:
             return b.data
         return None
+
+    @gerenciador_processos.setter
+    def gerenciador_processos(self, a: str):
+        b = self.__bloco_por_tipo(CaminhoGerenciadorProcessos, 0)
+        if b is not None:
+            b.data = a
```

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py` & `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/blocos/parsubmercados.py` & `inewave-0.0.96/inewave/nwlistop/modelos/blocos/parsubmercados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/blocos/ree.py` & `inewave-0.0.96/inewave/nwlistop/modelos/blocos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/blocos/submercado.py` & `inewave-0.0.96/inewave/nwlistop/modelos/blocos/submercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/blocos/usina.py` & `inewave-0.0.96/inewave/nwlistop/modelos/blocos/usina.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/blocos/valoresserie.py` & `inewave-0.0.96/inewave/nwlistop/modelos/blocos/valoresserie.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py` & `inewave-0.0.96/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/cdef.py` & `inewave-0.0.96/inewave/nwlistop/modelos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/cdefsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/cmarg.py` & `inewave-0.0.96/inewave/nwlistop/modelos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/cmargmed.py` & `inewave-0.0.96/inewave/nwlistop/modelos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/coper.py` & `inewave-0.0.96/inewave/nwlistop/modelos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/corteolm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/cterm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ctermsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/def.py` & `inewave-0.0.96/inewave/nwlistop/modelos/def.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/defsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/depminuh.py` & `inewave-0.0.96/inewave/nwlistop/modelos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/dflppdfmaxm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/dflppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/dflpptbmaxm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/dflpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/dfphauh.py` & `inewave-0.0.96/inewave/nwlistop/modelos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/dlppdfmax.py` & `inewave-0.0.96/inewave/nwlistop/modelos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/dlppdfmaxs.py` & `inewave-0.0.96/inewave/nwlistop/modelos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/dlpptbmax.py` & `inewave-0.0.96/inewave/nwlistop/modelos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/dlpptbmaxs.py` & `inewave-0.0.96/inewave/nwlistop/modelos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/dtbmax.py` & `inewave-0.0.96/inewave/nwlistop/modelos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/dtbmin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/dvazmax.py` & `inewave-0.0.96/inewave/nwlistop/modelos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/eaf.py` & `inewave-0.0.96/inewave/nwlistop/modelos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/eafb.py` & `inewave-0.0.96/inewave/nwlistop/modelos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/eafbm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/eafbsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/eafm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/earmf.py` & `inewave-0.0.96/inewave/nwlistop/modelos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/earmfm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/earmfp.py` & `inewave-0.0.96/inewave/nwlistop/modelos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/earmfpm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/earmfpsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/earmfsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/evert.py` & `inewave-0.0.96/inewave/nwlistop/modelos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/evertm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/evertsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/exces.py` & `inewave-0.0.96/inewave/nwlistop/modelos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/excessin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/fteolm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/fteolsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/geol.py` & `inewave-0.0.96/inewave/nwlistop/modelos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/geolm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/geolsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ghiduh.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ghmax.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ghmaxm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ghmaxmr.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ghmaxr.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ghmaxrsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ghmaxsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ghtot.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ghtotm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/ghtotsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/gttot.py` & `inewave-0.0.96/inewave/nwlistop/modelos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/gttotsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/intercambio.py` & `inewave-0.0.96/inewave/nwlistop/modelos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/invade.py` & `inewave-0.0.96/inewave/nwlistop/modelos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/invadem.py` & `inewave-0.0.96/inewave/nwlistop/modelos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/mediasmerc.py` & `inewave-0.0.96/inewave/nwlistop/modelos/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/mediassin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/mercl.py` & `inewave-0.0.96/inewave/nwlistop/modelos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/merclsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/perdf.py` & `inewave-0.0.96/inewave/nwlistop/modelos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/perdfm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/perdfsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/qafluh.py` & `inewave-0.0.96/inewave/nwlistop/modelos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/qincruh.py` & `inewave-0.0.96/inewave/nwlistop/modelos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/rhslppdf.py` & `inewave-0.0.96/inewave/nwlistop/modelos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/rhslpptb.py` & `inewave-0.0.96/inewave/nwlistop/modelos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vagua.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/varmpuh.py` & `inewave-0.0.96/inewave/nwlistop/modelos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/varmuh.py` & `inewave-0.0.96/inewave/nwlistop/modelos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vento.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vertuh.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/verturb.py` & `inewave-0.0.96/inewave/nwlistop/modelos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/verturbm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/verturbsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vevmin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vevminm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vevminsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vghmin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vghminm.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vghminsin.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vghminuh.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/modelos/vturuh.py` & `inewave-0.0.96/inewave/nwlistop/modelos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/inewave/nwlistop/perdfm.py` & `inewave-0.0.96/inewave/nwlistop/ghmaxmr.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
-    ArquivoSubmercado,
+from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
+    ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.perdfm import PerdfAnos
+from inewave.nwlistop.modelos.ghmaxmr import GHAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Perdfm(ArquivoSubmercado):
+
+class Ghmaxmr(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes ao vertimento fio d'água
-    , por Submercado.
+    Armazena os dados das saídas referentes à geração hidraulica máxima
+    considerando restrições elétricas por patamar, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `perdfm00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `ghmaxmr00x.out`, onde x varia conforme o
     Submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        PerdfAnos,
+        GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="perdfm001.out"
-    ) -> "Perdfm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="perdfm001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="ghmaxmr001.out"
+    ) -> "Ghmaxmr":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/qafluh.py` & `inewave-0.0.96/inewave/nwlistop/qafluh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousina import (
     ArquivoUsina,
 )
 from inewave.nwlistop.modelos.qafluh import QaflAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class QaflUH(ArquivoUsina):
     """
     Armazena os dados das saídas referentes às vazões afluentes por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `qafluh00x.out`, onde x varia conforme a
@@ -20,11 +24,13 @@
         QaflAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="qafluh001.out"
     ) -> "QaflUH":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="qafluh001.out"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/rhslppdf.py` & `inewave-0.0.96/inewave/nwlistop/evert.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
-    ArquivoREEPatamar,
-)
-from inewave.nwlistop.modelos.rhslppdf import RHSLPPdfAnos
+from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
+from inewave.nwlistop.modelos.evert import EvertAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class RHSLPPdf(ArquivoREEPatamar):
+
+class Evert(ArquivoREE):
     """
-    Armazena os dados das saídas referentes ao RHS das restrições LPP
-    de defluência máxima por patamar, por REE.
+    Armazena os dados das saídas referentes ao vertimento de reservatórios
+    , por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `rhslppdf00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `evert00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
-        RHSLPPdfAnos,
+        EvertAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="rhslppdf001.out"
-    ) -> "RHSLPPdf":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="rhslppdf001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="evert001.out"
+    ) -> "Evert":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/rhslpptb.py` & `inewave-0.0.96/inewave/nwlistop/dlppdfmaxs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
-    ArquivoREEPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
+    ArquivoSINPatamar,
 )
-from inewave.nwlistop.modelos.rhslpptb import RHSLPPtbAnos
+from inewave.nwlistop.modelos.dlppdfmaxs import DLPPdfmaxAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class RHSLPPtb(ArquivoREEPatamar):
+
+class DLPPdfmaxs(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes ao RHS das restrições LPP
-    de turbinamento máximo por patamar, por REE.
+    Armazena os dados das saídas referentes à violação das restrições
+    LPP de defluência máxima por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `rhslpptb00x.out`, onde x varia conforme o
-    REE em questão.
-
+    NWLISTOP e reproduzidas nos `dlppdfmaxs.out`.
     """
 
     BLOCKS = [
-        REE,
-        RHSLPPtbAnos,
+        DLPPdfmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="rhslpptb001.out"
-    ) -> "RHSLPPtb":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="rhslpptb001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="dlppdfmaxs.out"
+    ) -> "DLPPdfmaxs":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/vagua.py` & `inewave-0.0.96/inewave/nwlistop/eaf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
+from inewave.nwlistop.modelos.eaf import EafsAnos
 
-from inewave.nwlistop.modelos.vagua import VAAnos
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
 
-class Vagua(ArquivoREE):
+class Eaf(ArquivoREE):
     """
-    Armazena os dados das saídas referentes aos valores da água
-    por REE.
+    Armazena os dados das saídas referentes às energias
+    afluentes, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vagua00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `eaf00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
-        VAAnos,
+        EafsAnos,
     ]
 
     @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vagua001.out"
-    ) -> "Vagua":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vagua001.out"):
-        self.write(diretorio, nome_arquivo)
+    def le_arquivo(cls, diretorio: str, nome_arquivo="eaf001.out") -> "Eaf":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/vertuh.py` & `inewave-0.0.96/inewave/nwlistop/dtbmax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.vertuh import VertAnos
+from inewave.nwlistop.modelos.dtbmax import DtbmaxAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class VertUH(ArquivoUsinaPatamar):
+
+class Dtbmax(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes aos vertimentos por usina.
+    Armazena os dados das saídas referentes à violação de restrição de
+    turbinamento máximo por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vertuh00x.out`, onde x varia conforme a
-    usina em questão.
+    NWLISTOP e reproduzidas nos `dtbmax00x.out`, onde x varia conforme
+    a usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        VertAnos,
+        DtbmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vertuh001.out"
-    ) -> "VertUH":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vertuh001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="dtbmax001.out"
+    ) -> "Dtbmax":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/verturb.py` & `inewave-0.0.96/inewave/nwlistop/verturb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
 
 from inewave.nwlistop.modelos.verturb import VertAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Verturb(ArquivoREE):
     """
     Armazena os dados das saídas referentes às energias
     vertidas, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
@@ -20,11 +24,13 @@
         VertAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="verturb001.out"
     ) -> "Verturb":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="verturb001.out"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/vevmin.py` & `inewave-0.0.96/inewave/nwlistop/rhslppdf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
-from inewave.nwlistop.modelos.vevmin import VevminAnos
+from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
+    ArquivoREEPatamar,
+)
+from inewave.nwlistop.modelos.rhslppdf import RHSLPPdfAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Vevmin(ArquivoREE):
+
+class RHSLPPdf(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes às violações da meta
-    de energia da vazão mínima, por REE.
+    Armazena os dados das saídas referentes ao RHS das restrições LPP
+    de defluência máxima por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vevmin00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `rhslppdf00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
-        VevminAnos,
+        RHSLPPdfAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vevmin001.out"
-    ) -> "Vevmin":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vevmin001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="rhslppdf001.out"
+    ) -> "RHSLPPdf":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/vevminm.py` & `inewave-0.0.96/inewave/nwlistop/cmargmed.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
     ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.vevminm import VevminAnos
+from inewave.nwlistop.modelos.cmargmed import CmargsAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Vevminm(ArquivoSubmercado):
+
+class CmargMed(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes às violações da meta
-    de energia da vazão mínima, por Submercado.
+    Armazena os dados das saídas referentes aos custos marginais de operação
+    por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vevminm00x.out`, onde x varia conforme o
-    Submercado em questão.
+    NWLISTOP e reproduzidas nos `cmarg00x-med.out`, onde x varia conforme o
+    submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        VevminAnos,
+        CmargsAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vevminm001.out"
-    ) -> "Vevminm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vevminm001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="cmarg001-med.out"
+    ) -> "CmargMed":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/vevminsin.py` & `inewave-0.0.96/inewave/nwlistop/fteolsin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-from inewave.nwlistop.modelos.arquivos.arquivosin import (
-    ArquivoSIN,
+from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
+    ArquivoSINPatamar,
 )
-from inewave.nwlistop.modelos.vevminsin import VevminAnos
+from inewave.nwlistop.modelos.exces import ExcesAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class VevminSIN(ArquivoSIN):
+
+class FteolSIN(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes às violações da meta
-    de energia da vazão mínima para o SIN.
+    Armazena os dados das saídas referentes à folga da variável de
+    geração eólica para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vevminsin.out`
+    NWLISTOP e reproduzidas no `fteolsin.out`
 
     """
 
     BLOCKS = [
-        VevminAnos,
+        ExcesAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vevminsin.out"
-    ) -> "VevminSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vevminsin.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="fteolsin.out"
+    ) -> "FteolSIN":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/vghmin.py` & `inewave-0.0.96/inewave/nwlistop/vghmin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
     ArquivoREEPatamar,
 )
 from inewave.nwlistop.modelos.vghmin import VghminAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class Vghmin(ArquivoREEPatamar):
     """
     Armazena os dados das saídas referentes à violação da meta de geração
     hidraulica mínima por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
@@ -21,11 +25,13 @@
         VghminAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="vghmin001.out"
     ) -> "Vghmin":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vghmin001.out"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/vghminm.py` & `inewave-0.0.96/inewave/nwlistop/corteolm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
     ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.vghminm import VghminAnos
+from inewave.nwlistop.modelos.corteolm import CorteolmAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class Vghminm(ArquivoSubmercadoPatamar):
+
+class Corteolm(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes à violação da meta de geração
-    hidráulica mínima por patamar, por Submercado.
+    Armazena os dados das saídas referentes ao corte de geração eólica.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vghmin00x.out`, onde x varia conforme o
-    Submercado em questão.
+    NWLISTOP e reproduzidas nos `corteolm00x.out`, onde x varia conforme
+    a usina em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        VghminAnos,
+        CorteolmAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vghminm001.out"
-    ) -> "Vghminm":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vghminm001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="corteolm001.out"
+    ) -> "Corteolm":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/vghminuh.py` & `inewave-0.0.96/inewave/nwlistop/vghminuh.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
 from inewave.nwlistop.modelos.vghminuh import VGhminuhAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
+
 
 class VghminUH(ArquivoUsinaPatamar):
     """
     Armazena os dados das saídas referentes à violação da meta de
     geração hidráulica mínima por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
@@ -21,11 +25,13 @@
         VGhminuhAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="vghminuh001.out"
     ) -> "VghminUH":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vghminuh001.out"):
-        self.write(diretorio, nome_arquivo)
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave/nwlistop/vturuh.py` & `inewave-0.0.96/inewave/nwlistop/dfphauh.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.vturuh import VturAnos
+from inewave.nwlistop.modelos.dfphauh import DfphauhAnos
 
+# Para compatibilidade - até versão 1.0.0
+from os.path import join
+import warnings
 
-class VturUH(ArquivoUsinaPatamar):
+
+class Dfphauh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes às vazões turbinadas por usina.
+    Armazena os dados das saídas referentes à variável de folga da
+    FPHA da usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vturuh00x.out`, onde x varia conforme a
-    usina em questão.
+    NWLISTOP e reproduzidas nos `dfphauh00x.out`, onde x varia conforme
+    a usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        VturAnos,
+        DfphauhAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vturuh001.out"
-    ) -> "VturUH":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vturuh001.out"):
-        self.write(diretorio, nome_arquivo)
+        cls, diretorio: str, nome_arquivo="dfphauh001.out"
+    ) -> "Dfphauh":
+        msg = (
+            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
+            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
+        )
+        warnings.warn(msg, category=FutureWarning)
+        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.95/inewave.egg-info/PKG-INFO` & `inewave-0.0.96/inewave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 0.0.95
+Version: 0.0.96
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-0.0.95/inewave.egg-info/SOURCES.txt` & `inewave-0.0.96/inewave.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 inewave/newave/eolicageracao.py
 inewave/newave/eolicahistorico.py
 inewave/newave/eolicaposto.py
 inewave/newave/eolicasubmercado.py
 inewave/newave/exph.py
 inewave/newave/expt.py
 inewave/newave/forward.py
-inewave/newave/forwardh.py
+inewave/newave/forwarh.py
 inewave/newave/gee.py
 inewave/newave/ghmin.py
 inewave/newave/gtminpat.py
 inewave/newave/hidr.py
 inewave/newave/itaipu.py
 inewave/newave/manutt.py
 inewave/newave/modif.py
@@ -96,14 +96,15 @@
 inewave/newave/modelos/bid.py
 inewave/newave/modelos/cadic.py
 inewave/newave/modelos/caso.py
 inewave/newave/modelos/clasgas.py
 inewave/newave/modelos/clast.py
 inewave/newave/modelos/confhd.py
 inewave/newave/modelos/conft.py
+inewave/newave/modelos/cortes.py
 inewave/newave/modelos/cortesh.py
 inewave/newave/modelos/curva.py
 inewave/newave/modelos/cvar.py
 inewave/newave/modelos/dger.py
 inewave/newave/modelos/dsvagua.py
 inewave/newave/modelos/eafpast.py
 inewave/newave/modelos/elnino.py
@@ -119,14 +120,16 @@
 inewave/newave/modelos/eolicafte.py
 inewave/newave/modelos/eolicageracao.py
 inewave/newave/modelos/eolicahistorico.py
 inewave/newave/modelos/eolicaposto.py
 inewave/newave/modelos/eolicasubmercado.py
 inewave/newave/modelos/exph.py
 inewave/newave/modelos/expt.py
+inewave/newave/modelos/forward.py
+inewave/newave/modelos/forwarh.py
 inewave/newave/modelos/gee.py
 inewave/newave/modelos/ghmin.py
 inewave/newave/modelos/gtminpat.py
 inewave/newave/modelos/hidr.py
 inewave/newave/modelos/itaipu.py
 inewave/newave/modelos/manutt.py
 inewave/newave/modelos/modif.py
@@ -492,14 +495,16 @@
 tests/newave/test_avl_desvfpha_s.py
 tests/newave/test_avl_desvfpha_v_q.py
 tests/newave/test_cadic.py
 tests/newave/test_caso.py
 tests/newave/test_clast.py
 tests/newave/test_confhd.py
 tests/newave/test_conft.py
+tests/newave/test_cortes.py
+tests/newave/test_cortesh.py
 tests/newave/test_curva.py
 tests/newave/test_cvar.py
 tests/newave/test_dger.py
 tests/newave/test_dsvagua.py
 tests/newave/test_eafpast.py
 tests/newave/test_enavazb.py
 tests/newave/test_enavazf.py
@@ -511,14 +516,16 @@
 tests/newave/test_eolicaconfiguracao.py
 tests/newave/test_eolicafte.py
 tests/newave/test_eolicageracao.py
 tests/newave/test_eolicahistorico.py
 tests/newave/test_eolicaposto.py
 tests/newave/test_eolicasubmercado.py
 tests/newave/test_exph.py
+tests/newave/test_forward.py
+tests/newave/test_forwarh.py
 tests/newave/test_hidr.py
 tests/newave/test_modif.py
 tests/newave/test_newavetim.py
 tests/newave/test_nwv_avl_evap.py
 tests/newave/test_nwv_cortes_evap.py
 tests/newave/test_nwv_eco_evap.py
 tests/newave/test_parp.py
```

### Comparing `inewave-0.0.95/setup.py` & `inewave-0.0.96/setup.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/adterm.py` & `inewave-0.0.96/tests/mocks/arquivos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/arquivos.py` & `inewave-0.0.96/tests/mocks/arquivos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/avl_cortesfpha_nwv.py` & `inewave-0.0.96/tests/mocks/arquivos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/avl_desvfpha_s.py` & `inewave-0.0.96/tests/mocks/arquivos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/avl_desvfpha_v_q.py` & `inewave-0.0.96/tests/mocks/arquivos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/cadic.py` & `inewave-0.0.96/tests/mocks/arquivos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/cdef.py` & `inewave-0.0.96/tests/mocks/arquivos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/cdefsin.py` & `inewave-0.0.96/tests/mocks/arquivos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/clast.py` & `inewave-0.0.96/tests/mocks/arquivos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/cmarg.py` & `inewave-0.0.96/tests/mocks/arquivos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/cmargmed.py` & `inewave-0.0.96/tests/mocks/arquivos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/confhd.py` & `inewave-0.0.96/tests/mocks/arquivos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/conft.py` & `inewave-0.0.96/tests/mocks/arquivos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/coper.py` & `inewave-0.0.96/tests/mocks/arquivos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/corteolm.py` & `inewave-0.0.96/tests/mocks/arquivos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/cterm.py` & `inewave-0.0.96/tests/mocks/arquivos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ctermsin.py` & `inewave-0.0.96/tests/mocks/arquivos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/curva.py` & `inewave-0.0.96/tests/mocks/arquivos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/cvar.py` & `inewave-0.0.96/tests/mocks/arquivos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/deficit.py` & `inewave-0.0.96/tests/mocks/arquivos/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/defsin.py` & `inewave-0.0.96/tests/mocks/arquivos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/depminuh.py` & `inewave-0.0.96/tests/mocks/arquivos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dfphauh.py` & `inewave-0.0.96/tests/mocks/arquivos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dger.py` & `inewave-0.0.96/tests/mocks/arquivos/dger.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,9 +95,11 @@
     "REST.LPP TURB.MAX REE   1   (=0 NAO CONSIDERA , =1 CONSIDERA)\n",
     "REST.LPP DEFL.MAX REE   1   (=0 NAO CONSIDERA , =1 CONSIDERA)\n",
     "REST.LPP TURB.MAX UHE   1   (=0 NAO CONSIDERA , =1 CONSIDERA)\n",
     "REST.LPP DEFL.MAX UHE   1   (=0 NAO CONSIDERA , =1 CONSIDERA)\n",
     "REST.ELETRI ESPECIAIS   0   (=0 NAO CONSIDERA , =1 CONSIDERA)\n",
     "FUNCAO DE PROD. UHE     0   (0=FPHA, 1=LINEAR GH=rho*Q)\n",
     "FCF POS ESTUDO          0   (0=NAO, 1=SIM)\n",
+    "ESTACOES BOMBEAMENTO    1   (=0 NAO CONSIDERA , =1 CONSIDERA)\n",
+    "CANAL DE DESVIO         1   (=0 NAO CONSIDERA , =1 CONSIDERA)\n",
     "",
 ]
```

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dlppdfmax.py` & `inewave-0.0.96/tests/mocks/arquivos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dlppdfmaxm.py` & `inewave-0.0.96/tests/mocks/arquivos/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dlppdfmaxs.py` & `inewave-0.0.96/tests/mocks/arquivos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dlpptbmax.py` & `inewave-0.0.96/tests/mocks/arquivos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dlpptbmaxm.py` & `inewave-0.0.96/tests/mocks/arquivos/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dlpptbmaxs.py` & `inewave-0.0.96/tests/mocks/arquivos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dsvagua.py` & `inewave-0.0.96/tests/mocks/arquivos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dtbmax.py` & `inewave-0.0.96/tests/mocks/arquivos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dtbmin.py` & `inewave-0.0.96/tests/mocks/arquivos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/dvazmax.py` & `inewave-0.0.96/tests/mocks/arquivos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eaf.py` & `inewave-0.0.96/tests/mocks/arquivos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eafb.py` & `inewave-0.0.96/tests/mocks/arquivos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eafbm.py` & `inewave-0.0.96/tests/mocks/arquivos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eafbsin.py` & `inewave-0.0.96/tests/mocks/arquivos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eafm.py` & `inewave-0.0.96/tests/mocks/arquivos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eafpast.py` & `inewave-0.0.96/tests/mocks/arquivos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/earmf.py` & `inewave-0.0.96/tests/mocks/arquivos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/earmfm.py` & `inewave-0.0.96/tests/mocks/arquivos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/earmfp.py` & `inewave-0.0.96/tests/mocks/arquivos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/earmfpm.py` & `inewave-0.0.96/tests/mocks/arquivos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/earmfpsin.py` & `inewave-0.0.96/tests/mocks/arquivos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/earmfsin.py` & `inewave-0.0.96/tests/mocks/arquivos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eolicacadastro.py` & `inewave-0.0.96/tests/mocks/arquivos/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eolicaconfig.py` & `inewave-0.0.96/tests/mocks/arquivos/eolicaconfig.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eolicafte.py` & `inewave-0.0.96/tests/mocks/arquivos/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eolicageracao.py` & `inewave-0.0.96/tests/mocks/arquivos/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eolicahistorico.py` & `inewave-0.0.96/tests/mocks/arquivos/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/eolicaposto.py` & `inewave-0.0.96/tests/mocks/arquivos/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/estados.py` & `inewave-0.0.96/tests/mocks/arquivos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/evert.py` & `inewave-0.0.96/tests/mocks/arquivos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/evertm.py` & `inewave-0.0.96/tests/mocks/arquivos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/evertsin.py` & `inewave-0.0.96/tests/mocks/arquivos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/exces.py` & `inewave-0.0.96/tests/mocks/arquivos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/excessin.py` & `inewave-0.0.96/tests/mocks/arquivos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/exph.py` & `inewave-0.0.96/tests/mocks/arquivos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/fteolm.py` & `inewave-0.0.96/tests/mocks/arquivos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/fteolsin.py` & `inewave-0.0.96/tests/mocks/arquivos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/geol.py` & `inewave-0.0.96/tests/mocks/arquivos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/geolm.py` & `inewave-0.0.96/tests/mocks/arquivos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/geolsin.py` & `inewave-0.0.96/tests/mocks/arquivos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ghiduh.py` & `inewave-0.0.96/tests/mocks/arquivos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ghmax.py` & `inewave-0.0.96/tests/mocks/arquivos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ghmaxm.py` & `inewave-0.0.96/tests/mocks/arquivos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ghmaxmr.py` & `inewave-0.0.96/tests/mocks/arquivos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ghmaxr.py` & `inewave-0.0.96/tests/mocks/arquivos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ghmaxrsin.py` & `inewave-0.0.96/tests/mocks/arquivos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ghmaxsin.py` & `inewave-0.0.96/tests/mocks/arquivos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ghtot.py` & `inewave-0.0.96/tests/mocks/arquivos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ghtotm.py` & `inewave-0.0.96/tests/mocks/arquivos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ghtotsin.py` & `inewave-0.0.96/tests/mocks/arquivos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/gttot.py` & `inewave-0.0.96/tests/mocks/arquivos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/gttotsin.py` & `inewave-0.0.96/tests/mocks/arquivos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/intercambio.py` & `inewave-0.0.96/tests/mocks/arquivos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/invade.py` & `inewave-0.0.96/tests/mocks/arquivos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/invadem.py` & `inewave-0.0.96/tests/mocks/arquivos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/mercl.py` & `inewave-0.0.96/tests/mocks/arquivos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/merclsin.py` & `inewave-0.0.96/tests/mocks/arquivos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/modif.py` & `inewave-0.0.96/tests/mocks/arquivos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/newavetim.py` & `inewave-0.0.96/tests/mocks/arquivos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/nwlistcf.py` & `inewave-0.0.96/tests/mocks/arquivos/nwlistcf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/nwv_avl_evap.py` & `inewave-0.0.96/tests/mocks/arquivos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/nwv_cortes_evap.py` & `inewave-0.0.96/tests/mocks/arquivos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/nwv_eco_evap.py` & `inewave-0.0.96/tests/mocks/arquivos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/parp.py` & `inewave-0.0.96/tests/mocks/arquivos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/parpeol.py` & `inewave-0.0.96/tests/mocks/arquivos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/parpvaz.py` & `inewave-0.0.96/tests/mocks/arquivos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/patamar.py` & `inewave-0.0.96/tests/mocks/arquivos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/penalid.py` & `inewave-0.0.96/tests/mocks/arquivos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/perdf.py` & `inewave-0.0.96/tests/mocks/arquivos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/perdfm.py` & `inewave-0.0.96/tests/mocks/arquivos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/perdfsin.py` & `inewave-0.0.96/tests/mocks/arquivos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/pmo.py` & `inewave-0.0.96/tests/mocks/arquivos/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/qafluh.py` & `inewave-0.0.96/tests/mocks/arquivos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/qincruh.py` & `inewave-0.0.96/tests/mocks/arquivos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/re.py` & `inewave-0.0.96/tests/mocks/arquivos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/ree.py` & `inewave-0.0.96/tests/mocks/arquivos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/restricaoeletrica.py` & `inewave-0.0.96/tests/mocks/arquivos/restricaoeletrica.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/restricaoenergia.py` & `inewave-0.0.96/tests/mocks/arquivos/restricaoenergia.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/restricaovazao.py` & `inewave-0.0.96/tests/mocks/arquivos/restricaovazao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/rhslppdf.py` & `inewave-0.0.96/tests/mocks/arquivos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/rhslpptb.py` & `inewave-0.0.96/tests/mocks/arquivos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/sistema.py` & `inewave-0.0.96/tests/mocks/arquivos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/term.py` & `inewave-0.0.96/tests/mocks/arquivos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vagua.py` & `inewave-0.0.96/tests/mocks/arquivos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/varmpuh.py` & `inewave-0.0.96/tests/mocks/arquivos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/varmuh.py` & `inewave-0.0.96/tests/mocks/arquivos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vazpast.py` & `inewave-0.0.96/tests/mocks/arquivos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vento.py` & `inewave-0.0.96/tests/mocks/arquivos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vertuh.py` & `inewave-0.0.96/tests/mocks/arquivos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/verturb.py` & `inewave-0.0.96/tests/mocks/arquivos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/verturbm.py` & `inewave-0.0.96/tests/mocks/arquivos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/verturbsin.py` & `inewave-0.0.96/tests/mocks/arquivos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vevmin.py` & `inewave-0.0.96/tests/mocks/arquivos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vevminm.py` & `inewave-0.0.96/tests/mocks/arquivos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vevminsin.py` & `inewave-0.0.96/tests/mocks/arquivos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vghmin.py` & `inewave-0.0.96/tests/mocks/arquivos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vghminm.py` & `inewave-0.0.96/tests/mocks/arquivos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vghminsin.py` & `inewave-0.0.96/tests/mocks/arquivos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vghminuh.py` & `inewave-0.0.96/tests/mocks/arquivos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/arquivos/vturuh.py` & `inewave-0.0.96/tests/mocks/arquivos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/mocks/mock_open.py` & `inewave-0.0.96/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.95/tests/newave/test_adterm.py` & `inewave-0.0.96/tests/newave/test_adterm.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.adterm import MockBlocoUTEAdTerm
 
 
-def test_bloco_ute_adterm():
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
+def test_bloco_ute_adterm():
     m: MagicMock = mock_open(read_data="".join(MockBlocoUTEAdTerm))
     b = BlocoUTEAdTerm()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 6
@@ -20,51 +22,51 @@
     assert b.data.iloc[0, 3] == 230.70
     assert b.data.iloc[-1, -1] == 0.00
 
 
 def test_atributos_encontrados_adterm():
     m: MagicMock = mock_open(read_data="".join(MockBlocoUTEAdTerm))
     with patch("builtins.open", m):
-        ad = AdTerm.le_arquivo("")
+        ad = AdTerm.read(ARQ_TESTE)
         assert ad.despachos is not None
 
 
 def test_atributos_nao_encontrados_adterm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = AdTerm.le_arquivo("")
+        ad = AdTerm.read(ARQ_TESTE)
         assert ad.despachos is None
 
 
 def test_eq_adterm():
     m: MagicMock = mock_open(read_data="".join(MockBlocoUTEAdTerm))
     with patch("builtins.open", m):
-        ad1 = AdTerm.le_arquivo("")
-        ad2 = AdTerm.le_arquivo("")
+        ad1 = AdTerm.read(ARQ_TESTE)
+        ad2 = AdTerm.read(ARQ_TESTE)
         assert ad1 == ad2
 
 
 def test_neq_adterm():
     m: MagicMock = mock_open(read_data="".join(MockBlocoUTEAdTerm))
     with patch("builtins.open", m):
-        ad1 = AdTerm.le_arquivo("")
-        ad2 = AdTerm.le_arquivo("")
+        ad1 = AdTerm.read(ARQ_TESTE)
+        ad2 = AdTerm.read(ARQ_TESTE)
         ad2.despachos.iloc[0, 0] = -1
         assert ad1 != ad2
 
 
 def test_leitura_escrita_adterm():
     m_leitura: MagicMock = mock_open(read_data="".join(MockBlocoUTEAdTerm))
     with patch("builtins.open", m_leitura):
-        ad1 = AdTerm.le_arquivo("")
+        ad1 = AdTerm.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        ad1.escreve_arquivo("", "")
+        ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        ad2 = AdTerm.le_arquivo("")
+        ad2 = AdTerm.read(ARQ_TESTE)
         assert ad1 == ad2
```

### Comparing `inewave-0.0.95/tests/newave/test_arquivos.py` & `inewave-0.0.96/tests/newave/test_arquivos.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from inewave.newave import Arquivos
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.arquivos import MockArquivos
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_nomes_arquivos():
 
+def test_bloco_nomes_arquivos():
     m: MagicMock = mock_open(read_data="".join(MockArquivos))
     b = BlocoNomesArquivos()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 44
@@ -20,15 +21,15 @@
     assert b.data.iloc[0, 1] == "dger.dat"
     assert b.data.iloc[-1, 1] == "cortesh-pos.dat"
 
 
 def test_atributos_encontrados_arquivos():
     m: MagicMock = mock_open(read_data="".join(MockArquivos))
     with patch("builtins.open", m):
-        ad = Arquivos.le_arquivo("")
+        ad = Arquivos.read(ARQ_TESTE)
         assert ad.dger is not None
         assert ad.sistema is not None
         assert ad.confhd is not None
         assert ad.modif is not None
         assert ad.conft is not None
         assert ad.term is not None
         assert ad.clast is not None
@@ -70,15 +71,15 @@
         assert ad.cortes_pos_estudo is not None
         assert ad.cortesh_pos_estudo is not None
 
 
 def test_atributos_nao_encontrados_arquivos():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = Arquivos.le_arquivo("")
+        ad = Arquivos.read(ARQ_TESTE)
         assert ad.dger is None
         assert ad.sistema is None
         assert ad.confhd is None
         assert ad.modif is None
         assert ad.conft is None
         assert ad.term is None
         assert ad.clast is None
@@ -120,37 +121,37 @@
         assert ad.cortes_pos_estudo is None
         assert ad.cortesh_pos_estudo is None
 
 
 def test_eq_arquivos():
     m: MagicMock = mock_open(read_data="".join(MockArquivos))
     with patch("builtins.open", m):
-        ad1 = Arquivos.le_arquivo("")
-        ad2 = Arquivos.le_arquivo("")
+        ad1 = Arquivos.read(ARQ_TESTE)
+        ad2 = Arquivos.read(ARQ_TESTE)
         assert ad1 == ad2
 
 
 def test_neq_arquivos():
     m: MagicMock = mock_open(read_data="".join(MockArquivos))
     with patch("builtins.open", m):
-        ad1 = Arquivos.le_arquivo("")
-        ad2 = Arquivos.le_arquivo("")
+        ad1 = Arquivos.read(ARQ_TESTE)
+        ad2 = Arquivos.read(ARQ_TESTE)
         ad2.dger = "teste"
         assert ad1 != ad2
 
 
 def test_leitura_escrita_arquivos():
     m_leitura: MagicMock = mock_open(read_data="".join(MockArquivos))
     with patch("builtins.open", m_leitura):
-        ad1 = Arquivos.le_arquivo("")
+        ad1 = Arquivos.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        ad1.escreve_arquivo("", "")
+        ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        ad2 = Arquivos.le_arquivo("")
+        ad2 = Arquivos.read(ARQ_TESTE)
         assert ad1 == ad2
```

### Comparing `inewave-0.0.95/tests/newave/test_avl_cortesfpha_nwv.py` & `inewave-0.0.96/tests/newave/test_avl_cortesfpha_nwv.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from inewave.newave.avl_cortesfpha_nwv import AvlCortesFpha
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.avl_cortesfpha_nwv import MockAvlCortesFphaNwv
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_avl_nwv_cortesfpha_nwv():
     m: MagicMock = mock_open(read_data="".join(MockAvlCortesFphaNwv))
     with patch("builtins.open", m):
-        rel = AvlCortesFpha.le_arquivo("")
+        rel = AvlCortesFpha.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
         assert rel.tabela.at[0, "indice_usina"] == 4
         assert rel.tabela.at[0, "periodo"] == 1
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert rel.tabela.at[0, "indice_corte"] == 1
         assert rel.tabela.at[0, "fator_correcao"] == 1.0
         assert rel.tabela.at[0, "rhs_energia"] == 0.0
@@ -25,19 +27,19 @@
         assert rel.tabela.at[0, "coeficiente_vazao_vertida_MW_m3s"] == 0.0
         assert rel.tabela.at[0, "coeficiente_vazao_lateral_MW_m3s"] == 0.0
 
 
 def test_eq_avl_nwv_cortesfpha_nwv():
     m: MagicMock = mock_open(read_data="".join(MockAvlCortesFphaNwv))
     with patch("builtins.open", m):
-        rel1 = AvlCortesFpha.le_arquivo("")
-        rel2 = AvlCortesFpha.le_arquivo("")
+        rel1 = AvlCortesFpha.read(ARQ_TESTE)
+        rel2 = AvlCortesFpha.read(ARQ_TESTE)
         assert rel1 == rel2
 
 
 def test_neq_avl_nwv_cortesfpha_nwv():
     m: MagicMock = mock_open(read_data="".join(MockAvlCortesFphaNwv))
     with patch("builtins.open", m):
-        rel1 = AvlCortesFpha.le_arquivo("")
-        rel2 = AvlCortesFpha.le_arquivo("")
+        rel1 = AvlCortesFpha.read(ARQ_TESTE)
+        rel2 = AvlCortesFpha.read(ARQ_TESTE)
         rel1.tabela.iloc[0, 0] = -1
         assert rel1 != rel2
```

### Comparing `inewave-0.0.95/tests/newave/test_avl_desvfpha_s.py` & `inewave-0.0.96/tests/newave/test_avl_desvfpha_s.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.newave.avl_desvfpha_s import AvlDesvFphaS
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.avl_desvfpha_s import MockAvlDesvFphaS
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_avl_desvfpha_s():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvFphaS))
     with patch("builtins.open", m):
-        rel = AvlDesvFphaS.le_arquivo("")
+        rel = AvlDesvFphaS.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
         assert rel.tabela.at[0, "indice_usina"] == 4
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert rel.tabela.at[0, "volume_armazenado_percentual"] == 100.0
         assert rel.tabela.at[0, "vazao_turbinada_m3s"] == 0.0
         assert rel.tabela.at[0, "vazao_vertida_m3s"] == 0.0
         assert rel.tabela.at[0, "desvio_percentual"] == 0.0
 
 
 def test_eq_avl_desvfpha_s():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvFphaS))
     with patch("builtins.open", m):
-        rel1 = AvlDesvFphaS.le_arquivo("")
-        rel2 = AvlDesvFphaS.le_arquivo("")
+        rel1 = AvlDesvFphaS.read(ARQ_TESTE)
+        rel2 = AvlDesvFphaS.read(ARQ_TESTE)
         assert rel1 == rel2
 
 
 ## Não precisa comparar isto, é somente leitura - passa por agregação
 # def test_neq_avl_desvfpha_s():
 #     m: MagicMock = mock_open(read_data="".join(MockAvlDesvFphaS))
 #     with patch("builtins.open", m):
-#         rel1 = AvlDesvFphaS.le_arquivo("")
-#         rel2 = AvlDesvFphaS.le_arquivo("")
+#         rel1 = AvlDesvFphaS.read(ARQ_TESTE)
+#         rel2 = AvlDesvFphaS.read(ARQ_TESTE)
 #         rel1.tabela.iloc[0, 0] = -1
 #         assert rel1 != rel2
```

### Comparing `inewave-0.0.95/tests/newave/test_avl_desvfpha_v_q.py` & `inewave-0.0.96/tests/newave/test_avl_desvfpha_v_q.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from inewave.newave.avl_desvfpha_v_q import AvlDesvFphaVQ
 import pandas as pd  # type: ignore
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.avl_desvfpha_v_q import MockAvlDesvFphaVQ
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_avl_desvfpha_v_q():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvFphaVQ))
     with patch("builtins.open", m):
-        rel = AvlDesvFphaVQ.le_arquivo("")
+        rel = AvlDesvFphaVQ.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
         assert rel.tabela.at[0, "indice_usina"] == 4
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert pd.isna(rel.tabela.at[0, "volume_armazenado_percentual"])
         assert rel.tabela.at[0, "vazao_turbinada_m3s"] == 0.0
         assert rel.tabela.at[0, "desvio_percentual"] == 0.0
 
 
 def test_eq_avl_desvfpha_v_q():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvFphaVQ))
     with patch("builtins.open", m):
-        rel1 = AvlDesvFphaVQ.le_arquivo("")
-        rel2 = AvlDesvFphaVQ.le_arquivo("")
+        rel1 = AvlDesvFphaVQ.read(ARQ_TESTE)
+        rel2 = AvlDesvFphaVQ.read(ARQ_TESTE)
         assert rel1 == rel2
 
 
 ## Não precisa comparar isto, é somente leitura - passa por agregação
 # def test_neq_avl_desvfpha_v_q():
 #     m: MagicMock = mock_open(read_data="".join(MockAvlDesvFphaVQ))
 #     with patch("builtins.open", m):
-#         rel1 = AvlDesvFphaVQ.le_arquivo("")
-#         rel2 = AvlDesvFphaVQ.le_arquivo("")
+#         rel1 = AvlDesvFphaVQ.read(ARQ_TESTE)
+#         rel2 = AvlDesvFphaVQ.read(ARQ_TESTE)
 #         rel1.tabela.iloc[0, 0] = -1
 #         assert rel1 != rel2
```

### Comparing `inewave-0.0.95/tests/newave/test_cadic.py` & `inewave-0.0.96/tests/newave/test_cadic.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.cadic import MockBlocoCargasAdicionais
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_ute_cadic():
 
+def test_bloco_ute_cadic():
     m: MagicMock = mock_open(read_data="".join(MockBlocoCargasAdicionais))
     b = BlocoCargasAdicionais()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 12
@@ -22,53 +23,53 @@
     assert b.data.iloc[0, 2] == "CONS.ITAIPU"
     assert b.data.iloc[-1, -1] == 2246
 
 
 def test_atributos_encontrados_cadic():
     m: MagicMock = mock_open(read_data="".join(MockBlocoCargasAdicionais))
     with patch("builtins.open", m):
-        ad = CAdic.le_arquivo("")
+        ad = CAdic.read(ARQ_TESTE)
         assert ad.cargas is not None
 
 
 def test_atributos_nao_encontrados_cadic():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = CAdic.le_arquivo("")
+        ad = CAdic.read(ARQ_TESTE)
         assert ad.cargas is None
 
 
 def test_eq_cadic():
     m: MagicMock = mock_open(read_data="".join(MockBlocoCargasAdicionais))
     with patch("builtins.open", m):
-        ad1 = CAdic.le_arquivo("")
-        ad2 = CAdic.le_arquivo("")
+        ad1 = CAdic.read(ARQ_TESTE)
+        ad2 = CAdic.read(ARQ_TESTE)
         assert ad1 == ad2
 
 
 def test_neq_cadic():
     m: MagicMock = mock_open(read_data="".join(MockBlocoCargasAdicionais))
     with patch("builtins.open", m):
-        ad1 = CAdic.le_arquivo("")
-        ad2 = CAdic.le_arquivo("")
+        ad1 = CAdic.read(ARQ_TESTE)
+        ad2 = CAdic.read(ARQ_TESTE)
         ad2.cargas.iloc[0, 0] = -1
         assert ad1 != ad2
 
 
 def test_leitura_escrita_cadic():
     m_leitura: MagicMock = mock_open(
         read_data="".join(MockBlocoCargasAdicionais)
     )
     with patch("builtins.open", m_leitura):
-        ad1 = CAdic.le_arquivo("")
+        ad1 = CAdic.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        ad1.escreve_arquivo("", "")
+        ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        ad2 = CAdic.le_arquivo("")
+        ad2 = CAdic.read(ARQ_TESTE)
         assert ad1 == ad2
```

### Comparing `inewave-0.0.95/tests/newave/test_caso.py` & `inewave-0.0.96/tests/newave/test_re.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,94 @@
-from inewave.newave.modelos.caso import NomeCaso, CaminhoGerenciadorProcessos
-from inewave.newave import Caso
+# Rotinas de testes associadas ao arquivo re.dat do NEWAVE
+from inewave.newave.modelos.re import (
+    BlocoUsinasConjuntoRE,
+    BlocoConfiguracaoRestricoesRE,
+)
+
+from inewave.newave import RE
+
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.caso import (
-    MockNomeCaso,
-    MockCaminhoGerenciador,
-    MockCaso,
+from tests.mocks.arquivos.re import (
+    MockBlocoUsinasRestricoes,
+    MockBlocoRestricoes,
+    MockRE,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_nome_caso():
 
-    m: MagicMock = mock_open(read_data="".join(MockNomeCaso))
-    b = NomeCaso()
+def test_bloco_usinas_conjuntos_re():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoUsinasRestricoes))
+    b = BlocoUsinasConjuntoRE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
-    assert b.data == "arquivos.dat"
-
+    assert b.data.iloc[0, 0] == 1
+    assert b.data.iloc[-1, 0] == 10
+    assert b.data.iloc[-1, 2] == 284
 
-def test_bloco_caminho_gerenciador_caso():
 
-    m: MagicMock = mock_open(read_data="".join(MockCaminhoGerenciador))
-    b = CaminhoGerenciadorProcessos()
+def test_bloco_restricoes_re():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoRestricoes))
+    b = BlocoConfiguracaoRestricoesRE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
-    assert b.data == "/home/newave/"
+    assert b.data.iloc[0, 0] == 1
+    assert b.data.iloc[-1, 0] == 10
+    assert b.data.iloc[-1, -1] == "C. CALDEIRAO E F. GOMES"
 
 
-def test_atributos_encontrados_caso():
-    m: MagicMock = mock_open(read_data="".join(MockCaso))
+def test_atributos_encontrados_re():
+    m: MagicMock = mock_open(read_data="".join(MockRE))
     with patch("builtins.open", m):
-        ad = Caso.le_arquivo("")
-        assert ad.arquivos is not None
-        assert ad.gerenciador_processos is not None
+        ad = RE.read(ARQ_TESTE)
+        assert ad.usinas_conjuntos is not None
+        assert ad.restricoes is not None
 
 
-def test_atributos_nao_encontrados_caso():
+def test_atributos_nao_encontrados_re():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = Caso.le_arquivo("")
-        assert ad.arquivos == ""
-        assert ad.gerenciador_processos == ""
+        ad = RE.read(ARQ_TESTE)
+        assert ad.usinas_conjuntos is None
+        assert ad.restricoes is None
 
 
-def test_eq_caso():
-    m: MagicMock = mock_open(read_data="".join(MockCaso))
+def test_eq_re():
+    m: MagicMock = mock_open(read_data="".join(MockRE))
     with patch("builtins.open", m):
-        ad1 = Caso.le_arquivo("")
-        ad2 = Caso.le_arquivo("")
-        assert ad1 == ad2
+        cf1 = RE.read(ARQ_TESTE)
+        cf2 = RE.read(ARQ_TESTE)
+        assert cf1 == cf2
 
 
-def test_neq_caso():
-    m: MagicMock = mock_open(read_data="".join(MockCaso))
+def test_neq_re():
+    m: MagicMock = mock_open(read_data="".join(MockRE))
     with patch("builtins.open", m):
-        ad1 = Caso.le_arquivo("")
-        ad2 = Caso.le_arquivo("")
-        ad2.gerenciador_processos = "/bin"
-        assert ad1 != ad2
+        cf1 = RE.read(ARQ_TESTE)
+        cf2 = RE.read(ARQ_TESTE)
+        cf2.usinas_conjuntos.loc[0, 0] = 0
+        assert cf1 != cf2
 
 
-def test_leitura_escrita_caso():
-    m_leitura: MagicMock = mock_open(read_data="".join(MockCaso))
+def test_leitura_escrita_re():
+    m_leitura: MagicMock = mock_open(read_data="".join(MockRE))
     with patch("builtins.open", m_leitura):
-        ad1 = Caso.le_arquivo("")
+        cf1 = RE.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        ad1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        ad2 = Caso.le_arquivo("")
-        assert ad1 == ad2
+        cf2 = RE.read(ARQ_TESTE)
+        assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_clast.py` & `inewave-0.0.96/tests/newave/test_exph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,98 +1,80 @@
-# Rotinas de testes associadas ao arquivo clast.dat do NEWAVE
-from inewave.newave.modelos.clast import BlocoUTEClasT
-from inewave.newave.modelos.clast import BlocoModificacaoUTEClasT
-
-from inewave.newave import ClasT
-
+from datetime import datetime
+from inewave.newave.modelos.exph import BlocoUHEExph
+from inewave.newave import Exph
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.clast import MockBlocoUTEClasT
-from tests.mocks.arquivos.clast import MockBlocoModificacaoClasT
-from tests.mocks.arquivos.clast import MockClasT
-
-
-def test_bloco_ute_clast():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoUTEClasT))
-    b = BlocoUTEClasT()
-    with patch("builtins.open", m):
-        with open("", "") as fp:
-            b.read(fp)
-
-    assert b.data.iloc[0, 0] == 1
-    assert b.data.iloc[-1, -1] == 0.0
-
-
-def test_atributos_encontrados_ute_clast():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoUTEClasT))
-    with patch("builtins.open", m):
-        ct = ClasT.le_arquivo("")
-        assert ct.usinas is not None
+from tests.mocks.arquivos.exph import MockExph
 
-
-def test_atributos_nao_encontrados_ute_clast():
-    m: MagicMock = mock_open(read_data="")
-    with patch("builtins.open", m):
-        ct = ClasT.le_arquivo("")
-        assert ct.usinas is None
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_bloco_modificacao_clast():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoModificacaoClasT))
-    b = BlocoModificacaoUTEClasT()
+def test_bloco_uhe_exph():
+    m: MagicMock = mock_open(read_data="".join(MockExph))
+    b = BlocoUHEExph()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
-    assert b.data.iloc[0, 0] == 211
-    assert b.data.iloc[-1, -1] == "PORTO ITAQUI"
+    assert b.data.shape[0] == 7
+    assert b.data.shape[1] == 9
+    assert b.data.iloc[0, 0] == 309
+    assert b.data.iloc[0, 1] == "JURUENA"
+    assert b.data.iloc[0, 2] == datetime(2024, 10, 1)
+    assert b.data.iloc[0, 3] == 3
+    assert b.data.iloc[0, 4] == 0.0
+    assert b.data.iloc[1, 5] == datetime(2025, 1, 1)
+    assert b.data.iloc[1, 6] == 25.0
+    assert b.data.iloc[1, 7] == 1
+    assert b.data.iloc[1, 8] == 1
+    assert b.data.iloc[-1, -1] == 3
 
 
-def test_atributos_encontrados_modificacao_clast():
-    m: MagicMock = mock_open(read_data="".join(MockClasT))
+def test_atributos_encontrados_exph():
+    m: MagicMock = mock_open(read_data="".join(MockExph))
     with patch("builtins.open", m):
-        ct = ClasT.le_arquivo("")
-        assert ct.modificacoes is not None
+        ad = Exph.read(ARQ_TESTE)
+        assert ad.expansoes is not None
 
 
-def test_atributos_nao_encontrados_modificacao_clast():
+def test_atributos_nao_encontrados_exph():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ct = ClasT.le_arquivo("")
-        assert ct.modificacoes is None
+        ad = Exph.read(ARQ_TESTE)
+        assert ad.expansoes is None
 
 
-def test_eq_clast():
-    m: MagicMock = mock_open(read_data="".join(MockClasT))
+def test_eq_exph():
+    m: MagicMock = mock_open(read_data="".join(MockExph))
     with patch("builtins.open", m):
-        ct1 = ClasT.le_arquivo("")
-        ct2 = ClasT.le_arquivo("")
-        assert ct1 == ct2
+        ad1 = Exph.read(ARQ_TESTE)
+        ad2 = Exph.read(ARQ_TESTE)
+        assert ad1 == ad2
 
 
-def test_neq_cadic():
-    m: MagicMock = mock_open(read_data="".join(MockClasT))
+def test_neq_exph():
+    m: MagicMock = mock_open(read_data="".join(MockExph))
     with patch("builtins.open", m):
-        ct1 = ClasT.le_arquivo("")
-        ct2 = ClasT.le_arquivo("")
-        ct2.usinas.iloc[0, 0] = -1
-        assert ct1 != ct2
+        ad1 = Exph.read(ARQ_TESTE)
+        ad2 = Exph.read(ARQ_TESTE)
+        ad2.expansoes.iloc[0, 0] = -1
+        assert ad1 != ad2
 
 
-def test_leitura_escrita_clast():
-    m_leitura: MagicMock = mock_open(read_data="".join(MockClasT))
+def test_leitura_escrita_exph():
+    m_leitura: MagicMock = mock_open(read_data="".join(MockExph))
     with patch("builtins.open", m_leitura):
-        ct1 = ClasT.le_arquivo("")
+        ad1 = Exph.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        ct1.escreve_arquivo("", "")
+        ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        ct2 = ClasT.le_arquivo("")
-        assert ct1 == ct2
+        ad2 = Exph.read(ARQ_TESTE)
+        assert ad1 == ad2
```

### Comparing `inewave-0.0.95/tests/newave/test_confhd.py` & `inewave-0.0.96/tests/newave/test_term.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,73 @@
-# Rotinas de testes associadas ao arquivo confhd.dat do NEWAVE
-from inewave.newave.modelos.confhd import BlocoConfUHE
+# Rotinas de testes associadas ao arquivo term.dat do NEWAVE
+from inewave.config import MESES_DF
+from inewave.newave.modelos.term import BlocoTermUTE
 
-from inewave.newave import Confhd
+from inewave.newave import Term
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.confhd import MockBlocoConfUHE
+from tests.mocks.arquivos.term import MockBlocoUTE
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_uhe_confhd():
 
-    m: MagicMock = mock_open(read_data="".join(MockBlocoConfUHE))
-    b = BlocoConfUHE()
+def test_bloco_usinas_term():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoUTE))
+    b = BlocoTermUTE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
+    assert b.data.shape[0] == 125
+    assert b.data.iloc[0, 0] == 1
+    assert b.data.iloc[-1, -1] == 63.0
 
-    assert b.data.shape[0] == 164
-    assert b.data.iloc[0, 0] == 4
-    assert b.data.iloc[-1, -1] == 1995
 
-
-def test_atributos_encontrados_confhd():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoConfUHE))
+def test_atributos_encontrados_term():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoUTE))
     with patch("builtins.open", m):
-        ad = Confhd.le_arquivo("")
+        ad = Term.read(ARQ_TESTE)
         assert ad.usinas is not None
 
 
-def test_atributos_nao_encontrados_confhd():
+def test_atributos_nao_encontrados_term():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = Confhd.le_arquivo("")
+        ad = Term.read(ARQ_TESTE)
         assert ad.usinas is None
 
 
-def test_eq_confhd():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoConfUHE))
+def test_eq_term():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoUTE))
     with patch("builtins.open", m):
-        cf1 = Confhd.le_arquivo("")
-        cf2 = Confhd.le_arquivo("")
+        cf1 = Term.read(ARQ_TESTE)
+        cf2 = Term.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
-def test_neq_confhd():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoConfUHE))
+def test_neq_term():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoUTE))
     with patch("builtins.open", m):
-        cf1 = Confhd.le_arquivo("")
-        cf2 = Confhd.le_arquivo("")
+        cf1 = Term.read(ARQ_TESTE)
+        cf2 = Term.read(ARQ_TESTE)
         cf2.usinas.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
-def test_leitura_escrita_confhd():
-    m_leitura: MagicMock = mock_open(read_data="".join(MockBlocoConfUHE))
+def test_leitura_escrita_term():
+    m_leitura: MagicMock = mock_open(read_data="".join(MockBlocoUTE))
     with patch("builtins.open", m_leitura):
-        cf1 = Confhd.le_arquivo("")
+        cf1 = Term.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = Confhd.le_arquivo("")
+        cf2 = Term.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_conft.py` & `inewave-0.0.96/tests/newave/test_conft.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,68 +5,69 @@
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.conft import MockBlocoConfUTE
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_ute_conft():
 
+def test_bloco_ute_conft():
     m: MagicMock = mock_open(read_data="".join(MockBlocoConfUTE))
     b = BlocoConfUTE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 125
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 209
 
 
 def test_atributos_encontrados_conft():
     m: MagicMock = mock_open(read_data="".join(MockBlocoConfUTE))
     with patch("builtins.open", m):
-        ad = ConfT.le_arquivo("")
+        ad = ConfT.read(ARQ_TESTE)
         assert ad.usinas is not None
 
 
 def test_atributos_nao_encontrados_conft():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = ConfT.le_arquivo("")
+        ad = ConfT.read(ARQ_TESTE)
         assert ad.usinas is None
 
 
 def test_eq_conft():
     m: MagicMock = mock_open(read_data="".join(MockBlocoConfUTE))
     with patch("builtins.open", m):
-        cf1 = ConfT.le_arquivo("")
-        cf2 = ConfT.le_arquivo("")
+        cf1 = ConfT.read(ARQ_TESTE)
+        cf2 = ConfT.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_conft():
     m: MagicMock = mock_open(read_data="".join(MockBlocoConfUTE))
     with patch("builtins.open", m):
-        cf1 = ConfT.le_arquivo("")
-        cf2 = ConfT.le_arquivo("")
+        cf1 = ConfT.read(ARQ_TESTE)
+        cf2 = ConfT.read(ARQ_TESTE)
         cf2.usinas.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
 def test_leitura_escrita_conft():
     m_leitura: MagicMock = mock_open(read_data="".join(MockBlocoConfUTE))
     with patch("builtins.open", m_leitura):
-        cf1 = ConfT.le_arquivo("")
+        cf1 = ConfT.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = ConfT.le_arquivo("")
+        cf2 = ConfT.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_curva.py` & `inewave-0.0.96/tests/newave/test_curva.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,154 +22,149 @@
     MockMaximoIteracoesProcessoIterativoEtapa2,
     MockIteracaoAPartirProcessoIterativoEtapa2,
     MockToleranciaProcessoIterativoEtapa2,
     MockImpressaoRelatorioProcessoIterativoEtapa2,
     MockCurva,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_configuracoes_penalizacao_curva():
 
+def test_bloco_configuracoes_penalizacao_curva():
     m: MagicMock = mock_open(read_data="".join(MockBlockTipoPenalizacao))
     b = BlocoConfiguracoesPenalizacaoCurva()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data == [1, 11, 1]
 
 
 def test_bloco_penalidades_ree():
-
     m: MagicMock = mock_open(read_data="".join(MockBlocoCustoPorSistema))
     b = BlocoPenalidadesViolacaoREECurva()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 1745.08
 
 
 def test_bloco_curva_seguranca():
-
     m: MagicMock = mock_open(read_data="".join(MockBlocoCurvaSeguranca))
     b = BlocoCurvaSegurancaSubsistema()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 10.0
 
 
 def test_bloco_maximo_iteracoes():
-
     m: MagicMock = mock_open(
         read_data="".join(MockMaximoIteracoesProcessoIterativoEtapa2)
     )
     b = BlocoMaximoIteracoesProcessoIterativoEtapa2()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data == 0
 
 
 def test_bloco_iteracao_a_partir():
-
     m: MagicMock = mock_open(
         read_data="".join(MockIteracaoAPartirProcessoIterativoEtapa2)
     )
     b = BlocoIteracaoAPartirProcessoIterativoEtapa2()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data == 10
 
 
 def test_bloco_tolerancia_processo():
-
     m: MagicMock = mock_open(
         read_data="".join(MockToleranciaProcessoIterativoEtapa2)
     )
     b = BlocoToleranciaProcessoIterativoEtapa2()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data == 0.01
 
 
 def test_bloco_impressao_relatorio():
-
     m: MagicMock = mock_open(
         read_data="".join(MockImpressaoRelatorioProcessoIterativoEtapa2)
     )
     b = BlocoImpressaoRelatorioProcessoIterativoEtapa2()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data == 0
 
 
 def test_atributos_encontrados_curva():
     m: MagicMock = mock_open(read_data="".join(MockCurva))
     with patch("builtins.open", m):
-        ad = Curva.le_arquivo("")
+        ad = Curva.read(ARQ_TESTE)
         assert ad.configuracoes_penalizacao != [None, None, None]
         assert ad.custos_penalidades is not None
         assert ad.curva_seguranca is not None
         assert ad.maximo_iteracoes_etapa2 is not None
         assert ad.iteracao_a_partir_etapa2 is not None
         assert ad.tolerancia_processo_etapa2 is not None
         assert ad.impressao_relatorio_etapa2 is not None
 
 
 def test_atributos_nao_encontrados_curva():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = Curva.le_arquivo("")
+        ad = Curva.read(ARQ_TESTE)
         assert ad.configuracoes_penalizacao == [None, None, None]
         assert ad.custos_penalidades is None
         assert ad.curva_seguranca is None
         assert ad.maximo_iteracoes_etapa2 is None
         assert ad.iteracao_a_partir_etapa2 is None
         assert ad.tolerancia_processo_etapa2 is None
         assert ad.impressao_relatorio_etapa2 is None
 
 
 def test_eq_curva():
     m: MagicMock = mock_open(read_data="".join(MockCurva))
     with patch("builtins.open", m):
-        cf1 = Curva.le_arquivo("")
-        cf2 = Curva.le_arquivo("")
+        cf1 = Curva.read(ARQ_TESTE)
+        cf2 = Curva.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_curva():
     m: MagicMock = mock_open(read_data="".join(MockCurva))
     with patch("builtins.open", m):
-        cf1 = Curva.le_arquivo("")
-        cf2 = Curva.le_arquivo("")
+        cf1 = Curva.read(ARQ_TESTE)
+        cf2 = Curva.read(ARQ_TESTE)
         cf2.curva_seguranca.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
 def test_leitura_escrita_curva():
     m_leitura: MagicMock = mock_open(read_data="".join(MockCurva))
     with patch("builtins.open", m_leitura):
-        cf1 = Curva.le_arquivo("")
+        cf1 = Curva.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = Curva.le_arquivo("")
+        cf2 = Curva.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_cvar.py` & `inewave-0.0.96/tests/newave/test_penalid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,109 +1,62 @@
-# Rotinas de testes associadas ao arquivo cvar.dat do NEWAVE
-from inewave.newave.modelos.cvar import (
-    BlocoValoresConstantesCVAR,
-    BlocoAlfaVariavelNoTempo,
-    BlocoLambdaVariavelNoTempo,
-)
+# Rotinas de testes associadas ao arquivo penalid.dat do NEWAVE
 
-from inewave.newave import CVAR
+from inewave.newave.penalid import Penalid
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.cvar import (
-    MockBlocoValoresConstantes,
-    MockBlocoValoresAlfaVariaveis,
-    MockBlocoValoresLambdaVariaveis,
-    MockCVAR,
+from tests.mocks.arquivos.penalid import (
+    MockPenalid,
 )
 
-
-def test_bloco_valores_constantes_cvar():
-
-    m: MagicMock = mock_open(read_data="".join(MockBlocoValoresConstantes))
-    b = BlocoValoresConstantesCVAR()
-    with patch("builtins.open", m):
-        with open("", "") as fp:
-            b.read(fp)
-
-    assert b.data == [50.0, 40.0]
-
-
-def test_bloco_alfa_variavel_cvar():
-
-    m: MagicMock = mock_open(read_data="".join(MockBlocoValoresAlfaVariaveis))
-    b = BlocoAlfaVariavelNoTempo()
-    with patch("builtins.open", m):
-        with open("", "") as fp:
-            b.read(fp)
-
-    assert b.data.iloc[0, 0] == "2017"
-    assert b.data.iloc[-1, -1] == 5.0
-
-
-def test_bloco_lambda_variavel_cvar():
-
-    m: MagicMock = mock_open(
-        read_data="".join(MockBlocoValoresLambdaVariaveis)
-    )
-    b = BlocoLambdaVariavelNoTempo()
-    with patch("builtins.open", m):
-        with open("", "") as fp:
-            b.read(fp)
-
-    assert b.data.iloc[0, 0] == "2017"
-    assert b.data.iloc[-1, -1] == 10.0
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_cvar():
-    m: MagicMock = mock_open(read_data="".join(MockCVAR))
+def test_atributos_encontrados_penalid():
+    m: MagicMock = mock_open(read_data="".join(MockPenalid))
     with patch("builtins.open", m):
-        ad = CVAR.le_arquivo("")
-        assert ad.valores_constantes != [None, None]
-        assert ad.alfa_variavel is not None
-        assert ad.lambda_variavel is not None
+        ad = Penalid.read(ARQ_TESTE)
+        assert ad.penalidades is not None
 
 
-def test_atributos_nao_encontrados_cvar():
+def test_atributos_nao_encontrados_penalid():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = CVAR.le_arquivo("")
-        assert ad.valores_constantes is None
-        assert ad.alfa_variavel is None
-        assert ad.lambda_variavel is None
+        ad = Penalid.read(ARQ_TESTE)
+        assert ad.penalidades is None
 
 
-def test_eq_cvar():
-    m: MagicMock = mock_open(read_data="".join(MockCVAR))
+def test_eq_penalid():
+    m: MagicMock = mock_open(read_data="".join(MockPenalid))
     with patch("builtins.open", m):
-        cf1 = CVAR.le_arquivo("")
-        cf2 = CVAR.le_arquivo("")
+        cf1 = Penalid.read(ARQ_TESTE)
+        cf2 = Penalid.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
-def test_neq_cvar():
-    m: MagicMock = mock_open(read_data="".join(MockCVAR))
+def test_neq_penalid():
+    m: MagicMock = mock_open(read_data="".join(MockPenalid))
     with patch("builtins.open", m):
-        cf1 = CVAR.le_arquivo("")
-        cf2 = CVAR.le_arquivo("")
-        cf2.valores_constantes = [0, 0]
+        cf1 = Penalid.read(ARQ_TESTE)
+        cf2 = Penalid.read(ARQ_TESTE)
+        cf2.penalidades.loc[0, 0] = 0
         assert cf1 != cf2
 
 
-def test_leitura_escrita_cvar():
-    m_leitura: MagicMock = mock_open(read_data="".join(MockCVAR))
+def test_leitura_escrita_penalid():
+    m_leitura: MagicMock = mock_open(read_data="".join(MockPenalid))
     with patch("builtins.open", m_leitura):
-        cf1 = CVAR.le_arquivo("")
+        cf1 = Penalid.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = CVAR.le_arquivo("")
+        cf2 = Penalid.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_dger.py` & `inewave-0.0.96/tests/newave/test_dger.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from inewave.newave.dger import DGer
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dger import MockDger
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_nao_encontrados_dger():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.nome_caso == ""
         assert d.tipo_execucao is None
         assert d.duracao_periodo is None
         assert d.num_anos_estudo is None
         assert d.mes_inicio_pre_estudo is None
         assert d.mes_inicio_estudo is None
         assert d.ano_inicio_estudo is None
@@ -125,20 +127,22 @@
         assert d.restricao_lpp_turbinamento_maximo_ree is None
         assert d.restricao_lpp_defluencia_maxima_ree is None
         assert d.restricao_lpp_turbinamento_maximo_uhe is None
         assert d.restricao_lpp_defluencia_maxima_uhe is None
         assert d.restricoes_eletricas_especiais is None
         assert d.funcao_producao_uhe is None
         assert d.fcf_pos_estudo is None
+        assert d.estacoes_bombeamento is None
+        assert d.canal_desvio is None
 
 
 def test_atributos_encontrados_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.nome_caso is not None
         assert d.tipo_execucao is not None
         assert d.duracao_periodo is not None
         assert d.num_anos_estudo is not None
         assert d.mes_inicio_pre_estudo is not None
         assert d.mes_inicio_estudo is not None
         assert d.ano_inicio_estudo is not None
@@ -249,619 +253,621 @@
         assert d.restricao_lpp_turbinamento_maximo_ree is not None
         assert d.restricao_lpp_defluencia_maxima_ree is not None
         assert d.restricao_lpp_turbinamento_maximo_uhe is not None
         assert d.restricao_lpp_defluencia_maxima_uhe is not None
         assert d.restricoes_eletricas_especiais is not None
         assert d.funcao_producao_uhe is not None
         assert d.fcf_pos_estudo is not None
+        assert d.estacoes_bombeamento is not None
+        assert d.canal_desvio is not None
 
 
 def test_nome_caso_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.nome_caso == (
             "PMO JANEIRO - 2021  22/12/2020 12:43:55  Niveis"
             + " para 26/12 NW Versao 27.5_CPAMP"
         )
         novo_valor = "Teste"
         d.nome_caso = novo_valor
         assert d.nome_caso == novo_valor
 
 
 def test_tipo_execucao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.tipo_execucao == 1
         novo_valor = 0
         d.tipo_execucao = novo_valor
         assert d.tipo_execucao == novo_valor
 
 
 def test_duracao_periodo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.duracao_periodo == 1
         novo_valor = 0
         d.duracao_periodo = novo_valor
         assert d.duracao_periodo == novo_valor
 
 
 def test_num_anos_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.num_anos_estudo == 5
         novo_valor = 0
         d.num_anos_estudo = novo_valor
         assert d.num_anos_estudo == novo_valor
 
 
 def test_mes_inicio_pre_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.mes_inicio_pre_estudo == 1
         novo_valor = 0
         d.mes_inicio_pre_estudo = novo_valor
         assert d.mes_inicio_pre_estudo == novo_valor
 
 
 def test_mes_inicio_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.mes_inicio_estudo == 1
         novo_valor = 0
         d.mes_inicio_estudo = novo_valor
         assert d.mes_inicio_estudo == novo_valor
 
 
 def test_ano_inicio_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.ano_inicio_estudo == 2021
         novo_valor = 0
         d.ano_inicio_estudo = novo_valor
         assert d.ano_inicio_estudo == novo_valor
 
 
 def test_num_anos_pre_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.num_anos_pre_estudo == 0
         novo_valor = 5
         d.num_anos_pre_estudo = novo_valor
         assert d.num_anos_pre_estudo == novo_valor
 
 
 def test_num_anos_pos_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.num_anos_pos_estudo == 5
         novo_valor = 0
         d.num_anos_pos_estudo = novo_valor
         assert d.num_anos_pos_estudo == novo_valor
 
 
 def test_num_anos_pos_sim_final_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.num_anos_pos_sim_final == 0
         novo_valor = 1
         d.num_anos_pos_sim_final = novo_valor
         assert d.num_anos_pos_sim_final == novo_valor
 
 
 def test_imprime_dados_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.imprime_dados == 1
         novo_valor = 0
         d.imprime_dados = novo_valor
         assert d.imprime_dados == novo_valor
 
 
 def test_imprime_mercados_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.imprime_mercados == 1
         novo_valor = 0
         d.imprime_mercados = novo_valor
         assert d.imprime_mercados == novo_valor
 
 
 def test_imprime_energias_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.imprime_energias == 1
         novo_valor = 0
         d.imprime_energias = novo_valor
         assert d.imprime_energias == novo_valor
 
 
 def test_imprime_modelo_estocastico_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.imprime_modelo_estocastico == 1
         novo_valor = 0
         d.imprime_modelo_estocastico = novo_valor
         assert d.imprime_modelo_estocastico == novo_valor
 
 
 def test_imprime_subsistema_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.imprime_subsistema == 1
         novo_valor = 0
         d.imprime_subsistema = novo_valor
         assert d.imprime_subsistema == novo_valor
 
 
 def test_num_max_iteracoes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.num_max_iteracoes == 45
         novo_valor = 0
         d.num_max_iteracoes = novo_valor
         assert d.num_max_iteracoes == novo_valor
 
 
 def test_num_forwards_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.num_forwards == 200
         novo_valor = 0
         d.num_forwards = novo_valor
         assert d.num_forwards == novo_valor
 
 
 def test_num_aberturas_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.num_aberturas == 20
         novo_valor = 0
         d.num_aberturas = novo_valor
         assert d.num_aberturas == novo_valor
 
 
 def test_num_series_sinteticas_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.num_series_sinteticas == 2000
         novo_valor = 0
         d.num_series_sinteticas = novo_valor
         assert d.num_series_sinteticas == novo_valor
 
 
 def test_ordem_maxima_parp_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.ordem_maxima_parp == 6
         novo_valor = 0
         d.ordem_maxima_parp = novo_valor
         assert d.ordem_maxima_parp == novo_valor
 
 
 def test_ano_inicial_historico_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.ano_inicial_historico == 1931
         novo_valor = 0
         d.ano_inicial_historico = novo_valor
         assert d.ano_inicial_historico == novo_valor
 
 
 def test_tamanho_registro_arquivo_historico_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.tamanho_registro_arquivo_historico == 0
         novo_valor = 1
         d.tamanho_registro_arquivo_historico = novo_valor
         assert d.tamanho_registro_arquivo_historico == novo_valor
 
 
 def test_calcula_volume_inicial_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.calcula_volume_inicial == 1
         novo_valor = 0
         d.calcula_volume_inicial = novo_valor
         assert d.calcula_volume_inicial == novo_valor
 
 
 def test_volume_inicial_subsistema_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.volume_inicial_subsistema == [0.0, 0.0, 0.0, 0.0, 0.0]
         novo_valor = [1.0, 1.0, 1.0, 1.0, 1.0]
         d.volume_inicial_subsistema = novo_valor
         assert d.volume_inicial_subsistema == novo_valor
 
 
 def test_tolerancia_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.tolerancia == 95.0
         novo_valor = 0.0
         d.tolerancia = novo_valor
         assert d.tolerancia == novo_valor
 
 
 def test_taxa_de_desconto_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.taxa_de_desconto == 12.0
         novo_valor = 0.0
         d.taxa_de_desconto = novo_valor
         assert d.taxa_de_desconto == novo_valor
 
 
 def test_tipo_simulacao_final_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.tipo_simulacao_final == 1
         novo_valor = 0
         d.tipo_simulacao_final = novo_valor
         assert d.tipo_simulacao_final == novo_valor
 
 
 def test_agregacao_simulacao_final_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.agregacao_simulacao_final == 1
         novo_valor = 0
         d.agregacao_simulacao_final = novo_valor
         assert d.agregacao_simulacao_final == novo_valor
 
 
 def test_impressao_operacao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.impressao_operacao == 1
         novo_valor = 0
         d.impressao_operacao = novo_valor
         assert d.impressao_operacao == novo_valor
 
 
 def test_impressao_convergencia_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.impressao_convergencia == 1
         novo_valor = 0
         d.impressao_convergencia = novo_valor
         assert d.impressao_convergencia == novo_valor
 
 
 def test_intervalo_para_gravar_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.intervalo_para_gravar == 1
         novo_valor = 0
         d.intervalo_para_gravar = novo_valor
         assert d.intervalo_para_gravar == novo_valor
 
 
 def test_num_minimo_iteracoes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.num_minimo_iteracoes == 30
         novo_valor = 0
         d.num_minimo_iteracoes = novo_valor
         assert d.num_minimo_iteracoes == novo_valor
 
 
 def test_racionamento_preventivo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.racionamento_preventivo == 0
         novo_valor = 1
         d.racionamento_preventivo = novo_valor
         assert d.racionamento_preventivo == novo_valor
 
 
 def test_num_anos_manutencao_utes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.num_anos_manutencao_utes == 1
         novo_valor = 0
         d.num_anos_manutencao_utes = novo_valor
         assert d.num_anos_manutencao_utes == novo_valor
 
 
 def test_tendencia_hidrologica_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.considera_tendencia_hidrologica_calculo_politica == 2
         assert d.considera_tendencia_hidrologica_sim_final == 2
         novo_valor = 0
         d.considera_tendencia_hidrologica_calculo_politica = novo_valor
         assert d.considera_tendencia_hidrologica_calculo_politica == novo_valor
         d.considera_tendencia_hidrologica_sim_final = novo_valor
         assert d.considera_tendencia_hidrologica_sim_final == novo_valor
 
 
 def test_restricao_itaipu_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricao_itaipu == 0
         novo_valor = 1
         d.restricao_itaipu = novo_valor
         assert d.restricao_itaipu == novo_valor
 
 
 def test_bid_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.bid == 0
         novo_valor = 1
         d.bid = novo_valor
         assert d.bid == novo_valor
 
 
 def test_perdas_rede_transmissao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.perdas_rede_transmissao == 0
         novo_valor = 1
         d.perdas_rede_transmissao = novo_valor
         assert d.perdas_rede_transmissao == novo_valor
 
 
 def test_el_nino_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.el_nino == 0
         novo_valor = 1
         d.el_nino = novo_valor
         assert d.el_nino == novo_valor
 
 
 def test_enso_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.enso == 0
         novo_valor = 1
         d.enso = novo_valor
         assert d.enso == novo_valor
 
 
 def test_duracao_por_patamar_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.duracao_por_patamar == 1
         novo_valor = 0
         d.duracao_por_patamar = novo_valor
         assert d.duracao_por_patamar == novo_valor
 
 
 def test_outros_usos_da_agua_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.outros_usos_da_agua == 1
         novo_valor = 0
         d.outros_usos_da_agua = novo_valor
         assert d.outros_usos_da_agua == novo_valor
 
 
 def test_correcao_desvio_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.correcao_desvio == 1
         novo_valor = 0
         d.correcao_desvio = novo_valor
         assert d.correcao_desvio == novo_valor
 
 
 def test_curva_aversao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.curva_aversao == 1
         novo_valor = 0
         d.curva_aversao = novo_valor
         assert d.curva_aversao == novo_valor
 
 
 def test_tipo_geracao_enas_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.tipo_geracao_enas == 0
         novo_valor = 1
         d.tipo_geracao_enas = novo_valor
         assert d.tipo_geracao_enas == novo_valor
 
 
 def test_risco_deficit_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.primeira_profundidade_risco_deficit == 1.0
         assert d.segunda_profundidade_risco_deficit == 2.5
         novo_valor = 0.0
         d.primeira_profundidade_risco_deficit = novo_valor
         assert d.primeira_profundidade_risco_deficit == novo_valor
         d.segunda_profundidade_risco_deficit = novo_valor
         assert d.segunda_profundidade_risco_deficit == novo_valor
 
 
 def test_iteracao_para_simulacao_final_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.iteracao_para_simulacao_final == 0
         novo_valor = 1
         d.iteracao_para_simulacao_final = novo_valor
         assert d.iteracao_para_simulacao_final == novo_valor
 
 
 def test_agrupamento_livre_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.agrupamento_livre == 1
         novo_valor = 0
         d.agrupamento_livre = novo_valor
         assert d.agrupamento_livre == novo_valor
 
 
 def test_equalizacao_penal_intercambio_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.equalizacao_penal_intercambio == 1
         novo_valor = 0
         d.equalizacao_penal_intercambio = novo_valor
         assert d.equalizacao_penal_intercambio == novo_valor
 
 
 def test_representacao_submotorizacao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.representacao_submotorizacao == 2
         novo_valor = 0
         d.representacao_submotorizacao = novo_valor
         assert d.representacao_submotorizacao == novo_valor
 
 
 def test_ordenacao_automatica_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.ordenacao_automatica == 0
         novo_valor = 1
         d.ordenacao_automatica = novo_valor
         assert d.ordenacao_automatica == novo_valor
 
 
 def test_considera_carga_adicional_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.considera_carga_adicional == 1
         novo_valor = 0
         d.considera_carga_adicional = novo_valor
         assert d.considera_carga_adicional == novo_valor
 
 
 def test_delta_zsup_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.delta_zsup == 10
         novo_valor = 0.0
         d.delta_zsup = novo_valor
         assert d.delta_zsup == novo_valor
 
 
 def test_delta_zinf_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.delta_zinf == 0.2
         novo_valor = 0.0
         d.delta_zinf = novo_valor
         assert d.delta_zinf == novo_valor
 
 
 def test_deltas_consecutivos_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.deltas_consecutivos == 3
         novo_valor = 0
         d.deltas_consecutivos = novo_valor
         assert d.deltas_consecutivos == novo_valor
 
 
 def test_despacho_antecipado_gnl_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.despacho_antecipado_gnl == 1
         novo_valor = 0
         d.despacho_antecipado_gnl = novo_valor
         assert d.despacho_antecipado_gnl == novo_valor
 
 
 def test_modif_automatica_adterm_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.modif_automatica_adterm == 1
         novo_valor = 0
         d.modif_automatica_adterm = novo_valor
         assert d.modif_automatica_adterm == novo_valor
 
 
 def test_considera_ghmin_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.considera_ghmin == 1
         novo_valor = 0
         d.considera_ghmin = novo_valor
         assert d.considera_ghmin == novo_valor
 
 
 def test_simulacao_final_com_data_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.simulacao_final_com_data == 0
         novo_valor = 1
         d.simulacao_final_com_data = novo_valor
         assert d.simulacao_final_com_data == novo_valor
 
 
 def test_gerenciamento_pls_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.utiliza_gerenciamento_pls == 0
         assert d.comunicacao_dois_niveis == 0
         assert d.armazenamento_local_arquivos_temporarios == 0
         assert d.alocacao_memoria_ena == 0
         assert d.alocacao_memoria_cortes == 0
         novo_valor = 1
         d.utiliza_gerenciamento_pls = novo_valor
@@ -875,95 +881,95 @@
         d.alocacao_memoria_cortes = novo_valor
         assert d.alocacao_memoria_cortes == novo_valor
 
 
 def test_sar_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.sar == 0
         novo_valor = 1
         d.sar = novo_valor
         assert d.sar == novo_valor
 
 
 def test_cvar_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.cvar == 1
         novo_valor = 0
         d.cvar = novo_valor
         assert d.cvar == novo_valor
 
 
 def test_considera_zsup_min_convergencia_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.considera_zsup_min_convergencia == 0
         novo_valor = 0
         d.considera_zsup_min_convergencia = novo_valor
         assert d.considera_zsup_min_convergencia == novo_valor
 
 
 def test_desconsidera_vazao_minima_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.desconsidera_vazao_minima == 0
         novo_valor = 1
         d.desconsidera_vazao_minima = novo_valor
         assert d.desconsidera_vazao_minima == novo_valor
 
 
 def test_restricoes_eletricas_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricoes_eletricas == 1
         novo_valor = 0
         d.restricoes_eletricas = novo_valor
         assert d.restricoes_eletricas == novo_valor
 
 
 def test_selecao_de_cortes_backward_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.selecao_de_cortes_backward == 1
         novo_valor = 0
         d.selecao_de_cortes_backward = novo_valor
         assert d.selecao_de_cortes_backward == novo_valor
 
 
 def test_selecao_de_cortes_forward_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.selecao_de_cortes_forward == 1
         novo_valor = 0
         d.selecao_de_cortes_forward = novo_valor
         assert d.selecao_de_cortes_forward == novo_valor
 
 
 def test_janela_de_cortes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.janela_de_cortes == 0
         novo_valor = 1
         d.janela_de_cortes = novo_valor
         assert d.janela_de_cortes == novo_valor
 
 
 def test_reamostragem_cenarios_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.considera_reamostragem_cenarios == 1
         assert d.tipo_reamostragem_cenarios == 1
         assert d.passo_reamostragem_cenarios == 1
         novo_valor = 0
         d.considera_reamostragem_cenarios = novo_valor
         assert d.considera_reamostragem_cenarios == novo_valor
         d.tipo_reamostragem_cenarios = novo_valor
@@ -971,380 +977,400 @@
         d.passo_reamostragem_cenarios = novo_valor
         assert d.passo_reamostragem_cenarios == novo_valor
 
 
 def test_converge_no_zero_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.converge_no_zero == 0
         novo_valor = 1
         d.converge_no_zero = novo_valor
         assert d.converge_no_zero == novo_valor
 
 
 def test_consulta_fcf_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.consulta_fcf == 0
         novo_valor = 1
         d.consulta_fcf = novo_valor
         assert d.consulta_fcf == novo_valor
 
 
 def test_impressao_ena_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.impressao_ena == 1
         novo_valor = 0
         d.impressao_ena = novo_valor
         assert d.impressao_ena == novo_valor
 
 
 def test_impressao_cortes_ativos_sim_final_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.impressao_cortes_ativos_sim_final == 0
         novo_valor = 1
         d.impressao_cortes_ativos_sim_final = novo_valor
         assert d.impressao_cortes_ativos_sim_final == novo_valor
 
 
 def test_representacao_agregacao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.representacao_agregacao == 1
         novo_valor = 0
         d.representacao_agregacao = novo_valor
         assert d.representacao_agregacao == novo_valor
 
 
 def test_matriz_correlacao_espacial_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.matriz_correlacao_espacial == 1
         novo_valor = 0
         d.matriz_correlacao_espacial = novo_valor
         assert d.matriz_correlacao_espacial == novo_valor
 
 
 def test_desconsidera_convergencia_estatistica_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.desconsidera_convergencia_estatistica == 1
         novo_valor = 0
         d.desconsidera_convergencia_estatistica = novo_valor
         assert d.desconsidera_convergencia_estatistica == novo_valor
 
 
 def test_momento_reamostragem_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.momento_reamostragem == 1
         novo_valor = 0
         d.momento_reamostragem = novo_valor
         assert d.momento_reamostragem == novo_valor
 
 
 def test_mantem_arquivos_energias_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.mantem_arquivos_energias == 0
         novo_valor = 1
         d.mantem_arquivos_energias = novo_valor
         assert d.mantem_arquivos_energias == novo_valor
 
 
 def test_inicio_teste_convergencia_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.inicio_teste_convergencia == 1
         novo_valor = 0
         d.inicio_teste_convergencia = novo_valor
         assert d.inicio_teste_convergencia == novo_valor
 
 
 def test_sazonaliza_vmint_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.sazonaliza_vmint == 0
         novo_valor = 1
         d.sazonaliza_vmint = novo_valor
         assert d.sazonaliza_vmint == novo_valor
 
 
 def test_sazonaliza_vmaxt_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.sazonaliza_vmaxt == 0
         novo_valor = 1
         d.sazonaliza_vmaxt = novo_valor
         assert d.sazonaliza_vmaxt == novo_valor
 
 
 def test_sazonaliza_vminp_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.sazonaliza_vminp == 0
         novo_valor = 1
         d.sazonaliza_vminp = novo_valor
         assert d.sazonaliza_vminp == novo_valor
 
 
 def test_sazonaliza_cfuga_cmont_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.sazonaliza_cfuga_cmont == 0
         novo_valor = 1
         d.sazonaliza_cfuga_cmont = novo_valor
         assert d.sazonaliza_cfuga_cmont == novo_valor
 
 
 def test_restricoes_emissao_gee_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricoes_emissao_gee == 0
         novo_valor = 1
         d.restricoes_emissao_gee = novo_valor
         assert d.restricoes_emissao_gee == novo_valor
 
 
 def test_afluencia_anual_parp_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.consideracao_media_anual_afluencias == 3
         assert d.reducao_automatica_ordem == 0
         novo_valor = 1
         d.consideracao_media_anual_afluencias = novo_valor
         assert d.consideracao_media_anual_afluencias == novo_valor
         d.reducao_automatica_ordem = novo_valor
         assert d.reducao_automatica_ordem == novo_valor
 
 
 def test_restricoes_fornecimento_gas_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricoes_fornecimento_gas == 0
         novo_valor = 1
         d.restricoes_fornecimento_gas = novo_valor
         assert d.restricoes_fornecimento_gas == novo_valor
 
 
 def test_memoria_calculo_cortes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.memoria_calculo_cortes == 0
         novo_valor = 1
         d.memoria_calculo_cortes = novo_valor
         assert d.memoria_calculo_cortes == novo_valor
 
 
 def test_considera_geracao_eolica_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.considera_geracao_eolica == 1
         novo_valor = 0
         d.considera_geracao_eolica = novo_valor
         assert d.considera_geracao_eolica == novo_valor
 
 
 def test_penalidade_corte_geracao_eolica_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.penalidade_corte_geracao_eolica == 0.0063
         novo_valor = 1.0
         d.penalidade_corte_geracao_eolica = novo_valor
         assert d.penalidade_corte_geracao_eolica == novo_valor
 
 
 def test_compensacao_correlacao_cruzada_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.compensacao_correlacao_cruzada == 1
         novo_valor = 0
         d.compensacao_correlacao_cruzada = novo_valor
         assert d.compensacao_correlacao_cruzada == novo_valor
 
 
 def test_restricao_turbinamento_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricao_turbinamento == 1
         novo_valor = 0
         d.restricao_turbinamento = novo_valor
         assert d.restricao_turbinamento == novo_valor
 
 
 def test_restricao_defluencia_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricao_defluencia == 1
         novo_valor = 0
         d.restricao_defluencia = novo_valor
         assert d.restricao_defluencia == novo_valor
 
 
 def test_aproveitamento_base_pls_backward_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.aproveitamento_bases_backward == 1
         novo_valor = 0
         d.aproveitamento_bases_backward = novo_valor
         assert d.aproveitamento_bases_backward == novo_valor
 
 
 def test_impressao_estados_geracao_cortes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.impressao_estados_geracao_cortes == 1
         novo_valor = 0
         d.impressao_estados_geracao_cortes = novo_valor
         assert d.impressao_estados_geracao_cortes == novo_valor
 
 
 def test_semente_forward_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.semente_forward == 0
         novo_valor = 1000
         d.semente_forward = novo_valor
         assert d.semente_forward == novo_valor
 
 
 def test_semente_backward_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.semente_backward == 0
         novo_valor = 1000
         d.semente_backward = novo_valor
         assert d.semente_backward == novo_valor
 
 
 def test_restricao_lpp_turbinamento_maximo_ree_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricao_lpp_turbinamento_maximo_ree == 1
         novo_valor = 0
         d.restricao_lpp_turbinamento_maximo_ree = novo_valor
         assert d.restricao_lpp_turbinamento_maximo_ree == novo_valor
 
 
 def test_restricao_lpp_defluencia_maxima_ree_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricao_lpp_defluencia_maxima_ree == 1
         novo_valor = 0
         d.restricao_lpp_defluencia_maxima_ree = novo_valor
         assert d.restricao_lpp_defluencia_maxima_ree == novo_valor
 
 
 def test_restricao_lpp_turbinamento_maximo_uhe_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricao_lpp_turbinamento_maximo_uhe == 1
         novo_valor = 0
         d.restricao_lpp_turbinamento_maximo_uhe = novo_valor
         assert d.restricao_lpp_turbinamento_maximo_uhe == novo_valor
 
 
 def test_restricao_lpp_defluencia_maxima_uhe_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricao_lpp_defluencia_maxima_uhe == 1
         novo_valor = 0
         d.restricao_lpp_defluencia_maxima_uhe = novo_valor
         assert d.restricao_lpp_defluencia_maxima_uhe == novo_valor
 
 
 def test_restricoes_eletricas_especiais():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.restricoes_eletricas_especiais == 0
         novo_valor = 1
         d.restricoes_eletricas_especiais = novo_valor
         assert d.restricoes_eletricas_especiais == novo_valor
 
 
 def test_funcao_producao_uhe():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.funcao_producao_uhe == 0
         novo_valor = 1
         d.funcao_producao_uhe = novo_valor
         assert d.funcao_producao_uhe == novo_valor
 
 
 def test_fcf_pos_estudo():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.le_arquivo("")
+        d = DGer.read(ARQ_TESTE)
         assert d.fcf_pos_estudo == 0
         novo_valor = 1
         d.fcf_pos_estudo = novo_valor
         assert d.fcf_pos_estudo == novo_valor
 
 
+def test_estacoes_bombeamento():
+    m: MagicMock = mock_open(read_data="".join(MockDger))
+    with patch("builtins.open", m):
+        d = DGer.read(ARQ_TESTE)
+        assert d.estacoes_bombeamento == 1
+        novo_valor = 0
+        d.estacoes_bombeamento = novo_valor
+        assert d.estacoes_bombeamento == novo_valor
+
+
+def test_canal_desvio():
+    m: MagicMock = mock_open(read_data="".join(MockDger))
+    with patch("builtins.open", m):
+        d = DGer.read(ARQ_TESTE)
+        assert d.canal_desvio == 1
+        novo_valor = 0
+        d.canal_desvio = novo_valor
+        assert d.canal_desvio == novo_valor
+
+
 def test_eq_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d1 = DGer.le_arquivo("")
-        d2 = DGer.le_arquivo("")
+        d1 = DGer.read(ARQ_TESTE)
+        d2 = DGer.read(ARQ_TESTE)
         assert d1 == d2
 
 
 def test_neq_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d1 = DGer.le_arquivo("")
-        d2 = DGer.le_arquivo("")
+        d1 = DGer.read(ARQ_TESTE)
+        d2 = DGer.read(ARQ_TESTE)
         d2.nome_caso = "Teste"
         assert d1 != d2
 
 
 def test_leitura_escrita_dger():
     m_leitura: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m_leitura):
-        d1 = DGer.le_arquivo("")
+        d1 = DGer.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        d1.escreve_arquivo("", "")
+        d1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        d2 = DGer.le_arquivo("")
+        d2 = DGer.read(ARQ_TESTE)
         assert d1 == d2
```

### Comparing `inewave-0.0.95/tests/newave/test_dsvagua.py` & `inewave-0.0.96/tests/newave/test_dsvagua.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,68 +5,69 @@
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dsvagua import MockBlocoDesviosAgua
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_desvios_dsvagua():
 
+def test_bloco_desvios_dsvagua():
     m: MagicMock = mock_open(read_data="".join(MockBlocoDesviosAgua))
     b = BlocoDsvUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 1045
     assert b.data.iloc[0, 0] == 2020
     assert b.data.iloc[-1, 0] == 2024
 
 
 def test_atributos_encontrados_dsvagua():
     m: MagicMock = mock_open(read_data="".join(MockBlocoDesviosAgua))
     with patch("builtins.open", m):
-        ad = DSVAgua.le_arquivo("")
+        ad = DSVAgua.read(ARQ_TESTE)
         assert ad.desvios is not None
 
 
 def test_atributos_nao_encontrados_dsvagua():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = DSVAgua.le_arquivo("")
+        ad = DSVAgua.read(ARQ_TESTE)
         assert ad.desvios is None
 
 
 def test_eq_dsvagua():
     m: MagicMock = mock_open(read_data="".join(MockBlocoDesviosAgua))
     with patch("builtins.open", m):
-        cf1 = DSVAgua.le_arquivo("")
-        cf2 = DSVAgua.le_arquivo("")
+        cf1 = DSVAgua.read(ARQ_TESTE)
+        cf2 = DSVAgua.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_dsvagua():
     m: MagicMock = mock_open(read_data="".join(MockBlocoDesviosAgua))
     with patch("builtins.open", m):
-        cf1 = DSVAgua.le_arquivo("")
-        cf2 = DSVAgua.le_arquivo("")
+        cf1 = DSVAgua.read(ARQ_TESTE)
+        cf2 = DSVAgua.read(ARQ_TESTE)
         cf2.desvios.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
 def test_leitura_escrita_dsvagua():
     m_leitura: MagicMock = mock_open(read_data="".join(MockBlocoDesviosAgua))
     with patch("builtins.open", m_leitura):
-        cf1 = DSVAgua.le_arquivo("")
+        cf1 = DSVAgua.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = DSVAgua.le_arquivo("")
+        cf2 = DSVAgua.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_eafpast.py` & `inewave-0.0.96/tests/newave/test_eafpast.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,69 +5,70 @@
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.eafpast import MockBlocoAfluenciasPassadas
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_desvios_eafpast():
 
+def test_bloco_desvios_eafpast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoAfluenciasPassadas))
     b = BlocoEafPast()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
     assert b.data.shape[0] == 12
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 544.91
 
 
 def test_atributos_encontrados_eafpast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoAfluenciasPassadas))
     with patch("builtins.open", m):
-        ad = EafPast.le_arquivo("")
+        ad = EafPast.read(ARQ_TESTE)
         assert ad.tendencia is not None
 
 
 def test_atributos_nao_encontrados_eafpast():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = EafPast.le_arquivo("")
+        ad = EafPast.read(ARQ_TESTE)
         assert ad.tendencia is None
 
 
 def test_eq_eafpast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoAfluenciasPassadas))
     with patch("builtins.open", m):
-        cf1 = EafPast.le_arquivo("")
-        cf2 = EafPast.le_arquivo("")
+        cf1 = EafPast.read(ARQ_TESTE)
+        cf2 = EafPast.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_eafpast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoAfluenciasPassadas))
     with patch("builtins.open", m):
-        cf1 = EafPast.le_arquivo("")
-        cf2 = EafPast.le_arquivo("")
+        cf1 = EafPast.read(ARQ_TESTE)
+        cf2 = EafPast.read(ARQ_TESTE)
         cf2.tendencia.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eafpast():
     m_leitura: MagicMock = mock_open(
         read_data="".join(MockBlocoAfluenciasPassadas)
     )
     with patch("builtins.open", m_leitura):
-        cf1 = EafPast.le_arquivo("")
+        cf1 = EafPast.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = EafPast.le_arquivo("")
+        cf2 = EafPast.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_enavazb.py` & `inewave-0.0.96/tests/newave/test_enavazb.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,71 +2,71 @@
 from inewave.newave.enavazb import Enavazb
 
 from os.path import join
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
-ARQ_TEST = "./tests/mocks/arquivos"
+ARQ_TESTE = "./tests/mocks/arquivos/enavazb.dat"
 
 NUM_FORWARDS = 2
 NUM_REES = 1
 NUM_ABERTURAS = 20
 NUM_ESTAGIOS = 16
 NUM_ENTRADAS = NUM_FORWARDS * NUM_ABERTURAS * NUM_REES * NUM_ESTAGIOS
 
 
 def test_secao_enavaz():
     r = SecaoDadosEnavazb()
-    with open(join(ARQ_TEST, "enavazb.dat"), "rb") as fp:
+    with open(ARQ_TESTE, "rb") as fp:
         r.read(
             fp,
             numero_forwards=NUM_FORWARDS,
             numero_aberturas=NUM_ABERTURAS,
             numero_rees=NUM_REES,
             numero_estagios=NUM_ESTAGIOS,
         )
 
     assert len(r.data) == NUM_ENTRADAS
 
 
 def test_atributos_encontrados_enavaz():
-    h = Enavazb.le_arquivo(
-        ARQ_TEST,
+    h = Enavazb.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_aberturas=NUM_ABERTURAS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
     )
     assert h.series is not None
     assert h.series.isna().sum().sum() == 0
 
 
 def test_atributos_nao_encontrados_enavaz():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        h = Enavazb.le_arquivo(
-            "",
+        h = Enavazb.read(
+            ARQ_TESTE,
             numero_forwards=NUM_FORWARDS,
             numero_aberturas=NUM_ABERTURAS,
             numero_rees=NUM_REES,
             numero_estagios=NUM_ESTAGIOS,
         )
         assert h.series.isna().sum().sum() == NUM_ENTRADAS
 
 
 def test_eq_enavaz():
-    h1 = Enavazb.le_arquivo(
-        ARQ_TEST,
+    h1 = Enavazb.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_aberturas=NUM_ABERTURAS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
     )
-    h2 = Enavazb.le_arquivo(
-        ARQ_TEST,
+    h2 = Enavazb.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_aberturas=NUM_ABERTURAS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
     )
     assert h1 == h2
```

### Comparing `inewave-0.0.95/tests/newave/test_enavazf.py` & `inewave-0.0.96/tests/newave/test_enavazf.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,71 +2,71 @@
 from inewave.newave.enavazf import Enavazf
 
 from os.path import join
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
-ARQ_TEST = "./tests/mocks/arquivos"
+ARQ_TESTE = "./tests/mocks/arquivos/enavazf.dat"
 
 NUM_FORWARDS = 2
 NUM_REES = 1
 NUM_ESTAGIOS = 16
 NUM_ESTAGIOS_TH = 12
 NUM_ENTRADAS = NUM_FORWARDS * NUM_REES * (NUM_ESTAGIOS_TH + NUM_ESTAGIOS)
 
 
 def test_secao_enavaz():
     r = SecaoDadosEnavazf()
-    with open(join(ARQ_TEST, "enavazf.dat"), "rb") as fp:
+    with open(ARQ_TESTE, "rb") as fp:
         r.read(
             fp,
             numero_forwards=NUM_FORWARDS,
             numero_rees=NUM_REES,
             numero_estagios=NUM_ESTAGIOS,
             numero_estagios_th=NUM_ESTAGIOS_TH,
         )
 
     assert len(r.data) == NUM_ENTRADAS
 
 
 def test_atributos_encontrados_enavaz():
-    h = Enavazf.le_arquivo(
-        ARQ_TEST,
+    h = Enavazf.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
     assert h.series is not None
     assert h.series.isna().sum().sum() == 0
 
 
 def test_atributos_nao_encontrados_enavaz():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        h = Enavazf.le_arquivo(
-            "",
+        h = Enavazf.read(
+            ARQ_TESTE,
             numero_forwards=NUM_FORWARDS,
             numero_rees=NUM_REES,
             numero_estagios=NUM_ESTAGIOS,
             numero_estagios_th=NUM_ESTAGIOS_TH,
         )
         assert h.series.isna().sum().sum() == NUM_ENTRADAS
 
 
 def test_eq_enavaz():
-    h1 = Enavazf.le_arquivo(
-        ARQ_TEST,
+    h1 = Enavazf.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
-    h2 = Enavazf.le_arquivo(
-        ARQ_TEST,
+    h2 = Enavazf.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
     assert h1 == h2
```

### Comparing `inewave-0.0.95/tests/newave/test_energiab.py` & `inewave-0.0.96/tests/newave/test_energiab.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,71 +2,71 @@
 from inewave.newave.energiab import Energiab
 
 from os.path import join
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
-ARQ_TEST = "./tests/mocks/arquivos"
+ARQ_TESTE = "./tests/mocks/arquivos/energiab.dat"
 
 NUM_FORWARDS = 2
 NUM_REES = 1
 NUM_ABERTURAS = 20
 NUM_ESTAGIOS = 16
 NUM_ENTRADAS = NUM_FORWARDS * NUM_ABERTURAS * NUM_REES * NUM_ESTAGIOS
 
 
 def test_secao_energia():
     r = SecaoDadosEnergiab()
-    with open(join(ARQ_TEST, "energiab.dat"), "rb") as fp:
+    with open(ARQ_TESTE, "rb") as fp:
         r.read(
             fp,
             numero_forwards=NUM_FORWARDS,
             numero_aberturas=NUM_ABERTURAS,
             numero_rees=NUM_REES,
             numero_estagios=NUM_ESTAGIOS,
         )
 
     assert len(r.data) == NUM_ENTRADAS
 
 
 def test_atributos_encontrados_energia():
-    h = Energiab.le_arquivo(
-        ARQ_TEST,
+    h = Energiab.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_aberturas=NUM_ABERTURAS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
     )
     assert h.series is not None
     assert h.series.isna().sum().sum() == 0
 
 
 def test_atributos_nao_encontrados_energia():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        h = Energiab.le_arquivo(
-            "",
+        h = Energiab.read(
+            ARQ_TESTE,
             numero_forwards=NUM_FORWARDS,
             numero_aberturas=NUM_ABERTURAS,
             numero_rees=NUM_REES,
             numero_estagios=NUM_ESTAGIOS,
         )
         assert h.series.isna().sum().sum() == NUM_ENTRADAS
 
 
 def test_eq_energia():
-    h1 = Energiab.le_arquivo(
-        ARQ_TEST,
+    h1 = Energiab.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_aberturas=NUM_ABERTURAS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
     )
-    h2 = Energiab.le_arquivo(
-        ARQ_TEST,
+    h2 = Energiab.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_aberturas=NUM_ABERTURAS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
     )
     assert h1 == h2
```

### Comparing `inewave-0.0.95/tests/newave/test_energiaf.py` & `inewave-0.0.96/tests/newave/test_energiaf.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,71 +2,71 @@
 from inewave.newave.energiaf import Energiaf
 
 from os.path import join
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
-ARQ_TEST = "./tests/mocks/arquivos"
+ARQ_TESTE = "./tests/mocks/arquivos/energiaf.dat"
 
 NUM_FORWARDS = 2
 NUM_REES = 1
 NUM_ESTAGIOS = 16
 NUM_ESTAGIOS_TH = 12
 NUM_ENTRADAS = NUM_FORWARDS * NUM_REES * (NUM_ESTAGIOS_TH + NUM_ESTAGIOS)
 
 
 def test_secao_energia():
     r = SecaoDadosEnergiaf()
-    with open(join(ARQ_TEST, "energiaf.dat"), "rb") as fp:
+    with open(ARQ_TESTE, "rb") as fp:
         r.read(
             fp,
             numero_forwards=NUM_FORWARDS,
             numero_rees=NUM_REES,
             numero_estagios=NUM_ESTAGIOS,
             numero_estagios_th=NUM_ESTAGIOS_TH,
         )
 
     assert len(r.data) == NUM_ENTRADAS
 
 
 def test_atributos_encontrados_energia():
-    h = Energiaf.le_arquivo(
-        ARQ_TEST,
+    h = Energiaf.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
     assert h.series is not None
     assert h.series.isna().sum().sum() == 0
 
 
 def test_atributos_nao_encontrados_energia():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        h = Energiaf.le_arquivo(
-            "",
+        h = Energiaf.read(
+            ARQ_TESTE,
             numero_forwards=NUM_FORWARDS,
             numero_rees=NUM_REES,
             numero_estagios=NUM_ESTAGIOS,
             numero_estagios_th=NUM_ESTAGIOS_TH,
         )
         assert h.series.isna().sum().sum() == NUM_ENTRADAS
 
 
 def test_eq_energia():
-    h1 = Energiaf.le_arquivo(
-        ARQ_TEST,
+    h1 = Energiaf.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
-    h2 = Energiaf.le_arquivo(
-        ARQ_TEST,
+    h2 = Energiaf.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
     assert h1 == h2
```

### Comparing `inewave-0.0.95/tests/newave/test_energias.py` & `inewave-0.0.96/tests/newave/test_energias.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,71 +2,71 @@
 from inewave.newave.energias import Energias
 
 from os.path import join
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
-ARQ_TEST = "./tests/mocks/arquivos"
+ARQ_TESTE = "./tests/mocks/arquivos/energias.dat"
 
 NUM_SERIES = 2
 NUM_REES = 1
 NUM_ESTAGIOS = 16
 NUM_ESTAGIOS_TH = 12
 NUM_ENTRADAS = NUM_SERIES * NUM_REES * (NUM_ESTAGIOS_TH + NUM_ESTAGIOS)
 
 
 def test_secao_energia():
     r = SecaoDadosEnergias()
-    with open(join(ARQ_TEST, "energias.dat"), "rb") as fp:
+    with open(ARQ_TESTE, "rb") as fp:
         r.read(
             fp,
             numero_series=NUM_SERIES,
             numero_rees=NUM_REES,
             numero_estagios=NUM_ESTAGIOS,
             numero_estagios_th=NUM_ESTAGIOS_TH,
         )
 
     assert len(r.data) == NUM_ENTRADAS
 
 
 def test_atributos_encontrados_energia():
-    h = Energias.le_arquivo(
-        ARQ_TEST,
+    h = Energias.read(
+        ARQ_TESTE,
         numero_series=NUM_SERIES,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
     assert h.series is not None
     assert h.series.isna().sum().sum() == 0
 
 
 def test_atributos_nao_encontrados_energia():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        h = Energias.le_arquivo(
-            "",
+        h = Energias.read(
+            ARQ_TESTE,
             numero_series=NUM_SERIES,
             numero_rees=NUM_REES,
             numero_estagios=NUM_ESTAGIOS,
             numero_estagios_th=NUM_ESTAGIOS_TH,
         )
         assert h.series.isna().sum().sum() == NUM_ENTRADAS
 
 
 def test_eq_energia():
-    h1 = Energias.le_arquivo(
-        ARQ_TEST,
+    h1 = Energias.read(
+        ARQ_TESTE,
         numero_series=NUM_SERIES,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
-    h2 = Energias.le_arquivo(
-        ARQ_TEST,
+    h2 = Energias.read(
+        ARQ_TESTE,
         numero_series=NUM_SERIES,
         numero_rees=NUM_REES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
     assert h1 == h2
```

### Comparing `inewave-0.0.95/tests/newave/test_engnat.py` & `inewave-0.0.96/tests/newave/test_engnat.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,65 +2,65 @@
 from inewave.newave.engnat import Engnat
 from inewave.config import MAX_ANOS_HISTORICO
 from os.path import join
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
-ARQ_TEST = "./tests/mocks/arquivos"
+ARQ_TESTE = "./tests/mocks/arquivos/engnat.dat"
 
 NUM_CONFIGURACOES = 1
 NUM_REES = 12
 ANO_INICIO_HISTORICO = 1931
 NUM_ENTRADAS = NUM_CONFIGURACOES * NUM_REES * 12 * MAX_ANOS_HISTORICO
 
 
 def test_secao_engnat():
     r = SecaoDadosEngnat()
-    with open(join(ARQ_TEST, "engnat.dat"), "rb") as fp:
+    with open(ARQ_TESTE, "rb") as fp:
         r.read(
             fp,
             numero_rees=NUM_REES,
             ano_inicio_historico=ANO_INICIO_HISTORICO,
             numero_configuracoes=NUM_CONFIGURACOES,
         )
 
     assert len(r.data) == NUM_ENTRADAS
 
 
 def test_atributos_encontrados_engnat():
-    h = Engnat.le_arquivo(
-        ARQ_TEST,
+    h = Engnat.read(
+        ARQ_TESTE,
         numero_rees=NUM_REES,
         ano_inicio_historico=ANO_INICIO_HISTORICO,
         numero_configuracoes=NUM_CONFIGURACOES,
     )
     assert h.series is not None
     assert h.series.isna().sum().sum() == 0
 
 
 def test_atributos_nao_encontrados_engnat():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        h = Engnat.le_arquivo(
-            "",
+        h = Engnat.read(
+            ARQ_TESTE,
             numero_rees=NUM_REES,
             ano_inicio_historico=ANO_INICIO_HISTORICO,
             numero_configuracoes=NUM_CONFIGURACOES,
         )
         assert h.series.isna().sum().sum() == NUM_ENTRADAS
 
 
 def test_eq_engnat():
-    h1 = Engnat.le_arquivo(
-        ARQ_TEST,
+    h1 = Engnat.read(
+        ARQ_TESTE,
         numero_rees=NUM_REES,
         ano_inicio_historico=ANO_INICIO_HISTORICO,
         numero_configuracoes=NUM_CONFIGURACOES,
     )
-    h2 = Engnat.le_arquivo(
-        ARQ_TEST,
+    h2 = Engnat.read(
+        ARQ_TESTE,
         numero_rees=NUM_REES,
         ano_inicio_historico=ANO_INICIO_HISTORICO,
         numero_configuracoes=NUM_CONFIGURACOES,
     )
     assert h1 == h2
```

### Comparing `inewave-0.0.95/tests/newave/test_eolicacadastro.py` & `inewave-0.0.96/tests/newave/test_eolicacadastro.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,17 +22,18 @@
     MockRegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo,
     MockRegistroEolicaConjuntoAerogeradoresPotenciaEfetiva,
     MockRegistroPEECadastro,
     MockRegistroPEEPotenciaInstaladaPeriodo,
     MockEolicaCadastro,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_registro_eolica_cadastro_eolicacadastro():
 
+def test_registro_eolica_cadastro_eolicacadastro():
     m: MagicMock = mock_open(read_data="".join(MockRegistroEolicaCadastro))
     r = RegistroEolicaCadastro()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [1, "NEInterior", "", 1]
@@ -43,15 +44,14 @@
     assert r.identificador_eolica == ""
     r.identificador_eolica = "   "
     assert r.quantidade_conjuntos == 1
     r.quantidade_conjuntos = 5
 
 
 def test_registro_cadastro_aerogerador_eolicacadastro():
-
     m: MagicMock = mock_open(
         read_data="".join(MockRegistroEolicaCadastroAerogerador)
     )
     r = RegistroEolicaCadastroAerogerador()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -74,15 +74,14 @@
     assert r.potencia_velocidade_cutout == 0
     r.potencia_velocidade_cutout = 10000
     assert r.altura_torre == 0
     r.altura_torre = 100
 
 
 def test_registro_cadastro_conjunto_eolicacadastro():
-
     m: MagicMock = mock_open(
         read_data="".join(MockRegistroEolicaCadastroConjuntoAerogeradores)
     )
     r = RegistroEolicaCadastroConjuntoAerogeradores()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -95,15 +94,14 @@
     assert r.nome_conjunto == "NEInterior_cj"
     r.nome_conjunto = "Teste"
     assert r.quantidade_aerogeradores == 1
     r.quantidade_aerogeradores = 2
 
 
 def test_registro_cadastro_operacao_eolicacadastro():
-
     m: MagicMock = mock_open(
         read_data="".join(
             MockRegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo
         )
     )
     r = RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo()
     with patch("builtins.open", m):
@@ -120,15 +118,14 @@
     assert r.periodo_final == datetime(2030, 12, 1)
     r.periodo_final = datetime(2025, 12, 1)
     assert r.numero_aerogeradores == 1
     r.numero_aerogeradores = 3
 
 
 def test_registro_potenciaefetiva_eolicacadastro():
-
     m: MagicMock = mock_open(
         read_data="".join(
             MockRegistroEolicaConjuntoAerogeradoresPotenciaEfetiva
         )
     )
     r = RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva()
     with patch("builtins.open", m):
@@ -151,30 +148,28 @@
     assert r.periodo_final == datetime(2030, 12, 1)
     r.periodo_final = datetime(2025, 12, 1)
     assert r.potencia_efetiva == 6058.890
     r.potencia_efetiva = 5
 
 
 def test_registro_pee_cadastro():
-
     m: MagicMock = mock_open(read_data="".join(MockRegistroPEECadastro))
     r = RegistroPEECadastro()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [1, "NEInterior"]
     assert r.codigo_pee == 1
     r.codigo_pee = 2
     assert r.nome_pee == "NEInterior"
     r.nome_pee = "NEInterior"
 
 
 def test_registro_pee_potencia_instalada_periodo():
-
     m: MagicMock = mock_open(
         read_data="".join(MockRegistroPEEPotenciaInstaladaPeriodo)
     )
     r = RegistroPEEPotenciaInstaladaPeriodo()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -194,15 +189,15 @@
     assert r.potencia_instalada == 6058.89
     r.potencia_instalada = 1000.0
 
 
 def test_atributos_encontrados_eolicacadastro():
     m: MagicMock = mock_open(read_data="".join(MockEolicaCadastro))
     with patch("builtins.open", m):
-        e = EolicaCadastro.le_arquivo("")
+        e = EolicaCadastro.read(ARQ_TESTE)
         assert len(e.eolica_cadastro()) > 0
         assert len(e.eolica_cadastro_aerogerador()) > 0
         assert len(e.eolica_cadastro_conjunto_aerogeradores()) > 0
         assert (
             len(e.eolica_conjunto_aerogeradores_quantidade_operando_periodo())
             > 0
         )
@@ -210,37 +205,37 @@
             len(e.eolica_conjunto_aerogeradores_potencia_efetiva_periodo()) > 0
         )
 
 
 def test_eq_eolicacadastro():
     m: MagicMock = mock_open(read_data="".join(MockEolicaCadastro))
     with patch("builtins.open", m):
-        cf1 = EolicaCadastro.le_arquivo("")
-        cf2 = EolicaCadastro.le_arquivo("")
+        cf1 = EolicaCadastro.read(ARQ_TESTE)
+        cf2 = EolicaCadastro.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_eolicacadastro():
     m: MagicMock = mock_open(read_data="".join(MockEolicaCadastro))
     with patch("builtins.open", m):
-        cf1 = EolicaCadastro.le_arquivo("")
-        cf2 = EolicaCadastro.le_arquivo("")
+        cf1 = EolicaCadastro.read(ARQ_TESTE)
+        cf2 = EolicaCadastro.read(ARQ_TESTE)
         cf2.deleta_registro(cf1.eolica_cadastro()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicacadastro():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaCadastro))
     with patch("builtins.open", m_leitura):
-        cf1 = EolicaCadastro.le_arquivo("")
+        cf1 = EolicaCadastro.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = EolicaCadastro.le_arquivo("")
+        cf2 = EolicaCadastro.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_eolicaconfiguracao.py` & `inewave-0.0.96/tests/newave/test_eolicaconfiguracao.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 from tests.mocks.arquivos.eolicaconfig import (
     MockRegistroEolicaConfiguracaoPeriodo,
     MockRegistroPEEConfiguracaoPeriodo,
     MockEolicaConfig,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_registro_eolica_configuracao_periodo_eolicaconfig():
 
+def test_registro_eolica_configuracao_periodo_eolicaconfig():
     m: MagicMock = mock_open(
         read_data="".join(MockRegistroEolicaConfiguracaoPeriodo)
     )
     r = RegistroEolicaConfiguracao()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -40,15 +41,14 @@
     assert r.data_final_estado_operacao == datetime(2030, 12, 1)
     r.data_final_estado_operacao = datetime(2030, 11, 1)
     assert r.estado_operacao == "centralizado"
     r.estado_operacao = "fixo"
 
 
 def test_registro_pee_configuracao_periodo_eolicaconfig():
-
     m: MagicMock = mock_open(
         read_data="".join(MockRegistroPEEConfiguracaoPeriodo)
     )
     r = RegistroPEEConfiguracaoPeriodo()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -68,44 +68,44 @@
     assert r.estado_operacao == "centralizado"
     r.estado_operacao = "fixo"
 
 
 def test_atributos_encontrados_eolicaconfig():
     m: MagicMock = mock_open(read_data="".join(MockEolicaConfig))
     with patch("builtins.open", m):
-        e = EolicaConfiguracao.le_arquivo("")
+        e = EolicaConfiguracao.read(ARQ_TESTE)
         assert len(e.eolica_configuracao()) > 0
 
 
 def test_eq_eolicaconfig():
     m: MagicMock = mock_open(read_data="".join(MockEolicaConfig))
     with patch("builtins.open", m):
-        cf1 = EolicaConfiguracao.le_arquivo("")
-        cf2 = EolicaConfiguracao.le_arquivo("")
+        cf1 = EolicaConfiguracao.read(ARQ_TESTE)
+        cf2 = EolicaConfiguracao.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_eolicaconfig():
     m: MagicMock = mock_open(read_data="".join(MockEolicaConfig))
     with patch("builtins.open", m):
-        cf1 = EolicaConfiguracao.le_arquivo("")
-        cf2 = EolicaConfiguracao.le_arquivo("")
+        cf1 = EolicaConfiguracao.read(ARQ_TESTE)
+        cf2 = EolicaConfiguracao.read(ARQ_TESTE)
         cf2.deleta_registro(cf1.eolica_configuracao()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicaconfig():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaConfig))
     with patch("builtins.open", m_leitura):
-        cf1 = EolicaConfiguracao.le_arquivo("")
+        cf1 = EolicaConfiguracao.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = EolicaConfiguracao.le_arquivo("")
+        cf2 = EolicaConfiguracao.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_eolicafte.py` & `inewave-0.0.96/tests/newave/test_eolicafte.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 from tests.mocks.arquivos.eolicafte import (
     MockRegistroFuncaoProducao,
     MockEolicaFTE,
     MockRegistroPEEFTE,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_registro_eolica_funcao_producao_eolicafte():
     m: MagicMock = mock_open(read_data="".join(MockRegistroFuncaoProducao))
     r = RegistroEolicaFTE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -65,44 +67,44 @@
     assert r.coeficiente_angular == 0.10904637648150100
     r.coeficiente_angular = 0.5
 
 
 def test_atributos_encontrados_eolicafte():
     m: MagicMock = mock_open(read_data="".join(MockEolicaFTE))
     with patch("builtins.open", m):
-        e = EolicaFTE.le_arquivo("")
+        e = EolicaFTE.read(ARQ_TESTE)
         assert len(e.eolica_funcao_producao()) > 0
 
 
 def test_eq_eolicafte():
     m: MagicMock = mock_open(read_data="".join(MockEolicaFTE))
     with patch("builtins.open", m):
-        cf1 = EolicaFTE.le_arquivo("")
-        cf2 = EolicaFTE.le_arquivo("")
+        cf1 = EolicaFTE.read(ARQ_TESTE)
+        cf2 = EolicaFTE.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_eolicafte():
     m: MagicMock = mock_open(read_data="".join(MockEolicaFTE))
     with patch("builtins.open", m):
-        cf1 = EolicaFTE.le_arquivo("")
-        cf2 = EolicaFTE.le_arquivo("")
+        cf1 = EolicaFTE.read(ARQ_TESTE)
+        cf2 = EolicaFTE.read(ARQ_TESTE)
         cf2.deleta_registro(cf1.eolica_funcao_producao()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicafte():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaFTE))
     with patch("builtins.open", m_leitura):
-        cf1 = EolicaFTE.le_arquivo("")
+        cf1 = EolicaFTE.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = EolicaFTE.le_arquivo("")
+        cf2 = EolicaFTE.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_eolicageracao.py` & `inewave-0.0.96/tests/newave/test_eolicageracao.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 from tests.mocks.arquivos.eolicageracao import (
     MockRegistroEolicaGeracaoPatamar,
     MockEolicaGeracao,
     MockRegistroPEEGeracaoPatamar,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_registro_eolica_geracao_patamar_eolicageracao():
 
+def test_registro_eolica_geracao_patamar_eolicageracao():
     m: MagicMock = mock_open(
         read_data="".join(MockRegistroEolicaGeracaoPatamar)
     )
     r = RegistroEolicaGeracaoPatamar()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -37,15 +38,14 @@
     assert r.indice_patamar == 2
     r.indice_patamar = 1
     assert r.profundidade == 1.0496
     r.profundidade = 2.0
 
 
 def test_registro_pee_geracao_patamar_eolicageracao():
-
     m: MagicMock = mock_open(read_data="".join(MockRegistroPEEGeracaoPatamar))
     r = RegistroPEEGeracaoPatamar()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [1, datetime(2021, 1, 1), datetime(2021, 1, 1), 1, 0.88]
@@ -60,46 +60,46 @@
     assert r.profundidade == 0.88
     r.profundidade = 2.0
 
 
 def test_atributos_encontrados_eolicageracao():
     m: MagicMock = mock_open(read_data="".join(MockEolicaGeracao))
     with patch("builtins.open", m):
-        e = EolicaGeracao.le_arquivo("")
+        e = EolicaGeracao.read(ARQ_TESTE)
         assert len(e.eolica_geracao_profundidade_periodo_patamar()) > 0
 
 
 def test_eq_eolicageracao():
     m: MagicMock = mock_open(read_data="".join(MockEolicaGeracao))
     with patch("builtins.open", m):
-        cf1 = EolicaGeracao.le_arquivo("")
-        cf2 = EolicaGeracao.le_arquivo("")
+        cf1 = EolicaGeracao.read(ARQ_TESTE)
+        cf2 = EolicaGeracao.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_eolicageracao():
     m: MagicMock = mock_open(read_data="".join(MockEolicaGeracao))
     with patch("builtins.open", m):
-        cf1 = EolicaGeracao.le_arquivo("")
-        cf2 = EolicaGeracao.le_arquivo("")
+        cf1 = EolicaGeracao.read(ARQ_TESTE)
+        cf2 = EolicaGeracao.read(ARQ_TESTE)
         cf2.deleta_registro(
             cf1.eolica_geracao_profundidade_periodo_patamar()[0]
         )
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicageracao():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaGeracao))
     with patch("builtins.open", m_leitura):
-        cf1 = EolicaGeracao.le_arquivo("")
+        cf1 = EolicaGeracao.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = EolicaGeracao.le_arquivo("")
+        cf2 = EolicaGeracao.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_eolicahistorico.py` & `inewave-0.0.96/tests/newave/test_eolicahistorico.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,17 +16,18 @@
     MockRegistroEolicaHistoricoHorizonte,
     MockRegistroEolicaHistorico,
     MockRegistroHistoricoVentoHorizonte,
     MockRegistroHistoricoVento,
     MockEolicaHistorico,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_registro_eolica_historico_horizonte_eolicahistorico():
 
+def test_registro_eolica_historico_horizonte_eolicahistorico():
     m: MagicMock = mock_open(
         read_data="".join(MockRegistroEolicaHistoricoHorizonte)
     )
     r = RegistroEolicaHistoricoVentoHorizonte()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -35,15 +36,14 @@
     assert r.data_inicial == datetime(1979, 1, 1)
     r.data_inicial = datetime(1980, 1, 1)
     assert r.data_final == datetime(2016, 1, 1)
     r.data_final = datetime(2018, 1, 1)
 
 
 def test_registro_eolica_historico_eolicahistorico():
-
     m: MagicMock = mock_open(read_data="".join(MockRegistroEolicaHistorico))
     r = RegistroEolicaHistoricoVento()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [1, datetime(1979, 1, 1), datetime(1979, 2, 1), 3.43, 1.0]
@@ -56,15 +56,14 @@
     assert r.velocidade == 3.43
     r.velocidade = 5.0
     assert r.direcao == 1.0
     r.direcao = 0.0
 
 
 def test_registro_historico_vento_horizonte_eolicahistorico():
-
     m: MagicMock = mock_open(
         read_data="".join(MockRegistroHistoricoVentoHorizonte)
     )
     r = RegistroHistoricoVentoHorizonte()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -73,15 +72,14 @@
     assert r.data_inicial == datetime(1979, 1, 1)
     r.data_inicial = datetime(1980, 1, 1)
     assert r.data_final == datetime(2016, 1, 1)
     r.data_final = datetime(2018, 1, 1)
 
 
 def test_registro_historico_vento_eolicahistorico():
-
     m: MagicMock = mock_open(read_data="".join(MockRegistroHistoricoVento))
     r = RegistroHistoricoVento()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [1, datetime(1979, 1, 1), datetime(1979, 2, 1), 4.05, 1.0]
@@ -96,44 +94,44 @@
     assert r.direcao == 1.0
     r.direcao = 0.0
 
 
 def test_atributos_encontrados_eolicahistorico():
     m: MagicMock = mock_open(read_data="".join(MockEolicaHistorico))
     with patch("builtins.open", m):
-        e = EolicaHistorico.le_arquivo("")
+        e = EolicaHistorico.read(ARQ_TESTE)
         assert len(e.eolica_historico_vento()) > 0
 
 
 def test_eq_eolicahistorico():
     m: MagicMock = mock_open(read_data="".join(MockEolicaHistorico))
     with patch("builtins.open", m):
-        cf1 = EolicaHistorico.le_arquivo("")
-        cf2 = EolicaHistorico.le_arquivo("")
+        cf1 = EolicaHistorico.read(ARQ_TESTE)
+        cf2 = EolicaHistorico.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_eolicahistorico():
     m: MagicMock = mock_open(read_data="".join(MockEolicaHistorico))
     with patch("builtins.open", m):
-        cf1 = EolicaHistorico.le_arquivo("")
-        cf2 = EolicaHistorico.le_arquivo("")
+        cf1 = EolicaHistorico.read(ARQ_TESTE)
+        cf2 = EolicaHistorico.read(ARQ_TESTE)
         cf2.deleta_registro(cf1.eolica_historico_vento()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicahistorico():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaHistorico))
     with patch("builtins.open", m_leitura):
-        cf1 = EolicaHistorico.le_arquivo("")
+        cf1 = EolicaHistorico.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = EolicaHistorico.le_arquivo("")
+        cf2 = EolicaHistorico.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_eolicaposto.py` & `inewave-0.0.96/tests/newave/test_eolicaposto.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 
 from tests.mocks.arquivos.eolicaposto import (
     MockRegistroPostoCadastro,
     MockRegistroPEEPosto,
     MockEolicaPosto,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_registro_posto_cadastro_eolicaposto():
 
+def test_registro_posto_cadastro_eolicaposto():
     m: MagicMock = mock_open(read_data="".join(MockRegistroPostoCadastro))
     r = RegistroPostoVentoCadastro()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [1, "NEInterior"]
     assert r.codigo_posto == 1
     r.codigo_posto = 1
     assert r.nome_posto == "NEInterior"
     r.nome_posto = "NEInterior"
 
 
 def test_registro_pee_posto_eolicaposto():
-
     m: MagicMock = mock_open(read_data="".join(MockRegistroPEEPosto))
     r = RegistroPEEPostoVento()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [1, 1]
@@ -46,45 +46,45 @@
     assert r.codigo_pee == 1
     r.codigo_pee = 2
 
 
 def test_atributos_encontrados_eolicaposto():
     m: MagicMock = mock_open(read_data="".join(MockEolicaPosto))
     with patch("builtins.open", m):
-        e = EolicaPosto.le_arquivo("")
+        e = EolicaPosto.read(ARQ_TESTE)
         assert len(e.posto_vento_cad()) > 0
         assert len(e.pee_posto()) > 0
 
 
 def test_eq_eolicaposto():
     m: MagicMock = mock_open(read_data="".join(MockEolicaPosto))
     with patch("builtins.open", m):
-        cf1 = EolicaPosto.le_arquivo("")
-        cf2 = EolicaPosto.le_arquivo("")
+        cf1 = EolicaPosto.read(ARQ_TESTE)
+        cf2 = EolicaPosto.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_eolicaposto():
     m: MagicMock = mock_open(read_data="".join(MockEolicaPosto))
     with patch("builtins.open", m):
-        cf1 = EolicaPosto.le_arquivo("")
-        cf2 = EolicaPosto.le_arquivo("")
+        cf1 = EolicaPosto.read(ARQ_TESTE)
+        cf2 = EolicaPosto.read(ARQ_TESTE)
         cf2.deleta_registro(cf1.posto_vento_cad()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicaposto():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaPosto))
     with patch("builtins.open", m_leitura):
-        cf1 = EolicaPosto.le_arquivo("")
+        cf1 = EolicaPosto.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = EolicaPosto.le_arquivo("")
+        cf2 = EolicaPosto.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_eolicasubmercado.py` & `inewave-0.0.96/tests/newave/test_eolicasubmercado.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 
 from tests.mocks.arquivos.eolicasubmercado import (
     MockRegistroEolicaSubmercado,
     MockRegistroPEESubmercado,
     MockEolicaSubmercado,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_registro_eolica_submercado_eolicasubmercado():
 
+def test_registro_eolica_submercado_eolicasubmercado():
     m: MagicMock = mock_open(read_data="".join(MockRegistroEolicaSubmercado))
     r = RegistroEolicaSubmercado()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [5, 2]
     assert r.codigo_eolica == 5
     r.codigo_eolica = 2
     assert r.codigo_submercado == 2
     r.codigo_submercado = 1
 
 
 def test_registro_pee_submercado_eolicasubmercado():
-
     m: MagicMock = mock_open(read_data="".join(MockRegistroPEESubmercado))
     r = RegistroPEESubmercado()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [1, 3]
@@ -45,44 +45,44 @@
     assert r.codigo_submercado == 3
     r.codigo_submercado = 1
 
 
 def test_atributos_encontrados_eolicasubmercado():
     m: MagicMock = mock_open(read_data="".join(MockEolicaSubmercado))
     with patch("builtins.open", m):
-        e = EolicaSubmercado.le_arquivo("")
+        e = EolicaSubmercado.read(ARQ_TESTE)
         assert len(e.eolica_submercado()) > 0
 
 
 def test_eq_eolicasubmercado():
     m: MagicMock = mock_open(read_data="".join(MockEolicaSubmercado))
     with patch("builtins.open", m):
-        cf1 = EolicaSubmercado.le_arquivo("")
-        cf2 = EolicaSubmercado.le_arquivo("")
+        cf1 = EolicaSubmercado.read(ARQ_TESTE)
+        cf2 = EolicaSubmercado.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_eolicasubmercado():
     m: MagicMock = mock_open(read_data="".join(MockEolicaSubmercado))
     with patch("builtins.open", m):
-        cf1 = EolicaSubmercado.le_arquivo("")
-        cf2 = EolicaSubmercado.le_arquivo("")
+        cf1 = EolicaSubmercado.read(ARQ_TESTE)
+        cf2 = EolicaSubmercado.read(ARQ_TESTE)
         cf2.deleta_registro(cf1.eolica_submercado()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicasubmercado():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaSubmercado))
     with patch("builtins.open", m_leitura):
-        cf1 = EolicaSubmercado.le_arquivo("")
+        cf1 = EolicaSubmercado.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = EolicaSubmercado.le_arquivo("")
+        cf2 = EolicaSubmercado.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_modif.py` & `inewave-0.0.96/tests/newave/test_modif.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,57 +32,55 @@
     MockCMONT,
     MockVMAXT,
     MockVMINT,
     MockVMINP,
     MockVAZMINT,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_registro_usina_modif():
 
+def test_registro_usina_modif():
     m: MagicMock = mock_open(read_data="".join(MockUSINA))
     r = USINA()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [1, "CAMARGOS"]
     assert r.codigo == 1
     assert r.nome == "CAMARGOS"
 
 
 def test_registro_vazmin_modif():
-
     m: MagicMock = mock_open(read_data="".join(MockVAZMIN))
     r = VAZMIN()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [34]
     assert r.vazao == 34
 
 
 def test_registro_vmaxt_modif():
-
     m: MagicMock = mock_open(read_data="".join(MockVMAXT))
     r = VMAXT()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [12, 2021, 61.310, "'%'"]
     assert r.mes == 12
     assert r.ano == 2021
     assert r.volume == 61.310
     assert r.unidade == "'%'"
 
 
 def test_registro_vazmint_modif():
-
     m: MagicMock = mock_open(read_data="".join(MockVAZMINT))
     r = VAZMINT()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [10, 2021, 10.00]
@@ -113,84 +111,78 @@
 
 #     assert r.data == [15563.63, "'h'"]
 #     assert r.volume == 15563.63
 #     assert r.unidade == "'h'"
 
 
 def test_registro_numcnj_modif():
-
     m: MagicMock = mock_open(read_data="".join(MockNUMCNJ))
     r = NUMCNJ()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [2]
     assert r.numero == 2
 
 
 def test_registro_nummaq_modif():
-
     m: MagicMock = mock_open(read_data="".join(MockNUMMAQ))
     r = NUMMAQ()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [2, 5]
     assert r.conjunto == 2
     assert r.numero_maquinas == 5
 
 
 def test_registro_vmint_modif():
-
     m: MagicMock = mock_open(read_data="".join(MockVMINT))
     r = VMINT()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [10, 2021, 20.0, "'%'"]
     assert r.mes == 10
     assert r.ano == 2021
     assert r.volume == 20.0
     assert r.unidade == "'%'"
 
 
 def test_registro_vminp_modif():
-
     m: MagicMock = mock_open(read_data="".join(MockVMINP))
     r = VMINP()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [10, 2021, 20.0, "'%'"]
     assert r.mes == 10
     assert r.ano == 2021
     assert r.volume == 20.0
     assert r.unidade == "'%'"
 
 
 def test_registro_cfuga_modif():
-
     m: MagicMock = mock_open(read_data="".join(MockCFUGA))
     r = CFUGA()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [10, 2021, 5.60]
     assert r.mes == 10
     assert r.ano == 2021
     assert r.nivel == 5.60
 
 
 def test_registro_cmont_modif():
-
     m: MagicMock = mock_open(read_data="".join(MockCMONT))
     r = CMONT()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
 
     assert r.data == [10, 2021, 71.30]
@@ -198,15 +190,15 @@
     assert r.ano == 2021
     assert r.nivel == 71.30
 
 
 def test_atributos_encontrados_modif():
     m: MagicMock = mock_open(read_data="".join(MockModif))
     with patch("builtins.open", m):
-        ad = Modif.le_arquivo("")
+        ad = Modif.read(ARQ_TESTE)
         assert len(ad.usina()) > 0
         assert len(ad.vazmin()) > 0
         assert len(ad.vmaxt()) > 0
         assert len(ad.vazmint()) > 0
         assert isinstance(ad.volmin(), VOLMIN)
         assert isinstance(ad.volmax(), VOLMAX)
         assert len(ad.numcnj()) > 0
@@ -216,37 +208,37 @@
         assert len(ad.cfuga()) > 0
         assert len(ad.cmont()) > 0
 
 
 # def test_eq_patamar():
 #     m: MagicMock = mock_open(read_data="".join(MockPatamar))
 #     with patch("builtins.open", m):
-#         cf1 = Patamar.le_arquivo("")
-#         cf2 = Patamar.le_arquivo("")
+#         cf1 = Patamar.read(ARQ_TESTE)
+#         cf2 = Patamar.read(ARQ_TESTE)
 #         assert cf1 == cf2
 
 
 # def test_neq_patamar():
 #     m: MagicMock = mock_open(read_data="".join(MockPatamar))
 #     with patch("builtins.open", m):
-#         cf1 = Patamar.le_arquivo("")
-#         cf2 = Patamar.le_arquivo("")
+#         cf1 = Patamar.read(ARQ_TESTE)
+#         cf2 = Patamar.read(ARQ_TESTE)
 #         cf2.numero_patamares = 0
 #         assert cf1 != cf2
 
 
 # def test_leitura_escrita_patamar():
 #     m_leitura: MagicMock = mock_open(read_data="".join(MockPatamar))
 #     with patch("builtins.open", m_leitura):
-#         cf1 = Patamar.le_arquivo("")
+#         cf1 = Patamar.read(ARQ_TESTE)
 #     m_escrita: MagicMock = mock_open(read_data="")
 #     with patch("builtins.open", m_escrita):
-#         cf1.escreve_arquivo("", "")
+#         cf1.write(ARQ_TESTE)
 #         # Recupera o que foi escrito
 #         chamadas = m_escrita.mock_calls
 #         linhas_escritas = [
 #             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
 #         ]
 #     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
 #     with patch("builtins.open", m_releitura):
-#         cf2 = Patamar.le_arquivo("")
+#         cf2 = Patamar.read(ARQ_TESTE)
 #         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_newavetim.py` & `inewave-0.0.96/tests/newave/test_newavetim.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.newavetim import MockBlocoTemposEtapas, MockNewaveTim
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_tempos_etapas():
 
+def test_tempos_etapas():
     m: MagicMock = mock_open(read_data="".join(MockBlocoTemposEtapas))
     b = BlocoTemposEtapasTim()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 5
@@ -25,33 +26,33 @@
     assert b.data.iloc[0, 0] == "Leitura de Dados"
     assert b.data.iloc[-1, -1] == timedelta(hours=3, minutes=26, seconds=7)
 
 
 def test_atributos_encontrados_newavetim():
     m: MagicMock = mock_open(read_data="".join(MockNewaveTim))
     with patch("builtins.open", m):
-        nt = NewaveTim.le_arquivo("")
+        nt = NewaveTim.read(ARQ_TESTE)
         assert nt.tempos_etapas is not None
 
 
 def test_atributos_nao_encontrados_newavetim():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        nt = NewaveTim.le_arquivo("")
+        nt = NewaveTim.read(ARQ_TESTE)
         assert nt.tempos_etapas is None
 
 
 def test_eq_newavetim():
     m: MagicMock = mock_open(read_data="".join(MockNewaveTim))
     with patch("builtins.open", m):
-        nt1 = NewaveTim.le_arquivo("")
-        nt2 = NewaveTim.le_arquivo("")
+        nt1 = NewaveTim.read(ARQ_TESTE)
+        nt2 = NewaveTim.read(ARQ_TESTE)
         assert nt1 == nt2
 
 
 def test_neq_newavetim():
     m: MagicMock = mock_open(read_data="".join(MockNewaveTim))
     with patch("builtins.open", m):
-        nt1 = NewaveTim.le_arquivo("")
-        nt2 = NewaveTim.le_arquivo("")
+        nt1 = NewaveTim.read(ARQ_TESTE)
+        nt2 = NewaveTim.read(ARQ_TESTE)
         nt2.tempos_etapas.iloc[0, 0] = ""
         assert nt1 != nt2
```

### Comparing `inewave-0.0.95/tests/newave/test_nwv_avl_evap.py` & `inewave-0.0.96/tests/newave/test_nwv_avl_evap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from inewave.newave.nwv_avl_evap import NwvAvlEvap
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.nwv_avl_evap import MockNwvAvlEvap
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_nwv_avl_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvAvlEvap))
     with patch("builtins.open", m):
-        rel = NwvAvlEvap.le_arquivo("")
+        rel = NwvAvlEvap.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
         assert rel.tabela.at[0, "periodo"] == 1
         assert rel.tabela.at[0, "indice_usina"] == 4
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert rel.tabela.at[0, "volume_armazenado_hm3"] == 265.86
         assert rel.tabela.at[0, "evaporacao_calculada_hm3"] == 0.23
         assert rel.tabela.at[0, "evaporacao_modelo_hm3"] == 0.23
         assert rel.tabela.at[0, "desvio_absoluto_hm3"] == 0.0
         assert rel.tabela.at[0, "desvio_percentual"] == 0.0
 
 
 def test_eq_nwv_avl_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvAvlEvap))
     with patch("builtins.open", m):
-        rel1 = NwvAvlEvap.le_arquivo("")
-        rel2 = NwvAvlEvap.le_arquivo("")
+        rel1 = NwvAvlEvap.read(ARQ_TESTE)
+        rel2 = NwvAvlEvap.read(ARQ_TESTE)
         assert rel1 == rel2
 
 
 def test_neq_nwv_avl_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvAvlEvap))
     with patch("builtins.open", m):
-        rel1 = NwvAvlEvap.le_arquivo("")
-        rel2 = NwvAvlEvap.le_arquivo("")
+        rel1 = NwvAvlEvap.read(ARQ_TESTE)
+        rel2 = NwvAvlEvap.read(ARQ_TESTE)
         rel1.tabela.iloc[0, 0] = -1
         assert rel1 != rel2
```

### Comparing `inewave-0.0.95/tests/newave/test_nwv_cortes_evap.py` & `inewave-0.0.96/tests/newave/test_nwv_cortes_evap.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from inewave.newave.nwv_cortes_evap import NwvCortesEvap
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.nwv_cortes_evap import MockNwvCortesEvap
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_nwv_cortes_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvCortesEvap))
     with patch("builtins.open", m):
-        rel = NwvCortesEvap.le_arquivo("")
+        rel = NwvCortesEvap.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
         assert rel.tabela.at[0, "periodo"] == 1
         assert rel.tabela.at[0, "indice_usina"] == 4
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert rel.tabela.at[0, "derivada_cota_area"] == 0.0000000000
         assert rel.tabela.at[0, "derivada_volume_cota"] == 0.0000000000
         assert rel.tabela.at[0, "volume_referencia_hm3"] == 265.86
@@ -21,19 +23,19 @@
         assert rel.tabela.at[0, "coeficiente_volume"] == 0.0000000000
         assert rel.tabela.at[0, "rhs_volume"] == 0.2263
 
 
 def test_eq_nwv_cortes_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvCortesEvap))
     with patch("builtins.open", m):
-        rel1 = NwvCortesEvap.le_arquivo("")
-        rel2 = NwvCortesEvap.le_arquivo("")
+        rel1 = NwvCortesEvap.read(ARQ_TESTE)
+        rel2 = NwvCortesEvap.read(ARQ_TESTE)
         assert rel1 == rel2
 
 
 def test_neq_nwv_cortes_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvCortesEvap))
     with patch("builtins.open", m):
-        rel1 = NwvCortesEvap.le_arquivo("")
-        rel2 = NwvCortesEvap.le_arquivo("")
+        rel1 = NwvCortesEvap.read(ARQ_TESTE)
+        rel2 = NwvCortesEvap.read(ARQ_TESTE)
         rel1.tabela.iloc[0, 0] = -1
         assert rel1 != rel2
```

### Comparing `inewave-0.0.95/tests/newave/test_nwv_eco_evap.py` & `inewave-0.0.96/tests/newave/test_nwv_eco_evap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from inewave.newave.nwv_eco_evap import NwvEcoEvap
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.nwv_eco_evap import MockNwvEcoEvap
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_nwv_eco_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvEcoEvap))
     with patch("builtins.open", m):
-        rel = NwvEcoEvap.le_arquivo("")
+        rel = NwvEcoEvap.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
         assert rel.tabela.at[0, "periodo"] == 1
         assert rel.tabela.at[0, "indice_usina"] == 4
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert rel.tabela.at[0, "volume_referencia_hm3"] == 265.86
         assert rel.tabela.at[0, "evaporacao_referencia_hm3"] == 0.23
         assert rel.tabela.at[0, "coeficiente_evaporacao_mm_mes"] == 6
@@ -21,19 +23,19 @@
         assert rel.tabela.at[0, "evaporacao_linear"] == 1
         assert rel.tabela.at[0, "tipo_volume_referencia"] == 1
 
 
 def test_eq_nwv_eco_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvEcoEvap))
     with patch("builtins.open", m):
-        rel1 = NwvEcoEvap.le_arquivo("")
-        rel2 = NwvEcoEvap.le_arquivo("")
+        rel1 = NwvEcoEvap.read(ARQ_TESTE)
+        rel2 = NwvEcoEvap.read(ARQ_TESTE)
         assert rel1 == rel2
 
 
 def test_neq_nwv_eco_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvEcoEvap))
     with patch("builtins.open", m):
-        rel1 = NwvEcoEvap.le_arquivo("")
-        rel2 = NwvEcoEvap.le_arquivo("")
+        rel1 = NwvEcoEvap.read(ARQ_TESTE)
+        rel2 = NwvEcoEvap.read(ARQ_TESTE)
         rel1.tabela.iloc[0, 0] = -1
         assert rel1 != rel2
```

### Comparing `inewave-0.0.95/tests/newave/test_parp.py` & `inewave-0.0.96/tests/newave/test_parp.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,31 +29,31 @@
     MockSerieMedia12MesesREE,
     MockCorrelCruzadaMedia12Meses,
     MockCorrelEspacialAnual,
     MockCorrelEspacialMensal,
     MockPARp,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_series_energia_ree():
 
+def test_series_energia_ree():
     m: MagicMock = mock_open(read_data="".join(MockSeriesEnergiaPARp))
     b = BlocoSerieEnergiaREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 87
     assert b.data.shape[1] == 15
     assert b.data.iloc[0, 3] == 8536.82
     assert b.data.iloc[-1, -1] == 5616.44
 
 
 def test_correlacao_series_energia_ree():
-
     m: MagicMock = mock_open(
         read_data="".join(MockCorrelacaoSeriesEnergiasREE)
     )
     b = BlocoCorrelEnergiasREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
@@ -61,15 +61,14 @@
     assert b.data.shape[0] == 120
     assert b.data.shape[1] == 12
     assert b.data.iloc[0, 1] == 0.28570
     assert b.data.iloc[-1, -1] == 0.04142
 
 
 def test_correlacao_parcial_series_energia_ree():
-
     m: MagicMock = mock_open(
         read_data="".join(MockCorrelacaoParcialSeriesEnergiaREE)
     )
     b = BlocoCorrelParcialEnergiasREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
@@ -77,29 +76,27 @@
     assert b.data.shape[0] == 120
     assert b.data.shape[1] == 12
     assert b.data.iloc[0, 1] == 0.19220
     assert b.data.iloc[-1, -1] == -0.15513
 
 
 def test_ordem_modelo_ree():
-
     m: MagicMock = mock_open(read_data="".join(MockOrdemOriginalModeloREE))
     b = BlocoOrdemModeloREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 10
     assert b.data.shape[1] == 14
     assert b.data.iloc[0, 2] == 1
     assert b.data.iloc[-1, -1] == 4
 
 
 def test_coeficientes_modelo_ree():
-
     m: MagicMock = mock_open(read_data="".join(MockCoeficientesModeloREE))
     b = BlocoCoeficientesModeloREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 1
@@ -107,85 +104,79 @@
     assert b.data.loc[0, "Psi 1"] == 0.207
     assert b.data.loc[0, "Psi Norm 1"] == 0.263
     assert b.data.loc[0, "Psi A"] == 0.177
     assert b.data.loc[0, "Psi Norm A"] == 0.485
 
 
 def test_serie_ruidos_ree():
-
     m: MagicMock = mock_open(read_data="".join(MockSerieRuidosREE))
     b = BlocoSerieRuidosREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 87
     assert b.data.shape[1] == 14
     assert b.data.iloc[0, 1] == 0.0
     assert b.data.iloc[-1, -1] == -0.152
 
 
 def test_correl_serie_ruidos_ree():
-
     m: MagicMock = mock_open(read_data="".join(MockCorrelSerieRuidosREE))
     b = BlocoCorrelRuidosREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 120
     assert b.data.shape[1] == 12
     assert b.data.iloc[0, 1] == -0.05921
     assert b.data.iloc[-1, -1] == -0.08159
 
 
 def test_serie_media_12_meses_ree():
-
     m: MagicMock = mock_open(read_data="".join(MockSerieMedia12MesesREE))
     b = BlocoSerieMediasREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 87
     assert b.data.shape[1] == 14
     assert b.data.iloc[0, 1] == 0.0000
     assert b.data.iloc[-1, -1] == 3136.70
 
 
 def test_correl_cruzada_media_12_meses_ree():
-
     m: MagicMock = mock_open(read_data="".join(MockCorrelCruzadaMedia12Meses))
     b = BlocoCorrelCruzadaMediaREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 120
     assert b.data.shape[1] == 13
     assert b.data.iloc[0, 1] == 0.26913
     assert b.data.iloc[-1, -1] == 0.76845
 
 
 def test_correl_espacial_anual():
-
     m: MagicMock = mock_open(read_data="".join(MockCorrelEspacialAnual))
     b = BlocoCorrelEspacialAnualConfig()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 12
     assert b.data.shape[1] == 14
     assert b.data.iloc[0, 2] == 1.000
     assert b.data.iloc[-1, -1] == 1.000
 
 
 def test_correl_espacial_mensal():
-
     m: MagicMock = mock_open(read_data="".join(MockCorrelEspacialMensal))
     b = BlocoCorrelEspacialMensalConfig()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 12
@@ -193,15 +184,15 @@
     assert b.data.iloc[0, 3] == 1.0000
     assert b.data.iloc[-1, -1] == 0.0671
 
 
 def test_atributos_encontrados_parp():
     m: MagicMock = mock_open(read_data="".join(MockPARp))
     with patch("builtins.open", m):
-        parp = PARp.le_arquivo("")
+        parp = PARp.read(ARQ_TESTE)
         assert parp.series_energia_ree is not None
         assert parp.correlacao_series_energia_ree is not None
         assert parp.correlacao_parcial_series_energia_ree is not None
         assert parp.ordem_original_modelo is not None
         assert parp.ordem_final_modelo is not None
         assert parp.coeficientes is not None
         assert parp.series_media_ree is not None
@@ -211,15 +202,15 @@
         assert parp.correlacao_espacial_anual is not None
         assert parp.correlacao_espacial_mensal is not None
 
 
 def test_atributos_nao_encontrados_parp():
     m: MagicMock = mock_open(read_data="".join(MockSeriesEnergiaPARp))
     with patch("builtins.open", m):
-        parp = PARp.le_arquivo("")
+        parp = PARp.read(ARQ_TESTE)
         assert parp.series_energia_ree is not None
         assert parp.correlacao_series_energia_ree is None
         assert parp.correlacao_parcial_series_energia_ree is None
         assert parp.ordem_original_modelo is None
         assert parp.ordem_final_modelo is None
         assert parp.coeficientes is None
         assert parp.series_media_ree is None
@@ -229,19 +220,19 @@
         assert parp.correlacao_espacial_anual is None
         assert parp.correlacao_espacial_mensal is None
 
 
 def test_eq_parp():
     m: MagicMock = mock_open(read_data="".join(MockPARp))
     with patch("builtins.open", m):
-        parp1 = PARp.le_arquivo("")
-        parp2 = PARp.le_arquivo("")
+        parp1 = PARp.read(ARQ_TESTE)
+        parp2 = PARp.read(ARQ_TESTE)
         assert parp1 == parp2
 
 
 def test_neq_parp():
     m: MagicMock = mock_open(read_data="".join(MockPARp))
     with patch("builtins.open", m):
-        parp1 = PARp.le_arquivo("")
-        parp2 = PARp.le_arquivo("")
+        parp1 = PARp.read(ARQ_TESTE)
+        parp2 = PARp.read(ARQ_TESTE)
         parp2.series_energia_ree.iloc[0, 0] = -1
         assert parp1 != parp2
```

### Comparing `inewave-0.0.95/tests/newave/test_parpeol.py` & `inewave-0.0.96/tests/newave/test_parpeol.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,87 +19,83 @@
     MockSerieRuidosUEE,
     MockCorrelSerieRuidosUEE,
     MockCorrelEspacialAnual,
     MockCorrelEspacialMensal,
     MockPARpeol,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_series_ventos_uee():
 
+def test_series_ventos_uee():
     m: MagicMock = mock_open(read_data="".join(MockSeriesVentosUEE))
     b = BlocoSerieVentosUEE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 40
     assert b.data.shape[1] == 15
     assert b.data.iloc[0, 3] == 6.31
     assert b.data.iloc[-1, -1] == 6.93
 
 
 def test_correlacao_series_ventos_uee():
-
     m: MagicMock = mock_open(read_data="".join(MockCorrelacaoSeriesVentosUEE))
     b = BlocoCorrelVentosUEE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 120
     assert b.data.shape[1] == 12
     assert b.data.iloc[0, 1] == -0.06591
     assert b.data.iloc[-1, -1] == 0.29579
 
 
 def test_serie_ruidos_uee():
-
     m: MagicMock = mock_open(read_data="".join(MockSerieRuidosUEE))
     b = BlocoSerieRuidosUEE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 40
     assert b.data.shape[1] == 14
     assert b.data.iloc[0, 1] == 0.0
     assert b.data.iloc[-1, -1] == 0.497
 
 
 def test_correl_serie_ruidos_uee():
-
     m: MagicMock = mock_open(read_data="".join(MockCorrelSerieRuidosUEE))
     b = BlocoCorrelRuidosUEE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 120
     assert b.data.shape[1] == 12
     assert b.data.iloc[0, 1] == 0.29579
     assert b.data.iloc[-1, -1] == 0.00582
 
 
 def test_correl_espacial_anual():
-
     m: MagicMock = mock_open(read_data="".join(MockCorrelEspacialAnual))
     b = BlocoCorrelEspacialAnualConfig()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 2
     assert b.data.shape[1] == 16
     assert b.data.iloc[0, 2] == -0.2010
     assert b.data.iloc[-1, -1] == 1.000
 
 
 def test_correl_espacial_mensal():
-
     m: MagicMock = mock_open(read_data="".join(MockCorrelEspacialMensal))
     b = BlocoCorrelEspacialMensalConfig()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 24
@@ -107,43 +103,43 @@
     assert b.data.iloc[0, 3] == -0.3616
     assert b.data.iloc[-1, -1] == 1.000
 
 
 def test_atributos_encontrados_parpeol():
     m: MagicMock = mock_open(read_data="".join(MockPARpeol))
     with patch("builtins.open", m):
-        parp = PARpeol.le_arquivo("")
+        parp = PARpeol.read(ARQ_TESTE)
         assert parp.series_ventos_uee is not None
         assert parp.correlacao_series_ventos_uee is not None
         assert parp.series_ruido_uee is not None
         assert parp.correlacao_series_ruidos_uee is not None
         assert parp.correlacao_espacial_anual is not None
         assert parp.correlacao_espacial_mensal is not None
 
 
 def test_atributos_nao_encontrados_parp():
     m: MagicMock = mock_open(read_data="".join(""))
     with patch("builtins.open", m):
-        parp = PARpeol.le_arquivo("")
+        parp = PARpeol.read(ARQ_TESTE)
         assert parp.series_ventos_uee is None
         assert parp.correlacao_series_ventos_uee is None
         assert parp.series_ruido_uee is None
         assert parp.correlacao_series_ruidos_uee is None
         assert parp.correlacao_espacial_anual is None
         assert parp.correlacao_espacial_mensal is None
 
 
 def test_eq_parpeol():
     m: MagicMock = mock_open(read_data="".join(MockPARpeol))
     with patch("builtins.open", m):
-        parp1 = PARpeol.le_arquivo("")
-        parp2 = PARpeol.le_arquivo("")
+        parp1 = PARpeol.read(ARQ_TESTE)
+        parp2 = PARpeol.read(ARQ_TESTE)
         assert parp1 == parp2
 
 
 def test_neq_parpeol():
     m: MagicMock = mock_open(read_data="".join(MockPARpeol))
     with patch("builtins.open", m):
-        parp1 = PARpeol.le_arquivo("")
-        parp2 = PARpeol.le_arquivo("")
+        parp1 = PARpeol.read(ARQ_TESTE)
+        parp2 = PARpeol.read(ARQ_TESTE)
         parp2.series_ventos_uee.iloc[0, 0] = -1
         assert parp1 != parp2
```

### Comparing `inewave-0.0.95/tests/newave/test_parpvaz.py` & `inewave-0.0.96/tests/newave/test_parpvaz.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,31 +23,31 @@
     MockCoeficientesModeloPARpvaz,
     MockSerieRuidosPARpvaz,
     MockCorrelogramoSerieRuidosPARpvaz,
     MockCorrelacaoEspacialPARpvaz,
     MockPARpvaz,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_series_vazoes_uhe():
 
+def test_series_vazoes_uhe():
     m: MagicMock = mock_open(read_data="".join(MockSeriesVazoesPARpvaz))
     b = BlocoSerieVazoesUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 90
     assert b.data.shape[1] == 15
     assert b.data.iloc[0, 3] == 302.0
     assert b.data.iloc[-1, -1] == 176.0
 
 
 def test_correlacao_series_vazoes_uhe():
-
     m: MagicMock = mock_open(
         read_data="".join(MockCorrelogramoSerieVazoesPARpvaz)
     )
     b = BlocoCorrelVazoesUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
@@ -55,15 +55,14 @@
     assert b.data.shape[0] == 12
     assert b.data.shape[1] == 12
     assert b.data.iloc[0, 1] == 0.45003
     assert b.data.iloc[-1, -1] == 0.2489
 
 
 def test_correlacao_parcial_series_vazoes_uhe():
-
     m: MagicMock = mock_open(
         read_data="".join(MockCorrelogramoParcialSerieVazoesPARpvaz)
     )
     b = BlocoCorrelParcialVazoesUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
@@ -71,29 +70,27 @@
     assert b.data.shape[0] == 12
     assert b.data.shape[1] == 12
     assert b.data.iloc[0, 1] == 0.45003
     assert b.data.iloc[-1, -1] == 0.00987
 
 
 def test_ordem_modelo_uhe():
-
     m: MagicMock = mock_open(read_data="".join(MockOrdemOriginalModeloPARpvaz))
     b = BlocoOrdemModeloUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 1
     assert b.data.shape[1] == 14
     assert b.data.iloc[0, 2] == 6
     assert b.data.iloc[-1, -1] == 6
 
 
 def test_coeficientes_modelo_uhe():
-
     m: MagicMock = mock_open(read_data="".join(MockCoeficientesModeloPARpvaz))
     b = BlocoCoeficientesModeloUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
     print(b.data)
     assert b.data.shape[0] == 1
@@ -101,29 +98,27 @@
     assert b.data.loc[0, "Psi 1"] == 0.450
     assert b.data.loc[0, "Psi Norm 1"] == 0.727
     assert b.data.loc[0, "Psi A"] == 0.0
     assert b.data.loc[0, "Psi Norm A"] == 0.0
 
 
 def test_serie_ruidos_uhe():
-
     m: MagicMock = mock_open(read_data="".join(MockSerieRuidosPARpvaz))
     b = BlocoSerieRuidosUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 90
     assert b.data.shape[1] == 14
     assert b.data.iloc[0, 1] == 0.0
     assert b.data.iloc[-1, -1] == -0.0752
 
 
 def test_correl_serie_ruidos_uhe():
-
     m: MagicMock = mock_open(
         read_data="".join(MockCorrelogramoSerieRuidosPARpvaz)
     )
     b = BlocoCorrelRuidosUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
@@ -131,15 +126,14 @@
     assert b.data.shape[0] == 12
     assert b.data.shape[1] == 12
     assert b.data.iloc[0, 1] == -0.06325
     assert b.data.iloc[-1, -1] == 0.00761
 
 
 def test_correl_espacial_anual_mensal():
-
     m: MagicMock = mock_open(read_data="".join(MockCorrelacaoEspacialPARpvaz))
     b = BlocoCorrelEspacialAnualMensalUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 17
@@ -147,49 +141,49 @@
     assert b.data.iloc[0, 2] == 0.55
     assert b.data.iloc[-1, -1] == 0.52
 
 
 def test_atributos_encontrados_parpvaz():
     m: MagicMock = mock_open(read_data="".join(MockPARpvaz))
     with patch("builtins.open", m):
-        parp = PARpvaz.le_arquivo("")
+        parp = PARpvaz.read(ARQ_TESTE)
         assert parp.series_vazoes_uhe is not None
         assert parp.correlacao_series_vazoes_uhe is not None
         assert parp.correlacao_parcial_series_vazoes_uhe is not None
         assert parp.ordem_original_modelo is not None
         assert parp.ordem_final_modelo is not None
         assert parp.coeficientes is not None
         assert parp.series_ruido_uhe is not None
         assert parp.correlacao_series_ruidos_uhe is not None
         assert parp.correlacao_espacial_anual_mensal is not None
 
 
 def test_atributos_nao_encontrados_parpvaz():
     m: MagicMock = mock_open(read_data="".join(MockSerieRuidosPARpvaz))
     with patch("builtins.open", m):
-        parp = PARpvaz.le_arquivo("")
+        parp = PARpvaz.read(ARQ_TESTE)
         assert parp.series_vazoes_uhe is None
         assert parp.correlacao_series_vazoes_uhe is None
         assert parp.correlacao_parcial_series_vazoes_uhe is None
         assert parp.ordem_original_modelo is None
         assert parp.ordem_final_modelo is None
         assert parp.coeficientes is None
         assert parp.series_ruido_uhe is None
         assert parp.correlacao_series_ruidos_uhe is None
         assert parp.correlacao_espacial_anual_mensal is None
 
 
 def test_eq_parpvaz():
     m: MagicMock = mock_open(read_data="".join(MockPARpvaz))
     with patch("builtins.open", m):
-        parp1 = PARpvaz.le_arquivo("")
-        parp2 = PARpvaz.le_arquivo("")
+        parp1 = PARpvaz.read(ARQ_TESTE)
+        parp2 = PARpvaz.read(ARQ_TESTE)
         assert parp1 == parp2
 
 
 def test_neq_parpvaz():
     m: MagicMock = mock_open(read_data="".join(MockPARpvaz))
     with patch("builtins.open", m):
-        parp1 = PARpvaz.le_arquivo("")
-        parp2 = PARpvaz.le_arquivo("")
+        parp1 = PARpvaz.read(ARQ_TESTE)
+        parp2 = PARpvaz.read(ARQ_TESTE)
         parp2.series_vazoes_uhe.iloc[0, 0] = -1
         assert parp1 != parp2
```

### Comparing `inewave-0.0.95/tests/newave/test_patamar.py` & `inewave-0.0.96/tests/newave/test_patamar.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,28 +18,28 @@
     MockBlocoDuracaoMensalPatamares,
     MockBlocoCargaSubsistema,
     MockBlocoIntercambioSubsistemas,
     MockBlocoUsinasNaoSimuladas,
     MockPatamar,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_numero_patamares_patamar():
 
+def test_bloco_numero_patamares_patamar():
     m: MagicMock = mock_open(read_data="".join(MockBlocoNumeroPatamares))
     b = BlocoNumeroPatamares()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data == 3
 
 
 def test_bloco_duracao_patamares_patamar():
-
     m: MagicMock = mock_open(
         read_data="".join(MockBlocoDuracaoMensalPatamares)
     )
     b = BlocoDuracaoPatamar()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
@@ -57,15 +57,14 @@
     assert b.data.iloc[0, 10] == 0.2823
     assert b.data.iloc[0, 11] == 0.2222
     assert b.data.iloc[0, 12] == 0.2366
     assert b.data.iloc[-1, -1] == 0.5081
 
 
 def test_bloco_carga_subsistema_patamar():
-
     m: MagicMock = mock_open(read_data="".join(MockBlocoCargaSubsistema))
     b = BlocoCargaPatamar()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.iloc[0, 0] == 1
@@ -82,15 +81,14 @@
     assert b.data.iloc[0, 11] == 1.1531
     assert b.data.iloc[0, 12] == 1.1623
     assert b.data.iloc[0, 13] == 1.1494
     assert b.data.iloc[-1, -1] == 0.9673
 
 
 def test_bloco_intercambio_patamar():
-
     m: MagicMock = mock_open(
         read_data="".join(MockBlocoIntercambioSubsistemas)
     )
     b = BlocoIntercambioPatamarSubsistemas()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
@@ -110,15 +108,14 @@
     assert b.data.iloc[0, 12] == 0.9681
     assert b.data.iloc[0, 13] == 0.9669
     assert b.data.iloc[0, 14] == 0.9683
     assert b.data.iloc[-1, -1] == 1.0
 
 
 def test_bloco_usinas_nao_simuladas_patamar():
-
     m: MagicMock = mock_open(read_data="".join(MockBlocoUsinasNaoSimuladas))
     b = BlocoUsinasNaoSimuladas()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.iloc[0, 0] == 1
@@ -139,59 +136,59 @@
     assert b.data.iloc[0, 15] == 0.9965
     assert b.data.iloc[-1, -1] == 1.0
 
 
 def test_atributos_encontrados_patamar():
     m: MagicMock = mock_open(read_data="".join(MockPatamar))
     with patch("builtins.open", m):
-        ad = Patamar.le_arquivo("")
+        ad = Patamar.read(ARQ_TESTE)
         assert ad.numero_patamares is not None
         assert ad.duracao_mensal_patamares is not None
         assert ad.carga_patamares is not None
         assert ad.intercambio_patamares is not None
         assert ad.usinas_nao_simuladas is not None
 
 
 def test_atributos_nao_encontrados_patamar():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = Patamar.le_arquivo("")
+        ad = Patamar.read(ARQ_TESTE)
         assert ad.numero_patamares is None
         assert ad.duracao_mensal_patamares is None
         assert ad.carga_patamares is None
         assert ad.intercambio_patamares is None
         assert ad.usinas_nao_simuladas is None
 
 
 def test_eq_patamar():
     m: MagicMock = mock_open(read_data="".join(MockPatamar))
     with patch("builtins.open", m):
-        cf1 = Patamar.le_arquivo("")
-        cf2 = Patamar.le_arquivo("")
+        cf1 = Patamar.read(ARQ_TESTE)
+        cf2 = Patamar.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_patamar():
     m: MagicMock = mock_open(read_data="".join(MockPatamar))
     with patch("builtins.open", m):
-        cf1 = Patamar.le_arquivo("")
-        cf2 = Patamar.le_arquivo("")
+        cf1 = Patamar.read(ARQ_TESTE)
+        cf2 = Patamar.read(ARQ_TESTE)
         cf2.numero_patamares = 0
         assert cf1 != cf2
 
 
 def test_leitura_escrita_patamar():
     m_leitura: MagicMock = mock_open(read_data="".join(MockPatamar))
     with patch("builtins.open", m_leitura):
-        cf1 = Patamar.le_arquivo("")
+        cf1 = Patamar.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = Patamar.le_arquivo("")
+        cf2 = Patamar.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_penalid.py` & `inewave-0.0.96/tests/nwlistop/test_qincruh.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,39 @@
-# Rotinas de testes associadas ao arquivo penalid.dat do NEWAVE
-
-from inewave.newave.penalid import Penalid
-
+from inewave.nwlistop.qincruh import QincrUH
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.penalid import (
-    MockPenalid,
-)
+from tests.mocks.arquivos.qincruh import MockQincrUH
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_penalid():
-    m: MagicMock = mock_open(read_data="".join(MockPenalid))
+
+def test_atributos_encontrados_qincruh():
+    m: MagicMock = mock_open(read_data="".join(MockQincrUH))
     with patch("builtins.open", m):
-        ad = Penalid.le_arquivo("")
-        assert ad.penalidades is not None
+        n = QincrUH.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
+        assert n.valores is not None
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 105.02
 
 
-def test_atributos_nao_encontrados_penalid():
+def test_atributos_nao_encontrados_qincruh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = Penalid.le_arquivo("")
-        assert ad.penalidades is None
+        n = QincrUH.read(ARQ_TESTE)
+        assert n.usina is None
+        assert n.valores is None
 
 
-def test_eq_penalid():
-    m: MagicMock = mock_open(read_data="".join(MockPenalid))
+def test_eq_qincruh():
+    m: MagicMock = mock_open(read_data="".join(MockQincrUH))
     with patch("builtins.open", m):
-        cf1 = Penalid.le_arquivo("")
-        cf2 = Penalid.le_arquivo("")
-        assert cf1 == cf2
+        n1 = QincrUH.read(ARQ_TESTE)
+        n2 = QincrUH.read(ARQ_TESTE)
+        assert n1 == n2
 
 
-def test_neq_penalid():
-    m: MagicMock = mock_open(read_data="".join(MockPenalid))
-    with patch("builtins.open", m):
-        cf1 = Penalid.le_arquivo("")
-        cf2 = Penalid.le_arquivo("")
-        cf2.penalidades.loc[0, 0] = 0
-        assert cf1 != cf2
-
-
-def test_leitura_escrita_penalid():
-    m_leitura: MagicMock = mock_open(read_data="".join(MockPenalid))
-    with patch("builtins.open", m_leitura):
-        cf1 = Penalid.le_arquivo("")
-    m_escrita: MagicMock = mock_open(read_data="")
-    with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
-        # Recupera o que foi escrito
-        chamadas = m_escrita.mock_calls
-        linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
-        ]
-    m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
-    with patch("builtins.open", m_releitura):
-        cf2 = Penalid.le_arquivo("")
-        assert cf1 == cf2
+# Não deve ter teste de diferença, visto que o atributo é
+# implementado como Lazy Property.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `inewave-0.0.95/tests/newave/test_pmo.py` & `inewave-0.0.96/tests/newave/test_pmo.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from tests.mocks.arquivos.pmo import MockBlocoMARSPMOInicial
 from tests.mocks.arquivos.pmo import MockBlocoMARSPMOFinal
 from tests.mocks.arquivos.pmo import MockBlocoRiscoDeficitENSPMO
 from tests.mocks.arquivos.pmo import MockBlocoCustoOperacaoPMO
 from tests.mocks.arquivos.pmo import MockBlocoCustoOperacaoTotalPMO
 from tests.mocks.arquivos.pmo import MockPMO
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_eafpast_tendencia_hidrologica():
     m: MagicMock = mock_open(
         read_data="".join(MockBlocoEafPastTendenciaHidrolPMO)
     )
     b = BlocoEafPastTendenciaHidrolPMO()
     with patch("builtins.open", m):
@@ -163,15 +165,15 @@
     assert b.data.iloc[1, 14] == 2.2292
     assert b.data.iloc[1, 15] == 2.2697
 
 
 def test_atributos_encontrados_pmo():
     m: MagicMock = mock_open(read_data="".join(MockPMO))
     with patch("builtins.open", m):
-        pmo = PMO.le_arquivo("")
+        pmo = PMO.read(ARQ_TESTE)
         assert pmo.eafpast_tendencia_hidrologica is not None
         assert pmo.eafpast_cfuga_medio is not None
         assert pmo.convergencia is not None
         assert pmo.configuracoes_alteracao_potencia is not None
         assert pmo.configuracoes_entrada_reservatorio is not None
         assert pmo.configuracoes_qualquer_modificacao is not None
         assert pmo.retas_perdas_engolimento(1) is not None
@@ -184,30 +186,30 @@
         assert pmo.desvio_custo_operacao_total is not None
         assert pmo.produtibilidades_equivalentes is not None
 
 
 def test_atributos_nao_encontrados_pmo():
     m: MagicMock = mock_open(read_data="".join(MockBlocoConvergenciaPMO))
     with patch("builtins.open", m):
-        pmo = PMO.le_arquivo("")
+        pmo = PMO.read(ARQ_TESTE)
         assert pmo.convergencia is not None
         assert pmo.custo_operacao_series_simuladas is None
         assert pmo.custo_operacao_total is None
         assert pmo.desvio_custo_operacao_total is None
         assert pmo.produtibilidades_equivalentes is None
 
 
 def test_eq_pmo():
     m: MagicMock = mock_open(read_data="".join(MockPMO))
     with patch("builtins.open", m):
-        pmo1 = PMO.le_arquivo("")
-        pmo2 = PMO.le_arquivo("")
+        pmo1 = PMO.read(ARQ_TESTE)
+        pmo2 = PMO.read(ARQ_TESTE)
         assert pmo1 == pmo2
 
 
 def test_neq_pmo():
     m: MagicMock = mock_open(read_data="".join(MockPMO))
     with patch("builtins.open", m):
-        pmo1 = PMO.le_arquivo("")
-        pmo2 = PMO.le_arquivo("")
+        pmo1 = PMO.read(ARQ_TESTE)
+        pmo2 = PMO.read(ARQ_TESTE)
         pmo2.configuracoes_alteracao_potencia
         assert pmo1 == pmo2
```

### Comparing `inewave-0.0.95/tests/newave/test_re.py` & `inewave-0.0.96/tests/newave/test_ree.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,63 @@
-# Rotinas de testes associadas ao arquivo re.dat do NEWAVE
-from inewave.newave.modelos.re import (
-    BlocoUsinasConjuntoRE,
-    BlocoConfiguracaoRestricoesRE,
-)
-
-from inewave.newave import RE
+# Rotinas de testes associadas ao arquivo ree.dat do NEWAVE
+from inewave.newave.ree import REE
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.re import (
-    MockBlocoUsinasRestricoes,
-    MockBlocoRestricoes,
-    MockRE,
+from tests.mocks.arquivos.ree import (
+    MockREE,
 )
 
-
-def test_bloco_usinas_conjuntos_re():
-
-    m: MagicMock = mock_open(read_data="".join(MockBlocoUsinasRestricoes))
-    b = BlocoUsinasConjuntoRE()
-    with patch("builtins.open", m):
-        with open("", "") as fp:
-            b.read(fp)
-
-    assert b.data.iloc[0, 0] == 1
-    assert b.data.iloc[-1, 0] == 10
-    assert b.data.iloc[-1, 2] == 284
-
-
-def test_bloco_restricoes_re():
-
-    m: MagicMock = mock_open(read_data="".join(MockBlocoRestricoes))
-    b = BlocoConfiguracaoRestricoesRE()
-    with patch("builtins.open", m):
-        with open("", "") as fp:
-            b.read(fp)
-
-    assert b.data.iloc[0, 0] == 1
-    assert b.data.iloc[-1, 0] == 10
-    assert b.data.iloc[-1, -1] == "C. CALDEIRAO E F. GOMES"
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_re():
-    m: MagicMock = mock_open(read_data="".join(MockRE))
+def test_atributos_encontrados_ree():
+    m: MagicMock = mock_open(read_data="".join(MockREE))
     with patch("builtins.open", m):
-        ad = RE.le_arquivo("")
-        assert ad.usinas_conjuntos is not None
-        assert ad.restricoes is not None
+        ad = REE.read(ARQ_TESTE)
+        assert ad.rees is not None
+        assert ad.remocao_ficticias is not None
 
 
-def test_atributos_nao_encontrados_re():
+def test_atributos_nao_encontrados_ree():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = RE.le_arquivo("")
-        assert ad.usinas_conjuntos is None
-        assert ad.restricoes is None
+        ad = REE.read(ARQ_TESTE)
+        assert ad.rees is None
+        assert ad.remocao_ficticias is None
 
 
-def test_eq_re():
-    m: MagicMock = mock_open(read_data="".join(MockRE))
+def test_eq_ree():
+    m: MagicMock = mock_open(read_data="".join(MockREE))
     with patch("builtins.open", m):
-        cf1 = RE.le_arquivo("")
-        cf2 = RE.le_arquivo("")
+        cf1 = REE.read(ARQ_TESTE)
+        cf2 = REE.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
-def test_neq_re():
-    m: MagicMock = mock_open(read_data="".join(MockRE))
+def test_neq_ree():
+    m: MagicMock = mock_open(read_data="".join(MockREE))
     with patch("builtins.open", m):
-        cf1 = RE.le_arquivo("")
-        cf2 = RE.le_arquivo("")
-        cf2.usinas_conjuntos.loc[0, 0] = 0
+        cf1 = REE.read(ARQ_TESTE)
+        cf2 = REE.read(ARQ_TESTE)
+        cf2.rees.loc[0, 0] = 0
         assert cf1 != cf2
 
 
-def test_leitura_escrita_re():
-    m_leitura: MagicMock = mock_open(read_data="".join(MockRE))
+def test_leitura_escrita_ree():
+    m_leitura: MagicMock = mock_open(read_data="".join(MockREE))
     with patch("builtins.open", m_leitura):
-        cf1 = RE.le_arquivo("")
+        cf1 = REE.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = RE.le_arquivo("")
+        cf2 = REE.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_ree.py` & `inewave-0.0.96/tests/nwlistop/test_vturuh.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,39 @@
-# Rotinas de testes associadas ao arquivo ree.dat do NEWAVE
-from inewave.newave.ree import REE
-
+from inewave.nwlistop.vturuh import VturUH
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ree import (
-    MockREE,
-)
+from tests.mocks.arquivos.vturuh import MockVturUH
+
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_ree():
-    m: MagicMock = mock_open(read_data="".join(MockREE))
+def test_atributos_encontrados_vturuh():
+    m: MagicMock = mock_open(read_data="".join(MockVturUH))
     with patch("builtins.open", m):
-        ad = REE.le_arquivo("")
-        assert ad.rees is not None
-        assert ad.remocao_ficticias is not None
+        n = VturUH.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
+        assert n.valores is not None
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 98.77
 
 
-def test_atributos_nao_encontrados_ree():
+def test_atributos_nao_encontrados_vturuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = REE.le_arquivo("")
-        assert ad.rees is None
-        assert ad.remocao_ficticias is None
+        n = VturUH.read(ARQ_TESTE)
+        assert n.usina is None
+        assert n.valores is None
 
 
-def test_eq_ree():
-    m: MagicMock = mock_open(read_data="".join(MockREE))
+def test_eq_vturuh():
+    m: MagicMock = mock_open(read_data="".join(MockVturUH))
     with patch("builtins.open", m):
-        cf1 = REE.le_arquivo("")
-        cf2 = REE.le_arquivo("")
-        assert cf1 == cf2
+        n1 = VturUH.read(ARQ_TESTE)
+        n2 = VturUH.read(ARQ_TESTE)
+        assert n1 == n2
 
 
-def test_neq_ree():
-    m: MagicMock = mock_open(read_data="".join(MockREE))
-    with patch("builtins.open", m):
-        cf1 = REE.le_arquivo("")
-        cf2 = REE.le_arquivo("")
-        cf2.rees.loc[0, 0] = 0
-        assert cf1 != cf2
-
-
-def test_leitura_escrita_ree():
-    m_leitura: MagicMock = mock_open(read_data="".join(MockREE))
-    with patch("builtins.open", m_leitura):
-        cf1 = REE.le_arquivo("")
-    m_escrita: MagicMock = mock_open(read_data="")
-    with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
-        # Recupera o que foi escrito
-        chamadas = m_escrita.mock_calls
-        linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
-        ]
-    m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
-    with patch("builtins.open", m_releitura):
-        cf2 = REE.le_arquivo("")
-        assert cf1 == cf2
+# Não deve ter teste de diferença, visto que o atributo é
+# implementado como Lazy Property.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `inewave-0.0.95/tests/newave/test_restricaoeletrica.py` & `inewave-0.0.96/tests/newave/test_restricaoeletrica.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from tests.mocks.arquivos.restricaoeletrica import (
     MockRE,
     MockREHorizPer,
     MockRELimFormPer,
     MockRestricaoEletrica,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_registro_re_restricaoeletrica():
     m: MagicMock = mock_open(read_data="".join(MockRE))
     r = RegistroRE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -75,46 +77,46 @@
     assert r.limite_superior == 5000
     r.limite_superior = 0
 
 
 def test_atributos_encontrados_restricaoeletrica():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoEletrica))
     with patch("builtins.open", m):
-        e = RestricaoEletrica.le_arquivo("")
+        e = RestricaoEletrica.read(ARQ_TESTE)
         assert len(e.re()) > 0
         assert len(e.re_horiz_per()) > 0
         assert len(e.re_lim_form_per()) > 0
 
 
 def test_eq_restricaoeletrica():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoEletrica))
     with patch("builtins.open", m):
-        cf1 = RestricaoEletrica.le_arquivo("")
-        cf2 = RestricaoEletrica.le_arquivo("")
+        cf1 = RestricaoEletrica.read(ARQ_TESTE)
+        cf2 = RestricaoEletrica.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_restricaoeletrica():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoEletrica))
     with patch("builtins.open", m):
-        cf1 = RestricaoEletrica.le_arquivo("")
-        cf2 = RestricaoEletrica.le_arquivo("")
+        cf1 = RestricaoEletrica.read(ARQ_TESTE)
+        cf2 = RestricaoEletrica.read(ARQ_TESTE)
         cf2.deleta_registro(cf1.re()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_restricaoeletrica():
     m_leitura: MagicMock = mock_open(read_data="".join(MockRestricaoEletrica))
     with patch("builtins.open", m_leitura):
-        cf1 = RestricaoEletrica.le_arquivo("")
+        cf1 = RestricaoEletrica.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = RestricaoEletrica.le_arquivo("")
+        cf2 = RestricaoEletrica.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_restricaoenergia.py` & `inewave-0.0.96/tests/newave/test_restricaoenergia.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from tests.mocks.arquivos.restricaoenergia import (
     MockRHE,
     MockRHEHorizPer,
     MockRHQLsLPPEarmi,
     MockRestricaoEnergia,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_registro_rhe_restricaoenergia():
     m: MagicMock = mock_open(read_data="".join(MockRHE))
     r = RegistroRHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -66,46 +68,46 @@
     assert r.coeficiente_linear == 4000.0
     r.coeficiente_linear = 3500.0
 
 
 def test_atributos_encontrados_restricaoenergia():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoEnergia))
     with patch("builtins.open", m):
-        e = RestricaoEnergia.le_arquivo("")
+        e = RestricaoEnergia.read(ARQ_TESTE)
         assert len(e.rhe()) > 0
         assert len(e.rhe_horiz_per()) > 0
         assert len(e.rhe_ls_lpp_earmi()) > 0
 
 
 def test_eq_restricaoenergia():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoEnergia))
     with patch("builtins.open", m):
-        cf1 = RestricaoEnergia.le_arquivo("")
-        cf2 = RestricaoEnergia.le_arquivo("")
+        cf1 = RestricaoEnergia.read(ARQ_TESTE)
+        cf2 = RestricaoEnergia.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_restricaoenergia():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoEnergia))
     with patch("builtins.open", m):
-        cf1 = RestricaoEnergia.le_arquivo("")
-        cf2 = RestricaoEnergia.le_arquivo("")
+        cf1 = RestricaoEnergia.read(ARQ_TESTE)
+        cf2 = RestricaoEnergia.read(ARQ_TESTE)
         cf2.deleta_registro(cf1.rhe()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_restricaoenergia():
     m_leitura: MagicMock = mock_open(read_data="".join(MockRestricaoEnergia))
     with patch("builtins.open", m_leitura):
-        cf1 = RestricaoEnergia.le_arquivo("")
+        cf1 = RestricaoEnergia.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = RestricaoEnergia.le_arquivo("")
+        cf2 = RestricaoEnergia.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_restricaovazao.py` & `inewave-0.0.96/tests/newave/test_restricaovazao.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from tests.mocks.arquivos.restricaovazao import (
     MockRHQ,
     MockRHQHorizPer,
     MockRHQLsLPPVoli,
     MockRestricaoVazao,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_registro_rhq_restricaovazao():
     m: MagicMock = mock_open(read_data="".join(MockRHQ))
     r = RegistroRHQ()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
@@ -66,46 +68,46 @@
     assert r.coeficiente_linear == 3000.0
     r.coeficiente_linear = 3500.0
 
 
 def test_atributos_encontrados_restricaovazao():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoVazao))
     with patch("builtins.open", m):
-        e = RestricaoVazao.le_arquivo("")
+        e = RestricaoVazao.read(ARQ_TESTE)
         assert len(e.rhq()) > 0
         assert len(e.rhq_horiz_per()) > 0
         assert len(e.rhq_ls_lpp_voli()) > 0
 
 
 def test_eq_restricaovazao():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoVazao))
     with patch("builtins.open", m):
-        cf1 = RestricaoVazao.le_arquivo("")
-        cf2 = RestricaoVazao.le_arquivo("")
+        cf1 = RestricaoVazao.read(ARQ_TESTE)
+        cf2 = RestricaoVazao.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_restricaovazao():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoVazao))
     with patch("builtins.open", m):
-        cf1 = RestricaoVazao.le_arquivo("")
-        cf2 = RestricaoVazao.le_arquivo("")
+        cf1 = RestricaoVazao.read(ARQ_TESTE)
+        cf2 = RestricaoVazao.read(ARQ_TESTE)
         cf2.deleta_registro(cf1.rhq()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_restricaovazao():
     m_leitura: MagicMock = mock_open(read_data="".join(MockRestricaoVazao))
     with patch("builtins.open", m_leitura):
-        cf1 = RestricaoVazao.le_arquivo("")
+        cf1 = RestricaoVazao.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = RestricaoVazao.le_arquivo("")
+        cf2 = RestricaoVazao.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_sistema.py` & `inewave-0.0.96/tests/newave/test_sistema.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,67 +18,64 @@
     MockBlocoCustoDeficit,
     MockBlocoLimitesIntercambio,
     MockBlocoMercadoEnergia,
     MockBlocoGeracaoUsinasNaoSimuladas,
     MockSistema,
 )
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_numero_patamares_deficit_sistema():
 
+def test_bloco_numero_patamares_deficit_sistema():
     m: MagicMock = mock_open(
         read_data="".join(MockBlocoNumeroPatamaresDeficit)
     )
     b = BlocoNumeroPatamaresDeficit()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data == 1
 
 
 def test_bloco_custos_deficit_sistema():
-
     m: MagicMock = mock_open(read_data="".join(MockBlocoCustoDeficit))
     b = BlocoCustosDeficit()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, 0] == 11
     assert b.data.iloc[0, 3] == 6524.05
 
 
 def test_bloco_limites_intercambio_sistema():
-
     m: MagicMock = mock_open(read_data="".join(MockBlocoLimitesIntercambio))
     b = BlocoIntercambioSubsistema()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 7500.0
 
 
 def test_bloco_mercado_energia_sistema():
-
     m: MagicMock = mock_open(read_data="".join(MockBlocoMercadoEnergia))
     b = BlocoMercadoEnergiaSistema()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 6657.0
 
 
 def test_bloco_usinas_nao_simuladas_sistema():
-
     m: MagicMock = mock_open(
         read_data="".join(MockBlocoGeracaoUsinasNaoSimuladas)
     )
     b = BlocoGeracaoUsinasNaoSimuladas()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
@@ -86,59 +83,59 @@
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 1.0
 
 
 def test_atributos_encontrados_sistema():
     m: MagicMock = mock_open(read_data="".join(MockSistema))
     with patch("builtins.open", m):
-        ad = Sistema.le_arquivo("")
+        ad = Sistema.read(ARQ_TESTE)
         assert ad.numero_patamares_deficit is not None
         assert ad.custo_deficit is not None
         assert ad.limites_intercambio is not None
         assert ad.mercado_energia is not None
         assert ad.geracao_usinas_nao_simuladas is not None
 
 
 def test_atributos_nao_encontrados_sistema():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = Sistema.le_arquivo("")
+        ad = Sistema.read(ARQ_TESTE)
         assert ad.numero_patamares_deficit is None
         assert ad.custo_deficit is None
         assert ad.limites_intercambio is None
         assert ad.mercado_energia is None
         assert ad.geracao_usinas_nao_simuladas is None
 
 
 def test_eq_sistema():
     m: MagicMock = mock_open(read_data="".join(MockSistema))
     with patch("builtins.open", m):
-        cf1 = Sistema.le_arquivo("")
-        cf2 = Sistema.le_arquivo("")
+        cf1 = Sistema.read(ARQ_TESTE)
+        cf2 = Sistema.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_sistema():
     m: MagicMock = mock_open(read_data="".join(MockSistema))
     with patch("builtins.open", m):
-        cf1 = Sistema.le_arquivo("")
-        cf2 = Sistema.le_arquivo("")
+        cf1 = Sistema.read(ARQ_TESTE)
+        cf2 = Sistema.read(ARQ_TESTE)
         cf2.numero_patamares_deficit = 0
         assert cf1 != cf2
 
 
 def test_leitura_escrita_sistema():
     m_leitura: MagicMock = mock_open(read_data="".join(MockSistema))
     with patch("builtins.open", m_leitura):
-        cf1 = Sistema.le_arquivo("")
+        cf1 = Sistema.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = Sistema.le_arquivo("")
+        cf2 = Sistema.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_term.py` & `inewave-0.0.96/tests/newave/test_vazpast.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,75 @@
-# Rotinas de testes associadas ao arquivo term.dat do NEWAVE
-from inewave.config import MESES_DF
-from inewave.newave.modelos.term import BlocoTermUTE
+# Rotinas de testes associadas ao arquivo vazpast.dat do NEWAVE
+from inewave.newave.modelos.vazpast import BlocoVazPast
 
-from inewave.newave import Term
+from inewave.newave import VazPast
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.term import MockBlocoUTE
+from tests.mocks.arquivos.vazpast import MockBlocoVazoesPassadas
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_usinas_term():
 
-    m: MagicMock = mock_open(read_data="".join(MockBlocoUTE))
-    b = BlocoTermUTE()
+def test_bloco_desvios_vazpast():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
+    b = BlocoVazPast()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
-    assert b.data.shape[0] == 125
+
+    assert b.data.shape[0] == 217
     assert b.data.iloc[0, 0] == 1
-    assert b.data.iloc[-1, -1] == 63.0
+    assert b.data.iloc[-1, -1] == 20.0
 
 
-def test_atributos_encontrados_term():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoUTE))
+def test_atributos_encontrados_vazpast():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
     with patch("builtins.open", m):
-        ad = Term.le_arquivo("")
-        assert ad.usinas is not None
+        ad = VazPast.read(ARQ_TESTE)
+        assert ad.tendencia is not None
 
 
-def test_atributos_nao_encontrados_term():
+def test_atributos_nao_encontrados_vazpast():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = Term.le_arquivo("")
-        assert ad.usinas is None
+        ad = VazPast.read(ARQ_TESTE)
+        assert ad.tendencia is None
 
 
-def test_eq_term():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoUTE))
+def test_eq_vazpast():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
     with patch("builtins.open", m):
-        cf1 = Term.le_arquivo("")
-        cf2 = Term.le_arquivo("")
+        cf1 = VazPast.read(ARQ_TESTE)
+        cf2 = VazPast.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
-def test_neq_term():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoUTE))
+def test_neq_vazpast():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
     with patch("builtins.open", m):
-        cf1 = Term.le_arquivo("")
-        cf2 = Term.le_arquivo("")
-        cf2.usinas.iloc[0, 0] = -1
+        cf1 = VazPast.read(ARQ_TESTE)
+        cf2 = VazPast.read(ARQ_TESTE)
+        cf2.tendencia.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
-def test_leitura_escrita_term():
-    m_leitura: MagicMock = mock_open(read_data="".join(MockBlocoUTE))
+def test_leitura_escrita_vazpast():
+    m_leitura: MagicMock = mock_open(
+        read_data="".join(MockBlocoVazoesPassadas)
+    )
     with patch("builtins.open", m_leitura):
-        cf1 = Term.le_arquivo("")
+        cf1 = VazPast.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = Term.le_arquivo("")
+        cf2 = VazPast.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/newave/test_vazaob.py` & `inewave-0.0.96/tests/newave/test_vazaob.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,71 +2,71 @@
 from inewave.newave.vazaob import Vazaob
 
 from os.path import join
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
-ARQ_TEST = "./tests/mocks/arquivos"
+ARQ_TESTE = "./tests/mocks/arquivos/vazaob.dat"
 
 NUM_FORWARDS = 2
 NUM_ABERTURAS = 20
 NUM_UHES = 1
 NUM_ESTAGIOS = 16
 NUM_ENTRADAS = NUM_FORWARDS * NUM_ABERTURAS * NUM_UHES * NUM_ESTAGIOS
 
 
 def test_secao_vazao():
     r = SecaoDadosVazaob()
-    with open(join(ARQ_TEST, "vazaob.dat"), "rb") as fp:
+    with open(ARQ_TESTE, "rb") as fp:
         r.read(
             fp,
             numero_forwards=NUM_FORWARDS,
             numero_aberturas=NUM_ABERTURAS,
             numero_uhes=NUM_UHES,
             numero_estagios=NUM_ESTAGIOS,
         )
 
     assert len(r.data) == NUM_ENTRADAS
 
 
 def test_atributos_encontrados_vazao():
-    h = Vazaob.le_arquivo(
-        ARQ_TEST,
+    h = Vazaob.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_aberturas=NUM_ABERTURAS,
         numero_uhes=NUM_UHES,
         numero_estagios=NUM_ESTAGIOS,
     )
     assert h.series is not None
     assert h.series.isna().sum().sum() == 0
 
 
 def test_atributos_nao_encontrados_vazao():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        h = Vazaob.le_arquivo(
-            "",
+        h = Vazaob.read(
+            ARQ_TESTE,
             numero_forwards=NUM_FORWARDS,
             numero_aberturas=NUM_ABERTURAS,
             numero_uhes=NUM_UHES,
             numero_estagios=NUM_ESTAGIOS,
         )
         assert h.series.isna().sum().sum() == NUM_ENTRADAS
 
 
 def test_eq_vazao():
-    h1 = Vazaob.le_arquivo(
-        ARQ_TEST,
+    h1 = Vazaob.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_aberturas=NUM_ABERTURAS,
         numero_uhes=NUM_UHES,
         numero_estagios=NUM_ESTAGIOS,
     )
-    h2 = Vazaob.le_arquivo(
-        ARQ_TEST,
+    h2 = Vazaob.read(
+        ARQ_TESTE,
         numero_forwards=NUM_FORWARDS,
         numero_aberturas=NUM_ABERTURAS,
         numero_uhes=NUM_UHES,
         numero_estagios=NUM_ESTAGIOS,
     )
     assert h1 == h2
```

### Comparing `inewave-0.0.95/tests/newave/test_vazaof.py` & `inewave-0.0.96/tests/newave/test_vazaos.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from inewave.newave.modelos.vazaof import SecaoDadosVazaof
-from inewave.newave.vazaof import Vazaof
+from inewave.newave.modelos.vazaos import SecaoDadosVazaos
+from inewave.newave.vazaos import Vazaos
 
 from os.path import join
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
-ARQ_TEST = "./tests/mocks/arquivos"
+ARQ_TESTE = "./tests/mocks/arquivos/vazaos.dat"
 
-NUM_FORWARDS = 2
+NUM_SERIES = 2
 NUM_UHES = 1
 NUM_ESTAGIOS = 16
 NUM_ESTAGIOS_TH = 12
-NUM_ENTRADAS = NUM_FORWARDS * NUM_UHES * (NUM_ESTAGIOS_TH + NUM_ESTAGIOS)
+NUM_ENTRADAS = NUM_SERIES * NUM_UHES * (NUM_ESTAGIOS_TH + NUM_ESTAGIOS)
 
 
 def test_secao_vazao():
-    r = SecaoDadosVazaof()
-    with open(join(ARQ_TEST, "vazaof.dat"), "rb") as fp:
+    r = SecaoDadosVazaos()
+    with open(ARQ_TESTE, "rb") as fp:
         r.read(
             fp,
-            numero_forwards=NUM_FORWARDS,
+            numero_series=NUM_SERIES,
             numero_uhes=NUM_UHES,
             numero_estagios=NUM_ESTAGIOS,
             numero_estagios_th=NUM_ESTAGIOS_TH,
         )
 
     assert len(r.data) == NUM_ENTRADAS
 
 
 def test_atributos_encontrados_vazao():
-    h = Vazaof.le_arquivo(
-        ARQ_TEST,
-        numero_forwards=NUM_FORWARDS,
+    h = Vazaos.read(
+        ARQ_TESTE,
+        numero_series=NUM_SERIES,
         numero_uhes=NUM_UHES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
     assert h.series is not None
     assert h.series.isna().sum().sum() == 0
 
 
 def test_atributos_nao_encontrados_vazao():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        h = Vazaof.le_arquivo(
-            "",
-            numero_forwards=NUM_FORWARDS,
+        h = Vazaos.read(
+            ARQ_TESTE,
+            numero_series=NUM_SERIES,
             numero_uhes=NUM_UHES,
             numero_estagios=NUM_ESTAGIOS,
             numero_estagios_th=NUM_ESTAGIOS_TH,
         )
         assert h.series.isna().sum().sum() == NUM_ENTRADAS
 
 
 def test_eq_vazao():
-    h1 = Vazaof.le_arquivo(
-        ARQ_TEST,
-        numero_forwards=NUM_FORWARDS,
+    h1 = Vazaos.read(
+        ARQ_TESTE,
+        numero_series=NUM_SERIES,
         numero_uhes=NUM_UHES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
-    h2 = Vazaof.le_arquivo(
-        ARQ_TEST,
-        numero_forwards=NUM_FORWARDS,
+    h2 = Vazaos.read(
+        ARQ_TESTE,
+        numero_series=NUM_SERIES,
         numero_uhes=NUM_UHES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
     assert h1 == h2
```

### Comparing `inewave-0.0.95/tests/newave/test_vazaos.py` & `inewave-0.0.96/tests/newave/test_vazaof.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from inewave.newave.modelos.vazaos import SecaoDadosVazaos
-from inewave.newave.vazaos import Vazaos
+from inewave.newave.modelos.vazaof import SecaoDadosVazaof
+from inewave.newave.vazaof import Vazaof
 
 from os.path import join
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
-ARQ_TEST = "./tests/mocks/arquivos"
+ARQ_TESTE = "./tests/mocks/arquivos/vazaof.dat"
 
-NUM_SERIES = 2
+NUM_FORWARDS = 2
 NUM_UHES = 1
 NUM_ESTAGIOS = 16
 NUM_ESTAGIOS_TH = 12
-NUM_ENTRADAS = NUM_SERIES * NUM_UHES * (NUM_ESTAGIOS_TH + NUM_ESTAGIOS)
+NUM_ENTRADAS = NUM_FORWARDS * NUM_UHES * (NUM_ESTAGIOS_TH + NUM_ESTAGIOS)
 
 
 def test_secao_vazao():
-    r = SecaoDadosVazaos()
-    with open(join(ARQ_TEST, "vazaos.dat"), "rb") as fp:
+    r = SecaoDadosVazaof()
+    with open(ARQ_TESTE, "rb") as fp:
         r.read(
             fp,
-            numero_series=NUM_SERIES,
+            numero_forwards=NUM_FORWARDS,
             numero_uhes=NUM_UHES,
             numero_estagios=NUM_ESTAGIOS,
             numero_estagios_th=NUM_ESTAGIOS_TH,
         )
 
     assert len(r.data) == NUM_ENTRADAS
 
 
 def test_atributos_encontrados_vazao():
-    h = Vazaos.le_arquivo(
-        ARQ_TEST,
-        numero_series=NUM_SERIES,
+    h = Vazaof.read(
+        ARQ_TESTE,
+        numero_forwards=NUM_FORWARDS,
         numero_uhes=NUM_UHES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
     assert h.series is not None
     assert h.series.isna().sum().sum() == 0
 
 
 def test_atributos_nao_encontrados_vazao():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        h = Vazaos.le_arquivo(
-            "",
-            numero_series=NUM_SERIES,
+        h = Vazaof.read(
+            ARQ_TESTE,
+            numero_forwards=NUM_FORWARDS,
             numero_uhes=NUM_UHES,
             numero_estagios=NUM_ESTAGIOS,
             numero_estagios_th=NUM_ESTAGIOS_TH,
         )
         assert h.series.isna().sum().sum() == NUM_ENTRADAS
 
 
 def test_eq_vazao():
-    h1 = Vazaos.le_arquivo(
-        ARQ_TEST,
-        numero_series=NUM_SERIES,
+    h1 = Vazaof.read(
+        ARQ_TESTE,
+        numero_forwards=NUM_FORWARDS,
         numero_uhes=NUM_UHES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
-    h2 = Vazaos.le_arquivo(
-        ARQ_TEST,
-        numero_series=NUM_SERIES,
+    h2 = Vazaof.read(
+        ARQ_TESTE,
+        numero_forwards=NUM_FORWARDS,
         numero_uhes=NUM_UHES,
         numero_estagios=NUM_ESTAGIOS,
         numero_estagios_th=NUM_ESTAGIOS_TH,
     )
     assert h1 == h2
```

### Comparing `inewave-0.0.95/tests/newave/test_vazoes.py` & `inewave-0.0.96/tests/newave/test_vazoes.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,93 +2,92 @@
 from inewave.newave.vazoes import Vazoes
 
 from os.path import join
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
-ARQ_TEST = "./tests/mocks/arquivos"
+ARQ_TESTE = "./tests/mocks/arquivos/vazoes.dat"
 
 
 def test_registro_vazoesposto_vazoes():
-
     r = RegistroVazoesPostos()
-    with open(join(ARQ_TEST, "vazoes.dat"), "rb") as fp:
+    with open(ARQ_TESTE, "rb") as fp:
         r.read(fp, storage="BINARY")
 
     assert len(r.data) == 320
 
 
 def test_atributos_encontrados_vazoes():
-    h = Vazoes.le_arquivo(ARQ_TEST)
+    h = Vazoes.read(ARQ_TESTE)
     assert h.vazoes is not None
 
 
 def test_atributos_nao_encontrados_vazoes():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = Vazoes.le_arquivo("")
+        ad = Vazoes.read(ARQ_TESTE)
         assert ad.vazoes is None
 
 
 def test_eq_vazoes():
-    h1 = Vazoes.le_arquivo(ARQ_TEST)
-    h2 = Vazoes.le_arquivo(ARQ_TEST)
+    h1 = Vazoes.read(ARQ_TESTE)
+    h2 = Vazoes.read(ARQ_TESTE)
     assert h1 == h2
 
 
 def test_neq_vazoes():
-    h1 = Vazoes.le_arquivo(ARQ_TEST)
-    h2 = Vazoes.le_arquivo(ARQ_TEST)
+    h1 = Vazoes.read(ARQ_TESTE)
+    h2 = Vazoes.read(ARQ_TESTE)
     h2.vazoes.iloc[0, 0] = -1
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        h2.escreve_arquivo("")
+        h2.write(ARQ_TESTE)
         assert h1 != h2
 
 
 def test_leitura_escrita_vazoes():
-    h1 = Vazoes.le_arquivo(ARQ_TEST)
+    h1 = Vazoes.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        h1.escreve_arquivo("", "")
+        h1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data=b"".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        h2 = Vazoes.le_arquivo("")
+        h2 = Vazoes.read(ARQ_TESTE)
         assert h1 == h2
 
 
 def test_leitura_escrita_editando_vazoes():
-    h1 = Vazoes.le_arquivo(ARQ_TEST)
+    h1 = Vazoes.read(ARQ_TESTE)
     vaz = h1.vazoes
     num_vazoes_original = vaz.shape[0]
     h1.vazoes.loc[vaz.shape[0]] = 0
     m_escrita: MagicMock = mock_open(read_data="")
     # Testa aumentando a quantidade de vazões
     with patch("builtins.open", m_escrita):
-        h1.escreve_arquivo("", "")
+        h1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
         assert len(linhas_escritas) == num_vazoes_original
     # Testa reduzindo a quantidade de vazões
     num_vazoes_reduzidas = 10
     h1.vazoes.drop(
         index=list(range(num_vazoes_reduzidas, num_vazoes_original + 1)),
         inplace=True,
     )
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        h1.escreve_arquivo("", "")
+        h1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
         assert len(linhas_escritas) == num_vazoes_reduzidas
```

### Comparing `inewave-0.0.95/tests/newave/test_vazpast.py` & `inewave-0.0.96/tests/newave/test_confhd.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,73 @@
-# Rotinas de testes associadas ao arquivo vazpast.dat do NEWAVE
-from inewave.newave.modelos.vazpast import BlocoVazPast
+# Rotinas de testes associadas ao arquivo confhd.dat do NEWAVE
+from inewave.newave.modelos.confhd import BlocoConfUHE
 
-from inewave.newave import VazPast
+from inewave.newave import Confhd
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vazpast import MockBlocoVazoesPassadas
+from tests.mocks.arquivos.confhd import MockBlocoConfUHE
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_bloco_desvios_vazpast():
 
-    m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
-    b = BlocoVazPast()
+def test_bloco_uhe_confhd():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoConfUHE))
+    b = BlocoConfUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
-    assert b.data.shape[0] == 217
-    assert b.data.iloc[0, 0] == 1
-    assert b.data.iloc[-1, -1] == 20.0
+    assert b.data.shape[0] == 164
+    assert b.data.iloc[0, 0] == 4
+    assert b.data.iloc[-1, -1] == 1995
 
 
-def test_atributos_encontrados_vazpast():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
+def test_atributos_encontrados_confhd():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoConfUHE))
     with patch("builtins.open", m):
-        ad = VazPast.le_arquivo("")
-        assert ad.tendencia is not None
+        ad = Confhd.read(ARQ_TESTE)
+        assert ad.usinas is not None
 
 
-def test_atributos_nao_encontrados_vazpast():
+def test_atributos_nao_encontrados_confhd():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = VazPast.le_arquivo("")
-        assert ad.tendencia is None
+        ad = Confhd.read(ARQ_TESTE)
+        assert ad.usinas is None
 
 
-def test_eq_vazpast():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
+def test_eq_confhd():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoConfUHE))
     with patch("builtins.open", m):
-        cf1 = VazPast.le_arquivo("")
-        cf2 = VazPast.le_arquivo("")
+        cf1 = Confhd.read(ARQ_TESTE)
+        cf2 = Confhd.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
-def test_neq_vazpast():
-    m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
+def test_neq_confhd():
+    m: MagicMock = mock_open(read_data="".join(MockBlocoConfUHE))
     with patch("builtins.open", m):
-        cf1 = VazPast.le_arquivo("")
-        cf2 = VazPast.le_arquivo("")
-        cf2.tendencia.iloc[0, 0] = -1
+        cf1 = Confhd.read(ARQ_TESTE)
+        cf2 = Confhd.read(ARQ_TESTE)
+        cf2.usinas.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
-def test_leitura_escrita_vazpast():
-    m_leitura: MagicMock = mock_open(
-        read_data="".join(MockBlocoVazoesPassadas)
-    )
+def test_leitura_escrita_confhd():
+    m_leitura: MagicMock = mock_open(read_data="".join(MockBlocoConfUHE))
     with patch("builtins.open", m_leitura):
-        cf1 = VazPast.le_arquivo("")
+        cf1 = Confhd.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
-        cf1.escreve_arquivo("", "")
+        cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = VazPast.le_arquivo("")
+        cf2 = Confhd.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.95/tests/nwlistcf/test_estados.py` & `inewave-0.0.96/tests/nwlistcf/test_estados.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from inewave.nwlistcf import Estados
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.estados import MockEstados
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_estados():
     m: MagicMock = mock_open(read_data="".join(MockEstados))
     with patch("builtins.open", m):
-        n = Estados.le_arquivo("")
+        n = Estados.read(ARQ_TESTE)
         print(n.estados)
         assert n.estados is not None
 
 
 def test_atributos_nao_encontrados_estados():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Estados.le_arquivo("")
+        n = Estados.read(ARQ_TESTE)
         assert n.estados is None
 
 
 def test_eq_estados():
     m: MagicMock = mock_open(read_data="".join(MockEstados))
     with patch("builtins.open", m):
-        n1 = Estados.le_arquivo("")
-        n2 = Estados.le_arquivo("")
+        n1 = Estados.read(ARQ_TESTE)
+        n2 = Estados.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistcf/test_nwlistcf.py` & `inewave-0.0.96/tests/nwlistcf/test_nwlistcf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from inewave.nwlistcf import Nwlistcf
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.nwlistcf import MockNwlistcf
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_nwlistcf():
     m: MagicMock = mock_open(read_data="".join(MockNwlistcf))
     with patch("builtins.open", m):
-        n = Nwlistcf.le_arquivo("")
+        n = Nwlistcf.read(ARQ_TESTE)
         assert n.cortes is not None
 
 
 def test_atributos_nao_encontrados_nwlistcf():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Nwlistcf.le_arquivo("")
+        n = Nwlistcf.read(ARQ_TESTE)
         assert n.cortes is None
 
 
 def test_eq_nwlistcf():
     m: MagicMock = mock_open(read_data="".join(MockNwlistcf))
     with patch("builtins.open", m):
-        n1 = Nwlistcf.le_arquivo("")
-        n2 = Nwlistcf.le_arquivo("")
+        n1 = Nwlistcf.read(ARQ_TESTE)
+        n2 = Nwlistcf.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_cdef.py` & `inewave-0.0.96/tests/nwlistop/test_mercl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-from inewave.nwlistop.cdef import Cdef
+from inewave.nwlistop.mercl import Mercl
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.cdef import MockCdef
+from tests.mocks.arquivos.mercl import MockMercl
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_cdef():
-    m: MagicMock = mock_open(read_data="".join(MockCdef))
+
+def test_atributos_encontrados_mercl():
+    m: MagicMock = mock_open(read_data="".join(MockMercl))
     with patch("builtins.open", m):
-        n = Cdef.le_arquivo("")
+        n = Mercl.read(ARQ_TESTE)
         assert n.valores is not None
+        print(n.valores)
         assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[-1, -2] == 37783.0
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_cdef():
+def test_atributos_nao_encontrados_mercl():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Cdef.le_arquivo("")
+        n = Mercl.read(ARQ_TESTE)
         assert n.valores is None
         assert n.submercado is None
 
 
-def test_eq_cdef():
-    m: MagicMock = mock_open(read_data="".join(MockCdef))
+def test_eq_mercl():
+    m: MagicMock = mock_open(read_data="".join(MockMercl))
     with patch("builtins.open", m):
-        n1 = Cdef.le_arquivo("")
-        n2 = Cdef.le_arquivo("")
+        n1 = Mercl.read(ARQ_TESTE)
+        n2 = Mercl.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_cdefsin.py` & `inewave-0.0.96/tests/nwlistop/test_cdefsin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from inewave.nwlistop.cdefsin import CdefSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.cdefsin import MockCdefSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_cdefsin():
     m: MagicMock = mock_open(read_data="".join(MockCdefSIN))
     with patch("builtins.open", m):
-        n = CdefSIN.le_arquivo("")
+        n = CdefSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_cdefsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = CdefSIN.le_arquivo("")
+        n = CdefSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_cdefsin():
     m: MagicMock = mock_open(read_data="".join(MockCdefSIN))
     with patch("builtins.open", m):
-        n1 = CdefSIN.le_arquivo("")
-        n2 = CdefSIN.le_arquivo("")
+        n1 = CdefSIN.read(ARQ_TESTE)
+        n2 = CdefSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_cmarg.py` & `inewave-0.0.96/tests/nwlistop/test_cmarg.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.cmarg import Cmarg
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.cmarg import MockCmarg
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_cmarg():
     m: MagicMock = mock_open(read_data="".join(MockCmarg))
     with patch("builtins.open", m):
-        n = Cmarg.le_arquivo("")
+        n = Cmarg.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 1995
         assert n.valores.iloc[-1, -1] == 35.42
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_cmarg():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Cmarg.le_arquivo("")
+        n = Cmarg.read(ARQ_TESTE)
         assert n.valores is None
         assert n.submercado is None
 
 
 def test_eq_cmarg():
     m: MagicMock = mock_open(read_data="".join(MockCmarg))
     with patch("builtins.open", m):
-        n1 = Cmarg.le_arquivo("")
-        n2 = Cmarg.le_arquivo("")
+        n1 = Cmarg.read(ARQ_TESTE)
+        n2 = Cmarg.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_cmargmed.py` & `inewave-0.0.96/tests/nwlistop/test_cmargmed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.cmargmed import CmargMed
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.cmargmed import MockCmargMed
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_cmargmed():
     m: MagicMock = mock_open(read_data="".join(MockCmargMed))
     with patch("builtins.open", m):
-        n = CmargMed.le_arquivo("")
+        n = CmargMed.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2021
         assert n.valores.iloc[-1, -1] == 354.22
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_cmargmed():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = CmargMed.le_arquivo("")
+        n = CmargMed.read(ARQ_TESTE)
         assert n.valores is None
         assert n.submercado is None
 
 
 def test_eq_cmargmed():
     m: MagicMock = mock_open(read_data="".join(MockCmargMed))
     with patch("builtins.open", m):
-        n1 = CmargMed.le_arquivo("")
-        n2 = CmargMed.le_arquivo("")
+        n1 = CmargMed.read(ARQ_TESTE)
+        n2 = CmargMed.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_coper.py` & `inewave-0.0.96/tests/nwlistop/test_coper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from inewave.nwlistop.coper import Coper
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.coper import MockCoper
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_coper():
     m: MagicMock = mock_open(read_data="".join(MockCoper))
     with patch("builtins.open", m):
-        n = Coper.le_arquivo("")
+        n = Coper.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 1155.67
 
 
 def test_atributos_nao_encontrados_coper():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Coper.le_arquivo("")
+        n = Coper.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_coper():
     m: MagicMock = mock_open(read_data="".join(MockCoper))
     with patch("builtins.open", m):
-        n1 = Coper.le_arquivo("")
-        n2 = Coper.le_arquivo("")
+        n1 = Coper.read(ARQ_TESTE)
+        n2 = Coper.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_corteolm.py` & `inewave-0.0.96/tests/nwlistop/test_ghtotm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.corteolm import Corteolm
+from inewave.nwlistop.ghtotm import Ghtotm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.corteolm import MockCorteolm
+from tests.mocks.arquivos.ghtotm import MockGhtotm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_corteolm():
-    m: MagicMock = mock_open(read_data="".join(MockCorteolm))
+
+def test_atributos_encontrados_ghtotm():
+    m: MagicMock = mock_open(read_data="".join(MockGhtotm))
     with patch("builtins.open", m):
-        n = Corteolm.le_arquivo("")
+        n = Ghtotm.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[-1, -1] == 24494.9
 
 
-def test_atributos_nao_encontrados_corteolm():
+def test_atributos_nao_encontrados_ghtotm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Corteolm.le_arquivo("")
+        n = Ghtotm.read(ARQ_TESTE)
         assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_corteolm():
-    m: MagicMock = mock_open(read_data="".join(MockCorteolm))
+def test_eq_ghtotm():
+    m: MagicMock = mock_open(read_data="".join(MockGhtotm))
     with patch("builtins.open", m):
-        n1 = Corteolm.le_arquivo("")
-        n2 = Corteolm.le_arquivo("")
+        n1 = Ghtotm.read(ARQ_TESTE)
+        n2 = Ghtotm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_cterm.py` & `inewave-0.0.96/tests/nwlistop/test_ghtotsin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from inewave.nwlistop.cterm import Cterm
+from inewave.nwlistop.ghtotsin import GhtotSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.cterm import MockCterm
+from tests.mocks.arquivos.ghtotsin import MockGhtotsin
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_cterm():
-    m: MagicMock = mock_open(read_data="".join(MockCterm))
+
+def test_atributos_encontrados_ghtotsin():
+    m: MagicMock = mock_open(read_data="".join(MockGhtotsin))
     with patch("builtins.open", m):
-        n = Cterm.le_arquivo("")
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        n = GhtotSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 585.36
+        assert n.valores.iloc[-1, -1] == 46994.0
 
 
-def test_atributos_nao_encontrados_cterm():
+def test_atributos_nao_encontrados_ghtotsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Cterm.le_arquivo("")
-        assert n.submercado is None
+        n = GhtotSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_cterm():
-    m: MagicMock = mock_open(read_data="".join(MockCterm))
+def test_eq_ghtotsin():
+    m: MagicMock = mock_open(read_data="".join(MockGhtotsin))
     with patch("builtins.open", m):
-        n1 = Cterm.le_arquivo("")
-        n2 = Cterm.le_arquivo("")
+        n1 = GhtotSIN.read(ARQ_TESTE)
+        n2 = GhtotSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ctermsin.py` & `inewave-0.0.96/tests/nwlistop/test_ctermsin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from inewave.nwlistop.ctermsin import CtermSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.ctermsin import MockCtermSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_ctermsin():
     m: MagicMock = mock_open(read_data="".join(MockCtermSIN))
     with patch("builtins.open", m):
-        n = CtermSIN.le_arquivo("")
+        n = CtermSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2021
         assert n.valores.iloc[-1, -1] == 1230.35
 
 
 def test_atributos_nao_encontrados_ctermsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = CtermSIN.le_arquivo("")
+        n = CtermSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_ctermsin():
     m: MagicMock = mock_open(read_data="".join(MockCtermSIN))
     with patch("builtins.open", m):
-        n1 = CtermSIN.le_arquivo("")
-        n2 = CtermSIN.le_arquivo("")
+        n1 = CtermSIN.read(ARQ_TESTE)
+        n2 = CtermSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_deficit.py` & `inewave-0.0.96/tests/nwlistop/test_evertsin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from inewave.nwlistop.deficit import Def
+from inewave.nwlistop.evertsin import EvertSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.deficit import MockDef
+from tests.mocks.arquivos.evertsin import MockEvertSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_def():
-    m: MagicMock = mock_open(read_data="".join(MockDef))
+
+def test_atributos_encontrados_evertsin():
+    m: MagicMock = mock_open(read_data="".join(MockEvertSIN))
     with patch("builtins.open", m):
-        n = Def.le_arquivo("")
+        n = EvertSIN.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 0.0
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 146.0
 
 
-def test_atributos_nao_encontrados_def():
+def test_atributos_nao_encontrados_evertsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Def.le_arquivo("")
+        n = EvertSIN.read(ARQ_TESTE)
         assert n.valores is None
-        assert n.submercado is None
 
 
-def test_eq_def():
-    m: MagicMock = mock_open(read_data="".join(MockDef))
+def test_eq_evertsin():
+    m: MagicMock = mock_open(read_data="".join(MockEvertSIN))
     with patch("builtins.open", m):
-        n1 = Def.le_arquivo("")
-        n2 = Def.le_arquivo("")
+        n1 = EvertSIN.read(ARQ_TESTE)
+        n2 = EvertSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_defsin.py` & `inewave-0.0.96/tests/nwlistop/test_gttotsin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.defsin import DefSIN
+from inewave.nwlistop.gttotsin import GttotSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.defsin import MockDefSIN
+from tests.mocks.arquivos.gttotsin import MockGttotsin
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_defsin():
-    m: MagicMock = mock_open(read_data="".join(MockDefSIN))
+
+def test_atributos_encontrados_gttotsin():
+    m: MagicMock = mock_open(read_data="".join(MockGttotsin))
     with patch("builtins.open", m):
-        n = DefSIN.le_arquivo("")
+        n = GttotSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[-1, -1] == 5106.0
 
 
-def test_atributos_nao_encontrados_defsin():
+def test_atributos_nao_encontrados_gttotsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DefSIN.le_arquivo("")
+        n = GttotSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_defsin():
-    m: MagicMock = mock_open(read_data="".join(MockDefSIN))
+def test_eq_gttotsin():
+    m: MagicMock = mock_open(read_data="".join(MockGttotsin))
     with patch("builtins.open", m):
-        n1 = DefSIN.le_arquivo("")
-        n2 = DefSIN.le_arquivo("")
+        n1 = GttotSIN.read(ARQ_TESTE)
+        n2 = GttotSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_depminuh.py` & `inewave-0.0.96/tests/nwlistop/test_depminuh.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.depminuh import Depminuh
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.depminuh import MockDepminUH
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_depminuh():
     m: MagicMock = mock_open(read_data="".join(MockDepminUH))
     with patch("builtins.open", m):
-        n = Depminuh.le_arquivo("")
+        n = Depminuh.read(ARQ_TESTE)
         assert n.usina is not None
         assert n.usina == "CAMARGOS"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 3.57
 
 
 def test_atributos_nao_encontrados_depminuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Depminuh.le_arquivo("")
+        n = Depminuh.read(ARQ_TESTE)
         assert n.usina is None
         assert n.valores is None
 
 
 def test_eq_depminuh():
     m: MagicMock = mock_open(read_data="".join(MockDepminUH))
     with patch("builtins.open", m):
-        n1 = Depminuh.le_arquivo("")
-        n2 = Depminuh.le_arquivo("")
+        n1 = Depminuh.read(ARQ_TESTE)
+        n2 = Depminuh.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_dfphauh.py` & `inewave-0.0.96/tests/nwlistop/test_vertuh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.dfphauh import Dfphauh
+from inewave.nwlistop.vertuh import VertUH
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dfphauh import MockDfphauh
+from tests.mocks.arquivos.vertuh import MockVertuh
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_fphauh():
-    m: MagicMock = mock_open(read_data="".join(MockDfphauh))
+
+def test_atributos_encontrados_vertuh():
+    m: MagicMock = mock_open(read_data="".join(MockVertuh))
     with patch("builtins.open", m):
-        n = Dfphauh.le_arquivo("")
+        n = VertUH.read(ARQ_TESTE)
         assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        assert n.usina == "ESPORA"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 30.74
 
 
-def test_atributos_nao_encontrados_fphauh():
+def test_atributos_nao_encontrados_vertuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Dfphauh.le_arquivo("")
+        n = VertUH.read(ARQ_TESTE)
         assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_fphauh():
-    m: MagicMock = mock_open(read_data="".join(MockDfphauh))
+def test_eq_vertuh():
+    m: MagicMock = mock_open(read_data="".join(MockVertuh))
     with patch("builtins.open", m):
-        n1 = Dfphauh.le_arquivo("")
-        n2 = Dfphauh.le_arquivo("")
+        n1 = VertUH.read(ARQ_TESTE)
+        n2 = VertUH.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_dlppdfmax.py` & `inewave-0.0.96/tests/nwlistop/test_dlppdfmaxs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from inewave.nwlistop.dlppdfmax import DLPPdfmax
+from inewave.nwlistop.dlppdfmaxs import DLPPdfmaxs
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dlppdfmax import MockDLPPdfmax
+from tests.mocks.arquivos.dlppdfmaxs import MockDLPPdfmaxs
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_dlppdfmax():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmax))
+
+def test_atributos_encontrados_dlppdfmaxs():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxs))
     with patch("builtins.open", m):
-        n = DLPPdfmax.le_arquivo("")
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        n = DLPPdfmaxs.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_dlppdfmax():
+def test_atributos_nao_encontrados_dlppdfmaxs():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPdfmax.le_arquivo("")
-        assert n.ree is None
+        n = DLPPdfmaxs.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_dlppdfmax():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmax))
+def test_eq_dlppdfmaxs():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxs))
     with patch("builtins.open", m):
-        n1 = DLPPdfmax.le_arquivo("")
-        n2 = DLPPdfmax.le_arquivo("")
+        n1 = DLPPdfmaxs.read(ARQ_TESTE)
+        n2 = DLPPdfmaxs.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_dlppdfmaxm.py` & `inewave-0.0.96/tests/nwlistop/test_vento.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.dlppdfmaxm import DLPPdfmaxm
+from inewave.nwlistop.vento import Vento
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dlppdfmaxm import MockDLPPdfmaxm
+from tests.mocks.arquivos.vento import MockVento
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_dlppdfmaxm():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxm))
+
+def test_atributos_encontrados_vento():
+    m: MagicMock = mock_open(read_data="".join(MockVento))
     with patch("builtins.open", m):
-        n = DLPPdfmaxm.le_arquivo("")
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        n = Vento.read(ARQ_TESTE)
+        assert n.usina is not None
+        # assert n.usina == "cluster_NE_1"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[0, 0] == 2021
+        assert n.valores.iloc[-1, -1] == 7.8825
 
 
-def test_atributos_nao_encontrados_dlppdfmaxm():
+def test_atributos_nao_encontrados_vento():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPdfmaxm.le_arquivo("")
-        assert n.submercado is None
+        n = Vento.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_dlppdfmaxm():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxm))
+def test_eq_vento():
+    m: MagicMock = mock_open(read_data="".join(MockVento))
     with patch("builtins.open", m):
-        n1 = DLPPdfmaxm.le_arquivo("")
-        n2 = DLPPdfmaxm.le_arquivo("")
+        n1 = Vento.read(ARQ_TESTE)
+        n2 = Vento.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_dlppdfmaxs.py` & `inewave-0.0.96/tests/nwlistop/test_ghmaxm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from inewave.nwlistop.dlppdfmaxs import DLPPdfmaxs
+from inewave.nwlistop.ghmaxm import Ghmaxm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dlppdfmaxs import MockDLPPdfmaxs
+from tests.mocks.arquivos.ghmaxm import MockGhmaxm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_dlppdfmaxs():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxs))
+
+def test_atributos_encontrados_ghmaxm():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxm))
     with patch("builtins.open", m):
-        n = DLPPdfmaxs.le_arquivo("")
+        n = Ghmaxm.read(ARQ_TESTE)
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[0, 0] == 2021
+        assert n.valores.iloc[-1, -1] == 54602.6
 
 
-def test_atributos_nao_encontrados_dlppdfmaxs():
+def test_atributos_nao_encontrados_ghmaxm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPdfmaxs.le_arquivo("")
+        n = Ghmaxm.read(ARQ_TESTE)
+        assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_dlppdfmaxs():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxs))
+def test_eq_ghmaxm():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxm))
     with patch("builtins.open", m):
-        n1 = DLPPdfmaxs.le_arquivo("")
-        n2 = DLPPdfmaxs.le_arquivo("")
+        n1 = Ghmaxm.read(ARQ_TESTE)
+        n2 = Ghmaxm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_dlpptbmax.py` & `inewave-0.0.96/tests/nwlistop/test_dlpptbmaxs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from inewave.nwlistop.dlpptbmax import DLPPtbmax
+from inewave.nwlistop.dlpptbmaxs import DLPPtbmaxs
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dlpptbmax import MockDLPPtbmax
+from tests.mocks.arquivos.dlpptbmaxs import MockDLPPtbmaxs
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_dlpptbmax():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmax))
+
+def test_atributos_encontrados_dlpptbmaxs():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxs))
     with patch("builtins.open", m):
-        n = DLPPtbmax.le_arquivo("")
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        n = DLPPtbmaxs.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_dlpptbmax():
+def test_atributos_nao_encontrados_dlpptbmaxs():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPtbmax.le_arquivo("")
-        assert n.ree is None
+        n = DLPPtbmaxs.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_dlpptbmax():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmax))
+def test_eq_dlpptbmaxs():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxs))
     with patch("builtins.open", m):
-        n1 = DLPPtbmax.le_arquivo("")
-        n2 = DLPPtbmax.le_arquivo("")
+        n1 = DLPPtbmaxs.read(ARQ_TESTE)
+        n2 = DLPPtbmaxs.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_dlpptbmaxm.py` & `inewave-0.0.96/tests/nwlistop/test_dtbmax.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.dlpptbmaxm import DLPPtbmaxm
+from inewave.nwlistop.dtbmax import Dtbmax
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dlpptbmaxm import MockDLPPtbmaxm
+from tests.mocks.arquivos.dtbmax import MockDtbmax
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_dlpptbmaxm():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxm))
+
+def test_atributos_encontrados_dtbmax():
+    m: MagicMock = mock_open(read_data="".join(MockDtbmax))
     with patch("builtins.open", m):
-        n = DLPPtbmaxm.le_arquivo("")
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        n = Dtbmax.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_dlpptbmaxm():
+def test_atributos_nao_encontrados_dtbmax():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPtbmaxm.le_arquivo("")
-        assert n.submercado is None
+        n = Dtbmax.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_dlpptbmaxm():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxm))
+def test_eq_dtbmax():
+    m: MagicMock = mock_open(read_data="".join(MockDtbmax))
     with patch("builtins.open", m):
-        n1 = DLPPtbmaxm.le_arquivo("")
-        n2 = DLPPtbmaxm.le_arquivo("")
+        n1 = Dtbmax.read(ARQ_TESTE)
+        n2 = Dtbmax.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_dlpptbmaxs.py` & `inewave-0.0.96/tests/nwlistop/test_rhslpptb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from inewave.nwlistop.dlpptbmaxs import DLPPtbmaxs
+from inewave.nwlistop.rhslpptb import RHSLPPtb
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dlpptbmaxs import MockDLPPtbmaxs
+from tests.mocks.arquivos.rhslpptb import MockRHSLPPtb
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_dlpptbmaxs():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxs))
+
+def test_atributos_encontrados_rhslpptb():
+    m: MagicMock = mock_open(read_data="".join(MockRHSLPPtb))
     with patch("builtins.open", m):
-        n = DLPPtbmaxs.le_arquivo("")
+        n = RHSLPPtb.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_dlpptbmaxs():
+def test_atributos_nao_encontrados_rhslpptb():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPtbmaxs.le_arquivo("")
+        n = RHSLPPtb.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_dlpptbmaxs():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxs))
+def test_eq_rhslpptb():
+    m: MagicMock = mock_open(read_data="".join(MockRHSLPPtb))
     with patch("builtins.open", m):
-        n1 = DLPPtbmaxs.le_arquivo("")
-        n2 = DLPPtbmaxs.le_arquivo("")
+        n1 = RHSLPPtb.read(ARQ_TESTE)
+        n2 = RHSLPPtb.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_dtbmax.py` & `inewave-0.0.96/tests/nwlistop/test_eaf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.dtbmax import Dtbmax
+from inewave.nwlistop.eaf import Eaf
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dtbmax import MockDtbmax
+from tests.mocks.arquivos.eaf import MockEaf
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_dtbmax():
-    m: MagicMock = mock_open(read_data="".join(MockDtbmax))
+
+def test_atributos_encontrados_eaf():
+    m: MagicMock = mock_open(read_data="".join(MockEaf))
     with patch("builtins.open", m):
-        n = Dtbmax.le_arquivo("")
-        assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        n = Eaf.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[0, 0] == 2021
+        assert n.valores.iloc[-1, -1] == 2929.0
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_dtbmax():
+def test_atributos_nao_encontrados_eaf():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Dtbmax.le_arquivo("")
-        assert n.usina is None
+        n = Eaf.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.ree is None
 
 
-def test_eq_dtbmax():
-    m: MagicMock = mock_open(read_data="".join(MockDtbmax))
+def test_eq_eaf():
+    m: MagicMock = mock_open(read_data="".join(MockEaf))
     with patch("builtins.open", m):
-        n1 = Dtbmax.le_arquivo("")
-        n2 = Dtbmax.le_arquivo("")
+        n1 = Eaf.read(ARQ_TESTE)
+        n2 = Eaf.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_dtbmin.py` & `inewave-0.0.96/tests/nwlistop/test_dtbmin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.dtbmin import Dtbmin
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dtbmin import MockDtbmin
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_dtbmin():
     m: MagicMock = mock_open(read_data="".join(MockDtbmin))
     with patch("builtins.open", m):
-        n = Dtbmin.le_arquivo("")
+        n = Dtbmin.read(ARQ_TESTE)
         assert n.usina is not None
         assert n.usina == "CAMARGOS"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_dtbmin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Dtbmin.le_arquivo("")
+        n = Dtbmin.read(ARQ_TESTE)
         assert n.usina is None
         assert n.valores is None
 
 
 def test_eq_dtbmin():
     m: MagicMock = mock_open(read_data="".join(MockDtbmin))
     with patch("builtins.open", m):
-        n1 = Dtbmin.le_arquivo("")
-        n2 = Dtbmin.le_arquivo("")
+        n1 = Dtbmin.read(ARQ_TESTE)
+        n2 = Dtbmin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_dvazmax.py` & `inewave-0.0.96/tests/nwlistop/test_geolsin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from inewave.nwlistop.dvazmax import Dvazmax
+from inewave.nwlistop.geolsin import GeolSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dvazmax import MockDvazmax
+from tests.mocks.arquivos.geolsin import MockGeolSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_dvazmax():
-    m: MagicMock = mock_open(read_data="".join(MockDvazmax))
+
+def test_atributos_encontrados_geolsin():
+    m: MagicMock = mock_open(read_data="".join(MockGeolSIN))
     with patch("builtins.open", m):
-        n = Dvazmax.le_arquivo("")
-        assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        n = GeolSIN.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[0, 0] == 2021
+        assert n.valores.iloc[-1, -1] == 6574.3
 
 
-def test_atributos_nao_encontrados_dvazmax():
+def test_atributos_nao_encontrados_geolsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Dvazmax.le_arquivo("")
-        assert n.usina is None
+        n = GeolSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_dvazmax():
-    m: MagicMock = mock_open(read_data="".join(MockDvazmax))
+def test_eq_geolsin():
+    m: MagicMock = mock_open(read_data="".join(MockGeolSIN))
     with patch("builtins.open", m):
-        n1 = Dvazmax.le_arquivo("")
-        n2 = Dvazmax.le_arquivo("")
+        n1 = GeolSIN.read(ARQ_TESTE)
+        n2 = GeolSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_eaf.py` & `inewave-0.0.96/tests/nwlistop/test_ghmax.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.eaf import Eaf
+from inewave.nwlistop.ghmax import Ghmax
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.eaf import MockEaf
+from tests.mocks.arquivos.ghmax import MockGhmax
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_eaf():
-    m: MagicMock = mock_open(read_data="".join(MockEaf))
+
+def test_atributos_encontrados_ghmax():
+    m: MagicMock = mock_open(read_data="".join(MockGhmax))
     with patch("builtins.open", m):
-        n = Eaf.le_arquivo("")
-        assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 2929.0
+        n = Ghmax.read(ARQ_TESTE)
         assert n.ree is not None
         assert n.ree == "SUDESTE"
+        assert n.valores is not None
+        assert n.valores.iloc[0, 0] == 2021
+        assert n.valores.iloc[-1, -1] == 7841.2
 
 
-def test_atributos_nao_encontrados_eaf():
+def test_atributos_nao_encontrados_ghmax():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Eaf.le_arquivo("")
-        assert n.valores is None
+        n = Ghmax.read(ARQ_TESTE)
         assert n.ree is None
+        assert n.valores is None
 
 
-def test_eq_eaf():
-    m: MagicMock = mock_open(read_data="".join(MockEaf))
+def test_eq_ghmax():
+    m: MagicMock = mock_open(read_data="".join(MockGhmax))
     with patch("builtins.open", m):
-        n1 = Eaf.le_arquivo("")
-        n2 = Eaf.le_arquivo("")
+        n1 = Ghmax.read(ARQ_TESTE)
+        n2 = Ghmax.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_eafb.py` & `inewave-0.0.96/tests/nwlistop/test_evertm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-from inewave.nwlistop.eafb import Eafb
+from inewave.nwlistop.evertm import Evertm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.eafb import MockEafb
+from tests.mocks.arquivos.evertm import MockEvertm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_eafb():
-    m: MagicMock = mock_open(read_data="".join(MockEafb))
+
+def test_atributos_encontrados_evertm():
+    m: MagicMock = mock_open(read_data="".join(MockEvertm))
     with patch("builtins.open", m):
-        n = Eafb.le_arquivo("")
+        n = Evertm.read(ARQ_TESTE)
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 4523.0
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        assert n.valores.iloc[-1, -1] == 146.0
 
 
-def test_atributos_nao_encontrados_eafb():
+def test_atributos_nao_encontrados_evertm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Eafb.le_arquivo("")
+        n = Evertm.read(ARQ_TESTE)
+        assert n.submercado is None
         assert n.valores is None
-        assert n.ree is None
 
 
-def test_eq_eafb():
-    m: MagicMock = mock_open(read_data="".join(MockEafb))
+def test_eq_evertm():
+    m: MagicMock = mock_open(read_data="".join(MockEvertm))
     with patch("builtins.open", m):
-        n1 = Eafb.le_arquivo("")
-        n2 = Eafb.le_arquivo("")
+        n1 = Evertm.read(ARQ_TESTE)
+        n2 = Evertm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_eafbm.py` & `inewave-0.0.96/tests/nwlistop/test_perdfm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-from inewave.nwlistop.eafbm import Eafbm
+from inewave.nwlistop.perdfm import Perdfm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.eafbm import MockEafbm
+from tests.mocks.arquivos.perdfm import MockPerdfm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_eafbm():
-    m: MagicMock = mock_open(read_data="".join(MockEafbm))
+
+def test_atributos_encontrados_perdfm():
+    m: MagicMock = mock_open(read_data="".join(MockPerdfm))
     with patch("builtins.open", m):
-        n = Eafbm.le_arquivo("")
-        assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 1995
-        assert n.valores.iloc[-1, -1] == 38424.0
-        assert n.submercado is not None
+        n = Perdfm.read(ARQ_TESTE)
         assert n.submercado == "SUDESTE"
+        assert n.valores is not None
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 231.0
 
 
-def test_atributos_nao_encontrados_eafbm():
+def test_atributos_nao_encontrados_perdfm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Eafbm.le_arquivo("")
-        assert n.valores is None
+        n = Perdfm.read(ARQ_TESTE)
         assert n.submercado is None
+        assert n.valores is None
 
 
-def test_eq_eafbm():
-    m: MagicMock = mock_open(read_data="".join(MockEafbm))
+def test_eq_perdfm():
+    m: MagicMock = mock_open(read_data="".join(MockPerdfm))
     with patch("builtins.open", m):
-        n1 = Eafbm.le_arquivo("")
-        n2 = Eafbm.le_arquivo("")
+        n1 = Perdfm.read(ARQ_TESTE)
+        n2 = Perdfm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_eafbsin.py` & `inewave-0.0.96/tests/nwlistop/test_eafbsin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from inewave.nwlistop.eafbsin import EafbSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.eafbsin import MockEafbSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_eafbsin():
     m: MagicMock = mock_open(read_data="".join(MockEafbSIN))
     with patch("builtins.open", m):
-        n = EafbSIN.le_arquivo("")
+        n = EafbSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 64920.0
 
 
 def test_atributos_nao_encontrados_eafbsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = EafbSIN.le_arquivo("")
+        n = EafbSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_eafbsin():
     m: MagicMock = mock_open(read_data="".join(MockEafbSIN))
     with patch("builtins.open", m):
-        n1 = EafbSIN.le_arquivo("")
-        n2 = EafbSIN.le_arquivo("")
+        n1 = EafbSIN.read(ARQ_TESTE)
+        n2 = EafbSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_eafm.py` & `inewave-0.0.96/tests/nwlistop/test_earmf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.eafm import Eafm
+from inewave.nwlistop.earmf import Earmf
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.eafm import MockEafm
+from tests.mocks.arquivos.earmf import MockEarmf
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_eafm():
-    m: MagicMock = mock_open(read_data="".join(MockEafm))
+
+def test_atributos_encontrados_earmf():
+    m: MagicMock = mock_open(read_data="".join(MockEarmf))
     with patch("builtins.open", m):
-        n = Eafm.le_arquivo("")
+        n = Earmf.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 17577.0
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        assert n.valores.iloc[-1, -1] == 20770.0
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_eafm():
+def test_atributos_nao_encontrados_earmf():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Eafm.le_arquivo("")
+        n = Earmf.read(ARQ_TESTE)
         assert n.valores is None
-        assert n.submercado is None
+        assert n.ree is None
 
 
-def test_eq_eafm():
-    m: MagicMock = mock_open(read_data="".join(MockEafm))
+def test_eq_earmf():
+    m: MagicMock = mock_open(read_data="".join(MockEarmf))
     with patch("builtins.open", m):
-        n1 = Eafm.le_arquivo("")
-        n2 = Eafm.le_arquivo("")
+        n1 = Earmf.read(ARQ_TESTE)
+        n2 = Earmf.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_earmf.py` & `inewave-0.0.96/tests/nwlistop/test_varmpuh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.earmf import Earmf
+from inewave.nwlistop.varmuh import VarmUH
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.earmf import MockEarmf
+from tests.mocks.arquivos.varmuh import MockVarmUH
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_earmf():
-    m: MagicMock = mock_open(read_data="".join(MockEarmf))
+
+def test_atributos_encontrados_varmuh():
+    m: MagicMock = mock_open(read_data="".join(MockVarmUH))
     with patch("builtins.open", m):
-        n = Earmf.le_arquivo("")
+        n = VarmUH.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 20770.0
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[-1, -1] == 662.80
 
 
-def test_atributos_nao_encontrados_earmf():
+def test_atributos_nao_encontrados_varmuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Earmf.le_arquivo("")
+        n = VarmUH.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
-        assert n.ree is None
 
 
-def test_eq_earmf():
-    m: MagicMock = mock_open(read_data="".join(MockEarmf))
+def test_eq_varmuh():
+    m: MagicMock = mock_open(read_data="".join(MockVarmUH))
     with patch("builtins.open", m):
-        n1 = Earmf.le_arquivo("")
-        n2 = Earmf.le_arquivo("")
+        n1 = VarmUH.read(ARQ_TESTE)
+        n2 = VarmUH.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_earmfm.py` & `inewave-0.0.96/tests/nwlistop/test_earmfm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.earmfm import Earmfm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.earmfm import MockEarmfm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_earmfm():
     m: MagicMock = mock_open(read_data="".join(MockEarmfm))
     with patch("builtins.open", m):
-        n = Earmfm.le_arquivo("")
+        n = Earmfm.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 122223.0
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_earmfm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Earmfm.le_arquivo("")
+        n = Earmfm.read(ARQ_TESTE)
         assert n.valores is None
         assert n.submercado is None
 
 
 def test_eq_earmfm():
     m: MagicMock = mock_open(read_data="".join(MockEarmfm))
     with patch("builtins.open", m):
-        n1 = Earmfm.le_arquivo("")
-        n2 = Earmfm.le_arquivo("")
+        n1 = Earmfm.read(ARQ_TESTE)
+        n2 = Earmfm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_earmfp.py` & `inewave-0.0.96/tests/nwlistop/test_eafb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.earmfp import Earmfp
+from inewave.nwlistop.eafb import Eafb
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.earmfp import MockEarmfp
+from tests.mocks.arquivos.eafb import MockEafb
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_earmfp():
-    m: MagicMock = mock_open(read_data="".join(MockEarmfp))
+
+def test_atributos_encontrados_eafb():
+    m: MagicMock = mock_open(read_data="".join(MockEafb))
     with patch("builtins.open", m):
-        n = Earmfp.le_arquivo("")
+        n = Eafb.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 71.2
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 4523.0
         assert n.ree is not None
         assert n.ree == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_earmfp():
+def test_atributos_nao_encontrados_eafb():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Earmfp.le_arquivo("")
+        n = Eafb.read(ARQ_TESTE)
         assert n.valores is None
         assert n.ree is None
 
 
-def test_eq_earmfp():
-    m: MagicMock = mock_open(read_data="".join(MockEarmfp))
+def test_eq_eafb():
+    m: MagicMock = mock_open(read_data="".join(MockEafb))
     with patch("builtins.open", m):
-        n1 = Earmfp.le_arquivo("")
-        n2 = Earmfp.le_arquivo("")
+        n1 = Eafb.read(ARQ_TESTE)
+        n2 = Eafb.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_earmfpm.py` & `inewave-0.0.96/tests/nwlistop/test_earmfpm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.earmfpm import Earmfpm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.earmfpm import MockEarmfpm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_earmfpm():
     m: MagicMock = mock_open(read_data="".join(MockEarmfpm))
     with patch("builtins.open", m):
-        n = Earmfpm.le_arquivo("")
+        n = Earmfpm.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 1995
         assert n.valores.iloc[-1, -1] == 63.0
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_earmfpm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Earmfpm.le_arquivo("")
+        n = Earmfpm.read(ARQ_TESTE)
         assert n.valores is None
         assert n.submercado is None
 
 
 def test_eq_earmfpm():
     m: MagicMock = mock_open(read_data="".join(MockEarmfpm))
     with patch("builtins.open", m):
-        n1 = Earmfpm.le_arquivo("")
-        n2 = Earmfpm.le_arquivo("")
+        n1 = Earmfpm.read(ARQ_TESTE)
+        n2 = Earmfpm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_earmfpsin.py` & `inewave-0.0.96/tests/nwlistop/test_earmfpsin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from inewave.nwlistop.earmfpsin import EarmfpSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.earmfpsin import MockEarmfpsin
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_earmfpsin():
     m: MagicMock = mock_open(read_data="".join(MockEarmfpsin))
     with patch("builtins.open", m):
-        n = EarmfpSIN.le_arquivo("")
+        n = EarmfpSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2021
         assert n.valores.iloc[-1, -1] == 42.1
 
 
 def test_atributos_nao_encontrados_earmfpsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = EarmfpSIN.le_arquivo("")
+        n = EarmfpSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_earmfpsin():
     m: MagicMock = mock_open(read_data="".join(MockEarmfpsin))
     with patch("builtins.open", m):
-        n1 = EarmfpSIN.le_arquivo("")
-        n2 = EarmfpSIN.le_arquivo("")
+        n1 = EarmfpSIN.read(ARQ_TESTE)
+        n2 = EarmfpSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_earmfsin.py` & `inewave-0.0.96/tests/nwlistop/test_earmfsin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from inewave.nwlistop.earmfsin import EarmfSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.earmfsin import MockEarmfSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_earmfsin():
     m: MagicMock = mock_open(read_data="".join(MockEarmfSIN))
     with patch("builtins.open", m):
-        n = EarmfSIN.le_arquivo("")
+        n = EarmfSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 177927.0
 
 
 def test_atributos_nao_encontrados_earmfsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = EarmfSIN.le_arquivo("")
+        n = EarmfSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_earmfsin():
     m: MagicMock = mock_open(read_data="".join(MockEarmfSIN))
     with patch("builtins.open", m):
-        n1 = EarmfSIN.le_arquivo("")
-        n2 = EarmfSIN.le_arquivo("")
+        n1 = EarmfSIN.read(ARQ_TESTE)
+        n2 = EarmfSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_evert.py` & `inewave-0.0.96/tests/nwlistop/test_evert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from inewave.nwlistop.evert import Evert
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.evert import MockEvert
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_evert():
     m: MagicMock = mock_open(read_data="".join(MockEvert))
     with patch("builtins.open", m):
-        n = Evert.le_arquivo("")
+        n = Evert.read(ARQ_TESTE)
         assert n.ree == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 24.0
 
 
 def test_atributos_nao_encontrados_evert():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Evert.le_arquivo("")
+        n = Evert.read(ARQ_TESTE)
         assert n.ree is None
         assert n.valores is None
 
 
 def test_eq_evert():
     m: MagicMock = mock_open(read_data="".join(MockEvert))
     with patch("builtins.open", m):
-        n1 = Evert.le_arquivo("")
-        n2 = Evert.le_arquivo("")
+        n1 = Evert.read(ARQ_TESTE)
+        n2 = Evert.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_evertm.py` & `inewave-0.0.96/tests/nwlistop/test_eafbm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-from inewave.nwlistop.evertm import Evertm
+from inewave.nwlistop.eafbm import Eafbm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.evertm import MockEvertm
+from tests.mocks.arquivos.eafbm import MockEafbm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_evertm():
-    m: MagicMock = mock_open(read_data="".join(MockEvertm))
+
+def test_atributos_encontrados_eafbm():
+    m: MagicMock = mock_open(read_data="".join(MockEafbm))
     with patch("builtins.open", m):
-        n = Evertm.le_arquivo("")
-        assert n.submercado == "SUDESTE"
+        n = Eafbm.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 146.0
+        assert n.valores.iloc[0, 0] == 1995
+        assert n.valores.iloc[-1, -1] == 38424.0
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_evertm():
+def test_atributos_nao_encontrados_eafbm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Evertm.le_arquivo("")
-        assert n.submercado is None
+        n = Eafbm.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.submercado is None
 
 
-def test_eq_evertm():
-    m: MagicMock = mock_open(read_data="".join(MockEvertm))
+def test_eq_eafbm():
+    m: MagicMock = mock_open(read_data="".join(MockEafbm))
     with patch("builtins.open", m):
-        n1 = Evertm.le_arquivo("")
-        n2 = Evertm.le_arquivo("")
+        n1 = Eafbm.read(ARQ_TESTE)
+        n2 = Eafbm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_evertsin.py` & `inewave-0.0.96/tests/nwlistop/test_perdfsin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.evertsin import EvertSIN
+from inewave.nwlistop.perdfsin import PerdfSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.evertsin import MockEvertSIN
+from tests.mocks.arquivos.perdfsin import MockPerdfSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_evertsin():
-    m: MagicMock = mock_open(read_data="".join(MockEvertSIN))
+
+def test_atributos_encontrados_perdfsin():
+    m: MagicMock = mock_open(read_data="".join(MockPerdfSIN))
     with patch("builtins.open", m):
-        n = EvertSIN.le_arquivo("")
+        n = PerdfSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 146.0
+        assert n.valores.iloc[-1, -1] == 438.0
 
 
-def test_atributos_nao_encontrados_evertsin():
+def test_atributos_nao_encontrados_perdfsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = EvertSIN.le_arquivo("")
+        n = PerdfSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_evertsin():
-    m: MagicMock = mock_open(read_data="".join(MockEvertSIN))
+def test_eq_perdfsin():
+    m: MagicMock = mock_open(read_data="".join(MockPerdfSIN))
     with patch("builtins.open", m):
-        n1 = EvertSIN.le_arquivo("")
-        n2 = EvertSIN.le_arquivo("")
+        n1 = PerdfSIN.read(ARQ_TESTE)
+        n2 = PerdfSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_exces.py` & `inewave-0.0.96/tests/nwlistop/test_exces.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.exces import Exces
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.exces import MockExces
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_exces():
     m: MagicMock = mock_open(read_data="".join(MockExces))
     with patch("builtins.open", m):
-        n = Exces.le_arquivo("")
+        n = Exces.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_exces():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Exces.le_arquivo("")
+        n = Exces.read(ARQ_TESTE)
         assert n.submercado is None
         assert n.valores is None
 
 
 def test_eq_exces():
     m: MagicMock = mock_open(read_data="".join(MockExces))
     with patch("builtins.open", m):
-        n1 = Exces.le_arquivo("")
-        n2 = Exces.le_arquivo("")
+        n1 = Exces.read(ARQ_TESTE)
+        n2 = Exces.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_excessin.py` & `inewave-0.0.96/tests/nwlistop/test_defsin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.excessin import ExcesSIN
+from inewave.nwlistop.defsin import DefSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.excessin import MockExcesSIN
+from tests.mocks.arquivos.defsin import MockDefSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_excessin():
-    m: MagicMock = mock_open(read_data="".join(MockExcesSIN))
+
+def test_atributos_encontrados_defsin():
+    m: MagicMock = mock_open(read_data="".join(MockDefSIN))
     with patch("builtins.open", m):
-        n = ExcesSIN.le_arquivo("")
+        n = DefSIN.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_excessin():
+def test_atributos_nao_encontrados_defsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = ExcesSIN.le_arquivo("")
+        n = DefSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_excessin():
-    m: MagicMock = mock_open(read_data="".join(MockExcesSIN))
+def test_eq_defsin():
+    m: MagicMock = mock_open(read_data="".join(MockDefSIN))
     with patch("builtins.open", m):
-        n1 = ExcesSIN.le_arquivo("")
-        n2 = ExcesSIN.le_arquivo("")
+        n1 = DefSIN.read(ARQ_TESTE)
+        n2 = DefSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_fteolm.py` & `inewave-0.0.96/tests/nwlistop/test_cdef.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.fteolm import Fteolm
+from inewave.nwlistop.cdef import Cdef
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.fteolm import MockFteolm
+from tests.mocks.arquivos.cdef import MockCdef
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_fteolm():
-    m: MagicMock = mock_open(read_data="".join(MockFteolm))
+
+def test_atributos_encontrados_cdef():
+    m: MagicMock = mock_open(read_data="".join(MockCdef))
     with patch("builtins.open", m):
-        n = Fteolm.le_arquivo("")
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        n = Cdef.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 0.0
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_fteolm():
+def test_atributos_nao_encontrados_cdef():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Fteolm.le_arquivo("")
-        assert n.submercado is None
+        n = Cdef.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.submercado is None
 
 
-def test_eq_fteolm():
-    m: MagicMock = mock_open(read_data="".join(MockFteolm))
+def test_eq_cdef():
+    m: MagicMock = mock_open(read_data="".join(MockCdef))
     with patch("builtins.open", m):
-        n1 = Fteolm.le_arquivo("")
-        n2 = Fteolm.le_arquivo("")
+        n1 = Cdef.read(ARQ_TESTE)
+        n2 = Cdef.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_fteolsin.py` & `inewave-0.0.96/tests/nwlistop/test_merclsin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.fteolsin import FteolSIN
+from inewave.nwlistop.merclsin import MerclSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.fteolsin import MockFteolSIN
+from tests.mocks.arquivos.merclsin import MockMerclSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_fteolsin():
-    m: MagicMock = mock_open(read_data="".join(MockFteolSIN))
+
+def test_atributos_encontrados_merclsin():
+    m: MagicMock = mock_open(read_data="".join(MockMerclSIN))
     with patch("builtins.open", m):
-        n = FteolSIN.le_arquivo("")
+        n = MerclSIN.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[-1, -2] == 56819.0
 
 
-def test_atributos_nao_encontrados_fteolsin():
+def test_atributos_nao_encontrados_merclsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = FteolSIN.le_arquivo("")
+        n = MerclSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_fteolsin():
-    m: MagicMock = mock_open(read_data="".join(MockFteolSIN))
+def test_eq_merclsin():
+    m: MagicMock = mock_open(read_data="".join(MockMerclSIN))
     with patch("builtins.open", m):
-        n1 = FteolSIN.le_arquivo("")
-        n2 = FteolSIN.le_arquivo("")
+        n1 = MerclSIN.read(ARQ_TESTE)
+        n2 = MerclSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_geol.py` & `inewave-0.0.96/tests/nwlistop/test_geol.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.geol import Geol
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.geol import MockGeol
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_geol():
     m: MagicMock = mock_open(read_data="".join(MockGeol))
     with patch("builtins.open", m):
-        n = Geol.le_arquivo("")
+        n = Geol.read(ARQ_TESTE)
         assert n.usina is not None
         # assert n.pee == "cluster_NE_1"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2021
         assert n.valores.iloc[-1, -1] == 2652.7
 
 
 def test_atributos_nao_encontrados_geol():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Geol.le_arquivo("")
+        n = Geol.read(ARQ_TESTE)
         assert n.usina is None
         assert n.valores is None
 
 
 def test_eq_geol():
     m: MagicMock = mock_open(read_data="".join(MockGeol))
     with patch("builtins.open", m):
-        n1 = Geol.le_arquivo("")
-        n2 = Geol.le_arquivo("")
+        n1 = Geol.read(ARQ_TESTE)
+        n2 = Geol.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_geolm.py` & `inewave-0.0.96/tests/nwlistop/test_vevminm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.geolm import Geolm
+from inewave.nwlistop.vevminm import Vevminm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.geolm import MockGeolm
+from tests.mocks.arquivos.vevminm import MockVevminm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_geolm():
-    m: MagicMock = mock_open(read_data="".join(MockGeolm))
+
+def test_atributos_encontrados_vevminm():
+    m: MagicMock = mock_open(read_data="".join(MockVevminm))
     with patch("builtins.open", m):
-        n = Geolm.le_arquivo("")
-        assert n.submercado is not None
-        assert n.submercado == "NORDESTE"
+        n = Vevminm.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 5850.4
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_geolm():
+def test_atributos_nao_encontrados_vevminm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Geolm.le_arquivo("")
-        assert n.submercado is None
+        n = Vevminm.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.submercado is None
 
 
-def test_eq_geolm():
-    m: MagicMock = mock_open(read_data="".join(MockGeolm))
+def test_eq_vevminm():
+    m: MagicMock = mock_open(read_data="".join(MockVevminm))
     with patch("builtins.open", m):
-        n1 = Geolm.le_arquivo("")
-        n2 = Geolm.le_arquivo("")
+        n1 = Vevminm.read(ARQ_TESTE)
+        n2 = Vevminm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_geolsin.py` & `inewave-0.0.96/tests/nwlistop/test_verturbsin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.geolsin import GeolSIN
+from inewave.nwlistop.verturbsin import VerturbSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.geolsin import MockGeolSIN
+from tests.mocks.arquivos.verturbsin import MockVerturbSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_geolsin():
-    m: MagicMock = mock_open(read_data="".join(MockGeolSIN))
+
+def test_atributos_encontrados_verturbsin():
+    m: MagicMock = mock_open(read_data="".join(MockVerturbSIN))
     with patch("builtins.open", m):
-        n = GeolSIN.le_arquivo("")
+        n = VerturbSIN.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 6574.3
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == -29007.0
 
 
-def test_atributos_nao_encontrados_geolsin():
+def test_atributos_nao_encontrados_verturbsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GeolSIN.le_arquivo("")
+        n = VerturbSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_geolsin():
-    m: MagicMock = mock_open(read_data="".join(MockGeolSIN))
+def test_eq_verturbsin():
+    m: MagicMock = mock_open(read_data="".join(MockVerturbSIN))
     with patch("builtins.open", m):
-        n1 = GeolSIN.le_arquivo("")
-        n2 = GeolSIN.le_arquivo("")
+        n1 = VerturbSIN.read(ARQ_TESTE)
+        n2 = VerturbSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ghiduh.py` & `inewave-0.0.96/tests/nwlistop/test_vagua.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.ghiduh import GhidUH
+from inewave.nwlistop.vagua import Vagua
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghiduh import MockGhidUH
+from tests.mocks.arquivos.vagua import MockVagua
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_ghiduh():
-    m: MagicMock = mock_open(read_data="".join(MockGhidUH))
+
+def test_atributos_encontrados_vagua():
+    m: MagicMock = mock_open(read_data="".join(MockVagua))
     with patch("builtins.open", m):
-        n = GhidUH.le_arquivo("")
-        assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        n = Vagua.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 8.21
+        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[-1, -1] == -1.90
 
 
-def test_atributos_nao_encontrados_ghiduh():
+def test_atributos_nao_encontrados_vagua():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GhidUH.le_arquivo("")
-        assert n.usina is None
+        n = Vagua.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_ghiduh():
-    m: MagicMock = mock_open(read_data="".join(MockGhidUH))
+def test_eq_vagua():
+    m: MagicMock = mock_open(read_data="".join(MockVagua))
     with patch("builtins.open", m):
-        n1 = GhidUH.le_arquivo("")
-        n2 = GhidUH.le_arquivo("")
+        n1 = Vagua.read(ARQ_TESTE)
+        n2 = Vagua.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ghmax.py` & `inewave-0.0.96/tests/nwlistop/test_ghmaxrsin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from inewave.nwlistop.ghmax import Ghmax
+from inewave.nwlistop.ghmaxrsin import GhmaxrSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghmax import MockGhmax
+from tests.mocks.arquivos.ghmaxrsin import MockGhmaxrSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_ghmax():
-    m: MagicMock = mock_open(read_data="".join(MockGhmax))
+
+def test_atributos_encontrados_ghmaxrsin():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxrSIN))
     with patch("builtins.open", m):
-        n = Ghmax.le_arquivo("")
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        n = GhmaxrSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 7841.2
+        assert n.valores.iloc[-1, -1] == 94172.9
 
 
-def test_atributos_nao_encontrados_ghmax():
+def test_atributos_nao_encontrados_ghmaxrsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Ghmax.le_arquivo("")
-        assert n.ree is None
+        n = GhmaxrSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_ghmax():
-    m: MagicMock = mock_open(read_data="".join(MockGhmax))
+def test_eq_ghmaxrsin():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxrSIN))
     with patch("builtins.open", m):
-        n1 = Ghmax.le_arquivo("")
-        n2 = Ghmax.le_arquivo("")
+        n1 = GhmaxrSIN.read(ARQ_TESTE)
+        n2 = GhmaxrSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ghmaxm.py` & `inewave-0.0.96/tests/nwlistop/test_gttot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.ghmaxm import Ghmaxm
+from inewave.nwlistop.gttot import Gttot
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghmaxm import MockGhmaxm
+from tests.mocks.arquivos.gttot import MockGttot
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_ghmaxm():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxm))
+
+def test_atributos_encontrados_gttot():
+    m: MagicMock = mock_open(read_data="".join(MockGttot))
     with patch("builtins.open", m):
-        n = Ghmaxm.le_arquivo("")
+        n = Gttot.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 54602.6
+        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[-1, -1] == 2710.5
 
 
-def test_atributos_nao_encontrados_ghmaxm():
+def test_atributos_nao_encontrados_gttot():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Ghmaxm.le_arquivo("")
+        n = Gttot.read(ARQ_TESTE)
         assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_ghmaxm():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxm))
+def test_eq_gttot():
+    m: MagicMock = mock_open(read_data="".join(MockGttot))
     with patch("builtins.open", m):
-        n1 = Ghmaxm.le_arquivo("")
-        n2 = Ghmaxm.le_arquivo("")
+        n1 = Gttot.read(ARQ_TESTE)
+        n2 = Gttot.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ghmaxmr.py` & `inewave-0.0.96/tests/nwlistop/test_ghmaxmr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.ghmaxmr import Ghmaxmr
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.ghmaxmr import MockGhmaxmr
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_ghmaxmr():
     m: MagicMock = mock_open(read_data="".join(MockGhmaxmr))
     with patch("builtins.open", m):
-        n = Ghmaxmr.le_arquivo("")
+        n = Ghmaxmr.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2021
         assert n.valores.iloc[-1, -1] == 54233.6
 
 
 def test_atributos_nao_encontrados_ghmaxmr():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Ghmaxmr.le_arquivo("")
+        n = Ghmaxmr.read(ARQ_TESTE)
         assert n.submercado is None
         assert n.valores is None
 
 
 def test_eq_ghmaxmr():
     m: MagicMock = mock_open(read_data="".join(MockGhmaxmr))
     with patch("builtins.open", m):
-        n1 = Ghmaxmr.le_arquivo("")
-        n2 = Ghmaxmr.le_arquivo("")
+        n1 = Ghmaxmr.read(ARQ_TESTE)
+        n2 = Ghmaxmr.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ghmaxr.py` & `inewave-0.0.96/tests/nwlistop/test_ghmaxr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.ghmaxr import Ghmaxr
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.ghmaxr import MockGhmaxr
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_ghmaxr():
     m: MagicMock = mock_open(read_data="".join(MockGhmaxr))
     with patch("builtins.open", m):
-        n = Ghmaxr.le_arquivo("")
+        n = Ghmaxr.read(ARQ_TESTE)
         assert n.ree is not None
         assert n.ree == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2021
         assert n.valores.iloc[-1, -1] == 7686.3
 
 
 def test_atributos_nao_encontrados_ghmaxr():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Ghmaxr.le_arquivo("")
+        n = Ghmaxr.read(ARQ_TESTE)
         assert n.ree is None
         assert n.valores is None
 
 
 def test_eq_ghmaxr():
     m: MagicMock = mock_open(read_data="".join(MockGhmaxr))
     with patch("builtins.open", m):
-        n1 = Ghmaxr.le_arquivo("")
-        n2 = Ghmaxr.le_arquivo("")
+        n1 = Ghmaxr.read(ARQ_TESTE)
+        n2 = Ghmaxr.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ghmaxrsin.py` & `inewave-0.0.96/tests/nwlistop/test_dlpptbmax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from inewave.nwlistop.ghmaxrsin import GhmaxrSIN
+from inewave.nwlistop.dlpptbmax import DLPPtbmax
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghmaxrsin import MockGhmaxrSIN
+from tests.mocks.arquivos.dlpptbmax import MockDLPPtbmax
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_ghmaxrsin():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxrSIN))
+
+def test_atributos_encontrados_dlpptbmax():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmax))
     with patch("builtins.open", m):
-        n = GhmaxrSIN.le_arquivo("")
+        n = DLPPtbmax.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 94172.9
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_ghmaxrsin():
+def test_atributos_nao_encontrados_dlpptbmax():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GhmaxrSIN.le_arquivo("")
+        n = DLPPtbmax.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_ghmaxrsin():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxrSIN))
+def test_eq_dlpptbmax():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmax))
     with patch("builtins.open", m):
-        n1 = GhmaxrSIN.le_arquivo("")
-        n2 = GhmaxrSIN.le_arquivo("")
+        n1 = DLPPtbmax.read(ARQ_TESTE)
+        n2 = DLPPtbmax.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ghmaxsin.py` & `inewave-0.0.96/tests/nwlistop/test_dlppdfmax.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from inewave.nwlistop.ghmaxsin import GhmaxSIN
+from inewave.nwlistop.dlppdfmax import DLPPdfmax
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghmaxsin import MockGhmaxSIN
+from tests.mocks.arquivos.dlppdfmax import MockDLPPdfmax
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_ghmaxsin():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxSIN))
+
+def test_atributos_encontrados_dlppdfmax():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmax))
     with patch("builtins.open", m):
-        n = GhmaxSIN.le_arquivo("")
+        n = DLPPdfmax.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 97716.9
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_ghmaxsin():
+def test_atributos_nao_encontrados_dlppdfmax():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GhmaxSIN.le_arquivo("")
+        n = DLPPdfmax.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_ghmaxsin():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxSIN))
+def test_eq_dlppdfmax():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmax))
     with patch("builtins.open", m):
-        n1 = GhmaxSIN.le_arquivo("")
-        n2 = GhmaxSIN.le_arquivo("")
+        n1 = DLPPdfmax.read(ARQ_TESTE)
+        n2 = DLPPdfmax.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ghtot.py` & `inewave-0.0.96/tests/nwlistop/test_ghtot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from inewave.nwlistop.ghtot import Ghtot
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.ghtot import MockGhtot
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
+
 
 def test_atributos_encontrados_ghtot():
     m: MagicMock = mock_open(read_data="".join(MockGhtot))
     with patch("builtins.open", m):
-        n = Ghtot.le_arquivo("")
+        n = Ghtot.read(ARQ_TESTE)
         assert n.ree is not None
         assert n.ree == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 2578.7
 
 
 def test_atributos_nao_encontrados_ghtot():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Ghtot.le_arquivo("")
+        n = Ghtot.read(ARQ_TESTE)
         assert n.ree is None
         assert n.valores is None
 
 
 def test_eq_ghtot():
     m: MagicMock = mock_open(read_data="".join(MockGhtot))
     with patch("builtins.open", m):
-        n1 = Ghtot.le_arquivo("")
-        n2 = Ghtot.le_arquivo("")
+        n1 = Ghtot.read(ARQ_TESTE)
+        n2 = Ghtot.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ghtotm.py` & `inewave-0.0.96/tests/nwlistop/test_verturbm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.ghtotm import Ghtotm
+from inewave.nwlistop.verturbm import Verturbm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghtotm import MockGhtotm
+from tests.mocks.arquivos.verturbm import MockVerturbm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_ghtotm():
-    m: MagicMock = mock_open(read_data="".join(MockGhtotm))
+
+def test_atributos_encontrados_verturbm():
+    m: MagicMock = mock_open(read_data="".join(MockVerturbm))
     with patch("builtins.open", m):
-        n = Ghtotm.le_arquivo("")
+        n = Verturbm.read(ARQ_TESTE)
+        assert n.valores is not None
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 0.0
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
-        assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 24494.9
 
 
-def test_atributos_nao_encontrados_ghtotm():
+def test_atributos_nao_encontrados_verturbm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Ghtotm.le_arquivo("")
-        assert n.submercado is None
+        n = Verturbm.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.submercado is None
 
 
-def test_eq_ghtotm():
-    m: MagicMock = mock_open(read_data="".join(MockGhtotm))
+def test_eq_verturbm():
+    m: MagicMock = mock_open(read_data="".join(MockVerturbm))
     with patch("builtins.open", m):
-        n1 = Ghtotm.le_arquivo("")
-        n2 = Ghtotm.le_arquivo("")
+        n1 = Verturbm.read(ARQ_TESTE)
+        n2 = Verturbm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_ghtotsin.py` & `inewave-0.0.96/tests/nwlistop/test_vevminsin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.ghtotsin import GhtotSIN
+from inewave.nwlistop.vevminsin import VevminSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghtotsin import MockGhtotsin
+from tests.mocks.arquivos.vevminsin import MockVevminSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_ghtotsin():
-    m: MagicMock = mock_open(read_data="".join(MockGhtotsin))
+
+def test_atributos_encontrados_vevminsin():
+    m: MagicMock = mock_open(read_data="".join(MockVevminSIN))
     with patch("builtins.open", m):
-        n = GhtotSIN.le_arquivo("")
+        n = VevminSIN.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 46994.0
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_ghtotsin():
+def test_atributos_nao_encontrados_vevminsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GhtotSIN.le_arquivo("")
+        n = VevminSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_ghtotsin():
-    m: MagicMock = mock_open(read_data="".join(MockGhtotsin))
+def test_eq_vevminsin():
+    m: MagicMock = mock_open(read_data="".join(MockVevminSIN))
     with patch("builtins.open", m):
-        n1 = GhtotSIN.le_arquivo("")
-        n2 = GhtotSIN.le_arquivo("")
+        n1 = VevminSIN.read(ARQ_TESTE)
+        n2 = VevminSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_gttot.py` & `inewave-0.0.96/tests/nwlistop/test_varmuh.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.gttot import Gttot
+from inewave.nwlistop.varmpuh import VarmpUH
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.gttot import MockGttot
+from tests.mocks.arquivos.varmpuh import MockVarmpUH
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_gttot():
-    m: MagicMock = mock_open(read_data="".join(MockGttot))
+
+def test_atributos_encontrados_varmpuh():
+    m: MagicMock = mock_open(read_data="".join(MockVarmpUH))
     with patch("builtins.open", m):
-        n = Gttot.le_arquivo("")
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        n = VarmpUH.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 2710.5
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 95.35
 
 
-def test_atributos_nao_encontrados_gttot():
+def test_atributos_nao_encontrados_varmpuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Gttot.le_arquivo("")
-        assert n.submercado is None
+        n = VarmpUH.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_gttot():
-    m: MagicMock = mock_open(read_data="".join(MockGttot))
+def test_eq_varmpuh():
+    m: MagicMock = mock_open(read_data="".join(MockVarmpUH))
     with patch("builtins.open", m):
-        n1 = Gttot.le_arquivo("")
-        n2 = Gttot.le_arquivo("")
+        n1 = VarmpUH.read(ARQ_TESTE)
+        n2 = VarmpUH.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_gttotsin.py` & `inewave-0.0.96/tests/nwlistop/test_excessin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.gttotsin import GttotSIN
+from inewave.nwlistop.excessin import ExcesSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.gttotsin import MockGttotsin
+from tests.mocks.arquivos.excessin import MockExcesSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_gttotsin():
-    m: MagicMock = mock_open(read_data="".join(MockGttotsin))
+
+def test_atributos_encontrados_excessin():
+    m: MagicMock = mock_open(read_data="".join(MockExcesSIN))
     with patch("builtins.open", m):
-        n = GttotSIN.le_arquivo("")
+        n = ExcesSIN.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 5106.0
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_gttotsin():
+def test_atributos_nao_encontrados_excessin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GttotSIN.le_arquivo("")
+        n = ExcesSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_gttotsin():
-    m: MagicMock = mock_open(read_data="".join(MockGttotsin))
+def test_eq_excessin():
+    m: MagicMock = mock_open(read_data="".join(MockExcesSIN))
     with patch("builtins.open", m):
-        n1 = GttotSIN.le_arquivo("")
-        n2 = GttotSIN.le_arquivo("")
+        n1 = ExcesSIN.read(ARQ_TESTE)
+        n2 = ExcesSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_invade.py` & `inewave-0.0.96/tests/nwlistop/test_invadem.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.invade import Invade
+from inewave.nwlistop.invadem import Invadem
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.invade import MockInvade
+from tests.mocks.arquivos.invadem import MockInvadem
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_invade():
-    m: MagicMock = mock_open(read_data="".join(MockInvade))
+
+def test_atributos_encontrados_invadem():
+    m: MagicMock = mock_open(read_data="".join(MockInvadem))
     with patch("builtins.open", m):
-        n = Invade.le_arquivo("")
+        n = Invadem.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_invade():
+def test_atributos_nao_encontrados_invadem():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Invade.le_arquivo("")
+        n = Invadem.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_invade():
-    m: MagicMock = mock_open(read_data="".join(MockInvade))
+def test_eq_invadem():
+    m: MagicMock = mock_open(read_data="".join(MockInvadem))
     with patch("builtins.open", m):
-        n1 = Invade.le_arquivo("")
-        n2 = Invade.le_arquivo("")
+        n1 = Invadem.read(ARQ_TESTE)
+        n2 = Invadem.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_invadem.py` & `inewave-0.0.96/tests/nwlistop/test_invade.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.invadem import Invadem
+from inewave.nwlistop.invade import Invade
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.invadem import MockInvadem
+from tests.mocks.arquivos.invade import MockInvade
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_invadem():
-    m: MagicMock = mock_open(read_data="".join(MockInvadem))
+
+def test_atributos_encontrados_invade():
+    m: MagicMock = mock_open(read_data="".join(MockInvade))
     with patch("builtins.open", m):
-        n = Invadem.le_arquivo("")
+        n = Invade.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_invadem():
+def test_atributos_nao_encontrados_invade():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Invadem.le_arquivo("")
+        n = Invade.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_invadem():
-    m: MagicMock = mock_open(read_data="".join(MockInvadem))
+def test_eq_invade():
+    m: MagicMock = mock_open(read_data="".join(MockInvade))
     with patch("builtins.open", m):
-        n1 = Invadem.le_arquivo("")
-        n2 = Invadem.le_arquivo("")
+        n1 = Invade.read(ARQ_TESTE)
+        n2 = Invade.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_mercl.py` & `inewave-0.0.96/tests/nwlistop/test_ghiduh.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-from inewave.nwlistop.mercl import Mercl
+from inewave.nwlistop.ghiduh import GhidUH
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.mercl import MockMercl
+from tests.mocks.arquivos.ghiduh import MockGhidUH
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_mercl():
-    m: MagicMock = mock_open(read_data="".join(MockMercl))
+
+def test_atributos_encontrados_ghiduh():
+    m: MagicMock = mock_open(read_data="".join(MockGhidUH))
     with patch("builtins.open", m):
-        n = Mercl.le_arquivo("")
+        n = GhidUH.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        print(n.valores)
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -2] == 37783.0
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == 8.21
 
 
-def test_atributos_nao_encontrados_mercl():
+def test_atributos_nao_encontrados_ghiduh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Mercl.le_arquivo("")
+        n = GhidUH.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
-        assert n.submercado is None
 
 
-def test_eq_mercl():
-    m: MagicMock = mock_open(read_data="".join(MockMercl))
+def test_eq_ghiduh():
+    m: MagicMock = mock_open(read_data="".join(MockGhidUH))
     with patch("builtins.open", m):
-        n1 = Mercl.le_arquivo("")
-        n2 = Mercl.le_arquivo("")
+        n1 = GhidUH.read(ARQ_TESTE)
+        n2 = GhidUH.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_merclsin.py` & `inewave-0.0.96/tests/nwlistop/test_deficit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from inewave.nwlistop.merclsin import MerclSIN
+from inewave.nwlistop.deficit import Def
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.merclsin import MockMerclSIN
+from tests.mocks.arquivos.deficit import MockDef
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_merclsin():
-    m: MagicMock = mock_open(read_data="".join(MockMerclSIN))
+
+def test_atributos_encontrados_def():
+    m: MagicMock = mock_open(read_data="".join(MockDef))
     with patch("builtins.open", m):
-        n = MerclSIN.le_arquivo("")
+        n = Def.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -2] == 56819.0
+        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_merclsin():
+def test_atributos_nao_encontrados_def():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = MerclSIN.le_arquivo("")
+        n = Def.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.submercado is None
 
 
-def test_eq_merclsin():
-    m: MagicMock = mock_open(read_data="".join(MockMerclSIN))
+def test_eq_def():
+    m: MagicMock = mock_open(read_data="".join(MockDef))
     with patch("builtins.open", m):
-        n1 = MerclSIN.le_arquivo("")
-        n2 = MerclSIN.le_arquivo("")
+        n1 = Def.read(ARQ_TESTE)
+        n2 = Def.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_perdf.py` & `inewave-0.0.96/tests/nwlistop/test_dfphauh.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-from inewave.nwlistop.perdf import Perdf
+from inewave.nwlistop.dfphauh import Dfphauh
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.perdf import MockPerdf
+from tests.mocks.arquivos.dfphauh import MockDfphauh
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_perdf():
-    m: MagicMock = mock_open(read_data="".join(MockPerdf))
+
+def test_atributos_encontrados_fphauh():
+    m: MagicMock = mock_open(read_data="".join(MockDfphauh))
     with patch("builtins.open", m):
-        n = Perdf.le_arquivo("")
-        assert n.ree == "SUDESTE"
+        n = Dfphauh.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 230.0
+        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_perdf():
+def test_atributos_nao_encontrados_fphauh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Perdf.le_arquivo("")
-        assert n.ree is None
+        n = Dfphauh.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_perdf():
-    m: MagicMock = mock_open(read_data="".join(MockPerdf))
+def test_eq_fphauh():
+    m: MagicMock = mock_open(read_data="".join(MockDfphauh))
     with patch("builtins.open", m):
-        n1 = Perdf.le_arquivo("")
-        n2 = Perdf.le_arquivo("")
+        n1 = Dfphauh.read(ARQ_TESTE)
+        n2 = Dfphauh.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_perdfm.py` & `inewave-0.0.96/tests/nwlistop/test_qafluh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-from inewave.nwlistop.perdfm import Perdfm
+from inewave.nwlistop.qafluh import QaflUH
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.perdfm import MockPerdfm
+from tests.mocks.arquivos.qafluh import MockQaflUH
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_perdfm():
-    m: MagicMock = mock_open(read_data="".join(MockPerdfm))
+
+def test_atributos_encontrados_qafluh():
+    m: MagicMock = mock_open(read_data="".join(MockQaflUH))
     with patch("builtins.open", m):
-        n = Perdfm.le_arquivo("")
-        assert n.submercado == "SUDESTE"
+        n = QaflUH.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 231.0
+        assert n.valores.iloc[-1, -1] == 105.02
 
 
-def test_atributos_nao_encontrados_perdfm():
+def test_atributos_nao_encontrados_qafluh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Perdfm.le_arquivo("")
-        assert n.submercado is None
+        n = QaflUH.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_perdfm():
-    m: MagicMock = mock_open(read_data="".join(MockPerdfm))
+def test_eq_qafluh():
+    m: MagicMock = mock_open(read_data="".join(MockQaflUH))
     with patch("builtins.open", m):
-        n1 = Perdfm.le_arquivo("")
-        n2 = Perdfm.le_arquivo("")
+        n1 = QaflUH.read(ARQ_TESTE)
+        n2 = QaflUH.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_perdfsin.py` & `inewave-0.0.96/tests/nwlistop/test_rhslppdf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from inewave.nwlistop.perdfsin import PerdfSIN
+from inewave.nwlistop.rhslppdf import RHSLPPdf
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.perdfsin import MockPerdfSIN
+from tests.mocks.arquivos.rhslppdf import MockRHSLPPdf
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_perdfsin():
-    m: MagicMock = mock_open(read_data="".join(MockPerdfSIN))
+
+def test_atributos_encontrados_rhslppdf():
+    m: MagicMock = mock_open(read_data="".join(MockRHSLPPdf))
     with patch("builtins.open", m):
-        n = PerdfSIN.le_arquivo("")
+        n = RHSLPPdf.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 438.0
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_perdfsin():
+def test_atributos_nao_encontrados_rhslppdf():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = PerdfSIN.le_arquivo("")
+        n = RHSLPPdf.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_perdfsin():
-    m: MagicMock = mock_open(read_data="".join(MockPerdfSIN))
+def test_eq_rhslppdf():
+    m: MagicMock = mock_open(read_data="".join(MockRHSLPPdf))
     with patch("builtins.open", m):
-        n1 = PerdfSIN.le_arquivo("")
-        n2 = PerdfSIN.le_arquivo("")
+        n1 = RHSLPPdf.read(ARQ_TESTE)
+        n2 = RHSLPPdf.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_qafluh.py` & `inewave-0.0.96/tests/nwlistop/test_cterm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.qafluh import QaflUH
+from inewave.nwlistop.cterm import Cterm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.qafluh import MockQaflUH
+from tests.mocks.arquivos.cterm import MockCterm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_qafluh():
-    m: MagicMock = mock_open(read_data="".join(MockQaflUH))
+
+def test_atributos_encontrados_cterm():
+    m: MagicMock = mock_open(read_data="".join(MockCterm))
     with patch("builtins.open", m):
-        n = QaflUH.le_arquivo("")
-        assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        n = Cterm.read(ARQ_TESTE)
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 105.02
+        assert n.valores.iloc[0, 0] == 2021
+        assert n.valores.iloc[-1, -1] == 585.36
 
 
-def test_atributos_nao_encontrados_qafluh():
+def test_atributos_nao_encontrados_cterm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = QaflUH.le_arquivo("")
-        assert n.usina is None
+        n = Cterm.read(ARQ_TESTE)
+        assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_qafluh():
-    m: MagicMock = mock_open(read_data="".join(MockQaflUH))
+def test_eq_cterm():
+    m: MagicMock = mock_open(read_data="".join(MockCterm))
     with patch("builtins.open", m):
-        n1 = QaflUH.le_arquivo("")
-        n2 = QaflUH.le_arquivo("")
+        n1 = Cterm.read(ARQ_TESTE)
+        n2 = Cterm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_qincruh.py` & `inewave-0.0.96/tests/nwlistop/test_vghminuh.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.qincruh import QincrUH
+from inewave.nwlistop.vghminuh import VghminUH
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.qincruh import MockQincrUH
+from tests.mocks.arquivos.vghminuh import MockVghminUH
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_qincruh():
-    m: MagicMock = mock_open(read_data="".join(MockQincrUH))
+
+def test_atributos_encontrados_vghminuh():
+    m: MagicMock = mock_open(read_data="".join(MockVghminUH))
     with patch("builtins.open", m):
-        n = QincrUH.le_arquivo("")
+        n = VghminUH.read(ARQ_TESTE)
         assert n.usina is not None
         assert n.usina == "CAMARGOS"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 105.02
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_qincruh():
+def test_atributos_nao_encontrados_vghminuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = QincrUH.le_arquivo("")
+        n = VghminUH.read(ARQ_TESTE)
         assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_qincruh():
-    m: MagicMock = mock_open(read_data="".join(MockQincrUH))
+def test_eq_vghminuh():
+    m: MagicMock = mock_open(read_data="".join(MockVghminUH))
     with patch("builtins.open", m):
-        n1 = QincrUH.le_arquivo("")
-        n2 = QincrUH.le_arquivo("")
+        n1 = VghminUH.read(ARQ_TESTE)
+        n2 = VghminUH.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_rhslppdf.py` & `inewave-0.0.96/tests/nwlistop/test_fteolsin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from inewave.nwlistop.rhslppdf import RHSLPPdf
+from inewave.nwlistop.fteolsin import FteolSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.rhslppdf import MockRHSLPPdf
+from tests.mocks.arquivos.fteolsin import MockFteolSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_rhslppdf():
-    m: MagicMock = mock_open(read_data="".join(MockRHSLPPdf))
+
+def test_atributos_encontrados_fteolsin():
+    m: MagicMock = mock_open(read_data="".join(MockFteolSIN))
     with patch("builtins.open", m):
-        n = RHSLPPdf.le_arquivo("")
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        n = FteolSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_rhslppdf():
+def test_atributos_nao_encontrados_fteolsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = RHSLPPdf.le_arquivo("")
-        assert n.ree is None
+        n = FteolSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_rhslppdf():
-    m: MagicMock = mock_open(read_data="".join(MockRHSLPPdf))
+def test_eq_fteolsin():
+    m: MagicMock = mock_open(read_data="".join(MockFteolSIN))
     with patch("builtins.open", m):
-        n1 = RHSLPPdf.le_arquivo("")
-        n2 = RHSLPPdf.le_arquivo("")
+        n1 = FteolSIN.read(ARQ_TESTE)
+        n2 = FteolSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_rhslpptb.py` & `inewave-0.0.96/tests/nwlistop/test_dvazmax.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.rhslpptb import RHSLPPtb
+from inewave.nwlistop.dvazmax import Dvazmax
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.rhslpptb import MockRHSLPPtb
+from tests.mocks.arquivos.dvazmax import MockDvazmax
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_rhslpptb():
-    m: MagicMock = mock_open(read_data="".join(MockRHSLPPtb))
+
+def test_atributos_encontrados_dvazmax():
+    m: MagicMock = mock_open(read_data="".join(MockDvazmax))
     with patch("builtins.open", m):
-        n = RHSLPPtb.le_arquivo("")
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        n = Dvazmax.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == 2022
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_rhslpptb():
+def test_atributos_nao_encontrados_dvazmax():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = RHSLPPtb.le_arquivo("")
-        assert n.ree is None
+        n = Dvazmax.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_rhslpptb():
-    m: MagicMock = mock_open(read_data="".join(MockRHSLPPtb))
+def test_eq_dvazmax():
+    m: MagicMock = mock_open(read_data="".join(MockDvazmax))
     with patch("builtins.open", m):
-        n1 = RHSLPPtb.le_arquivo("")
-        n2 = RHSLPPtb.le_arquivo("")
+        n1 = Dvazmax.read(ARQ_TESTE)
+        n2 = Dvazmax.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_vagua.py` & `inewave-0.0.96/tests/nwlistop/test_verturb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.vagua import Vagua
+from inewave.nwlistop.verturb import Verturb
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vagua import MockVagua
+from tests.mocks.arquivos.verturb import MockVerturb
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_vagua():
-    m: MagicMock = mock_open(read_data="".join(MockVagua))
+
+def test_atributos_encontrados_verturb():
+    m: MagicMock = mock_open(read_data="".join(MockVerturb))
     with patch("builtins.open", m):
-        n = Vagua.le_arquivo("")
+        n = Verturb.read(ARQ_TESTE)
+        assert n.valores is not None
+        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[-1, -1] == -2347.0
         assert n.ree is not None
         assert n.ree == "SUDESTE"
-        assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == -1.90
 
 
-def test_atributos_nao_encontrados_vagua():
+def test_atributos_nao_encontrados_verturb():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Vagua.le_arquivo("")
-        assert n.ree is None
+        n = Verturb.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.ree is None
 
 
-def test_eq_vagua():
-    m: MagicMock = mock_open(read_data="".join(MockVagua))
+def test_eq_verturb():
+    m: MagicMock = mock_open(read_data="".join(MockVerturb))
     with patch("builtins.open", m):
-        n1 = Vagua.le_arquivo("")
-        n2 = Vagua.le_arquivo("")
+        n1 = Verturb.read(ARQ_TESTE)
+        n2 = Verturb.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_varmpuh.py` & `inewave-0.0.96/tests/nwlistop/test_earmfp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.varmuh import VarmUH
+from inewave.nwlistop.earmfp import Earmfp
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.varmuh import MockVarmUH
+from tests.mocks.arquivos.earmfp import MockEarmfp
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_varmuh():
-    m: MagicMock = mock_open(read_data="".join(MockVarmUH))
+
+def test_atributos_encontrados_earmfp():
+    m: MagicMock = mock_open(read_data="".join(MockEarmfp))
     with patch("builtins.open", m):
-        n = VarmUH.le_arquivo("")
-        assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        n = Earmfp.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 662.80
+        assert n.valores.iloc[-1, -1] == 71.2
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_varmuh():
+def test_atributos_nao_encontrados_earmfp():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VarmUH.le_arquivo("")
-        assert n.usina is None
+        n = Earmfp.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.ree is None
 
 
-def test_eq_varmuh():
-    m: MagicMock = mock_open(read_data="".join(MockVarmUH))
+def test_eq_earmfp():
+    m: MagicMock = mock_open(read_data="".join(MockEarmfp))
     with patch("builtins.open", m):
-        n1 = VarmUH.le_arquivo("")
-        n2 = VarmUH.le_arquivo("")
+        n1 = Earmfp.read(ARQ_TESTE)
+        n2 = Earmfp.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_varmuh.py` & `inewave-0.0.96/tests/nwlistop/test_vghminm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.varmpuh import VarmpUH
+from inewave.nwlistop.vghminm import Vghminm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.varmpuh import MockVarmpUH
+from tests.mocks.arquivos.vghminm import MockVghminm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_varmpuh():
-    m: MagicMock = mock_open(read_data="".join(MockVarmpUH))
+
+def test_atributos_encontrados_vghminm():
+    m: MagicMock = mock_open(read_data="".join(MockVghminm))
     with patch("builtins.open", m):
-        n = VarmpUH.le_arquivo("")
-        assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        n = Vghminm.read(ARQ_TESTE)
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 95.35
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_varmpuh():
+def test_atributos_nao_encontrados_vghminm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VarmpUH.le_arquivo("")
-        assert n.usina is None
+        n = Vghminm.read(ARQ_TESTE)
+        assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_varmpuh():
-    m: MagicMock = mock_open(read_data="".join(MockVarmpUH))
+def test_eq_vghminm():
+    m: MagicMock = mock_open(read_data="".join(MockVghminm))
     with patch("builtins.open", m):
-        n1 = VarmpUH.le_arquivo("")
-        n2 = VarmpUH.le_arquivo("")
+        n1 = Vghminm.read(ARQ_TESTE)
+        n2 = Vghminm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_vertuh.py` & `inewave-0.0.96/tests/nwlistop/test_fteolm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.vertuh import VertUH
+from inewave.nwlistop.fteolm import Fteolm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vertuh import MockVertuh
+from tests.mocks.arquivos.fteolm import MockFteolm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_vertuh():
-    m: MagicMock = mock_open(read_data="".join(MockVertuh))
+
+def test_atributos_encontrados_fteolm():
+    m: MagicMock = mock_open(read_data="".join(MockFteolm))
     with patch("builtins.open", m):
-        n = VertUH.le_arquivo("")
-        assert n.usina is not None
-        assert n.usina == "ESPORA"
+        n = Fteolm.read(ARQ_TESTE)
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 30.74
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_vertuh():
+def test_atributos_nao_encontrados_fteolm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VertUH.le_arquivo("")
-        assert n.usina is None
+        n = Fteolm.read(ARQ_TESTE)
+        assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_vertuh():
-    m: MagicMock = mock_open(read_data="".join(MockVertuh))
+def test_eq_fteolm():
+    m: MagicMock = mock_open(read_data="".join(MockFteolm))
     with patch("builtins.open", m):
-        n1 = VertUH.le_arquivo("")
-        n2 = VertUH.le_arquivo("")
+        n1 = Fteolm.read(ARQ_TESTE)
+        n2 = Fteolm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_verturbsin.py` & `inewave-0.0.96/tests/nwlistop/test_vevmin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from inewave.nwlistop.verturbsin import VerturbSIN
+from inewave.nwlistop.vevmin import Vevmin
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.verturbsin import MockVerturbSIN
+from tests.mocks.arquivos.vevmin import MockVevmin
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_verturbsin():
-    m: MagicMock = mock_open(read_data="".join(MockVerturbSIN))
+
+def test_atributos_encontrados_vevmin():
+    m: MagicMock = mock_open(read_data="".join(MockVevmin))
     with patch("builtins.open", m):
-        n = VerturbSIN.le_arquivo("")
+        n = Vevmin.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == -29007.0
+        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_verturbsin():
+def test_atributos_nao_encontrados_vevmin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VerturbSIN.le_arquivo("")
+        n = Vevmin.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.ree is None
 
 
-def test_eq_verturbsin():
-    m: MagicMock = mock_open(read_data="".join(MockVerturbSIN))
+def test_eq_vevmin():
+    m: MagicMock = mock_open(read_data="".join(MockVevmin))
     with patch("builtins.open", m):
-        n1 = VerturbSIN.le_arquivo("")
-        n2 = VerturbSIN.le_arquivo("")
+        n1 = Vevmin.read(ARQ_TESTE)
+        n2 = Vevmin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_vevmin.py` & `inewave-0.0.96/tests/nwlistop/test_vghmin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.vevmin import Vevmin
+from inewave.nwlistop.vghmin import Vghmin
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vevmin import MockVevmin
+from tests.mocks.arquivos.vghmin import MockVghmin
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_vevmin():
-    m: MagicMock = mock_open(read_data="".join(MockVevmin))
+
+def test_atributos_encontrados_vghmin():
+    m: MagicMock = mock_open(read_data="".join(MockVghmin))
     with patch("builtins.open", m):
-        n = Vevmin.le_arquivo("")
+        n = Vghmin.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 0.0
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_vevmin():
+def test_atributos_nao_encontrados_vghmin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Vevmin.le_arquivo("")
-        assert n.valores is None
+        n = Vghmin.read(ARQ_TESTE)
         assert n.ree is None
+        assert n.valores is None
 
 
-def test_eq_vevmin():
-    m: MagicMock = mock_open(read_data="".join(MockVevmin))
+def test_eq_vghmin():
+    m: MagicMock = mock_open(read_data="".join(MockVghmin))
     with patch("builtins.open", m):
-        n1 = Vevmin.le_arquivo("")
-        n2 = Vevmin.le_arquivo("")
+        n1 = Vghmin.read(ARQ_TESTE)
+        n2 = Vghmin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_vevminm.py` & `inewave-0.0.96/tests/nwlistop/test_dlpptbmaxm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.vevminm import Vevminm
+from inewave.nwlistop.dlpptbmaxm import DLPPtbmaxm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vevminm import MockVevminm
+from tests.mocks.arquivos.dlpptbmaxm import MockDLPPtbmaxm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_vevminm():
-    m: MagicMock = mock_open(read_data="".join(MockVevminm))
+
+def test_atributos_encontrados_dlpptbmaxm():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxm))
     with patch("builtins.open", m):
-        n = Vevminm.le_arquivo("")
+        n = DLPPtbmaxm.read(ARQ_TESTE)
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 0.0
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_vevminm():
+def test_atributos_nao_encontrados_dlpptbmaxm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Vevminm.le_arquivo("")
-        assert n.valores is None
+        n = DLPPtbmaxm.read(ARQ_TESTE)
         assert n.submercado is None
+        assert n.valores is None
 
 
-def test_eq_vevminm():
-    m: MagicMock = mock_open(read_data="".join(MockVevminm))
+def test_eq_dlpptbmaxm():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxm))
     with patch("builtins.open", m):
-        n1 = Vevminm.le_arquivo("")
-        n2 = Vevminm.le_arquivo("")
+        n1 = DLPPtbmaxm.read(ARQ_TESTE)
+        n2 = DLPPtbmaxm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_vevminsin.py` & `inewave-0.0.96/tests/nwlistop/test_vghminsin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.vevminsin import VevminSIN
+from inewave.nwlistop.vghminsin import VghminSIN
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vevminsin import MockVevminSIN
+from tests.mocks.arquivos.vghminsin import MockVghminSIN
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_vevminsin():
-    m: MagicMock = mock_open(read_data="".join(MockVevminSIN))
+
+def test_atributos_encontrados_vghminsin():
+    m: MagicMock = mock_open(read_data="".join(MockVghminSIN))
     with patch("builtins.open", m):
-        n = VevminSIN.le_arquivo("")
+        n = VghminSIN.read(ARQ_TESTE)
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_vevminsin():
+def test_atributos_nao_encontrados_vghminsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VevminSIN.le_arquivo("")
+        n = VghminSIN.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_vevminsin():
-    m: MagicMock = mock_open(read_data="".join(MockVevminSIN))
+def test_eq_vghminsin():
+    m: MagicMock = mock_open(read_data="".join(MockVghminSIN))
     with patch("builtins.open", m):
-        n1 = VevminSIN.le_arquivo("")
-        n2 = VevminSIN.le_arquivo("")
+        n1 = VghminSIN.read(ARQ_TESTE)
+        n2 = VghminSIN.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_vghmin.py` & `inewave-0.0.96/tests/nwlistop/test_intercambio.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-from inewave.nwlistop.vghmin import Vghmin
+from inewave.nwlistop.intercambio import Intercambio
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vghmin import MockVghmin
+from tests.mocks.arquivos.intercambio import MockIntercambio
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_vghmin():
-    m: MagicMock = mock_open(read_data="".join(MockVghmin))
+
+def test_atributos_encontrados_intercambio():
+    m: MagicMock = mock_open(read_data="".join(MockIntercambio))
     with patch("builtins.open", m):
-        n = Vghmin.le_arquivo("")
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        n = Intercambio.read(ARQ_TESTE)
+        assert n.submercado_de is not None
+        assert n.submercado_de == "SUDESTE"
+        assert n.submercado_para == "SUL"
         assert n.valores is not None
         assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[-1, -2] == 2835.2
 
 
-def test_atributos_nao_encontrados_vghmin():
+def test_atributos_nao_encontrados_intercambio():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Vghmin.le_arquivo("")
-        assert n.ree is None
+        n = Intercambio.read(ARQ_TESTE)
+        assert n.submercado_de is None
+        assert n.submercado_para is None
         assert n.valores is None
 
 
-def test_eq_vghmin():
-    m: MagicMock = mock_open(read_data="".join(MockVghmin))
+def test_eq_intercambio():
+    m: MagicMock = mock_open(read_data="".join(MockIntercambio))
     with patch("builtins.open", m):
-        n1 = Vghmin.le_arquivo("")
-        n2 = Vghmin.le_arquivo("")
+        n1 = Intercambio.read(ARQ_TESTE)
+        n2 = Intercambio.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.95/tests/nwlistop/test_vturuh.py` & `inewave-0.0.96/tests/nwlistop/test_corteolm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from inewave.nwlistop.vturuh import VturUH
+from inewave.nwlistop.corteolm import Corteolm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vturuh import MockVturUH
+from tests.mocks.arquivos.corteolm import MockCorteolm
 
+ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
-def test_atributos_encontrados_vturuh():
-    m: MagicMock = mock_open(read_data="".join(MockVturUH))
+
+def test_atributos_encontrados_corteolm():
+    m: MagicMock = mock_open(read_data="".join(MockCorteolm))
     with patch("builtins.open", m):
-        n = VturUH.le_arquivo("")
-        assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        n = Corteolm.read(ARQ_TESTE)
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 98.77
+        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_vturuh():
+def test_atributos_nao_encontrados_corteolm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VturUH.le_arquivo("")
-        assert n.usina is None
+        n = Corteolm.read(ARQ_TESTE)
+        assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_vturuh():
-    m: MagicMock = mock_open(read_data="".join(MockVturUH))
+def test_eq_corteolm():
+    m: MagicMock = mock_open(read_data="".join(MockCorteolm))
     with patch("builtins.open", m):
-        n1 = VturUH.le_arquivo("")
-        n2 = VturUH.le_arquivo("")
+        n1 = Corteolm.read(ARQ_TESTE)
+        n2 = Corteolm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

