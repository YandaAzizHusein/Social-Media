# 🎯 EngageSense – AI Content Insight Generator

EngageSense adalah alat analisis performa konten berbasis **AI** yang membantu agensi sosial media dan kreator konten memahami kinerja postingan mereka secara cepat dan efisien.  
Dengan menggabungkan **analisis data** (pandas) dan **Google Gemini API**, tool ini menghasilkan **laporan otomatis** berisi KPI utama, insight AI, serta rekomendasi strategis untuk peningkatan performa konten berikutnya.

---

## 🚀 Fitur Utama

- **📊 Analisis Performa Otomatis**
  - Menghitung KPI penting seperti *views, engagement rate,* dan *top performing content* dari file CSV TikTok Export.

- **🧠 Insight AI**
  - Menggunakan **Gemini 2.0 Flash** untuk membuat ringkasan performa mingguan, alasan keberhasilan konten, serta ide dan rekomendasi jadwal posting berikutnya.

- **📄 Laporan Otomatis**
  - Menghasilkan laporan teks siap dibaca klien/agency (dapat dikonversi ke PDF/Notion).

- **⚡ Plug-and-Play**
  - Cukup upload file `Content.csv` hasil export TikTok Analytics, jalankan script, dan laporan otomatis muncul.

---

## 🧰 Tech Stack

| Komponen | Deskripsi |
|-----------|------------|
| **Python** | Bahasa utama |
| **Pandas** | Analisis data & KPI |
| **Google Gemini API** | Insight dan rekomendasi berbasis AI |
| **ReportLab (optional)** | Ekspor laporan ke PDF |
| **Jupyter / Terminal** | Menjalankan script secara lokal |

---

## 📂 Struktur Folder

```

EngageSense/
│
├── Content.csv                # Data TikTok hasil export
├── main.py                    # Script utama (AI Insight Generator)
├── requirements.txt           # Dependensi Python
├── weekly_report.txt          # Laporan insight AI hasil generate
└── README.md                  # Dokumentasi project

````

---

## ⚙️ Cara Menjalankan

1. **Clone / Download project**
   ```bash
   git clone https://github.com/<username>/EngageSense.git
   cd EngageSense
    ````

2. **Install dependensi**

   ```bash
   pip install pandas google-generativeai reportlab
   ```

3. **Tambahkan API Key**

   * Dapatkan API key di [Google AI Studio](https://aistudio.google.com)
   * Ganti di baris berikut:

     ```python
     API_KEY = "YOUR_GEMINI_API_KEY"
     ```

4. **Jalankan program**

   ```bash
   python main.py
   ```

5. **Hasil laporan**

   * Akan muncul di terminal dan disimpan otomatis dalam file:

     ```
     weekly_report.txt
     ```

---

## 🧩 Contoh Output

```
TIKTOK WEEKLY PERFORMANCE REPORT
========================================
Total Video       : 15
Total Views       : 13,820
Avg Engagement Rt : 6.82%

Top 3 by Engagement Rate:
- #run #gymtok (ER 8.21%, Views 3,200)
- #boxing #hybridathlete (ER 7.54%, Views 2,980)
- #timnas (ER 6.43%, Views 2,600)

=== INSIGHT & RECOMMENDATION (AI) ===
1. Konten bertema sport dan hybrid athlete menunjukkan performa tertinggi.
2. Faktor utama keberhasilan adalah hook visual dan caption aktif.
3. Rekomendasi minggu depan: eksperimen video pendek 10–12 detik, gunakan hashtag tren (#physicalasia, #fypシ゚), dan upload di jam 19.00–21.00.
```

---

## 📧 Kontak

**Yanda Aziz Husein**
- AI Engineer & Data Scientist
- 📍 Medan, Indonesia
- 📩 [yandaazizhusein1122@gmail.com](mailto:yandaazizhusein1122@gmail.com)
- 🔗 [LinkedIn](https://linkedin.com/in/yanda-aziz-husein) | [GitHub](https://github.com/YandaAzizHusein)

