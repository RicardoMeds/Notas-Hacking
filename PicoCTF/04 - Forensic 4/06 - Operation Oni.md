#### - **Descripción** 
Descargue esta imagen de disco, busque la clave e inicie sesión en la máquina remota.Nota: si está usando el shell web, descargue y extraiga la imagen del disco en un `/tmp`directorio que no sea su directorio de inicio.

Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.

- [Download disk image](https://artifacts.picoctf.net/c/69/disk.img.gz)
- Remote machine: `ssh -i key_file -p 64732 ctf-player@saturn.picoctf.net`
- 
**Pista**

#### - **Solución** 
richi@RicardoMedina:~/tmp$ fls -o 206848 disk.img 470
r/r 2344:       .ash_history
d/d 3916:       .ssh
richi@RicardoMedina:~/tmp$ fls -o 206848 disk.img 3916
r/r 2345:       id_ed25519
r/r 2346:       id_ed25519.pub
richi@RicardoMedina:~/tmp$ fls -o 206848 disk.img 2345
Error extracting file from image (ext2fs_dir_open_meta: Error reading directory contents: 2345
)
richi@RicardoMedina:~/tmp$ icat -o 206848 disk.img 2345
-----BEGIN OPENSSH PRIVATE KEY-----
b3BlbnNzaC1rZXktdjEAAAAABG5vbmUAAAAEbm9uZQAAAAAAAAABAAAAMwAAAAtzc2gtZW
QyNTUxOQAAACBgrXe4bKNhOzkCLWOmk4zDMimW9RVZngX51Y8h3BmKLAAAAJgxpYKDMaWC
gwAAAAtzc2gtZWQyNTUxOQAAACBgrXe4bKNhOzkCLWOmk4zDMimW9RVZngX51Y8h3BmKLA
AAAECItu0F8DIjWxTp+KeMDvX1lQwYtUvP2SfSVOfMOChxYGCtd7hso2E7OQItY6aTjMMy
KZb1FVmeBfnVjyHcGYosAAAADnJvb3RAbG9jYWxob3N0AQIDBAUGBw==
-----END OPENSSH PRIVATE KEY-----
richi@RicardoMedina:~/tmp$ icat -o 206848 disk.img 2346
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIGCtd7hso2E7OQItY6aTjMMyKZb1FVmeBfnVjyHcGYos root@localhost
richi@RicardoMedina:~/tmp$ icat -o 206848 disk.img 2345 > id_ed25519
richi@RicardoMedina:~/tmp$ ls
disk.img  id_ed25519
richi@RicardoMedina:~/tmp$ chmod 600 id_ed25519
richi@RicardoMedina:~/tmp$ ls -al
total 235532
drwxr-xr-x  2 richi richi      4096 May  7 23:07 .
drwxr-x--- 25 richi richi      4096 May  7 22:54 ..
-rw-r--r--  1 richi richi 241172480 Aug  4  2023 disk.img
-rw-------  1 richi richi       411 May  7 23:07 id_ed25519
richi@RicardoMedina:~/tmp$ ssh -i id_ed25519 -p 64732 ctf-player@saturn.picoctf.net
ctf-player@challenge:~$ ls
flag.txt
ctf-player@challenge:~$ cat flag.txt
picoCTF{k3y_5l3u7h_339601ed}ctf-player@challenge:~$ Connection to saturn.picoctf.net closed by remote host.
Connection to saturn.picoctf.net closed.

picoCTF{k3y_5l3u7h_339601ed}