# Forecasting Mobile Network Traffic in Milan

This repository contains the code and documentation for the assignment **"Comparative Time Series Analysis and Forecasting of Mobile Network Traffic"**. The project processes a 19.4 GB dataset of mobile Internet activity across 10,000 geographical squares in Milan, performs exploratory data analysis, and compares three forecasting models (Holt–Winters, GRU, LSTM) on a held-out test week.


## Setup Instructions

1. **Clone the repository** and navigate into the folder:
   ```bash
   git clone 
   cd Time_Series_Forecasting
Create and activate a virtual environment:

bash
python -m venv venv
source venv/bin/activate       # Linux / macOS
venv\Scripts\activate          # Windows
Install dependencies:

bash
pip install -r requirements.txt
Download the raw dataset (if you wish to rerun the full pipeline):

Obtain the “Telecommunications activity dataset for the city of Milan” from Harvard Dataverse.

Download all 62 files (≈19.4 GB). Place them in a folder named Milan_Network_Traffic_Dataset.

The Grid dataset (spatial mapping) is available here – not strictly required but recommended for spatial analysis.

Run the notebook:

Launch Jupyter:

bash
jupyter notebook notebook.ipynb
Execute cells sequentially. The notebook is self-contained and will process the data, generate all plots, and produce forecast results.

Reproducibility
All random seeds are fixed (NumPy, random, TensorFlow) to ensure deterministic neural network training.

The Google Colab environment used for Task 3 is documented in the notebook; hardware details are recorded in the report.

If you cannot run the full pipeline due to resource constraints, the provided data/Target_Squares_TimeSeries.csv contains the pre-extracted time series for the three target squares, so you can still run all EDA and forecasting models directly.

