# Submission 1: Nama Proyek Anda

Nama: Rizki Alandani

Username dicoding: rizki_alandani_D3S9

|                         | Deskripsi                                                                                                                                                           |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Dataset                 | [Heart Failure](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)                                                                               |
| Masalah                 | Gagal jantung mempengaruhi jutaan orang di seluruh dunia dan merupakan penyebab utama kematian. Ada beberapa faktor yang dapat meningkatkan kemungkinan seseorang mengalami gagal jantung, termasuk usia, tekanan darah, kolesterol, dan lainnya. Oleh karenanya perlu adanya diognosis secara dini bagi pasien untuk dapat mencegah terjadinya gagal jantung melalu data-data rekam medis yang ada.                                                                                                                                  |
| Solusi machine learning |  Membangun model prediksi yang dapat mengidentifikasi pasien yang berisiko tinggi mengalami gagal jantung berdasarkan faktor-faktor tersebut. Tujuan akhirnya adalah untuk membantu praktisi medis dalam melakukan diagnosis dini dan pengelolaan risiko bagi pasien yang rentan terhadap kondisi serius ini.                                                                                                                  |
| Metode pengolahan       | Pengolahan data dilakukan oleh Tensorflow pipeline, yang mana pada prosesnya meliputi ExampleGen, SchemaGen, StatisticsGen, dan ExampleValidator. Kemudian dilanjukan oleh proses Transform, Trainer, Evaluator, dan Pusher.                                                                                        |
| Arsitektur model        | Model ini terdiri dari beberapa layer yaitu: input layer yang tersusun oleh semua features, concatenate layer yang menjadi masukan seluruh input features, 3 dense layer diantaranya 256 64 dan 16 tensor, dan terakhir output layer biner.                                                                                                                         |
| Metrik evaluasi         | Beberapa metrik yang digunakan untuk mengevaluasi model klasifikasi pada projek ini adalah AUC, Precision, Recall, ExampleCount, dan BinaryAccuracy.                                                                                                    |
| Performa model          | Performa model yang dihasilkan adalah AUC 0.90958, BinaryAccuracy 0.82381, Precision 0.89524, dan Recall 0.78333                                                                                                                                  |
| Opsi deployment         | Deployment dilakukan dengan menggunakan Tensorflow Serving yang di host di Railway. Termasuk monitoring metrics menggunakan Prometheus.                                                                                                                                   |
| Web app                 | [Heart Detection](https://mlops-tfx-production-1022.up.railway.app/v1/models/cc-model/metadata) |
| Monitoring              | Hasil monitoring model serving menunjukan status up yang artinya model dapat diakses. Selain itu beberapa metrics juga dapat ditampilkan seperti jumlah request yang ada (:tensorflow:serving:request_count) yang menunjukkan request sukses atau error.                                                                                                                |
