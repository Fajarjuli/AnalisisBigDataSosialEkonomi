# Dashboard Garis Kemiskinan Jawa Barat

Proyek sederhana: halaman statis `index.html` berisi dashboard Garis Kemiskinan Jawa Barat.

## Tujuan
- Deploy ke GitHub dan (opsional) aktifkan GitHub Pages untuk hosting statis.

## Langkah cepat (di Windows PowerShell)
1. Inisialisasi git, commit file:

```
cd "c:\xampp\htdocs\AnalisisBigDataSosialEkonomi"
git init
git add .
git commit -m "Initial commit"
git branch -M main
```

2. Buat repo di GitHub dan push:

- Opsi A (menggunakan `gh` CLI):
```
gh repo create <USERNAME>/<REPO_NAME> --public --source=. --remote=origin --push
```
Ganti `<USERNAME>` dan `<REPO_NAME>`.

- Opsi B (manual via website):
  - Buat repo baru di https://github.com/new (jangan centang README).
  - Lalu jalankan:
```
git remote add origin https://github.com/<USERNAME>/<REPO_NAME>.git
git push -u origin main
```

3. (Opsional) Aktifkan GitHub Pages:
  - Buka `Settings` → `Pages` di repo GitHub, pilih `Source: main branch` lalu `Save`.
  - Tunggu beberapa menit, lalu buka URL Pages yang diberikan.

## File penting
- `index.html` — halaman dashboard
- `.gitignore` — file untuk mengecualikan file lokal

Jika mau, saya bisa:
- Membuat repo GitHub untuk Anda (butuh akses token/`gh` CLI), atau
- Menjalankan perintah git di terminal Anda (saya bisa berikan perintah yang tepat).