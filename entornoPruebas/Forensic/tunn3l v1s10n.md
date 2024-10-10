## Objetivo

We found this [file](https://mercury.picoctf.net/static/01be2b38ba97802285a451b94505ea75/tunn3l_v1s10n). Recover the flag.

## Datos de Acceso al Nivel

We found this [file](https://mercury.picoctf.net/static/01be2b38ba97802285a451b94505ea75/tunn3l_v1s10n).
## Solucion

```
└─$ ls
tunn3l_v1s10n

┌──(kali㉿kali)-[~/picoCTF/forensic/tunn3lvision]
└─$ mv tunn3l_v1s10n tunn3l_v1s10n.bmp

┌──(kali㉿kali)-[~/picoCTF/forensic/tunn3lvision]
└─$ ls
tunn3l_v1s10n.bmp

┌──(kali㉿kali)-[~/picoCTF/forensic/tunn3lvision]
└─$ open tunn3l_v1s10n.bmp 

┌──(kali㉿kali)-[~/picoCTF/forensic/tunn3lvision]
└─$ hexeditor tunn3l_v1s10n.bmp 

┌──(kali㉿kali)-[~/picoCTF/forensic/tunn3lvision]
└─$ open tunn3l_v1s10n.bmp 
   
┌──(kali㉿kali)-[~/picoCTF/forensic/tunn3lvision]
└─$ 

```

## Notas Adicionales

se cambio el tamaño

picoCTF{qu1t3_a_v13w_2020}

## Referencias