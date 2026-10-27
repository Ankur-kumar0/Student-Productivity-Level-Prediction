# Student Productivity Level Prediction

## About the Project

This project uses machine learning to predict a student's productivity
level based on information such as study habits, phone usage,
attendance, and other student-related factors.

The project covers the main steps of a machine learning workflow:
understanding the dataset, cleaning the data, exploring it, preparing
features, training models, and comparing model performance.

## Project Files

| File | Description |
|---|---|
| dataset_understanding.py | Loads the dataset and checks its columns, data types, missing values, duplicates, and basic statistics. |
| data_cleaning.py | Removes duplicate rows and fills missing numerical and categorical values. |
| eda.py | Performs exploratory data analysis and creates charts. |
| eature_engineering.py | Creates productivity-level labels, encodes categorical data, splits the data, and scales features. |
| ml_models.py | Trains Logistic Regression, Gaussian Naive Bayes, KNN, and Decision Tree models. |
| model_comparison.py | Compares model performance using evaluation metrics and charts. |
| student_productivity_pipeline.py | Runs the complete project pipeline, if configured as the combined script. |
| equirements.txt | Lists the Python libraries needed for the project. |

## Dataset

The project uses a student productivity and distraction dataset.

Place the CSV dataset in the project's data folder. Update the dataset
path in the code to match its location on your computer. For example:

`python
df = pd.read_csv("data/student_productivity_distraction_dataset_20000.csv")
`

The cleaned dataset is saved as:

`	ext
data/student_productivity_cleaned.csv
`

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Models Used

The project trains and compares these four classification models:

1. Logistic Regression
2. Gaussian Naive Bayes
3. K-Nearest Neighbors (KNN)
4. Decision Tree

The models are evaluated using accuracy, precision, recall, F1-score,
confusion matrices, and classification reports.

## How to Run

1. Download or clone this repository.

2. Open the project folder in VS Code or another Python editor.

3. Make sure the dataset is placed in the data folder.

4. Install the required libraries:

   `ash
   pip install -r requirements.txt
   `

5. Run the Python files in order, starting with data understanding and continuing
   through model comparison. Alternatively, run student_productivity_pipeline.py
   if it contains the complete pipeline.

Example:

`ash
python dataset_understanding.py
`

## Output

The project creates cleaned data, analysis results, and visualizations.
Depending on the scripts, these are saved in:

- data/ -- cleaned dataset
- output/results/ -- analysis results and model comparison CSV files
- output/figures/ -- charts, heatmaps, confusion matrices, and the decision tree diagram

Make sure these folders exist before running the scripts, or create them
in the code before saving files.

## Notes

- The dataset path may need to be changed for your computer.
- The code saves files using relative paths such as data/ and output/.
- Model results depend on the dataset and the train-test split.
