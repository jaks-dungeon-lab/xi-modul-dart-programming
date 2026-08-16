# Closures

**Closure** (Penutupan) adalah sebuah konsep *Functional Programming* di mana suatu fungsi ternyata terbukti memiliki sebuah "ingatan" yang luar biasa kuat. 

Secara teknis penulisan kode, Closure adalah *anonymous function* yang mampu **mengingat dan mengakses langsung variabel-variabel yang ada di lingkungan luar asalnya**, meskipun lingkungan luar tersebut secara logika pemrograman seharusnya sudah musnah atau terhapus dari memori komputer.

**Analogi:** Bayangkan kamu masuk ke dalam sebuah ruang rahasia milik gurumu (Fungsi Induk) yang berisi sebuah lemari brankas ujian. Di dalam ruang tersebut, kamu diam-diam menciptakan sebuah tali ajaib tak kasat mata (Closure). 

Anehnya, meskipun kamu sudah keluar dari ruang rahasia tersebut dan pintunya sudah dikunci lalu dihancurkan selamanya, talimu itu **tetap terhubung** secara magis menembus dinding ruangan langsung ke brankas ujian tadi. Kapan pun kamu menarik talinya di lapangan terbuka, kamu tetap memengaruhi isi brankas di dalam ruang rahasia yang telah hancur tersebut.

## Contoh Closure di Dart

Perhatikan dengan sangat saksama logika luar biasa pada kode berikut:

```dart
// Ini adalah Fungsi Induk yang bertugas menciptakan dan mengeluarkan sebuah fungsi
Function pembuatPenghitung() {
  int angka = 0; // Variabel ini terkunci rapat di dalam ruang Fungsi Induk

  // Fungsi anonim yang dikembalikan ini adalah sebuah Closure
  return () {
    angka++; // Ia mengingat secara magis dan mengubah variabel 'angka' milik induknya
    print('Nilai angka saat ini: $angka');
  };
}

void main() {
  // Kita menjalankan pembuatPenghitung() dan menyimpan tali ajaibnya
  var penghitungSaya = pembuatPenghitung();
  
  // Secara logika normal, pembuatPenghitung() sudah selesai berjalan dan memori ruangannya dibuang.
  // Tapi tas ajaib yang kita simpan ternyata MASIH MENGINGAT letak variabel 'angka'!
  
  penghitungSaya(); // Hasil tercetak: Nilai angka saat ini: 1
  penghitungSaya(); // Hasil tercetak: Nilai angka saat ini: 2
  penghitungSaya(); // Hasil tercetak: Nilai angka saat ini: 3
}
```

## Kenapa Konsep Closure Sangat Penting?

Closure sangat diandalkan ketika kamu ingin melindungi sebuah data sensitif agar tidak bisa diedit sembarangan dari luar (menghindari ancaman *bug* perubahan variabel global), namun kamu tetap memberikan akses berupa "sebuah tombol *remote control* kecil" untuk memodifikasi data tersebut dengan cara yang aman dan terkontrol.
