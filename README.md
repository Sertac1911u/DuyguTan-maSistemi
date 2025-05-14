#  Duygu Tanıma Sistemi

## Proje Açıklaması
Bu proje, Namık Kemal Üniversitesi Bilgisayar Mühendisliği Bölümü BMSB402 - Görüntü İşleme dersi kapsamında, Doç. Dr. Ahmet Saygılı danışmanlığında, proje hazırlama ödevi olarak gerçekleştirilmiştir.

Projenin temel amacı, görüntü işleme tekniklerini gerçek zamanlı uygulamalara entegre ederek, insan yüzü tespiti ve duygu analizi gibi alanlarda öğrencilere pratik deneyim kazandırmaktır. Python dili kullanılarak geliştirilen bu sistemde, OpenCV kütüphanesi ile yüz algılama işlemleri gerçekleştirilmiş, DeepFace kütüphanesi ile de yedi temel insan duygusu analiz edilmiştir.

Uygulama, bilgisayar kamerası üzerinden alınan görüntülerde yüzleri tespit eder ve her bir yüz bölgesi için duygu analizi yaparak ekrana anlık sonuçları yansıtır. Proje; insan-bilgisayar etkileşimi, güvenlik sistemleri, kullanıcı analizi gibi birçok alanda uygulanabilir temel bir görüntü işleme uygulamasını modellemektedir.

Bu çalışma, öğrencilerin görüntü işleme tekniklerini yapay zekâ kütüphaneleri ile birleştirerek gerçek dünya problemlerine yönelik çözümler üretme becerilerini geliştirmeyi hedeflemektedir. Projenin sonunda geliştirilen sistem, gerçek zamanlı analiz yapabilen, kullanıcı dostu ve işlevsel bir duygu tanıma aracı olarak çalışmaktadır.


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
```

### Uygulamayı Başlatmak için:
```bash
python emotion_detector.py
```

### Çıkmak için:
q tuşuna basmanız yeterlidir.

## Demo Videosu
https://drive.google.com/file/d/1KGw2SPB6-2toi8SmXsaqYOyovRevVHHa/view?usp=sharing

## Katkıda Bulunanlar
2210656010 Kadir Han YARTAŞI   
2210656033 Abdülkerim AKTAŞ

