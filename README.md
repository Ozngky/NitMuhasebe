# Muhasebe API - Shopify & Facebook Entegrasyonu

Bu proje, Shopify mağazanızdan satış verilerini ve Facebook'tan reklam harcamalarını çekerek otomatik kar-zarar hesaplaması yapan profesyonel bir muhasebe sistemidir. E-ticaret işletmelerinin finansal performansını gerçek zamanlı olarak takip etmelerini ve optimize etmelerini sağlar.

## 📋 Sistem Özeti

| Özellik | Durum | Açıklama |
|---------|-------|----------|
| 🛍️ **Shopify Entegrasyonu** | ✅ Aktif | Admin API v2023-10 ile tam entegrasyon |
| 📊 **Facebook Ads** | ✅ Aktif | Marketing API v18.0 ile reklam verisi çekme |
| 💰 **Kar-Zarar Hesaplama** | ✅ Aktif | Otomatik maliyet hesaplama ve kar analizi |
| 📱 **Web Dashboard** | ✅ Aktif | Bootstrap 5 ile responsive tasarım |
| 📈 **Grafikler** | ✅ Aktif | Chart.js ile interaktif veri görselleştirme |
| 🔌 **RESTful API** | ✅ Aktif | JSON formatında veri erişimi |
| 💡 **Akıllı Öneriler** | ✅ Aktif | Performans optimizasyon tavsiyeleri |
| 🔒 **Güvenlik** | ✅ Aktif | Environment variables ile güvenli yapı |
| 📚 **Dokümantasyon** | ✅ Tam | Detaylı kurulum ve kullanım kılavuzu |
| 🌍 **Türkçe Destek** | ✅ Tam | Arayüz ve dokümantasyon Türkçe |

### 🎯 Desteklenen Metrikler
- **Finansal**: Gelir, maliyet, kar, marj
- **Reklam**: ROAS, CPC, CTR, CPA
- **Satış**: AOV, sipariş sayısı, dönüşüm oranı
- **Trend**: Günlük, haftalık, aylık analiz

## 🚀 Hızlı Başlangıç

```bash
# 1. Projeyi klonlayın
git clone https://github.com/Ozngky/NitMuhasebe.git
cd NitMuhasebe

# 2. Bağımlılıkları yükleyin
composer install

# 3. Ortam değişkenlerini ayarlayın
cp .env.example .env
# .env dosyasını düzenleyin ve API anahtarlarınızı ekleyin

# 4. Sistem kontrolü yapın
php setup.php

# 5. Sunucuyu başlatın
php -S localhost:8000 -t public
```

**🌐 Tarayıcınızda açın**: `http://localhost:8000`

## 📸 Ekran Görüntüleri

### Dashboard Ana Sayfa
- **Finansal Metrikler**: Gelir, kar, marj, ROAS
- **Interaktif Grafikler**: Maliyet dağılımı, trend analizi
- **Akıllı Öneriler**: Performans iyileştirme tavsiyeleri

### Responsive Tasarım
- **Desktop**: Tam özellikli dashboard
- **Tablet**: Optimize edilmiş görünüm
- **Mobile**: Dokunmatik ekran desteği

## Özellikler

### 🛍️ **Shopify Entegrasyonu**
- Gerçek zamanlı satış verilerini otomatik çekme
- Sipariş detayları ve müşteri bilgileri
- Ürün performans analizi
- Vergi, kargo ve iade hesaplamaları
- Günlük, haftalık, aylık satış raporları

### 📊 **Facebook Ads Entegrasyonu**
- Reklam kampanya performansını takip etme
- Harcama analizi ve bütçe optimizasyonu
- CTR, CPC, CPM metrikleri
- Dönüşüm oranları ve ROAS hesaplamaları
- Kampanya bazlı kar-zarar analizi

### 💰 **Gelişmiş Kar-Zarar Hesaplaması**
- Otomatik maliyet hesaplama (ürün, reklam, kargo, işlem ücretleri)
- Kar marjı analizi ve trend takibi
- Günlük kar-zarar dökümü
- Maliyet dağılımı ve optimizasyon önerileri
- Özelleştirilebilir kar marjı ayarları

### 📈 **Performans Metrikleri**
- **ROAS (Return on Ad Spend)**: Reklam yatırım getirisi
- **AOV (Average Order Value)**: Ortalama sipariş değeri
- **CPA (Cost Per Acquisition)**: Müşteri edinme maliyeti
- **LTV (Lifetime Value)**: Müşteri yaşam boyu değeri
- **Conversion Rate**: Dönüşüm oranları

