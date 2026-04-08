# Pima Indians Diabetes Prediction with AdaBoost 🩺

Bu proje, Kaggle üzerindeki **Pima Indians Diabetes** veri setini kullanarak makine öğrenmesi teknikleriyle diyabet tahmini yapmayı amaçlar. Veri setindeki eksik değerlerin giderilmesi, model seçimi ve hiperparametre optimizasyonu süreçlerini içerir.

## 📊 Proje Özeti

Proje aşamasında veri setindeki mantıksal hatalar giderilmiş ve topluluk öğrenme (ensemble learning) yöntemlerinden biri olan **AdaBoost** algoritması kullanılmıştır. Model performansı **GridSearchCV** ile optimize edilmiştir.

* **Veri Seti:** [Kaggle - Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
* **Model:** AdaBoost Classifier
* **Başarı Skoru:** %77 Accuracy

---

## 🛠️ Uygulanan İşlemler

### 1. Veri Temizleme (Data Cleaning)
Veri setinde Glikoz, Kan Basıncı ve BMI gibi sütunlarda bulunan **0 değerleri** (mantıksal olarak imkansız olan veriler) tespit edilmiştir. Bu değerler veri setinin genel dağılımını korumak adına:
* İlgili özelliklerin **medyan (median)** değerleri ile doldurulmuştur.

### 2. Model Eğitimi ve Optimizasyon
* **Algoritma:** AdaBoost Classifier seçilerek başlangıç eğitimi yapılmıştır.
* **Hiperparametre Ayarı:** `GridSearchCV` kullanılarak en iyi `learning_rate` ve `n_estimators` parametreleri aranmıştır.
* **Final Model:** Bulunan en iyi parametreler ile model yeniden eğitilerek test edilmiştir.

### 3. Sonuçlar
Model, optimizasyon işlemlerinin ardından test verisi üzerinde **%77** başarı oranına ulaşmıştır.

---

## 🚀 Kullanılan Teknolojiler

* **Python 3.x**
* **Pandas & NumPy** (Veri Analizi)
* **Scikit-Learn** (Makine Öğrenmesi)
* **Matplotlib / Seaborn** (Görselleştirme)

---

## 📂 Kurulum ve Çalıştırma

1. Repoyu klonlayın:
   ```bash
   git clone [https://github.com/kullaniciadi/repo-ismi.git](https://github.com/kullaniciadi/repo-ismi.git)
