# Pengenalan Futures (Asynchronous)

Sejauh ini, seluruh program yang kita pelajari dan kita buat selalu berjalan secara **Synchronous** (Sinkron/berurutan). Artinya, mesin internal Dart akan selalu membaca dan mengeksekusi baris kode dari atas ke bawah, persis satu demi satu secara ketat. Jika baris ke-3 membutuhkan waktu pengerjaan yang lama, maka baris ke-4 dan seterusnya terpaksa harus mengantre diam menunggu.

Namun di dalam dunia nyata pengembangan aplikasi, banyak sekali kejadian yang memakan waktu dan tidak bisa dipastikan kapan selesainya. Contoh utamanya adalah mengambil foto dari server internet atau membaca data panjang dari dalam *database*. 

Jika programmu menunggu proses unduhan tersebut secara *Synchronous* (berhenti total menunggu), maka layar aplikasi Flutter-mu akan terlihat **macet total (hang/freeze)**. Pengguna tidak akan bisa memencet tombol apapun di layar selama foto tersebut belum selesai diunduh.

Di sinilah kita sangat membutuhkan pahlawan bernama **Asynchronous Programming**, dengan mengandalkan sebuah objek sakti bernama **Future**.

## Synchronous vs Asynchronous

**Analogi Synchronous:**
Kamu pergi ke sebuah warung makan tradisional, memesan nasi goreng, dan sistem warung tersebut menyuruhmu berdiri tegak terus menerus di depan kasir sampai nasi gorengmu selesai dimasak. Akibatnya, antrean pembeli di belakangmu menjadi macet tidak bisa memesan makanan sama sekali karena kamu diam menghalangi jalan di depan kasir.

**Analogi Asynchronous (Menggunakan Future):**
Kamu pergi ke sebuah restoran cepat saji moderen. Kamu memesan burger, membayar di kasir, dan sang kasir dengan sigap memberimu sebuah **Nomor Antrean (Future)** berwujud kertas fisik. 

Karena kamu sudah memegang struk nomor antrean, kamu bebas minggir dari kasir, duduk nyaman di meja, dan bermain HP (program terus berjalan). Kasir pun bisa dengan bebas melayani pembeli lain di belakangmu. 
Ketika burgermu sudah benar-benar jadi, barulah kasir akan berteriak memanggil nomormu (masa depan/Future terpenuhi), lalu kamu berjalan untuk mengambil burgermu.

## Kenapa dinamakan "Future"?

Di dalam bahasa Dart, seluruh operasi yang sifat kerjanya *asynchronous* (operasi yang berjalan di latar belakang tanpa menghentikan sisa baris kode di bawahnya) akan selalu mengembalikan sebuah objek pelindung dengan tipe data bernama `Future`.

Sesuai terjemahan namanya, `Future` melambangkan **janji akan adanya sebuah nilai atau data di masa depan**. Ia berfungsi persis seperti struk nomor antrean yang membuktikan bahwa kamu sedang menunggu sebuah pesanan data, dan pesanan itu pasti akan tiba nanti entah kapan.

Pada halaman-halaman selanjutnya, kita akan membedah tuntas anatomi dari struk antrean (Future) ini dan bagaimana cara terbaik kita menggunakannya.
