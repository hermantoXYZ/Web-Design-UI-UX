---
icon: atom-simple
---

# Organisms

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

***

### **Organisms dalam Atomic Design**

**Organisms** adalah **komponen UI (User Interface)** yang relatif kompleks, terbentuk dari gabungan:

* Molekul
* Atom
* Bahkan organisme lainnya

Organisme mewakili **bagian-bagian nyata dan utuh** dari suatu antarmuka — misalnya: **header**, **footer**, **sidebar**, atau **section berita**.

***

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

#### Contoh Penerapan:

Kita ambil contoh **search form** (formulir pencarian) yang sebelumnya kita anggap sebagai sebuah **molekul**.

Sekarang bayangkan kita menyusun **organisme header**. Maka:

* **Logo** (atom)
* **Menu navigasi** (molekul)
* **Search form** (molekul)
* **Profil pengguna** (molekul atau organisme kecil)

Digabungkan menjadi satu kesatuan: **Organisme Header**

🧠 **Logikanya:**

> Molekul pencarian tidak hidup sendirian. Ia sering muncul **dalam konteks** — misalnya dalam header. Jadi ketika molekul-molekul itu digabung, mereka membentuk **organisme yang utuh** dan memiliki peran spesifik dalam UI.

***

#### Ciri-ciri Organisme:

* Lebih **kompleks** dari molekul
* Memiliki **fungsi spesifik** dan nyata dalam interface
* Bisa terdiri dari **atom, molekul, bahkan organisme lain**
* Menjadi **blok penyusun utama** dalam layout sebuah halaman

***

#### Kenapa Penting?

* Membantu tim UI merancang bagian antarmuka **dengan konteks nyata**
* Menghasilkan sistem desain yang **modular** dan **terstruktur**
* Memudahkan **pemeliharaan dan pengembangan** antarmuka
* Meningkatkan **konsistensi dan efisiensi**

***

#### Ilustrasi Sederhana:

```
Organisme: Header
└── Logo (Atom)
└── Menu Navigasi (Molekul)
└── Form Pencarian (Molekul)
└── Profil Pengguna (Organisme kecil)
```

***

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
