
## Objetivo


Here's a program that plays rock, paper, scissors against you. I hear something good happens if you win 5 times in a row. The program's source code with the flag redacted can be downloaded [here](https://artifacts.picoctf.net/c/147/game-redacted.c). Connect to the program with netcat: `$ nc saturn.picoctf.net 60657`
## Datos de Acceso al Nivel


## Solucion

```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{	
	int i;
	for(i = 0; i < 5; i++)
	{
		printf("1\n");
		
		srand(time(0));
		
		int computer_turn = rand() % 3;
		
		if (computer_turn == 0)
			printf("paper\n");
		else if (computer_turn == 1)
			printf("scissors\n");
		else
			printf("rock\n");
		
	}
	return 0;
}

┌──(kali㉿kali)-[~/picoCTF/binexp/rps]
└─$ ./rps | nc saturn.picoctf.net 60657
Welcome challenger to the game of Rock, Paper, Scissors
For anyone that beats me 5 times in a row, I will offer up a flag I found
Are you ready?
Type '1' to play a game
Type '2' to exit the program
1
scissors
1
scissors
1
scissors
1
scissors
1
scissors


Please make your selection (rock/paper/scissors):
You played: scissors
The computer played: paper
You win! Play again?
Type '1' to play a game
Type '2' to exit the program


Please make your selection (rock/paper/scissors):
You played: scissors
The computer played: paper
You win! Play again?
Type '1' to play a game
Type '2' to exit the program


Please make your selection (rock/paper/scissors):
You played: scissors
The computer played: paper
You win! Play again?
Type '1' to play a game
Type '2' to exit the program


Please make your selection (rock/paper/scissors):
You played: scissors
The computer played: paper
You win! Play again?
Type '1' to play a game
Type '2' to exit the program


Please make your selection (rock/paper/scissors):
You played: scissors
The computer played: paper
You win! Play again?
Congrats, here's the flag!
picoCTF{50M3_3X7R3M3_1UCK_C85AF58A}
Type '1' to play a game
Type '2' to exit the program
                              
```

## Notas Adicionales



## Referencias
