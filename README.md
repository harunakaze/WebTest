TugasWebBro
===========
git init = untuk meng-initialize Git repository
git status = untuk melihat status projek kita
	contoh : apakah ada file baru yang dibuat

git add <namafile> = untuk menambahkan <namafile> ke staging area agar bisa di commit
	bisa juga dengan perintah "git add -A ." dimana semua file pada directory tersebut (ditandai dengan titik) akan dimasukan ke staging area.
	-A berarti memastikan bahwa file yang dibuang juga termasuk daftar yang akan diurus di staging area.
	Kita juga bisa menggunakan wildcard (Contoh : '*.txt' <- mencari semua file dengan extensi .txt) pada <namafile> untuk mempermudah proses penambahan.

git reset <namafile> = untuk mengeluarkan file dari staging area.

git commit -m "PESAN COMMIT" = untuk melakukan commit, dimana -m "PESAN COMMIT" merupakan deskripsi dari apa yang kita commit.

git log = menampilkan history commit yang kita lakukan

git remote <remote name> <URL repository> = untuk menamnbahkan remote repository di server github.

git push = untuk meng-push dari local repository kita ke server github.
	-u <remote name> <branch name> bisa ditambahkan untuk mempermudah proses push di masa yang akan datang.

git pull <remote name> <branch name> = untuk meng-pull dari remote repository ke local repository.

git diff [parameter] = untuk melihat perbedaan apa yang dilakukan per commit
	HEAD bisa digunakan dalam parameter, untuk melihat perbedaan pada commit terbaru
	<SHA> bisa digunakan dalam parameter, dimana isi <SHA> adalah SHA commit yang ingin dilihat
	--staged bisa digunakan dalam parameter, untuk melihat perbedaan pada staging area

git branch <nama branch> = untuk membuat branch/meng-copy dari master repository, yang nanti bisa digabung kembali.
	-d <nama branch> juga bisa digunakan untuk membuang <nama branch> (Biasa dipakai setelah proses merging), -f bisa digunakan untuk force deleting.

git checkout <nama branch> = untuk pindah branch ke <nama branch>
	kita juga bisa membuat dan langsung pindah ke suatu branch baru dengan command : git checkout -b <nama branch>
	-- <nama file> bisa digunakan untuk mengembalikan file pada keadaan commit terakhir (Undo)

git rm <nama file> = untuk membuang <nama file> dan secara langsung dicatat di staging area, jika tidak automatis di catat di staging area, pada saat commit kita bisa menggunakan "git commit -a" untuk menyertakan file yang telah terbuang/terhapus.
	-r <nama folder> bisa digunakan untuk membuang suatu folder beserta isinya secara langsung.

git merge <nama branch> = untuk menggabungkan dua buah branch menjadi satu branch.	
