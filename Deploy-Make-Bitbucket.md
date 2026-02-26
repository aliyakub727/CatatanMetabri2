### ATM/CRM BITBUTCKET
Step By Step Push Atm Ke bitbucket

---

1. Inisiasi User
   Melakukan Login User yang ingin melakukan push kedalam bitbucket
   
   ```
   git config --global user.name "Muhamad Aulia Kartego"
   ```

   ```
   git config --global user.email "90169927@bri.co.id"
   ```

2. Membuat dan Berpindah Branch
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
3. Melihat Status & Log
   Lihat file yang diubah:

     ```
     git status
     ```
     
   Lihat riwayat commit:

     ```
     git log
     ```
     
4. Menambahkan File ke Staging Area
   Tambahkan semua file ke staging area:

     ```
     git add .
     ```
   Atau tambahkan file tertentu:

    ```  
     git add namafile.txt
    ``` 

5. Commit Perubahan
   Commit file yang sudah di-stage:

   ```  
   git commit -m "Pesan commit kamu"
   ```
   
6. Menghubungkan ke Repository Remote (seperti GitHub)
   Jika kamu belum menghubungkan repo lokal ke remote repo:

   ```  
   git remote add origin https://github.com/username/nama-repo.git
   ```
   
   Push ke Repository Remote
   untuk push pertama kali (misalnya ke main):

   ```
   git push -u origin main
   ```
   
   Setelah itu, cukup gunakan:

   ```
   git push
   ```  

---
Selesai
