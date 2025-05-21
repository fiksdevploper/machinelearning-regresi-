# machinelearning-regresi

Proyek ini mengimplementasikan algoritma regresi linear untuk melakukan prediksi. Proyek ini dibangun menggunakan pustaka-pustaka Python populer seperti:

* **Pandas:** Untuk manipulasi dan analisis data.
* **Matplotlib:** Untuk visualisasi data dasar.
* **Seaborn:** Untuk visualisasi data statistik yang lebih menarik dan informatif.
* **Scikit-learn (sklearn):** Pustaka machine learning yang menyediakan implementasi algoritma regresi linear dan alat bantu lainnya seperti pembagian data training dan testing, serta metrik evaluasi.

## Deskripsi Proyek

> Proyek ini bertujuan untuk memprediksi daerang yang rawan terkena banjir bandang.

## Cara Penggunaan

1.  **Instalasi *dependencies***:
    Jika Anda menjalankan proyek ini di Google Colab, pustaka-pustaka yang diperlukan umumnya sudah terinstal. Namun, jika ada pustaka spesifik yang kurang, Anda dapat menginstalnya menggunakan pip di dalam *notebook*:
    ```python
    !pip install pandas matplotlib seaborn scikit-learn
    ```
    
2.  **Unduh atau siapkan dataset**:
    dataset yang saya gunakan tersebut bisa didapatkan di kaggle yang judul nya Regression with a Flood Prediction Dataset. untuk ukurang dataset sendiri kurang lebih 100mb.

    > Dataset yang digunakan adalah data`train` untuk melatih data machine learning dan data`test` untung menguji model machine learning. Anda dapat mengunggah file ini ke Google Colab melalui panel sebelah kiri (ikon folder) atau dengan meletakkannya di Google Drive Anda dan kemudian me-mount Drive di *notebook*.

3.  **Jalankan *notebook* Python di Google Colab**:
    Buka file Jupyter Notebook (`.ipynb`) yang berisi kode proyek ini di Google Colab. Anda dapat mengunggahnya atau membukanya langsung dari GitHub jika repository Anda bersifat publik. Setelah dibuka, Anda dapat menjalankan setiap sel kode secara berurutan untuk melakukan analisis data, melatih model, dan melihat hasilnya.

    
## Hasil Model

Berikut adalah hasil evaluasi dari beberapa algoritma yang diuji pada proyek prediksi banjir ini:

| Algoritma                   | MAE       | MSE       | R2        |
| :-------------------------- | :-------- | :-------- | :-------- |
| Lars                        | 0.806497  | 0.998246  | 0.000764  |
| GradientBoostingRegressor   | 0.512672  | 0.380491  | 0.619132  |
| Linear Regression           | 0.329142  | 0.171296  | 0.828534  |

**Interpretasi Hasil:**

* **Lars:** Algoritma Lars menunjukkan nilai Mean Absolute Error (MAE) yang cukup tinggi (0.806), Mean Squared Error (MSE) yang juga relatif tinggi (0.998), dan nilai R-squared yang sangat rendah (0.000764). Ini mengindikasikan bahwa algoritma Lars kurang baik dalam melakukan prediksi dan hanya mampu menjelaskan sebagian kecil varians dalam data.

* **GradientBoostingRegressor:** Algoritma ini menunjukkan performa yang jauh lebih baik dibandingkan Lars, dengan MAE sebesar 0.513 dan MSE sebesar 0.380. Nilai R-squared sebesar 0.619 menunjukkan bahwa algoritma ini mampu menjelaskan sekitar 61.9% varians dalam data target.

* **Linear Regression:** Algoritma Regresi Linear menunjukkan performa terbaik di antara ketiga algoritma ini. Dengan MAE terendah sebesar 0.329 dan MSE terendah sebesar 0.171, algoritma ini memiliki kemampuan prediksi yang lebih akurat. Selain itu, nilai R-squared yang tinggi sebesar 0.829 menunjukkan bahwa algoritma ini mampu menjelaskan sekitar 82.9% varians dalam data target dengan baik.

**Kesimpulan:**

Berdasarkan metrik evaluasi ini, algoritma **Linear Regression** menunjukkan performa terbaik untuk tugas prediksi banjir ini, diikuti oleh **GradientBoostingRegressor**. algoritma **Lars** menunjukkan performa yang paling buruk. Langkah selanjutnya mungkin melibatkan fine-tuning lebih lanjut pada algoritma Linear Regression atau Gradient Boosting Regressor untukPotensi peningkatan performa.

## Kontribusi

fiksdeveloper | dicoding academy

## Lisensi
[Attribution 4.0 International]

PERATURAN LISENSI:
Bagikan — salin dan sebarkan materi dalam bentuk atau format apa pun untuk tujuan apa pun, bahkan secara komersial. 
Ubah — remix, transformasi, dan kembangkan materi untuk tujuan apa pun, bahkan secara komersial. 
---

"terimakasih sunshine"
