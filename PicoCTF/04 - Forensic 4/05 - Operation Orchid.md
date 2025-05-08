#### - **Descripción** 
Descargue esta imagen de disco y busque la bandera.Nota: si está usando el shell web, descargue y extraiga la imagen del disco en un `/tmp`directorio que no sea su directorio de inicio.

- [Descargar imagen de disco comprimida](https://artifacts.picoctf.net/c/212/disk.flag.img.gz)

**Pista**

#### - **Solución** 
richi@RicardoMedina:~/tmp$ file disk.flag.img
disk.flag.img: DOS/MBR boot sector; partition 1 : ID=0x83, active, start-CHS (0x0,32,33), end-CHS (0xc,223,19), startsector 2048, 204800 sectors; partition 2 : ID=0x82, start-CHS (0xc,223,20), end-CHS (0x19,159,6), startsector 206848, 204800 sectors; partition 3 : ID=0x83, start-CHS (0x19,159,7), end-CHS (0x32,253,11), startsector 411648, 407552 sectors
richi@RicardoMedina:~/tmp$ file disk.flag.img -0 2048
disk.flag.img: DOS/MBR boot sector; partition 1 : ID=0x83, active, start-CHS (0x0,32,33), end-CHS (0xc,223,19), startsector 2048, 204800 sectors; partition 2 : ID=0x82, start-CHS (0xc,223,20), end-CHS (0x19,159,6), startsector 206848, 204800 sectors; partition 3 : ID=0x83, start-CHS (0x19,159,7), end-CHS (0x32,253,11), startsector 411648, 407552 sectors
2048:          cannot open `2048' (No such file or directory)
richi@RicardoMedina:~/tmp$ fls disk.flag.img 472 -o 411648
r/r 1875:       .ash_history
r/r * 1876(realloc):    flag.txt
r/r 1782:       flag.txt.enc
richi@RicardoMedina:~/tmp$ icat -o 411648 disk.flag.img 1872 > flag.txt.enc
richi@RicardoMedina:~/tmp$ ls
disk.flag.img  flag.txt.enc

richi@RicardoMedina:~/tmp$ openssl aes256 -d -salt -in flag.txt.enc -out flag.txt -k unbreakablepassword1234567

picoCTF{h4un71ng_p457_0a710765}