# Latihan Matematika SD (PWA)

Isi folder: `index.html` (aplikasi), `manifest.webmanifest`, `sw.js` (agar bisa offline), folder `icons/`.

## 1. Taruh di hosting (wajib HTTPS, gratis)
Pilih salah satu, lalu unggah SEMUA isi folder ini apa adanya:
- **Netlify**: buka app.netlify.com/drop, seret folder ini ke halaman itu. Selesai, Anda dapat alamat https://...netlify.app
- **GitHub Pages**: buat repository, unggah semua file, lalu Settings > Pages > Deploy from branch (main).
- **Cloudflare Pages**: Create project > Direct Upload > unggah folder ini.

PWA tidak bisa dipasang kalau dibuka langsung dari file di HP/komputer (file://); harus lewat alamat https.

## 2. Pasang di perangkat
- **Android (Chrome)**: buka alamat tadi > menu titik tiga > "Instal aplikasi" / "Tambahkan ke layar utama".
- **iPhone / iPad (Safari)**: buka alamat tadi di Safari > tombol Bagikan > "Tambah ke Layar Utama". (Harus Safari, bukan Chrome.)
- **Tablet Android / komputer (Chrome, Edge)**: ikon instal muncul di ujung kanan kolom alamat.

Setelah dibuka sekali dengan internet, aplikasi bisa dipakai offline.

## 3. Memperbarui aplikasi
Ganti isi `index.html`, lalu ubah angka versi di baris pertama `sw.js` (`math-sd-v1` menjadi `math-sd-v2`), dan unggah ulang. Perangkat akan mengambil versi baru saat dibuka dengan internet.

## 4. Catatan
- Akun (nama + PIN) dan hasil latihan tersimpan di penyimpanan perangkat masing-masing, tidak tersinkron antar perangkat. Menghapus data browser/aplikasi menghapus data latihan.
- Untuk APK/Play Store atau App Store: setelah PWA ini online, gunakan pwabuilder.com (masukkan alamat https tadi) atau Capacitor untuk membungkusnya.
