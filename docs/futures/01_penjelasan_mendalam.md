# Penjelasan Mendalam: Fase Kehidupan Futures

Ketika kamu memerintahkan program untuk menjalankan sebuah fungsi yang bersifat *asynchronous* (misalnya perintah untuk mengunduh foto besar dari internet), fungsi tersebut akan secara sangat instan (tanpa perlu menunggu fotonya selesai diunduh) memberimu sebuah objek **Future**.

Objek Future ini pada dasarnya mengalami perpindahan **tiga status fase utama** selama rentang masa hidupnya.

## 1. Uncompleted (Belum Selesai / Sedang Berjalan)
Pada detik pertama saat fungsi dipanggil, ia akan langsung mengembalikan sebuah objek Future yang menyandang status *Uncompleted*. 
**Analogi:** Ini adalah momen di mana kamu baru saja menerima kertas struk nomor antrean dari kasir. Pesanan burgermu saat ini masih sedang sibuk dimasak oleh koki di dapur.

## 2. Completed with Data (Selesai dan Berhasil)
Jika operasi berat yang memakan waktu tersebut ternyata sukses dituntaskan oleh mesin (misalnya foto dari server internet berhasil diunduh 100%), maka objek Future tersebut akan segera merubah statusnya menjadi *Completed*, dan ajaibnya ia akan membawa **Data** yang selama ini kamu tunggu-tunggu di dalamnya.
**Analogi:** Nomormu diteriakkan oleh koki, pesanan burgermu selesai dan diserahkan ke tanganmu dengan bentuk yang sempurna.

## 3. Completed with Error (Selesai namun Gagal)
Jika terjadi sebuah kendala teknis atau kecelakaan di tengah jalan (misalnya kabel internet komputermu tiba-tiba dicabut, atau server pusat ternyata mati), maka objek Future tetap akan mengabarkan bahwa ia sudah *Completed* (selesai bekerja), namun ia sama sekali tidak membawa data apapun, melainkan membawa pesan **Error**.
**Analogi:** Nomormu dipanggil oleh kasir, tapi kamu bukan diberi burger. Sang kasir malah meminta maaf dan memberitahumu bahwa stok daging sapi di restoran ternyata kebetulan baru saja habis.

---

## Cara Tradisional Mengambil Data Future: `.then()` dan `.catchError()`

Di bahasa Dart versi lama, cara standar programmer mengawasi fase status Future dan mengambil data aslinya adalah dengan merangkai metode `.then()` (yang akan dipicu otomatis jika berhasil) dan metode `.catchError()` (yang akan menyala jika gagal).

```dart
// Kita membuat sebuah fungsi simulasi yang pura-pura memakan waktu 2 detik
// Perhatikan bahwa tipe kembaliannya BUKAN String biasa, melainkan Future<String>
Future<String> pesanBurgerDiKasir() {
  return Future.delayed(Duration(seconds: 2), () {
    return 'Ini burger super enak pesanan Anda!'; // Simulasi jika berhasil
  });
}

void main() {
  print('1. Saya berdiri memesan burger ke kasir...');
  
  // Kita mulai memanggil fungsi asynchronous
  pesanBurgerDiKasir()
    .then((hasilDariDapur) {
      // PERHATIKAN: Baris ini HANYA akan dijalankan nanti saat burgernya sudah jadi 
      // (Fase Completed with Data)
      print('3. Asyik nomorku dipanggil! Kasir bilang: $hasilDariDapur');
    })
    .catchError((errorYangTerjadi) {
      // PERHATIKAN: Baris ini HANYA akan dijalankan jika tiba-tiba terjadi kegagalan sistem
      // (Fase Completed with Error)
      print('Waduh pesananku gagal: $errorYangTerjadi');
    });

  // Karena sifatnya Asynchronous, baris di bawah ini akan TEREKSEKUSI DULUAN 
  // tanpa perlu repot menunggu pesanan burger selesai!
  print('2. Saya berjalan menjauhi kasir, duduk santai sambil main HP...');
}
```

Walaupun cara tradisional di atas berfungsi sempurna, tulisan kodenya akan berubah menjadi sangat curam dan membingungkan (*callback hell*) jika di dalam sebuah aplikasi kita memiliki sangat banyak proses pengunduhan data yang berurutan. 

Itulah alasan utama mengapa para kreator Dart menghadirkan gaya penulisan modern luar biasa bernama `async` dan `await` yang akan kita pelajari tuntas di halaman berikutnya.
