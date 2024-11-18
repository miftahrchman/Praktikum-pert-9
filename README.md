# Praktikum-pert-9
Tugas Praktikum

Buat program sederhana untuk menambahkan data kedalam sebuah
list dengan rincian sebagai berikut:
• Progam meminta memasukkan data sebanyak-banyaknya (gunakan
perulangan)
• Tampilkan pertanyaan untuk menambah data (y/t?), apabila jawaban
t (Tidak), maka program akan menampilkan daftar datanya. • Nilai Akhir diambil dari perhitungan 3 komponen nilai (tugas: 30%,
uts: 35%, uas: 35%)
• Buat flowchart dan penjelasan programnya

MENJALANKAN PROGRAM
![Program](https://github.com/user-attachments/assets/c73377f7-fe6f-4e46-8fb6-d2ddceeea9bd)

HASIL PROGRAM
![Hasil program 1](https://github.com/user-attachments/assets/2dc1446a-a194-4ef3-901e-92375e15e40f)
![Hasil program 2](https://github.com/user-attachments/assets/18da5f01-cd2d-444c-a490-eb127418ba40)

PENJELASAN PROGRAM

Program ini bertujuan untuk mengumpulkan data mahasiswa, termasuk nama, NIM, nilai tugas, UTS, dan UAS, serta menghitung nilai akhir berdasarkan bobot yang telah ditentukan. Setelah data dimasukkan, program akan menampilkan semua data mahasiswa dalam format tabel.
Langkah-langkah Program:

    Fungsi hitung_nilai_akhir:
        Menerima nilai tugas, UTS, dan UAS sebagai parameter.
        Menghitung nilai akhir berdasarkan rumus: [ \text{Nilai Akhir} = (0.3 \times \text{Tugas}) + (0.35 \times \text{UTS}) + (0.35 \times \text{UAS}) ]

    Fungsi main:
        Membuat list kosong daftar_mahasiswa untuk menyimpan data mahasiswa.
        Memasuki loop untuk meminta input dari pengguna:
            Meminta nama mahasiswa, NIM, nilai tugas, UTS, dan UAS.
            Menghitung nilai akhir menggunakan fungsi hitung_nilai_akhir.
            Menyimpan data mahasiswa dalam bentuk dictionary dan menambahkannya ke daftar_mahasiswa.
            Menanyakan kepada pengguna apakah ingin menambah data lagi.
        Setelah pengguna memilih untuk tidak menambah data, program akan menampilkan semua data mahasiswa dalam format tabel.

    Menampilkan Data:
        Menampilkan header tabel.
        Menggunakan loop untuk mencetak setiap data mahasiswa dengan format yang rapi.

FLOWCHART


![image](https://github.com/user-attachments/assets/0fa8d88a-087f-4a2a-94c3-b98c60077b5b)


