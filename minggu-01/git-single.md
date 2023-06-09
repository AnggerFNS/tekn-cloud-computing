# Instalasi Git Pada Windows


sebelum kita menginstall Git di windows, kita sudah harus memiliki editor teks. Bisa menggunakan [Notepad++](https://notepad-plus-plus.org/) atau [Visual Studion Code](https://code.visualstudio.com/) atau [Vim](https://www.vim.org/).


1. Setelah download [Git](https://git-scm.com/downloads), lalu buka filenya yang telah di download, lalu akan muncul lisensi, selanjutnya klik **Next**.


![install-01](https://github.com/AnggerFNS/tekn-cloud-computing/blob/83bc7adabb39b735cc1d1f27056c2d7927bd54a3/minggu-01/Picture1.png)


2. Kemudian pilih folder untuk menyimpan Git, Secara default Git akan tersimpan di folder C:\Program Files\Git, setelah itu klik **Next**.


![install-02](https://github.com/AnggerFNS/tekn-cloud-computing/blob/83bc7adabb39b735cc1d1f27056c2d7927bd54a3/minggu-01/Picture2.png)


3. Lalu klik **Next**, biarkan settingan Git secara default.


![install-02](https://github.com/AnggerFNS/tekn-cloud-computing/blob/83bc7adabb39b735cc1d1f27056c2d7927bd54a3/minggu-01/Picture3.png)


4. Klik **Next**.


![install-04](https://github.com/AnggerFNS/tekn-cloud-computing/blob/83bc7adabb39b735cc1d1f27056c2d7927bd54a3/minggu-01/Picture4.png)


5. Lalu pilih editor teks yang ingin anda gunakan (Disini saya menggunakan editor teks Visual Code Code), lalu klik **Next**.


![install-04](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture5.png)


6. Checklist pada pilihan **Git from the command line and also from 3rd-party software** selanjutnya klik **Next**.


![install-04](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture6.png)


7. Checklist pada pilihan **Use the OpenSSL library** selanjutnya klik **Next**.


![install-04](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture7.png)


8. Selanjutnya checklist pada pilihan **Checkout Windows-style, commit Unix-style...**, lalu klik **Next**.


![install-04](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture8.png)


9. Selanjutnya checklist pada pilihan **Use MinTTY...**, lalu klik **Next**.


![install-04](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture9.png)


10. Selanjutnya checklist pada pilihan **Enable file System chacing**, lalu klik **Next**.


![install-04](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture10.png)


11. Selanjutnya merupakan proses pengextract file git.


![install-04](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture11.png)


12. Selanjutnya unchecklist pada pilihan **View Release Note**, lalu klik **Finish**.


![install-04](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture12.png)


13. Cek versi Git menggunakan CMD dengan mengetikkan **git --version**.


![install-04](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture13.png)


# 02 konfigurasi git di windows
Konfigurasi Git pada windows dapat dilakukan dengan cara mengetikkan kode dibawah ini
```
$ git config --global user.name "(sesuai username pada git)"
$ git config --global user.email sesuai email yang digunakan pada git
```
![konfig1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture14.png)

Selanjutnya jika kalian ingin melihat hasil dari konfigurasi diatas maka kalian dapat mengetikkan code berikut
```
$ git config --lists
```
![konfig2](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture15.png)

Langkah ini cukup dilakukan sekali saja, kecuali jika anda ingin melakukan perubahan nama ataupun email yang sudah digunakan.


# 03. Membuat Repo Di Account Git Kita
  Untuk membuat repo, dapat menggunakan langkah-langkah berikut :
  1.  Klik tanda **+** pada bagian atas dekat profil Git, lalu pilih **New repository**
  
  ![repo1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture16.png)
  
  2. Isikan nama owner, nama repo, keterangan, pilih settingan repo untuk private atau public, checklist untuk add README.md atau tidak, serta pilih lisensi.

  ![repo2](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture17.png)
  
  3. Klik **Create Repository**
  Setelah langkah tersebut berhasil, maka repo akan dibuat dan bisa diakses dengan menggunakan pola ```https://github.com/username/reponame```. Pada repo tersebut, hanya akan muncul 1 file, yaitu LICENSE. Jika kalian memilih membuat README pada saat langkah ke 2, juga akan muncul file README.md.

  ![repo3](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture18.png)

   Ada atau tidaknya README.md tidak ada efek apapun di langkah ini.
 
 # Clone Repo
Untuk clone repo, kalian dapat mengetikkan code dibawah,

```git clone https://github.com/UserName/NameRepository```

![clone](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture19.png)

Sehingga hasil clonenya akan masuk ke penyimpanan lokal komputer kita.

![clone2](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture20.png)

# Mengelola Repo
  Setelah melakukan ```clone``` ke penyimpanan lokal komputer kita, semua manipulasi konten dilakukan di komputer lokal dan hasilnya akan di-**push** ke remote repo di GitHub. Dengan demikian, jangan ganti-ganti remote lokal sekalinya dibuat disitu, tetap disitu. Jika kehilangan repo lokal, maka anda harus melakukan clone ulang ke direktori yang kosong setelah itu baru melakukan pengelolaan repo. Beberapa hal yang biasanya dilakukan seperti berikut ini.

# Mengubah Isi - Push Tanpa Branching dan Merging
Perubahan isi bisa terjadi karena satu atau kombinasi beberapa hal berikut:
  1. File dihapus
  2. File diedit
  3. Membuat file / direktori baru
  4. Menghapus direktori

Untuk kasus-kasus tersebut, lakukan perubahan di komputer lokal, setelah itu push ke repo. 

![isi](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture21.png)

# Mengubah Isi dengan Branching and Merging
Dengan menggunakan cara ini, setiap kali akan melakukan perubahan, perubahan itu dilakukan di komputer lokal dengan membuat suatu *cabang* yang nantinya digunakan untuk menampung perubahan tersebut. Setelah itu, cabang itu yang akan dikirim ke repo GitHub untuk diminta review kemudian digabungkan (```merge```) ke master. Secara umum, repo yang dibuat biasanya sudah mempunyai satu branch yang disebut dengan ```master```. Cara ini lebih aman, terstruktur, dan mempunyai history yang lebih baik. Jika perubahan yang kita buat sudah kacau dan kita menyesal, maka ada cara untuk "membersihkan" repo lokal kita. Secara umum, langkahnya adalah sebagai berikut :

   1. Buat branch untuk menampung perubahan-perubahan
   2. Lakukan perubahan-perubahan
   3. Add dan commit perubahan-perubahan tersebut ke branch
   4. Kembali ke repo master
   5. Buat pull request di GitHub
   6. Merge pull request di GitHub
   7. Merge branch untuk menampung perubahan-perubahan tersebut ke master.
   8. Selesai.

![isi1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture22.png)

Setelah itu, klik *compare & pull request*, selanjutnya kita bisa langsung merge :

![pull](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture23.png)

Setelah itu, ```Confirm Merge```, branch yang kita kirimkan tadi sudah dimasukkan ke branch ```master```. Setelah itu, merge di komputer lokal kita :

![merge1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture24.png)

# Sinkronisasi
Suatu saat, bisa saja terjadi kita menggunakan komputer lain dan mengedit repo melalui repo lokal di komputer lain, setelah itu pindah ke kamputer lain lagi. Saat itu, kita perlu melakukan sinkronisasi ke kemputer lokal. Perintah untuk sinkronisasi adalah:

```
$ git pull
```

![pull5](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture25.png)

Perintah ini dikerjakan di direktori tempat repo lokal kita berada.

# Membatalkan Perubahan
Praktik yang baik adalah membuat *branch* pada saat kita akan melakukan perubahan-perubahan. Jika perubahan-perubahan yang kita lakukan sudah sedemikian kacaunya, maka kita bisa membuat supaya perubahan-perubahan yang kacau tersebut hilang dan kembali ke kondisi bersih seperti semula.

![batal1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture26.png)


# Undo Commit Terakhir
Suatu saat, mungkin kita sudah terlanjur mem-*push* perubahan ke repo GitHub, setelah itu kita baru menyadari bahwa perubahan tersebut salah. Untuk itu, kita bisa melakukan ```git revert```.

![batal2](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture27.png)

![undo1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture28.png)


Selanjutnya, tinggal di-*push* ke repo GitHub.

![undo2](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture29.png)



Untuk kembali ke perubahan pada saat yang sudah lama, yang perlu dilakukan adalah melakukan ```git revert <posisi>``` kemudian mengedit secara manual kemudian push ke repo.

![undo3](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture30.png)

![revert1](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture31.png)

![revert2](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture32.png)

![revert3](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture33.png)

![revert4](https://github.com/AnggerFNS/tekn-cloud-computing/blob/master/minggu-01/Picture34.png)
