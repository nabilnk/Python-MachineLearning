# 🏠 Prediksi Harga Rumah dengan Machine Learning

Project machine learning untuk memprediksi harga rumah menggunakan berbagai algoritma seperti Random Forest, Gradient Boosting, dan ensemble methods.

## 📊 Dataset

### Dataset Utama (Recommended)
**House Prices - Advanced Regression Techniques** dari Kaggle:
- **Link**: https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data
- **Deskripsi**: Dataset kompetisi Kaggle dengan 79 fitur untuk prediksi harga rumah
- **Jumlah Data**: 1460 sampel training
- **Target**: SalePrice (harga jual rumah)

### Dataset Alternatif
Jika tidak bisa mengakses Kaggle, notebook akan otomatis menggunakan:
1. **Boston Housing Dataset**: https://raw.githubusercontent.com/selva86/datasets/master/BostonHousing.csv
2. **Synthetic Dataset**: Dataset buatan dengan karakteristik realistis

## 🚀 Cara Menggunakan

### Opsi 1: Dengan Dataset Kaggle (Recommended)
1. **Download Dataset**:
   - Kunjungi: https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data
   - Download file `train.csv`
   - Letakkan di folder yang sama dengan notebook

2. **Jalankan Notebook**:
   - Buka `house_price_prediction.ipynb`
   - Jalankan semua cell secara berurutan

### Opsi 2: Tanpa Download (Auto Dataset)
1. **Langsung Jalankan**:
   - Buka `house_price_prediction.ipynb`
   - Notebook akan otomatis menggunakan dataset alternatif
   - Jalankan semua cell secara berurutan

## 🔧 Requirements

\`\`\`bash
pip install pandas numpy matplotlib seaborn scikit-learn
\`\`\`

## 📋 Struktur Project

\`\`\`
house-price-ml-notebook/
├── house_price_prediction.ipynb    # Main notebook
├── README.md                       # Dokumentasi ini
└── train.csv                      # Dataset Kaggle (optional)
\`\`\`

## 🎯 Fitur Utama

### 1. Exploratory Data Analysis (EDA)
- Analisis statistik deskriptif
- Visualisasi distribusi data
- Analisis korelasi
- Deteksi missing values dan outliers

### 2. Data Preprocessing
- Handling missing values
- Feature selection berdasarkan korelasi
- Label encoding untuk variabel kategorikal
- Data splitting dan scaling

### 3. Machine Learning Models
- **Linear Regression**: Model baseline
- **Decision Tree**: Model tree-based sederhana
- **Random Forest**: Ensemble method dengan multiple trees
- **Gradient Boosting**: Sequential ensemble learning
- **Support Vector Regression**: Model dengan kernel RBF
- **Ensemble Model**: Kombinasi model terbaik

### 4. Model Evaluation
- **Metrik**: MAE, RMSE, R² Score
- **Visualisasi**: Actual vs Predicted plots
- **Feature Importance**: Untuk tree-based models
- **Residuals Analysis**: Analisis error model

### 5. Comprehensive Visualization
- Perbandingan performa model
- Scatter plots prediksi vs aktual
- Feature importance charts
- Distribusi residuals
- Error analysis

## 📊 Expected Results

### Model Performance
- **R² Score**: 0.85 - 0.95 (sangat baik)
- **MAE**: $15,000 - $25,000 (tergantung dataset)
- **Best Model**: Biasanya Random Forest atau Gradient Boosting

### Key Insights
- Luas rumah (GrLivArea) biasanya fitur paling penting
- Kualitas keseluruhan (OverallQual) berpengaruh signifikan
- Lokasi (Neighborhood) mempengaruhi harga
- Model ensemble memberikan prediksi lebih stabil

## 🎓 Learning Objectives

1. **Data Science Workflow**: End-to-end ML project
2. **EDA Skills**: Analisis dan visualisasi data
3. **Preprocessing**: Cleaning dan feature engineering
4. **Model Comparison**: Multiple algorithms evaluation
5. **Ensemble Methods**: Combining models for better performance
6. **Model Interpretation**: Understanding feature importance

## 🔍 Troubleshooting

### Dataset Issues
- **File not found**: Notebook akan otomatis menggunakan dataset alternatif
- **Internet connection**: Dataset online mungkin tidak bisa diakses
- **Kaggle access**: Perlu akun Kaggle untuk download dataset utama

### Common Errors
- **Missing libraries**: Install dengan `pip install [library-name]`
- **Memory issues**: Reduce dataset size atau gunakan sampling
- **Encoding errors**: Pastikan file CSV dalam format UTF-8

## 📈 Extensions

### Possible Improvements
1. **Hyperparameter Tuning**: GridSearchCV, RandomizedSearchCV
2. **Feature Engineering**: Polynomial features, feature interactions
3. **Advanced Models**: XGBoost, LightGBM, Neural Networks
4. **Cross Validation**: K-fold CV untuk evaluasi lebih robust
5. **Model Deployment**: Flask/FastAPI untuk web service

### Advanced Analysis
1. **SHAP Values**: Model interpretability
2. **Learning Curves**: Training vs validation performance
3. **Feature Selection**: Recursive feature elimination
4. **Outlier Treatment**: Advanced outlier detection methods

## 📝 Notes

- Notebook dirancang untuk berjalan dengan atau tanpa dataset Kaggle
- Semua visualisasi menggunakan matplotlib dan seaborn
- Code dilengkapi dengan komentar dan penjelasan
- Hasil evaluasi ditampilkan dalam format yang mudah dipahami
- Project cocok untuk pembelajaran dan portfolio

## 🏆 Success Criteria

✅ **Completed Features**:
- [x] Comprehensive EDA
- [x] Multiple ML algorithms
- [x] Model evaluation dan comparison
- [x] Feature importance analysis
- [x] Ensemble modeling
- [x] Extensive visualization
- [x] Auto dataset fallback
- [x] Detailed documentation

**Happy Learning! 🚀**
