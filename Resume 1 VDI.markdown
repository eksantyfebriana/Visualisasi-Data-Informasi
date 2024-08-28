# RESUME ARTIKEL

```{=html}
Judul Artikel     = Making data visualization more efficient and effective: a survey
Jurnal            = The VLDB Journal
Volume & Halaman  = Vol. 29, halaman 93-117
Tahun             = 2020
Penulis           = Xuedi Qin, Yuyu Luo & Guoliang Li
Riviewer          = Eksanty F Sugma Islamiaty (122450001)
Tanggal           = 27 Agustus 2024
```
## **Latar Belakang**

Visualisasi data sangat penting dalam dunia bisnis berbasis data pada
saat ini, yang telah digunakan secara luas untuk membantu pengambilan
keputusan yang berkaitan erat dengan pendapatan utama banyak perusahaan
industri. Namun, karena tingginya permintaan pemrosesan data terkait
volume, kecepatan, dan kebenaran data, terdapat kebutuhan mendesak akan
ahli database untuk membantu melakukan visualisasi data yang efisien dan
efektif. Menanggapi permintaan ini, artikel ini mensurvei teknik-teknik
yang membuat visualisasi data menjadi lebih efisien dan efektif.

1.  *Spesifikasi visualisasi* mendefinisikan bagaimana pengguna dapat
    menentukan kebutuhan mereka untuk menghasilkan visualisasi
2.  *Pendekatan yang efisien untuk visualisasi data* memproses data dan
    spesifikasi visualisasi yang diberikan, kemudian menghasilkan
    visualisasi dengan target utama untuk menjadi efisien dan terukur
    dengan kecepatan interaktif.
3.  *Visualisasi data rekomendasi* untuk melengkapi spesifikasi yang
    tidak lengkap secara otomatis, atau untuk menemukan visualisasi yang
    lebih menarik berdasarkan visualisasi acuan.

## **Tujuan**

1.  Untuk mengenal lebih dalam tentang visualisasi data dan informasi
2.  Untuk mengetahui alat (*tools*) yang digunakan dalam
    memvisualisasikan data dan informasi
3.  Untuk memberikan pemahaman lebih terkait cara membuat visualisasi
    data dan informasi yang lebih akurat, mudah dipahami, dan efisien



## **Metodologi**

Metodologi penelitian yang digunakan adalah deskriptif kualitatif. Hal
ini karena data yang dikumpulkan berupa kata-kata, gambar, dan bukan
angka (angka digunakan hanya pada contoh kasus). Peneliti melakukan
tinjauan komprehensif melalui survei dengan cara *sintesis* yaitu
merangkum temuan-temuan utama dari setiap penelitian dan
mengidentifikasi tren, juga kesenjangan, dan *perbandingan* yaitu
membandingkan berbagai pendekatan yang berbeda untuk mengatasi masalah
yang sama dalam visualisasi data.

## **Hasil**

#### **1. Berkembangnya Cara Untuk Memvisualisasikan Data**

> Visualisasi data merupakan cara yang ampuh untuk menyajikan data
> secara menarik yang mudah direpresentasikan oleh ilmuwan data dan
> mudah dipahami oleh siapapun. Visualisasi data dapat memberikan
> gambaran umum untuk data kecil maupun data besar sekalipun, terlebih
> di masa kini data lebih banyak daripada sebelumya.

> Visualisasi data dapat dibuat diberbagai macam aplikasi seperti Excel,
> Google Sheet, Oracle, IBM DB2, Amazon Quicksight, Microsoft Power BI,
> dan lain-lain. Langkah umum dalam memvisualisasikan data adalah dengan
> mengimpor data, persiapan data (menormalkan nilai atau mengoreksi),
> manipulasi data (filtering / joining / grouping), pemetaan, dan
> merepresentasikannya. Dua langkah umum terakhir haruslah efisien dan
> terukur.

> Penggunaan visualisasi haruslah tepat dan sesuai dengan yang
> diinginkan para pengguna oleh karena itu sistem visualisasi biasanya
> memberikan rekomendasi yang secara otomatis melengkapi visualisasi
> agar hasil yang didapatkan tidak ambigu.

#### **2. Spesifikasi Visualisasi**

