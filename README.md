# 🔐 Kullanıcı Şifre Davranışlarının Güvenlik Perspektifinden İncelenmesi

Bu proje, büyük veri analizi ve makine öğrenmesi yöntemleriyle kullanıcıların şifre belirleme alışkanlıklarını incelemeyi amaçlamaktadır. Gerçek dünya şifre veri setleri kullanılarak yapılan bu çalışmada hem istatistiksel analizler gerçekleştirilmiş hem de şifrelerin zayıf, orta veya güçlü olarak sınıflandırılması için yapay zeka modelleri geliştirilmiştir.

---

## 📁 Proje İçeriği

### 📊 `big_data_analyzing.ipynb`
Kullanıcı şifreleri üzerinde istatistiksel analizler gerçekleştiren not defteridir. İçerdiği bazı analizler:
- En sık kullanılan harfler, rakamlar, semboller
- Şifre uzunluk dağılımı
- Karakter türü ve karakter sınıfı dağılımları
- Şifre kalıpları ve doğum yılı analizleri
- Kelime bulutu görselleştirmesi

### 🤖 `big_data_machine_learning.ipynb`
Etiketlenmiş şifre veri seti kullanılarak şifrelerin zayıf/orta/güçlü olarak sınıflandırıldığı makine öğrenmesi modelleme not defteridir. İçerdiği modeller:
- Random Forest  
- XGBoost  
- KNN  
- Logistic Regression  
- Gradient Boosting  
- LightGBM  
- Convolutional Neural Network (CNN)

> Hiperparametre optimizasyonu için **RandomizedSearchCV** yöntemi kullanılmıştır.

Ayrıca Gradio arayüzü ile etkileşimli bir demo oluşturulmuştur.

---

## 🧠 Kullanılan Veri Setleri

1. **VimeWorld Şifre Veri Seti**  
   Kullanıcı davranışlarını analiz etmek için kullanıldı.  
   [🔗 Kaggle Linki](https://www.kaggle.com/datasets/tempuserpavelbiz/leaked-passwords-of-the-vimeworld-minecraft-server)

2. **Etiketli Şifre Gücü Veri Seti**  
   Makine öğrenmesi modellerini eğitmek için kullanıldı.  
   [🔗 Kaggle Linki](https://www.kaggle.com/datasets/rouhalahebrahimi/common-passwords-dataset-for-machine-learning)

---

## 🧪 Modellerin Başarı Oranları (Accuracy)

| Model                  | Accuracy  |
|------------------------|-----------|
| Random Forest          | 0.9950    |
| XGBoost                | 0.9950    |
| KNN                    | 0.9910    |
| Logistic Regression    | 0.9414    |
| Gradient Boosting      | 0.9945    |
| LightGBM               | 0.9949    |
| CNN                    | 0.9943    |

---

## 🚀 Gradio Arayüzü

Projede ayrıca bir **Gradio arayüzü** geliştirilmiştir. Kullanıcılar bir şifre girdiklerinde, tüm modellerin bu şifreyi zayıf, orta veya güçlü olarak hangi olasılıkla sınıflandırdığını görebilirler.

---

## 📌 Kullanılan Teknolojiler

- Python 3.x
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn, XGBoost, LightGBM
- TensorFlow / Keras
- Gradio
- Google Colab

---
