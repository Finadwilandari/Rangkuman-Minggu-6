# 22 Agustus 2022-26 Agustus 2022

## React JS Hooks
Hooks adalah suatu fitur baru di React 16.8. Fitur ini memungkinkan kita menggunakan state dan fitur React lainnya tanpa menuliskan sebuah kelas.

>Adapun kelebihan dari penggunaan hooks yaitu dengan menggunakan functional component dan menggunakan hooks maka kode akan terlihat lebih clean, pendek, dan mudah dimengerti.

## UseState

Penerapannya:

Cara menggunakannya :

Import useStates dari react
>import {useStates} from "react";

Menulis useStates hooks
>const [nama, setNama] = useStates("luthfi")

Memanggil data
><p> Hallo, saya {nama} </p>

Mengupdate state
><button onClick={ setNama("nama")> }> ubah </button>

contoh:

<img src="react code.jpg">

adapun beberapa hooks yang jarang digunakan, diantaranya:
1. useContext
2. useReducer

>Dalam menggunakan hooks, perintah harus selalu dipanggil di bagian atas component. Biasanya setelah pembuatan function component sama halnya dengan useStates dan useEffect

<img src="hooks code.jpg">

dari tampilan di atas, gunakan tanda [] di akhir useEffect agar tidak terjadi re render yang berlebihan.

<img src="hooks code change.jpg">

## React Router 

React Router merupakan sistem perpustakaan standar yang dibangun di atas React dan digunakan untuk membuat perutean di aplikasi React menggunakan Paket React Router.

Basic Instalation:

>npm install recat-router-dom@6

Create React App dengan cara import 

>import {BrowserRouter} from "react-router-dom";

Barulah kita bisa menggunakan React Router.

## Penggunaan Tag Script HTML

```Salah satu cara tercepat untuk menambahkan React dan React Router ke situs web adalah dengan menggunakan <script>tag lama dan variabel global. React Router kompatibel dengan React 16.8+. Cukup tambahkan <script>tag berikut ke HTML Anda, tepat sebelum </body>tag penutup```.

Komponen di React Router

>Ada dua jenis komponen router:
><BrowserRouter: digunakan untuk menangani URL dinamis.
><HashRouter: digunakan untuk menangani permintaan statis.

## React Redux
Redux merupakan salah satu library state management yang biasa disandingkan dengan react.
sederhananya yaitu dengan menyimpan state di satu tempat, sehingga lebih mudah untuk di manage.

## Cara kerja Redux
Ada 4 faktor utama :
- UI
yaitu tampilan aplikasi
- Action
yaitu sebuah function yang mereturn sebuah objek.
Objek tersebut memiliki sebuah property wajib yaitu type.
Type inilah yang menentukan bagaimana statenya akan diubah.
- Reducer
yaitu sebuah fungsi yang tugasnya untuk mengolah state yang ada di store.
Misalnya menambah data, menghapus data, mengambil data, dan lain-lain.
Ada 2 parameter wajib dari reducer, yaitu state dan action.
- Store
yaitu tempat untuk menampung state.
Jadi store ibarat database untuk frontend.
Alur kerjanya seperti berikut:
Pertama akan ada triger dari UI
Kemudian ke action. Lalu
dari action reducer akan mengubah state yang sesuai dengan type dari action tadi. Kemudian terahir update UI lagi.
