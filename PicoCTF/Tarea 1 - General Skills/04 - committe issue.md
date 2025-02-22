#### - **Descripción** 
I accidentally wrote the flag down. Good thing I deleted it!You download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/137/challenge.zip)


**Pista**
Version control can help you recover files if you change or lose them!
Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control)
You can 'checkout' commits to see the files inside them

#### - **Solución** 
Thejacker-picoctf@webshell:~$ cd drop-in/
Thejacker-picoctf@webshell:~/drop-in$ ls -agit log
ls: cannot access 'log': No such file or directory
Thejacker-picoctf@webshell:~/drop-in$ ls -a
.  ..  .git  message.txt
Thejacker-picoctf@webshell:~/drop-in$ git log
Thejacker-picoctf@webshell:~/drop-in$ 
Thejacker-picoctf@webshell:~/drop-in$ git checkout ea859bf3b5d94ee74ce5ee1afa3edd7d4d6b35f0
Note: switching to 'ea859bf3b5d94ee74ce5ee1afa3edd7d4d6b35f0'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at ea859bf create flag
Thejacker-picoctf@webshell:~/drop-in$ cat message.txt
picoCTF{s@n1t1z3_cf09a485}
Thejacker-picoctf@webshell:~/drop-in$ 

ea859bf3b5d94ee74ce5ee1afa3edd7d4d6b35f0

picoCTF{s@n1t1z3_cf09a485}