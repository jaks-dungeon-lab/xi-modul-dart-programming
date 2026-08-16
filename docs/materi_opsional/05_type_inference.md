# Type Inference

Jika kamu memiliki pengalaman mempelajari bahasa pemrograman generasi lawas (seperti bahasa C atau Java versi lama), kamu mungkin pernah terbiasa dipaksa untuk terus-menerus menuliskan tipe data secara persis setiap kali membuat variabel baru. Tradisi lama ini membuat kodemu terasa sangat kaku dan bertele-tele.

Di dalam ekosistem bahasa Dart, terdapat sebuah teknologi cerdas yang bekerja mengamati kodemu dari balik layar, teknologi ini dinamakan **Type Inference** (Penebakan Tipe Data). 

**Analogi:** Proses ini sangat mirip seperti seorang pelayan restoran profesional yang melihatmu memesan "Sepiring Nasi Goreng Spesial". Sang pelayan di otaknya otomatis langsung mencatat ke dalam bon sebagai "Makanan", tanpa perlu kamu bentak dan kamu tegaskan dengan kalimat, *"Hai pelayan, ingat ya, nasi goreng ini adalah tipe data makanan!"*

## Bagaimana Dart Menebak?

Ketika kamu mendeklarasikan sebuah variabel dengan kata kunci pemanggil ringan seperti `var` atau `final` dan kamu **langsung mengisinya dengan sebuah nilai**, mesin internal Dart akan diam-diam menoleh melihat wujud nilai yang tertulis di sebelah kanan tanda sama dengan (`=`), lalu dengan ajaib ia langsung mengunci tipe data variabel tersebut secara permanen.

```dart
void main() {
  // Mesin Dart melihat ada teks 'Gatotkaca' di sebelah kanan.
  // Secara gaib ia diam-diam mengunci variabel ini sebagai String.
  var namaPahlawan = 'Gatotkaca';
  
  // Mesin Dart melihat sebuah angka bulat.
  // Secara instan ia mengunci variabel ini menjadi int.
  final tahunRilis = 2024;
  
  // Error! Dart akan langsung menolak karena ia sudah tahu di awal bahwa 'namaPahlawan' adalah String.
  // namaPahlawan = 100; 
}
```

## Kapan Boleh, Kapan Tidak Boleh?

**Gunakan `var` atau `final`** (Berikan izin bagi mesin yang menebak):
- Jika isi datanya langsung diberikan secara jelas di baris dan waktu yang sama.
- Sangat diwajibkan saat kamu melakukan proses cetak instansiasi objek (*Object Instantiation*), contohnya: `var player1 = Ksatria();` (Perhatikan betapa lebih rapinya tulisan ini dibandingkan gaya bahasa lama `Ksatria player1 = Ksatria();`).

**Tulis tipe data secara Eksplisit** (Larang mesin untuk menebak):
- Pada saat kamu membuat "variabel keranjang kosongan" yang isinya baru akan kamu isi nanti di baris bawah. Jika kamu hanya menulis `var skor;`, Dart akan sangat kebingungan lalu menetapkannya sebagai status `dynamic` yang sangat tidak aman.
- Wajib digunakan pada bagian kolom *Parameter* sebuah fungsi (agar programmer teman satu timmu tahu persis jenis data apa yang wajib dilemparkan ke dalam fungsi tersebut).

Menguasai seni kapan harus diam membiarkan Dart menggunakan `var` dan kapan harus tegas menuliskan tipe data, akan membuat kelas gaya tulisan kodemu langsung meloncat setara dengan keindahan baris kode para programmer profesional.
