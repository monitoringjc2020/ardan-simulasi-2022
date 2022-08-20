# Dokumentasi Simulasi Linux Administration 2022

## Membuat repository di github
Apabila belum punya account di github maka bisa mendaftar dengan email masing-masing, tambahkan ssh key sehingga memudahkan saat pull dan push ke github.
Caranya sebagai berikut:
```
ardan@ardan-X8DTU:~/Documents/github.com$ cat ~/.ssh/id_rsa.pub 
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQD2vn9zvan3Z5r47Tjr08w5wbN0uKC8tz78+GbLHk9na+OPBKtFVr2kvil4LbyJW+2WgWgKpd/CAKRc3QY4Tv1DGT2sTB0jAxb7T/Y9Z4n15RdDWV7ixvVgFX67z9/1FFULUG9ehGbiLi7xqeJUA0JWezDiyzl/DCzojBmOtu7w45XeWxdfflr7GIm+xYC6/BX3BoIYS0/S8wDu4fjXE2/g/oWTOPviG6qrYNYUOyunJxpBAxWI9++yWNg6gOnderTjP8vOD15nota8rovCtzei2nc0UBEPpDGLNSe8JWtPFbgkGnrSlpN+D0RHzdlFvPNZjUca2bnU3gF+EtijtFaz ardan@ardan-X8DTU
ardan@ardan-X8DTU:~/Documents/github.com$ 
```

Langkah selanjutnya membuat repository dan clone repository tersebut ke lokal.
```
ardan@ardan-X8DTU:~/Documents/github.com$ git clone git@github.com:monitoringjc2020/ardan-simulasi-2022.git
Cloning into 'ardan-simulasi-2022'...
remote: Enumerating objects: 13, done.
remote: Counting objects: 100% (13/13), done.
remote: Compressing objects: 100% (12/12), done.
remote: Total 13 (delta 2), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (13/13), 6.74 KiB | 6.74 MiB/s, done.
Resolving deltas: 100% (2/2), done.
ardan@ardan-X8DTU:~/Documents/github.com$ mkdocs new ardan-simulasi-2022
INFO    -  Writing config file: ardan-simulasi-2022/mkdocs.yml 
INFO    -  Writing initial docs: ardan-simulasi-2022/docs/index.md 
ardan@ardan-X8DTU:~/Documents/github.com$ cd ardan-simulasi-2022
ardan@ardan-X8DTU:~/Documents/github.com/ardan-simulasi-2022$ ls -l
total 24
drwxrwxr-x 2 ardan ardan  4096 Agu 20 11:25 docs
-rw-rw-r-- 1 ardan ardan 11357 Agu 20 11:25 LICENSE
-rw-rw-r-- 1 ardan ardan    19 Agu 20 11:25 mkdocs.yml
-rw-rw-r-- 1 ardan ardan   456 Agu 20 11:25 README.md
ardan@ardan-X8DTU:~/Documents/github.com/ardan-simulasi-2022$ 
```

Membuat halaman dokumentasi dalam folder docs dengan nama dokumentasi-simulasi.md seperti contoh halaman ini untuk isi dari dokumentasi yang sudah dibuat.
Nantinya setelah perubahan file markdown ini maka bisa di push ke github dengan urutan perintah berikut:
```
git add .
git commit -m "komentar tentang apa yang di push"
git push origin main
```