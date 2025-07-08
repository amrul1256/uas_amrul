# UAS Pengembangan Web – Debug REST API CI4
Nama: Muhammad Amrul Sihabbuddin 
Nim:231080200064
Kelas:4 B1 informatika 

## Tugas:
- Perbaiki minimal 5 bug dari aplikasi
- Catat bug dan solusinya dalam tabel laporan

### Laporan Bug
| No | File                     | Baris | Bug                        | Solusi                          |
|----|--------------------------|-------|-----------------------------|----------------------------------|
| 1 | app/config/Routes.php | 13 |route tidak memiliki filter otentikasi| Tambah ` ['filter' => 'jwt']
| 2 | app/config/Routes.php | 18 |Route users tidak konsisten dengan prefix api/| 'api/users',  |
| 3 | app/config/Routes.php | 35 |Filter salah di api/tasks |  ['filter' => 'jwt']|
| 4 | app/controller/auth.php |23|Tidak ada validasi input saat register | tambahkan validasi input|
| 5 | app/controller/auth.php |16|Password tidak di-hash |$password = password_hash|

- POST /login
- POST /register
- GET /users (token diperlukan)
