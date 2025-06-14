

### **Kelola Format Kode Surat**

**Aktor:** Admin

| **Aksi Admin**                                          | **Reaksi Sistem**                                                       |
| ------------------------------------------------------- | ----------------------------------------------------------------------- |
| **Skenario Normal – Tambah Kode**                       |                                                                         |
| 1. Admin menambahkan kode baru.                         |                                                                         |
|                                                         | 2. Sistem memvalidasi dan menyimpan kode.                               |
|                                                         | 3. Sistem menampilkan notifikasi "Kode berhasil ditambahkan".           |
| **Skenario Alternatif – Tambah Kode**                   |                                                                         |
| 1a. Admin mengisi data kode tidak valid (misal kosong). |                                                                         |
|                                                         | 2a. Sistem menampilkan pesan error (contoh: "Kode tidak boleh kosong"). |
| **Skenario Normal – Edit Kode**                         |                                                                         |
| 1. Admin memilih salah satu kode dari daftar.           |                                                                         |
| 2. Admin mengklik tombol "Edit".                        |                                                                         |
|                                                         | 3. Sistem menampilkan form edit dengan data terisi.                     |
| 4. Admin memperbarui kode.                              |                                                                         |
|                                                         | 5. Sistem memvalidasi dan menyimpan perubahan.                          |
|                                                         | 6. Sistem menampilkan notifikasi "Kode berhasil diperbarui".            |
| **Skenario Alternatif – Edit Kode**                     |                                                                         |
| 4a. Admin mengosongkan kolom saat edit.                 |                                                                         |
|                                                         | 5a. Sistem menampilkan pesan error (contoh: "Kode tidak boleh kosong"). |
| **Skenario Normal – Hapus Kode**                        |                                                                         |
| 1. Admin mengklik tombol "Hapus" pada salah satu kode.  |                                                                         |
|                                                         | 2. Sistem menampilkan dialog konfirmasi penghapusan.                    |
| 3. Admin mengonfirmasi penghapusan.                     |                                                                         |
|                                                         | 4. Sistem menghapus kode dari basis data.                               |
|                                                         | 5. Sistem menampilkan notifikasi "Kode berhasil dihapus".               |

---


