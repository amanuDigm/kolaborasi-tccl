# kolaborasi-tccl

KOLABORATOR
1. Pada situs github fork dulu repo yang akan dijadikan proyek bersama (repo upstream)
 
2. Clone repo hasil fork kita ke lokal menggunakan terminal.
contoh perintah : git clone https://github.com/amanuDigm/kolaborasi-tccl.git
 
3. Hubungkan repo lokal dengan repo upstream dengan cara mengetikkan di terminal :  git remote add upstream https://github.com/amanuDigm/kolaborasi-tccl.git 
 
4. Untuk mengedit file di lokal pastikan membuat branch baru terlebih dahulu sesuai issue yang ada . Menggunakan perintah : 
git checkout -b namabranch	
 
5. Edit kode program ….

6. commit kode yang telah di edit dengan mengetikan perintah sebagai berikut : 
	git add .
	git commit -m “nama commit nya”
 
7. Kemudian push branch kita tadi ke repo origin dengan cara :  
	git push origin namabranch
 
8. Buka repository di github, lalu klik New Pull Request
 
9. Pilih opsi base fork ke master dan head form ke namabranch
 
10. Isikan keterangan lalu klik Create Pull Request
 
11. Tunggu Pull Request di Merge oleh upstream
 
12. Setelah di merge oleh upstream selanjutnya samakan branch master repo lokal dengan branch master repo upstream. Dengan cara : 
	git fetch upstream
	git checkout master
	git merge upstream/master
	git push origin master

