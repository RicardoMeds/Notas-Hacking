#### - **Descripción** 
How well can you perfom basic binary operations?

Additional details will be available after launching your challenge instance.

**Pista**


#### - **Solución** 

Thejacker-picoctf@webshell:~$ nc titan.picoctf.net 51048

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 00101011
Binary Number 2: 00101011


Question 1/6:
Operation 1: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 01010110
Correct!

Question 2/6:
Operation 2: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 00101011
Incorrect. Try again
Enter the binary result: 11100111001
Correct!

Question 3/6:
Operation 3: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 1010110
Correct!

Question 4/6:
Operation 4: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 00101011
Correct!

Question 5/6:
Operation 5: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 00010101
Correct!

Question 6/6:
Operation 6: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 00101011
Correct!

Enter the results of the last operation in hexadecimal: 2B

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_6862762d}
