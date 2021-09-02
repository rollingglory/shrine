# Text Input

Komponen untuk merekam masukan tulisan dari user ke dalam aplikasi, lazim dikenal dengan istilah _text field_ dan _text area_.

Penting untuk desain menampilkan varian/state dari teks input \(bagaimana teks input terlihat saat sedang aktif, error, disabled, dsb.\)

![Text field material](../../../.gitbook/assets/image%20%2816%29.png)

![Text area material](https://gblobscdn.gitbook.com/assets%2F-M2kGe7z4GuDhxTkJybv%2F-MiZg4XzaAvtohB-Oks_%2F-Mi_abYjpRI5gbFpuDWG%2Fimage.png?alt=media&token=d4ba4628-e4dc-4490-9927-01e0da0ace7a)

#### **State Umum** <a id="state-umum"></a>

* Inactive - ketika user tidak memberikan input/gestur apapun terhadap kolom input, dan kolom tersebut kosong
* Focused - ketika user menekan kolom input dan muncul keyboard untuk user melakukan input teks
* Activated - ketika user telah selesai mengisi kolom input dan menekan di luar kolom input sehingga kolom input tidak lagi terfokus
* Error - ketika terjadi kesalahan pada input user \(tidak sesuai validasi\)
* DIsabled - ketika user tidak bisa/tidak boleh melakukan perubahan terhadap isi kolom input

TODO: types, common behavior

**Referensi**

{% embed url="https://material.io/components/text-fields" %}

{% embed url="https://developer.apple.com/design/human-interface-guidelines/ios/controls/text-fields/" %}

