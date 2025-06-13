## Tabel Pengujian Blackbox - Fitur Pengguna dan Admin

Dokumen ini mencakup seluruh skenario pengujian blackbox (termasuk skenario positif dan negatif) untuk fitur-fitur yang dapat diakses oleh aktor **Pengguna** maupun **Admin** dalam sistem manajemen surat, digabungkan dalam satu tabel.

| No   | Peran    | Fitur             | Langkah Pengujian                     | Input                    | Ekspektasi Output                        | Catatan                                   |
| ---- | -------- | ----------------- | ------------------------------------- | ------------------------ | ---------------------------------------- | ----------------------------------------- |
| 1.1  | Pengguna | Backup Database   | Klik tombol "Backup Database"         | Klik                     | Proses pencadangan dimulai               | Tampilan loading atau progres             |
| 1.2  | Pengguna | Backup Database   | Proses backup selesai                 | -                        | Notifikasi sukses muncul                 | File tersimpan otomatis atau bisa diunduh |
| 1.3  | Pengguna | Backup Database   | Gagal mencadangkan                    | Gangguan koneksi         | Tampilkan error "Gagal melakukan backup" | Validasi kesalahan sistem                 |
| 2.1  | Pengguna | Verifikasi Surat  | Akses menu "Verifikasi Surat"         | Klik                     | Form verifikasi muncul                   | Input untuk file atau ID surat            |
| 2.2  | Pengguna | Verifikasi Surat  | Input surat valid                     | ID/file sah              | Surat diverifikasi, notifikasi sukses    | Validasi server-side                      |
| 2.3  | Pengguna | Verifikasi Surat  | Input surat tidak valid               | ID/file tidak sah        | Notifikasi gagal verifikasi              | Jelaskan alasan penolakan                 |
| 2.4  | Pengguna | Verifikasi Surat  | Input kosong                          | Kosong                   | Tampilkan pesan "ID surat wajib diisi"   | Validasi form                             |
| 3.1  | Pengguna | Baca Surat Masuk  | Akses menu "Surat Masuk"              | Klik                     | Tabel daftar surat muncul                | Termasuk status, pengirim, dan tanggal    |
| 3.2  | Pengguna | Baca Surat Masuk  | Klik surat yang tidak tersedia        | ID salah                 | Tampilkan pesan "Surat tidak ditemukan"  | Validasi ID                               |
| 4.1  | Pengguna | Setujui Surat     | Akses surat dengan status "Menunggu"  | Surat valid              | Tombol "Setujui" tersedia                | Hak akses harus tersedia                  |
| 4.2  | Pengguna | Setujui Surat     | Klik tombol "Setujui"                 | Klik                     | Surat berubah jadi status "Disetujui"    | Notifikasi sukses muncul                  |
| 4.3  | Pengguna | Setujui Surat     | Setujui surat yang sudah ditolak      | Surat status "Ditolak"   | Tampilkan pesan error                    | Tidak boleh bisa disetujui lagi           |
| 5.1  | Pengguna | Revisi Surat      | Akses surat yang perlu direvisi       | Klik                     | Tombol "Revisi" tersedia                 | Input catatan harus muncul                |
| 5.2  | Pengguna | Revisi Surat      | Kirim revisi tanpa catatan            | Kosong                   | Tampilkan error "Catatan wajib diisi"    | Validasi form                             |
| 5.3  | Pengguna | Revisi Surat      | Kirim revisi dengan catatan           | Komentar jelas           | Status surat berubah ke "Direvisi"       | Histori dicatat                           |
| 6.1  | Pengguna | Tolak Surat       | Klik tombol "Tolak"                   | Klik                     | Muncul dialog alasan penolakan           | Isian wajib diisi                         |
| 6.2  | Pengguna | Tolak Surat       | Kirim penolakan dengan alasan         | Teks alasan              | Status surat menjadi "Ditolak"           | Notifikasi sukses                         |
| 6.3  | Pengguna | Tolak Surat       | Tolak surat yang disetujui            | Surat status "Disetujui" | Tampilkan error "Tidak dapat ditolak"    | Validasi status                           |
| 7.1  | Pengguna | Kirim Draft Surat | Akses daftar draft surat              | Klik                     | Tabel draft muncul                       | Tampilkan subjek, tanggal, tujuan         |
| 7.2  | Pengguna | Kirim Draft Surat | Klik tombol "Kirim"                   | Klik                     | Status surat jadi "Terkirim"             | Notifikasi sukses                         |
| 7.3  | Pengguna | Kirim Draft Surat | Kirim draft tanpa isi/lampiran wajib  | Draft kosong             | Tampilkan error validasi                 | Tidak boleh terkirim                      |
| 8.1  | Admin    | Manage Users      | Tambah pengguna baru                  | Form lengkap             | Pengguna ditambahkan ke sistem           | Validasi input                            |
| 8.2  | Admin    | Manage Users      | Edit data pengguna                    | Form dengan perubahan    | Perubahan tersimpan                      | Data diperbarui                           |
| 8.3  | Admin    | Manage Users      | Hapus pengguna                        | Klik konfirmasi          | Pengguna dihapus                         | Konfirmasi diperlukan                     |
| 8.4  | Admin    | Manage Users      | Tambah pengguna dengan email duplikat | Email sudah terdaftar    | Tampilkan error                          | Validasi duplikat                         |
| 9.1  | Admin    | Manage Group      | Tambah grup baru                      | Form grup                | Grup tersimpan                           | Nama grup unik                            |
| 9.2  | Admin    | Manage Group      | Tambah anggota ke grup                | Pilih pengguna dan grup  | Anggota ditambahkan                      | Validasi ganda                            |
| 9.3  | Admin    | Manage Group      | Tambah anggota tanpa memilih pengguna | Kosong                   | Tampilkan error "Pilih pengguna"         | Validasi input                            |
| 10.1 | Admin    | Manage Division   | Tambah divisi                         | Nama divisi              | Divisi ditambahkan                       | Nama tidak boleh kosong                   |
| 10.2 | Admin    | Manage Division   | Tetapkan grup ke divisi               | Pilih grup dan divisi    | Grup terhubung ke divisi                 | Perlu hak akses                           |
| 11.1 | Admin    | Manage Template   | Tambah template surat                 | Nama dan isi template    | Template disimpan                        | Bisa digunakan ulang                      |
| 11.2 | Admin    | Manage Template   | Edit template                         | Isi diubah               | Perubahan tersimpan                      | Tersedia versi terbaru                    |
| 11.3 | Admin    | Manage Template   | Hapus template                        | Klik hapus               | Template dihapus                         | Konfirmasi diminta                        |
| 11.4 | Admin    | Manage Template   | Tambah template tanpa nama            | Kosong                   | Tampilkan pesan "Nama template wajib"    | Validasi form                             |
| 12.1 | Admin    | Manage Kode Surat | Tambah kode surat                     | Kode dan deskripsi       | Kode tersimpan                           | Kode harus unik                           |
| 12.2 | Admin    | Manage Kode Surat | Edit kode surat                       | Perbarui deskripsi       | Tersimpan dengan sukses                  | Validasi isi                              |
| 12.3 | Admin    | Manage Kode Surat | Hapus kode surat                      | Klik hapus               | Kode dihapus                             | Harus tidak terpakai aktif                |
| 12.4 | Admin    | Manage Kode Surat | Tambah kode surat kosong              | Kosong                   | Tampilkan error                          | Validasi input                            |
| 13.1 | Admin    | Manage Sent Mails | Baca surat terkirim                   | Klik surat               | Isi surat ditampilkan                    | Termasuk lampiran                         |
| 13.2 | Admin    | Manage Sent Mails | Baca draft                            | Klik draft               | Draft dibuka untuk edit                  | Bisa dikirim ulang                        |
| 13.3 | Admin    | Manage Sent Mails | Hapus draft                           | Klik hapus               | Draft dihapus                            | Konfirmasi diperlukan                     |
| 13.4 | Admin    | Manage Sent Mails | Kirim draft tanpa isi                 | Draft kosong             | Tampilkan pesan kesalahan                | Validasi wajib                            |

**Catatan Umum:**

* Tabel ini mencakup uji skenario positif (fungsi berjalan sesuai harapan) dan skenario negatif (input salah atau situasi gagal).
* Fokus pada pengujian masukan dan keluaran sistem (blackbox), tanpa mempertimbangkan implementasi internal.
* Validasi hak akses, integritas data, dan pesan kesalahan menjadi bagian penting dari skenario uji.
