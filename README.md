Nama : Brian Jonathan
Kelas : PBP D

Tugas 2

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


4. Jelaskan mengapa kita menggunakan virtual environment? Apakah kita tetap dapat membuat aplikasi web berbasis Django tanpa menggunakan virtual environment?
Kita menggunakan virtual environment karena berguna untuk mengisolasi package serta dependencies dari aplikasi sehingga tidak bertabrakan dengan versi lain yang ada pada komputer. Hal ini akan memberikan dependencies yang berbeda-beda antara project satu dengan lainnya yang berjalan pada satu system operasi yang sama. Tanpa menggunakan virtual environment, kita tetap dapat membuat aplikasi web berbasis django, walau demikian hal ini tidak direkomendasikan. Terdapat beberapa masalah yang mungkin dihadapi, seperti :

    - konflik dependensi : Jika Anda menginstal paket-paket Python secara global di sistem Anda, proyek-proyek yang berbeda dapat bersaing untuk versi yang sama dari paket-paket ini, yang dapat menyebabkan konflik dan kesulitan dalam mengelola proyek-proyek tersebut.

    - Kesulitan dalam penyebaran proyek : Ketika Anda ingin membagikan proyek Anda atau mengerjakannya bersama dengan orang lain, menggunakan virtual environment membuatnya lebih mudah untuk memastikan bahwa semua orang bekerja dengan versi yang sama dari dependensi.

    - Keselamatan proyek: Jika Anda melakukan perubahan pada instalasi Python sistem Anda tanpa sadar, Anda dapat merusak proyek-proyek yang ada. Dengan virtual environment, Anda dapat mengisolasi proyek-proyek tersebut dari instalasi Python sistem.

5. Jelaskan apakah itu MVC, MVT, MVVM dan perbedaan dari ketiganya.
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


Jawaban Tugas 3 (Implementasi Form dan Data Delivery pada Django) :
Apa perbedaan antara form POST dan form GET dalam Django?
    POST mengirimkan data formulir ke server dalam badan permintaan HTTP, sedangkan GET mengirim data formulir sebagai parameter yang ditambahkan ke URL. Hal ini membuat POST lebih aman untuk pengiriman data yang bersifat sensitif atau tidak semua orang boleh melihatnya, seperti password. GET lebih cocok untuk permintaan yang tidak sensitif, seperti pencarian atau tampilan data yang tidak mengubah status server.
    POST tidak memiliki batasan ukuran data sedangkan GET memiliki batasan ukuran URL di browser dan server sehingga terbatas dalam jumlah dan ukuran data yang dapat dikirim.    

Apa perbedaan utama antara XML, JSON, dan HTML dalam konteks pengiriman data?
    Salah atu perbedaan utama antara XML, JSON, dan HTML adalah Struktur XML menggunakan tag kustom yang didefinisikan oleh pengguna untuk menggambarkan data. Struktur JSON menggunakan key-value pair dimana data dapat berupa objek atau array. Struktur HTML memiliki elemen bawaan yang telah didefinisikan, seperti <p> untuk paragraf dan <a> untuk tautan.

Mengapa JSON sering digunakan dalam pertukaran data antara aplikasi web modern?
    JSON sering digunakan dalam pertukaran data antara aplikasi web modern karena JSON merupakan format pertukaran data yang sangat ringat dan lebih mucah dibaca dan ditulis oleh manusia, sehingga gampang untuk diterjemahkan dan dibuat oleh komputer. Beberapa kelebihan dari JSON juga adalah dapat menyimpan data dalam bentuk array dan menjadikan transfer data menjadi lebih mudah dan lebih cepat dalam parsing data  di sisi server.

Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).
    Checklist diatas dilengkapi dengan pertama-tama membuat form input yang nantinya akan menampilkan 3 hal, name, amount, dan description. Setelah itu untuk checklist kedua, ditambahkan 5 function baru untuk HTML, XML, JSON, XML by ID, dan JSON by ID. Untuk checklist ketiga hanya melanjutkan dengan routing URL di masing-masing views dengan penambahan path di urls.py.

