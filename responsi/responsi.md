# Konfigurasi Image MySQL
1. Buka [Docker Official Image](https://hub.docker.com/search?q=&type=image&image_filter=official) lalu cari image yang diinginkan, disini saya menggunakan [image MySQL](https://hub.docker.com/_/mysql)
2. Selanjutnya pull image MySQL dengan mengetikkan perintah ```docker pull mysql``` lalu Cek apakah image berhasil di pull dengan mengetikkan perintah ```docker images```<br>
![gb1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/ab8961b1212e72a485de712d84f1ca993cdd5a0a/responsi/1.PNG)<br>
3. Setelah itu jalankan containers MySQL yang dibuat tadi pada cmd dengan mengetikkan perintah berikut ```docker run --name=mysql-docker -d mysql:latest``` dan cek apakah containers MySQL tadi berhasil berjalan atau tidak dengan mengetikkan perintah ```docker ps```<br>
![gb2](https://github.com/AnggerFNS/tekn-cloud-computing/blob/ab8961b1212e72a485de712d84f1ca993cdd5a0a/responsi/2.PNG)
4. Cek apakah Client MySQL sudah bisa digunakan atau belum dengan mengetikkan perintah ```docker logs some-mysql```<br>
![gb3](https://github.com/AnggerFNS/tekn-cloud-computing/blob/ab8961b1212e72a485de712d84f1ca993cdd5a0a/responsi/3.PNG)
5. Coba jalankan Client MySQL dengan mengetikkan perintah ```docker exec -it some-mysql bash``` lalu ketikkan perintah ```mysql -uroot -p``` pada terminal bash<br>
![gb4](https://github.com/AnggerFNS/tekn-cloud-computing/blob/ab8961b1212e72a485de712d84f1ca993cdd5a0a/responsi/4.PNG)

# Buat Repository Baru Di DockerHUB
1. Kunjungu website [DockerHUB](https://hub.docker.com/), lalu klik create repository, isikan repository name, lalu klik create untuk membuat repository baru<br>
![gb5](https://github.com/AnggerFNS/tekn-cloud-computing/blob/ab8961b1212e72a485de712d84f1ca993cdd5a0a/responsi/5.PNG)
2. Selanjutnya login pada Docker lokal dengan akun Docker Hub dengan mengetikkan perintah ```docker login``` Kemudian buat tag pada sample docker dengan mengetikkan perintah ```docker tag mysql:latest anggerfadhlullah/mysql_docker:latest```<br> <br>
![gb6](https://github.com/AnggerFNS/tekn-cloud-computing/blob/ab8961b1212e72a485de712d84f1ca993cdd5a0a/responsi/6.PNG)
3. Push sample ke Docker Hub dengan mengetikkan perintah ```docker push anggerfadhlullah/mysql_docker:latesst.<br>
![gb7](https://github.com/AnggerFNS/tekn-cloud-computing/blob/ab8961b1212e72a485de712d84f1ca993cdd5a0a/responsi/7.PNG)

# Mencoba Menjalankan Perintah SQL
Disini saya membuat perintah SQL untuk CRUD (Create, Read, Update, dan Delete) data dalam database, untuk perintah yang pertama disini saya membuat sebuah database dengan mengetikkan perintah ```CREATE database tekcloud;```, setelah itu membuat table list_mahasiswa dengan perintah ```CREATE TABLE mahasiswa (id int, nama varchar (255), alamat varchar (255);```, selanjutnya isikan data ke dalam table list_mahasiswa dengan mengetikkan perintah ```INSERT INTO mahasiswa (id, nama, alamat) VALUES ('1', `Angger', 'Bojonegoro');```, lalu membaca data yang diinputkan tadi dengan perintah ```SELECT * FROM mahasiswa;```, lalu update data, disini saya mengupdate data nama yang awalnya ***Angger*** di update menjadi ***Angger Fadhlulloh*** dengan mengetikkan perintah ```UPDATE mahasiswa SET nama='Angger Fadhlulloh' WHERE id='1';```, Cek lagi apakah data berhasil terupdate atau tidak dengan mengetikkan perintah ```SELECT * FROM mahasiswa;```, Proses yang terakhir adalah menghapus data mahasiswa yang tersimpan di table dengan mengetikkan perintah ```DELETE FROM mahasiswa;```, cek kembali apakah data berhasil terhapus atau tidak dengan mengetikkan perintah ```SELECT * FROM mahasiswa```, disini proses CRUD pada MySQL telah berhasil dilakukan<br>
![gb8](https://github.com/AnggerFNS/tekn-cloud-computing/blob/ab8961b1212e72a485de712d84f1ca993cdd5a0a/responsi/8.PNG)<br>
![gb9](https://github.com/AnggerFNS/tekn-cloud-computing/blob/ab8961b1212e72a485de712d84f1ca993cdd5a0a/responsi/9.PNG)<br>
![gb10](https://github.com/AnggerFNS/tekn-cloud-computing/blob/ab8961b1212e72a485de712d84f1ca993cdd5a0a/responsi/10.PNG)

