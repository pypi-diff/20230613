# Comparing `tmp/proposal-7.6.0.tar.gz` & `tmp/proposal-7.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proposal-7.6.0.tar", last modified: Sat Jun 10 19:36:48 2023, max compression
+gzip compressed data, was "proposal-7.6.1.tar", last modified: Tue Jun 13 09:39:26 2023, max compression
```

## Comparing `proposal-7.6.0.tar` & `proposal-7.6.1.tar`

### file list

```diff
@@ -1,446 +1,446 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.200896 proposal-7.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-10 19:36:26.000000 proposal-7.6.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-10 19:36:26.000000 proposal-7.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-10 19:36:26.000000 proposal-7.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-10 19:36:48.200896 proposal-7.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-10 19:36:26.000000 proposal-7.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-10 19:36:26.000000 proposal-7.6.0/conanfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.144895 proposal-7.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-10 19:36:26.000000 proposal-7.6.0/docs/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.144895 proposal-7.6.0/proposal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-10 19:36:48.000000 proposal-7.6.0/proposal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-06-10 19:36:48.000000 proposal-7.6.0/proposal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:36:48.000000 proposal-7.6.0/proposal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:36:47.000000 proposal-7.6.0/proposal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 19:36:48.000000 proposal-7.6.0/proposal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-10 19:36:26.000000 proposal-7.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-10 19:36:48.200896 proposal-7.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-10 19:36:26.000000 proposal-7.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.144895 proposal-7.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-10 19:36:26.000000 proposal-7.6.0/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.144895 proposal-7.6.0/src/PROPOSAL/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/Config.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.148895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/Constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/DefaultFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/EnergyCutSettings.h
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/Logging.h
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/PROPOSAL.h
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/Propagator.h
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/RegisteredInDefault.h
--rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/Secondaries.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.152895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSection.h
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionBuilder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.152895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.h
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.h
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.156895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.h
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.h
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.156895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.h
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.h
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDirect.h
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionInterpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionMultiplier.h
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.156895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/AnnihilationFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/ComptonFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/EpairProductionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/IonizationFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/MupairProductionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoeffectFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotonuclearFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoproductionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/WeakInteractionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/ParticleDefaultCrossSectionList.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.160895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Annihilation.h
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Bremsstrahlung.h
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Compton.h
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/EpairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Ionization.h
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/MupairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParamTables.h
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.h
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParametrizationDirect.h
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoPairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.h
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.h
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoeffect.h
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photonuclear.h
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoproduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/WeakInteraction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.160895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/DecayChannel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/DecayTable.h
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/LeptonicDecayChannel.h
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/ManyBodyPhaseSpace.h
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/StableChannel.h
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/TwoBodyPhaseSpace.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.160895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_distr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_exponential.h
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_polynomial.h
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_splines.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.160895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Box.h
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Cylinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Geometry.h
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/GeometryFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Sphere.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.164895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Cartesian3D.h
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Function.h
--rw-r--r--   0 runner    (1001) docker     (123)    25604 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Integral.h
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Interpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/InterpolantBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/MathMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/RandomGenerator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Spherical3D.h
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Spline.h
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/TableWriter.h
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Vector3D.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.164895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/Components.h
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/Medium.h
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/MediumFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/methods.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.164895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/particle/
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/particle/Particle.h
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/particle/ParticleDef.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.164895 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/ContRand.h
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/ContRandBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Decay.h
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/DecayBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Displacement.h
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/DisplacementBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Interaction.h
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/InteractionBuilder.h
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtility.h
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Time.h
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/TimeBuilder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/Scattering.h
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/ScatteringFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/ScatteringMultiplier.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Coefficients.h
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Highland.h
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.h
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Moliere.h
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Parametrization.h
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/ScatteringFactory.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/Parametrization.h
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ScatteringFactory.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.h
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.h
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/Bremsstrahlung.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.h
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairProduction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.h
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/Ionization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.h
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.h
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/Photonuclear.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/SecondariesCalculator.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/Parametrization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/Annihilation.h
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.h
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.h
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.h
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.168896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/Compton.h
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/NaivCompton.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/EpairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/NaivEpairProduction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/Ionization.h
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/MupairProduction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/Photoeffect.h
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/Photonuclear.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionInterpolant.h
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionKochMotz.h
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.h
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/SauterSampling.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/Photoproduction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.h
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakInteraction.h
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/PROPOSAL/version.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/detail/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Constants.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/EnergyCutSettings.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Logging.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    24313 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Propagator.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Secondaries.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.172896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSection.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.176895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.176895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.176895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.176895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/AnnihilationFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/ComptonFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/EpairProductionFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/IonizationFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/MupairProductionFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoeffectFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotonuclearFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoproductionFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/WeakInteractionFactory.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.180896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Annihilation.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    23803 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Bremsstrahlung.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Compton.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    22472 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/EpairProduction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Ionization.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/MupairProduction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)  1205025 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/ParamTables.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoPairProduction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    36224 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoeffect.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photonuclear.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoproduction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/WeakInteraction.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.180896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/DecayChannel.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/DecayTable.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/LeptonicDecayChannel.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/ManyBodyPhaseSpace.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/StableChannel.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/TwoBodyPhaseSpace.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.180896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_distr.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_exponential.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_homogeneous.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_polynomial.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_splines.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.184896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Box.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Cylinder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Geometry.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/GeometryFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Sphere.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.184896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Cartesian3D.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Function.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    66888 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Integral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    54597 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Interpolant.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/InterpolantBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/MathMethods.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/RandomGenerator.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Spherical3D.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Spline.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Vector3D.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.184896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/Components.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    17084 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/Medium.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/MediumFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/methods.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.184896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/particle/
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/particle/Particle.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/particle/ParticleDef.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.184896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRand.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRandBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Decay.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DecayBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Displacment.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DisplacmentBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Interaction.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/InteractionBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtility.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityIntegral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Time.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/TimeBuilder.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.132895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Coefficients.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Highland.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Moliere.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Parametrization.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.136895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/SecondariesCalculator.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.136895 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/NaivCompton.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-10 19:36:26.000000 proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.188896 proposal-7.6.0/src/pyPROPOSAL/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.192896 proposal-7.6.0/src/pyPROPOSAL/detail/
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/components.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/crosssection.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/decay.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/density_distribution.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/geometry.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/math.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/medium.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    48752 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/parametrization.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    34074 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/particle.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/pybindings.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/scattering.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/detail/secondaries.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.192896 proposal-7.6.0/src/pyPROPOSAL/pyPROPOSAL/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-10 19:36:26.000000 proposal-7.6.0/src/pyPROPOSAL/pyPROPOSAL/pyBindings.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.196896 proposal-7.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Annihilation_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Bremsstrahlung_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Compton_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/ContinuousRandomization_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/CrossSection_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    32454 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/DecayChannel_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/DecayTable_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Decay_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Density_distribution_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Displacement_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/EnergyCutSettings_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Epairproduction_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    42070 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Geometry_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Integral_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Interaction_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Interpolant_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Ionization_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/MathMethods_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Medium_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Mupairproduction_TEST.cxx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.196896 proposal-7.6.0/tests/PROPOSALTestUtilities/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/PROPOSALTestUtilities/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/PROPOSALTestUtilities/TestFilesHandling.h
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/ParticleDef_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Particle_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/PhotoMuPair_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/PhotoPair_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Photoeffect_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    23832 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Photonuclear_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Propagator_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Scattering_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Secondaries_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/SecondaryProduction_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Sector_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Spline_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Time_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/UtilityIntegral_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/UtilityInterpolant_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Utility_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/Vector3D_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/WeakInteraction_TEST.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/conanfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.200896 proposal-7.6.0/tests/gen_testfiles_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/annihilation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/bremsstrahlung.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/compton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/continous_randomization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/epairproduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/ionization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/mupairproduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/photomupair.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/photonuclear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/photopair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/scattering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/sector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/gen_testfiles_scripts/weak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:36:48.200896 proposal-7.6.0/tests/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-10 19:36:26.000000 proposal-7.6.0/tests/python/test_continuous_loss_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.472467 proposal-7.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-13 09:39:05.000000 proposal-7.6.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-13 09:39:05.000000 proposal-7.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-13 09:39:05.000000 proposal-7.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-13 09:39:26.472467 proposal-7.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-13 09:39:05.000000 proposal-7.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-13 09:39:05.000000 proposal-7.6.1/conanfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.420466 proposal-7.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 09:39:05.000000 proposal-7.6.1/docs/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.420466 proposal-7.6.1/proposal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-06-13 09:39:26.000000 proposal-7.6.1/proposal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-06-13 09:39:26.000000 proposal-7.6.1/proposal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:39:26.000000 proposal-7.6.1/proposal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:39:26.000000 proposal-7.6.1/proposal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 09:39:26.000000 proposal-7.6.1/proposal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 09:39:05.000000 proposal-7.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 09:39:26.472467 proposal-7.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-13 09:39:05.000000 proposal-7.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.420466 proposal-7.6.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-13 09:39:05.000000 proposal-7.6.1/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.420466 proposal-7.6.1/src/PROPOSAL/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/Config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.424466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/DefaultFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/EnergyCutSettings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/Logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/PROPOSAL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/Propagator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/RegisteredInDefault.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/Secondaries.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.424466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSection.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionBuilder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.424466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.h
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.424466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.h
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.424466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.h
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDirect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionInterpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionMultiplier.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.428466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/AnnihilationFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/ComptonFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/EpairProductionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/IonizationFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/MupairProductionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoeffectFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotonuclearFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotoproductionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/WeakInteractionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/ParticleDefaultCrossSectionList.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.428466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Annihilation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Bremsstrahlung.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Compton.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/EpairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Ionization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/MupairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParamTables.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParametrizationDirect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoPairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoeffect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photonuclear.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoproduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/WeakInteraction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.428466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/DecayChannel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/DecayTable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/LeptonicDecayChannel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/ManyBodyPhaseSpace.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/StableChannel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/TwoBodyPhaseSpace.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.432466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/density_distr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/density_exponential.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/density_homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/density_polynomial.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/density_splines.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.432466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/Box.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/Cylinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/Geometry.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/GeometryFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/Sphere.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.432466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Cartesian3D.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Function.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25604 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Integral.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Interpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/InterpolantBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/MathMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/RandomGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Spherical3D.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Spline.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/TableWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Vector3D.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.432466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/medium/
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/medium/Components.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/medium/Medium.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/medium/MediumFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/methods.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.432466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/particle/
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/particle/Particle.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/particle/ParticleDef.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/ContRand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/ContRandBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/Decay.h
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/DecayBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/Displacement.h
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/DisplacementBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/Interaction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/InteractionBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtility.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/Time.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/TimeBuilder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/Scattering.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/ScatteringFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/ScatteringMultiplier.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Coefficients.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Highland.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Moliere.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Parametrization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/ScatteringFactory.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/Parametrization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ScatteringFactory.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.h
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/Bremsstrahlung.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.h
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairProduction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.h
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/Ionization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.h
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/Photonuclear.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/SecondariesCalculator.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/Parametrization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.436466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/Annihilation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.h
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.h
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/Compton.h
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/NaivCompton.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/EpairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/NaivEpairProduction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/Ionization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/MupairProduction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/Photoeffect.h
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/Photonuclear.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionInterpolant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionKochMotz.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/SauterSampling.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/Photoproduction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.h
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakInteraction.h
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/PROPOSAL/version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.440466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/Constants.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/EnergyCutSettings.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/Logging.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    24313 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/Propagator.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/Secondaries.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.444466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSection.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.444466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.444466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.444466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.448466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/AnnihilationFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/ComptonFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/EpairProductionFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/IonizationFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/MupairProductionFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoeffectFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotonuclearFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoproductionFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/WeakInteractionFactory.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.448466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Annihilation.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    23803 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Bremsstrahlung.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Compton.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    22472 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/EpairProduction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Ionization.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/MupairProduction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)  1205025 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/ParamTables.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoPairProduction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    36224 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoeffect.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photonuclear.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoproduction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/WeakInteraction.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.452466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/DecayChannel.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/DecayTable.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/LeptonicDecayChannel.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/ManyBodyPhaseSpace.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/StableChannel.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/TwoBodyPhaseSpace.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.452466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_distr.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_exponential.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_homogeneous.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_polynomial.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_splines.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.452466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/Box.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/Cylinder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/Geometry.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/GeometryFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/Sphere.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.452466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Cartesian3D.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Function.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    66888 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Integral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    54597 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Interpolant.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/InterpolantBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/MathMethods.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/RandomGenerator.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Spherical3D.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Spline.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Vector3D.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.452466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/medium/
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/medium/Components.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    17084 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/medium/Medium.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/medium/MediumFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/methods.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.452466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/particle/
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/particle/Particle.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/particle/ParticleDef.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.456466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRand.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRandBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Decay.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DecayBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Displacment.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DisplacmentBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Interaction.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/InteractionBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtility.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityIntegral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Time.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/TimeBuilder.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.416466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.456466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Coefficients.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Highland.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Moliere.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Parametrization.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.416466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.456466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.456466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.456466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.456466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.456466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/SecondariesCalculator.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.420466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.456466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/NaivCompton.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-13 09:39:05.000000 proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/pyPROPOSAL/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/pyPROPOSAL/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/components.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/crosssection.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/decay.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/density_distribution.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/geometry.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/math.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/medium.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    48752 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/parametrization.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    34074 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/particle.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    22377 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/pybindings.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/scattering.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/detail/secondaries.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.460466 proposal-7.6.1/src/pyPROPOSAL/pyPROPOSAL/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-13 09:39:05.000000 proposal-7.6.1/src/pyPROPOSAL/pyPROPOSAL/pyBindings.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.468467 proposal-7.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Annihilation_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Bremsstrahlung_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Compton_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/ContinuousRandomization_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/CrossSection_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    32454 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/DecayChannel_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/DecayTable_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Decay_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Density_distribution_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Displacement_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/EnergyCutSettings_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Epairproduction_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    42070 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Geometry_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Integral_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Interaction_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Interpolant_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Ionization_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/MathMethods_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Medium_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Mupairproduction_TEST.cxx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.468467 proposal-7.6.1/tests/PROPOSALTestUtilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/PROPOSALTestUtilities/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/PROPOSALTestUtilities/TestFilesHandling.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/ParticleDef_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Particle_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/PhotoMuPair_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/PhotoPair_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Photoeffect_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    23832 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Photonuclear_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Propagator_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Scattering_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Secondaries_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/SecondaryProduction_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Sector_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Spline_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Time_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/UtilityIntegral_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/UtilityInterpolant_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Utility_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/Vector3D_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/WeakInteraction_TEST.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/conanfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.468467 proposal-7.6.1/tests/gen_testfiles_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/annihilation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/bremsstrahlung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/compton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/continous_randomization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/epairproduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/ionization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/mupairproduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/photomupair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/photonuclear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/photopair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/sector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/gen_testfiles_scripts/weak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:39:26.468467 proposal-7.6.1/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-13 09:39:05.000000 proposal-7.6.1/tests/python/test_continuous_loss_output.py
```

### Comparing `proposal-7.6.0/CMakeLists.txt` & `proposal-7.6.1/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cmake_minimum_required(VERSION 3.9)
 
 set(PROPOSAL_VERSION_MAJOR 7)
 set(PROPOSAL_VERSION_MINOR 6)
