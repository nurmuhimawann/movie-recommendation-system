# Laporan Proyek Machine Learning - Mawan



<p align='center'>
  <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />        
  </a>
  <a href="https://github.com/nurmuhimawann/">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />        
  </a>
  <a href="https://www.kaggle.com/datasets/atharvaingle/crop-recommendation-dataset">
    <img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white" />
  </a
   <a href="https://colab.research.google.com/">
    <img src="https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252" />
  </a
</p>
    
<div align="center">

| Profile       |                                           |
| ------------- | ----------------------------------------- |
| Nama          | Nur Muhammad Himawan                      |
| Learning Path | Machine Learning & Front End Development  |
| Progam        | Studi Independen Batch 3 - Kampus Merdeka |
| Submission    | Proyek Machine Learning Terapan           |

</div>

<p align='center'>
    <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/hero-images.png?raw=true" alt="netflix-images">
</p>



## Project Overview

Dalam era digital saat ini, informasi sangat mudah untuk didapatkan dan ketersediaannya memiliki jumlah yang tidak terbatas. informasi menjadi kebutuhan utama dalam bisnis yang berkembang saat ini. Ada ketergantungan yang meningkat pada penggalian informasi dari sekumpulan data untuk mendorong solusi bisnis. Berbagai perusahaan memanfaatkan informasi guna mengetahui apa yang disukai oleh pelanggannya. Hal inilah yang mendorong munculnya sistem rekomendasi. Dimana, sistem rekomendasi memainkan peranan yang sangat penting saat ini karena penerapannya dalam berbagai bidang yang sangat powerfull. Sistem ini banyak diadopsi oleh berbagai perusahaan untuk memberikan pengalaman pengguna yang lebih baik untuk mencapai pertumbuhan pelanggan. Sistem rekomendasi bekerja dengan memprediksi preferensi pengguna terhadap item tertentu berdasarkan perilaku pengguna di masa lalu atau perilaku pengguna lainnya untuk memberikan saran berdasarkan preferensi ini di masa mendatang. Sistem ini sangat populer saat ini dan banyak diaplikasikan seperti rekomendasi film, konten video pada platform youtube, hingga music pada spotify juga menerapkan sistem rekomendasi.

Dilain sisi, pandemi COVID-19 telah mengakselerasi pertumbuhan konten digital di masyarakat. Salah satunya adalah banyaknya pilihan TV Series dan Film untuk dinikmati banyak orang di dunia termasuk masyarakat Tanah Air. Selain itu, menjamurnya layanan streaming seperti Netflix, Disney Plus, dll. ternyata membentuk tren baru dalam menonton film. Diantaranya adalah binge watching dan hopping, yakni suatu aktivitas atau kebiasaan menonton film berturut-turut tanpa jeda. Dengan banyaknya konten dan pilihan genre film yang tersedia, platform penyedia layanan perlu memberikan item-item yang relevan sesuai dengan minat pelanggannya guna mempertahankan pelanggan. Sistem rekomendasi merupakan alternatif yang solutif untuk memberikan rekomendasi film yang sesuai dengan minat pengguna. Oleh karena itu, proyek machine learning ini bertujuan untuk mengembangkan model machine learning yang digunakan untuk sistem rekomendasi film dengan mempertimbangkan rating film di masa lalu yang diberikan oleh berbagai pengguna untuk memberikan rekomendasi kepada pengguna.

**Artikel dan Jurnal Referensi**:

