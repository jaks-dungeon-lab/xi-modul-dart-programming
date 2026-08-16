# Operators

Operator digunakan untuk memanipulasi atau menghitung data yang ada di dalam variabel.

**Analogi:** Operator adalah perkakas tukang. Tanda tambah (`+`) seperti palu untuk menggabungkan dua benda. Tanda kurang (`-`) seperti gergaji untuk memotong sebagian.

## Operator Aritmatika

Digunakan untuk melakukan hitungan matematika biasa layaknya kalkulator.

- `+` (Tambah)
- `-` (Kurang)
- `*` (Kali)
- `/` (Bagi)

```dart
void main() {
  int hargaAwal = 10000;
  int diskon = 2000;
  
  int hargaAkhir = hargaAwal - diskon;
  print(hargaAkhir); // Hasilnya: 8000
}
```

## Operator Perbandingan

Digunakan untuk membandingkan dua buah nilai. Hasil akhir dari operator perbandingan selalu berupa nilai logika (`true` atau `false`).

- `==` (Sama dengan)
- `!=` (Tidak sama dengan)
- `>` (Lebih besar dari)
- `<` (Lebih kecil dari)

```dart
void main() {
  int umur = 16;
  bool bolehBawaMotor = umur >= 17; // Hasilnya akan false
}
```
