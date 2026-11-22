# Warga RT005 — Prototipe Portal Digital

Website responsif untuk administrasi lingkungan RT. Dibuat sebagai prototipe frontend statis yang dapat di-host gratis di Vercel.

## Jalankan lokal
Buka `index.html` di browser, atau jalankan server lokal:
```bash
python -m http.server 8000
```
Lalu buka `http://localhost:8000`.

## Deploy gratis ke Vercel
1. Buat repository GitHub baru, misalnya `warga-rt005-baru`.
2. Upload seluruh isi folder ini ke root repository (index.html harus berada di root).
3. Buka https://vercel.com/new dan impor repository tersebut.
4. Framework Preset: **Other**.
5. Build Command: kosongkan.
6. Output Directory: `.` (atau kosongkan jika Vercel mendeteksi static site).
7. Klik Deploy.

## Penting — status prototipe
Ini adalah prototipe frontend dengan data contoh di memori browser. Belum ada:
- Login/otorisasi sungguhan dan pemisahan peran warga/pengurus/bendahara.
- Database online, sinkronisasi antarperangkat, backup, dan audit log.
- Penyimpanan dokumen, tanda tangan elektronik, atau notifikasi WhatsApp.
- Perlindungan data pribadi dan kontrol akses produksi.

Jangan masukkan NIK, nomor KK, alamat rinci, atau data pribadi warga sungguhan ke versi demo. Tahap berikutnya adalah menghubungkan Supabase (paket gratis sesuai batas layanan) dan menambahkan Row Level Security serta autentikasi sebelum digunakan warga.
