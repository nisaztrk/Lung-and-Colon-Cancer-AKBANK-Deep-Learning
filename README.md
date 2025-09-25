# Lung and Colon Cancer Classification (AKBANK Deep Learning)

## 📌 Projenin Amacı
Bu projenin temel amacı, **akciğer ve kolon kanseri histopatolojik görüntülerini derin öğrenme yöntemleriyle sınıflandırmak** ve tıbbi görüntü analizi alanında yapay zekâ tabanlı bir karar destek sistemi oluşturmaktır.  
Çalışmanın hedefi, kanser teşhisinde doğruluk oranını artırmak, erken tanıya katkıda bulunmak ve sağlık alanında derin öğrenmenin gücünü ortaya koymaktır. 

Kaggle Notebook Çalışma: https://www.kaggle.com/code/nisaztrkk/lung-and-colon-cancer-akbank-deep-learning

## 📂 Veri Seti
- **Kaynak:** [Kaggle – Lung and Colon Cancer Histopathological Images](https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images)  
- **İçerik:** Akciğer ve kolon kanserine ait histopatolojik görüntüler.  
- **Boyut:** ~25.000 görüntü, 5 sınıf.  

## 🧠 Kullanılan Yöntemler
- Veri ön işleme (normalizasyon, yeniden boyutlandırma, veri artırma).  
- Convolutional Neural Networks (CNN) tabanlı derin öğrenme mimarileri.  
- Hiperparametre optimizasyonu denemeleri (öğrenme oranı, dropout, optimizer vs.).  
- TensorFlow/Keras kütüphaneleri ile model eğitimi.  

## 📊 Elde Edilen Sonuçlar
Modelin eğitim sürecinde ulaşılan temel başarımlar:  

- **CNN (Veri ön işleme sonrası):**  
  - Eğitim doğruluğu: **%94.4**  
  - Doğrulama doğruluğu: **%95.2**  
  - Kayıp (loss): 0.14 – 0.12 aralığında  

- **Hiperparametre Optimizasyonu Denemeleri:**  
  - İlk denemelerde doğrulama doğruluğu ~%86 seviyesinde kaldı.  
  - En iyi optimizasyon denemesinde doğrulama doğruluğu **%89.7** elde edildi.  
  - **CNN modeli**, hiperparametre denemelerinden daha yüksek başarı sağlamıştır.  

📌 Bu sonuçlar, CNN tabanlı yaklaşımın akciğer ve kolon kanseri histopatolojik görüntülerinin sınıflandırılmasında etkili bir yöntem olduğunu göstermektedir.  

Gerekli kütüphaneyi yükleyin:
pip install -r requirements.txt

Modeli eğitmek için:
python train.py

Tekil bir görüntü üzerine tahmin yapmak için:
python predict.py --image <path_to_image>


