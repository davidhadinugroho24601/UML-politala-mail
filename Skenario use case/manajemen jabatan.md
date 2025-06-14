Berikut adalah **tabel skenario lengkap** untuk fitur **Kelola Jabatan**, mencakup skenario tambah, edit, dan hapus jabatan beserta skenario alternatif:

---

### **Kelola Jabatan**

**Aktor:** Admin

| **Aksi Admin**                                   | **Reaksi Sistem**                                                        |
| ------------------------------------------------ | ------------------------------------------------------------------------ |
| **Skenario Normal – Tambah Jabatan**             |                                                                          |
| 1. Admin mengklik tombol "Tambah Jabatan".       |                                                                          |
|                                                  | 2. Sistem menampilkan form pengisian jabatan.                            |
| 3. Admin mengisi nama jabatan.                   |                                                                          |
|                                                  | 4. Sistem menyimpan data dan memperbarui daftar jabatan.                 |
|                                                  | 5. Sistem menampilkan notifikasi "Jabatan berhasil ditambahkan".         |
| **Skenario Alternatif – Tambah Jabatan**         |                                                                          |
| 3a. Admin tidak mengisi nama jabatan.            |                                                                          |
|                                                  | 4a. Sistem menampilkan pesan error (contoh: "Nama jabatan wajib diisi"). |
| **Skenario Normal – Edit Jabatan**               |                                                                          |
| 1. Admin memilih salah satu jabatan dari daftar. |                                                                          |
| 2. Admin mengklik tombol "Edit".                 |                                                                          |
|                                                  | 3. Sistem menampilkan form edit dengan data lama.                        |
| 4. Admin memperbarui nama jabatan.               |                                                                          |
|                                                  | 5. Sistem menyimpan perubahan dan memperbarui daftar.                    |
|                                                  | 6. Sistem menampilkan notifikasi "Jabatan berhasil diperbarui".          |
| **Skenario Alternatif – Edit Jabatan**           |                                                                          |
| 4a. Admin mengosongkan nama jabatan saat edit.   |                                                                          |
|                                                  | 5a. Sistem menampilkan pesan error (contoh: "Nama jabatan wajib diisi"). |
| **Skenario Normal – Hapus Jabatan**              |                                                                          |
| 1. Admin menghapus jabatan "Sekretaris".         |                                                                          |
|                                                  | 2. Sistem menampilkan dialog konfirmasi penghapusan.                     |
| 3. Admin mengonfirmasi penghapusan.              |                                                                          |
|                                                  | 4. Sistem menghapus jabatan dari basis data.                             |
|                                                  | 5. Sistem menampilkan notifikasi "Jabatan berhasil dihapus".             |

---

Siap digunakan dalam dokumen skripsi atau dijadikan file DOCX jika kamu mau. Silakan beri perintah selanjutnya.
