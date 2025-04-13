# Feature-Engineering-Boruta-RFE-PCA
This project demonstrates three popular techniques for feature selection and dimensionality reduction using the **Breast Cancer Wisconsin dataset**:

- ✅ **Boruta** (all-relevant feature selection)
- 🔁 **Recursive Feature Elimination (RFE)**
- 📉 **Principal Component Analysis (PCA)**

The project compares how each technique affects model performance using a **Random Forest Classifier** and visualizes PCA components.

## 📂 Project Structure

```
├── feature_selection_demo.py       # Main script (or notebook)
├── requirements.txt                # Dependencies
├── README.md                       # Project overview
```

## 🚀 Techniques Used

### 1. Boruta
A wrapper method that uses a Random Forest classifier to iteratively find all features that are statistically significant.

### 2. RFE
Selects a specified number of features by recursively removing the least important ones based on a base estimator (e.g., Logistic Regression).

### 3. PCA
Transforms features into a smaller number of uncorrelated components while preserving as much variance as possible.

## 📊 Dataset

- **Source**: `sklearn.datasets.load_breast_cancer`
- **Shape**: 569 samples × 30 features
- **Task**: Binary classification (malignant vs. benign)

## ⚙️ How to Run

```bash
# Install dependencies
pip install -r requirements.txt

# Run the script
python feature_selection_demo.py
```
Alternatively, open the project in Jupyter Notebook to view interactive outputs and visualizations.

## ✅ Results

The script evaluates and compares classification performance on features selected by:
- **Boruta**
- **RFE**
- **PCA-transformed components**

It also visualizes PCA components to show how the data distributes across dimensions.

## 📌 Dependencies

- `scikit-learn`
- `pandas`
- `numpy`
- `boruta`
- `matplotlib`
- `seaborn`

## 📈 Sample Output

- Features selected by Boruta and RFE
- Classification reports for each method
- PCA variance explained
- 2D scatter plot of PCA components
