#### - **Descripción** 
Someone's commits seems to be preventing the program from working. Who is it?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/72/challenge.zip)

**Pista**
In collaborative projects, many users can make many changes. How can you see the changes within one file?
Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).
You can use `python3 <file>.py` to try running the code, though you won't need to for this challenge.
#### - **Solución** 
Thejacker-picoctf@webshell:~$ cd drop-in/
Thejacker-picoctf@webshell:~/drop-in$ git log
Thejacker-picoctf@webshell:~/drop-in$ git log message.py
Thejacker-picoctf@webshell:~/drop-in$ 
Thejacker-picoctf@webshell:~/drop-in$ 

 picoCTF{@sk_th3_1nt3rn_b64c4705}