# 1
## query
```sql
CREATE table tabel_guru (
    -> id_guru int(10) primary key not null,
    -> nama_depan varchar(25) not null,
    -> nama_belakang varchar(25) null,
    -> mapel varchar(50) not null,
    -> jabatan varchar(25) null,
    -> usia int(10) not null,
    -> tanggal_lahir varchar(25) not null);
```
## hasil
![](remed/aset/ss.png)
## analisis
- `id_guru`: Kolom ini adalah kunci utama, artinya kolom ini mengidentifikasi secara unik setiap record dalam tabel. Ini adalah tipe data integer dengan panjang maksimal 10 digit dan wajib diisi (BUKAN NULL).
- `nama_depan`: Kolom ini menyimpan nama depan guru dan wajib diisi (BUKAN NULL).
- `nama_belakang`: Kolom ini menyimpan nama belakang guru dan bersifat opsional (NULL diperbolehkan).
- `mapel`: Kolom ini menyimpan mata pelajaran atau mata kuliah yang diajarkan oleh guru dan wajib diisi (BUKAN NULL).
- `jabatan`: Kolom ini menyimpan jabatan atau jabatan guru dan bersifat opsional (NULL diperbolehkan).
- `usia`: Kolom ini menyimpan umur guru dan wajib diisi (BUKAN NULL).
- `tanggal_lahir`: Kolom ini menyimpan tanggal lahir guru dan wajib diisi (BUKAN NULL).
## kesimpulan
1. `id_guru`: Kolom ini berisi ID guru, bertipe data `int(10)`, bertindak sebagai primary key, dan tidak boleh bernilai NULL.
2. `nama_depan`: Kolom ini berisi nama depan guru, bertipe data `varchar(25)`, dan tidak boleh bernilai NULL.
3. `nama_belakang`: Kolom ini berisi nama belakang guru, bertipe data `varchar(25)`, dan boleh bernilai NULL.
4. `mapel`: Kolom ini berisi mata pelajaran yang diajarkan oleh guru, bertipe data `varchar(50)`, dan tidak boleh bernilai NULL.
5. `jabatan`: Kolom ini berisi jabatan guru, bertipe data `varchar(25)`, dan boleh bernilai NULL.
6. `usia`: Kolom ini berisi usia guru, bertipe data `int(10)`, dan tidak boleh bernilai NULL.
7. `tanggal_lahir`: Kolom ini berisi tanggal lahir guru, bertipe data `varchar(25)`, dan tidak boleh bernilai NULL.

# 2
## query
```sql
INSERT INTO tabel_guru
    -> values (1, "Adrianty", null, "Pemrograman Web","Ketua Jurusan",34,"1982-06-29"),
    -> (2, "Ibrahim","Mallombasang", "Basis Data", "Kepala Sekola", 21, "2000-09-21"),
    -> (3, "Muhammad", "Yusuf","Pemodelan Perangkat Lunak", null, 28, "1992-12-24"),
    -> (4, "Rusdyansyar", null, "Pemrograman Berorientasi Objek", "Asisten Kepala Sekolah", 25, "1996-01-21");
```
## hasil
![](remed/aset/ss1.png)
## analisis
**Kolom tabel_guru:**
- `id`: Kolom ini kemungkinan besar merupakan kolom identitas utama (primary key) yang digunakan untuk mengidentifikasi setiap baris data secara unik.
- `nama_depan`: Kolom ini menyimpan nama depan guru.
- `nama_belakang`: Kolom ini menyimpan nama belakang guru.
- `bidang_keahlian`: Kolom ini menyimpan bidang keahlian guru.
- `jabatan`: Kolom ini menyimpan jabatan guru di sekolah.
- `usia`: Kolom ini menyimpan usia guru.
- `tanggal_lahir`: Kolom ini menyimpan tanggal lahir guru.

