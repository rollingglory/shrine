---
description: Styles of the family
---

# Typography

Tipografi yang digunakan dalam suatu aplikasi _mobile_ memiliki andil dalam merepresentasikan _brand_ yang diangkat. Selain keperluan tersebut, tipografi juga baiknya memiliki aturan penggunaan sebagai komponen dalam aplikasi serta bersifat memudahkan bagi pengguna yang membacanya.

Teks yang terlalu kecil akan menyulitkan pengguna untuk membaca informasi yang disediakan, pun teks terlalu besar bisa mengganggu mata dari pengguna. Oleh karena itu, kebutuhan akan ukuran yang pasti sebagai dasar penggunaan teks dan skalanya menjadi penting, dan untuk mencapai hal tersebut, setidaknya diperlukan pertimbangan dalam menentukan _**font size**_ dan _**line height**_ yang cocok bagi aplikasi yang akan digarap.

Kombinasi dari _font size_ dan _line height_ dengan rasio yang cocok akan memudahkan baik desainer dan developer dalam mengembangkan aplikasi, serta memudahkan pengguna dalam membaca informasi yang disajikan.

#### **Font Size**

_Font size_ merupakan ukuran dari karakter dalam teks itu sendiri. Ditentukan dalam _unit_ px atau pixel, serta diklasifikasikan sesuai fungsi dari setiap ukuran yang ada.

Dalam aturan ukuran teks pada aplikasi _mobile_, ada _guideline_ yang dimiliki oleh Apple dan Google.

Apple pada halaman **Human Interface Guidelines**-nya menuliskan bahwa teks tidak boleh lebih kecil dari 11px, serta _body text_ utama baiknya berukuran 17px.

Google pada halaman **Material Design Guidelines**-nya menuliskan teks terkecil pada aplikasi _mobile_ adalah 12px, serta _body text_ utama berukuran 16px.

Tentu kedua aturan tersebut tidak bersifat wajib diikuti sepenuhnya, karena perlu diingat, masing-masing _brand_ menetapkan aturan tersebut berdasarkan OS _smartphone_ yang dimiliki. iOS, macOS, serta ipadOS memiliki rentetan _guideline_ yang setelah melewati banyak perhitungan, dianggap cocok untuk menggunakan aturan 11px-17px di atas.

Begitu pula Google, bersama AndroidOS-nya, menentukan ukuran cocok bagi teksnya di angka 12px-16px.

#### **Line Height**

_Line height_ adalah jarak/spasi dari suatu teks dengan baris lebih dari satu, biasanya berupa paragraf. Penggunaan _line height_ yang baik akan membantu tingkat _readability_ teks yang disajikan. Sebaliknya, _line height_ yang tidak baik akan menyulitkan pengguna dalam membaca informasi. _Line height_ variatif sendiri umumnya hanya diaplikasikan pada teks berbentuk paragraf, namun jika diperlukan, dapat digunakan pada teks berbentuk _label_, _placeholder_, _text field_, dan lain-lain.

Untuk mengakomodir _readability_ suatu paragraf, diperlukan _line height_ yang sedikit lebih besar dari _font size_ yang dipakai. Tidak ada besaran pasti yang dapat menentukan ukuran _line height_ yang paling baik. Google, melalui **Material Design 3**-nya tidak menentukan takaran pasti bagi _line height_ di setiap skala tipografi yang mereka miliki. Semakin kecil _font size_, maka semakin besar rasio-nya _line height_-nya. Sebagai contoh, skala _Display Large_ Material memiliki _size_ 57 dengan _line height_ 64 (sekitar 1,12x), sementara skala _Headline Large_ memiliki _size_ 32 dan _line height_ 40 (rasionya sebesar 1,25x).

Sementara **Human Resource Guideline** Apple memiliki skala teks _Large Title_ dengan ukuran 34 dan _line height_ 41 (sekitar 1,2x) dan _Body Text_ ukuran 17 dengan _line height_ 22 (rasio 1,29).&#x20;

Ketidakseragaman ini mungkin membingungkan bagi baik desainer dan developer, namun setelah ditelaah lebih jauh, bagi aplikasi _mobile_, rasio _line height_ ini seringkali berada di antara 1,2 hingga 1,5x dari _font size_ yang dipakai, dengan aturan berbanding terbalik dimana _font size_ yang lebih kecil memiliki rasio _line height_ yang lebih besar.

{% hint style="info" %}
Jika menyulitkan, desainer dapat mematok rasio **1,3x** bagi _line height_, berapapun ukuran _font_-nya.
{% endhint %}

#### Font Type/Family

_Font_ yang digunakan pada aplikasi mobile juga perlu ditentukan, _font_ tersebut harus sesuai dengan _brand_ yang diangkat, tingkat _readability_-nya, dan juga dicek penggunaan hak ciptanya. Biasanya satu aplikasi atau _brand_ akan menggunakan satu tipe _font family_, atau maksimal dua tipe. Dengan klasifikasi satu tipe untuk _body text_ dan satu lainnya untuk _title/headline_. Pada dasarnya tidak ada aturan khusus mengenai penggunaan _font type/family_ pada aplikasi, sehingga pada hal ini desainer memiliki kebebasan untuk memilih _font_ yang digunakan.

