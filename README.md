# Capstone Project - IMDB Sentiment Analysis with LLM (IBM Granite via Replicate)

# Deskripsi Proyek
- Proyek ini adalah bagian dari Capstone Project SDI Data Wave 10 (Batch 26).
- Dataset yang digunakan adalah IMDB Movie Reviews (50.000 review) dengan label positive dan negative.

# Tujuan utama proyek ini adalah:
1. Mengeksplorasi dataset menggunakan LLM (IBM Granite Models).
2. Menggunakan LLM untuk klasifikasi sentimen review film.
3. Melakukan evaluasi sederhana terhadap performa klasifikasi.
4. Menyusun insight bisnis yang relevan dari hasil analisis.

# Dataset
- Sumber: Kaggle - IMDB Movie Reviews https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews/code
- Jumlah data: 50.000 review
- Format: CSV, dengan kolom:
  - review → teks ulasan film.
  - sentiment → label (positive / negative).

# Tools & Teknologi
1. Python (Google Colab) untuk data handling & eksperimen.
2. Library Pandas, Matplotlib untuk analisis data & visualisasi.
3. IBM Granite LLM (via Replicate API) untuk klasifikasi sentimen & eksplorasi insight.
4. Kaggle, sebagai Dataset Sumber

# Contoh Langkah Analisis
1. Load & Explorasi Data
2. Cek jumlah data, distribusi label, panjang review.
3. Visualisasi distribusi sentimen.
4. Insight dengan LLM
5. Mengajukan beberapa pertanyaan ke model Granite:
6. Pentingnya data balance.
7. Tantangan NLP (misalnya sarkasme, opini campuran).
8. Alasan split train/test.
9. Insight bisnis untuk industri film/streaming.
10. Klasifikasi Sentimen
11. Sampling 50 review dari dataset.
12. Mengirim review ke LLM → prediksi positive / negative.
13. Menyimpan hasil prediksi & bandingkan dengan label asli.
14. Evaluasi
15. Hitung akurasi sederhana.
16. Buat confusion matrix.
17. Summary
18. Ringkasan hasil analisis & insight bisnis.

# Hasil
1. Dataset berisi 50.000 review, Distribusi sentimen: ~50% positif, ~50% negatif.
2. LLM Granite berhasil memberikan insight yang baik terkait dataset dan tantangan NLP.
3. Pada sample 50 review:
   - Akurasi model: ~90% (hasil bisa berbeda tiap eksekusi).
   - Confusion matrix menunjukkan prediksi cukup baik, tapi ada beberapa error pada review ambigu.
   - Insight bisnis: analisis sentimen review dapat membantu perusahaan streaming meningkatkan rekomendasi, kualitas konten, dan kepuasan pelanggan.

# Cara Menjalankan:
1. Clone repo:
   git clone https://github.com/achmaulanaa/imdb-llm-capstone.git
   cd imdb-llm-capstone
2. Upload dataset IMDB Dataset.csv ke Google Drive.
3. Buka notebook di Google Colab.
4. Pastikan sudah setup API Key Replicate.
5. Jalankan notebook secara berurutan.

# Kesimpulan
- LLM dapat digunakan tidak hanya untuk classification, tetapi juga untuk memberikan penjelasan & insight data.
- IMDB dataset cocok untuk proyek klasifikasi teks & NLP dasar.
- Proyek ini menunjukkan integrasi LLM + dataset publik + evaluasi sederhana → bisa menjadi dasar untuk proyek lanjutan dengan dataset yang lebih kompleks.
