## Objetivo

Fix the syntax error in this Python script to print the flag.

## Datos de Acceso al Nivel

[Download Python script](https://artifacts.picoctf.net/c/27/fixme1.py)
## Solucion

```
┌──(kali㉿kali)-[~/Downloads]
└─$ python fixme1.py   
  File "/home/kali/Downloads/fixme1.py", line 20
    print('That is correct! Here\'s your flag: ' + flag)
IndentationError: unexpected indent
                                                                                      
┌──(kali㉿kali)-[~/Downloads]
└─$ nano fixme1.py 
┌──(kali㉿kali)-[~/Downloads]
└─$ python fixme1.py 
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_182342f7}

```

## Notas Adicionales

Se modifico una linea en donde tenia una tabulación donde no debia

## Referencias