# Laporan Proyek Machine Learning – Prediksi Risiko Penyakit Mental Pelajar

Laporan ini disusun mengikuti format *contoh laporan.md* fileciteturn1file0.

---

## Domain Proyek  
Proyek *Machine Learning* ini berfokus pada deteksi dini risiko penyakit mental pada pelajar, dengan memanfaatkan data demografis, akademik, dan gaya hidup untuk memodelkan kemungkinan depresi.

## Latar Belakang  
Kesehatan mental pelajar merupakan isu yang semakin krusial di era modern, di mana tekanan akademik, beban pekerjaan sampingan, dan perubahan sosial dapat memicu gangguan berupa depresi dan kecemasan. Deteksi dini risiko masalah kesehatan mental sangat penting untuk intervensi tepat waktu, mencegah gejala memburuk, dan meningkatkan kesejahteraan siswa.

---

## Business Understanding

### Problem Statements  
1. Fitur apa saja yang berkontribusi paling kuat terhadap prediksi depresi pada pelajar?  
2. Bagaimana cara membangun model klasifikasi untuk memprediksi status depresi (ya/tidak) pada pelajar?  
3. Model *machine learning* mana yang paling optimal berdasarkan metrik akurasi, precision, recall, dan F1-score?

### Goals  
1. Mengidentifikasi variabel terpenting yang memengaruhi risiko depresi pada pelajar.  
2. Membangun dan membandingkan beberapa model klasifikasi.  
3. Menentukan model terbaik untuk prediksi risiko depresi dengan metrik evaluasi tertinggi.

### Solution Statements  
1. **Eksplorasi dan pembersihan data**: mengonversi tipe data, mengatasi _missing values_, dan membuat fitur baru.  
2. **Feature engineering**: pembuatan metrik `Stress_Score` dan `Lifestyle_Balance` berdasarkan kombinasi beberapa atribut.  
3. **Modeling**: melatih tiga algoritma klasifikasi—Gaussian Naive Bayes, Decision Tree, dan Support Vector Machine—dengan pembagian data train/test 80/20.  
4. **Evaluasi**: membandingkan hasil menggunakan akurasi, precision, recall, dan F1-score untuk memilih model terbaik.

---

## Data Understanding  
Dataset yang digunakan adalah *Student Depression Dataset* dari Kaggle, berisi **27.901 baris** dengan **18 kolom** citeturn0search2. Berikut adalah ringkasan variabel:

- **id**: Identifier unik  
- **Gender**, **City**, **Profession**, **Degree**: Atribut kategorikal  
- **Academic Pressure**, **Work Pressure**, **CGPA**, **Study Satisfaction**, **Job Satisfaction**, **Work/Study Hours**, **Financial Stress**: Skala 1–X numerik  
- **Sleep Duration** (kemudian dikonversi menjadi `Sleep_Duration_Num`), **Dietary Habits**, **Suicidal_Thoughts**, **Family History of Mental Illness**: Berbagai indikator kesejahteraan dan riwayat  
- **Depression**: Label target (0 = tidak depresi, 1 = depresi)

### Missing Value, Duplikat, dan Outlier  
Setelah pemeriksaan, **tidak ditemukan missing value, duplikat, maupun outlier signifikan** pada dataset fileciteturn1file4.

---

## Data Preparation  
1. **Konversi tipe data**:  
   - Categorical → `category` untuk `Gender` dan `City`.  
   - Rename dan mapping *Yes/No* → 1/0 untuk `Suicidal_Thoughts` dan `Family History of Mental Illness`.  
   - Bersihkan `Sleep Duration` dan ubah menjadi numeric `Sleep_Duration_Num`.  
2. **Feature engineering**:  
   - `Stress_Score` = (Academic Pressure + Work Pressure) / 2  
   - Scale fitur `Sleep_Duration_Num`, `Study Satisfaction`, dan `Job Satisfaction` menggunakan *StandardScaler*, lalu gabungkan menjadi komposit `Lifestyle_Balance` (bobot 0.4, 0.3, 0.3).  
3. **Seleksi fitur**:  
   ```python
   predictor_cols = [
       'Age', 'Academic Pressure', 'Work Pressure', 'CGPA',
       'Study Satisfaction', 'Job Satisfaction', 'Sleep_Duration_Num',
       'Stress_Score', 'Lifestyle_Balance',
       'Work/Study Hours', 'Financial Stress', 'Family History of Mental Illness'
   ]
   ```  
4. **Imputasi dan split**:  
   - Isi _missing values_ pada X dengan median.  
   - Bagi data menjadi training (80%) dan testing (20%) fileciteturn1file1.

---

## Modeling  
Tiga model yang dilatih pada data training:

- **Gaussian Naive Bayes**  
- **Decision Tree Classifier** (random_state=42)  
- **Support Vector Machine** (kernel=linear, random_state=42)  

---

## Evaluasi  
| Model                      | Accuracy | Precision (0) | Recall (0) | F1-score (0) | Precision (1) | Recall (1) | F1-score (1) |
|----------------------------|----------|---------------|------------|--------------|---------------|------------|--------------|
| **Naive Bayes**            | 0.7840   | 0.75          | 0.73       | 0.74         | 0.81          | 0.82       | 0.82         |
| **Decision Tree**          | 0.7039   | 0.64          | 0.66       | 0.65         | 0.75          | 0.74       | 0.74         |
| **Support Vector Machine** | 0.8000   | 0.78          | 0.72       | 0.75         | 0.81          | 0.86       | 0.83         |

Model SVM menunjukkan kinerja terbaik dengan **accuracy 80%** dan nilai F1-score tertinggi pada kelas positif fileciteturn0file1.

---

## Penyelesaian Permasalahan  
1. Fitur paling berpengaruh teridentifikasi: `Depression`, `Academic Pressure`, `Work Pressure`, `CGPA`, `Sleep_Duration_Num`, `Stress_Score`, `Lifestyle_Balance`.  
2. Tiga model klasifikasi berhasil dibangun dan dievaluasi.  
3. SVM terpilih sebagai model optimal dengan metrik tertinggi.

---

## Kesimpulan  
- Composite features (`Stress_Score`, `Lifestyle_Balance`) memberikan nilai tambah dalam memprediksi risiko depresi.  
- **Support Vector Machine** adalah model terbaik untuk masalah klasifikasi risiko depresi pada pelajar.  
- Pendekatan ini dapat diintegrasikan dalam sistem pendukung keputusan untuk deteksi dini dan intervensi kesehatan mental pelajar.

---

## Referensi  
- *contoh laporan.md* fileciteturn1file0  
- Student Depression Dataset, Kaggle. citeturn0search2
