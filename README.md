# 🍪 Azmi Products — Website Roti Kering Premium

<div align="center">

![Azmi Products Banner](https://images.unsplash.com/photo-1509440159596-0249088772ff?q=80&w=1200&auto=format&fit=crop)

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![WhatsApp](https://img.shields.io/badge/WhatsApp_Order-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/6289677803066)

> **Website toko kue kering & roti premium handmade dengan UI/UX modern, animasi kekinian, dan sistem keranjang belanja terintegrasi WhatsApp.**

[🌐 Live Demo](https://rynero932-hue.github.io/azmiproducts/) · [📱 Pesan Sekarang](https://wa.me/6289677803066) · [🛍️ Shopee](https://shopee.co.id/albarakahstore11)

</div>

---

## 📋 Daftar Isi

- [Tentang Project](#-tentang-project)
- [Fitur Unggulan](#-fitur-unggulan)
- [Tampilan Website](#-tampilan-website)
- [Struktur Halaman](#-struktur-halaman)
- [Teknologi](#-teknologi)
- [Cara Pakai](#-cara-pakai)
- [Kustomisasi](#-kustomisasi)
- [Produk](#-daftar-produk)
- [Kontak](#-kontak)

---

## 🎯 Tentang Project

**Azmi Products** adalah website toko kue kering & roti premium berbasis HTML/CSS/JS murni (tanpa framework), didesain dengan pendekatan **mobile-first** dan pengalaman pengguna yang mulus di semua ukuran layar.

Website ini berfungsi sebagai **katalog digital + landing page + mini e-commerce** yang terhubung langsung ke WhatsApp untuk proses pemesanan — tanpa backend, tanpa database, siap deploy di mana saja.

### 🏆 Keunggulan
- ✅ **Zero dependency** — HTML/CSS/JS murni, tidak butuh Node.js atau framework apapun
- ✅ **Ringan & cepat** — satu file HTML, loading instan
- ✅ **Fully responsive** — optimal di HP, tablet, dan PC
- ✅ **WhatsApp ready** — order langsung generate pesan otomatis ke WA admin

---

## ✨ Fitur Unggulan

### 🎨 UI & Animasi
| Fitur | Deskripsi |
|-------|-----------|
| **Loading Screen** | Animasi progress bar saat halaman pertama dibuka |
| **Hero Section** | Gambar utama melayang (float animation) dengan tag dinamis |
| **Marquee Strip** | Teks berjalan otomatis menampilkan nama produk |
| **Scroll Reveal** | Elemen muncul dengan animasi saat di-scroll (slide, scale, fade) |
| **Hover Effects** | Kartu produk terangkat dan zoom saat disentuh/hover |
| **Scroll Spy** | Navigasi otomatis highlight menu sesuai posisi scroll |

### 🧭 Navigasi
| Perangkat | Navigasi |
|-----------|----------|
| **Desktop / PC** | Pill nav bar transparan di atas dengan tombol aktif bergradient |
| **Mobile / HP** | Bottom tab bar menempel di bawah layar (seperti aplikasi native) |
| **Hamburger Menu** | Dropdown dari atas dengan grid 2 kolom + shortcut WA |

### 🛒 Sistem Belanja
- **Keranjang belanja** — tambah, kurangi, hapus produk
- **Filter katalog** — saring produk by kategori (Nastar, Cookies, Brownies)
- **Cart drawer** — slide-in dari kanan, tidak mengganggu halaman utama
- **Auto-generate WA message** — saat checkout, pesan otomatis terformat rapi ke WhatsApp
- **LocalStorage** — isi keranjang tersimpan walau browser ditutup
- **Toast notification** — konfirmasi saat produk berhasil ditambahkan

---

## 📸 Tampilan Website

```
┌─────────────────────────────────────┐
│  🍪 Azmi Products    [Pill Nav] [🛒] │  ← Top Navbar (Desktop)
├─────────────────────────────────────┤
│                                     │
│   HERO SECTION                      │
│   Judul • Deskripsi • CTA Buttons   │
│   Stats: 500+ Pelanggan | 9+ Varian │
│                                [📸] │  ← Floating images
├─────────────────────────────────────┤
│  ✦ Nastar ✦ Cookies ✦ Almond ✦ ... │  ← Marquee strip
├─────────────────────────────────────┤
│  TENTANG KAMI                       │
│  [Foto kolase] | Teks + Poin        │
├─────────────────────────────────────┤
│  KATALOG PRODUK                     │
│  [Filter] [Semua|Nastar|Cookies|..] │
│  ┌──┐ ┌──┐ ┌──┐ ┌──┐              │
│  │🍪│ │🍪│ │🍪│ │🍪│  ← Cards    │
│  └──┘ └──┘ └──┘ └──┘              │
├─────────────────────────────────────┤
│  TESTIMONI                          │
│  ◀ [Card] [Card] [Card] ▶          │
├─────────────────────────────────────┤
│  CARA PESAN  1→2→3→4               │
├─────────────────────────────────────┤
│  CTA — Pesan via WhatsApp           │
├─────────────────────────────────────┤
│  FOOTER                             │
│  Logo | Menu | Produk | Sosial      │
└─────────────────────────────────────┘
         [🏠][🛍️][📋][⭐][🛒]       ← Bottom Nav (Mobile only)
```

---

## 📂 Struktur Halaman

```
azmi-products.html
│
├── #loader          → Loading screen animasi
├── #navbar          → Top navigation (desktop)
├── .mob-menu        → Dropdown menu (mobile hamburger)
├── .btm-nav         → Bottom tab bar (mobile)
│
├── #hero            → Hero section utama
├── .marquee-wrap    → Strip teks berjalan
├── #about           → Tentang Kami
├── #produk          → Katalog produk + filter
├── #testimoni       → Slider testimoni pelanggan
├── #cara-pesan      → 4 langkah cara pesan
├── #cta             → Call-to-action WhatsApp
└── footer           → Footer + sosial media
    │
    ├── .cart-overlay  → Background overlay keranjang
    └── .cart-drawer   → Panel keranjang belanja
```

---

## 🛠️ Teknologi

```
Frontend:
├── HTML5            — Struktur semantik
├── CSS3             — Styling, animasi, responsive
│   ├── CSS Variables (--cream, --gold, --brown-dark, dll)
│   ├── Grid & Flexbox layout
│   ├── @keyframes animations
│   ├── Intersection Observer API (scroll reveal)
│   └── backdrop-filter blur (glassmorphism)
│
└── Vanilla JavaScript
    ├── Cart state management (localStorage)
    ├── IntersectionObserver (scroll reveal)
    ├── Scroll spy (active nav highlight)
    └── WhatsApp deep link (wa.me)

Fonts (Google Fonts):
├── Playfair Display — Heading & display text
└── DM Sans         — Body & UI text
```

---

## 🚀 Cara Pakai

### 1. Download / Clone
```bash
# Jika pakai Git
git clone https://github.com/username/azmi-products.git

# Atau langsung download file
# azmi-products.html → buka di browser
```

### 2. Buka di Browser
```
Cukup double-click file azmi-products.html
→ Langsung terbuka di browser, tidak perlu server
```

### 3. Deploy ke GitHub Pages
```bash
# 1. Buat repository baru di GitHub
# 2. Upload azmi-products.html → rename jadi index.html
# 3. Settings → Pages → Deploy from main branch
# 4. Website live di: https://username.github.io/repo-name/
```

### 4. Deploy ke Netlify / Vercel
```
1. Drag & drop folder ke netlify.com/drop
2. Selesai — dapat URL gratis langsung
```

---

## ⚙️ Kustomisasi

### Ganti Nomor WhatsApp Admin
Cari dan ganti teks berikut di dalam file HTML:

```javascript
// Di bagian JavaScript — fungsi checkout()
window.open(`https://wa.me/6289677803066?text=...`)

// Di HTML — tombol WA di section CTA
href="https://wa.me/6289677803066"
href="https://wa.me/6282326501499"
```

### Tambah / Edit Produk
Temukan array `products` di bagian `<script>`:

```javascript
const products = [
  {
    id: 10,                    // ID unik (angka)
    name: "Nama Produk Baru",  // Nama produk
    tag: "New",                // Label badge (Best Seller, New, dll)
    cat: "cookies",            // Kategori: nastar | cookies | brownies
    price: 65000,              // Harga dalam Rupiah (angka)
    desc: "Deskripsi singkat produk",
    img: "https://url-gambar-produk.jpg"
  },
  // ... produk lainnya
];
```

### Ubah Warna Tema
Edit CSS variables di `:root`:

```css
:root {
  --cream: #fdf6ec;      /* Warna latar belakang utama */
  --warm: #f5e6cc;       /* Warna latar hangat */
  --gold: #c8963e;       /* Warna aksen emas */
  --gold-light: #e8b96a; /* Aksen emas terang */
  --brown: #5c3d1e;      /* Warna coklat medium */
  --brown-dark: #3a2310; /* Warna coklat gelap */
}
```

### Tambah Kategori Filter Baru
```html
<!-- Di HTML -->
<button class="filter-btn" data-filter="namakategori">Label Kategori</button>

<!-- Di data produk, sesuaikan cat -->
{ cat: "namakategori", ... }
```

---

## 🍪 Daftar Produk

| No | Produk | Kategori | Harga |
|----|--------|----------|-------|
| 1 | Nastar Premium | Nastar | Rp 85.000 |
| 2 | Nastar Ekonomis | Nastar | Rp 45.000 |
| 3 | Thumbprint Cookies | Cookies | Rp 48.000 |
| 4 | Noir Choco Cookies | Cookies | Rp 70.000 |
| 5 | Almond London | Cookies | Rp 70.000 |
| 6 | Lidah Kucing | Cookies | Rp 70.000 |
| 7 | Sagu Keju | Cookies | Rp 65.000 |
| 8 | Choco Cheese Bites | Cookies | Rp 55.000 |
| 9 | Brownies Fudge Topping | Brownies | Rp 77.000 |

> Semua kue kering dalam kemasan **toples 600ml** kecuali Brownies Fudge (per loyang).

---

## 📞 Kontak

<div align="center">

| Channel | Info |
|---------|------|
| 📱 **Admin 1 (WA)** | [0896-7780-3066](https://wa.me/6289677803066) |
| 📱 **Admin 2 (WA)** | [0823-2650-1499](https://wa.me/6282326501499) |
| 📱 **Admin 3 (WA)** | [0821-3805-1011](https://wa.me/6282138051011) |
| 📸 **Instagram** | [@azmiproducts](https://www.instagram.com/nayluvar_lavirlaez.04/) |
| 🛍️ **Shopee** | [albarakahstore11](https://shopee.co.id/albarakahstore11) |
| 📍 **Lokasi** | [Lihat di Google Maps](https://maps.app.goo.gl/mpJN6RYazo99SKJ7A) |

</div>

---

## 📄 Lisensi

Project ini dibuat khusus untuk **Azmi Products** © 2026. Seluruh konten, desain, dan foto produk adalah milik Azmi Products.

---

<div align="center">

**Dibuat dengan ❤️ untuk Azmi Products**

*Kue Homemade Premium • Sekali Coba Pasti Repeat Order*

</div>
