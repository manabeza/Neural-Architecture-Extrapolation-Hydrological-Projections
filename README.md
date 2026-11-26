# Neural Architecture and Extrapolation Uncertainty in Hybrid Hydrological Projections under Climate Change

[![Software DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24565795.svg)](https://doi.org/10.5281/zenodo.24565795)
[![Dataset DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24564390.svg)](https://doi.org/10.5281/zenodo.24564390)

## Overview

This repository contains the research code for evaluating neural architecture and extrapolation uncertainty in hybrid SWAT–deep learning streamflow projections under CMIP6 climate change scenarios.

The framework investigates how different deep learning architectures influence projected streamflow changes when coupled with the same SWAT hydrological simulations and climate forcing data.

## Deep Learning Architectures

Five neural network architectures are investigated:

- Long Short-Term Memory (LSTM)
- Gated Recurrent Unit (GRU)
- Temporal Convolutional Network (TCN)
- Multilayer Perceptron (MLP)
- LSTM–Fully Convolutional Network (LSTM-FCN)

## Climate Scenarios

Future streamflow projections are evaluated under:

- SSP2-4.5 (SSP245)
- SSP5-8.5 (SSP585)

Two future periods are considered:

- Near future: 2041–2070
- Far future: 2071–2100

## Repository Structure


Neural-Architecture-Extrapolation-Hydrological-Projections/
│
├── Neural-Architecture-Extrapolation-Hydrological-Projections.ipynb
├── README.md
├── requirements.txt
├── CITATION.cff
├── LICENSE
├── .gitignore
│
├── data/
│   └── README.md
│
└── results/
    └── README.md


The SSP245, SSP585, and station descriptor datasets are archived separately on Zenodo.

## Data Availability

Historical hydroclimatic data were obtained from the Ministry of Water Resources and Energy of Ethiopia. These data are not redistributed in this repository. Researchers interested in accessing them should submit a formal request to the Ministry, subject to its approval and applicable data-sharing requirements.

The CMIP6 SSP245 and SSP585 climate input datasets, together with the station descriptor file, are publicly archived on Zenodo:

**Dataset DOI:** https://doi.org/10.5281/zenodo.24564390

The Historical.xlsx file must be obtained separately to execute the complete workflow.

## Installation

The code was developed using Python 3.11.18.
Install the required packages using:

pip install -r requirements.txt

## Running the Notebook

1. Clone or download this repository.
2. Place the required historical dataset (`Historical.xlsx`) and station descriptor file (`Station_Descriptor.xlsx`) in the `data/` directory.
3. Ensure that the SSP245 and SSP585 datasets are also available in the `data/` directory.
4. Launch Jupyter Notebook.
5. Open the research notebook and execute the cells sequentially.

## Code Availability

The complete computational workflow is publicly available on GitHub and archived on Zenodo.

**Software DOI:** https://doi.org/10.5281/zenodo.24565795

**Software version:** 1.0.1

The notebook includes data preparation, model training, performance evaluation, architectural uncertainty analysis, and future streamflow projection procedures.

## Citation

If you use this software in your research, please cite:

Dinku, M. B. (2026). *Neural Architecture and Extrapolation Uncertainty in Hybrid Hydrological Projections under Climate Change* (Version 1.0.1) [Computer software]. Zenodo. https://doi.org/10.5281/zenodo.24565795

If you use the associated climate input datasets, please also cite:

Dinku, M. B., & You, J. (2026). *CMIP6 SSP245 and SSP585 Climate Input Datasets for Hybrid SWAT–Deep Learning Hydrological Projections* (Version 1.0.0) [Dataset]. Zenodo. https://doi.org/10.5281/zenodo.24564390

## License

This repository is distributed under the MIT License. See the `LICENSE` file for details.
