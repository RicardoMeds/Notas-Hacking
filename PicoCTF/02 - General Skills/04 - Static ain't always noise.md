#### Description

Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/bc72945175d643626d6ea9a689672dbd/static)? This [BASH script](https://mercury.picoctf.net/static/bc72945175d643626d6ea9a689672dbd/ltdis.sh) might help!

#### Solución 
Thejacker-picoctf@webshell:~$ ls
README.txt  ltdis.sh  static
Thejacker-picoctf@webshell:~$ bash ltdis.sh static
Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset
Thejacker-picoctf@webshell:~$ cat.static.strings.txt | grep picoCTF 
-bash: cat.static.strings.txt: command not found
Thejacker-picoctf@webshell:~$ LS
-bash: LS: command not found
Thejacker-picoctf@webshell:~$ ls
README.txt  ltdis.sh  static  static.ltdis.strings.txt  static.ltdis.x86_64.txt
Thejacker-picoctf@webshell:~$ cat static.ltdis.strings.txt | grep pico
   1020 picoCTF{d15a5m_t34s3r_1e6a7731}
Thejacker-picoctf@webshell:~$ 


picoCTF{d15a5m_t34s3r_1e6a7731}