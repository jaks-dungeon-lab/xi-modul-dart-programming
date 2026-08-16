# Class dan Object

Di dalam OOP, dua kata yang paling sering kamu dengar adalah **Class** dan **Object**.

- **Class** adalah cetak biru (blueprint), rancangan, atau cetakannya.
- **Object** adalah hasil nyata wujud fisik yang dibuat dari cetakan tersebut.

**Analogi:**

- **Class**: Cetakan kue puding beruang.
- **Object**: Kue puding beruang sungguhan yang sudah matang dan bisa dimakan. Dari satu cetakan silikon (Class), kamu bisa mencetak puluhan puding nyata (Object) secara identik.

## Membuat Class

Di Dart, kita menggunakan kata kunci `class` diikuti dengan nama class-nya. Biasakan menulis nama class dengan huruf depan kapital (PascalCase).

```dart
// Ini adalah Cetakan (Class)
class Kucing {
  // Isi class (sifat dan tindakan) akan kita tulis di sini nanti
}
```

## Membuat Object (Instansiasi)

Setelah cetakannya ada, kita bisa membuat wujud nyatanya (Object) di dalam fungsi utama `main()`. Proses membuat object ini disebut **Instansiasi**.

```dart
void main() {
  // Membuat object kucingPertama dari cetakan Kucing
  var kucingPertama = Kucing();
  
  // Membuat object kucingKedua dari cetakan Kucing yang sama
  var kucingKedua = Kucing();
}
```

Sederhana bukan? Kamu baru saja "menciptakan" dua ekor kucing yang benar-benar terpisah di dalam memori komputer, dengan hanya menggunakan satu buah cetakan!
