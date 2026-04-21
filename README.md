# Commit 1 Reflection Notes

Fungsi `handle_connection` bertugas untuk memproses koneksi TCP yang masuk dengan cara:
- Menerima `TcpStream` sebagai input.
- Menggunakan `bufReader` untuk meningkatkan efisiensi dari pembacaan data dari stream.
- Membagi dan membaca data baris per baris dan berhenti jika menemukan baris kosong (dalam HTTP berarti akhir dari header).
- Semua baris header disimpan di `Vec` dan di print ke terminal.

# Commit 2 Reflection Notes

Pada milestone 2, hal yang saya pelajari dari kode baru di fungsi `handle_connection`:
- Pada milestone 1, kita hanya menerima/mengambil data dari browser. Pada milestone ini, kita memberikan response dengan mengirim hello.html
- Kita kirim dengan status 200 OK. variable `response` berguna sebagai formatting ke dalam bentuk HTTP Response.

![Commit 2 screen capture](image.png)