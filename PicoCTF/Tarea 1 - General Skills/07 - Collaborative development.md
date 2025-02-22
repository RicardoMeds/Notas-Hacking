#### - **Descripción** 
My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/177/challenge.zip)

**Pista**
`git branch -a` will let you see available branches
How can file 'diffs' be brought to the main branch? Don't forget to `git config`!
Merge conflicts can be tricky! Try a text editor like nano, emacs, or vim.
#### - **Solución** 

Thejacker-picoctf@webshell:~$ cd drop-in/
Thejacker-picoctf@webshell:~/drop-in$ git branch -a
Thejacker-picoctf@webshell:~/drop-in$ 
Thejacker-picoctf@webshell:~/drop-in$ git checkout feature/part-1 && cat flag.py && git checkout feature/part-2 && cat flag.py && git checkout feature/part-3 && cat flag.py
Switched to branch 'feature/part-1'
print("Printing the flag...")
print("picoCTF{t3@mw0rk_", end='')Switched to branch 'feature/part-2'
print("Printing the flag...")

print("m@k3s_th3_dr3@m_", end='')Switched to branch 'feature/part-3'
print("Printing the flag...")

print("w0rk_7ae8dd33}")
Thejacker-picoctf@webshell:~/drop-in$ 

picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_7ae8dd33}