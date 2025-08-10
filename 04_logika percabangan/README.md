
<div align="center">
  
# Logika Percabangan (If, Elif, Else)

</div>
<div align="justify">

<a id="1"><h2>Daftar Isi</h2></a>
* [Daftar Isi](#1)
* [Pendahuluan](#pendahuluan)
* [Pernyataan if )](#2)
* [Pernyataan else](#3)
* [Pernyataan elif](#4)


<a id="pendahuluan"><h2>Pendahuluan</h2></a>
Sejauh ini, program kita berjalan lurus dari atas ke bawah. Tapi, bagaimana jika kita ingin program bisa membuat keputusan dan mengambil "jalan" yang berbeda tergantung pada kondisi tertentu?

Misalnya, jika di luar hujan, kita bawa payung. Jika tidak, kita tidak perlu bawa. Kemampuan untuk membuat keputusan seperti inilah yang disebut **percabangan** atau **kontrol alur (_control flow_)**. Di Python, kita menggunakan `if`, `elif`, dan `else` untuk melakukannya.


<br>
<br>
<a id="2"><h2>Pernyataan `if` (Jika...) 🤔</h2></a>


Pernyataan `if` adalah yang paling dasar. Pernyataan ini digunakan untuk menjalankan sebuah blok kode **hanya jika** sebuah kondisi bernilai `True`.

**Anatomi:**
`if kondisi:`
<br>
`....# Blok kode ini dijalankan jika kondisi True`
<br>
`....# Perhatikan indentasi (spasi menjorok ke dalam)`


```python
# Contoh: Cek apakah seseorang boleh menonton film rating dewasa
umur = 22

if umur >= 17:
  print("Anda boleh masuk untuk menonton film ini.")

print("Terima kasih telah berkunjung.") # Baris ini akan selalu dijalankan
````

Karena `umur` (22) lebih besar dari 17, maka kondisi `umur >= 17` bernilai `True`, dan pesan "Anda boleh masuk..." akan ditampilkan.

<br>
<br>
<a id="3"><h2>Pernyataan `else` (Jika Tidak...) 🤷 </h2></a>

 
Bagaimana jika kondisi `if` tidak terpenuhi (bernilai `False`)? Di sinilah `else` berperan. Blok kode di dalam `else` akan dijalankan sebagai alternatif jika kondisi `if` gagal.
 

```python
# Melanjutkan contoh sebelumnya
umur = 15

if umur >= 17:
  print("Anda boleh masuk untuk menonton film ini.")
else:
  print("Maaf, Anda belum cukup umur untuk menonton film ini.")
```

Dalam contoh ini, karena `umur` (15) tidak memenuhi kondisi `umur >= 17`, program akan "melompat" dan menjalankan blok kode di dalam `else`.

<br>
<br>
<a id="4"><h2>Pernyataan `elif` (Jika Tidak, Coba Kondisi Lain...) 🧐</h2></a>

 
`elif` adalah kependekan dari *else if*. Digunakan ketika kita memiliki lebih dari dua kemungkinan atau "cabang jalan". `elif` memungkinkan kita untuk memeriksa beberapa kondisi secara berurutan.
 

```python
# Contoh: Konversi nilai angka menjadi nilai huruf
nilai = 85

if nilai >= 90:
  print("Nilai Anda: A")
elif nilai >= 80:
  print("Nilai Anda: B")
elif nilai >= 70:
  print("Nilai Anda: C")
else:
  print("Nilai Anda: D")
```

**Cara kerjanya:**

1.  Python memeriksa `if nilai >= 90`. Hasilnya `False` (karena 85 tidak lebih besar dari 90).
2.  Python pindah ke `elif nilai >= 80`. Hasilnya `True` (karena 85 lebih besar dari 80).
3.  Blok kode di dalam `elif` ini dijalankan (`Nilai Anda: B`), dan **seluruh sisa percabangan diabaikan**.

### Contoh Lengkap: Program Tebak Angka Sederhana

```python
# Program sederhana untuk menebak angka rahasia
angka_rahasia = 7
tebakan_user = 5

print("Aku punya angka rahasia antara 1-10. Coba tebak!")

if tebakan_user == angka_rahasia:
  print("Selamat! Tebakanmu benar!")
elif tebakan_user < angka_rahasia:
  print("Salah! Angka rahasiamu terlalu kecil.")
else:
  print("Salah! Angka rahasiamu terlalu besar.")
```

-----


Luar biasa ! Anda sekarang bisa membuat program yang lebih "pintar" dan dinamis. Kemampuan untuk mengontrol alur program adalah keterampilan inti seorang programmer.

Di materi selanjutnya, kita akan membahas konsep fundamental lainnya: **perulangan (*looping*)**, yang memungkinkan kita menjalankan blok kode yang sama berulang kali secara otomatis.

</div>