### 📱 **Modern Web Dashboard**
- Responsive tasarım (mobil, tablet, desktop)
- Gerçek zamanlı veri güncelleme
- Interaktif grafikler (Chart.js)
- Özelleştirilebilir tarih aralıkları
- Koyu/açık tema desteği
- Türkçe arayüz

### 📊 **Gelişmiş Veri Görselleştirme**
- **Pasta Grafikleri**: Maliyet dağılımı
- **Çubuk Grafikleri**: Gelir vs maliyet karşılaştırması
- **Çizgi Grafikleri**: Trend analizi
- **Tablo Görünümü**: Detaylı sayısal veriler
- **KPI Kartları**: Önemli metriklerin öne çıkarılması

### 💡 **Akıllı Öneriler ve Uyarılar**
- Düşük kar marjı uyarıları
- Yüksek reklam harcaması bildirimleri
- Performans iyileştirme önerileri
- Bütçe optimizasyonu tavsiyeleri
- Sezonsal trend analizleri

## Teknolojiler

### Backend
- **PHP 8.0+**: Modern PHP syntax ve özellikleri
- **Guzzle HTTP**: Güvenli ve hızlı API iletişimi
- **Composer**: Bağımlılık yönetimi ve autoloading
- **PSR-4**: Standart autoloading yapısı
- **DotEnv**: Güvenli ortam değişkeni yönetimi

### Frontend
- **HTML5**: Modern web standartları
- **CSS3**: Flexbox, Grid, Animation
- **JavaScript ES6+**: Async/await, fetch API
- **Bootstrap 5**: Responsive tasarım framework
- **Chart.js**: Interaktif grafik kütüphanesi
- **Font Awesome**: Modern ikonlar

### API Entegrasyonları
- **Shopify Admin API v2023-10**: En güncel Shopify API
- **Facebook Marketing API v18.0**: Facebook reklam platformu
- **RESTful API**: Standart REST endpoint'ları
- **JSON**: Veri formatı ve API yanıtları

## Kurulum

### 1. Sistem Gereksinimleri

#### Sunucu Gereksinimleri
- **PHP 8.0+** (önerilen: PHP 8.2)
- **Web Sunucusu**: Apache 2.4+ veya Nginx 1.18+
- **Composer**: En güncel sürüm
- **SSL Sertifikası**: HTTPS bağlantıları için (production)

#### PHP Uzantıları
- `curl`: HTTP istekleri için
- `json`: JSON işleme
- `mbstring`: String manipülasyonu
- `openssl`: SSL/TLS bağlantıları
- `zip`: Composer bağımlılıkları için

#### API Erişim Gereksinimleri
- **Shopify Admin API**: Private app veya custom app
- **Facebook Developer Account**: Business Manager erişimi
- **Facebook Marketing API**: Reklam hesabı yönetim izni

#### Tarayıcı Desteği
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

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

### Web Arayüzü Kullanımı

#### Dashboard Ana Sayfası
1. **Tarayıcınızda** `http://localhost:8000` adresini açın
2. **Tarih Seçimi**: Başlangıç ve bitiş tarihlerini seçin
3. **Analiz Et** butonuna tıklayın
4. **Sonuçları İnceleme**: Aşağıdaki bilgileri görebilirsiniz:

#### Gösterge Paneli Özellikleri

**📊 Ana Metrikler**
- **Toplam Gelir**: Brüt satış rakamları
- **Net Kar**: Tüm maliyetler düşülmüş kar
- **Kar Marjı**: Yüzde olarak karlılık oranı
- **ROAS**: Reklam yatırım getirisi

**📈 Grafikler**
- **Maliyet Dağılımı**: Pasta grafik ile maliyet analizi
- **Gelir vs Maliyet**: Çubuk grafik ile karşılaştırma
- **Trend Analizi**: Zaman serisi grafikleri
- **Günlük Performans**: Tarih bazlı detaylar

**💡 Akıllı Öneriler**
- **Performans Uyarıları**: Düşük kar marjı bildirimleri
- **Optimizasyon Önerileri**: Maliyet azaltma tavsiyeleri
- **Başarı Bildirimleri**: Yüksek performans onayları

#### Mobil Kullanım
- **Responsive Tasarım**: Tüm ekran boyutlarında çalışır
- **Touch Friendly**: Dokunmatik ekran desteği
- **Hızlı Yükleme**: Optimize edilmiş performans

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

