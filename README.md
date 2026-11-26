Neural Architecture and Extrapolation Uncertainty in Hybrid Hydrological Projections under Climate Change

#Overview

This repository contains the research code for evaluating neural architecture and extrapolation uncertainty in hybrid SWAT–deep learning streamflow projections under CMIP6 climate change scenarios.
The framework investigates how different deep learning architectures influence projected streamflow changes when coupled with the same SWAT hydrological simulations and climate forcing data.

#Deep Learning Architectures
Five neural network architectures are investigated:

- Long Short-Term Memory (LSTM)
- Gated Recurrent Unit (GRU)
- Temporal Convolutional Network (TCN)
- Multilayer Perceptron (MLP)
- LSTM–Fully Convolutional Network (LSTM-FCN)

#Climate Scenarios
Future streamflow projections are evaluated under SSP2-4.5 (SSP245)and SSP5-8.5 (SSP585)
Two future periods are considered: Near future (2041–2070) and Far future (2071–2100)

# Repository Structure
Neural-Architecture-Extrapolation-Hydrological-Projections/

Neural-Architecture-Extrapolation-Hydrological-Projections.ipynb
    README.md
    requirements.txt
    CITATION.cff
    LICENSE
   .gitignore
   data/SSP245.xlsx, SSP585.xlsx and README.md
   results/README.md
# Data Availability
Historical hydroclimatic data were obtained from the Ministry of Water Resources and Energy of Ethiopia.
These data are not redistributed in this repository. 
Researchers interested in accessing them should submit a formal request to the Ministry, subject to its approval and applicable data-sharing requirements.
The SSP245 and SSP585 datasets are provided in this repository. The Historical.xlsx files must be obtained separately to execute the complete workflow.

#Installation
The code was developed using Python 3.11.18.
Install the required packages:

pip install -r requirements.txt

Running the Notebook

1. Clone or download this repository.
2. Place the required historical dataset and station descriptor file in the `data/` directory.
3. Confirm that the SSP245 and SSP585 datasets are also in the `data/` directory.
4. Launch Jupyter Notebook.
5. Open the research notebook and execute the cells sequentially.

#Code Availability
The complete computational workflow is provided in this repository. 
The notebook includes data preparation, model training, evaluation, and future streamflow projection procedures.

#Citation

If you use this code in your research, please cite the associated research publication. 
A formal software citation and DOI will be added following Zenodo archival.

#License
The license and reuse conditions will be specified in the repository's LICENSE file.