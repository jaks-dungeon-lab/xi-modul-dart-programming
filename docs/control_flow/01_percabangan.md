# Percabangan (If, Else, Switch)

Percabangan memungkinkan programmu mengambil keputusan. Program akan memeriksa sebuah kondisi (benar atau salah), lalu menjalankan blok kode yang sesuai.

## If dan Else

**Analogi:** Ini persis seperti **lampu lalu lintas** di perempatan jalan. *Jika* (if) lampu hijau, kamu jalan. *Selain itu jika* (else if) lampu kuning, kamu bersiap. *Selain itu* (else) yang artinya lampu merah, kamu berhenti.

```dart
void main() {
  int nilaiUjian = 85;

  if (nilaiUjian >= 90) {
    print('Nilai kamu A. Luar biasa!');
  } else if (nilaiUjian >= 75) {
    print('Nilai kamu B. Bagus!');
  } else {
    print('Kamu harus ikut remedial.');
  }
}
```

- `if` memeriksa kondisi pertama.
- `else if` memeriksa kondisi tambahan jika kondisi sebelumnya salah.
- `else` menangkap semua kemungkinan sisa jika semua kondisi di atasnya salah.

## Switch dan Case

Saat kamu punya banyak sekali opsi pasti (bukan rentang nilai seperti > atau <), `switch` jauh lebih rapi daripada membuat rentetan `if-else` yang panjang.

**Analogi:** Seperti **mesin penjual otomatis (Vending Machine)**. Kamu menekan tombol tertentu (misal tombol 2), lalu mesin langsung mencari laci nomor 2 dan menjatuhkan minumannya.

```dart
void main() {
  String nilaiHuruf = 'B';

  switch (nilaiHuruf) {
    case 'A':
      print('Sempurna!');
      break;
    case 'B':
      print('Bagus!');
      break;
    case 'C':
      print('Cukup.');
      break;
    default:
      print('Nilai tidak dikenali.');
  }
}
```

- `case` adalah opsi atau laci-lacinya.
- `break` wajib ditulis untuk menghentikan mesin mencari laci lain setelah opsi yang benar ditemukan.
- `default` sama seperti `else`, berjalan jika tidak ada opsi yang cocok.
