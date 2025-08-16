# Superstore Capstone 


## Project Overview
Tujuan proyek ini adalah menganalisis dataset **Superstore** untuk memahami faktor-faktor yang memengaruhi penjualan dan profitabilitas, serta menyusun rekomendasi yang **actionable**. Fokus analisis:
1) Identifikasi sub-kategori penyumbang utama revenue (Pareto 80/20)
2) Menemukan **ambang diskon** yang mulai membuat median profit menjadi negatif
3) Memetakan hotspot pesanan **rugi** (kombinasi wilayah × kategori)
4) (Opsional) Membangun baseline model klasifikasi **untung vs rugi**

**Pendekatan:** Data understanding → Data cleaning → EDA tematik → Insight & Rekomendasi


## Raw Dataset Link
- Sumber: Kaggle — *Superstore Dataset*: https://www.kaggle.com/datasets/ishanshrivastava28/superstore-sales
- File yang dianalisis: `Superstore.csv`


## Insight & Findings
- Insight 1: Ada masalah di profit margin - sales bisa tembus 110K namun profit hanya 18K maximal (margin cuma 16%). Penjualan naik-turun drastis tapi profit hampir flat, artinya ada inefisiensi operasional atau pricing strategy yang salah.
- Insight 2: Technology merupakan penjualan tertinggi namun selisihnya sedikit sekali dengan kategori lain. Hal tersebut baik pada diversifikasi risikonya, namun mengartikan belum ada kategori yang bener-bener "cash cow" untuk di-leverage maksimal.
- Insight 3: West region profit hampir 3x lipat Central region ini merupakan masalah besar. Kemungkinan ada masalah distribusi, kompetisi lokal, atau tim sales Central yang perlu di-revamp atau rombak total.
- Insight 4: Terlalu bergantung pada satu produk (Canon Copier) kalau kompetitor nyerang produk ini atau ada supply issue, langsung collapse. Produk lainnya gap-nya kejauhan.


## AI Support Explanation
- Data cleaning & pemahaman data: AI membantu menyiapkan kode untuk membaca data, mengatasi encoding error, parsing tanggal, dan cek missing/duplikat sehingga proses awal lebih cepat.
- Exploratory Data Analysis (EDA): AI menyarankan metode seperti Pareto 80/20, analisis diskon vs profit, dan tren time series untuk menemukan pola margin, profit, dan ketergantungan produk.
- Visualisasi & interpretasi: AI menghasilkan template grafik (barplot, lineplot, distribusi) untuk memvisualisasikan selisih sales-profit, perbandingan region, serta dominasi produk tertentu.
- Perumusan insight: AI membantu menyusun insight dari output grafik/tabel ke dalam bahasa bisnis (misalnya margin rendah, gap antar region, dominasi Canon Copier), sementara interpretasi akhir diverifikasi manual.
