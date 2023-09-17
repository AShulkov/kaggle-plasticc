PLAsTiCC Astronomical Classification competition on Kaggle: https://www.kaggle.com/c/PLAsTiCC-2018

What else could be done:
- two different classifiers for `hostgal_photoz` = 0 and `hostgal_photoz` != 0
- for `hostgal_photoz` > 2 -> replace by median value
- use logarithms for `hostgal_photoz`, `hostgal_photoz_err`, `mwebv`
- convert `flux` to magnitude, use all datapoints regardless of `detected` value

Possible additional feature engineering:
- Number of peaks
- Derivatives: max slope, min slope
- Range (normalized)
- STD normalized
