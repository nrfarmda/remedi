# Analisis Ujian Flower
## Index 
```html
<html>
    <head>
        <title> halaman pertama </title>
    </head>
    <body>
        <div>
        <table border="0" width="100%" width="100%">
            <tr> 
                <td height="50px" bgcolor="yellow"> Flower Shop </td>  
            </tr>
        </table>
    </div>

    <div align="center">
        <h1> Selamat datang di flower shop </h1>
        <img src="3.jpg" width="410px" height="410px">
    </div> <br>

    <div align="center">
            <a href="order bunga.html"> <input type="submit" value="Order Now!"> </a>
    </div> <br>

    <div>
        <table border="1">
            <tr>
                <td colspan="2" bgcolor="aqua" width="1000" align="center"> <a href="list bungaa.html"> List daftar bunga </a></td>
                <td colspan="2" bgcolor="aqua" width="1000" align="center"> <a href="order bunga.html"> Pesan Bunga </a></td>
            </tr>
        </table>
    </div>
    </body>
</html>
```
### Analisis
1. Struktur Dasar,
    - Dokumen HTML dimulai dengan tag `<html>` dan diakhiri dengan tag `</html>`.
    - Bagian kepala dokumen HTML didefinisikan menggunakan tag `<head>`.
    - Judul halaman ditentukan menggunakan tag `<title>` di dalam elemen `<head>`.
    - Bagian tubuh dokumen HTML didefinisikan menggunakan tag `<body>`, yang berisi konten yang akan ditampilkan pada halaman.
2. Header dan Nama Toko, 
    - Terdapat sebuah tabel di dalam elemen `<div>`.
    - Tabel ini memiliki atribut `border="0"` dan `width="100%"`.
    - Tabel tersebut memiliki satu baris (`<tr>`) dan satu kolom (`<td>`).
    - Kolom tersebut memiliki tinggi (`height`) sebesar 50 piksel dan latar belakang (`bgcolor`) kuning.
    - Teks "Flower Shop" ditampilkan di dalam kolom tersebut.
3. Selamat Datang dan Gambar Bunga, 
    - Terdapat sebuah elemen `<div>` dengan atribut `align="center"`.
    - Di dalam elemen `<div>` tersebut, terdapat elemen `<h1>` yang menampilkan teks "Selamat datang di flower shop".
    - Selain itu, ada elemen `<img>` yang menampilkan gambar bunga.
    - Gambar bunga ditentukan menggunakan atribut `src` yang menunjuk ke file "bunga 2.jpg".
    - Gambar bunga juga memiliki atribut `width` sebesar 410 piksel dan `height` sebesar 410 piksel.
4. Tombol Order Now,
    - Terdapat elemen `<div>` dengan atribut `align="center"`.
    - Di dalam elemen `<div>` tersebut, terdapat elemen `<a>` yang memiliki atribut `href` bernilai "order bunga.html".
    - Di dalam elemen `<a>`, terdapat elemen `<input>` dengan atribut `type="submit"` dan `value="Order Now!"`.
    - Ini menghasilkan tombol dengan label "Order Now!" yang menghubungkan ke halaman "order bunga.html" ketika diklik.
5. Tabel Daftar Bunga dan Pesan Bunga,
    - Terdapat elemen `<table>` dengan atribut `border="1"`.
    - Tabel ini memiliki satu baris (`<tr>`) dengan dua kolom (`<td>`).
    - Kolom pertama memiliki atribut `colspan="2"`, `bgcolor="aqua"`, `width="1000"`, dan `align="center"`.
    - Di dalam kolom ini terdapat tautan (`<a>`) dengan atribut `href` yang menghubungkan ke halaman "list bungaa.html" dan menampilkan teks "List daftar bunga".
    - Kolom kedua memiliki atribut yang sama dengan kolom pertama.
    - Di dalam kolom ini terdapat tautan (`<a>`) dengan atribut `href` yang menghubungkan ke halaman "order bunga.html" dan menampilkan teks "Pesan Bunga".
