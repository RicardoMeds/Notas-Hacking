#### - **Descripción** 
Utilice `srch_strings` de sleuthkit y algo de terminal-fu para encontrar una bandera en esta imagen de disco: [dds1-alpine.flag.img.gz](https://mercury.picoctf.net/static/ac394d24f88e51a09cc909687cf6d853/dds1-alpine.flag.img.gz)

**Pista**
¿Alguna vez has utilizado «archivo» para determinar qué era un archivo?
Terminal-fu relevante en picoGym: https://play.picoctf.org/practice/challenge/85
Dominar esta terminal-fu te permitirá encontrar la bandera con un solo comando: https://play.picoctf.org/practice/challenge/48
¡Usando tu propia computadora, podrías usar qemu para arrancar desde este disco!

#### - **Solución** 
richi@RicardoMedina:~$ gunzip dds1-alpine.flag.img.gz
richi@RicardoMedina:~$ srch_strings dds1-alpine.flag.img | grep picoCTF
  SAY picoCTF{f0r3ns1c4t0r_n30phyt3_dcbf5942}
richi@RicardoMedina:~$

 picoCTF{f0r3ns1c4t0r_n30phyt3_dcbf5942}