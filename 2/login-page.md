---
hidden: true
---

# Login Page

Saat mendesain UX/UI untuk halaman login dengan HTML dan CSS, ada beberapa hal penting yang perlu diperhatikan agar pengguna mendapatkan pengalaman yang baik:

#### 1. **Desain Sederhana & Intuitif**

* Buat layout yang bersih dan minimalis.
* Gunakan hierarki visual yang jelas agar pengguna bisa dengan mudah memahami alur login.
* Pastikan hanya elemen yang diperlukan saja yang ditampilkan.

#### 2. **Formulir yang Mudah Diisi**

* Gunakan placeholder dan label yang jelas.
* Pastikan input field cukup besar dan mudah diklik, terutama untuk mobile users.
* Gunakan ikon mata pada input password untuk opsi "show/hide password".
* Tambahkan autofill pada input email/username untuk pengalaman yang lebih baik.

#### 3. **Feedback & Validasi yang Jelas**

* Gunakan validasi real-time untuk memberi tahu pengguna jika ada kesalahan.
* Tampilkan pesan error yang spesifik dan mudah dimengerti, misalnya:
  * ❌ "Email tidak valid"
  * ❌ "Password harus memiliki minimal 8 karakter"
* Gunakan warna yang sesuai, misalnya merah untuk error dan hijau untuk sukses.

#### 4. **Responsiveness & Mobile-Friendly**

* Pastikan desain responsif dan nyaman digunakan di berbagai perangkat.
* Gunakan CSS Flexbox atau Grid agar tata letak dinamis.
* Pastikan ukuran tombol cukup besar untuk layar sentuh.

#### 5. **Keamanan**

* Gunakan input type `password` dengan `autocomplete="off"`.
* Implementasikan CSRF token untuk keamanan tambahan.
* Gunakan `HTTPS` agar data yang dikirim lebih aman.

#### 6. **Aksesibilitas (Accessibility)**

* Gunakan `aria-label` pada elemen input untuk membantu pengguna dengan keterbatasan.
* Pastikan halaman bisa dinavigasi hanya dengan keyboard.
* Kontras warna cukup tinggi agar bisa terbaca dengan jelas.

#### 7. **Fitur Tambahan yang Membantu**

* **Opsi login alternatif**: Misalnya, login dengan Google atau Facebook untuk kemudahan.
* **"Remember Me" Checkbox**: Agar pengguna tidak perlu login ulang setiap saat.
* **"Forgot Password?" Link**: Untuk memudahkan pengguna yang lupa password.

Jika kamu butuh contoh kode HTML & CSS untuk login page, kasih tahu saya ya!&#x20;



<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    /* background-color: #f4f4f4; */
}

/* CSS LOGIN */
.container {
    background: white;
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0 1px 10px rgb(142 142 142 / 10%);
    width: 90%;
    max-width: 400px;
    text-align: center;
}
.logo img {
    width: 120px;
}
.logo h2 {
    color: #4a90e2;
    font-size: 24px;
    margin-top: 5px;
}
.info {
    font-size: 12px;
    color: gray;
    margin: 10px 0;
}
input {
    width: 100%;
    padding: 12px;
    margin: 10px 0;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 14px;
    text-align: left;
}
.terms {
    text-align: left;
    font-size: 12px;
    display: flex;
    display: block;
    align-items: flex-start;
}
.terms a {
text-decoration: none;
}

button {
    width: 100%;
    padding: 12px;
    background: #4a90e2;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
    margin-top: 10px;
}
.links {
    display: flex;
    justify-content: space-between;
    font-size: 12px;
    margin-top: 15px;
}

.links a {
    text-decoration: none;
    color: #4a90e2;
}

.separator {
    margin: 15px 0;
    font-size: 12px;
    color: gray;
}
.google-login {
    background: white;
    color: black;
    border: 1px solid #ccc;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
}
.google-login img {
    width: 20px;
}
@media (max-width: 600px) {
    .container {
        padding: 20px;
    }
}

/* END CSS LOGIN */
```

```html

<div data-gb-custom-block data-tag="load"></div>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DeepSeek Login</title>
    <link rel="stylesheet" href="<div data-gb-custom-block data-tag="static" data-0='styles.css'></div>?v={{ STATIC_VERSION }}"> 
</head>
<body>
    <div class="container">
        <div class="logo">
            <img src="https://unm.ac.id/wp-content/uploads/2022/02/logo-unm-blu-800x186.png" alt="Success">
        </div>
        <p class="info">Silahkan login untuk melanjutkan ke Dashboard layanan Akademik Success FEB UNM</p>
        <form>
            <input type="text" placeholder="Phone number / email address" required>
            <input type="password" placeholder="Password" required>
            <div class="terms">
                <label for="terms">I confirm that I have read, consent and agree to DeepSeek's <a href="#">Terms of Use</a> and <a href="#">Privacy Policy</a>.</label>
            </div>
            <button type="submit">Log in</button>
            <div class="links">
                <a href="#">Forgot password?</a>
                <a href="#">Sign up</a>
            </div>
            <div class="separator">OR</div>
            <button type="submit">Google AUTH</button>
        </form>
    </div>
</body>
</html>
```

Silahkan ubah gambar di atas, menjadi seperti ini:

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>
