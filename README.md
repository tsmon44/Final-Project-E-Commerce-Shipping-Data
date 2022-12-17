# Final-Project-E-Commerce-Shipping-Data
## Product Shipment Delivered on time or not? To Meet E-Commerce Customer Demand

Perusahaan e-niaga internasional yang berbasis ingin menemukan wawasan utama dari basis data pelanggan mereka. Mereka ingin menggunakan beberapa teknik pembelajaran mesin tercanggih untuk mempelajari pelanggan mereka. Perusahaan menjual produk elektronik.

Dataset yang digunakan untuk pembuatan model berisi 10999 pengamatan dari 12 variabel.

## Sumber Dataset
Sumber : https://www.kaggle.com/datasets/prachi13/customer-analytics?datasetId=1176727

## Tujuan Project
- Memprediksi tingkat pengiriman produk disampaikan tepat waktu atau tidak
- Menentukan penyebab keterlambatan produk
- Membuat rekomendasi untuk meminimalisir keterlambatan pengiriman produk

## Model Machine Learning
Pemodelan yang akan digunakan bertujuan untuk memprediksi pengiriman produk disampaikan tepat waktu atau tidak tepat waktu. Target Variabel yang akan digunakan adalah Reached.on.Time_Y.N. Untuk mengurangi kesalahan prediksi (False Positive) dan (False Negative), maka pilih nilai Recall yang tinggi atau presisi yang tinggi. Classification Task :

- False Positive: Diprediksi pengiriman produk disampaikan tepat waktu, ternyata tidak tepat waktu

- False Negative: Diprediksi pengiriman produk disampaikan tidak tepat waktu, ternyata tepat waktu

Model Machine Learning yang akan diuji antara lain:

- Logical Regression
- K-NN
- Decision Tree Classification
- Random Forest Classification

## Conclusion
Dari observasi yang dilakukan, maka dapat disimpulkan bahwa model terbaik untuk memprediksi pengiriman produk disampaikan tepat waktu atau tidak adalah Model Hyperparameter Tuning using Optuna (Random Forest Undersampling), karena memiliki nilai Recall terbaik yaitu 97% serta nilai F1-score yaitu 72%. Walaupun nilai Precission jelek, tapi masih bisa dipertanggungjawabkan karena nilai Recallnya bagus.

## Recommendation
- Perbanyak pengiriman melalui layanan Flight (Penerbangan) dan Road (Jalan) untuk mengurangi keterlambatan pengiriman
- Buat gudang blok F agar cepat dalam melakukan pengiriman, sehingga dapat mengurangi keterlambatan pengiriman atau pindahkan beberapa barang ke gudang blok lainnya.
- Tingkatkan pengiriman agar tepat waktu sehingga rating 1-3 bisa naik menjadi 4-5. Karena, diberikan diskon lebih dari 10% pun tidak akan menaikkan rating. Walaupun, sudah ada rating 4-5. Tetapi, akan lebih baik jika semua ratingnya 4-5.
