# Laporan Proyek Machine Learning - Muhamad Thirafi Qaed Setiawan

## Domain Proyek

Proyek Machine Learning ini mengangkat domain kesehatan mental. Proyek yang dibangun adalah
Prediksi Risiko Penyakit Mental pelajar yang dikembangkan berdasarkan data.

## Latar Belakang
Masalah kesehatan mental pada pelajar menjadi perhatian serius dalam beberapa tahun terakhir, seiring dengan meningkatnya tekanan akademik, sosial, dan perubahan gaya hidup digital. Berdasarkan data dari Indonesia National Adolescent Mental Health Survey tahun 2022, sebanyak 34% remaja dilaporkan mengalami masalah kesehatan mental, seperti stres berat, kecemasan, hingga depresi ringan hingga sedang. Selain itu, laporan dari Kementerian Pendidikan, Kebudayaan, Riset, dan Teknologi menunjukkan bahwa lebih dari 20% pelajar di Indonesia menunjukkan gejala gangguan emosi yang memengaruhi konsentrasi belajar dan interaksi sosial. Kondisi ini menegaskan bahwa kesehatan mental pelajar merupakan isu strategis yang memerlukan perhatian dari berbagai pihak, termasuk institusi pendidikan, tenaga kesehatan, orang tua, dan pembuat kebijakan.

<br/>
Di tengah kompleksitas faktor penyebab gangguan mental pada pelajar, mulai dari tekanan akademik, pekerjaan , keuangan, gaya hidup, hingga masalah keluarga, dibutuhkan pendekatan yang proaktif dan terukur untuk mendeteksi risiko sejak dini. Pemanfaatan teknologi, khususnya pendekatan berbasis machine learning, memberikan peluang besar untuk melakukan prediksi dan pemetaan risiko kesehatan mental secara lebih objektif dan efisien. Dengan menganalisis berbagai data seperti kebiasaan belajar, interaksi sosial, gaya hidup digital, dan hasil survei psikologis, sistem berbasis kecerdasan buatan dapat membantu mengidentifikasi pola-pola yang mengarah pada potensi gangguan mental pada pelajar.

<br/>
Pengembangan model prediktif ini diharapkan dapat menjadi langkah awal dalam menciptakan sistem pendukung berbasis teknologi yang mampu memberikan peringatan dini (early warning system), mendukung pengambilan keputusan, serta memfasilitasi intervensi yang lebih cepat dan tepat sasaran. Dalam jangka panjang, integrasi teknologi ini ke dalam sistem pendidikan dapat menjadi salah satu strategi preventif dalam membangun ekosistem pembelajaran yang lebih sehat secara mental dan emosional.

## Business Understanding

### Problem Statements
Berdasarkan latar belakang yang telah disampaikan, terdapat beberapa rumusan masalah yang akan diselesaikan pada proyek ini:
1. Faktor-faktor apa saja yang memengaruhi tingkat risiko gangguan kesehatan mental pada pelajar?
2. Bagaimana cara membangun model machine learning untuk memprediksi kondisi kesehatan mental pelajar berdasarkan data yang tersedia?
3. Bagaimana cara memilih model machine learning yang paling optimal berdasarkan metrik evaluasi seperti akurasi, precision, recall, dan F1-score untuk kasus prediksi kesehatan mental pelajar?

### Goals
Proyek ini dibangun dengan tujuan:
1. Mengidentifikasi variabel-variabel yang berkontribusi signifikan terhadap risiko gangguan kesehatan mental pada pelajar, seperti tekanan akademik, stres finansial, dan kepuasan belajar.
2. Membangun dan melatih model machine learning untuk melakukan klasifikasi kondisi kesehatan mental pelajar berdasarkan fitur numerik dan kategorikal.
3. Mengevaluasi dan membandingkan beberapa algoritma machine learning guna menentukan model terbaik berdasarkan akurasi, precision, recall, dan F1-score dalam memprediksi risiko kesehatan mental pelajar.