-set(PROPOSAL_VERSION_PATCH 0)
+set(PROPOSAL_VERSION_PATCH 1)
 set(PROPOSAL_VERSION ${PROPOSAL_VERSION_MAJOR}.${PROPOSAL_VERSION_MINOR}.${PROPOSAL_VERSION_PATCH})
 
 project(PROPOSAL
     VERSION ${PROPOSAL_VERSION}
     LANGUAGES CXX
     DESCRIPTION "The very best photon and lepton propagator."
     )
```

### Comparing `proposal-7.6.0/LICENSE.md` & `proposal-7.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/PKG-INFO` & `proposal-7.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proposal
-Version: 7.6.0
+Version: 7.6.1
 Summary: Monte Carlo simulation library to propagate leptons and gamma rays
 Home-page: https://github.com/tudo-astroparticlephysics/PROPOSAL
 Author: PROPOSAL Development Team
 Author-email: jean-marco.alameddine@tu-dortmund.de
 License: LGPLv3
 Platform: unix
 Classifier: Intended Audience :: Science/Research
```

### Comparing `proposal-7.6.0/README.md` & `proposal-7.6.1/README.md`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/conanfile.py` & `proposal-7.6.1/conanfile.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/proposal.egg-info/PKG-INFO` & `proposal-7.6.1/proposal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proposal
-Version: 7.6.0
+Version: 7.6.1
 Summary: Monte Carlo simulation library to propagate leptons and gamma rays
 Home-page: https://github.com/tudo-astroparticlephysics/PROPOSAL
 Author: PROPOSAL Development Team
 Author-email: jean-marco.alameddine@tu-dortmund.de
 License: LGPLv3
 Platform: unix
 Classifier: Intended Audience :: Science/Research
```

