# Solar UV Emission from Active Regions

This project investigates the relationship between ultraviolet (UV) emission from solar active regions and their magnetic complexity.

The research combines NOAA active-region classifications with observations from the Solar Dynamics Observatory (SDO), focusing on data from **2014–2024**.

## Research question

How does ultraviolet emission from solar active regions vary with their magnetic complexity and Hale classification?

## Data sources

- **NOAA Solar Region Summary:** Active-region numbers, locations, sunspot areas, and magnetic classifications.
- **SDO/HMI SHARP:** Active-region bitmap data used to identify selected pixels.
- **SDO/AIA:** Ultraviolet observations at 1600 Å used to measure emission.

## Methodology

The project follows this workflow:

1. Identify active regions from NOAA Solar Region Summary records.
2. Select regions within approximately ±10° of the solar central meridian.
3. Match NOAA active-region numbers with HMI Active Region Patch (HARP) numbers.
4. Obtain HMI SHARP bitmaps and AIA 1600 Å observations close in time.
5. Align the observations using their world coordinate system information.
6. Select bitmap values 33 and 34 and extract the corresponding AIA intensities.
7. Validate the measurements and compare UV emission across magnetic classifications.

The current measurement sums the intensities of selected pixels. Because that sum depends on both brightness and the number of selected pixels, active-region size and mean intensity are also relevant when comparing regions.

## Project status

This research is **in progress**. Initial work includes NOAA data processing, observation scans, active-region matching, image-alignment methods, and tests of UV intensity extraction.

The complete multi-year dataset still needs validation. Statistical comparisons, final figures, and scientific conclusions are planned. Machine-learning prediction of UV emission is a possible future extension.

## Repository structure

- `data/` — data and associated metadata
- `src/` — project source code
- `notebooks/` — exploratory work and analysis
- `docs/` — project documentation
- `theory/` — scientific background
- `results/` — analysis outputs
- `test/` — project tests
- `requirements.txt` — Python dependencies

## Installation

Clone the repository:

```bash
git clone https://github.com/Priyansh2624/solar-uv-emission-analysis.git
cd solar-uv-emission-analysis
```

Create and activate a Python virtual environment, then install the dependencies:

```bash
python -m pip install -r requirements.txt
```

Refer to the project files for individual script and data-access instructions. Large FITS observations may need to be obtained separately from the original archives.
