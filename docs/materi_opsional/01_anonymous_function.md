# Anonymous Function

Sejauh ini, setiap kali kita membuat fungsi (method), kita selalu memberinya nama yang jelas agar mudah dipanggil. Misalnya fungsi `void berjalan()` atau `int tambah()`. 

Namun di dalam Dart, kita ternyata bisa membuat fungsi yang **sama sekali tidak memiliki nama**. Fungsi misterius ini disebut sebagai **Anonymous Function** (Fungsi Anonim). Beberapa orang juga sering menyebutnya sebagai *Lambda* atau *Closure*.

## Kapan kita menggunakannya?

Fungsi tanpa nama ini biasanya sangat berguna saat kita hanya perlu melakukan aksi kecil secara instan, dan kita tidak berencana memanggil fungsi tersebut berulang kali di tempat lain di masa depan. Karena bentuknya sangat pendek dan ringkas, ia sering diselipkan secara langsung ke dalam parameter fungsi lain.

**Analogi:** Bagaikan menyewa kuli angkut harian. Jika sebuah toko butuh tenaga memindahkan satu dus barang hari ini saja, mereka tidak perlu repot-repot mendaftarkan nama pegawainya ke buku besar perusahaan (Fungsi Bernama). Toko tersebut cukup memanggil orang tak dikenal di jalan, menyuruh dia melakukan tugas angkat barang, lalu orang itu pergi dan tugas selesai (Fungsi Anonim).

## Contoh Penggunaan Biasa

Perhatikan cara penulisannya. Kita membiarkannya kosong dengan kurung `()` dan langsung menuliskan isi logikanya di dalam kurung kurawal `{}`. Untuk membuktikannya, kita menyimpan wujud fungsinya ke dalam sebuah variabel `sapaan`.

```dart
void main() {
  
  // Ini adalah bentuk asli dari Anonymous Function
  var sapaan = (String nama) {
    return 'Halo, $nama!';
  };

  print(sapaan('Budi')); // Hasil: Halo, Budi!
}
```

## Arrow Syntax (`=>`)

Jika fungsi anonim yang kamu buat sangatlah pendek dan hanya berisi **satu baris** pengembalian nilai (*return*), kamu bisa menyingkatnya secara drastis menggunakan tanda panah gemuk (`=>`). 

Tanda panah gemuk ini secara otomatis memiliki arti "mengembalikan nilai" sehingga kamu tidak perlu lagi mengetik kata kunci `return` dan kurung kurawal.

```dart
void main() {
  
  // Menggunakan Arrow Syntax yang sangat ringkas
  var sapaanSingkat = (String nama) => 'Halo, $nama!';
  
  print(sapaanSingkat('Andi'));
}
```

Penulisan cepat dengan panah gemuk (`=>`) ini akan sangat sering kamu lihat dan gunakan nantinya.
