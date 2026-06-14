MirrorSync Download Site
========================

Repo ini adalah halaman download MirrorSync. Source aplikasi dan asset release
resmi tetap berada di:
https://github.com/shyper21/local-android-mirror-releases

Sinkronisasi update:
- `latest.json` dibaca oleh `index.html` untuk menampilkan versi, link, dan SHA-256.
- Workflow `.github/workflows/sync-release.yml` menyinkronkan metadata dari repo
  release utama setiap 30 menit.
- Workflow juga dapat dijalankan manual melalui tab Actions > Sync MirrorSync
  release metadata > Run workflow.

Keamanan:
- Tidak ada token GitHub di `index.html`.
- Link installer hanya diarahkan ke GitHub Release resmi.
- Metadata divalidasi: versi semver, URL HTTPS GitHub Release, dan SHA-256.
- Halaman tidak menerima upload dan tidak mengumpulkan data HP atau user.

Versi metadata saat dokumen ini diperbarui: MirrorSync v1.3.1.

Created by Hachiman
