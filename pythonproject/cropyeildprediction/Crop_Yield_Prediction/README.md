# Crop Yield Prediction

## Project Overview

This project is a web application that predicts crop yield based on several input features such as year, average rainfall, pesticide usage, temperature, area, and crop type. The application uses a machine learning model to make predictions and provides an intuitive interface for users to input data.

## Features

- User-friendly web interface built with HTML, CSS, and Bootstrap.
- Backend server implemented using Flask.
- Integration of pre-trained machine learning models.
- Real-time crop yield prediction based on user inputs.

## Folder Structure

```
|-- templates/
|   |-- index.html          # HTML file for the web interface
|-- static/
|   |-- css/                # CSS files for styling (if any additional styles are added)
|-- app.py                  # Main Flask application
|-- dtr.pkl                 # Pickle file for the Decision Tree Regressor model
|-- preprocessor.pkl        # Pickle file for the preprocessing pipeline
|-- requirements.txt        # Python dependencies
|-- README.md               # Documentation for the project
```

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- Python 3.8 or above
- pip (Python package manager)

## Installation

1. Clone the repository to your local system:

   ```bash
   git clone <repository_url>
   cd <repository_folder>
   ```

2. Create a virtual environment and activate it:

   ```bash
   python -m venv venv
   source venv/bin/activate  # For Linux/MacOS
   venv\Scripts\activate   # For Windows
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Ensure `dtr.pkl` and `preprocessor.pkl` are in the project directory.

## Usage

1. Start the Flask application:

   ```bash
   python app.py
   ```

2. Open your web browser and navigate to:

   ```
   http://127.0.0.1:5000
   ```

3. Enter the required inputs into the web form and click "Predict" to get the predicted crop yield.

## Input Features

The application requires the following inputs:

- **Year**: The year for which the prediction is to be made.
- **Average Rainfall (mm/year)**: The average annual rainfall in millimeters.
- **Pesticides (tonnes)**: The quantity of pesticides used in tonnes.
- **Average Temperature (°C)**: The average temperature in degrees Celsius.
- **Area**: The geographical area (e.g., country or region).
- **Item**: The type of crop (e.g., wheat, maize).

## Dependencies

The `requirements.txt` file includes:

- Flask
- numpy
- scikit-learn

Install dependencies with:

```bash
pip install -r requirements.txt
```

## Model Details

- **Decision Tree Regressor (********`dtr.pkl`********)**: A machine learning model trained on historical crop yield data.
- **Preprocessing Pipeline (********`preprocessor.pkl`********)**: Handles categorical data encoding, scaling, and other preprocessing steps.

## How It Works

1. User inputs features in the form.
2. The Flask backend processes the data and applies preprocessing using the `preprocessor.pkl` file.
3. The transformed features are passed to the decision tree model (`dtr.pkl`) for prediction.
4. The predicted yield is displayed on the web page.

## Example Input

```text
Year: 2013
Average Rainfall (mm/year): 1200
Pesticides (tonnes): 10
Average Temperature (°C): 25
Area: Argentina
Item: Wheat
```

## Example Output

```text
Predicted Yield: 2500 kg/ha
```

##

## License

## Authors

- Suraj Ashok Chaugule

# Crop-Yield-Prediction-
# Crop-Yield-Prediction-
# Crop-Yield-Prediction-
