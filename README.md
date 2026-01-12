# Dashboard Garis Kemiskinan Jawa Barat

git add .
git commit -m "Initial commit"
git branch -M main
git push -u origin main
Proyek sederhana: halaman statis `index.html` berisi dashboard "Garis Kemiskinan Jawa Barat".

Deskripsi singkat
- Dashboard statis (HTML/CSS/JS) menampilkan ringkasan garis kemiskinan Jawa Barat (2022–2024), tabel, grafik, dan visual SNA sederhana.

Struktur proyek
- `index.html` — halaman dashboard utama (buka langsung di browser).
- `README.md` — dokumen ini.
- `.gitignore` — file pengecualian git.

Menjalankan lokal
- Cara paling mudah: buka file `index.html` di browser (double-click atau `Ctrl+O`).
- Untuk development dengan server lokal (opsional):
  - Jika Anda punya Python 3: `python -m http.server 8000` lalu buka `http://localhost:8000/`.
  - Atau gunakan VS Code Live Server extension.

Deploy ke GitHub (ringkas)
1) Jika belum membuat repo GitHub, buat repo baru di https://github.com/new.
2) Jalankan di PowerShell dari folder proyek:

```powershell
cd "c:\xampp\htdocs\AnalisisBigDataSosialEkonomi"
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<USERNAME>/<REPO_NAME>.git
git push -u origin main
```

Aktifkan GitHub Pages (opsional)
- Web: buka `Settings` → `Pages` di repo GitHub, pilih `Branch: main` dan folder `/ (root)`, lalu klik `Save`.
- CLI (jika `gh` terpasang):
  - `gh auth login`
  - `gh api -X POST /repos/<USERNAME>/<REPO_NAME>/pages -f source.branch=main -f source.path=/`

Catatan
- Jika Anda ingin, saya bisa membantu menyiapkan `gh` atau menjalankan langkah-langkah di terminal Anda.
- Jangan letakkan credential/token di file proyek.

Lisensi & Kontak
- Lisensi: tidak dispesifikasikan (tambahkan file `LICENSE` jika perlu).
- Kontak: tambahkan alamat email atau nama pemilik repo di GitHub.

Terakhir: beri tahu saya jika Anda mau saya aktifkan GitHub Pages (saya akan pandu atau jalankan perintah jika Anda mengizinkan). 