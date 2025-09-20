# Cars Dataset Analysis - Trainee Data Scientist Task (Project Skeleton)

This repository is a template/skeleton to complete the Trainee Data Scientist task. It contains step-by-step code templates, structured folders for **plots** and **tables**, and instructions for committing to GitHub.

## How the project is organized
- `data/` - put the downloaded dataset here (name it `cars_dataset.csv` or update path in code)
- `step_1_reading_and_preprocessing/`
  - `step_1_code.py` - code to load, inspect and clean the dataset
  - `plots/` - images from step 1
  - `tables/` - CSV outputs from step 1 (e.g., missing_values.csv, duplicates.csv, cleaned_data.csv)
- `step_2_working_with_numeric_data/`
  - `step_2_code.py` - numeric analysis + saving tables/plots
  - `plots/`
  - `tables/`
- `step_3_working_with_text_data/`
  - `step_3_code.py` - text-based analysis (models per company, electric manufacturers)
  - `plots/`
  - `tables/`
- `step_4_visualisations/`
  - `step_4_code.py` - plotting functions (histogram, scatter, bar chart)
  - `plots/` - final visualization images
  - `tables/`
- `step_5_optional_average_price_speed/`
  - `step_5_code.py` - optional task (avg price window and top speed cars)
  - `plots/`
  - `tables/`

## How to use
1. Download the dataset from Kaggle:
   https://www.kaggle.com/datasets/abdulmalik1518/cars-datasets-2025
   Put the CSV in `data/cars_dataset.csv` (or change `DATA_PATH` in the scripts).
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run files step-by-step (you can run them as scripts or open them inside Jupyter). Each script will save tables to `tables/` and plots to `plots/` inside its step folder.
   ```bash
   python step_1_reading_and_preprocessing/step_1_code.py
   python step_2_working_with_numeric_data/step_2_code.py
   python step_3_working_with_text_data/step_3_code.py
   python step_4_visualisations/step_4_code.py
   python step_5_optional_average_price_speed/step_5_code.py
   ```

## Git & GitHub instructions (where to commit and upload files)
We recommend committing step-by-step so reviewers can follow progress.
Example sequence (run from repo root):

1. Initialize repo (first time):
```bash
git init
git add .
git commit -m "initial commit: project skeleton and README"
git branch -M main
git remote add origin git@github.com:yourusername/cars-dataset-analysis.git
git push -u origin main
```

2. After finishing Step 1, commit only step 1 files:
```bash
git add step_1_reading_and_preprocessing/
git commit -m "step_1: load CSV, inspect, clean fuel types, save missing/duplicates/cleaned_data"
git push
```

3. After Step 2:
```bash
git add step_2_working_with_numeric_data/
git commit -m "step_2: avg price by company, top5 horsepower, acceleration comparison saved"
git push
```

4. Repeat for Steps 3, 4 and (optional) 5. Keep messages short and descriptive.

## File naming conventions (recommended)
- Tables: `*.csv` (snake_case, no spaces) e.g. `avg_price_by_company.csv`
- Plots: `*.png` e.g. `toyota_price_hist.png`
- Scripts: `step_n_code.py` (match the folder `step_n_name_of_step`)

## Questions / Next steps
- If you want, I can populate the scripts with runnable code templates that try to detect column names robustly (so you can just drop the CSV and run).

Good luck 👊