- [How to Build a Movie Recommendation System](https://towardsdatascience.com/how-to-build-a-movie-recommendation-system-67e321339109) 
- [Mengenal Istilah Binge Watching dan Hopping yang Jadi Tren Terbaru Nonton Film](https://kumparan.com/millennial/mengenal-istilah-binge-watching-dan-hopping-yang-jadi-tren-terbaru-nonton-film-1wREvjSoXeB/1) 
- [Perancangan Sistem Rekomendasi Menggunakan Metode Collaborative Filtering dengan Studi Kasus Perancangan Website Rekomendasi Film](https://www.neliti.com/publications/504836/perancangan-sistem-rekomendasi-menggunakan-metode-collaborative-filtering-dengan) 
- [Sistem Rekomendasi Film Menggunakan Metode Hybrid Collaborative Filtering Dan Content-based Filtering](https://openlibrarypublications.telkomuniversity.ac.id/index.php/engineering/article/view/18066) 

## Business Understanding

### Problem Statements

Berdasarkan uraian yang telah dipaparkan pada latar belakang diatas, maka dapat diambil sebuah rumusan masalah yang dirumuskan sebagai berikut:
- Bagaimana mengembangkan sistem rekomendasi film yang sesuai dengan preferensi, minat atau perilaku pengguna?
- Bagaimana hasil dan evaluasi model dalam mengembangkan sistem rekomendasi film yang sesuai dengan preferensi, minat atau perilaku pengguna?

### Goals

Berdasarkan rumusan masalah yang telah dipaparkan di atas, maka proyek penelitian ini memiliki tujuan, yaitu:

- Mengetahui cara pengembangan sistem rekomendasi film yang sesuai dengan preferensi, minat atau perilaku pengguna.
- Mengetahui hasil dan evaluasi model dalam mengembangkan sistem rekomendasi film yang sesuai dengan preferensi, minat atau perilaku pengguna.

### Solution statements

Berdasarkan tujuan yang telah dipaparkan diatas, maka proyek penelitian ini memiliki solusi atau tahapan sebagai berikut:

- Melakukan data preprocessing dan exploratory data analysis (EDA) pada dataset yang dipakai dengan melihat keterkaitan antar feature pada data tersebut untuk mendapatkan insight dan knowledge.
- Mengembangkan model machine lerning yang sesuai untuk membangun sistem rekomendasi dan melakukan evaluasi model dengan menggunakan evaluation matrix. Teknik yang akan diimplementasikan untuk membangun sistem ini adalah sebagai berikut:
  - Content-Based Filtering, merekomendasikan beberapa item berdasarkan kemiripan antar item yang direkomendasikan dengan item yang dipilih.
  - Collaborative Filtering, merupakan sistem rekomendasi yang memberikan rekomendasi item berdasarkan preferensi komunitas atau pengguna lain.

- Menampilkan hasil rekomendasi berdasarkan model yang telah dikembangkan.
- Melakukan evaluasi berdasarkan metriks evaluasi dari model sistem rekomendasi yang telah dikembangkan.

## Data Understanding
Dataset yang digunakan pada proyek ini merupakan data film yang dipublikasikan melalui website MovieLens dengan judul [MovieLens 25M Dataset](https://grouplens.org/datasets/movielens/#:~:text=MovieLens%2025M%20Dataset). Dataset ini berformat zip yang memiliki 7 file terpisah diantaranya `movies.csv`, `ratings.csv`, `genome-scores.csv`, `links.csv`,  `tags.csv`, `genome-tags.csv`,  dan `README.txt`. Berdasarkan `README.txt` yang telah disediakan, dataset ini (ml-25m) merupakan dataset yang berisi data films dan rating yang telah diberikan oleh pengguna. yang mana data ratings berisi 25.000.095 peringkat film. Dataset ini dibuat pada 21 November 2019 oleh 162.541 pengguna yang dikumpulkan dalam kurun waktu film rilis pada 09 Januari 1995 hingga 21 November 2019.

<p align='center'>
    <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/movielens25m.png?raw=true" alt="netflix-images">
</p>

**Dataset Information:**

| Jenis     | Keterangan                                                   |
| --------- | ------------------------------------------------------------ |
| Title     | MovieLens 25M Dataset                                        |
| Source    | [GroupLens](https://grouplens.org/datasets/movielens/#:~:text=MovieLens%2025M%20Dataset) |
| Owner     | [GroupLens Research](https://grouplens.org/about/what-is-grouplens/) |
| Permalink | https://grouplens.org/datasets/movielens/25m/                |

### Variabel-variabel pada dataset:

Pada file `movies.csv` berisi daftar film yang memiliki 62.423 records data dan 3 feature:

- `movieId` : memuat nomor ID film  
- `title` : memuat judul film
- `genres` : memuat genre film

Pada file `ratings.csv` berisi daftar ratings atau penilaian terhadap satu film yang memiliki 25.000.095 records data dan 4 feature:

- `userId` : memuat nomor ID users
- `movieId` : memuat nomor ID film  
- `rating` : memuat rating atau penilaian films dalam skala bintang, dengan peningkatan setengah bintang dalam rentang 0,5 - 5 bintang
- `timestamp` : memuat kode timestamp

Pada file `tags.csv` berisi daftar tags pada film yang diberikan users yang memiliki 1.093.360 records data dan 4 feature:

- `userId` : memuat nomor ID users
- `movieId` : memuat nomor ID film  
- `tag` : memuat tag film
- `timestamp` : memuat kode timestamp

Pada file `links.csv` berisi daftar links film yang mengarah ke laman website films memiliki 62.423 records data dan 3 feature: 

- `movieId` : memuat nomor ID film yang merujuk pada website MovieLens
- `imdbId` : memuat nomor ID film yang merujuk pada website IMDb
- `tmdbId` : memuat nomor ID film yang merujuk pada website TMDB

Pada file `genome_tags.csv` berisi daftar deskripsi tags yang mereference ke `tagId` yang memiliki 1.128 records data dan 2 feature:

- `tagId` : memuat nomor ID tags
- `tag` : memuat deskripsi tag

Pada file `genome_scores.csv` berisi daftar deskripsi tags yang mereference ke `tagId` yang memiliki 15.584.448 records data dan 3 feature:

- `movieId` : memuat nomor ID film 
- `tagId` : memuat nomor ID tags
- `relevance` : memuat skor relevansi

### Exploratory Data Analysis (EDA)

proses EDA dilakukan dengan menganalisis dataset untuk mendapatkan pemahaman yang utuh mengenai dataset guna menemukan insight & knowledge.

**Univariate Analysis**

Berdasarkan informasi sebelumnya, terdapat 6 berkas csv. saya ingin membagi 6 berkas tersebut menjadi 3 data secara umum berdasarkan kategori ID-nya yaitu data films, users, dan skor relevansi films. kemudian, saya akan mencoba melihat jumlah datanya.

- tag relevance scores

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/relevance-scores.png?raw=true" alt="relevance-score">
  </p>

- films

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/films.png?raw=true" alt="films">
  </p>

- user ratings

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/users%20ratings.png?raw=true" alt="users ratings">
  </p>

Berdasarkan 3 informasi tersebut, terdapat 1.128 pada data unik genome tag, 62.423 untuk data unik films, dan data unik users sebanyak 162.541. menurut saya, jumlah data pada relevancy score berdasarkan tagId sangat sedikit yaitu 1K. berbanding terbalik dengan jumlah data user dan films yang masing-masing berjumlah sekitar 62K dan 162K. maka, saya memutuskan untuk bekerja dengan menggunakan data film dan users saja.

## Data Preparation
Teknik yang digunakan dalam Data Preparation adalah sebagai berikut:

Dilihat dari sudut pandang kerunutan proses dalam data preparation, saya melakukan data cleaning terlebih dahulu pada data `movies.csv` dan `ratings.csv`. setelah kedua data tersebut dirasa sudah terlihat cukup baik, saya melakukan merging dataframe pada kedua data tersebut dan menjadikannya sebagai dataframe yang utuh untuk mengembangkan sistem rekomendasi. Berikut langkah-langkahnya:

1. **Data Cleaning** `movies.csv`

   Pada data `movies.csv`, terdapat tahun rilis dari film yang disertakan secara bersamaan pada feature judul film. Hal ini diperlukan penanganan khusus untuk memisahkan antara judul film dengan tahun rilis agar tidak terjadi permasalahan yang tidak diinginkan pada proses training model. dimana, tahun rilis dari setiap film akan dipisahkan ke dalam kolom tersendiri.

2. **Data Cleaning** `ratings.csv`

   Pada data `ratings.csv`, skala rating pada feature rating memiliki sebaran yang tidak normal. dimana data rating memiliki skala 0.5 sampai 5 dengan perbedaan 0.5 setiap skalanya. handling yang dilakukan untuk pada case ini adalah dengan membulatkan nilai skala pada feature rating agar distribusi skala memiliki rentang 1-5.

   Selanjutnya, terdapat data dalam bentuk kode timestamp. Akan susah untuk dipahami, kapan data tersebut diambil secara spesifik. maka, proses konversi dilakukan untuk mengubah timestamps menjadi data datetime.

3. **Data Merging** `movies` dengan `ratings`

   Penggabungan dilakukan dengan melakukan merge pada kedua dataframe antara `movies` dengan `ratings` menjadi satu dataframe yang utuh dan mengassignnya kedalam variabel `films`.

4. **Data Cleaning** `films`

   Ada beberapa handling yang dilakukan pada dataframe `films`, diantaranya sebagai berikut.

   - Handling Missing Values

     Data yang hilang, null, NaN atau tidak terbaca merupakan hal umum yang seringkali ditemui. Agar data yang missing tidak memengaruhi kinerja model yang akan dikembangkan, maka saya akan menghapusnya. Pada proyek ini, saya menemukan missing values pada beberapa feature, salah satunya adalah genre dimana terdapat data **'(no genres listed)'**.

   - Data Reduction

     Data yang terlalu banyak akan memperlambat kinerja proses machine learning. Pada proyek ini, saya memiliki asumsi kalau terdapat beberapa films yang mendapatkan sedikit review dari users. Dengan mengetahui fakta rating terendah adalah 1 dan rating tertinggi adalah 5. maka, saya akan membuang film yang mendapatkan penilaian kurang dari 50 pereview (jumlah rating 50-250) yaitu yang setidaknya memiliki rating kurang dari 50. Saya berfikir hal ini tidak akan menjadi masalah. Karena, selain jumlah data pada datasetnya memiliki jumlah yang cukup banyak, proses reduction dapat mempercepat runtime model dengan menghemat memory.

   - Handling Duplicate Data

     Dataset yang berantakan dan terduplikasi dapat mempengaruhi hasil modeling dan analisis akhir. Pada proyek ini, terdapat banyak duplikasi data didalamnya berdasarkan id film dan judul film. Menghapusnya merupakan langkah yang tepat untuk merapikan data.

   - Fixed data in genre features

     Pada features genre, saya mendapati genre ***Sci-Fi***. setelah saya pahami, ternyata ***Sci-Fi*** merupakan akronim dari kata ***Science Fiction*** yang menggambarkan film fiksi ilmiah. kata ***Sci-Fi*** memiliki separator dash atau tanda pisah. Hal ini, perlu dihilangkan. apabila tidak dihilangkan maka pada tahap vektorisasi TF-IDF nantinya kata ***Sci-Fi*** akan diperlakukan sebagai 2 kata yang berbeda ***Sci*** dan ***Fi***. karena, pada tahap TF-IDF selain melakukan vektorisasi juga dilakukan tokenisasi.

## Modeling
Pada proyek ini, pendekatan yang dipakai untuk mengembangkan model dalam sistem rekomendasi adalah `Content-Based Filtering` dan `Collaborative Filtering`.

- **Content-Based Filtering**

  Konsep dasar dari content-based filtering adalah memberikan rekomendasi item dengan memperhatikan kemiripan dari item yang disukai oleh pengguna berdasarkan aktivitas pengguna tersebut di masa lalu. Ambil contoh, mawan menyukai film disney Coco. maka, sistem akan merekomendasikan film dengan genre animation yang mirip seperti Encanto. Pada akhirnya, semakin banyak informasi yang didapatkan dari aktivitas pengguna, semakin baik pula akurasi dari sistem rekomendasi yang dihasilkan.

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/content-based.png?raw=true" width=600px alt="content-based">
  </p>

  Nah, pada proyek kali ini, saya akan menerapkan pendekatan content-based filtering untuk mengembangkan model guna membangun sistem rekomendasi film sesuai dengan goals dari proyek ini. Ada beberapa tahapan yang saya lakukan, diantaranya sebagai berikut.

  1. Prepare data

     Menyiapkan dataframe yang telah dibersihkan dalam tahap data preparation sebelumnya.

  2. TF-IDF Vectorizer

     Proses term frequency-inverse document frequency (TF-IDF) diperlukan untuk menemukan representasi kata yang penting dalam kolom genre. Pada proyek ini, proses vectorizer dilakukan dengan memanfaatkan function [tfidfvectorizer()](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html) yang telah tersedia pada library scikit-learn. berikut hasil tf-idf dalam bentuk matrix. yang mana pada matrix menunjukkan korelasi antara film dengan genre-nya.

     <p align='center'>
         <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/vectorizer.png?raw=true" width=auto alt="tfidf">
     </p>

  3. Perhitungan Cosine Similarity

     cosine similarity digunakan untuk menghitung derajat kesamaan (similarity degree) antar film. Pada proyek ini, kalkulasi similarity dilakukan dengan mengimplementasikan function [cosine_similarity()](http://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html) yang telah tersedia pada library sklearn. Perhitungan similarity merupakan tahapan paling penting dalam pendekatan content-based filtering, karena pada dasarnya pendekatan ini menerapkan prinsip kesamaan antar item untuk mendapatkan hasil rekomendasi yang sesuai. Output dari cosine similarity akan menghasilkan suatu matrix kesamaan yang bisa dilihat pada konversi ke bentuk dataframe berikut.

     <p align='center'>
         <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/cosine-similarity.png?raw=true" width=auto alt="cosine-sim">
     </p>

  4. Create Custom Functions

     Tahapan terakhir adalah membangun custom function untuk mendapatkan rekomendasi terhadap data input yang diinginkan. functions ini bekerja dengan mengambil similarity dari data film yang ingin dicari, data yang similar akan dimasukkan ke dalam variabel closest. parameter K di define untuk menghasilkan top-K recommendation berdasarkan tingkat similarity tertinggi. film yang dicari akan dihapus agar tidak muncul dalam daftar rekomendasi. Step terakhir, return digunakan untuk mengembalikan values dalam bentuk dataframe, dimana values yang di return merupakan rekomendasi dari judul film berdasarkan tingkat similarity.

     <p align='center'>
         <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/recommendation-content-based.png?raw=true" width=auto alt="functions">
     </p>

  5. Recommendations

     <p align='center'>
         <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/harry-potter.png?raw=true" width=auto alt="harry">
     </p>

     Berikut ini merupakan Top 5 Recommendations berdasarkan genre dari film 'Harry Potter and the Prisioner of Azkaban'. Sistem telah berhasil merekomendasikan film dengan sesuai, bisa dilihat pada hasil yang mendapatkan rekomendasi film yang mirip dengan genre Adventure dan Fantasy. 

     <p align='center'>
         <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/output-content-based.png?raw=true" width=auto alt="output-cb">
     </p>

  

  Kelebihan Content-Based Filtering

  - Mampu menjelaskan bagaimana hasil rekomendasi didapatkan
  - Kemampuan untuk merekomendasikan item yang sifatnya baru bagi pengguna bahkan belum pernah di-rate oleh siapapun, karena prinsip kerjanya yaitu dengan melihat deskripsi item yang terdapat pada item yang pernah diberi nilai rating tinggi

  Kekurangan Content-Based Filtering

  - Terbatasnya rekomendasi hanya pada item-item yang mirip (similar) sehingga tidak ada kesempatan untuk mendapatkan item yang tidak terduga (serendipity)

  - Sistem tidak dapat memberikan rekomendasi kepada pengguna baru yang belum pernah melakukan aktivitas apapun dan tidak memiliki profil user yang cukup (Cold Start Problem)

    

- **Collaborative Filtering**

  Konsep dasar dari collaborative filtering adalah

  1. Data Understanding

     Pada tahap awal, diperlukan beberapa library salah satunya adalah tensorflow dan dataframe yang dipakai adalah dataframe 'preparation' yang sebelumnya telah digunakan.

  2. Data Preparation

     Proses encoding dilakukan pada tahap ini, dengan melakukan encode pada feature 'userId' dan 'movieId'. proses encode akan memetakan setiap nilai pada kedua feature tersebut ke dalam bentuk index.

  3. Split Data for Training and Validation

     Data dibagi untuk data train dan validasi dengan komposisi 80/20. Pembagian ini bertujuan agar data yang digunakan dapat digunakan untuk mengembangkan model dan mengevaluasi performance dari model yang telah dikembangkan.

  4. Training

     Proses training dilakukan dengan mengimplementasikan teknik embedding untuk menghitung skor kecocokan antara film dengan users. kemudian, pada  proses compile dilakukan menggunakan BinaryCrossentropy untuk menghitung loss function, Adam (Adaptive Moment Estimation) sebagai optimizer, dan root mean squared error (RMSE) sebagai metrics evaluation. Proses training model berjalan sebanyak 25 epochs sebagai berikut.

  5. Metrics Visualization

     Berdasarkan visualisasi, pada proses training model didapatkan nilai error akhir sebesar sekitar 0.17 dan error pada data validasi sebesar 0.26

     <p align='center'>
         <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/plot-metrics.png?raw=true" width=auto alt="metrics">
     </p>

  6. Recommendations

     Kemudian menggunakan model.predict(), sistem akan memberikan rekomendasi sebagai berikut.

     <p align='center'>
         <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/output-collaborative.png?raw=true" width=auto alt="output-collaborative">
     </p>

  Kelebihan Collaborative Filtering

  - Dapat memberikan rekomendasi berdasarkan preferensi komunitas atau pengguna lain

  Kekurangan Collaborative Filtering

  - Membutuhkan banyak users atau pengguna



## Evaluation
Evaluasi dilakukan untuk mengukur sejauh mana performance atau kinerja dari model sistem rekomendasi. Pada proyek ini, evaluasi diukur menggunakan metriks evaluasi sesuai dengan pendekatan yang dipakai dalam pengembangan sistem rekomendasi.

- **Content-Based Filtering**

  Pada pendekatan Content-Based Filtering, performance model diukur menggunakan nilai metriks precisions dengan similarity. Cosinus Similarity merupakan ukuran yang mengkuantifikasi kesamaan antara dua atau lebih vektor. 

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/cosine-sim-formula.png?raw=true" width=auto alt="cosine-sim">
  </p>

  Nilai cosinus similarity memiliki rentang yang terbatas antara 0 dan 1. ukuran kemiripan ditentukan oleh ukuran cosinus sudut antara dua vektor tak nol. Semakin besar nilai cosinus similarity semakin mendekati 1, maka sudut antara kedua vektor juga semakin kecil. Bisa dilihat pada gambar di bawah ini.

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/example-cos-sim.png?raw=true" width=650px alt="example-cosine-sim">
  </p>

  Precision merupakan tingkat ketepatan antara informasi yang diminta oleh pengguna dengan hasil yang diberikan oleh sistem. Precision sangat cocok diterapkan sebagai metriks evaluasi pada sistem rekomendasi yang mana pengukuran kualitas akan ditentukan melalui seberapa bergunakah sistem dapat melakukan prediksi. 

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/precision.png?raw=true" width=auto alt="precision">
  </p>

  Keterangan:

  - **True Postive (TP):** prediksinya **Positif** dan hasil yang sebenarnya memang **Positif.**

  - **False Positive (FP)**: prediksinya **Positif**, namun hasil yang sebenarnya adalah **Negatif.**
  - **True Negative (TN):** prediksinya **Negatif** dan hasil yang sebenarnya memang **Negatif.**
  - **False Negative (FN)**: prediksinya **Negatif**, namun hasil yang sebenarnya adalah **Positif.**

  

  Formula diatas merupakan rumus precision. Namun, dalam sistem rekomendasi lebih sederhana menggunakan rumus seperti gambar dibawah ini. pada dasarnya sama saja, precisions membantu pengguna memilih item yang mirip di antara set item yang tersedia.

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/precision-recommendations.png?raw=true " width=auto alt="precision-for-recommendations">
  </p>

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/harry-potter.png?raw=true" width=auto alt="harry">
  </p>

  Pada pendekatan content-based filtering ini, saya memakai film 'Harry Potter and the Prisioner of Azkaban' untuk mencari rekomendasi film lain yang sesuai. dan mendapatkan hasil sebagai berikut.

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/output-content-based.png?raw=true" width=auto alt="output-cb">
  </p>

  Dengan memakai metrics precision, maka dapat dihitung:

  - 'Harry Potter and the Prisioner of Azkaban' bergenre Adventure, Fantasy, IMAX.
  - Dari 5 film rekomendasi, terdapat 3 film yang memiliki genre yang sama dengan yang dicari yaitu, genre Adventure, Fantasy, IMAX. film terakhir, merekomendasikan film lain dengan genre drama dan thriller. Ini tidak sesuai dengan apa yang dicari.

  Maka, sesuai dengan formula,

  *precision = (# of our recommended that are relevan) / (# of items we recommended item)*

  *precision = 3 / 5*

  *precision = 0.6*

  *precision = 60%*

  Berdasarkan Top 5 rekomendasi film yang diberikan didapatkan pricisions sebesar 60% dari model content-based filtering untuk sistem rekomendasi yang telah dikembangkan.

  

- **Collaborative Filtering**

  Performance dari pendekatan Collaborative Filtering diukur menggunakan metriks evaluasi Root Mean Squared Error (RMSE). RMSE merupakan cara standar untuk mengukur rata-rata kesalahan suatu model dalam memprediksi. RMSE bekerja dengan cara mengurangi nilai prediksi dengan nilai observasi yang kemudian dikuadratkan. Hasilnya akan dijumlahkan (sigma jumlah) dengan keseluruhan hasil lainnya yang selanjutnya dibagi dengan banyaknya data (n). Hasil perhitungan yang didapatkan akan diakar kuadrat sehingga mendapatkan nilai RMSE sesuai dengan formula sebagai berikut.

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/rmse.png?raw=true" width=40% alt="rmse">
  </p>

  Saat melakukan training model, RMSE sangat membantu untuk mengevaluasi dari model dengan melihat penurunan kesalahan pada setiap iterasi (epochs). Kemudian, hasil dari proses training model dapat divisualiasasikan ke dalam plot metrics sebagai berikut.

  <p align='center'>
      <img src ="https://github.com/nurmuhimawann/MLT2-Dicoding/blob/main/images/plot-metrics.png?raw=true" width=auto alt="metrics">
  </p>

  Berdasarkan plot metriks di atas, nilai RMSE didapatkan sebesar 0.17 dan pada data validasi sebesar 0.26 yang mana sistem yang telah dikembangkan sudah cukup baik.



## Conclusion

Disini, saya telah berhasil mengembangkan model sistem rekomendasi untuk film menggunakan dua teknik yang berbeda, yaitu Content-Based Filtering dan Collaborative Filtering. Hasil rekomendasi yang didapatkan cukup bagus. Metode collaborative filtering dapat memberikan hasil rekomendasi yang cukup sesuai. sedangkan metode content-based filtering juga dapat memberikan rekomendasi film yang similar dengan film yang memiliki kemiripan genre. Namun, ada yang perlu diperhatikan bahwa dataset yang digunakan memiliki data film dengan jumlah yang terbatas, bisa jadi pada dunia nyata model tidak memberikan rekomendasi sesuai yang diinginkan pengguna, dimana ada beberapa pengguna yang menyukai rekomendasi film-film terbaru. sedangkan model bisa saja merekomendasikan film-film keluaran lama.



## Reference

- Arfisko, Hilmi Hidayat dan Wibowo, Agung Toto. 2022. “Sistem Rekomendasi Film Menggunakan Metode Hybrid Collaborative Filtering Dan Content-based Filtering”. *e-Proceeding of Engineering*, Vol.9, No. 3 Juni 2022: 2159.
- F. Maxwell Harper dan Joseph A. Konstan. 2015. Kumpulan Data MovieLens: Sejarah dan Konteks. Transaksi ACM pada Sistem Cerdas Interaktif (TiiS) 5, 4: 19:1–19:19. https://doi.org/10.1145/2827872
- kumparan.com. (2021, 31 Agustus). Mengenal Istilah Binge Watching dan Hopping yang Jadi Tren Terbaru Nonton Film. Diakses pada 23 September 2022, dari https://kumparan.com/millennial/mengenal-istilah-binge-watching-dan-hopping-yang-jadi-tren-terbaru-nonton-film-1wREvjSoXeB
- towardsdatascience.com. (2020, 2 Oktober). How to Build a Movie Recommendation System. Diakses pada 23 September 2022, dari https://towardsdatascience.com/how-to-build-a-movie-recommendation-system-67e321339109
- Wiputra, Michael M., and Yusup J. Shandi. "Perancangan Sistem Rekomendasi Menggunakan Metode Collaborative Filtering dengan Studi Kasus Perancangan Website Rekomendasi Film". *Media Informatika*, vol. 20, no. 1, 2021, pp. 1-18, doi:[10.37595/mediainfo.v20i1.54](https://dx.doi.org/10.37595/mediainfo.v20i1.54).
