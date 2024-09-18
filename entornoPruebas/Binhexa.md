## Objetivo
How well can you perfom basic binary operations?


## Datos de Acceso al Nivel

`nc titan.picoctf.net 49697`

## Solucion

```
┌──(kali㉿kali)-[~]
└─$ nc titan.picoctf.net 49697

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 01101000
Binary Number 2: 10010000


Question 1/6:
Operation 1: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 11010000
Correct!

Question 2/6:
Operation 2: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11111000
Correct!

Question 3/6:
Operation 3: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11111000
Correct!

Question 4/6:
Operation 4: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11101010000000
Correct!

Question 5/6:
Operation 5: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 1001000
Correct!

Question 6/6:
Operation 6: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 0.10111000111001

Incorrect input. Provide the right input
Enter the binary result: 00000000
Correct!

Enter the results of the last operation in hexadecimal: 0

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_675602ae}


```
## Notas Adicionales

## Referencias