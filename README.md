<h1>Tugas 8: Navigation, Layout, Forms, & Input Elements</h1>
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

<h2>1. Apa kegunaan const di Flutter? Jelaskan apa keuntungan ketika menggunakan const pada kode Flutter. Kapan sebaiknya kita menggunakan const, dan kapan sebaiknya tidak digunakan?</h2>
<h2>2. Jelaskan dan bandingkan penggunaan Column dan Row pada Flutter. Berikan contoh implementasi dari masing-masing layout widget ini!</h2>
<h2>3. Sebutkan apa saja elemen input yang kamu gunakan pada halaman form yang kamu buat pada tugas kali ini. Apakah terdapat elemen input Flutter lain yang tidak kamu gunakan pada tugas ini? Jelaskan!</h2>
<h2>4. Bagaimana cara kamu mengatur tema (theme) dalam aplikasi Flutter agar aplikasi yang dibuat konsisten? Apakah kamu mengimplementasikan tema pada aplikasi yang kamu buat?</h2>
<h2>5. Bagaimana cara kamu menangani navigasi dalam aplikasi dengan banyak halaman pada Flutter?</h2>
