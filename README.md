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




# PRAKTIKUM 12 - Lanjutan Codeigniter - Pemrograman Web

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

Membuat Tampilan Detail Artikel
![lab12  9](https://user-images.githubusercontent.com/56400200/123499299-f96f7300-d65f-11eb-9dd6-e46bd78bd0e9.PNG)

Membuat View Detail
Buat view baru untuk halaman detail dengan nama app/views/artikel/detail.php.
![lab12  10](https://user-images.githubusercontent.com/56400200/123499676-9c28f100-d662-11eb-88ee-a9c7c1f00e4f.PNG)
Membuat Routing untuk artikel detail

Buka Kembali file app/config/Routes.php, kemudian tambahkan routing untuk artikel 
detail.
![lab12  10 ke 2](https://user-images.githubusercontent.com/56400200/123499700-cc708f80-d662-11eb-9761-4172a500567f.png)
![lab12  10(1)](https://user-images.githubusercontent.com/56400200/123499720-f1650280-d662-11eb-83bf-4fdc6b2957e1.png)

Membuat Tampilan Detail Artikel
![lab12  11](https://user-images.githubusercontent.com/56400200/123499852-cb8c2d80-d663-11eb-8383-f449e4796a3d.PNG)
Membuat View Detail
Buat view baru untuk halaman detail dengan nama app/views/artikel/detail.php.
![lab12  11 ke 2](https://user-images.githubusercontent.com/56400200/123499880-05f5ca80-d664-11eb-8e2c-e9b7d3368e75.PNG)
![lab12  11 ke 3](https://user-images.githubusercontent.com/56400200/123499911-30478800-d664-11eb-97c3-7e7edbf73a51.PNG)
![lab12  11 ke 4](https://user-images.githubusercontent.com/56400200/123502077-aacbd400-d673-11eb-8f62-27e482198179.png)
![lab12  11(1)](https://user-images.githubusercontent.com/56400200/123502038-70623700-d673-11eb-8976-8b534da619a0.PNG)

![lab12  12](https://user-images.githubusercontent.com/56400200/123502142-1746d300-d674-11eb-9be9-3c223fdc5543.PNG)
![lab12  12 ke 2](https://user-images.githubusercontent.com/56400200/123502249-20846f80-d675-11eb-9f9c-0d0c23c3d304.PNG)
![lab12  12(1)](https://user-images.githubusercontent.com/56400200/123502285-70fbcd00-d675-11eb-97ce-b3865fa8eec9.PNG)

![lab12 naw](https://user-images.githubusercontent.com/56400200/123503016-760f4b00-d67a-11eb-8838-ab8694dd83ff.PNG)
Kemudian buat view untuk form tambah dengan nama form_edit.php
![lab12  13](https://user-images.githubusercontent.com/56400200/123502572-a9040f80-d677-11eb-9a3d-a1e7ef041b93.PNG)
![lab12  13(1)](https://user-images.githubusercontent.com/56400200/123502004-195c6200-d673-11eb-94ab-2143c345fe8a.PNG)
Menghapus Data
Tambahkan fungsi/method baru pada Controller Artikel dengan nama delete(). 
![lab12  14](https://user-images.githubusercontent.com/56400200/123502651-2e87bf80-d678-11eb-86b5-166a04810752.PNG)




# PRAKTIKUM 13 Lanjutan 

Membuat Tabel User
![lab13  1 ke 2](https://user-images.githubusercontent.com/56400200/124339373-edede180-db62-11eb-93b0-0f2cc89c2fbc.PNG)

Kemudian Membuart file baru dengan nama UserModel.php
![lab13  2](https://user-images.githubusercontent.com/56400200/124339425-5210a580-db63-11eb-933d-4547849c7632.PNG)

Selanjutnya membuat User.php
![lab13  3](https://user-images.githubusercontent.com/56400200/124339495-b0d61f00-db63-11eb-857f-c4cd1c7ae057.PNG)
![lab13  3 ke 2](https://user-images.githubusercontent.com/56400200/124339516-da8f4600-db63-11eb-99ee-53b7e2bc773a.PNG)

Membuat file baru dengan nama Login.php 
![lab13  4](https://user-images.githubusercontent.com/56400200/124339568-41146400-db64-11eb-9cc4-00091ae817ce.PNG)

UserSeeder.php
![lab13  5](https://user-images.githubusercontent.com/56400200/124339619-9486b200-db64-11eb-87bb-ac4251d25b57.PNG)
![lab13  5(1)](https://user-images.githubusercontent.com/56400200/124339661-d283d600-db64-11eb-91d2-463c16e1c588.PNG)

Selanjutnya membuat filer untuk halaman admin. Buat file baru dengan nama Auth.php
![lab13  6](https://user-images.githubusercontent.com/56400200/124339700-15de4480-db65-11eb-863e-09df0164fa4a.PNG)

Selanjutnya buka file app/Config/Filters.php tambahkan kode berikut:
![lab13  7](https://user-images.githubusercontent.com/56400200/124339807-c4828500-db65-11eb-9524-1235d8bebb63.PNG)

Selanjutnya buka file app/Config/Routes.php dan sesuaikan kodenya.
![lab13  7 ke 2](https://user-images.githubusercontent.com/56400200/124339844-fdbaf500-db65-11eb-9d8e-9655363630c0.PNG)

Buka url dengan alamat http://localhost:8080/admin/artikel ketika alamat tersebut 
diakses maka, akan dimuculkan halaman login. 
![lab13  7(1)](https://user-images.githubusercontent.com/56400200/124339888-3fe43680-db66-11eb-89f6-038f69d9cdb7.PNG)

Fungsi Logout
Tambahkan method logout pada Controller User seperti berikut:

![lab13  8](https://user-images.githubusercontent.com/56400200/124339921-73bf5c00-db66-11eb-9573-2ced753bb442.png)

![labb13  9](https://user-images.githubusercontent.com/56400200/124340029-25f72380-db67-11eb-9412-2cbb416e4786.PNG)



# Praktikum 14 

Untuk membuat pagination, buka Kembali Controller Artikel, kemudian modifikasi 
kode pada method admin_index
![Lab14  1](https://user-images.githubusercontent.com/56400200/125151234-3f194a80-e0fa-11eb-9576-0783bd4f6302.PNG)

Kemudian buka file views/artikel/admin_index.php dan tambahkan kode berikut
dibawah deklarasi tabel data.
![lab14  2](https://user-images.githubusercontent.com/56400200/125151424-dc747e80-e0fa-11eb-962b-4d99f2fbb950.PNG)

Kemudian buka file admin.css di folder public lalu tambahkan kode berikut untuk mempercantik tampilan pagination
![lab14  3](https://user-images.githubusercontent.com/56400200/125151461-252c3780-e0fb-11eb-96d9-081261790ccb.PNG)
![lab14  3(1)](https://user-images.githubusercontent.com/56400200/125151522-9f5cbc00-e0fb-11eb-935f-77cf94cbce75.PNG)

Untuk membuat pencarian data, buka kembali Controller Artikel, pada method 
admin_index
![lab14  4](https://user-images.githubusercontent.com/56400200/125151578-f2367380-e0fb-11eb-8683-242b29e0736c.PNG)

Kemudian buka kembali file views/artikel/admin_index.php dan tambahkan form 
pencarian sebelum deklarasi tabel 
![lab14  5](https://user-images.githubusercontent.com/56400200/125151618-43defe00-e0fc-11eb-8441-ba2838b6f397.PNG)

pada link pager ubah seperti berikut.

![lab14  6](https://user-images.githubusercontent.com/56400200/125151726-04fd7800-e0fd-11eb-845c-ac2ee7084e78.PNG)

![lab14  7](https://user-images.githubusercontent.com/56400200/125151751-45f58c80-e0fd-11eb-9262-e4d681578076.PNG)
![lab14  7(1)](https://user-images.githubusercontent.com/56400200/125151782-7d643900-e0fd-11eb-85a8-aefb85ba972c.PNG)

![lab14  8](https://user-images.githubusercontent.com/56400200/125151843-024f5280-e0fe-11eb-922e-f82c8d9721c2.PNG)

Kemudian pada file views/artikel/form_add.php tambahkan field input file seperti 
berikut.
![lab14  9](https://user-images.githubusercontent.com/56400200/125151921-7db10400-e0fe-11eb-8e51-9de2779d9634.PNG)

![lab14  10](https://user-images.githubusercontent.com/56400200/125151961-c49ef980-e0fe-11eb-82c9-3e4648b2aa16.PNG)
![lab14  10(1)](https://user-images.githubusercontent.com/56400200/125152197-f1074580-e0ff-11eb-9f93-887ddb6e1a86.PNG)




































































