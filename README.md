# StoreApp - Product Catalog & Cart App

Aplikasi web e-commerce sederhana yang dikembangkan untuk Frontend Intern Technical Test. Aplikasi ini mengintegrasikan API DummyJSON, pengelolaan state global, serta antarmuka yang responsif.

## Tech Stack & Tools
- Framework: React.js (Vite)
- Styling: Tailwind CSS & Bootstrap Icons
- Routing: React Router DOM (v6)
- State Management: React Context API & LocalStorage
- API: DummyJSON API
- Tools: VS Code, GitHub

## Fitur Utama
1. API Logic & Katalog:
   - Halaman katalog produk dengan gambar, harga, rating, dan kategori.
   - Server-side pagination (limit 12 item per halaman).
   - Pencarian produk dengan fitur Debounce.
   - Filter berdasarkan kategori dan sorting harga/rating.
   - Halaman detail produk (/products/:id) lengkap dengan galeri dan ulasan.
   - State handling untuk Loading, Empty State, dan Error State.

2. State Management & Stok:
   - Keranjang belanja (tambah, ubah qty, hapus, kalkulasi total).
   - Indikator jumlah cart dan favorit di Navbar.
   - Fitur Favorit / Wishlist.
   - Persistensi data menggunakan LocalStorage.
   - Validasi batas stok produk.

3. Responsive UI:
   - Grid produk responsif (Mobile, Tablet, Desktop).
   - Navigation drawer untuk tampilan seluler.

## Alasan Pemilihan State Management
React Context API dipilih karena efisien untuk aplikasi skala kecil-menengah tanpa overhead Redux, memudahkan pembagian state keranjang/favorit ke seluruh komponen secara global, serta mudah diintegrasikan dengan LocalStorage.

## Cara Menjalankan Project
1. Clone Repository:
   git clone <LINK_REPOSITORY_GITHUB>
   cd store-app

2. Install Dependensi:
   npm install

3. Jalankan Mode Development:
   npm run dev