### Comparing `proposal-7.6.0/proposal.egg-info/SOURCES.txt` & `proposal-7.6.1/proposal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/setup.cfg` & `proposal-7.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/setup.py` & `proposal-7.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/CMakeLists.txt` & `proposal-7.6.1/src/PROPOSAL/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/Config.cmake.in` & `proposal-7.6.1/src/PROPOSAL/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/Constants.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/Constants.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/DefaultFactory.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/DefaultFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/EnergyCutSettings.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/EnergyCutSettings.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/Logging.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/Logging.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/PROPOSAL.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/PROPOSAL.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/Propagator.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/Propagator.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/RegisteredInDefault.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/RegisteredInDefault.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/Secondaries.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/Secondaries.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSection.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSection.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionBuilder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXBuilder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXBuilder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXBuilder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDirect.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionDirect.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionIntegral.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionInterpolant.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionMultiplier.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionMultiplier.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionVector.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/CrossSectionVector.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/EpairProductionFactory.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/EpairProductionFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotonuclearFactory.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/Factories/PhotonuclearFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/ParticleDefaultCrossSectionList.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/ParticleDefaultCrossSectionList.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Annihilation.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Annihilation.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Bremsstrahlung.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Bremsstrahlung.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Compton.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Compton.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/EpairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/EpairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Ionization.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Ionization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/MupairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/MupairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParamTables.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParamTables.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.hpp` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Parametrization.hpp`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParametrizationDirect.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/ParametrizationDirect.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoPairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoPairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoeffect.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoeffect.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photonuclear.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photonuclear.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoproduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/Photoproduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/crosssection/parametrization/WeakInteraction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/crosssection/parametrization/WeakInteraction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/DecayChannel.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/DecayChannel.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/DecayTable.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/DecayTable.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/LeptonicDecayChannel.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/LeptonicDecayChannel.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/ManyBodyPhaseSpace.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/ManyBodyPhaseSpace.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/StableChannel.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/StableChannel.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/decay/TwoBodyPhaseSpace.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/decay/TwoBodyPhaseSpace.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_distr.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/density_distr.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_exponential.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/density_exponential.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_homogeneous.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/density_homogeneous.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_polynomial.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/density_polynomial.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/density_distr/density_splines.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/density_distr/density_splines.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Box.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/Box.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Cylinder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/Cylinder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Geometry.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/Geometry.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/GeometryFactory.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/GeometryFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/geometry/Sphere.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/geometry/Sphere.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Cartesian3D.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Cartesian3D.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Function.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Function.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Integral.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Integral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Interpolant.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Interpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/InterpolantBuilder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/InterpolantBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/MathMethods.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/MathMethods.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/RandomGenerator.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/RandomGenerator.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Spherical3D.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Spherical3D.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Spline.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Spline.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/TableWriter.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/TableWriter.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/math/Vector3D.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/math/Vector3D.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/Components.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/medium/Components.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/Medium.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/medium/Medium.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/medium/MediumFactory.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/medium/MediumFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/methods.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/methods.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/particle/Particle.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/particle/Particle.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/particle/ParticleDef.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/particle/ParticleDef.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/ContRand.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/ContRand.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/ContRandBuilder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/ContRandBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Decay.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/Decay.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/DecayBuilder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/DecayBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Displacement.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/Displacement.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/DisplacementBuilder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/DisplacementBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/Interaction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/Interaction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/InteractionBuilder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/InteractionBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtility.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtility.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityIntegral.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/propagation_utility/TimeBuilder.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/propagation_utility/TimeBuilder.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/Scattering.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/Scattering.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/ScatteringFactory.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/ScatteringFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/ScatteringMultiplier.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/ScatteringMultiplier.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Coefficients.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Coefficients.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Highland.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Highland.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Moliere.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Moliere.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Parametrization.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/Parametrization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/ScatteringFactory.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/multiple_scattering/ScatteringFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/Parametrization.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/Parametrization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ScatteringFactory.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ScatteringFactory.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/Ionization.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/ionization/Ionization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/Photonuclear.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/scattering/stochastic_deflection/photonuclear/Photonuclear.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/SecondariesCalculator.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/SecondariesCalculator.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/Parametrization.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/Parametrization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/Annihilation.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/Annihilation.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsNoDeflection.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/Compton.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/Compton.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/NaivCompton.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/compton/NaivCompton.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/EpairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/EpairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/KelnerKokoulinPetrukhinEpairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/NaivEpairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/epairproduction/NaivEpairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/Ionization.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/Ionization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/MupairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/mupairproduction/MupairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/Photoeffect.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/Photoeffect.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/Photonuclear.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photonuclear/Photonuclear.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionInterpolant.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionInterpolant.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionKochMotz.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionKochMotz.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/SauterSampling.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photopairproduction/SauterSampling.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/Photoproduction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/photoproduction/Photoproduction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakInteraction.h` & `proposal-7.6.1/src/PROPOSAL/PROPOSAL/secondaries/parametrization/weakinteraction/WeakInteraction.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Constants.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/Constants.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/EnergyCutSettings.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/EnergyCutSettings.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Propagator.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/Propagator.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/Secondaries.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/Secondaries.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSection.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSection.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/AxisBuilderDE2DX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXIntegral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDE2DX/CrossSectionDE2DXInterpolant.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/AxisBuilderDEDX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXIntegral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDEDX/CrossSectionDEDXInterpolant.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/AxisBuilderDNDX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDX.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXIntegral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/CrossSectionDNDX/CrossSectionDNDXInterpolant.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/AnnihilationFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/AnnihilationFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/BremsstrahlungFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/ComptonFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/ComptonFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/EpairProductionFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/EpairProductionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/IonizationFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/IonizationFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/MupairProductionFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/MupairProductionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoMuPairProductionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoPairProductionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoeffectFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoeffectFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotonuclearFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotonuclearFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoproductionFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/PhotoproductionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/WeakInteractionFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/Factories/WeakInteractionFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Annihilation.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Annihilation.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Bremsstrahlung.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Bremsstrahlung.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Compton.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Compton.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/EpairProduction.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/EpairProduction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Ionization.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Ionization.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/MupairProduction.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/MupairProduction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/ParamTables.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/ParamTables.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoMuPairProduction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoPairProduction.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoPairProduction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoQ2Integration.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/PhotoRealPhotonAssumption.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoeffect.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoeffect.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photonuclear.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photonuclear.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoproduction.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/Photoproduction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/WeakInteraction.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/crosssection/parametrization/WeakInteraction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/DecayChannel.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/DecayChannel.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/DecayTable.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/DecayTable.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/LeptonicDecayChannel.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/LeptonicDecayChannel.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/ManyBodyPhaseSpace.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/ManyBodyPhaseSpace.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/StableChannel.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/StableChannel.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/decay/TwoBodyPhaseSpace.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/decay/TwoBodyPhaseSpace.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_distr.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_distr.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_exponential.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_exponential.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_homogeneous.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_homogeneous.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_polynomial.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_polynomial.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/density_distr/density_splines.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/density_distr/density_splines.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Box.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/Box.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Cylinder.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/Cylinder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Geometry.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/Geometry.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/GeometryFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/GeometryFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/geometry/Sphere.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/geometry/Sphere.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Cartesian3D.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Cartesian3D.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Function.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Function.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Integral.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Integral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Interpolant.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Interpolant.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/InterpolantBuilder.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/InterpolantBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/MathMethods.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/MathMethods.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/RandomGenerator.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/RandomGenerator.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Spherical3D.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Spherical3D.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Spline.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Spline.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/math/Vector3D.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/math/Vector3D.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/Components.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/medium/Components.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/Medium.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/medium/Medium.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/medium/MediumFactory.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/medium/MediumFactory.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/methods.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/methods.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/particle/Particle.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/particle/Particle.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/particle/ParticleDef.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/particle/ParticleDef.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRand.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRand.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRandBuilder.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/ContRandBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Decay.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Decay.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DecayBuilder.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DecayBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DisplacmentBuilder.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/DisplacmentBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Interaction.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/Interaction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/InteractionBuilder.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/InteractionBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtility.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtility.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityIntegral.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityIntegral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/PropagationUtilityInterpolant.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/propagation_utility/TimeBuilder.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/propagation_utility/TimeBuilder.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Coefficients.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Coefficients.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Highland.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Highland.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/HighlandIntegral.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Moliere.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Moliere.cxx`

 * *Files 2% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 
     double sum = c1[69] / (2. * 69 + 1.);
 
     // Horner's method
     for (int p = 68; p >= 0; p--)
         sum = sum * x + c1[p] / (2. * p + 1.);
 
