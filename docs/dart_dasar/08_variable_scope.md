# Variable Scope

*Scope* (ruang lingkup) adalah batas wilayah di mana sebuah variabel bisa dibaca atau digunakan oleh program. Di Dart, wilayah ini dibatasi oleh tanda kurung kurawal `{ }`.

**Analogi:** Sama seperti batas peraturan rumah. Perabot yang ada di ruang tamu rumahmu (*global scope*) bisa dilihat dan dipakai oleh semua anggota keluarga. Tapi barang pribadi yang dikunci di laci kamarmu (*local scope*) tidak bisa dilihat atau diambil oleh penghuni kamar sebelah.

## Local vs Global Scope

Variabel yang dibuat di dalam sebuah fungsi (berada di dalam `{ }`) tidak akan pernah bisa dikenali oleh fungsi lain di luarnya.

```dart
// Ini variabel 'global', ada di luar semua kurung
int angkaGlobal = 100; 

void fungsiA() {
  // Ini variabel 'lokal', hanya milik fungsiA
  int angkaLokal = 50; 
  print(angkaGlobal); // Boleh, semua orang bisa akses global
}

void main() {
  print(angkaGlobal); // Boleh, sukses!
  
  // print(angkaLokal); 
  // Error! 'main' tidak tahu ada variabel bernama 'angkaLokal'
  // karena itu milik fungsiA secara eksklusif.
}
```
