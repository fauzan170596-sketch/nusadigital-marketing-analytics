# 📊 NusaDigital Media: Social Media Content & Campaign Performance Analytics (2025)

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

## 👨‍💻 About Me
* **Name:** Fauzan Falah Rabbani
* **Background:** S1 Hukum Universitas Pancasila (2014–2018) | Mantan Legal & Compliance Staff (4+ tahun) yang kini bertransisi menjadi **Data Analyst**.
* **Core Skills:** Python, Pandas, SQL, Power BI, Exploratory Data Analysis (EDA).

## 📌 Executive Summary
Proyek ini menganalisis performa kampanye media sosial **NusaDigital Media** sepanjang tahun 2025 (1.000 record data dari 5 platform utama: Instagram, Facebook, TikTok, X/Twitter, dan YouTube). Analisis berfokus pada evaluasi efisiensi alokasi sumber daya, mengurai volatilitas produksi bulanan, dan memberikan rekomendasi berbasis data untuk optimasi saluran pemasaran.

---

## 🎯 Core Business Problems & Objectives
1. **Resource & Effort Mismatch:** Tingginya alokasi biaya & waktu produksi pada format video (Reels/Video) belum sebanding dengan perolehan *Engagement Rate* yang justru didominasi oleh konten visual statis (Infographic/Image).
2. **False Signal Hazard:** Risiko evaluasi parsial berbasis total *Reach* absolut (seperti pada TikTok) tanpa melihat rasio efisiensi per postingan.
3. **Operational Inconsistency:** Fluktuasi volume publikasi bulanan yang tajam (seperti *drop* di April & November) akibat ketiadaan standardisasi *content buffer*.

---

## 📈 Macro Performance Baseline (H1 vs H2 2025)
- **Total Reach:** 409 Juta (*H1: 198 Jt vs H2: 211 Jt* | 🟢 **+6,5%**)
- **Total Engagement:** 37 Juta (*H1: 18,1 Jt vs H2: 18,9 Jt* | 🟢 **+4,4%**)
- **Total Clicks:** 823 Ribu (*H1: 402 Rb vs H2: 421 Rb* | 🟢 **+4,7%**)
- **Avg. Engagement Rate:** 8,01% (*H1: 8,02% vs H2: 8,00%* | ⚪ **Stabil ~8,00%**)

---

## 🛠️ Data Pipeline & Cleaning Process
Proses pengolahan data mentah (`1.002 records`) dilakukan menggunakan **Python (Pandas)**:
- **Missing Value Handling:** Imputasi median pada kolom `Reach` dan `Comments` (masing-masing 2 nilai kosong).
- **Deduplication:** Menghapus 2 baris data duplikat (`drop_duplicates()`).
- **Feature Engineering:** Konversi string tanggal ke format `datetime` dan ekstraksi variabel `Month` & `Month_Number`.
- **Hasil Akhir:** Dataset bersih berukuran **1.000 records & 20 variabel** siap pakai untuk EDA dan Dashboarding.

---

## 💡 Key Strategic Recommendations
1. **Atur Minimum Quota Buffer (SOP):** Tetapkan ambang batas publikasi minimal **80 post/bulan** untuk mencegah *drop* operasional.
2. **Prioritaskan High-ROI Format:** Pertahankan dan skalakan alokasi format **Infographic (19%) & Image (18,08%)** yang memimpin total keterlibatan audiens.
3. **Diferensiasi Peran Platform:**
   - **Instagram & X (Twitter):** Difokuskan sebagai *Conversion Driver* utama (konten beriklan & CTA penarik klik).
   - **TikTok:** Difokuskan sebagai *Growth Headroom* untuk jangkauan organik melalui strategi *cross-posting* konten pendek.

---

## 📄 Project Presentation
- 📑 [Unduh / Lihat Presentation Deck (PPTX)](Final_Project_Marketing_Channel_Analysis%20-%20Fauzan%20Falah%20Rabbani.pptx)
- 📑 [Unduh / Lihat Power BI, Google Collab, dan Excel](https://drive.google.com/drive/folders/1L2NsKAZH7NIPJDr9xP4wQU0qox-IvwDI?hl=ID)

## 🚀 Repository Structure
```text
├── data/
│   ├── raw/                  # Raw dataset (Excel/CSV)
│   └── processed/            # Cleaned dataset (Clean CSV)
├── notebooks/
│   └── data_cleaning_eda.ipynb # Python script for Data Cleaning & EDA
├── dashboard/
│   └── NusaDigital_Analytics.pbix # Interactive Power BI Dashboard
├── presentation/
│   └── Final_Project_Deck.pdf # Professional Business Presentation
└── README.md
