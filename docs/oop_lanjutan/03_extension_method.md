# Extension Method

Pernahkah kamu bekerja menggunakan tipe data resmi bawaan Dart (seperti tipe teks `String` atau tipe angka `int`), dan kamu tiba-tiba berpikir: *"Andai saja ada fungsi instan di dalam String untuk menghitung jumlah suku katanya."*

Karena `String` adalah tipe data sakral bawaan dari bahasa pemrograman Dart, kita tentu tidak bisa (dan tidak boleh) menembus masuk lalu mengedit kerangka kode sumber aslinya. 

Nah, **Extension Method** diciptakan untuk menjawab kebutuhan tersebut. Fitur ini memungkinkan kita menyuntikkan (menambahkan) fungsi baru ke dalam class atau tipe data apa pun yang sudah ada sebelumnya tanpa harus mengubah satu baris pun isi kode aslinya.

**Analogi:** Bayangkan kamu memiliki mesin HP keluaran lama. HP dari pabrik aslinya tidak punya fitur anti-air. Namun, kamu kemudian membeli dan memasang alat *casing tambahan*. Setelah alat itu terpasang erat, HP lamamu tiba-tiba punya kemampuan baru untuk dipakai menyelam, tanpa perlu repot membongkar kerangka mesin di dalam HP-nya.

## Cara Menggunakan Extension

Gunakan kata kunci `extension`, lalu berikan nama extension-nya, diikuti dengan kata kunci `on` (pada tipe data apa fitur ini akan disuntikkan).

```dart
// Menyuntikkan fitur tambahan ke dalam tipe data 'int' (angka bulat) bawaan Dart
extension FiturTambahanAngka on int {
  
  // Kita membuat method baru untuk mengalikan angkanya sendiri dengan 100.
  // Kata kunci 'this' merujuk pada nilai asli dari angka int itu sendiri.
  int kaliSeratus() {
    return this * 100;
  }
}

void main() {
  int angkaBiasa = 5;
  
  // Ajaib! Sekarang semua variabel bertipe int di program kita 
  // memiliki akses ke sebuah method resmi baru bernama kaliSeratus()
  int hasil = angkaBiasa.kaliSeratus();
  
  print(hasil); // Hasil yang keluar: 500
}
```

Fitur Extension ini sangat digemari karena membuat kode menjadi sangat cantik. Fungsi-fungsi buatan pribadi akan terasa senatural fitur asli bawaan bahasa Dart.
