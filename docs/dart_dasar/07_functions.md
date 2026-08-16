# Functions

Fungsi adalah sekumpulan baris kode yang dirancang untuk melakukan satu tugas khusus dan bisa dipanggil berulang kali. Ini membuat kodemu jauh lebih rapi karena kamu tidak perlu menulis ulang kode yang sama.

**Analogi:** Bayangkan fungsi sebagai **mesin pembuat jus (juicer)**. Buah segar yang kamu masukkan adalah data *parameter*. Mesin akan memproses buah tersebut secara otomatis di dalam. Jus buah yang mengalir keluar ke gelas adalah nilai kembalian (*return*).

## Membuat Fungsi Dasar

Sebuah fungsi membutuhkan: tipe data kembalian (misalnya `int`), nama fungsi, *parameter* (data masukan) di dalam tanda kurung, dan blok kode logika utama.

```dart
// Ini adalah mesin kita: 'hitungLuas'
int hitungLuas(int panjang, int lebar) {
  int luas = panjang * lebar;
  return luas; // Keluarkan hasil jus-nya
}

void main() {
  // Kita bisa memakai mesinnya berkali-kali!
  int luasKamar = hitungLuas(4, 3);
  int luasTaman = hitungLuas(10, 5);
  
  print(luasKamar); // Hasil: 12
  print(luasTaman); // Hasil: 50
}
```
