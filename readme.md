# Freight Rate Prediction Challenge

See `Freight_Rate_ML_Assessment.pdf` for the assessment instructions.

## What to do

1. Train and validate your model using `data/train_test.csv`.
2. Predict every load in `data/validation.csv`. Each load has a unique `load_id`.
3. Fill the matching `predicted_rate` values in `data/validation_predictions_template.csv` and save it as `validation_predictions.csv`.
4. Predict every row in `data/december_chart_inputs.csv` by filling its `predicted_rate` column.
5. Install the scorer requirements and run:

```bash
python -m pip install -r requirements.txt
python score.py --predictions validation_predictions.csv --december-predictions data/december_chart_inputs.csv
```

The scorer validates both files and creates `scorer_results/candidate_december.png`.

## How to run this project

1. Create the conda environment:

2. Launch Jupyter from this project folder:

3. Open `freight_rate_model.ipynb` and run all cells top to bottom (Cell → Run All). This will:
   - Clean and explore `train-test.csv`
   - Train and evaluate the models
   - Generate `validation_predictions.csv`
   - Generate the completed `december-chart-inputs.csv`

4. Validate the outputs and generate the chart:
