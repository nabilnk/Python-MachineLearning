# 📊 Panduan Dataset Kaggle House Prices

## 🏠 Overview Dataset
Dataset **House Prices - Advanced Regression Techniques** dari Kaggle berisi data penjualan rumah di Ames, Iowa dari tahun 2006-2010. Dataset ini memiliki 79 fitur yang sangat detail untuk memprediksi harga rumah.

## 📋 Fitur Dataset (79 Fitur)

### 🏗️ **Karakteristik Properti Dasar**
- **MSSubClass**: Tipe bangunan (20=1-Story 1946+, 60=2-Story 1946+, dll)
- **MSZoning**: Zoning (RL=Residential Low Density, RM=Residential Medium, dll)
- **LotFrontage**: Panjang depan lot (feet)
- **LotArea**: Luas lot (square feet)
- **Street**: Tipe jalan (Grvl=Gravel, Pave=Paved)
- **LotShape**: Bentuk lot (Reg=Regular, IR1=Slightly irregular, dll)

### 🏘️ **Lokasi & Lingkungan**
- **Neighborhood**: 25 lokasi di Ames (Blmngtn, Blueste, BrDale, dll)
- **Condition1/2**: Kedekatan dengan fasilitas (Norm=Normal, Artery=Arterial street, dll)
- **BldgType**: Tipe bangunan (1Fam=Single-family, Duplx=Duplex, dll)

### 🏠 **Kualitas & Kondisi Bangunan**
- **OverallQual**: Kualitas keseluruhan (1=Very Poor, 10=Very Excellent)
- **OverallCond**: Kondisi keseluruhan (1=Very Poor, 10=Very Excellent)
- **YearBuilt**: Tahun dibangun
- **YearRemodAdd**: Tahun renovasi

### 🏗️ **Struktur Bangunan**
- **RoofStyle**: Gaya atap (Gable, Hip, Shed, dll)
- **RoofMatl**: Material atap (CompShg=Standard Shingle, Metal, dll)
- **Exterior1st/2nd**: Material eksterior (VinylSd, HdBoard, BrkFace, dll)
- **Foundation**: Tipe fondasi (PConc=Poured Concrete, CBlock, dll)

### 🏠 **Ukuran & Ruangan**
- **1stFlrSF**: Luas lantai 1 (sq ft)
- **2ndFlrSF**: Luas lantai 2 (sq ft)
- **GrLivArea**: Luas area tinggal di atas tanah (sq ft)
- **BedroomAbvGr**: Jumlah kamar tidur di atas tanah
- **FullBath**: Jumlah kamar mandi lengkap
- **HalfBath**: Jumlah kamar mandi setengah
- **KitchenAbvGr**: Jumlah dapur di atas tanah

### 🏠 **Basement**
- **BsmtQual**: Kualitas basement (Ex=Excellent, Gd=Good, TA=Typical, dll)
- **BsmtCond**: Kondisi basement
- **BsmtExposure**: Eksposur basement (Gd=Good, Av=Average, dll)
- **BsmtFinType1/2**: Tipe finishing basement
- **BsmtFinSF1/2**: Luas basement yang sudah di-finish
- **BsmtUnfSF**: Luas basement yang belum di-finish
- **TotalBsmtSF**: Total luas basement

### 🚗 **Garasi**
- **GarageType**: Tipe garasi (Attchd=Attached, Detchd=Detached, dll)
- **GarageYrBlt**: Tahun garasi dibangun
- **GarageFinish**: Finishing garasi (Fin=Finished, Unf=Unfinished)
- **GarageCars**: Kapasitas mobil di garasi
- **GarageArea**: Luas garasi (sq ft)
- **GarageQual/Cond**: Kualitas dan kondisi garasi

### 🔥 **Fasilitas Tambahan**
- **Fireplaces**: Jumlah perapian
- **FireplaceQu**: Kualitas perapian (Ex=Excellent, Gd=Good, TA=Average, dll)
- **PoolArea**: Luas kolam renang (sq ft)
- **PoolQC**: Kualitas kolam renang
- **Fence**: Kualitas pagar (GdPrv=Good Privacy, MnPrv=Minimum Privacy, dll)
- **MiscFeature**: Fitur tambahan (Elev=Elevator, Gar2=2nd Garage, Shed, dll)

### 🏡 **Area Outdoor**
- **WoodDeckSF**: Luas deck kayu (sq ft)
- **OpenPorchSF**: Luas teras terbuka (sq ft)
- **EnclosedPorch**: Luas teras tertutup (sq ft)
- **3SsnPorch**: Luas teras 3 musim (sq ft)
- **ScreenPorch**: Luas teras berjaring (sq ft)

