<h1>Tugas 7: Elemen Dasar Flutter</h1>
Nama: <b>Theodore Kevin Himawan</b><br>
NPM: <b>2306210973</b>

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
<p align="justify">
<h2 align="left"> 5. Jelaskan bagaimana cara kamu mengimplementasikan <i>checklist-checklist</i> di atas</h2>
