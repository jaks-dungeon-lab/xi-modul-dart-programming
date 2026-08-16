# Set (Daftar Unik Tanpa Duplikat)

**Set** adalah jenis koleksi yang sekilas sangat mirip dengan `List` karena bentuk penulisannya, namun ia memiliki satu hukum besi yang tidak bisa diganggu gugat: **Tidak boleh ada data yang kembar (duplikat) di dalam himpunannya**.

**Analogi:** Bayangkan **Set** sebagai **Daftar Buku Tamu VIP** di sebuah pesta eksklusif mewah. Meskipun seorang tamu VIP bernama "Andi" memaksakan diri masuk melewati pintu sebanyak lima kali dan namanya dicatat berkali-kali, buku tamu ajaib ini hanya akan mendaftarkan nama "Andi" tepat satu kali. Buku tamu ini secara otomatis memusnahkan semua nama ganda agar laporannya bersih.

## Membuat Set

Seperti `Map`, pembuatan *Set* juga diawali dengan tanda kurung kurawal `{}`. Bedanya, isinya hanya berupa nilai tunggal berjejer layaknya *List*.

```dart
Set<String> himpunanNama = {'Budi', 'Ayu', 'Siti'};
```

## Hukum Pemusnahan Data Kembar

Jika kamu tanpa sengaja atau sengaja memasukkan data yang sama ke dalam himpunan *Set*, Dart akan menelan data tersebut secara utuh dan membuang versi kembarnya tanpa menghasilkan peringatan *error*.

```dart
Set<int> angkaUnik = {1, 2, 2, 2, 3, 4, 4, 5};

// Mari kita cetak hasilnya
print(angkaUnik); 
// Hasil yang dicetak mesin adalah: {1, 2, 3, 4, 5}
```

## Menambah Data

Seperti biasa, kita bisa menggunakan fungsi `add()` untuk menyuntikkan anggota himpunan baru. Namun perlu diingat, operasi pencarian data pada `Set` melalui fungsi `contains()` jauh lebih ringan dan cepat membelah memori dibandingkan mencari data kembar pada `List`.

```dart
Set<String> namaVIP = {'Andi'};

namaVIP.add('Siti');
namaVIP.add('Andi'); // Baris perintah ini akan diabaikan oleh Set

print(namaVIP); // Hasilnya hanya: {Andi, Siti}
```
