NAMA: CALLISTA RAHMA PUTRI 
KELAS: D3-1A
MATA PERKULIAHAN: PROJEK 3 - PENGEMBANGAN PERANGKAT LUNAK BERBASIS WEB
TANGGAL: 10 SEPTEMBER 2026
-------------------------------
1. KASUS A 
Kasus A - Gambar tidak tampil: Ubah assets/kampus.jpg menjadi asset/Kampus.JPG. 
Muat ulang halaman, buka DevTools > Network, pilih filter Img, lalu catat status request. 
Perbaiki path berdasarkan nama folder dan file yang benar. 

**Gejala yang terlihat:** 
Gambar tidak muncul dalam website yang dijalankan
**Penyebab:**
Dikarenakan penulisan folder “assets” tidak sesuai dengan folder yang disudah dideklarasikan pada folder yang existing.
Bukan dikarenakan filename yang diubah, dikarenakan browser ataupun search engine menerapkan case-insensitive  
**Perbaikan:**
Perbaikan nama folder yang dideklarasikan dalam dokumen, “asset” menjadi “assets”

2. KASUS B
Kasus B - Tautan internal gagal: Ubah href="#jadwal" menjadi href="#agenda", 
tetapi jangan ubah ID section. Klik tautan, bandingkan href dengan ID target melalui panel Elements, 
lalu perbaiki agar pasangan nilainya sama. 

**Gejala yang terlihat:**
Link tautan tidak langsung directed menuju section yang diminta 
**Penyebab:** 
Dikarenakan Perbedaan identifier link yang diberikan pada a href dengan bagian section yang dideklarasikan pada kode 
**Perbaikan:**
Perbaikan link identifier yang dituju dengan yang berada pada bagian section. Disamakan nilainya 

3. KASUS C
Kasus C - Struktur tidak valid: Hapus tag penutup </section> dan letakkan footer sebelum penutup main. Amati DOM hasil parsing pada panel Elements, kemudian jalankan validator. Perbaiki berdasarkan pesan error pertama, lalu validasi ulang. 

**Gejala yang terlihat:**
Tidak ditemukan gejala yang signifikan terhadap tampilan website 
**Penyebab:**
Tidak ditemukannya gejala, dikarenakan browser atau search engine secara otomatis mengaktifkan error recovery pada kode yang digunakan. 
Browser langsung menganggap bahwa semua anak yang berada dibawah kolom tertentu merupakan bagian dari kolom diatasnya 
**Perbaikan:**
Perbaikan pada struktural kode yang ditulis. Penempatan dan penutup 

4. KASUS D
Kasus D - Karakter tidak terbaca: Ubah charset menjadi nilai yang salah atau hapus meta charset, 
lalu tambahkan teks Pemrograman Web: struktur, gaya, dan aksesibilitas. Amati hasilnya. 
Kembalikan <meta charset="utf-8"> pada bagian awal head.  
**Gejala yang terlihat:**
Munculnya simbol-simbol tidak relevan
**Penyebab:**
Dengan tidak menggunakan standarisasi yang telah ditentukan untuk penulisan di HTML. Website menjalankan sesuai dengan perintah.
Namun, apabila hanya dihilangkan saja bagia meta = UTF-8, web browser atau live server akan secara otomatis melakukan pelacakan dan berasumsi bahwa website yang dibangun menggunakan UTF-8.

Nilai ISO-8859-1 merupakan pengodean karakter lama. Dimana mesin membaca per em-dash dan disimpan di dalam 3 bit data. Oleh sebab itu, salah menggunakan pengkodean karakter dapat berakibat fatal pada tampilan website 
**Perbaikan:**
Mengembalikan nilai pengkodean karakter sesuai dengan standarisasi universal yaitu UTF-8



