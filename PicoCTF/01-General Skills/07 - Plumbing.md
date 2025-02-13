#### Description

Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 7480`.


What's a pipe? No not that kind of pipe... This [kind](http://www.linfo.org/pipes.html)

#### Solución 

Thejacker-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 7480 > salida 

Thejacker-picoctf@webshell:~$ cat salida | grep pico 
picoCTF{digital_plumb3r_06e9d954}
Thejacker-picoctf@webshell:~$ 

picoCTF{digital_plumb3r_06e9d954}