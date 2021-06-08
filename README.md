# Praktikum 9 : PHP Modular

Pada praktikum 9 ini, kita akan membahas mengenai PHP Modular.

## Pengertian PHP Modular

 - **PHP Modular** atau disebut dengan **modularisasi** merupakan penyusunan atau pembuatan program berdasarkan modul-modul.
 - Setiap modul dikembangkan untuk tujuan atau fungsi khusus. Modul dibuat secara general (umum). Modul dapat berupa fungsi atau prosedur.
 - Modularisasi dalam pemrograman umum dilakukan dan sangat diperlukan untuk mempermudah debugging dan pengembangan program.

## Jenis Modularisasi 

Jenis modularisasi di dalam PHP antara lain:

#### 1. `require()`

 - Bentuk modular yang digunakan untuk menggabungkan suatu script PHP atau teks dari file lain dengan script PHP yang memanggilnya, file yang digabungkan tidak harus script PHP.
 - Teknik *require* sangat berguna untuk membuat template (pola) yang memudahkan proses pengembangan aplikasi dengan menggunakan pola tampilan.

#### 2. `include()`

 - Hampir sama dengan `require()`, akan tetapi `include()` digunakan untuk menggabungkan suatu script atau file dengan script pemanggilnya.
 - `include()` dapat digunakan dalam struktur pengulangan, untuk melakukan pemanggilan file-file yang berbeda.

#### 3. `require_once()`

Pada dasarnya sama dengan `require()`, akan tetapi di dalam `require_once()` duplikasi fungsi atau duplikasi pemanggilan dapat dihindari, karena secara *default* `require_once()` akan memaksa PHP untuk menggunakan nama fungsi atau pemanggilan yang telah ada.

#### 4. `include_once()`

Hampir sama dengan `require_once()`, akan tetapi pada `include_once()` setiap kali dijalankan akan selalu ada evaluasi ulang.

## Contoh Modularisasi

#### header.php

Pertama kita membuat sebuah file baru dengan nama `header.php`, dengan kode program sebagai berikut.

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/header.PNG)

Dan hasilnya seperti berikut.

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ss_header.PNG)

#### footer.php

Selanjutnya, membuat file `footer.php`

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/footer.PNG)

**Hasilnya**

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ss_footer.PNG)

#### home.php

Kemudian membuat file dengan nama `home.php`, dimana di dalamnya menggunakan konsep modularisasi `require()`. Berikut ini kode programnya.

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/home.PNG)

Untuk implementasi modularisasi bentuk `require()` pada kode program di atas yaitu script `home.php` telah dipanggil suatu file yang bernama `header.php` dan `footer.php`. Jadi, apabila kita meng-klik link navigasi ***'home'*** pada laman `header.php` seperti ini,

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ss_header.PNG)

maka output `home.php` akan gabung bersama dengan *header* dan *footer* seperti pada gambar di bawah ini.

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ss_home.PNG)

#### about.php

Membuat file lagi dengan nama `about.php`, dimana di dalam kode nya terdapat bentuk modularisasi `require()` yang sama halnya seperti `home.php`

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/about.PNG)

Hasilnya, apabila kita meng-klik ***'tentang'*** pada laman seperti berikut.

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ss_header.PNG)

Maka akan muncul gabungan output seperti di bawah ini.

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ss_about.PNG)

## Implementasi Konsep Modularisasi pada kode program Praktikum 8 mengenai Database

#### Kode utama index.php

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/index.PNG)

**Output** `index.php` sebagai berikut.

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ss_index.PNG)

#### Kode utama tambah.php

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/tambah.PNG)

Implementasi konsep modularisasi pada kode di atas, yaitu menggunakan bentuk `require()`, dimana file `tambah.php` telah dipanggil oleh `index.php`, sehingga tampilan *output*-nya seperti di bawah ini.

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ss_tambah.PNG)

#### Kode utama ubah.php

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ubah1.PNG)

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ubah2.PNG)

Pada kode program `ubah.php` juga sama halnya dengan `tambah.php`, dimana menggunakan bentuk modular `require()`. Dan seperti ini tampilan *output*-nya.

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ss_ubah.PNG)

#### Kode hapus.php

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/hapus.PNG)

Dan terakhir untuk kode program `hapus.php` juga menggunakan bentuk `require()`, hasilnya sebagai berikut.

![enter image description here](https://github.com/kameliacindy/Lab9Web/blob/main/img/ss_hapus.PNG)

Jadi, implementasi konsep modularisasi pada kode program Praktikum 8 mengenai Database adalah menggunakan bentuk modular `require()`.

Terima kasih, semoga bermanfaat...

Nama	: Kamelia Cindy Astuti

NIM	: 311910104

Kelas	: TI. 19.A .1
