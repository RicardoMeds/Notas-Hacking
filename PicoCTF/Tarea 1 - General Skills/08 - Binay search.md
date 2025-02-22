#### - **Descripción** 
Want to play a game? As you use more of the shell, you might be interested in how they work! Binary search is a classic algorithm used to quickly find an item in a sorted list. Can you find the flag? You'll have 1000 possibilities and only 10 guesses.Cyber security often has a huge amount of data to look through - from logs, vulnerability reports, and forensics. Practicing the fundamentals manually might help you in the future when you have to write your own tools!You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_atlas/18/challenge.zip)

Additional details will be available after launching your challenge instance.

**Pista**
Have you ever played hot or cold? Binary search is a bit like that.
You have a very limited number of guesses. Try larger jumps between numbers!
The program will randomly choose a new number each time you connect. You can always try again, but you should start your binary search over from the beginning - try around 500. Can you think of why?
#### - **Solución** 
Thejacker-picoctf@webshell:~$ ssh -p 55979 ctf-player@atlas.picoctf.net
ctf-player@atlas.picoctf.net's password: 
Welcome to the Binary Search Game!
I'm thinking of a number between 1 and 1000.
Enter your guess: 500
Lower! Try again.
Enter your guess: 250
Lower! Try again.
Enter your guess: 100
Higher! Try again.
Enter your guess: 150
Higher! Try again.
Enter your guess: 190
Higher! Try again.
Enter your guess: 200
Higher! Try again.
Enter your guess: 225
Lower! Try again.
Enter your guess: 220
Higher! Try again.
Enter your guess: 223
Lower! Try again.
Enter your guess: 221
Congratulations! You guessed the correct number: 221
Here's your flag: picoCTF{g00d_gu355_2e90d29b}
Connection to atlas.picoctf.net closed.
Thejacker-picoctf@webshell:~$ 
Here's your flag: picoCTF{g00d_gu355_2e90d29b}