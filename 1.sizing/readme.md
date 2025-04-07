# 📏 Tailwind CSS - Types of Sizing

Dalam Tailwind CSS, terdapat dua jenis pendekatan utama dalam menentukan ukuran elemen: **Fixed Sizing** dan **Relative & Viewport Sizing**. Pemilihan jenis sizing ini penting untuk menciptakan desain yang konsisten dan responsif.

---

## 1. 🔒 Fixed Sizing

Fixed sizing berarti ukuran elemen ditentukan secara tetap menggunakan kelas utilitas seperti `w-16`, `h-8`, `p-4`, dll. Tailwind menggunakan skala spacing yang telah ditentukan sebelumnya.

### ✅ Contoh:

html

```
<div class="w-64 h-32 bg-blue-500">Fixed Size Box (256px x 128px)</div>
```

📌 Ciri-ciri: Ukuran tidak berubah meskipun viewport berubah. Sangat cocok untuk
layout statis atau komponen dengan ukuran spesifik. Lebih mudah dikontrol dan
konsisten.

## 2. 🌐 Relative & Viewport Sizing

Relative sizing menggunakan satuan seperti persen (%), viewport width (vw), viewport height (vh), atau unit
fleksibel lainnya. Tailwind menyediakan utility class untuk mendukung hal ini
seperti w-full, h-screen, w-[80vw], dll.

✅ Contoh:

```
<!-- Menggunakan persen -->
<div class="w-1/2 h-32 bg-green-500">Width 50%</div>

<!-- Menggunakan unit viewport -->
<div class="w-[80vw] h-[60vh] bg-purple-500">80vw width & 60vh height</div>

<!-- Full width & full height of screen -->
<div class="w-full h-screen bg-red-500">Full screen</div>
```

📌 Ciri-ciri: Responsif terhadap perubahan ukuran layar atau kontainer. Cocok
untuk layout adaptif dan mobile-first. Fleksibel dan mengikuti konteks tampilan
pengguna.

📊 Perbandingan Jenis Sizing Kelas Tailwind Responsif Kegunaan Umum
Fixed Sizing w-64, h-32, p-4 ❌ Komponen statis atau ukuran pasti Relative
Sizing w-full, h-screen, w-1/2, w-[80vw] ✅ Desain responsif, layout fleksibel

📝 Kesimpulan Gunakan fixed sizing ketika kamu ingin ukuran elemen tetap dan
konsisten di semua kondisi. Sebaliknya, gunakan relative & viewport sizing
ketika kamu ingin tampilan yang responsif, adaptif, dan menyesuaikan dengan
berbagai ukuran layar. Tailwind CSS mempermudah pengelolaan kedua jenis
pendekatan ini hanya dengan utility class yang intuitif.