### Solution Statements
Untuk mencapai tujuan dalam studi kasus ini, dilakukan beberapa tahapan solusi sebagai berikut:
1. Melakukan eksplorasi dan analisis data untuk memahami karakteristik dataset yang terdiri dari fitur numerik dan kategorikal, seperti Academic Pressure, Financial Stress, Sleep Duration, dan Family History of Mental Illness. Tahapan ini mencakup pembersihan data (data cleaning), transformasi data kategorikal, visualisasi distribusi variabel, serta analisis korelasi untuk mengidentifikasi fitur-fitur yang paling berpengaruh terhadap risiko gangguan kesehatan mental.
2. Membangun model machine learning klasifikasi untuk memprediksi status kesehatan mental pelajar berdasarkan fitur yang telah diolah. Dalam proyek ini, tiga algoritma klasifikasi digunakan:
    - **Naive Bayes**: Model probabilistik yang efisien dan cocok untuk data kategorikal dan numerik yang bersih serta bebas multikolinearitas.
    - **Decision Tree**: Model yang mudah diinterpretasi dan mampu menangani relasi non-linear antara fitur dan label.
    - **Support Vector Machine (SVM)**: Model yang efektif dalam menangani data berdimensi tinggi dan memisahkan kelas dengan margin maksimal.
3. Melakukan evaluasi dan pemilihan model terbaik dengan membandingkan performa masing-masing model berdasarkan metrik evaluasi seperti akurasi, precision, recall, dan F1-score. Hasil evaluasi akan digunakan untuk menentukan model yang paling akurat dan andal dalam memprediksi risiko gangguan kesehatan mental pelajar.


## Data Understanding
Paragraf awal bagian ini menjelaskan informasi mengenai data yang Anda gunakan dalam proyek. Sertakan juga sumber atau tautan untuk mengunduh dataset. Contoh: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Restaurant+%26+consumer+data).

Selanjutnya uraikanlah seluruh variabel atau fitur pada data. Sebagai contoh:  

### Variabel-variabel pada Restaurant UCI dataset adalah sebagai berikut:
- accepts : merupakan jenis pembayaran yang diterima pada restoran tertentu.
- cuisine : merupakan jenis masakan yang disajikan pada restoran.
- dst

**Rubrik/Kriteria Tambahan (Opsional)**:
- Melakukan beberapa tahapan yang diperlukan untuk memahami data, contohnya teknik visualisasi data atau exploratory data analysis.

## Data Preparation
Pada bagian ini Anda menerapkan dan menyebutkan teknik data preparation yang dilakukan. Teknik yang digunakan pada notebook dan laporan harus berurutan.

**Rubrik/Kriteria Tambahan (Opsional)**: 
- Menjelaskan proses data preparation yang dilakukan
- Menjelaskan alasan mengapa diperlukan tahapan data preparation tersebut.

## Modeling
Tahapan ini membahas mengenai model machine learning yang digunakan untuk menyelesaikan permasalahan. Anda perlu menjelaskan tahapan dan parameter yang digunakan pada proses pemodelan.

**Rubrik/Kriteria Tambahan (Opsional)**: 
- Menjelaskan kelebihan dan kekurangan dari setiap algoritma yang digunakan.
- Jika menggunakan satu algoritma pada solution statement, lakukan proses improvement terhadap model dengan hyperparameter tuning. **Jelaskan proses improvement yang dilakukan**.
- Jika menggunakan dua atau lebih algoritma pada solution statement, maka pilih model terbaik sebagai solusi. **Jelaskan mengapa memilih model tersebut sebagai model terbaik**.

## Evaluation
Pada bagian ini anda perlu menyebutkan metrik evaluasi yang digunakan. Lalu anda perlu menjelaskan hasil proyek berdasarkan metrik evaluasi yang digunakan.

Sebagai contoh, Anda memiih kasus klasifikasi dan menggunakan metrik **akurasi, precision, recall, dan F1 score**. Jelaskan mengenai beberapa hal berikut:
- Penjelasan mengenai metrik yang digunakan
- Menjelaskan hasil proyek berdasarkan metrik evaluasi

Ingatlah, metrik evaluasi yang digunakan harus sesuai dengan konteks data, problem statement, dan solusi yang diinginkan.

