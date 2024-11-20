<h1>Tugas 9: Integrasi Layanan Web Django dengan Aplikasi Flutter</h1>
Nama: <b>Theodore Kevin Himawan</b><br>
NPM: <b>2306210973</b>

<h2>Tugas Sebelumnya😎👨‍💻</h2>
<details>
<summary>Tugas 7: Elemen Dasar Flutter</summary>
<h2 align="left"> 1. Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget, dan jelaskan perbedaan dari keduanya.</h2>
<p align="justify">Stateless widget dan stateful widget adalah dua jenis widget utama dalam Flutter. Stateless widget adalah widget yang tidak memiliki "state" atau kondisi yang berubah-ubah. Sementara itu, stateful widget adalah widget yang memiliki "state" atau kondisi yang bisa saja berubah. Stateless widget sedikit lebih cepat dan digunakan untuk button static. Stateful widget digunakan dalam kondisi dynamic, seperti tombol yang bisa berubah warna bila diklik.
</p>

<h2 align="left"> 2. Sebutkan widget apa saja yang kamu gunakan pada proyek ini dan jelaskan fungsinya.</h2>
<p align="justify">Dalam proyek ini, saya menggunakan stateless widget. Beberapa widget yang saya gunakan termasuk:

<ul>
    <li align="justify"><b>Scaffold</b>: Sebuah widget yang menyediakan struktur dasar aplikasi saya. Widget ini membantu membuild halaman dan memiliki AppBar dan Body. </li>
    <li align="justify"><b>AppBar</b>: Sebuah widget di bagian atas untuk menampilkan judul. Di kasus saya, AppBar menampilkan judul Toko Messi Indah.</li>
    <li align="justify"><b>InfoCard</b>: Custom widget yang telah saya buat. Widget ini menampilkan data saya, seperti nama, npm, dan kelas PBP.</li>
    <li align="justify"><b>ItemCard</b>: Custom widget yang telah saya buat untuk menampilkan buttons sesuai ketentuan. Widget ini menampilkan Lihat Daftar Produk, Tambah Produk, dan Logout.</li>
    <li align="justify"><b>SnackBar</b>: SnackBar adalah widget yang menampilkan pesan sementara di bagian bawah layar saat ada interaksi tertentu. Di proyek ini, SnackBar digunakan untuk memberikan notifikasi singkat ketika pengguna menekan tombol.</li>
</ul>
</p>

<h2 align="left"> 3. Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.</h2>
<p align="justify">setState() adalah fungsi yang digunakan dalam stateful widget di Flutter untuk memberi tahu framework bahwa ada perubahan pada data atau kondisi dalam widget yang memerlukan pembaruan tampilan. Ketika setState() dipanggil, Flutter akan merender ulang bagian UI yang telah diklik oleh user. </p>

<h2 align="left"> 4. Jelaskan perbedaan antara const dengan final.</h2>
<p align="justify">Dari pemahaman saya, const menjadikan nilai benar-benar konstan dan immutable, bahkan dalam konteks objek atau daftar, sementara final hanya memastikan nilai tidak dapat diubah setelah inisialisasi pertama.
<h2 align="left"> 5. Jelaskan bagaimana cara kamu mengimplementasikan <i>checklist-checklist</i> di atas</h2>
<p>
    <ul>
        <li>Membuat repositori baru di github untuk proyek ini.</li>
        <li>Membuat proyek baru dengan menjalankan flutter create toko_messi_indah</li>
        <li>Dalam folder lib, membuat file baru bernama menu.dart</li>
        <li>Dalam main.dart, mengubah warna aplikasi menjadi biru dengan mengganti colorScheme</li>
        <li>Mengubah class MyHomePage menjadi stateless widget</li>
        <li>Membuat card yang berisi data nama, npm, dan kelas saya</li>
        <li>Membuat class baru bernama InfoCard di file menu.dart</li>
        <li>Membuat button yang bisa diklik oleh user dengan Icon</li>
        <li>Mengganti warna button supaya memiliki warna yang berbeda</li>
        <li>Mengisi list ItemHomePage dengan buttons sesuai dengan ketentuan tugas</li>
        <li align="justify">Membuat class baru bernama ItemCard untuk menampilkan buttons yang sudah dibuat. Terdapat juga SnackBar yang menunjukkan message di bagian bawah page setelah button diklik</li>
        <li>Mengintegrasikan InfoCard dan ItemCard untuk ditampilkan di MyHomePage</li>
        <li>Mengecek program dengan menjalankan flutter analyze</li>
        <li>Melihat bentuk program dengan menjalankan flutter run</li>
        <li>Melakukan git add, commit, dan push</li>
    </ul>
</p>
</details>

<details>
<summary>Tugas 8: Navigation, Layout, Forms, & Input Elements</summary>
<h2>1️⃣ Apa kegunaan const di Flutter? Jelaskan apa keuntungan ketika menggunakan const pada kode Flutter. Kapan sebaiknya kita menggunakan const, dan kapan sebaiknya tidak digunakan?</h2>

