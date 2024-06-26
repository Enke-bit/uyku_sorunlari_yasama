
# Veri Seti

Veri seti liki: https://www.kaggle.com/datasets/henryshan/sleep-health-and-lifestyle

Veri seti aşağıdaki özellikleri içermektedir:

Person ID: Kişiye özel kimlik numarası.

Gender: Cinsiyet (0: Kadın, 1: Erkek).

Age: Yaş.

Occupation: Meslek kategorisi.

Sleep Duration: Günlük uyku süresi (saat cinsinden).

Quality of Sleep: Uyku kalitesi (ölçek: 0-10).

Physical Activity Level: Fiziksel aktivite düzeyi (ölçek: 0-10).

Stress Level: Stres düzeyi (ölçek: 0-10).

BMI Category: Vücut kitle indeksi kategorisi (normal, kilolu, obez).

Blood Pressure: Kan basıncı (format: "Systolic/Diastolic").

Heart Rate: Kalp atış hızı (bpm).

Daily Steps: Günlük adım sayısı.

Sleep Disorder: Uyku bozukluğu var mı? (0: Yok, 1: Var)

# Model Oluşturma
Veri seti üzerinde lojistik regresyon modeli kullanılarak 'Sleep Disorder' tahmini yapılmıştır. Aşağıda modelin performansı ve katsayılarına ilişkin detaylar bulunmaktadır:

# Model Performansı
Accuracy Score: 0.871

# Confusion Matrix
[[11  2]
 [ 2 16]]

## Classification Report
              precision    recall  f1-score   support

         0       0.85      0.85      0.85        13
         1       0.89      0.89      0.89        18


 # Accuracy 
  
  accuracy                           0.87        31
 macro avg       0.87      0.87      0.87        31



### Özellik Katsayıları

- **Person ID**: -0.437
- **Gender**: -0.254
- **Age**: 0.128
- **Occupation**: 0.914
- **Sleep Duration**: 0.067
- **Quality of Sleep**: -0.128
- **Physical Activity Level**: 0.011
- **Stress Level**: 0.025
- **BMI Category**: -0.364
- **Heart Rate**: 0.704
- **Daily Steps**: 1.047
- **Sleep Disorder**: 0.903

## Model Değerlendirme

Model, veri setindeki özellikler kullanılarak 'Sleep Disorder' varlığını tahmin etmek için oluşturulmuştur. Accuracy skoru %87 ile iyi bir performans göstermektedir ve sınıflandırma raporu da doğruluk, hassasiyet ve geri çağırma değerlerini detaylandırmaktadır.

Bu README dosyası modelin oluşturulması ve değerlendirilmesi sürecini açıklamakta olup, veri seti ve model performansıyla ilgili detaylı bilgiler sağlamaktadır.

---
