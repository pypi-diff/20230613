# Comparing `tmp/reasonable-0.2.2a4.tar.gz` & `tmp/reasonable-0.2.3a1.tar.gz`

## Comparing `reasonable-0.2.2a4.tar` & `reasonable-0.2.3a1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 reasonable-0.2.2a4/Cargo.toml
--rw-r--r--   0      501       20      111 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.cargo/config
--rw-r--r--   0      501       20     7144 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.github/workflows/Python.yml
--rw-r--r--   0      501       20     2263 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.github/workflows/builds.yml
--rw-r--r--   0      501       20      542 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.github/workflows/manylinux_build.sh
--rw-r--r--   0      501       20     1127 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.github/workflows/nightly-builds.yml
--rw-r--r--   0      501       20      568 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/.gitignore
--rw-r--r--   0      501       20    17449 2022-11-26 19:12:43.000000 reasonable-0.2.2a4/Cargo.lock
--rw-r--r--   0      501       20     1519 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/LICENSE
--rw-r--r--   0      501       20     1608 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/Makefile
--rw-r--r--   0      501       20     5360 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/README.md
--rw-r--r--   0      501       20     4490 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/my_benchmark.rs
--rw-r--r--   0      501       20     3755 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/bench.py
--rw-r--r--   0      501       20   438888 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ACAD(v1.1).ttl
--rw-r--r--   0      501       20    15738 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/AMRL(v1.1).ttl
--rw-r--r--   0      501       20     4663 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/AOB4(v1.1).ttl
--rw-r--r--   0      501       20     2456 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/AQUA(v1.1).ttl
--rw-r--r--   0      501       20   148837 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ARC(v1.1).ttl
--rw-r--r--   0      501       20     8626 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ART(v1.1).ttl
--rw-r--r--   0      501       20    32114 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ARTX(v1.1).ttl
--rw-r--r--   0      501       20    32336 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ASMUN(v1.1).ttl
--rw-r--r--   0      501       20     5821 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/BIXB(v1.1).ttl
--rw-r--r--   0      501       20   680383 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/BRIG(v1.1).ttl
--rw-r--r--   0      501       20    52446 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/BWFP(v1.1).ttl
--rw-r--r--   0      501       20   103849 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/Bainer(v1.1).ttl
--rw-r--r--   0      501       20     2740 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/C113(v1.1).ttl
--rw-r--r--   0      501       20   234090 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/CHEM(v1.1).ttl
--rw-r--r--   0      501       20   201232 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/CHEMX(v1.1).ttl
--rw-r--r--   0      501       20    26964 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/CONT(v1.1).ttl
--rw-r--r--   0      501       20    23617 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/COWL(v1.1).ttl
--rw-r--r--   0      501       20    56380 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/CRUS(v1.1).ttl
--rw-r--r--   0      501       20     2785 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/CURR(v1.1).ttl
--rw-r--r--   0      501       20   197473 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/DH(v1.1).ttl
--rw-r--r--   0      501       20   435076 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/EPS(v1.1).ttl
--rw-r--r--   0      501       20    27951 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/FDPD(v1.1).ttl
--rw-r--r--   0      501       20   530501 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/GBSF(v1.1).ttl
--rw-r--r--   0      501       20   210071 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/GHA_ICS(v1.1).ttl
--rw-r--r--   0      501       20    48299 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/GIEDT(v1.1).ttl
--rw-r--r--   0      501       20     5808 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/GILM(v1.1).ttl
--rw-r--r--   0      501       20   304349 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/HART(v1.1).ttl
--rw-r--r--   0      501       20     8128 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/HICK(v1.1).ttl
--rw-r--r--   0      501       20     5628 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/HUNT(v1.1).ttl
--rw-r--r--   0      501       20   303396 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/HUTCH(v1.1).ttl
--rw-r--r--   0      501       20   194712 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/HWC(v1.1).ttl
--rw-r--r--   0      501       20    57424 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/JUNGER(v1.1).ttl
--rw-r--r--   0      501       20     6215 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/KERR(v1.1).ttl
--rw-r--r--   0      501       20     6999 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/KING(v1.1).ttl
--rw-r--r--   0      501       20     6609 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/KLEIBER(v1.1).ttl
--rw-r--r--   0      501       20    18419 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/LFH(v1.1).ttl
--rw-r--r--   0      501       20    19160 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/LSA(v1.1).ttl
--rw-r--r--   0      501       20    84768 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MADDY(v1.1).ttl
--rw-r--r--   0      501       20    28687 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MANN(v1.1).ttl
--rw-r--r--   0      501       20    15662 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MATH(v1.1).ttl
--rw-r--r--   0      501       20   131812 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MEYR(v1.1).ttl
--rw-r--r--   0      501       20    23894 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MIWF(v1.1).ttl
--rw-r--r--   0      501       20   164159 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MRAK(v1.1).ttl
--rw-r--r--   0      501       20    18750 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MSB(v1.1).ttl
--rw-r--r--   0      501       20    11894 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MSC(v1.1).ttl
--rw-r--r--   0      501       20     3115 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MSD(v1.1).ttl
--rw-r--r--   0      501       20    42466 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MU(v1.1).ttl
--rw-r--r--   0      501       20     8421 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/MUSIC(v1.1).ttl
--rw-r--r--   0      501       20    14105 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/OLS(v1.1).ttl
--rw-r--r--   0      501       20   476097 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/PES_ICS(v1.1).ttl
--rw-r--r--   0      501       20     7860 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/PHSL(v1.1).ttl
--rw-r--r--   0      501       20     2785 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/PINE(v1.1).ttl
--rw-r--r--   0      501       20    86053 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/PRB(v1.1).ttl
--rw-r--r--   0      501       20    20839 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/RECH(v1.1).ttl
--rw-r--r--   0      501       20    42143 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ROES(v1.1).ttl
--rw-r--r--   0      501       20     2454 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/RPL(v1.1).ttl
--rw-r--r--   0      501       20     5498 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/RYER(v1.1).ttl
--rw-r--r--   0      501       20    47682 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SCC(v1.1).ttl
--rw-r--r--   0      501       20     6683 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SCHM(v1.1).ttl
--rw-r--r--   0      501       20     2785 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SEQU(v1.1).ttl
--rw-r--r--   0      501       20   271074 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SHIELDS(v1.1).ttl
--rw-r--r--   0      501       20   166666 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SLAB(v1.1).ttl
--rw-r--r--   0      501       20     6312 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SLEC(v1.1).ttl
--rw-r--r--   0      501       20    63381 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SMOA(v1.1).ttl
--rw-r--r--   0      501       20   489384 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SOCS(v1.1).ttl
--rw-r--r--   0      501       20     4380 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SPRL(v1.1).ttl
--rw-r--r--   0      501       20   222603 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/STOR(v1.1).ttl
--rw-r--r--   0      501       20    32752 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SURGE3(v1.1).ttl
--rw-r--r--   0      501       20     3657 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/SWL(v1.1).ttl
--rw-r--r--   0      501       20    73442 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/TAPS(v1.1).ttl
--rw-r--r--   0      501       20     2457 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/THOR(v1.1).ttl
--rw-r--r--   0      501       20    91770 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/THUR(v1.1).ttl
--rw-r--r--   0      501       20    26122 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/TUPP(v1.1).ttl
--rw-r--r--   0      501       20    34129 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VEIH(v1.1).ttl
--rw-r--r--   0      501       20   137513 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VM2(v1.1).ttl
--rw-r--r--   0      501       20  1100244 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VM3A(v1.1).ttl
--rw-r--r--   0      501       20     6920 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VM3B(v1.1).ttl
--rw-r--r--   0      501       20    37918 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMEP(v1.1).ttl
--rw-r--r--   0      501       20   130411 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMIF(v1.1).ttl
--rw-r--r--   0      501       20    13294 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMLF(v1.1).ttl
--rw-r--r--   0      501       20    55576 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMTH(v1.1).ttl
--rw-r--r--   0      501       20     4286 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMTHB(v1.1).ttl
--rw-r--r--   0      501       20     4286 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/VMTHC(v1.1).ttl
--rw-r--r--   0      501       20    91018 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/WELL(v1.1).ttl
--rw-r--r--   0      501       20    27797 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/WICK(v1.1).ttl
--rw-r--r--   0      501       20    73670 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/WSRC(v1.1).ttl
--rw-r--r--   0      501       20    23245 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/YOUNG(v1.1).ttl
--rw-r--r--   0      501       20    13281 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/avenal-animal-shelter(v1.1).ttl
--rw-r--r--   0      501       20    39438 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/avenal-movie-theatre(v1.1).ttl
--rw-r--r--   0      501       20    10692 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/avenal-public-works-yard(v1.1).ttl
--rw-r--r--   0      501       20    14596 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/avenal-recreation-center(v1.1).ttl
--rw-r--r--   0      501       20    27336 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/avenal-veterans-hall(v1.1).ttl
--rw-r--r--   0      501       20    29969 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl
--rw-r--r--   0      501       20    82637 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ciee(v1.1).ttl
--rw-r--r--   0      501       20    81292 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl
--rw-r--r--   0      501       20   474074 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/csu-dominguez-hills(v1.1).ttl
--rw-r--r--   0      501       20    13557 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/garber(v1.1).ttl
--rw-r--r--   0      501       20    24179 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/hayward-station-1(v1.1).ttl
--rw-r--r--   0      501       20    18716 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/hayward-station-8(v1.1).ttl
--rw-r--r--   0      501       20    76388 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/jesse-turner-center(v1.1).ttl
--rw-r--r--   0      501       20    10088 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/local-butcher-shop(v1.1).ttl
--rw-r--r--   0      501       20    21969 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl
--rw-r--r--   0      501       20    58913 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/orinda-community-center(v1.1).ttl
--rw-r--r--   0      501       20    98730 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/orinda-public-library(v1.1).ttl
--rw-r--r--   0      501       20    18839 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/rfs(v1.1).ttl
--rw-r--r--   0      501       20   424960 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/sdh(v1.1).ttl
--rw-r--r--   0      501       20    31717 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl
--rw-r--r--   0      501       20    32735 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/buildings/word-of-faith-cc(v1.1).ttl
--rw-r--r--   0      501       20       41 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/benches/python/requirements.txt
--rw-r--r--   0      501       20  2189973 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/example_models/ontologies/Brick.n3
--rw-r--r--   0      501       20    64515 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/example_models/ontologies/owl.n3
--rw-r--r--   0      501       20     3812 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/example_models/ontologies/rdfs.ttl
--rw-r--r--   0      501       20     2263 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/example_models/small1.n3
--rw-r--r--   0      501       20   707359 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/example_models/soda_hall.n3
--rw-r--r--   0      501       20    43207 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/img/benchmark.png
--rw-r--r--   0      501       20    21469 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/poetry.lock
--rw-r--r--   0      501       20      599 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/pyproject.toml
--rw-r--r--   0      501       20       84 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/reasonable/__init__.py
--rwxr-xr-x   0      501       20     1117 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/scripts/bench_examples.sh
--rwxr-xr-x   0      501       20      318 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/scripts/convert_to_n3.py
--rwxr-xr-x   0      501       20      323 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/scripts/reason_owlrl.py
--rw-r--r--   0      501       20     5741 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/common.rs
--rw-r--r--   0      501       20     4181 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/disjoint_sets.rs
--rw-r--r--   0      501       20     2102 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/error.rs
--rw-r--r--   0      501       20     1034 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/index.rs
--rw-r--r--   0      501       20      795 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/lib.rs
--rw-r--r--   0      501       20      584 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/main.rs
--rw-r--r--   0      501       20     6240 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/pyreason.rs
--rw-r--r--   0      501       20    11950 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/query.rs
--rw-r--r--   0      501       20    61875 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/reasoner.rs
--rw-r--r--   0      501       20    26068 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/src/tests.rs
--rw-r--r--   0      501       20      350 2022-11-26 19:11:08.000000 reasonable-0.2.2a4/test.py
--rw-r--r--   0        0        0     5733 1970-01-01 00:00:00.000000 reasonable-0.2.2a4/PKG-INFO
+-rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 reasonable-0.2.3a1/Cargo.toml
+-rw-r--r--   0      501       20      111 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/.cargo/config
+-rw-r--r--   0      501       20     7144 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/.github/workflows/Python.yml
+-rw-r--r--   0      501       20     2255 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/.github/workflows/builds.yml
+-rw-r--r--   0      501       20      542 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/.github/workflows/manylinux_build.sh
+-rw-r--r--   0      501       20     1127 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/.github/workflows/nightly-builds.yml
+-rw-r--r--   0      501       20      568 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/.gitignore
+-rw-r--r--   0      501       20    16794 2023-06-13 03:25:42.000000 reasonable-0.2.3a1/Cargo.lock
+-rw-r--r--   0      501       20     1519 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/LICENSE
+-rw-r--r--   0      501       20     1608 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/Makefile
+-rw-r--r--   0      501       20     5360 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/README.md
+-rw-r--r--   0      501       20     4490 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/my_benchmark.rs
+-rw-r--r--   0      501       20     3755 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/bench.py
+-rw-r--r--   0      501       20   438888 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/ACAD(v1.1).ttl
+-rw-r--r--   0      501       20    15738 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/AMRL(v1.1).ttl
+-rw-r--r--   0      501       20     4663 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/AOB4(v1.1).ttl
+-rw-r--r--   0      501       20     2456 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/AQUA(v1.1).ttl
+-rw-r--r--   0      501       20   148837 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/ARC(v1.1).ttl
+-rw-r--r--   0      501       20     8626 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/ART(v1.1).ttl
+-rw-r--r--   0      501       20    32114 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/ARTX(v1.1).ttl
+-rw-r--r--   0      501       20    32336 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/ASMUN(v1.1).ttl
+-rw-r--r--   0      501       20     5821 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/BIXB(v1.1).ttl
+-rw-r--r--   0      501       20   680383 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/BRIG(v1.1).ttl
+-rw-r--r--   0      501       20    52446 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/BWFP(v1.1).ttl
+-rw-r--r--   0      501       20   103849 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/Bainer(v1.1).ttl
+-rw-r--r--   0      501       20     2740 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/C113(v1.1).ttl
+-rw-r--r--   0      501       20   234090 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/CHEM(v1.1).ttl
+-rw-r--r--   0      501       20   201232 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/CHEMX(v1.1).ttl
+-rw-r--r--   0      501       20    26964 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/CONT(v1.1).ttl
+-rw-r--r--   0      501       20    23617 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/COWL(v1.1).ttl
+-rw-r--r--   0      501       20    56380 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/CRUS(v1.1).ttl
+-rw-r--r--   0      501       20     2785 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/CURR(v1.1).ttl
+-rw-r--r--   0      501       20   197473 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/DH(v1.1).ttl
+-rw-r--r--   0      501       20   435076 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/EPS(v1.1).ttl
+-rw-r--r--   0      501       20    27951 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/FDPD(v1.1).ttl
+-rw-r--r--   0      501       20   530501 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/GBSF(v1.1).ttl
+-rw-r--r--   0      501       20   210071 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/GHA_ICS(v1.1).ttl
+-rw-r--r--   0      501       20    48299 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/GIEDT(v1.1).ttl
+-rw-r--r--   0      501       20     5808 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/GILM(v1.1).ttl
+-rw-r--r--   0      501       20   304349 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/HART(v1.1).ttl
+-rw-r--r--   0      501       20     8128 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/HICK(v1.1).ttl
+-rw-r--r--   0      501       20     5628 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/HUNT(v1.1).ttl
+-rw-r--r--   0      501       20   303396 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/HUTCH(v1.1).ttl
+-rw-r--r--   0      501       20   194712 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/HWC(v1.1).ttl
+-rw-r--r--   0      501       20    57424 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/JUNGER(v1.1).ttl
+-rw-r--r--   0      501       20     6215 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/KERR(v1.1).ttl
+-rw-r--r--   0      501       20     6999 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/KING(v1.1).ttl
+-rw-r--r--   0      501       20     6609 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/KLEIBER(v1.1).ttl
+-rw-r--r--   0      501       20    18419 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/LFH(v1.1).ttl
+-rw-r--r--   0      501       20    19160 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/LSA(v1.1).ttl
+-rw-r--r--   0      501       20    84768 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MADDY(v1.1).ttl
+-rw-r--r--   0      501       20    28687 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MANN(v1.1).ttl
+-rw-r--r--   0      501       20    15662 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MATH(v1.1).ttl
+-rw-r--r--   0      501       20   131812 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MEYR(v1.1).ttl
+-rw-r--r--   0      501       20    23894 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MIWF(v1.1).ttl
+-rw-r--r--   0      501       20   164159 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MRAK(v1.1).ttl
+-rw-r--r--   0      501       20    18750 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MSB(v1.1).ttl
+-rw-r--r--   0      501       20    11894 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MSC(v1.1).ttl
+-rw-r--r--   0      501       20     3115 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MSD(v1.1).ttl
+-rw-r--r--   0      501       20    42466 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MU(v1.1).ttl
+-rw-r--r--   0      501       20     8421 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/MUSIC(v1.1).ttl
+-rw-r--r--   0      501       20    14105 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/OLS(v1.1).ttl
+-rw-r--r--   0      501       20   476097 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/PES_ICS(v1.1).ttl
+-rw-r--r--   0      501       20     7860 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/PHSL(v1.1).ttl
+-rw-r--r--   0      501       20     2785 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/PINE(v1.1).ttl
+-rw-r--r--   0      501       20    86053 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/PRB(v1.1).ttl
+-rw-r--r--   0      501       20    20839 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/RECH(v1.1).ttl
+-rw-r--r--   0      501       20    42143 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/ROES(v1.1).ttl
+-rw-r--r--   0      501       20     2454 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/RPL(v1.1).ttl
+-rw-r--r--   0      501       20     5498 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/RYER(v1.1).ttl
+-rw-r--r--   0      501       20    47682 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SCC(v1.1).ttl
+-rw-r--r--   0      501       20     6683 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SCHM(v1.1).ttl
+-rw-r--r--   0      501       20     2785 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SEQU(v1.1).ttl
+-rw-r--r--   0      501       20   271074 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SHIELDS(v1.1).ttl
+-rw-r--r--   0      501       20   166666 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SLAB(v1.1).ttl
+-rw-r--r--   0      501       20     6312 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SLEC(v1.1).ttl
+-rw-r--r--   0      501       20    63381 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SMOA(v1.1).ttl
+-rw-r--r--   0      501       20   489384 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SOCS(v1.1).ttl
+-rw-r--r--   0      501       20     4380 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SPRL(v1.1).ttl
+-rw-r--r--   0      501       20   222603 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/STOR(v1.1).ttl
+-rw-r--r--   0      501       20    32752 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SURGE3(v1.1).ttl
+-rw-r--r--   0      501       20     3657 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/SWL(v1.1).ttl
+-rw-r--r--   0      501       20    73442 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/TAPS(v1.1).ttl
+-rw-r--r--   0      501       20     2457 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/THOR(v1.1).ttl
+-rw-r--r--   0      501       20    91770 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/THUR(v1.1).ttl
+-rw-r--r--   0      501       20    26122 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/TUPP(v1.1).ttl
+-rw-r--r--   0      501       20    34129 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/VEIH(v1.1).ttl
+-rw-r--r--   0      501       20   137513 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/VM2(v1.1).ttl
+-rw-r--r--   0      501       20  1100244 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/VM3A(v1.1).ttl
+-rw-r--r--   0      501       20     6920 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/VM3B(v1.1).ttl
+-rw-r--r--   0      501       20    37918 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/VMEP(v1.1).ttl
+-rw-r--r--   0      501       20   130411 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/VMIF(v1.1).ttl
+-rw-r--r--   0      501       20    13294 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/VMLF(v1.1).ttl
+-rw-r--r--   0      501       20    55576 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/VMTH(v1.1).ttl
+-rw-r--r--   0      501       20     4286 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/VMTHB(v1.1).ttl
+-rw-r--r--   0      501       20     4286 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/VMTHC(v1.1).ttl
+-rw-r--r--   0      501       20    91018 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/WELL(v1.1).ttl
+-rw-r--r--   0      501       20    27797 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/WICK(v1.1).ttl
+-rw-r--r--   0      501       20    73670 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/WSRC(v1.1).ttl
+-rw-r--r--   0      501       20    23245 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/YOUNG(v1.1).ttl
+-rw-r--r--   0      501       20    13281 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/avenal-animal-shelter(v1.1).ttl
+-rw-r--r--   0      501       20    39438 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/avenal-movie-theatre(v1.1).ttl
+-rw-r--r--   0      501       20    10692 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/avenal-public-works-yard(v1.1).ttl
+-rw-r--r--   0      501       20    14596 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/avenal-recreation-center(v1.1).ttl
+-rw-r--r--   0      501       20    27336 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/avenal-veterans-hall(v1.1).ttl
+-rw-r--r--   0      501       20    29969 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl
+-rw-r--r--   0      501       20    82637 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/ciee(v1.1).ttl
+-rw-r--r--   0      501       20    81292 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl
+-rw-r--r--   0      501       20   474074 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/csu-dominguez-hills(v1.1).ttl
+-rw-r--r--   0      501       20    13557 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/garber(v1.1).ttl
+-rw-r--r--   0      501       20    24179 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/hayward-station-1(v1.1).ttl
+-rw-r--r--   0      501       20    18716 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/hayward-station-8(v1.1).ttl
+-rw-r--r--   0      501       20    76388 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/jesse-turner-center(v1.1).ttl
+-rw-r--r--   0      501       20    10088 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/local-butcher-shop(v1.1).ttl
+-rw-r--r--   0      501       20    21969 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl
+-rw-r--r--   0      501       20    58913 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/orinda-community-center(v1.1).ttl
+-rw-r--r--   0      501       20    98730 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/orinda-public-library(v1.1).ttl
+-rw-r--r--   0      501       20    18839 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/rfs(v1.1).ttl
+-rw-r--r--   0      501       20   424960 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/sdh(v1.1).ttl
+-rw-r--r--   0      501       20    31717 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl
+-rw-r--r--   0      501       20    32735 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/buildings/word-of-faith-cc(v1.1).ttl
+-rw-r--r--   0      501       20       41 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/benches/python/requirements.txt
+-rw-r--r--   0      501       20  2189973 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/example_models/ontologies/Brick.n3
+-rw-r--r--   0      501       20    64515 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/example_models/ontologies/owl.n3
+-rw-r--r--   0      501       20     3812 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/example_models/ontologies/rdfs.ttl
+-rw-r--r--   0      501       20     2263 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/example_models/small1.n3
+-rw-r--r--   0      501       20   707359 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/example_models/soda_hall.n3
+-rw-r--r--   0      501       20    43207 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/img/benchmark.png
+-rw-r--r--   0      501       20    21479 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/poetry.lock
+-rw-r--r--   0      501       20      599 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/pyproject.toml
+-rw-r--r--   0      501       20       84 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/reasonable/__init__.py
+-rwxr-xr-x   0      501       20     1117 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/scripts/bench_examples.sh
+-rwxr-xr-x   0      501       20      318 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/scripts/convert_to_n3.py
+-rwxr-xr-x   0      501       20      323 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/scripts/reason_owlrl.py
+-rw-r--r--   0      501       20     5741 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/src/common.rs
+-rw-r--r--   0      501       20     4181 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/src/disjoint_sets.rs
+-rw-r--r--   0      501       20     2102 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/src/error.rs
+-rw-r--r--   0      501       20     1034 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/src/index.rs
+-rw-r--r--   0      501       20      795 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/src/lib.rs
+-rw-r--r--   0      501       20      584 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/src/main.rs
+-rw-r--r--   0      501       20     6240 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/src/pyreason.rs
+-rw-r--r--   0      501       20    11950 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/src/query.rs
+-rw-r--r--   0      501       20    61875 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/src/reasoner.rs
+-rw-r--r--   0      501       20    26591 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/src/tests.rs
+-rw-r--r--   0      501       20      350 2023-06-13 03:25:23.000000 reasonable-0.2.3a1/test.py
+-rw-r--r--   0        0        0     5733 1970-01-01 00:00:00.000000 reasonable-0.2.3a1/PKG-INFO
```

### Comparing `reasonable-0.2.2a4/Cargo.toml` & `reasonable-0.2.3a1/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "reasonable"
-version = "0.2.2-a4"
+version = "0.2.3-a1"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 repository = "https://github.com/gtfierro/reasonable"
 homepage = "https://brickschema.org/"
 license-file = "LICENSE"
 readme = "README.md"
 description = "An OWL 2 RL reasoner with reasonable performance"
 edition = "2018"
