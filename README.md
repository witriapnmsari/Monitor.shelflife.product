# 📦 ShelfLife Penerimaan Barang Banjarmasin MT

Aplikasi manajemen dan kalkulator otomatis persentase sisa masa simpan (*remaining shelf life*) barang saat penerimaan di gudang (**Goods Receipt / GR**). Dibuat khusus dengan tampilan mobile-friendly untuk kemudahan input menggunakan smartphone di area gudang.

---

## 🚀 Fitur Utama

- **Database Master Produk Lengkap (750+ SKU):**
  - Dilengkapi master data produk lengkap (Nabati, Richeese, Richoco, Nextar, Siip, Pink Lava, Time Break, Simba, dll).
  - Kolom lengkap: Kode Barang, Nama Produk, Isi Kemasan, Isi per Karton, Umur (Bulan), dan Standar Total Shelf Life (Hari).
- **Kalkulasi Sisa Umur Otomatis & Real-Time:**
  - Cukup masukkan **Tanggal Penerimaan** & **Tanggal Kadaluarsa (EXP)** dari fisik kemasan.
  - Otomatis menghitung **Sisa Hari**, **Persentase Sisa Umur (%)**, dan status penerimaan:
    - 🟢 **Lolos / Diterima ($\ge 75\%$)**: Standar FEFO langsung masuk rak gudang.
    - 🟡 **Review / Butuh Approval ($< 75\%$)**: Butuh persetujuan manajer / program fast moving.
    - 🔴 **Ditolak / Expired ($\le 0\%$ / Hari ini):** Retur ke supplier (RTV).
- **Menu Tambah Master Barang Baru:**
  - Tambah SKU / produk baru langsung dari HP yang otomatis tersimpan di LocalStorage.
- **Ekspor & Rekap Laporan Lengkap:**
  - 📊 **Download Excel (.xlsx)** dengan format rapi.
  - 📄 **Download CSV** untuk integrasi ERP / WMS.
  - 🖨️ **Cetak / Simpan PDF** format Berita Acara Gudang.
  - 💬 **Salin Ringkasan ke WhatsApp** untuk laporan instan ke grup koordinasi tim.
- **Offline First & Ringan:**
  - Tidak memerlukan database backend yang rumit, data tersimpan aman di browser/HP masing-masing.

---

## 🛠️ Struktur File

```
├── index.html        # Aplikasi web utama (UI, logic, dashboard & kalkulator)
├── master_data.js    # Database JavaScript 750+ produk master barang
├── master_data.json  # Data master barang dalam format JSON mentah
└── README.md         # Dokumentasi proyek
```

---

## 🌐 Cara Menjalankan via GitHub Pages

1. Buka repositori ini di GitHub.
2. Masuk ke menu **Settings** > **Pages**.
3. Pada bagian **Branch**, pilih `main` (atau `master`) dan folder `/ (root)`.
4. Klik **Save**.
5. Tunggu sekitar 1 menit, website Anda akan otomatis online di:
   `https://<username-github>.github.io/<nama-repo>/`

---

*Dibuat untuk operasional Gudang Banjarmasin MT.*
