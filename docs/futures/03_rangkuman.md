# Rangkuman Futures

**Asynchronous Programming** (Pemrograman Asinkron) adalah teknik mutlak nan krusial yang wajib dikuasai oleh setiap programmer Flutter. Teknik ini menjadi senjata utama untuk mencegah layar aplikasi menjadi macet tidak bisa disentuh (*freeze*) saat aplikasi tersebut terpaksa sedang menunggu proses berat yang memakan waktu cukup lama (seperti mengunduh rentetan gambar kualitas tinggi atau berinteraksi meminta data ke *database* pusat).

Berikut adalah ringkasan padat dari seluruh materi Futures yang harus selalu kamu simpan kuat-kuat di dalam ingatanmu:

1. **Synchronous vs Asynchronous**

    - **Synchronous**: Dieksekusi secara berurutan, tegak lurus, dan sangat ketat. Baris perintah di bawah harus rela mengantre diam hingga perintah di baris atas selesai dikerjakan.
    - **Asynchronous**: Dieksekusi secara pintar tanpa memblokir urutan baris. Program akan langsung melompat cerdas untuk mengerjakan perintah di baris bawah, sambil tetap sabar menunggu proses baris atas selesai berjalan mandiri di latar belakang layar.

2. **Objek Future (Sang Kertas Struk Antrean)**
   
    - Pada saat fungsi beraliran *asynchronous* pertama kali dipanggil, ia akan dengan kecepatan tinggi langsung mengembalikan sebuah pelindung "struk antrean" yang wujud nyatanya disebut dengan tipe data `Future`.
    - `Future` secara absolut memiliki 3 siklus fase kehidupan:
        - **Uncompleted**: Masa di mana ia masih sedang sibuk di dalam proses, dan belum ada hasil yang matang.
        - **Completed with Data**: Masa kemenangan, di mana proses sukses dan hasil datanya berhasil ditarik didapatkan.
        - **Completed with Error**: Masa kegagalan, selesai dikerjakan namun secara menyedihkan sistemnya gagal (misalnya sinyal internet tiba-tiba terputus).

3. **Duet Kata Kunci Ajaib `async` dan `await`**
   
    - Merupakan gaya dan aturan penulisan paling modern standar perusahaan (*Best Practice*) untuk menangani keliaran objek Future.
    - Keajaibannya mampu membuat baris kode asinkron yang tadinya rumit bersarang, menjadi terlihat sangat lurus, rapi, dan mudah dibaca layaknya baris kode *synchronous* biasa.
    - **`async`**: Merupakan syarat segel wajib yang harus ditempelkan pada peresmian nama fungsi utama, guna memberitahu mesin pengolah secara tegas bahwa di dalam ruangan fungsi ini nanti terdapat proses *delay* yang memakan waktu.
    - **`await`**: Merupakan saklar "rem tangan" tebal yang mutlak ditaruh persis di depan panggilan objek Future, berguna untuk menekan dan menyuruh program "menunggu membeku" tepat di baris tersebut sampai hasil datanya benar-benar dikirimkan secara matang.

4. **Benteng Penanganan Error**
   
    - Pada saat kamu sudah menggunakan gaya `async/await`, pastikan selalu membungkus panggilan datamu menggunakan blok pertahanan **`try-catch`** konvensional. Ini digunakan untuk jaring keamanan menangkap lontaran error liar jika ternyata Future berakhir dengan tragis membawa status *Completed with Error*.

Bab istimewa ini pada dasarnya merupakan "ujian kelulusan" sekaligus jembatan pintu keluar terakhirmu di dalam kurikulum bahasa Dart murni, sebelum pada akhirnya kamu benar-benar melangkahkan kaki terjun ke dalam dunia cerah pembuatan *User Interface* (antarmuka grafis) yang dinamis menggunakan *framework* kebanggaan, **Flutter**. 

Pastikan seluruh logika inti *Asynchronous* ini sudah tertanam menjadi insting kuat di kepalamu!