**Analisis data:**
- Baris pertama menambahkan data guru dengan nama "Adrianty", bidang keahlian "Pemrograman Web", jabatan "Ketua Jurusan", usia 34 tahun, dan tanggal lahir "1982-06-29". Nama belakangnya tidak diisikan (null).
- Baris kedua menambahkan data guru dengan nama "Ibrahim Mallombasang", bidang keahlian "Basis Data", jabatan "Kepala Sekolah", usia 21 tahun, dan tanggal lahir "2000-09-21".
- Baris ketiga menambahkan data guru dengan nama "Muhammad Yusuf", bidang keahlian "Pemodelan Perangkat Lunak", jabatan tidak diisikan (null), usia 28 tahun, dan tanggal lahir "1992-12-24".
- Baris keempat menambahkan data guru dengan nama "Rusdyansyar", nama belakang tidak diisikan (null), bidang keahlian "Pemrograman Berorientasi Objek", jabatan "Asisten Kepala Sekolah", usia 25 tahun, dan tanggal lahir "1996-01-21".
## kesimpulan
Pernyataan `INSERT` ini akan berhasil menambahkan empat baris data ke tabel `tabel_guru`, dengan catatan untuk memperbaiki kesalahan penulisan "Kepala Sekola" menjadi "Kepala Sekolah". Data yang dimasukkan sesuai dengan tipe data dan aturan nullability yang didefinisikan dalam tabel `tabel_guru`.
# 3
## query
```sql
 INSERT INTO tabel_guru
    -> values (5, "ani", "dya", "Bahasa Inggris", null, 17, "2006-10-08");
```
## hasil
![](remed/aset/ss2.png)
## analisis
- `id_guru`: Nilai yang dimasukkan adalah `5`. Ini menandakan bahwa data guru dengan ID 5 akan dimasukkan ke dalam tabel.
- `nama_depan`: Nilai yang dimasukkan adalah `"ani"`. Ini adalah nama depan guru.
- `nama_belakang`: Nilai yang dimasukkan adalah `"dya"`. Ini adalah nama belakang guru.
- `mapel`: Nilai yang dimasukkan adalah `"Bahasa Inggris"`. Ini adalah mata pelajaran yang diajarkan oleh guru ini.
- `jabatan`: Nilai yang dimasukkan adalah `null`. Ini menandakan bahwa jabatan guru ini tidak diisi.
- `usia`: Nilai yang dimasukkan adalah `17`. Ini adalah usia dari guru tersebut.
- `tanggal_lahir`: Nilai yang dimasukkan adalah `"2006-10-08"`. Ini adalah tanggal lahir dari guru tersebut.
## kesimpulan
Pernyataan `INSERT INTO tabel_guru` menambahkan data satu guru ke tabel `tabel_guru`. Data tersebut termasuk nama, bidang keahlian, usia, dan tanggal lahir guru. Jabatan guru tidak diisikan dalam pernyataan ini.
# 4
## query
```sql
 SELECT * FROM tabel_guru;
```
## hasil
![](remed/aset/ss3.png)
## analisis
1. `SELECT *`: Ini adalah perintah untuk memilih semua kolom dari tabel yang ditentukan.
2. `FROM tabel_guru`: Ini adalah spesifikasi tabel yang akan diambil datanya. Dalam hal ini, tabelnya adalah `tabel_guru`.
## kesimpulan
Pernyataan `SELECT * FROM tabel_guru;` akan mengembalikan semua data dari tabel `tabel_guru`, menampilkan setiap kolom untuk setiap baris data yang ada. Berdasarkan data yang telah di-insert sebelumnya, hasil query ini akan mencerminkan data yang telah dijelaskan di atas. Tidak ada masalah yang terdeteksi dalam struktur atau isi tabel berdasarkan analisis ini.
# 5
## query
```sql
SELECT * FROM tabel_guru
    -> WHERE nama_depan = "rusdyansyar";
```
## hasil
![](remed/aset/ss4.png)
## analisis
1. `SELECT *`: Ini adalah perintah untuk memilih semua kolom dari tabel yang ditentukan.
2. `FROM tabel_guru`: Ini adalah spesifikasi tabel yang akan diambil datanya. Dalam hal ini, tabelnya adalah `tabel_guru`.
3. `WHERE nama_depan = "rusdyansyar"`: Ini adalah klausa filter yang akan memilih hanya baris-baris dari tabel `tabel_guru` yang memiliki nilai `nama_depan` sama dengan `"rusdyansyar"`.
## kesimpulan
Query ini berhasil menemukan dan menampilkan satu baris data dari tabel `tabel_guru` di mana `nama_depan` adalah "rusdyansyar". Data yang dihasilkan lengkap dan sesuai dengan struktur tabel yang ada. Namun, penting untuk mempertimbangkan kasus sensitivitas dalam pencarian string, yang bisa berbeda di berbagai sistem manajemen basis data.
# 6
## query
```sql
 UPDATE tabel_guru SET nama_belakang ="Ganteng" WHERE id_guru="2";
```
## hasil
![](remed/aset/ss5.png)
## analisis
1. `UPDATE tabel_guru`: Ini adalah perintah untuk memperbarui data pada tabel `tabel_guru`.
2. `SET nama_belakang = "Ganteng"`: Ini adalah bagian yang menentukan kolom yang akan diperbarui dan nilai baru yang akan diberikan. Dalam hal ini, kolom `nama_belakang` akan diubah menjadi `"Ganteng"`.
3. `WHERE id_guru = "2"`: Ini adalah klausa filter yang akan membatasi perubahan hanya pada baris-baris di tabel `tabel_guru` yang memiliki nilai `id_guru` sama dengan `"2"`.
## kesimpulan
update query `UPDATE tabel_guru SET nama_belakang ="Ganteng" WHERE id_guru="2";` akan mengubah nama belakang guru dengan `id_guru` 2 menjadi "Ganteng.
# 7
## query
```sql
 DELETE FROM tabel_guru WHERE id_guru=5;
```
## hasil
![](remed/aset/ss6.png)
## analisis
1. `DELETE FROM tabel_guru`: Ini adalah perintah untuk menghapus data dari tabel `tabel_guru`.
2. `WHERE id_guru = 5`: Ini adalah klausa filter yang akan membatasi penghapusan hanya pada baris-baris di tabel `tabel_guru` yang memiliki nilai `id_guru` sama dengan `5`.
## kesimpulan
Pernyataan `DELETE FROM tabel_guru WHERE id_guru=5;` akan menghapus satu baris data dari tabel `tabel_guru` di mana nilai kolom `id_guru` adalah 5. Baris yang memiliki `id_guru = 5` akan dihapus dari tabel. Tidak ada data lain yang akan terpengaruh oleh pernyataan ini karena kondisi hanya memilih baris dengan `id_guru = 5`.
# 8
## query
```sql
SELECT * FROM tabel_guru
    -> WHERE mapel LIKE 'Pem%' and usia < 30
    -> ORDER BY usia ASC;
```
## hasil
![](remed/aset/ss7.png)
## analisis
1. `SELECT *`: Ini adalah perintah untuk memilih semua kolom dari tabel.
2. `FROM tabel_guru`: Ini menentukan tabel yang akan diakses, yaitu `tabel_guru`.
3. `WHERE mapel LIKE 'Pem%' AND usia < 30`: Ini adalah klausa filter yang akan membatasi data yang dipilih. Kriterianya adalah:
    - `mapel LIKE 'Pem%'`: Memilih data di mana kolom `mapel` dimulai dengan "Pem" (misalnya "Pemrograman", "Pemeliharaan", dll.).
    - `AND usia < 30`: Memilih data di mana kolom `usia` kurang dari 30.
