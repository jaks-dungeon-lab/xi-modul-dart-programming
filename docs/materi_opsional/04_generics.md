# Generics

**Generics** adalah salah satu fitur paling mengagumkan di dalam sistem tipe data Dart. Ciri utamanya yang paling terlihat adalah keberadaan penggunaan simbol kurung sudut (biasanya berupa huruf kapital `<T>`, `<E>`, dsb.). 

Generics memungkinkan kita untuk menciptakan satu buah class atau satu buah fungsi yang **sangat fleksibel menerima tipe data apa pun** secara dinamis, namun secara ajaib ia **tetap sangat ketat dan aman** (*type-safe*) pada saat program sedang berjalan.

**Analogi:** Bayangkan kamu memiliki sebuah "Kardus Ajaib" (Generic Class). Saat kamu membelinya dari pabrik, kardus ini bebas digunakan untuk menyimpan barang apapun. 
Namun, sesaat sebelum kamu mulai menggunakannya, kamu menempelkan label bertuliskan `<Buku>`. Semenjak detik itu, kardus ajaibmu akan langsung menolak keras dan mengunci rapat jika kamu mencoba memasukkan "Baju" ke dalamnya. Ia fleksibel sebelum dilabeli, tapi menjadi sangat disiplin setelah dilabeli.

## Kenapa kita sangat butuh Generics?

Bayangkan jika fitur Generics tidak ada. Saat kamu ingin membuat program brankas penyimpanan, kamu terpaksa harus menulis kodenya berulang-ulang dari nol untuk membuat `BrankasAngka`, `BrankasTeks`, `BrankasDesimal`. Sangat membuang waktu dan memanjangkan baris kodemu. 

Sebaliknya, jika kamu nekat menggunakan tipe `dynamic` agar brankasmu bisa menerima data apa saja, kodemu memang pendek, tapi ia menjadi tidak aman! Kamu bisa saja suatu saat tidak sengaja memasukkan angka uang ke dalam brankas yang sebetulnya sejak awal kamu siapkan untuk dokumen teks, dan programmu akan meledak (error).

## Contoh Membuat Generic Class

Gunakan simbol `<T>` (singkatan universal dari *Type*) persis di sebelah nama class.

```dart
// Class ini sekarang resmi menjadi Kardus Ajaib!
class Brankas<T> {
  // Variabel 'isi' tipe datanya tidak pasti, ia akan menyesuaikan dengan nilai T
  T isi;
  
  Brankas(this.isi);
  
  void cekIsi() {
    print('Brankas ini sedang menyimpan data: $isi');
  }
}

void main() {
  // Kita membuat brankas baru, lalu MELABELINYA KHUSUS untuk String (teks)
  var brankasRahasia = Brankas<String>('Dokumen Perjanjian');
  brankasRahasia.cekIsi();
  
  // Jika kamu mencoba memaksa: brankasRahasia.isi = 100;
  // Sistem IDE-mu akan langsung mencoret merah (error), karena brankas ini sudah dikunci untuk String!
  
  // Sebaliknya, kita bisa dengan mudah membuat brankas lain khusus untuk int (angka)
  var brankasUang = Brankas<int>(5000000);
  brankasUang.cekIsi();
}
```

## Generics pada Fungsi

Selain disematkan pada Class, fitur luar biasa ini juga sangat sering diletakkan pada fungsi agar fungsi tersebut mampu mengolah tipe data apa pun yang dilemparkan kepadanya secara aman.

```dart
// Fungsi ini secara otomatis akan mengembalikan data yang SAMA PERSIS tipenya dengan data masukannya
T cetakDanKembalikan<T>(T dataMasukan) {
  print('Sedang memproses data yang dilempar: $dataMasukan');
  return dataMasukan; // Tipe datanya aman terjaga!
}
```
