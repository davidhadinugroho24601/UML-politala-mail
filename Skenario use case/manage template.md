| **Aksi Admin**                                                                 | **Reaksi Sistem**                                                           |
| ------------------------------------------------------------------------------ | --------------------------------------------------------------------------- |
| **Skenario Normal – Tambah Template**                                          |                                                                             |
| 1. Admin masuk dan login ke sistem.                                            |                                                                             |
| 2. Admin memilih menu "Kelola Template Surat".                                 |                                                                             |
|                                                                                | 3. Sistem menampilkan daftar template surat yang tersedia.                  |
| 4. Admin mengklik tombol "Tambah Template".                                    |                                                                             |
|                                                                                | 5. Sistem menampilkan formulir pengisian template (nama, format, konten).   |
| 6. Admin mengisi data template sesuai form.                                    |                                                                             |
|                                                                                | 7. Sistem memvalidasi data template.                                        |
|                                                                                | 8. Sistem menyimpan template ke basis data.                                 |
|                                                                                | 9. Sistem menampilkan notifikasi "Template berhasil ditambahkan".           |
| 10. Admin melihat notifikasi keberhasilan.                                     |                                                                             |
| **Skenario Alternatif – Tambah Template**                                      |                                                                             |
| 6a. Admin mengisi form dengan data tidak valid (contoh: nama template kosong). |                                                                             |
|                                                                                | 7a. Sistem menampilkan pesan error (contoh: "Nama template wajib diisi").   |
| **Skenario Normal – Edit Template**                                            |                                                                             |
| 1. Admin membuka halaman "Kelola Template Surat".                              |                                                                             |
| 2. Admin memilih salah satu template dari daftar.                              |                                                                             |
| 3. Admin mengklik tombol "Edit".                                               |                                                                             |
|                                                                                | 4. Sistem menampilkan formulir edit dengan data template terisi sebelumnya. |
| 5. Admin memperbarui data template.                                            |                                                                             |
|                                                                                | 6. Sistem memvalidasi perubahan data.                                       |
|                                                                                | 7. Sistem menyimpan perubahan ke basis data.                                |
|                                                                                | 8. Sistem menampilkan notifikasi "Template berhasil diperbarui".            |
| 9. Admin melihat notifikasi keberhasilan.                                      |                                                                             |
| **Skenario Alternatif – Edit Template**                                        |                                                                             |
| 5a. Admin mengosongkan nama template saat edit.                                |                                                                             |
|                                                                                | 6a. Sistem menampilkan pesan error (contoh: "Nama template wajib diisi").   |
| **Skenario Normal – Hapus Template**                                           |                                                                             |
| 1. Admin membuka halaman "Kelola Template Surat".                              |                                                                             |
| 2. Admin mengklik tombol "Hapus" pada salah satu template.                     |                                                                             |
|                                                                                | 3. Sistem menampilkan dialog konfirmasi penghapusan.                        |
| 4. Admin mengonfirmasi penghapusan.                                            |                                                                             |
|                                                                                | 5. Sistem menghapus template dari basis data.                               |
|                                                                                | 6. Sistem menampilkan notifikasi "Template berhasil dihapus".               |
| 7. Admin melihat notifikasi keberhasilan.                                      |                                                                             |
