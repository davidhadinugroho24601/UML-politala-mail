Terima kasih, berikut adalah **tabel skenario lengkap untuk fitur Verifikasi Surat**, disesuaikan dengan penjelasan bahwa sistem akan **memeriksa apakah surat (PDF) yang diunggah berasal dari sistem ini**. Fitur ini dapat diakses oleh **semua jenis pengguna**.

---

### **Verifikasi Surat**

**Aktor:** Semua (Dosen, Tendik, Admin)

| **Aksi Pengguna**                                        | **Reaksi Sistem**                                                                              |
| -------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **Skenario Normal – Verifikasi Surat**                   |                                                                                                |
| 1. Pengguna membuka menu "Verifikasi Surat".             |                                                                                                |
| 2. Pengguna mengunggah file surat (PDF).                 |                                                                                                |
|                                                          | 3. Sistem memeriksa file PDF yang diunggah, mencari kode tersembunyi / identitas unik.         |
|                                                          | 4. Jika ditemukan dan valid, sistem menampilkan status "Surat valid dan terverifikasi".        |
|                                                          | 5. Sistem menampilkan informasi surat (judul, tanggal, penerbit, dsb).                         |
| **Skenario Alternatif – Surat Tidak Valid**              |                                                                                                |
| 3a. Sistem tidak menemukan kode yang sesuai dalam surat. |                                                                                                |
|                                                          | 4a. Sistem menampilkan status "Surat tidak valid / tidak dikeluarkan oleh sistem".             |
| **Skenario Alternatif – Format Tidak Didukung**          |                                                                                                |
| 2a. Pengguna mengunggah file bukan PDF.                  |                                                                                                |
|                                                          | 3a. Sistem menampilkan pesan error "Format file tidak didukung, hanya PDF yang diperbolehkan." |

---

Jika kamu ingin, saya bisa gabungkan semua skenario yang sudah kita buat sebelumnya ke dalam satu file `.docx`. Silakan beri instruksi selanjutnya!
