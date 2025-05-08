#### - **Descripción** 
Descargue la imagen de disco y úsela `mmls`para determinar el tamaño de la partición de Linux. Conéctese al servicio de verificación remota para comprobar su respuesta y obtener la bandera.Nota: si está usando el shell web, descargue y extraiga la imagen del disco en un `/tmp`directorio que no sea su directorio de inicio.[Descargar imagen de disco](https://artifacts.picoctf.net/c/164/disk.img.gz)

Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.

**Pista**
¿Alguna vez has utilizado «archivo» para determinar qué era un archivo?
Terminal-fu relevante en picoGym: https://play.picoctf.org/practice/challenge/85
Dominar esta terminal-fu te permitirá encontrar la bandera con un solo comando: https://play.picoctf.org/practice/challenge/48
¡Usando tu propia computadora, podrías usar qemu para arrancar desde este disco!

#### - **Solución** 
richi@RicardoMedina:~$ file disk.img
disk.img: DOS/MBR boot sector; partition 1 : ID=0x83, active, start-CHS (0x0,32,33), end-CHS (0xc,190,50), startsector 2048, 202752 sectors
richi@RicardoMedina:~$ file disk*
disk.img: DOS/MBR boot sector; partition 1 : ID=0x83, active, start-CHS (0x0,32,33), end-CHS (0xc,190,50), startsector 2048, 202752 sectors
richi@RicardoMedina:~$ mmls disk.flag*
Error stat(ing) image file (raw_open: image "disk.flag*" - No such file or directory)
richi@RicardoMedina:~$ mmls disk.img*
DOS Partition Table
Offset Sector: 0
Units are in 512-byte sectors

      Slot      Start        End          Length       Description
000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
001:  -------   0000000000   0000002047   0000002048   Unallocated
002:  000:000   0000002048   0000204799   0000202752   Linux (0x83)
richi@RicardoMedina:~$

0000202752 

richi@RicardoMedina:~$ nc saturn.picoctf.net 59620
What is the size of the Linux partition in the given disk image?
Length in sectors: 202752
202752
Great work!
picoCTF{mm15_f7w!}