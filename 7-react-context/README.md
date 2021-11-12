# React Context

---
## 1.0 - Routing

- Buatlah rute:
  - `/` : Menampilkan komponen `Home` (di dalamnya terdapat komponen `Cats`)
  - `/login` : Menampilkan komponen `Login`
  - `/cat/:nama-kucing` : Menampilkan komponen `CatDetail`
  - Selain rute diatas, tampilkan komponen `NotFound404`

---

## 2.0 - Cats

- Pada komponen `Cats`, ambil data pada API ini
  ```
  https://api.thecatapi.com/v1/breeds
  ```
- Simpan hasil data yg sudah di dapatkan ke dalam property `cats` pada `CatContext`, lalu tampilkan datanya
- Setiap data kucing dapat di klik. Ketika di klik, ambil nama kucing lalu ubah url menggunakan `history` menjadi `/cat/{namaKucing}`

---

## 3.0 - Cat Detail

- Pada komponen `CatDetail`, ambil parameter nama kucing dari url lalu ambil data dari api berikut
  ```
  https://api.thecatapi.com/v1/breeds/search?q={namaKucing}
  ```
- Simpan hasil data yg sudah di dapatkan ke dalam state `cat`
- Lalu tampilkan datanya

---

## 3.0 - Login

- Buat data user pada `mockapi.io`
- Jika data yg di input sesuai dengan data pada `mockapi.io`, maka buat data `isLogin` dgn nilai `true` ke dalam localStorage
- Buat `UserContext`, di dalamnya tambahkan useEffect untuk mengambil data isLogin dari localStorage.
- Pada `App.js`, ambil `isLogin` dari `UserContext`.
- Jika `isLogin`
  - `false`, alihkan rute `/` ke rute `/login`
  - `true`, buat navigasi logout

---


