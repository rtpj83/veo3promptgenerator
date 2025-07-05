# Prompt Generator

Aplikasi web untuk generate prompt video menggunakan Google Gemini API.

## Setup

### 1. Konfigurasi API Key

Untuk menggunakan aplikasi ini, Anda perlu mendapatkan Google API Key:

1. Kunjungi [Google Cloud Console](https://console.cloud.google.com/)
2. Buat project baru atau pilih project yang sudah ada
3. Aktifkan Gemini API
4. Buat API Key di bagian Credentials

### 2. Setup File Konfigurasi

1. Copy file `config.example.js` menjadi `config.js`:
   ```bash
   cp config.example.js config.js
   ```

2. Edit file `config.js` dan ganti `your_google_api_key_here` dengan API key Anda:
   ```javascript
   const CONFIG = {
     GOOGLE_API_KEY: 'AIzaSyDO65JAzRl0aEry-xxxxxxxxxxxxxx' // Ganti dengan API key Anda
   };
   ```

### 3. Jalankan Aplikasi

Buka file `index.html` di browser Anda.

## Keamanan

- File `config.js` sudah ditambahkan ke `.gitignore` untuk mencegah API key ter-commit ke repository
- Jangan pernah commit file yang berisi API key asli
- Gunakan file `config.example.js` sebagai template

## Fitur

- Generate prompt Indonesia dan Inggris
- Upload gambar untuk deskripsi otomatis
- Character creator dengan AI
- Mode single scene dan conversation
- Sistem koin untuk penggunaan API

## Troubleshooting

Jika muncul error "API key tidak ditemukan":
1. Pastikan file `config.js` sudah dibuat
2. Pastikan API key sudah diisi dengan benar
3. Pastikan file `config.js` di-load sebelum `script.js` di HTML
