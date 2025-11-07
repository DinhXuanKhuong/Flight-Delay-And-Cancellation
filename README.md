# Flight Delay and Cancellation Analysis

This repository contains an exploratory data analysis and baseline modeling project that investigates flight delays and cancellations using the provided 2024 flight data.

## Project overview

We analyze a dataset of flights (see `data/flight_data_2024.csv`) to answer practical questions such as:
- What are the main causes of delays and cancellations?
- Which routes, carriers, or airports have higher delay or cancellation rates?
- Can a simple model predict whether a flight will be delayed or cancelled from historical features?

The analysis and experiments are implemented in the Jupyter notebook `my_code.ipynb`. The notebook includes data loading, cleaning, exploratory visualizations, feature engineering, and baseline predictive modeling steps.

Dataset source: [Flight Delay & Cancellation Data (1 Million+ 2024)](https://www.kaggle.com/datasets/nalisha/flight-delay-and-cancellation-data-1-million-2024)

## Repository structure

- `my_code.ipynb` — primary notebook containing the data analysis and modeling workflow.
- `data/flight_data_2024.csv` — dataset used for analysis.
- `min_ds-env.yml` — recommended conda environment (minimal data-science environment) used to reproduce the notebook environment.
- `LICENSE` — repository license.

## Reproducible environment (recommended)

This project ships a conda environment file at `min_ds-env.yml`. It pins Python 3.11 and common data-science packages. Using this environment is the recommended way to reproduce the notebook exactly as run by the authors.

To create the environment with conda (requires conda or mamba):

```bash
# Create the environment using conda
conda env create -f min_ds-env.yml

# Activate the environment
conda activate min_ds-env

# (Optional) If you update the yaml later, update the env with:
conda env update -f min_ds-env.yml -n min_ds-env
```

If you prefer mamba for faster solves (recommended if you have it):

```bash
mamba env create -f min_ds-env.yml
mamba activate min_ds-env
```

If you don't use conda, create a lightweight virtual environment and install the core packages with pip. Example (approximate — package versions may differ):

```bash
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install pandas numpy scipy scikit-learn matplotlib seaborn plotly jupyterlab
```


## How to run the notebook

1. Ensure the dataset `data/flight_data_2024.csv` is present in the `data/` folder (it's already included).
2. Create and activate the environment (see previous section).
3. Start Jupyter Lab or Notebook from the repository root:

```bash
jupyter lab
# or
jupyter notebook
```

4. Open `my_code.ipynb` and run cells from top to bottom. Notebook cell numbers start from 1 in the interface.

Tips:
- Restart the kernel and run all cells if you switch environments.
- If a cell depends on heavy computation or large datasets, consider running it on a sample first.

## Quick notes on `min_ds-env.yml`

- Name: `min_ds-env` (the environment created will use this name by default).
- Python: 3.11.5 (as pinned in the YAML). If you need a different Python, you can modify the file or create a separate environment.
- Channels: `conda-forge`, `defaults` — these are defined in the YAML and used automatically by conda/mamba.

## Authors

- Le Minh Duc - FIT HCMUS
- Dinh Xuan Khuong - FIT HCMUS


## License

This project is provided under the terms in the `LICENSE` file in the repository root.

