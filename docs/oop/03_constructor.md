# Constructor

Pada halaman sebelumnya, kita membuat object kosong lalu mengisi datanya satu per satu secara manual (contoh: `kucingku.nama = 'Oyen'`). Bayangkan jika ada 20 data yang harus diisi, tentu akan sangat melelahkan. **Constructor** hadir untuk membuat proses pengisian data ini menjadi instan.

**Constructor** adalah method spesial yang akan **otomatis dijalankan** pada detik pertama sebuah Object dibuat dari cetakannya.

**Analogi:** Seperti memesan minuman di restoran. Daripada pelayan memberikan gelas kosong lalu kamu disuruh menuang air dan mencampur gula sendiri (manual), lebih baik kamu menyebutkan pesananmu di awal ("Es teh manis satu!"), dan pelayan akan membawakan gelas yang **sudah langsung terisi** (instan).

## Cara Membuat Constructor

Satu aturan baku: Nama constructor **wajib sama persis** dengan nama Class-nya.

```dart
class Kucing {
  String nama;
  String warna;

  // Ini adalah Constructor
  // this.nama artinya menyalin data inputan langsung ke properties 'nama'
  Kucing(this.nama, this.warna);
}

void main() {
  // Membuat object sekaligus MENGISI datanya dalam satu baris!
  var kucing1 = Kucing('Oyen', 'Oranye');
  var kucing2 = Kucing('Moli', 'Hitam');

  print(kucing1.nama); // Hasil: Oyen
}
```

## Named Parameters di Constructor

Jika sebuah class punya properti yang sangat banyak (misal lebih dari 3), kita bisa memakai kurung kurawal `{}` pada parameter constructor. Ini dinamakan Named Parameters. Tujuannya agar kita bisa memanggil datanya dengan menyebut nama propertinya secara spesifik, sehingga isiannya tidak akan terbalik-balik.

Tambahkan kata kunci `required` jika data tersebut sifatnya wajib diisi.

```dart
class Kucing {
  String nama;
  String warna;

  // Named Constructor dengan kurung kurawal
  Kucing({required this.nama, required this.warna});
}

void main() {
  // Sangat jelas terbaca dan tidak perlu takut urutannya tertukar!
  var kucingku = Kucing(warna: 'Putih', nama: 'Miko');
}
```
