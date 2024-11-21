
## Objetivo

Can you figure out what is in the `eax` register at the end of the `main` function? Put your answer in the picoCTF flag format: `picoCTF{n}` where `n` is the contents of the `eax` register in the decimal number base. If the answer was `0x11` your flag would be `picoCTF{17}`. Debug [this](https://artifacts.picoctf.net/c/520/debugger0_b).

## Datos de Acceso al Nivel

 [this](https://artifacts.picoctf.net/c/520/debugger0_b).
## Solucion

```
set disassembly-flavor intel


info functions

disassemble main
break *0x401142
print/d $eax
```

## Notas Adicionales



## Referencias
