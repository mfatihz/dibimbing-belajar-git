Dibimbing.
AIML Batch 5.
Hands on Day 5 - GIT

Materi yang dipelajari:

mengaktifkan git bash cmd dan berpindah ke folder project

memeriksa nama dan email yang terhubung dengan akun github

git config --global user.name

git config --global user.email

Jika nama dan email belum terhubung dengan akun GitHub, daftarkan nama dan email dengan syntax sebagai berikut ini:

git config --global user.name "nama-user"

git config --global user.email "nama-email@email.xyz"

Langkah pertama adalah membuat repository git lokal

git init

git init akan menghasilkan hidden folder ".git"

git init dipakai jika project ada/dibuat di local tapi belum memiliki Git. Jika project diperoleh dari proses git clone, perintah git init tidak perlu dijalankan.

menambahkan file ke dalam Git staging area (Git staging area, atau index, adalah file yang menyimpan informasi apa saja yang akan dilakukan pada "commit" berikutnya)

git add "namafile.ext" perintah ini menambahkan file spesifik

git add . untuk menambahkan seluruh file dalam folder project, kecuali file-file yang dinyatakan dalam file .gitignore

Memeriksa status Git (working directory dan staging area)

git status

Menyimpan perubahan (history) secara local

git commit -m "komentar untuk commit ini..."

git commit mirip dengan "save point"!

Membuat remote repository dalam GitHub.com dan menghubungkan dengan repository lokal

buat dahulu repository dalam GitHub.com

Kemudian jalankan perintah berikut ini:

git branch -M main

git remote add origin <remote-URL>. Contoh url: https://github.com/<nama-user>/<nama-repsoitory.git>

lakukan setidaknya satu kali git commit lalu lakukan ...

git push -u origin main untuk memulai tracking

Membuat clone

pindahkan directory cmd ke directory project

git clone <url-yang-akan-diclone>

Membuat cabang (branch)

git branch memeriksa branch yang ada dan yang sedang aktif

git checkout -b "nama-branch" membuat branch baru (jika belum ada) dan sekaligus berpindah ke branch nama-branch" tersebut

git checkout "nama-branch" berpindah ke branch nama-branch" tersebut


Menggabungkan ranch

checkout ke branch yang akan dijadikan tempat penggabungan lalu

git merge "branch-yang-ingin-digabungkan"



mengupdate remote

git push
