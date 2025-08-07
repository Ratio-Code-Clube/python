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
  * [String](#3)
  * [Integer](#4)
  * [Float](#5)
  * [Boolean](#6)
  * [List](#7)
  * [Tuple](#8)
  * [Set](#9)
  * [Dictionary](#10)

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

  * **nama _variabel**: Label yang Anda berikan (contoh: `nama`).
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

<a id="6"> <h3>4. Boolean (`bool`)</h3> </a>

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

Luar biasa ! Anda sekarang tahu cara menyimpan informasi (dengan variabel) dan jenis-jenis informasi dasar (tipe data) dalam Python. Di materi selanjutnya, kita akan belajar bagaimana cara **mengolah** data-data ini !

<br>
<br>


<a id="tipedatakoleksi"><h2>Tipe Data Koleksi: List, Tuple, Set, & Dictionary</h2></a>



Sejauh ini, kita telah menyimpan satu informasi dalam satu variabel, misalnya `umur = 25`. Namun, bagaimana jika kita ingin menyimpan daftar nama siswa dalam satu variabel? Atau daftar belanjaan?

Untuk kebutuhan ini, Python menyediakan **tipe data koleksi**. Anggap saja ini seperti "wadah super" yang bisa menampung banyak "wadah" (variabel) di dalamnya. Mari kita kenali empat jenis utamanya.



<a id="7"> <h3>1. List (`[]`)</h3> </a>




**Analogi:** Anggap **List** seperti **daftar belanjaan**. Anda bisa menambah barang baru, mencoret barang yang sudah dibeli, atau bahkan mengubah urutannya.

**Karakteristik Utama:**
* **Terurut (_Ordered_):** Urutan data penting dan tidak akan berubah.
* **Dapat Diubah (_Mutable_):** Anda bisa menambah, menghapus, atau mengubah isinya setelah dibuat.
* **Mengizinkan Duplikat:** Anda bisa memiliki beberapa data yang sama persis di dalamnya.
* **Sintaks:** Dibuat menggunakan kurung siku `[]`.


```python
# Contoh sebuah list nama buah
daftar_buah = ["apel", "jeruk", "mangga", "apel"]

print(daftar_buah)

# Mengubah data di list
daftar_buah[1] = "anggur" # Mengganti "jeruk" dengan "anggur"
print(daftar_buah)
````

Output:

```
['apel', 'jeruk', 'mangga', 'apel']
['apel', 'anggur', 'mangga', 'apel']
```

<a id="8"> <h3>2. Tuple (`()`)</h3> </a>



**Analogi:** Anggap **Tuple** seperti **daftar tanggal lahir** pada dokumen resmi. Sekali ditulis, data tersebut tidak seharusnya diubah lagi untuk menjaga integritasnya.

**Karakteristik Utama:**

  * **Terurut (*Ordered*):** Sama seperti List, urutannya tetap.
  * **Tidak Dapat Diubah (*Immutable*):** Isinya **tidak bisa** diubah setelah dibuat. Ini adalah perbedaan utamanya dengan List.
  * **Mengizinkan Duplikat:** Sama seperti List.
  * **Sintaks:** Dibuat menggunakan kurung biasa `()`.

 

```python
# Contoh tuple untuk koordinat geografis
koordinat_gps = (34.0522, -118.2437)

print(koordinat_gps)

# Baris di bawah ini akan menyebabkan error karena tuple tidak bisa diubah!
# koordinat_gps[0] = 10
```

<a id="9"> <h3>3. Set (`{}`)</h3> </a>

 

**Analogi:** Anggap **Set** seperti **kumpulan email unik** untuk undangan. Anda tidak ingin ada email yang sama terdaftar dua kali, dan urutan emailnya pun tidak penting.

**Karakteristik Utama:**

  * **Tidak Terurut (*Unordered*):** Urutan datanya tidak dijamin sama setiap saat.
  * **Dapat Diubah (*Mutable*):** Anda bisa menambah atau menghapus data, tetapi tidak bisa mengubah data yang sudah ada.
  * **Tidak Mengizinkan Duplikat:** Semua data di dalamnya dijamin unik.
  * **Sintaks:** Dibuat menggunakan kurung kurawal `{}`.

 

```python
# Contoh set hobi
hobi_unik = {"membaca", "bersepeda", "memasak", "membaca"}

print(hobi_unik)
```

Output (urutan bisa berbeda):

```
{'bersepeda', 'memasak', 'membaca'}
```

Perhatikan, "membaca" yang duplikat otomatis dihilangkan.

<a id="10"> <h3>4. Dictionary (`{}`)</h3> </a>




**Analogi:** Anggap **Dictionary** persis seperti **kamus** atau **kontak telepon**. Setiap data disimpan dalam format **pasangan kunci-nilai (`key-value`)**. Anda mencari "kata" (kunci) untuk menemukan "artinya" (nilai).

**Karakteristik Utama:**

  * **Pasangan Kunci-Nilai:** Setiap data terdiri dari `kunci` yang unik dan `nilai`-nya.
  * **Dapat Diubah (*Mutable*):** Anda bisa menambah, menghapus, atau mengubah pasangan kunci-nilai.
  * **Kunci Harus Unik:** Tidak boleh ada kunci yang sama.
  * **Sintaks:** Dibuat menggunakan kurung kurawal `{}` dengan format `{'kunci': 'nilai'}`.

 

```python
# Contoh dictionary untuk biodata
biodata_mahasiswa = {
    "nama": "Ghozi Waridi",
    "nim": "123456",
    "ipk": 3.87,
    "aktif": True
}

# Mengakses data menggunakan kuncinya
print("Nama Mahasiswa:", biodata_mahasiswa["nama"])
print("IPK:", biodata_mahasiswa["ipk"])
```

Output:

```
Nama Mahasiswa: Ghozi Waridi
IPK: 3.87
```

-----


 


</div>