```

### Comparing `reasonable-0.2.2a4/.github/workflows/Python.yml` & `reasonable-0.2.3a1/.github/workflows/Python.yml`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/.github/workflows/builds.yml` & `reasonable-0.2.3a1/.github/workflows/builds.yml`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         rust:
           # - stable
           - nightly
         os: [ubuntu-latest, macos-latest]
-        python-version: [3.6.12, 3.7.9, 3.8.5, 3.9.0]
+        python-version: ["3.9","3.10","3.11"]
     steps:
       - uses: actions/checkout@v2
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: ${{ matrix.rust }}
           override: true
```

### Comparing `reasonable-0.2.2a4/.github/workflows/manylinux_build.sh` & `reasonable-0.2.3a1/.github/workflows/manylinux_build.sh`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/.github/workflows/nightly-builds.yml` & `reasonable-0.2.3a1/.github/workflows/nightly-builds.yml`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/.gitignore` & `reasonable-0.2.3a1/.gitignore`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/Cargo.lock` & `reasonable-0.2.3a1/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "ahash"
-version = "0.7.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
-dependencies = [
- "getrandom",
- "once_cell",
- "version_check",
-]
-
-[[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.66"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "216261ddc8289130e551ddcd5ce8a064710c0d064a4d2895c67151c92b5443f6"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
@@ -73,17 +62,17 @@
 name = "disjoint-sets"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ccbbca7d6a247007ca2535c616d4bb4a5fcad176ef0218671f96b88c52c3d34"
 
 [[package]]
 name = "either"
-version = "1.8.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "env_logger"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44533bbbb3bb3c1fa17d9f2e4e38bbbaf8396ba82193c4cb1b6445d711445d36"
 dependencies = [
@@ -98,33 +87,24 @@
 name = "farmhash"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f35ce9c8fb9891c75ceadbc330752951a4e369b50af10775955aeb9af3eee34b"
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
-name = "hashbrown"
-version = "0.11.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab5ef0d4909ef3724cc8cce6ccc8572c5c817592e9285f5464f8e86f8bd3726e"
-dependencies = [
- "ahash",
-]
-
-[[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
@@ -136,66 +116,54 @@
 checksum = "df004cfca50ef23c36850aaaa59ad52cc70d0e90243c3c7737a4dd32dc7a3c4f"
 dependencies = [
  "quick-error",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.7"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itertools"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f56a2d0bc861f9165be4eb3442afd3c236d8a98afd426f65d92324ae1091a484"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.4"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4217ad341ebadf8d8e724e264f13e593e0648f5b3e94b3896a5df283be015ecc"
-
-[[package]]
-name = "lasso"
-version = "0.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aeb7b21a526375c5ca55f1a6dfd4e1fad9fa4edd750f530252a718a44b2608f0"
-dependencies = [
- "hashbrown",
-]
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "libc"
-version = "0.2.137"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc7fcc620a3bff7cdd7a365be3376c97191aeaccc2a603e600951e452615bf89"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
@@ -206,17 +174,17 @@
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.16.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oxilangtag"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d91edf4fbb970279443471345a4e8c491bf05bb283b3e6c88e4e606fd8c181b"
 
@@ -224,19 +192,18 @@
 name = "oxiri"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb175ec8981211357b7b379869c2f8d555881c55ea62311428ec0de46d89bd5c"
 
 [[package]]
 name = "oxrdf"
-version = "0.1.0"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4593f3eb15863b265238459105a00062be6176906de20b62950a6c57e563c526"
+checksum = "6463bbf464af8b7e3951191b22bcbbadbacb3f58d0bf3f8d15ad44ac41acd018"
 dependencies = [
- "lasso",
  "oxilangtag",
  "oxiri",
  "rand",
 ]
 
 [[package]]
 name = "parking_lot"
@@ -246,36 +213,36 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.4"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dc9e0dc2adc1c69d09143aff38d3d30c5c3f0df0dad82e6d25547af174ebec0"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.47"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ea3d908b0e36316caf9e9e2c4625cdde190a7e6f440d794667ed17a1855e725"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
@@ -318,39 +285,39 @@
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -385,15 +352,15 @@
 name = "rdf"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb1725bf0133fe4a3279e18efd6d69f952cb8356bf8b835023042e1b98d4c646"
 
 [[package]]
 name = "reasonable"
-version = "0.2.2-a4"
+version = "0.2.3-a1"
 dependencies = [
  "anyhow",
  "datafrog",
  "disjoint-sets",
  "env_logger",
  "farmhash",
  "itertools",
@@ -409,37 +376,37 @@
  "serde_derive",
  "serde_json",
  "tinytemplate",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.0"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e076559ef8e241f2ae3479e36f97bd5741c0330689e217ad51ce2c76808b868a"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "rio_api"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f6196ea9fb6791ce3dcd1cfc0d7f1074972aec0572db73dfb7396fcd9c3bc76"
 
@@ -461,80 +428,91 @@
 checksum = "4af20e5d3e44732a57489fa297768ca29361b54fbc3b20cdeb738fa6932cc22d"
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.11"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4501abdff3ae82a1c1b477a17252eb69cee9e66eb915c1abaa4f44d873df9f09"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.147"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d193d69bae983fc11a79df82342761dfbf28a99fc8d203dca4c3c1b590948965"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 
 [[package]]
 name = "serde_derive"
-version = "1.0.147"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f1d362ca8fc9c3e3a7484440752472d68a6caa98f1ab81d99b5dfe517cec852"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.89"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "020ff22c755c2ed3f8cf162dbb41a7268d934702f3ed3631656ea597e08fc3db"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "syn"
-version = "1.0.103"
+version = "1.0.109"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a864042229133ada95abf3b54fdc62ef5ccabe9515b64717bcb9a1919e59445d"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "termcolor"
-version = "1.1.3"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
+checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
@@ -543,29 +521,23 @@
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.5"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ceab39d59e4c9499d4e5a8ee0e2735b891bb7308ac83dfb4e80cad195c9f6f3"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
-
-[[package]]
-name = "version_check"
-version = "0.9.4"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
@@ -597,62 +569,62 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows-targets"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `reasonable-0.2.2a4/LICENSE` & `reasonable-0.2.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/Makefile` & `reasonable-0.2.3a1/Makefile`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/README.md` & `reasonable-0.2.3a1/README.md`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/my_benchmark.rs` & `reasonable-0.2.3a1/benches/my_benchmark.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/bench.py` & `reasonable-0.2.3a1/benches/python/bench.py`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/ACAD(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/ACAD(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/AMRL(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/AMRL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/AOB4(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/AOB4(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/AQUA(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/AQUA(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/ARC(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/ARC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/ART(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/ART(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/ARTX(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/ARTX(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/ASMUN(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/ASMUN(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/BIXB(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/BIXB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/BRIG(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/BRIG(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/BWFP(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/BWFP(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/Bainer(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/Bainer(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/C113(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/C113(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/CHEM(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/CHEM(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/CHEMX(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/CHEMX(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/CONT(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/CONT(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/COWL(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/COWL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/CRUS(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/CRUS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/CURR(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/CURR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/DH(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/DH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/EPS(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/EPS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/FDPD(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/FDPD(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/GBSF(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/GBSF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/GHA_ICS(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/GHA_ICS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/GIEDT(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/GIEDT(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/GILM(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/GILM(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/HART(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/HART(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/HICK(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/HICK(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/HUNT(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/HUNT(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/HUTCH(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/HUTCH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/HWC(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/HWC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/JUNGER(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/JUNGER(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/KERR(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/KERR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/KING(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/KING(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/KLEIBER(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/KLEIBER(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/LFH(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/LFH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/LSA(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/LSA(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MADDY(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MADDY(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MANN(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MANN(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MATH(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MATH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MEYR(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MEYR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MIWF(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MIWF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MRAK(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MRAK(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MSB(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MSB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MSC(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MSC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MSD(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MSD(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MU(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MU(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/MUSIC(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/MUSIC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/OLS(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/OLS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/PES_ICS(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/PES_ICS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/PHSL(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/PHSL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/PINE(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/PINE(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/PRB(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/PRB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/RECH(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/RECH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/ROES(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/ROES(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/RPL(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/RPL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/RYER(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/RYER(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SCC(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SCC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SCHM(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SCHM(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SEQU(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SEQU(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SHIELDS(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SHIELDS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SLAB(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SLAB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SLEC(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SLEC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SMOA(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SMOA(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SOCS(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SOCS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SPRL(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SPRL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/STOR(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/STOR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SURGE3(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SURGE3(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/SWL(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/SWL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/TAPS(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/TAPS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/THOR(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/THOR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/THUR(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/THUR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/TUPP(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/TUPP(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/VEIH(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/VEIH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/VM2(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/VM2(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/VM3A(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/VM3A(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/VM3B(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/VM3B(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/VMEP(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/VMEP(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/VMIF(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/VMIF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/VMLF(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/VMLF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/VMTH(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/VMTH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/VMTHB(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/VMTHB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/VMTHC(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/VMTHC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/WELL(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/WELL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/WICK(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/WICK(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/WSRC(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/WSRC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/YOUNG(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/YOUNG(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/avenal-animal-shelter(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/avenal-animal-shelter(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/avenal-movie-theatre(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/avenal-movie-theatre(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/avenal-public-works-yard(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/avenal-public-works-yard(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/avenal-recreation-center(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/avenal-recreation-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/avenal-veterans-hall(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/avenal-veterans-hall(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/ciee(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/ciee(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/csu-dominguez-hills(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/csu-dominguez-hills(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/garber(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/garber(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/hayward-station-1(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/hayward-station-1(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/hayward-station-8(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/hayward-station-8(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/jesse-turner-center(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/jesse-turner-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/local-butcher-shop(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/local-butcher-shop(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/orinda-community-center(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/orinda-community-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/orinda-public-library(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/orinda-public-library(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/rfs(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/rfs(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/sdh(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/sdh(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/benches/python/buildings/word-of-faith-cc(v1.1).ttl` & `reasonable-0.2.3a1/benches/python/buildings/word-of-faith-cc(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/example_models/ontologies/Brick.n3` & `reasonable-0.2.3a1/example_models/ontologies/Brick.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/example_models/ontologies/owl.n3` & `reasonable-0.2.3a1/example_models/ontologies/owl.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/example_models/ontologies/rdfs.ttl` & `reasonable-0.2.3a1/example_models/ontologies/rdfs.ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/example_models/small1.n3` & `reasonable-0.2.3a1/example_models/small1.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/example_models/soda_hall.n3` & `reasonable-0.2.3a1/example_models/soda_hall.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/img/benchmark.png` & `reasonable-0.2.3a1/img/benchmark.png`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/poetry.lock` & `reasonable-0.2.3a1/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -99,23 +99,23 @@
 docs = ["myst-parser", "sphinx (<6)", "sphinx-autodoc-typehints", "sphinxcontrib-apidoc", "sphinxcontrib-kroki"]
 html = ["html5lib"]
 networkx = ["networkx"]
 tests = ["html5lib", "pytest", "pytest-cov"]
 
 [[package]]
 name = "setuptools"
