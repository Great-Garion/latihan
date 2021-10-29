# React useEffect

---
## 1.0 - Mengambil data
- Buat komponen `CatList`
- siapkan state `cats` dan `catsTemp`
- Gunakan `useEffect()` yg bejalan 1x saja untuk mengambil data dari API, lalu masukkan data yg sudah didapatkan ke dalam `cats` dan `catsTemp`
  ```
  API -> https://api.thecatapi.com/v1/breeds
  ```
- Tampilkan data kucing yg berasal dari state `cats`

---
## 2.0 - Mencari Data

- Di dalam komponen `CatList`, tambahkan input text untuk melakukan pencarian. Setiap hasil ketikan akan di simpan pada state `input`
- Buat `useEffect()` baru yg berjalan ketika state `input` terjadi perubahan
- Di dalam `useEffect()`, lakukan filter pada state `catsTemp` yg sesuai dengan input.
- Hasil dari filter akan disimpan pada state `cats`


