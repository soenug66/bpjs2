# Generator Kartu Indonesia Sehat - GitHub Pages

Aplikasi HTML statis untuk input data peserta, preview kartu, generate PDF, dan cetak.

## Struktur

```text
kartu-bpjs/
├── index.html
├── README.md
└── assets/
    ├── template.png
    └── template.pdf
```

## Menjalankan lokal

Buka `index.html` menggunakan Chrome/Edge. Untuk hasil terbaik saat Generate PDF, gunakan koneksi internet karena aplikasi memuat `pdf-lib` dan `JsBarcode` dari jsDelivr.

## Deploy ke GitHub Pages

1. Buat repository GitHub, misalnya `kartu-bpjs`.
2. Upload seluruh isi folder ini.
3. Pastikan `index.html` berada di root repository.
4. Buka **Settings → Pages**.
5. Pada **Build and deployment**, pilih **Deploy from a branch**.
6. Pilih branch `main` dan folder `/ (root)`.
7. Simpan, lalu tunggu GitHub Pages selesai melakukan deployment.

URL umumnya:

`https://USERNAME.github.io/kartu-bpjs/`

## Catatan keamanan

Jangan menyimpan data peserta nyata, NIK, alamat, atau nomor kartu di source code/repository. Versi ini adalah frontend statis. Untuk aplikasi produksi dengan login, database, dan riwayat penerbitan, gunakan backend/database seperti Supabase dengan aturan akses yang sesuai.
