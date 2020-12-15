# ViewAndViewGroup
### Teori
Pada dasarnya semua elemen antar pengguna di aplikasi Android dibangun menggunakan dua buah komponen inti, yaitu view dan viewgroup.
Sebuah view adalah obyek yang menggambar komponen tampilan ke layar yang mana pengguna dapat melihat dan berinteraksi langsung. Contoh komponen turunan dari view seperti :
1.  **TextView**, komponen yang berguna untuk menampilkan teks ke layar.
2. 	**Button**, komponen yang membuat pengguna dapat berinteraksi dengan cara ditekan untuk melakukan sesuatu.
3.  **ImageView**, Komponen untuk menampilkan gambar.
4.  **ListView**, komponen untuk menampilkan informasi dalam bentuk list.
5.	**GridView**, komponen untuk menampilkan informasi dalam bentuk grid.
6. 	**RadioButton**, komponen yang memungkinkan pengguna dapat memilih satu pilihan dari berbagai pilihan yang disediakan.
7.	**Checkbox**, komponen yang memungkinkan pengguna dapat memilih lebih dari satu dari pilihan yang ada.
<br>
Sedangkan viewgroup adalah sebuah obyek yang mewadahi obyek-obyek view dan viewgroup itu sendiri sehingga membentuk satu kesatuan tampilan aplikasi yang utuh. Contoh komponen viewgroup adalah:
1.  **LinearLayout**,Akan menempatkan komponen-komponen di dalamnya secara horizontal atau vertikal. Linearlayout memiliki atribut weight untuk masing-masing child view yang berguna untuk menentukan porsi ukuran view dalam sebuah  ruang (space) yang tersedia.
2.	**FrameLayout**,Layout ini adalah layout yang paling sederhana. Layout ini akan membuat komponen yang ada di dalamnya menjadi menumpuk atau saling menutupi satu dengan yang lainnya.Komponen yang paling pertama pada layout ini akan menjadi alas bagi komponen-komponen di atasnya. Pada materi penggunaan fragment di materi sebelumnya, framelayout memiliki kemampuan untuk menjadi kontainer untuk fragment-fragment di dalam sebuah activity. Berikut ilustrasi penggunaan framelayout terhadap child view yang dimilikinya.
3.	**RelativeLayout**,Layout yang paling fleksible dikarenakan posisi dari masing-masing komponen di dalamnya dapat mengacu secara relatif pada komponen yang lainnya dan juga dapat mengacu secara relatif ke batas layar.
4.  **TableLayout**,Susunan komponen di dalam tablelayout akan berada dalam baris dan kolom. Namun layout jenis ini tidak akan menampilkan garis pembatas untuk baris, kolom atau cell-nya. 
<br>
Salah satu perbedaan mendasar dari keempat jenis layout di atas adalah bagaimana komponen view di dalamnya tersusun. <br>
Kapan saatnya menggunakan linearlayout, relativelayout, framelayout dan tablelayout? Jawabannya tergantung pada kebutuhan dan performa aplikasi yang dibuat. <br>
Salah satu tips performa untuk aplikasi Android adalah dengan menyusun hierarki layout dalam sebuah file layout xml secara sederhana dan flat. Artinya, kita tidak membuat layout dengan jumlah kedalaman yang tinggi. Selain itu, penting juga bagi kita untuk memahami dasar pembangunan antar muka, pengalaman pengguna ketika menggunakannya, dan selalu mencari pendekatan terbaik dalam penggunaan komponen antar muka. <br>
Semua tergantung latihan dan seberapa sering kita mengubah mockup menjadi tampilan sebenarnya, terutama dengan memaksimalkan penulisan kode antara muka di berkas xml. 
<br>
Ketika aplikasi memuat informasi yang banyak dan melebihi ukuran layar, maka Anda membutuhkan tampilan yang memungkinkan pengguna untuk membaca informasi dengan lengkap. Kita membutuhkan komponen scrollview untuk mengatasi masalah ini.
<br>
1.  **ScrollView**,Adalah layout yang memungkinkan komponen di dalamnya digeser (scroll) secara vertikal dan horizontal. Komponen di dalam scrollview hanya diperbolehkan memiliki 1 parent utama dari linearlayout, relativelayout, framelayout, atau tablelayout.
<br>
**Satuan Dimensi Android**
<br>
Platform Android dikenal karena keberagamannya. Mulai ukuran perangkatnya, layar, spesifikasi, hingga level operating system-nya. Karena keberagaman tersebut, tak heran jika dibutuhkan tampilan yang konsisten agar aplikasi kita bisa berjalan dan tampil maksimal. <br>
Android sendiri memiliki satuan unit dimensi untuk ukuran tinggi dan lebar sebuah komponen view atau viewgroup. Berikut adalah esensi dari satuan dimensi unit di android. 
1.	Ekosistem Android dikenal dengan fragmentasi spesifikasi perangkat yang sangat bervariasi. Beragam perangkat Android memiliki perbedaan dimensi layar dan kerapatan pixel (density). <br>
2.	Untuk tampilan yang konsisten di perangkat Android, terdapat 2 jenis satuan, yaitu dip/dp (density-independent pixel) dan sp (scale-independent pixels). 
3.	Satuan dp/dip digunakan untuk satuan dari nilai dimensi misal width (attribut : layout_width) dan height (attribut : layout_height) dari sebuah komponen view atau viewgroup.
4.	Satuan sp digunakan untuk ukuran teks. Perbedaannya dengan dp/dip adalah satuan sp android akan men-scale ukuran teks sesuai dengan setting ukuran teks di peranti (yang biasa dapat diakses melalui menu settings)
<br>






