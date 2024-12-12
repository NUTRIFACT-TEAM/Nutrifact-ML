# Nutrifact Machine Learning

## Pendahuluan
Notebook ini dirancang untuk:
1. Membaca teks dari gambar menggunakan **Tesseract OCR**.
2. Melakukan preprocessing gambar dan teks untuk analisis lebih lanjut.
3. Menggunakan model pembelajaran mesin untuk sistem grading berdasarkan data yang diproses.

## Nutrition Grade Model Documentation
Dokumentasi ini menjelaskan cara menggunakan model penilaian nutrisi yang diterapkan dalam buku catatan Colab yang disediakan. Model ini menganalisis informasi nutrisi dari gambar tabel nutrisi produk makanan dan menetapkan nilai berdasarkan kandungan gula dan lemak.

## Fitur Utama
1. **OCR (Optical Character Recognition)**
    - Mengekstrak informasi nutrisi dari gambar produk makanan.
    - Mengenali nilai gula, lemak, dan ukuran takaran saji.
    
2. **Nutrition Grading**
    - Memberikan penilaian produk pada skala **A-D** berdasarkan:
        - Kandungan gula per 100g
        - Kandungan lemak per 100g
    - Menormalkan nilai ke standar ukuran saji 100g.

## Rlibrary yang Digunakan
- **OpenCV (cv2)**: Untuk tugas pengolahan gambar
- **pytesseract**: Untuk OCR (Optical Character Recognition) untuk mengekstrak teks dari gambar
- **pandas**: Untuk manipulasi dan analisis data
- **numpy**: Untuk operasi numerik
- **tensorflow**: Untuk membangun dan melatih model pembelajaran mesin
- **scikit-learn**: Untuk preprocessing, evaluasi model, dan pembagian data
- **matplotlib**: Untuk visualisasi data

## Persyaratan Software
- **Python**: Versi 3.10 atau lebih tinggi.
- **Google Colab** *(direkomendasikan untuk menjalankan notebook tanpa setup tambahan)*.

## Instalasi Library
Untuk menginstal library yang diperlukan, jalankan perintah berikut di terminal atau notebook:
```bash
pip install pytesseract opencv-python-headless numpy tensorflow pandas matplotlib scikit-learn joblib
