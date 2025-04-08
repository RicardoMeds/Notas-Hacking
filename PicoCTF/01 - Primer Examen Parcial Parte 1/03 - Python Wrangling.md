#### - **Descripción** 
#### Description

Los scripts de Python se invocan de forma similar a los programas en la Terminal... ¿Puedes ejecutar [este script de Python](https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/ende.py) usando [esta contraseña](https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/pw.txt) para obtener [la bandera](https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/flag.txt.en) ?
#### Pista 
Haga que el script de Python sea accesible en su shell ingresando el siguiente comando en el indicador de Terminal:`$ wget https://mercury.picoctf.net/static/5c4c0cbfbc149f3b0fc55c26f36ee707/ende.py`
`$ man python`
#### - **Solución** 
richi@RicardoMedina:~$ cat pw.txt | python3 ende.py -d flag.txt.en
Please enter the password:picoCTF{4p0110_1n_7h3_h0us3_192ee2db}
richi@RicardoMedina:~$

picoCTF{4p0110_1n_7h3_h0us3_192ee2db}
