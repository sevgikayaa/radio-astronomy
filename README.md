# radio-astronomy
Radio astronomy data analysis and visualization using Python
# Radio Astronomy Data Analysis

Python-based analysis and visualization of radio astronomy spectral data stored in FITS format.

## Overview

This project explores the processing and analysis of three-dimensional radio astronomy data cubes using Python. The notebook demonstrates how to inspect spectral data, generate intensity maps, extract spectral profiles, visualize individual channels, and apply statistical masking to reduce low-significance data.

## Features

* Read and inspect FITS spectral cubes
* Analyze cube dimensions and physical units
* Generate Moment 0 (integrated intensity) maps
* Extract and visualize spectral profiles at selected pixels
* Visualize individual spectral channels
* Calculate channel-based statistics
* Apply a 3σ threshold mask to spectral data
* Save processed data as a new FITS file
* Use memory mapping for more efficient handling of large FITS datasets

## Technologies

* Python
* NumPy
* Matplotlib
* Astropy
* SpectralCube
* Plotly
* Jupyter Notebook
* FITS

## Data Processing

The project uses a three-dimensional spectral data cube with dimensions corresponding to the spectral axis and two spatial axes.

The workflow includes:

1. Loading the FITS data cube.
2. Inspecting its dimensions, units, and spectral axis.
3. Producing an integrated intensity (Moment 0) map.
4. Extracting spectral profiles from selected spatial pixels.
5. Visualizing individual spectral channels.
6. Calculating channel statistics.
7. Estimating the noise level over a selected channel range.
8. Applying a 3σ mask to isolate significant emission.
9. Saving the processed data as a new FITS file.

## Memory-Efficient Processing

For the larger FITS dataset, the project uses `memmap=True` when opening the FITS file. This allows the data to be accessed through memory mapping rather than loading the entire dataset into memory at once.

## Example Output

The notebook produces:

* Integrated intensity maps
* Spectral profiles
* Individual channel maps
* Statistical distributions
* Noise estimates
* A 3σ-masked FITS data cube

## Repository Structure

```text
radio-astronomy/
├── radio_astronomy.ipynb
└── README.md
```

## Author

Sevgi Kaya

Astronomy & Space Sciences Graduate
Python | Data Analysis | Scientific Computing
