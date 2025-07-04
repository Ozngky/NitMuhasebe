# Muhasebe API - Shopify & Facebook Entegrasyonu

Bu proje, Shopify mağazanızdan satış verilerini ve Facebook'tan reklam harcamalarını çekerek otomatik kar-zarar hesaplaması yapan bir muhasebe sistemidir.

## Özellikler

- 🛍️ **Shopify Entegrasyonu**: Satış verilerini otomatik çekme
- 📊 **Facebook Ads Entegrasyonu**: Reklam harcamalarını takip etme
- 💰 **Kar-Zarar Hesaplaması**: Otomatik finansal analiz
- 📈 **ROAS Hesaplama**: Reklam yatırım getirisini takip etme
- 📱 **Modern Web Arayüzü**: Responsive ve kullanıcı dostu tasarım
- 📊 **Grafik ve Çizelgeler**: Görsel veri analizi
- 💡 **Akıllı Öneriler**: Performans iyileştirme önerileri

## Teknolojiler

- **Backend**: PHP 8.0+
- **Frontend**: HTML5, CSS3, JavaScript, Bootstrap 5
- **API İletişimi**: Guzzle HTTP
- **Grafik Kütüphanesi**: Chart.js
- **Bağımlılık Yönetimi**: Composer

## Kurulum

### 1. Gereksinimler

- PHP 8.0 veya üzeri
- Composer
- Web sunucusu (Apache/Nginx)
- Shopify Admin API erişimi
- Facebook Developer hesabı

### 2. Projeyi İndirin

```bash
git clone https://github.com/Ozngky/NitMuhasebe.git
cd NitMuhasebe
```

### 3. Bağımlılıkları Yükleyin

```bash
composer install
```

### 4. Ortam Değişkenlerini Ayarlayın

`.env` dosyasını oluşturun ve API anahtarlarınızı ekleyin:

```env
# Shopify API Ayarları
SHOPIFY_SHOP_URL=your-shop.myshopify.com
SHOPIFY_ACCESS_TOKEN=your_shopify_access_token
SHOPIFY_API_VERSION=2023-10

# Facebook API Ayarları
FACEBOOK_APP_ID=your_facebook_app_id
FACEBOOK_APP_SECRET=your_facebook_app_secret
FACEBOOK_ACCESS_TOKEN=your_facebook_access_token
FACEBOOK_AD_ACCOUNT_ID=act_your_ad_account_id

# Uygulama Ayarları
APP_ENV=development
APP_DEBUG=true
APP_URL=http://localhost:8000

# Kar Marjı Ayarları (varsayılan %)
DEFAULT_PROFIT_MARGIN=30
```

### 5. Web Sunucusunu Başlatın

```bash
cd public
php -S localhost:8000
```

## API Anahtarlarını Alma

### Shopify API

1. Shopify Admin panelinde **Apps** > **App and sales channel settings** bölümüne gidin
2. **Develop apps** butonuna tıklayın
3. **Create an app** ile yeni uygulama oluşturun
4. **Admin API** sekmesinde gerekli izinleri ekleyin:
   - `read_orders`
   - `read_products`
   - `read_analytics`
5. **Install app** ile uygulamayı kurun ve Access Token'ı kopyalayın

### Facebook API

1. [Facebook Developers](https://developers.facebook.com/) hesabı oluşturun
2. **Create App** ile yeni uygulama oluşturun
3. **Marketing API** ürününü ekleyin
4. **Ad Account** ID'nizi `act_` prefiksi ile birlikte alın
5. **Access Token** oluşturun (Marketing API izinleri gerekli)

## Kullanım

### Web Arayüzü

1. Tarayıcınızda `http://localhost:8000` adresini açın
2. Tarih aralığını seçin
3. **Analiz Et** butonuna tıklayın
4. Sonuçları görüntüleyin

### API Endpoints

#### Kar-Zarar Raporu
```
GET /api/profit-loss?start_date=2023-01-01&end_date=2023-12-31
```

#### Detaylı Rapor
```
GET /api/detailed-report?start_date=2023-01-01&end_date=2023-12-31
```

#### Shopify Verileri
```
GET /api/shopify-data?start_date=2023-01-01&end_date=2023-12-31
```

#### Facebook Verileri
```
GET /api/facebook-data?start_date=2023-01-01&end_date=2023-12-31
```

### Örnek API Yanıtı

```json
{
  "summary": {
    "period": {
      "start_date": "2023-01-01",
      "end_date": "2023-12-31"
    },
    "revenue": {
      "gross_sales": 50000,
      "net_sales": 47000,
      "tax_collected": 2000,
      "total_orders": 250
    },
    "costs": {
      "product_costs": 32900,
      "advertising_costs": 8000,
      "shipping_costs": 1200,
      "payment_processing": 1410,
      "total_costs": 43510
    },
    "profit": {
      "gross_profit": 14100,
      "net_profit": 3490,
      "profit_margin": 7.43,
      "roas": 5.88
    },
    "metrics": {
      "average_order_value": 200,
      "cost_per_acquisition": 32,
      "conversion_rate": 3.2
    }
  },
  "recommendations": [
    {
      "type": "warning",
      "title": "Düşük Kar Marjı",
      "message": "Kar marjınız %7.43 seviyesinde. Maliyetlerinizi gözden geçirin."
    }
  ]
}
```

## Özelleştirme

### Kar Marjını Değiştirme

```php
$accountingService->updateProfitMargin(25); // %25 kar marjı
```

### Maliyet Hesaplama Metodlarını Özelleştirme

`src/Services/AccountingService.php` dosyasında aşağıdaki metodları düzenleyebilirsiniz:

- `calculateProductCosts()`: Ürün maliyeti hesaplama
- `calculateShippingCosts()`: Kargo maliyeti hesaplama
- `calculatePaymentProcessingFees()`: Ödeme işlem ücreti hesaplama

## Güvenlik

- API anahtarlarınızı asla kodun içine koymayın
- `.env` dosyasını `.gitignore`'a ekleyin
- Üretim ortamında `APP_DEBUG=false` yapın
- HTTPS kullanın

## Sorun Giderme

### Yaygın Hatalar

1. **Shopify API Hatası**: Access Token ve shop URL'yi kontrol edin
2. **Facebook API Hatası**: Ad Account ID'nin `act_` prefiksi ile başladığından emin olun
3. **Composer Hatası**: PHP 8.0+ kullandığınızdan emin olun

### Hata Logları

Debug mode açıkken hatalar ekranda gösterilir. Üretim ortamında hata loglarını kontrol edin.

## Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Commit yapın (`git commit -m 'Add amazing feature'`)
4. Push yapın (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun

## Lisans

Bu proje MIT lisansı altında lisanslanmıştır.

## Destek

Herhangi bir sorunuz varsa:
- GitHub Issues bölümünden bildirin
- E-posta: [your-email@example.com]

## Gelecek Özellikler

- [ ] Veritabanı entegrasyonu
- [ ] Çoklu mağaza desteği
- [ ] Excel/PDF rapor çıktısı
- [ ] Email bildirimleri
- [ ] Gelişmiş analitik dashboard
- [ ] Mobil uygulama
- [ ] Multi-language destek

## Changelog

### v1.0.0 (2024-01-01)
- İlk stabil sürüm
- Shopify ve Facebook entegrasyonu
- Kar-zarar hesaplaması
- Web arayüzü
- API endpoints 