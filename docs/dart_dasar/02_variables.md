# Variables

Variabel adalah tempat untuk menyimpan data sementara di dalam memori komputer. Jika kamu menggunakan perintah `var`, Dart akan otomatis menebak tipe datanya berdasarkan isi yang kamu berikan.

**Analogi:** Anggap variabel sebagai **kotak kardus** kosong. Label di luar kotak adalah nama variabel, dan barang di dalamnya adalah isinya. Jika kotaknya berlabel `umur`, maka kamu menaruh angka di dalamnya.

```dart
void main() {
  var nama = 'Budi';
  var umur = 16;
  
  // Isi variabel bisa diubah kapan saja
  umur = 17; 
  
  print(nama);
  print(umur);
}
```

## Constants & Final

Kadang ada data yang sifatnya tetap dan tidak boleh diubah (misalnya nilai pi, atau tanggal lahir). Agar aman dari perubahan tidak disengaja, gunakan kata kunci `final` atau `const`.

**Analogi:** Seperti kotak kardus yang sudah dilakban mati. Sekali diisi, kotaknya tidak bisa dibuka lagi untuk diganti isinya.

```dart
void main() {
  final kotaKelahiran = 'Bandung';
  const nilaiPi = 3.14;
  
  // kotaKelahiran = 'Jakarta'; // Baris ini akan menyebabkan error!
}
```
