# Tugas 2: Scraping Keyword Twitter

## Latar Belakang Pemilihan Keyword
Pada tugas ini, saya memilih keyword **"korupsi"** untuk dikumpulkan dari Twitter (X). Ada beberapa pertimbangan mengapa kata kunci ini dipilih:

1. **Isu Publik yang Relevan**  
   Korupsi merupakan salah satu isu besar di Indonesia yang banyak dibicarakan di ruang publik. Dengan menggunakan keyword ini, data yang terkumpul dapat memberikan gambaran persepsi masyarakat terkait isu korupsi di media sosial.

2. **Variasi Diskusi**  
   Topik korupsi sering dikaitkan dengan berbagai sektor seperti politik, hukum, birokrasi, hingga kehidupan sehari-hari. Hal ini memungkinkan adanya variasi data yang lebih kaya untuk dianalisis.

3. **Frekuensi Tinggi**  
   Karena sering muncul di berita maupun trending topic, keyword ini relatif menghasilkan banyak tweet dalam waktu singkat, sehingga mempermudah pencapaian target minimal **1000 data**.

4. **Potensi Analisis Sosial**  
   Dengan data ini, kita bisa melakukan analisis sentimen, tren percakapan, serta jaringan diskusi terkait isu korupsi. Hal ini sangat bermanfaat untuk memahami opini publik.

---

## Alur Kode / Proses Scraping

1. **Persiapan Alat**  
   - **Tweet Harvest** digunakan sebagai tools utama, karena API resmi Twitter memiliki banyak keterbatasan (rate limit) sehingga sulit mengumpulkan data dalam jumlah besar.  
   - Hasil dari Tweet Harvest berupa file **CSV** yang berisi tweet sesuai keyword pencarian.

2. **Proses Pengambilan Data**  
   - Keyword: `"korupsi"`  
   - Jumlah data terkumpul: **±1500 tweet**  
   - Format penyimpanan: `.csv` dan kemudian diekspor ke `.xlsx` untuk mempermudah analisis lebih lanjut.

3. **Struktur Data yang Dikumpulkan**  
   Dari hasil scraping, setiap tweet mengandung metadata berikut:
   - **Tanggal/Waktu** publikasi
   - **Username** pemilik tweet
   - **Isi tweet**
   - **Jumlah likes**
   - **Jumlah retweets**
   - **Jumlah replies**

   Format ini memungkinkan analisis kuantitatif (misalnya menghitung engagement) maupun kualitatif (menganalisis isi teks tweet).

---

## Hasil dan Penyimpanan
- Jumlah total tweet yang berhasil dikumpulkan: **1500+**
- Disimpan dalam dua format:
  - `tweets_korupsi.csv`
  - `tweets_korupsi.xlsx`
- Data siap digunakan untuk analisis lebih lanjut, seperti:
  - Analisis frekuensi kata (word cloud, bigram, trigram).
  - Analisis sentimen (positif, negatif, netral).
  - Identifikasi akun yang paling aktif membicarakan korupsi.

---

## Kesimpulan
Scraping dengan keyword **"korupsi"** berhasil mengumpulkan lebih dari 1500 data tweet. Pemilihan keyword ini terbukti tepat karena menghasilkan data yang variatif, relevan, dan banyak dibicarakan masyarakat. Dengan data tersebut, berbagai analisis lanjutan dapat dilakukan untuk memahami bagaimana isu korupsi dipersepsikan di media sosial.
