# Properties dan Method

Setelah kita punya cetakan (Class) yang kosong, kita perlu mengisinya. Sebuah class umumnya berisi dua hal utama: **Properties** dan **Method**.

## Properties (Sifat / Data)

Properties adalah variabel yang menempel di dalam class. Ia mendeskripsikan ciri-ciri, status, atau data yang dimiliki oleh object tersebut.

**Analogi**: Sifat-sifat fisik kucing. Kucing memiliki *nama*, *warna bulu*, dan *berat badan*.

```dart
class Kucing {
  // Ini adalah Properties
  String nama = '';
  String warna = '';
  int berat = 0;
}
```

## Method (Tindakan / Aksi)

Method adalah fungsi (`function`) yang dibuat di dalam class. Ia mendeskripsikan tindakan apa saja yang bisa dilakukan oleh object tersebut.

**Analogi**: Aksi kucing. Kucing bisa melakukan tindakan seperti *makan*, *tidur*, dan *mengeong*.

```dart
class Kucing {
  String nama = '';

  // Ini adalah Method
  void mengeong() {
    print('$nama berkata: Meoooong!');
  }
}
```

## Mengakses Properties dan Method

Untuk mengakses data (properties) atau menyuruh object melakukan aksi (method), kita menggunakan operator tanda titik (`.`).

```dart
void main() {
  var kucingku = Kucing();
  
  // Mengisi data ke dalam properties
  kucingku.nama = 'Oyen';
  kucingku.warna = 'Oranye';
  
  // Menyuruh object memanggil method
  kucingku.mengeong(); // Hasil yang tercetak: Oyen berkata: Meoooong!
}
```
