**Table of Contents**

- [Chapter 1: Getting Started](#Chapter_1_Getting_Started)
	- [An Origin Story](#An_Origin_Story)
		- [Blender Begins](#Blender_Begins)
		- [The Dark Nights](#The_Dark_Nights)
		- [Blender Rises](#Blender_Rises)
	- [About Blender](#About_Blender)
		- [About the Game Engine](#About_the_Game_Engine)
		- [Future of BGE](#Future_of_BGE)
	- [3D Basics](#3D_Basics)
		- [Coordinate System](#Coordinate_System)
		- [Points, Edges, Triangles, and Meshes](#Points,_Edges,_Triangles,_and_Meshes)
		- [Basic Transforms](#Basic_Transforms)
		- [Materials and Textures](#Materials_and_Textures)
		- [Lights](#Lights)
		- [Camera](#Camera)
		- [Animation](#Animation)
		- [Game](#Game)
	- [Setting up](#Setting_up)
		- [Installation](#Installation)
		- [System Requirements](#System_Requirements)
	- [Blender Basics](#Blender_Basics)
		- [Main Menu](#Main_Menu)
		- [3D Viewport](#3D_Viewport)
		- [Outliner](#Outliner)
		- [Properties Editor](#Properties_Editor)
		- [Timeline](#Timeline)
		- [Workspace Customization](#Workspace_Customization)
		- [More on the 3D View](#More_on_the_3D_View)
		- [Viewport Shading Modes](#Viewport_Shading_Modes)
		- [Editing Modes](#Editing_Modes)
		- [Keyboard and Mouse](#Keyboard_and_Mouse)
		- [Search](#Search)
		- [Blender Philosophy](#Blender_Philosophy)
		- [Interface](#Interface)
		- [Keyboard](#Keyboard)
		- [Mouse](#Mouse)
		- [Context](#Context)
		- [Datablocks](#Datablocks)
		- [Parenting and Grouping](#Parenting_and_Grouping)
		- [Backward Compatibility](#Backward_Compatibility)
	- [Onward](#Onward)
# Chapter 1: Getting Started

Ada satu hal yang anda tidak tahu tentang Mike (`salah satu penulis buku ini`). Dia memiliki buku Linux lebih banyak dari yang dia tahu. Sayangnya, Mike jarang membaca lebih dari bab 2. Hal tersebut karena dua bab pertama biasanya hanya ada perkenalan dan sejarah dari software yang dibahas. Ada dua konsekuensi dari gaya penulisan seperti ini. Pertama, Mike menceritakan sejarah Linux jauh lebih baik daripada orang lain. Kedua dia masih belum bisa bagaimana sebenarnya cara menggunakan Linux. Untungnya, konsekuensi pertama jauh lebih menguntungkan saat *party* dibanding mengetahui perbedaan "tar cvfz" dan "lshw".

Untuk menjaga tradisi, buku ini akan tetap ditulis menggunakan gaya yang sama. Di bab ini kita akan belajar sejarah Blender yang menarik disertai dengan pengenalan akan dasar-dasar cara penggunaan Blender. 

## An Origin Story

Waktu itu saat pertengahan 1990-an dan popularitas *personal computer* meroket lebih cepat dibandingkan prediksi. Bersamaan dengan meningkatnya popularitas *personal computer*, teknologi *animated graphics* dan *3D games* juga ikut meningkat pesat. 

### Blender Begins

Blender memulai sejarahnya sebagai software animasi 3D yang dibuat oleh sebuah perusahaan animasi kecil asal Belanda bernama NeoGeo. Mungkin karena belum adanya software animasi 3D yang murah dan mampu menjadi pengganti software yang sudah ada, atau mungkin juga karena ambisi NeoGeo yang ingin memiliki software animasi sendiri yang membuat mereka memutuskan untuk menelurkan Blender dari nol daripada menggunakan yang sudah ada. Programmer utama Blender saat itu adalah *Ton Roosendaal,* yang bertanggung jawab untuk menulis bagian utama fungsionalitas Blender.

Sampai beberapa tahun berikutnya, Blender hanya dipakai sebagai aplikasi internal sebuah perusahaan animasi yang amat sukses. Karena menjadi software yang sangat bagus, maka di tahun 1998 Blender mulai diperkenalkan ke publik. Sebuah perusahaan baru , Not a Number (NaN), dibuat untuk mengawasi perkembangan dan ditribusi Blender. Distribusinya dilakukan melalui dua versi yang berbeda: sebuah versi gratis dengan fungsi terbatas dan sebuah versi dengan fungsi utuh yang tidak gratis (bernama Blender Publisher). Dengan menjadi satu-satunya software animasi 3D yang lengkap dengan paket untuk membuat game yang tersedia gratis membuat popularitas Blender meningkat dan banyak komunitas online yang membantu artis membagikan pengetahuan dan hasil karyanya.

[![Left: Blender 1.6. Right: Blender 2.65](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-01.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-01.jpg)

### The Dark Nights

Sayang, bersamaan dengan terjadinya *Internet bubble* dan keadaan lain yang kurang menguntungkan, Not a Number (NaN) diumumkan bangkrut pada tahun 2002. Karena Blender merupakan hak kekayaan intelektual milik perusahaan tersebut mengakibatkan masa dengan yang suram bagi aplikasi animasi 3D ini. Melihat kondisi seperti ini, komunitas Blender tidak ingin aplikasi kesayangan mereka jatuh bersama dengan NaN. Oleh karena itu, sebuah kesepakatan dibuat dimana NaN akan merilis source code Blender ke publik dengan bayaran €100,000. Penggalangan dana bernama "Free the Blender" dimulai. Komunitas online merespon dengan baik hati. Beberapa bulan kemudian, uang yang berhasil dikumpulkan diberikan kepada NaN dan memindah tangankan software ini sebagai open source software ke Blender Foundation. Blender Foundation merupakan yayasan yang dibuat khusus untuk mengawasi perkembangan Blender dengan Ton Roosendaal sebagai ketuanya. 

### Blender Rises

Berlokasi di Amsterdam yang indah, Blender Foundation kini mengawal pengembangan, distribusi, dan pemasaran dari Blender. Namun, karena sifat *open source*-nya, pengembangan Blender sebagian besar dilakukan oleh kontributor sukarela dari seluruh dunia.

Blender Foundation juga membuat Blender Institute, sebuah studio animasi dan game yang fokus membuat film dan game menggunakan Blender. Blender Institute sudah memproduksi film berjudul *Elephants Dream, Big Buck Bunny, Sintel, Tears of Steel, Comos Laundromat* dan game *Yo, Frankie!* Proyek-proyek ini memiliki dua tujuan utama: proses produksi film dan game ini untuk menguji Blender di lingkungan studio yang nyata serta menunjukkan hasil kerjanya sebagai sarana pembukti kemampuan Blender itu sendiri (iklan).

[![Top: Elephants Dream, Big Buck Bunny, Yo, Frankie!, Bottom:  Sintel, Tears of Steel, Cosmos Laundromat](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-02.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-02.jpg)

Dirilislah Blender 2.5 yang banyak mengubah tampilan dan cara pakai Blender. Perubahan ini membutuhkan perencanaan dan pengembangan selama bertahun-tahun. Blender 2.5 menandai tonggak sejarah dari sejarah Blender. Bagi user yang datang dari seri 2.4x, antarmukanya terlihat sangat berbeda: menu item diatur ulang, shoftcut keyboard diganti, bahwa color scheme bawaan sudah berubah dari warna abu-abu yang *boring* menjadi warna abu yang tidak terlalu *boring*. Blender 2.5 didesain agar lebih intuitif, lebih cepat, dan juga lebih mudah untuk dipelajari dibanding pendahulunya. 

Blender menggunakan bahasa pemrograman Python untuk *scripting*-nya. Dengan Python kita bisa mengubah perilaku Blender, menambah fungsionalitasnya, serta yang paling penting, mengontrol game engine-nya. Mengetahui bagaimana membuat program bukan syarat untuk menggunakan Blender, tapi mengetahui cara menggunakan Python akan membuat kita menjadi game-maker yang lebih cakap.

[![Blender Commit statistics form 2003 to 2012](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-03.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-03.png)

Tentu saja, software ada untuk melayani pengguna - yaitu pembaca. Setiap kali seorang pengguna Blender membuat sebuah karya, karya ini membalas, meskipun sangat sedikit, waktu dan usaha untuk membuat software ini. Kami berharap dengan membaca buku ini, pembaca dapat membuat sesuai yang menarik untuk dibagikan dengan dunia.

------

## About Blender

Bisa jadi, pembaca sudah tahu bahwa Blender adalah software animasi 3D open source yang mampu melakukan modeling, animasi, rendering, compositing, dan producing sebuah game di satu package. Meskipun belum tahu apa maksud dari istilah-istilah tadi, jangan gentar!

Mari kita bahas istilah "software animasi 3D open source/open source 3D animation software". 

"Open source" artinya source code Blender tersedia bagi siapapun untuk membaca dan mengubahnya. Keuntungan yang paling kelihatan dari software open source adalah sebagai seorang artis, kita bisa menggunakan Blender tanpa biaya baik untuk non-komersil maupun komersil. Sebagai seorang developer, pembaca juga boleh memodifikasi Blender sesuai kebutuhan. Tapi, open source tidak berarti semua orang dapat melakukan perubahan ke kode-kode Blender tanpa persetujuan terlebih dahulu. Blender menggunakan lisensi GNU Public License v2 (GPL2). Singkatnya, hal ini berarti bahwa Blender dapat disalin, dimodifikasi, dan apabila dibagikan ulang, perubahan-perubahan pada source code harus dilisensikan dengan lisensi yang sama. 

> **Peringatan**:
>
> Sebelum mempublikasikan sebuah game menggunakan Blender, pembaca harus mengetahui batasan lisensi GPL. Topik ini dibahas di Bab 9, "Publishing and Beyond".

Istilah "3D" berarti tiga dimensi. Dunia yang kita tinggali adalah 3D karena memiliki tinggi, lebar, dan kedalaman. Dibandingkan dengan program 2D berikut, Photoshop, GIMP atau Krita, proses pembuatan konten di Blender dilakukan di ruang 3D bukan kanvas 2D.

[![2D vs. 3D](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-04.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-04.jpg)

Istilah "animasi" mungkin agak berbeda dengan yang pembaca tahu. Meskipun kita biasa menghubungkan istilah "animasi komputer" untuk setiap film yang dibuat dengan komputer, kita harus ingat bahwa Blender tidak terbatas hanya untuk membuat animasi. Blender juga dapat melakukan modeling, rendering, compositing, dan membuat game sebaik ia membuat animasi.

Istilah "software" menunjukkan bawah Blender adalah sebuah aplikasi komputer untuk membuat animasi dan game. Jadi buku ini akan membantu pembaca memahami setiap fitur Blender sehingga pembaca dapat memanfaatkannya untuk membuat apapun yang pembaca inginkan. 

Buku ini membahas Blender dari sisi aplikasinya bukan buku tentang desain game. Topik-topik seperti *storyline, art direction, * dan *game playability* diluar cakupan buku ini. Blender hanyalah sebuah alat yang membantu kita membuat sebuah karya seni. 

### About the Game Engine

Blender merupakan alat dengan banyak kegunaan. Buku ini akan membahas salah satu aspeknya saja: proses pembuatan game. Jika pembaca baru mengenal BLender, mempelajari game engine juga berarti pembaca akan ikut mempelajari dasar-dasar modeling, animasi, dan kemampuan lain seiring jalan. Jika sudah memiliki pengalaman menggunakan Blender, kemampuan yang pembaca miliki akan membuat transisi ke game engine menjadi lebih mudah. 

Dibandingkan game engine komersial yang tersedia saat ini, Blender Game Engine (BGE atau GE saja) relatif lebih sederhana. Apakah hal tersebut merupakan hal buruk? Tidak juga. Sistem sederhana seperti Blender sangat mudah untuk dipelajari tapi juga cukup fleksibel untuk melakukan banyak hal. 

Untuk memberikan gambaran apa kemampuan game engine ini, Bab 10, "Case Studies", ditulis untuk menunjukkan proyek yang dibuat dengan GE.

### Future of BGE

Satu kesulitan menulis tentang software adalah karena sifatnya yang akan terus berkembang. Bahkan hari ini, proyek seperti [UPBGE](https://upbge.org/) cukup menjanjinkan untuk meningkatkan fitur dan fungsionalitas Blender Game Engine.Kami akan mencoba membuat ebook ini se-*up-to-date* mungkin. Yang pembaca cukup lakukan ialah menggunakan versi terbaru dari Blender. 

> **Test Builds**
>
> Bila belum cukup puas dengan versi terbaru, pembaca bisa menemukan versi yang lebih baru lagi di  [builder.blender.org](https://builder.blender.org/download/). Sebagai tambahan, banyak test builds dari pihak ketiga yang tersedia juga di  [graphicall.org](http://graphicall.org/).

## 3D Basics

Jika pembaca belum pernah menggunakan aplikasi 3D sebelumnya, istilah modeling, animasi, dan rendering mungkin terdengar asing. Jadi sebelum mulai membuat game spektakuler yang selalu ingin pembaca buat, mari kita pelajari dulu dasar-dasar grafika komputer. Pembaca tidak perlu menyelami pembahasan di bawah ini jika sudah paham apa maksud RGB dan perbedaan antara Cartesian dan Gaussian.

Pengetahuan di bagian ini bersifat umum dan dapat diaplikasikan ke semua aplikasi 3D lainnya. Jadi meskipun pembaca datang dari aplikasi yang berbeda, konsep dasarnya tetap sama.

### Coordinate System

[![The three axes illustrated](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-05.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-05.png)

### Points, Edges, Triangles, and Meshes

Meskipun kita menentukan sebuah posisi di ruang menggunakan koordinat XYZ, satu titik (atau sebuah "vertex," istilah yang paling sering digunakan di grafika komputer) tidak lah begitu berguna karena satu titik terlalu kecil. Akan tetapi, kita bisa menggabungkan vertex ini dengan vertex lain untuk membuat sebuah garis (yang dikenal juga dengan istilah "edge"). Sebuah edge juga tidak begitu terlihat, sehingga kita membuat vertex baru kemudian menggabungkan ketiganya dengan baris lain lalu mengisi bagian tengahnya. Sekarang, ada sesuatu yang lebih menarik muncul, sebuah triangle (juga dikenal dengan istilah "face"). Dengan menghubungkan beberapa face kita dapat membuat bentuk lain yang menghasilkan bentuk dengan istilah "mesh" atau "model". Gambar di bawah menunjukkan bagaimana sebuah mes dapat dipecah menjadi face, lalu edges, dan terakhir, vertices. 

[![Teapot, cube, face, edge and vertex.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-06.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-06.jpg)

Mengapa triangle sangat penting? Ternyata, grafik komputer modern menggunakan triangle sebagai dasar untuk hampir semua jenis bentuk alias shape. Sebuah persegi panjang, (dikenal juga dengan istilah quadrangle atau quad) sebetulnya terdiri dari dua triangle. Sebuah kotak/kubus/dadu terdiri dari enam persegi yang saling terhubung. 

Di Blender, sebuah mesh dapat dibuat dengan kombinasi triangle, quad, atau n-gon. Keuntungan menggunakan n-gon adalah kemampuan untuk mengambil topologi yang rapi saat modeling. Tanpa n-gon, beberapa area dari sebuah model (seperti jendela atau dinding) akan membutuhkan lebih banyak triangle atau quad seperti pada gambar di bawah. Meski n-gon memudahkan proses modeling, Blender tetap mengubahnya menjadi triangle saat game dijalankan. 

[![The same cylinder cap can be made up of triangles, quads, or an n-gon.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-07.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-07.jpg)

Proses membuat sebuah mesh dengan menyusun vertice, edge, dan face disebut dengan modeling. Blender memiliki banyak tool untuk membantu kita membuat bentuk geometri yang diinginkan. 

Perlu dicatat bahwa tidak seperti di dunia nyata, model-model poligonal tidak memiliki volume. Mereka hanya kulit yang terdiri dari face yang saling terhubung dan membentuk suatu objek, tapi di dalamnya selalu kosong. 

[![Surface normals are displayed as cyan lines protruding from the faces.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-08.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-08.jpg)

Konsep lain yang mungkin akan ditemukan seorang modeler adalah "surface normal", atau "normal" saja. Normal adalah properti setiap face yang mengindikasikan arah yang dihadapi oleh sebuah poligon. Karena normal dipakai untuk melakukan shading computation dari sebuah permukaan/surface, idealnya semua normal untuk sebuah mesh harus bernilai "outward". Salah mengarahkan normal dapat membuat mesh menampilkan warna hitam atau tidak terlihat. Untungnya, ada fungsi Make Normals Consistent di Blender yang biasanya akan menyelesaikan permasalahan ini. Gambar 1.8 menunjukkan bagaimana normal ditampilkan di Blender.

> **Beyond Polygons**
>
> Secara teknis ada beberapa pendekatan untuk grafika komputer yang tidak bergantung pada triangle atau poligon seperti NURBS (Non-uniform rational B-spline) dan voxel (singkatan dari VOlumetric piXEL). Tapi polygon modeling dan rendering masih menjadih solusi yang paling umum dan menjadi satu-satunya metode yang didukung oleh game engine ini. 

### Basic Transforms

Ada tiga basic transform yang perlu diketahui yaitu:

- **Translation:** Menggeser sebuah objek ke arah manapun tanpa memutarnya.
- **Scaling:** Mengubah ukuran suatu objek dari satu titik.
- **Rotation:** Memutar sebuah objek dari satu titik.

Ketiganya merupakan manipulasi paling sering yang akan kita temui. Perhatikan ilustrasi di bawah.

[![Translation, scaling, and rotation.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-09.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-09.jpg)

### Materials and Textures

Menggunakan poligon, kita bisa mendefinisikan bentuk dari sebuah mesh. Untuk mengubah warna dan tapilannya, kita perlu menggaplikasikan material ke objek tersebut. Material mengontrol warna, terang, pantulan, bahkan transparansi sebuah objek. Variabel-variabel ini menambahkan detail ke objek tersebut. 

Seringkali, mengubah warna tidak cukup untuk membuat sebuah permukaan terlihat realistis. Disinilah dimana texture datang. Texturing merupakan teknik yang umum dipakai untuk menambah warna dan detail ke sebuah mes dengan membungkus mesh tersebut dengan sebuah gambar, seperti stiker. Bayangkan sebuah globe mainan, jika pembaca menyobek kertas yang membungkus globe tersebut secara hati-hati, maka akan terlihat bahwa kertas tersebut adalah sebuah texture dengan bolanya sebagai mesh. Proyeksi gambar 2D menjadi mesh 3D disebut dengan texture mapping. Texture mapping dapat dioperasikan secara otomatis menggunakan fungsi proyeksi yang sudah ada atu dilakukan secara manual yang menggunakan UV layout untuk memetakan gambar 2D ke mesh 3D. Gambar 1.10 mengilustrasikan bagaimana sebuah gambar dipetakan ke sebuah model. 

[![Meshes with texture applied.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-10.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-10.jpg)

Secara tradisional, sebuah texture akan mengubah warna sebuah permukaan. Tapi bukan hanya itu saja yang ia bisa lakukan, texture juga bisa mengubah properti lain dari sebuah permukaan misalnya transparansi, daya pantul, bahkan daya pantulnya untuk membuat ilusi sebuah permukaan yang lebih detail. 

[![From left to right: diffuse map, normal map, and specular map.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-11.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-11.jpg)

Sebuah diffuse map mengontrol warna dasar sebuah permukaan. Sebuah normal map mengontrol permukaan normal sebuah objek, membuat efek pantul dengan mengubah bagaimana sebuah cahaya direfleksikan dari objek tersebut. Sebuah specular map mengontrol refleksi specular dari sebuah objek, membuatnya terlihat terang ditempat tertentu dan redup ditempat lain. Sebuah texture map juga bisa memiliki pixel yang transparan, merender bagian tertentu dari objek menjadi transparan. 

Secara umum, texture adalah file gambar. Tapi ada juga cara lain untuk membentuk sebuah permukaan, misalnya dengan menggunakan procedural texture. Procedural texture berbeda dengan sebuah gambar karena ia dibuat oleh sebuah algoritma secara real time, bukan dari gambar yang sudah jadi. Blender game engine belum mendukung fitur procedural textures.

### Lights

Semua yang pembaca lihat merupakan hasil dari cahaya yang masuk ke dalam mata, tanpa cahaya, dunia akan kelam. Seperti itu pula pentingnya sebuah cahaya di dunia maya. Dengan adanya cahaya, maka akan ada pula sebuah bayangan. Bayangan mungkin bukan sesuatu yang penting untuk dipikirkan sehari-hari, tapi peran sebuah bayangan dan gambar membuat sebuah perbedaan yang amat besar untuk sebuah scene yang ditampilkan. 

Disebagian besar aplikasi 3D, ada beberapa jenis pencahayaan yang tersedia, setiap tipe memiliki keuntungan dan kekurangan. Contoh, sebuah Spot lamp meniru sebuah lampu dengan arah cahaya yang kerucut, sebuah sun lamp meniru sumber cahaya dari jarak yang jauh. Lamp di blender diperlakukan seperti objek biasa, mereka bisa diposisikan dan diputar seperti objek lain. Gambar 1.12 menunjukkan bagainana perbedaan lamp yang ada di Blender. 

[![From left: Lamp, Sun, Spot lamp, Hemi lamp, and Area lamp.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-12.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-12.png)

Anggap pencahayaan/lighting sebagai sesuatu yang membuat sebuah scene terlihat. Pencahayaan yang baik dapat menampilkan bagian yang penting dan menyembunyikan bagian yang tidak terlalu penting dengan bayangan sehingga terlihat lebih realitastis. 

### Camera

[![Camera objects](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-13.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-13.png)

Saat membuat tampilan 3D, kita melihat sebuah dunia virtual dari sudut pandang serba tahu. Dalam mode ini kita bisa melihat dan mengubah dunia 3D ini dari sudut manapun seperti seorang sutradara film berjalan keliling untuk mengatur sesuatu. Setelah game dimulai, pemain harus melihat game tersebut dari predetermined camera/sebuah kamera yang sudah ditentukan. Catat bahwa predetermined camera bukan berarti kamera tersebut sudah fixed alias tidak akan berubah-ubah. Hampir semua jenis game memiliki kamera yang bereaksi terhadap masukan pemain. Dalam game action, camera akan mengikuti gerakan karakter dari belakang, dalam game straetegi, kamera mungkin melihat dari atas, di game platformer, kamera biasanya mengikuti dari sisi samping. 

Kamera juga dianggap sebagai sebuah objek biasa oleh Blender sehingga kita bisa memanipulasi lokasi dan posisi seperti objek lain.

> **Drawing and Composition for Visual Storytellers**
>
> Berbicara tentang pencahayaan dan kamera, ada buku berjudul Framed Ink yang ditulis oleh Marcos Mateu-Mestre. Buku ini menggunakan banyak gambar untuk enjelaskan prinsip-prinsip visual storytelling.

### Animation

Dalam konteks buku ini, animation merujuk pada teknik yang membuat sesuatu berubah seiring dengan berjalannya waktu. Misal, animasi dapat terdiri dari menggeser objek, mengubah bentuknya, atau mengubah wanrnya. Untuk mengatur sebuah animasi, kita akan membuat "keyframe", yang merupakan snapshot disatu waktu yang menyimpan nilai tertentu yang berkaitan dengan animasi tadi. Software lalu dapat menambahkan sesuatu diantara nilai-nilai tadi untuk melakukan transisi yang halus. Gambar di bawha menujukan Dopesheet Editor milik Blender. Dopesheet memungkinkan kita untuk melihat beberapa properti yang berubah saat sebuah animasi terjadi, sumbu horisontal merepresentasikan waktu sedangkan sumbu vertikal menampilkan properti-properti, misal lokasi dan rotasi.

[![Dopesheet Editor: each diamond shape is a keyframe.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-14.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-14.png)

[![LocRotScale animation](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-15.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-15.png)

[![Armature animation](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-16.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-16.png)

[![Shape keys animation.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-17.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-17.jpg)

Cara ketiga untuk menganimasi ialah menggunakan shape keys. Shape keys adalah snapshot dari mesh di beberapa bentuk. Cara ini biasanay dipakai untuk menganimasikan perubahan yang tidak bisa dianimasikan dengan cara biasa. 



[![Procedural physics-based motion.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-18.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-18.jpg)

### Game

Sejauh ii, kita sudah cukup banyak membahas tentang 3D. Tapi bagaimana game engine memanfaatkan teori-teori tadi? Jadi, sebuah game engine sebetulnya hanya mengambil aset 3D yang sudah ada lalu memberikan "otak" ke objek tersebut sehingga mereka tahu bagaimana merespon suatu event. "Otak" ini dapat berubah logic bricks (melakukan akse berdasarkan input user), skrip (yang dapat menambah fungsionalitas logic bricks), atau properti fisik dari sebuah objek (misal memberikan pengaturan rigid body sehingga sebuah objek dapat jatuh secara realistis).

[![Game = Object + Logic.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-19.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-19.jpg)

Sebuah game engine terdiri dari beberapa komponen:

- **Rendering Engine** : Mengubah tampilan 3D yang sudah dibuat (termasuk models, lights, dan camera) menjadi gambar yang ditampilkan di layar.
- **Physics** : Menangani simulasi fisika seperti tabrakan dari objek-objek yang ada. 
- **Logic/Scripting** : Otak dibelakang sebuah game yang bereaksi pada masukan pengguna, menentukan arah, dan mengingat apa yang terjadi di dalam game. 
- **Sound** : Memproduksi event audio. 

Daftar di atas belum lengkap tapi dapat memberikan ide dasar apa yang dilakukan sebuah game engine. Blender game engine memberikan kita kontrol setiap komponen-komponen ini yang akan kita pelajari satu per satu. 

> **Quality vs. Performance**
>
> Membuat sebuah video game akan menyeimbangkan antara kualitas dan performa. Sebagai seorang desainer, kita ingin membuat dunia virtual yang kaya dan sedetail mungkin, disisi lain, kita juga harus memastikan game berjalan dengan halus bagi orang yang mungkin tidak memiliki komputer berspesifikasi tinggi. 
>
> Sepanjang proses pembuatan game, kita akan menemui kasus dimana kita harus mengambil keputusan untuk memprioritaskan kualitas visual atau performa game. Kita juga akan mempelajari trik untuk mencapai visual yang bagus tnapa mengorbankan performa juga bagaimana mengoptimalkan bagian game yang lambat. 

## Setting up

Akhirnya tiba waktu untuk menyelami dunia Blender! Mulai dari sini sampai ke bab terakhir, akan lebih baik jika pembaca berada didepan komputer. Penulis di bab ini penulis akan menujukkan bagaimana tampilan Blender sehingga pembaca dapat lebih mengeal aplikasi ini. 

### Installation

Blender berjalan di Windows, Mac OS X, dan Linux. Pembaca dapat mengunduh pemasang Blender untuk sistem operasi yang digunakan dari [www.blender.org](http://www.blender.org). Ukuran lengkap aplikasi Blender sekitar 100MB.

Silahkan unduh dan pasang Blender. Mulai aplikasi setelah terpasang

> **Installation Not Required**
>
> Secara teknis Blender tidak perlu dipasang sebelum digunakan. Berkas pemasang yang kita unduh dibuat untuk mempermudah kita saja. Blender dapat dijalankan dari tempat mana saja. Kita bahkan bisa menyalin foldernya ke USB sehingga bisa membuka Blender kapan pun dimana pun. Meskipun, secara default, Blender akan menyimpan beberapa pengaturan di direktori user. 

Meskipun kita membutuhkan Blender untuk membuat game, game yang kita buat dapat dipaketkan sebagai *stand alone application* sehingga orang lain tidak perlu memasang aplikasi tambahan apapun selain game tersebut. Lihat Bab 9, "Publishing and Beyond", untuk lebih detailnya.

### System Requirements

Blender tidak punya permintaan khusus akan spesifikasi komputer yang ia butuhkan. Performa aplikasi ini bergantung pada kompleksitas proyek. Jadi, semakin kencang komputer kita, semakin baik pula Blender akan bekerja.

## Blender Basics

Saat memulai Blender, kita akan disambut dengan sebuah *splash screen.* Buku ini akan mengasumsikan pembaca menggunakan pengaturan dan shortcut bawaan Blender.

Klik di mana saja untuk menutup *splash screen*, kita akan melihat tampilan *empty workspace* seperti ini:

[![Blender default workspace.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-20.jpg)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-20.jpg)

Jendel Blender dibagi menjadi Editor-Editor. Setiap bagian Editor dapat diubah ukurannya, dipindah, dan diganti untuk menampilkan konten tertentu. Untuk saat ini, mari kita biarkan seperti apa adanya.

#### Main Menu

Dibagian atas layar adalah  main menu yang memberikan fungsionalitas standar seperti Open, Save, dan Help. Selebihnya, main menu mengontrol tampilan dari jendela Blender yang lain. Opsi Render Engine ditengah menu mngontrol bagaimana antarmuka dikonfigurasi. 

[![Selecting the Game Engine](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-21.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-21.png)

#### 3D Viewport

Bagian yang paling banyak memakan tempat di layar adalah 3D Viewport. Disini kita bisa melihat dunia 3D yang kita buat dan saat menguji game. Untuk saat ini, silahkan eksplor 3D Viewport menggunakan middle mouse button (tombol yang ada di tengah mouse, biasanya ada di *scroll wheel*) dengan cara klik tahan dan geser (pengguna Mac dapat menggunakan two-finger rotate gesture di trackpad). Scene bawaannya memiliki tiga objek, sebuah cube (kubus), camera (kamera), dan light (pencahayaan). Untuk memilih salah satu objek, klik kanan. Objek yang terpilih akan memiliki tanda kuning. 

> **Basic Navigation Controls**

> Klik dan tahan middle mouse button untuk memutar 3D view. Scroll untuk melakukan zoom. Klik kanan  untuk memilih sebuah objek 3D. 

[![Number pad keyboard layout.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-23.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-23.png)

Untuk pindah view lebih cepat (side, top, front, dll.), numper pad dapat dipakai.

#### Outliner

[![Outliner](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-20b.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-20b.png)

Disebelah kanan layar ada dua Editor. Dibagian atas adalah Outliner, ia memiliki daftar seluruh data yang ada di file Blender saat ini. Untuk proyek besar, Outliner akan menjadi tool paling *mantep* untuk mengorganisir scene. Untuk saat ini, kita bisa mengabaikannya dulu.

#### Properties Editor

[![Properties Editor icons.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-24.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-24.png)

#### Timeline

Dibagian bawah layar adalah jendela timeline yang akan sangat berguna saat kita mulai membuat animasi. [![Timeline](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-20c.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-20c.png)

#### Workspace Customization

Tampilan layan bawaan seperti yang sudah dijelaskan sebelumnya, diatur untuk penggunaan secara umum. Ada waktu tertentu dimana perubahan layout menjadi penting untuk dilakukan. Untuk menggantinya, gunakan Screens layout drop-down menu dari main menu.

Selain layout yang sudah ditentukan, kita bisa memiliki layout sesuai keinginan. Kita bisa membagi satu editor untuk ditempati oleh dua editor bersamaan, dll. 

> **Editor, Region, and Area**
>
> Sebauh area di dalam jendela Blender disebut dengan Editor. Sebuah editor menampilkan konten dan tools spesifik. Misalnya: 3D View, Properties Editor, UV/Image Editor, dan Logic Brick Editor. 

Gambar 1.25 menampilkan sebuah area yang di bagi menjadi dua. Kita bisa men-*drag* bagian pojok kanan atas atau bawah.  

[![Area Splitting](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-25.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-25.png)



[![Editor selection.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-27.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-27.png)

[![Dopesheet, Image Editor, and Logic Brick Editor.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-28.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-28.png)

### More on the 3D View

3D View adalah tempat dimana kita akan menghabiskan sebagian besar waktu kita, jadi mari kita lihat dengan lebih detail. Kita sudah mempelajari beberapa cara untuk melakukan navigasi scene di bab ini, dengan menggunakan mouse dan keyboard. 

#### Viewport Shading Modes

[![Drawing Modes](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-29.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-29.png)

- **Bounding Box** : Merepresentasikan semua objek sebagai wireframe boundary. Berguna saat scene menjadi kompleks. 
- **Wireframe** : Menampilkan seluruh objek sebagai wirefram sehingga kita bisa melihat objek tembu pandang. 
- **Solid** : Menampilkan seluruh objek dengan permukaan yang solid, biasanya dipakai saat modeling
- **Textured** : Menampilkan seluruh objek dengan permukaan yang solid ditambah dengan texture dan lightning yang akurat. Biasanya dipakai untuk melakukan preview scene. 

Dua mode Shading yang paling sering dipakai adalah Wireframe dan Solid. Oleh karena itu, keduanya diberikan tombol keyboard untuk akses cepat. Tekan tombol Z untuk mengganti mode antara Wireframe dan Solid. Sebagai atmbahan, kita bisa menekan Alt+Z untuk mengaanti mode antara Solid dan Textured. 

> **Standing Out**
>
> Objek individu dapat menimpa model Viewport Sharing lewat pengaturan Properties Editor > Object > Display > Type. 

### Editing Modes

Disebelah kiri dari Shading mode selector adalah Editing Mode selector.

- **Object Mode** : Mode bawaan yang memungkinkan kita memanipulasi keseluruhan objek di scene. Dari mode ini kita bisa memilih objek apapun di scene, memindahkannya, memutarnya, juga mengubah ukurannya. Malah, hampir semua aksi selain modeling bisa dilakukan di Object mode. 
- **Edit Mode**: Mode ini dapat dilihat sebagai kebalikan dari Object mode. Mode ini memungkinkan kita untuk mengubah geometri dari sebuah objek. Saat melakukan modeling, pembaca mungkin akan memutuhkan Edit mode. Untuk alasan ini, Edit mode tidak tersedia saat objek yang tidak dapat di-edit terpilih (misalnya camera atau lamp).

Untuk berpindah antara Object mode dan Edit mode, tekan tombol tab. 

Sebagai tambahan untuk dua mode editing yang baru saja kita bahas, ada beberapa mode lain yang jarang dipakai. 

- **Sculpt Mode** : Hanya tersedia untuk objek Mesh. Memungkinkan modifikasi sebuah mesh seperti mengotak-atik tanah liat. 


- **Vertex** , **Weight,** dan **Texture Paint Mode** : Hanya tersedia untuk objek Mesh. Mode-mode ini memungkinkan penentuan warna atau obot ke mesh.
- **Pose Mode** : Dipakai untuk menganimasi bones disebuah armature.

Edit mode dan Object mode sejauh ini merupakan mode yang paling umum dipakai untuk melakukan editting, jadi kita akan menahan diri dari membahas mode lain terlalu dalam.

### Keyboard and Mouse

Ada *joke* di Blender yang mengatakan bahwa untuk memindahkan sebuah objek kita harus menekan tombol G yang berasal dari "movinG". *Joke* ini muncul karena penentuan *shortcut* yang agak berbeda dengan aplikasi lain. Namun, ada beberapa alasan mengapa "G" dipilih dibanding "M". Dalam kasus ini, G lebih cepat diakses oleh tangan kiri saat tangan kanan menggunakan mouse. Selain itu, G merupakan huruf dari kata Grab. 

> **Think Different**
>
> Keyboard Mac menggunakan Command bukannya Control. Jadi setiap kali pembaca melihat Ctrl+Sesuatu di buku ini, cukup gunakan Cmd. 
>
> Sebagai tambahan, Blender memiliki dukungan multi-touch gesture di OS X. Kita bisa melakukan pinch to zoom, rotate to orbit around, dan pan around. 

Mari kita mulai dengan *shortcut* yang penggunaannya sama dengan aplikasi-aplikasi lain:

- **Ctrl + S:** Save File
- **Ctrl + O:** Open File
- **Ctrl + N:** New File
- **Ctrl + Z:** Undo
- **Ctrl + Shift + Z:** Redo
- **Ctrl + Q:** Close(Quit) Application

Shortcut dapat bekerja di manapun didalam Blender, efeknya terjadi secara global. 

Untuk memanipulasi objek di 3D view, pada umumnya kita harus memilih salah satu objek dulu:

- **Right-click:** Memilih objek
- **Shift + Right-click:** Memperluas seleksi ke beberapa objek
- **A:** Pilih semua

Semua aksi di atas "reversible." Jadi jika sesuatu telah terpilih, saat di right-click lagi maka kita melepas pemilihan objek tersebut. Jika semua objek sudah dipilih, menekan tombol A lagi akan melepas pemilihan semua objek.

Setelah semua objek terpilih, kita bisa mulai memanipulasinya. Shortcut keyboard di bawah untuk melakukan tiga teknik transform paling dasar:

- **G:** Start Grabbing
- **S:** Start Scaling
- **R:** Start Rotating
- **Move mouse:** Carry out transform action
- **Left-click:** Confirm transformation
- **Enter:** Confirm transformation

Menekan salah satu tombol akan memuali transformasi, lalu kita bisa mulai menggeser mouse untuk mengontrol tingkat efek yang diberikan pada suatu objek. Untuk menyelesaikan proses transformasi, left-click atau tekan Enter.

### Search

[![The Search Box](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-30.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-30.png)

Tips terakhir yang akan kita pelajari adalah pencarian di Blender. Jika pembaca lupa untuk melakukan operasi tertentu baik itu melalui sebuah button atau shortcut keyboard, cara tercepat ialah dengan mencarinya menggunakan fungsi search di Blender. Tuliskan beberapa huruf untuk sesuatu yang kita cari maka hasilnya akan tampil seperti pada gambar 1.30.

Tekan sombol spasi dimana saja untuk menampilkan sebuah kotak pencarian ini. 

Implementasi pencarian saat ini belum begitu *context-aware*, jadi terkadang ada beberapa operasi yang tidak muncul di context yang aktif. 

### Blender Philosophy

Blender didesain dengan sebuah filosofi. Memahami filosofi Blender memungkinkan kita untuk menggunakannya sebagaimana dimaksudkan oleh pengembang sehingga kita bisa melakukan navigasi didalam Blender lebih cepat dan lebih efisien. 

### Interface

Karena Blender awalnya dibuat sebagai software in-house, antarmukanya dibuat untuk memaksimalkan kecepatan dan efisiensi untuk pengguna yang sudah menguasainya. Sejak Blender 2.5, banyak usaha telah dilakukan untuk membuat antarmuka Blender lebih *user-friendly*. Blender bisa jadi tidak seperti program-program lain yang sudah pernah pembaca pakai, termasuk software 3D lain. Untungnya, antarmuka Blender sangat konsisten. Ini artinya apabila pembaca sudah pernah mempelajari sesuatu sekali, pembaca bisa menggunakannya dibagian manapun di program ini. 

### Keyboard

Saking banyaknya perintah yang dapat dilakukan oleh Blender, memanggil fungsi tertentu melalui tombol keyboard pada umumnya lebih cepat dibanding menggunakan mouse untuk mencarinya. Saat mengikuti sisa isi buku ini, berikan perhatian pada tombol shortcut yang dipakai karena Blender didesain untuk bekerja lebih cepat setelah kita mempelajari shortcutnya. 

Shortcut Blender dioptimalisasi untuk keyboard QWERTY full-sized. Number pad (yang sayangnya tidak tersedia disebagian besar laptop) dipakai untuk melakukan navigasi cepat di 3D scene. Pengguna laptop biasanya harus menekan tombol tertentu di keyboard (seperti Fn atau toggle) untuk menggunakan number pad. Sebagai solusi, klik File > User Preferences (Ctrl + Alt + U), lalu masuk ke tab INput kemudian beri tanda centang pada "Emulate Numpad" untuk menggunakan tombol 1 sampai 0 tanpa menggunakan Numpad. Jika ingin menggunakan opsi ini secara permanen, klik tombol "Save User Settings". 

[![Emulate Numpad](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-30-1.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-30-1.png)

[![3D Navigator.](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-31.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-31.png)

### Mouse

Blender didesain untuk menggunakan mouse dengan tiga tombol atau sebuah mouse dengan dua tombol dan satu scroll wheel. Meskipun ada sebuah opsi untuk menyiasasi middle-mouse button (saat mengklik scroll wheel), buku ini akan mengasumsikan pembaca bekerja dengan sebuah mouse dengan tiga tombol untuk lebih memudah

> **How to Emulate a Thre-Button Mouse**
>
> Jika tidak punya mouse tiga tombol, gunakan Alt+Left mouse button untuk mengemulasi tombol tengah. Untuk mengaktifkan fitur ini klik File > User Preferences > Input dan beri tanda centang pada Emulate 3 Button Mouse.

### Context

Di Blender, aksi yang dapat dilakukan disatu waktu dibatasi oleh status Blender saat itu. Status ini dikenal dengan nama "context". Misalnya, operasi tertentu hanya bisa dipanggil jika sebuah objek sedang terseleksi; Properti editor akan berubah bergantung pada objek mana yang terseleksi; efek dari shortcut keyboard bahwa bisa berubah tergantung posisi mouse. Sifatnya yang sensitif akan context membuat kita fokus pada pekerjaan dengan opsi-opsi yang hanya bisa dipakai saat itu saja. Ini adalah cara Blender untuk menjaga antarmuka dari hal-hal yang tidak perlu. 

"Context" biasanya mengacu pada salah satu atau kombinasi dari daftar berikut:

- **Active rendering engine:** Blender Render, Blender Games, dan Cycles Render adalah tiga bawaan Blender.
- **Active editor:** Active editor ada bagian jendela Blender dimana kursor mouse sedang aktif. Shoftcut biasanya akan memiliki efek berbeda bergantung pada editor yang ada di bawah kursor mouse.
- **Active object:** Active object adalah objek yang sedang diseleksi.
- **Selected object:** Semua objek yang telah diseleksi. Perlu diingat bahwa kita bisa memilih lebih dari satu objek secara bersamaan, tapi hanya bisa ada satu objek yang aktif (active object). 
- **Editing mode:** Blender memiliki enam mode berbeda untuk editing. Dua diantaranya yang paling umum dipakai adalah Edit mode dan Object mode. Di Object mode, kita bisa memanipulasi objek sebagai satu kesatuan. Di Edit mode kita bisa mengubah bentuk mesh. Di setiap mode, ada beberapa kumpulan tools dan opsi yang bisa dipakai dan akan kita pelajari empat diantaranya (Sculpt, Vertex Paint, Texture Paint, Weight Paint). 

### Datablock

Seringkali, satu file Blender memiliki ratusan objek dengan warna, texture, dan animasi yang berbeda-beda. bagaimana semua objek ini diorganisir?

Blender menggunakan "data blocks" untuk merepresentasikan konten yang disimpan didalam sebuah file Blender. Setiap data block merepresentasikan sebuah koleksi data atau setting. Beberapa tipe datablock yang akan kita temui adalah Object datablock, Mesh datablock, Material datablock, Texture datablock, dan Image datablock. 

Dalam rangka mengurangi kompleksitas program, Blender mengorganisir data block ini dalam bentuk hirarki. Di level paling atas adalah scenes yang dapat memiliki beberapa world, setiap word ini bisa memiliki banyak objek (objek bisa berupa mesh, lamp, camera, dll.). Jika objek tersebut adalah mesh, maka Mesh datablock akan ditempelkan. Jika objek tersebut adalah lamp, maka Lamp datablock akan ditempelkan ke objek tersebut. 

Sebuah contoh hirarki datablock ini bisa dilihat di gambar 1.32: Scene > Object > Mesh > Material > Texture > Image



[![Datablock hierarchy](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-32.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-32.png)

Kita akan sering bertemu dengan datablock manager diantarmuka Blender. Mereka terlihat seperti pada gambar 1.33

[![Datablock Sharing](https://github.com/mikepan/GameEngineBook/raw/master/figures/Chapter1/Fig01-33.png)](https://github.com/mikepan/GameEngineBook/blob/master/figures/Chapter1/Fig01-33.png)

Karena datablock dapat dibagikan, disalin, dan digunakan ulang, scenes yang besar dapat diatur secara efisien dengan menggunakan shared datablocks. Gambar 1.33 menampilkan sebuah datablock yang dibagian oleh tiga "user", seperti yang ditampilkan oleh angka di sebelah namanya. 

### Parenting and Grouping

Grouping dan parenting memungkinkan kita untuk memberikan semacam urutan ke sebuah scene dengan mengaitkan satu objek dengan objek yang lain. Tapi grouping dan parenting bekerja dengan cara yang berbeda.

Parent dipakai untuk membuat sebuah tautan antara beberapa objek sehingga transformasi seperti lokasi, rotasi, dan penskalaan disebarkan dari parent ke children-nya. Dengan begini, setiap transformasi yang diberikan kepada parent secara otomatis akan diberikan pula kepada children. dengan menggunakan Parenting kita bisa menempelkan beberapa objek bersamaan sehingga seolah-olah mereka adalah satu objek.

Untuk melakukannya, pertama pilih sebuah objek yang ingin dijadikan child dulu. Jika lebih dari satu objek ingin dijadikan child, pilih semuanya sekaligus. Terakhir, pilih satu objek yang akan dijadikan parent (pilihan terakhir). Setelah itu tekan Ctrl+P untuk mengatur parent. 

Sebuah objek hanya bisa memiliki satu parent, tapi sebuah parent dapat memiliki banyak children. 

Grouping juga bisa dipakai untuk menautkan beberapa objek secara logika didalam sebuah scene tanpa ada pemaksaan transformasi. Tidak seperti parenting yang memiliki hubungan parent-child, grouping tidak memiliki hubung seperti itu, objek hanya sekedar member group saja. 

Pilih semua objek yang ingin dimasukkan ke dalam group yang sama lalu tekan Ctrl+G. Kita juga bisa mengatur keanggotaan group lewat Object Properties Editor.

Group bisa dipakai untuk membuat salinan beberapa objek sekaligus tanpa membuatnya satu persatu. Grouping juga bisa bermanfaat untuk melakukan manajemen aset yang mana akan kita diskusikan di bab berikutnya. 

Satu objek bisa memiliki beberapa group dan sebuah group bisa memiliki beberapa objek.

### Backward Compatibility

Blender didesain sehingga file-file lama masih bisa dibuka dengan versi Blender yang baru. Namun, karena banyaknya hal baru yang ditambahkan ke Blender, beberapa hal tak terduga mungkin dapat terjadi. 

Karena API Python Blender berubah di Blender 2.5, skrip yang ditulis untuk 2.4x tidak akan berjalan dengan baik di versi Blender yang baru. Tapi, saat membaca buku ini, seharusnya sudah cukup banyak konten baru yang bisa pembaca temukan. 

## Onward

Bagian ini menutup penjelasan dasar-dasar Blender dan game engine-nya. Sekarang, pembaca seharusnya sudah memiliki dasar-dasar pengetahuan fungsi dari sebuah game engine dan sudah akrab dengan antarmuka Blender. DI bab berikutnya kita akan mencoba membuat sebuah game sederhan dengan mengikuti tutorial ste-by-step.
