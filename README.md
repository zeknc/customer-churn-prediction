# 🎯 Customer Churn Prediction

E-ticaret müşterilerinin churn (kayıp) tahminini makine öğrenmesi ile gerçekleştiren bir veri bilimi projesi.

## 📊 Proje Hakkında

Bu proje, bir telekom şirketinin müşteri verilerini kullanarak hangi müşterilerin şirketten ayrılma (churn) olasılığının yüksek olduğunu tahmin eder.

**Proje Hedefleri:**
- Müşteri kayıp oranını (churn rate) analiz etmek
- Churn'ü etkileyen faktörleri belirlemek
- Makine öğrenmesi modelleri ile yüksek doğrulukta tahmin yapmak
- İnteraktif bir dashboard ile sonuçları görselleştirmek

## 🛠️ Kullanılan Teknolojiler

- **Python 3.10**
- **Pandas & NumPy** - Veri manipülasyonu ve analiz
- **Scikit-learn** - Makine öğrenmesi modelleri
- **XGBoost** - Gradient boosting algoritması
- **Matplotlib & Seaborn** - Veri görselleştirme
- **Streamlit** - İnteraktif web dashboard
- **Plotly** - Dinamik grafikler

## 📁 Proje Yapısı
```
customer-churn-prediction/
│
├── data/
│   ├── raw/              # Ham veri dosyaları
│   └── processed/        # İşlenmiş veri
│
├── notebooks/            # Jupyter notebook'lar
│   ├── 01_eda.ipynb
│   ├── 02_preprocessing.ipynb
│   └── 03_modeling.ipynb
│
├── src/                  # Python kaynak kodları
│   ├── data_processing.py
│   └── model.py
│
├── app/                  # Streamlit dashboard
│   └── dashboard.py
│
├── models/               # Eğitilmiş modeller
│
├── requirements.txt      # Gerekli kütüphaneler
└── README.md
```

## 🚀 Kurulum
```bash
# Repository'yi klonla
git clone https://github.com/zeknc/customer-churn-prediction.git

# Proje klasörüne gir
cd customer-churn-prediction

# Gerekli kütüphaneleri yükle
pip install -r requirements.txt
```

## 📊 Veri Seti

Kaggle'dan alınan Telco Customer Churn veri seti kullanılmıştır.
- 7043 müşteri kaydı
- 21 özellik
- Hedef değişken: Churn (Yes/No)

## 🔍 Analiz Adımları

1. **Keşifsel Veri Analizi (EDA)**
   - Veri kalitesi kontrolü
   - İstatistiksel analizler
   - Görselleştirmeler

2. **Veri Ön İşleme**
   - Eksik veri yönetimi
   - Kategorik değişken kodlama
   - Feature engineering
   - Veri normalizasyonu

3. **Model Geliştirme**
   - Logistic Regression
   - Random Forest
   - XGBoost
   - Model karşılaştırması

4. **Model Değerlendirme**
   - Accuracy, Precision, Recall, F1-Score
   - ROC-AUC analizi
   - Feature importance

## 📈 Sonuçlar

*(Proje tamamlandığında güncellenecek)*

## 🎯 Dashboard

*(Streamlit dashboard linki eklenecek)*

## 👨‍💻 Geliştirici

**Zehra Ekinci**
- GitHub: (https://github.com/zeknc)
- LinkedIn: [(https://www.linkedin.com/in/zehra-ekinci-264496253/)]
- Email: zhrekncr7@gmail.com

## 📝 Lisans

Bu proje MIT lisansı altındadır.

## 🙏 Teşekkürler

Bu proje, veri bilimi portföyümün bir parçası olarak geliştirilmiştir.# customer-churn-prediction
Makine öğrenimi kullanarak e-ticaret müşteri kaybı tahmini
