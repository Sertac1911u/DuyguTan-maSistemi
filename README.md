#  Duygu Tanıma Sistemi

## Proje Açıklaması
Bu proje, bilgisayar kamerası üzerinden alınan görüntülerde insan yüzlerini algılayarak duygularını analiz eden gerçek zamanlı bir görüntü işleme uygulamasıdır. OpenCV ile yüz algılama yapılırken, DeepFace kütüphanesi kullanılarak yedi temel duygunun tespiti gerçekleştirilmiştir.

## Amaç
- Görüntü işleme konularını yapay zekâ ile entegre etmek
- Gerçek zamanlı yüz ve duygu tanıma uygulaması geliştirmek
- OpenCV ve DeepFace gibi güçlü kütüphaneleri pratikte kullanmak

## Kullanılan Teknolojiler
- Python 3.x
- OpenCV (cv2)
- DeepFace
- Haar Cascade Classifier

## Uygulama Akışı
1. Bilgisayar kamerası `cv2.VideoCapture(0)` ile açılır.
2. Görüntü gri formata çevrilir (`cv2.cvtColor`).
3. Haar Cascade sınıflandırıcısı ile yüzler algılanır.
4. Algılanan her yüz `DeepFace.analyze()` ile analiz edilir.
5. Tespit edilen duygu etiketi, yüz üzerine kutu ve metin olarak çizilir.

## Tanınan Duygular
- Happy
- Sad
- Angry
- Fear
- Surprise
- Disgust
- Neutral

## Kurulum ve Çalıştırma

### Gerekli Kurulumlar:
```bash
pip install opencv-python deepface

Uygulamayı Başlatmak için:
```bash
python emotion_detector.py

Çıkmak için:
q tuşuna basmanız yeterlidir.

## Demo Videosu
https://drive.google.com/file/d/1KGw2SPB6-2toi8SmXsaqYOyovRevVHHa/view?usp=sharing

## Katkıda Bulunanlar
2210656010 Kadir Han YARTAŞI   
2210656033 Abdülkerim AKTAŞ

