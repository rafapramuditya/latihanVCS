# CARA PENGGUNAAN GIT
## Instalasi GIT
#### - Download GIT,buka website resminya GIT (git-scm-com).
#### - Kemudian untuk git suseuai dengan arsitektur komputer kita. Kalau menggunakan 64bit. Begitu juga kalau menggunakan 32bit.
#### - Selamat, GIT sudah terinstal di Windows, Untuk mencobanya, silahkan buka CMD atau PowerShell, Kemudian Ketik perintah
```
## git --Version
```
![Gambar1](gambar/git.png)
#### - Pada saat pertama kali menggunakan git, perlu dilakukan Konfigurasi user.name dan user.email
#### - konfigurasi ini bisa dilakukan untuk global repository atau individual revository
#### - Apabila belum di lakukan Konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah global git commit
#### - Config Global Repository
$ git config -- global user.name "nama_user"
$ git config -- global user.email "nama_user"

## Perintah Dasar Git
#### - git init,perintah untuk membuat repository lokal.
#### - git add,perintah untuk menambahkan file pada staging sebelum proses commit.
#### - git push-u origin master, perintah untuk menggirim perubahan pada repository lokal menuju server repository.
#### - git clone [url], perintah untuk membuat working di rectory yang di ambil dari repository server.
#### - git remote add origin[url],perintah untuk menambahkan remote server/repository server pada lokal repository(*working directory*)
#### - git pull, perintah untuk mengambil/mendownload perubahan terbaru dari server repository ke lokal repository.

## Membuat Repository Lokal

#### - Buka directory aktif misal : C:\Users\User\Desktop\dlabs_pemograman1 (buka menggunakan Windows Explorer)
#### - Klik kanan pada directory aktif tersebut, dan pilih menu Git Bash. sehingga muncul git bash command
#### - Buat directory project praktikum pertama dengan nama Latihan1

$ mkdir Latihan1

$ cd Latihan1

#### - Sehingga terbentuk suatu directory baru dibawahnya, selanjutnya masuk kedalam directory tersebut dengan perintah cd (change directory).
#### - Directory aktif menjadi : C:\Users\User\Desktop\dlabs_pemograman1\Latihan1

## Membuat Repository Lokal

#### - Jalankan perintah git init, untuk membuat repository lokal.

$ git init
#### - Repository baru berhasil di inisialisasi, dengan terbentuknya satu directory hidden dengan nama .git
#### - Pada directory tersebut, semua perubahan pada working directory akan disimpan.

## Menambahkan File Baru pada Repository

#### - Untuk menambahkan file dapat menggunakan text editor, lalu menyimpan filenya pada directory aktif (repository).
#### - Disini kita akan coba buat satu file bernama README.md (text file)

$ echo "# Latihan 1 " >> README.md
#### - File README.md berhasil dibuat.

#### - Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.

$ git add README.md

#### - File README.md berhasil ditambahkan.

## Commit (Menyimpan Perubahan ke Database)
#### - Untuk menyimpan perubahan yang ada kedalam databse repository lokal, gunakan perintah git commit -m "komentar commit"
#### - Perubahann berhasil disimpan

## Membuat Reposity Server

#### - Server repository yang akan kita gunakan adalah http://github.com
#### - Anda harus membuat akun terlebih dahulu
#### - Pada laman github, klik tombol start a project, atau 
####   dari menu (icon +) klik New Repository.


#### - Isi nama repositorynya, misal: labpy.
#### - Lalu klik tombol Create repository.


## Menambahkan Remote Repository

#### - Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada lokal repository, sehingga dapat diakses oleh banya user.
#### - Untuk menambahkan remote repository server, gunakanlah perintah
####  Git remote add origin [url]

$ git remote add https://github.com/rafapramuditya/labpy1.git

## Push ( Mengirim Perubahan ke Server)

#### - Untuk mengirim perubahan pada lokal repostiory ke server gunakan perintah git push.

$ git push -u origin master

#### - Perintah ini akan meminta memasukkan username dan password pada akun anda di github.com

## Melihat Hasilnya pada Server Repository
#### - Buka laman github.com, arahkan pada repositorynya
#### - Maka perubahan akan terlihat pada laman tersebut


## Clone Repository
#### - Clone repository, pada dasarya adalah meng-copy repository server dan secara otomatis membuat satu directory sesuai dengan nama repositorynya (working directory).
#### - Untuk melakukan cloning, gunakan perintah git clone [url]

$ git clone [https://github.com/rafapramuditya/labpy1.git]

## Kegunaan file README.md
#### - Apabila kita menggunakan github, untuk memberikan penjelasan awal pada project yang kita buat, maka dapat menggunakan sebuah file yang bernama README.md.
#### - Pada file tersebut kita dapat membuat dokumentasi awal dari setiap project yang kita buat untuk memberikan penjelasan atau sekedar cara peggunaan dari aplikasi yang kita kembangkan.
#### - Penulisan file README.md berbasis teks, dan untuk pemformatannya menggunakan Markdown format.
#### - Untuk lebih jelasnya, dapat anda pelajari cara penggunaannya markdown pada url berikut: https://guides.github.com/features/mastering-markdown/
