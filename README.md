**Baca dengan teliti agar memahami dengan baik**

# penggunaan-git <img height="30" src="https://user-images.githubusercontent.com/25181517/192108372-f71d70ac-7ae6-4c0d-8395-51d8870c2ef0.png"> 

**informasi**
> _**penggunaan git untuk pemula dengan cara yang mudah, lebih pratis jika ingin dengan `mobiitas tinggi langsung menggunakan github.dev pada web browser atau menggunakan github.remote di visual studio code`**_

# Pertama `login user di terminal`

### `login untuk push` di `derektory local`

`clik kanan` dan pilih `open git bash hare` atau `buka git yang ada di pc/laptop` masukkan satu-satu :
```
git config --global user.name "username"
git config --global user.email "email@example.com"
```
### ini untuk local 
`click kanan pada folder yang ingiin di push tekan cari open git bash hare`
```
git config  user.name "username"
git config  user.email "email@example.com"
```
### `logout akun` di `derektory local`
```
git config --unset user.email "masukkan gmail"
git config --unset user.name "masukkan username"
```
# kedua `create dan push` file pertama kali
**langkah-langkah**
- `buat repositori` pada github terlebih dahulu
- buat menjadi `publik`
- buat `tanpa file readme.md`
- `buka terminal git` pada file project yang mau di uplod atau `buka terminal visual projek` yang di mau di oploud
masukkan perintah :
```
git init
```
selanjutnya jika semua file 
```
git add .
```
jika file tertentu
```
git add "nama_file"
```
selanjutnya
```
git commit -m "first commit"
git branch -M main
git remote add origin link_repositori_guthub_yang_sudah_di_buat
```
contoh `git remote` :
```
git remote add origin https://github.com/rusdy-cyber/penggunaan-git.git
```
selanjutnya
```
git push -u origin main
```


# ketiga jika ingin `update filenya` 

**langkah-langkah :**

> _`sebelum melakukan git push untuk update` di sarankan `melakukan git pull origin main` atau melakukan `gitu clone` agar file yang ada di repository local dan git sama, untuk menghindari `fatal eror`_

cara `rekomendasi` :
```
git remote add origin link_repository_github
git add .
git commit -m "update"
git push -u origin main
```
jika `terjadi eror` atau `sudah melakukan perubahan pada github di sarankan` berikut: 
```
git remote add origin link_repository_github
git pull origin main
git add .
git commit -m "update"
git push -u origin main
```
cara lain :
```
git remote add origin link_repository_github
git add .
git commit -m "update"
git branch -M main
git push -u origin main
```

<img height="30" src="https://user-images.githubusercontent.com/25181517/192108372-f71d70ac-7ae6-4c0d-8395-51d8870c2ef0.png">       <img height="30" src="https://user-images.githubusercontent.com/25181517/192108374-8da61ba1-99ec-41d7-80b8-fb2f7c0a4948.png">     <img height="30" src="https://user-images.githubusercontent.com/25181517/192107856-aa92c8b1-b615-47c3-9141-ed0d29a90239.png">     <img height="30" src="https://github.com/marwin1991/profile-technology-icons/assets/25181517/1275d076-f047-432b-9084-308f88f8c176">        <img height="30" src="https://user-images.githubusercontent.com/25181517/192108890-200809d1-439c-4e23-90d3-b090cf9a4eea.png">        <img height="30" src="https://user-images.githubusercontent.com/25181517/192108893-b1eed3c7-b2c4-4e1c-9e9f-c7e83637b33d.png">        <img height="30" src="https://user-images.githubusercontent.com/25181517/192108891-d86b6220-e232-423a-bf5f-90903e6887c3.png">
## penggunaan git lainnya 
## melihat akun yang terhubung 
```
git config --list
```
## melihat info repositori yang di remote
```
git remote -v
```
## membuat repositori baru di dalam folder local
```
git init nama-dir
```
[![Github all releases](https://img.shields.io/github/downloads/Naereen/StrapDown.js/total.svg)](https://GitHub.com/Naereen/StrapDown.js/releases/)  [![Github Releases (by release)](https://img.shields.io/github/downloads/Naereen/StrapDown.js/v1.0.0/total.svg)](https://GitHub.com/Naereen/StrapDown.js/releases/)
## meyalin repositori server ke local
```
git clone
```
## menambahkan file atau perubahan ke indeks (staging area) sebelum melakukan commit.
```
git add nama_file
```
## menyimpan perubahan Anda ke repositori lokal dengan pesan commit.
```
git commit
```
contoh :
```
git commit -m "Menambahkan file README.md"
```
## melihat status file dan perubahan Anda di repositori lokal Anda.
```
git status
```
## mengirimkan perubahan Anda ke repositori jarak jauh dan memperbarui cabang (branch) yang ditentukan.
```
git push -u origin master
```
## mengambil dan menggabungkan (merge) perubahan dari repositori jarak jauh ke repositori lokal Anda
```
git pull origin master
```
## membuat, menghapus, atau melihat cabang-cabang yang ada di repositori Anda.
```
git branch
```
contoh
```
$ git branch
* master
$ git branch fitur-baru
$ git branch
  fitur-baru
* master
$ git branch -d fitur-baru
Deleted branch fitur-baru (was f3a4b5c).
```
## beralih dari satu cabang ke cabang lain, atau untuk membatalkan perubahan lokal Anda.
```
git checkout
```
contoh :
```
$ git checkout fitur-baru
Switched to branch 'fitur-baru'
$ git checkout master
Switched to branch 'master'
$ git checkout -- index.html
```
## menggabungkan perubahan dari satu cabang ke cabang lain, atau untuk menyelesaikan konflik yang mungkin terjadi.
```
git merge
```
contoh :
```
$ git checkout fitur-baru
Switched to branch 'fitur-baru'
$ git checkout master
Switched to branch 'master'
$ git checkout -- index.html
```
## mengembalikan file, indeks, atau repositori Anda ke keadaan sebelumnya, atau untuk membatalkan perubahan yang tidak diinginkan.
```
git reset
```
contoh:
```
$ git reset --hard HEAD~1
HEAD is now at 9a1b2c3 Menambahkan file README.md
```
## mengatur atau melihat konfigurasi git Anda, seperti nama pengguna, email, editor, dll.
```
git config
```
contoh :
```
$ git config --global user.name "Petani Kode"
$ git config --global user.email petanikode@gmail.com
$ git config --list
user.name=Petani Kode
user.email=petanikode@gmail.com
```
