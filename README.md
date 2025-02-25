# Car Price Analysis

This project analyzes a used-car dataset to determine which features have the greatest impact on a vehicle’s selling price. The analysis includes data cleaning, exploratory data analysis (EDA), regression modeling, and interpretation of key factors influencing car price.

## Project Structure

CarPriceAnalysis/
├── data/
│ └── car_price_dataset.csv # The dataset (if included)
├── CarPrice_Analysis.ipynb # Jupyter Notebook with end-to-end analysis
├── requirements.txt # List of dependencies
├── .gitignore # Files/folders to ignore (e.g., venv/, .ipynb_checkpoints)
└── README.md # This file

1. **data/** – Contains the CSV file with car price data
2. **CarPrice_Analysis.ipynb** – A Jupyter Notebook that walks through data loading, cleaning, EDA, modeling, and evaluation.
3. **requirements.txt** – Lists all Python packages required to run this project.
4. **.gitignore** – Specifies files and folders to ignore (e.g., `venv/`, `.ipynb_checkpoints`).

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/thilankajayathilaka/CarPriceAnalysis.git
cd CarPriceAnalysis
```

### 2. Create and Activate a Virtual Environment

It's best practice to run this project in an isolated environment.

Using venv (Python built-in):

```bash
python -m venv venv
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate
Using conda:
```

```bash
conda create -n carpriceenv python=3.9
conda activate carpriceenv
```

### 3. Install Dependencies

Install the required Python packages from requirements.txt:

```bash
pip install -r requirements.txt
```

### 4. Register Environment with Jupyter

If you want to run the Jupyter Notebook in your virtual environment:

```bash
pip install ipykernel
python -m ipykernel install --user --name carpriceenv --display-name "CarPrice Analysis Env"
```

## Usage

### 1. Open the Notebook

In your activated environment, launch Jupyter Notebook:

```bash
jupyter notebook
```

### 2.Select Kernel

If you installed the IPython kernel, select "CarPrice Analysis Env" (or your chosen display name) from the kernel menu.

### 3.Run the Analysis

The notebook CarPrice_Analysis.ipynb loads the dataset, performs data cleaning and preprocessing, carries out exploratory data analysis, and trains a regression model to predict car price. It then evaluates the model using R², MAE, and RMSE, and examines which features most influence the price.

## Project Overview

Business Question:
"Which factors are most influential in determining a car’s price?"

## Workflow:

- **Data Loading:** Reads the car price dataset.
- **Data Cleaning & Preprocessing:** Removes duplicates, handles missing values, and encodes categorical features.
- **Exploratory Data Analysis (EDA):** Visualizes distributions, correlations, and relationships (e.g., Price vs. Mileage).
- **Modeling:** Implements linear regression (with options for advanced models) to predict car price.
- **Evaluation:** Computes performance metrics (R², MAE, RMSE) and inspects regression coefficients to identify key factors.
- **Insights:** Summarizes which features (e.g., Mileage, Year, Make, Model) most affect the car's price.
