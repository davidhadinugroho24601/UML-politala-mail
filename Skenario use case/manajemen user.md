Baik! Berikut adalah **tabel skenario akhir untuk fitur Kelola Pengguna**, **tanpa opsi nonaktifkan**, hanya mencakup **tambah, edit, hapus**, dan **skenario alternatif**:

---

### **Kelola Pengguna**

**Aktor:** Admin

| **Aksi Admin**                                             | **Reaksi Sistem**                                                 |
| ---------------------------------------------------------- | ----------------------------------------------------------------- |
| **Skenario Normal – Tambah Pengguna**                      |                                                                   |
| 1. Admin mengklik tombol "Tambah Pengguna".                |                                                                   |
|                                                            | 2. Sistem menampilkan form input data pengguna.                   |
| 3. Admin mengisi form pengguna (nama, email, peran, dll).  |                                                                   |
|                                                            | 4. Sistem memvalidasi dan menyimpan data pengguna.                |
|                                                            | 5. Sistem menampilkan notifikasi "Pengguna berhasil ditambahkan". |
| **Skenario Alternatif – Tambah Pengguna**                  |                                                                   |
| 3a. Admin mengosongkan kolom wajib (misal: email kosong).  |                                                                   |
|                                                            | 4a. Sistem menampilkan pesan error (contoh: "Email wajib diisi"). |
| **Skenario Normal – Edit Pengguna**                        |                                                                   |
| 1. Admin memilih pengguna dari daftar.                     |                                                                   |
| 2. Admin mengklik tombol "Edit".                           |                                                                   |
|                                                            | 3. Sistem menampilkan form edit dengan data pengguna.             |
| 4. Admin memperbarui data pengguna.                        |                                                                   |
|                                                            | 5. Sistem menyimpan perubahan dan memperbarui daftar.             |
|                                                            | 6. Sistem menampilkan notifikasi "Pengguna berhasil diperbarui".  |
| **Skenario Alternatif – Edit Pengguna**                    |                                                                   |
| 4a. Admin menghapus isi email saat edit.                   |                                                                   |
|                                                            | 5a. Sistem menampilkan pesan error (contoh: "Email wajib diisi"). |
| **Skenario Normal – Hapus Pengguna**                       |                                                                   |
| 1. Admin mengklik tombol "Hapus" pada salah satu pengguna. |                                                                   |
|                                                            | 2. Sistem menampilkan konfirmasi penghapusan.                     |
| 3. Admin mengonfirmasi penghapusan.                        |                                                                   |
|                                                            | 4. Sistem menghapus pengguna dari basis data.                     |
|                                                            | 5. Sistem menampilkan notifikasi "Pengguna berhasil dihapus".     |

---

Silakan lanjutkan ke fitur berikutnya atau minta penggabungan semua skenario dalam satu dokumen jika diperlukan.
