# Rangkuman OOP Lanjutan

Materi OOP Lanjutan ini memperkenalkan fitur-fitur modern yang fungsinya mungkin belum terasa saat kamu membuat program terminal kecil, namun akan menjadi senjata yang **sangat sering** kamu manfaatkan saat mulai membangun arsitektur aplikasi berskala besar (misalnya saat kita masuk ke materi Flutter nanti).

Berikut adalah ringkasan kelima materi yang telah dipelajari:

1. **Abstract Class**: Kerangka yang dibiarkan "setengah jadi" dan mengunci rancangan struktur dasar, tidak akan pernah bisa dicetak hidup menjadi wujud object fisik di memori.
2. **Interface (`implements`)**: Sebuah lembar kontrak kerja paksa. Ia tidak mewariskan isi kemampuan apa pun, namun ia dengan ketat memaksa class yang menandatanganinya untuk membangun ulang semua kerangka kerjanya dari nol.
3. **Enums**: Sekumpulan pilihan kaku yang nilainya tetap, mutlak, dan pasti. Sangat handal digunakan untuk menghindari kesalahan fatal *typo* (salah ketik) saat membuat kondisi logika.
4. **Mixins (`with`)**: Komponen tempel bergaya *plug-and-play*. Potongan kode berisi kemampuan instan yang bisa ditempelkan dan dipakai secara bebas ke berbagai class meskipun class-class tersebut tidak sedarah/tidak memiliki garis keturunan yang sama.
5. **Extension Method**: *Alat pelindung casing anti-air*. Teknik ajaib tingkat tinggi untuk menyuntikkan fungsi/method baru buatan sendiri ke dalam class tertutup atau tipe data resmi bawaan (seperti `int` dan `String`) tanpa harus menyentuh kode sumber aslinya.

Selamat! Fondasi konsep penulisan kode terstruktur (*Object-Oriented*) kamu kini sudah di atas rata-rata dan siap menjadi bekal berharga ke tahap selanjutnya.
