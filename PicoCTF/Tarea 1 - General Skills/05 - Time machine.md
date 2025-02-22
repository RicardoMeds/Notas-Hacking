#### - **Descripción** 
What was I last working on? I remember writing a note to help me remember...You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/162/challenge.zip)

**Pista**
The `cat` command will let you read a file, but that won't help you here!
Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).
When committing a file with git, a message can (and should) be included.
#### - **Solución** 
hejacker-picoctf@webshell:~$ ls
README.txt  challenge.zip  drop-in
Thejacker-picoctf@webshell:~$ git log
fatal: not a git repository (or any parent up to mount point /)
Stopping at filesystem boundary (GIT_DISCOVERY_ACROSS_FILESYSTEM not set).
Thejacker-picoctf@webshell:~$ cd drop-in/
Thejacker-picoctf@webshell:~/drop-in$ git log
Thejacker-picoctf@webshell:~/drop-in$ 

picoCTF{t1m3m@ch1n3_e8c98b3a}