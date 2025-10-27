# Praktikum 6: Web Framework

- **Nama**  : Rafli Dhiya Fadhaly
- **NIM**   : 312410251
- **Kelas** : TI 24 A2
- **Dosen** : Agung Nugroho, S.Kom., M.Kom.
- **Mata Kuliah** : Pemrograman Web 1

## Tujuan
1. Mahasiswa mampu memahami konsep dasar dari **Web Framework**.  
2. Mahasiswa mampu memahami struktur dasar layout web menggunakan **CSS Framework (Bootstrap)**.  
3. Mahasiswa mampu memahami elemen-elemen dasar pada **CSS Framework**.

---

## Instruksi Praktikum
1. Persiapkan text editor seperti **Visual Studio Code**.  
2. Buat folder baru dengan nama **lab6_css_framework**.  
3. Buat file baru bernama `index.html`.  
4. Buat struktur dasar dari dokumen HTML.  
5. Buatlah layout web sederhana menggunakan **CSS Framework (Bootstrap)**.  
6. Lakukan validasi HTML di [http://validator.w3.org](http://validator.w3.org).

---

## Langkah-langkah Praktikum

### **Step 1 – Membuat Struktur Dasar HTML**
Pada tahap pertama, dibuat **kerangka dasar dokumen HTML** sebagai pondasi sebelum menambahkan framework atau elemen lain.

Struktur ini terdiri dari elemen utama seperti `<!DOCTYPE html>`, `<html>`, `<head>`, dan `<body>`.

```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Praktikum 6 - Web Framework</title>
</head>
<body>
  <h1>Halo Dunia!</h1>
  <p>Struktur dasar HTML berhasil.</p>
</body>
</html>
```

**Screenshot:**  
<img width="1920" height="1080" alt="Screenshot (137)" src="https://github.com/user-attachments/assets/228f9b4f-d870-463d-84a3-e89b6d93d28f" />


---

### **Step 2 – Menambahkan Bootstrap (CSS & JS CDN)**
Langkah kedua adalah menambahkan **Bootstrap Framework** ke dalam proyek dengan menggunakan **CDN (Content Delivery Network)**.  
Bootstrap berfungsi untuk mempermudah pembuatan tampilan web modern dan responsif tanpa menulis CSS manual.

```html
<!-- Tambahkan di <head> -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- Tambahkan sebelum </body> -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

**Screenshot:**  
<img width="1920" height="1080" alt="Screenshot (138)" src="https://github.com/user-attachments/assets/9010a83e-db36-41f7-b011-df98000719a1" />


---

### **Step 3 – Membuat Navbar (Bagian Atas Web)**
Menambahkan **Navbar** sebagai menu navigasi di bagian atas halaman.  
Bootstrap menyediakan komponen `navbar` yang responsif dan bisa otomatis berubah tampilan di layar kecil.

```html
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand" href="#">MyWebsite</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div id="navbarNav" class="collapse navbar-collapse">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a class="nav-link active" href="#">Beranda</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Tentang</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Kontak</a></li>
      </ul>
    </div>
  </div>
</nav>
```

**Screenshot:**  
<img width="1920" height="1080" alt="Screenshot (140)" src="https://github.com/user-attachments/assets/bca0a6fd-d5bb-42ca-85d8-1a6ca7de8440" />


---

### **Step 4 – Menambahkan Hero Section / Header Biru**
Bagian **Hero Section** digunakan untuk menampilkan judul utama halaman.  
Class `bg-primary`, `text-white`, dan `text-center` dari Bootstrap membantu membuat tampilannya menarik.

```html
<header class="bg-primary text-white text-center py-5 mb-4">
  <div class="container">
    <h1 class="fw-light">Selamat Datang di Website Saya!</h1>
    <p class="lead">Belajar menggunakan Bootstrap CSS Framework</p>
  </div>
</header>
```

**Screenshot:**  
<img width="1920" height="1080" alt="Screenshot (141)" src="https://github.com/user-attachments/assets/7f0ce607-94d8-4c94-989d-50cd0d851eb0" />

---

### **Step 5 – Membuat Main Content & Sidebar**
Menggunakan sistem **grid Bootstrap (row & col)** untuk membagi halaman menjadi dua kolom:  
- **Kolom kiri (8)** untuk artikel utama,  
- **Kolom kanan (4)** untuk sidebar dan alert.

```html
<div class="container">
  <div class="row">
    <!-- Kolom Kiri -->
    <div class="col-md-8">
      <h2>Artikel Utama</h2>
      <p>Bootstrap mempermudah pembuatan layout responsif.</p>

      <div class="card mb-3">
        <div class="card-body">
          <h5 class="card-title">Card Contoh</h5>
          <p class="card-text">Contoh penggunaan card Bootstrap.</p>
          <a href="#" class="btn btn-primary">Baca Selengkapnya</a>
        </div>
      </div>
    </div>

    <!-- Kolom Kanan -->
    <div class="col-md-4">
      <h3>Sidebar</h3>
      <ul class="list-group mb-3">
        <li class="list-group-item">Link 1</li>
        <li class="list-group-item">Link 2</li>
        <li class="list-group-item">Link 3</li>
      </ul>

      <div class="alert alert-info">Contoh alert Bootstrap.</div>
    </div>
  </div>
</div>
```

**Screenshot:**  
<img width="1920" height="1080" alt="Screenshot (142)" src="https://github.com/user-attachments/assets/bd9c3281-932f-4d38-96fa-ebe73be836a2" />

---

### **Step 6 – Menambahkan Footer**
Bagian terakhir yaitu **footer**, diletakkan di bawah halaman untuk menampilkan informasi hak cipta.

```html
<footer class="bg-dark text-white text-center py-3 mt-4">
  <div class="container">
    <p class="mb-0">© 2025 Praktikum Web Framework | Bootstrap</p>
  </div>
</footer>
```

**Screenshot:**  
<img width="1920" height="1080" alt="Screenshot (143)" src="https://github.com/user-attachments/assets/db6b711f-632e-4310-97fc-cc11e146146c" />


---

## Hasil Akhir
Tampilan akhir web setelah semua langkah diterapkan:

<img width="1920" height="1080" alt="Screenshot (143)" src="https://github.com/user-attachments/assets/8d5da690-0356-498d-89ba-712fab796bca" />

---

## Bukti Validasi Dokumen

<img width="1920" height="1080" alt="Screenshot (144)" src="https://github.com/user-attachments/assets/fa7b3ee1-1c02-4c7e-892d-d2f9b12be237" />

---

## Kesimpulan
Dari hasil praktikum ini dapat disimpulkan bahwa:
- **Bootstrap** sangat membantu dalam pembuatan tampilan web yang menarik dan responsif.  
- Dengan hanya menambahkan class bawaan Bootstrap, kita dapat membuat layout lengkap tanpa menulis CSS manual.  
- Struktur web terdiri dari **navbar**, **hero section**, **main content**, **sidebar**, dan **footer**, yang seluruhnya dapat dibangun dengan cepat menggunakan Bootstrap.