### hasil
![](remed/remed-HTML/aset/ss.png)
## List
```html
<html>
    <head>
        <title> LIST BUNGA </title>
    </head>
    <body>
        <h1> List Bunga </h1>
        <table border="1">
            <tr>
                <td> Bunga 1 <br> <img src="1.jpg" width="100"></td>
                <td>
                <ul>
                    <li> Asal : <b> gunung latimojong </b></li>
                    <li> Keharuman : <b> Tahan lama </b> </li>
                    <li> harga : <b> 75.000 </b> </li>
                </ul>
                <td> Bunga 4 <br> <img src="4.jpg" width="100"></td>
                <td>
                <ul>
                    <li> Asal : <b> Danau Tanralili </b></li>
                    <li> Keharuman : <b> Sedang </b> </li>
                    <li> harga : <b> 50.000 </b> </li>
                </ul>
            </tr>
            <tr>
                <td> Bunga 2 <br> <img src="2.jpg" width="100"></td>
                <td>
                <ul>
                    <li> Asal : <b> Taman Macan </b></li>
                    <li> Keharuman : <b> Biasa </b> </li>
                    <li> harga : <b> 15.000 </b> </li>
                </ul>
                <td> Bunga 5 <br> <img src="5.jpg" width="100"></td>
                <td>
                <ul>
                    <li> Asal : <b> Gunung Bawakaraeng </b></li>
                    <li> Keharuman : <b> Tahan lama </b> </li>
                    <li> harga : <b> 100.000 </b> </li>
                </ul>
            </tr>
            <tr>
                <td> Bunga 3 <br> <img src="3.jpg" width="100"></td>
                <td>
                <ul>
                    <li> Asal : <b> Taman Pakui </b></li>
                    <li> Keharuman : <b> Sedang </b> </li>
                    <li> harga : <b> 25.000 </b> </li>
                </ul>
                <td colspan="3" align="center" bgcolor="grey"> kosong </td>
            </tr>
            <tr>
                <td bgcolor="red" align="center" colspan="4"> <a href="order bunga.html"> Pesan Sekarang </a></td>
            </tr>
        </table> <br>
        <a href="index.html"> kembali ke home </a>
    </body>
</html>
```
### Analisis
1. Struktur Dasar:
    - Dokumen HTML dimulai dengan tag `<html>` dan diakhiri dengan tag `</html>`.
    - Bagian kepala dokumen HTML didefinisikan menggunakan tag `<head>`.
    - Judul halaman ditentukan menggunakan tag `<title>` di dalam elemen `<head>`.
    - Bagian tubuh dokumen HTML didefinisikan menggunakan tag `<body>`, yang berisi konten yang akan ditampilkan pada halaman.
2. Judul Halaman:
    - Terdapat sebuah elemen `<h1>` yang menampilkan teks "List Bunga".
3. Tabel Daftar Bunga:
    - Terdapat elemen `<table>` dengan atribut `border="1"`.
    - Tabel ini memiliki beberapa baris (`<tr>`) dan kolom (`<td>`).
    - Setiap baris mewakili satu bunga dan ditempatkan di dalam elemen `<tr>`.
    - Setiap kolom mewakili informasi spesifik tentang bunga dan ditempatkan di dalam elemen `<td>`.
4. Data Bunga:
    - Setiap bunga memiliki dua kolom yang menunjukkan gambar dan informasi terkait.
    - Gambar bunga ditampilkan menggunakan elemen `<img>` dengan atribut `src` yang menunjuk ke file gambar yang terkait.
    - Informasi bunga ditampilkan dalam elemen `<ul>` (unordered list).
    - Setiap informasi bunga ditampilkan dalam elemen `<li>` (list item) di dalam elemen `<ul>`.
    - Informasi yang ditampilkan termasuk asal bunga, keharuman, dan harga.
5. Kolom Kosong:
    - Terdapat satu baris yang memiliki kolom dengan atribut `colspan="3"` dan `bgcolor="grey"`.
    - Kolom tersebut menampilkan teks "kosong" dan mengisi tiga kolom dalam satu baris.
6. Tombol Pesan Sekarang:
    - Terdapat satu baris yang memiliki kolom dengan atribut `colspan="4"`, `bgcolor="red"`, dan `align="center"`.
    - Kolom tersebut berisi tautan (`<a>`) dengan atribut `href` yang menghubungkan ke halaman "order bunga.html" dan menampilkan teks "Pesan Sekarang".