-version = "65.5.0"
+version = "65.5.1"
 description = "Easily download, build, install, upgrade, and uninstall Python packages"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-hoverxref (<2)", "sphinx-inline-tabs", "sphinx-notfound-page (==0.8.3)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
-testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8 (<5)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "mock", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
+testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8 (<5)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
 testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
 
 [[package]]
 name = "six"
 version = "1.16.0"
 description = "Python 2 and 3 compatibility utilities"
 category = "dev"
@@ -265,16 +265,16 @@
     {file = "pyparsing-3.0.9.tar.gz", hash = "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb"},
 ]
 rdflib = [
     {file = "rdflib-6.2.0-py3-none-any.whl", hash = "sha256:85c34a86dfc517a41e5f2425a41a0aceacc23983462b32e68610b9fad1383bca"},
     {file = "rdflib-6.2.0.tar.gz", hash = "sha256:62dc3c86d1712db0f55785baf8047f63731fa59b2682be03219cb89262065942"},
 ]
 setuptools = [
-    {file = "setuptools-65.5.0-py3-none-any.whl", hash = "sha256:f62ea9da9ed6289bfe868cd6845968a2c854d1427f8548d52cae02a42b4f0356"},
-    {file = "setuptools-65.5.0.tar.gz", hash = "sha256:512e5536220e38146176efb833d4a62aa726b7bbff82cfbc8ba9eaa3996e0b17"},
+    {file = "setuptools-65.5.1-py3-none-any.whl", hash = "sha256:d0b9a8433464d5800cbe05094acf5c6d52a91bfac9b52bcfc4d41382be5d5d31"},
+    {file = "setuptools-65.5.1.tar.gz", hash = "sha256:e197a19aa8ec9722928f2206f8de752def0e4c9fc6953527360d1c36d94ddb2f"},
 ]
 six = [
     {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
     {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
 ]
 tomli = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
```

### Comparing `reasonable-0.2.2a4/pyproject.toml` & `reasonable-0.2.3a1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasonable"
-version = "0.2.2a4"
+version = "0.2.3a1"
 description = "Python interface to 'reasonable', a Datalog implementation of the OWL 2 RL profile"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "bsd-3-clause"
 readme = "README.md"
 homepage = "https://github.com/gtfierro/reasonable"
 
 [tool.poetry.dependencies]
```

### Comparing `reasonable-0.2.2a4/scripts/bench_examples.sh` & `reasonable-0.2.3a1/scripts/bench_examples.sh`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/src/common.rs` & `reasonable-0.2.3a1/src/common.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/src/disjoint_sets.rs` & `reasonable-0.2.3a1/src/disjoint_sets.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/src/error.rs` & `reasonable-0.2.3a1/src/error.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/src/index.rs` & `reasonable-0.2.3a1/src/index.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/src/lib.rs` & `reasonable-0.2.3a1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/src/main.rs` & `reasonable-0.2.3a1/src/main.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/src/pyreason.rs` & `reasonable-0.2.3a1/src/pyreason.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/src/query.rs` & `reasonable-0.2.3a1/src/query.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.2a4/src/reasoner.rs` & `reasonable-0.2.3a1/src/reasoner.rs`

 * *Files 0% similar despite different names*

```diff
@@ -919,15 +919,15 @@
                 self.all_triples_input
                     .from_join(&self.owl_inv1, &self.pso, |&p1, &p2, &(x, y)| (y, (p2, x)));
 
                 // prp-inv2
                 // T(?p1, owl:inverseOf, ?p2)
                 // T(?x, ?p2, ?y) => T(?y, ?p1, ?x)
                 self.all_triples_input
-                    .from_join(&self.owl_inv2, &self.pso, |&p2, &p1, &(x, y)| (x, (p2, y)));
+                    .from_join(&self.owl_inv2, &self.pso, |&p2, &p1, &(x, y)| (y, (p1, x)));
 
                 // cax-sco
                 cax_sco_1.from_join(&self.pso, &rdfs_subclass_relation, |&_, &(c1, c2), &()| {
                     (c1, c2)
                 });
                 // ?c1, ?x, rdf:type
                 cax_sco_2.from_map(&rdf_type, |&(inst, class)| (class, inst));
```

### Comparing `reasonable-0.2.2a4/src/tests.rs` & `reasonable-0.2.3a1/src/tests.rs`

 * *Files 0% similar despite different names*

```diff
@@ -424,14 +424,36 @@
         "<urn:p2>".to_string(),
         "<urn:x>".to_string()
     )));
     Ok(())
 }
 
 #[test]
+fn test_prp_inv2() -> Result<(), String> {
+    let mut r = Reasoner::new();
+    let trips = vec![
+        ("urn:p1", OWL_INVERSEOF, "urn:p2"),
+        ("urn:y", "urn:p2", "urn:x"),
+    ];
+    r.load_triples_str(trips);
+    r.reason();
+    let res = r.get_triples_string();
+    for i in res.iter() {
+        let (s, p, o) = i;
+        println!("{} {} {}", s, p, o);
+    }
+    assert!(res.contains(&(
+        "<urn:x>".to_string(),
+        "<urn:p1>".to_string(),
+        "<urn:y>".to_string()
+    )));
+    Ok(())
+}
+
+#[test]
 fn test_prp_symp() -> Result<(), String> {
     let mut r = Reasoner::new();
     let trips = vec![
         ("urn:p", RDF_TYPE, OWL_SYMMETRICPROP),
         ("urn:x", "urn:p", "urn:y"),
     ];
     r.load_triples_str(trips);
```

### Comparing `reasonable-0.2.2a4/PKG-INFO` & `reasonable-0.2.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasonable
-Version: 0.2.2a4
+Version: 0.2.3a1
 Summary: An OWL 2 RL reasoner with reasonable performance
 Home-Page: https://brickschema.org/
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/gtfierro/reasonable
```

