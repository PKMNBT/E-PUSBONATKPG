# E-PUSBONAT — Mobile Premium v1.7

Pembaruan responsif berbasis file aplikasi yang dipilih pengguna. Struktur data dan handler aplikasi dipertahankan; perubahan difokuskan pada visual responsif, foto header, dan perilaku drawer menu di layar kecil.

## Instalasi GitHub Pages
1. Unggah `index.html`, `README.md`, dan folder `assets` ke root repository.
2. Pilih Settings → Pages → Deploy from a branch → `main` → `/(root)`.
3. Setelah deploy, lakukan hard refresh di browser.

## Yang diperbaiki
- Foto header dipasang inline sebagai WebP teroptimasi sehingga tetap tampil walau aset lokal tidak ikut terunggah; file aset juga tetap disediakan.
- Foto header HP diberi area yang cukup dan fokus gambar diarahkan ke matahari/senja, tanpa blur tambahan.
- Menu HP menjadi drawer dengan lebar maksimum 84% layar, backdrop, penguncian scroll latar, dan penutupan lewat tap di luar, tombol navigasi, atau Escape.
- Kartu, label grafik, form, tabel, dan footer menyesuaikan lebar layar serta sudut membulat.

## Catatan data
Versi ini tetap aplikasi statis yang menggunakan localStorage di browser/perangkat. Tidak tersinkron antarpengguna dan bukan sistem aman untuk data pasien yang dapat mengidentifikasi individu.
