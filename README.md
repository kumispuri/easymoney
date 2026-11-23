# easymoney — Pelacak Keuangan Pribadi & Berdua

Aplikasi web pelacak keuangan modern berbasis **single HTML file** tanpa server atau login, siap pakai langsung di browser atau di-deploy ke GitHub Pages.

## 🚀 Fitur Lengkap

### 🏠 Beranda
- Kartu saldo premium bergaya kartu debit/kredit metal (easymoney card) lengkap dengan EMV Chip, Contactless NFC, efek 3D tilt, shimmer glossy, dan tombol sembunyikan saldo (👁️)
- Pilihan mata uang langsung di kartu & header (Rupiah IDR, Yen JPY, USD, Euro EUR)
- Ringkasan pemasukan & pengeluaran bulan ini
- Banner dompet tabungan (terpisah dari saldo harian)
- **Catat Pintar AI** — input multi-item sekaligus (mis: `beli kopi 20rb sama makan 30rb` atau `lunch 15 usd dan coffee 5$`)
- Daftar 5 transaksi terakhir

### 📋 Riwayat
- Pencarian real-time
- Filter jenis: Semua / Pemasukan / Pengeluaran
- Filter anggota: Semua / Member 1 / Member 2

### 🏦 Tabungan
- Total dompet tabungan (terpisah dari saldo harian)
- Buat banyak kantong dengan nama, target, warna
- Progress bar menuju target
- Tombol **+ Nabung** dan **– Tarik** per kantong

### 📊 Laporan
- Navigasi bulan (← →)
- Pengeluaran per kategori (bar chart sederhana + persentase)
- Pemasukan per sumber
- Rincian per orang (income, expense, net, jumlah transaksi)

### 🏷️ Kategori
- Manajemen kategori pemasukan & pengeluaran bersih dan rapi
- Tambah kategori/sumber baru dengan pilihan warna & ikon

### ⚙️ Pengaturan (Modal Sheet)
- Pilihan mata uang: 🇮🇩 IDR (Rp), 🇯🇵 JPY (¥), 🇺🇸 USD ($), 🇪🇺 EUR (€)
- Atur nama 2 anggota
- Mode tema: Terang / Gelap / Otomatis
- Palet warna: Light Blue, Burgundy, Sage, Sunset
- Ganti bahasa: 🇮🇩 Indonesia / 🇬🇧 English
- **Ekspor JSON** — backup data ke file
- **Impor JSON** — restore data dari file
- **Hapus Semua Data** — reset dengan konfirmasi ganda

## 📁 Struktur File
```
finance-tracker/
└── index.html   ← Semua kode (HTML + CSS + JS) dalam 1 file
```

## 🌐 Deploy ke GitHub Pages

1. Buat repo baru di GitHub (mis: `finance-tracker`)
2. Upload `index.html` ke repo
3. Buka **Settings → Pages → Branch: main → / (root) → Save**
4. Akses di `https://<username>.github.io/<repo>/`

## 💾 Penyimpanan Data
Semua data tersimpan di **LocalStorage** browser — tidak ada server, tidak ada login.  
Gunakan fitur **Ekspor JSON** secara berkala sebagai cadangan.

## 🧑‍💻 Teknologi
- Vanilla HTML5 / CSS3 / JavaScript (ES6+)
- Tidak ada dependensi eksternal
- Responsif: mobile & desktop
- PWA-ready (tambahkan `manifest.json` untuk install ke homescreen)
