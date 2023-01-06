# PolyBin
PolyBin estimates the binned power spectrum, bispectrum, and trispectrum for full-sky HEALPix maps such as the CMB, using the algorithms of [Philcox 2023](TODO). For each statistic, two estimators are available: the standard (ideal) estimators, which do not take into account the mask, and window-deconvolved estimators. In the second case, we require computation of a Fisher matrix; this depends on binning and the mask, but does not need to be recomputed for each new simulation. For the trispectra, we can compute both the *parity-even* and *parity-odd* components.

PolyBin contains the following modules:
- `pspec`: Binned (auto) power spectra
- `bspec`: Binned (auto) bispectra
- `tspec`: Binned (auto) parity-even and parity-odd trispectra

Other functions can straightforwardly be added!

## Usage
See the [Tutorial](Tutorial.ipynb)

### Authors
- [Oliver Philcox](mailto:ohep2@cantab.ac.uk) (Columbia / Simons Foundation)

### Dependencies
- Python 2/3
- healpy
- pywigxjpf
- fitsio
- tqdm
