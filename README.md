# 📊 Analisis Big Data Sosial Ekonomi

📌 **Dashboard Garis Kemiskinan Jawa Barat**

![Dashboard Garis Kemiskinan](ss1.png)

Dashboard Analisis Garis Kemiskinan Jawa Barat

Proyek ini merupakan aplikasi dashboard berbasis web yang dikembangkan untuk menganalisis dan memvisualisasikan data garis kemiskinan di Provinsi Jawa Barat menggunakan pendekatan Big Data Analytics, visualisasi interaktif, dan Social Network Analysis (SNA). Dashboard ini bertujuan membantu pengguna memahami tren kemiskinan serta faktor sosial ekonomi yang memengaruhinya secara komprehensif.

Sorotan Utama

Visualisasi tren garis kemiskinan Jawa Barat periode 2022–2024.

Analisis data time series untuk melihat pola kenaikan dari waktu ke waktu.

Social Network Analysis (SNA) untuk memetakan keterkaitan antara tahun dan faktor sosial ekonomi.

Dashboard interaktif berbasis web dengan grafik, tabel, dan filter dinamis.

Fitur ekspor data ke format CSV untuk analisis lanjutan.

Arsitektur Singkat

Struktur proyek dirancang modular agar mudah dikembangkan dan dipelihara:

dashboard/
Aplikasi utama dashboard (HTML, CSS, JavaScript, visualisasi grafik dan SNA).

data/
Penyimpanan data mentah dan data hasil pemrosesan.

src/
Modul logika analisis data, termasuk pembersihan data dan analisis jaringan sosial.

assets/
Aset pendukung seperti logo, ikon, dan gambar visualisasi.

Sumber Data

Data yang digunakan dalam proyek ini berasal dari data terbuka pemerintah yang memuat informasi garis kemiskinan Provinsi Jawa Barat. Data dikumpulkan dalam format terstruktur dan diproses untuk memastikan konsistensi, kelengkapan, serta kesiapan analisis.

Metodologi

Proyek ini menggunakan metodologi Data Analytics Pipeline, yang meliputi tahap pengumpulan data melalui teknik web scraping dan data terbuka, pemrosesan data menggunakan data cleaning dan normalisasi, serta analisis data dengan pendekatan time series analysis dan Social Network Analysis (SNA). Seluruh hasil analisis disajikan dalam bentuk dashboard visual interaktif.

Social Network Analysis (SNA)

Analisis jaringan sosial digunakan untuk memvisualisasikan hubungan antara tahun pengamatan dan faktor sosial ekonomi seperti inflasi, harga pangan, dan biaya hidup. Metrik sederhana seperti degree centrality diterapkan untuk mengidentifikasi faktor yang paling dominan memengaruhi perubahan garis kemiskinan.

Menjalankan Aplikasi Secara Lokal

Pastikan Python sudah terpasang.

Jalankan perintah berikut di terminal:

python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt


Jalankan dashboard:

streamlit run dashboard/app.py


Aplikasi akan berjalan di:

http://localhost:8501

Opsi Deployment
1. Streamlit Community Cloud

Push repository ke GitHub.

Buka https://share.streamlit.io.

Pilih repository, branch, dan file utama (dashboard/app.py).

Deploy aplikasi secara langsung.

2. Docker (VPS / Cloud)

Contoh Dockerfile:

FROM python:3.11-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
EXPOSE 8501
CMD ["streamlit", "run", "dashboard/app.py", "--server.port=8501", "--server.address=0.0.0.0"]

Kesimpulan

Dashboard ini menunjukkan bahwa garis kemiskinan di Provinsi Jawa Barat mengalami peningkatan secara konsisten dalam beberapa tahun terakhir. Dengan pendekatan Big Data dan visualisasi interaktif, proyek ini dapat menjadi alat bantu analisis yang efektif bagi akademisi, pemerintah, dan masyarakat dalam memahami dinamika kemiskinan serta faktor-faktor yang memengaruhinya.
---

## 🧾 Deskripsi

Repositori ini berisi:

- `index.html` — Halaman dashboard utama  
- Beberapa asset seperti gambar/logo untuk visualisasi  
- Dokumen README ini sebagai dokumentasi  
- `.gitignore` untuk mengelola file yang diabaikan oleh Git  

Dashboard ini menampilkan **tabel, grafik, dan gambaran ringkas garis kemiskinan** yang bisa digunakan sebagai bahan laporan atau presentasi analisis sosial ekonomi.

---


🛠️ Teknologi yang Digunakan
✨ HTML, CSS dan JavaScript untuk front-end
📈 Visualisasi dashboard tanpa backend
📁 Struktur sederhana untuk kemudahan modifikasi

Terima kasih sudah melihat proyek ini! 🚀