### Yaygın Hatalar ve Çözümleri

#### 🔴 Shopify API Hataları
**Hata**: "Shopify API hatası: Unauthorized"
- **Çözüm**: Access Token'ın doğru ve güncel olduğunu kontrol edin
- **Kontrol**: Shopify Admin → Apps → Develop apps → API credentials

**Hata**: "Shop URL bulunamadı"
- **Çözüm**: `SHOPIFY_SHOP_URL`'nin `.myshopify.com` ile bittiğinden emin olun
- **Örnek**: `your-shop.myshopify.com`

#### 🔴 Facebook API Hataları
**Hata**: "Facebook API hatası: Invalid Ad Account ID"
- **Çözüm**: Ad Account ID'nin `act_` prefiksi ile başladığından emin olun
- **Örnek**: `act_123456789`

**Hata**: "Access Token Expired"
- **Çözüm**: Facebook Developer Console'dan yeni token alın
- **Not**: Token'ların belirli süre sonra sona erer

#### 🔴 Kurulum Hataları
**Hata**: "Composer install failed"
- **Çözüm**: PHP 8.0+ kullandığınızdan emin olun: `php --version`
- **Çözüm**: Gerekli PHP uzantılarını yükleyin: `php -m`

**Hata**: "Class not found"
- **Çözüm**: Autoloader'ı yeniden oluşturun: `composer dump-autoload`

### Sistem Kontrol Komutları

#### Kurulum Kontrolü
```bash
# Sistem gereksinimlerini kontrol et
php setup.php

# PHP uzantılarını kontrol et
php -m | grep -E "(curl|json|mbstring|openssl)"

# Composer bağımlılıklarını kontrol et
composer validate
```

#### Hata Ayıklama
```bash
# Debug mode'u açın (.env dosyasında)
APP_DEBUG=true

# Hata loglarını görüntüleyin
tail -f logs/error.log

# API bağlantılarını test edin
php tests/example_usage.php
```

### Performans Optimizasyonu

#### Önbellek Ayarları
```bash
# Önbellek klasörünü oluştur
mkdir -p cache/api

# Yazma izinlerini ayarla
chmod 755 cache/
```

#### Sunucu Ayarları
```apache
# Apache .htaccess
<IfModule mod_rewrite.c>
    RewriteEngine On
    RewriteCond %{REQUEST_FILENAME} !-f
    RewriteCond %{REQUEST_FILENAME} !-d
    RewriteRule ^(.*)$ index.php [QSA,L]
</IfModule>
```

### Güvenlik Kontrolleri

#### Ortam Değişkenleri
```bash
# .env dosyasının izinlerini kontrol et
ls -la .env

# Sadece owner okuyabilmeli
chmod 600 .env
```

#### API Güvenliği
- **HTTPS kullanın** production ortamında
- **API rate limiting** uygulayın
- **IP whitelist** kullanın mümkünse
- **Access token'ları düzenli yenileyin**

### Destek Alma

#### Adım 1: Hata Detaylarını Toplayın
```bash
# Sistem bilgilerini toplayın
php -v
composer --version
php setup.php
```

#### Adım 2: Log Dosyalarını Kontrol Edin
```bash
# Hata loglarını kontrol edin
cat logs/error.log

# API çağrı loglarını kontrol edin
cat logs/api.log
```

#### Adım 3: Test Sonuçlarını Paylaşın
```bash
# Test scriptini çalıştırın
php tests/example_usage.php > test_results.txt
```

## Katkıda Bulunma

