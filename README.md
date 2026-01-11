# 🎯 Customer Churn Prediction - Müşteri Kaybı Tahmin Sistemi

[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3.0-orange.svg)](https://scikit-learn.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28-red.svg)](https://streamlit.io/)

E-ticaret ve telekom sektöründeki müşteri kayıplarını (churn) makine öğrenmesi ile tahmin eden end-to-end veri bilimi projesi.

---

## 📋 Proje Özeti

Bu proje, bir telekom şirketinin 7000+ müşteri verisini kullanarak hangi müşterilerin şirketten ayrılma (churn) olasılığının yüksek olduğunu **%80+ doğrulukla** tahmin eder.

### 🎯 Proje Hedefleri
- Müşteri kaybı riskini erken tespit etmek
- Churn'ü etkileyen faktörleri belirlemek
- İnteraktif bir dashboard ile tahmin sistemi sunmak
- Şirketlere müşteri sadakatini artırma stratejileri önermek

---

## 🚀 Özellikler

✅ **Kapsamlı Veri Analizi (EDA)**
- 21 farklı müşteri özelliğinin detaylı analizi
- İstatistiksel testler (Chi-Square, T-Test)
- 15+ görselleştirme

✅ **3 Farklı Makine Öğrenmesi Modeli**
- Logistic Regression
- Random Forest
- XGBoost (En iyi performans: %80.5 accuracy)

✅ **Feature Engineering**
- Tenure grupları
- Ortalama aylık harcama
- Ücret oranları

✅ **İnteraktif Web Dashboard**
- Streamlit ile geliştirilmiş
- Gerçek zamanlı churn tahmini
- Risk skorlama sistemi
- Görsel raporlama

---

## 📊 Model Performansı

| Model | Accuracy | Precision | Recall | F1-Score | AUC |
|-------|----------|-----------|--------|----------|-----|
| Logistic Regression | 78.0% | 0.65 | 0.52 | 0.55 | 0.84 |
| Random Forest | 79.0% | 0.66 | 0.55 | 0.58 | 0.85 |
| **XGBoost** | **80.5%** | **0.67** | **0.54** | **0.60** | **0.86** |

🏆 **XGBoost** modeli en iyi performansı göstermiştir.

---

## 🔍 Önemli Bulgular

### En Önemli Churn Risk Faktörleri:
1. **Sözleşme Tipi:** Aylık sözleşmesi olanlar %42 churn (2 yıllık: %3)
2. **Müşteri Süresi:** İlk 12 ayda churn riski %50+
3. **İnternet Servisi:** Fiber optic kullanıcıları %41 churn
4. **Ödeme Yöntemi:** Electronic check kullananlar %45 churn
5. **Aylık Ücret:** $70+ ödemeler yüksek risk

### 💡 İş Önerileri:
- İlk 12 aydaki müşterilere özel destek programı
- Aylık sözleşmelilere uzun vadeli sözleşme teşviki
- Fiber optic kullanıcılarına hizmet kalitesi iyileştirme
- Otomatik ödeme teşvikleri

---

## 🛠️ Kullanılan Teknolojiler

### Veri İşleme & Analiz
- **Python 3.10**
- **Pandas** - Veri manipülasyonu
- **NumPy** - Sayısal hesaplamalar
- **Matplotlib & Seaborn** - Görselleştirme

### Makine Öğrenmesi
- **Scikit-learn** - ML modelleri ve preprocessing
- **XGBoost** - Gradient boosting
- **Imbalanced-learn** - Dengesiz veri yönetimi

### Web Dashboard
- **Streamlit** - İnteraktif web uygulaması
- **Plotly** - Dinamik grafikler

### Araçlar
- **Jupyter Notebook** - Analiz ve modelleme
- **Git & GitHub** - Versiyon kontrolü
- **Kaggle** - Veri kaynağı

---

## 📁 Proje Yapısı
```
customer-churn-prediction/
│
├── data/
│   ├── raw/                          # Ham veri (CSV)
│   └── processed/                    # İşlenmiş veri (PKL)
│
├── notebooks/
│   ├── 01_eda.ipynb                 # Keşifsel veri analizi
│   └── 02_preprocessing_modeling.ipynb  # Veri işleme ve modelleme
│
├── models/
│   ├── random_forest_model.pkl      # Random Forest modeli
│   ├── xgboost_model.pkl            # XGBoost modeli
│   └── scaler.pkl                   # StandardScaler
│
├── app/
│   └── dashboard.py                 # Streamlit dashboard
│
├── requirements.txt                 # Gerekli kütüphaneler
└── README.md
```

---

## 🚀 Kurulum ve Çalıştırma

### 1. Repository'yi Klonla
```bash
git clone https://github.com/zeknc/customer-churn-prediction.git
cd customer-churn-prediction
```

### 2. Gerekli Kütüphaneleri Yükle
```bash
pip install -r requirements.txt
```

### 3. Veri Setini İndir
- [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- `WA_Fn-UseC_-Telco-Customer-Churn.csv` dosyasını `data/raw/` klasörüne kaydet

### 4. Jupyter Notebook'ları Çalıştır
```bash
jupyter notebook
# notebooks/01_eda.ipynb ve 02_preprocessing_modeling.ipynb dosyalarını sırayla çalıştır
```

### 5. Dashboard'u Çalıştır
```bash
cd app
streamlit run dashboard.py
```

Dashboard otomatik olarak tarayıcıda açılacaktır: `http://localhost:8501`

---

## 📊 Dashboard Kullanımı

### 📈 Veri Analizi Sekmesi
- Genel müşteri istatistikleri
- Churn dağılımı grafikleri
- Sözleşme tipi analizleri

### 🤖 Model Tahmini Sekmesi
1. Müşteri bilgilerini girin (cinsiyet, sözleşme tipi, ücret vb.)
2. "Tahmin Yap" butonuna tıklayın
3. Churn riskini ve önerileri görün

### 📊 Model Performansı Sekmesi
- Model karşılaştırma grafikleri
- Performans metrikleri
- En iyi model bilgisi

---

## 📈 Sonuçlar ve Etkiler

### İş Etkisi
- **%27 churn oranı** tespit edildi
- **%80.5 doğrulukla** risk tahmini yapılıyor
- **İlk 12 ay** kritik dönem olarak belirlendi
- **4 ana risk faktörü** tanımlandı

### Teknik Başarılar
- End-to-end ML pipeline oluşturuldu
- 3 farklı model karşılaştırıldı
- Feature engineering ile performans artırıldı
- Production-ready dashboard geliştirildi

---

## 🎓 Öğrenilen Konular

Bu proje kapsamında:
- ✅ Gerçek dünya veri analizi
- ✅ İstatistiksel hipotez testleri
- ✅ Veri ön işleme teknikleri
- ✅ Makine öğrenmesi model geliştirme
- ✅ Model değerlendirme ve karşılaştırma
- ✅ Web uygulaması geliştirme
- ✅ Git/GitHub kullanımı

---

## 🔮 Gelecek Geliştirmeler

- [ ] Daha fazla model deneme (CatBoost, LightGBM)
- [ ] Hyperparameter tuning (GridSearch, Optuna)
- [ ] SHAP values ile model açıklanabilirliği
- [ ] Real-time prediction API
- [ ] Docker containerization
- [ ] Cloud deployment (AWS/Azure)
- [ ] A/B testing simulasyonu

---

## 👨‍💻 Geliştirici

**İsim:** Zehra Ekinci
**LinkedIn:** (https://www.linkedin.com/in/zehra-ekinci-264496253/)
**Email:** zhrekncr7@gmail.com  
**GitHub:** [@zeknc](https://github.com/zeknc)

---

## 📝 Lisans

Bu proje MIT lisansı altındadır.

---

## 🙏 Teşekkürler

- **Veri Kaynağı:** [Kaggle - Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **İlham:** Gerçek dünya veri bilimi problemleri

---

## 📞 İletişim

Sorularınız veya geri bildirimleriniz için:
- GitHub Issues açabilirsiniz
- LinkedIn'den mesaj gönderebilirsiniz

---

**⭐ Projeyi beğendiyseniz yıldız vermeyi unutmayın!**

---

*Son Güncelleme: Ocak 2025*
