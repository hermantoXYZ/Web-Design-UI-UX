---
hidden: true
icon: react
---

# React X Vitejs

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Installing React

Create a React web application. Here's a step-by-step guide to install and set up a new React project:

1. First, make sure you have Node.js installed. You can check by running on your command line:

```bash
node -v
```

2. Also check if npm (Node Package Manager) is installed:

```bash
npm -v
```

3. Create a new React project using Create React App:

```bash
npx create-react-app .
```

4. Once the installation is complete, install the required dependencies:

```bash
npm install
```

5. Start the development server:

```bash
npm start
```

After following these steps:

* React application will be running at `http://localhost:3000`
* The development server includes hot-reloading, meaning your changes will automatically reflect in the browser
* Basic project structure with:
  * `src/` - contains your source code
  * `public/` - contains static assets
  * `package.json` - lists your project dependencies and scripts
  * `src/App.js` - your main application component

## Installing React using Vite js

Membuat project React menggunakan Vite, yang menawarkan performa lebih cepat dibanding Create React App.

1. Buat project React dengan Vite:

```bash
npm create vite@latest .
```

2. Ketika diminta, pilih:
   * Framework: Pilih "React"
   * Variant: Pilih "JavaScript" (atau "TypeScript" jika ingin menggunakan TypeScript)
3. Install dependencies:

```bash
npm install
```

4. Jalankan development server:

```bash
npm run dev
```

Setelah langkah-langkah di atas:

* Aplikasi akan berjalan di `http://localhost:5173`
* Struktur project Vite lebih sederhana dan ringan dibanding Create React App
* Struktur folder utama:
  * `src/` - kode sumber aplikasi
  * `public/` - asset statis
  * `index.html` - file HTML utama
  * `vite.config.js` - konfigurasi Vite

Keunggulan menggunakan Vite:

* Development server yang jauh lebih cepat
* Build time yang lebih cepat
* Konfigurasi yang lebih sederhana
* Bundle size yang lebih kecil
* Hot Module Replacement (HMR) yang lebih cepat

<figure><img src="../.gitbook/assets/image (4) (1) (1).png" alt=""><figcaption></figcaption></figure>
