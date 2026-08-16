# Built-in Types

Tipe data adalah aturan yang menentukan jenis isi yang boleh masuk ke dalam sebuah variabel. 

**Analogi:** Seperti wadah spesifik di dapur. Galon dipakai khusus benda cair, sedangkan toples dipakai khusus benda padat. Begitu juga data: teks harus masuk wadah teks, angka harus masuk wadah angka.

## Numbers (Angka)

Dart memiliki dua tipe data khusus untuk angka:
- **int**: Untuk menyimpan angka bilangan bulat (contoh: `10`, `-5`, `1000`).
- **double**: Untuk menyimpan angka pecahan atau desimal (contoh: `3.14`, `0.5`).

```dart
void main() {
  int umur = 16;
  double beratBadan = 55.5;
}
```

## Strings (Teks)

**String** digunakan untuk menyimpan teks (kata atau kalimat). Teks harus selalu diapit dengan tanda kutip tunggal (`'`) atau tanda kutip ganda (`"`).

```dart
void main() {
  String sekolah = 'SMK ICB';
  String pesan = "Selamat pagi teman-teman";
}
```

## Booleans (Logika)

**bool** adalah tipe data yang paling sederhana. Variabel ini hanya bisa menyimpan dua keadaan: `true` (benar) atau `false` (salah). Sangat berguna sebagai sakelar on/off dalam program.

```dart
void main() {
  bool sudahLulus = false;
  bool sedangBelajar = true;
}
```
