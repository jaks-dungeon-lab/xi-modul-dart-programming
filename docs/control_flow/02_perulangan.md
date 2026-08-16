# Perulangan (For dan While)

Perulangan (Looping) digunakan untuk mengeksekusi blok kode yang sama berkali-kali tanpa harus menulisnya berulang-ulang secara manual.

## For Loop

Gunakan `for` ketika kamu **sudah tahu pasti** berapa kali perulangan itu harus dilakukan.

**Analogi:** Seperti dihukum guru olahraga untuk **lari keliling lapangan sebanyak 5 putaran**. Kamu mulai dari putaran 1, lalu berlari, menghitung, dan berhenti saat mencapai putaran ke-5.

```dart
void main() {
  // Mulai dari i=1; terus berlari selama i <= 5; setiap putaran i bertambah 1
  for (int i = 1; i <= 5; i++) {
    print('Lari putaran ke-$i');
  }
}
```

## While Loop

Gunakan `while` ketika kamu **belum tahu pasti** berapa kali perulangan dilakukan, tapi kamu tahu **syarat berhentinya**.

**Analogi:** Seperti **makan**. Kamu tidak menghitung sudah berapa suap nasi yang kamu makan. Kamu hanya akan terus menyuap nasi *selama (while)* perutmu masih lapar.

```dart
void main() {
  bool perutLapar = true;
  int jumlahSuapan = 0;

  while (perutLapar == true) {
    jumlahSuapan++;
    print('Makan suapan ke-$jumlahSuapan');
    
    // Berhenti makan setelah 3 suapan
    if (jumlahSuapan == 3) {
      print('Kenyang!');
      perutLapar = false; // Ini akan menghentikan perulangan
    }
  }
}
```
