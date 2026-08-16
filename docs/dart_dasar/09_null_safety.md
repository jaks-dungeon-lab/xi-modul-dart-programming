# Null Safety

Di dunia pemrograman, *Null* berarti "kosong" atau "tidak ada nilainya sama sekali" (bukan angka 0, dan bukan teks kosong, melainkan benar-benar tidak ada wujudnya). Dart memiliki fitur **Null Safety** yang melarang variabel dibiarkan kosong secara tidak sengaja, agar aplikasi tidak tiba-tiba *crash*.

**Analogi:** Bayangkan kamu memberikan kotak kado kosong kepada temanmu. Saat dia membuka dan mengharapkan hadiah, dia akan kecewa (aplikasi *crash*). Null Safety adalah penjaga toko yang tegas melarangmu membungkus kado kosong, kecuali kamu menempelkan label khusus "Isi menyusul".

## Variabel Tidak Boleh Kosong

Secara otomatis, semua variabel di Dart tidak boleh null. Kamu harus langsung mengisinya.

```dart
void main() {
  // String nama; // Ini akan merah (error) karena belum diisi
  String nama = 'Budi'; // Benar
}
```

## Mengizinkan Variabel Kosong (Tanda Tanya)

Jika kamu memang belum tahu nilainya di awal dan sengaja ingin mengisinya belakangan, tambahkan tanda tanya `?` tepat setelah penulisan tipe datanya.

```dart
void main() {
  String? pekerjaan; // Sekarang boleh kosong, nilainya terbaca 'null'
  
  // Nanti diisi di tengah program
  pekerjaan = 'Programmer'; 
}
```
