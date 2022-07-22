---
description: Daftar komponen minimum yang harus ada pada design system aplikasi mobile
---

# Design System Checklist

### Core

iOS, Android ataupun Hybrid memiliki kesamaan struktur dalam desain aplikasinya, beberapa di bawah ini adalah fondasi/dasar dari pengembangan aplikasi mobile baik dalam tahap UI/UX atau coding. Di bagian sebelumnya, sudah dijelaskan tiap komponen yang termasuk ke dalam fondasi dari Mobile UI Tech Guideline.

#### Typography

Berisi **Font** serta **Type Scale**. Dituliskan font apa saja yang digunakan pada aplikasi, beserta ukuran-ukurannya. Secara umum dan merujuk pada design system Material, type scale berisi setidaknya:

_Headline 1, Headline 2, Headline 3, Headline 4, Headline 5, Headline 6, Subtitle 1, Subtitle 2, Body 1, Body 2, Button, Caption_ dan _Overline._

Namun skala ini dianggap terlalu banyak, sehingga diberikan perampingan khusus untuk design system mobile, dengan menghapus Headline 5 dan Headline 6.

Sehingga jika dikelompokkan ada **4 headline, 2 subtitle, 2 body, 1 button, 1 caption** dan **1 overline.** Setiap scale mengandung informasi yang dapat diakses berupa: **text size** dan **line height**.&#x20;

Penting bagi designer dan engineer untuk menjaga konsistensi dari type scale yang ada dan tidak merambah ke font berukuran lain yang tidak dicantumkan dalam type scale.

Detail panduan tipografi bisa diakses di sini

{% content-ref url="foundation/typography.md" %}
[typography.md](foundation/typography.md)
{% endcontent-ref %}

#### Colors

Seluruh warna yang digunakan pada aplikasi. Warna boleh dibuat acak atau dikelompokkan ke berbagai fungsi, seperti memisahkan warna brand, warna teks, warna aksen, warna background, warna state (sukses, error, warning, informasi), dan lain-lain sesuai kebutuhan.

Selain itu, warna khusus pada dark mode juga diperlukan bagi aplikasi yang memiliki fitur gelap.

#### Spacing

Mencakup **Spacing System, Margin, Padding** dan (opsional) **Grid/Column System**. Anjuran spacing system yang digunakan adalah faktor dan kelipatan 4. Secara umum berisi (dalam pixel) 1, 2, 4, 8, 12, 16, 20, 24, 28, 32, dst. Penggunaan margin, padding serta sistem grid/column dapat disesuaikan.

Detail panduan spasi bisa diakses di sini

{% content-ref url="foundation/spacing.md" %}
[spacing.md](foundation/spacing.md)
{% endcontent-ref %}

### Components

#### Navigations

Berisi **header** dan **bottom navigation bar**. Segala navigasi aplikasi utama sesuai flow/fiturnya bisa diakses oleh user ada di sini.

#### Button

Berisi rangkaian button mulai dari standard button, icon button serta text button. Jika ada beberapa macam button, dapat diklasifikasikan ke dalam primary button, secondary button, tertiary button, dst.

#### Text Input

Berisi rangkaian field input di mana user dapat memasukkan informasi ke dalam field tersebut. Field (terutama text field) biasanya memiliki beberapa state, di antaranya **empty/default, hover, focused, active, error,** dan **disabled**.

#### Selection

Berisi **checkbox** dan **radio button**, biasanya dua komponen ini mengikuti spesifikasi dari komponen yang sama pada masing-masing platform, dengan behavior yang khusus juga, namun desainer dapat menyeragamkan hal tersebut untuk mendapatkan spesifikasi dan behavior yang sama baik bagi Android atau iOS.

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

Card sudah menjadi suatu komponen yang hampir selalu ada di setiap aplikasi, sehingga kebutuhan akan card yg terstandarisasi menjadi lebih tinggi supaya engineer tidak meraba-raba dalam membuat komponen yang satu ini. Card menggabungkan container dengan effect, serta layout di dalamnya yang juga merupakan kumpulan komponen-komponen kecil.
