# Optuna CNN Tuning in PyTorch

Project demonstrating hyperparameter optimization with Optuna on a small CNN.  
Includes saved trial plots and a YouTube walkthrough video.

## Goals
- Keep the project reproducible in one Jupyter notebook
- Run Optuna trials on a CNN in PyTorch
- Save best trial, study, and plots
- Provide a short video walkthrough

## Dataset
I use the public Telco Customer Churn dataset:

| source | rows | key fields | notes |
|---|---:|---|---|
| Telco Customer Churn | 7043 | customerID, tenure, MonthlyCharges, TotalCharges, Contract, PaymentMethod, InternetService, Churn | URL in data_sources.txt |

Dataset URL: https://www.kaggle.com/datasets/blastchar/telco-customer-churn

## Repository structure
.
├── optuna_cnn.ipynb              # notebook with training + tuning
├── plots/
│   ├── best_trial_history.png
│   └── param_importances.png
├── presentation/
│   └── optuna_walkthrough.txt    # link to YouTube video
├── docs/
│   └── notes.md
├── data_sources.txt
├── requirements.txt
├── .gitignore
└── LICENSE

## How to run
1. Create a virtual environment and install dependencies.
2. Open the notebook in VS Code or Jupyter and run all cells.

Commands:
    python -m venv .venv
    # Windows
    .\.venv\Scripts\activate
    # macOS/Linux
    . .venv/bin/activate

    pip install -r requirements.txt

Open optuna_cnn.ipynb in VS Code (with the Jupyter extension) or Jupyter Lab/Notebook, then run all cells.

## Tools and workflow
tool | purpose
---- | -------
VS Code | notebook editing and version control
Python venv | isolated dependencies
PyTorch | model and training loop
Optuna | hyperparameter optimization
matplotlib | plots

## Artifacts
- plots/best_trial_history.png
- plots/param_importances.png
- YouTube walkthrough video (link in presentation/optuna_walkthrough.txt)

## License
MIT License © 2025 Fabrizio Petrozzi