**Rubrik/Kriteria Tambahan (Opsional)**: 
- Menjelaskan formula metrik dan bagaimana metrik tersebut bekerja.

**---Ini adalah bagian akhir laporan---**

_Catatan:_
- _Anda dapat menambahkan gambar, kode, atau tabel ke dalam laporan jika diperlukan. Temukan caranya pada contoh dokumen markdown di situs editor [Dillinger](https://dillinger.io/), [Github Guides: Mastering markdown](https://guides.github.com/features/mastering-markdown/), atau sumber lain di internet. Semangat!_
- Jika terdapat penjelasan yang harus menyertakan code snippet, tuliskan dengan sewajarnya. Tidak perlu menuliskan keseluruhan kode project, cukup bagian yang ingin dijelaskan saja.





\n


 Laporan Proyek Pertama Kelas Machine Learning Terapan - Dwi Laras Setyadita
---
## Domain Proyek
Proyek *Machine Learning* ini mengangkat domain kesehatan. Proyek yang dibangun adalah  
*Prediksi Risiko Penyakit Mental* yang dikembangkan berdasarkan data.

## Latar Belakang
Masalah kesehatan mental dan regulasi emosi menjadi isu yang semakin memerlukan perhatian serius, khususnya di kalangan pelajar. Masa pendidikan sering kali menjadi fase yang penuh tekanan, baik dari segi akademik maupun sosial. Berdasarkan Survei Kesehatan Indonesia 2023 yang dilakukan oleh Kementerian Kesehatan, prevalensi depresi nasional mencapai 1,4%, menunjukkan bahwa gangguan kesehatan mental bukanlah hal yang jarang terjadi. Lebih lanjut, survei dari Indonesia National Adolescent Mental Health 2022 mengungkap bahwa satu dari tiga remaja mengalami masalah kesehatan mental, sementara satu dari dua puluh mengalami gangguan mental dalam 12 bulan terakhir. Temuan ini menunjukkan bahwa pelajar merupakan kelompok yang rentan, dan penanganan terhadap isu ini perlu dilakukan secara lebih sistematis dan terukur.

<br/>
Dalam konteks kehidupan pelajar, terdapat berbagai faktor yang berpotensi memengaruhi kondisi mental seseorang, seperti tekanan akademik (academic pressure), tekanan kerja (work pressure), indeks prestasi (CGPA), kepuasan belajar (study satisfaction), jam belajar atau bekerja, stres keuangan, serta kebiasaan tidur dan pola makan. Selain itu, faktor-faktor demografis dan sosial seperti jenis kelamin, latar belakang pendidikan, dan riwayat keluarga terhadap gangguan mental juga turut berperan dalam memengaruhi kesejahteraan psikologis pelajar. Melalui pengumpulan data yang mencakup variabel-variabel tersebut—baik numerik maupun kategorikal—diperoleh gambaran komprehensif mengenai kondisi dan potensi risiko kesehatan mental pada pelajar.

<br/>
Pemanfaatan teknologi digital, khususnya sistem prediktif berbasis machine learning, berpotensi menjadi solusi inovatif untuk mendeteksi risiko masalah kesehatan mental secara dini. Dengan kemampuan analisis data yang cepat dan akurat, algoritma machine learning dapat mengidentifikasi pola dan hubungan tersembunyi antar faktor yang berkaitan dengan depresi dan kondisi mental lainnya. Dalam proyek ini, data yang mencakup berbagai aspek kehidupan pelajar—seperti tekanan akademik, stres finansial, kebiasaan tidur, dan riwayat kesehatan keluarga—digunakan untuk membangun model prediksi yang dapat memetakan risiko depresi secara individual.

<br/>
Dengan pendekatan ini, diharapkan dapat dihasilkan sistem pendukung yang mampu memberikan peringatan dini terhadap potensi gangguan mental, khususnya pada pelajar. Teknologi ini dapat menjadi alat bantu bagi institusi pendidikan, psikolog sekolah, maupun pengambil kebijakan dalam menyusun strategi intervensi yang tepat sasaran, serta menciptakan lingkungan belajar yang lebih sehat secara mental dan emosional.



## Business Understanding

## Problem Statements
Berdasarkan latar belakang yang telah disampaikan, terdapat beberapa rumusan masalah yang akan diselesaikan pada proyek ini:
1. Faktor-faktor apa saja yang memengaruhi tingkat risiko gangguan kesehatan mental pada pelajar?
2. Bagaimana cara membangun model machine learning untuk memprediksi kondisi kesehatan mental pelajar berdasarkan data yang tersedia?
3. Bagaimana cara memilih model machine learning yang paling optimal berdasarkan metrik evaluasi seperti akurasi, precision, recall, dan F1-score untuk kasus prediksi kesehatan mental pelajar?

### Goals
Proyek ini dibangun dengan tujuan:
1. Mengidentifikasi variabel-variabel yang berkontribusi signifikan terhadap risiko gangguan kesehatan mental pada pelajar, seperti tekanan akademik, stres finansial, dan kepuasan belajar.
2. Membangun dan melatih model machine learning untuk melakukan klasifikasi kondisi kesehatan mental pelajar berdasarkan fitur numerik dan kategorikal.
3. Mengevaluasi dan membandingkan beberapa algoritma machine learning guna menentukan model terbaik berdasarkan akurasi, precision, recall, dan F1-score dalam memprediksi risiko kesehatan mental pelajar.

### Solution Statements
Untuk mencapai tujuan dalam studi kasus ini, dilakukan beberapa tahapan solusi sebagai berikut:
1. Melakukan eksplorasi dan analisis data untuk memahami karakteristik dataset yang terdiri dari fitur numerik dan kategorikal, seperti Academic Pressure, Financial Stress, Sleep Duration, dan Family History of Mental Illness. Tahapan ini mencakup pembersihan data (data cleaning), transformasi data kategorikal, visualisasi distribusi variabel, serta analisis korelasi untuk mengidentifikasi fitur-fitur yang paling berpengaruh terhadap risiko gangguan kesehatan mental.
2. Membangun model machine learning klasifikasi untuk memprediksi status kesehatan mental pelajar berdasarkan fitur yang telah diolah. Dalam proyek ini, tiga algoritma klasifikasi digunakan:
    - **Naive Bayes**: Model probabilistik yang efisien dan cocok untuk data kategorikal dan numerik yang bersih serta bebas multikolinearitas.
    - **Decision Tree**: Model yang mudah diinterpretasi dan mampu menangani relasi non-linear antara fitur dan label.
    - **Support Vector Machine (SVM)**: Model yang efektif dalam menangani data berdimensi tinggi dan memisahkan kelas dengan margin maksimal.
3. Melakukan evaluasi dan pemilihan model terbaik dengan membandingkan performa masing-masing model berdasarkan metrik evaluasi seperti akurasi, precision, recall, dan F1-score. Hasil evaluasi akan digunakan untuk menentukan model yang paling akurat dan andal dalam memprediksi risiko gangguan kesehatan mental pelajar.

## Data Understanding
Dataset yang digunakan pada proyek ini diambil dari 
<br/>
https://www.kaggle.com/datasets/mahdimashayekhi/mental-health
<br/>
### EDA - Deskripsi Variabel
## Deskripsi Dataset
Dataset yang digunakan terdiri dari **10.000 baris data** dan **14 kolom**, yang merepresentasikan berbagai informasi 
terkait kondisi kesehatan mental individu. Berikut adalah penjelasan masing-masing kolom:
- **age**: Usia responden dalam tahun.
- **gender**: Jenis kelamin responden (Male, Female, Non-binary, dan Prefer not to say).
- **employment_status**: Status pekerjaan responden (Employed, Student, Self-employed, dan Unemployed).
- **work_environment**: Kondisi lingkungan kerja responden (Onsite, Online, dan Hybrid).
- **mental_health_history**: Riwayat kesehatan mental sebelumnya (Yes/No).
- **seeks_treatment**: Apakah responden pernah mencari perawatan kesehatan mental (Yes/No).
- **stress_level**: Tingkat stres yang dialami responden, dengan rentang nilai 1–10.
- **sleep_hours**: Jumlah rata-rata jam tidur per hari, dengan rentang nilai 1–10.
- **physical_activity_days**: Jumlah hari dalam seminggu di mana responden melakukan aktivitas fisik, dengan rentang 1–7.
- **depression_score**: Skor tingkat depresi yang dialami responden, dengan rentang 1–30.
- **anxiety_score**: Skor tingkat kecemasan yang dialami responden, dengan rentang 1–21.
- **social_support_score**: Skor tingkat dukungan sosial yang diterima responden, dengan rentang 1–100.
- **productivity_score**: Skor tingkat produktivitas responden, dengan rentang 1–100.
- **mental_health_risk**: Kategori risiko kesehatan mental hasil dari analisis data (High, Medium, Low).

### Variable - variable pada dataset
- Data Integer = age, stress_level, physical_activity_days, depression_score, anxiety_score, social_support_score.  
- Data Float = sleep_hours, productivity_score.  
- Data Object = gender, employment_status, work_environment, mental_health_history, seeks_treatment, mental_health_risk.

### Missing Value, Data Duplikat dan Outlier
- Tidak ditemukan missing value di dalam dataset.  
- Tidak ditemukan outlier di dalam dataset.  
- Tidak ditemukan data duplikat di dalam dataset.

### EDA - Univariate Analysis
Analisis univariat dilakukan untuk memahami distribusi masing-masing variabel secara individual. Beberapa temuan awal:

##### Kolom Categorical 
![Grafik Univariate Numeric Data](./gambar/univariate_categorical.png)
- Terdapat 4 kategori dalam fitur gender yang didominasi dengan kategori Male dan Female dengan perbandingan yang cukup seimbang. 
- Terdapat 4 kategori dalam fitur employment, secara berurutan dari yang paling banyak adalah employed, kemudian diikuti student, self emoployed, dan yang paling sedikit adalah unemployed.
- Terdapat 3 kategori dalam fitur work_environtment. secara berurutan dari yang paling banyak adalah onsite, Remote, dan Hybrid.
- Terdapat 2 kategori dalam fitur mental_health_history. dengan hampir 70% data memiliki value no yang berarti sebagian besar tidak memiliki riwayat penyakit mental.
- Terdapat 2 kategori dalam fitur seeks_treatment, yaitu yes dan no. dengan hampir 60% data menyatakan no yang artinya belum pernah mencari bantuan professional dalam masalah kesehatan mental.
- Terdapat 3 kategori dalam fitur mental_health_risk. Secara berurutan dari yang terbesar adalah medium sebesar 58,9% high sebesar 23,7%, dan low sebesar 17,4%.

##### Kolom Numerik
![Grafik Univariate Numeric Data](./gambar/univariate_numeric.png)
- Data pada kolom stress_level, age, physical_activity_days, anxiety_score, dan social_support_score cenderung memiliki persebaran yang merata.  
- Terdapat peningkatan jumlah yang signifikan pada data fitur depression_score pada nilai maksimal (30).  
- Terdapat peningkatan jumlah yang signifikan pada data fitur productivity_score pada nilai maksimal (100).  
- Data sleep_hours cenderung terdistribusi normal.

### EDA - Multivariate Analysis

##### Kolom Categorical
![Grafik Multivariate Categorical Data](./gambar/multivariate_categorical.png)

- Pada fitur gender, risiko kesehatan mental cenderung merata di semua gender dengan mayoritas berada pada risiko sedang.  
  Tidak ada kategori tertentu yang cenderung memiliki risiko kesehatan mental tinggi, sedang, maupun rendah.  
- Pada fitur employment_status, risiko kesehatan mental pada setiap kategori cenderung merata.  
  Tidak ada kategori tertentu yang cenderung memiliki risiko kesehatan mental tinggi, sedang, maupun rendah.  
- Pada fitur work_environment, risiko kesehatan mental pada setiap kategori juga cenderung merata.  
  Tidak ada kategori tertentu yang cenderung memiliki risiko kesehatan mental tinggi, sedang, maupun rendah.  
- Pada fitur mental_health_history, risiko kesehatan mental pada setiap kategori cenderung merata.  
  Tidak ada kategori tertentu yang cenderung memiliki risiko kesehatan mental tinggi, sedang, maupun rendah.  
- Pada fitur seeks_treatment, tidak ada kategori tertentu yang cenderung memiliki risiko kesehatan mental tinggi, sedang, maupun rendah.  

<br/>

- Fitur seeks_treatment menunjukkan hubungan yang signifikan secara statistik terhadap fitur mental_health_risk.  
  Hal ini dapat diartikan bahwa kecenderungan individu untuk mencari bantuan atau perawatan memiliki pengaruh yang signifikan  
  terhadap tingkat risiko kesehatan mental mereka.  
- Fitur lain seperti gender, employment_status, work_environment, dan mental_health_history tidak menunjukkan hubungan  
  statistik yang signifikan terhadap fitur mental_health_risk.  
  Hal ini dapat diartikan bahwa faktor-faktor tersebut tidak cukup kuat untuk membedakan tingkat risiko kesehatan mental pada individu.

##### Kolom Numerik
![Grafik Multivariate Categorical Data](./gambar/multivariate_numeric.png)
- Pada fitur age, tidak terdapat kalangan umur tertentu yang memiliki kecenderungan risiko kesehatan mental kategori high,  
  medium, maupun low.  
- Pada fitur stress_level, variasi stres pada setiap individu di dalam kategori mental_health_risk cenderung mirip,  
  namun tingkat stres secara umum (berdasarkan median) pada fitur mental_health_risk kategori low cenderung memiliki  
  tingkat stres yang lebih rendah.  
- Pada fitur sleep_hours, tidak terdapat waktu tidur tertentu yang memiliki kecenderungan kesehatan mental kategori  
  high, medium, maupun low.  
- Pada fitur physical_activity_days, individu dengan risiko kesehatan mental kategori high menunjukkan kecenderungan  
  memiliki tingkat aktivitas fisik yang lebih tinggi dibandingkan kategori lainnya. Individu dengan risiko kesehatan mental  
  high dan low memiliki median aktivitas fisik mingguan yang sama, yaitu sekitar 4 hari. Sementara itu, individu dengan  
  risiko kategori medium memiliki median aktivitas fisik yang lebih rendah, yaitu sekitar 3 hari.  
- Pada fitur depression_score, menunjukkan bahwa semakin tinggi risiko kesehatan mental seseorang, semakin tinggi pula  
  skor depresi yang dimilikinya. Ini menunjukkan bahwa kolom depression_score memiliki korelasi yang tinggi dengan  
  kolom mental_health_risk.  
- Pada fitur anxiety_score, menunjukkan bahwa semakin tinggi risiko kesehatan mental seseorang, semakin tinggi pula  
  anxiety_score yang dimilikinya. Ini menunjukkan bahwa kolom anxiety_score memiliki korelasi yang cukup tinggi dengan  
  kolom mental_health_risk.  
- Distribusi nilai pada fitur social_support terlihat relatif merata di setiap kategori mental_health_risk, tanpa adanya  
  perbedaan yang mencolok di antara kategori tersebut.  
- Pada fitur productivity_score menunjukkan korelasi yang kuat dengan fitur mental_health_risk, dimana risiko kesehatan  
  mental individu dengan kategori low memiliki tingkat produktivitas tertinggi dengan nilai median sekitar 95, kemudian  
  individu dengan risiko kesehatan mental kategori medium memiliki nilai median tingkat produktivitas yang lebih rendah  
  yaitu sekitar 80, dan yang terakhir adalah individu dengan tingkat risiko kesehatan mental kategori high memiliki  
  tingkat produktivitas terendah dengan median sekitar 60-an.


## Data Preparation
- Menghapus kolom yang tidak relevan. Beberapa kolom tersebut adalah 'gender', 'employment_status', 'work_environment', 'mental_health_history', 'age', 'stress_level', 'sleep_hours', dan 'social_support_score' dihapus karena tidak memiliki pengaruh yang signifikan terhadap tingkat resiko kesehatan mental (variabel target).
- Melakukan Label Encoding untuk seeks_treatment (data kategorikal non ordinal dengan 2 label memungkinkan untuk dilakukan label encoding) dan mental_health_risk adalah data ordinal sehingga encoder dilakukan dengan metode labeling.
- Melakukan spliting pada dataset dengan rasio pembagian 90% untuk data training dan 10% untuk data testing. Berdasarkan data yang berjumlah 10.000, rasio ini sudaha baik karena model memiliki cukup data untuk training dan cukup data untuk melakukan testing.
- Melakukan Scalling dengan StandardScaller untuk membuat data numerik berada pada rentang nilai yang sama. Hal ini dilakukan agar algoritma tidak bias, kecenderungan model seperti KNN menganggap kolom dengan rentang nilai yang tinggi adalah kolom yang penting. 

## Modeling
- KNN (K-Nearest Neighbor) adalah model machine learning yang bekerja dengan cara membandingkan jarak dari suatu sampel  
  ke sampel pelatihan yang lain dengan memilih sejumlah (k) tetangga terdekat. Dalam studi kasus ini,  
  model K-Nearest Neighbors (KNN) digunakan untuk mengklasifikasikan risiko kesehatan mental dengan parameter  
  n_neighbors=10, yang berarti setiap prediksi didasarkan pada 10 tetangga terdekat dalam data latih. KNN adalah  
  algoritma yang sederhana dan mudah dipahami, namun memiliki kelemahan seperti kurang efektif pada data berdimensi  
  tinggi (curse of dimensionality), sensitif terhadap outlier, dan performa yang menurun jika data tidak seimbang.  
  Selain itu, waktu prediksi bisa menjadi lambat pada dataset besar karena perlu menghitung jarak ke seluruh data latih.

- Random Forest adalah algoritma machine learning yang digunakan untuk menyelesaikan masalah klasifikasi dan regresi.  
  Random Forest adalah kumpulan dari beberapa model decision tree yang masing-masing memiliki hyperparameter berbeda dan  
  dilatih pada beberapa bagian data yang berbeda. Dengan melakukan beberapa keputusan sekaligus melalui beberapa pohon,  
  algoritma Random Forest sangat cocok digunakan pada kasus klasifikasi.  
  Random Forest merupakan metode ensemble yang menggabungkan hasil dari banyak pohon keputusan untuk meningkatkan  
  akurasi dan mengurangi risiko overfitting. Dalam studi kasus ini, model yang dibangun menggunakan n_estimators=50,  
  artinya 50 pohon dibangun, serta max_depth=16 yang membatasi kedalaman maksimal tiap pohon untuk mengontrol kompleksitas model.  
  Parameter random_state=55 digunakan agar hasil pelatihan konsisten dan dapat direproduksi. Sementara itu, n_jobs=-1  
  memungkinkan model memanfaatkan seluruh inti CPU yang tersedia untuk mempercepat proses pelatihan. Random Forest sangat kuat  
  dalam menangani data kompleks dan tahan terhadap noise, tetapi model ini sulit diinterpretasikan dan membutuhkan sumber daya  
  komputasi yang lebih besar.

- Boosting adalah metode klasifikasi yang menggabungkan banyak model sederhana secara bertahap untuk meningkatkan  
  akurasi dengan fokus memperbaiki kesalahan prediksi sebelumnya. Dalam studi kasus ini, AdaBoostClassifier digunakan  
  sebagai metode boosting, dengan learning_rate=0.05, yang menentukan seberapa besar kontribusi setiap model lemah dalam pembelajaran bertahap.  
  Model ini juga menggunakan random_state=55 untuk memastikan hasil yang konsisten. Boosting bekerja dengan memperbaiki  
  kesalahan model sebelumnya secara iteratif, sehingga meningkatkan performa keseluruhan. Namun, AdaBoost dapat menjadi  
  sensitif terhadap outlier dan noise, serta memiliki waktu pelatihan yang lebih lambat dibandingkan beberapa metode lain  
  karena proses pembelajarannya yang bertahap.

## Evaluasi
![Grafik Akurasi Model](./gambar/accuracy2.png)

Evaluasi model dilakukan menggunakan metric accuracy, precision, Recall, dan F1-score untuk mengukur performa dari 
masing-masing model yang digunakan yaitu KNN, Random Forest, dan Boosting Algorithm. 
Berdasarkan hasil akurasi didapatkan informasi sebagai berikut:
- Model terbaik model dengan algoritma random forest yang menghasilkan akurasi, precision, f1-score, dan recall tertinggi, 
yaitu seluruhnya sebesar 99,4%.

- Model kedua terbaik adalah KNN yang menghasilkan akurasi, precision, f1-score, dan recall tidak berbeda jauh dengan random 
forest yaitu semuanya sebesar 97,6%.

- Model terburuk untuk studi kasus ini adalah model yang dibangun dengan algoritma Boosting yang menghasilkan akurasi, 
precision, f1-score dan recall yang cukup rendah, yaitu secara berturut-turut 59,3%; 35,1%; 44,1%; dan 59,3%.

### Penyelesaian permasalahan
1. Setelah melakukan proses EDA, berhasil dilakukan identifikasi fitur-fitur penting dalam klasifikasi resiko kesehatan 
mental yaitu: seeks_treatment, physical_activity_days,	depression_score,	anxiety_score, dan	productivity_score
2. Didalam proyek ini telah dibangun  3 algoritma klasifikasi untuk melakukan prediksi klasifikasi resiko kesehatan mental.
3 model yang dibangun adalah : KNN, Random Forest, dan Boosting Algorithm. Penggunaan parameter seperti n_neighbors, 
n_estimators, dan learning_rate juga sudah dioptimalkan sesuai kebutuhan.
3. Dari evaluasi yang dilakukan, Random Forest terbukti sebagai model paling optimal, karena memiliki nilai tertinggi untuk semua 
metrik dibandingkan model lain. Meskipun KNN mencapai metrik yang hampir sama dengan Random Forest, semua metrik evaluasi 
yang dihasilkan masih lebih rendah. 

### Kesimpulan 
Analisis fitur mengungkapkan bahwa seeks_treatment, physical_activity_days, depression_score, anxiety_score, dan 
productivity_score merupakan variabel paling penting yang memengaruhi prediksi risiko kesehatan mental.
<br/>
Berdasarkan hasil evaluasi, model Random Forest merupakan model terbaik untuk prediksi klasifikasi risiko kesehatan 
mental pada studi kasus ini. Model ini menunjukkan performa tertinggi pada semua metrik evaluasi dibandingkan dengan 
model lainnya.
<br/>
Meskipun model KNN memiliki nilai akurasi, recall, precision, dan F1-score yang sedikit lebih rendah, selisihnya 
tidak signifikan sehingga model ini tetap dapat dipertimbangkan sebagai alternatif.
<br/>
Dengan tercapainya tujuan prediksi risiko kesehatan mental secara dini, diharapkan proyek ini dapat membantu 
meningkatkan kesadaran individu untuk lebih cepat mencari bantuan atau perawatan ketika terdapat indikasi risiko 
kesehatan mental yang dialami.
![Grafik Akurasi Model](./gambar/accuracy.png)
## Referensi

[1]: Kementerian Kesehatan Republik Indonesia, *Laporan Tematik Survei Kesehatan Indonesia Tahun 2023: Potret Indonesia Sehat*, Jakarta: Kementerian Kesehatan RI, 2024. Diterbitkan oleh Kementerian Kesehatan RI dan dikeluarkan oleh Badan Kebijakan Pembangunan Kesehatan. [Online]. Available: https://drive.google.com/file/d/1AnuDQgQufa5JSXEJWpBSv4r7v6d5YZm7/view. [Accessed: May 24, 2025].

[2]: Universitas Gadjah Mada, Universitas Sumatera Utara, Universitas Hasanuddin, The University of 
Queensland Australia, Johns Hopkins Bloomberg School of Public Health, and Kementerian Kesehatan Republik 
Indonesia, *I-NAMHS: Indonesia-National Adolescent Mental Health Survey*, 2022.
