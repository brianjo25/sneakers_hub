Nama : Brian Jonathan
Kelas : PBP D

Tautan menuju aplikasi adaptable : https://sneakershub.adaptable.app

1. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).
Untuk mengimplementasikan checklist pada soal secara step-by-step, saya menggunakan bantuan tahapan dari tutorial sebagai bantuan utama saya. Pada tutorial 1 dan 2, sudah dijelaskan dengan sangat baik tentang cara pengerjaan tugas 2 ini. Walau demikian, saya tidak hanya bergantung pada tutorial. Pengetahuan dan ide yang saya miliki juga saya tuangkan kepada pengerjaan ini, seperti contohnya membuat Sneakers Hub, website inventori sepatu.

2. Buatlah bagan yang berisi request client ke web aplikasi berbasis Django beserta responnya dan jelaskan pada bagan tersebut kaitan antara urls.py, views.py, models.py, dan berkas html.

                     HTTPS Request ------urls.py
                                            |                        
                                            |
                                            |
    Models.py ---- read/write data ------- View.py ----------- HTTP Response
                                            |                    (HTML)
                                            |
                                            |
                                    Templates html


    1. url.py : request dari client akan mencapai django melalui URL. URL ini akan mencocokan permintaan dengan pola URL yang sesua idengan memutuskan nama ciew mana yang akan menangani permintaan tersebut.

    2. views.py : Setelah URl menentukan view yang akan menangani permintaan, view tersebut akan dipanggil. View tersebut berisi logika aplikasi yang dapat melakukan hal seperti memproses data dan lainnya.

    3. models.py : Mendefinisikan struktur data yang akan digunakan dalam aplikasi.

    4. Templates : Digunakan untuk menghasilkan tampilan yang akan ditampilkan kepada users. Biasa berisikan markup HTML serta placeholder untuk data yang diberikan oleh view.

    5. Response : Setelah data masuk ke dalam template, view akan mengirimkan response dalam bentuk HTML ke users. Users menerima response.


3. Jelaskan mengapa kita menggunakan virtual environment? Apakah kita tetap dapat membuat aplikasi web berbasis Django tanpa menggunakan virtual environment?
Kita menggunakan virtual environment karena berguna untuk mengisolasi package serta dependencies dari aplikasi sehingga tidak bertabrakan dengan versi lain yang ada pada komputer. Hal ini akan memberikan dependencies yang berbeda-beda antara project satu dengan lainnya yang berjalan pada satu system operasi yang sama. Tanpa menggunakan virtual environment, kita tetap dapat membuat aplikasi web berbasis django, walau demikian hal ini tidak direkomendasikan. Terdapat beberapa masalah yang mungkin dihadapi, seperti :

    - konflik dependensi : Jika Anda menginstal paket-paket Python secara global di sistem Anda, proyek-proyek yang berbeda dapat bersaing untuk versi yang sama dari paket-paket ini, yang dapat menyebabkan konflik dan kesulitan dalam mengelola proyek-proyek tersebut.

    - Kesulitan dalam penyebaran proyek : Ketika Anda ingin membagikan proyek Anda atau mengerjakannya bersama dengan orang lain, menggunakan virtual environment membuatnya lebih mudah untuk memastikan bahwa semua orang bekerja dengan versi yang sama dari dependensi.

    - Keselamatan proyek: Jika Anda melakukan perubahan pada instalasi Python sistem Anda tanpa sadar, Anda dapat merusak proyek-proyek yang ada. Dengan virtual environment, Anda dapat mengisolasi proyek-proyek tersebut dari instalasi Python sistem.

4. Jelaskan apakah itu MVC, MVT, MVVM dan perbedaan dari ketiganya.
    - MVC : Model View Controller adalah suatu model yang digunakan oleh para software developer yang berisikan komponen model, view, dan controller. 
        - Model merupakan komponen yang berisi logika bisnis dan status data yang terdapat di dalam aplikasi. Model bertugas untuk mendapatkan dan memanipulasi data, berkomunikasi dengan controller, berinteraksi dengan data base, dan terkadang juga refresh tampilan dari aplikasi yang dikembangkan.
    
        - View merupakan komponen yang berhubungan dengan HTML/CSS.XML (interface) dan menyajikan data yang sesuai. View berkomunikasi dengan pengontrol dan berinteraksi dengan model. komponen ini juga bekerja sama dengan controller untuk menciptakan tampilan yang dinamis (bergerak). 

        - Controller merupakan suatu fragmen yang berfungsi sebagai komunikator antara view dan model. Controller membutuhkan input user dari view/REST. Lalu permintaan "Get Data" diprosesd ari model dan diteruskan ke view untuk ditampiilkan.

    - MVT : Model View Template adalah sebuah konsep arsitektur dalam web development untuk memisahkan komponen utama sebuah aplikasi dan membantu developer mengorganisasi dan mengelola kode dengan lebih terstruktur.

        - Model merupakan komponen yang bertanggung jawab untuk mengatur dan mengelola data dari aplikasi. Model menghubungkan aplikasi dengan basis data dan mengatur interaksi dengan data tersebut.

        - View merupakan komponen yang menangani logika presentasi dan menangani bagaimana data yang dikelola oleh model untuk ditampilkan kepada pengguna.

        - Template merupakan komponen yang mengatur interface, memisahkan kode HTML dari logika aplikasi, dan digunakan untuk merancang tampilan yang akhirnya akan diisi dengan data dari model melalui view.

    - MVVM : Model View ViewModel merupakan pola arsitektural yang memisahkan pengembangan UI dari logika bisnis dan perilaku dalam aplikasi.
        - Model merupakan komponen yang terdiri dari data dasar yang digunakan untuk menjalankan software.

        - View merupakan komponen yang digunakan sebagai antarmuka grafis antara user dan pola desain, serta menampilkan output dari data yang telah diproses.

        - ViewModel merupakan abstraksi dari view dan penyedia pembungkus data model untuk ditautkan. ViewModel terdiri dari Model yang diubah menjadi View, dan berisi perintah yang dapat digunakan oleh View untuk mempengaruhi Model.

    Perbedaan antara ketiganya terdapat pada komponennya, bagaimana cara mereka mengorganisasi komponen aplikasi, dan cara mererka memisahkan logika aplikasi dan tampilan. MVC memiliki controller yang memegang peran utama dalam mengendalikan alur aplikasi, MVT memiliki view yang memiliki peran serupa dengan Controller tetapi memiliki template untuk tampilan, sedangkan MVVM memisahkan logika tampilan ke dalam ViewModel dan membuat View lebih pasif.

Referensi :
- Tutorial 0 & Tutorial 1 PBP
- https://dev.notnoob.com/python/tutorial-virtual-environment/#:~:text=Virtual%20Environment%20sangat%20berguna%20ketika,digunakan%20untuk%20project%20berbasis%20Python.
- https://chat.openai.com/share/437eba17-1b53-4a41-aecc-06e5d473c175
- https://agus-hermanto.com/blog/detail/mvc-vs-mvp-vs-mvvm-apa-perbedaannya-mana-yang-terbaik-diantara-ketiganya-a
- https://chat.openai.com/share/ab3a8b46-16d9-4810-b827-8b05ba442f9c
- https://chat.openai.com/share/5cf78bd9-144b-44e8-9603-f31b65568478