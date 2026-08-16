# Mixins

Di dalam dunia OOP, sebuah class memiliki aturan yang ketat: ia hanya boleh memiliki **satu** Parent Class (orang tua kandung). Ia tidak diperbolehkan melakukan `extends` ke dua atau tiga class sekaligus.

Lalu bagaimana jika kita punya sebuah kumpulan fitur keren, dan kita ingin "menempelkan" fitur keren tersebut ke banyak class secara bebas yang tidak berasal dari satu keluarga? Jawabannya adalah **Mixins**.

**Mixins** adalah teknik mutakhir untuk mendaur ulang potongan kode dengan cara menempelkannya ke berbagai class secara bebas tanpa harus merusak silsilah pewarisan (inheritance).

**Analogi:** Anggaplah ada sebuah benda tambahan bernama *Jetpack terbang*. Jetpack ini rancangannya fleksibel dan bisa dipakaikan bebas ke punggung Manusia, ditempel di tubuh Anjing, atau dipasang di bodi Mobil. Ketiga objek itu tidak memiliki hubungan keluarga sama sekali, tapi tiba-tiba ketiganya langsung memiliki kemampuan "terbang" yang sama.

## Cara Menggunakan Mixins

Gunakan kata kunci `mixin` untuk membuat bungkusannya, dan gunakan kata kunci `with` pada class tujuan untuk memasangkan mixin tersebut.

```dart
// 1. Ini adalah Mixin
mixin KemampuanTerbang {
  void terbang() {
    print('Melesat melayang tinggi ke udara!');
  }
}

class Hewan {}

// 2. Burung mewarisi sifat Hewan, DAN ditempeli kemampuan terbang (with)
class Burung extends Hewan with KemampuanTerbang {
  // Burung sekarang otomatis punya method terbang() tanpa harus menulisnya
}

// SuperHero adalah class manusia biasa, lalu kita pasangkan dengan kemampuan terbang
class SuperHero with KemampuanTerbang {
  String nama = 'Superman';
}

void main() {
  var merpati = Burung();
  merpati.terbang(); // Hasil: Melesat melayang tinggi ke udara!
  
  var clark = SuperHero();
  clark.terbang(); // Hasil: Melesat melayang tinggi ke udara!
}
```
