
## Objetivo
Someone's commits seems to be preventing the program from working. Who is it? You can download the challenge files here:


## Datos de Acceso al Nivel

[challenge.zip](https://artifacts.picoctf.net/c_titan/156/challenge.zip)


## Solucion

```
                                                                             
┌──(kali㉿kali)-[~/Downloads]
└─$ ls
challenge.zip  drop-in
                                                                             
┌──(kali㉿kali)-[~/Downloads]
└─$ cd drop-in  
                                                                             
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ ls
message.py
                                                                             
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ git log message.py           
commit 0351e0474493168ca76441c24630c17554fd09ca
Author: picoCTF{@sk_th3_1nt3rn_d2d29f22} <ops@picoctf.com>
Date:   Tue Mar 12 00:07:01 2024 +0000

    optimize file size of prod code

commit c9e851509190f5887e91339ee18087e3e77ebfda
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:07:01 2024 +0000

    create top secret project
                                                                             
┌──(kali㉿kali)-[~/Downloads/drop-in]


```
## Notas Adicionales

## ¿Qué hace Git log?

El comando `git log` muestra todas las commits en el historial del repositorio.

## Referencias

[FreeCode](https://www.freecodecamp.org/espanol/news/explicacion-del-comando-git-log/)
