# Abstract Class dan Interface

Dalam membangun program yang sangat besar dan dikerjakan oleh banyak orang, terkadang kita butuh sebuah aturan wajib yang memaksa bagian-bagian tertentu untuk memiliki kemampuan standar yang sama. Di sinilah peran Abstract Class dan Interface.

## Abstract Class

**Abstract Class** adalah cetakan yang sengaja dibiarkan "setengah jadi". Ia tidak akan pernah bisa langsung dicetak menjadi object nyata. Tugas utamanya hanyalah berfungsi sebagai kerangka dasar untuk diwariskan ke class-class turunannya.

**Analogi:** Seperti sketsa kasar rancangan kendaraan bermotor. Sebuah kertas sketsa "Kendaraan" tidak bisa dikendarai di jalan raya. Tapi jika sketsa itu diwariskan dan disempurnakan menjadi wujud "Mobil", maka mobilnya baru bisa dikendarai.

```dart
// Ini adalah Abstract Class, kerangka mati yang tidak bisa dicetak langsung
abstract class Kendaraan {
  
  // Ini adalah Method abstrak (hanya ada nama fungsinya, tapi tidak ada isinya)
  void nyalakanMesin();
}

// Class Mobil mewarisi dan wajib menyempurnakan kerangkanya
class Mobil extends Kendaraan {
  
  // Wajib menimpa (override) dan memberikan isi pada method nyalakanMesin
  @override
  void nyalakanMesin() {
    print('Mesin mobil menyala: Vroom!');
  }
}
```

## Interface (`implements`)

Di bahasa Dart, semua class pada dasarnya bisa dijadikan **Interface** menggunakan kata kunci `implements`. 

Bedanya dengan `extends` (pewarisan), jika kamu menggunakan `implements`, kamu **wajib membangun ulang** seluruh properties dan method yang ada di dalamnya dari titik nol. Kamu tidak akan mendapat warisan isi kode sedikitpun dari Parent Class-nya.

**Analogi:** Kamu menandatangani kontrak pekerjaan dengan sebuah perusahaan raksasa. Kontrak itu mewajibkanmu memiliki kemampuan "berbicara Bahasa Inggris", tapi perusahaan itu tidak akan mengajarimu. Kamu bebas belajar dari mana saja, yang penting saat dites kamu bisa berbicara Bahasa Inggris.

```dart
class MesinPemanas {
  void panaskan() {
    print('Memanaskan...');
  }
}

// Oven "menandatangani kontrak" dengan MesinPemanas
class Oven implements MesinPemanas {
  
  // Walaupun MesinPemanas punya isi perintah print('Memanaskan...'), 
  // Oven tidak mewarisi kode itu. Oven wajib menulis perintahnya sendiri.
  @override
  void panaskan() {
    print('Oven memanaskan adonan kue hingga suhu 200 derajat...');
  }
}
```
