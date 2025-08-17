# Blood Pressure Estimation from ECG and Arterial Signals

This project looks at whether blood pressure can be estimated from ECG and arterial pressure waveforms using data analysis and machine learning. The work started as part of my Honours research, and the notebook shows the steps I took from cleaning the raw data through to building and testing models.

## What the notebook does

Loads a multi-channel ECG/arterial dataset.

Cleans and preprocesses the data (scaling, filtering, trimming sections).

Plots the signals so it’s easier to see what’s happening.

Splits the dataset into training and testing.

Trains simple machine learning models to predict blood pressure.

Evaluates performance with error metrics (mainly Mean Squared Error).

The focus is on building a complete workflow, rather than squeezing out maximum model accuracy.

## Files in this repo

model.ipynb – the main notebook with all steps (data prep, visualisation, training, evaluation).

X000.txt – sample raw data file (ECG and arterial signals).

## How to run it

1. Clone this repo:

```
git clone https://github.com/yourusername/blood-pressure-ml.git
cd blood-pressure-ml
```

2. Install the required Python libraries:

```
pip install numpy pandas matplotlib scipy scikit-learn
```

3. Open the notebook in Jupyter:

```
jupyter notebook model.ipynb
```

## Results so far

The models were able to pick up relationships between the ECG/arterial inputs and blood pressure, though accuracy still leaves room for improvement. It’s a good starting point and shows that the approach is viable for non-invasive estimation.

Next steps

Try different model types (e.g. CNNs or LSTMs for time-series).

Do more feature engineering, especially frequency-domain features.

Improve hyperparameter tuning.
