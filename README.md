# Commit 1 Reflection Notes

Fungsi `handle_connection` bertugas untuk memproses koneksi TCP yang masuk dengan cara:
- Menerima `TcpStream` sebagai input.
- Menggunakan `bufReader` untuk meningkatkan efisiensi dari pembacaan data dari stream.
- Membagi dan membaca data baris per baris dan berhenti jika menemukan baris kosong (dalam HTTP berarti akhir dari header).
- Semua baris header disimpan di `Vec` dan di print ke terminal.
