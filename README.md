# Tugas Praktikum { Pertemuan ke 6 } <img src=https://qph.fs.quoracdn.net/main-qimg-648763cc041459725b62108f4fdf5b91 width="110px" >
|Nama|NIM|Kelas|Matkul|
|----|---|-----|------|
|WIORETA VEBRA AZHARI LEANDER|312310567|TI.23.A5|Basis Data|

# Soal Latihan Praktikum
## 1. Tulis semua perintah-perintah SQL percobaan di atas beserta outputnya!

1. Buat sebuah database dengan nama latihan2

Untuk membuat database gunakan perintah sebagai berikut :

CREATE DATABASE [nama_database]

CREATE DATABASE latihan2;

lalu, setelah kita membuat database. kita masuk kedalam database tersebut dengan perintah sebagai berikut :

USE latihan2;

![Cuplikan layar 2024-04-24 144527](https://github.com/crslouis/pertemuan6/assets/147572011/2246f0d3-c623-4bc5-8481-49aca27e3fba)


2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan2!

Untuk membuat Tabel gunakan perintah sebagai berikut :

`CREATE TABLE nama_tabel (
    nama_field1 tipe _data(ukuran), nama_field2 tipe_data(ukuran), ..., nama_fieldn tipe_data(ukuran)
    );`

`CREATE TABLE biodata (
    nama varchar (100),
    alamat text
    );`

![Cuplikan layar 2024-04-24 144701](https://github.com/crslouis/pertemuan6/assets/147572011/1c3e3639-8506-4862-a4b7-2ee96bfef74a)


3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom terakhir!

Contoh :

ALTER TABLE biodata ADD COLUMN keterangan VARCHAR (15);

![Cuplikan layar 2024-04-24 144724](https://github.com/crslouis/pertemuan6/assets/147572011/0c24097d-9c0e-4082-aa65-61ff6c2544df)


4.Tambahkan kolom id(int 11) di awal (sebagai kolom pertama)!

Untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut :

`ALTER TABLE biodata ADD COLUMN id int FIRST; `

![Cuplikan layar 2024-04-24 144737](https://github.com/crslouis/pertemuan6/assets/147572011/3f056fb7-c6ab-464d-932b-a95ec3112a04)


5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!

Untuk menambahkan kolom setelah kolom lain yaitu dengan perintah AFTER

![Cuplikan layar 2024-04-24 144752](https://github.com/crslouis/pertemuan6/assets/147572011/92b5e4ff-fa2d-4e88-b327-4441ffd13c95)


6. Ubah tipe data kolom id menjadi char(11)!

Untuk mengubah type data yaitu dengan perintah sebagai berikut :

ALTER TABLE [nama_tabel] MODIFY nama_field tipe_data_baru(ukuran);

![Cuplikan layar 2024-04-24 145002](https://github.com/crslouis/pertemuan6/assets/147572011/dde7713b-d5c4-48fb-b52a-3e962dfe528d)


7. Ubah nama kolom phone menjadi hp (char 20)!

Untuk mengubah kolom yaitu dengan perintah sebgai berikut :

ALTER TABLE [nama_tabel] CHANGE nama_field_lama nama_field_baru tipe_data(ukuran);

![alt text](ss/4.1.png)

8. Tambahkan kolom email setelah kolom hp

![alt text](ss/4.2.png)

9. Hapus kolom keterangan dari tabel!

Untuk menghapus kolom dari tabel yaitu dengan perintah sebagai berikut :

ALTER TABLE [nama_tabel] DROP nama_field;

![alt text](ss/5.1.png)

10. Ganti nama tabel menjadi data_mahasiswa!

Untuk mengganti nama tabel yaitu dengan perintah sebagai berikut :

ALTER TABLE [nama_tabel] RENAME [nama_tabel_baru];

![alt text](ss/5.2.png)

11. Ganti nama field id menjadi nim!

![alt text](ss/6.1.png)

12. Jadikan nim sebagai PRIMARY KEY!

Untuk menambahkan index atau key, gunakan perintah sebagai berikut :

tipe index :

- PRIMARY KEY
- UNIQUE KEY
- FULLTEXT

ALTER TABLE [nama_tabel] ADD [INDEX|PRIMARY KEY] (nama_field);

![Cuplikan layar 2024-04-24 145012](https://github.com/crslouis/pertemuan6/assets/147572011/d8bbf3dd-0b90-4c52-bee5-f043b0837662)


13. Jadikan kolom email sebagai UNIQUE KEY!

Perintah nya sama seperti diatas, hanya saja diganti menjadi UNIQUE KEY

![Cuplikan layar 2024-04-24 145030](https://github.com/crslouis/pertemuan6/assets/147572011/0440d1b9-1868-43fa-b0a5-0f4e2f7799aa)



## 2. Apa Maksud Dari INT(11) ?

- INT(11) Adalah Nama Tipe Datanya Yaitu Integer dan Memiliki Panjang 11 Karakter.

## 3. Ketika Kita Melihat Struktur Tabel Dengan Perintah DESC , Ada Kolom Null yang Berisi Yes dan No. Apa Maksudnya ?

- Yaitu Untuk Menjelaskan Bahwa Pada Record yg NO Harus diisi , Sedangkan YES Boleh Tidak diisi.


### Sekian Tugas Praktikum Saya di Pertemuan kali ini, Jika Masih Ada Yang Salah Saya Mohon Maaf.
