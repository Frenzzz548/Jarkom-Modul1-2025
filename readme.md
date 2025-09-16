[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/tPVgLsdF)
| Name                 | NRP        | Class |
|----------------------|-----------|-------|
| Bagus Cahya Saputra  | 5025241067 | B     |



## Task 1

- Flag

  `JARKOM25{Ja0G_Bbbb4ng3t_S1_O88A0OTA5IJ4SUPMVI9NLOARZQ34M0xl0vel1o5yepswvpgrzj42cdka9bb2_4cc430660c3773420189ed1475e9e6fc}`

> a. Berapa banyak packet yang terekam pada file pcapng?

> _a. How many packets are recorded in the pcapng file?_

**Answer:** `9596`

- Filter expression

  `-`

- Explanation

  `untuk mengetahui packet yang ada di soal bisa dilihat pada display kanan bawah`

- Output result

  <img width="181" height="40" alt="soal 1a" src="https://github.com/user-attachments/assets/5a318157-7320-49e7-a10f-43126b543ed1" />


<br>
<br>

> b. Ada berapa jenis protocol (total) yang terekam pada traffic?

> _b. How many types of protocol (totals) are recorded in the traffic?_

**Answer:** `12`

- Filter expression

  `-`

- Explanation

  `telusuri melalui statistic kemudian protocol hierarchy dan terlihat ada 12 protokol yang terekam traffic`

- Output result

  <img width="1409" height="444" alt="soal 1b" src="https://github.com/user-attachments/assets/01b47829-eaf1-431d-8a86-8fb519d4829f" />


<br>
<br>

> c. Ada berapa jenis protocol berbasis TCP yang terekam pada traffic?

> _c. How many types of TCP-based applications protocol are recorded in the traffic?_

**Answer:** `8`

- Filter expression

  `-`

- Explanation

  `masih di laman yang sam adengan 1b bisa dihitung bawah ada 8 TCP yang terekam traffic`

- Output result

  <img width="1276" height="234" alt="soal 1c" src="https://github.com/user-attachments/assets/7a256718-7f4f-41c3-9afe-252a0472bbc6" />


  <br>
  <br>

> d. Ada berapa banyak packet dengan protokol TCP murni yang terekam pada traffic (tanpa data)?

> _d. How many packets with pure TCP protocol are recorded in the traffic (without data)?_

**Answer:** `3223`

- Filter expression

  `-`

- Explanation

  `masih di laman yang sama juga, bisa dilihat pada TCP kolom end packets (biasanya tidak ada data) ada 3223`

- Output result

  <img width="1106" height="367" alt="soal 1d" src="https://github.com/user-attachments/assets/6d554bd5-ef19-4fad-9930-11e8a67ff4ba" />


## Task 2

- Flag

  `put your flag here`

> a. Berapa banyak packet berhasil yang berbasis murni TCP dan memiliki flag [ACK]?

> _a. How many packets succeed that are pure TCP based and have [ACK] flag?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> b. Berapa banyak packet berhasil yang berbasis murni TCP yang hanya memiliki flag [ACK]?

> _b. How many packets succeed that are pure TCP based and have only [ACK] flag?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> c. Berapa banyak packet berhasil yang berbasis murni TCP dan memiliki flag selain hanya [ACK]?

> _c. How many packets succeed that are pure TCP based and contain flags other than just [ACK] flag?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

## Task 3

- Flag
  
  `JARKOM25{W0w_Y0uU_h4V33e_d0n3_444_9ood_j0bB_1FE0Pg0dl1k3gqlzwt2y0svvpodhncpdmy_cf9a937c7ebbd5107199f62a67eb9715}`

> a. Pada port berapa client telnet terbuka?

> _a. In what port is the telnet client open?_

**Answer:** `54184`

- Filter expression

  `telnet`

- Explanation

  `ketika di filter telnet port yang digunakannya adalah 54184`

- Output result

  <img width="956" height="590" alt="soal 3a" src="https://github.com/user-attachments/assets/66423b96-4e71-4515-9edd-c8cc7d7f758c" />


  <br>
  <br>

> b. Berapa byte file response yang dikirim dari server?

> _b. How many bytes of the response files are sent from the server?_

**Answer:** `1449`

- Filter expression

  `telnet`

- Explanation

  `pilih salah satu kemudian follow tcp stream setelah itu ubah padah kiri bawah yang semulanya entire conversastion menjadi yang dikirim ke servernya (172.16.16.102:23 -> 172.16.16.101:54184)`

