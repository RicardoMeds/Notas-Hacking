#### - **Descripción** 
**¿Puedes descifrar la contraseña para obtener la bandera?Descargue el verificador de contraseñas [aquí](https://artifacts.picoctf.net/c/12/level1.py) y también necesitará la [bandera](https://artifacts.picoctf.net/c/12/level1.flag.txt.enc) cifrada en el mismo directorio.**

**Pista**
Para ver el archivo en el webshell, haga lo siguiente:`$ nano level1.py`
Para salir `nano`, presione Ctrl y x y siga las instrucciones en pantalla.

#### - **Solución** 
hejacker-picoctf@webshell:~$ nano level1.py 
Thejacker-picoctf@webshell:~$ nano level1.flag.txt.enc 
Thejacker-picoctf@webshell:~$ python3 level1.py 
Please enter correct password for flag: 8713
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_1b2fd683}
Thejacker-picoctf@webshell:~$ 

picoCTF{545h_r1ng1ng_1b2fd683}