# machine-learning
👟 Hitung Ukuran Sepatu

Aplikasi web sederhana untuk menghitung perkiraan ukuran sepatu berdasarkan tinggi badan.

Project ini dibuat menggunakan HTML, CSS, dan JavaScript murni (Vanilla JavaScript) tanpa menggunakan framework atau library tambahan.

Pengguna cukup memasukkan tinggi badan dalam bentuk angka, kemudian aplikasi akan menghitung dan menampilkan perkiraan ukuran sepatu secara otomatis.

✨ Fitur
Input tinggi badan pengguna.
Validasi dasar melalui konversi nilai menggunakan Number().
Menghitung perkiraan ukuran sepatu berdasarkan tinggi badan.
Membulatkan hasil perhitungan menggunakan Math.round().
Menampilkan hasil langsung pada halaman.
Tampilan sederhana dengan tema warna gelap.
Responsive terhadap ukuran layar karena menggunakan layout Flexbox.
Tidak membutuhkan database atau backend.
🛠️ Teknologi yang Digunakan

Project ini menggunakan beberapa teknologi dasar web:

HTML5 — untuk membuat struktur halaman.
CSS3 — untuk mengatur tampilan dan layout.
JavaScript — untuk menangani input dan proses perhitungan.
Flexbox — untuk memposisikan aplikasi di tengah halaman.
Linear Gradient — untuk membuat background.
DOM Manipulation — untuk mengambil input dan menampilkan hasil.
📁 Struktur Project

Struktur file project sangat sederhana:

Hitung-Ukuran-Sepatu/
├── index.html
├── script.js
├── style.css
└── README.md

index.html

File index.html merupakan halaman utama aplikasi.

File ini bertanggung jawab untuk membuat:

Judul halaman.
Label input tinggi badan.
Input untuk memasukkan tinggi badan.
Tombol untuk menjalankan perhitungan.
Area untuk menampilkan hasil ukuran sepatu.
Import file style.css.
Import file script.js.

Bagian utama aplikasi menggunakan elemen berikut:

<input
    type="text"
    id="inputNumber"
    placeholder="Masukkan tinggi badan"
/>

<button onclick="result()">
    Hitung Ukuran Sepatu
</button>

<div>
    Ukuran Sepatu : <span id="result">-</span>
</div>


Ketika tombol "Hitung Ukuran Sepatu" ditekan, fungsi result() pada script.js akan dijalankan.

🧮 Cara Kerja Perhitungan

Perhitungan dilakukan di dalam fungsi result() pada file script.js.

Alur prosesnya adalah:

Mengambil nilai dari input tinggi badan.
Mengubah nilai input menjadi angka menggunakan Number().
Menghitung nilai perkiraan ukuran sepatu.
Membulatkan hasil menggunakan Math.round().
Menampilkan hasil ke halaman.

Bagian utama proses perhitungannya adalah:

let x = Number(input);
let y = x * 0.24 + 0.42;
output.innerHTML = Math.round(y);


Secara matematis, program menggunakan rumus:

Ukuran Sepatu = (Tinggi Badan × 0.24) + 0.42


Kemudian hasil akhirnya dibulatkan ke bilangan terdekat.

Sebagai contoh, jika tinggi badan yang dimasukkan adalah 170, maka program akan menghitung:

170 × 0.24 + 0.42
= 41.22


Setelah dibulatkan menggunakan Math.round():

41


Sehingga aplikasi akan menampilkan:

Ukuran Sepatu : 41


Catatan: Rumus tersebut merupakan rumus yang digunakan oleh aplikasi ini untuk menghasilkan perkiraan ukuran sepatu. Hasilnya tidak dapat dianggap sebagai ukuran sepatu yang pasti karena ukuran sepatu aktual dapat berbeda berdasarkan standar ukuran, merek, dan bentuk kaki.

⚙️ Penjelasan script.js

Fungsi utama aplikasi berada pada file script.js:

function result() {
    let input = document.getElementById("inputNumber").value;
    let output = document.getElementById("result");
    let x = Number(input);
    let y = x * 0.24 + 0.42;

    output.innerHTML = Math.round(y);
    console.info(input);
}

Mengambil nilai input
let input = document.getElementById("inputNumber").value;


Kode tersebut mengambil nilai yang dimasukkan pengguna pada elemen dengan ID inputNumber.

Mengambil elemen output
let output = document.getElementById("result");


Kode tersebut mengambil elemen <span> yang digunakan untuk menampilkan hasil.

Mengubah input menjadi angka
let x = Number(input);


Karena nilai dari input HTML pada dasarnya berupa string, Number() digunakan untuk mengubahnya menjadi tipe data angka.

Melakukan perhitungan
let y = x * 0.24 + 0.42;


Baris tersebut menjalankan rumus perhitungan ukuran sepatu.

Membulatkan hasil
Math.round(y);


