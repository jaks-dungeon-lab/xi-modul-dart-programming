# Async & Await

Teknik penulisan kode menggunakan rantai `.then()` memang sangat tangguh, namun hal itu seringkali menyebabkan struktur baris kode kita menjadi bersarang-sarang dan menjorok tajam ke dalam (kondisi ini biasa disebut sebagai *callback hell* oleh para programmer). 

Untuk mengatasi mimpi buruk keindahan penulisan kode ini, Dart memperkenalkan dua buah kata kunci ajaib modern: **`async`** dan **`await`**.

Dengan kekuatan duet maut `async` dan `await`, kita bisa memaksa program untuk **berhenti sejenak dan menunggu** hingga sebuah proses *asynchronous* benar-benar matang selesai, namun hebatnya kita dapat menuliskannya dengan gaya penulisan lurus, rapi ke bawah, dan sangat mudah dibaca (persis seperti kita sedang menulis kode *synchronous* biasa).

## Cara Menggunakan Secara Tepat

1. **`async`**: Tambahkan kata kunci wajib ini persis sebelum kurung kurawal pembuka `{` dari sebuah blok fungsi. Kehadiran kata ini berfungsi seperti rambu lalu lintas yang memberitahu mesin Dart bahwa: *"Tolong awas, di dalam ruangan fungsi ini nanti akan ada proses berat yang membutuhkan waktu (asynchronous)"*.
2. **`await`**: Letakkan kata ajaib ini persis di depan fungsi yang mengembalikan objek Future. Kata ini murni berfungsi sebagai "Rem Tangan" sakti yang akan seketika membekukan eksekusi baris kode di titik tersebut, sampai proses pengunduhan Future-nya selesai memberikan hasil (baik itu hasil berhasil maupun gagal).

```dart
// Kita siapkan sebuah fungsi simulasi yang sengaja memakan waktu lambat 2 detik
Future<String> ambilDataRahasiaDariInternet() {
  return Future.delayed(Duration(seconds: 2), () {
    return 'File Dokumen Data Rahasia Negara berhasil diunduh';
  });
}

// Tambahkan kata kunci 'async' di ujung penamaan fungsi utama
void main() async {
  print('1. Memulai proses pengunduhan panjang...');
  
  // Karena kita dengan tegas memasang rem 'await', program kita akan BERHENTI MENUNGGU 
  // tepat di baris ini secara paksa, sampai 2 detik berlalu dan si Future memberikan data aslinya
  String hasilDownload = await ambilDataRahasiaDariInternet();
  
  // Baris ke-3 di bawah ini TIDAK AKAN PERNAH dicetak sebelum baris ke-2 di atas 100% selesai
  print('2. Pengunduhan beres! Isi pesannya: $hasilDownload');
}
```

## Menangani Potensi Error dengan Blok `try-catch`

Karena kini kita menggunakan gaya penulisan baris kode biasa yang rapi berurutan ke bawah, kita secara otomatis tidak bisa lagi menempelkan fungsi penangkap `.catchError()`. 

Sebagai jurus penggantinya, kita akan memanggil kembali teknik pengamanan **`try-catch`** klasik tangguh yang sudah pernah kita pelajari di bab Exceptions awal.

```dart
Future<void> main() async {
  print('Memulai uji coba mengunduh file besar...');
  
  try {
    // Kita "mencoba" mengerem waktu dan memaksanya menunggu hasil unduhan...
    String hasilDownload = await ambilDataRahasiaDariInternet();
    print('Sistem Berhasil: $hasilDownload');
    
  } catch (errorYangTerjadi) {
    // Jika ternyata di tengah masa menunggu mesin servernya terbakar, 
    // kita tangkap luapan errornya di sini agar aplikasi tidak crash!
    print('Gagal mengunduh sama sekali! Laporan pesan error: $errorYangTerjadi');
  }
}
```

### Sebuah Kewajiban Mutlak Industri

Gaya penulisan kombinasi `async` dan `await` adalah **standar industri mutlak tak tertulis** pada era pengembangan aplikasi saat ini. Hampir 99% logika proses pengambilan data krusial dari API server internet, membaca sensor GPS HP, atau menarik data dari *database* di dalam framework Flutter nantinya akan sepenuhnya mengandalkan teknik rapi dan elegan ini.
