==== Machine Learning Models Evaluation on Imbalanced Data - Cervical Cancer =====

Anaconda Version: 2.5.2

JupyterNotebook Version: 7.3.2

==== Project Description:====

This project focuses on predicting cervical cancer diagnosis using a medical dataset collected from Hospital Universitario de Caracas. 

This project explores multiple machine learning models on an imbalanced binary classification dataset. It uses the `risk_factors.csv` dataset for Cervical Cancer (858 entries and 36 columns). 

The goal is to train and compare 2 machine learning models, primarily Decision Tree and Random Forest, to identify patients at risk of cervical cancer based on a single target variable. Because of the imbalance in the dataset—where positive cancer cases are fewer, special emphasis is placed on recall and F1-score to minimize false negatives, which are critical in medical diagnosis.

- Loading and preprocessing the dataset

- Cleaning the dataset

- Visualisation

- Splitting the dataset into Train, Test and Validation Sets

- Feature Selection using chi2 and SelectKBest

- Data Modelling of Random Forest and Decision Tree

- Evaluating the 2 Models by looking at the Accuracy, Recall, Precision and F1-score as well as the Confusion Matrix

==== Technologies Used: ====

- Python and Jupyter Notebook

- scikit-learn

- pandas/numpy

- Matplotlib/Seaborn: For visualization


==== How to install and Run the Project: ====

1. Download the .ipynb notebook file
2. Upload the .ipynb file in JupyterNotebook
3. Install dependencies if not already installed
	i. Open Anaconda Prompt
	ii. Switch from base terminal to TF terminal using "conda activate tf" 
	iii. Install dependencies " pip3 install pandas numpy scikit-learn matplotlib seaborn"

4. The pre-executed cells should show the results. If not then run the cells sequentially.

==== Contributors ====

Laiba Faraz, Faiq Ahmed Shaikh, Ma Bowen
