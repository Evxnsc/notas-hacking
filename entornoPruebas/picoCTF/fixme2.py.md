## Objetivo

Fix the syntax error in the Python script to print the flag.

## Datos de Acceso al Nivel

[Download Python script](https://artifacts.picoctf.net/c/4/fixme2.py)
## Solucion

```
┌──(kali㉿kali)-[~/Downloads]
└─$ ls
drop-in  fixme2.py
                                                                                      
┌──(kali㉿kali)-[~/Downloads]
└─$ python fixme2.py
  File "/home/kali/Downloads/fixme2.py", line 22
    if flag = "":
       ^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?
                                                                                      
┌──(kali㉿kali)-[~/Downloads]
└─$ nano fixme2.py 
                                                                                                                                                             
┌──(kali㉿kali)-[~/Downloads]
└─$ nano fixme2.py
                                                                                                                                                             
┌──(kali㉿kali)-[~/Downloads]
└─$ python fixme2.py
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_e8814d03}
```

## Notas Adicionales



## Referencias