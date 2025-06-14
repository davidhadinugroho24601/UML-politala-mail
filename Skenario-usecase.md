Berikut adalah **format skenario use case** untuk semua daftar use case yang telah Anda berikan sebelumnya, menggunakan struktur tabel yang konsisten:

---

### **1. Login**  
**Aktor:** Semua Pengguna  

| **Aksi Pengguna**            | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Pengguna membuka halaman login. |                                                                                  |
| 2. Pengguna memasukkan email dan password. |                                                                                  |
|                                | 3. Sistem memvalidasi kredensial.                                               |
|                                | 4. Jika valid, sistem mengarahkan ke halaman pemilihan role.                    |
| **Skenario Alternatif**      |                                                                                  |
| 2a. Pengguna memasukkan password salah. |                                                                                  |
|                                | 3a. Sistem menampilkan pesan error: "Email atau password salah".                |

---

### **2. Pilih Role untuk Masuk**  
**Aktor:** Semua Pengguna  

| **Aksi Pengguna**            | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Pengguna memilih role (Admin/Dosen/Tendik). |                                                                                  |
|                                | 2. Sistem mengarahkan ke dashboard sesuai role.                                 |
| **Skenario Alternatif**      |                                                                                  |
| 1a. Pengguna tidak memilih role. |                                                                                  |
|                                | 2a. Sistem menampilkan pesan: "Silakan pilih role terlebih dahulu".              |

---

### **3. Kelola Template Surat** *(Contoh sudah diberikan sebelumnya)*  
**Aktor:** Admin  
Berikut adalah format yang Anda minta untuk **Skenario Use Case "Kelola Template Surat"** (sesuai dengan daftar use case sebelumnya), dengan struktur yang konsisten seperti contoh yang diberikan:

---

### **Use Case: Kelola Template Surat**  
**Aktor:** Admin  

| **Aksi Admin**               | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Admin masuk dan login ke sistem. |                                                                                  |
| 2. Admin memilih menu "Kelola Template Surat". |                                                                                  |
|                                | 3. Sistem menampilkan daftar template surat yang tersedia.                       |
| 4. Admin mengklik tombol "Tambah Template". |                                                                                  |
|                                | 5. Sistem menampilkan formulir pengisian template (nama, format, konten).        |
| 6. Admin mengisi data template sesuai form. |                                                                                  |
|                                | 7. Sistem memvalidasi data template.                                             |
|                                | 8. Sistem menyimpan template ke basis data.                                      |
|                                | 9. Sistem menampilkan notifikasi "Template berhasil ditambahkan".                |
| 10. Admin melihat notifikasi keberhasilan. |                                                                                  |
| **Skenario Alternatif**      |                                                                                  |
| 6a. Admin mengisi form dengan data tidak valid (contoh: format kosong). |                                                                                  |
|                                | 7a. Sistem mendeteksi kesalahan dan menampilkan pesan error (contoh: "Format wajib diisi"). |

---

### **Penjelasan:**  
1. **Skenario Normal**:  
   - Admin berhasil menambahkan template surat setelah mengisi form dengan data valid.  
   - Sistem menyimpan data dan memberikan konfirmasi.  

2. **Skenario Alternatif**:  
   - Jika ada kesalahan input (misal: kolom wajib kosong), sistem akan menolak penyimpanan dan menampilkan pesan error.  

---

### **Catatan:**  
- Format ini bisa diterapkan untuk use case lain (misal: *Kelola Kode Surat*, *Kirim Surat*) dengan menyesuaikan **aksi admin/pengguna** dan **reaksi sistem**.  
- Tambahkan **skenario alternatif** lain jika diperlukan (contoh: edit/hapus template, atau akses ditolak untuk role non-admin).  

Jika Anda ingin contoh untuk use case lainnya, beri tahu saya!
---

### **4. Kelola Kode Surat**  
**Aktor:** Admin  

| **Aksi Admin**               | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Admin memilih menu "Kelola Kode Surat". |                                                                                  |
|                                | 2. Sistem menampilkan daftar kode surat.                                        |
| 3. Admin mengedit format kode. |                                                                                  |
|                                | 4. Sistem menyimpan perubahan dan menampilkan notifikasi "Berhasil diperbarui". |

---

### **5. Kelola Daftar Kode**  
**Aktor:** Admin  

