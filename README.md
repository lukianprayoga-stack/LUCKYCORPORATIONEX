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

## Divisi

**Operasional Toko** (manusia kartun kantoran): Lucky (CEO Assistant), Raka, Sinta, Dimas, Nala, Bima, Tari.

**Lukky Studio** (Lucky Sprouts, ruang kedua di sebelah kanan): Pip (Produk & Template), Mochi (Konten Instagram), Kiko (Order & Admin DM), Tumi (Jasa Custom & Dashboard), Bobo (Keuangan Studio), Zuzu (Video Clipper). Mereka membaca Profil Lukky Studio dan catatan penjualan (identitas pembeli disembunyikan). Profil dan ID spreadsheet disimpan di pengaturan akun Claude, tidak di kode ini.

Tombol di kiri atas kantor memindahkan kamera: Operasional Toko · Lukky Studio · Semua.

## Produksi konten

- **Carousel otomatis:** hasil Mochi yang berisi blok `slides` dirender menjadi slide 1080x1350 bergaya Lukky Studio; unduh per slide (PNG) atau semua (ZIP).
- **Video Clipper (Zuzu), mode link:** tempel link YouTube (atau Google Drive, Vimeo, dll.) + kredit kreator, centang izin program clipper. Video diproses di server OpusClip lewat koneksi OpusClip pemilik (memakai kuota OpusClip; bisa dibatasi ke bagian video tertentu). Klip 9:16 bercaption muncul dengan skor, caption + kredit, pratinjau, dan tombol Siapkan/Unduh HD. Progres dicek lagi otomatis saat dashboard dibuka.
- **Video Clipper (Zuzu), mode upload:** upload video + tempel transkrip (YouTube: Tampilkan transkrip) + kredit kreator, centang izin program clipper. Zuzu memilih momen terbaik (atau isi momen manual), lalu klip 9:16 dirender di browser dengan judul hook, subtitle, dan kredit sumber. Hasil MP4 (H.264; AAC jika browser mendukung) atau WebM, lengkap dengan caption + hashtag. Render berjalan secepat durasi klip; biarkan tab tetap terbuka. Di GitHub Pages, AI tidak aktif, jadi isi momen manual.
- **Paket konten tiap pagi:** tugas terjadwal di akun Claude membuat ide, carousel PNG, caption, story, dan naskah reels, menyimpannya ke Google Drive ("Lukky Studio – Konten Harian"), dan mencatatnya di papan atas nama Mochi.

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
