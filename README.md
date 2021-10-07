# pemweb-test-tg1

Repo ini berisi kumpulan tugas yang diberikan saat kelas.

|   |   |
| - | - |
| Nama | Andhika Wibawa |
| NIM | 119140218 |
| Kelas | PemWeb-RA |

## Instruksi Penggunaan Git

1. Pastikan Git telah terpasang dan terdeteksi pada `PATH`. Pastikan juga repo online Github sudah terbuat (atau buatlah jika belum)

2. Buat folder kosong terlebih dahulu (misal `D:\Koding\Pemweb`)

3. Buka Terminal atau PowerShell atau Command Prompt (tekan `` Ctrl + ` `` bila menggunakan VSCode)

4. Ubah direktori ke `D:\Koding\Pemweb` dengan perintah:

   ```shell
   cd "D:\Koding\Pemweb"
   ```

   Ganti `cd` dengan `pushd` bila terdapat error. **Alternatif:** Gunakan `Open Folder...` pada VSCode, maka `workdir` akan menyesuaikan

5. Inisialisasi repository kosong (lokal) pada folder `D:\Koding\Pemweb` dengan perintah:

   ```shell
   git init
   ```

6. Tambahkan repository online Github yang saya anggap telah dibuat dengan perintah:

   ```shell
   git remote add <alias-repo> <link-repo>
   ```

   Misal, pada repository ini yaitu `git remote add pemweb-dhika https://github.com/AndhikaWB/pemweb-test-tg1.git` (nama alias repo bebas)

7. Download revisi terakhir suatu `branch` (berisi kumpulan source code) pada repo:

   ```shell
   git pull <alias-repo> <nama-branch>
   ```

   Misal, pada repository ini yaitu `git pull pemweb-dhika master` (branch utama biasanya `master` atau `main`)

8. Setelah kumpulan file source code pada suatu branch selesai di download, kita dapat memodifikasi file-file tersebut

9. Setelah modifikasi file dirasa cukup layak, gunakan perintah ini agar semua perubahan tercatat pada Git:

   ```shell
   git add -A
   ```

10. Bila sudah yakin terdapat perubahan tersebut, kita dapat menambahkan revisi baru dari branch disertai pesan revisi dengan perintah berikut:

    ```shell
    git commit -m "<pesan-revisi>"
    ```

    Misal pada repository ini yaitu `git commit -m "Memperbarui deskripsi file README.md"` (tanda kutip dua wajib ditulis bila terdapat spasi pada pesan). **Note:** jangan terlalu sering commit hal yang tidak penting karena history pesan revisi nantinya akan terkesan berantakan

11. Untuk menggunggah hasil commit kembali ke repository online Github, gunakan perintah:

    ```shell
    git push <alias-repo> <nama-branch>
    ```

    Misal, pada repository ini yaitu `git push pemweb-dhika master`. **Note:** bila mendapat peran member atau kontributor jangan asal push apalagi ke repository orang lain. Tidak semua repository diaktifkan mekanisme review perubahan (sehingga perubahan akan langsung masuk tanpa proses review terlebih dahulu)

12. Cek perubahan dengan mengunjungi repository online Github. Misal pada repo ini yaitu `https://github.com/AndhikaWB/pemweb-test-tg1`

13. **Tambahan:** Untuk berganti/menambah branch, dapat digunakan perintah:

    ```shell
    git checkout -b <nama-branch>
    ```

    **Note:** Untuk mengunggah branch baru tersebut (dari lokal) ke repo online Github dapat diulang kembali langkah 8 dst. **Note 2:** Bila branch sudah ada pada repo online sebelumnya (hanya berganti branch, bukan sekaligus membuat branch baru), disarankan menggunakan `git pull <alias-repo> <nama-branch>` untuk mengunduh data file pada branch tersebut terlebih dahulu (sebelum melakukan modifikasi)