<p align="justify">Kegunaan const di Flutter adalah untuk membuat objek yang bersifat tetap (immutable) dan hanya dihitung sekali saat kompilasi. Keuntungan menggunakan const di Flutter adalah membuat objek yang bersifat konstan sehingga tidak perlu dibuat ulang setiap kali widget di-rebuild. Karena itu, kode menjadi lebih efisien dan "ringan". Sebaiknya, const digunakan saat kita tahu tampilan akan tetap statis, dan sebaiknya tidak digunakan apabila terdapat objek yang dinamis dan tampilannya berubah-ubah terus.</p>

<h2>2️⃣ Jelaskan dan bandingkan penggunaan Column dan Row pada Flutter. Berikan contoh implementasi dari masing-masing layout widget ini!</h2>
<p align="justify">
Column dan Row di Flutter digunakan untuk menyusun widget secara vertikal dan horizontal. Column menempatkan widget dalam urutan dari atas ke bawah, sedangkan Row dari kiri ke kanan.

<b>Contoh implementasi Row:</b></p>
```dart
Row(
  mainAxisAlignment: MainAxisAlignment.spaceAround,
  children: [Icon(Icons.star), Icon(Icons.star_border)],
)
```
<b>Contoh implementasi Column:</b>
```dart
Column(
  mainAxisAlignment: MainAxisAlignment.center,
  children: [Text("Item 1"), Text("Item 2")],
)
```

<h2>3️⃣ Sebutkan apa saja elemen input yang kamu gunakan pada halaman form yang kamu buat pada tugas kali ini. Apakah terdapat elemen input Flutter lain yang tidak kamu gunakan pada tugas ini? Jelaskan!</h2>
<p align="justify">Pada halaman form tugas kali ini, saya menggunakan beberapa elemen input Flutter, seperti TextFormField untuk menerima teks (misalnya nama produk, kategori, deskripsi, dan harga), dan ElevatedButton sebagai tombol untuk submit data. Elemen input lain di Flutter yang tidak saya gunakan adalah DropdownButton, yang berguna untuk memilih opsi dari daftar, Checkbox untuk pilihan (ya/tidak), dan Slider untuk memilih nilai dalam rentang tertentu.</p>

<h2>4️⃣ Bagaimana cara kamu mengatur tema (theme) dalam aplikasi Flutter agar aplikasi yang dibuat konsisten? Apakah kamu mengimplementasikan tema pada aplikasi yang kamu buat?</h2>
<p align="justify">Iya, saya mengimplementasikan tema pada aplikasi ini. Untuk mengatur tema dalam aplikasi Flutter agar konsisten, saya menggunakan ThemeData di bagian MaterialApp. Dengan ThemeData, kita bisa mengatur warna utama (primaryColor), warna teks, gaya teks (textTheme), serta gaya elemen seperti AppBar, tombol, dan icons.</p>

<h2>5️⃣ Bagaimana cara kamu menangani navigasi dalam aplikasi dengan banyak halaman pada Flutter?</h2>
<p align="justify">Saya menangani navigasi menggunakan Navigator untuk berpindah antara halaman menggunakan metode push dan pop. Metode push digunakan untuk menambah halaman ke tumpukan (stack), sementara pop menghapus halaman dari tumpukan dan kembali ke halaman sebelumnya.</p>
</details>

## 1. Jelaskan mengapa kita perlu membuat model untuk melakukan pengambilan ataupun pengiriman data JSON? Apakah akan terjadi error jika kita tidak membuat model terlebih dahulu?
Membuat model untuk pengambilan atau pengiriman data JSON sangat penting karena model mempermudah proses pemetaan data JSON ke dalam struktur data yang terorganisir, seperti objek. Hal ini memudahkan untuk pengelolaan, validasi, dan manipulasi data, serta mengurangi risiko kesalahan ketika format data berubah. Jika model tidak dibuat, kita harus menangani data secara manual, yang lebih rawan error, sulit di-maintain, dan cenderung meningkatkan kompleksitas kode.

## 2. Jelaskan fungsi dari library http yang sudah kamu implementasikan pada tugas ini
Library `http` digunakan dalam aplikasi Flutter untuk mengirim request `HTTP`, seperti `GET` dan `POST`, ke server backend. Library ini juga berfungsi untuk menerima respons dari server, termasuk mem-parsing data JSON yang dikembalikan. Jadi, `http` ini menjadi penghubung antara aplikasi Flutter dan API backend untuk mengelola pertukaran data.

## 3. Jelaskan fungsi dari CookieRequest dan jelaskan mengapa instance CookieRequest perlu untuk dibagikan ke semua komponen di aplikasi Flutter.
`CookieRequest` berfungsi untuk menyimpan cookie sesi pengguna, yang berguna untuk mempertahankan status autentikasi pengguna, seperti login. Cookie ini akan secara otomatis dikirim bersama setiap request HTTP yang memerlukan autentikasi. Instance CookieRequest perlu dibagikan ke seluruh komponen aplikasi agar semua fitur yang memerlukan autentikasi dapat mengakses status sesi yang sama tanpa perlu dikelola ulang di setiap bagian aplikasi.

