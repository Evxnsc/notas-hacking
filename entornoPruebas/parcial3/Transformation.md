
## Objetivo

I wonder what this really is... [enc](https://mercury.picoctf.net/static/dd6004f51362ff76f98cb8c699510f23/enc) `''.join([chr((ord(flag[i]) << 8) + ord(flag[i + 1])) for i in range(0, len(flag), 2)])`

## Datos de Acceso al Nivel

 [enc](https://mercury.picoctf.net/static/dd6004f51362ff76f98cb8c699510f23/enc)
## Solucion

```
└─$ python3                     
Python 3.12.7 (main, Nov  8 2024, 17:55:36) [GCC 14.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> enc=open("enc").read()
>>> print(enc)
灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸弰摤捤㤷慽
>>> print(enc[0])
灩
>>> print(hex(ord(enc[0])))
0x7069
>>> for c in enc: 
...     print(hex(ord(c)).lstrip("0x"),end='')
... 
7069636f4354467b31365f626974735f696e73743334645f6f665f385f30646463643937617d>>> 

```

## Notas Adicionales



## Referencias
[convert](https://www.rapidtables.com/convert/number/hex-to-ascii.html)