> Bahasa Visualisasi terdiri dari tiga bagian berdasarkan
> ekspresifitasnya yaitu (1) data, (2) tanda atau isyarat visual, dan
> (3) pemetaan atau pemberian tanda yang sesuai. Semakin rendah level
> sebuah bahasa maka semakin ekspresif pula artinya pengguna harus
> menentukan fungsi pemetaan. Kebalikannya, semakin tinggi level bahasa
> maka semakin mudah untuk digunakan yaitu hanya perlu menambahkan jenis
> tanda. Tiga contoh bahasa tingkat tinggi yaitu (1) ggplot2 dalam
> bahasa R, (2) Altair untuk komunitas python, (3) Echarts pembuatan
> visualisasi yang mudah bagi para non-programmer.

> Dalam proses visualisasi pengguna harus terus menyempurnakan hasil
> visualisasi dengan menambahkan / menghapus / mengubah atribut maupun
> jenis grafik agar hasilnya lebih akurat. **Penyempurnaan kueri
> bertahap** dapat dilakukan pada *Polaris* juga *Tableau* menghasilkan
> grafik multidimensi. **Navigasi Facet** dapat dilakukan pada *DeepEye*
> dengan mencari rekomendasi lewat kata kunci.

> Alat interaktif berbasis GUI biasanya digunakan untuk membuat
> prototipe dengan cepat atau untuk menemukan visualisasi yang berguna.
> Sedangkan bahasa tingkat rendah akan digunakan untuk penyetelan halus
> atau implementasi ulang visualisasi yang diinginkan. Perihal
> spesifikasi yang tidak lengkap dapat menggunakan petunjuk berdasarkan
> referensi, berdasarkan kata kunci, dan berdasarkan bahasa natural yang
> menyediakan antarmuka visual seperti pada *Evizeon*.

#### **3. Pendekatan Yang Efisien Untuk Visualisasi Data**

> **Visualisasi data eksak** bisa dilakukan karena menerjemahkan kueri
> secara natural memiliki banyak kelemahan seperti banyak fungsionalitas
> yang diulang, dan metode yang tidak terhubung dan sulit dipelihara,
> diperluas, dan dioptimalkan sehingga dibutuhkan Sistem Manajemen
> Visualisasi Data (DVMS) yang menggunakan fitur visualisasi untuk
> mendukung interaksi menggunakan estimasi visualisasi, rekomendasi, dan
> sebagainya.

> **Penempatan Kolom** penting untuk tata letak data dapat menimbulkan
> perbedaan hasil visualisasi yang besar karena dalam beberapa kasus
> pengguna hanya tertarik pada kolom-kolom tertentu saja.

> **Indeks** digunakan untuk meminimalkan waktu pencarian berdasarkan
> letak.

> **Komputasi Paralel** pada imMens memparalelkan kueri agregasi dengan
> menggunakan representasi indeks padat.

> **Prediksi dan Prefetching** dengan cara eksplorasi data dan juga
> menggunakan data historis dengan memilih arah, fokus, juga vektor.

> **Pendekatan Berbasis Machine Learning** menggunakan model Support
> Vector Machine (SVM) da strategi berbasis aksi dengan Markov chain.

> **Berbasis AQP** dapat menghasilkan visualisasi dengan aproksimasi
> yang cepat namun tingkat keakuratannya sangat kecil sehingga
> terciptalah *Pangloss* yang dapat menghasilkan aproksimasi cepat dan
> lebih akurat.

> **Berbasis Pengambilan Sampel Inkremental** yang dapat
> menghasilkan visualisasi aproksimasi dari kumpulan data dengan cepat
> dan sistem terus mempebarui visualisasi sehingga kualitas visualiasi
> terus meningkat.

> **Berbasis Presepsi Manusia** pendekatan ini dapat menghentikan
> pengambilan sampel ketika tidak ada perbedaan yang jelas, namun
> kekurangannya adalah keterbatasan kognitif persepsi manusia dalam
> mengidentifikasi.

#### **4. Rekomendasi Visualisasi**

> **Spesifikasi Tidak Lengkap** : Visualisasi yang tepat digunakan dalam
> berbagai macam masalah adalah dengan mempertimbangkan beberapa faktor,
> mengubah data, memilih visual yang tepat (batang, garis, atau titik)
> dan jenis nya (lebar batang atau posisi titik).Setelah
> mempertimbangkannya, pengguna dapat membuang bagian yang tidak
> diperlukan dengan cara meentukan batasan, menentukan kueri, menentukan
> variabel, batasan dari ahli, dan lain-lain. Pengguna harus pandai
> memilah dan memilih bentuk visualisasi, seperti hal nya orang mungkin
> menggunakan grafik garis untuk memvisualisasikan deret waktu dalam
> sebagian besar kasus, namun terkadang dalam beberapa kasus grafik
> scatter adalah pilihan yang terbaik, karena grafik scatter memberikan
> tren yang lebih jelas daripada grafik garis ketika ada banyak outlier
> dalam deret waktu. Keuntungannya sangat membantu pengguna untuk dengan
> cepat mengeksplorasi data ketika pengguna tidak terlalu familiar
> dengan data dan visualisasi yang diinginkan.

