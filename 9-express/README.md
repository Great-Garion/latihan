# Express

## Simple CRUD

Buatlah sebuah API dengan data dan ketentuan berikut

- Data user memiliki beberapa properti
  ```
  {
    id, 
    name
    email, 
    username, 
    password, 
  }
  ```

- `GET` `/user` 
  
  mendapatkan semua data user

- `GET` `/user/:username` 

  mendapatkan data user berdasarkan username. Jika username tidak ditemukan, berikan sebuah response `user not found`.

- `POST` `/user` 

  menambahkan data user baru. Jika username sudah ada, berikan sebuah response `user already exist`

- `DELETE` `/user/:username`

  Hapus data user berdasarkan username. Jika username tidak ditemukan, berikan sebuah response `user not found`. Jika berhasil di hapus, beri response `user has been deleted`

- `PUT` `/user/:username`
  
  Update data user berdasarkan username. Jika username tidak ditemukan, berikan sebuah response `user not found`. Jika berhasil di edit, beri response `user has been updated`
