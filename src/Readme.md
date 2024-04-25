# Capstone Project Module 2 - Analisis Harga Sewa Properti Airbnb

<p align="center">
  <img src="..\docs\gambar landscape airbnb.jpg" alt="Header" width="800" height="400">
</p>

## Context
Airbnb memainkan peran penting dalam penyewaan properti di Bangkok dengan harga dipengaruhi oleh lokasi, jenis akomodasi, dan fasilitas. Faktor-faktor seperti lokasi strategis dan jenis properti menentukan harga sewa. Analisis data membantu pemilik dan pengguna mengoptimalkan pengalaman dan strategi harga, meningkatkan potensi penghasilan dan kepuasan pelanggan.

## Problem Statement
Penelitian ini bertujuan untuk memberikan informasi terkait apa saja yang mempengaruhi harga sewa properti yang ada di platform Airbnb yang ada di Bangkok, Thailand.

## Data
Menggunakan dataset `Airbnb Listings Bangkok.csv` bulan April 2023. [Download di sini](https://drive.google.com/drive/folders/1A_KBMRFTS5Mthpp46nulso679ML4ZwTF)

**Deskripsi Kolom**:

| Kolom                              | Deskripsi                                                                                            |
|------------------------------------|------------------------------------------------------------------------------------------------------|
| id                                 | ID unik untuk setiap pendaftaran properti                                                            |
| name                               | Deskripsi nama dari setiap properti yang tersedia                                                    |
| host_id                            | ID unik untuk setiap tuan rumah                                                                      |
| host_name                          | Nama dari tiap tuan rumah, umumnya hanya nama depan                                                  |
| neighbourhood                      | Nama distrik di Kota Bangkok                                                                         |
| latitude                           | Titik garis lintang untuk lokasi proyeksi                                                            |
| longitude                          | Titik garis bujur untuk lokasi proyeksi                                                              |
| room_type                          | Jenis ruangan yang tersedia (seluruh rumah/apartemen, kamar pribadi, kamar bersama, dan hotel)       |
| price                              | Harga sewa harian dalam mata uang lokal                                                              |
| minimum_nights                     | Jumlah minimum malam yang harus dipesan                                                               |
| number_of_reviews                  | Jumlah ulasan yang diterima oleh setiap pendaftaran                                                  |
| last_review                        | Tanggal ulasan terakhir                                                                              |
| reviews_per_month                  | Rata-rata jumlah ulasan per bulan                                                                    |
| calculated_host_listings_count     | Jumlah pendaftaran yang dimiliki oleh tuan rumah dalam wilayah geografis tertentu                    |
| availability_365                   | Ketersediaan pendaftaran dalam 365 hari ke depan                                                     |
| number_of_reviews_ltm              | Jumlah ulasan dalam 12 bulan terakhir                                                                |
| city_zone                          | Pengelompokkan distrik yang ada di Bangkok. Meliputi inner zone, middle zone, dan outer zone.       |


## Analisis
Lihat file ipynb & ppt.

## Kesimpulan
1. **Variabel Kategorikal (`room_type` dan `neighbourhood`)**:
   - **Room Type**: Ada perbedaan harga yang signifikan antara berbagai tipe kamar di kedua dataset (reguler dan premium), dengan p-value yang sangat kecil, menunjukkan kepercayaan yang tinggi dalam hasil ini. Hal ini menunjukkan bahwa tipe kamar adalah faktor penting dalam menentukan harga.
   - **Neighbourhood**: Sama seperti tipe kamar, lokasi atau neighbourhood juga menunjukkan perbedaan yang signifikan dalam harga di kedua dataset. Ini menunjukkan bahwa lokasi adalah salah satu faktor utama yang mempengaruhi harga sewa.

2. **Pengaruh Variabel Numerik**:
   - Analisis korelasi Spearman menunjukkan bahwa hubungan antara variabel numerik (seperti `number_of_reviews`, `availability_365`, dan lainnya) dengan harga cenderung lemah. Ini menunjukkan bahwa sementara faktor-faktor ini mungkin memiliki beberapa pengaruh, mereka tidak sekuat pengaruh tipe kamar dan lokasi.Pembayaran.

## Rekomendasi
- **Penyesuaian Harga Berdasarkan Tipe Kamar dan Lokasi**: Mengingat bahwa tipe kamar dan lokasi sangat mempengaruhi harga, pengelola properti harus menyesuaikan harga sewa berdasarkan faktor-faktor ini untuk memaksimalkan pendapatan. Menawarkan harga yang kompetitif untuk tipe kamar yang sama di lokasi serupa dapat membantu meningkatkan okupansi.
- **Investasi Berdasarkan Lokasi**: Dalam memilih properti untuk investasi atau pengembangan lebih lanjut, pertimbangkan lokasi sebagai faktor utama. Neighbourhood yang menunjukkan harga sewa lebih tinggi bisa menjadi target investasi yang menarik.

#### Untuk Pembuat Kebijakan atau Peneliti:
- **Pengembangan Infrastruktur dan Layanan**: Mengingat pengaruh signifikan lokasi terhadap harga sewa, pembuat kebijakan lokal dapat fokus pada peningkatan infrastruktur dan layanan di neighbourhood yang lebih rendah harganya untuk meningkatkan daya tarik dan mungkin kesetaraan harga sewa.
- **Analisis Lebih Lanjut pada Faktor Lingkungan**: Melakukan studi lebih lanjut mengenai bagaimana berbagai faktor lingkungan (seperti keamanan, kebersihan, akses ke transportasi) mempengaruhi harga sewa dapat membantu dalam perencanaan kebijakan yang lebih efektif.

#### Untuk Pengguna atau Wisatawan:
- **Pilihan Berdasarkan Budget**: Wisatawan dan pengguna Airbnb dapat menggunakan informasi ini untuk membuat keputusan yang lebih baik dalam memilih akomodasi yang sesuai dengan budget mereka, dengan mempertimbangkan betapa signifikannya perbedaan harga antara berbagai tipe kamar dan lokasi.

[**Dashboard**](https://public.tableau.com/app/profile/arya.gamaseka/viz/AnalisisHargaSewaAirbnb/Dashboard1#1)