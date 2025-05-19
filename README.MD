# Klasifikasi Mata Uang Rupiah Indonesia

Pada projek kali ini kita diarahkan membuat projek klasifikasi gambar, saya memilih untuk membuat projek klasifikasi mata uang rupiah yang saya harap nantinya model ini diharapkan dapat membantu dalam pembuatan aplikasi edukatif atau kasir otomatis yang mampu mengenali nominal uang rupiah dari citra uang kertas.


## Dataset
sumber dataset: https://www.kaggle.com/datasets/anidwiastuti/rupiah-banknotes-dataset/data
Dataset terdiri dari gambar uang kertas Indonesia dengan total 2.409 gambar dalam 7 kelas:
- Rp1.000 (334 gambar)
- Rp2.000 (344 gambar)
- Rp5.000 (345 gambar)
- Rp10.000 (344 gambar)
- Rp20.000 (344 gambar)
- Rp50.000 (354 gambar)
- Rp100.000 (344 gambar)

## Arsitektur Model
Model dibangun menggunakan CNN (`Sequential`) dengan beberapa `Conv2D`, `MaxPooling`, dan `Dropout`, dilatih menggunakan `Adam` optimizer.


## Goals
- Menghasilkan model klasifikasi yang mampu mengenali uang kertas Indonesia (Rp1.000, Rp2.000, Rp5.000, dst) dari gambar.
- Mengekspor model ke dalam 3 format: TensorFlow SavedModel, TFLite, dan TensorFlow.js.
