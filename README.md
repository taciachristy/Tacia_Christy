# 📊 Superstore Capstone — Beginner Edition


## Project Overview
Tujuan proyek ini adalah menganalisis dataset Superstore untuk memahami faktor-faktor yang memengaruhi penjualan dan profitabilitas, serta memberikan rekomendasi perbaikan. Fokus analisis:
1) Mendeskripsikan struktur & kualitas data Superstore.
2) Membersihkan data (tanggal, duplikat, diskon tidak wajar).
3) Mengeksplorasi distribusi numerik (Sales, Profit, Discount, Quantity).
4) Menganalisis kontribusi kategori, segment, dan region terhadap kinerja penjualan & profit.
5) Melihat tren bulanan penjualan dan profit.

**Pendekatan**: Data understanding → Data cleaning → EDA → Insight & Rekomendasi


## Raw Dataset Link
- Sumber: Kaggle — *Superstore Dataset*: https://www.kaggle.com/datasets/ishanshrivastava28/superstore-sales
- File yang dianalisis: `Superstore.csv`


## Insight & Findings
- Sales dan Profit: distribusi tidak merata, banyak transaksi kecil dengan beberapa transaksi sangat besar.
- Profit margin tipis: ada banyak order dengan profit negatif meski sales tinggi → indikasi pricing atau diskon tidak efisien.
- Kategori:
 - Technology menghasilkan penjualan tertinggi.
 - Furniture dan Office Supplies juga signifikan, tapi margin profit bervariasi.
- Segment: Consumer menyumbang transaksi terbanyak dibanding Corporate dan Home Office.
- Region: West menghasilkan profit lebih baik dibanding Central.
- Time Series: terdapat fluktuasi musiman; akhir tahun cenderung lebih tinggi baik sales maupun profit.


## AI Support Explanation
- Data preparation: AI bantu membuat kode untuk membaca CSV, parsing tanggal, cek missing & duplicate.
- EDA: AI bantu menyusun kode eksplorasi (distribusi numerik, groupby kategori, visualisasi tren).
- Visualisasi: AI menghasilkan template grafik (histogram, bar chart, line chart time series).
- Insight: AI membantu merangkum output grafik (margin tipis, perbedaan region, dominasi kategori tertentu) menjadi insight bisnis.