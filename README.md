# Nutrifact Machine Learning

## Daftar Isi

1. [Team C242-PS378](#C242-PS378---ml)
2. [Pendahuluan](#Pendahuluan)
3. [Nutrition Grade Model Documentation](#NutritionGradeModelDocumentation)
4. [Fitur Utama](#FiturUtama)

## C242-PS378 - ml

| Bangkit ID    | Nama                     | Learning Path       | Universitas                      |
|---------------|--------------------------|---------------------|----------------------------------|
| M117B4KY3021  |  M. Rama Reyswara        | Machine Learning    | Institut Teknologi Nasional Bandung |
| M117B4KY4584  | Yuval Adilah             | Machine Learning    | Institut Teknologi Nasional Bandung |
| M125B4KY3691  |  Rangga Rizky Radityo    | Machine Learning    |  Politeknik Manufaktur Bandung      |

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

```
Cara Penggunaan
- Buka Google Colab.
- Unggah file
```
Tesseract&Grading.ipynb

```
### 1. Persiapkan Input 
Gambar untuk OCR:
```

Siapkan gambar dalam format `.png`, `.jpg`, atau `.jpeg`. Notebook akan membaca gambar tersebut dan mengekstrak teks menggunakan pytesseract.

```
 Dataset untuk Grading:
```
Jika grading dilakukan menggunakan dataset, siapkan file dataset dalam format `.csv`
```
 ### 2. Jalankan Notebook
Import dan Instalasi:
```
Jalankan sel pertama untuk mengimpor library dan menginstal dependensi.
```
Preprocessing:
```
Jalankan preprocessing gambar, seperti mengubah gambar ke skala abu-abu, binarisasi, atau penajaman gambar, untuk meningkatkan hasil OCR.
```
Model Training:
```
Jika menggunakan grading berbasis data, jalankan sel untuk melatih model pembelajaran mesin.
```
Evaluasi dan Visualisasi:
```
Evaluasi model dengan data uji. Notebook akan menampilkan hasil evaluasi dalam bentuk metrik dan grafik performa.
```
Hasil Akhir:
```
Notebook akan menghasilkan teks dari gambar atau hasil grading berdasarkan dataset.
```
### 4. Menyimpan Model dan Hasil
```
Model pembelajaran mesin yang telah dilatih dapat disimpan menggunakan format `.h5`
```
### 5. konversi model h5 ke json 
```
setelah model tersimpan pada format `.h5` lakukan konversi ke format json untuk dapat digunakan untuk aplikasi berbasis web atau integrasi lebih lanjus
