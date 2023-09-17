PLAsTiCC Astronomical Classification competition on Kaggle: https://www.kaggle.com/c/PLAsTiCC-2018

Features to extract from time-series data:
- Number of peaks
- Derivatives: max slope, min slope
- Range (normalized)
- STD normalized
- Fraction of `detected` data points for the object
- Weighted mean
- Normalized flux STD
- Normalized amplitude (range)
- Normalized MAD (median of deviation)
- Fraction of data points beyond 1 STD
- Skew (spstat.skew) for `flux`

What else could be done:
- different models for galactic vs extragalactic (by `redshift`)
- different models for `ddf` = 1 vs `ddf` = 0
- different models for `redshift` bins
- different models for `hostgal_photoz` = 0 and `hostgal_photoz` != 0
- for `hostgal_photoz` > 2 -> replace by median value
- use logarithms for `hostgal_photoz`, `hostgal_photoz_err`, `mwebv`
- convert `flux` to magnitude (-2.5*log10(`flux`)), use all datapoints regardless of `detected` value
