---
description: 'My canvas, my adventure'
---

# Intro: Canvas

Sebelum beranjak ke dalam _guideline,_ perlu diketahui elemen penting mendasar yang dapat mengurangi perbedaan implementasi ketika _development_ sudah dijalankan. Yaitu penggunaan _canvas_ dalam menciptakan desain. 

Referensi _canvas_ diambil dari statistik pengguna _smartphone_ dunia, dengan mengambil tipe _smartphone_ yang paling banyak digunakan baik bagi perangkat iOS maupun Android. Dari sini desainer dan _developer_ diberikan kemudahan untuk menentukan ukuran _canvas_ yang tepat dengan cara yang sederhana, yaitu:

#### Langkah 1: Pilih referensi _platform_ \(iOS atau Android\)

Bisa dipilih sesuai arahan manajer, atau pertimbangan dari _device_ yang digunakan klien.

#### Langkah 2: Gunakan _canvas_ di bawah ini sesuai pilihan _platform_

| Platform | iOS | Android |
| :--- | :---: | :---: |
| **Device - Phone** | iPhone X | Google Pixel 2 |
| **Canvas Size** | 375 x 812 | 411 x 731 |
| **Device - Tablet** | iPad Pro 11" | Surface Pro 3 |
| **Canvas Size** | 834 x 1194 | 990 x 1440 |

#### Penting: Pertimbangan _safe area_

Ukuran _canvas_ pada tabel di atas sudah mencakup ukuran keseluruhan dari _device_ yang dituju, seperti pada iPhone X, ukuran 375 x 812 sudah mencakup bagian atas \(_status bar_\) dan bawah \(_home indicator_\) yang mana merupakan _unsafe area_ di mana sebaiknya tidak menaruh desain di _area_ ini, dan menambahkan _padding_ lebih sesuai ukuran dari _area_ tersebut.

![iOS safe area](../../.gitbook/assets/image%20%2824%29.png)

Desainer sebaiknya memberi _padding_ atas sebesar 44px dan bawah sebesar 34px ketika menggunakan _canvas_ iPhone X, atau menambahkan _status bar_ dan _home indicator_ pada desain.

Hal yang sama berlaku pada Google Pixel 2, di mana ukuran 411 x 731 sudah mencakup bagian _status bar_ dan _navigation button \(back, home, running apps\)._

![Status bar Android setinggi 24dp \(24px\)](../../.gitbook/assets/image%20%2819%29.png)

![Android navigation bar setinggi 48dp \(48px\)](../../.gitbook/assets/image%20%2811%29.png)

Desainer sebaiknya memberi padding atas sebesar 24px dan bawah sebesar 48px ketika menggunakan _canvas_ Google Pixel 2, atau menambahkan _status bar_ dan _android navigation bar_ pada desain.





Referensi untuk bacaan lebih lanjut:

{% embed url="https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/adaptivity-and-layout/" %}

{% embed url="https://material.io/design/platform-guidance/android-bars.html\#android-navigation-bar" %}