1. Fork yapın
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Commit yapın (`git commit -m 'Add amazing feature'`)
4. Push yapın (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun

## Lisans

Bu proje MIT lisansı altında lisanslanmıştır.

## ❓ Sık Sorulan Sorular

### Genel Sorular

**S: Bu sistem ücretsiz mi?**
A:  Bu sistem MIT lisansı ile ücretsiz paylaşılacaktır ancak şu anda beta sürecinde ve ileri özellikler sadece müşterilerimize sunulmaktadır.

**S: Shopify Plus hesabı gerekli mi?**
A: Hayır, temel Shopify hesabı yeterlidir. Ancak Plus hesaplarında API limitleri daha yüksektir.

**S: Facebook Business Manager gerekli mi?**
A: Evet, Facebook reklam verilerine erişmek için Business Manager hesabı gereklidir.

### Teknik Sorular

**S: Hangi PHP sürümü gerekli?**
A: Minimum PHP 8.0, önerilen PHP 8.2 veya üzeri.

**S: Veritabanı gerekli mi?**
A: Mevcut sürümde hayır, ancak v1.1'de MySQL/PostgreSQL desteği eklenecek.

**S: Cron job kurmak gerekli mi?**
A: Hayır, sistem anlık API çağrıları ile çalışır. Gelecekte otomatik raporlar için cron job seçeneği eklenecek.

### Güvenlik Sorular

**S: API anahtarlarım güvenli mi?**
A: Evet, tüm API anahtarları .env dosyasında saklanır ve Git'e yüklenmez.

**S: HTTPS gerekli mi?**
A: Production ortamında kesinlikle HTTPS kullanın. Development için HTTP yeterli.

**S: Rate limiting var mı?**
A: Şu anda yoktur, ancak v1.2'de eklenecek. Shopify ve Facebook'un kendi limitleri vardır.

### Performans Sorular

**S: Kaç mağaza destekliyor?**
A: Şu anda tek mağaza, v1.2'de çoklu mağaza desteği eklenecek.

**S: Büyük veri setlerini işleyebilir mi?**
A: Evet, ancak çok büyük veri setleri için tarih aralığını bölerek kullanın.

**S: Mobil cihazlarda çalışır mı?**
A: Evet, responsive tasarım ile tüm cihazlarda optimize çalışır.

## 📞 Destek

### GitHub Issues
En hızlı destek için GitHub Issues kullanın:
- **Bug Report**: Hata bildirimi
- **Feature Request**: Özellik talebi
- **Documentation**: Dokümantasyon iyileştirme

### İletişim
- **GitHub**: [@Ozngky](https://github.com/Ozngky)
- **Email**: [mail@bloknit.com](mailto:mail@bloknit.com)

### Topluluk
- **GitHub Discussions**: Sorular ve tartışmalar
- **Wiki**: Detaylı rehberler ve örnekler

## Gelecek Özellikler

### 🔮 Yaklaşan Özellikler (v1.1)
- [ ] **Veritabanı Entegrasyonu**: MySQL/PostgreSQL desteği
- [ ] **Gelişmiş Raporlama**: Excel/PDF çıktıları
- [ ] **Email Bildirimleri**: Otomatik rapor gönderimi
- [ ] **Webhook Desteği**: Gerçek zamanlı veri senkronizasyonu
- [ ] **Önbellek Sistemi**: Redis/Memcached desteği

### 🚀 Orta Vadeli Özellikler (v1.2)
- [ ] **Çoklu Mağaza Desteği**: Birden fazla Shopify mağazası
- [ ] **Kullanıcı Yönetimi**: Rol tabanlı erişim kontrolü
- [ ] **API Rate Limiting**: Güvenli API kullanımı
- [ ] **Gelişmiş Analitik**: Makine öğrenmesi ile tahmin
- [ ] **Mobil PWA**: Progressive Web App desteği

### 🌟 Uzun Vadeli Özellikler (v2.0)
- [ ] **Multi-Platform**: Instagram, TikTok, Google Ads entegrasyonu
- [ ] **AI Önerileri**: Yapay zeka destekli optimizasyon
- [ ] **Mobil Uygulama**: iOS/Android native app
- [ ] **Multi-Language**: İngilizce, Almanca, Fransızca destek
- [ ] **SaaS Versiyon**: Bulut tabanlı çözüm

### 🎯 Topluluk Talepleri
- [ ] **Dark Mode**: Koyu tema tam desteği
- [ ] **Grafik Customization**: Kullanıcı tanımlı grafikler
- [ ] **Automated Reporting**: Programlanmış raporlar
- [ ] **Integration Marketplace**: Üçüncü parti entegrasyonlar
- [ ] **Advanced Filtering**: Gelişmiş veri filtreleme

### 🔧 Teknik İyileştirmeler
- [ ] **Unit Testing**: Kapsamlı test coverage
- [ ] **CI/CD Pipeline**: Otomatik deployment
- [ ] **Docker Support**: Containerization
- [ ] **Monitoring**: Application performance monitoring
- [ ] **Security Audit**: Güvenlik taraması ve iyileştirmeler

## Changelog

### v1.0.0 (2024-01-01)
- İlk stabil sürüm
- Shopify ve Facebook entegrasyonu
- Kar-zarar hesaplaması
- Web arayüzü
- API endpoints 