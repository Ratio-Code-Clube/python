
<a id="9"><h2>Perulangan (Looping) pada Python</h2></a>

<div align="justify">

Bayangkan Anda harus menulis "Selamat Pagi!" sebanyak seratus kali. Tentu akan sangat melelahkan jika ditulis satu per satu. Dalam pemrograman, ada cara yang jauh lebih efisien untuk melakukan tugas berulang seperti ini, yaitu dengan menggunakan **perulangan** atau **_loop_**.

Perulangan memungkinkan kita untuk menjalankan satu blok kode yang sama berulang kali, baik untuk jumlah tertentu maupun selama sebuah kondisi terpenuhi. Di Python, ada dua jenis perulangan utama: `for` dan `while`.

</div>

### 1. Perulangan `for` 🚶‍♀️

<div align="justify">
Perulangan `for` digunakan ketika kita ingin mengulang sebuah blok kode untuk setiap item dalam sebuah urutan (seperti _List_, _Tuple_, atau _String_). Ini adalah jenis perulangan yang paling umum digunakan di Python.

**Analogi:** Anggap Anda memiliki sebuah daftar belanjaan (_List_). Anda akan mengambil setiap barang satu per satu dari daftar tersebut sampai semua barang terambil.
</div>

```python
# Contoh: Menampilkan setiap buah dalam sebuah list
daftar_buah = ["apel", "jeruk", "mangga"]

for buah in daftar_buah:
  print("Saya suka makan", buah)
````

**Cara kerjanya:**

1.  Python mengambil item pertama dari `daftar_buah` ("apel") dan menyimpannya di variabel `buah`.
2.  Blok kode di dalam loop dijalankan (`print(...)`).
3.  Python kembali ke atas, mengambil item kedua ("jeruk"), dan mengulangi prosesnya hingga semua item habis.

#### Menggunakan `range()`

 <div align="justify" >
Jika kita ingin mengulang untuk jumlah tertentu, kita bisa menggunakan fungsi `range()`.
 </div >

```python
# Contoh: Perulangan dari 0 hingga 4
for i in range(5):
  print("Perulangan ke-", i)
```

### 2 . Perulangan `while` 🏃‍♂️

 <div align="justify" >
Perulangan `while` digunakan untuk menjalankan sebuah blok kode **selama** sebuah kondisi bernilai `True`.

**Analogi:** Anggap Anda sedang berlari di *treadmill*. Anda akan terus berlari **selama** tombol "start" masih menyala. Begitu tombolnya "off" (kondisi menjadi `False`), Anda berhenti.

 </div >

```python
# Contoh: Hitung mundur dari 5
angka = 5

while angka > 0:
  print(angka)
  angka = angka - 1 # Atau angka -= 1

print("Meluncur!")
```

**Cara kerjanya:**

1.  Python memeriksa `while angka > 0`. Awalnya `True` (karena 5  > 0).
2.  Blok kode dijalankan (`print(angka)` dan `angka` dikurangi 1).
3.  `angka` sekarang menjadi 4. Python kembali ke atas dan memeriksa kondisi lagi. Proses ini berlanjut sampai `angka` menjadi 0, di mana kondisi `0 > 0` menjadi `False` dan perulangan berhenti.

> ⚠️ **Peringatan !**: Hati-hati dengan **perulangan tak terbatas (*infinite loop*)**. Pastikan kondisi di dalam `while` pada akhirnya bisa berubah menjadi `False`. Jika tidak, program Anda akan terus berjalan selamanya dan bisa membuat komputer macet.

### Kontrol Perulangan: `break` dan `continue`

Kadang kita perlu sedikit kontrol lebih terhadap alur perulangan.

  * **`break`**: Untuk **menghentikan paksa** seluruh perulangan, bahkan jika kondisinya masih terpenuhi.

<!-- end list -->

```python
# Contoh: Berhenti jika menemukan angka 5
for i in range(10):
  if i == 5:
    break # Hentikan loop sekarang juga!
  print(i)
```

Outputnya hanya akan mencetak `0, 1, 2, 3, 4`.

  * **`continue`**: Untuk **melewatkan** sisa kode di iterasi saat ini dan langsung loncat ke iterasi berikutnya.

<!-- end list -->

```python
# Contoh: Melewatkan angka ganjil
for i in range(10):
  if i % 2 != 0: # Jika i adalah ganjil
    continue # Lewatkan iterasi ini, lanjut ke angka berikutnya
  print(i) # Baris ini hanya dijalankan untuk angka genap
```

Outputnya hanya akan mencetak `0, 2, 4, 6, 8`.

-----

 <div align="justify" >
Dengan percabangan dan perulangan, Anda kini memiliki dua alat paling kuat dalam pemrograman. Anda bisa membuat program yang tidak hanya membuat keputusan, tetapi juga melakukan tugas-tugas berulang secara efisien.

Selanjutnya, kita akan belajar tentang **fungsi**, cara untuk mengelompokkan kode kita menjadi blok yang bisa digunakan kembali.

</div >
