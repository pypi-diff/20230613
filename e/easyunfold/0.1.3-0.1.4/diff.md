# Comparing `tmp/easyunfold-0.1.3.tar.gz` & `tmp/easyunfold-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyunfold-0.1.3.tar", last modified: Mon Mar 27 14:56:20 2023, max compression
+gzip compressed data, was "easyunfold-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `easyunfold-0.1.3.tar` & `easyunfold-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1076 2023-03-27 14:56:10.161251 easyunfold-0.1.3/LICENSE
--rw-r--r--   0        0        0     3859 2023-03-27 14:56:10.161251 easyunfold-0.1.3/README.md
--rw-r--r--   0        0        0       69 2023-03-27 14:56:10.161251 easyunfold-0.1.3/easyunfold/__init__.py
--rw-r--r--   0        0        0    18880 2023-03-27 14:56:10.161251 easyunfold-0.1.3/easyunfold/cli.py
--rw-r--r--   0        0        0    11516 2023-03-27 14:56:10.161251 easyunfold-0.1.3/easyunfold/effective_mass.py
--rw-r--r--   0        0        0    22927 2023-03-27 14:56:10.161251 easyunfold-0.1.3/easyunfold/plotting.py
--rw-r--r--   0        0        0     4750 2023-03-27 14:56:10.161251 easyunfold-0.1.3/easyunfold/procar.py
--rw-r--r--   0        0        0    43895 2023-03-27 14:56:10.161251 easyunfold-0.1.3/easyunfold/unfold.py
--rw-r--r--   0        0        0     1935 2023-03-27 14:56:10.161251 easyunfold-0.1.3/easyunfold/vasp_constant.py
--rw-r--r--   0        0        0    11470 2023-03-27 14:56:10.161251 easyunfold-0.1.3/easyunfold/wavecar.py
--rw-r--r--   0        0        0      955 2023-03-27 14:56:10.473270 easyunfold-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 easyunfold-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-13 16:28:16.079295 easyunfold-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3860 2023-06-13 16:28:16.079295 easyunfold-0.1.4/README.md
+-rw-r--r--   0        0        0       69 2023-06-13 16:28:16.079295 easyunfold-0.1.4/easyunfold/__init__.py
+-rw-r--r--   0        0        0    21540 2023-06-13 16:28:16.079295 easyunfold-0.1.4/easyunfold/cli.py
+-rw-r--r--   0        0        0    11517 2023-06-13 16:28:16.079295 easyunfold-0.1.4/easyunfold/effective_mass.py
+-rw-r--r--   0        0        0    22927 2023-06-13 16:28:16.079295 easyunfold-0.1.4/easyunfold/plotting.py
+-rw-r--r--   0        0        0     4750 2023-06-13 16:28:16.079295 easyunfold-0.1.4/easyunfold/procar.py
+-rw-r--r--   0        0        0    42775 2023-06-13 16:28:16.079295 easyunfold-0.1.4/easyunfold/unfold.py
+-rw-r--r--   0        0        0     9413 2023-06-13 16:28:16.079295 easyunfold-0.1.4/easyunfold/utils.py
+-rw-r--r--   0        0        0     1935 2023-06-13 16:28:16.079295 easyunfold-0.1.4/easyunfold/vasp_constant.py
+-rw-r--r--   0        0        0    11470 2023-06-13 16:28:16.079295 easyunfold-0.1.4/easyunfold/wavecar.py
+-rw-r--r--   0        0        0     3392 2023-06-13 16:28:16.079295 easyunfold-0.1.4/easyunfold/wavefun.py
+-rw-r--r--   0        0        0     1069 2023-06-13 16:28:16.347298 easyunfold-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5117 1970-01-01 00:00:00.000000 easyunfold-0.1.4/PKG-INFO
```

### Comparing `easyunfold-0.1.3/LICENSE` & `easyunfold-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easyunfold-0.1.3/README.md` & `easyunfold-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Easyunfold
 
 
 ![build](https://github.com/SMTG-UCL/easyunfold/actions/workflows/ci.yaml/badge.svg)
 [![docs](https://github.com/SMTG-UCL/easyunfold/actions/workflows/docs.yaml/badge.svg)](https://smtg-ucl.github.io/easyunfold/)
-[![codecov](https://codecov.io/gh/SMTG-UCL/easyunfold/branch/dev/graph/badge.svg?token=XLLWWU5UM2)](https://codecov.io/gh/SMTG-UCL/easyunfold)
+[![codecov](https://codecov.io/gh/SMTG-UCL/easyunfold/branch/main/graph/badge.svg?token=XLLWWU5UM2)](https://codecov.io/gh/SMTG-UCL/easyunfold)
 
 ![easyunfold](docs/img/logo.svg)
 
 Documentation: https://smtg-ucl.github.io/easyunfold/
 
 This package is intended for obtaining the effective band structure of a supercell for a certain path of the primitive cell.
 It was originally based on [PyVaspwfc](https://github.com/QijingZheng/VaspBandUnfolding) for reading wavefunction output of VASP, and contains some code of the latter.
```

### Comparing `easyunfold-0.1.3/easyunfold/cli.py` & `easyunfold-0.1.4/easyunfold/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import click
 from ase.io import read
 
 from easyunfold.unfold import process_projection_options
 
 # pylint:disable=import-outside-toplevel,too-many-locals
 
+SUPPORTED_DFT_CODES = ('vasp', 'castep')
+
 DEFAULT_CMAPS = [
     'Purples', 'Greens', 'Oranges', 'Reds', 'Blue', 'YlOrBr', 'YlOrRd', 'OrRd', 'PuRd', 'RdPu', 'BuPu', 'GnBu', 'PuBu', 'YlGnBu', 'PuBuGn',
     'BuGn', 'YlGn'
 ]
 
 
 @click.group('easyunfold')
@@ -26,27 +28,52 @@
 
 
 @easyunfold.command()
 @click.option('--time-reversal/--no-time-reversal', default=True)
 @click.argument('pc-file')
 @click.argument('sc-file')
 @click.argument('kpoints')
+@click.option(
+    '--code',
+    '-c',
+    help='Name of the DFT code that the kpoints should be formatted to.',
+    default='vasp',
+    type=click.Choice(SUPPORTED_DFT_CODES),
+    show_default=True,
+)
 @click.option('--matrix', '-m', help='Transformation matrix')
-@click.option('--symprec', help='Transformation matrix', type=float, default=1e-5)
+@click.option('--symprec', help='Transformation matrix', type=float, default=1e-5, show_default=True)
 @click.option('--out-file', default='easyunfold.json', help='Name of the output file')
 @click.option('--no-expand', help='Do not expand the kpoints by symmetry', default=False, is_flag=True)
 @click.option('--nk-per-split', help='Number of band structure kpoints per split.', type=int)
 @click.option('--scf-kpoints',
               help='File (IBZKPT) to provide SCF kpoints for self-consistent calculations. Needed for hybrid functional calculations.',
               type=click.Path(exists=True, dir_okay=False))
-def generate(pc_file, sc_file, matrix, kpoints, time_reversal, out_file, no_expand, symprec, nk_per_split, scf_kpoints):
+@click.option('--yes', '-y', is_flag=True, default=False, help='Skip and confirmation.')
+def generate(pc_file, code, sc_file, matrix, kpoints, time_reversal, out_file, no_expand, symprec, nk_per_split, scf_kpoints, yes):
     """
-    Generate the kpoints for sampling the supercell
+    Generate the kpoints for performing supercell calculations.
+
+    There are two modes of running supercell calculations:
+
+    1. Use the generated kpoints for unfolding for non-SCF calculations, e.g. with a fixed
+       charged density from the SCF calculation.
+    2. Include the generated kpoints in SCF calculation but set their weights to zeros.
+
+    In both cases, the kpoints can be split into multiple calculations.
+
+    This command defaults to go down the first route where the kpoints generated are only
+    those needed for the unfolding, all kpoints and written into the same file, but the user
+    is free to manually split them into multiple calculations.
+    The second approach can be activated with the ``--nk-per-split`` option and in the same
+    time provide the ``--scf-kpoints``. This will generate a serial of kpoints files containing
+    the SCF kpoints followed by the actual kpoints needed for unfolding with zero weights.
     """
-    from easyunfold.unfold import UnfoldKSet, read_kpoints
+    from easyunfold.unfold import UnfoldKSet
+    from easyunfold.utils import read_kpoints
 
     primitive = read(pc_file)
     supercell = read(sc_file)
     if matrix:
         transform_matrix = matrix_from_string(matrix)
         if not np.allclose(primitive.cell @ transform_matrix, supercell.cell):
             click.echo('Warning: the super cell and the the primitive cell are not commensure.')
@@ -57,49 +84,75 @@
         transform_matrix = np.rint(tmp)
         if not np.allclose(tmp, transform_matrix):
             click.echo('The super cell and the the primitive cell are not commensure.')
             raise click.Abort()
 
         click.echo(f'(Guessed) Transform matrix:\n{transform_matrix.tolist()}')
 
-    kpoints, _, labels, _ = read_kpoints(kpoints)
+    kpoints, _, labels, _ = read_kpoints(kpoints, code=code)
     click.echo(f'{len(kpoints)} kpoints specified along the path')
 
     unfoldset = UnfoldKSet.from_atoms(transform_matrix,
                                       kpoints,
                                       primitive,
                                       supercell,
                                       time_reversal=time_reversal,
                                       expand=not no_expand,
+                                      dft_code=code,
                                       symprec=symprec)
     unfoldset.kpoint_labels = labels
     try:
         print_symmetry_data(unfoldset)
     except KeyError:
         pass
 
     out_file = Path(out_file)
+    if code == 'vasp':
+        out_kpt_name = f'KPOINTS_{out_file.stem}'
+    elif code == 'castep':
+        out_kpt_name = f'{out_file.stem}_sc_kpoints.cell'
+    else:
+        raise RuntimeError(f'Unknown code: {code}')
+
     if scf_kpoints is not None:
-        scf_kpt, _, _, scf_weights = read_kpoints(scf_kpoints)
-        unfoldset.write_sc_kpoints(f'KPOINTS_{out_file.stem}', nk_per_split=nk_per_split, scf_kpoints_and_weights=(scf_kpt, scf_weights))
+        scf_kpt, _, _, scf_weights = read_kpoints(scf_kpoints, code=code)
+        scf_kpoints_and_weights = (scf_kpt, scf_weights)
     else:
-        unfoldset.write_sc_kpoints(f'KPOINTS_{out_file.stem}', nk_per_split=nk_per_split)
-    click.echo('Supercell kpoints written to KPOITNS_' + out_file.stem)
+        scf_kpoints_and_weights = None
+
+    if Path(out_kpt_name).is_file() and not yes:
+        click.confirm(f'Output file {out_kpt_name} already exists, continue?', abort=True)
+
+    unfoldset.write_sc_kpoints(
+        out_kpt_name,
+        nk_per_split=nk_per_split,
+        scf_kpoints_and_weights=scf_kpoints_and_weights,
+        source=sc_file,
+    )
+
+    click.echo(f'Supercell kpoints written to {out_kpt_name}')
 
     # Serialize the data
+    if Path(out_file).is_file() and not yes:
+        click.confirm(f'Output file {out_file} already exists, continue?', abort=True)
+
     Path(out_file).write_text(unfoldset.to_json(), encoding='utf-8')
 
     click.echo('Unfolding settings written to ' + str(out_file))
 
 
 @easyunfold.group('unfold')
-@click.option('--data-file', default='easyunfold.json', type=click.Path(exists=True, file_okay=True, dir_okay=False))
+@click.option('--data-file', default='easyunfold.json', type=click.Path(exists=True, file_okay=True, dir_okay=False), show_default=True)
 @click.pass_context
 def unfold(ctx, data_file):
-    """Perform unfolding and plotting"""
+    """
+    Perform unfolding and plotting
+
+    There are multiple sub-command available under this command group.
+    """
 
     unfoldset = loadfn(data_file)
     click.echo(f'Loaded data from {data_file}')
     ctx.obj = {'obj': unfoldset, 'fname': data_file}
 
 
 @unfold.command('status')
@@ -124,28 +177,31 @@
         click.echo('Unfolding had been performed - use `unfold plot` to plot the spectral function.')
     else:
         click.echo('Please run the supercell band structure calculation and run `unfold calculate`.')
 
 
 @unfold.command('calculate')
 @click.pass_context
-@click.argument('wavecar', type=click.Path(exists=True, dir_okay=False), nargs=-1)
+@click.argument('wavefunc', type=click.Path(exists=True, dir_okay=False), nargs=-1)
 @click.option('--save-as')
-@click.option('--gamma', is_flag=True)
-@click.option('--ncl', is_flag=True)
-def unfold_calculate(ctx, wavecar, save_as, gamma, ncl):
+@click.option('--gamma', is_flag=True, help='If the calculation is $\\Gamma$-only')
+@click.option('--ncl', is_flag=True, help='If the calculation has non-collinear spins.')
+def unfold_calculate(ctx, wavefunc, save_as, gamma, ncl):
     """
     Perform the unfolding
 
-    Multiple WAVECAR files can be supplied for split-path calculations.
+    Multiple wave function (e.g. the WAVECAR file if using VASP) files can be supplied for
+    split-path calculations.
+    Once the calculation is done, the wave function data are not longer needed as the
+    spectral weights will be stored in the outputs ``json`` file.
     """
     from easyunfold.unfold import UnfoldKSet
 
     unfoldset: UnfoldKSet = ctx.obj['obj']
-    unfoldset.get_spectral_weights(wavecar, gamma, ncl=ncl)
+    unfoldset.get_spectral_weights(wavefunc, gamma, ncl=ncl)
 
     out_path = save_as if save_as else ctx.obj['fname']
     Path(out_path).write_text(unfoldset.to_json(), encoding='utf-8')
     click.echo('Unfolding data written to ' + out_path)
 
 
 def add_plot_options(func):
@@ -153,58 +209,65 @@
     click.option('--gamma', is_flag=True, help='Is the calculation a gamma only one?')(func)
     click.option('--ncl', is_flag=True, help='Is the calculation with non-colinear spin?')(func)
     click.option('--npoints', type=int, default=2000, help='Number of bins for the energy.', show_default=True)(func)
     click.option('--sigma', type=float, default=0.02, help='Smearing width for the energy in ' 'eV.', show_default=True)(func)
     click.option('--eref', type=float, help='Reference energy in eV.')(func)
     click.option('--emin', type=float, default=-5., help='Minimum energy in eV relative to the ' 'reference.', show_default=True)(func)
     click.option('--emax', type=float, default=5., help='Maximum energy in eV relative to the ' 'reference.', show_default=True)(func)
-    click.option('--vscale', type=float, help='A scaling factor for the colour mapping.', default=1.0)(func)
-    click.option('--out-file', default='unfold.png', help='Name of the output file.')(func)
+    click.option('--vscale', type=float, help='A scaling factor for the colour mapping.', default=1.0, show_default=True)(func)
+    click.option('--out-file', default='unfold.png', help='Name of the output file.', show_default=True)(func)
     click.option('--cmap',
                  default='PuRd',
                  help='Name of the colour map(s) to use. Passing a list separated by "|" for the '
                  'combined plot.',
                  show_default=True)(func)
     click.option('--show', is_flag=True, default=False, help='Show the plot interactively.')(func)
     click.option('--no-symm-average',
                  is_flag=True,
                  default=False,
                  help='Do not include symmetry '
                  'related kpoints for '
                  'averaging.',
                  show_default=True)(func)
-    click.option('--procar', multiple=True, help='PROCAR files used for atomic weighting')(func)
+    click.option('--procar',
+                 multiple=True,
+                 help=('PROCAR files used for atomic weighting, '
+                       'can be passed multiple times if more than one PROCAR should be used.'))(func)
     click.option('--atoms-idx', help='Indices of the atoms to be used for weighting (1-indexed).')(func)
     click.option('--orbitals', help='Orbitals of to be used for weighting.')(func)
     click.option('--title', help='Title to be used')(func)
     return func
 
 
 @unfold.command('effective-mass')
 @click.pass_context
-@click.option('--intensity-threshold', type=float, default=0.1, help='Intensity threshold for detecting valid bands.')
-@click.option('--spin', type=int, default=0, help='Index of the spin channel.')
-@click.option('--npoints', type=int, default=3, help='Number of kpoints used for fitting from the extrema.')
-@click.option('--extrema-detect-tol', type=float, default=0.01, help='Tolerance for band extrema detection.')
-@click.option('--degeneracy-detect-tol', type=float, default=0.01, help='Tolerance for band degeneracy detection at extrema.')
-@click.option('--nocc', type=int)
+@click.option('--intensity-threshold', type=float, default=0.1, help='Intensity threshold for detecting valid bands.', show_default=True)
+@click.option('--spin', type=int, default=0, help='Index of the spin channel.', show_default=True)
+@click.option('--npoints', type=int, default=3, help='Number of kpoints used for fitting from the extrema.', show_default=True)
+@click.option('--extrema-detect-tol', type=float, default=0.01, help='Tolerance for band extrema detection.', show_default=True)
+@click.option('--degeneracy-detect-tol',
+              type=float,
+              default=0.01,
+              help='Tolerance for band degeneracy detection at extrema.',
+              show_default=True)
+@click.option('--nocc', type=int, help='DEV: Use this band as the extrema at all kpoints.')
 @click.option('--plot', is_flag=True, default=False)
 @click.option('--plot-fit', is_flag=True, default=False, help='Generate plots of the band edge and parabolic fits.')
-@click.option('--fit-label', help='Which branch to use for plot fitting. e.g. electrons:0', default='electrons:0')
+@click.option('--fit-label', help='Which branch to use for plot fitting. e.g. electrons:0', default='electrons:0', show_default=True)
 @click.option('--band-filter', default=None, type=int, help='Only displace information for this band.')
-@click.option('--out-file', default='unfold-effective-mass.png', help='Name of the output file.')
+@click.option('--out-file', default='unfold-effective-mass.png', help='Name of the output file.', show_default=True)
 def unfold_effective_mass(ctx, intensity_threshold, spin, band_filter, npoints, extrema_detect_tol, degeneracy_detect_tol, nocc, plot,
                           plot_fit, fit_label, out_file):
     """
     Compute and print effective masses by tracing the unfolded weights.
 
     Note that this functionality only works for simple unfolded band structures,
     and it is likely to fail for complex cases.
 
-    Use the `--plot-fit` flag to generate the detected band edge verses the parabolic fit
+    Use the ``--plot-fit`` flag to generate the detected band edge verses the parabolic fit
     for visual confirmation if unsure.
     """
     from easyunfold.effective_mass import EffectiveMass
     from easyunfold.unfold import UnfoldKSet
     from tabulate import tabulate
     unfoldset: UnfoldKSet = ctx.obj['obj']
     efm = EffectiveMass(unfoldset, intensity_tol=intensity_threshold, extrema_tol=extrema_detect_tol, degeneracy_tol=degeneracy_detect_tol)
@@ -279,30 +342,30 @@
 @click.pass_context
 @add_plot_options
 def unfold_plot(ctx, gamma, npoints, sigma, eref, out_file, show, emin, emax, cmap, ncl, no_symm_average, vscale, procar, atoms_idx,
                 orbitals, title):
     """
     Plot the spectral function
 
-    This command uses the stored unfolding data to plot the effective bands structure (EBS).
+    This command uses the stored unfolding data to plot the effective bands structure (EBS) using the spectral function.
     """
     _unfold_plot(ctx, gamma, npoints, sigma, eref, out_file, show, emin, emax, cmap, ncl, no_symm_average, vscale, procar, atoms_idx,
                  orbitals, title)
 
 
 @unfold.command('plot-projections')
 @click.pass_context
 @add_plot_options
 @click.option('--combined/--no-combined', is_flag=True, default=False, help='Plot all projections in a combined graph.')
 @click.option('--intensity', default=1.0, help='Color intensity for combined plot', type=float, show_default=True)
-@click.option('--colors', help='Colors to be used for combined plot. Comma separated. Default = "r,g,b".')
+@click.option('--colors', help='Colors to be used for combined plot, comma separated')
 def unfold_plot_projections(ctx, gamma, npoints, sigma, eref, out_file, show, emin, emax, cmap, ncl, no_symm_average, vscale, procar,
                             atoms_idx, orbitals, title, combined, intensity, colors):
     """
-    Plot with subplots with multiple atomic projections
+    Plot the effective band structure with atomic projections.
     """
     from easyunfold.unfold import UnfoldKSet
     from easyunfold.plotting import UnfoldPlotter
     import matplotlib.pyplot as plt
 
     unfoldset: UnfoldKSet = ctx.obj['obj']
     click.echo(f'Loading projections from: {procar}')
@@ -348,17 +411,15 @@
                  vscale,
                  procar,
                  atoms_idx,
                  orbitals,
                  title,
                  ax=None):
     """
-    Plot the spectral function
-
-    This command uses the stored unfolding data to plot the effective bands structure (EBS).
+    Routine for plotting the spectral function.
     """
     from easyunfold.unfold import UnfoldKSet
     from easyunfold.plotting import UnfoldPlotter
 
     unfoldset: UnfoldKSet = ctx.obj['obj']
     if not unfoldset.is_calculated:
         click.echo('Unfolding has not been performed yet, please run `unfold calculate` command.')
```

### Comparing `easyunfold-0.1.3/easyunfold/effective_mass.py` & `easyunfold-0.1.4/easyunfold/effective_mass.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         for mode in ['cbm', 'vbm']:
             name = 'electrons' if mode == 'cbm' else 'holes'
             outputs[name] = self._get_effective_masses(mode, npoints=npoints, ispin=ispin)
         return outputs
 
     def _get_effective_masses(self, mode: str = 'cbm', ispin: int = 0, npoints: Union[None, int] = None):
         """
-        Workout the effective masses based on the unfolded band structure for CBM or VBM
+        Work out the effective masses based on the unfolded band structure for CBM or VBM
         """
         iks, _, iband = self.get_band_extrema(mode=mode)
         # Override occupations
         if self.nocc:
             iband = [self.nocc for _ in iband]
 
         npoints = self.get_npoints(npoints)
```

### Comparing `easyunfold-0.1.3/easyunfold/plotting.py` & `easyunfold-0.1.4/easyunfold/plotting.py`

 * *Files identical despite different names*

### Comparing `easyunfold-0.1.3/easyunfold/procar.py` & `easyunfold-0.1.4/easyunfold/procar.py`

 * *Files identical despite different names*

### Comparing `easyunfold-0.1.3/easyunfold/unfold.py` & `easyunfold-0.1.4/easyunfold/unfold.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 The main module for unfolding workflow and algorithm
 """
 # pylint: disable=invalid-name,protected-access,too-many-locals
 
 ############################################################
 import re
 from typing import Union, List, Tuple
-from pathlib import Path
 
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.colors import ListedColormap, hex2color
 from monty.json import MSONable
 from monty.serialization import loadfn
 from tqdm import tqdm
 import ase
 import spglib
 
 from easyunfold import __version__
 from .wavecar import Wavecar
 from .procar import Procar
+from .wavefun import VaspWaveFunction, CastepWaveFunction
+from .utils import write_kpoints, reduce_kpoints, wrap_kpoints, kpoints_equal
 
 ############################################################
 
 
 def get_symmetry_dataset(atoms: ase.Atoms, symprec: float = 1e-5):
     """Get the symmetry dataset using spglib"""
     return spglib.get_symmetry_dataset((atoms.get_cell(), atoms.get_scaled_positions(), atoms.get_atomic_numbers()), symprec=symprec)
@@ -42,15 +43,16 @@
 
     where G is a reciprocal space vector of supercell
     """
 
     M = np.array(M)
     Kc = np.dot(k, M.T)
     G = np.array(np.round(Kc), dtype=int)
-    KG = Kc - np.round(Kc)
+    # Wrap to -0.5, 0.5
+    KG = wrap_kpoints(Kc)
 
     return KG, G
 
 
 def rotate_kpt(k: np.ndarray, opt: np.ndarray):
     """
     Apply rotation to a kpoint based on the rotations of the crystals (in the real space)
@@ -126,39 +128,42 @@
                  pc_opts: np.ndarray,
                  sc_opts: np.ndarray,
                  time_reversal: bool = True,
                  expand: bool = True,
                  metadata: Union[None, dict] = None,
                  expansion_results: Union[None, dict] = None,
                  calculated_quantities: Union[None, dict] = None,
-                 kpoint_labels: Union[None, list] = None):
+                 kpoint_labels: Union[None, list] = None,
+                 dft_code='vasp'):
         """
         Instantiate an `UnfoldKSet` object.
 
         :param M: The supercell transformation matrix
         :param kpts_pc: A list of kpoints in the PC
         :param pc_latt: A 3x3 matrix of row lattice vectors of the primitive cell
         :param pc_opts: Symmetry operations of the primitive cell
         :param sc_opts: Symmetry operations of the supercell
         :param expand: Whether to expand the kpoint to take account of broken symmetry or not
         :param expansion_results: Using existing results of symmetry expansion
         :param calculated_quantities: Existing calculated quantities
         :param kpoint_labels: Labels of the kpoints as passed in `pc_latt` as a list of tuples `(<idx>, <label>)`
+        :param dft_code: Name of the DFT code to be used.
         """
         # Basic properties - needed to recreate the object
         self.kpts_pc = kpts_pc
         self.pc_latt = pc_latt
         self.pc_opts = pc_opts
         self.sc_opts = sc_opts
         self.expand = expand
         self.M = M
         self.expansion_results = expansion_results
         self.time_reversal = time_reversal
         self.calculated_quantities = {} if not calculated_quantities else calculated_quantities
         self.kpoint_labels = kpoint_labels
+        self.dft_code = dft_code
         if metadata is None:
             metadata = {}
         self.metadata = metadata
         self.metadata['program_version'] = __version__
         self.transient_quantities = {}
 
         # Transient properties
@@ -174,22 +179,25 @@
 
     @property
     def has_averaged_spectral_weights(self) -> bool:
         """Return True if the spectral weights stored is averaged"""
         return self.calculated_quantities.get('spectral_weights_is_averaged', False)
 
     @classmethod
-    def from_atoms(cls,
-                   M: np.ndarray,
-                   kpts_pc: list,
-                   pc: ase.Atoms,
-                   sc: ase.Atoms,
-                   time_reversal: bool = True,
-                   expand=True,
-                   symprec: float = 1e-5):
+    def from_atoms(
+        cls,
+        M: np.ndarray,
+        kpts_pc: list,
+        pc: ase.Atoms,
+        sc: ase.Atoms,
+        time_reversal: bool = True,
+        expand=True,
+        symprec: float = 1e-5,
+        dft_code='vasp',
+    ):
         """
         Initialise from primitive cell and supercell atoms
 
         :param M: The supercell transformation matrix
         :param kpts_pc: A list of kpoints in the PC
         :param pc: Primitive cell structure
         :param sc: Supercell structure
@@ -208,14 +216,15 @@
             sc_opts=sc_symm_data['rotations'],
             time_reversal=time_reversal,
             expand=expand,
             metadata={
                 'symmetry_dataset_pc': pc_symm_data,
                 'symmetry_dataset_sc': sc_symm_data,
             },
+            dft_code=dft_code,
         )
 
     @classmethod
     def from_file(cls, fname: str):
         """Load from a file"""
         return loadfn(fname)
 
@@ -261,43 +270,52 @@
 
     def generate_sc_kpoints(self) -> None:
         """
         Generate the supercell kpoints to be calculated.
         Results are stored into `self.expansion_results`.
         """
 
-        assert bool(self.expansion_results)
+        assert self.expansion_results
         expended_sc = []
         all_sc = []
         # Find the SC kpoint for each PC kpoint
         for kset in self.expansion_results['kpoints']:
             this_k = []
             for kpt in kset:
                 sc_k, _ = find_K_from_k(kpt, self.M)
                 this_k.append(sc_k)
             expended_sc.append(this_k)
+            # A flat list containing all SC
             all_sc.extend(this_k)
+
         # We now have bunch of supercell kpoints for each set of expanded kpoints
         # Try to find duplicated SC kpoints
-        reduced_sckpts, sc_kpts_map = remote_duplicated_kpoints(all_sc, return_map=True)
+        # TODO: We can further reduce this by time-reversal symmetry here
+        all_sc = np.array(all_sc)
+        reduced_sckpts, _, sc_kpts_map = reduce_kpoints(all_sc, time_reversal=self.time_reversal)
         sc_kpts_map = list(sc_kpts_map)
 
-        # Mapping between the pckpts to the redcued sckpts
+        # Mapping between the pckpts to the reduced sckpts
+        # Collect from form nested list containing the mappings to the reduce sc kpoints
         reduced_sc_map = []
         for sc_set in expended_sc:
             map_indx = []
             for _ in sc_set:
                 map_indx.append(sc_kpts_map.pop(0))
             reduced_sc_map.append(map_indx)
 
         self.expansion_results['reduced_sckpts'] = reduced_sckpts
         self.expansion_results['reduced_sckpts_map'] = reduced_sc_map
         # A nested list that stores the indices of the sc kpts in the reduced_sckpts list
 
-    def write_sc_kpoints(self, file: str, nk_per_split: Union[None, list] = None, scf_kpoints_and_weights: Union[None, list] = None):
+    def write_sc_kpoints(self,
+                         file: str,
+                         nk_per_split: Union[None, list] = None,
+                         scf_kpoints_and_weights: Union[None, list] = None,
+                         **kwargs):
         """
         Write the supercell kpoints to a file.
 
         :param file: Name of the file
         :param nk_per_split: Number of kpoints per split along the path
         :param scf_kpoints_and_weights: SCF kpoint and their weights needed for split-path calculations
         """
@@ -306,44 +324,52 @@
         kpoints = np.asarray(self.expansion_results['reduced_sckpts'])
         weights = None
         if nk_per_split is None:
             if scf_kpoints_and_weights:
                 # Prepend with SCF kpoints
                 kpoints, weights = concatenate_scf_kpoints(scf_kpoints_and_weights[0], scf_kpoints_and_weights[1], kpoints)
 
-            write_kpoints(kpoints, file, comment='supercell kpoints', weights=weights)
+            write_kpoints(kpoints, file, comment='supercell kpoints', weights=weights, code=self.dft_code, **kwargs)
         else:
             splits = [kpoints[i:i + nk_per_split] for i in range(0, kpoints.shape[0], nk_per_split)]
             for i_spilt, kpt in enumerate(splits):
                 if scf_kpoints_and_weights:
                     kpt, weights = concatenate_scf_kpoints(scf_kpoints_and_weights[0], scf_kpoints_and_weights[1], kpt)
-                write_kpoints(kpt, f'{file}_{i_spilt + 1:03d}', f'supercell kpoints split {i_spilt + 1}', weights)
+                write_kpoints(kpt,
+                              f'{file}_{i_spilt + 1:03d}',
+                              f'supercell kpoints split {i_spilt + 1}',
+                              code=self.dft_code,
+                              weights=weights,
+                              **kwargs)
 
-    def write_pc_kpoints(self, file: str, expanded: bool = False):
+    def write_pc_kpoints(self, file: str, expanded: bool = False, **kwargs):
         """Write the primitive cell kpoints"""
         if expanded:
             all_pc = []
             for tmp in self.expansion_results['kpoints']:
                 all_pc.extend(tmp)
-            write_kpoints(all_pc, file, comment='expanded primitive cell kpoints')
         else:
-            write_kpoints(self.kpts_pc, file, comment='primitive cell kpoints')
+            all_pc = self.kpts_pc
+        write_kpoints(all_pc, file, comment='expanded primitive cell kpoints', code=self.dft_code, **kwargs)
 
-    def _read_weights(self, wavecar: Union[str, List[str]], gamma: bool, ncl: bool, gamma_half: str):
+    def _read_weights(self, wavefunction: Union[str, List[str]], gamma: bool, ncl: bool, gamma_half: str):
         """
-        Read the weights from the wavecar for all kpoints
+        Read the weights from the wave function files for all kpoints
 
         Returns the averaged weights and the original weights per set of kpoints
         """
         weights_per_set = []
         averaged_weights = []
-        if not isinstance(wavecar, (list, tuple)):
-            wavecar = [wavecar]
-        # Load the WAVECAR unfold objects
-        unfold_objs = [Unfold(self.M, name, gamma=gamma, lsorbit=ncl, gamma_half=gamma_half) for name in wavecar]
+        if not isinstance(wavefunction, (list, tuple)):
+            wavefunction = [wavefunction]
+        # Load the unfold objects
+        unfold_objs = [
+            Unfold(self.M, name, gamma=gamma, lsorbit=ncl, gamma_half=gamma_half, dft_code=self.dft_code, time_reversal=self.time_reversal)
+            for name in wavefunction
+        ]
         # Record the VBM and the CBM values
         varray = np.array([obj.get_vbm_cbm() for obj in unfold_objs])
         self.calculated_quantities['vbm'] = float(varray[:, 0].max())
         self.calculated_quantities['cbm'] = float(varray[:, 1].min())
         # Read the spectral weights for each set of expanded kpoints
         for kset, weights in tqdm(zip(self.expansion_results['kpoints'], self.expansion_results['weights']),
                                   desc='kpt',
@@ -368,14 +394,15 @@
         if self.procars and not force:
             pass
 
         if not isinstance(procar, (tuple, list)):
             procar = [procar]
 
         # Load the procars
+        # Note that this method should be generalised for non-VASP as well.
         self.transient_quantities['procars'] = [Procar(path) for path in procar]
         # Construct mapping from the primitive cell kpoints to those in the PROCAR
         self.transient_quantities['procars_kmap'] = self._construct_procar_kmap()
 
     def _construct_procar_kmap(self) -> list:
         """Construct mapping from the set of kpoints to that in the PROCAR"""
         ksets = self.expansion_results['kpoints']
@@ -385,15 +412,15 @@
             for kpoint in kset:
                 # Find the supercell kpoint
                 K_super, _ = find_K_from_k(kpoint, self.M)
                 # Search for kpoints in the procar
                 found = False
                 for iprocar, procar in enumerate(self.procars):
                     for ikpt, kprocar in enumerate(procar.kvecs[0]):
-                        if np.allclose(K_super, kprocar):
+                        if kpoints_equal(K_super, kprocar, time_reversal=self.time_reversal):
                             kidx_procar_sets[-1].append([iprocar, ikpt])
                             found = True
                             break
                     if found:
                         break
                 if found is False:
                     raise ValueError(f'Cannot found kpoint {K_super} in PROCAR files')
@@ -406,15 +433,15 @@
 
     @property
     def procar_kmaps(self):
         """Loaded PROCAR kpoint mapping"""
         return self.transient_quantities.get('procars_kmap')
 
     def _get_spectral_weights(self,
-                              wavecar,
+                              wavefunction,
                               npoints=2000,
                               sigma=0.01,
                               emin=None,
                               emax=None,
                               gamma=False,
                               ncl=False,
                               gamma_half='x',
@@ -425,20 +452,20 @@
         """
         Fetch spectral weights from a wavecar and compute spectral function is requested
 
         Args:
 
             atomic_projects (tuple): A tuple of atoms and orbitals whose projected weights should be used.
         """
-        # If WAVECAR is given - reload from the data
-        if wavecar:
-            self._read_weights(wavecar, gamma=gamma, ncl=ncl, gamma_half=gamma_half)
+        # If wave function is given - reload from the data
+        if wavefunction:
+            self._read_weights(wavefunction, gamma=gamma, ncl=ncl, gamma_half=gamma_half)
         else:
             if not self.is_calculated:
-                raise RuntimeWarning('The spectral weights need to be calculated first - please pass the WAVECAR file(s).')
+                raise RuntimeWarning('The spectral weights need to be calculated first - please pass the wave function file(s).')
 
         # Use existing results
         if symm_average:
             sws = self.calculated_quantities['spectral_weights_per_set']
             kweight_sets = self.expansion_results['weights']
         else:
             # No averaging - we just return the first item of each set, which is the weight of the original set
@@ -494,73 +521,78 @@
             # Search
             for iprocar, kidx in kset:
                 band_weight = projs[iprocar][:, kidx]
                 band_weight_sets[-1].append(band_weight)
         return band_weight_sets
 
     def get_spectral_function(self,
-                              wavecar: Union[None, Wavecar] = None,
+                              wavefunction: Union[None, List[str]] = None,
                               npoints: int = 2000,
                               sigma: float = 0.1,
                               gamma: bool = False,
                               ncl: bool = False,
                               gamma_half: str = 'x',
                               symm_average: bool = True,
                               atoms_idx: Union[None, List[int]] = None,
                               orbitals: Union[None, str, List[str]] = None):
         """
         Compute and return the spectral function
 
-        :param wavecar: The WAVECAR files to be used
+        :param wavecar: The wavefunction files to be used
         :param npoints: Number of points for the energy axis
         :param sigma: Smearing width for the Gaussian smearing
         :param gamma: Need to be set to `True` for Gamma-only calculation
         :param ncl: Need to be set to `True` for non-collinear magnetism calculation
         :param gamma_half: Flag used for reading WAVECAR
         :param symm_average: Whether to perform symmetry averaging
         :param atoms_idx: Indices for the atoms for projection
         :param orbitals: Indices for the atoms for projection
 
         :returns: A tuple of the energies and the spectral functioin.
         """
-        _, e0, spectral_function = self._get_spectral_weights(wavecar,
+        _, e0, spectral_function = self._get_spectral_weights(wavefunction,
                                                               npoints=npoints,
                                                               sigma=sigma,
                                                               gamma=gamma,
                                                               ncl=ncl,
                                                               gamma_half=gamma_half,
                                                               also_spectral_function=True,
                                                               atoms_idx=atoms_idx,
                                                               orbitals=orbitals,
                                                               symm_average=symm_average)
         return e0, spectral_function
 
-    def get_spectral_weights(self, wavecar=None, gamma: bool = False, ncl: bool = False, gamma_half: str = 'x', symm_average: bool = True):
+    def get_spectral_weights(self,
+                             wavefunction=None,
+                             gamma: bool = False,
+                             ncl: bool = False,
+                             gamma_half: str = 'x',
+                             symm_average: bool = True):
         """
         Return the spectral weights calculated
 
-        :param wavecar: The WAVECAR file(s) for calculation. Not need if the weights has been calculated.
-        :param gamma: Whether the WAVECAR files are from $\\Gamma$-only calculation.
+        :param wavefunction: The wavefunction file(s) for calculation. Not need if the weights has been calculated.
+        :param gamma: Whether the wavefunction files are from $\\Gamma$-only calculation.
 
         :returns: An array storing the spectral weights.
 
         """
-        return self._get_spectral_weights(wavecar=wavecar,
+        return self._get_spectral_weights(wavefunction=wavefunction,
                                           gamma=gamma,
                                           ncl=ncl,
                                           gamma_half=gamma_half,
                                           also_spectral_function=False,
                                           symm_average=symm_average)
 
     def as_dict(self) -> dict:
         """Convert the object into a dictionary representation"""
         output = {'@module': self.__class__.__module__, '@class': self.__class__.__name__, '@version': __version__}
         for key in [
                 'M', 'kpts_pc', 'pc_latt', 'pc_opts', 'sc_opts', 'expansion_results', 'time_reversal', 'calculated_quantities',
-                'kpoint_labels', 'expand', 'metadata'
+                'kpoint_labels', 'expand', 'metadata', 'dft_code'
         ]:
             output[key] = getattr(self, key)
         return output
 
     def get_kpoint_distances(self):
         """
         Distances between the kpoints along the path in the reciprocal space.
@@ -596,17 +628,19 @@
         \Delta(x) = \lim_{\sigma\to 0} Gaussian
     $$
     """
 
     return 1. / (np.sqrt(2 * np.pi) * sigma) * np.exp(-(x - x0)**2 / (2 * sigma**2))
 
 
-def remote_duplicated_kpoints(kpoints: list, return_map=False, decimals=6):
+def remove_duplicated_kpoints(kpoints: list, return_map=False, decimals=6):
     """
     remove duplicate kpoints in the list.
+
+    TODO: improve this implementation by clipping the range of the fractional coorindates
     """
     kpoints = np.asarray(kpoints)
     _, kid, inv_kid = np.unique(
         np.round(kpoints, decimals),
         axis=0,
         return_index=True,
         return_inverse=True,
@@ -614,109 +648,14 @@
     reducedK = kpoints[kid]
 
     if return_map:
         return reducedK, inv_kid
     return reducedK
 
 
-def write_kpoints(kpoints: Union[np.ndarray, list], outpath: str = 'KPOINTS', comment: str = '', weights: Union[None, List[float]] = None):
-    """
-    Write kpoints to VASP KPOINTS file
-
-    :param kpoints: A list of kpoints to be written
-    :param outpath: Path to the output file
-    :param comments: Comments to be put into the `KPOINTS` file
-    :param weights: If given, the weighting of the kpoints, otherwise all kpoints are equal weighted.
-    """
-    kpoints = np.asarray(kpoints)
-    nkpts = kpoints.shape[0]
-
-    with open(outpath, 'w', encoding='utf-8') as vaspkpt:
-        vaspkpt.write(comment + '\n')
-        vaspkpt.write(f'{nkpts}\n')
-        vaspkpt.write('Rec\n')
-        for ik in range(nkpts):
-            if weights is not None:
-                line = f'  {kpoints[ik, 0]:12.8f} {kpoints[ik, 1]:12.8f} {kpoints[ik,2]:12.8f}  {weights[ik]:12.8f}\n'
-            else:
-                line = f'  {kpoints[ik, 0]:12.8f} {kpoints[ik, 1]:12.8f} {kpoints[ik,2]:12.8f}  1.0\n'
-            vaspkpt.write(line)
-
-
-def read_kpoints(path='KPOINTS'):
-    """
-    Read kpoints from a KPOINTS file containing reciprocal space coordinates (fractional)
-
-    :returns: The kpoints, the comment, the labels, and the weights at each kpoint.
-    """
-    content = Path(path).read_text(encoding='utf-8').split('\n')
-    comment = content[0]
-    nkpts = int(content[1])
-    if content[2].lower().startswith('lin'):
-        return read_kpoints_line(content)
-    assert content[2].lower().startswith('rec'), 'Only Reciprocal space KPOINT file is supported'
-    kpts = []
-    labels = []
-    weights = []
-    ik = 0
-    for line in content[3:]:
-        tokens = line.split()
-        this_kpt = [float(value) for value in tokens[:3]]
-        weights.append(float(tokens[3]))
-
-        if len(tokens) >= 5:
-            labels.append([ik, tokens[4]])
-
-        kpts.append(this_kpt)
-        ik += 1
-        if ik == nkpts:
-            break
-    return kpts, comment, labels, weights
-
-
-def read_kpoints_line(content, density=20):
-    """
-    Read kpoints in the VASP KPOINTS file line mode
-
-    Resolve to explicit kpoints
-
-    :returns: The kpoints, the comment, the labels, and the weights at each kpoint
-    """
-    comment = content[0]
-    density = int(content[1]) if content[1] else density
-
-    assert content[2].lower().startswith('lin'), 'Only Line mode KPOINT file is supported'
-    assert content[3].lower().startswith('rec'), 'Only Reciprocal coorindates are supported!'
-
-    segs = []
-    labels = []
-    for line in content[4:]:
-        tokens = line.split()
-        if not tokens:
-            continue
-        point = [float(x) for x in tokens[:3]]
-        labels.append(tokens[-1])
-        segs.append(point)
-    # Process the segments
-    kpoints = []
-    labels_loc = []
-    for i in range(int(len(segs) / 2)):
-        k1 = segs[i * 2]
-        k2 = segs[i * 2 + 1]
-        # Check for duplicate end point
-        if kpoints and kpoints[-1] == k1:
-            kpoints.pop()
-            labels_loc.pop()
-        this_seg = np.linspace(k1, k2, density)
-        labels_loc.append((len(kpoints), labels[i]))
-        kpoints.extend(this_seg.tolist())
-        labels_loc.append((len(kpoints) - 1, labels[i + 1]))
-    return kpoints, comment, labels_loc, None
-
-
 def make_kpath(kbound: List[float], nseg=40):
     """
     Return a list of kpoints defining the path between the given kpoints.
     """
     kbound = np.array(kbound, dtype=float)
     kdist = np.diff(kbound, axis=0)
 
@@ -783,27 +722,35 @@
                                                 axis=1) * kweight
     return e0, spectral_function
 
 
 ############################################################
 
 
-class Unfold():
+class Unfold:
     """
-    Low lever interface for performing unfolding related calculations.
+    Low level interface for performing unfolding related calculations.
     obtain the effective band structure (EBS).
 
     :::{admonition} Reference
     "Extracting E versus k effective band structure from supercell
      calculations on alloys and impurities"
     Phys. Rev. B 85, 085201 (2012)
     :::
     """
 
-    def __init__(self, M=None, wavecar: str = 'WAVECAR', gamma: bool = False, lsorbit: bool = False, gamma_half: str = 'x', verbose=False):
+    def __init__(self,
+                 M=None,
+                 fname: str = 'WAVECAR',
+                 gamma: bool = False,
+                 lsorbit: bool = False,
+                 gamma_half: str = 'x',
+                 verbose=False,
+                 time_reversal=False,
+                 dft_code='vasp'):
         """
         Initialization.
 
         M is the transformation matrix between supercell and primitive cell:
 
         ```python
         M = np.dot(A, np.linalg.inv(a))
@@ -817,57 +764,60 @@
         ```
 
         Whereas in reciprocal space
 
         ```python
         b = np.dot(M.T, B);    B = np.dot(np.linalg.inv(M).T, b)
         ```
-
-        wavecar is the location of VASP WAVECAR file that contains the
-        wavefunction information of a supercell calculation.
         """
 
         # Whether the WAVECAR is a gamma-only version
-        self._lgam = gamma
-        self._lsoc = lsorbit
+        self._lgam = gamma  # Applicable only for VASP
+        self._lsoc = lsorbit  # Applicable only for VASP
+
+        self.time_reversal = time_reversal
 
         self.M = np.array(M, dtype=float)
         assert self.M.shape == (3, 3), 'Shape of the tranformation matrix must be (3,3)'
-
-        self.wfc = Wavecar(wavecar, lsorbit=self._lsoc, lgamma=self._lgam, gamma_half=gamma_half)
+        if dft_code == 'vasp':
+            self.wfc = VaspWaveFunction(Wavecar(fname, lsorbit=self._lsoc, lgamma=self._lgam, gamma_half=gamma_half))
+        elif dft_code == 'castep':
+            self.wfc = CastepWaveFunction.from_file(fname)
+        else:
+            raise NotImplementedError(f'Code {dft_code} has not being implemented!')
         # all the K-point vectors
-        self.kvecs = self.wfc._kvecs
+        self.kvecs = self.wfc.kpoints
         # all the KS energies in shape (ns, nk, nb)
-        self.bands = self.wfc._bands
+        self.bands = self.wfc.bands
 
         # spectral weight for all the kpoints
         self.SW = None
 
         self.verbose = verbose
 
     def get_vbm_cbm(self, thresh: float = 1e-8) -> Tuple[float, float]:
-        """Locate the VBM from the WAVECAR"""
-        occ = self.wfc._occs
+        """Locate the VBM from the wave function data"""
+        occ = self.wfc.occupancies
 
         occupied = np.abs(occ) > thresh
         vbm = float(self.bands[occupied].max())
         cbm = float(self.bands[~occupied].min())
         return vbm, cbm
 
     def get_ovlap_G(self, ikpt: int = 1, epsilon: float = 1E-5) -> Tuple[np.ndarray, np.ndarray]:
         """
         Get subset of the reciprocal space vectors of the supercell,
         specifically the ones that match the reciprocal space vectors of the
         primitive cell.
         """
 
-        assert 1 <= ikpt <= self.wfc._nkpts, 'Invalid K-point index!'
+        assert 1 <= ikpt <= self.wfc.nkpts, 'Invalid K-point index!'
 
         # Reciprocal space vectors of the supercell in fractional unit
-        Gvecs = self.wfc.get_gvectors(ikpt=ikpt)
+        Gvecs = self.wfc.get_gvectors(ik=ikpt)
 
         if self._lgam:
             nplw = Gvecs.shape[0]
             tmp = np.zeros((nplw * 2 - 1, 3), dtype=int)
             # the gvectors of Gamma version only contains half the number of a
             # normal version.
             tmp[:nplw, ...] = Gvecs
@@ -883,19 +833,23 @@
         gd = gvecs - np.round(gvecs)
         match = np.alltrue(np.abs(gd) < epsilon, axis=1)
 
         return Gvecs[match], Gvecs
 
     def find_K_index(self, K0: np.ndarray) -> int:
         """
-        Find the index of a point `K0`.
+        Find the (one-based) index of a point `K0`.
         """
-
-        for ii in range(self.wfc._nkpts):
-            if np.alltrue(np.abs(self.wfc._kvecs[ii] - K0) < 1E-5):
+        kpts_wrapped = wrap_kpoints(self.wfc.kpoints)
+        K0_wrapped = wrap_kpoints(K0)
+        for ii in range(self.wfc.nkpts):
+            if np.alltrue(np.abs(kpts_wrapped[ii] - K0_wrapped) < 1E-5):
+                return ii + 1
+            # Check for kpoint related with time-reversal symmetry
+            if self.time_reversal and np.alltrue(np.abs(kpts_wrapped[ii] + K0_wrapped) < 1E-5):
                 return ii + 1
         raise ValueError('Cannot find the corresponding K-points in WAVECAR!')
 
     def k2K_map(self, kpath) -> List[int]:
         """
         Return the map from primitive-cell k-points to supercell k-points.
         """
@@ -928,47 +882,47 @@
 
         # get the overlap G-vectors
         Gvalid, Gall = self.get_ovlap_G(ikpt=ikpt)
         # Gnew = Gvalid + k0 - K0
         Goffset = Gvalid + G0[np.newaxis, :]
 
         # Index of the Gvalid in 3D grid
-        GallIndex = Gall % self.wfc._ngrid[np.newaxis, :]
-        GoffsetIndex = Goffset % self.wfc._ngrid[np.newaxis, :]
+        GallIndex = Gall % self.wfc.mesh_size[np.newaxis, :]
+        GoffsetIndex = Goffset % self.wfc.mesh_size[np.newaxis, :]
 
         # 3d grid for planewave coefficients
-        wfc_k_3D = np.zeros(self.wfc._ngrid, dtype=np.complex128)
+        wfc_k_3D = np.zeros(self.wfc.mesh_size, dtype=np.complex128)
 
         # the weights and corresponding energies
-        P_Km = np.zeros(self.wfc._nbands, dtype=float)
-        E_Km = np.zeros(self.wfc._nbands, dtype=float)
+        P_Km = np.zeros(self.wfc.nbands, dtype=float)
+        E_Km = np.zeros(self.wfc.nbands, dtype=float)
 
-        for nb in range(self.wfc._nbands):
+        for nb in range(self.wfc.nbands):
             # initialize the array to zero, which is unnecessary since the
             # GallIndex is the same for the same K-point
             # wfc_k_3D[:,:,:] = 0.0
 
             if self._lsoc:
                 # pad the coefficients to 3D grid
-                band_coeff = self.wfc.read_band_coeffs(ispin=whichspin, ikpt=ikpt, iband=nb + 1, norm=True)
+                band_coeff = self.wfc.get_band_coeffs(ispin=whichspin, ik=ikpt, ib=nb + 1, norm=True)
                 nplw = band_coeff.shape[0] // 2
                 band_spinor_coeff = [band_coeff[:nplw], band_coeff[nplw:]]
 
                 # energy
                 E_Km[nb] = self.bands[whichspin - 1, ikpt - 1, nb]
                 for Ispinor in range(2):
                     # band = band_spinor_coeff[Ispinor]
                     # band /= np.linalg.norm(band)
                     wfc_k_3D[GallIndex[:, 0], GallIndex[:, 1], GallIndex[:, 2]] = band_spinor_coeff[Ispinor]
 
                     # spectral weight
                     P_Km[nb] += np.linalg.norm(wfc_k_3D[GoffsetIndex[:, 0], GoffsetIndex[:, 1], GoffsetIndex[:, 2]])**2
             else:
                 # pad the coefficients to 3D grid
-                band_coeff = self.wfc.read_band_coeffs(ispin=whichspin, ikpt=ikpt, iband=nb + 1, norm=True)
+                band_coeff = self.wfc.get_band_coeffs(ispin=whichspin, ik=ikpt, ib=nb + 1, norm=True)
                 if self._lgam:
                     nplw = band_coeff.size
                     tmp = np.zeros((nplw * 2 - 1), dtype=band_coeff.dtype)
                     # for Gamma version, the coefficients corresponding to G \ne 0
                     # is multiplied by a factor of sqrt(2)
                     band_coeff[1:] /= np.sqrt(2.)
                     tmp[:nplw] = band_coeff
@@ -987,16 +941,16 @@
         """
         Calculate the spectral weight for a list of kpoints in the primitive BZ.
         """
 
         NKPTS = len(kpoints)
 
         sw = []
-        for ispin in range(self.wfc._nspin):
-            if self.wfc._nspin == 2:
+        for ispin in range(self.wfc.nspins):
+            if self.wfc.nspins == 2:
                 if self.verbose:
                     print('#' * 60)
                     print(f'Spin component: {ispin}')
                     print('#' * 60)
             sw.append([self.spectral_weight_k(kpoints[ik], whichspin=ispin + 1) for ik in range(NKPTS)])
 
         self.SW = np.array(sw)
@@ -1013,15 +967,15 @@
 
         Where the $\Delta$ function can be approximated by Lorentzian or Gaussian
         function.
         """
 
         assert self.SW is not None, 'Spectral weight must be calculated first!'
 
-        NS = self.wfc._nspin
+        NS = self.wfc.nspins
         # Number of kpoints
         nk = self.SW.shape[1]
         # spectral function
         SF = np.zeros((NS, nedos, nk), dtype=float)
 
         emin = self.SW[:, :, :, 0].min()
         emax = self.SW[:, :, :, 0].max()
@@ -1036,24 +990,25 @@
                                           axis=1)
         return e0, SF
 
 
 def spectral_weight_multiple_source(kpoints: list, unfold_objs: List[Unfold], transform_matrix: np.ndarray):
     """
     Calculate the spectral weight for a list of kpoints in the primitive BZ
-    from a list of `WAVECARs`.
+    from a list of wave function files.
     """
 
     nk = len(kpoints)
-    ns = unfold_objs[0].wfc._nspin
+    ns = unfold_objs[0].wfc.nspins
     for obj in unfold_objs[1:]:
-        assert ns == obj.wfc._nspin
+        assert ns == obj.wfc.nspins
 
-    # When reading from multiple WAVECAR, it is possible that each of them may have differnt number of bands
-    # if so, we take only the first N bands, where N is the minimum values of bands
+    # When reading from multiple wave function files (e.g. WAVECAR for VASP),
+    # it is possible that each of them may have differnt number of bands.
+    # Ff so, we take only the first N bands, where N is the minimum values of bands
     nb = []
     for source in unfold_objs:
         nb.append(source.bands.shape[2])
     nbands = min(nb)
 
     spectral_weights = []
     for ispin in range(ns):
@@ -1069,15 +1024,15 @@
                 except ValueError:
                     continue
                 sw_this_spin.append(source.spectral_weight_k(this_k, whichspin=ispin + 1)[:nbands, :])
                 ok = True
                 break
 
             if not ok:
-                raise ValueError(f'This kpoint {this_k} this not found in the WAVECAR(s) provided')
+                raise ValueError(f'This kpoint {this_k_supercell} (PC:{this_k}) this not found in the wave function data provided')
 
         spectral_weights.append(sw_this_spin)
 
     return np.array(spectral_weights)
 
 
 def concatenate_scf_kpoints(scf_kpts: list, scf_weights: list, kpoints: list):
```

### Comparing `easyunfold-0.1.3/easyunfold/vasp_constant.py` & `easyunfold-0.1.4/easyunfold/vasp_constant.py`

 * *Files identical despite different names*

### Comparing `easyunfold-0.1.3/easyunfold/wavecar.py` & `easyunfold-0.1.4/easyunfold/wavecar.py`

 * *Files identical despite different names*

### Comparing `easyunfold-0.1.3/pyproject.toml` & `easyunfold-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
-dependencies = ["scipy", "numpy", "matplotlib", "ase", "spglib", "click", "monty", "tqdm", "tabulate", "colormath"]
+dependencies = ["scipy~=1.0", "numpy~=1.0", "matplotlib~=3.0", "ase~=3.14", "spglib~=2.0", "click", "monty", "tqdm~=4.0",
+                "tabulate~=0.8", "colormath~=3.0",
+                "castepxbin~=0.3.0", "castepinput~=0.1"]
 
 [project.urls]
 "Homepage" = "https://github.com/SMTG-UCL/easyunfold"
 "Documentation" = "https://smtg-ucl.github.io/easyunfold/"
 
 [project.scripts]
 easyunfold = "easyunfold.cli:easyunfold"
```

### Comparing `easyunfold-0.1.3/PKG-INFO` & `easyunfold-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: easyunfold
-Version: 0.1.3
+Version: 0.1.4
 Summary: Collection of code for band unfolding
 Author-email: Bonan Zhu <zhubonan@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: scipy
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: ase
-Requires-Dist: spglib
+Requires-Dist: scipy~=1.0
+Requires-Dist: numpy~=1.0
+Requires-Dist: matplotlib~=3.0
+Requires-Dist: ase~=3.14
+Requires-Dist: spglib~=2.0
 Requires-Dist: click
 Requires-Dist: monty
-Requires-Dist: tqdm
-Requires-Dist: tabulate
-Requires-Dist: colormath
+Requires-Dist: tqdm~=4.0
+Requires-Dist: tabulate~=0.8
+Requires-Dist: colormath~=3.0
+Requires-Dist: castepxbin~=0.3.0
+Requires-Dist: castepinput~=0.1
 Requires-Dist: sphinx-click>=4,<5 ; extra == "doc"
 Requires-Dist: sphinx-autodoc2>=0.4,<0.5 ; extra == "doc"
 Requires-Dist: sphinx-book-theme>=1,<2 ; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.3,<0.4 ; extra == "doc"
 Requires-Dist: myst-parser[linkify] ; extra == "doc"
 Requires-Dist: sphinx>=6,<7 ; extra == "doc"
 Requires-Dist: pytest ; extra == "test"
@@ -32,15 +34,15 @@
 Provides-Extra: test
 
 # Easyunfold
 
 
 ![build](https://github.com/SMTG-UCL/easyunfold/actions/workflows/ci.yaml/badge.svg)
 [![docs](https://github.com/SMTG-UCL/easyunfold/actions/workflows/docs.yaml/badge.svg)](https://smtg-ucl.github.io/easyunfold/)
-[![codecov](https://codecov.io/gh/SMTG-UCL/easyunfold/branch/dev/graph/badge.svg?token=XLLWWU5UM2)](https://codecov.io/gh/SMTG-UCL/easyunfold)
+[![codecov](https://codecov.io/gh/SMTG-UCL/easyunfold/branch/main/graph/badge.svg?token=XLLWWU5UM2)](https://codecov.io/gh/SMTG-UCL/easyunfold)
 
 ![easyunfold](docs/img/logo.svg)
 
 Documentation: https://smtg-ucl.github.io/easyunfold/
 
 This package is intended for obtaining the effective band structure of a supercell for a certain path of the primitive cell.
 It was originally based on [PyVaspwfc](https://github.com/QijingZheng/VaspBandUnfolding) for reading wavefunction output of VASP, and contains some code of the latter.
```

