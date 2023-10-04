# Lab2web2
## Langkah - Langkah Praktikum

### 1. Membuat Dokumen HTML
- Buatlah dokumen HTML seperti berikut
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Dasar</title>
</head>
<body>
  <header>
    <h1>CSS Internal dan <i>Inline CSS</i></h1>
  </header>
  <nav>
    <a href="lab2_css_dasar.html">CSS Dasar</a>
    <a href="lab2_css_eksternal.html">CSS Eksternal</a>
    <a href="lab1_tag_dasar.html">HTML Dasar</a>
  </nav>
  <!-- CSS ID Selector -->
  <div id="intro">
    <h1>Hello World</h1>
<p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
dan CSS.</p>
    <!-- CSS Class Selector -->
    <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
  </div>
</body>
</html>
```
- Selanjutnya buka pada brwoser untuk melihat hasilnya.

![image](https://github.com/adityaputrawijaya/Lab2web2/assets/115687055/4fc19a1c-2500-4b80-ad38-aa761935fa05)


### 2. Mendeklarasikan CSS Internal
- Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen.
```
<head>
  <title>CSS Dasar</title>
  <style>
  body {
  font-family:'Open Sans', sans-serif;
  }
  header {
  min-height: 80px;
  border-bottom:1px solid #77CCEF;
  }
  h1 {
  font-size: 24px;
  color: #0F189F;
  text-align: center;
  padding: 20px 10px;
  }
  h1 i {
  color:#6d6a6b;
  }
  </style>
</head>
```

Selanjutnya simpan perubahan yang ada, dan lakukan refresh pada browser untuk melihat
hasilnya.

![image](https://github.com/adityaputrawijaya/Lab2web2/assets/115687055/c46f1019-2bc7-4cfe-89f3-167ae479a280)


### 3. Menambahkan Inline CSS
- Kemudian tambahkan deklarasi inline CSS pada tag <p> seperti berikut.
```
<p style="color:#77CCEF">
```
- Simpan kembali dan refresh kembali browser untuk melihat perubahannya.

![image](https://github.com/adityaputrawijaya/Lab2web2/assets/115687055/46c9786e-7fb4-45a1-b1e7-d73514df2e5b)


### 4. Membuat CSS Eksternal
- Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.
```
nav {
  background: #20A759;
  color:#fff;
  padding: 10px;
}
nav a {
  color: #fff;
  text-decoration: none;
  padding:10px 20px;
}
nav .active,
nav a:hover {
  background: #0B6B3A;
}
```

- Kemudian tambahkan tag untuk merujuk file css yang sudah dibuat pada bagian
```
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- menyisipkan css eksternal -->
    <link rel="stylesheet" href="style_eksternal.css" type="text/css">
    <title>CSS Dasar</title>
</head>
```

- Selanjutnya refresh kembali browser untuk melihat perubahannya.

![image](https://github.com/adityaputrawijaya/Lab2web2/assets/115687055/0d368a4a-4e74-4830-9969-5699aef4f405)


### 5. Menambahkan CSS Selector
- Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
style_eksternal.css, tambahkan kode berikut.
```
/* ID Selector */
#intro {
  background: #418fb1;
  border: 1px solid #099249;
  min-height: 100px;
  padding: 10px;
}
#intro h1 {
  text-align: left;
  border: 0;
  color: #fff;
}
/* Class Selector */
.button {
  padding: 15px 20px;
  background: #bebcbd;
  color: #fff;
  display: inline-block;
  margin: 10px;
  text-decoration: none;
}
.btn-primary {
  background: #E42A42;
}
```

- Kemudian simpan kembali dan refresh browser untuk melihat perubahannya

![image](https://github.com/adityaputrawijaya/Lab2web2/assets/115687055/9cedb3c5-98e0-4266-a1cf-ba9ad4764761)


### Modul Praktikum Pemrograman Web

## Pertanyaan dan Tugas
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
penjelasannya!
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
penjelasan dan contohnya!
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )
