# Tugas 7

## Pertanyaan

1. Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget dan jelaskan perbedaan dari keduanya.

_Stateless_ widget adalah widget statis dimana seluruh konfigurasi yang dimuat didalamnya telah diinisiasi sejak awal. Sedangkan _stateful_ widget berlaku sebaliknya dimana sifatnya adalah dinamis, sehingga widget ini dapat diperbaharui kapanpun dibutuhkan berdasarkan _user actions_ atau ketika terjadinya perubahan data.

Secara sederhana, _stateless_ widget dapat diartikan sebagai widget yang tidak dapat dirubah atau tidak akan pernah berubah. Sedangkan _stateful_ widget merupakan widget yang dinamis atau dapat berubah.

2. Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.

- MaterialApp(), membuat aplikasi menerapkan Material Design (_design language system_ milik Google).
- Scaffold(), sebagai landasan halaman.
- AppBar(), biasanya menjadi judul (dari sebuah aplikasi atau halaman).
- Text(), menampilkan teks dan memberikan style pada teks. Dalam proyek ini digunakan untuk menampilkan penentuan ganjil genap berdasarkan nilai pada counter.
- Center(), semua Widget yang ada didalam Widget ini akan diletakkan di bagian tengah.
- Row(), untuk mengurutkan children widget yang terdapat di dalamnya dalam bentuk berbaris atau dari atas ke bawah sesuai dengan order atau susunan dari children tersebut. Dalam proyek ini digunakan untuk menjadi wadah dua button increment dan decrement.
- Column(), untuk mengurutkan children widget yang terdapat di dalamnya dalam bentuk kolom dengan disusun menyamping yang disesuaikan dengan susunan dari widget children yang ada di dalamnya. Dalam proyek ini digunakan untuk menjadi wadah penampil counter dan value ganjil/genap-nya.
- Container(), untuk menjadi wadah yang dapat memberikan aturan margin, padding, dan batasan yang diterapkan pada ukurannya.
- FloatingActionButton(), adalah tombol icon mengambang berbentuk lingkaran yang digunakan untuk memberikan tindakan atau menambahkan sesuatu pada halaman aplikasi. Dalam proyek ini digunakan untuk menambah dan mengurangi nilai dari counter.

3. Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.

setState() adalah fungsi yang akan bertugas untuk memberitahu widget bahwa ada objek yang berubah pada State sehingga aplikasi akan memuat ulang widget tersebut dengan nilai yang sudah diubah. Variabel yang terdampak pada program ini adalah variabel `_counter`.

4. Jelaskan perbedaan antara const dengan final.

Const digunakan untuk deklarasi variabel immutable yang nilainya bersifat konstan dan harus sudah diketahui pada saat waktu kompilasi berjalan, artinya adalah nilai dari variabel tersebut harus sudah di berikan value secara langsung. Sedangkan final juga memiliki sifat immutable, namun tidak harus untuk langsung diberikan value.

5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.

- Membuat fungsi increment dan decrement untuk mengubah nilai pada counter, dan mengaplikasikannya pada FloatingActionButton().

- Menerapkan conditional pada decrement apabila counter lebih dari 0, maka decrement baru bisa dijalankan.

- Membuat sebuah variabel boolean untuk penentuan nilai ganjil atau genap dengan menggunakan modulus, apabila _counter modulus 2 sama dengan nol maka akan mengembalikan nilai genap. Menggunakan widget Text() untuk menampilkan value, apabila genap akan menampilkan tulisan berwarna merah dan ganjil akan menampilkan tulisan berwarna biru.