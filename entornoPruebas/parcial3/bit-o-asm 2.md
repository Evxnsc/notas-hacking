
## Objetivo

Can you figure out what is in the `eax` register? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`. Download the assembly dump [here](https://artifacts.picoctf.net/c/510/disassembler-dump0_b.txt).

## Datos de Acceso al Nivel

[here](https://artifacts.picoctf.net/c/510/disassembler-dump0_b.txt).
## Solucion

```


┌──(kali㉿kali)-[~/picoCTF/parcial3/bit-o-asm-2]
└─$ cat disassembler-dump0_b.txt 
<+0>:     endbr64 
<+4>:     push   rbp
<+5>:     mov    rbp,rsp
<+8>:     mov    DWORD PTR [rbp-0x14],edi
<+11>:    mov    QWORD PTR [rbp-0x20],rsi
<+15>:    mov    DWORD PTR [rbp-0x4],0x9fe1a
<+22>:    mov    eax,DWORD PTR [rbp-0x4]
<+25>:    pop    rbp
<+26>:    ret


zsh: corrupt history file /home/kali/.zsh_history
┌──(kali㉿kali)-[~/picoCTF/parcial3/bit-o-asm-2]
└─$ python3                     
Python 3.12.7 (main, Nov  8 2024, 17:55:36) [GCC 14.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 0x9fe1a
654874

```

## Notas Adicionales



## Referencias