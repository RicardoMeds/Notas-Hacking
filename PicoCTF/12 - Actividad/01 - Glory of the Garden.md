#### - **Descripción** 
Este [jardín](https://jupiter.challenges.picoctf.org/static/4153422e18d40363e7ffc7e15a108683/garden.jpg) contiene más de lo que parece

**Pista**
¿Qué es un editor hexadecimal?
#### - **Solución** 
richi@RicardoMedina:~$ strings garden.jpg > strings.txt
richi@RicardoMedina:~$ wc -l strings.txt
28584 strings.txt
richi@RicardoMedina:~$ cat strings.txt | grep pico
Here is a flag "picoCTF{more_than_m33ts_the_3y33dd2eEF5}"
richi@RicardoMedina:~$