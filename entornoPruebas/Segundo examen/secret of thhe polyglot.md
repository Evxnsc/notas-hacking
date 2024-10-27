## Objetivo

The Network Operations Center (NOC) of your local institution picked up a suspicious file, they're getting conflicting information on what type of file it is. They've brought you in as an external expert to examine the file. Can you extract all the information from this strange file? Download the suspicious file [here](https://artifacts.picoctf.net/c_titan/9/flag2of2-final.pdf).

## Datos de Acceso al Nivel

[here](https://artifacts.picoctf.net/c_titan/9/flag2of2-final.pdf).
## Solucion

```
 open flag2of2-final.pdf    
    
┌──(kali㉿kali)-[~/picoCTF/examen/secretofthepolyglot]
└─$ convert flag2of2-final.pdf flag2of2-final.png 
convert-im6.q16: profile 'icc': 'RGB ': RGB color space not permitted on grayscale PNG `flag2of2-final.png' @ warning/png.c/MagickPNGWarningHandler/1669.

┌──(kali㉿kali)-[~/picoCTF/examen/secretofthepolyglot]
└─$ ls
flag2of2-final.pdf  flag2of2-final.png

┌──(kali㉿kali)-[~/picoCTF/examen/secretofthepolyglot]
└─$ open flag2of2-final.png

```

## Notas Adicionales



## Referencias
