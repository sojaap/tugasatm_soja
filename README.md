## Dokumentasi

1. Opsi Ubah Pin pada Menu utama :
   Untuk pengubahan Pin dari akun yang digunakan untuk masuk ke dalam menu. Bila pin akun berubah maka saat verifikasi login pin yang dimasukkan juga akan berubah supaya bisa melanjutkan transaksi.

   Dengan menambahkan metode fungsi changePin() pada Account.java supaya user atau pengguna dapat mengganti pin milik mereka. Alur penggantian pin ini dilakukan dengan pengguna akan memasukkan pin sebelumnya, lalu konfirmasi pin dilakukan dengan memasukkan pinnya dua kali untuk memastikan pin yang dimasukkan adalah pin yang benar. Dilakukan pemisalan disini dengan dua kondisi. Kondisi pertama adalah saat pin dimasukan pengguna dengan pin sebelumnya, jika memenuhi kondisi akan diberikan output pin yang dimasukkan adalah pin yang sudah pernah dipakai artinya pin tidak akan dapat diganti dengan pin tersebut. Kondisi kedua ialah bila pin baru yang dimasukkan sama dengan pin baru kedua sebagai pemastian pin yang dimasukkan sama isinya maka kondisinya terpenuhi ddan penggantian pin baru akan dilakukan. Bila sebaliknya tidak memenuhi kondisi dan salah satu tidak sesuai maka outputnya akan menyatakan "PIN tidak sama, periksa kembali."

   Menu ini akan memanggil method yang ada pada file ATM.java tepatnya di case 5 yaitu ubah pin. Maka pengubahan pin bisa dilakukan melalui pilihan menu Ubah Pin.

2. Melakukan Verifikasi Akun :
   Verifikasi akun dilakukan setelah metode penggantian pin untuk memastikan pergantian pin berhasil dan terverifikasi agar dapat mengakses fitur transaksi di dalam sistem atm. Skema pada metode ini ialah memasukkan pin yang terbaru pada saat melakukan login dengan memasukkan kembali nomor akun dan pin terbaru, menggunakan 2 kondisi if else yang menyertakan input dari nomor akun beserta pinnya yang menyatakan bila pin yang dimasukkan saat login adalah benar maka transaksi dapat dilakukan dengan akun tersebut. bila tidak maka verfikasi akan gagal dan transaksi tidak bisa dilanjutkan atau di akses.

3. Menambahkan Saldo Minimal pada Akun (50.000) :
   Skema yang digunakan disini adalah kondisi dimana pengguna ingin menarik uang namun saldo yang ada dalam sistem harus menggunakan minimal saldo yang disisakan agar pengguna dapat mengetahui limit transaksi mereka.
   
   Pada file Account.java, dapat dilakukan penambahan private static final double MINIMUM_BALANCE - 50000, artinya nilai yang diset adalah nilai statik berupa angka dengan peran sebagai minimum saldo yang dipasang. Variable final disini digunakan untuk tujuan agar variable nilai didalamnya tidak akan dapat diubah setelah didefinisikan, karena hal ini akan membuat saldo minimumnya tetap dalam nilai konstan dan tidak berubah-ubah. MINIMUM_BALANCE digunakan dalam kelas withdrawal guna memastikan penarikan yang terjadi tidak akan melakukan pengurangan saldo yang melebihi saldo minimum yang telah ditentukan.

   Dalam eksekusinya di kelas withdrawal, program akan memeriksa jumlah penarikan yang diminta untuk dilakukan sudahakan sesuai dengan batas minimum saldo yang harus disimpan atau tidak. hal ini tidak memperbolehkan penarikan yang akan mengurangi saldo akun lebih rendah dari yang ditetapkan oleh MINIMUM_BALANCENYA. bila hal itu terjadi maka penarikan akan ditolak dengan mengirimkan pesan peringatan bahwa saldo yang disimpan tidak mencukupi untuk dilakukannya transaksi penarikan, sedangkan bila mencukupi maka saldo akan berkurang sesuai dengan penarikan yang diminta tapi tidak akan di bawah minimum saldo yang ada. Maka dengan adanya penetapan saldo minimum ini program dapat mencegah pengguna dari pengosongan saldo akun mereka di bawah batas minimum yang ditetapkan oleh sistem.
   

## Folder Structure

The workspace contains two folders by default, where:

- `src`: the folder to maintain sources
- `lib`: the folder to maintain dependencies

Meanwhile, the compiled output files will be generated in the `bin` folder by default.

> If you want to customize the folder structure, open `.vscode/settings.json` and update the related settings there.

## Dependency Management

The `JAVA PROJECTS` view allows you to manage your dependencies. More details can be found [here](https://github.com/microsoft/vscode-java-dependency#manage-dependencies).
