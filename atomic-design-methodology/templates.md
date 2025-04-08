# Templates

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

***

### **Templates dalam Atomic Design**

#### Peralihan dari Analogi Kimia

Pada tahap ini, kita **meninggalkan analogi kimia** (atom, molekul, organisme) karena sudah waktunya memakai istilah yang lebih **familiar dan fungsional** dalam konteks UI nyata — terutama untuk **stakeholder non-teknis** seperti klien atau manajer.

***

Apa itu Template?

**Templates** adalah **kerangka halaman** (page-level objects) yang:

* Menempatkan **komponen UI** (atom, molekul, organisme) ke dalam **layout nyata**
* Menunjukkan **struktur konten dasar** dari sebuah halaman
* Menyusun **sistem antarmuka yang utuh dan berfungsi penuh**

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

***

#### 🧩 Contoh Sederhana:

Misalnya kita sudah membuat organisme header (dengan menu dan pencarian), dan organisme footer.

Dalam **homepage template**, kita susun seperti ini:

```
Template: Beranda
┌────────────────────────────┐
│     Header Organism        │
├────────────────────────────┤
│   Banner Gambar Besar      │
│   Daftar Artikel (Organism)│
│   Sidebar (Organism)       │
├────────────────────────────┤
│     Footer Organism        │
└────────────────────────────┘
```

Template ini **belum diisi konten final**, tapi sudah menunjukkan **struktur kontennya**:

* Di mana gambar besar akan tampil?
* Di mana heading artikel diletakkan?
* Berapa panjang maksimal teks dalam satu paragraf?

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

***

#### 📌 Kenapa Templates Itu Penting?

1. ✅ **Menghubungkan komponen ke konteks nyata**
2. ✅ **Membantu tim melihat tampilan halaman secara keseluruhan**
3. ✅ **Menjelaskan struktur konten yang ideal** (misalnya ukuran gambar, panjang teks)
4. ✅ **Menjadi fondasi sistem yang dinamis** — siap menampung konten berbeda-beda

***

#### 💬 Kutipan Penting:

> "You can create good experiences without knowing the content. What you can’t do is create good experiences without knowing your content structure,"\
> — **Mark Boulton**

***

#### 🎯 Intinya:

Template adalah **kerangka tampilan** yang:

* Memastikan **komponen berfungsi dalam konteks halaman**
* Menjadi jembatan antara **desain dan implementasi**
* Menyediakan **batasan dan pedoman** untuk konten yang dinamis

