# IDX_FinalTask_Rakamin
Final Task ini bertujuan untuk menganalisis risiko gagal bayar pinjaman menggunakan analisis deskriptif dan model Logistic Regression sebagai model dasar (baseline).

*Tujuan:*
- Melakukan analisis deskriptif terhadap data pinjaman
- Mengidentifikasi faktor-faktor yang berkaitan dengan risiko gagal bayar
- Membangun model Logistic Regression sebagai model prediksi dasar
- Mengevaluasi performa model pada data yang tidak seimbang

*Gambaran Dataset*
Jumlah data: ±46.000 data pinjaman
Variabel target: risk_flag
0 = Pinjaman lancar (Good Loan)
1 = Pinjaman bermasalah (Bad Loan)

*Fitur utama yang digunakan:*
- loan_amnt
- int_rate
- grade

Catatan: Dataset bersifat tidak seimbang, dengan proporsi pinjaman bermasalah sekitar 11%.

*Model & Evaluasi*
Model Logistic Regression digunakan karena bersifat sederhana dan mudah diinterpretasikan.
Untuk mengatasi ketidakseimbangan data, digunakan penyesuaian bobot kelas agar model lebih mampu mendeteksi pinjaman bermasalah.

*Hasil evaluasi model:*
Nilai ROC–AUC: 0.67
Model cukup mampu membedakan antara pinjaman berisiko dan tidak berisiko

*Insight Utama*
- Tingkat bunga yang lebih tinggi berkaitan dengan risiko gagal bayar yang lebih besar
- Pinjaman dengan tujuan usaha kecil memiliki risiko lebih tinggi
- Jumlah pinjaman dan rasio utang terhadap pendapatan (DTI) yang tinggi meningkatkan risiko kredit
- Penanganan data yang tidak seimbang sangat penting dalam pemodelan risiko kredit

*Keterbatasan*
- Model yang digunakan masih bersifat sederhana dan belum menangkap hubungan non-linear
- Belum dilakukan tuning hyperparameter
- Fokus utama pada interpretasi model, bukan pada performa prediksi maksimum

Proyek ini merupakan contoh analisis risiko kredit tingkat pemula yang menunjukkan bagaimana Logistic Regression dapat digunakan sebagai model dasar yang transparan dan mudah dipahami dalam memprediksi risiko gagal bayar.
