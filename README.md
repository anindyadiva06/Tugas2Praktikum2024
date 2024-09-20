# Tugas Pertemuan 2
Penjelasan

Dalam FormData, setiap TextField dilengkapi dengan TextEditingController yang berfungsi untuk mengambil teks dari input pengguna. Ada tiga `TextEditingController` yang digunakan:
1. _namaController untuk mengelola nama.
2. _nimController untuk mengelola NIM.
3. _tahunController untuk mengelola tahun lahir.

Metode _textboxNama(), _textboxNIM(), dan _textboxTahun() menghubungkan controller tersebut dengan widget TextField. Ketika tombol "Simpan" diklik, data diambil dari setiap controller dengan menggunakan .text dan kemudian diproses. Dalam proyek ini, Navigator.of(context).push digunakan untuk beralih ke tampilan baru (`TampilData`) dan mengirimkan data sebagai parameter.

Data yang dikumpulkan dikirim ke tampilan TampilData melalui konstruktor TampilData. Konstruktor ini menerima data dan menyimpannya dalam variabel final berikut:
1. final String nama;
2. final String nim;
3. final int tahun;

Di dalam TampilData, data yang diterima digunakan untuk menampilkan informasi kepada pengguna. Contohnya, umur dihitung berdasarkan tahun lahir dan ditampilkan dalam teks.

## Screenshot

![image](https://github.com/user-attachments/assets/77192c2c-6f33-4113-8427-3ad4222364f6)
![image](https://github.com/user-attachments/assets/896e04f2-d002-4277-9704-bf920add0aee)



