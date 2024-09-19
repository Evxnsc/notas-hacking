## Objetivo

There's an interesting script in the user's home directory The work computer is running SSH. We've been given a script which performs some basic calculations, explore the script and find a flag.

## Datos de Acceso al Nivel

```
Hostname: saturn.picoctf.net
Port:     56824
Username: picoplayer
Password: password
```
## Solucion

```
picoplayer@challenge:~$ ./useless -h
Read the code first
picoplayer@challenge:~$ ./useless add 2 4
The Sum is: 6
picoplayer@challenge:~$ man useless 

useless
     useless, — This is a simple calculator script

SYNOPSIS
     useless, [add sub mul div] number1 number2

DESCRIPTION
     Use the useless, macro to make simple calulations like addition,subtraction, multiplication and division.

Examples
     ./useless add 1 2
       This will add 1 and 2 and return 3

     ./useless mul 2 3
       This will return 6 as a product of 2 and 3

     ./useless div 6 3
       This will return 2 as a quotient of 6 and 3

     ./useless sub 6 5
       This will return 1 as a remainder of substraction of 5 from 6

Authors
     This script was designed and developed by Cylab Africa

     picoCTF{us3l3ss_ch4ll3ng3_3xpl0it3d_6194}
```

## Notas Adicionales

El comando man permite a los usuarios acceder al manual de referencia para ver información sobre la funcionalidad de los comandos en un terminal Linux.

## Referencias
[man](https://www.linode.com/es/content/use-the-man-command-to-learn-any-linux-command-top-docs-with-learn-linux-tv/#:~:text=El%20comando%20man%20permite%20a,y%20c%C3%B3mo%20navegar%20por%20ellas.)
