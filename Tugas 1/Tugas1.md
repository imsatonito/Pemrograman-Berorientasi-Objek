# Tugas 1

1. Buatlah struktur dasar sebuah halaman HTML yang terdiri dari header, main content, dan footer. Sertakan elemen judul di header, paragraf di main content, dan teks hak cipta di footer.
2. Tulis kode CSS untuk:
   - Mengatur warna latar belakang halaman menjadi biru muda.
   - Mengubah warna teks header menjadi putih.
   - Menambahkan margin 20px di sekitar elemen main.
3. Jelaskan perbedaan antara selektor ID (#), kelas (.), dan elemen di CSS. Berikan contoh penggunaan masing-masing.
4. Jelaskan konsep box model dalam CSS dan bagaimana padding, border, dan margin berpengaruh terhadap elemen. Berikan contoh kode untuk elemen dengan padding 10px, border 2px solid, dan margin 15px.
5. Buatlah kode HTML dan CSS untuk membuat menu navigasi horizontal dengan tiga link: Home, About, dan Contact. Menu ini harus memiliki latar belakang abu-abu dan link berubah warna menjadi merah saat di-hover.

## Jawaban

1.

```html
<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Halaman Web Saya</title>
    <style>
      /* Bagian untuk mendefinisikan gaya CSS internal */
      body {
        font-family: Arial, sans-serif; /* Mengatur jenis font untuk seluruh dokumen */
        margin: 0; /* Menghilangkan margin default */
        padding: 0; /* Menghilangkan padding default */
        display: flex; /* Menggunakan flexbox untuk tata letak */
        flex-direction: column; /* Mengatur arah flex menjadi kolom */
        min-height: 100vh; /* Mengatur tinggi minimum body sesuai tinggi viewport */
        background-color: #f0f0f0; /* Mengatur warna latar belakang body */
      }
      header {
        background-color: #3498db; /* Mengatur warna latar belakang header */
        color: white; /* Mengatur warna teks header */
        text-align: center; /* Mengatur perataan teks header ke tengah */
        padding: 20px; /* Menambahkan ruang dalam di sekitar konten header */
      }
      main {
        flex: 1; /* Mengatur main content untuk mengisi ruang yang tersedia */
        padding: 20px; /* Menambahkan ruang dalam di sekitar konten utama */
        max-width: 800px; /* Mengatur lebar maksimum konten utama */
        margin: 0 auto; /* Memusatkan konten utama */
        background-color: white; /* Mengatur warna latar belakang konten utama */
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Menambahkan bayangan pada konten utama */
      }
      footer {
        background-color: #34495e; /* Mengatur warna latar belakang footer */
        color: white; /* Mengatur warna teks footer */
        text-align: center; /* Mengatur perataan teks footer ke tengah */
        padding: 10px; /* Menambahkan ruang dalam di sekitar konten footer */
      }
    </style>
  </head>
  <body>
    <!-- Bagian tubuh dokumen yang berisi konten yang terlihat -->
    <header>
      <!-- Bagian header halaman web -->
      <h1>Selamat Datang di Halaman Web Saya</h1>
      <!-- Judul utama halaman -->
    </header>

    <main>
      <!-- Bagian konten utama halaman web -->
      <h2>Tentang Kami</h2>
      <!-- Sub-judul untuk bagian "Tentang Kami" -->
      <p>
        Ini adalah paragraf di dalam main content. Anda dapat menambahkan
        informasi penting atau menarik tentang website atau perusahaan Anda di
        sini. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
        eiusmod tempor incididunt ut labore et dolore magna aliqua.
      </p>
      <!-- Paragraf pertama konten utama -->
      <p>
        Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi
        ut aliquip ex ea commodo consequat. Duis aute irure dolor in
        reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
        pariatur.
      </p>
      <!-- Paragraf kedua konten utama -->
    </main>

    <footer>
      <!-- Bagian footer halaman web -->
      <p>&copy; 2024 Halaman Web Saya. Hak Cipta Dilindungi.</p>
      <!-- Teks hak cipta di footer -->
    </footer>
  </body>
</html>
```

2.

```css
body {
  background-color: lightblue; /* Mengatur warna latar belakang halaman menjadi biru muda */
}
header {
  color: white; /* Mengubah warna teks header menjadi putih */
}
main {
  margin: 20px; /* Menambahkan margin 20px di sekitar elemen main */
}
```

3.

- Selektor ID (#) adalah selektor yang mengacu pada elemen HTML berdasarkan atribut id. ID harus unik dan hanya dapat digunakan sekali dalam satu halaman.
- Selektor Kelas (.) adalah selektor yang mengacu pada elemen HTML berdasarkan atribut class. Kelas dapat digunakan lebih dari satu kali dan dapat diterapkan pada elemen yang sama.
- Selektor Elemen adalah selektor yang mengacu pada elemen HTML berdasarkan nama elemen.

Contoh penggunaan:

```css
/* Selektor ID */
#header {
  background-color: #3498db; /* Mengatur warna latar belakang header */
}

/* Selektor Kelas */
.highlight {
  color: red; /* Mengatur warna teks menjadi merah */
}

/* Selektor Elemen */
p {
  font-size: 16px; /* Mengatur ukuran font paragraf */
}
```

4.

- Box model adalah konsep dasar dalam CSS yang menggambarkan bagaimana elemen HTML diatur dalam kotak-kotak. Setiap elemen dianggap sebagai kotak dengan margin, border, padding, dan content.
- Padding adalah ruang di dalam kotak yang menambah ukuran kotak.
- Border adalah garis yang membatasi padding dan margin.
- Margin adalah ruang di luar border yang menambah ukuran kotak.

Contoh kode untuk elemen dengan padding 10px, border 2px solid, dan margin 15px:

```css
.box {
  padding: 10px; /* Menambahkan padding 10px */
  border: 2px solid black; /* Menambahkan border 2px solid */
  margin: 15px; /* Menambahkan margin 15px */
}
```

5.

```html
<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Menu Navigasi</title>
    <style>
      body {
        font-family: Arial, sans-serif; /* Mengatur jenis font untuk seluruh dokumen */
        margin: 0; /* Menghilangkan margin default */
        padding: 0; /* Menghilangkan padding default */
        display: flex; /* Menggunakan flexbox untuk tata letak */
        flex-direction: column; /* Mengatur arah flex menjadi kolom */
        min-height: 100vh; /* Mengatur tinggi minimum body sesuai tinggi viewport */
        background-color: #f0f0f0; /* Mengatur warna latar belakang body */
      }
      header {
        background-color: #3498db; /* Mengatur warna latar belakang header */
        color: white; /* Mengatur warna teks header */
        text-align: center; /* Mengatur perataan teks header ke tengah */
        padding: 20px; /* Menambahkan ruang dalam di sekitar konten header */
      }
      main {
        flex: 1; /* Mengatur main content untuk mengisi ruang yang tersedia */
        padding: 20px; /* Menambahkan ruang dalam di sekitar konten utama */
        max-width: 800px; /* Mengatur lebar maksimum konten utama */
        margin: 0 auto; /* Memusatkan konten utama */
        background-color: white; /* Mengatur warna latar belakang konten utama */
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Menambahkan bayangan pada konten utama */
      }
      nav {
        background-color: #808080; /* Mengatur warna latar belakang navigasi menjadi abu-abu */
        color: white; /* Mengatur warna teks navigasi */
        text-align: center; /* Mengatur perataan teks navigasi ke tengah */
        padding: 10px; /* Menambahkan ruang dalam di sekitar konten navigasi */
      }
      nav a {
        color: white; /* Mengatur warna teks link navigasi */
        text-decoration: none; /* Menghilangkan garis bawah pada link */
        margin: 0 10px; /* Menambahkan margin horizontal pada link */
      }
      nav a:hover {
        color: red; /* Mengubah warna teks link saat di-hover */
      }
    </style>
  </head>
  <body>
    <header>
      <h1>Selamat Datang di Halaman Web Saya</h1>
    </header>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </body>
</html>
```
