# API Automation with Postman

Repository ini berisi Postman Collection lengkap dengan:
- Chaining API (CRUD)
- Environment variables
- Upload image test
- Eksekusi otomatis menggunakan Newman + HTML Report

---

## 📁 Project Structure
├─ collection.json

├─ env.json

├─ images/

   └─example.jpg

├─ README.md

## 🛠️ TOOLS YANG HARUS DIPERSIAPKAN 

✅ 1. Install NodeJS
Untuk bisa menjalankan Newman (Postman CLI Runner), Newman berjalan di Node.js, jadi harus install Node.js dulu.
- Download dari situs resmi: https://nodejs.org
- Pilih: LTS version (recommended)
- Install seperti aplikasi biasa (Next → Next → Finish)
- Cek apakah berhasil terinstall, lakukan perintah di cmd: node -v
- Harus muncul versi, contoh: v20.11.0
- ✓ NodeJS sudah terinstall


✅ 2. Install Newman via npm
- Lakukan perintah di cmd untuk install newman:  npm install -g newman
- Cek apakah berhasil, lakukan perintah di cmd: newman -v
- Jika muncul versi, contoh:5.3.2
✓ Newman sudah terinstall

✅ 3. Install Newman HTML Reporter 
- Lakukan perintah di cmd untuk install html report: npm install -g newman-reporter-htmlextra



## ▶️ CARA MENJALANKAN TEST


1. Jalankan API Testing dengan Newman
- Lakukan perintah berikut di cmd:  newman run collection.json -e env.json

2. Jalankan API Testing dengan Newman + HTML Report
- Lakukan perintah berikut di cmd: newman run collection.json -e env.json \ -r htmlextra --reporter-htmlextra-export report.html



