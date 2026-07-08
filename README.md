# DACSS 690C — Homework 1: Spatial Autocorrelation (LISA)

Homework for the Computational Social Science Methods course (DACSS, UMass Amherst).

This repository contains:

- **PeruMaps.gpkg** — geopackage of Peru's districts with social indicators
  (population, HDI, high school completion, poverty, sanitation). Same file used in the course tutorial.
- **HW1.ipynb** — Jupyter notebook that, for the department of **Lima**:
  1. Reads the map and verifies/reprojects the CRS
  2. Builds a Queen contiguity weights matrix (row-normalized) and produces a LISA cluster map of `Educ_sec_comp2019_pct`
  3. Repeats the LISA analysis with a KNN (k = 8) weights matrix
  4. Compares the two classifications and reports which districts change groups

## Running it

Open the notebook in Google Colab and run all cells. The first cell installs PySAL (`libpysal` + `esda`); the data is read directly from this repository's URL.