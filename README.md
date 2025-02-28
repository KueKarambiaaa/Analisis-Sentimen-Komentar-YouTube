# Analisis-Sentimen-Komentar-YouTube

## Deskripsi Proyek
Proyek ini bertujuan untuk melakukan analisis sentimen pada komentar YouTube menggunakan berbagai metode Machine Learning dan Deep Learning. Data yang digunakan diperoleh melalui proses web scraping menggunakan YouTube API, kemudian diproses untuk ekstraksi fitur dan pelabelan data. Model yang digunakan mencakup algoritma seperti Naïve Bayes, SVM, Random Forest, serta pendekatan berbasis deep learning dengan LSTM.

## Dataset
Dataset yang digunakan dalam proyek ini diperoleh dari komentar YouTube, yang dikumpulkan menggunakan YouTube API. Setelah scraping, dataset melewati proses pembersihan dan pelabelan sebelum digunakan untuk pelatihan model.

**Tahapan Pengolahan Data:**
1. Pengumpulan data menggunakan **YouTube API**.
2. **Preprocessing** teks: pembersihan teks, stemming, dan normalisasi.
3. **Ekstraksi fitur** menggunakan TF-IDF dan Word Embeddings.
4. **Pelabelan sentimen** secara manual atau berbasis model pre-trained.

## Model yang Digunakan
Beberapa model telah diuji dalam proyek ini, antara lain:

### 1. **Naïve Bayes**
- Akurasi: 91.75%
- Cocok untuk dataset dengan distribusi teks sederhana.

### 2. **Support Vector Machine (SVM)**
- Akurasi: 98.29%
- Performa sangat baik dalam klasifikasi teks.

### 3. **Random Forest**
- Akurasi: 98.79%
- Model yang andal dan memberikan interpretabilitas tinggi.

### 4. **Long Short-Term Memory (LSTM)**
- Akurasi: 98.50%
- Model berbasis deep learning yang mampu menangkap konteks lebih dalam dalam teks.

## Evaluasi dan Visualisasi
- **Akurasi dan F1-score** dibandingkan antar model untuk menentukan performa terbaik.
- **Confusion Matrix** untuk melihat distribusi kesalahan prediksi.
- **Grafik Loss dan Accuracy** untuk model deep learning guna memahami konvergensi model.

## Instalasi dan Penggunaan
1. Clone repository ini:
   ```sh
   git clone https://github.com/username/repository.git
   ```
2. Install dependensi yang diperlukan:
   ```sh
   pip install -r requirements.txt
   ```
3. Jalankan skrip utama:
   ```sh
   python main.py
   ```

## Kesimpulan
- Model **Random Forest** dan **SVM** memberikan performa terbaik dalam klasifikasi sentimen.
- LSTM juga memberikan hasil yang kompetitif, tetapi memerlukan lebih banyak sumber daya komputasi.
- Proyek ini dapat diperluas dengan menggunakan lebih banyak data atau fine-tuning model berbasis Transformer (seperti BERT).
