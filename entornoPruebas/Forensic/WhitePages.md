## Objetivo

I stopped using YellowPages and moved onto WhitePages... but [the page they gave me](https://jupiter.challenges.picoctf.org/static/95be9526e162185c741259a75dffa0ab/whitepages.txt) is all blank!

## Datos de Acceso al Nivel

but [the page they gave me](https://jupiter.challenges.picoctf.org/static/95be9526e162185c741259a75dffa0ab/whitepages.txt) is all blank!
## Solucion

```
from pwn import *  
  
file = open('whitepages.txt', 'rb')  
data = bytearray(file.read())  
data = data.replace(b'\xe2\x80\x83',b'0')  
data = data.replace(b'\x20',b'1')  
data = data.decode('ascii')  
data = unbits(data)  
  
print(data)
```

## Notas Adicionales

No pude instalar la libreria desde kali y lo hice en pycharm en windows

## Referencias