---
description: Bunga dan kumbang, selai dan roti, gutter dan margin
---

# Grid & Column

Sebagai alat bantu, grid dan column menjadi tool yang sering digunakan desainer dan biasanya juga oleh front-end web developer. Resolusi yang lebar, dimudahkan dengan adanya grid dan column bagi developer dalam membuat komponen UI yang rapi. Di sisi desainer, grid dan column membantu menjaga konsistensi dari elemen-elemen UI, menciptakan koneksi di antara elemen tersebut dan membantu membangun sistem visual yang telrihat harmonis dan membantu end-user dalam menavigasi app.

Namun begitu, pada desain UI mobile app, seringkali yang digunakan hanyalah column, karena secara natural desain UI mobile app mengalir secara vertikal dari atas ke bawah, sehingga desainer dan engineer hanya perlu memperhatikan konten secara horizontal.

#### Column Usage in Mobile App UI Design

> “What is the optimal number of columns in the grid for mobile?”

Pada desain UI website, penggunaan column sebagai guide sudah sangat lazim, dengan jumlah 12 atau 16 column. Jumlah ini memungkinkan karena website menggunakan viewport/resolusi lebar dan bisa dibuka di layar besar. Namun apabila website bersifat responsif, perlu dipikirkan kembali berapa column yang cocok untuk membantu desainer dalam proses designing. Hal ini serupa dengan problematika jumlah column untuk mobile app.&#x20;

Salah satu sistem column pada mobile app atau website responsive, adalah penggunaan 12 column, sama seperti pada website full-width, karena 12 column memungkinkan desainer untuk menempatkan elemen UI dengan jumlah ganjil atau genap di satu baris (row).

![12 columns untuk canvas mobile app](<../../../.gitbook/assets/image (3) (2).png>)

Untuk simplisitas, beberapa guide menyebutkan bahwa desain UI mobile app hanya membutuhkan 4 hingga 6 column. Hal ini memeungkinkan apabila app yang dibuat termasuk seamless dan sederhana, dengan sedikit elemen atau fitur di dalamnya. Namun apabila desain UI yang digarap merupakan app marketplace, dengan bejibun elemen, 4 atau 6 column bisa dibilang terlalu sedikit untuk mengakomodasi jenis elemen yang beragam dengan ukuran yang berbeda-beda.

**Apakah setiap halaman memerlukan sistem grid/column yang sama?**

Jawaban mudah: Tidak sama sekali.&#x20;

Sebelum memasuki step desain wireframe/lo-fi, desainer dapat menentukan sistem column seperti apa yang cocok untuk desain halaman yang akan digarap. Seringkali beberapa halaman memiliki elemen yang berbeda-beda sehingga sistem column-pun dapat berbeda.

#### Gutter & Margin

Berhubungan dengan spacing, gutter adalah jarak antar column, sementara margin adalah spasi di sebelah kiri dan kanan keseluruhan column. Secara umum, nilai margin untuk column pada desain UI mobile app adalah sebesar **16px**. Nilai ini sejalan dengan aturan spacing pada guide sebelumnya. Sementara, nilai dari gutter, biasanya lebih kecil dari nilai margin, dan pada kasus ini, berada di angka sebesar **8px**.

![Gutter & margin](<../../../.gitbook/assets/image (1) (1) (1).png>)

Tentu aturan column, gutter dan margin ini tidak bersifat memaksa, maka dari itu desainer boleh merubahnya sesuai dengan kebutuhan projek/produk yang digarap.

#### Responsive Columns

Smartphone senantiasa berevolusi, dengan sistem yang lebih canggih, dan resolusi serta ukuran layar yang bervariasi. Untuk mengakomodasi hal ini, desain UI mobile app perlu memiliki guide column yang responsif. Dua hal harus bernilai sama, apapun ukuran layarnya:

1. Gutter
2. Margin

Selama gutter dan margin memiliki nilai yang sama, desain UI akan terlihat konsisten ketika dibuka pada layar dengan ukuran yang berbeda.

Pada figma, konfigurasi ini dapat dilakukan dengan mengubah **Type** Column menjadi **Stretch**. Ketika ukuran layar diubah, lebar tiap kolom akan menyesuaikan, dengan mempertahankan nilai gutter & margin.

![Column type pada figma](<../../../.gitbook/assets/Screen Shot 2022-08-05 at 15.43.40.png>)

#### Consideration

Pengunanaan grid/column baiknya dipadukan dengan sistem spacing yang sudah ada, menggunakan aturan besaran/nilai margin untuk container, card, dan konten, dengan besaran spasi yang seragam dan teratur. Hal ini akan memudahkan baik sesama desainer atau engineer dalam membentuk desain UI, terutama pada mobile app dengan kebutuhan sederhana atau MVP.

Sementara untuk desain UI pada mobile app yang cukup kompleks, sistem spacing dan column dapat disesuaikan sesuai kebutuhan.
