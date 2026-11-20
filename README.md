# Lucky Corporation HQ

Kantor 3D WebGL (Three.js) bergaya kantor kartun yang sibuk, dengan dinding bata, meja abu-abu, monitor tabung, tumpukan kertas, dan kertas beterbangan. Pegawainya tujuh manusia kartun kantoran orisinal: kemeja, dasi warna divisi, sebagian berkacamata. Lucky (CEO Assistant) menerima perintah, membagi tugas ke divisi yang tepat, lalu berjalan mengantarkannya ke meja karyawan.

| Karyawan | Divisi |
|---|---|
| Lucky | CEO Assistant · koordinator |
| Raka | Operasional Toko |
| Sinta | Sales & Target |
| Dimas | Tim & Shift |
| Nala | Kreatif & Konten |
| Bima | Laporan & Arsip |
| Tari | OFA Hub & SH Kit |

## Fitur

- Kantor 3D WebGL dengan cahaya dan bayangan nyata: geser untuk memutar, scroll/cubit untuk zoom, tombol Tur untuk kamera otomatis. Kalau browser tidak mendukung WebGL, papan tugas tetap berfungsi.
- Pegawai bergerak: berjalan dengan tangan dan kaki berayun, mengetik dengan layar monitor menyala, Lucky membawa kertas tugas, pegawai mengambil kopi, dan kertas beterbangan saat tugas selesai.
- Papan tugas: Antrian → Dikerjakan → Siap dicek → Selesai.
- Profil toko yang dibaca semua karyawan sebelum bekerja.

## Data OFA Hub

Di versi Claude, karyawan bisa membaca data asli toko dari spreadsheet OFA Hub (DSR/Dashboard RA, target bulanan, traffic, produk terlaris, stok pusat, barang masuk, promo, new arrival, blind counting, PICA, tinggalan, SH Kit) lewat koneksi Google Sheets pemilik. Kolom data pelanggan (telepon, email, nama) dibuang sebelum data dibaca AI. ID spreadsheet disimpan di pengaturan akun Claude, tidak di kode ini.

## Dua cara membuka

1. **Versi Claude (AI aktif)**: https://claude.ai/artifact/MhyzG7a3uGXQmWeSRT2uwg
   Karyawan benar-benar mengerjakan tugas dengan AI. Tugas tersimpan di akun Claude, dan hasilnya bisa disimpan ke Google Drive.
2. **Versi GitHub Pages**: `https://lukianprayoga-stack.github.io/LUCKYCORPORATIONEX/`
   Kantor 3D dan papan tugas berjalan penuh, dan tugas tersimpan di browser. AI hanya aktif di versi Claude, karena GitHub Pages tidak punya akses ke model AI.

## Mengaktifkan GitHub Pages

Settings → Pages → Build and deployment → Source: **Deploy from a branch** → Branch: `main` / `(root)` → Save. Tunggu 1–2 menit, lalu buka alamat di atas.

Semua kode ada di satu file: `index.html`.
