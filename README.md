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

tutorial
- kunjugi web react (https://react.dev/)
- klik learn
- installation
- klik download this HTML page. (coba.html)
- buat file html (coba123.html)

menyiapkan aplikasi 
- untuk menyiapkan aplikasi react pada halaman kita, kita butuh method ReactDom.createRoot() yang diambil dari package react-dom
- method tersebut digunakan sebagai wadah untk aplikasi
- kita juga butuh method render untuk menampilkan elemen h1 kita

jika terjadi error
- klik kanan
- klik inspeksi
- klik console

error karena 
- react dimengenali h1, h1 didalam method render bukan javascript, itu adalah JSX. 
- secara default browser tidak mengenali JSX. 
- kita butuh sebuah compiler yang dapat menerjemahkan JSX jadi sintaks javascript biasa.
- kita akan menggunakan babel sebagai penerjemah-nya

menambahkan babel (babeljs.io)
- tambahkan script babel pada project kita lewat unpkg
- jangan lupa juga untuk mengubah type pada script menjadi "text/jsx" untuk menginformasikan pada babel kita akan mengubah jsx menjadi javascript

(vanila JS = JavaScript murni) = (vanilaJS.html)
react = coba123.html

bandingkan script vanila JS & React


apa bedanya JSX sama html

JSX
- JSX adalah ekstensi sintaks untuk javascript yang dapat mendeskripsikan UI dengan sintaks seperti HTML
- Meskipun masih ada cara lain untuk membuat komponen, kebanyakan developer React menggunakan JSX
- Sintaks JSX terlihat seperti HTML, tapi lebih strict dalam penulisannya dan bisa menampilkan informasi yang dinamis
- untuk menulisnya, kita harus ingat 3 aturan JSX 
- https://react.dev/learn/writing-markup-with-jsx

1. -Selalu mengembalikan satu elemen
<script type="text/babel">
   const container = document.getElementById('root');
   const root = ReactDOM.createRoot(container);
   root.render(<h1>belajar react oyyyyy 🚀</h1>);
</script>

2. -Selalu tutup semua tag

3. -Gunakan camelCase untuk atribut
const container = document.getElementById('root');
const root = ReactDOM.createRoot(container);
root.render(
    <>
        <h1>Belajar React oyyy 🚀</h1>
        <p>hahahahahha</p>
        <p onClick={e => {alert('ok!')}}>Belajar React menyenangkan bukan?!</p>
    </>
);







