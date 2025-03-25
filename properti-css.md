---
icon: file-code
---

# Properti CSS

## 1. align-content

**`align-content`** digunakan dalam **CSS Flexbox** dan **CSS Grid** untuk mengatur perataan baris dalam sebuah container yang memiliki **lebih dari satu baris**. Properti ini hanya berfungsi jika:  `display: flex;` dengan `flex-wrap: wrap; display: grid;`

#### **📌 Sintaks Dasar**

```css
.container {
    display: flex;
    flex-wrap: wrap;
    align-content: center;
}
```

***

### **Nilai yang Didukung oleh `align-content`**

| Nilai                 | Fungsi                                                           |
| --------------------- | ---------------------------------------------------------------- |
| `flex-start`          | Semua baris disejajarkan ke atas                                 |
| `flex-end`            | Semua baris disejajarkan ke bawah                                |
| `center`              | Semua baris berada di tengah                                     |
| `space-between`       | Baris pertama di atas, baris terakhir di bawah, sisanya tersebar |
| `space-around`        | Setiap baris memiliki ruang di atas dan bawah                    |
| `space-evenly`        | Ruang antar baris merata                                         |
| `stretch` _(default)_ | Baris akan diperluas untuk memenuhi container                    |

***

### **Contoh Penggunaan dalam Flexbox**

```css
.container {
    display: flex;
    flex-wrap: wrap;
    height: 300px;
    align-content: space-between;
    background: lightgray;
}

.item {
    width: 100px;
    height: 50px;
    background: royalblue;
    margin: 5px;
}
```

Jika ada lebih dari satu baris, properti `align-content` akan menentukan cara baris-baris tersebut disusun di dalam container.

```
<h2>Contoh align-content dalam Flexbox</h2>
    <div class="container">
        <div class="item">1</div>
        <div class="item">2</div>
        <div class="item">3</div>
        <div class="item">4</div>
        <div class="item">5</div>
        <div class="item">6</div>
        <div class="item">7</div>
        <div class="item">8</div>
        <div class="item">9</div>
        <div class="item">10</div>
    </div>
```

***

### **Perbedaan `align-content` vs `align-items`**

| Properti        | Fungsi                                    |
| --------------- | ----------------------------------------- |
| `align-content` | Mengatur posisi **baris** dalam container |
| `align-items`   | Mengatur posisi **item** dalam satu baris |

### 2. Align Items

`align-items` adalah properti CSS yang digunakan untuk menentukan bagaimana elemen-elemen dalam **container flexbox** disejajarkan sepanjang **sumbu silang (cross axis)**.

### Nilai-nilai `align-items`

1. **stretch** _(default)_: Elemen akan diperluas agar memenuhi tinggi container (jika tidak ada tinggi yang ditentukan).
2. **flex-start**: Elemen akan disejajarkan ke awal sumbu silang.
3. **flex-end**: Elemen akan disejajarkan ke akhir sumbu silang.
4. **center**: Elemen akan disejajarkan ke tengah sumbu silang.
5. **baseline**: Elemen akan disejajarkan berdasarkan garis dasar teksnya.

### Contoh Penggunaan

#### Contoh 1: Menggunakan `align-items: center;`

```css
.container {
    display: flex;
    align-items: center;
    height: 200px;
    background-color: lightgray;
}
.item {
    width: 50px;
    height: 50px;
    background-color: blue;
    color: white;
    text-align: center;
}
```

```html
<div class="container">
    <div class="item">1</div>
    <div class="item">2</div>
    <div class="item">3</div>
</div>
```

Hasilnya: Elemen akan berada di tengah secara vertikal.

#### Contoh 2: Menggunakan `align-items: flex-start;`

```css
.container {
    display: flex;
    align-items: flex-start;
}
```

Hasilnya: Semua elemen akan sejajar di bagian atas.

#### Contoh 3: Menggunakan `align-items: stretch;`

```css
.container {
    display: flex;
    align-items: stretch;
}
.item {
    width: 50px;
}
```

Hasilnya: Elemen akan merentang secara otomatis mengisi tinggi container.

### Kesimpulan

`align-items` sangat berguna untuk mengontrol posisi elemen dalam flexbox secara vertikal, tergantung pada sumbu silang yang digunakan. Dengan memahami properti ini, tata letak desain menjadi lebih fleksibel dan responsif.

