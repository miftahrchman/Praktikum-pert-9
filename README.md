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




def hitung_nilai_akhir(tugas, uts, uas):
    return (tugas * 0.3) + (uts * 0.35) + (uas * 0.35)

def main():
    daftar_mahasiswa = []
    
    while True:
        nama = input("Masukkan nama mahasiswa: ")
        nim = input("Masukkan NIM mahasiswa: ")
        tugas = float(input("Masukkan nilai tugas: "))
        uts = float(input("Masukkan nilai UTS: "))
        uas = float(input("Masukkan nilai UAS: "))
        
        nilai_akhir = hitung_nilai_akhir(tugas, uts, uas)
        
        mahasiswa = {
            "nama": nama,
            "nim": nim,
            "tugas": tugas,
            "uts": uts,
            "uas": uas,
            "nilai_akhir": nilai_akhir
        }
        
        daftar_mahasiswa.append(mahasiswa)
        
        tanya = input("Apakah Anda ingin menambah data? (y/t): ")
        if tanya.lower() == 't':
            break
    
    # Menampilkan daftar mahasiswa dalam format tabel
    print("\nDaftar Mahasiswa:")
    print(f"{'Nama':<20} {'NIM':<15} {'Tugas':<10} {'UTS':<10} {'UAS':<10} {'Nilai Akhir':<15}")
    print("=" * 80)
    
    for mhs in daftar_mahasiswa:
        print(f"{mhs['nama']:<20} {mhs['nim']:<15} {mhs['tugas']:<10} {mhs['uts']:<10} {mhs['uas']:<10} {mhs['nilai_akhir']:<15.2f}")

if __name__ == "__main__":
    main()
