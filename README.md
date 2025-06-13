# 🧪 Molecular Solubility Prediction using ML

This project aims to predict the solubility (`logS`) of molecules based on various chemical descriptors using regression models. The dataset used is the Delaney solubility dataset, available [here](https://raw.githubusercontent.com/dataprofessor/data/master/delaney_solubility_with_descriptors.csv).

## 📊 Dataset

- **Source**: Delaney Solubility Dataset
- **Size**: 1144 molecules
- **Features**:
  - `MolLogP`
  - `MolWt`
  - `NumRotatableBonds`
  - `AromaticProportion`
  - Target: `logS` (solubility)

## 🛠️ Steps

1. **Load and inspect data**
2. **Split into features (`X`) and target (`y`)**
3. **Train-test split (80/20)**
4. **Train models**:
   - Linear Regression
   - Random Forest Regressor
5. **Evaluate with**:
   - Mean Squared Error (MSE)
   - R² Score
6. **Visualize predicted vs. actual values**

## 📈 Model Performance

| Model             | Train R² | Test R² | Train MSE | Test MSE |
|------------------|----------|---------|-----------|----------|
| Linear Regression| 0.764    | 0.789   | 1.007     | 1.021    |
| Random Forest    | 0.760    | 0.709   | 1.028     | 1.408    |

## 🖼️ Visual Output

- Scatter plot of predicted vs actual values for `logS` using Linear Regression.

## 📌 Requirements

- Python
- pandas
- scikit-learn
- matplotlib
- numpy

## 💡 Conclusion

Even simple molecular descriptors can be effective in predicting solubility. Linear regression generalized better than a shallow Random Forest in this case.

