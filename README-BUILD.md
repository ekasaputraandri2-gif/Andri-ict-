# ICT Macros — build APK dengan GitHub Actions

## Isi proyek
- `ict-macros.html`: antarmuka aplikasi.
- `capacitor.config.json`: konfigurasi Capacitor Android.
- `.github/workflows/build-apk.yml`: workflow otomatis untuk membangun APK debug.

## Cara menjalankan build
1. Ekstrak isi ZIP ini.
2. Buat repository GitHub baru dan unggah **isi folder `ict-app`** ke root repository (sehingga folder `.github/workflows` berada di root repository).
3. Pastikan branch bernama `main`.
4. Buka tab **Actions** di repository dan pilih **Build APK**.
5. Klik **Run workflow**. Workflow juga berjalan otomatis saat ada push ke `main`.
6. Setelah selesai, buka run yang berstatus berhasil, lalu unduh artefak **`ict-macros-debug-apk`** pada bagian Artifacts.

## Lokasi APK
Di dalam artefak hasil unduhan, file APK berada di:
`android/app/build/outputs/apk/debug/app-debug.apk`

APK debug ini untuk pengujian/sideload, bukan APK rilis yang ditandatangani untuk publikasi Play Store. Build belum dijalankan oleh ZIP ini sendiri; APK baru tersedia setelah workflow GitHub Actions berhasil dijalankan.
