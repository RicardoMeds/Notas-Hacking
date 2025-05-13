#### - **Descripción** 
Los archivos siempre se pueden modificar de forma secreta. ¿Puedes encontrar la bandera? [cat.jpg](https://mercury.picoctf.net/static/7cf6a33f90deeeac5c73407a1bdc99b6/cat.jpg)
#### Pista 
Asegúrese de enviar la bandera como picoCTF{XXXXX}

Mira los detalles del archivo
#### - **Solución** 
richi@RicardoMedina:~$ exiftool cat.jpg | grep License | sed -e 's/.*: //' | base64 -d
picoCTF{the_m3tadata_1s_modified}richi@RicardoMedina:~$