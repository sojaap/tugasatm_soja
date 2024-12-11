## Dokumentasi

1. Opsi Ubah Pin pada Menu utama :
   Untuk pengubahan Pin dari akun yang digunakan untuk masuk ke dalam menu. Bila pin akun berubah maka saat verifikasi login pin yang dimasukkan juga akan berubah supaya bisa melanjutkan transaksi.

   Dengan menambahkan metode fungsi changePin() pada Account.java supaya user atau pengguna dapat mengganti pin milik mereka. Alur penggantian pin ini dilakukan dengan pengguna akan memasukkan pin sebelumnya, lalu konfirmasi pin dilakukan dengan memasukkan pinnya dua kali untuk memastikan pin yang dimasukkan adalah pin yang benar. Dilakukan pemisalan disini dengan dua kondisi. Kondisi pertama adalah saat pin dimasukan pengguna dengan pin sebelumnya, jika memenuhi kondisi akan diberikan output pin yang dimasukkan adalah pin yang sudah pernah dipakai artinya pin tidak akan dapat diganti dengan pin tersebut.

2.

## Folder Structure

The workspace contains two folders by default, where:

- `src`: the folder to maintain sources
- `lib`: the folder to maintain dependencies

Meanwhile, the compiled output files will be generated in the `bin` folder by default.

> If you want to customize the folder structure, open `.vscode/settings.json` and update the related settings there.

## Dependency Management

The `JAVA PROJECTS` view allows you to manage your dependencies. More details can be found [here](https://github.com/microsoft/vscode-java-dependency#manage-dependencies).
