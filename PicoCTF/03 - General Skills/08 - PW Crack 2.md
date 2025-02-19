#### - **Descripción** 
¿Puedes descifrar la contraseña para obtener la bandera?Descargue el verificador de contraseñas [aquí](https://artifacts.picoctf.net/c/14/level2.py) y también necesitará la [bandera](https://artifacts.picoctf.net/c/14/level2.flag.txt.enc) cifrada en el mismo directorio.

**Pista**
¿Te resulta familiar esta codificación?
#### - **Solución** 
Thejacker-picoctf@webshell:~$ nano level2.py 
Thejacker-picoctf@webshell:~$ python3
Python 3.10.12 (main, Sep 11 2024, 15:47:36) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print(chr(0x34) + chr(0x65) + chr(0x63) + chr(0x39))
4ec9
>>> exit()
Thejacker-picoctf@webshell:~$ python3 level2.py 
Please enter correct password for flag: 4ec9
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_9701e681}
Thejacker-picoctf@webshell:~$ 

picoCTF{tr45h_51ng1ng_9701e681}