# Rapikan Resi

Aplikasi untuk menggabung PDF resi TikTok, mengelompokkan per produk, menambah halaman keterangan, dan memberi nama packer + gambar PNG di bawah tiap resi. Semua diproses di browser, tidak ada file yang dikirim ke server.

## Upload ke GitHub dan aktifkan GitHub Pages
1. Buat repository baru di github.com (misal `rapikan-resi`), set **Public**.
2. Klik **Add file > Upload files**, lalu drag semua file di folder ini (`index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`). Klik **Commit changes**.
3. Buka **Settings > Pages**. Di bagian **Build and deployment**, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu **Save**.
4. Tunggu 1-2 menit. Alamatnya: `https://USERNAME.github.io/rapikan-resi/`

## Install di PC
Buka alamat di Chrome atau Edge, lalu klik ikon **Install** di ujung kanan address bar (atau menu titik tiga > **Cast, save, and share > Install page as app** di Chrome / **Apps > Install this site as an app** di Edge). Aplikasi muncul di Start Menu dan desktop seperti program biasa.

## Fitur
- Resi dikelompokkan per produk (A-Z), Express dulu baru Cargo. Di tiap jenis, resi Qty lebih dari 1 ditaruh di urutan terakhir, dilingkari, dan diberi kotak "Qty : N".
- Gambar "Jangan lupa video unboxing" sudah tertanam di aplikasi dan otomatis dipasang di bawah semua resi bersama nama packer.

## Catatan
- Buka sekali dengan internet. Setelah itu library dan font tersimpan, jadi bisa dipakai offline.
- Kalau mengganti file di GitHub dan tampilan belum berubah, ubah `CACHE = 'rapikan-resi-v1'` di `sw.js` menjadi `v2` (dan seterusnya) agar versi baru terambil.
- Tidak bisa dibuka dengan klik dua kali (`file://`) untuk fitur install. Fitur install hanya jalan dari alamat https GitHub Pages. Tapi `index.html` tetap bisa dipakai biasa kalau dibuka langsung, selama ada internet.
