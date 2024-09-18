## Objetivo

Our flag printing service has started glitching!

## Datos de Acceso al Nivel

`nc saturn.picoctf.net`
## Solucion

```
┌──(kali㉿kali)-[~/Downloads]
└─$ nc saturn.picoctf.net 50607        
'picoCTF{gl17ch_m3_n07_' + chr(0x62) + chr(0x64) + chr(0x61) + chr(0x36) + chr(0x38) + chr(0x66) + chr(0x37) + chr(0x35) + '}'

```

## Notas Adicionales

Se convierte los numeros de hexadecimal a texto y nos daria la bandera

## Referencias
[RapidTables](https://www.rapidtables.com/convert/number/hex-to-ascii.html)
