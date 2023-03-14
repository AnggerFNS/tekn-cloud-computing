# Instalasi Git Pada Wnidows


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
Konfigurasi Git pada windows dapat dilakukan dengan cara mengetikkan kode dibawah ini di CMD
```
$ git config --global user.name "AnggitaAlbiantara
$ git config --global user.email anggita.albiantara@students.utdi.ac.id
```
![konfig1](https://github.com/AnggitaAlbiantara/tekn-cloud-computing/blob/f9ab2c90c09b90fbacf1ae39145622ad0f97faaf/minggu-01/konfig1.PNG)

Selanjutnya jika kalian ingin melihat hasil dari konfigurasi diatas maka kalian dapat mengetikkan code berikut di CMD
```
$ git config --lists
```
![konfig2](https://github.com/AnggitaAlbiantara/tekn-cloud-computing/blob/f9ab2c90c09b90fbacf1ae39145622ad0f97faaf/minggu-01/konfig2.png)

Langkah ini cukup dilakukan sekali saja, kecuali jika kalian ingin melakukan perubahan nama dan email.
