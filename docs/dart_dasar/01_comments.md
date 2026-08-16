# Comments

Komentar adalah baris kode yang diabaikan oleh komputer saat program dijalankan. Fungsinya hanya sebagai catatan untuk manusia (pembuat kode).

**Analogi:** Seperti *sticky notes* (kertas catatan tempel) di buku pelajaran. Catatan itu tidak mengubah isi buku, tapi membantumu mengingat bagian penting saat membacanya lagi.

Di Dart, ada dua jenis komentar utama:

## Komentar Satu Baris

Gunakan dua garis miring `//`. Komputer akan mengabaikan apa pun setelah tanda ini pada baris tersebut.

```dart
void main() {
  // Ini adalah komentar satu baris
  print('Halo'); // Ini juga komentar di sebelah kode
}
```

## Komentar Banyak Baris

Gunakan `/*` untuk memulai komentar dan `*/` untuk menutupnya. Sangat cocok jika catatanmu panjang.

```dart
void main() {
  /* 
    Komentar ini
    bisa memanjang
    hingga beberapa baris
  */
  print('Halo');
}
```
