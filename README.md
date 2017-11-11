# Cara penggunaan github
Cara penggunaan github untuk berkolaborasi mengelola pekerjaan

### 1. git clone

Perintah "**git clone**" digunakan untuk mengunduh code yang ada pada repository.

**git clone < repository yang akan di gunakan >**

**contoh penggunaan perintah "git clone":**
```bash
$ git clone https://github.com/bantenprov/advancetrust.git
$ cd advancetrust/
```

<img src="images/git-tut1.png">

### 2. git pull
Perintah git pull ini akan sering kali digunakan apabila kita dalam bekerja membuat suatu aplikasi atau mengembangkan aplikasi secara tim.

**contoh penggunaan git pull**
```bash
$ git pull origin master
```
<img src="images/git-tut3.png">

<br><br>
Setelah berhasil menjalankan perintah **git clone**, di sini akan di contohkan bagaimana menambahkan folder baru yang di beri nama **flowchart** 

```bash
$ mkdir flowchart
```
<img src="images/git-tut4.png">

setelah menjalankan perintah diatas maka akan ada folder baru dengan nama **flowchart**, selanjutnya berpindah ke folder / directory yang telah dibuat tadi, dengan menggunakan perintah :

```bash
$ cd flowchart
```
<img src="images/git-tut5.png">

setelah berada di folder / directory "**flowchart**", pada contoh ini akan mencoba menambahkan file baru yang di beri nama "**.gitignore**" dengab cara menjalankan perintah seperti di bawah ini :

```bash
$ echo "" > .gitignore
```
<img src="images/git-tut6.png">

jika berhasil maka akan ada file baru dengan nama "**.gitignore**", untuk melihat file yang telah berhasil di buat tadi jalankan perintah berikut :

```bash
$ ls -la
```
maka akan terlihat seperti gambar berikut :

<img src="images/git-tut7.png">
sampai pada langkah ini kita telah berhasil menambahkan folder "**flowchart**" dan di dalam folder tersebut telah ada file "**.gitignore**"

berikutnya kita akan update folder dan file yang sudah di buat tadi ke repository yang di clone di awal tadi dengan cara kita kembali ke folder awal yang di clone tadi dengan perintah berikut :

### 3. git add
Dengan menggunakan perintah ini, maka artinya sama aja kita menyuruh agar si git untuk melakukan penambahan (add) pada semua file dalam folder


```bash
$ cd ../
$ git add flowchart/
$ git status

```
jika semua berhasil dan tidak ada masalah maka akan tampil seperti gambar berikut :

<img src="images/git-tut8.png">

perintah selanjutnya 

```bash

$ git commit -m "<isi pesan>"

```

<img src="images/git-tut9.png">

### 4. git push
 **git push** adalah memasukkan file-file atau direktori hasil kerjaan kita yang dilakukan setelah melakukan commit ke tempat penyimpanan projeknya (misal dalam kasus ini adalah github).

terakhir kita akan menjalankan perintah **git push** 

```bash
$ git push origin master
```
jika tidak ada error maka akan tampil seperti gambar berikut :

<img src="images/git-tut10.png" alt="">


