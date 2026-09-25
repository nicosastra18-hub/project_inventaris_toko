# ZAVEN Smart Inventory

Source lengkap website manajemen inventaris.

## Menjalankan website

1. Ekstrak arsip proyek ini.
2. Pastikan Node.js dan pnpm tersedia.
3. Buka terminal dari folder proyek, lalu jalankan:

   ```sh
   pnpm install
   pnpm dev
   ```

4. Buka URL lokal yang ditampilkan terminal.

Untuk membuka versi file statis, buka `client/index.html`; keenam berkas statisnya harus tetap berada dalam folder `client` yang sama. Instalasi PWA dan service worker membutuhkan localhost atau hosting HTTPS.

## Menghubungkan Supabase

Di aplikasi, buka **Pengaturan → Hubungkan Supabase**, lalu masukkan Project URL dan publishable key. Gunakan hanya `sb_publishable_...` (atau anon/public key yang memang untuk frontend). **Jangan pernah memasukkan `sb_secret_...` atau `service_role` key ke browser.**

Aplikasi mendukung login Supabase Auth dan tabel `products`, `categories`, serta `suppliers`. Aktifkan Row Level Security (RLS) dan kebijakan akses yang sesuai di Supabase sebelum memakai data cloud.

## Berkas statis

Di `client/` tersedia `index.html`, `style.css`, `app.js`, `manifest.json`, `service-worker.js`, dan `icon.png`.
