#### - **Descripción** 
¿Cómo automatizar tareas para que se ejecuten a intervalos en servidores Linux?

Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.
How to automate tasks to run at intervals on linux servers?Use ssh to connect to this server:

```
Server: saturn.picoctf.net
Port: 64196
Username: picoplayer 
Password: emrdK96SGH
```

**Pista**

#### - **Solución** 
picoplayer@challenge:/home$ cd ..
picoplayer@challenge:/$ ls
bin  boot  challenge  dev  etc  home  lib  lib32  lib64  libx32  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
picoplayer@challenge:/$ cd challenge/
-bash: cd: challenge/: Permission denied
picoplayer@challenge:/$ cd /challenge/
-bash: cd: /challenge/: Permission denied
picoplayer@challenge:/$ cat etc/crontab 

picoCTF{Sch3DUL7NG_T45K3_L1NUX_0bb95b71}
picoplayer@challenge:/$ Connection to saturn.picoctf.net closed by remote host.
Connection to saturn.picoctf.net closed.
Thejacker-picoctf@webshell:~$ 

picoCTF{Sch3DUL7NG_T45K3_L1NUX_0bb95b71}