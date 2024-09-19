
## Objetivo
#### Description

Want to play a game? As you use more of the shell, you might be interested in how they work! Binary search is a classic algorithm used to quickly find an item in a sorted list. Can you find the flag? You'll have 1000 possibilities and only 10 guesses. Cyber security often has a huge amount of data to look through - from logs, vulnerability reports, and forensics. Practicing the fundamentals manually might help you in the future when you have to write your own tools! You can download the challenge files here:




## Datos de Acceso al Nivel

`ssh -p 56063 ctf-player@atlas.picoctf.net`

## Solucion

```
┌──(kali㉿kali)-[~]
└─$ ssh -p 56063 ctf-player@atlas.picoctf.net
The authenticity of host '[atlas.picoctf.net]:56063 ([18.217.83.136]:56063)' can't be established.
ED25519 key fingerprint is SHA256:M8hXanE8l/Yzfs8iuxNsuFL4vCzCKEIlM/3hpO13tfQ.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[atlas.picoctf.net]:56063' (ED25519) to the list of known hosts.
ctf-player@atlas.picoctf.net's password: 
Welcome to the Binary Search Game!
I'm thinking of a number between 1 and 1000.
Enter your guess: 500
Lower! Try again.
Enter your guess: 300
Lower! Try again.
Enter your guess: 100
Lower! Try again.
Enter your guess: 50
Higher! Try again.
Enter your guess: 60
Higher! Try again.
Enter your guess: 80
Lower! Try again.
Enter your guess: 70
Lower! Try again.
Enter your guess: 65
Higher! Try again.
Enter your guess: 66
Higher! Try again.
Enter your guess: 67
Higher! Try again.
Sorry, you've exceeded the maximum number of guesses.
Connection to atlas.picoctf.net closed.
                                                                             
┌──(kali㉿kali)-[~]
└─$ ssh -p 56063 ctf-player@atlas.picoctf.net
ctf-player@atlas.picoctf.net's password: 
Welcome to the Binary Search Game!
I'm thinking of a number between 1 and 1000.
Enter your guess: 100
Higher! Try again.
Enter your guess: 200
Lower! Try again.
Enter your guess: 150
Higher! Try again.
Enter your guess: 170
Higher! Try again.
Enter your guess: 190
Higher! Try again.
Enter your guess: 195
Higher! Try again.
Enter your guess: 198
Lower! Try again.
Enter your guess: 197
Congratulations! You guessed the correct number: 197
Here's your flag: picoCTF{g00d_gu355_6dcfb67c}
Connection to atlas.picoctf.net closed.
                                                                             
┌──(kali㉿kali)-[~]
└─$ 


```
## Notas Adicionales

## Referencias