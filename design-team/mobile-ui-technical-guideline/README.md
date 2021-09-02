---
description: The right technique meets the best design
---

# Mobile UI Technical Guideline

Kaidah-kaidah fundamental yang penting dalam proses _UI design_, untuk menciptakan desain aplikasi yang tidak hanya _**visually pleasing\***,_ tapi juga _**technically appropriate\***_.

\*menyenangkan mata dan \*sesuai secara teknis

Secara umum, _platform_ tujuan _development_ aplikasi _mobile_ didominasi oleh iOS dan Android \(setidaknya begitu sampai artikel ini dibuat\). Sehingga desainer memiliki 2 sumber referensi dalam menciptakan desain aplikasi _mobile_. _Guideline_ ini dibuat untuk membantu desainer dalam menentukan spesifikasi dalam desain ciptaannya sehingga desain tersebut memiliki spesifikasi yang lazim dan dapat diterima oleh khalayak dan juga harapannya dapat membantu sesama desainer dan _developer_.

Di dalam _guideline_ ini _coaster_ juga bisa menemukan dan memahami istilah dari komponen-komponen utama yang membentuk suatu desain halaman aplikasi _mobile_ yang sudah diamini oleh Rolling Glory, sebagai acuan bagi seluruh _coaster_ dalam berkomunikasi ketika membicarakan sebuah desain, supaya tidak menimbulkan kebingungan karena perbedaan istilah maupun bahasa.

{% hint style="info" %}
_Sebelum memasuki guideline, baiknya coaster melihat dulu pemilihan canvas sebagai persiapan awal membuat desain di halaman berikut_
{% endhint %}

{% page-ref page="intro-canvas.md" %}

Pada dasarnya _guideline_ yang tersedia memiliki tujuan untuk menciptakan _design system_ yang sesuai dengan kaidah-kaidah yang dipaparkan. _Design system_ sebagai hasil akhir dari implementasi seluruh _guideline_ yang akan membantu _coasters_ dalam bekerja. Bersinggungan dengan itu, untuk memudahkan penentuan prioritas desainer dalam mengikuti _guideline_, digunakan apa yang disebut sebagai _**design system complexity pyramid**_, seperti ditunjukkan pada gambar di bawah.

![Design system complexity pyramid](../../.gitbook/assets/image%20%2840%29.png)

Dibaca dari bawah ke atas, dan dimulai dari _**foundation**_ yang mencakup unsur-unsur dasar dalam _UI design_, yang menjadi cikal bakal dari rangkaian komponen sebagai tubuh dari _layout_ desain yang diciptakan untuk diimplementasi oleh _developer_. Unsur-unsur tersebut di antaranya: _grid, column,_ warna, tipografi, jarak \(_space, margin, padding_\), _icon_, dan sebagainya.

Untuk melihat detil dari _guideline foundation_, _coaster_ bisa pindah ke halaman ini:

{% page-ref page="foundation/" %}

Selanjutnya adalah _**core components**_**.** Tingkatan ini berisi komponen-komponen dasar yang lazim ada di dalam sebuah aplikasi _mobile_ secara umum, memiliki sifat tersendiri, bersifat sebagai blok-blok untuk membangun sebuah desain halaman dan biasanya terklasifikasi sesuai _platform_ \(iOS dan Android\). Sehingga dalam _guideline core components, coaster_ akan menemukan berbagai macam komponen yang biasa ditemukan, namun dibedakan sesuai _platform_ dan disediakan pula spesifikasi umumnya.

Untuk melihat detil dari _guideline core component, coaster_ bisa pindah ke halaman ini:

{% page-ref page="core-components/" %}

Setelah _core components_, tingkat selanjutnya adalah _**complex components**_**.** Singkatnya tingkatan ini berisi komponen besar/utuh yang dirangkai oleh beberapa komponen dasar \(_core components_\) dan dibalut oleh unsur-unsur _foundation._ Benda-benda kompleks seperti _scrolling list_ baik yang berbentuk horisontal, vertikal, atau _grid_ \(gabungan keduanya\), _carousel, card,_ serta komponen lain yang menjadi komponen utama dari desain yang diciptakan.

Untuk melihat detil dari _guideline complex component_, _coaster_ bisa pindah ke halaman ini:

{% page-ref page="complex-components.md" %}

Jika ke-tiga tingkatan di atas sudah diimplementasi, maka secara otomatis sudah tercipta sebuah _**layout**_ yang menjadi tahap akhir dari desain suatu halaman pada aplikasi _mobile_. Pada tingkat ini tidak ada _guideline_ spesifik karena pada dasarnya _layout_ merupakan gabungan dari komponen di tahap sebelumnya, baik yang sudah mengikuti spesifikasi anjuran maupun tidak.

Maka dari itu tahap _layout_ tidak akan dipaparkan di dalam sebuah _design system_, tapi sudah terimplementasi di dalam _design file_ baik yang berbentuk _file_ Adobe XD, Figma, atau _software UI design_ lainnya. Melalui _design file_ inilah _coaster_ bisa berkomunikasi secara _non-verbal_ mengenai spesifikasi desain suatu projek atau produk yang sedang digarap. Namun untuk mengganti ketiadaan _guideline_ khusus mengenai _layout_, ada beberapa anjuran terkait _layout_ yang bisa menjadi bahan pertimbangan desainer dalam melakukan proses _layouting_. Untuk hal itu, _coaster_ bisa pindah ke halaman ini:

{% page-ref page="layout.md" %}

Ketika kaidah-kaidah yang sudah dijelaskan dapat diimplementasikan dengan baik, maka seharusnya _design system_ dan _design file_ yang dihasilkan dapat mengurangi--bahkan dalam skenario terbaik, meniadakan--kebingungan yang rentan terjadi dalam proses _hand-off_ dari desainer ke _developer_, dan sebaliknya.



