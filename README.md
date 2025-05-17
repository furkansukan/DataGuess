## 🔍 Proje Özeti

* **Amaç:** Görüntülerdeki yangınları gerçek zamanlı olarak tespit etmek.
* **Teknolojiler:** Python, YOLOv8, OpenCV.
* **Model:** Eğitilmiş YOLOv8 modeli (`best.pt`).
* **Kullanım Alanları:** Endüstriyel tesisler, orman yangını izleme sistemleri, güvenlik kameraları.

---

## 📁 Proje Dosya Yapısı

* `app.py`: Uygulamanın ana dosyası. YOLOv8 modelini yükler ve görüntü üzerinde yangın tespiti yapar.
* `main.py`: Alternatif bir giriş noktası; modelin nasıl kullanılacağını gösterir.
* `fire-detection.ipynb`: Jupyter Notebook formatında, modelin nasıl çalıştığını adım adım gösterir.
* `best.pt`: Eğitilmiş YOLOv8 model ağırlıkları.
* `fire.jpeg`: Test görüntüsü.
* `requirements.txt`: Gerekli Python kütüphanelerinin listesi.

---

## 🧠 Model Eğitimi ve Kullanımı

Proje, önceden eğitilmiş bir YOLOv8 modelini kullanır. Model, yangın içeren ve içermeyen görüntülerle eğitilmiştir. Kullanıcı, `app.py` dosyasını çalıştırarak modelin bir görüntüde yangın tespiti yapmasını sağlayabilir.

---

## 🛠️ Kurulum ve Çalıştırma

1. **Gerekli Kütüphaneleri Kurun:**

   ```bash
   pip install -r requirements.txt
   ```



2. **Uygulamayı Çalıştırın:**

   ```bash
   python app.py
   ```



Bu komut, `fire.jpeg` dosyasını kullanarak yangın tespiti yapar ve sonucu gösterir.

