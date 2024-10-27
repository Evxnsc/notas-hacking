
## Objetivo

The developer of this website mistakenly left an important artifact in the website source, can you find it? The website is [here](http://saturn.picoctf.net:50970/)

## Datos de Acceso al Nivel

[here](http://saturn.picoctf.net:50970/)
## Solucion

```
┌──(kali㉿kali)-[~/picoCTF/examen/searchsource]
└─$ ls
saturn.picoctf.net:50970

┌──(kali㉿kali)-[~/picoCTF/examen/searchsource]
└─$ grep -R pico saturn.picoctf.net:50970 
saturn.picoctf.net:50970/css/style.css:/** banner_main picoCTF{1nsp3ti0n_0f_w3bpag3s_8de925a7} **/
```

## Notas Adicionales



## Referencias