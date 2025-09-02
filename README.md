# Covolt - Enerji Yönetimi Platformu Landing Page

Covolt, işletmeler için enerji yönetimi ve optimizasyon platformunun resmi landing page'idir. Bu proje Astro ve Tailwind CSS v4 kullanılarak geliştirilmiştir.

## Proje Hakkında

Covolt, işletmelerin elektrik tüketimini daha görünür, yönetilebilir ve sürdürülebilir hale getiren bir SaaS platformudur. Tek tesisli küçük işletmeden, çok tesisli endüstriyel gruplara kadar çalışabilir.

### Temel Özellikler

- **OSOS Entegrasyonu**: Türkiye'deki tüm 21 EDAŞ altyapısından anlık veri toplama
- **Fatura Doğrulama**: Elektrik faturalarını kontrol ederek gereksiz ödemeleri engelleme
- **Uyarı Sistemi**: Reaktif ceza ve maksimum talep aşımından önce akıllı uyarılar
- **Çok Tesis Yönetimi**: Birden fazla tesisi tek panelden yönetme
- **Raporlama**: CFO, CEO ve enerji yöneticisi için özelleştirilmiş raporlar

## Teknoloji Stack

- **Astro** - Static Site Generator
- **Tailwind CSS v4** - Styling framework
- **Alpine.js** - Lightweight JavaScript framework

## Kurulum ve Çalıştırma

### Gereksinimler

- Node.js 18+ 
- npm veya pnpm

### Kurulum Adımları

1. Projeyi klonlayın:
```bash
git clone <repository-url>
cd covolt-landing-page
```

2. Bağımlılıkları yükleyin:
```bash
npm install
# veya
pnpm install
```

3. Geliştirme sunucusunu başlatın:
```bash
npm run dev
# veya
pnpm dev
```

4. Tarayıcınızda `http://localhost:4321` adresini açın.

### Tailwind CSS v4 Kullanımı

Bu proje Tailwind CSS v4 kullanmaktadır. Styling `src/styles/global.css` dosyasında yapılır:

```css
@import "tailwindcss";
@plugin "@tailwindcss/typography";
@plugin "@tailwindcss/forms";

@theme {
  /* Özel renkler ve tema ayarları burada */
}
```

## Proje Yapısı

```
/
├── public/              # Statik dosyalar (images, favicon, etc.)
├── src/
│   ├── components/      # Astro/Alpine.js componentleri
│   │   ├── global/      # Header, Footer, Navigation
│   │   ├── landing/     # Landing page bölümleri
│   │   └── forms/       # Form componentleri
│   ├── layouts/         # Sayfa layout'ları
│   ├── pages/          # Sayfalar (routing)
│   └── styles/         # CSS dosyaları
└── package.json
```

## Komutlar

Tüm komutlar proje kök dizininde terminal'den çalıştırılır:

| Komut                  | Açıklama                                         |
| :--------------------- | :----------------------------------------------- |
| `npm install`          | Bağımlılıkları yükler                            |
| `npm run dev`          | Geliştirme sunucusunu başlatır (`localhost:4321`) |
| `npm run build`        | Production build oluşturur (`./dist/`)           |
| `npm run preview`      | Build'i yerel olarak önizler                     |
| `npm run astro ...`    | Astro CLI komutlarını çalıştırır                |

## Özelleştirme

### Renkler ve Tema
Tema renkleri `src/styles/global.css` dosyasındaki `@theme` bölümünde özelleştirilebilir.

### İçerik Güncelleme
- Hero metinleri: `src/components/landing/Hero.astro`
- Özellikler: `src/components/landing/SectionOne.astro`
- Hedef kitle: `src/components/landing/SectionTwo.astro`
- Müşteri yorumları: `src/components/global/Testimonial.astro`

## Deployment

Bu proje Vercel, Netlify veya herhangi bir statik hosting sağlayıcısında deploy edilebilir.

### Vercel ile Deploy
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=your-repo-url)

## Lisans

Bu proje Covolt - Premium Enerji için özel olarak geliştirilmiştir.

---
Covolt Enerji Yönetimi Platformu © 2024
