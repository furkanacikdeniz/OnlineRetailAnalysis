
### Online Retail Veri Analizi Not Defteri

# 🛒 Online Retail Veri Analizi

Bu Jupyter Notebook, [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/online+retail) üzerinde yer alan **Online Retail** veri setini kullanarak temel veri analizi, veri temizleme ve zaman serisi tahmini işlemlerini gerçekleştirmektedir.

## 📦 Veri Kümesi

- **Kayıt Sayısı:** 541,909
- **Değişkenler:** InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country
- **Dönem:** 2010 Aralık - 2011 Aralık
- **Veri Tipi:** Satış kayıtları (İngiltere merkezli bir online perakende şirketi)

## 🛠️ Kullanılan Kütüphaneler

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `prophet` (eski adıyla `fbprophet`)
- `datetime`
- `warnings`

## 📊 Yapılan Analizler

### 1. **Veri Ön İnceleme**
- Veri kümesinin genel yapısı (`info`, `describe`)
- Eksik verilerin analizi
- Veri tipi dönüşümleri

### 2. **Veri Temizleme**
- Null kayıtların silinmesi
- İade işlemlerinin (InvoiceNo 'C' içeren) filtrelenmesi
- Ürün açıklaması olmayanların çıkarılması

### 3. **Satış Trend Analizi**
- Günlük satış adetlerinin hesaplanması
- Belirli günlerde satış olmaması durumunun değerlendirilmesi (örneğin Cumartesi günleri satış yok)

### 4. **Zaman Serisi Tahmini (Prophet ile)**
- Prophet için veri formatlama (`ds` ve `y`)
- Model eğitimi ve tahmini
- Grafiksel tahmin gösterimi

## 📈 Örnek Görseller
- Satış trendi
- Tahmin edilen satışlar ve gerçek değerlerin karşılaştırması

## 🚀 Nasıl Kullanılır?

### 1. Ortam Hazırlığı

```bash
pip install pandas numpy matplotlib seaborn prophet
````

### 2. Notebook'u Çalıştırma

Notebook'u açmak ve çalıştırmak için bir Jupyter ortamı kullanın:

```bash
jupyter notebook
```

ve ardından `OnlineRetail.ipynb` dosyasını çalıştırın.

## 🧠 Öğrenilecek Konular

* E-ticaret veri analizine giriş
* Zaman serisi modellemesi
* Prophet kütüphanesi ile tahmin
* Gerçek veri üzerinden veri temizleme uygulaması

## 📄 Lisans

Bu proje eğitim amaçlıdır. Veri seti UCI Machine Learning Repository tarafından paylaşılmıştır.
