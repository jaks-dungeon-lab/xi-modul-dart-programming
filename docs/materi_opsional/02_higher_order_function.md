# Higher-Order Function

Salah satu sihir terbesar dan paling canggih dalam seni Functional Programming adalah keberadaan **Higher-Order Function** (Fungsi Tingkat Tinggi).

Sebuah fungsi baru bisa dinobatkan sebagai Higher-Order Function apabila ia berhasil memenuhi **minimal salah satu** dari dua syarat berat berikut:
1. Ia bersedia menerima fungsi lain sebagai data masukannya (Parameter).
2. Ia sanggup mengeluarkan (mereturn) fungsi lain sebagai hasil akhirnya.

**Analogi:** Bayangkan sebuah Pabrik Pembuat Roti (Higher-Order Function). Pabrik ini sangat unik karena bahan baku utamanya bukanlah gandum atau mentega, melainkan "Kertas Resep" (Fungsi lain). Kamu memasukkan "Kertas Resep Roti Cokelat" ke dalam pabrik, lalu pabrik akan mengeksekusi resep tersebut di dalam mesinnya. Pabrik ini tidak peduli resep jenis apa yang kamu masukkan, ia hanya bertugas patuh menjalankan resepnya.

## 1. Menerima Fungsi Sebagai Parameter

Perhatikan kode simulasi pabrik di bawah ini. Fungsi `jalankanAksi` menerima tipe data berupa `Function` sebagai inputannya.

```dart
// Ini adalah wujud nyata dari Higher-Order Function
void jalankanAksi(String nama, Function aksiKustom) {
  print('Memulai proses persiapan untuk $nama...');
  
  // Menjalankan (mengeksekusi) resep fungsi yang dikirimkan dari luar
  aksiKustom(); 
  
  print('Semua persiapan selesai dilakukan.');
}

void main() {
  // Kita mengirimkan Anonymous Function secara langsung ke dalam parameter kedua!
  jalankanAksi('Budi', () {
    print('Budi sedang mencuci tangan.');
  });
}
```

## Contoh Nyata di Bahasa Dart

Dalam kehidupan pemrograman sehari-hari, bahasa Dart sudah menyiapkan segudang Higher-Order Function bawaan, terutama untuk memproses deretan kumpulan data (seperti *List*).

Metode canggih `.forEach()` pada List adalah contoh sempurna dari Higher-Order Function. Ia memaksa kita mengirimkan sebuah fungsi anonim untuk dijalankan ke setiap buah data di dalam urutannya.

```dart
void main() {
  var kumpulanAngka = [10, 20, 30];

  // Kita mengirimkan aksi (apa yang harus dilakukan) ke dalam parameter forEach
  kumpulanAngka.forEach((isiData) {
    print('Ditemukan angka: $isiData');
  });
}
```

Gaya penulisan seperti ini membuat struktur program terasa lebih mengalir dan terbaca seperti kalimat bahasa manusia: *"Wahai kumpulan angka, tolong ya untuk setiap data isimu, jalankan aksi cetak nilainya ke layar."*
