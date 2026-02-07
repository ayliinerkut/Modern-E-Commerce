# NOIR - Modern E-Commerce UI

Modern, şık ve tamamen işlevsel bir e-ticaret arayüzü. Koyu tema, lüks estetik ve pürüzsüz animasyonlarla tasarlanmıştır.

## 🎨 Özellikler

### Tasarım
- **Koyu Tema**: Lüks ve modern görünüm için siyah-altın renk paleti
- **Premium Tipografi**: Playfair Display ve Space Mono font kombinasyonu
- **Animasyonlar**: Sayfa yükleme, hover efektleri ve geçiş animasyonları
- **Responsive**: Mobil ve masaüstü cihazlara tam uyumlu

### Fonksiyonellik
- ✅ Ürün grid sistemi
- ✅ Çalışan alışveriş sepeti
- ✅ Miktar artırma/azaltma
- ✅ Gerçek zamanlı toplam hesaplama
- ✅ Sepete ürün ekleme/çıkarma
- ✅ Kategori filtreleme butonları
- ✅ Ürün derecelendirme ve fiyat gösterimi
- ✅ Yan panel sepet tasarımı

## 🚀 Kullanım

### Basit Kullanım
Sadece `ecommerce-ui.html` dosyasını tarayıcınızda açın. Ekstra kurulum gerekmez!

### Özelleştirme

#### Ürün Eklemek
JavaScript kodundaki `products` dizisini düzenleyin:

```javascript
const products = [
    { 
        id: 1, 
        name: 'Ürün Adı', 
        category: 'Kategori', 
        price: 299, 
        originalPrice: 399, 
        rating: 4.8, 
        reviews: 124, 
        badge: 'YENİ', 
        icon: '🎩' 
    },
    // Daha fazla ürün ekleyin...
];
```

#### Renkleri Değiştirmek
CSS'teki `:root` değişkenlerini düzenleyin:

```css
:root {
    --noir-black: #0a0a0a;
    --noir-white: #fafafa;
    --noir-gray: #2a2a2a;
    --noir-accent: #ff4757;  /* Ana vurgu rengi */
    --noir-gold: #f0a500;    /* Altın rengi */
    --noir-border: #333;
}
```

#### Logo ve Marka
HTML'deki `.logo` class'ını bulun ve "NOIR" yazısını kendi markanızla değiştirin:

```html
<div class="logo">KENDİ MARKANIZ</div>
```

## 📱 Responsive Tasarım

- **Masaüstü**: Tam özellikli navigasyon ve çoklu sütun grid
- **Tablet**: Otomatik ayarlanan grid sistemi
- **Mobil**: Tam ekran sepet ve optimize edilmiş layout

## 🎯 Kullanılan Teknolojiler

- **HTML5**: Semantik yapı
- **CSS3**: Modern animasyonlar ve grid sistemi
- **Vanilla JavaScript**: Framework'süz, saf JS
- **Google Fonts**: Playfair Display & Space Mono

## 🛠️ Geliştirme

### Sepet Fonksiyonları

```javascript
addToCart(productId)      // Ürün ekle
updateQuantity(id, change) // Miktar güncelle
removeItem(productId)      // Ürün çıkar
updateCart()              // Sepeti güncelle
```

### Filtre Sistemi
Filtre butonlarını genişletmek için:

```javascript
filterBtns.forEach(btn => {
    btn.addEventListener('click', function() {
        const filter = this.dataset.filter;
        // Filtreleme mantığınızı buraya ekleyin
    });
});
```

## 🎨 Özelleştirme İpuçları

1. **Ürün Görselleri**: `icon` alanını emoji yerine `<img>` tag'i ile değiştirin
2. **Kategori Sayfaları**: Her kategori için ayrı HTML sayfaları oluşturun
3. **Backend Entegrasyonu**: API endpoint'lerinizi bağlayın
4. **Ödeme Sistemi**: `.checkout-btn` butonuna ödeme fonksiyonu ekleyin
5. **Kullanıcı Girişi**: Header'a login/register butonları ekleyin

## 📦 Örnek Ürünler

Proje 6 örnek ürünle gelir:
- Midnight Blazer (Erkek)
- Classic Leather Bag (Aksesuar)
- Silk Evening Dress (Kadın)
- Premium Watch (Aksesuar)
- Urban Sneakers (Erkek)
- Designer Sunglasses (Aksesuar)

## 🔧 Gelecek Geliştirmeler

- [ ] Backend API entegrasyonu
- [ ] Ödeme sistemi (Stripe/PayPal)
- [ ] Kullanıcı hesap sistemi
- [ ] Ürün arama fonksiyonu
- [ ] Favori ürünler
- [ ] Ürün karşılaştırma
- [ ] Canlı filtre sistemi
- [ ] Çoklu resim galerisi
- [ ] Ürün zoom özelliği
- [ ] İstek listesi

## 📄 Lisans

Bu proje kişisel ve ticari kullanım için ücretsizdir.

## 🤝 Katkıda Bulunma

Bu projeyi forklayıp geliştirmekten çekinmeyin! Her türlü iyileştirme önerisi kabul edilir.

---

**Geliştirici Notu**: Bu UI, modern web standartlarıyla oluşturulmuş, production-ready bir şablondur. Gerçek bir e-ticaret sitesi için backend entegrasyonu, güvenlik önlemleri ve ödeme sistemi eklemeniz gerekecektir.
