# Break dan Continue

Saat berada di dalam perulangan (`for` atau `while`), kamu bisa menginterupsi jalannya putaran menggunakan perintah khusus: `break` dan `continue`.

## Break (Berhenti Paksa)

`break` akan menghentikan seluruh perulangan saat itu juga, tidak peduli apakah putaran sebenarnya belum selesai. Program akan langsung melompat keluar dari blok perulangan.

**Analogi:** Seperti **tombol stop darurat** di mesin *treadmill*. Saat dipencet, mesin langsung berhenti total walau target larimu belum tercapai.

```dart
void main() {
  for (int i = 1; i <= 10; i++) {
    if (i == 5) {
      print('Darurat! Berhenti di angka 5.');
      break; // Menghentikan seluruh perulangan
    }
    print('Angka $i');
  }
  // Hasil yang tercetak hanya 1, 2, 3, 4
}
```

## Continue (Lewati Satu Putaran)

`continue` tidak menghentikan seluruh perulangan. Ia hanya menghentikan putaran yang sedang berjalan saat itu, lalu langsung melompat ke putaran berikutnya.

**Analogi:** Seperti **tombol skip (next)** di pemutar musik. Saat ada lagu yang tidak kamu suka, kamu pencet skip. Lagu itu berhenti dimainkan, tapi *playlist* tetap berlanjut memutar lagu berikutnya.

```dart
void main() {
  for (int i = 1; i <= 5; i++) {
    if (i == 3) {
      print('Melewati angka 3...');
      continue; // Lewati sisa kode di putaran ke-3 ini
    }
    print('Angka $i');
  }
  // Hasil yang tercetak: 1, 2, Melewati angka 3..., 4, 5
}
```
