# Dokumentasi Tugas 2 - Pemrograman Web
**Nama:** Muhammad Dzaky  
**NIM:** 123140039  
**Tugas 2:** Halaman utama & Portal Berita ITERA  
**Link Pages:** https://14-039-muhammaddzaky.github.io/PAW_123140039/Tugas%202/  
**Mata Kuliah:** Pengembangan Aplikasi Web

---

## 1. Alasan Penggunaan Struktur Semantik HTML

Penggunaan elemen semantik pada HTML5 memberikan makna  pada struktur halaman web, sehingga memudahkan mesin pencari, pembaca layar , serta pengembang web dalam memahami hirarki dan konten web.

Elemen-elemen semantik yang digunakan dalam proyek ini beserta alasannya:

1. **`<header>`**:
   - **Lokasi & Penggunaan:** Digunakan di bagian paling atas `index.html` dan `berita.html`, serta di dalam elemen `<article>`.
   - **Alasan:** Menandai bagian kepala halaman yang berisi identitas utama seperti logo ITERA, judul utama  `<h1>` , dan tagline  `<h2>` , serta judul artikel berita.
2. **`<nav>`**:
   - **Lokasi & Penggunaan:** Membungkus daftar menu navigasi utama  `<ul>` dan `<li>` .
   - **Alasan:** Membantu agen pengguna  browser & screen reader  mengenali kumpulan tautan navigasi utama website untuk berpindah antar halaman  `index.html` dan `berita.html` .
3. **`<main>`**:
   - **Lokasi & Penggunaan:** Membungkus seluruh konten inti/utama di halaman.
   - **Alasan:** Memisahkan konten utama dari komponen berulang seperti `<header>`, `<nav>`, dan `<footer>`. Setiap halaman hanya memiliki tepat satu elemen `<main>`.
4. **`<section>`**:
   - **Lokasi & Penggunaan:** Digunakan untuk mengelompokkan konten bertema spesifik di halaman utama  Profil, Fakultas & Prodi, Keunggulan Kampus .
   - **Alasan:** Membagi halaman menjadi bagian-bagian logis yang masing-masing dilengkapi dengan judul  `<h2>` / `<h3>` .
5. **`<table>`**:
   - **Lokasi & Penggunaan:** Digunakan pada seksi Fakultas & Program Studi di `index.html`.
   - **Alasan:** Memenuhi ketentuan teknis tugas  minimal 1 tabel  untuk menyajikan data tabular secara terstruktur menggunakan `<caption>`, `<thead>`, `<tbody>`, `<tr>`, `<th>`, dan `<td>`.
6. **`<article>`**:
   - **Lokasi & Penggunaan:** Digunakan pada `berita.html` untuk membungkus berita utama dan pengumuman.
   - **Alasan:** Menandai konten mandiri yang dapat didistribusikan atau dibaca secara independen  seperti artikel berita atau postingan blog .
7. **`<aside>`**:
   - **Lokasi & Penggunaan:** Berada di dalam `<main>` sebagai bilah samping  sidebar .
   - **Alasan:** Menyajikan informasi pelengkap/sekunder yang berhubungan secara tidak langsung dengan konten utama, seperti pengumuman penting, tautan cepat  quick links , dan daftar berita populer.
8. **`<footer>`**:
   - **Lokasi & Penggunaan:** Terletak di bagian bawah halaman.
   - **Alasan:** Menampung informasi penutup seperti alamat kampus  `<address>` , kontak humas/redaksi, serta pernyataan hak cipta  copyright .
9. **Heading Terstruktur  `<h1>` hingga `<h6>` **:
   - **Alasan:** Menjamin hirarki dokumen yang logis dan konsisten dari `<h1>`  judul halaman/site , `<h2>`  sub-bagian utama , `<h3>`  sub-topik , hingga `<h6>`.

---

## 2. Tantangan dan Solusi

During implementation and design, several challenges were addressed:

1. **Tantangan:** Memastikan hirarki heading  `<h1>` - `<h6>`  runtut tanpa ada tingkatan yang terlewat  heading level skip  sesuai aturan semantik HTML5.  
   **Solusi:** Melakukan pemetaan hirarki konten terlebih dahulu sebelum menulis kode HTML, memastikan setiap `<h3>` selalu berada di dalam konteks `<h2>`, dan `<h4>` di dalam `<h3>`.

2. **Tantangan:** Menyusun tabel HTML murni yang informatif dan valid W3C tanpa bergantung pada styling CSS.  
   **Solusi:** Memanfaatkan elemen tabel standar HTML5 seperti `<caption>` untuk judul tabel, `<thead>` untuk baris header, `<tbody>` untuk isi data, serta atribut `<th>` untuk sel judul kolom.

3. **Tantangan:** Memastikan seluruh halaman  `index.html` dan `berita.html`  lolos validasi W3C tanpa error sintaks seperti unclosed tags atau invalid attributes.  
   **Solusi:** Melakukan pengujian berkala menggunakan layanan W3C Markup Validation Service dan memperbaiki seluruh peringatan/penandaan sintaks.

---

## 3. Hasil Validasi W3C

### Hasil Validasi index.html
![Hasil Validasi W3C Index](Validasi%20W3C%20Index.png)

### Hasil Validasi berita.html
![Hasil Validasi W3C Berita](Validasi%20W3C%20Berita.png)
