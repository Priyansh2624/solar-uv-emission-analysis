# Data

This project combines records and observations from three sources to study solar active-region UV emission and magnetic complexity.

## Data sources

### NOAA Solar Region Summary

Daily records provide active-region numbers, locations, sunspot areas, and magnetic classifications.

- Source: [NOAA Solar Region Summary](https://www.swpc.noaa.gov/products/solar-region-summary)
- Project use: identify active regions and their magnetic classifications.

### SDO/HMI SHARP

HMI SHARP observations provide active-region patches and bitmap data.

- Source: [Joint Science Operations Center (JSOC)](http://jsoc.stanford.edu/)
- Project use: associate NOAA active regions with HARPs and select pixels using the bitmap.

### SDO/AIA 1600 Å

AIA observations provide ultraviolet images of the Sun.

- Source: [SDO and JSOC](http://jsoc.stanford.edu/)
- Data series used in the acquisition workflow: `aia.lev1_uv_24s`
- Project use: measure UV intensity at locations selected by the HMI bitmap.

## Study period and selection

The intended study period is **2014–2024**. The initial selection focuses on active regions within approximately ±10° of the solar central meridian.

## Data storage

The original FITS observations can be large and are not intended to be stored in full in this repository. They should be obtained from the source archives.

Small manifests and processed measurement tables can be added to this folder as they are validated. These should record enough information to identify the original observations, including dates, NOAA and HARP numbers, observation times, and processing status.

## Validation

The dataset is still being validated. Missing observations and unsuccessful matches should be recorded explicitly rather than treated as zero-intensity measurements.
