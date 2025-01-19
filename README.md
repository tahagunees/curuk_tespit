# Fruit Detection with YOLOv8

Bu proje, **YOLOv8** kullanarak meyve tespiti yapmak için geliştirilmiştir. Modelin eğitimi ve çalıştırılması için gerekli kütüphaneler **requirements.txt** dosyasında belirtilmiştir.

## 🚀 Kurulum

Projeyi çalıştırmak için aşağıdaki adımları takip edebilirsin:

### 1️⃣ Gerekli Kütüphaneleri Kur
```bash
pip install -r requirements.txt
```

### 2️⃣ Modeli Çalıştır
Eğer modelin eğitimini veya testini yapmak istiyorsan, aşağıdaki komutları kullanabilirsin:
```bash
# Modelin eğitimi
python train.py --data dataset.yaml --epochs 50(değiştirilebilir --weights yolov8n.pt

# Modeli test etme
python detect.py --source test_images/ --weights best.pt --conf 0.5
```

## 📂 Dosya Yapısı
```
fruit-detect/
│── data/                  # Eğitim ve test verileri
│── models/                # Eğitilmiş modeller
│── scripts/               # Yardımcı Python dosyaları
│── requirements.txt       # Gerekli Python kütüphaneleri
│── README.md              # Proje dökümantasyonu
```

## 📌 Bağımlılıklar
Bu proje aşağıdaki ana kütüphaneleri kullanmaktadır:
- **Ultralytics YOLOv8** (`ultralytics==8.0.196`)
- **PyTorch** (`torch>=1.13.1`, `torchvision>=0.14.1`)
- **NumPy** (`numpy>=1.22.0`)
- **Matplotlib** (`matplotlib>=3.7.1`)
- **OpenCV** (`opencv-python>=4.7.0.72`)
- **Google Colab** (`google-colab`)
- **IPython Kernel** (`ipykernel`)

## 🛠 Geliştirme Ortamı
Proje, **Google Colab** ve **Jupyter Notebook** desteğiyle geliştirilebilir.

## 📜 Lisans
Bu proje açık kaynaklıdır. Kullanırken kaynak göstermeyi unutmayın! 😊

