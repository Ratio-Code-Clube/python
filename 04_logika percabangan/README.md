
<a id="8"><h2>Logika Percabangan (If, Elif, Else)</h2></a>

<div align="justify">

Sejauh ini, program kita berjalan lurus dari atas ke bawah. Tapi, bagaimana jika kita ingin program bisa membuat keputusan dan mengambil "jalan" yang berbeda tergantung pada kondisi tertentu?

Misalnya, jika di luar hujan, kita bawa payung. Jika tidak, kita tidak perlu bawa. Kemampuan untuk membuat keputusan seperti inilah yang disebut **percabangan** atau **kontrol alur (_control flow_)**. Di Python, kita menggunakan `if`, `elif`, dan `else` untuk melakukannya.

</div>

### 1. Pernyataan `if` (Jika...) 🤔

<div align="justify">
Pernyataan `if` adalah yang paling dasar. Pernyataan ini digunakan untuk menjalankan sebuah blok kode **hanya jika** sebuah kondisi bernilai `True`.

**Anatomi:**
`if kondisi:`
<br>
`....# Blok kode ini dijalankan jika kondisi True`
<br>
`....# Perhatikan indentasi (spasi menjorok ke dalam)`
</div>

```python
# Contoh: Cek apakah seseorang boleh menonton film rating dewasa
umur = 22

if umur >= 17:
  print("Anda boleh masuk untuk menonton film ini.")

print("Terima kasih telah berkunjung.") # Baris ini akan selalu dijalankan
````

Karena `umur` (22) lebih besar dari 17, maka kondisi `umur >= 17` bernilai `True`, dan pesan "Anda boleh masuk..." akan ditampilkan.

### 2 . Pernyataan `else` (Jika Tidak...) 🤷

 <div align="justify" >
Bagaimana jika kondisi `if` tidak terpenuhi (bernilai `False`)? Di sinilah `else` berperan. Blok kode di dalam `else` akan dijalankan sebagai alternatif jika kondisi `if` gagal.
 </div >

```python
# Melanjutkan contoh sebelumnya
umur = 15

if umur >= 17:
  print("Anda boleh masuk untuk menonton film ini.")
else:
  print("Maaf, Anda belum cukup umur untuk menonton film ini.")
```

Dalam contoh ini, karena `umur` (15) tidak memenuhi kondisi `umur >= 17`, program akan "melompat" dan menjalankan blok kode di dalam `else`.

### 3 . Pernyataan `elif` (Jika Tidak, Coba Kondisi Lain...) 🧐

 <div align="justify" >
`elif` adalah kependekan dari *else if*. Digunakan ketika kita memiliki lebih dari dua kemungkinan atau "cabang jalan". `elif` memungkinkan kita untuk memeriksa beberapa kondisi secara berurutan.
 </div >

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

 <div align="justify" >
Luar biasa ! Anda sekarang bisa membuat program yang lebih "pintar" dan dinamis. Kemampuan untuk mengontrol alur program adalah keterampilan inti seorang programmer.

Di materi selanjutnya, kita akan membahas konsep fundamental lainnya: **perulangan (*looping*)**, yang memungkinkan kita menjalankan blok kode yang sama berulang kali secara otomatis.

 </div >