-    return sum * std::sqrt(x);
+    return sum * std::sqrt(std::max(x, 0.));
 }
 
 //----------------------------------------------------------------------------//
 
 double F2Mlarge(double x)
 {
     double a = -0.00026360133958801203364619158975302;
@@ -317,28 +317,28 @@
         return F2Mlarge(x);
 
     double sum = c2[69] / (2. * 69 + 1.);
 
     for (int p = 68; p >= 0; p--)
         sum = sum * x + c2[p] / (2. * p + 1.);
 
-    return sum * std::sqrt(x);
+    return sum * std::sqrt(std::max(x, 0.));
 }
 
 //----------------------------------------------------------------------------//
 
 double Moliere::F(double theta)
 {
     double y1 = 0;
 
     for (int i = 0; i < numComp_; i++) {
         double x = theta * theta / (chiCSq_ * B_[i]);
 
         y1 += weight_ZZ_[i]
-            * (0.5 * std::erf(std::sqrt(x))
+            * (0.5 * std::erf(std::sqrt(std::max(x, 0.)))
                 + std::sqrt(1. / PI)
                     * (F1M(x) / B_[i] + F2M(x) / (B_[i] * B_[i])));
     }
 
     return (theta < 0.) ? (-1.) * y1 * weight_ZZ_sum_ : y1 * weight_ZZ_sum_;
 }
```

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Parametrization.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/multiple_scattering/Parametrization.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsGinneken.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/bremsstrahlung/BremsTsaiApproximation.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/epairproduction/EpairGinneken.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/ionization/IonizNaive.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoBorogPetrukhin.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/scattering/stochastic_deflection/photonuclear/PhotoGinneken.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/SecondariesCalculator.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/SecondariesCalculator.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/annihilation/HeitlerAnnihilation.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsEGS4Approximation.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/BremsKochMotz.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/bremsstrahlung/Bremsstrahlung.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/NaivCompton.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/compton/NaivCompton.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/ionization/NaivIonization.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/mupairproduction/KelnerKokoulinPetrukhinMupairProduction.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photoeffect/PhotoeffectNoDeflection.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photomupairproduction/PhotoMuPairProductionBurkhardtKelnerKokoulin.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/photopairproduction/PhotoPairProductionTsai.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.cxx` & `proposal-7.6.1/src/PROPOSAL/detail/PROPOSAL/secondaries/parametrization/weakinteraction/WeakCooperSarkarMertsch.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/CMakeLists.txt` & `proposal-7.6.1/src/pyPROPOSAL/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/components.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/components.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/crosssection.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/crosssection.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/decay.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/decay.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/density_distribution.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/density_distribution.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/geometry.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/geometry.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/math.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/math.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/medium.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/medium.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/parametrization.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/parametrization.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/particle.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/particle.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/pybindings.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/pybindings.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/scattering.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/scattering.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/src/pyPROPOSAL/detail/secondaries.cxx` & `proposal-7.6.1/src/pyPROPOSAL/detail/secondaries.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Annihilation_TEST.cxx` & `proposal-7.6.1/tests/Annihilation_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Bremsstrahlung_TEST.cxx` & `proposal-7.6.1/tests/Bremsstrahlung_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/CMakeLists.txt` & `proposal-7.6.1/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Compton_TEST.cxx` & `proposal-7.6.1/tests/Compton_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/ContinuousRandomization_TEST.cxx` & `proposal-7.6.1/tests/ContinuousRandomization_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/CrossSection_TEST.cxx` & `proposal-7.6.1/tests/CrossSection_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/DecayChannel_TEST.cxx` & `proposal-7.6.1/tests/DecayChannel_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/DecayTable_TEST.cxx` & `proposal-7.6.1/tests/DecayTable_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Decay_TEST.cxx` & `proposal-7.6.1/tests/Decay_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Density_distribution_TEST.cxx` & `proposal-7.6.1/tests/Density_distribution_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Displacement_TEST.cxx` & `proposal-7.6.1/tests/Displacement_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/EnergyCutSettings_TEST.cxx` & `proposal-7.6.1/tests/EnergyCutSettings_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Epairproduction_TEST.cxx` & `proposal-7.6.1/tests/Epairproduction_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Geometry_TEST.cxx` & `proposal-7.6.1/tests/Geometry_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Integral_TEST.cxx` & `proposal-7.6.1/tests/Integral_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Interaction_TEST.cxx` & `proposal-7.6.1/tests/Interaction_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Interpolant_TEST.cxx` & `proposal-7.6.1/tests/Interpolant_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Ionization_TEST.cxx` & `proposal-7.6.1/tests/Ionization_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/MathMethods_TEST.cxx` & `proposal-7.6.1/tests/MathMethods_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Medium_TEST.cxx` & `proposal-7.6.1/tests/Medium_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Mupairproduction_TEST.cxx` & `proposal-7.6.1/tests/Mupairproduction_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/PROPOSALTestUtilities/TestFilesHandling.h` & `proposal-7.6.1/tests/PROPOSALTestUtilities/TestFilesHandling.h`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/ParticleDef_TEST.cxx` & `proposal-7.6.1/tests/ParticleDef_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Particle_TEST.cxx` & `proposal-7.6.1/tests/Particle_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/PhotoMuPair_TEST.cxx` & `proposal-7.6.1/tests/PhotoMuPair_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/PhotoPair_TEST.cxx` & `proposal-7.6.1/tests/PhotoPair_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Photoeffect_TEST.cxx` & `proposal-7.6.1/tests/Photoeffect_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Photonuclear_TEST.cxx` & `proposal-7.6.1/tests/Photonuclear_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Propagator_TEST.cxx` & `proposal-7.6.1/tests/Propagator_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Scattering_TEST.cxx` & `proposal-7.6.1/tests/Scattering_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Secondaries_TEST.cxx` & `proposal-7.6.1/tests/Secondaries_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/SecondaryProduction_TEST.cxx` & `proposal-7.6.1/tests/SecondaryProduction_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Sector_TEST.cxx` & `proposal-7.6.1/tests/Sector_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Spline_TEST.cxx` & `proposal-7.6.1/tests/Spline_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Time_TEST.cxx` & `proposal-7.6.1/tests/Time_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/UtilityIntegral_TEST.cxx` & `proposal-7.6.1/tests/UtilityIntegral_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/UtilityInterpolant_TEST.cxx` & `proposal-7.6.1/tests/UtilityInterpolant_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Utility_TEST.cxx` & `proposal-7.6.1/tests/Utility_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/Vector3D_TEST.cxx` & `proposal-7.6.1/tests/Vector3D_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/WeakInteraction_TEST.cxx` & `proposal-7.6.1/tests/WeakInteraction_TEST.cxx`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/conanfile.py` & `proposal-7.6.1/tests/conanfile.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/__init__.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/annihilation.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/annihilation.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/bremsstrahlung.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/bremsstrahlung.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/compton.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/compton.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/continous_randomization.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/continous_randomization.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/decay.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/decay.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/epairproduction.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/epairproduction.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/ionization.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/ionization.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/mupairproduction.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/mupairproduction.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/photomupair.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/photomupair.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/photonuclear.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/photonuclear.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/photopair.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/photopair.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/propagation.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/propagation.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/scattering.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/scattering.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/sector.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/sector.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/gen_testfiles_scripts/weak.py` & `proposal-7.6.1/tests/gen_testfiles_scripts/weak.py`

 * *Files identical despite different names*

### Comparing `proposal-7.6.0/tests/python/test_continuous_loss_output.py` & `proposal-7.6.1/tests/python/test_continuous_loss_output.py`

 * *Files identical despite different names*

