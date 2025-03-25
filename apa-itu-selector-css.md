---
icon: file-code
---

# Apa Itu Selector CSS?

**Selector CSS** digunakan untuk memilih elemen HTML yang ingin diberi gaya (style). Dengan selector, kita bisa menentukan elemen mana yang akan diubah tampilannya.

<figure><img src=".gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

***

### **1️⃣ Jenis-Jenis Selector CSS**

<figure><img src=".gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

#### **1. Selector Elemen (Tag Selector)**

Memilih semua elemen dengan tag tertentu.

🔹 **Contoh:**

```css
p {
    color: blue;
    font-size: 18px;
}
```

🔹 **Penjelasan:**

* Semua `<p>` di halaman akan memiliki teks berwarna **biru** dan ukuran **18px**.

🔹 **HTML:**

```html
<p>Ini paragraf pertama.</p>
<p>Ini paragraf kedua.</p>
```

***

#### **2. Selector ID**

Memilih elemen berdasarkan atribut **id** (`#id`).

> ⚠️ **ID harus unik**, hanya bisa digunakan untuk satu elemen!

🔹 **Contoh CSS:**

```css
#judul {
    color: red;
    text-align: center;
}
```

🔹 **HTML:**

```html
<h1 id="judul">Halo, Dunia!</h1>
```

🔹 **Hasil:**

* `<h1>` dengan **id="judul"** akan berwarna merah dan rata tengah.

***

#### **3. Selector Class**

Memilih elemen berdasarkan **class** (`.class`).

> ✅ **Bisa digunakan untuk banyak elemen!**

🔹 **Contoh CSS:**

```css
.teks-biru {
    color: blue;
    font-weight: bold;
}
```

🔹 **HTML:**

```html
<p class="teks-biru">Teks ini berwarna biru.</p>
<p class="teks-biru">Teks ini juga biru.</p>
```

🔹 **Hasil:**

* Semua elemen dengan **class="teks-biru"** akan berwarna **biru** dan tebal.

***

#### **4. Selector Universal (`*`)**

Memilih **semua elemen** dalam halaman.

🔹 **Contoh:**

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

🔹 **Penjelasan:**

* Menghapus margin dan padding default semua elemen.
* Menerapkan sistem `box-sizing: border-box` agar ukuran elemen tetap stabil.

***

#### **5. Selector Turunan (Descendant Selector)**

Memilih elemen yang berada **di dalam elemen lain**.

🔹 **Contoh:**

```css
div p {
    color: green;
}
```

🔹 **HTML:**

```html
<div>
    <p>Paragraf ini hijau.</p>
</div>
<p>Paragraf ini tidak berubah.</p>
```

🔹 **Hasil:**

* Hanya `<p>` di dalam `<div>` yang akan berubah warna menjadi **hijau**.

***

#### **6. Selector Anak Langsung (`>`)**

Memilih **hanya** anak langsung dari elemen tertentu.

🔹 **Contoh:**

```css
div > p {
    color: orange;
}
```

🔹 **HTML:**

```html
<div>
    <p>Paragraf ini oranye.</p>
    <span>
        <p>Paragraf ini tidak berubah.</p>
    </span>
</div>
```

🔹 **Hasil:**

* `<p>` **langsung** di dalam `<div>` berwarna **oranye**.
* `<p>` **di dalam `<span>`** tidak berubah.

***

#### **7. Selector Saudara Sebaya (`+` & `~`)**

Memilih elemen yang berada setelah elemen tertentu dalam satu level.

**Selector Saudara Langsung (`+`)**

🔹 **Contoh:**

```css
h1 + p {
    color: purple;
}
```

🔹 **HTML:**

```html
<h1>Judul</h1>
<p>Paragraf ini ungu.</p>
<p>Paragraf ini tidak berubah.</p>
```

🔹 **Hasil:**

* Hanya **paragraf pertama** setelah `<h1>` yang berubah jadi **ungu**.

**Selector Saudara Umum (`~`)**

🔹 **Contoh:**

```css
h1 ~ p {
    color: brown;
}
```

🔹 **HTML:**

```html
<h1>Judul</h1>
<p>Paragraf ini cokelat.</p>
<p>Paragraf ini juga cokelat.</p>
```

🔹 **Hasil:**

* Semua `<p>` setelah `<h1>` berubah jadi **cokelat**.

***

#### **8. Selector Atribut**

Memilih elemen berdasarkan atributnya.

**Selector Atribut Spesifik (`[atribut="nilai"]`)**

🔹 **Contoh:**

```css
input[type="text"] {
    border: 2px solid blue;
}
```

🔹 **HTML:**

```html
<input type="text" placeholder="Nama">
<input type="password" placeholder="Kata sandi">
```

🔹 **Hasil:**

* **Hanya** input dengan `type="text"` yang memiliki **border biru**.

**Selector Atribut yang Mengandung Kata Kunci (`*=`)**

🔹 **Contoh:**

```css
a[href*="google"] {
    color: red;
}
```

🔹 **HTML:**

```html
<a href="https://google.com">Google</a>
<a href="https://yahoo.com">Yahoo</a>
```

🔹 **Hasil:**

* **Hanya** link yang mengandung `"google"` yang berwarna **merah**.

***

#### **9. Selector Pseudo-class**

Memilih elemen berdasarkan **keadaan spesifik**.

**Selector `:hover` (Efek Saat Dihover)**

🔹 **Contoh:**

```css
button:hover {
    background-color: green;
    color: white;
}
```

🔹 **HTML:**

```html
<button>Klik Saya</button>
```

🔹 **Hasil:**

* Saat tombol **diarahkan kursor**, warna latar berubah jadi **hijau**.

**Selector `:first-child` (Memilih Elemen Pertama)**

🔹 **Contoh:**

```css
p:first-child {
    font-weight: bold;
}
```

🔹 **HTML:**

```html
<div>
    <p>Paragraf pertama.</p>
    <p>Paragraf kedua.</p>
</div>
```

🔹 **Hasil:**

* **Hanya paragraf pertama** yang menjadi **tebal**.

***

#### **10. Selector Pseudo-element**

Memilih **bagian spesifik** dari elemen.

**Selector `::first-letter` (Huruf Pertama)**

🔹 **Contoh:**

```css
p::first-letter {
    font-size: 30px;
    color: red;
}
```

🔹 **HTML:**

```html
<p>Ini contoh teks.</p>
```

🔹 **Hasil:**

* Huruf pertama pada paragraf menjadi **besar** dan **merah**.

**Selector `::before` dan `::after` (Menambahkan Konten)**

🔹 **Contoh:**

```css
h1::before {
    content: "🔥 ";
}
h1::after {
    content: " 🚀";
}
```

🔹 **HTML:**

```html
<h1>Judul</h1>
```

🔹 **Hasil:**

* **Sebelum** `<h1>` ada emoji **🔥**, **setelahnya** ada emoji **🚀**.

***

