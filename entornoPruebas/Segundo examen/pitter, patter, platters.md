## Objetivo

'Suspicious' is written all over this disk image. Download 

## Datos de Acceso al Nivel

[suspicious.dd.sda1](https://jupiter.challenges.picoctf.org/static/c4852a91e1d0d180c75af188ea8d8a2c/suspicious.dd.sda1)
## Solucion

```
┌──(kali㉿kali)-[~/picoCTF/examen/pitter]
└─$ ls
suspicious.dd.sda1

┌──(kali㉿kali)-[~/picoCTF/examen/pitter]
└─$ strings -e b suspicious.dd.sda1 | rev       
picoCTF{b3_5t111_mL|_<3_f5290af6
bPOIiUYTWQq
sLKJjGF
cvXZ
scSC;3+#
aA1!
bPOIiUYTWQq
sLKJjGF
cvXZ
scSC;3+#
aA1!
scSC;3+#
aA1!
7777777777

```

## Notas Adicionales



## Referencias