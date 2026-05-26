# House Price Prediction

This project predicts house prices using a dataset of Hyderabad housing data. It includes a small Python entrypoint and an exploratory notebook for data analysis, preprocessing, and machine learning modeling.

## Project Contents

- `main.py` - simple entrypoint for the project.
- `requirements.txt` - Python dependencies for the notebook and scripts.
- `data/Hyderbad_House_price.csv` - raw housing dataset used for analysis and modeling.
- `notebook/house_price_prediction.ipynb` - Jupyter notebook with dataset exploration, preprocessing, feature analysis, model training, and evaluation.

## Dataset Details

The dataset file `data/Hyderbad_House_price.csv` contains housing market data for Hyderabad. Common columns include:

- `area_type` - type of area, such as Super built-up Area, Built-up Area, Plot Area, etc.
- `availability` - whether the property is ready to move or available from a future date.
- `location` - locality or neighborhood within Hyderabad.
- `size` - number of bedrooms or configuration, such as "2 BHK".
- `society` - society or housing development name.
- `total_sqft` - total area size in square feet.
- `bath` - number of bathrooms.
- `balcony` - number of balconies.
- `price` - target variable representing house price (typically in lakhs or the dataset's unit).

> Note: The column names and exact dataset format can be confirmed by opening the CSV file in a spreadsheet editor or inspecting the notebook.

## Module and File Descriptions

### `main.py`

- `def main():` - defines the main function for the script.
- `print("Hello from house-price-prediction!")` - prints a simple greeting message when the script is executed.
- `if __name__ == "__main__":` - standard Python guard to execute `main()` only when the file is run directly, not when imported.

This module currently acts as a placeholder and can be extended later to run training, evaluation, or prediction workflows.

### `notebook/house_price_prediction.ipynb`

This notebook contains the main data science workflow for the project:

1. Load the dataset from `data/Hyderbad_House_price.csv`.
2. Inspect the data structure, missing values, and data types.
3. Clean and preprocess columns such as `total_sqft`, `size`, and `location`.
4. Engineer features and encode categorical variables for machine learning.
5. Split the dataset into training and testing sets.
6. Train one or more regression models to predict house prices.
7. Evaluate model performance using metrics such as R-squared, mean absolute error, or root mean squared error.
8. Visualize relationships between features and the target price.

## How to Run

1. Create and activate a Python environment.
2. Install dependencies from `requirements.txt`.
3. Start Jupyter Notebook and open `notebook/house_price_prediction.ipynb`.

Example commands:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python -m notebook notebook/house_price_prediction.ipynb
```

## Future Improvements

- Add a dedicated Python script for preprocessing and training.
- Build a prediction API or command-line interface.
- Include model serialization and inference code.
- Expand dataset documentation with exact column types and units.