Math.round() digunakan untuk membulatkan hasil ke bilangan bulat terdekat.

Menampilkan hasil
output.innerHTML = Math.round(y);


Hasil perhitungan kemudian dimasukkan ke dalam elemen dengan ID result.

Menampilkan input di Console
console.info(input);


Kode tersebut digunakan untuk menampilkan nilai input pada Developer Console browser. Bagian ini berguna ketika melakukan debugging atau pengecekan nilai yang dimasukkan pengguna.

🎨 Penjelasan style.css

File style.css digunakan untuk memberikan tampilan visual pada aplikasi.

Layout halaman
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
}


Flexbox digunakan untuk menempatkan container aplikasi di tengah halaman secara horizontal dan vertikal.

height: 100vh membuat tinggi halaman mengikuti tinggi viewport browser.

Background

Aplikasi menggunakan gradient:

background: linear-gradient(to bottom, #000, #001f3f);


Warna background dibuat dari hitam menuju biru gelap.

Container aplikasi

Container utama menggunakan ID:

#UkSepatu


Container diberikan:

Background biru gelap.
Padding.
Border radius.
Box shadow.
Warna teks putih.
Text alignment di tengah.

Hal ini membuat tampilan aplikasi terlihat seperti sebuah card sederhana.

Input

Input diberikan padding dan border radius agar lebih nyaman digunakan:

input {
    padding: 10px;
    margin-bottom: 20px;
    width: 100%;
    box-sizing: border-box;
    border-radius: 15px;
}

Tombol

Tombol diberikan warna biru dan bentuk rounded:

button {
    padding: 10px 20px;
    border: none;
    border-radius: 15px;
    cursor: pointer;
    background-color: #0074cc;
    color: white;
    font-size: 16px;
}


Properti cursor: pointer membuat cursor berubah ketika pengguna mengarahkan mouse ke tombol.

🚀 Cara Menjalankan Project

Project ini tidak membutuhkan proses instalasi khusus karena hanya menggunakan HTML, CSS, dan JavaScript.

1. Clone Repository

Jika project berada di GitHub, clone repository menggunakan:

git clone <URL_REPOSITORY>


Kemudian masuk ke folder project:

cd Hitung-Ukuran-Sepatu

2. Jalankan Project

Cara paling sederhana adalah membuka file:

index.html


langsung menggunakan browser.

Anda juga dapat menggunakan extension seperti Live Server pada Visual Studio Code untuk mendapatkan pengalaman development yang lebih nyaman.

3. Masukkan Tinggi Badan

Pada halaman aplikasi, masukkan tinggi badan, misalnya:

170


Kemudian klik:

Hitung Ukuran Sepatu


Aplikasi akan menampilkan hasil perkiraan ukuran sepatu.

🖥️ Contoh Penggunaan

Input:

Masukkan tinggi badan: 170


Proses:

170 × 0.24 + 0.42
= 41.22


Hasil setelah pembulatan:

Ukuran Sepatu : 41


Contoh lainnya:

Tinggi Badan	Hasil Perhitungan	Ukuran
150	36.42	36
160	38.82	39
170	41.22	41
180	43.62	44
190	46.02	46
⚠️ Catatan dan Keterbatasan

Aplikasi ini merupakan project sederhana untuk melakukan perhitungan berdasarkan rumus yang telah ditentukan.

Beberapa kondisi belum ditangani secara khusus, misalnya:

Input kosong.
Input berupa huruf.
Input berupa angka negatif.
Tinggi badan yang tidak masuk akal.
Perbedaan standar ukuran sepatu antarnegara.
Perbedaan ukuran sepatu antarprodusen.
Perbedaan bentuk dan panjang kaki setiap orang.

Karena itu, hasil yang diberikan sebaiknya dianggap sebagai perkiraan, bukan sebagai pengukuran ukuran sepatu yang sebenarnya.

🔮 Pengembangan Selanjutnya

Project ini masih dapat dikembangkan dengan berbagai fitur tambahan, misalnya:

Menambahkan validasi input agar hanya menerima angka.
Memberikan pesan error ketika input kosong.
Menolak tinggi badan negatif atau tidak masuk akal.
Menggunakan <input type="number">.
Menambahkan pilihan satuan centimeter atau meter.
Menambahkan pilihan standar ukuran sepatu seperti EU, US, dan UK.
Menambahkan konversi panjang kaki ke ukuran sepatu.
Menambahkan animasi ketika hasil ditampilkan.
Membuat desain yang lebih responsive untuk perangkat mobile.
Menambahkan dark/light mode.
Menggunakan JavaScript yang lebih modern dengan addEventListener().
Menambahkan unit testing untuk fungsi perhitungan.
📄 Lisensi

Project ini dibuat untuk tujuan pembelajaran dan latihan dasar HTML, CSS, dan JavaScript.

Silakan gunakan, modifikasi, dan kembangkan project ini sesuai kebutuhan.
