# Portofolio Pribadi dengan Tailwind CSS

Ini adalah templat portofolio pribadi yang modern, responsif, dan siap pakai, dibangun menggunakan HTML, Tailwind CSS, dan Vanilla JavaScript.

## Fitur

-   **Desain Modern:** Tampilan bersih dengan tema gelap dan warna aksen teal.
-   **Sepenuhnya Responsif:** Tampil sempurna di desktop, tablet, dan perangkat mobile.
-   **Animasi Scroll:** Efek `fade-up`, `fade-right`, dan `fade-left` yang halus saat menggulir halaman, ditenagai oleh AOS.js.
-   **Navbar Interaktif:** Latar belakang navbar berubah menjadi solid saat halaman di-scroll.
-   **Smooth Scroll:** Navigasi yang mulus antar-section.
-   **Form Kontak Siap Pakai:** Terintegrasi dengan [Formspree](https://formspree.io/) untuk pengiriman pesan langsung ke email Anda.

## Cara Menggunakan

### 1. Prasyarat

Tidak ada prasyarat khusus. Anda tidak perlu menginstal Node.js atau Tailwind CLI karena proyek ini menggunakan Tailwind CSS melalui CDN. Cukup unduh atau kloning repositori ini.

### 2. Kustomisasi Konten

Buka file `index.html` dan edit bagian-bagian berikut sesuai dengan data pribadi Anda.

#### a. Mengubah Informasi Pribadi

-   **Nama & Profesi:** Di dalam `<section id="hero">`, ubah "John Doe" dan "Frontend Web Developer".
-   **Foto Profil:** Ganti file `assets/images/profile.jpg` dengan foto Anda. Pastikan nama filenya sama atau perbarui path di `<img>`.
-   **Deskripsi Diri & Skills:** Di dalam `<section id="about">`, ubah teks deskripsi dan daftar `<span>` untuk skills.
-   **Link Sosial Media:** Di `<section id="contact">` dan `<footer>`, ganti placeholder `href="#"` dengan link profil sosial media Anda.

#### b. Menambahkan Proyek Baru

Di dalam `<section id="projects">`, Anda akan menemukan beberapa `<div>` yang merepresentasikan kartu proyek. Untuk menambahkan proyek baru, cukup salin dan tempel salah satu blok kartu proyek.

**Contoh Blok Kartu Proyek:**
```html
<div class="bg-gray-800 rounded-lg overflow-hidden shadow-lg group" data-aos="fade-up" data-aos-delay="300">
    <div class="relative overflow-hidden">
        <img src="assets/images/project-baru.png" alt="Proyek Baru" class="w-full h-48 object-cover group-hover:scale-110 transition-transform duration-300">
        <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity duration-300">
            <a href="[https://link-ke-demo-proyek.com](https://link-ke-demo-proyek.com)" target="_blank" class="px-4 py-2 bg-teal-500 text-white rounded-lg hover:bg-teal-600">Lihat Proyek</a>
        </div>
    </div>
    <div class="p-6">
        <h3 class="text-2xl font-bold text-white mb-2">Nama Proyek Baru</h3>
        <p class="text-gray-400">Deskripsi singkat tentang proyek baru Anda.</p>
    </div>
</div>
```
**Langkah-langkah:**
1.  Siapkan gambar screenshot proyek Anda dan simpan di `assets/images/`.
2.  Perbarui `src` pada tag `<img>`.
3.  Perbarui `href` pada link "Lihat Proyek".
4.  Ubah judul (`<h3>`) dan deskripsi (`<p>`).

#### c. Mengatur Form Kontak

Formulir kontak ini menggunakan **Formspree** untuk mengirimkan pesan ke email Anda tanpa memerlukan backend.

1.  Buka [formspree.io](https://formspree.io/) dan buat akun (gratis).
2.  Buat formulir baru dan Anda akan mendapatkan URL unik, contohnya: `https://formspree.io/f/xxxxxxxx`.
3.  Buka `index.html`, cari `<form>`, dan ganti `action="https://formspree.io/f/YOUR_UNIQUE_ID"` dengan URL unik Anda.

Sekarang, setiap pesan yang dikirim melalui formulir akan diteruskan ke email yang Anda daftarkan di Formspree.

### 3. Deployment

Anda bisa mendeploy situs ini dengan mudah ke berbagai platform hosting statis.

#### Deploy ke GitHub Pages

1.  Buat repositori baru di GitHub.
2.  Unggah semua file proyek (`index.html`, `css/`, `js/`, `assets/`, `README.md`) ke repositori tersebut.
3.  Masuk ke tab **Settings** di repositori Anda.
4.  Di menu samping, pilih **Pages**.
5.  Di bawah "Build and deployment", pilih `main` (atau `master`) sebagai branch sumber.
6.  Klik **Save**.

Tunggu beberapa saat, dan situs portofolio Anda akan aktif di URL seperti `https://<username>.github.io/<nama-repositori>/`.