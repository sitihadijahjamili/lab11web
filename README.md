# lab11web
Mengaktifkan dahulu Xampp Control Panel pada bagian Apache klik Config PHP.ini
![lab11  2](https://user-images.githubusercontent.com/56400200/122626883-daf4ff00-d0d6-11eb-9b88-29e2ef26c231.png)
![lab11  1](https://user-images.githubusercontent.com/56400200/122626749-47233300-d0d6-11eb-8454-339f31ecadca.PNG)
Pada bagian extention, hilangkan tanda ; (titik koma) pada ekstensi yang akan 
diaktifkan. Kemudian simpan kembali filenya dan restart Apache web server.
![lab11  3](https://user-images.githubusercontent.com/56400200/122626820-9e290800-d0d6-11eb-92d1-c90ab7c88090.PNG)
Unduh Codeigniter dari website https://codeigniter.com/download. Extrak file zip Codeigniter ke direktori htdocs/lab11_ci.Ubah nama direktory framework-4.x.xx menjadi ci4.
Buka browser dengan alamat http://localhost/lab11_ci/ci4/public
![lab11  4](https://user-images.githubusercontent.com/56400200/122627525-34126200-d0da-11eb-9353-956d49beac23.png)
Perintah yang dapat dijalankan untuk memanggil CLI Codeigniter adalah:
php spar seperti berikut ini
![lab11  5](https://user-images.githubusercontent.com/56400200/122627589-a71bd880-d0da-11eb-8127-c7e32e74593a.png)
![lab11  6](https://user-images.githubusercontent.com/56400200/122627745-adf71b00-d0db-11eb-9eb3-7ee6df38c08c.png)
![lab11  7](https://user-images.githubusercontent.com/56400200/122627781-fb738800-d0db-11eb-9d7d-e3240640ee5e.png)
![lab11  8](https://user-images.githubusercontent.com/56400200/122627801-252caf00-d0dc-11eb-8ae8-0c2fd53201dd.png)

Fokus kita pada folder app, dimana folder tersebut adalah area kerja kita untuk 
membuat aplikasi. Dan folder public untuk menyimpan aset web seperti css,gambar, javascript.
![spark](https://user-images.githubusercontent.com/56400200/122627947-33c79600-d0dd-11eb-9a16-2fcb2ba6c042.PNG)
![lab11  9](https://user-images.githubusercontent.com/56400200/122628169-d5031c00-d0de-11eb-913c-bdf673387a63.png)
Untuk mengetahui route yang ditambahkan sudah benar, buka CLI dan jalankan 
perintah berikut.php spark routes
![Lab11  10](https://user-images.githubusercontent.com/56400200/122628207-0e3b8c00-d0df-11eb-8113-e62a3b64a77f.png)
![lab11  11](https://user-images.githubusercontent.com/56400200/122628305-93bf3c00-d0df-11eb-82be-cee4c070e30b.png)
membuat Controller Page. Buat file baru dengan nama page.php pada direktori Controller kemudian isi kodenya seperti berikut.
![lab11  12 (2)](https://user-images.githubusercontent.com/56400200/122628335-bd786300-d0df-11eb-90ea-439eae63c772.png)
![lab11  13](https://user-images.githubusercontent.com/56400200/122628371-e6005d00-d0df-11eb-9024-d61dd96f8098.png)
![lab11  14](https://user-images.githubusercontent.com/56400200/122628469-55764c80-d0e0-11eb-89a9-6685b43921f3.png)
![lab11  15](https://user-images.githubusercontent.com/56400200/122628513-a5551380-d0e0-11eb-8383-85ff6ee1138b.png)
Buat file css pada direktori public dengan nama style.css (copy file dari praktikum 
lab4_layout.
![lab11  16](https://user-images.githubusercontent.com/56400200/122629463-68404f80-d0e7-11eb-9904-e9033127f909.png)
<img width="363" alt="lab11  17 (2)" src="https://user-images.githubusercontent.com/56400200/122629528-df75e380-d0e7-11eb-9650-923bd8424112.png">
<img width="466" alt="lab11  17  1" src="https://user-images.githubusercontent.com/56400200/122629624-9f633080-d0e8-11eb-8625-da20cf039ec6.png">
<img width="307" alt="lab11  18" src="https://user-images.githubusercontent.com/56400200/122629684-054fb800-d0e9-11eb-8552-400ca89f4cdc.png">
<img width="890" alt="lab11  19" src="https://user-images.githubusercontent.com/56400200/122629707-2dd7b200-d0e9-11eb-8c14-93aeeb6acb49.png">



Praktikum 12 - Lanjutan Codeigniter - Pemrograman Web

Langkah pertama yaitu aktifkan dahulu XAMPPnya
![lab12  1](https://user-images.githubusercontent.com/56400200/123498560-e8703300-d65a-11eb-8310-e251ecd8605f.PNG)

Kemudian Buat Database Dengan menamakan lab_ci4; selanjutnya membuat Tabel seperti berikut ini
![lab12  2](https://user-images.githubusercontent.com/56400200/123498644-7e0bc280-d65b-11eb-9bd2-65e7f7b534c0.PNG)
![lab12  3](https://user-images.githubusercontent.com/56400200/123498858-9203f400-d65c-11eb-87b2-3a3d16ce681a.PNG)

Selanjutnya Konfigurasi koneksi database
Selanjutnya membuat konfigurasi untuk menghubungkan dengan database server. 
Konfigurasi dapat dilakukan dengan du acara, yaitu pada file app/config/database.php
atau menggunakan file .env. Pada praktikum ini kita gunakan konfigurasi pada file .env. 
![lab12  4](https://user-images.githubusercontent.com/56400200/123498887-d55e6280-d65c-11eb-964e-50afccbf6a0b.PNG)

Membuat Model
Selanjutnya adalah membuat Model untuk memproses data Artikel. Buat file nama ArtikelModel.php
![lab12  5](https://user-images.githubusercontent.com/56400200/123498967-6cc3b580-d65d-11eb-9bfa-156fa66ce8fc.PNG)

Buat Controller baru dengan nama Artikel.php pada direktori app/Controllers.
![lab12  6](https://user-images.githubusercontent.com/56400200/123498993-bad8b900-d65d-11eb-8ed6-fdc85e1d32f2.PNG)

Membuat View dengan nama artikel pada direktori app/views, kemudian buat file 
baru dengan nama index.php.
![lab12  7](https://user-images.githubusercontent.com/56400200/123499037-fffceb00-d65d-11eb-8a78-508a7055cffb.PNG)
Selanjutnya buka browser kembali, dengan mengakses url http://localhost:8080/artikel
![lab12  7(1)](https://user-images.githubusercontent.com/56400200/123499063-29b61200-d65e-11eb-942f-727dd7461861.png)

INSERT INTO artikel (judul, isi, slug) VALUE
('Artikel pertama', 'Lorem Ipsum adalah contoh teks atau dummy dalam industri 
percetakan dan penataan huruf atau typesetting. Lorem Ipsum telah menjadi 
standar contoh teks sejak tahun 1500an, saat seorang tukang cetak yang tidak 
dikenal mengambil sebuah kumpulan teks dan mengacaknya untuk menjadi sebuah 
buku contoh huruf.', 'artikel-pertama'), 
('Artikel kedua', 'Tidak seperti anggapan banyak orang, Lorem Ipsum bukanlah 
teks-teks yang diacak. Ia berakar dari sebuah naskah sastra latin klasik dari 
era 45 sebelum masehi, hingga bisa dipastikan usianya telah mencapai lebih 
dari 2000 tahun.', 'artikel-kedua');

![lab12  8](https://user-images.githubusercontent.com/56400200/123499243-8534cf80-d65f-11eb-901a-461815e8bccc.PNG)
![lab12  8(1)](https://user-images.githubusercontent.com/56400200/123499261-ad243300-d65f-11eb-8690-da25effdd9d0.png)

![lab12  9](https://user-images.githubusercontent.com/56400200/123499299-f96f7300-d65f-11eb-9dd6-e46bd78bd0e9.PNG)
![lab12  10](https://user-images.githubusercontent.com/56400200/123499676-9c28f100-d662-11eb-88ee-a9c7c1f00e4f.PNG)
![lab12  10 ke 2](https://user-images.githubusercontent.com/56400200/123499700-cc708f80-d662-11eb-9761-4172a500567f.png)




















