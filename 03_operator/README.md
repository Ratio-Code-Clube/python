
<a id="7"><h2>Operator pada Python</h2></a>

<div align="justify">

Setelah kita tahu cara menyimpan data dalam berbagai jenis variabel, sekarang saatnya kita belajar cara **mengolah** data tersebut. Untuk melakukannya, kita menggunakan **operator**.

Operator adalah simbol-simbol khusus yang digunakan untuk melakukan berbagai jenis operasi, seperti perhitungan matematika, perbandingan antara dua nilai, atau menggabungkan kondisi logika.

</div>

### 1. Operator Aritmatika 🧮

<div align="justify">
Ini adalah operator yang paling umum, digunakan untuk melakukan operasi matematika dasar.
</div>

| Operator | Nama                 | Contoh      | Hasil | Keterangan                                     |
|:--------:|:---------------------|:------------|:-----:|:-----------------------------------------------|
| `+`      | Penjumlahan          | `5 + 2`     | `7`   | Menjumlahkan dua nilai                         |
| `-`      | Pengurangan          | `5 - 2`     | `3`   | Mengurangkan dua nilai                         |
| `*`      | Perkalian            | `5 * 2`     | `10`  | Mengalikan dua nilai                           |
| `/`      | Pembagian            | `5 / 2`     | `2.5` | Membagi dua nilai, hasilnya selalu _float_.    |
| `%`      | Modulus (Sisa Bagi)  | `5 % 2`     | `1`   | Menghitung sisa dari hasil pembagian.          |
| `**`     | Pangkat (Eksponen)   | `5 ** 2`    | `25`  | Memangkatkan nilai (5 pangkat 2).              |
| `//`     | Pembagian Bulat      | `5 // 2`    | `2`   | Membagi dan membulatkan hasilnya ke bawah.     |

```python
x = 10
y = 3

print("Penjumlahan:", x + y)
print("Sisa Bagi:", x % y)
print("Pangkat:", x ** y)
````

### 2 . Operator Penugasan (*Assignment*) 📥

 <div align="justify" >
Operator ini digunakan untuk "menugaskan" atau memberikan nilai kepada sebuah variabel.
 </div >

| Operator | Contoh        | Ekuivalen dengan | Keterangan                                         |
|:--------:|:--------------|:-----------------|:---------------------------------------------------|
| `=`      | `x = 5`       | `x = 5`          | Operator penugasan dasar.                          |
| `+=`     | `x += 3`      | `x = x + 3`      | Menambah nilai variabel lalu mengisi kembali.      |
| `-=`     | `x -= 3`      | `x = x - 3`      | Mengurang nilai variabel lalu mengisi kembali.     |
| `*=`     | `x *= 3`      | `x = x * 3`      | Mengali nilai variabel lalu mengisi kembali.       |
| `/=`     | `x /= 3`      | `x = x / 3`      | Membagi nilai variabel lalu mengisi kembali.       |

```python
# Contoh penggunaan
umur = 20
print("Umur awal:", umur)

# 5 tahun kemudian
umur += 5 # Ini sama dengan umur = umur + 5
print("Umur sekarang:", umur)
```

### 3 . Operator Perbandingan ⚖️

 <div align="justify" >
Operator ini digunakan untuk membandingkan dua nilai. Hasil dari operasi ini **selalu** berupa nilai Boolean (`True` atau `False`).
 </div >

| Operator | Nama                  | Contoh       | Hasil   |
|:--------:|:----------------------|:-------------|:--------|
| `==`     | Sama dengan           | `5 == 5`     | `True`  |
| `!=`     | Tidak sama dengan     | `5 != 2`     | `True`  |
| `>`      | Lebih besar dari      | `5 > 2`      | `True`  |
| `<`      | Lebih kecil dari      | `5 < 2`      | `False` |
| `>=`     | Lebih besar atau sama | `5 >= 5`     | `True`  |
| `<=`     | Lebih kecil atau sama | `5 <= 2`     | `False` |

> ⚠️ **Penting !**: Jangan tertukar antara `=` (penugasan) dan `==` (perbandingan).
>
>   * `x = 10` artinya "masukkan nilai 10 ke dalam variabel x".
>   * `x == 10` artinya "apakah nilai x sama dengan 10?".

```python
nilai_ujian = 85
lulus = nilai_ujian >= 75 # Apakah nilai ujian lebih besar atau sama dengan 75?

print("Apakah siswa lulus?", lulus)
```

### 4 . Operator Logika 🧠

 <div align="justify" >
Operator ini digunakan untuk menggabungkan beberapa kondisi (nilai Boolean) menjadi satu.
 </div >

| Operator | Keterangan                                             | Contoh                             | Hasil   |
|:--------:|:-------------------------------------------------------|:-----------------------------------|:--------|
| `and`    | Hasilnya `True` jika **kedua** kondisi `True`.         | `(5 > 2) and (3 < 4)`              | `True`  |
| `or`     | Hasilnya `True` jika **salah satu** kondisi `True`.    | `(5 > 2) or (3 > 4)`               | `True`  |
| `not`    | Membalikkan hasil (dari `True` menjadi `False`, dan sebaliknya). | `not (5 > 2)`                  | `False` |

```python
# Contoh untuk syarat mendapatkan SIM
umur = 18
punya_ktp = True

# Syarat: harus berumur di atas 17 TAHUN DAN sudah punya KTP
boleh_buat_sim = (umur > 17) and (punya_ktp == True)

print("Boleh buat SIM?", boleh_buat_sim)
```

-----

 <div align="justify" >
Memahami operator adalah kunci untuk mulai menulis program yang dinamis dan bisa membuat keputusan. Di materi selanjutnya, kita akan menggunakan operator perbandingan dan logika ini untuk mengontrol alur program kita dengan **percabangan (if, else)**.
 </div >
