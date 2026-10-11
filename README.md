# E-PUSBONAT — Puskesmas Naibonat

Aplikasi web statis untuk GitHub Pages. Buka `index.html` atau publikasikan folder ini melalui GitHub Pages.

## Login demo
- Username: `pkmnbt`
- Password: `nbt26`

## Fitur
- Dashboard 12 indikator SPM, rata-rata, grafik batang berwarna, ringkasan dan monitoring.
- Kelola indikator SPM dan hitung persentase otomatis.
- CKG, lima klaster pelayanan, catatan umum, tautan regulasi, pengaturan.
- Cetak / Simpan sebagai PDF melalui dialog cetak browser.
- Ekspor CSV yang kompatibel dengan Excel, impor/ekspor cadangan JSON.
- Pencarian menu/program, logout, layout responsif.

## Penting — batasan GitHub Pages
Versi ini menyimpan data di `localStorage` browser/perangkat yang digunakan. Data tidak tersinkron antarpegawai/perangkat dan tidak memiliki database pusat. Login statis hanya gerbang tampilan; kredensial dapat dilihat dari kode sumber, sehingga bukan autentikasi aman. Jangan gunakan untuk menyimpan data pasien yang dapat mengidentifikasi individu. Untuk penggunaan operasional dengan banyak pengguna, perlu backend/API, database, autentikasi server-side, kontrol akses, dan pencadangan.

## Hosting GitHub Pages
1. Buat repository GitHub.
2. Unggah `index.html` dan `README.md` ke root repository.
3. Buka **Settings → Pages**.
4. Pada **Build and deployment**, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu **Save**.
5. Tunggu deployment selesai, kemudian buka URL Pages yang ditampilkan GitHub.


## Pembaruan desain premium
Header atas toska glass premium, marquee berjalan dengan slogan, dan pencarian menu/indikator/program/catatan/regulasi.


## Logo
Logo E-PUSBONAT dari pengguna berada di `assets/logo-e-pusbonat.png` dan ditampilkan di sisi kanan header.


## Logo
Logo E-PUSBONAT disimpan lokal di `assets/logo-e-pusbonat.png` agar ikut ter-host di GitHub Pages. Logo Kementerian Kesehatan ditampilkan dari URL eksternal; jika sumber eksternal berubah, ganti `src` gambar Kemenkes di `index.html` dengan file logo resmi yang sudah diverifikasi.


## Identitas header
Logo E-PUSBONAT dari aset lokal ditampilkan di sidebar kiri. Logo Kementerian Kesehatan RI pada sisi kanan header memakai sumber unduhan dari halaman logo resmi Kemenkes; tampilannya membutuhkan akses internet. Footer tetap berada di alur dokumen (position: static), tidak fixed/sticky, sehingga tidak menutupi konten saat scroll.
