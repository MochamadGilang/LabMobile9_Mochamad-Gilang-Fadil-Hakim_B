## TAMPILAN AWAL
![WhatsApp Image 2024-11-11 at 22 56 05_2d1f3f64](https://github.com/user-attachments/assets/e49eb5ba-3458-4ede-8ccb-bdabc1347b46)

## CREATE
![WhatsApp Image 2024-11-11 at 22 55 57_13de3f95](https://github.com/user-attachments/assets/c9512cf3-5e10-4f6d-97c6-08f464223cee)
![WhatsApp Image 2024-11-12 at 17 41 48_aed36169](https://github.com/user-attachments/assets/baf33b94-2bda-40e9-a764-e100c5a406be)
Fungsi tambahMahasiswa() bertugas memeriksa apakah input nama dan jurusan telah diisi. Jika keduanya tidak kosong, data tersebut dikemas dalam objek dan dikirim ke endpoint API tambah.php menggunakan metode POST melalui ApiService. Jika permintaan sukses, modal akan ditutup, data akan di-reset, dan fungsi getMahasiswa() akan dipanggil untuk memperbarui daftar mahasiswa. Jika terjadi kesalahan, pesan error akan ditampilkan.

## EDIT
![WhatsApp Image 2024-11-12 at 17 42 23_9e32c327](https://github.com/user-attachments/assets/59382b49-cbb5-4198-9020-993e085a64a9)
Fungsi editMahasiswa() digunakan untuk mengedit data mahasiswa. Sebelum proses pengeditan, pengguna membuka modal edit dengan memanggil fungsi openModalEdit dan memasukkan data mahasiswa yang sudah ada. Setelah data baru dimasukkan, objek data dibuat dengan properti id, nama, dan jurusan. Data tersebut kemudian dikirim ke endpoint API edit.php menggunakan metode POST atau PUT. Jika permintaan berhasil, modal akan ditutup, data di-reset, dan fungsi getMahasiswa() akan dipanggil untuk memperbarui daftar mahasiswa yang telah diubah. Jika terjadi kesalahan, pesan error akan ditampilkan

# DELETE
![WhatsApp Image 2024-11-12 at 17 58 01_d7124d80](https://github.com/user-attachments/assets/ebcfd69a-ecfb-4100-88f0-f644bc32a226)
Fungsi ini dimulai dengan menampilkan pesan konfirmasi penghapusan menggunakan window.confirm untuk memastikan bahwa pengguna benar-benar berniat menghapus data tersebut. Jika pengguna mengonfirmasi tindakan ini, fungsi akan mengirimkan permintaan ke API endpoint hapus.php dengan menyertakan id mahasiswa yang akan dihapus. Setelah penghapusan berhasil, fungsi getMahasiswa() akan dipanggil untuk memperbarui daftar mahasiswa. Jika ada kesalahan yang terjadi, pesan error akan ditampilkan.

