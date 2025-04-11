#### - **Descripción** 

BookShelf Pico, mi servicio premium de lectura de libros en línea.Creo que mi sitio web es súper seguro. ¡Te reto a que me demuestres lo contrario leyendo el libro "Flag"!

Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.

- Username: "user"
- Password: "user"

Source code can be downloaded [here](https://artifacts.picoctf.net/c/482/bookshelf-pico.zip).Website can be accessed [here!](http://saturn.picoctf.net:55090/).

#### Pista 
¿Quizás intentar encontrar la clave de firma JWT (la "clave secreta") en el código fuente? ¿Quizás esté codificada? ¿O intentar descifrarla?

¡Los campos 'role' y 'userId' en el JWT pueden ser de su interés!

Es posible que los paquetes Java "controladores", "servicios" y "seguridad" del código fuente requieran su atención. Proporcionamos un archivo README.md con documentación.

Actualiza tu rol con el _nuevo_ JWT (crackeado). Y vuelve a iniciar sesión para que el nuevo rol se refleje en el almacenamiento local del navegador

#### - **Solución** 
Se uso el JWT para modificarlo y poner Admin, 2, admin
eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJyb2xlIjoiQWRtaW4iLCJpc3MiOiJib29rc2hlbGYiLCJleHAiOjE3NDUwMDM5MjIsImlhdCI6MTc0NDM5OTEyMiwidXNlcklkIjoyLCJlbWFpbCI6ImFkbWluIn0.pPbYqq-piHj-xpe3ahmETvQR_2vxmdp-wfS__-AqEi8


picoCTF{w34k_jwt_n0t_g00d_d72df65e}

#### - **Referencias** 
https://jwt.io