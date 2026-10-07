# RT 005/05 Cilodong — Versi 1

## 1. Backend
1. Buat Google Spreadsheet kosong.
2. Extensions > Apps Script.
3. Masukkan `backend/Code.gs` dan `backend/appsscript.json`.
4. Isi `SPREADSHEET_ID` dengan ID Spreadsheet.
5. Jalankan `setupDatabase()` sekali dan beri izin.
6. Deploy > New deployment > Web app.
7. Execute as: Me.
8. Atur akses sesuai kebutuhan.
9. Salin URL `/exec`.

Akun awal: **admin / admin123**. Segera ganti setelah login pertama.

## 2. Frontend GitHub Pages
1. Upload seluruh isi folder `frontend` ke repository GitHub.
2. Masukkan logo resmi sebagai `assets/logo-rt005.png`.
3. Edit `js/config.js` dan isi `API_URL` dengan URL Web App `/exec`.
4. Aktifkan GitHub Pages.
5. Buka URL GitHub Pages.

## 3. Keamanan
- Jangan menyimpan password, API key, token WhatsApp, credential CCTV, atau secret pembayaran di frontend.
- Versi 1 adalah fondasi login/dashboard/database. Endpoint CRUD untuk warga, kas, panic, CCTV, QRIS, dan WhatsApp harus divalidasi server-side sebelum dipakai operasional.
