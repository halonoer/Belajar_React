# Belajar_React

html
div id =  app
h1 = belajar react bareng wpu

DOM Manipulation
1. // seleksi elemen div dengan id 'app'
   const app = document.getElementById('app');
3. // buat element h1 baru
   const header = document.createElement('h1');
5. // buat text node untuk elemen h1 tadi
   const headerContent = document.createTextNode('Belajar React bareng WPU');
7. // append teks ke dalam h1
   header.appendChild(headerContent);
9. // simpan elemen h1 didalam div
    app.appendchild(header);

 manipulasi DOM menggunakan JavaScript
 - HTML merepresentasikan konten halaman awal
 - DOM merepresentasikan konten halaman yang telah diperbarui
 - mengubah DOM menggunakan javascript 'polos' memang terlihat 'sakti', tapi menuliskan cukup 'ribet'
 -  dengan menggunakan cara penulisan JS Vanila, waktu yang dibutuhkan akan lebih banyak
 -  developer akan menghabiskan waktu menulis instruksi mengenai 'bagaimana' sesuatu akan dilakukan
 -  akan lebih baik jika kita bisa menuliskan 'apa' yang harus dilakukan dan biarkan komputer yang memikirkan 'bagaimana' nya
 -  hal itu disebut dengan 'imperactive' dan 'declarative' programming

imperactive dan declarative programming
- imperactive programming menuliskan langkah demi langkah bagaimana sesuatu harus dilakukan
- declarative programming menuliskan apa yang akan dihasilkan
- imperactive programming bagaikan memberikan instruksi pada koki direstoran saat kita ingin memesan pizza
- declarative programming itu saat kita memesan pizaa sesuai menu tanpa menghiraukan langkah demi langkahnya
- react merupakan sebuah UI libray yang declaritve
