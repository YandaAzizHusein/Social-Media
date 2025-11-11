# AI Content Insight Generator

EngageSense adalah alat analisis performa konten berbasis AI yang membantu agensi sosial media dan kreator memahami kinerja postingan mereka dengan cepat dan efisien.  
Dengan menggabungkan analisis data (pandas) dan Google Gemini API, alat ini menghasilkan laporan otomatis berisi KPI utama, insight AI, serta rekomendasi strategis untuk peningkatan performa konten berikutnya.

---

## Fitur Utama

- Analisis performa otomatis dari file CSV hasil export TikTok Analytics.
- Menghitung metrik utama seperti views, engagement rate, dan top performing content.
- Menggunakan Gemini 2.0 Flash untuk menghasilkan insight dan rekomendasi jadwal upload.
- Laporan otomatis dalam format teks yang siap dibaca oleh klien atau tim internal.

---

## Tech Stack

| Komponen | Deskripsi |
|-----------|------------|
| Python | Bahasa utama |
| Pandas | Analisis data dan KPI |
| Google Gemini API | Insight dan rekomendasi berbasis AI |
| ReportLab (opsional) | Ekspor laporan ke PDF |
| Jupyter / Terminal | Menjalankan script secara lokal |

---

## Struktur Folder

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

## Cara Menjalankan

1. Clone atau download project:
   ```bash
   git clone https://github.com/<username>/EngageSense.git
   cd EngageSense
   ````

2. Install dependensi:

   ```bash
   pip install pandas google-generativeai reportlab
   ```

3. Tambahkan API Key:

   * Dapatkan API key di [Google AI Studio](https://aistudio.google.com)
   * Ganti baris berikut di kode:

     ```python
     API_KEY = "YOUR_GEMINI_API_KEY"
     ```

4. Jalankan program:

   ```bash
   python main.py
   ```

5. Hasil laporan akan muncul di terminal dan disimpan otomatis ke:

   ```
   weekly_report.txt
   ```

---

## Contoh Output

```
TIKTOK PERFORMANCE REPORT
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

## Kontak

**Yanda Aziz Husein**
- AI Engineer & Data Scientist
- Medan, Indonesia
- Email: [yandaazizhusein1122@gmail.com](mailto:yandaazizhusein1122@gmail.com)
- LinkedIn: [linkedin.com/in/yanda-aziz-husein](https://linkedin.com/in/yanda-aziz-husein)
- GitHub: [github.com/YandaAzizHusein](https://github.com/YandaAzizHusein)
