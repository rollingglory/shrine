---
description: Daftar komponen minimum yang harus ada pada design system website
---

# Design System Checklist

### Core

Baik website company profile maupun enterprise/web-app, diharuskan ada core component yang menjadi basis dari design system. Penting bagi designer dan engineer untuk dapat memahami secara detil mengenai 3 core component ini.

#### Typography

Berisi **Font** serta **Type Scale**. Dituliskan font apa saja yang digunakan pada website, beserta ukuran-ukurannya. Secara umum dan merujuk pada design system Material, type scale berisi setidaknya:

_Headline 1, Headline 2, Headline 3, Headline 4, Headline 5, Headline 6, Subtitle 1, Subtitle 2, Body 1, Body 2, Button, Caption_ dan _Overline._

Sehingga jika dikelompokkan ada **6 headline, 2 subtitle, 2 body, 1 button, 1 caption** dan **1 overline.** Setiap scale mengandung informasi yang dapat diakses berupa: **text size** dan **line height**.&#x20;

Penting bagi designer dan engineer untuk menjaga konsistensi dari type scale yang ada dan tidak merambah ke font berukuran lain yang tidak dicantumkan dalam type scale.

#### Colors

Seluruh warna yang digunakan pada website. Warna boleh dibuat acak atau dikelompokkan ke berbagai fungsi, seperti memisahkan warna brand, warna teks, warna aksen, warna background, warna state (sukses, error, warning, informasi), dan lain-lain sesuai kebutuhan.

Selain itu, warna khusus pada dark mode juga diperlukan bagi aplikasi/website yang memiliki fitur gelap.

#### Spacing

Mencakup **Spacing System, Margin, Padding** dan (opsional) **Grid/Column System**. Anjuran spacing system yang digunakan adalah faktor dan kelipatan 4. Secara umum berisi (dalam pixel) 1, 2, 4, 8, 12, 16, 20, 24, 28, 32, dst. Penggunaan margin, padding serta sistem grid/column dapat disesuaikan.

### Components

#### Button

Berisi rangkaian button mulai dari standard button, icon button serta text button. Jika ada beberapa macam button, dapat diklasifikasikan ke dalam primary button, secondary button, tertiary button, dst.

#### Input Fields

Berisi rangkaian field input di mana user dapat memasukkan informasi ke dalam field tersebut. Field (terutama text field) biasanya memiliki beberapa state, di antaranya **empty/default, hover, focused, active, error,** dan **disabled**.

#### Effects

Merupakan serangkaian efek/trait pada komponen lain, biasanya mencakup **shadow/elevation, radius** dan **border**. Semua trait ini dapat digunakan ke dalam komponen lain seperti card, container, button, input field, dst.

#### Data State

Pada sebuah container yang memiliki data untuk dimuat atau diproses, misal sebuah list, terdapat beberapa state pada container tersebut yang dapat ditampilkan berdasarkan data yang dimuat.\
State **Complete** adalah state ideal app tersebut di mana data dimuat dengan baik.\
State **Empty** adalah state di mana app sudah memanggil data, namun tidak ada data tersedia.\
State **Loading** adalah state ketika app sedang dalam proses menunggu pengambilan data.\
State **Error** adalah state apabila app tidak dapat mengambil data karena suatu hal.

#### Feedback

Feedback berisi komponen-komponen yang bermaksud untuk memberikan informasi balikan dari suatu aksi yang dilakukan oleh user, bisa berupa notifikasi/**toast**, atau **modal dialog** dengan kemungkinan user untuk menginputkan sesuatu kembali.

#### Cards (opsional)

Card sudah menjadi suatu komponen yang hampir selalu ada di setiap website, sehingga kebutuhan akan card yg terstandarisasi menjadi lebih tinggi supaya engineer tidak meraba-raba dalam membuat komponen yang satu ini. Card menggabungkan container dengan effect, serta layout di dalamnya yang juga merupakan kumpulan komponen-komponen kecil.

#### Navigations (opsional)

Berisi **tab, breadcrumbs, pagination, header** dan (opsional) **footer**. Segala navigasi website sesuai flow/fiturnya bisa diakses oleh user ada di sini.

#### Icons (opsional)

Apabila designer menggunakan icon pack (misal Favicon, atau Flaticon, di mana disediakan juga oleh penyedia icon pack bagi enginer) maka tidak perlu memasukkan list icon ke dalam design system. Akan tetapi, apabila icon yang digunakan agak custom atau buat sendiri, maka penting untuk dimasukkan.
