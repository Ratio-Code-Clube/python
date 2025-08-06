<div align="center">

  
# Python

Selamat Datang di pemograman Python dasar. Di sini kita akan memberikan penjelasan bagi kalian yang ingin belajar python untuk anak no IT atau bagi kalian yang baru pertama kali belajar bahasa pemograman. 
  
</div>


<a id="1"><h2>Daftar Isi</h2></a>

* Introduction
  * [Daftar Isi](#1)
  * [Gambaran Singkat](#2)
  * [Instalasi Python](#3)
  * [COntoh Hello World](#4)


<a id="2"> <h2>Gambaran Umum</h2> </a>
### Apa itu Python 🐍

<div align="justify">

  Python merupakan salah satu baahsa pemograman tingkat atas, yang bertujuan untuk memberikan perintah dan berinteraksi dengan komputer.
  Bayangkan Anda ingin menyuruh komputer untuk melakukan sesuatu, misalnya menghitung total belanjaan atau menampilkan semua gambar yang ada di folder,
  untuk menyuruhnya anda memerlukan sebuah bahasa yang bisa dimengerti oleh komputer dan kita.

  Nah, **Python merupakan salah satu perantar _perantara_ itu.**


  Secara sederhana, Python adalah bahasa pemrograman yang diciptakan oleh **Guido van Rossum**. Bahasa ini sengaja dirancang agar **mudah dibaca dan ditulis**, bahkan sintaksnya hampir mirip seperti membaca kalimat dalam bahasa Inggris. Inilah yang menjadikannya bahasa yang sempurna bagi pemula.

### Mengapa Harus Memilih Python?

Di antara banyak bahasa pemrograman, mengapa Python sangat direkomendasikan untuk pemula?

1.  **Mudah Dipelajari dan Digunakan**
    Aturan penulisannya (sintaks) sangat bersih dan sederhana. Anda tidak akan langsung dipusingkan dengan simbol-simbol `{}` atau `;` yang rumit seperti pada bahasa lain. Fokus Anda bisa langsung tertuju pada logika pemecahan masalah.

2.  **Sangat Serbaguna (Bisa untuk Apa Saja!)**
    Python itu seperti pisau lipat serbaguna (_Swiss Army knife_). Dengan menguasai satu bahasa ini, Anda bisa membuat berbagai macam hal, mulai dari website hingga kecerdasan buatan.

3.  **Komunitas Besar dan Dukungan Kuat**
    Karena sangat populer, ada jutaan pengguna Python di seluruh dunia. Jika Anda mengalami kesulitan atau error, kemungkinan besar orang lain sudah pernah mengalami masalah yang sama dan solusinya sudah tersedia di internet (misalnya di forum seperti Stack Overflow).

4.  **Banyak "Perpustakaan" Siap Pakai**
    Python punya banyak sekali "perpustakaan" (*library*) atau "modul". Anggap saja ini seperti kepingan-kepingan LEGO yang sudah jadi. Anda tidak perlu membangun semuanya dari nol.
    * Butuh mengolah data? Ada *library* **Pandas**.
    * Butuh membuat grafik? Ada *library* **Matplotlib**.
    * Butuh membuat website? Ada kerangka kerja (*framework*) **Django** dan **Flask**.

### Jadi, Apa yang Bisa Dibuat dengan Python?

Ini bagian yang paling menarik! Dengan Python, Anda bisa membangun aplikasi nyata yang mungkin Anda gunakan sehari-hari.

* 🌐 **Pengembangan Website (Backend)**
    Membangun bagian "otak" dari sebuah website yang mengelola data dan logika. Perusahaan besar seperti **Instagram**, **Spotify**, dan **Netflix** menggunakan Python di sistem mereka.

* 📊 **Sains Data dan Analisis Data**
    Mengolah, membersihkan, menganalisis, dan memvisualisasikan data dalam jumlah besar. Python adalah "raja" di bidang ini dan menjadi alat utama para analis data.

* 🤖 **Kecerdasan Buatan (AI) & _Machine Learning_**
    Melatih komputer untuk belajar dari data, seperti pada fitur rekomendasi produk, pengenalan wajah, hingga sistem mobil tanpa pengemudi.

* ⚙️ **Otomatisasi Tugas (Scripting)**
    Menulis skrip sederhana untuk melakukan tugas-tugas membosankan secara otomatis. Misalnya, merapikan ribuan file, mengunduh data dari internet, atau mengisi formulir online secara otomatis.

* 🎮 **Pengembangan Game**
    Membuat game 2D sederhana dengan menggunakan _library_ seperti **Pygame**.

Singkatnya, Python adalah pintu gerbang yang sangat ramah untuk masuk ke dunia teknologi yang luas. Mari kita mulai perjalanan ini dengan melakukan instalasi Python di komputer Anda!
  
  
</div>


<a id="3"><h2>Instalasi Python</h2></a>

Sebelum kita bisa "berbicara" dengan komputer menggunakan bahasa Python, kita perlu memasang **"penerjemahnya"** terlebih dahulu. Penerjemah ini disebut **Python Interpreter**. Tugasnya adalah membaca kode yang kita tulis dan mengubahnya menjadi instruksi yang dimengerti oleh mesin.

Proses instalasi ini cukup dilakukan satu kali. Ikuti panduan yang sesuai dengan sistem operasi Anda.

<h4>1. Untuk Pengguna Windows 💻</h4>

1.  **Unduh Installer Python**
    Buka browser dan kunjungi halaman unduhan resmi Python: **[python.org/downloads/](https://python.org/downloads/)**. Klik tombol kuning untuk mengunduh versi terbaru.

2.  **Jalankan Installer**
    Buka file `.exe` yang baru saja Anda unduh. Anda akan melihat jendela instalasi.

3.  **Centang "Add Python to PATH" (SANGAT PENTING!)**
    Di bagian bawah jendela instalasi, ada sebuah kotak centang bertuliskan **"Add Python.exe to PATH"**. **PASTIKAN Anda mencentang kotak ini.** Langkah ini akan sangat mempermudah kita saat menjalankan Python dari terminal nanti.

    <img src="https://docs.python.org/3/using/images/win-install-launcher.png" alt="Centang Add to PATH" width="600"/>

4.  **Pilih "Install Now"**
    Klik pada **"Install Now"**. Proses instalasi akan berjalan. Setelah beberapa saat, instalasi akan selesai.

<h4>2. Untuk Pengguna macOS 🍎</h4>

Meskipun macOS biasanya sudah memiliki versi Python bawaan, seringkali itu adalah versi yang lebih lama. Sangat disarankan untuk memasang versi terbaru dari situs resminya.

1.  **Unduh Installer Python**
    Kunjungi **[python.org/downloads/](https://python.org/downloads/)** dan unduh installer untuk macOS (file dengan ekstensi `.pkg`).

2.  **Jalankan Installer**
    Buka file `.pkg` yang sudah diunduh. Ikuti petunjuk yang muncul di layar dengan mengklik "Continue", "Agree", dan "Install" hingga proses selesai. Anda mungkin akan diminta memasukkan kata sandi komputer Anda.

<h4>3. Untuk Pengguna Linux 🐧</h4>

Kebanyakan distribusi Linux sudah dilengkapi dengan Python 3. Anda bisa langsung memverifikasinya. Namun, jika belum ada atau Anda ingin versi yang lebih baru, Anda bisa menginstalnya melalui terminal.

* **Untuk Debian/Ubuntu:**
    ```bash
    sudo apt update
    sudo apt install python3
    ```

<h4>Verifikasi Instalasi</h4>

Setelah proses instalasi selesai, mari kita pastikan Python sudah terpasang dengan benar.

1.  Buka **Command Prompt** (di Windows) atau **Terminal** (di macOS/Linux).
2.  Ketik perintah di bawah ini, lalu tekan Enter:

    ```bash
    python --version
    ```
    *Catatan: Di macOS dan Linux, Anda mungkin perlu mengetik `python3 --version`*

Jika muncul tulisan seperti `Python 3.12.4`, maka selamat! Python sudah berhasil terpasang di komputer Anda.

<a id="4"><h2>Contoh "Hello, World!"</h2></a>

"Hello, World!" adalah sebuah tradisi. Ini adalah program pertama yang hampir selalu dibuat oleh programmer di seluruh dunia saat mempelajari bahasa baru. Anggap saja ini sebagai "salam perkenalan" kita pada dunia pemrograman Python.

Ada dua cara mudah untuk menjalankannya.

<h4>Cara 1: Mode Interaktif (Langsung di Terminal)</h4>

Cara ini cocok untuk mencoba perintah-perintah singkat secara langsung.

1.  Buka **Terminal** atau **Command Prompt**.
2.  Ketik `python` (atau `python3` untuk macOS/Linux), lalu tekan Enter.
3.  Anda akan melihat prompt berubah menjadi `>>>`. Ini artinya Anda sudah masuk ke mode interaktif Python.
4.  Sekarang, ketik perintah berikut dan tekan Enter:
    ```python
    print("Hello, World!")
    ```
5.  Komputer akan langsung merespons dan menampilkan:
    ```
    Hello, World!
    ```

<h4>Cara 2: Menjalankan dari File (Cara yang Sebenarnya)</h4>

Ini adalah cara kita akan bekerja untuk proyek-proyek yang lebih besar.

1.  **Buat File Baru**
    Buka editor teks sederhana seperti **Notepad** (di Windows) atau **TextEdit** (di macOS).

2.  **Tulis Kode**
    Ketik baris kode yang sama persis seperti sebelumnya di dalam editor teks tersebut:
    ```python
    print("Hello, World!")
    ```

3.  **Simpan File**
    Simpan file tersebut dengan nama **`halo.py`**. Pastikan ekstensinya adalah **`.py`**, bukan `.txt`. Anda bisa menyimpannya di folder mana pun yang mudah dijangkau, misalnya di Desktop.

4.  **Jalankan File via Terminal**
    * Buka **Terminal** atau **Command Prompt**.
    * Gunakan perintah `cd` (change directory) untuk berpindah ke folder tempat Anda menyimpan file tadi. Contoh, jika Anda menyimpannya di Desktop:
        ```bash
        cd Desktop
        ```
    * Setelah berada di folder yang benar, jalankan program Anda dengan perintah:
        ```bash
        python halo.py
        ```
        *(Gunakan `python3 halo.py` jika perlu)*

    Terminal akan menampilkan output yang sama: `Hello, World!`.

---

**Selamat!** 🎉 Anda baru saja menulis dan menjalankan program Python pertama Anda.

Perintah **`print()`** adalah sebuah "fungsi" bawaan Python yang tugasnya adalah menampilkan apa pun yang ada di dalam tanda kurung ke layar. Anda telah mengambil langkah pertama yang paling penting. Di bagian selanjutnya, kita akan mulai menyelami konsep-konsep dasar Python seperti variabel dan tipe data.
