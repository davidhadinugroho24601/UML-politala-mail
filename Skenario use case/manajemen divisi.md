Berikut adalah **tabel skenario lengkap** untuk fitur **Kelola Divisi**, dilengkapi dengan **skenario normal, alternatif, edit, dan hapus**:

---

### **Kelola Divisi**

**Aktor:** Admin

| **Aksi Admin**                                | **Reaksi Sistem**                                                       |
| --------------------------------------------- | ----------------------------------------------------------------------- |
| **Skenario Normal – Tambah Divisi**           |                                                                         |
| 1. Admin mengklik "Tambah Divisi".            |                                                                         |
|                                               | 2. Sistem menampilkan form pengisian.                                   |
| 3. Admin mengisi nama divisi.                 |                                                                         |
|                                               | 4. Sistem menyimpan data dan memperbarui daftar divisi.                 |
|                                               | 5. Sistem menampilkan notifikasi "Divisi berhasil ditambahkan".         |
| **Skenario Alternatif – Tambah Divisi**       |                                                                         |
| 3a. Admin mengosongkan kolom nama divisi.     |                                                                         |
|                                               | 4a. Sistem menampilkan pesan error (contoh: "Nama divisi wajib diisi"). |
| **Skenario Normal – Edit Divisi**             |                                                                         |
| 1. Admin memilih divisi dari daftar.          |                                                                         |
| 2. Admin mengklik tombol "Edit".              |                                                                         |
|                                               | 3. Sistem menampilkan form edit dengan data lama.                       |
| 4. Admin memperbarui nama divisi.             |                                                                         |
|                                               | 5. Sistem menyimpan perubahan dan memperbarui daftar.                   |
|                                               | 6. Sistem menampilkan notifikasi "Divisi berhasil diperbarui".          |
| **Skenario Alternatif – Edit Divisi**         |                                                                         |
| 4a. Admin mengosongkan nama divisi saat edit. |                                                                         |
|                                               | 5a. Sistem menampilkan pesan error (contoh: "Nama divisi wajib diisi"). |
| **Skenario Normal – Hapus Divisi**            |                                                                         |
| 1. Admin mengklik tombol "Hapus" pada divisi. |                                                                         |
|                                               | 2. Sistem menampilkan dialog konfirmasi penghapusan.                    |
| 3. Admin mengonfirmasi penghapusan.           |                                                                         |
|                                               | 4. Sistem menghapus divisi dari basis data.                             |
|                                               | 5. Sistem menampilkan notifikasi "Divisi berhasil dihapus".             |

---

Silakan lanjutkan ke fitur berikutnya atau beri tahu jika ingin semua skenario ini digabung dalam satu dokumen.