## 4. Jelaskan mekanisme pengiriman data mulai dari input hingga dapat ditampilkan pada Flutter.
Mekanisme pengiriman data dimulai ketika pengguna memasukkan data melalui form di Flutter. Data ini kemudian dikirim ke backend melalui request `HTTP`, misalnya `POST`. Backend (Django) akan memproses data tersebut, seperti menyimpannya ke database atau menghasilkan respons tertentu. Respons dari backend, dalam format JSON, diterima oleh Flutter, diproses, dan hasilnya ditampilkan kepada pengguna di antarmuka aplikasi flutter kita.

## 5. Jelaskan mekanisme autentikasi dari login, register, hingga logout. Mulai dari input data akun pada Flutter ke Django hingga selesainya proses autentikasi oleh Django dan tampilnya menu pada Flutter.
Proses autentikasi meliputi login, register, dan logout. Pada proses login, pengguna memasukkan kredensial di Flutter, yang kemudian dikirim ke Django melalui request POST. Django memverifikasi kredensial dan, jika valid, mengembalikan cookie atau token sesi yang disimpan di `CookieRequest`. Token ini digunakan untuk mengakses fitur yang memerlukan autentikasi. Pada register, data akun dikirim ke Django, diverifikasi, dan disimpan ke database jika valid. Django kemudian memberikan konfirmasi ke Flutter. Pada logout, Flutter mengirimkan request ke Django untuk menghapus sesi atau token, dan Django memastikan pengguna telah keluar. Setelah logout, Flutter menghapus data sesi lokal dan mengarahkan pengguna kembali ke halaman login.

## 6. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step! (bukan hanya sekadar mengikuti tutorial).
1. Pertama, saya mengimplementasikan fitur registrasi akun. Di Django, saya membuat aplikasi bernama authentication dan menambahkan fungsi `register` di file` views.py` untuk memvalidasi input, seperti memastikan password cocok dan username belum digunakan. Setelah itu, saya konfigurasi path di `urls.py`. Di Flutter, saya membuat file register.dart yang berisi form registrasi menggunakan widget seperti TextField untuk username, password, dan konfirmasi password. Saya menggunakan package pbp_django_auth untuk menghubungkan form ini dengan endpoint Django dan menampilkan pesan kesalahan jika registrasi gagal atau mengarahkan ke halaman login jika berhasil.

2. Selanjutnya, saya membuat halaman login pada Flutter. Di Django, saya menambahkan fungsi `login` di `views.py `untuk memverifikasi kredensial pengguna, lalu saya konfigurasi path di urls.py. Di Flutter, saya membuat file login.dart yang berisi form login. Saya menggunakan CookieRequest dari pbp_django_auth untuk mengirim data login ke server Django.

3. Setelah itu, saya mengintegrasikan sistem autentikasi Django dengan Flutter. Di Django, saya mengatur middleware `CorsMiddleware` pada settings.py untuk mendukung komunikasi lintas domain. Saya juga menambahkan variabel konfigurasi seperti `CORS_ALLOW_ALL_ORIGINS` dan `ALLOWED_HOSTS`. Di Flutter, saya menambahkan `Provider` di `main.dart `untuk menyediakan objek `CookieRequest` ke seluruh aplikasi, sehingga session dapat digunakan secara global.

4. Model product di django saya mencangkup `name`, `price`, `description`, dan `quantity`. Di Flutter, saya menggunakan Quicktype untuk membuat model Dart dari data JSON yang dihasilkan oleh endpoint Django.

5. Berikutnya, saya membuat halaman daftar item. Di Flutter, saya membuat file list_item.dart dan menggunakan `FutureBuilder` untuk mengambil data dari endpoint Django menggunakan `CookieRequest.get`. Data ditampilkan menggunakan widget ListView.builder, dengan menampilkan atribut seperti name, price, description, dan quantity. Saya juga memastikan view JSON untuk memfilter item berdasarkan pengguna yang sedang login menggunakan request.user.

6. Selanjutnya, saya mengimplementasikan fitur logout. Di Django, saya menambahkan fungsi logout di views.py yang memanggil `auth_logout` untuk menghapus sesi pengguna. Di Flutter, saya mengubah apa yang terjadi ketika tombol logout ditekan. Setelah logout, pengguna diarahkan kembali ke halaman login.

7. Terakhir, saya mengintegrasikan form input di Flutter dengan Django. Di Django, saya membuat path create-flutter/ untuk menerima data dari Flutter dan menyimpannya ke database. Di Flutter, saya membuat form menggunakan pbp_django_auth untuk mengirim data form ke Django.