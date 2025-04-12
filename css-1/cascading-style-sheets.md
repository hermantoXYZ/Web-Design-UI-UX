---
icon: file-code
---

# Cascading Style Sheets

## 1. Apa Itu CSS?

CSS (**Cascading Style Sheets**) adalah bahasa desain yang digunakan untuk mengatur tampilan dan tata letak elemen pada halaman web. CSS memungkinkan kita untuk mengontrol warna, font, ukuran, posisi, animasi, dan responsivitas sebuah website tanpa harus mengubah struktur HTML-nya.

<figure><img src="../.gitbook/assets/image (4) (1) (1).png" alt=""><figcaption></figcaption></figure>

## **2. Mengapa CSS Penting?**

* **Memisahkan desain dari struktur** → HTML digunakan untuk menyusun konten, sedangkan CSS untuk mempercantik tampilan.
* **Memudahkan pengelolaan** → Dengan CSS, satu perubahan di file eksternal bisa mempengaruhi seluruh halaman web.
* **Meningkatkan performa** → Website jadi lebih cepat karena kode HTML tidak dipenuhi dengan styling.
* **Membuat website responsif** → Dengan CSS, tampilan web bisa menyesuaikan berbagai ukuran layar (PC, tablet, HP).

## 3. Bagaimana Cara Menggunakan CSS?

There are three ways of inserting a style sheet:

* External CSS `link rel="stylesheet" href="style.css"`
* Internal CSS  `<style>{ color: red; }</style>`&#x20;
* Inline CSS `style="color: red;"`

### 3.1 External CSS

**External CSS** (file terpisah dengan ekstensi `.css`)

File CSS (`style.css`)

```css
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    text-align: center;
    padding: 50px;
}

h1 {
    color: #f30909;
}
```

HTML (`index.html`)

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Halaman Web Saya</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Halo, Dunia!</h1>
    <p>Ini adalah halaman web pertama saya.</p>
</body>
</html>

```

### **3.2 Internal CSS?**

Internal CSS adalah cara menambahkan style langsung ke dalam halaman HTML menggunakan tag `<style>` di dalam bagian `<head>` dokumen.

***

#### **Cara Menggunakan Internal CSS**

Berikut adalah contoh struktur penggunaan **Internal CSS**:

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Belajar Internal CSS</title>
    <style>
        body {
            background-color: #f4f4f4;
            font-family: Arial, sans-serif;
        }
        h1 {
            color: blue;
            text-align: center;
        }
        p {
            font-size: 18px;
            color: #333;
        }
    </style>
</head>
<body>
    <h1>Halo, Ini Internal CSS!</h1>
    <p>Ini adalah contoh penggunaan internal CSS dalam HTML.</p>
</body>
</html>
```

***

#### **Penjelasan Kode di Atas**

1️⃣ **Internal CSS diletakkan di dalam `<style>` di dalam `<head>`**

```html
<style>
    body {
        background-color: #f4f4f4;
        font-family: Arial, sans-serif;
    }
</style>
```

* Mengatur warna latar belakang halaman menjadi abu-abu muda (`#f4f4f4`).
* Mengatur font default halaman menjadi Arial atau sans-serif.

2️⃣ **Selector untuk Elemen HTML**

```css
h1 {
    color: blue;
    text-align: center;
}
```

* Semua `<h1>` akan berwarna biru dan teksnya rata tengah.

```css
p {
    font-size: 18px;
    color: #333;
}
```

* Semua `<p>` memiliki ukuran font **18px** dan warna teks abu-abu gelap (`#333`).

***

#### **Kelebihan & Kekurangan Internal CSS**

✅ **Kelebihan**\
✔️ Lebih terorganisir dibanding **Inline CSS**.\
✔️ Tidak perlu file terpisah seperti **External CSS**.\
✔️ Cocok untuk halaman sederhana atau pengujian cepat.

❌ **Kekurangan**\
✖️ Tidak efisien untuk proyek besar (lebih sulit dikelola).\
✖️ Jika ada banyak halaman, style harus ditulis ulang di setiap halaman.\
✖️ Memperlambat loading jika terlalu banyak kode dalam `<head>`.

***

### **Inline CSS?**

**Inline CSS** adalah cara menerapkan CSS langsung ke dalam elemen HTML menggunakan atribut `style`.

***

#### **Cara Menggunakan Inline CSS**

Inline CSS ditulis langsung di dalam tag HTML seperti ini:

```html
<p style="color: red; font-size: 20px;">Ini adalah teks merah dengan ukuran 20px.</p>
```

***

#### **Contoh Penggunaan Inline CSS dalam HTML**

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Belajar Inline CSS</title>
</head>
<body>
    <h1 style="color: blue; text-align: center;">Halo, Ini Inline CSS!</h1>
    <p style="font-size: 18px; color: green;">Teks ini berwarna hijau dengan ukuran 18px.</p>
    <button style="background-color: orange; color: white; padding: 10px 20px; border: none;">
        Klik Saya
    </button>
</body>
</html>
```

***

#### **Penjelasan Kode**

1️⃣ **Inline CSS ditulis langsung di atribut `style` dalam tag HTML**

```html
<h1 style="color: blue; text-align: center;">Halo, Ini Inline CSS!</h1>
```

* `color: blue;` → Mengubah warna teks menjadi biru
* `text-align: center;` → Membuat teks berada di tengah

2️⃣ **Mengubah tampilan teks dengan Inline CSS**

```html
<p style="font-size: 18px; color: green;">Teks ini berwarna hijau dengan ukuran 18px.</p>
```

* `font-size: 18px;` → Mengubah ukuran teks menjadi 18px
* `color: green;` → Mengubah warna teks menjadi hijau

3️⃣ **Mengubah tampilan tombol dengan Inline CSS**

```html
<button style="background-color: orange; color: white; padding: 10px 20px; border: none;">
    Klik Saya
</button>
```

* `background-color: orange;` → Mengubah warna latar belakang tombol menjadi oranye
* `color: white;` → Mengubah warna teks menjadi putih
* `padding: 10px 20px;` → Menambahkan jarak dalam tombol
* `border: none;` → Menghilangkan garis tepi tombol

***

#### **Kelebihan & Kekurangan Inline CSS**

✅ **Kelebihan**\
✔️ Mudah diterapkan pada satu elemen tanpa membuat file CSS terpisah.\
✔️ Berguna untuk pengujian cepat atau styling khusus.\
✔️ Prioritas tertinggi dibanding Internal & External CSS.

❌ **Kekurangan**\
✖️ Tidak efisien untuk proyek besar karena sulit dikelola.\
✖️ Mengurangi keterbacaan kode HTML.\
✖️ Tidak dapat digunakan kembali untuk elemen lain.

***

####