| **Aksi Admin**               | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Admin menambahkan kode baru. |                                                                                  |
|                                | 2. Sistem memvalidasi dan menyimpan kode.                                       |

---

### **6. Kelola Golongan Pengguna**  
**Aktor:** Admin  

| **Aksi Admin**               | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Admin menambahkan golongan baru (contoh: "Staf"). |                                                                                  |
|                                | 2. Sistem menyimpan data dan memperbarui daftar.                                |

---

### **7. Kelola Divisi**  
**Aktor:** Admin  

| **Aksi Admin**               | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Admin mengklik "Tambah Divisi". |                                                                                  |
|                                | 2. Sistem menampilkan form pengisian.                                           |
| 3. Admin mengisi nama divisi. |                                                                                  |
|                                | 4. Sistem menyimpan data.                                                       |

---

### **8. Kelola Jabatan**  
**Aktor:** Admin  

| **Aksi Admin**               | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Admin menghapus jabatan "Sekretaris". |                                                                                  |
|                                | 2. Sistem menampilkan konfirmasi penghapusan.                                   |

---

### **9. Kelola Pengguna**  
**Aktor:** Admin  

| **Aksi Admin**               | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Admin menonaktifkan akun pengguna. |                                                                                  |
|                                | 2. Sistem mengupdate status akun.                                               |

---

### **10. Kelola Draft Surat**  
**Aktor:** Dosen/Tendik  

| **Aksi Pengguna**            | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Dosen memilih "Buat Draft Surat". |                                                                                  |
|                                | 2. Sistem membuka editor surat.                                                 |
| 3. Dosen menyimpan draft.    |                                                                                  |
|                                | 4. Sistem menyimpan draft dan menampilkan notifikasi.                           |

---

### **11. Kirim Surat**  
**Aktor:** Dosen/Tendik  

| **Aksi Pengguna**            | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Pengguna mengklik "Kirim Surat". |                                                                                  |
|                                | 2. Sistem memvalidasi kelengkapan surat.                                        |
|                                | 3. Sistem mengirim surat dan memberi notifikasi.                                |

---

### **12. Lihat Surat Terkirim**  
**Aktor:** Dosen/Tendik  

| **Aksi Pengguna**            | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Pengguna membuka menu "Surat Terkirim". |                                                                                  |
|                                | 2. Sistem menampilkan daftar surat terkirim.                                    |

---

### **13. Lihat Surat Masuk**  
**Aktor:** Dosen/Tendik  

| **Aksi Pengguna**            | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Pengguna membuka menu "Surat Masuk". |                                                                                  |
|                                | 2. Sistem menampilkan daftar surat masuk.                                       |

---

### **14. Revisi Surat Masuk**  
**Aktor:** Dosen/Tendik  

| **Aksi Pengguna**            | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Pengguna memilih surat dan klik "Revisi". |                                                                                  |
|                                | 2. Sistem membuka editor revisi.                                                |

---

### **15. Tolak Surat Masuk**  
**Aktor:** Dosen/Tendik  

| **Aksi Pengguna**            | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Pengguna mengklik "Tolak Surat". |                                                                                  |
|                                | 2. Sistem meminta alasan penolakan.                                             |

---

### **16. Setujui Surat Masuk**  
**Aktor:** Dosen/Tendik  

| **Aksi Pengguna**            | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Pengguna mengklik "Setujui". |                                                                                  |
|                                | 2. Sistem mengubah status surat menjadi "Disetujui".                            |

---

### **17. Verifikasi Surat**  
**Aktor:** Semua  

| **Aksi Pengguna**            | **Reaksi Sistem**                                                                 |
|------------------------------|----------------------------------------------------------------------------------|
| **Skenario Normal**          |                                                                                  |
| 1. Pengguna memeriksa surat dan klik "Verifikasi". |                                                                                  |
|                                | 2. Sistem menandai surat sebagai "Terverifikasi".                               |

---

### **Catatan:**  
- Setiap use case memiliki **skenario normal** (alur ideal) dan **alternatif** (penanganan error/pengecualian).  
- Untuk menghemat ruang, skenario alternatif tidak selalu ditampilkan secara lengkap, tetapi dapat ditambahkan sesuai kebutuhan (contoh: validasi gagal, akses ditolak, dll).  

Jika Anda memerlukan penyesuaian atau penambahan detail tertentu, beri tahu saya!