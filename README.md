# 🍷 Wine Dataset Analysis

This project performs a comprehensive statistical and exploratory analysis of the famous **Wine Dataset** from the UCI Machine Learning Repository using Python. It includes data preprocessing, outlier detection, and dimensionality reduction using PCA.

---

## 📦 Dataset

The dataset is loaded from `sklearn.datasets.load_wine()` and contains chemical analysis results of wines grown in the same region in Italy, derived from three different cultivars.

- **Number of Instances:** 178  
- **Number of Features:** 13 (plus 1 target column)
- **Target:** Wine class (0, 1, or 2)

---

## 🧪 Project Structure

The analysis is divided into the following key sections:

### 1. **Descriptive Statistical Analysis**
- Calculates mean, median, standard deviation, skewness, and kurtosis for all features.
- Outputs summary statistics using `pandas.describe()` and additional statistical functions.

### 2. **Exploratory Data Analysis (EDA)**
- Visualizes the distribution of features using:
  - Histograms
  - KDE (Kernel Density Estimation) plots
  - Pair plots (colored by wine type)

### 3. **Outlier Detection**
- Uses the IQR (Interquartile Range) method to detect outliers.
- Boxplot-based logic for identifying data points outside the typical range.

### 4. **Correlation Analysis**
- Computes and visualizes feature correlations using a heatmap.
- Helps identify multicollinearity between features.

### 5. **Data Preprocessing**
- Applies two scaling techniques:
  - MinMax Scaling
  - Standard Scaling
- Scaled data is prepared for use in PCA and other ML models.

### 6. **Principal Component Analysis (PCA)**
- Applies PCA on both MinMax and Standard scaled data.
- Visualizes cumulative explained variance using scree plots.

---

## 🛠️ Dependencies

Make sure you have the following Python libraries installed:

```bash
pip install numpy pandas seaborn matplotlib scikit-learn
