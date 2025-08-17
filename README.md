# Balık Tür Tespit Modeli - YOLOv11

Bu proje, görüntüler üzerinde **balık türlerinin tespit edilmesi** amacıyla geliştirilmiştir.  
Modelde **YOLOv11** kullanılmıştır.  **Roboflow** üzerinden sağlanan özel bir dataset ile optimize edilmiştir.  

---

## Kullanılan Teknolojiler
- **YOLOv11 (Ultralytics)**
- **Python**
- **Google Colab (GPU Ortamı)**
- **Roboflow API**
- **CUDA (NVIDIA GPU)**

---

## Dataset
- Dataset, özel olup LabelImg ile etiketlenmiştir. **Roboflow** platformu üzerinden geliştirmeler yapılmıştır.  
- Eğitim, doğrulama ve test setleri dengeli şekilde hazırlanmıştır.  
- Görseller üzerinde balıkların baş, kuyruk ve tür bilgilerinin bulunduğu etiketler mevcuttur.  

---

## Eğitim Süreci
- Model, **100 epoch** boyunca eğitilmiştir.  
- Eğitim sürecinde Precision, Recall ve F1 skorları takip edilmiştir.  
- Eğitim çıktıları arasında:
  - **Precision, Recall, F1 Curves**
  - **Confusion Matrix**
  - **Eğitim & Doğrulama batch görselleri** yer almaktadır.

---


## Test Görselleri
![Prediction](runs/detect/train/val_batch0_pred.jpg)

---

## 📌 Notlar
- Bu proje balık tespiti için özelleştirilmiştir.  
- Eğitim süreci **Google Colab** ortamında, GPU desteği ile gerçekleştirilmiştir.  
- Sonuçlar, modelin balık nesnesini yüksek doğruluk oranıyla tespit edebildiğini göstermektedir.  


