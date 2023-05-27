## Pengenalan ke Amazon Elastic Compute Cloud (Amazon EC2)
kamu akan membutuhkan server yang dapat memberikan kapasitas komputasi untuk menjalankan aplikasi dan menyediakan daya komputasi sesuai kebutuhan bisnis Anda. Di AWS, server tersebut berbentuk virtual. Dan layanan yang dapat Anda gunakan untuk mendapatkan akses ke server virtual tersebut disebut dengan Amazon EC2. 
Dengan menggunakan layanan EC2, Anda memiliki kapasitas komputasi yang fleksibel, hemat biaya, dan cepat dibandingkan dengan menjalankan server sendiri di data center on-premise. Amazon EC2 memberikan kapasitas komputasi yang aman dan dapat Anda ubah-ubah ukurannya di cloud. AWS sudah menangani bagian-bagian yang sulit untuk kamu. AWS telah membangun dan mengamankan data center, membeli, menyusun, dan memasang server sehingga siap untuk kamu gunakan.

AWS terus mengoperasikan kapasitas komputasi dalam jumlah besar sehingga kamu dapat menggunakannya kapan pun dan berapa pun sesuai dengan porsi kapasitas yang Anda butuhkan. Anda hanya perlu membuat permintaan untuk EC2 instance sesuai keinginan dan saat itu juga mereka pun siap dalam hitungan menit. Di AWS, server virtual disebut sebagai instance.

jika kamu telah selesai menggunakannya, Anda dapat menghentikan atau mengakhiri instance tersebut dengan mudah. Anda tidak perlu lagi khawatir akan terjebak dengan server yang tidak digunakan. Anda hanya harus membayar sesuai dengan apa yang Anda gunakan saja (pay for what you use), bukannya saat instance berhenti atau berakhir.

Amazon EC2 berjalan di atas host (mesin fisik) yang dikelola oleh AWS menggunakan teknologi virtualisasi. Saat menjalankan instance, kamu tidak perlu menggunakan keseluruhan mesin host untuk sendiri melainkan Anda akan berbagi mesin host dengan beberapa instance lainnya. Ini dikenal dengan nama virtual machines alias mesin virtual.

Hypervisor-lah yang bertanggung jawab untuk membagi sumber daya fisik yang mendasarinya di antara mesin virtual tersebut. Ini sepenuhnya dikelola oleh AWS. Ide berbagi perangkat keras yang mendasarinya ini disebut multitenancy. Hypervisor juga bertanggung jawab untuk mengisolasi mesin virtual satu sama lain saat mereka berbagi sumber daya dari host. Ini berarti EC2 instance tetap aman meskipun mereka berbagi sumber daya. Satu instance tidak akan mengetahui keberadaan instance lainnya walau mereka ada di host yang sama. Mereka tetap aman dan terpisah satu sama lain.

Amazon EC2 memberikan Anda banyak fleksibilitas dan kontrol. Tak hanya dapat menjalankan server baru atau menghentikannya sesuka hati, Anda juga memiliki kuasa atas konfigurasinya.

Misal pada saat Anda membuat EC2 instance. Anda dapat memilih OS (operating system/sistem operasi) yang Anda inginkan, baik itu Windows atau Linux. Anda juga dapat membuat ribuan instance EC2 sekaligus dengan perpaduan sistem operasi dan konfigurasi sehingga dapat mendukung berbagai aplikasi bisnis Anda.

Selain OS, Anda juga dapat melakukan instalasi perangkat lunak apa yang ingin dijalankan pada instance. Baik itu aplikasi bisnis internal, web sederhana, web yang kompleks, database (basis data), hingga perangkat lunak pihak ketiga seperti paket perangkat lunak perusahaan. Anda memiliki kendali penuh atas apa yang ada di instance tersebut.

Instance EC2 juga dapat diubah-ubah ukurannya. Anda dapat mulai dengan menggunakan small instance (instance dengan tipe small).

Ketika aplikasi yang Anda jalankan mulai membutuhkan kapasitas yang lebih besar, Anda dapat menambahkan lebih banyak memori dan CPU. Itulah yang dinamakan vertical scaling atau mengatur skala instance secara vertikal. Intinya, Anda dapat membuat instance lebih besar atau lebih kecil kapan pun Anda mau.

Bahkan tak hanya itu. Anda juga dapat mengontrol aspek jaringan dari EC2, seperti jenis permintaan apa yang diizinkan atau bagaimana instance dapat diakses (publik atau privat). Di modul berikutnya kita akan membahas lebih lanjut berkenaan jaringan.

Sekali lagi, Amazon EC2 berjalan dengan bantuan teknologi virtualisasi. Mungkin Anda sudah tak asing ya dengan istilah mesin virtual. Yup! Karena ini bukanlah sesuatu yang baru.

Namun AWS membuat proses penyediaan server menjadi lebih mudah dan lebih hemat melalui model Compute as a Service (CaaS) seperti Amazon EC2 ini. Dengan semua keuntungan tersebut, programmer dan bisnis dapat berinovasi lebih cepat.

### Cara Kerja Amazon EC2
Mungkin kening Anda sempat sedikit mengerut, “Bagaimana cara kerja Amazon EC2?” Tak seperti server di data center yang memerlukan proses panjang, Amazon EC2 dapat digunakan dengan mudah dengan beberapa langkah saja.

- Luncurkan
Mulailah dengan memilih sebuah template dengan konfigurasi dasar untuk instance Anda. Konfigurasi dasar ini termasuk sistem operasi, server aplikasi, atau aplikasi lainnya. Anda juga dapat memilih tipe instance, yaitu konfigurasi perangkat keras tertentu dari instance Anda.
Selagi menyiapkan peluncuran instance, tentukanlah pengaturan keamanan untuk mengontrol lalu lintas jaringan yang dapat mengalir masuk dan keluar instance Anda. Nanti kita akan menjelajahi fitur keamanan Amazon EC2 secara lebih detail di materi selanjutnya.

- Hubungkan
Anda dapat terhubung ke instance dengan beberapa cara. Program dan aplikasi Anda memiliki beberapa metode berbeda untuk terhubung dan bertukar data langsung ke instance. Anda dapat terhubung juga ke instance dengan mengaksesnya dari desktop.

- Gunakan
Setelah terhubung ke instance, Anda dapat mulai menggunakannya. Ada banyak hal yang bisa dilakukan dengan Amazon EC2 instance, seperti menginstal perangkat lunak, menambah penyimpanan, menyalin dan mengatur file, dll.