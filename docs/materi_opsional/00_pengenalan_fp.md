# Pengenalan Functional Programming

Selain Pemrograman Berorientasi Objek (OOP) yang sudah kita pelajari secara mendalam, bahasa Dart ternyata juga memiliki dukungan yang sangat kuat untuk gaya penulisan **Functional Programming (FP)**. 

## Apa itu Functional Programming?

Jika dalam dunia OOP kita selalu memecah program berdasarkan "Benda" atau "Objek" yang memiliki sifat fisik dan aksi, maka dalam **Functional Programming**, kita menganggap **Fungsi (Function)** sebagai pemeran utamanya. 

Dalam gaya FP, fungsi diperlakukan sama istimewanya dengan tipe data biasa (seperti angka atau teks). Artinya, sebuah fungsi bisa disimpan ke dalam variabel, dikirim masuk ke dalam fungsi lain, bahkan bisa dikeluarkan sebagai hasil dari fungsi lain. Ini disebut sebagai *First-Class Citizen*.

**Analogi:** Bayangkan proses meracik minuman kopi.
- **Dalam OOP**: Kamu memesan kopi melalui sebuah "Mesin Kopi" (Objek). Mesin kopi itu memiliki alat fisik dan menyimpan datanya sendiri (misalnya mengetahui berapa sisa gram biji kopi di dalamnya).
- **Dalam FP**: Kamu tidak peduli dengan mesinnya. Kamu hanya fokus pada "Proses Meracik Kopi". Kamu hanya melempar biji kopi mentah ke dalam sebuah fungsi `buatKopi(biji)`, dan seketika langsung mendapatkan hasil secangkir kopi. Fungsi ini murni bekerja di tempat terisolasi, tidak memedulikan dunia luar, dan tidak mengubah barang apapun di sekitarnya.

## Kenapa harus tahu FP?

Di dalam penulisan bahasa pemrograman modern (seperti Dart) dan terutama saat kamu membangun aplikasi layar HP menggunakan *Flutter* nantinya, kamu akan **sangat sering** menemui gaya penulisan FP. 

Aksi seperti menekan tombol di layar HP akan dikendalikan oleh fungsi yang dikirim ke dalam fungsi lainnya. Memahami struktur FP akan membuat kodemu jauh lebih ringkas, elegan, dan sangat tahan terhadap risiko *bug* atau error logika.

Pada halaman-halaman berikutnya, kita akan menyelami tiga jurus utama dari Functional Programming: *Anonymous Function*, *Higher-Order Function*, dan *Closures*.
