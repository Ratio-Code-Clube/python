<div align="center">

# Variabel dan Tipe Data: "Kotak" Penyimpan Informasi 📦  
  
</div>

<div align="justify">

<a id="1"><h2>Daftar Isi</h2></a>
* [Daftar Isi](#1)
* [Pendahuluan](#pendahuluan)
* [Variabel](#variabel)
  * [Apa itu Variabel](#2)
* [Tipe Data](#tipedata)
  * [Mengenal Tipe Data](#3)

---

<a id="pendahuluan"> <h2>Pendahuluan</h2> </a>
Saat menulis program, kita perlu cara untuk menyimpan dan mengelola informasi, seperti nama pengguna, umur, atau harga barang. Untuk itu, kita menggunakan variabel sebagai "wadah" penyimpan data, dan setiap data yang kita simpan memiliki jenis atau tipe data yang berbeda.
nah, pada kesempatan kali ini kita akan mengulik lebih dalam lagi mengenai variabel dan tipe data yang ada di dalam bahasa python.

<br>
<br>

<a id="2"> <h2>Apa itu Variabel?</h2> </a>
Singkatnya Variabel adalah sebuah wadah untuk menampung data/informasi. <br>
**Analogi Sederhana:** Bayangkan variabel sebagai sebuah **kotak kosong** yang bisa Anda beri label. Anda bisa memasukkan informasi apa pun ke dalam kotak ini, dan kapan pun Anda butuh informasi itu, Anda cukup memanggil nama label kotaknya.

Mari kita lihat contohnya dalam kode:

```python
# Membuat variabel (kotak) dengan label "nama"
# dan mengisinya dengan informasi "Budi"
nama = "Budi"

# Sekarang kita panggil kotaknya untuk melihat isinya
print(nama)
# Output: Budi
````

Struktur pembuatan variabel sangat sederhana: `nama_variabel = nilai`.

  * **nama\_variabel**: Label yang Anda berikan (contoh: `nama`).
  * **=**: Operator "assignment", artinya "masukkan nilai ini ke dalam variabel".
  * **nilai**: Informasi yang Anda simpan (contoh: `"Budi"`).

> **💡 Tips:** Nama variabel bersifat *case-sensitive*, artinya `nama` dan `Nama` dianggap dua variabel yang berbeda. Sebaiknya gunakan huruf kecil dan pisahkan kata dengan garis bawah (*underscore*), contoh: `nama_lengkap`.

-----
<br>
<br>

<a id="tipedata"> <h2>Tipe Data</h2> </a>

Informasi yang kita masukkan ke dalam variabel memiliki jenis atau "tipe" yang berbeda. Python sangat pintar dan otomatis mengenali tipe data dari nilai yang Anda berikan. Mari kenali beberapa tipe data yang paling umum:

<a id="3"> <h3>1. String (`str`)</h3> </a>

Digunakan untuk menyimpan data berupa teks (kumpulan karakter). Teks harus diapit oleh tanda kutip, baik kutip satu (`'`) maupun kutip dua (`"`).

```python
nama_depan = "Andi"
kalimat_sapa = 'Selamat pagi!'
```

<a id="4"> <h3>2. Integer (`int`)</h3> </a>

Digunakan untuk menyimpan bilangan bulat (tanpa koma atau titik desimal).

```python
umur = 25
jumlah_barang = 100
```

<a id="5"> <h3>3. Float (`float`)</h3> </a>


Digunakan untuk menyimpan bilangan yang memiliki koma atau titik desimal.

```python
tinggi_badan = 175.5
harga_produk = 4999.99
```

<a id="5"> <h3>4. Boolean (`bool`)</h3> </a>

Ini adalah tipe data spesial yang hanya memiliki dua nilai: **`True`** (Benar) atau **`False`** (Salah). Ibarat sakelar lampu: ON atau OFF. Sangat berguna untuk merepresentasikan sebuah kondisi.

```python
sudah_menikah = False
lampu_menyala = True
```

> **⚠️ Perhatian:** Penulisan `True` dan `False` harus diawali huruf kapital. `true` atau `false` (huruf kecil) tidak akan dikenali sebagai Boolean.

-----

### Praktik: Membuat Biodata Sederhana

Mari kita gabungkan semua yang telah kita pelajari untuk membuat program biodata sederhana.

```python
# --- Program Biodata Sederhana ---

# Membuat variabel dengan berbagai tipe data
nama_lengkap = "Citra Lestari"       # String
pekerjaan = "Mahasiswa"              # String
umur = 20                            # Integer
ipk = 3.87                           # Float
status_aktif = True                  # Boolean

# Menampilkan informasi biodata ke layar
print("--- BIODATA ---")
print("Nama Lengkap:", nama_lengkap)
print("Pekerjaan:", pekerjaan)
print("Umur:", umur, "tahun")
print("IPK:", ipk)
print("Status Aktif:", status_aktif)
```

### Mengecek Tipe Data dengan `type()`

Jika Anda penasaran dengan tipe data sebuah variabel, Anda bisa menggunakan fungsi bawaan `type()` untuk memeriksanya.

```python
x = "Halo Dunia"
y = 50

print(type(x))  # Output: <class 'str'>
print(type(y))  # Output: <class 'int'>
```

Luar biasa\! Anda sekarang tahu cara menyimpan informasi (dengan variabel) dan jenis-jenis informasi dasar (tipe data) dalam Python. Di materi selanjutnya, kita akan belajar bagaimana cara **mengolah** data-data ini\!

</div>
