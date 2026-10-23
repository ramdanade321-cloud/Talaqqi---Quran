# Talaqqi Qur'an — Proyek Android awal

Ini adalah **kode sumber proyek Android Studio**, bukan APK yang sudah dibangun.

## Fitur versi awal
- Mengambil daftar 114 surah melalui API AlQuran Cloud.
- Menampilkan teks Arab dan memutar audio per ayat.
- Pilihan qari: Mishary Alafasy, Abdurrahman As-Sudais, dan Mahmoud Khalil Al-Husary.
- Pengulangan audio ayat dengan pilihan 1, 3, 5, 10 kali atau tanpa batas.
- Tombol ayat sebelumnya/berikutnya.
- Mode latihan potongan yang menampilkan bagian awal teks ayat.

## Catatan penting
- Internet dibutuhkan.
- Mode potongan pada versi awal hanya menampilkan teks bertahap; audio masih membaca satu ayat penuh.
- Ketersediaan edisi qari bergantung pada API. Jika salah satu edisi tidak tersedia, coba qari lain.
- Bacaan dan audio harus diverifikasi dengan sumber tepercaya dan guru Al-Qur'an. Aplikasi ini tidak menilai tajwid/makhraj.
- API dan ketentuan penggunaan sumber audio perlu diperiksa sebelum aplikasi dipublikasikan secara luas.

## Cara membuka dan membangun APK
1. Instal Android Studio di komputer.
2. Ekstrak folder proyek ini.
3. Android Studio → **Open** → pilih folder `TalaqqiQuranAndroid`.
4. Tunggu Gradle Sync selesai. JDK 17 dan Android SDK Platform 35 diperlukan.
5. Pilih **Build → Build APK(s)**.
6. Jika berhasil, APK debug biasanya ada di `app/build/outputs/apk/debug/app-debug.apk`.
7. Uji pada HP Android sebelum dibagikan.

## Teknologi
- Kotlin, Android Views, MediaPlayer, HttpURLConnection, API AlQuran Cloud.


## Membuat APK melalui GitHub Actions (tanpa komputer)

1. Unggah semua isi folder proyek ini ke repositori GitHub bernama `Talaqqi-Quran`.
2. Buka tab **Actions** di repositori.
3. Jika diminta, izinkan GitHub Actions untuk repositori ini.
4. Pilih workflow **Build Talaqqi Quran APK**, lalu tekan **Run workflow** jika tombol tersedia.
5. Tunggu proses selesai. Buka proses yang berikon centang hijau.
6. Di bagian **Artifacts**, unduh `Talaqqi-Quran-APK`. Ekstrak ZIP hasil unduhan untuk mendapatkan `app-debug.apk`.

Catatan: ini adalah APK debug untuk uji coba, belum aplikasi rilis yang ditandatangani untuk Play Store. Build bisa gagal jika ada masalah kode atau konfigurasi yang perlu diperbaiki.
