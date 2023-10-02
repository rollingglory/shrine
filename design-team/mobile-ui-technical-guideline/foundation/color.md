---
description: 50 shades of devs
---

# Color

Seringkali pada suatu desain UI, terdapat terlalu banyak warna yang digunakan secara acak tanpa aturan yang jelas, jikapun ada aturannya, tidak jarang muncul sebuah warna baru yang tidak pernah ditentukan di aturan tersebut sebelumnya.

Penggunaan warna yang teratur melalui sebuah desain sistem dapat membantu:

1. **Klien**, dalam men-visualisasikan brand-nya ke dalam desain dan aplikais;
2. **Desainer**, dalam menentukan warna yang cocok untuk setiap komponen dalam desain;
3. **Engineer**, dalam menentukan warna apa sajaa yang ada, dan warna mana yang harus dipakai untuk komponen tertentu;
4. **Publik**, dalam mengidentifikasi warna yang digunakan, jika diperlukan untuk kebutuhan komunikasi dengan pihak lain.

**Material Design** ([https://material.io/design/color/the-color-system.html#color-usage-and-palettes](https://material.io/design/color/the-color-system.html#color-usage-and-palettes)) yang digunakan Android dan **Human Interface Guidelines** ([https://developer.apple.com/design/human-interface-guidelines/foundations/color](https://developer.apple.com/design/human-interface-guidelines/foundations/color/)) yang digunakan iOS memiliki color system tersendiri. Isinya berupa kumpulan warna-warna dengan spektrum yang luas yang dapat dipilih desainer/engineer dalam menggunakan warna pada desain UI.&#x20;

Dalam menentukan warna untuk design system, sebetulnya tidak ada acuan khusus darimana desainer mengambil warna, apakah dari Material Design, Human Interface Guideline, atau yang lainnya. Bisa saja desainer menentukan palet tertentu untuk mempersembahkan sebuah brand untuk projek/produk yang digarap. Maka dari itu, desainer tidak terpaku atau terkekang dalam memilih warna.

#### Klasifikasi Warna

Pembagian warna menurut fungsinya masing-masing membantu desainer apabila suatu projek digarap oleh beberapa orang, juga membantu engineer dalam mengklasifikasikan warna-warna tersebut ke dalam kode.&#x20;

Secara umum, dengan membawa brand dari projek/produk yang digarap, warna pada design system dapat diklasifikasikan ke dalam 4 kategori, yaitu **Primary Colors**, **Secondary Colors**, **Grayscale/Neutral Colors** dan **Semantic Colors**.

**Primary colors**

Warna-warna primer adalah warna yang paling sering digunakan pada UI, membedakan produk dengan produk lainnya. Warna primer biasanya diambil dari warna utama brand yang diusung. Menggunakan warna brand sebagai warna primer memperkuat identitas brand pada UI yg dibuat.

![Warna primer dan warna brand](<../../../.gitbook/assets/image (3) (2) (1).png>)

**Secondary colors**

Warna sekunder bersifat sebagai komplemen dari warna primer. Warna-warna ini digunakan untuk membuat elemen/komponen UI mendapatkan tingkat fokus lebih dari elemen lainnya.&#x20;

Biasanya, brand memiliki 1-6 warna sekunder, namun pada desain UI mobile, lebih baik mengurangi jumlah warna ini untuk mempertahankan konsistensi dan mengurangi kebingungan pada sisi desainer dan engineer.

**Grayscale/Neutral colors**

Warna grayscale/netral adalah warna yang biasanya digunakan untuk background dan teks. Warna ini mencakup hampir 70-80% dari UI, sifatnya informatif dan berfungsi sebagai netralisir/penengah warna primer dan sekunder supaya UI tidak terkesan terlalu vibran.

Warna netral dapat berupa kumpulan nuansa abu-abu, dari putih hingga hitam, atau diberi hint warna lain, bisa mengikuti warna brand dengan intensitas rendah.

![Warna grayscale/netral untuk background dan teks](<../../../.gitbook/assets/image (51).png>)

**Semantic colors**

Adalah kumpulan warna yang memiliki maksud untuk memberitahukan kondisi tertentu. Secara umum, warna semantik mencakup warna untuk memvisualisasikan status **success, error, warning** dan **information**. Success biasanya diberi warna kehijauan, error diberi warna kemerahan, warning diberi warna kekuningan/keoranyean, dan information biasa diberi warna kebiruan. Bila ada status/kondisi lain, desainer dapat memasukkannya ke dalam warna semantik.

![Warna semantik](<../../../.gitbook/assets/image (34).png>)

#### Color Naming Convention

Mengomunikasikan pewarnaan, atau elemen design system lain kepada engineer, project manager, atau bahkan stakeholder bisa jadi agak sulit apabila tidak ada convention yang jelas. Bagi warna sendiri, lebih mudah mengidentifikasi warna melalui penamaan 'warna primer' daripada menyebutkan kode hexa.

Penamaan warna pada design system searah dengan penggunaan design token. Design token adalah entitas bernama untuk mereferensikan atribut design system (warna, tipografi, spacing, dll). Design token digunakan sebagai pengganti _value hardcode_ dari elemen design system, untuk menciptakan dan me-maintain design system yang scalable.

Pada tahap ini seharusnya desainer sudah menentunkan warna primer, sekunder, netral dan semantik, sehingga sebetulnya klasifikasi ini bisa digunakan sebagai nama dari warna-warna yang ada.

Sebagai contoh, design system memiliki 5 warna pada primary color dengan 1 warna utama. Warna utama ini bisa jadi secara brightness berada di tengah-tengah di antara 4 warna lainnya, dari kondisi ini, dapat ditentukan 5 token, yaitu:

![Warna primer dengan 5 design token](<../../../.gitbook/assets/image (6).png>)

Notice nama **primary-100, primary-90, primary-10, primary-5, primary-110**. Berdasarkan brightness-nya, dari warna utama (100), ke yang lebih terang (<100) dan lebih gelap (>100). Nama inilah yang disebut dengan **token**, dengan fungsi untuk membedakan satu elemen design system dengan yang lainnya (pada kasus ini, membedakan warna).

Pada tahap ini, sebuah design system dengan elemen warna di dalamnya sudah bisa dikatakan rampung, dengan tersedianya warna-warna primer, sekunder, netral, dan semantik. Baik desainer dan engineer tidak perlu bingung memasukkan warna, sehingga tinggal mendaftarkan saja seluruh warna yang sudah ditentukan sebelumnya.

#### BONUS: Color Design Token Usage Guide

Namun muncul pertanyaan baru.

_Warna apa yang harus digunakan untuk subtitle?_\
_Warna apa yang harus digunakan pada background button CTA sekunder?_\
_Warna mana yang merupakan warna disabled pada elemen UI?_

Masalah di atas dapat diselesaikan dengan membuat guideline penggunaan warna design token. Formatnya bisa berupa tabel yang menjelaskan warna dengan token apa, digunakan di elemen UI mana saja. Contoh:

| Color           | Token       | Usage                                        |
| --------------- | ----------- | -------------------------------------------- |
| Gray - #161616  | Neutral-100 | <p>Primary text;<br>Body copy;<br>Header</p> |
| Gray - #a8a8a8  | Neutral-40  | Placeholder text                             |
| White - #ffffff | Neutral-0   | Text on secondary button                     |
| Red - #da1e28   | Error-100   | Error message text                           |
