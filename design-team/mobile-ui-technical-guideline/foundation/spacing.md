---
description: Short distance relationship
---

# Spacing

Dalam menentukan jarak/spasi antar komponen dalam sebuah desain aplikasi _mobile_, digunakan apa yang disebut dengan _**base unit**_. _Base unit_ berupa suatu angka dasar yang menjadi acuan besaran spasi dari desain yang dibuat. Besaran spasi yang dipakai nantinya akan didapat dari kelipatan dan faktor dari _base unit_ itu sendiri.&#x20;

Rolling Glory mengikuti acuan Apple dan Google dalam menentukan _base unit_ untuk spasi, yaitu sebesar **8 **_**pixel/point**_ atau oleh beberapa sumber biasa disebut _**Rule of 8**_. Artinya, segala spasi yang digunakan dalam desain merupakan faktor dan kelipatan dari 8, yaitu 1, 2, 4, 8, 16, 24, 32, dst.

![Rule of 8](<../../../.gitbook/assets/image (34) (1).png>)

Namun banyak kasus di mana penggunaan spasi 8 dirasa terlalu sempit, sementara 16 dirasa terlalu lebar. Maka dari itu toleransi penggunaan angka tengah dapat dilakukan. Seperti pertengahan antara 8 dan 16 adalah 12, maka digunakan spasi sebesar 12 _pixel_. Untuk lebih jelasnya, referensi gambar dari _material design_ dapat membantu _coaster_ memahami _base unit_. (Angka tengah ini secara tidak langsung berupa faktor dan kelipatan dari 4, maka kombinasi _base unit_ 4 dan 8 adalah kombinasi yang cocok)

![Base unit 4 dan 8 dp pada Material Design](<../../../.gitbook/assets/image (32).png>)

Dari sekian banyak angka yang menjadi faktor dan kelipatan 4 dan 8, yang paling banyak digunakan dalam desain aplikasi _mobile_ adalah 2, 4, 8 dan 16 _pixel_.

![Most used spatial system in mobile app UI design](<../../../.gitbook/assets/image (31).png>)

### Aplikasi _Spacing_ Pada Komponen UI

Kapan dan di mana menggunakan 16px? Atau 8px? Atau angka lainnya?&#x20;

Anjuran penggunaan besaran spasi yang dapat membantu _coaster_ adalah dengan bantuan **Aturan 3C **_**(Container, Content, Component)**_**.**

* Aturan untuk _**Container**_ menggunakan spasi dengan angka besar, **minimal 16px** dan diterapkan di semua sisi _(box inset)_.
* Aturan untuk _**Content**_ menggunakan spasi sebesar **4px** untuk _header text_, dan variasi **0-8px** untuk _body text_, serta variasi **8px-16px** untuk spasi dan _padding_ konten (_icon, text_) dalam komponen kecil.
* Aturan untuk _**Component**_ menggunakan spasi sebesar **8px**.

#### 1C: _Container_

_Container_ merupakan sebuah bingkai yang menyimpan berbagai konten di dalamnya. Besaran spasi dari keliling/ujung _container_ terhadap konten didalamnya adalah apa yang disebut dengan _padding_. Sementara spasi antar _container_ atau dengan komponen lain biasa disebut _margin_.

_Padding_ _container_ secara umum lazim menggunakan spasi sebesar **minimal 16px** dan diterapkan di segala sisi, seperti referensi gambar berikut:

![16px padding for containers](<../../../.gitbook/assets/image (6) (1).png>)

#### 2C: _Content_

_Content_ merupakan isi dari _container_. Bisa berupa teks, gambar, _divider_, dan lain-lain. Untuk konten berupa teks _header_ yang berada di dalam suatu _container_, baiknya gunakan spasi (sekaligus padding dari _container_ yang membalut si konten) sebesar **4px**.

![Spasi konten header terhadap container](<../../../.gitbook/assets/image (14).png>)

Sementara untuk spasi antar konten, terutama yang berupa _body text_ yang memiliki posisi bertetanggaan langsung (tidak dipisah oleh _whitespace_) atau berbentuk _list_, bisa menggunakan _range_ angka 0px-8px. Namun dianjurkan menggunakan **2px**.

![Spasi body text](<../../../.gitbook/assets/image (15).png>)

![Padding konten dalam komponen lepas yang berukuran kecil (seperti button)](<../../../.gitbook/assets/image (9).png>)

#### 3C: _Component_

Adalah hubungan spasial antar komponen di dalam suatu _container,_ atau antar _container_ itu sendiri. Besaran umum dari jarak ini adalah **8px**, dan pada kasus khusus, dapat digunakan **4px.**

![Spasi antar komponen. Ungu: 8px, oranye: 4px](<../../../.gitbook/assets/image (39).png>)

![Spasi antar komponen](<../../../.gitbook/assets/image (30).png>)

{% hint style="info" %}
Besaran spasi yang digunakan dalam menciptakan desain tidak melulu kaku dan harus mengikuti aturan yang ada. Desainer memiliki keluwesan dalam menentukan spasi yang cocok untuk desain yang diciptakan. **Poin penting** dalam implementasi spasi pada desain terletak pada **konsistensi angka** yang digunakan, sehingga tidak menimbulkan kebingungan baik bagi sesama desainer maupun _developer_.
{% endhint %}





Referensi untuk bacaan lebih lanjut:

{% embed url="https://marvelapp.com/blog/harmonious-spacing-system-faster-design-dev-handoff/" %}

{% embed url="https://medium.com/swlh/the-comprehensive-8pt-grid-guide-aa16ff402179" %}

{% embed url="https://influencevibes.com/spacing-basics-and-rules-every-designer-should-know/" %}

{% embed url="https://material.io/design/layout/understanding-layout.html#resources" %}
