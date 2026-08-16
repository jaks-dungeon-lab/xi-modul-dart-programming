# Map (Daftar Berlabel)

**Map** (sering disebut *Dictionary* atau Kamus) adalah jenis koleksi yang memasangkan sebuah kata kunci (*Key*) dengan sebuah isi data (*Value*). Berbeda dengan `List` yang mencari data menggunakan nomor urut, `Map` mencari data dengan memanggil nama labelnya.

**Analogi:** Bayangkan **Map** sebagai **Loker Penitipan Barang** di stasiun kereta. Loker tersebut tidak memiliki nomor, melainkan setiap pintunya ditempeli stiker nama pelanggan. Jika kamu ingin mengambil tas, kamu tidak perlu tahu loker tersebut ada di urutan ke berapa; kamu cukup berteriak "Buka loker milik Budi!", maka loker berlabel "Budi" akan memuntahkan tas yang ada di dalamnya. Label nama itu adalah *Key*, dan isi tasnya adalah *Value*.

## Membuat Map

Untuk merakit sebuah *Map*, kita menggunakan tanda kurung kurawal `{}` dengan struktur `Kunci: Nilai`.

```dart
// Key berupa teks (String), Value berupa teks (String)
Map<String, String> dataIbukota = {
  'Indonesia': 'Jakarta',
  'Jepang': 'Tokyo',
  'Inggris': 'London',
};

// Key berupa teks (String), Value berupa angka (int)
Map<String, int> umurSiswa = {
  'Budi': 16,
  'Ayu': 17,
  'Joko': 16,
};
```

## Memanggil dan Mengubah Data

Untuk memanggil atau mengganti isi loker, panggil nama `Map`-nya lalu masukkan kunci labelnya ke dalam kurung siku `[]`.

```dart
Map<String, int> umurSiswa = {
  'Budi': 16,
  'Ayu': 17,
};

// Membaca data Ayu
print(umurSiswa['Ayu']); // Keluar angka 17

// Mengubah isi data milik Budi
umurSiswa['Budi'] = 18;

// Menambahkan data baru langsung ke dalam loker
umurSiswa['Siti'] = 15;
```

**Aturan Sangat Penting:** Kunci (*Key*) dalam *Map* bersifat sangat eksklusif dan harus mutlak unik. Kamu tidak boleh memiliki dua label "Budi" di dalam satu loker yang sama. Jika kamu melakukannya, nilai "Budi" yang lama akan dihancurkan tertimpa oleh nilai "Budi" yang baru dimasukkan.
