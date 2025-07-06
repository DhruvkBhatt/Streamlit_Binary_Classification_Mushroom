## Binary Classification WebApp

This Streamlit application allows you to build and evaluate binary classification models to predict whether mushrooms are edible or poisonous based on their characteristics.

### Features

* Load and preprocess the [UCI Mushroom Dataset](https://archive.ics.uci.edu/ml/datasets/Mushroom).
* Three classification algorithms:

  * Support Vector Machine (SVM)
  * Logistic Regression
  * Random Forest
* Interactive sidebar controls for setting hyperparameters:

  * **SVM:** Regularization (C), kernel type, gamma
  * **Logistic Regression:** Regularization (C), maximum iterations
  * **Random Forest:** Number of trees, maximum depth, bootstrap sampling
* Option to plot common evaluation metrics:

  * Confusion Matrix
  * ROC Curve
  * Precision–Recall Curve
* Display model accuracy, precision, and recall.
* View raw preprocessed data table.

### Project Structure

```
├── app.py             # Main Streamlit application
├── mushrooms.csv      # Mushroom dataset (CSV format)
├── requirements.txt   # Python dependencies
└── README.md          # Project overview and instructions
```

### Prerequisites

* Python 3.7 or above
* pip (package installer)

### Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

### Usage

Run the Streamlit app:

```bash
streamlit run app.py
```

* Select a classifier and adjust hyperparameters in the sidebar.
* Click **Classify** to train the model and view results.
* Choose which metrics to plot under **What metrics to plot?**
* Toggle **Show raw data** to inspect the preprocessed dataset.

### Dataset

* The dataset file `mushrooms.csv` should be placed in the same directory as `app.py`.
* It contains various categorical features of mushrooms encoded into numeric labels.

### Dependencies

```
pandas
scikit-learn
streamlit
matplotlib
```

You can freeze exact versions using:

```bash
pip freeze > requirements.txt
```

---

*Developed as a teaching example for binary classification workflows with Streamlit.*