Referensi :
- https://chat.openai.com/share/b53d1de1-e69f-40a1-a560-74e17477e31f
- https://www.dicoding.com/blog/apa-itu-json/
- https://chat.openai.com/share/679dede9-e0fb-4cf2-b70f-29697b1e5bf9
- https://media.neliti.com/media/publications/267827-penerapan-data-json-untuk-mendukung-peng-b1a9128a.pdf
- Tutorial 3

Berikut adalah tautan Screenshot terkait penggunaan Postman untuk melihat objek yang sudah ditambahkan dalam format HTML, XML, JSON, XML by ID, dan JSON by ID:

HTML :
![messageImage_1695175982125](https://github.com/brianjo25/sneakers_hub/assets/126589196/90224c34-471e-4d0f-8914-cff4f7d45b9f)
![messageImage_1695176004152](https://github.com/brianjo25/sneakers_hub/assets/126589196/d8798382-ffe8-4cca-b1f7-96ea01263d62)
![messageImage_1695176025953](https://github.com/brianjo25/sneakers_hub/assets/126589196/a3748d08-d964-41e7-8943-c596ce203fac)


XML :
![messageImage_1695151054815](https://github.com/brianjo25/sneakers_hub/assets/126589196/022d392d-4bde-4f22-a82a-ddcf1eadb5bb)

JSON :
![messageImage_1695151100144](https://github.com/brianjo25/sneakers_hub/assets/126589196/f78085e7-4d98-4efd-81e6-d821c706349b)

XML by ID :
![messageImage_1695151191994](https://github.com/brianjo25/sneakers_hub/assets/126589196/989d2c7f-5f27-4aff-98f0-b00029ff44cb)

JSON by ID :
![messageImage_1695151220373](https://github.com/brianjo25/sneakers_hub/assets/126589196/eaa09e54-91ba-492f-8f7a-524d526591fa)



Jawaban Tugas 4 (Implementasi Autentikasi, Session, dan Cookies pada Django):

1. Apa itu Django UserCreationForm, dan jelaskan apa kelebihan dan kekurangannya?
Django UsercreationForm merupakan formulir bawaan dari framework django yang digunakan untuk memudahkan membuat dan mendaftarkan sebuah user baru. Hal ini akan mengumpulkan username, password, dan konfirmasi password.

Kelebihan :
- Mudah untuk digunakan : Penggunaan UserCreationForm tidak ribet atau berbelit-belit sehingga mudah untuk digunakan.

- Bisa di custom : Penggunaan UserCreationForm bisa di customize sesuai dengan keperluan, bisa ditambahkan bidang, seperti menambahkan input email dan sebagainya.

- Auto Validation : UserCreationForm dilengkapi dengan auto validation yang akan memastikan password yang diinput sesuai dengan konfirmasi password.

Kekurangan:
- Tidak support opsi autentikasi alternatif : Jika ingin menambahkan opsi autentikasi seperti misalnya menggunakan google atau facebook, harus menabahkan sendiri. UserCreationForm hanya bisa melakukan pendaftaran secara konvensional, dengan username dan password.

- Preview default yang sangat sederhana : Tampilan yang sederhana ini tidak pasti cocok dengan semua orang. Jika seseorang menginginkan preview/ta,pilan yang lebih menarik atau kompleks, tampilan khusus harus dirancang lagi.


2. Apa perbedaan antara autentikasi dan otorisasi dalam konteks Django, dan mengapa keduanya penting?
Autentikasi adalah proses verifikasi identitas pengguna yang berguna untuk melakukan verifikasi ata pengguna dalam memberikan izin kepada sistem untuk melanjutkan, sedangkan otorisasi adalah penentuan hak akses pengguna terkait siapa saja yang bisa mengakses suatu hal. Simplenya, autentikasi memverifikasi usernya sedangkan otorisasi validasi dilakukan kepada akses user terhadap hal-hal yang ada di web/ aplikasi tersebut. 

Hal ini penting untuk mendukung sisi keamanan. Autentikasi memastikan hanya user yang valid/sah yang bisa mengakses ke aplikasi/web, sedangkan ototrisasi membatasi apa saja yang bisa diakses. Selain itu, Autentikasi dan (terkhususnya) otorisasi membantu menjaga privasi data user. Tanpa adanya autentikasi dan otorisasi, pembobolan dan pencurian data besar-besaran bisa dengan sangat mudah terjadi. 

3. Apa itu cookies dalam konteks aplikasi web, dan bagaimana Django menggunakan cookies untuk mengelola data sesi pengguna?
Cookies adalah file berukuran kecil yang diletakkan pada komputer user saat mengunjungi sebuah website. Cookies berguna untuk mengetahui aktivitas yang dilakukan user. 

Django menggunakan cookies dengan cara membuat cookie session yang berisi data user yang mencangkup ID Session unik untuk mengidentifikasi sesi itu. Ketika server menerima request dari browser dengan cookie session, server akan mengambil data sesi yang sesuai berdasarkan ID yang ada. Data sesi ini dapat digunakan untuk mengidentifikasi user, mengambil preferensi dari user, ataupun melakukan tindakan yang berdasarkan dengan data sesi. Server juga bisa mengubah data sesi selama sesi berlangsung, sepertii saat user log in maka server menyimpan informasi identifikasi user dalam sesi tersebut, jika user log out maka informasi itu akan dihapus oleh server. 

4. Apakah penggunaan cookies aman secara default dalam pengembangan web, atau apakah ada risiko potensial yang harus diwaspadai?
Terdapat beberapa resiko potensial yang tentunya harus diwaspadai, beberapa diantaranya adalah :
- Resiko Keamanan : Jika tidak digunakan secara benar, soockie dapat menimbulan resiko keamanan. Informasi sensitif pada cookie rentan terhadap akses tidak sah. Cookies juga bisa menjadi vektor untuk sereangan cross-site scripting (XSS) dan cross-site request forgery (CSRF), dimana hal itu bisa terjadi pada browser dengan mengeksploitasi kelemahan kode situs web.

- Masalah Kompabilitas : Beberapa browser memiliki cara yang berbeda dalam menangani cookie, atau bahkan beberapa user memilih untuk menonaktifkannya. Hal ini dapat menyebabkan user experience yang tidak konsisten dan merusak fitur yang mengandalkan cookie. Developer harus mempertimbahkan Cookie Support saat merancang dan membangun aplikasi web dan memastikan adanya mekanisme alternatif jika diperlukan.

5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).

Pertama-tama diawali dengan menambahkan fungsi dan form registrasi dimana terdapat UserCreationForm yang digunakan untuk memudahkan pembuatan formulir pendaftaran user pada web. Tidak terlupa juga untuk membuat register.html untuk pendaftarannya.

Kedua, setelah adanya registrasi, kita buat fungsi login yang berfungsi untuk autentikasi akun yang sudah diregistrasi tadi. Lengkapi juga dengan membuat login.html untuk fitur login ini.

Ketiga, sebuah fungsi log in tentunya juga harus dilengkapi dengan fungsi log out. Fungsi log out dibuat ditambahkan juga pada main.html untuk tombol log outnya.

Keempat, membuat restriction pada halaman awal. Hal ini mewajibkan setiap orang yang akan menggunakan web kita untuk melakukan log in terselbih dahulu.

Kelima, kita akan menggunakan data dari cookies. Hal ini dilakukan dengan menambahkan last_login setelah user log in. Pada web akan dapat dilihat sesi terakhir log in.

Keenam, kita menghubungkan Model Product dengan user. Hal ini berguna untuk menghubungkan product yang dibuat oleh sebuah user sehingga user tersebut yang terotorisasi hanya melihat produk-produk yang terlah dibuatnya sendiri.

Terakhir, saya menambahkan fitur-fitur bonus, yakni tombol tambah dan kurang, serta tombol delete untuk menghapus item pada website

![image](https://github.com/brianjo25/sneakers_hub/assets/126589196/34f70d6b-9644-4f15-b709-7ff5744fcada)
![image](https://github.com/brianjo25/sneakers_hub/assets/126589196/e1a02387-e963-40e4-b70e-66cea2ec2173)


Referensi :
- https://diginews.id/apa-perbedaan-antara-otentikasi-dan-otorisasi/
- https://glints.com/id/lowongan/cookies-adalah/
- https://appmaster.io/id/blog/peran-cookie-dalam-pengembangan-web

Jawaban Tugas 5 : Desain Web menggunakan HTML, CSS dan Framework CSS

1. Jelaskan manfaat dari setiap element selector dan kapan waktu yang tepat untuk menggunakannya.

Element Selector digunakan untuk mengatur gaya pada semua elemen dengan jenis tertentu. Berguna ketika ingin mengatur gaya dasar atau gaya global untuk semua elemen dengan jenis yang sama di seluruh web.

ID Selector digunakan untuk mengidentifikasi elemen secara unik dalam halaman HTML dan menerapkan gaya ke elemen tersebut. Digunakan ketika ingin mengatur gaya atau perilaku khusus untuk elemen tunggal dalam halaman dimana ID harus unik dalam satu halaman tesrebut.

Class Selector digunakan untuk mengidentifikasi satu atau lebih elemen dengan kelas yang sama dan menerapkan gaya atau perilaku yang sama pada mereka. Digunakan ketika ingin mengatur gaya atau perilaku yang sama untuk beberapa elemen dengan karakteristik yang serupa (kelas yang sama)

2. Jelaskan HTML5 Tag yang kamu ketahui.
Terdapat banyak sekali Tag HTML5, beberapa yang saya tau adalah:
- <audio> : Berfungsi untuk menanamkan audio pada halaman web
- <video> : Bergungsi untuk menanamkan video pada halaman web
- <header> : Merepresentasikan/mendefinisikan bagian header (atas) dari sebuah halaman atau elemen
- <footer> : Merepresentasikan/mendefinisikan bagian footer (bawah) dari sebuah halaman atau elemen
- <aside> : Merepresentasikan/mendefinisikan konten yang berhubungan dengan konten utama dan dapat dianggap sebagai "sidebar"
- <canvas> : Berfungsi untuk menggambarkan grafis dan animasi (biasa menggunakan JavaScript)
-<svg>: Menanamkan Scalable Vector Graphic dalam halaman web
 
3. Jelaskan perbedaan antara margin dan padding.
Margin berada di luar dua elemen yang berdekatan sedangkan padding ditempatkan di dalam batas elemen. Ibaratkan ada 2 buah kotak yang memiliki teks sebagai konten di dalamnya, jika ingin memberikan jarak antara teks dengan kotak, itu adalah padding. Jika ingin memberikan jarak antara kedua kotak sehingga tidak ada yang berdempetan, itulah Margin.

4. Jelaskan perbedaan antara framework CSS Tailwind dan Bootstrap. Kapan sebaiknya kita menggunakan Bootstrap daripada Tailwind, dan sebaliknya?
Berikut merupakan beberapa perbedaan antara Tailwind dan Bootstrap:

- Tailwind CSS membangun tampilan dengan menggabungkan kelas utilitas yang telah didefinisikan. Bootstrap menggunakan gaya dan komponen yang telah didefinisikan yang memiliki tampilan yang sudah jadi dan dapat digunakan secara langsung.

- Tailwind memberkan fleksibilitas yang lebih besar dengan pendekatan "utility-first" yang memungkinkan kita membangun desain yang sangat kustom. Bootstrap menawarkan kerangka kerja yang relatif terstruktur dengan banyak komponen yang telah dirancang sebelumnya.

- Tailwind dirancang untuk lebih ringan dalam hal ukuran file, tapi saat menggunakan banyak class utilitas dalam kode, ukuran file CSS dapat meningkat. Bootstrap memiliki ukuran file yang lebih besar karena menyediakan banyak fitur dan komponen siap pakai.

Kita sebaiknya menggunakan Bootstrap dari pada tailwind saat :
- Proyek dengan batas waktu singkat : Komponen siap pakai dari bootstrap membantu untuk melakukan pengerjaan yang lebih cepat.

- Pengembangan proyek besar : Bootstrap memiliki komponen dan utilitas untuk membantu pengembangan proyek besar menjadi lebih efisien.

- Dokumentasi yang diperlukan : Bootstrap memiliki sumber daya yang melimpah sehingga dokumentasi merupakan hal yang mudah.

Kita sebaiknya menggunakan Tailwind dari pada Bootstrap saat :
- Proyek yang memerlukan desain kustom : Tailwind CSS memberikan fleksibilitas untuk membuat tampilan seunik mungkin

- Proyek yang memerlukan kinerja yang lebih baik : tailwind CSS biasa lebih ringan karena kalian hanya menggunakan apa yang dibutuhkan saja sedangkan yang tidak dibutuhkan tidak perlu ada di sana.

- Proyek yang memerlukan pengkodean yang dibaca dengan baik : Tailwind CSS memiliki kelas-kelas yang deskriptif yang membuatnya lebih mudah untuk dibaca. Hal ini akan membantu jika adanya kolaborasi antar pengembang sehingga tidak tejadi kesulitan dalam pembacaan kode. 

5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).

Pertama-tama, saya mempelajari terlebih dahulu dokumentasi dan materi yang ada pada tutorial. Hal tersebut sangat membantu saya untuk memahami apa yang saya kerjakan. Setelah itu, saya memulai dengan memasukan Bootstrap CSS dan JS. 
Kode CSS : 
    <head>
        {% block meta %}
            ...
        {% endblock meta %}
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
</head>

Kode JS:
<head>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha384-KyZXEAg3QhqLMpG8r+J4jsl5c9zdLKaUk5Ae5f5b1bw6AUn5f5v8FZJoMxm6f5cH1" crossorigin="anonymous"></script>
</head>
    
Setelah itu, saya menambahkan juga Navbar atau Navigation bar untuk memperindah tampilan web sekaligus membuatnya bisa lebih multifungsi. Saya menambahkan kode pada edit_product dan membuat file html baru dengan nama edit_product.html. Setelah itu saya menambahkan pada urls.py untuk mengimport fungsi edit_product dan juga menambahkan path url ke urlpatterns. Saya juga menambahkan potongan kode berikut :

...
<tr>
    ...
    <td>
        <a href="{% url 'main:edit_product' product.pk %}">
            <button>
                Edit
            </button>
        </a>
    </td>
</tr>
...

Setelah itu, saya membuat fungsi untuk menghapus data produk. Diawali dengan membuat fungsi baru bernama delete_product, menyambungkannya ke urls.py dan menambahkan path url ke dalam urlpatterns. Setelah itu juga ada perubahan di main.html dengan kode betikut :

...
<tr>
    ...
    <td>
        <a href="{% url 'main:edit_product' product.pk %}">
            <button>
                Edit
            </button>
        </a>
        <a href="{% url 'main:delete_product' product.pk %}">
              <button>
                  Delete
              </button>
          </a>
    </td>
</tr>
...

Setelah ini semua, saya beralih ke card. Setelah membuat card, saya mengubah tampilan-tampilan seperti warna web, warna button, dan banyak lainnya untuk menyesuaikan dan memperindah web.

Referensi :
https://www.tutorialrepublic.com/html-reference/html5-tags.php
https://kotakode.com/pertanyaan/6133/Apa-perbedaan-margin-dan-padding%3F
