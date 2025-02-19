#### - **Descripción** 
¿Puedes descifrar la contraseña para obtener la bandera?Descargue el verificador de contraseñas [aquí](https://artifacts.picoctf.net/c/17/level3.py) y necesitará la [bandera](https://artifacts.picoctf.net/c/17/level3.flag.txt.enc) cifrada y el [hash](https://artifacts.picoctf.net/c/17/level3.hash.bin) en el mismo directorio también.Hay 7 contraseñas posibles, de las cuales 1 es correcta. Puedes encontrarlas examinando el script de verificación de contraseñas.

**Pista**
Para ver el archivo level3.hash.bin en el webshell, haga lo siguiente:`$ bvi level3.hash.bin`
Para salir `bvi`escriba `:q`y presione enter.
#### - **Solución** 
Thejacker-picoctf@webshell:~$ python level3.py 
Please enter correct password for flag: 87ab
Welcome back... your flag, user:

picoCTF{m45h_fl1ng1ng_cd6ed2eb}

Thejacker-picoctf@webshell:~$ 
