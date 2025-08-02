# PROYEK CAPSTONE: EKSPLORASI WAWASAN DARI DATASET PENYAKIT JANTUNG UCI

### Gambaran Umum Proyek

Proyek ini bertujuan untuk menganalisis **Dataset Penyakit Jantung UCI** untuk mengidentifikasi pola, korelasi, dan faktor-faktor risiko yang berkontribusi terhadap penyakit jantung. Dengan menggunakan model bahasa besar (**LLM**) **IBM Granite 3.3 8B Instruct** melalui **Google Colab** dan **API Replicate**, proyek ini akan menerapkan teknik klasifikasi dan ringkasan untuk menggali wawasan yang bermakna dari data.

### Tautan Dataset Mentah

Dataset yang digunakan dapat diunduh dari tautan berikut:

* **Kaggle Dataset:** <https://www.kaggle.com/datasets/ketangangal/heart-disease-dataset-uci/code>

### Deskripsi Fitur Dataset

Berikut adalah penjelasan untuk setiap kolom (fitur) yang ada dalam dataset `heart_cleveland_upload.csv`:

* **age**: Usia pasien dalam tahun.

* **sex**: Jenis kelamin pasien (1 = laki-laki, 0 = perempuan).

* **cp**: Jenis nyeri dada (chest pain type):

  * 0: Nyeri dada asimtomatik (asimtomatik).

  * 1: Angina atipikal (atypical angina).

  * 2: Nyeri non-angina (non-anginal pain).

  * 3: Angina tipikal (typical angina).

* **trestbps**: Tekanan darah istirahat (resting blood pressure) dalam mm Hg saat masuk rumah sakit.

* **chol**: Kolesterol serum dalam mg/dl.

* **fbs**: Gula darah puasa (fasting blood sugar) > 120 mg/dl (1 = ya, 0 = tidak).

* **restecg**: Hasil elektrokardiografi istirahat (resting electrocardiographic results):

  * 0: Normal.

  * 1: Memiliki kelainan gelombang ST-T.

  * 2: Menunjukkan hipertrofi ventrikel kiri yang mungkin atau pasti.

* **thalach**: Denyut jantung maksimum yang dicapai.

* **exang**: Angina akibat olahraga (exercise induced angina) (1 = ya, 0 = tidak).

* **oldpeak**: Depresi ST akibat olahraga relatif terhadap istirahat.

* **slope**: Kemiringan segmen ST latihan puncak (slope of the peak exercise ST segment):

  * 0: Kemiringan ke atas (upsloping).

  * 1: Datar (flat).

  * 2: Kemiringan ke bawah (downsloping).

* **ca**: Jumlah pembuluh darah besar ($0-3$) yang diwarnai oleh flourosopy.

* **thal**: Thalassemia:

  * 0: Normal.

  * 1: Cacat tetap (fixed defect).

  * 2: Cacat terbalik (reversible defect).

* **condition**: Status penyakit jantung (variabel target):

  * 0: Tidak ada penyakit jantung.

  * 1: Ada penyakit jantung.

### Wawasan & Temuan

Berikut adalah wawasan dan temuan utama yang diperoleh dari analisis data tersebut:

* **Pola Demografis**: Rata-rata usia pasien adalah 54,54 tahun, dengan standar deviasi 9,05 tahun. Mayoritas pasien adalah pria (sekitar 68%) dan cenderung lebih dominan terkena penyakit jantung.
* **Korelasi Signifikan**: Terdapat korelasi yang signifikan antara `age` (usia) dan `condition` (kondisi jantung) ($r=0.229$), menunjukkan bahwa semakin tua usia seseorang, semakin tinggi kemungkinan mereka memiliki penyakit jantung.
* **Faktor Risiko Lain**: Meskipun korelasi lemah, faktor-faktor seperti `sex` (jenis kelamin), `cp` (jenis nyeri dada), `thalach` (denyut jantung maksimum), `exang` (angina akibat olahraga), `oldpeak`, `slope`, dan `thal` juga memiliki hubungan dengan kondisi jantung. Pasien dengan nyeri dada asimtomatik (`cp`=0) dan angina tipikal (`cp`=3) menunjukkan prevalensi penyakit jantung yang lebih tinggi.
* **Wawasan Non-Teknis**: Penyakit jantung adalah masalah serius yang seringkali terkait dengan usia, jenis kelamin, dan gaya hidup. Kesadaran akan gejala awal seperti nyeri dada, kelelahan, atau sesak napas sangat penting untuk deteksi dini.

### Kesimpulan & Rekomendasi

Berdasarkan analisis dan temuan yang ada, dapat disimpulkan bahwa penyakit jantung memiliki hubungan yang erat dengan usia dan jenis kelamin, dengan prevalensi yang lebih tinggi pada pria seiring bertambahnya usia. Meskipun faktor lain memiliki korelasi yang lebih lemah, semuanya berkontribusi terhadap risiko penyakit.

Untuk meningkatkan kesadaran dan pencegahan, berikut adalah rekomendasi konkret yang dapat diterapkan:

* **Komunikasi Temuan**: Hasil analisis dapat dikomunikasikan secara visual dan sederhana kepada audiens non-teknis, seperti dalam bentuk infografis atau diagram yang mudah dipahami, untuk menyebarkan informasi tentang faktor-faktor risiko.
* **Peningkatan Kesadaran**: Mengedukasi masyarakat mengenai pentingnya deteksi dini, pengenalan gejala, dan pemeriksaan kesehatan rutin, terutama bagi kelompok usia dan jenis kelamin yang berisiko tinggi.
* **Gaya Hidup Sehat**: Mendorong adopsi gaya hidup sehat sebagai langkah pencegahan utama, meliputi diet seimbang, olahraga teratur, manajemen stres yang efektif, dan menghindari kebiasaan merokok.

### Penjelasan Dukungan AI

Model **IBM Granite 3.3 8B Instruct** digunakan sebagai alat bantu analisis untuk mempercepat dan memperdalam pemahaman terhadap dataset. Model ini berfungsi sebagai **LLM** yang mampu melakukan:

* **Klasifikasi**: Model ini dapat dilatih untuk mengidentifikasi pola dalam data dan mengklasifikasikan pasien ke dalam kategori berpenyakit jantung atau tidak.
* **Ringkasan**: Setelah analisis data dan visualisasi, model dapat digunakan untuk merangkum poin-poin utama secara efektif, membantu dalam penyusunan laporan atau presentasi.

Penggunaan model ini memungkinkan penemuan wawasan yang lebih efisien dan memberikan narasi yang lebih komprehensif dari hasil analisis.
