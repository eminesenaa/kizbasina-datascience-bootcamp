# ✈️ Havayolu Yolcu Memnuniyeti Analizi

Bu proje, **Kız Başına Veri Analizi Bootcamp** kapsamında tamamlanan 1. final case çalışmasıdır. Projede, bir havayolu firmasına ait yolcu memnuniyet verileri analiz edilmiştir. Amaç, müşteri memnuniyetini etkileyen temel faktörleri belirlemek ve veriyi anlamlı hale getirerek analiz edilebilir bir formatta sunmaktır.

## 📁 Proje İçeriği

- **Veri Seti Kaynağı**: [Airline Passenger Satisfaction Dataset](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction)
- **Kapsam**:
  - İstatistiksel özetleme
  - Eksik ve aykırı değer tespiti ve işlenmesi
  - Sayısal ve kategorik değişkenlerin görselleştirilmesi
  - Memnuniyet düzeyinin uçuş sınıfı ve hizmet unsurlarıyla ilişkisi

## 🔍 1. Veri Keşfi

- `train.csv` dosyası üzerinden analiz yapılmıştır.
- Toplam **103904** satır ve **25** sütun mevcuttur.
- Veri yapısı ve ilk gözlemler yapılmıştır.

## 📊 2. İstatistiksel Analiz

- Sayısal değişkenler (`Age`, `Flight Distance`, `Arrival Delay in Minutes` vb.) için temel istatistikler çıkarılmıştır.
- `describe()` fonksiyonu ile ortalama, medyan, minimum ve maksimum değerler analiz edilmiştir.

## 🧩 3. Eksik Değer Analizi

- `"", "Unknown", -1, 999` gibi eksiklik gösteren değerler `NaN` olarak tanımlanmıştır.
- Eksik veri sayısı ve yüzdeleri hesaplanmıştır.
- Eksik veriler sütun bazında görselleştirilmiştir.
- Gerekli yerlerde ortalama veya sıfır ile doldurma işlemleri uygulanmıştır.

## ⚠️ 4. Aykırı Değer (Outlier) Analizi

- `Arrival Delay in Minutes` değişkeninde aykırı değerler **IQR yöntemi** ile tespit edilmiştir.
- Boxplot grafikleri ile aykırılıklar görselleştirilmiştir.
- Gerekli temizlemeler yapılmıştır.

## 📈 5. Görselleştirme

### 5.1 Sayısal Değişkenler

- Histogram ve Boxplot grafikleri ile `Age`, `Flight Distance`, `Departure Delay`, `Arrival Delay` gibi değişkenler analiz edilmiştir.

### 5.2 Kategorik Değişkenler

- `Gender`, `Customer Type`, `Type of Travel` gibi kategorik değişkenler `Class` (uçuş sınıfı) değişkenine göre görselleştirilmiştir.

### 5.3 Memnuniyet Analizi

- `Seat comfort`, `Baggage handling`, `Leg room service`, `Inflight entertainment` gibi müşteri memnuniyetine dair değişkenler `Class` ile birlikte analiz edilmiştir.
- Uçuş sınıfına göre müşteri memnuniyeti seviyeleri yorumlanmıştır.

## ✅ 6. Sonuç

Bu analiz sayesinde:
- Veri seti temizlenmiş ve eksik değerlerden arındırılmıştır.
- Aykırı değerler tespit edilip yorumlanmıştır.
- Sayısal ve kategorik değişkenlerin müşteri memnuniyeti üzerindeki etkileri görselleştirilmiştir.
- Uçuş sınıfı ve memnuniyet arasındaki ilişki net bir şekilde ortaya konmuştur.

---

> 📌 **Not:** Projede kullanılan temel kütüphaneler:  
> `pandas`, `numpy`, `matplotlib`, `seaborn`, `warnings`

> 🧠 **Ek Yorum**: Memnuniyet düzeyleri özellikle business class yolcularında daha yüksektir. Eğlence, konfor ve bagaj işlemleri memnuniyet üzerinde belirgin rol oynamaktadır.

---

## 🔗 Projeye Erişim

Bu projeye ait Jupyter Notebook dosyasına **Kaggle hesabım üzerinden** aşağıdaki bağlantıdan ulaşabilirsiniz:

👉 [Kaggle Üzerinde Görüntüle](https://www.kaggle.com/code/eminesena/kiz-basina-bootcamp-final-case1)