4. `ORDER BY usia ASC`: Ini adalah klausa untuk mengurutkan hasil yang dipilih berdasarkan kolom `usia` secara ascending (dari yang terkecil ke terbesar).
## kesimpulan
Pernyataan `SELECT * FROM tabel_guru WHERE mapel LIKE 'Pem%' AND usia < 30 ORDER BY usia ASC;` akan mengambil dan menampilkan semua data guru dari tabel `tabel_guru` di mana mata pelajaran dimulai dengan "Pem" dan usia guru kurang dari 30 tahun, kemudian diurutkan berdasarkan usia secara menaik.
# 9
## query
```sql
 SELECT id_guru, nama_depan FROM tabel_guru
    -> WHERE nama_depan LIKE '__%i%';
```
## hasil
![](remed/aset/ss8.png)
## analisis
1. `SELECT id_guru, nama_depan`: Bagian kueri ini menentukan kolom yang akan diambil, dalam hal ini, kolom `id_guru`dan `nama_depan`.
2. `FROM tabel_guru`: Bagian kueri ini menunjukkan bahwa data akan diambil dari `tabel_guru`tabel.
3. `WHERE nama_depan LIKE '__%i%'`: Bagian kueri ini menerapkan filter pada data, hanya memilih baris yang kolomnya `nama_depan`berisi setidaknya satu karakter sebelum dan sesudah huruf "i".
    - Operator `LIKE`digunakan untuk pencocokan pola, dimana:
        - `_`cocok dengan satu karakter.
        - `%`cocok dengan urutan apa pun yang terdiri dari nol atau lebih karakter.
        - Jadi, `'__%i%'`cocok dengan string apa pun yang memiliki setidaknya satu karakter sebelum dan sesudah huruf "i".
