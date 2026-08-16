# Inheritance (Pewarisan)

**Inheritance** adalah salah satu pilar OOP yang paling kuat dan sering digunakan. Konsep ini memungkinkan sebuah class baru untuk mewarisi (mendapatkan) semua sifat (properties) dan aksi (method) dari class yang sudah ada sebelumnya.

- **Parent Class / Super Class**: Class utama yang sifatnya akan diwariskan.
- **Child Class / Sub Class**: Class baru yang menerima warisan tersebut.

**Analogi:**
Seorang Ayah (Parent Class) memiliki warna mata cokelat dan kemampuan menyetir mobil. Sang Anak (Child Class) secara otomatis mewarisi warna mata cokelat dan kemampuan menyetir dari ayahnya sejak lahir, tanpa perlu diajari dari nol. Menariknya, Sang Anak juga bisa punya kemampuannya sendiri (misal: bisa main gitar) yang ayahnya tidak bisa lakukan.

## Menggunakan kata kunci `extends`

Di Dart, kita menggunakan kata kunci `extends` untuk menandakan bahwa sebuah class adalah turunan dari class lain.

```dart
// Parent Class (Class Induk)
class Hewan {
  String nama;
  
  Hewan(this.nama);
  
  void bernapas() {
    print('$nama sedang bernapas...');
  }
}

// Child Class (Class Turunan)
class Kucing extends Hewan {
  // Menggunakan sintaks modern super.nama untuk melempar data langsung ke Parent Class.
  Kucing(super.nama);
  
  // Method khusus Kucing yang tidak dimiliki Hewan secara umum
  void mengeong() {
    print('$nama mengeong: Meoooong!');
  }
}

void main() {
  var oyen = Kucing('Oyen');
  
  // Oyen bisa bernapas (warisan dari orang tuanya, yaitu Hewan)
  oyen.bernapas(); 
  
  // Oyen bisa mengeong (kemampuannya sendiri)
  oyen.mengeong(); 
}
```

## Method Overriding

Terkadang, sang anak ingin melakukan suatu pekerjaan dengan gaya yang berbeda dari ayahnya. Kita bisa menimpa atau memodifikasi fungsi bawaan dari Parent Class menggunakan anotasi `@override`.

```dart
class Burung extends Hewan {
  Burung(super.nama);
  
  // Menimpa fungsi bernapas bawaan dari Hewan
  @override
  void bernapas() {
    print('$nama bernapas menggunakan pundi-pundi udara saat terbang!');
  }
}
```
