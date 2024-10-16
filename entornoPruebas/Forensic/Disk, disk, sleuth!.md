## Objetivo

Use `srch_strings` from the sleuthkit and some terminal-fu to find a flag in this disk image: [dds1-alpine.flag.img.gz](https://mercury.picoctf.net/static/ac394d24f88e51a09cc909687cf6d853/dds1-alpine.flag.img.gz)

## Datos de Acceso al Nivel

[dds1-alpine.flag.img.gz](https://mercury.picoctf.net/static/ac394d24f88e51a09cc909687cf6d853/dds1-alpine.flag.img.gz)
## Solucion

```
└─$ gzip -d dds1-alpine.flag.img.gz 
 
┌──(kali㉿kali)-[~/picoCTF/forensic/disksleuth]
└─$ ls
dds1-alpine.flag.img

┌──(kali㉿kali)-[~/picoCTF/forensic/disksleuth]
└─$ srch_strings dds1-alpine.flag.img | grep pico
ffffffff81399ccf t pirq_pico_get
ffffffff81399cee t pirq_pico_set
ffffffff820adb46 t pico_router_probe
  SAY picoCTF{f0r3ns1c4t0r_n30phyt3_dcbf5942}

```

## Notas Adicionales



## Referencias