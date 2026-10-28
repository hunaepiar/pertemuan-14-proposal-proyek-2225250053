PROPOSAL PROYEK PROGRAM SEDERHANA

Identitas Mahasiswa

- Nama: Khunaepi
- NIM: 2225250053
- Jenis Pengerjaan: Individu

1. Judul Proyek

Program Rekap dan Analisis Nilai Matematika Kelas.

2. Latar Belakang

Pengolahan nilai siswa membutuhkan ketelitian, terutama ketika jumlah siswa cukup banyak. Perhitungan rata-rata, pencarian nilai tertinggi dan terendah, serta penentuan kelulusan secara manual dapat memerlukan waktu lebih lama.

Oleh karena itu, dirancang program sederhana menggunakan Python untuk membantu proses rekapitulasi dan analisis nilai matematika siswa.

3. Tujuan Proyek

1. Membaca data nilai siswa dari file.
2. Memvalidasi nilai pada rentang 0 sampai 100.
3. Menghitung rata-rata, nilai tertinggi, dan nilai terendah.
4. Menentukan status kelulusan berdasarkan KKM.
5. Menyimpan laporan hasil analisis.

4. Pengguna dan Manfaat

Pengguna yang dituju adalah guru atau pihak yang membutuhkan rekap nilai matematika siswa. Program diharapkan dapat membantu mempercepat perhitungan nilai dan mengurangi kesalahan perhitungan manual.

5. Ruang Lingkup

Fitur yang dirancang

- Membaca data nilai dari file teks.
- Memvalidasi data nilai.
- Menghitung rata-rata nilai.
- Menentukan nilai tertinggi dan terendah.
- Menentukan status kelulusan.
- Menyimpan laporan ke file teks.

Batasan

- Program berjalan melalui terminal.
- Menggunakan Python.
- Nilai harus berada pada rentang 0–100.
- KKM rancangan awal ditetapkan sebesar 60.
- Program tidak menggunakan database, GUI, atau web.

6. Kebutuhan Program

Kebutuhan fungsional

1. Program dapat membaca data siswa.
2. Program dapat memeriksa validitas nilai.
3. Program dapat menghitung rata-rata nilai.
4. Program dapat mencari nilai tertinggi dan terendah.
5. Program dapat menentukan status kelulusan.
6. Program dapat menyimpan laporan.

Kebutuhan nonfungsional

1. Program mudah digunakan.
2. Program memiliki struktur modul yang jelas.
3. Program menampilkan pesan kesalahan jika data tidak valid.
4. Program menghasilkan laporan yang mudah dibaca.

7. Rancangan Input, Process, Output (IPO)

Input

- Nama siswa.
- Nilai matematika.
- File data nilai.

Process

1. Membaca data.
2. Memeriksa format data.
3. Memvalidasi rentang nilai.
4. Menghitung rata-rata.
5. Menentukan nilai tertinggi dan terendah.
6. Membandingkan nilai siswa dengan KKM.

Output

- Daftar nilai yang valid.
- Rata-rata kelas.
- Nilai tertinggi dan terendah.
- Status kelulusan siswa.
- File laporan.

8. Pseudocode

MULAI

Baca file data nilai.

JIKA file tidak ditemukan:
Tampilkan pesan kesalahan.

JIKA file ditemukan:
Periksa setiap data siswa.
Validasi nilai antara 0 dan 100.
Tandai data yang tidak valid.

Jika terdapat nilai valid:
    Hitung rata-rata nilai.
    Cari nilai tertinggi.
    Cari nilai terendah.

    Untuk setiap siswa:
        Jika nilai >= KKM:
            Status = Lulus.
        Jika nilai < KKM:
            Status = Belum Lulus.

    Tampilkan hasil analisis.
    Simpan hasil ke file laporan.

SELESAI

9. Rancangan Struktur Program

pertemuan-14-proposal-proyek-2225250053/
├── README.md
├── proposal.md
├── .gitignore
├── data/
│   └── nilai_contoh.txt
├── src/
│   ├── main.py
│   ├── data_io.py
│   ├── analisis.py
│   └── utilitas.py
├── tests/
│   └── test_case.md
└── output/

Fungsi setiap modul

- "main.py": mengatur jalannya program.
- "data_io.py": membaca data dan menyimpan laporan.
- "analisis.py": menghitung statistik dan status kelulusan.
- "utilitas.py": menyediakan fungsi pendukung.

10. Rancangan Data

Data siswa dirancang menggunakan dictionary dengan atribut nama dan nilai.

Contoh:

{
    "nama": "Ani",
    "nilai": 80
}

Data siswa dapat dikumpulkan dalam sebuah list.

11. Rancangan Pengujian

Kode| Skenario| Data| Hasil yang Diharapkan
TC01| Nilai normal| 80, 70, 90| Rata-rata 80
TC02| Nilai minimum| 0| Diterima
TC03| Nilai maksimum| 100| Diterima
TC04| Nilai melebihi batas| 105| Ditolak
TC05| File tidak ditemukan| File tidak tersedia| Pesan kesalahan
TC06| Semua nilai memenuhi KKM| 70, 80, 90| Semua lulus
TC07| Nilai bukan angka| abc| Data tidak valid
TC08| Nilai sama dengan KKM| 60| Status lulus

Catatan: KKM 60 merupakan asumsi untuk rancangan awal.

12. Tahapan Pengerjaan Individu

1. Menentukan masalah dan tujuan proyek.
2. Menentukan kebutuhan dan batasan.
3. Menyusun IPO dan pseudocode.
4. Merancang struktur program.
5. Menyusun skenario pengujian.
6. Menyelesaikan dokumentasi.
7. Mengunggah berkas ke GitHub.

13. Repository GitHub

URL repository: [https://github.com/hunaepiar/pertemuan-14-proposal-proyek-2225250053.git]

14. Kesimpulan

Program Rekap dan Analisis Nilai Matematika Kelas dirancang untuk membantu pengolahan nilai siswa secara terstruktur. Rancangan mencakup kebutuhan program, IPO, pseudocode, struktur modul, data, dan pengujian awal. Seluruh perancangan proyek dikerjakan secara individu sebagai persiapan implementasi pada pertemuan berikutnya.