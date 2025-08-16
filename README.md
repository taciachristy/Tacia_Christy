# 📊 Superstore Capstone — Beginner Edition


## Project Overview
Tujuan proyek ini adalah menganalisis dataset **Superstore** untuk memahami faktor-faktor yang memengaruhi penjualan dan profitabilitas, serta menyusun rekomendasi yang **actionable**. Fokus analisis:
1) Identifikasi sub-kategori penyumbang utama revenue (Pareto 80/20)
2) Menemukan **ambang diskon** yang mulai membuat median profit menjadi negatif
3) Memetakan hotspot pesanan **rugi** (kombinasi wilayah × kategori)
4) (Opsional) Membangun baseline model klasifikasi **untung vs rugi**

**Pendekatan:** Data understanding → Data cleaning → EDA tematik → (Opsional) Modeling baseline → Insight & Rekomendasi


## Raw Dataset Link
- Sumber: Kaggle — *Superstore Dataset* (contoh): https://www.kaggle.com/datasets/vivek468/superstore-dataset-final
- File yang dianalisis: `Superstore.csv`


## Insight & Findings
- Dataset berisi **9,994 baris** dan **21 kolom**. (encoding: latin1)
- Cakupan tanggal: Order Date: 2011-01-02 → 2014-12-31 | Ship Date: 2011-01-02 → 2015-06-01
- ~80% penjualan disumbang oleh **8** sub-kategori utama (contoh): Phones, Chairs, Storage, Tables, Binders, Machines, Accessories, Copiers
- Ambang diskon (median profit < 0) per sub-kategori (contoh): Bookcases: ≥20%; Storage: ≥20%; Chairs: ≥30%; Tables: ≥30%; Machines: ≥40%
- Jumlah baris **rugi**: **1,871**.
- Hotspot rugi (teratas): Central × Office Supplies × Binders (rugi: 233) | East × Office Supplies × Binders (rugi: 171) | Central × Furniture × Furnishings (rugi: 138) | South × Office Supplies × Binders (rugi: 132) | East × Technology × Phones (rugi: 97)


## AI Support Explanation
- **Perancangan pipeline analisis** (EDA Pareto, diskon vs profit, time series) dibantu dengan LLM (GPT) untuk mempercepat penulisan kode yang tetap dapat dipahami pemula.
- **Penyusunan baseline model** klasifikasi (Logistic Regression) dan contoh evaluasi (F1, ROC-AUC) disiapkan oleh LLM sebagai **baseline** yang mudah direplikasi.
- **Perumusan insight & rekomendasi** disusun dengan bantuan LLM, kemudian diverifikasi secara manual dari hasil output notebook.
- Catatan: LLM tidak menggantikan interpretasi kritis; keputusan akhir tetap berdasarkan observasi dan konteks bisnis.
