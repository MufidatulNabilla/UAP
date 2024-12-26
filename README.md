# Analisis Sentimen Ulasan Pengunjung Universal Studio

## Deskripsi Proyek

Proyek ini bertujuan untuk melakukan analisis sentimen pada ulasan pengunjung Universal Studios. Dataset yang digunakan diambil dari [Kaggle](https://www.kaggle.com/datasets/dwiknrd/reviewuniversalstudio). Dengan memahami sentimen yang terkandung dalam ulasan, proyek ini diharapkan dapat memberikan wawasan yang lebih baik tentang pengalaman pengunjung serta membantu Universal Studios dalam meningkatkan layanan dan atraksi mereka.

Model deep learning, seperti LSTM dan BERT, akan digunakan untuk menganalisis data ulasan. Pendekatan ini memungkinkan untuk menangkap pola dan konteks dalam data teks dengan lebih efektif.

---

## Dataset Overview

Dataset ini berisi ulasan pengunjung Universal Studios yang telah diambil dari Kaggle. Informasi yang disediakan dalam dataset ini mencakup:

- **sentiments**: Label sentimen untuk setiap ulasan, yang menggambarkan apakah ulasan tersebut positif atau negatif.
- **cleaned_review**: Ulasan yang telah melalui proses pembersihan seperti penghapusan karakter khusus, angka, dan simbol.
- **cleaned_review_length**: Panjang dari ulasan yang telah dibersihkan dalam bentuk jumlah kata.
- **review_score**: Skor yang diberikan oleh pengunjung, biasanya dalam rentang 1 hingga 5.

---

## Struktur Dataset

Dataset terdiri dari beberapa kolom utama:

| Kolom                 | Deskripsi                                                                 |
|-----------------------|---------------------------------------------------------------------------|
| **sentiments**        | Label sentimen (positif atau negatif)                                     |
| **cleaned_review**    | Teks ulasan yang telah dibersihkan                                       |
| **cleaned_review_length** | Panjang teks ulasan dalam jumlah kata                                  |
| **review_score**      | Skor yang diberikan oleh pengunjung                                      |

---

## Langkah-Langkah Proses

1. **Eksplorasi Data**: 
   - Memeriksa distribusi sentimen (positif vs negatif).
   - Melakukan visualisasi distribusi panjang ulasan dan skor ulasan.

2. **Pra-pemrosesan Data**:
   - Penghapusan stopword, stemming, dan tokenisasi pada teks ulasan.
   - Konversi teks menjadi representasi numerik menggunakan teknik seperti TF-IDF atau word embeddings.

3. **Pengembangan Model**:
   - Implementasi model LSTM untuk menangkap dependensi temporal dalam teks.
   - Transfer learning dengan BERT untuk memahami konteks ulasan secara lebih mendalam.

4. **Evaluasi**:
   - Menggunakan metrik seperti akurasi, F1-score, precision, dan recall untuk menilai performa model.

5. **Kesimpulan dan Rekomendasi**:
   - Menyusun wawasan berdasarkan hasil analisis sentimen.
   - Memberikan rekomendasi berdasarkan pola yang ditemukan.

---

## Tujuan Akhir

Proyek ini akan menghasilkan model prediksi sentimen yang akurat dan dapat diandalkan. Selain itu, hasil analisis akan disusun menjadi laporan untuk memberikan masukan kepada pihak Universal Studios terkait dengan pengalaman pengunjung berdasarkan data ulasan.

---

## Penulis

- **Nama**: Mufidatul Nabilla
- **NIM**: 202110370311227
- **Institusi**: Universitas Anda

---

## Cara Menggunakan

1. Clone repositori ini:
   ```bash
   git clone https://github.com/username/universal-studio-sentiment.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Jalankan skrip utama untuk melatih model:
   ```bash
   python train_model.py
   ```
4. Evaluasi model dapat dilakukan dengan menjalankan:
   ```bash
   python evaluate_model.py
   ```

