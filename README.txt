MirrorSync Download Site
========================

Repo ini adalah halaman download MirrorSync. Source aplikasi dan asset release
resmi tetap berada di:
https://github.com/shyper21/local-android-mirror-releases

Sinkronisasi update:
- `index.html` membaca `latest.json` langsung dari repo release utama setiap kali
  halaman dibuka, dengan cache-busting agar metadata lama tidak tersimpan.
- `latest.json` di repo ini dipakai sebagai fallback jika metadata utama sedang
  tidak dapat diakses.
- Halaman akan mengikuti release MirrorSync terbaru tanpa perlu mengubah HTML.

Keamanan:
- Tidak ada token GitHub di `index.html`.
- Link installer hanya diarahkan ke GitHub Release resmi.
- Metadata divalidasi: versi semver, URL HTTPS GitHub Release, dan SHA-256.
- Halaman tidak menerima upload dan tidak mengumpulkan data HP atau user.

Versi metadata saat dokumen ini diperbarui: MirrorSync v1.3.1.

Created by Hachiman
