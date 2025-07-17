#  Netflix Kullanıcı Memnuniyeti Analizi

Bu proje, bir makine öğrenmesi uygulamasıdır ve Patika.dev'in "Veri Analizi Bootcamp" kapsamında geliştirilmiştir. Amaç, Netflix içerikleriyle ilgili bazı niteliklere bakarak kullanıcı memnuniyeti tahminlemesi yapmaktır.

##  Proje Hedefi

Kullanıcı memnuniyetini etkileyen faktörleri analiz ederek, en iyi sınıflandırma modelini oluşturmak ve önemli öznitelikleri belirlemektir.

---

## 🔧 Kullanılan Kütüphaneler

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

---

##  Uygulanan Adımlar

### 1. Veri Ön İşleme
- Eksik değerlerin analizi ve giderilmesi (`drop`, `fillna`)
- Kategorik verilerin `one-hot encoding` ile dönüştürülmesi

### 2. Veri Bölme
- %70 eğitim
- %15 doğrulama
- %15 test seti

### 3. Modelleme
- **Lojistik Regresyon**
  - Accuracy: ~0.96
  - F1 Score: ~0.94
- **Random Forest**
  - Accuracy: ~0.96
  - F1 Score: ~0.94

### 4. Feature Importance
- Random Forest ile en önemli değişkenler görselleştirildi.

---

##  Öznitelik Önem Grafiği

- En önemli değişken: `director_Bilinmiyor`
- Ardından gelenler: `duration_2 Seasons`, `release_year`, `duration_3 Seasons`...

---

##  Sonuç

Random Forest ve Lojistik Regresyon benzer doğruluk oranlarına ulaşmıştır. Random Forest, daha yorumlanabilir olduğu için tercih edilmiştir. Önemli değişkenlere odaklanarak veri toplama ve iyileştirme yapılabilir.

---

##  Proje Sahibi

Zeynep Melike Aydoğmuş  
 Süleyman Demirel Üniversitesi – Bilgisayar Mühendisliği  
 Patika.dev Veri Analizi Bootcamp

---

##  Proje Yapısı

```bash
 Netflix-Satisfaction-ML
 ┣  notebook.ipynb
 ┣  README.md
 ┗ dataset.csv
# Dataset kaggle.com'dan alınmıştır.
