MirrorSync Download Site
========================

Isi paket:
- index.html
- latest.json

Cara pakai paling mudah:
1. Upload index.html dan latest.json ke root hosting/repository.
2. Buka index.html dari browser.
3. Setiap ada versi baru, update isi latest.json saja.
4. Tombol download di halaman akan otomatis mengikuti URL terbaru dari latest.json.

Jika halaman index.html tidak berada satu folder dengan latest.json:
- Buka index.html
- Cari bagian CONFIG
- Ubah fallbackLatestJsonUrl ke URL raw GitHub latest.json milik kamu.

Repo yang terbaca dari file contoh:
https://github.com/shyper21/local-android-mirror-releases

Catatan keamanan:
- File EXE tidak dijalankan/diperiksa oleh halaman ini.
- Jangan taruh token GitHub di index.html.
- Untuk repo private, pakai backend/proxy agar token tidak bocor.


UPDATE FOOTER:
- Footer modern sudah ditambahkan dengan teks "Created by Hachiman".
- Link download tetap otomatis membaca latest.json.
