#### - **Descripción** 
Descargue esta imagen de disco y busque la bandera.Nota: si está usando el shell web, descargue y extraiga la imagen del disco en un `/tmp`directorio que no sea su directorio de inicio.

- [Descargar imagen de disco comprimida](https://artifacts.picoctf.net/c/137/disk.flag.img.gz)

**Pista**

#### - **Solución** 
richi@RicardoMedina:~/sleu$ gzip -d disk.flag.img.gz
richi@RicardoMedina:~/sleu$ mmls  disk.flag.img
DOS Partition Table
Offset Sector: 0
Units are in 512-byte sectors

      Slot      Start        End          Length       Description
000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
001:  -------   0000000000   0000002047   0000002048   Unallocated
002:  000:000   0000002048   0000206847   0000204800   Linux (0x83)
003:  000:001   0000206848   0000360447   0000153600   Linux Swap / Solaris x86 (0x82)
004:  000:002   0000360448   0000614399   0000253952   Linux (0x83)
richi@RicardoMedina:~/sleu$ fsstat -o 2048 disk.flag.img
richi@RicardoMedina:~/sleu$ fls -i raw -f ext4 -o 2048 -r disk.flag.img

richi@RicardoMedina:~/sleu$ fls -i raw -f ext4 -o 360448 -r disk.flag.img | grep flag
++ r/r * 2082(realloc): flag.txt
++ r/r 2371:    flag.uni.txt
richi@RicardoMedina:~/sleu$ icat -i raw -f ext4 -o 360448 disk.flag.img 2082
            3.449677            13.056403
richi@RicardoMedina:~/sleu$ icat -i raw -f ext4 -o 360448 disk.flag.img 2371
picoCTF{by73_5urf3r_adac6cb4}
richi@RicardoMedina:~/sleu$