# Prediksi Produktivitas Pekerja pada Industri Garmen Menggunakan Neural Network Regressor
Model regresi berbasis neural network untuk memprediksi produktivitas pekerja garmen berdasarkan variabel operasional seperti target produksi, jumlah pekerja, dan jam lembur.

## Latar Belakang
Pabrik garmen mencatat produktivitas secara manual di tiap tim dan shift. Proyek ini membangun model regresi yang memperkirakan produktivitas aktual dari input operasional. Model ini membantu manajer mengidentifikasi tim dengan performa rendah lebih awal.
Dataset
Dataset yang digunakan adalah Productivity Prediction of Garment Employees dari UCI Machine Learning Repository. Dataset ini berisi data produktivitas pekerja garmen di Bangladesh, dengan fitur berikut:
<ul>
  <li>date</li>
  <li>quarter</li>
  <li>department</li>
  <li>day</li>
  <li>team</li>
  <li>targeted_productivity</li>
  <li>smv</li>
  <li>wip</li>
  <li>over_time</li>
  <li>incentive</li>
</ul>

## Metode
Tahap pertama adalah preprocessing data. Nilai yang hilang ditangani, fitur kategorikal di-encode, dan fitur numerik dinormalisasi.
Tahap kedua adalah membangun arsitektur model. Model menggunakan neural network feedforward dengan beberapa hidden layer dan fungsi aktivasi ReLU.
Tahap ketiga adalah pelatihan model. Dataset dibagi menjadi data latih dan data uji. Model dilatih hanya pada data latih.
Tahap terakhir adalah evaluasi. Performa model diukur pada data uji menggunakan Mean Absolute Error (MAE) dan Root Mean Squared Error (RMSE).

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / PyTorch
- Matplotlib / Seaborn

## Evaluasi
| Metric | Value |
|--------|-------|
| MAE    | 0.0933 |
| RMSE   | 0.1294 |
| R2     | 0.3695 |
