# machine-learning
👟 Hitung Ukuran Sepatu

Aplikasi web sederhana untuk menghitung perkiraan ukuran sepatu berdasarkan tinggi badan.

Project ini dibuat menggunakan HTML, CSS, dan JavaScript (Vanilla JavaScript) tanpa menggunakan framework atau library tambahan.

📌 Tentang Project

Hitung Ukuran Sepatu adalah aplikasi sederhana yang memungkinkan pengguna memasukkan tinggi badan, kemudian aplikasi akan menghitung perkiraan ukuran sepatu berdasarkan rumus yang telah ditentukan.

Aplikasi ini dibuat sebagai project pembelajaran untuk memahami dasar-dasar:

HTML untuk membuat struktur halaman.
CSS untuk membuat tampilan antarmuka.
JavaScript untuk menangani input dan proses perhitungan.
DOM Manipulation untuk mengambil data dari input dan menampilkan hasil.

Catatan: Hasil yang diberikan oleh aplikasi merupakan perkiraan berdasarkan rumus yang digunakan dan tidak dapat dijadikan sebagai ukuran sepatu yang pasti.

✨ Fitur
Input tinggi badan.
Menghitung perkiraan ukuran sepatu secara otomatis.
Membulatkan hasil perhitungan ke bilangan terdekat.
Menampilkan hasil langsung pada halaman.
Tampilan sederhana dan minimalis.
Menggunakan desain dengan tema gelap.
Responsive menggunakan CSS Flexbox.
Tidak membutuhkan database maupun backend.
🛠️ Teknologi

Project ini dibuat menggunakan:

Teknologi	Kegunaan
HTML5	Membuat struktur halaman
CSS3	Mengatur tampilan dan layout
JavaScript	Menjalankan logika dan perhitungan
DOM	Mengambil input dan menampilkan hasil
Flexbox	Mengatur posisi elemen
Linear Gradient	Membuat background
📁 Struktur Project
Hitung-Ukuran-Sepatu/
│
├── index.html
├── script.js
├── style.css
└── README.md

Penjelasan File
index.html

Berisi struktur utama halaman aplikasi, seperti:

Input tinggi badan.
Tombol untuk melakukan perhitungan.
Area untuk menampilkan hasil.
Link ke file CSS.
Link ke file JavaScript.
script.js

Berisi logika utama aplikasi, termasuk:

Mengambil nilai dari input.
Mengubah nilai input menjadi angka.
Melakukan perhitungan ukuran sepatu.
Membulatkan hasil.
Menampilkan hasil ke halaman.
style.css

Berisi seluruh styling aplikasi, seperti:

Background.
Layout.
Warna.
Padding dan margin.
Border radius.
Button.
Input.
Typography.
Box shadow.
README.md

Berisi dokumentasi mengenai project, cara penggunaan, struktur project, serta informasi lainnya.

🧮 Rumus Perhitungan

Aplikasi menggunakan rumus berikut:

Ukuran Sepatu = (Tinggi Badan × 0.24) + 0.42


Hasil perhitungan kemudian dibulatkan menggunakan fungsi JavaScript:

Math.round()

Contoh Perhitungan

Misalnya tinggi badan yang dimasukkan adalah:

170 cm


Maka:

170 × 0.24 + 0.42
= 40.8 + 0.42
= 41.22


Setelah dibulatkan:

41


Maka aplikasi akan menampilkan:

Ukuran Sepatu : 41

🔄 Alur Program

Secara sederhana, alur kerja aplikasi adalah sebagai berikut:

User memasukkan tinggi badan
            ↓
     Klik tombol "Hitung"
            ↓
     Ambil nilai input
            ↓
    Konversi menjadi Number
            ↓
      Jalankan perhitungan
            ↓
       Bulatkan hasil
            ↓
      Tampilkan hasil

💻 Contoh Penggunaan

Pengguna memasukkan:

170


Kemudian menekan tombol:

Hitung Ukuran Sepatu


Aplikasi akan menghasilkan:

Ukuran Sepatu : 41

Contoh Hasil
Tinggi Badan	Perkiraan Ukuran
150 cm	36
160 cm	39
170 cm	41
180 cm	44
190 cm	46

Nilai pada tabel merupakan hasil dari rumus yang digunakan dalam aplikasi dan bukan standar ukuran sepatu resmi.

⚙️ Cara Kerja JavaScript

Fungsi utama aplikasi berada pada script.js:

