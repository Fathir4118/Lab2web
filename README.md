# NAMA : MUHAMMAD FATHIR NURCHOLIS
# NIM : 312410287
# KELAS : TI.24.A.4
# MATKUL : PEMROGRAMAN WEB


# PRAKTEK LATIHAN

# 1
Pada langkah ini, dibuat sebuah file HTML baru (misalnya: lab2_css_dasar.html) yang berisi struktur dasar dokumen HTML.
```html
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
      <a href="lab2 css eksternal.html">CSS Eksternal</a>
      <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    <!-- CSS ID Selector -->
    <div id="intro">
      <h1>Hello World</h1>
      <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>
      <!-- CSS Class Selector -->
      <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
      </div>
</body>
</html>
```

# Hasil
![gambar](https://github.com/Fathir4118/Lab2web/blob/main/Gambar/Screenshot_20251002_132407.jpg) 

# 2
CSS internal ditulis pada bagian `<head>` menggunakan tag `<style>`.
CSS ini digunakan untuk mengatur tampilan elemen pada halaman yang sama.

**code**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Dasar</title>
  <style>
    body {
      font-family:'open sans', sans-serif;
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

<body>
  <header>
    <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    <nav>
      <a href="lab2_css_dasar.html">CSS Dasar</a>
      <a href="lab2 css eksternal.html">CSS Eksternal</a>
      <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    <!-- CSS ID Selector -->
    <div id="intro">
      <h1>Hello World</h1>
      <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>
      <!-- CSS Class Selector -->
      <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
      </div>
</body>
</html>
```

**Hasil**
![gambar](https://github.com/Fathir4118/Lab2web/blob/main/Gambar/IMG_20251002_140100.jpg) 


# 3
Inline CSS ditulis langsung pada elemen HTML menggunakan atribut `style`.
CSS jenis ini hanya berlaku pada elemen yang ditentukan.
**code**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Dasar</title>
  <style>
    body {
      font-family:'open sans', sans-serif;
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

<body>
  <header>
    <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    <nav>
      <a href="lab2_css_dasar.html">CSS Dasar</a>
      <a href="lab2 css eksternal.html">CSS Eksternal</a>
      <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    <!-- CSS ID Selector -->
    <div id="intro">
      <h1>Hello World</h1>
      <p style="text-align: center; color: #ccd8e4;">Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>
      <!-- CSS Class Selector -->
      <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
      </div>
</body>
</html>
```
**hasil**
![gambar](https://github.com/Fathir4118/Lab2web/blob/main/Gambar/Screenshot_20251002_143922.jpg) 

# 4

Selain internal dan inline, CSS juga bisa ditulis terpisah di file `.css`, lalu dipanggil ke HTML dengan `<link>`.
**Kode File CSS (`style_eksternal.css`):**

**code**
```html
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

```html
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
```

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Dasar</title>
  <link rel="stylesheet" href="style_eksternal.css" type="text/css">
  <style>
    body {
      font-family:'open sans', sans-serif;
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

<body>
  <header>
    <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    <nav>
      <a href="lab2_css_dasar.html">CSS Dasar</a>
      <a href="lab2 css eksternal.html">CSS Eksternal</a>
      <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>
    <!-- CSS ID Selector -->
    <div id="intro">
      <h1>Hello World</h1>
      <p style="text-align: center; color: #ccd8e4;">Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>
      <!-- CSS Class Selector -->
      <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
      </div>
</body>
</html>
```

**Hasil**
![gambar](https://github.com/Fathir4118/Lab2web/blob/main/Gambar/IMG_20251002_145157.jpg) 

# 5
Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file 

style_eksternal.css, tambahkan kode berikut.
**code**
```html
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

text-decoration: none
}

.btn-primary {
background: #E42A42;
}
```
**hasil**
![gambar](https://github.com/Fathir4118/Lab2web/blob/main/Gambar/IMG_20251002_225709.jpg) 


# SOAL
! [gambar](https://github.com/Fathir4118/Lab2web/blob/main/Gambar/IMG_20251002_225845.jpg) 

##**1. Eksperimen mengubah properti dan nilai CSS**
Disini saya mencoba mengubah dan menambah properti pada CSS dengan mengacu pada CSS Cheat Sheet.
### Contoh Kode:

```css
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

**hasil**
![gambar](
