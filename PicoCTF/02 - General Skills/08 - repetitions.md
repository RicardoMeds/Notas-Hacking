#### Description

Can you make sense of this file?Download the file [here](https://artifacts.picoctf.net/c/474/enc_flag).

#### Solución 
Thejacker-picoctf@webshell:~$ cat enc_flag | base64 --decode | base64 --decode | base64 --decode 
WTBkc2FtSXdUbFZTYm5ScFdWaE9iRTVxVW1aaWFrNTZaRVJPYTFneVVuQlpla0pyU1ZjME5GZ3lV
WGRrTWpWelRVUlNhMDB5VW1aTgpNbGswVFZkWk0xbHRWamxEWnowOUNnPT0K
Thejacker-picoctf@webshell:~$ cat enc_flag | base64 --decode | base64 --decode | base64 --decode | base64 --decode 
Y0dsamIwTlVSbnRpWVhObE5qUmZiak56ZEROa1gyUnBZekJrSVc0NFgyUXdkMjVzTURSa00yUmZN
Mlk0TVdZM1ltVjlDZz09Cg==
Thejacker-picoctf@webshell:~$ cat enc_flag | base64 --decode | base64 --decode | base64 --decode | base64 --decode | base64 --decode 
cGljb0NURntiYXNlNjRfbjNzdDNkX2RpYzBkIW44X2Qwd25sMDRkM2RfM2Y4MWY3YmV9Cg==
Thejacker-picoctf@webshell:~$ cat enc_flag | base64 --decode | base64 --decode | base64 --decode | base64 --decode | base64 --decode | base64 --decode 
picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_3f81f7be}
Thejacker-picoctf@webshell:~$ 

picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_3f81f7be}