> **Spesifikasi Berbasis Referensi**: Biasanya sistem akan
> merekomendasikan visualisasi yang mirip atau malah berbeda dengan
> referensi yang diberikan oleh pengguna. Hal ini dapat dilakukan dengan
> cara *berbasis deviasi* berupa menentukan kueri yang diminati dalam
> medapatkan data terget, lalu dihitug kombinasi yang berbedanya
> sehingga rekomendasi muncul dari nilai terbesar. Adapun *berbasis
> anomali* seperti halnya *Profiler* merekomendasikan visualisasi yang
> membedakan anomali terbaik dalam visualisasi utamanya. Terakhir
> berbasis kesamaan / jarak seeprti pada *Zenvisage* dengan memberikan
> tren, pola, atau wawasan yang diinginkan.

> **Rekomendasi Berbasis Perilaku** : membutuhkan input pengguna atas
> hal yang diinginkan sehingga sistem dapat memunculkan rekomendasi
> visualisasi.

> **Rekomendasi Yang Dipersonalisasi** : mempertimbangkan histori dari
> penggunanya.

#### **5. Arah Penelitian Lainnya**

> Data yang akan divisualkan harus dibersihkan untuk menormalisasi
> nilai, deduplikasi, menghapus nilai yang hilang, dan deteksi outlier.
> Pentingnya mendeteksi visualisasi yang bias, dan pembersihan data yang
> sesuai agar hasil visualisasi lebih akurat dan efisien waktu
> pengerjaannya. Peneliti mengingkan agar pengguna lebih teliti.

> Visualisasi data untuk aplikasi terkait database sudah banyak ada,
> misalnya seperti Excel, Google Sheets, dan lain-lain. Visualisasi data
> dalam hal ini dapat menimbulkan debugging data karena alur kerja
> analisis data yang salah diinputkan. Peneliti menginginkan ada yang
> mampu mengembangkan tentang permasalahan ini

## **Kesimpulan**

Visualisasi data adalah bidang yang berkembang pesat dengan banyak hasil
penelitian baru dan sistem baru yang dikembangkan. Penelitian dan
praktisi dari banyak bidang telah berkontribusi pada keberhasilan luar
biasa dari visualisasi data, yang didorong oleh sebagian besar (jika
tidak semua) domain dan aplikasi.

Artikel ini terutama membahas karya visualisasi data terbaru, dari
perspektif manajemen data. Secara khusus, penenliti telah secara
komprehensif menggambarkan karya-karya dalam spesifikasi visualisasi,
metode efisien untuk visualisasi data, dan rekomendasi visualisasi.
Seperti disebutkan sebelumnya, sebagian besar sistem visualisasi data
komersial sangat baik dalam kemudahan penggunaan dalam hal spesifikasi
visualisasi data. Namun, banyak praktisi masih menderita masalah
efisiensi dan rekomendasi dari sistem ini. Oleh karena itu, peneliti
juga membahas beberapa masalah terbuka yang dapat dikontribusikan oleh
peneliti database untuk memajukan bidang visualisasi data.

## **Kelebihan**

1.  Penjelasan sangat detail, dengan mendeskripsikan langsung uji coba
    pada *tools* yang berbeda
2.  mempunyai landasan teori yang sesuai fakta terlihat dari
    kutipan-kutipannya
3.  Terdapat rincian perbedaan pada masing-masing *tools* sehingga para
    pengguna dapat mempertimbangkan untuk memilih *tools* yang sesuai
    kebutuhannya
4.  Mampu membandingkan dari teori-teori yang telah ada sebelumya
5.  Peneliti memberikan saran atau rekomendasi untuk penelitian
    selanjutnya
6.  Visualisasi yang mendukung dengan informasi yang kompleks
7.  Topik yang diangkat sangat relavan karena perkembangan data yang
    semakin luas dan implementasinya dalam berbagai bidang

## **Kekurangan**

1.  Pemilihan kata yang sangat susah untuk para pemula yang akan mencoba
    visualisasi
2.  Topik yang dibahas tidak terlalu spesifik
3.  Terlalu banyak yang dibahas, sehingga topik utama tidak terlalu
    dalam dibahas
4.  Tidak ada rekomendasi pasti *tools* atau *bahasa* apa yang paling
    tepat atau fitur yang paling lengkapnya.
