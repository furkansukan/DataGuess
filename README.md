## 🔍 Proje Özeti

* **Amaç:** Görüntülerdeki yangınları gerçek zamanlı olarak tespit etmek.
* **Teknolojiler:** Python, YOLOv8, OpenCV.
* **Model:** Eğitilmiş YOLOv8 modeli (`best.pt`).
* **Kullanım Alanları:** Endüstriyel tesisler, orman yangını izleme sistemleri, güvenlik kameraları.

* Bu projede, yangın tespiti için YOLOv8 (You Only Look Once) nesne algılama algoritması temel alınarak bir bilgisayarla görme uygulaması geliştirilmiştir. Eğitim süreci, Roboflow platformundan temin edilen özel bir yangın veri kümesi kullanılarak gerçekleştirilmiş ve modelin çıktıları Google Colab ortamında görselleştirilmiştir.

* Kodlar, proje akışının her adımını net bir şekilde takip edebilecek biçimde açıklayıcı yorumlarla desteklenmiştir. Eğitim sırasında kullanılan tüm hiperparametreler (örneğin, epochs=80, imgsz=640) ve veri yolu (data.yaml) açıkça belirtilmiştir. Ek olarak modelin eğitim sonrası başarı durumu görselleştirilmiş ve doğrulama aşamasında elde edilen sonuçlar da değerlendirilmiştir.

* Geliştirilen yangın algılama modeli; akıllı güvenlik sistemleri, fabrika ortamları, enerji santralleri, orman gözetleme istasyonları ve endüstriyel kamera ağları gibi alanlarda kullanılabilir. Özellikle erken yangın uyarı sistemleri içinde yer alarak, insan müdahalesi olmaksızın gerçek zamanlı tespit sağlayabilir ve olası can ve mal kayıplarını azaltmaya yardımcı olabilir.

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

