# Git 

## Instalasi Git

### Guide Line Instalasi Git
https://docs.google.com/document/d/1g1Gh6oPnaRGno22VgFaSlcK_4cZxwwZ0/edit?usp=sharing&ouid=110024865534755627848&rtpof=true&sd=true

Setelah instalasi selesai jalankan command berikut dalam Command Prompt untuk Windows dan Terminal bagi Mac.
```powershell
git --version
```

Apabila instalasi berhasil maka command tersebut akan menunjukkan git versi berapa yang sudah terinstall di PC kalian, seperti pada gambar berikut.

![[Pasted image 20221215213827.png]]

## Konfigurasi Git

Pertama2 kita harus melakukan konfigurasi akun git terlebih dahulu, kalian dapat menggunakkan akun Github kalian untuk melanjutkan proses ini.

```powershell
# Command
git config --global user.name [username] 
git config --global user.email [isi@email.com]

# Misal username github anda mecoder
# Misal email github anda coder@gmail.com
# Contoh
git config --global user.name mecoder
git config --global user.email coder@gmail.com

# Untuk melihat akun yang sudah terdaftar dalam Git
git config --global --list
```

## How To Make an Online Repository (github.com)

1.  Buka github kalian di [github.com](http://github.com)

3.  Klik button new (warna hijau)
	![[Pasted image 20221215214012.png]]

3. Ketik nama repository yang kalian inginkan dan tentukan apakah repository ini bisa diakses secara public atau private
	![[Pasted image 20221215214050.png]]

4. Jika sudah terisi semua, klik create repository

## Let's Git Started
Sekarang buatlah satu folder yang akan digunakkan untuk mulai meng-_initialize_ git, dan buka Command Prompt / Terminal dalam folder tersebut.s

Cara membuka Command Prompt / Terminal dalam suatu folder.

-   Untuk Windows : [](https://www.lifewire.com/open-command-prompt-in-a-folder-5185505)[https://www.lifewire.com/open-command-prompt-in-a-folder-5185505](https://www.lifewire.com/open-command-prompt-in-a-folder-5185505)
-   Untuk Mac : [](https://www.maketecheasier.com/launch-terminal-current-folder-mac/)[https://www.maketecheasier.com/launch-terminal-current-folder-mac/](https://www.maketecheasier.com/launch-terminal-current-folder-mac/)

Menggunakkan command "cd" untuk menavigasikan Command Prompt ke folder yang diinginkan

-   [](https://www.howtogeek.com/659411/how-to-change-directories-in-command-prompt-on-windows-10/)[https://www.howtogeek.com/659411/how-to-change-directories-in-command-prompt-on-windows-10/](https://www.howtogeek.com/659411/how-to-change-directories-in-command-prompt-on-windows-10/)

#### Membuat Local Repository (git init)
```powershell
#Command
git init
```

#### Menambahkan File (git add)
```powershell
#Command
git add .
#digunain untuk nambahin semua file untuk di commit

git add [nama file]
#digunain untuk nambah satu file spesifik

#Misal nama file yang ingin ditambah home.css
#Contoh
git add home.css
```

#### Menyimpan Perubahan (git commit)
```powershell
#Command
git commit -m "[pesan commitnya]"

#Misal abis koding nambahin section contactus
#Contoh
git commit -m "added contactus section"
```

#### Menyambungkan Local Repo —> Remote Repo(Repository Github) (git remote)
```powershell
#Command
git remote add origin [link_repo_taro_sini]
git branch -M [nama_branch]

#Contoh
git remote add origin https://github.com/joshuajevon/training-git.git
git branch -M main
```
Link repo bisa didapat dari gambar yang terlampir dibawah ini
![[Pasted image 20221215214452.png]]

#### Meng-upload Local Repository ke Github (git push)
```powershell
#Command
git push -u origin main
#Melakukan upload dari local ke remote repo ke dalam branch main
#Command ini dilakukan apabila kalian melakukan init git di local terlebih dahulu

#Atau biasanya kalian hanya perlu menjalankan command ini
git push
```

#### Add Collaborator
1.  Langkah pertama adalah mendapatkan username dari calon kolaborator. Apabila belum memiliki username, maka harus terlebih dahulu mendaftar melalui link berikut “[Signing up for a new GitHub account](https://help.github.com/en/articles/signing-up-for-a-new-github-account)“.
    
2.  Silahkan mengakses halaman utama dari repository pada GitHub.
    
3.  Klik tombol **Settings** yang terdapat di bawah nama repository name.
	![[Pasted image 20221215214548.png]]
	
4. Klik link **Collaborators** yang tampil pada menu di bagian kiri
	![[Pasted image 20221215214643.png]]
	Menu Collaborators untuk berbagi repository Github ke kolaborator
	
5. Klik add people
	![[Pasted image 20221215214718.png]]
	
6.  Ketik username dari calon kolaborator sehingga muncul username yang sesuai
	![[Pasted image 20221215214754.png]]
	
7. Klik **Add Collaborator** untuk menambahkan user sebagai kolaborator.
	![[Pasted image 20221215214837.png]]
	Add Collaborator untuk berbagi repository Github
	
8.  Kolaborator akan mendapatkan email notifikasi yang berisi link untuk konfirmasi. Apabila konfirmasi dilakukan maka calon kolaborator tersebut akan menjadi kolaborator dan dapat mengakses repository yang terkait.
	![[Pasted image 20221215214919.png]]
	

#### Meng-clone Repository dari Github (git clone)
```powershell
#Command
git clone [link_repo_taro_sini]

#Contoh
git clone https://github.com/joshuajevon/training-git.git
```
Dapet link repo dari mana?

Pastikan link repository yang diambil itu yang HTTPS sesuai gambar yang terlampir
![[Pasted image 20221215215022.png]]

#### Mendapatkan perubahan terbaru dalam repository (git pull)
```powershell
#Command
git pull
```

#### Conflict yang mungkin terjadi saat menggunakkan git
- Push Error
	Error dimana saat kita ingin melakukan push ke repository
	![[Pasted image 20221215215153.png]]
	
- Pull Error
	Error dimana saat kita ingin melakukan pull ke codingan kita, dengan kondisi dimana repository online memiliki perbedaan codingan dengan remote local repository.
	![[Pasted image 20221215215215.png]]

