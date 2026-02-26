### Bitbucket Inisiasi

Inisiasi User
   ```
   git config --global user.name "Muhamad Aulia Kartego"
   ```
   ```
   git config --global user.email "90169927@bri.co.id"
   ```

Clone Dari Bitbucket

  ```
  git clone https://bitbucket.bri.co.id/scm/bup/new-crm.git
  ```

Pertamakali buat repo

  ```
  cd existing-project
  ```
  ```
  git init
  ```
  ```
  git add --all 
  ```
  ```
  git commit -m "Initial Commit"
  ```
 ```
 git remote add origin https://bitbucket.bri.co.id/scm/bup/new-crm.git
 ```
  ```
  git push -u origin HEAD:master
```

  Sudah ada file di repo
  
  ```
  cd existing-project
  ```
  ```
  git remote set-url origin https://bitbucket.bri.co.id/scm/bup/new-crm.git
  ```
  ```
  git push -u origin --all
  ```
  ```
  git push origin --tags
  ```

  ### Bitbucket Command

  1. Inisialisasi Repository
     Jika belum ada repositori git di folder proyek
     
     ```
     git init
     ```
     
  2. Menambahkan File ke Staging Area
     Tambahkan semua file ke staging area:
     
     ```
     git add .
     ```
     
     Atau tambahkan file tertentu:
     
     ```
     git add namafile.txt

     ```
     
  3. Commit Perubahan
     Commit file yang sudah di-stage:
     
     ```
     git commit -m "Pesan commit kamu"
     ```
     
  4. Menghubungkan ke Repository Remote (seperti GitHub)
     Jika kamu belum menghubungkan repo lokal ke remote repo:
     
     ```
     git remote add origin https://github.com/username/nama-repo.git
     ```
  5. Push ke Repository Remote

     Untuk push pertama kali (misalnya ke main):
     
     ```
     git push -u origin main
     ```

     Setelah itu, cukup gunakan:

     ```
     git push
     ```
     
  6. Menarik Perubahan dari Remote
     Untuk update lokal kamu dengan perubahan dari remote:

     ```
     git pull
     ```
    
  7. Melihat Status & Log
     Lihat file yang diubah:

     ```
     git status
     ```

     Lihat riwayat commit:

      ```
      git log
      ```
      
  8. Membuat dan Berpindah Branch
      Buat branch baru:

     ```
     git branch nama-branch
     ```

     Pindah ke branch itu:

     ```
     git checkout nama-branch
     ```

      Atau sekaligus buat dan pindah:

     ```
     git checkout -b nama-branch
     ```
     
  9. Menghapus Inisialisasi Git dari Folder (Lokal)
      Jika kamu ingin menghapus repo Git dari folder lokal (seperti tidak pernah di-git init), cukup hapus folder .git:

     ```
     rm -rf .git
     ```

     >⚠️ Ini akan menghapus semua riwayat Git, branch, commit, remote, dsb. Folder kamu tetap ada, tapi tidak lagi diatur oleh Git.
     
  10. Menghapus File dari Staging Area
      Jika kamu sudah git add file tapi belum commit, dan ingin membatalkannya:

      ```
      git reset nama_file.txt
      ```

      Atau untuk semua file:

      ```
      git reset
      ```
      
  11. Menghapus Commit Terakhir
      Untuk menghapus commit terakhir (tapi tidak menghapus file-nya):

      ```
      git reset --soft HEAD~1
      ```

      Jika ingin juga menghapus perubahan di file:

      ```
      git reset --hard HEAD~1
      ```
      
  12. Menghapus Remote Origin
      Jika kamu ingin menghapus koneksi ke GitHub atau remote repo:

      ```
      git remote remove origin
      ```
      
  13. Menghapus Branch
      Hapus branch lokal:

      ```
      git branch -d nama-branch
      ```
      
      Jika branch belum merge, paksa hapus:

      ```
      git branch -D nama-branch
      ```
      
  14. Lakukan merge

      ```
      git merge feature-login
      ```
      
  24. Jika Terjadi Konflik
      + Buka file yang konflik (ada tanda <<<<<<<, =======, >>>>>>>).
      + Pilih dan perbaiki isi file sesuai yang kamu inginkan.
      + Setelah selesai, tambahkan file itu ke staging
      + Lalu commit merge
