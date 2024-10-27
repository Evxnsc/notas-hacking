## Objetivo

How about some hide and seek heh? Download this [file](https://artifacts.picoctf.net/c/375/trace.pcap) and find the flag.

## Datos de Acceso al Nivel

 [file](https://artifacts.picoctf.net/c/375/trace.pcap)
## Solucion

```
└─$ ls
trace.pcap

┌──(kali㉿kali)-[~/picoCTF/examen/pcappoisoning]
└─$ strings trace.pcap | grep pico
picoCTF{P64P_4N4L7S1S_SU55355FUL_5b6a6061}@~

```

## Notas Adicionales



## Referencias
