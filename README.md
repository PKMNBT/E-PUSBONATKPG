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


## Pembaruan grafik SPM — v1.8
- Grafik 12 indikator SPM memakai dua warna berdasarkan rata-rata capaian aktual yang dihitung dari 12 indikator: hijau muda untuk capaian sama dengan/di atas rata-rata, oranye untuk capaian di bawah rata-rata.
- Warna tidak lagi berbeda per indikator. Perhitungan diperbarui otomatis mengikuti data SPM yang tersimpan.


## Pembaruan v1.9 — Tanggal Entri SPM dan Warna Grafik
- Grafik 12 indikator SPM menggunakan hijau muda untuk capaian sama dengan/di atas rata-rata 12 indikator dan oranye untuk capaian di bawah rata-rata.
- Form Edit SPM mencatat **Tanggal entri** (tanggal spesifik) sekaligus **Periode (bulan)**.
- Tanggal entri ditampilkan pada kartu indikator dan tabel monitoring dashboard serta ikut diekspor ke CSV/Excel.
- Data versi lama tetap dibaca; bila data lama belum memiliki tanggal entri, tanggal awal bulan dari periode lama digunakan sebagai nilai awal.


## Pembaruan v2.0 — Periode SPM
- Form SPM memakai satu kolom **Periode** bertipe tanggal lengkap (tanggal-bulan-tahun); kolom tanggal entri terpisah dihapus agar tidak ganda.
- Data periode SPM lama yang hanya berformat tahun-bulan dipertahankan dan dinormalisasi ke tanggal pertama pada bulan tersebut.
