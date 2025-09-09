
SVM-based binary classification model to predict salary levels (&lt;=50K or >50K) using UCI Adult dataset.
Salary Data Classification
Overview
This project develops a Support Vector Machine (SVM) model to predict whether an individual’s annual salary is <=50K or >50K based on demographic and socioeconomic features from the UCI Adult Income dataset. The model achieves ~83% accuracy and is built using Python and Scikit-learn.
Purpose
The goal is to classify salary levels for applications like targeted marketing or HR analytics. This project demonstrates skills in machine learning, data preprocessing, and model evaluation, showcasing proficiency in Python, SVM, and data analysis.
Methodology

Data Preprocessing:
Loaded SalaryData_Train(1).csv (30,162 rows) and SalaryData_Test(1).csv (15,060 rows).
Handled missing values (‘?’) using median for numerical features (e.g., age, capitalgain) and mode for categorical features (e.g., workclass, occupation).
Encoded categorical features with OneHotEncoder and scaled numerical features with StandardScaler.


Model Training:
Used LinearSVC with balanced class weights to address ~75% <=50K imbalance.
Trained on preprocessed training data; validated on 20% holdout.


Evaluation:
Metrics: Accuracy, precision, recall, F1-score, confusion matrix.
Achieved ~83% test accuracy and ~0.65 F1-score for >50K class.



How to Run

Clone the repository: git clone https://github.com/SyedaHabeeba/Salary-Data-Classification.git
Install dependencies: pip install -r requirements.txt
Run the Jupyter Notebook: jupyter notebook code/salary_svm.ipynb
Ensure datasets (data/*.csv) are in the correct folder.


View results in visualizations/confusion_matrix.png.

Files

code/salary_svm.ipynb: Jupyter Notebook with SVM implementation.
data/SalaryData_Train(1).csv, data/SalaryData_Test(1).csv: UCI Adult dataset (optional, not uploaded due to size; source: UCI Repository).
visualizations/confusion_matrix.png: Confusion matrix plot.
requirements.txt: Python dependencies.
README.md: Project documentation.
.gitignore: Ignores Python cache files.
LICENSE: MIT License.

Results

Test Accuracy: ~83%
F1-Score (>50K): ~0.65
Confusion Matrix: Visualized in visualizations/confusion_matrix.png.
Key Insight: Features like educationno, capitalgain, and hoursperweek are strong predictors of high salary.

Technologies

Python 3.8+
Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn
Tools: Jupyter Notebook, Git, GitHub

Contact

GitHub: Jamilath
LinkedIn: [Your LinkedIn URL]](https://www.linkedin.com/in/mohammed-jameel-2866028/)
