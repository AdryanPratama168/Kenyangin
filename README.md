# Kenyangin — Company Profile

Website profil usaha sederhana untuk **Kenyangin**, bisnis kuliner yang menjual
**egg drop sandwich** dan **dessert box**. Dibuat sebagai tugas mata kuliah
Entrepreneurship sekaligus halaman jualan yang bisa dipakai langsung.

Situs ini statis (HTML + CSS + JavaScript murni), tanpa build step dan tanpa
dependency — cukup buka `index.html` atau host gratis di GitHub Pages.

## Isi halaman

| Bagian | Keterangan |
| --- | --- |
| Hero | Tagline, ringkasan produk, tombol pesan WhatsApp |
| Tentang | Latar belakang usaha dan alasan pemilihan nama |
| Menu | 3 varian egg drop sandwich + 3 varian dessert box, harga, dan label |
| Visi & Misi | Visi dan 6 poin misi |
| Kenapa Kami | Tiga keunggulan + kutipan tim |
| Galeri | Enam foto produk |
| Cara Pesan | Tiga langkah pemesanan + CTA WhatsApp |
| Footer | Navigasi, kontak, jam layanan |

## Struktur folder

```
kenyangin/
├── index.html
├── assets/
│   ├── css/style.css
│   ├── js/main.js
│   └── img/            # foto produk (stok, lihat CREDITS.md)
├── CREDITS.md          # atribusi foto
└── README.md
```

## Menjalankan secara lokal

Buka `index.html` langsung di browser, atau jalankan server statis:

```bash
python3 -m http.server 8080
# lalu buka http://localhost:8080
```

## Yang perlu diganti sebelum dipakai jualan

1. **Nomor WhatsApp** — ganti `6281234567890` (ada di 3 tempat: nav, hero, CTA, dan floating button).
2. **Instagram & email** — ganti `@kenyangin.id` dan `halo@kenyangin.id` di bagian footer.
3. **Harga menu** — sesuaikan angka di `index.html` pada blok `#menu`.
4. **Foto produk** — ganti file di `assets/img/` dengan foto asli produk.
   Nama file boleh sama supaya tidak perlu mengubah HTML; kalau berbeda,
   sesuaikan atribut `src` dan `alt`.
5. **Jam layanan & alamat** — sesuaikan di footer.

## Deploy gratis

**GitHub Pages**

1. Buka *Settings → Pages* pada repo ini.
2. Source: `Deploy from a branch`, branch `main`, folder `/ (root)`.
3. Simpan, lalu situs tersedia di `https://<username>.github.io/kenyangin/`.

**Netlify / Vercel / Cloudflare Pages** — drag & drop folder ini, tidak perlu konfigurasi.

## Kredit

Foto produk memakai gambar stok berlisensi bebas dari Wikimedia Commons.
Detail dan atribusi lengkap ada di [CREDITS.md](CREDITS.md).
Kode situs bebas dipakai ulang (MIT).
