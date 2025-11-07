# Ases Stok Takip Sistemi

Modern ve kullanıcı dostu bir stok takip uygulaması. Flask framework'ü ile geliştirilmiştir.

## Özellikler

### 🏠 Ana Sayfa
- Genel istatistikler (toplam ürün, adet, hareket sayısı)
- Kategori bazlı stok dağılımı grafiği
- Son hareketler listesi
- Hızlı erişim butonları

### 📦 Ürün Yönetimi
- Ürün ekleme (marka, model, barkod, seri no, kategori, adet)
- Ürün listeleme ve arama
- Kategori bazlı filtreleme
- Ürün detay görüntüleme
- Stok durumu takibi

### 🔄 Hareket Yönetimi
- Giriş hareketleri (otomatik)
- Çıkış hareketleri (manuel)
- Hareket geçmişi görüntüleme
- Tarih ve kullanıcı bazlı filtreleme
- Hareket detayları

### 👥 Kullanıcı Yönetimi (Admin)
- Kullanıcı ekleme/silme
- Yetki seviyesi yönetimi (Admin/Normal)
- Kullanıcı istatistikleri
- Güvenli şifre yönetimi

### 📊 Analiz ve Raporlama
- Kategori bazlı stok analizi
- Günlük hareket grafikleri
- Stok durumu raporları
- İstatistiksel analizler
- Görsel grafikler (Chart.js)

## Kurulum

### Gereksinimler
- Python 3.7+
- pip

### Adımlar

1. **Projeyi klonlayın:**
```bash
git clone <repository-url>
cd ases
```

2. **Sanal ortam oluşturun:**
```bash
python -m venv venv
```

3. **Sanal ortamı aktifleştirin:**
```bash
# Windows
venv\Scripts\activate

# Linux/Mac
source venv/bin/activate
```

4. **Gerekli paketleri yükleyin:**
```bash
pip install -r requirements.txt
```

5. **Uygulamayı çalıştırın:**
```bash
python app.py
```

6. **Tarayıcıda açın:**
```
http://localhost:5000
```

## Giriş Bilgileri

**Admin Kullanıcı:**
- Email: admin@admin.com
- Şifre: admin

## Kullanım

### İlk Kurulum
1. Admin kullanıcısı ile giriş yapın
2. İlk ürünlerinizi ekleyin
3. Gerekirse yeni kullanıcılar oluşturun

### Ürün Ekleme
1. "Ürünler" menüsüne gidin
2. "Yeni Ürün Ekle" butonuna tıklayın
3. Gerekli bilgileri doldurun:
   - Marka ve model
   - Benzersiz barkod
   - Benzersiz seri numarası
   - Kategori seçimi
   - Başlangıç adedi

### Çıkış Yapma
1. "Hareketler" menüsüne gidin
2. "Çıkış Yap" butonuna tıklayın
3. Ürün seçin ve adet girin
4. Açıklama ekleyin (opsiyonel)

### Analiz Görüntüleme
1. "Analizler" menüsüne gidin
2. Kategori dağılımı grafiklerini inceleyin
3. Günlük hareket analizlerini görün
4. Detaylı raporları kontrol edin

## Teknik Detaylar

### Veritabanı
- SQLite veritabanı kullanılır
- Otomatik tablo oluşturma
- İlişkisel veri yapısı

### Güvenlik
- Şifre hashleme (Werkzeug)
- Kullanıcı oturum yönetimi
- Yetki kontrolü

### Frontend
- Bootstrap 5
- Font Awesome ikonları
- Chart.js grafikleri
- Responsive tasarım

## Geliştirme

### Proje Yapısı
```
ases/
├── app.py              # Ana uygulama dosyası
├── requirements.txt    # Python paketleri
├── README.md          # Bu dosya
├── templates/         # HTML şablonları
│   ├── base.html
│   ├── index.html
│   ├── login.html
│   ├── products.html
│   ├── add_product.html
│   ├── movements.html
│   ├── exit_product.html
│   ├── users.html
│   ├── add_user.html
│   └── analytics.html
└── static/            # Statik dosyalar (CSS, JS)
```

### Veritabanı Modelleri
- **User**: Kullanıcı bilgileri
- **Product**: Ürün bilgileri
- **Movement**: Hareket kayıtları

## Lisans

Bu proje MIT lisansı altında lisanslanmıştır.

## Destek

Herhangi bir sorun veya öneri için lütfen iletişime geçin.