- Output result

  <img width="480" height="78" alt="soal 3b" src="https://github.com/user-attachments/assets/be3ac643-7718-4a0a-94de-7abd33f59702" />


  <br>
  <br>

> c. Apa username yang digunakan client telnet untuk berhubungan dengan server?

> _c. What telnet client's username is used to connect with the server?_

**Answer:** `jovyan`

- Filter expression

  `telnet`

- Explanation

  `masih di laman yang sama, tetapi ganti ke sebaliknya (172.16.16.101:54184 -> 172.16.16.102:23) dengan mencocokan pada pengisian pengguna terlihat username yang dimasukkan adalah jovyan bisa juga di cek di entire conversation (untuk memudahkan ss saya pilih opsi pertama:))`

- Output result

  <img width="241" height="53" alt="soal 3cd" src="https://github.com/user-attachments/assets/3775ce42-18b7-4688-ab49-3d7db430f9cc" />


  <br>
  <br>

> d. Apa password client telnet?

> _d. What is the telnet client's password?_

**Answer:** `123`

- Filter expression

  `telnet`

- Explanation

  `masih di laman yang sama dan cara yang sama seperti 3c di (172.16.16.101:54184 -> 172.16.16.102:23) dengan mencocokan pada pengisian pengguna terlihat password yang dimasukkan adalah 123 bisa juga di cek di entire conversation (untuk memudahkan ss saya pilih opsi pertama:))`

- Output result

  <img width="241" height="53" alt="soal 3cd" src="https://github.com/user-attachments/assets/0cbf2163-1c41-4a1c-92a0-7d8ccbb03372" />


  <br>
  <br>

## Task 4

- Flag

  `JARKOM25{G04t__a4n4liz333er_NPISU7MXCGG5N4D0QXOOfr0gixro2rdtnc8tzbzr3ys7050166420_04be7ea5ea27cb6389d06d3d8461b8e9}`

> a. Apa perintah pertama yang ditulis client pada koneksi telnet?

> _a. What is the first command that client wrote on telnet connection?_

**Answer:** `echo`

- Filter expression

  `telnet`

- Explanation

  `masih dilaman yang sama dengan task sebelumnya kita pindah lagi ke entire conversation bisa diperhatikan perintah setelah memasukkan password adalah echo`

- Output result

  <img width="1254" height="235" alt="soal 4a" src="https://github.com/user-attachments/assets/28c26cc4-6994-4c01-aeeb-9e6abec2cb35" />


  <br>
  <br>

> b. Apa nama file .txt di server (ditulis bersama ekstensinya)?

> _b. What is the name of .txt file on the server (write with the extension)?_

**Answer:** `test.txt`

- Filter expression

  `telnet`

- Explanation

  `masih dilaman yang sama kita beralih lagi pada bagian (172.16.16.102:23 -> 172.16.16.101:54184) bisa terlihat file .txt yang di server adalah test.txt`

- Output result

  <img width="1249" height="746" alt="soal 4b" src="https://github.com/user-attachments/assets/8961a501-d214-4c2e-81d5-10f78713076d" />


  <br>
  <br>

> c. Apa kata pertama dari frasa yang dimasukkan client ke dalam file sebelumnya?

> _c. What is the first word that the client inserted into the previous file?_

**Answer:** `Jarkom`

- Filter expression

  `telnet`

- Explanation

  `lagi lagi masih di laman yang sama kembali ke (172.16.16.101:54184 -> 172.16.16.102:23) terlihat kata pertama yang dimasukan adalah N.Jarkom tapi karena N dihapus menyisakan Jarkom`

- Output result

  <img width="1230" height="234" alt="soal 4c" src="https://github.com/user-attachments/assets/bcd211e7-bd24-4acd-9607-3755244828b2" />


  <br>
  <br>

## Task 5

- Flag
  
  `JARKOM25{n4il0ng_m1lk_dr4g000n_RL6HH65EB92RF2T05DSUQTQXMLXJYYcr0c1v04hu6j3isln5nx9x0ob434_938c61b2e35cc578c858e491c092ee70}`

> a. Berapa banyak packet berbasis HTTP yang terekam pada file pcapng?

> _a. How many HTTP packets are recorded in the pcapng file?_

**Answer:** `298`

- Filter expression

  `http`

- Explanation

  `terlihat setelah di filter pada kanan bawah terdapat display sebanyak 298`

- Output result

  <img width="322" height="35" alt="soal 5a" src="https://github.com/user-attachments/assets/4b68e615-6643-45c7-8168-282819279283" />


  <br>
  <br>

> b. Ada berapa HTTP packet yang berupa response?

