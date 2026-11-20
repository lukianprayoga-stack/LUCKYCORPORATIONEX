# Lucky Corporation HQ

Kantor 3D bergaya film animasi berisi tim karyawan AI pribadi untuk Store Head. Pegawainya adalah **Lucky Sprouts**, maskot orisinal Lucky Corporation: makhluk bulat dengan tunas daun semanggi di kepala dan syal berwarna sesuai divisi. Lucky (CEO Assistant) menerima perintah, membagi tugas ke divisi yang tepat, lalu berjalan mengantarkannya ke meja karyawan.

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

- Kantor 3D (CSS 3D murni, tanpa library): geser untuk memutar, scroll/cubit untuk zoom, tombol Tur untuk kamera otomatis.
- Karyawan bergerak: badan memantul saat berjalan, tunas berputar saat bekerja, melompat dengan kilauan saat tugas selesai, Lucky berjalan mengantar tugas, karyawan sesekali mengambil kopi.
- Papan tugas: Antrian → Dikerjakan → Siap dicek → Selesai.
- Profil toko yang dibaca semua karyawan sebelum bekerja.

## Dua cara membuka

1. **Versi Claude (AI aktif)**: https://claude.ai/artifact/MhyzG7a3uGXQmWeSRT2uwg
   Karyawan benar-benar mengerjakan tugas dengan AI. Tugas tersimpan di akun Claude, dan hasilnya bisa disimpan ke Google Drive.
2. **Versi GitHub Pages**: `https://lukianprayoga-stack.github.io/LUCKYCORPORATIONEX/`
   Kantor 3D dan papan tugas berjalan penuh, dan tugas tersimpan di browser. AI hanya aktif di versi Claude, karena GitHub Pages tidak punya akses ke model AI.

## Mengaktifkan GitHub Pages

Settings → Pages → Build and deployment → Source: **Deploy from a branch** → Branch: `main` / `(root)` → Save. Tunggu 1–2 menit, lalu buka alamat di atas.

Semua kode ada di satu file: `index.html`.
