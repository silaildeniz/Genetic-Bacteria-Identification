# Genetic-Bacteria-Identification
Genetik Bakteri Sınıflandırılması
# Genetik Bakteri Tanımlama

## **Genel Bakış**
Antibiyotik direnci, bakteriyel enfeksiyonların tedavisini tehdit eden küresel bir sağlık krizine dönüşmüştür. Bakteriyel türlerin ve direnç desenlerinin hızlı ve doğru bir şekilde tanımlanması, etkili antibiyotiklerin seçimi için hayati öneme sahiptir. Özellikle sepsis gibi hayati tehlike oluşturan durumlarda bu tanımlama süreci büyük bir fark yaratabilir.

Bu proje, genomik dizileme verilerini kullanarak 10 farklı bakteriyel türü sınıflandırmayı ve antibiyotik direncini tahmin etmeyi amaçlamaktadır. Makine öğrenimi teknikleri kullanılarak, bakterilerin tanımlanması hızlandırılmakta ve doğruluk artırılmaktadır. Bu sayede, klinik sonuçlar iyileştirilmekte ve antibiyotiklerin daha etkin kullanılması sağlanmaktadır.

## **Veri Kümesi**
Bu projede kullanılan veri kümesi, bakteriyel DNA dizilerini ve bunlara karşılık gelen tür etiketlerini içermektedir. Veri seti Kaggle'dan alınmıştır ve makine öğrenimi modellerinin eğitimi ve test edilmesi için kullanılmıştır.

- **Veri Seti Kaynağı:** [Genetik Bakteri Tanımlama Veri Seti](https://www.kaggle.com/datasets/gauravduttakiit/genetic-bacteria-identification/data?select=train_dataset.csv)
- **Veri Seti İçeriği:**
  - Eğitim ve test verisi ayrımı
  - DNA dizi bilgileri
  - 10 farklı bakteriyel tür için etiketler

## **Proje Amaçları**
1. Genomik verilerin analizi ve ön işlenmesi.
2. Bakteriyel türlerin genomik dizilere dayanarak sınıflandırılması için makine öğrenimi modeli eğitimi.
3. Model performansının değerlendirilmesi ve optimizasyonu.

## **Proje İş Akışı**
1. **Veri Keşfi ve Ön İşleme:**
   - Veri setinin yüklenmesi ve temizlenmesi.
   - Türlerin dağılımının incelenmesi.
   - Kategorik verilerin kodlanması ve sayısal özelliklerin normalleştirilmesi.

2. **Özellik Mühendisliği:**
   - DNA dizilerinden anlamlı desenlerin çıkarılması.
   - Gerekirse boyut indirgeme işlemlerinin uygulanması.

3. **Model Eğitimi:**
   - Random Forest, XGBoost veya Sinir Ağları gibi modellerin eğitilmesi.
   - Çapraz doğrulama ile model performansının sağlamlaştırılması.

4. **Model Değerlendirmesi:**
   - Modelin doğruluk, kesinlik, duyarlılık ve F1 skorları gibi metriklerle değerlendirilmesi.
   - Yanlış sınıflandırmaları anlamak için karışıklık matrisinin analiz edilmesi.


## **Sonuçlar**
- En iyi performans gösteren model, test verisinde **61%** doğruluk elde etti.
- Her bir bakteriyel tür için kesinlik, duyarlılık ve F1 skorları `results` dizininde detaylı bir şekilde verilmiştir.
- Karışıklık matrisinin ve özellik öneminin görselleştirilmesi notebook dosyasına dahil edilmiştir.

## **Gelecekteki Çalışmalar**
- Daha yüksek doğruluk için derin öğrenme modellerinin uygulanması.
- Daha fazla bakteriyel türü içerecek şekilde veri setinin genişletilmesi.
- Gerçek zamanlı genomik veri işleme için boru hattının optimize edilmesi.


Bu proje, antibiyotik direncine yönelik küresel ihtiyacı ele almak için tasarlanmış ve halka açık genomik verilerden destek almıştır.


