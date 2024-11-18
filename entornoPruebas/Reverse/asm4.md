
## Objetivo

What will asm4("picoCTF_f97bb") return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/76ef117df9226a8a9306a8865b14068e/test.S)

## Datos de Acceso al Nivel

[Source](https://jupiter.challenges.picoctf.org/static/76ef117df9226a8a9306a8865b14068e/test.S)
## Solucion

```

──(kali㉿kali)-[~/picoCTF/reverse/asm4]
└─$ gcc -m32 -c solve.c -o solve.o -W
                                                                                                                
┌──(kali㉿kali)-[~/picoCTF/reverse/asm4]
└─$ gcc -m32 -o a.out solve.o chal.o 
/usr/bin/ld: warning: chal.o: missing .note.GNU-stack section implies executable stack
/usr/bin/ld: NOTE: This behaviour is deprecated and will be removed in a future version of the linker
                                                                                                                
┌──(kali㉿kali)-[~/picoCTF/reverse/asm4]
└─$ ./a.out  
flag: 0x265

```

## Notas Adicionales



## Referencias

