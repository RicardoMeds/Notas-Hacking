#### Descripción

Este archivo tiene una bandera a simple vista (también conocida como "sin trabas"). [Descargar bandera](https://mercury.picoctf.net/static/704f877da185904ec3992e7255a15c6c/flag) .

#### Solución 
Thejacker-picoctf@webshell:~$ wget https://mercury.picoctf.net/static/704f877da185904ec3992e7255a15c6c/flag
--2025-02-12 18:42:20--  https://mercury.picoctf.net/static/704f877da185904ec3992e7255a15c6c/flag
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 34 [application/octet-stream]
Saving to: 'flag'

flag                                                       100%[=======================================================================================================================================>]      34  --.-KB/s    in 0s      

2025-02-12 18:42:20 (16.4 MB/s) - 'flag' saved [34/34]
Thejacker-picoctf@webshell:~$ ls
README.txt  file  flag
Thejacker-picoctf@webshell:~$ cat flag | grep pico 

picoCTF{s4n1ty_v3r1f13d_1a94e0f9}
