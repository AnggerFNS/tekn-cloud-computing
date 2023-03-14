# 04. Git Kolaborasi
# FORK
  Fork adalah membuat clone dari suatu repo di GitHub milik upstream author, diletakkan ke milik kontributor dan Fork hanya dapat dilakukan sekali saja. Proses untuk fork ini meliputi:
1. Fork repo di web GitHub.
2. Clone fork tersebut de komputer lokal.
3. Kontributor harus memfork repo upstream author sehingga di repo kontributor muncul repo tersebut. Proses forking ini dijelaskan dengan langkah-langkah berikut:
    1. Login ke GitHub, 
    2. Akses repo yang akan di-fork : https://github.com/harry-prd/aksesoris-hp.git,
    3. Pada sisi kanan atas, klik tulisan Fork :
    
    ![fork1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab1.png)
    
    4. Selanjutnya isi Repo name, keterangan, lalu klik **Create Fork**
    
    ![fork2](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab2.png)
    
    5. Maka hasilnya akan seperti gambar dibawah ini.
    
    ![fork3](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab3.png)

Setelah proses tersebut, clone di komputer lokal:

![clone](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab4.png)

Untuk keperluan berkontribusi, ada 2 nama repo yang harus diatur:
   1. origin: menunjuk ke repo milik kontributor di GitHub, hasil dari fork.
   2. upstream: menunjuk ke repo milik upstream author (repo asli) di account harry-prd.
Repo origin sudah dituliskan konfigurasinya pada saat melakukan proses clone dari repo kontributor. Konfigurasi repo upstream harus dibuat, lalu tambahkan remote upstream, hasilnya maka akan seperti gambar dibawah ini

![kolab1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab5.png)

# Mengirimkan Pull Request
Setiap kali melakukan perubahan, kirim perubahan tersebut. Pengiriman ini disebut dengan Pull Request. Pada posisi ini, kontributor bisa mengirimkan kontribusi dengan cara mengirimkan pull request (PR) ke upstream author. Secara umum, langkahnya adalah sebagai berikut:
  1. Kontributor akan bekerja di repo lokal (create, update, delete isi)
  2. Commit
  3. Push ke repo kontributor
  4. Kirimkan PR ke repo upstream author.
  5. Upstream author me-review dan kemudian menyetujui (merge) atau menolak PR.
  6. Jika disetujui dan di-merge ke repo dari upstream author, sinkronkan repo di komputer lokal dan repo GitHub kontributor.
Berikut ini adalah contoh pengiriman perubahan isi README.md dengan menambahkan kontributor.
# Membuat Perubahan di Repo Lokal
Sebelum melakukan perubahan, pastikan:
  1. Sudah ada koordinasi secara manual tentang perubahan-perubahan yang akan dilakukan.
  2. Setelah melakukan perubahan-perubahan, pastikan bahwa isi repo lokal tersinkronisasi dengan repo dari upstream author.
  3. Cara melakukan sinkronisasi:
  4. Lakukan perubahan-perubahan, setelah itu push ke origin (milik kontributor)
  ![kolab2](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab6.png)
  
  ![kolab3](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab7.png)
  
  ![kolab4](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab8.png)

  
  5. Setelah itu, buka halaman Web dari repo kontributor https://github.com/harry-prd/aksesoris-hp.git. Pada halaman tersebut akan ditampilkan isi yang kita push.
  
  ![kolab6](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab9.png)
  
  6. Pilih ```Compare and pull request```, kemudian isikan deskripsi PR dan klik pada ```Create pull request```:
   
  ![kolab7](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab10.png)
  
  7. Pada repo upstream author, muncul angka 1 (artinya jumlahnya 1) pada Pull requests di bagian atas.
  8. Upstream author bisa menyetujui setelah melakukan review: klik pada Pull requests, akan muncul PR dengan message seperti yang ditulis oleh kontributor (Add: contributor). Klik pada PR tersebut, review kemudian klik Merge pull request diikuti dengan Confirm merge. Setelah itu, status akan berubah menjadi Merged.
  9. Sinkronkan semua repo (lokal maupun GitHub kontributor)
  
  ![kolab8](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/kolab11.png)
