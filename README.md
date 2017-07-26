# RESPONSI TCCL

### Membuat Aplikasi Web HTML

Web yang saya buat ini menggunakan HTML biasa. Hasilnya seperti gambar dibawah ini :
![hasil.JPG](https://github.com/endahprastiwi/responsitccl/blob/master/hasil.JPG)

IP yang diperoleh dari perintah docker-machine ip. Sehingga, diperoleh IP tersebut seperti pada url pada gambar.

### Dockerfile
Dockerfile merupakan script yang yang berisi dari serangkaian perintah yang akan dieksekusi secara otomatis dan berurutan untuk membuat sebuah image. Oleh karena itu, script yang digunakan untuk aplikasi web diatas pada Dockerfile adalah :
![3.JPG](https://github.com/endahprastiwi/responsitccl/blob/master/3.JPG)

Nah, penjelasan untuk gambar diatas adalah seperti berikut :
1. FROM httpd:2.4 merupakan images yang kita gunakan. Berarti kita menggunakan images httpd:2.42. 
2. Lalu, COPY ./public-html/ /usr/local/apache2/htdocs/ merupakan perintah yang digunakan untuk memindahkan file public_html ke dalam docker kita

Sebelum melangkah kedalam Dockerfile, kita harus membuat direktori terlebih dahulu. Perintah yang digunakan mkdir tccl. Kemudian, masuk ke dalam direktori tersebut dengan perintah cd tccl. Barulah touch Dockerfile. Lalu, vi Dockerfile dan mengetikkan script config pada file Dockerfile tersebut. Dapat dilihat pada gambar berikut ini :
![1.JPG](https://github.com/endahprastiwi/responsitccl/blob/master/1.JPG)

Gambar diatas terdapat perintah docker build -t responsi . Berarti perintah tersebut digunakan untuk membangun images yang akan kita gunakan yakni responsi. Hasilnya dapt dilihat pada gambar diatas.

![2.JPG](https://github.com/endahprastiwi/responsitccl/blob/master/2.JPG)

Gambar diatas terdapat perintah docker run -p 8080:80 --name responsi-1 responsi . Berarti perintah tersebut digunakan untuk menjalankan images responsi di localhost dengan port 80 yang namanya responsi-1. Hasilnya dapt dilihat pada gambar diatas.



### Prestasi
1. Github Contribution :https://github.com/RobertNorthard/adop-pipeline-builder/pulls?q=is%3Apr+author%3Aendahprastiwi                        


