## Objetivo

How about some hide and seek heh? Look at this image.

## Datos de Acceso al Nivel

 [here](https://artifacts.picoctf.net/c/235/atbash.jpg).
## Solucion

```
─$ steghide extract -sf atbash.jpg
Enter passphrase: 
wrote extracted data to "encrypted.txt".

┌──(kali㉿kali)-[~/picoCTF/crypto/hidetosee]
└─$ cat encrypted.txt 
krxlXGU{zgyzhs_xizxp_92533667}

```

## Notas Adicionales



## Referencias

cyberchef