> _b. How many response HTTP packets are recorded in the traffic?_

**Answer:** `149`

- Filter expression

  `http.response`

- Explanation

  `terlihat setelah di filter pada kanan bawah terdapat display sebanyak 149`

- Output result

  <img width="315" height="33" alt="soal 5b" src="https://github.com/user-attachments/assets/745908ba-7eac-4a2f-ac32-b8c9178f4e79" />


  <br>
  <br>

> c. Ada berapa paket berbasis HTTP yang berhasil?

> _c. How many HTTP packets that succeed?_

**Answer:** `296`

- Filter expression

  `http`

- Explanation

  `setelah di filter hhtp kemudian sort descending pada bagian info maka terlihat ada 2 packet yang not captured`

- Output result

  <img width="1850" height="192" alt="soal 5c" src="https://github.com/user-attachments/assets/27ace3ff-6099-4bb3-bd58-62ab223c9d68" />


  <br>
  <br>

> d. Apa alamat IP dari client HTTP yang tersambung lokal dengan mesin lain?

> _d. What is the client HTTP IP Address in connection with other local machine?_

**Answer:** `172.16.16.101`

- Filter expression

  `http.request`

- Explanation

  `dapat dilihat pada kolom source terdata IP 172.16.16.101 dengan destinasi berbeda`

- Output result

  <img width="1129" height="125" alt="soal 5d" src="https://github.com/user-attachments/assets/639e406b-da1b-423e-ad7d-4d54594823f4" />


  <br>
  <br>

## Task 6

- Flag

  `JARKOM25{br0mb44rdin0u_Cr0ccc0c0c0cdi1l10l_5929151114awaesalabqnqhdotsh1n0buBNHFFEFYK91AOZ2_b0fc0504b0cedfd7219647db13f318d9}`

> a. Apakah kamu menemukan fake flag? Tuliskan seluruhnya!

> _a. Did you find the fake flag? Write it whole!_

**Answer:** `FakeFlag{JarkomGampang}`

- Filter expression

  `falg.txt (string)`

- Explanation

  `karena pada hint dinyatakan bahwa fakeflag terletak di flag.txt jadi saya langsung filter sting flag.txt atau bisa temukan packet yang berisi flag.txt kemudian follow http stream dan terdapat fakeflag di dalamnya`

- Output result

  <img width="1074" height="118" alt="soal 6ab" src="https://github.com/user-attachments/assets/08b38a23-7259-4a23-942c-6936f1bb39a7" />

  <img width="515" height="361" alt="soal 6a" src="https://github.com/user-attachments/assets/dab46e08-9acb-47a3-b93d-d2bd1df6bbf4" />


  <br>
  <br>

> b. Tuliskan username dan password yang tertulis! (format username:password)

> _b. Write the written username and password! (format username:password)_

**Answer:** `Rey:123`

- Filter expression

  `http`

- Explanation

  `seperti terlihat pada ss sebelumnya kebetulan sudah tersort sehingga ada passwd kemudian follow http stream`

- Output result

  <img width="493" height="368" alt="soal 6b" src="https://github.com/user-attachments/assets/14672cb7-4fd4-418a-a910-c434ce6b749b" />


  <br>
  <br>

## Task 7

- Flag

  `JARKOM25{tr414le10_tr1lil1_lsfmc35a4ok3b0s0sQDVJ2A9DRDDTZZI_bdb74a493603c59b2a0c891696d47132c}`

> Apa nama gambar yang direquest oleh client? (tulis dengan ekstensinya)

> _What is the image that is being requested by the client? (write with its extension)_

**Answer:** `donalbebek.jpg`

- Filter expression

  `-`

- Explanation

  `Pilih menu File kemudian Export Objects pilih HTTP setelah itu ubah content type menjadi image/jpeg`

- Output result

  <img width="1095" height="145" alt="soal 7b" src="https://github.com/user-attachments/assets/770b49d6-8fbb-4be4-9708-cb651ff1a493" />


  <br>
  <br>

## Task 8

- Flag
  
  `JARKOM25{y0u_4r3_s0_G00d_1n_F0r3nsic_6ALN8PONQJF1GB8CL5UUZCHVMKIIHAx45y4n61rgu058amsie6wlbi9mdaa0_ac22c09cf55210d98ac5e637308d55c3}`

> a. Berapa banyak packet berbasis FTP yang terekam pada file pcapng? (with the data)

> _a. How many FTP packets are recorded in the pcapng file? (with the data)_

**Answer:** `81`

- Filter expression

  `ftp || ftp-data`

