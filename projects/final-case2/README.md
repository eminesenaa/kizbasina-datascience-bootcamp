# 📊 Power BI Proje Ödevi

Bu proje, veri görselleştirme ve iş zekâsı araçlarının kullanımını öğrenmek amacıyla Power BI üzerinde geliştirilmiştir. Sipariş verileri üzerinden çeşitli analizler yapılarak kullanıcıya anlamlı içgörüler sunulmuştur.

## 🔍 Proje Amacı

Kullanıcıların satın alma davranışlarını, satış eğilimlerini ve müşteri segmentasyonunu görselleştirerek analiz etmektir. Proje, üç ana perspektif üzerine inşa edilmiştir:

- Özet Sayfa
- Müşteri Perspektifi
- Kategori Perspektifi

## 🧩 Kullanılan Veriler

- `kullanicilar.csv`
- `siparis.csv`
- `siparisdetay.csv`
- `adres.csv`
- `urunler.csv`
- `date.txt`

Veriler Power BI'a yüklenmiş ve ilişkilendirilerek modelleme yapılmıştır.

## 📌 Sayfa Açıklamaları

### 1. Özet Sayfa
- Toplam Ciro, Toplam Müşteri, Toplam Sipariş gibi temel metrikler
- Haftasonu vs. Haftaiçi satış karşılaştırması (donut grafik)
- İstanbul’daki en çok ciro yapan ilk 10 müşteri (tablo)

### 2. Müşteri Perspektifi
- Kadın / Erkek müşteri sayıları (kart)
- Yaş grubuna göre satış analizi (bar grafik)
- Tekil müşteri sayısı

### 3. Kategori Perspektifi
- İstanbul'daki genç kullanıcıların yaptığı harcamalar (ağaç haritası)
- Satışlar kategori bazında segmentlenmiştir.

## 📌 Hesaplanan Ölçüler

- **ToplamCiro** = `SUM(siparisdetay[LINETOTAL])`
- **ToplamSatisAdeti** = `COUNT(siparisdetay[ID])`
- **ToplamMusteri** = `DISTINCTCOUNT(siparis[USERID])`
- **MusteriBasiCiro** = `[ToplamCiro] / [ToplamMusteri]`
- **MusteriBasiAdet** = `[ToplamSatisAdeti] / [ToplamMusteri]`
- **OrtalamaSiparisTutari** = `[ToplamCiro] / [ToplamSiparis]`

## 🧠 Öğrenilenler

- Veri modelleme ve ilişki kurma
- Ölçü (measure) ve koşullu sütun oluşturma
- Filtreleme, dilimleyiciler ve görselleştirme araçlarının kullanımı
- Treemap, donut, bar chart, table, card gibi görsel öğelerin efektif kullanımı

## ✨ Ekran Görüntüleri

Proje içerisinde oluşturulan sayfaların örnekleri:



📊 Özet Sayfa

<img width="600"  alt="Screenshot 2025-07-21 012701" src="https://github.com/user-attachments/assets/ffe19e93-2770-4294-af60-d84157c677b5" />



👤 Müşteri Perspektifi

<img width="600" alt="Screenshot 2025-07-21 012711" src="https://github.com/user-attachments/assets/ed756e90-8154-4dc0-a6e1-f3a559b604d5" />



🗂️ Kategori Perspektifi  

<img width="600" alt="Screenshot 2025-07-21 012716" src="https://github.com/user-attachments/assets/2ccb0449-ad31-446a-9452-ec8c18e51955" />






---

📌 **Not:** Bu proje bir ders ödevi kapsamında geliştirilmiş olup gerçek müşteri verisi içermez. Yalnızca eğitim amaçlıdır.

