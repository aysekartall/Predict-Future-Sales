# Predict-Future-Sales
Kaggle yarışmasındaki gelecekteki satış tahmini


# Predict Future Sales (Gelecekteki Satışları Tahmin Et)

## 1. Problemin Türü
Bu problem, Regresyon Problemi'dir. Bu problemde amaç, bir Rus teknoloji şirketinin çeşitli mağazalarında satılan aylık toplam ürün satış miktarını tahmin etmektir. 

## 2. Veriseti
1. **item_categories.csv**  -      _Ürün kategorileri hakkında tamamlayıcı bilgiler._

2. **items.csv**  -                _Ürünler hakkında tamamlayıcı bilgiler._

3. **sales_train.csv**  -          _Ocak 2013'ten Ekim 2015'e kadar günlük geçmiş verilerin tutulduğu eğitim verisetidir._

4. **sample_submissions.csv** -    _Doğru formatta bir örnek gönderim dosyası._

5. **shops.csv**  -                _Mağazalar hakkında ek bilgiler._

6. **test.csv**  -                 _Bu mağazalar ve ürünler için Kasım 2015 satışları tahmin edilecek test verisetidir._


## 3. Seçilen Öznitelikler ve Türleri
### Kategorik:
- **shop_id** - Bir mağazanın benzersiz tanımlayıcısı  
- **item_id** - Bir ürünün benzersiz tanımlayıcısı  
- **item_category_id** - Ürün kategorisinin benzersiz tanımlayıcısı   
- **date_block_num** - Kolaylık sağlamak için kullanılan ardışık bir ay numarası. Ocak 2013 0, Şubat 2013 1, ... Ekim 2015 33 

### Nümerik:
- **item_price** - Bir ürünün mevcut fiyatı  
- **date** - gg / aa / yyyy biçiminde tarih  
- **item_cnt_day** - Belirli bir günde satılan ürün sayısı.

### Çıktı verisi (y_test)
- **item_cnt_month**   - Nümerik

## 4. Performans Ölçütleri

### - Root Mean Square Error(RMSE):
Bir makine öğrenmesi modelinin, tahminleyicinin tahmin ettiği değerler ile gerçek değerleri arasındaki uzaklığın bulunmasında sıklıkla kullanılan,
hatanın büyüklğünü ölçen kuadratik bir metriktir. RMSE tahmin hatalarının (kalıntıların) standart sapmasıdır.