#### Type Scale

_Type scale_ merupakan rentetan ukuran kombinasi _font size_ dan _line height_ tertentu yang tiap ukurannya berbeda, sehingga dapat digunakan pada tipe-tipe teks yang berbeda pula. Skala ini, pada **Material Design** dibagi ke dalam _headline, subtitle, body, button, caption_ dan _overline_. Sementara pada **Human Interface Guideline** Apple, dibagi ke dalam _title, headline, body, subhead, footnote, callout_ dan _caption_. Keduanya memiliki skala yang berbeda, dengan perhitungan masing-masing dalam menentukan _font size_ dan _line height_ tiap ukuran.

Secara praktis, tidak ada aturan pasti dalam menentukan ukuran _type scale_, namun di banyak kasus dan kebutuhan _mobile app_, biasanya ukurannya berkisar di antara 10px sebagai ukuran terkecil, dan 24px sebagai ukuran terbesar. Ukuran lebih besar dari 24px kadang digunakan, terutama pada aplikasi iOS, karena memiliki ukuran judul halaman atau _large title_ yang membutuhkan ukuran lebih besar, yakni dengan _font size_ 34px.

{% hint style="info" %}
App iOS dan AndroidOS memiliki karakterisik yang berbeda, desainer dapat mengikuti guideline dari salah satu OS tersebut atau meleburnya untuk menciptakan type scale universal untuk app mobile.
{% endhint %}

_Guideline Design System_ _website_ yang digunakan Rolling Glory menggunakan skala Material Design dengan detail ukuran **6 **_**headline**_**, 2 **_**subtitle**_**, 2 **_**body text**_**, 1 **_**button**_**, 1 **_**caption**_**,** dan **1 **_**overline**_**.**  Skala ini bisa saja digunakan untuk _mobile app_, namun pada skenario riil, _headline_ 1 hingga 5 malah jarang sekali digunakan. _Headline_ 6 dengan _size_ 24px adalah ukuran yang paling sering digunakan sebagai ukuran terbesar. Untuk menanggulangi hal itu, skala bagi _design system mobile_ akan mengadopsi Material Design namun dengan beberapa _tweaking_.&#x20;

{% hint style="info" %}
Perlu diketahui, skala di bawah ini bisa ditambah sesuai dengan kebutuhan dan kreativitas desainer.
{% endhint %}

**Mobile Type Scale**

<table><thead><tr><th width="150">Scale</th><th width="150">Font Size</th><th width="150">Line Height* (approx. 1,3x of font size)</th><th width="300.1538461538462">Usage</th></tr></thead><tbody><tr><td>Headline 1</td><td>32/34</td><td>40/42</td><td>iOS large title</td></tr><tr><td>Headline 2</td><td>24</td><td>30</td><td>Banner title</td></tr><tr><td>Headline 3</td><td>20</td><td>26</td><td>Header title, page title, banner title, section title</td></tr><tr><td>Headline 4</td><td>18</td><td>24</td><td>iOS page title</td></tr><tr><td>Subtitle 1</td><td>16</td><td>20</td><td>Section title</td></tr><tr><td>Subtitle 2</td><td>14</td><td>18</td><td>Secondary section title</td></tr><tr><td>Body 1</td><td>16</td><td>20</td><td>Primary body text</td></tr><tr><td>Body 2</td><td>14</td><td>18</td><td>Secondary body text</td></tr><tr><td>Button</td><td>14</td><td>14</td><td>Button</td></tr><tr><td>Caption</td><td>12</td><td>16</td><td>Caption, label</td></tr><tr><td>Overline</td><td>10</td><td>13</td><td>Secondary label, tag title</td></tr></tbody></table>

Beberapa hal yang perlu diperhatikan untuk _text scale_ di atas adalah:

1. Pada komponen teks tunggal (bukan paragraf atau _button_), desainer dan developer bisa menghiraukan _line height_ (membuat _line height_-nya 1x dari _font size_), supaya posisi teks tersebut bisa dengan tepat berada di tengah _container_.
2. _Subtitle_ dan _body_ memiliki ukuran yang sama, yang membedakannya hanyalah pada _font weight_. _Body_ biasanya memiliki _weight_ regular (400\~500) sementara _subtitle_ memiliki _weight_ lebih _medium/semibold_ (600\~800).

**Contoh penggunaan **_**type scale**_

![Penggunaan type scale pada UI #1](<../../../.gitbook/assets/Screen Shot 2022-07-20 at 16.39.54.png>)

![Penggunaan type scale pada UI #2](<../../../.gitbook/assets/Screen Shot 2022-07-20 at 16.41.48.png>)

Referensi untuk bacaan lebih lanjut:

{% embed url="https://developer.apple.com/design/human-interface-guidelines/foundations/typography/" %}

{% embed url="https://material.io/design/typography/the-type-system.html" %}