function result() {
    let input = document.getElementById("inputNumber").value;
    let output = document.getElementById("result");
    let x = Number(input);
    let y = x * 0.24 + 0.42;

    output.innerHTML = Math.round(y);
    console.info(input);
}

1. Mengambil Input
let input = document.getElementById("inputNumber").value;


Kode tersebut mengambil nilai yang dimasukkan pengguna pada input dengan ID inputNumber.

2. Mengambil Element Output
let output = document.getElementById("result");


Kode tersebut mengambil elemen yang digunakan untuk menampilkan hasil perhitungan.

3. Mengubah Input Menjadi Angka
let x = Number(input);


Nilai dari input HTML biasanya berupa string. Fungsi Number() digunakan untuk mengubahnya menjadi tipe data angka.

4. Melakukan Perhitungan
let y = x * 0.24 + 0.42;


Baris tersebut menjalankan rumus untuk mendapatkan perkiraan ukuran sepatu.

5. Membulatkan Hasil
Math.round(y);


Math.round() digunakan untuk membulatkan hasil ke bilangan bulat terdekat.

6. Menampilkan Hasil
output.innerHTML = Math.round(y);


Hasil akhir kemudian ditampilkan pada halaman melalui elemen dengan ID result.

🎨 Tampilan

Aplikasi menggunakan desain sederhana dengan:

Background gradient hitam dan biru gelap.
Card utama berwarna biru gelap.
Teks berwarna putih.
Input dengan sudut membulat.
Button berwarna biru.
Shadow pada card.
Layout menggunakan Flexbox.

Tujuannya adalah membuat aplikasi tetap sederhana tetapi nyaman digunakan.

🚀 Cara Menjalankan

Project ini tidak membutuhkan instalasi dependency karena hanya menggunakan HTML, CSS, dan JavaScript.

1. Clone Repository

Jika project tersedia di GitHub:

git clone <URL_REPOSITORY>


Masuk ke folder project:

cd Hitung-Ukuran-Sepatu

2. Jalankan Project

Cara paling sederhana adalah membuka file:

index.html


menggunakan browser.

Alternatifnya, jika menggunakan Visual Studio Code, project dapat dijalankan menggunakan extension Live Server.

3. Gunakan Aplikasi

Masukkan tinggi badan, contohnya:

170


Kemudian klik:

Hitung Ukuran Sepatu


Hasil perkiraan ukuran sepatu akan ditampilkan pada halaman.

⚠️ Keterbatasan

Aplikasi ini masih menggunakan perhitungan sederhana sehingga memiliki beberapa keterbatasan.

Saat ini aplikasi belum memiliki validasi khusus untuk:

Input kosong.
Input berupa huruf.
Angka negatif.
Tinggi badan yang tidak valid.
Perbedaan standar ukuran sepatu.
Perbedaan ukuran antar merek.
Panjang kaki pengguna.

Oleh karena itu, hasil aplikasi hanya digunakan sebagai perkiraan.

🔮 Rencana Pengembangan

Beberapa fitur yang dapat ditambahkan pada versi berikutnya:

 Validasi input tinggi badan.
 Menolak input kosong.
 Menolak angka negatif.
 Menggunakan <input type="number">.
 Menambahkan satuan tinggi badan.
 Menambahkan pilihan ukuran EU, US, dan UK.
 Menambahkan konversi berdasarkan panjang kaki.
 Menambahkan animasi hasil.
 Meningkatkan responsive design.
 Menambahkan dark/light mode.
 Menggunakan addEventListener() daripada inline onclick.
 Menambahkan testing untuk fungsi perhitungan.
📚 Tujuan Pembelajaran

Project ini dapat digunakan untuk mempelajari konsep dasar web development, khususnya:

HTML
Struktur dokumen HTML.
Form input.
Button.
Label.
ID dan element HTML.
External stylesheet dan JavaScript.
CSS
Flexbox.
Positioning.
Margin dan padding.
Border radius.
Box shadow.
Gradient.
Styling input dan button.
JavaScript
Function.
Variable.
Number().
Math.round().
document.getElementById().
.value.
.innerHTML.
Event melalui onclick.
Console debugging menggunakan console.info().
📄 Lisensi

Project ini dibuat untuk tujuan pembelajaran dan latihan dasar HTML, CSS, dan JavaScript.

Silakan digunakan, dimodifikasi, dan dikembangkan sesuai kebutuhan.

👨‍💻 Author

Dibuat sebagai project pembelajaran Vanilla JavaScript.

⭐ Jika project ini bermanfaat, jangan lupa untuk memberikan Star pada repository.
