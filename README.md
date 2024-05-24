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

mulai react 
- untuk menggunakan react dalam project kita, kita butuh 2 script react yang bisa kita panggil lewat unpkg.com
- react sebagai libray utama
- reacdom agar kita bisa menggunakan method-method untuk menipulasi DOM

<html>
   <body>
      <div id="root"></div>
      <script src:"https://www.unpkg.com/browse/react@18.3.1/cjs/react.development.js"></script> 
      <script src:"https://unpkg.com/browse/react-dom@18.3.1/cjs/react-dom.development.js"></script>
      <script type:"text/javascript">
         const container = document.getElementById('root');
      </script>
   </body> 
</html>

kunjugi web react (https://react.dev/)
klik learn
installation
download

