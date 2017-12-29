# kolaborasi-tccl

### Nama Anggota Kelompok
- 145410034 Tri Hargianto		(colaborator)
- 145410073 Erwin Robbi P 	(colaborator)
- 135410203 Amanu Alatibi		(upstream)


### Step by step KOLABORATOR
1. Pada situs github fork dulu repo yang akan dijadikan proyek bersama (repo upstream)

2. Clone repo hasil fork kita ke lokal menggunakan terminal.
contoh perintah :
```bash
git clone https://github.com/amanuDigm/kolaborasi-tccl.git
```

3. Hubungkan repo lokal dengan repo upstream dengan cara mengetikkan di terminal :  
```bash
git remote add upstream https://github.com/amanuDigm/kolaborasi-tccl.git
```

4. Untuk mengedit file di lokal pastikan membuat branch baru terlebih dahulu sesuai issue yang ada . Menggunakan perintah :
```bash
git checkout -b namabranch
```
5. Edit kode README.md program

6. commit kode yang telah di edit dengan mengetikan perintah sebagai berikut :
```bash
- git add .
- git commit -m “nama commit nya”
  ```

7. Kemudian push branch kita tadi ke repo origin dengan cara :  
```bash
git push origin namabranch
```

8. Buka repository di github, lalu klik New Pull Request

9. Pilih opsi base fork ke __master__ dan head form ke __namabranch__

10. Isikan keterangan lalu klik __Create Pull Request__

11. Tunggu Pull Request di Merge oleh upstream

12. Setelah di merge oleh upstream, pastikan branch yang berisikan commit yang telah di merge oleh upstream dihapus di github dan repo lokal.
 - Untuk menghapus branch pada github bisa klik Delete Branch
 - Untuk menghapus branch pada repo lokal dengan terminal ketikkan :
```bash
git checkout master
git branch -d namabranch
```

13. Setelah di merge oleh upstream selanjutnya samakan branch master repo lokal dengan branch master repo upstream. Dengan cara :
```bash
	git fetch upstream
	git checkout master
	git merge upstream/master
	git push origin master
```

### Step by Step Upstream
1. Klik Pull Request jika ada pull request
2. Klik item yang ada
3. Jika terdapat Konflik maka klik tombol Resolve Conflicts
![alt tag](https://raw.githubusercontent.com/amanuDigm/kolaborasi-tccl/master/screen/Selection_002.png)
4. Edit/Hapus kode supaya tidak conflict
![alt tag](https://raw.githubusercontent.com/amanuDigm/kolaborasi-tccl/master/screen/Selection_003.png)
5. Selanjutnya klik Mark as Resolved jika sudah selesai editnya
![alt tag](https://raw.githubusercontent.com/amanuDigm/kolaborasi-tccl/master/screen/Selection_004.png)
6. Setelah itu Commit Changes
7. Setelah di commit , selanjutnya klik tombol Merge Pull Request untuk menggabungkan source code ke branch master
![alt tag](https://raw.githubusercontent.com/amanuDigm/kolaborasi-tccl/master/screen/Selection_005.png)