- Explanation

  `setelah di filter dapat dilihat pada display terdata ada 81 packets`

- Output result

  <img width="1920" height="911" alt="soal 8a" src="https://github.com/user-attachments/assets/1271c347-ae4e-4789-9d2d-21ac28efcbf0" />


  <br>
  <br>

> b. Apa username dan password client di koneksi FTP? (tulis dalam format username:password)

> _b. What is the client's username and password in FTP connection? (write in following format username:password)_

**Answer:** `rey:password123lingangu`

- Filter expression

  `ftp || ftp-data`

- Explanation

  `klik kanan dalah satu ftp kemudian follow tcp stream maka akan terlihat usernam beserta password dari client`

- Output result

  <img width="356" height="290" alt="soal 8b" src="https://github.com/user-attachments/assets/b13e54d9-17b6-42b9-ba5c-525fff21ea4a" />


  <br>
  <br>

> c. What is the client's command for showing server directory that was sent on request packet?

> _c. Apa command client untuk melihat direktori server yang dikirimkan dalam request packet?_

**Answer:** `LIST`

- Filter expression

  `ftp || ftp-data`

- Explanation

  `masih di laman yang sama scroll ke bawah sampai menemukan cmd LIST yang terlihat meminta server mengirimkan daftar file/direktori di direktori saat ini`

- Output result

  <img width="568" height="118" alt="soal 8c" src="https://github.com/user-attachments/assets/dbeca837-c99b-42fb-a186-f31d9575070f" />


  <br>
  <br>

## Task 9

- Flag

  `JARKOM25{j4rk000000mm_g4mpp4444n999999_40909707358i41L4hlrgjapz08l321k0ncolXILJW7BTGHQVWJ7_9aef277cb99e980cc3f2ebaefcb4c24b}`

> a. Apa alamat IP dari FTP server?

> _a. What is the FTP server IP Address?_

**Answer:** `172.16.16.101`

- Filter expression

  `ftp || ftp-data`

- Explanation

  `pada kolom info bisa dilihat ketika request pengguna destinasinya adalah 172.16.16.101 begitu juga response yang berasal 172.16.16.101 juga`

- Output result

  <img width="1522" height="381" alt="soal 9a" src="https://github.com/user-attachments/assets/3eea4fc0-098f-443f-bd7f-172bd0a858e3" />


  <br>
  <br>

> b. Berapa banyak file yang ada dalam direktori FTP server?

> _b. How many files are there inside the FTP server directory?_

**Answer:** `7`

- Filter expression

  `ftp-data`

- Explanation

  `terlihat ada 3 ftp-data dengan info LIST klik kanan salah satu kemudian follow tcp-stream hitung file yang ada kecuali drwxr-xr-x yang merupakan checkpoint`

- Output result

  <img width="1920" height="1080" alt="soal 9bc" src="https://github.com/user-attachments/assets/202fb69c-cb4e-41e9-9d31-8ced4d4b67e8" />

  <img width="829" height="208" alt="soal 9b" src="https://github.com/user-attachments/assets/f96722ce-1fc8-4009-b7b6-abac0a0517eb" />


  <br>
  <br>

> c. Apa nama dari file yang digunakan dalam page.html? (tulis lengkap namanya beserta ekstensinya dan dipisahkan dengan koma ',')

> _c. What are the filenames used in the page.html? (write the filebames with their extensions and separate them with comma ',')_

**Answer:** `pokijan.jpg,research_center.jpg`

- Filter expression

  `ftp-data`

- Explanation

  `terlihat pada info salah satu packet ada page html kemudian kita follow tcp stream dan terdapat dua file jpg`

- Output result

  <img width="1920" height="1080" alt="soal 9bc" src="https://github.com/user-attachments/assets/15ee0558-1562-4807-bb97-c025fe4e0509" />

  <img width="380" height="150" alt="soal 9c" src="https://github.com/user-attachments/assets/bfba6fa0-660d-49cd-9094-7db6580c71d6" />


  <br>
  <br>

## Task 10

- Flag

  `put your flag here`

> a. Apa nama file yang mengandung string terencode?

> _a. What is the filename that contains encoded string?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> b. Apa nama file hasil copy file sebelumnya?

> _b. What is the filename of the previous file copy?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

> c. What is the decoded string from the previous file?

> _c. Apa decoded string dari file tersebut?_

**Answer:** `put your answer here`

- Filter expression

  `put your filter here (if any)`

- Explanation

  `put your explanation here`

- Output result

  `put your output result here`

  <br>
  <br>

## Summary

## Problems