### 🏠 **Sistem & Utilitas**
- **Heating**: Tipe pemanas (GasA=Gas forced air, GasW=Gas hot water, dll)
- **HeatingQC**: Kualitas pemanas
- **CentralAir**: AC sentral (Y=Yes, N=No)
- **Electrical**: Sistem listrik (SBrkr=Standard Circuit Breakers, dll)

### 💰 **Informasi Penjualan**
- **MoSold**: Bulan terjual (1-12)
- **YrSold**: Tahun terjual (2006-2010)
- **SaleType**: Tipe penjualan (WD=Warranty Deed, New=New Home, dll)
- **SaleCondition**: Kondisi penjualan (Normal, Abnormal, Family, dll)
- **SalePrice**: Harga jual (TARGET VARIABLE)

## 🎯 **Fitur Paling Penting untuk Modeling**

### 📊 **Top Fitur Berdasarkan Korelasi**
1. **OverallQual** (0.79): Kualitas keseluruhan rumah
2. **GrLivArea** (0.71): Luas area tinggal
3. **GarageCars** (0.64): Kapasitas garasi
4. **GarageArea** (0.62): Luas garasi
5. **TotalBsmtSF** (0.61): Total luas basement
6. **1stFlrSF** (0.61): Luas lantai 1
7. **FullBath** (0.56): Jumlah kamar mandi lengkap
8. **TotRmsAbvGrd** (0.53): Total ruangan di atas tanah
9. **YearBuilt** (0.52): Tahun dibangun
10. **YearRemodAdd** (0.51): Tahun renovasi

### 🏘️ **Fitur Kategorikal Penting**
- **Neighborhood**: Lokasi sangat berpengaruh pada harga
- **ExterQual**: Kualitas material eksterior
- **KitchenQual**: Kualitas dapur
- **BsmtQual**: Kualitas basement
- **MSZoning**: Zoning area

## 📈 **Insights Dataset**

### 💵 **Distribusi Harga**
- **Rata-rata**: ~$180,000
- **Median**: ~$163,000
- **Range**: $34,900 - $755,000
- **Distribusi**: Right-skewed (banyak rumah murah, sedikit rumah mahal)

### 🏠 **Karakteristik Umum**
- **Luas rata-rata**: ~1,500 sq ft
- **Umur rata-rata**: ~35 tahun (built ~1971)
- **Garasi**: 85% rumah punya garasi
- **Basement**: 90% rumah punya basement

### 🏘️ **Neighborhood Insights**
- **Termahal**: StoneBr, NridgHt, NoRidge (~$300k+)
- **Termurah**: MeadowV, IDOTRR, BrDale (~$100k)
- **Paling populer**: NAmes, CollgCr, OldTown

## 🔧 **Tips Preprocessing**

### 🚫 **Missing Values Strategy**
- **High Missing** (>50%): PoolQC, MiscFeature, Alley, Fence → Drop atau fill 'None'
- **Medium Missing** (15-50%): FireplaceQu, LotFrontage → Fill dengan median/mode
- **Low Missing** (<15%): GarageYrBlt, MasVnrArea → Fill dengan median

### 🏷️ **Encoding Strategy**
- **Ordinal**: OverallQual, ExterQual, BsmtQual (1-10 atau Poor-Excellent)
- **Nominal**: Neighborhood, MSZoning, SaleType → Label/One-hot encoding
- **Binary**: CentralAir, PavedDrive → 0/1

### 📊 **Feature Engineering Ideas**
- **TotalSF**: 1stFlrSF + 2ndFlrSF + TotalBsmtSF
- **HouseAge**: YrSold - YearBuilt
- **RemodAge**: YrSold - YearRemodAdd
- **TotalBath**: FullBath + 0.5*HalfBath + BsmtFullBath + 0.5*BsmtHalfBath
- **HasPool**: PoolArea > 0
- **HasGarage**: GarageArea > 0

## 🎯 **Expected Model Performance**
- **Baseline (Linear)**: R² ~0.70-0.75
- **Tree-based (RF/GB)**: R² ~0.85-0.90
- **Advanced (XGB/Ensemble)**: R² ~0.90-0.95
- **Competition Winner**: R² ~0.95+ (dengan feature engineering ekstensif)

## 📝 **Catatan Penting**
- Dataset dari Ames, Iowa → hasil mungkin tidak general untuk kota lain
- Periode 2006-2010 → perlu adjustment untuk kondisi pasar saat ini
- Beberapa fitur sangat spesifik → butuh domain knowledge real estate
- Missing values banyak → perlu strategi handling yang tepat
