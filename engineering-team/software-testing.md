# Software Testing

> Software testing is the **process of evaluating** a system with the **intent of finding bugs**. And **verifying** that the software product is fit for use and **making sure of the software quality**.

Testing merupakan bagian dari proses development produk digital di Rolling Glory yang sangat krusial. Tujuan utama dari testing ini adalah memastikan bahwa produk digital yang dibuat sesuai dengan solusi yang sudah didesign untuk bisa menjadi solusi untuk masalah yang akan dipecahkan.

Product yang kualitasnya tidak bagus, penuh bug dan sering crash, tidak nyaman dipakai user, performanya tidak baik adalah hal yang sangat bertentangan dengan [forte Rolling Glory, yaitu menghasilkan premium product](../rolling-glory/forte.md).

Sebagian orang tidak aware bahwa testing ini adalah tanggungjawab keseluruhan stakeholder maupun anggota dalam team, bukan hanya QA Tester, namun juga developer, PM, cliend, maupun end-user. Oleh karena itu jika proses testing hanya dibebankan kepada QA Tester, kualitas aplikasi yang dikembangkan tidak akan bisa terjaga. 

### Levels of Testing

Level of testing dalam SDLC \(Software Development Life Cycle\) ditentukan berdasarkan scope dan detail yang di-test, yaitu: **unit** testing, **integration** testing, **system** testing, dan **acceptance** testing. Tujuan pembagian levels ini agak proses testing bisa menjadi lebih sistematis dan dan lebih mudah dalam melakukan testing untuk berbagai scenario yang mungkin muncul.

![4 levels of testing](../.gitbook/assets/image%20%285%29.png)

#### 1 Unit Testing

Bagian terkecil dari aplikasi yaitu code unit \(bisa jadi component, module, class, ataupun function\) harus sudah dipastikan oleh developer bahwa sudah berjalan semestinya, sudah mempertimbangkan berbagai scenario yang mungkin, menghasilkan output yang benar, dan jika ada kesalahan sudah menghandle dengan benar \(jangan sampai runtime error atau crash\).

Yang bertanggungjawab penuh pada fase unit testing ini adalah engineer, sebuah task coding unit mencakup proses unit testing ini, tidak hanya mengimplementasikan saja tanpa melakukan pengetesan untuk semua scenario yang mungkin.

|  |  |
| :--- | :--- |
| Yang di-test | Code unit, individual component |
| Yang dipastikan | Setiap code unit \(component, module, class, function\) sudah berjalan semestinya dalam berbagai scenario |
| Metode pengujian | White box |
| Dilakukan oleh | **Engineer** |

#### 2 Integration Testing

|  |  |
| :--- | :--- |
| Yang di-test | Integrated unit |
| Yang dipastikan | Flow integrated unit \(bisa flow program, flow data antar module, dll\) berjalan semestinya sesuai dengan design dan specification |
| Metode Pengujian | White box & Black box |
| Dilakukan oleh | **Engineer dan QA Tester** |

#### 3 System Testing

Dalam system testing, keseluruhan aplikasi ditest secara black box berdasarkan requirements. Apakah semua scenario baik positif ataupun negatif sudah ter-handle dengan baik semua, apakah UI maupun UX sudah sesuai dengan yang didesign, dan apakah sudah bug-free.Performance dan security testing juga dilakukan di dalam system testing. 

Yang bertanggungjawab dalam melakukan fase system testing ini adalah QA tester, namun yang memiliki accountability adalah Project Manager.

System testing ini adalah proses testing yang terakhir dilakukan tim development sebelum dipresentasikan ke client dan end-user, jadi benar-benar harus dipastikan bahwa dilakukan dengan baik dan benar.

|  |  |
| :--- | :--- |
| Yang di-test | Entire System |
| Yang dipastikan | System  secara keseluruhan sudah memenuhi requirement yang diharapkan, secara scenario sudah sesauai, UI dan UX juga sudah sesuai dengan yang didesign |
| Metode pengujian | Black box |
| Dilakukan oleh | **QA Tester** |

#### 4 Acceptance Testing

|  |  |
| :--- | :--- |
| Yang di-test | Final system |
| Yang dipastikan | Memastikan product / aplikasi sudah sesuai dengan kebutuhan bisnis dan menjadi solusi untuk masalah yang akan dipecahkan |
| Metode pengujian | Black box |
| Dilakukan oleh | **End-user, Client, Stakeholders** |

