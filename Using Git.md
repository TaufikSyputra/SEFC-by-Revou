# How to use Git 
Disclamer: Tulisan ini dibuat berdasarkan pengalaman penulis dan masih banyak kekurangan

catatan: sudah install git di laptop

Cara Autentifikasi Git
1. cek Git yang sudah terdaftar dengan command berikut.
>git confing --list
Pada saat anda pertama kali menggunakan git dan belum pernah autentifikasi akun Git, maka tidak ada list git yang ditampilkan.

2. Autentifikasi akun git dengan command berikut.
> git config --global user.email "useremail@gmail.com"
> git config --global user.name "username github"

3. Memastikan repositori lokal sudah terhubung dengan remote. Perintah berikut ini akan menunjukkan URL dari remote yang terhubung.
> git remote -v

4. Menambahkan URL remot ke repositori lokal agar bisa terhubung dengan command
> git remote add origin <URL-Repository>
atau untuk mengubah URL remote yg sudah ada
> gi remote set-url origin <URL-Repository>

5. Melihat status repository git 
> git status

6. memeriksa remote branch yang tersedia
> git branch -r

7. memeriksa branch yang sedang dipakai. akan menampilkan semua branch lokal
> git branch

8. beralih ke branch lain
> git checkout <nama branch>

9. Menghapus branch
> git push origin --delete <nama branch>

10. Reset Branch Lokal (Hard Reset). melakukan hard reset pada branch akan menghapus seluruh file pada branch
> git checkout <nama branch>
> git reset --hard origin/nama branch
command berikut akan menghapus seluruh commit pada branch
> rm -rf

11. mengubah nama branch yang sedang aktif
> git branch -M <nama branch>

11. membuat commit baru
> git add . 
> git commit -m "Initial commit with no history"

12. Update dari lokal ke remote (push)
> git init (menginisialisasi repositori Git di direktori lokal. Ketika kamu menjalankan git init, Git akan membuat repositori Git baru di folder tersebut, yang memungkinkan kamu untuk mulai melacak perubahan pada file dalam direktori tersebut.)
> git add <nama file> atau git add . (untuk semua file)
> git commit -m "pesan commit"
> git push -u origin main (untuk pertama kali push, gunakan >git push untuk push selanjutnya )

13. update dari remote ke lokal (pull)
> git add <nama file>
> git commit -m "pesan commit"
> git pull origin main