## kesimpulan
Pernyataan `SELECT id_guru, nama_depan FROM tabel_guru WHERE nama_depan LIKE '__%i%';` akan mengambil dan menampilkan kolom `id_guru` dan `nama_depan` dari tabel `tabel_guru` di mana nama depan memiliki minimal dua karakter sebelum huruf 'i' pertama kali muncul.
# 10
## query
```sql
 SELECT CONCAT_WS(" ",nama_depan, nama_belakang) AS nama_lengkap FROM tabel_guru;
```
## hasil
![](remed/aset/ss9.png)
## analisis
- `CONCAT_WS(" ",nama_depan, nama_belakang)`:
    - `CONCAT_WS`: Fungsi ini menggabungkan beberapa string dengan separator yang ditentukan.
    - `" "`: Separator yang digunakan adalah spasi.
    - `nama_depan`: Mengambil nilai dari kolom `nama_depan` di tabel `tabel_guru`.
    - `nama_belakang`: Mengambil nilai dari kolom `nama_belakang` di tabel `tabel_guru`.
- `AS nama_lengkap`: Memberi alias `nama_lengkap` pada hasil gabungan string.
- `tabel_guru`: Menunjukkan tabel yang ingin dipilih datanya, yaitu tabel `tabel_guru`.
## kesimpulan
Perintah SQL ini akan memilih dan menggabungkan nilai dari kolom `nama_depan` dan `nama_belakang` di tabel `tabel_guru` dengan spasi sebagai separator dan menyimpan hasilnya di kolom baru dengan alias `nama_lengkap`. Hasilnya adalah tabel baru yang berisi kolom `nama_lengkap` yang berisi nama lengkap guru dari gabungan nama depan dan nama belakang.
# 11
## query
```sql
ALTER TABLE tabel_guru
    -> ADD status enum("PNS", "PPPK", "Honorer");
```
## hasil
![](remed/aset/ss10.png)
## analisis
- **`ALTER TABLE tabel_guru`:** Bagian ini menunjukkan tabel yang ingin dimodifikasi, yaitu tabel `tabel_guru`.
- **`ADD status`:** Bagian ini menambahkan kolom baru bernama `status` ke tabel `tabel_guru`.
- **`enum("PNS", "PPPK", "Honorer")`:** Bagian ini menentukan tipe data kolom `status` sebagai `enum` dan mendefinisikan tiga nilai yang mungkin: "PNS", "PPPK", dan "Honorer". Tipe data `enum` memungkinkan untuk menyimpan data kategori dengan pilihan yang terbatas.
## kesimpulan
Perintah SQL tersebut menambahkan kolom baru yang disebut `status` ke tabel `tabel_guru` dengan tipe data ENUM. Tipe data ENUM memungkinkan Anda untuk membatasi nilai yang dapat dimasukkan ke dalam kolom tersebut hanya pada nilai-nilai yang telah ditentukan.
# 12
## query
```sql
 SELECT nama_depan, MAX(usia) AS usia FROM tabel_guru;
```
## hasil
![](remed/aset/ss11.png)
## analisis
- `nama_depan`: Mengambil nilai dari kolom `nama_depan` di tabel `tabel_guru`.
- `MAX(usia) AS usia`:
    - `MAX(usia)`: Menghitung nilai maksimum dari kolom `usia` di tabel `tabel_guru`.
    - `AS usia`: Memberi alias `usia` pada hasil perhitungan nilai maksimum.
- `tabel_guru`: Menunjukkan tabel yang ingin dipilih datanya, yaitu tabel `tabel_guru`.
## kesimpulan
Perintah SQL ini akan memilih nama depan dan usia maksimum dari setiap guru di tabel `tabel_guru`. Hasilnya adalah tabel baru dengan dua kolom: `nama_depan` dan `usia`. Kolom `usia` berisi usia maksimum dari setiap guru.