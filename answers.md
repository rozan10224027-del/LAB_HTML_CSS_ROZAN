
# Jawaban Praktikum: Rozan (10224027)

## Bagian 1: Pemanasan

1. Selector: `nav a.active:hover`, property: `color`, value: `red`.

2. `span`: inline; `p`: block; `a`: inline; `li`: block; `h2`: block; `strong`: inline.

3. Paragraf A dan B berwarna hijau karena merupakan keturunan `.box`. Paragraf C dan D tidak termasuk keturunan `.box`, sehingga tidak terkena aturan `.box p`.

4. Selector `#title` lebih spesifik daripada selector class dan elemen, sehingga warna merah dari `#title` diterapkan.

5. HTML tersebut tidak valid karena elemen `<p>` ditutup sebelum elemen `<strong>`, padahal `<strong>` masih berada di dalam paragraf. Seharusnya `<strong>` ditutup terlebih dahulu.

## Bagian 3: Prediksi Selector Golf

P1. Sebelum diuji:
- Weekly hack nights: hijau, karena selector `section p` lebih spesifik daripada `p`.
- Bring your own laptop: oranye, karena selector `.note` lebih spesifik daripada `section p`.
- Copyright footer: biru, karena hanya terkena selector `p`.

P2. Urutan specificity dari tertinggi ke terendah:
1. `#tech p`
2. `.club p`
3. `main section p`
4. `p`

Setelah diuji (hasil sebenarnya):

- Weekly hack nights: hijau.
- Bring your own laptop: oranye.
- Copyright footer: biru.

## Bagian 4: Box model

Q1 (content-box):

Lebar total dari konten, padding, dan border adalah 334px.
Perhitungannya: 300px + (16px × 2) + (1px × 2) = 334px.
Margin 24px tidak termasuk dalam ukuran tersebut.

Q2 (border-box):

Lebar keseluruhan konten, padding, dan border adalah 300px karena ukuran width sudah mencakup padding dan border. Margin tidak termasuk.

Pengecekan DevTools:

Belum diperiksa melalui DevTools.

## Bagian 5: Tabel debug

| # | Baris | Bug | Perbaikan | Cara menemukannya |
|---|---|---|---|---|
| 1 | CSS | `colour` digunakan sebagai properti | Ganti menjadi `color` | Memeriksa properti CSS |
| 2 | CSS | Tanda titik koma setelah nilai `background` hilang | Tambahkan `;` | Memeriksa sintaks CSS |
| 3 | HTML/CSS | Nama class tidak konsisten | Samakan nama class HTML dan CSS menjadi `card` | Memeriksa selector dan atribut class |
| 4 | CSS | `18 px` memiliki spasi yang salah | Ganti menjadi `18px` | Memeriksa nilai ukuran CSS |
| 5 | CSS | `centre` bukan nilai CSS yang valid untuk perataan teks | Ganti menjadi `center` | Memeriksa nilai properti |
| 6 | HTML | Tag heading dibuka dengan `h1` tetapi ditutup dengan `h2` | Gunakan tag penutup `</h1>` | Memeriksa pasangan tag |
| 7 | HTML | Tanda kutip atribut `href` tidak lengkap | Tutup tanda kutip pada URL | Memeriksa atribut HTML |
| 8 | HTML/CSS | ID HTML berbeda dari selector CSS | Samakan ID dan selector, misalnya `news-list` | Memeriksa kecocokan ID |
| 9 | HTML | Gambar tidak memiliki atribut `alt` | Tambahkan deskripsi alternatif gambar | Memeriksa aksesibilitas gambar |

## Bagian 6: Tabel Code Review

| # | Baris | Masalah | Mengapa penting | Perbaikan saya |
|---|---|---|---|---|
| 1 | HTML | Tidak ada deklarasi DOCTYPE | Browser dapat menggunakan mode rendering yang berbeda | Menambahkan `<!DOCTYPE html>` |
| 2 | HTML | Elemen HTML tidak memiliki atribut `lang` | Membantu browser dan teknologi pembaca layar mengenali bahasa | Menambahkan `lang="id"` |
| 3 | HTML | Tidak ada meta charset | Membantu karakter ditampilkan dengan benar | Menambahkan `<meta charset="UTF-8">` |
| 4 | HTML | Tidak ada meta viewport | Tampilan dapat bermasalah di perangkat seluler | Menambahkan meta viewport |
| 5 | HTML | Menggunakan elemen nonsemantik untuk semua bagian | Struktur halaman sulit dipahami | Menggunakan `header`, `main`, `section`, dan `footer` |
| 6 | CSS | Menggunakan inline style | HTML dan CSS menjadi sulit dipelihara | Memindahkan aturan ke CSS |
| 7 | CSS | Menggunakan `!important` | Membuat pengaturan specificity lebih sulit dikelola | Mengatur selector dengan specificity yang sesuai |
| 8 | CSS | Lebar halaman terlalu besar dan tetap | Konten dapat melampaui layar perangkat kecil | Menggunakan `max-width` dan lebar responsif |
| 9 | HTML | Gambar tidak memiliki teks alternatif | Informasi gambar tidak tersedia bagi pembaca layar | Menambahkan atribut `alt` |
| 10 | HTML | Input email memakai tipe teks | Validasi email bawaan browser tidak digunakan | Mengubah menjadi `type="email"` |
| 11 | HTML | Input tidak memiliki label yang terhubung | Formulir lebih sulit digunakan | Menambahkan `label` dengan atribut `for` dan ID input |
| 12 | HTML | Tombol menggunakan aksi JavaScript yang tidak berfungsi | Pengguna dapat mengira formulir sudah terkirim | Membuat formulir dengan struktur dan aksi yang jelas |

Refleksi:

1. Saya belajar bahwa struktur HTML yang semantik membuat halaman lebih mudah dipahami dan diakses.
2. Saya belajar bahwa selector CSS dan specificity menentukan aturan mana yang diterapkan pada elemen.
3. Saya akan membiasakan diri memeriksa HTML menggunakan validator dan menguji tampilan halaman di browser.

## Bagian 7: Exit ticket

1. HTML digunakan untuk menyusun struktur konten halaman web, sedangkan CSS digunakan untuk mengatur tampilan halaman.

2. Selector ID memiliki specificity lebih tinggi daripada selector class dan selector elemen.

3. Saya akan memeriksa struktur HTML, memastikan selector CSS sesuai, dan menggunakan validator untuk menemukan kesalahan.