7. Tautan Kembali ke Home:
    - Terdapat tautan (`<a>`) dengan atribut `href` yang menghubungkan ke halaman "index.html" dan menampilkan teks "kembali ke home".
### hasil
![](remed/remed-HTML/aset/ss1.png)
## Order
```html
<html> 
    <head> 
        <title> ORDER BUNGA </title>
    </head>
    <body>
        <h1> Pesan Bunga </h1>

        <label for="nama"> <b> nama </b></label> <br>
        <input type="text" id="nama" required> <br> <br>

        <label for="Jenis Bunga"> Jenis Bunga : </label> <br>
        <select id="jenis bunga" name="bunga">
            <option disabled> --- Pilih Bunga --- </option>
            <option value="Bunga 1">  Bunga 1 </option>
            <option value="Bunga 2"> Bunga  2</option>
            <option value="Bunga 3">  Bunga 3</option>
            <option value="Bunga 4">  Bunga 4</option>
            <option value="Bunga 5">  Bunga 5 </option>
        </select> <br> <br>

        <label for="pembayaran"> Pembayaran </label><br>
        <input type="radio" name="pembayaran"> 
        <label> Tunai </label>
        <input type="radio" name="pembayaran"> 
        <label> Transfer </label> <br> <br>

         Alamat Pengiriman: <br>
        <textarea cols="25" rows="5"> </textarea> <br> <br>

        <label for="waktu"> <B> Waktu Pengiriman </B></label> <BR>
        <input type="checkbox" name="pagi"> pagi
        <input type="checkbox" name="siang"> siang 
        <input type="checkbox" name="sore"> sore
        <input type="checkbox" name="malam"> malam 
        <BR> <BR>
        <input type="submit" value="Pesan">
        <input type="reset" value="ulang"> <br>
        
        <br> <br> <hr>
        
        <a href="list bungaa.html"> Liat daftar Bunga </a> <BR>
        <a href="index.html"> Kembali ke home </a>

    </body>
</html>
```
### Analisi
1. Struktur Dasar:
    - Dokumen HTML dimulai dengan tag `<html>` dan diakhiri dengan tag `</html>`.
    - Bagian kepala dokumen HTML didefinisikan menggunakan tag `<head>`.
    - Judul halaman ditentukan menggunakan tag `<title>` di dalam elemen `<head>`.
    - Bagian tubuh dokumen HTML didefinisikan menggunakan tag `<body>`, yang berisi konten yang akan ditampilkan pada halaman.
2. Judul Halaman:
    - Terdapat sebuah elemen `<h1>` yang menampilkan teks "Pesan Bunga".
3. Formulir Pemesanan Bunga:
    - Terdapat beberapa elemen `<label>` dan `<input>` yang digunakan untuk mengumpulkan informasi dari pengguna.
    - Elemen `<label>` digunakan untuk memberikan label pada input.
    - Elemen `<input>` digunakan untuk memasukkan data, seperti nama pengguna, jenis bunga, dan alamat pengiriman.
    - Terdapat elemen `<select>` dengan id "jenis bunga" yang memungkinkan pengguna memilih jenis bunga dari daftar yang disediakan.
    - Terdapat elemen `<input>` dengan tipe "radio" yang memungkinkan pengguna memilih metode pembayaran.
    - Terdapat elemen `<textarea>` yang memungkinkan pengguna memasukkan alamat pengiriman dalam bentuk teks yang lebih panjang.
    - Terdapat elemen `<input>` dengan tipe "checkbox" yang memungkinkan pengguna memilih waktu pengiriman yang diinginkan.
    - Terdapat elemen `<input>` dengan tipe "submit" yang memungkinkan pengguna mengirimkan formulir.
    - Terdapat elemen `<input>` dengan tipe "reset" yang memungkinkan pengguna menghapus data yang telah dimasukkan dalam formulir.
4. Tautan Lain:
    - Terdapat dua tautan (`<a>`) yang mengarahkan pengguna ke halaman lain.
    - Tautan pertama mengarah ke halaman "list bungaa.html" dengan teks "Liat daftar Bunga".
    - Tautan kedua mengarah ke halaman "index.html" dengan teks "Kembali ke home".
### hasil
![](remed/remed-HTML/aset/ss2.png)