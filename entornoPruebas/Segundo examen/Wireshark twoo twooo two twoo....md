## Objetivo

Can you find the flag? [shark2.pcapng](https://mercury.picoctf.net/static/719e81d6fbb6b3157624268588fc0de8/shark2.pcapng).

## Datos de Acceso al Nivel

 [shark2.pcapng](https://mercury.picoctf.net/static/719e81d6fbb6b3157624268588fc0de8/shark2.pcapng).
## Solucion

```
┌──(kali㉿kali)-[~/picoCTF/examen/wiresark]
└─$ tshark -nr shark2.pcapng -Y 'dns && ip.src == 192.168.38.104 && frame contains "local" && ip.dst==18.217.1.57' | awk '{ print $12 }' | awk -F. '{ print $1 }' | tr -d "\n"
cGljb0NURntkbnNfM3hmMWxfZnR3X2RlYWRiZWVmfQ==fQ==   

─(kali㉿kali)-[~/picoCTF/examen/wiresark]
└─$ echo cGljb0NURntkbnNfM3hmMWxfZnR3X2RlYWRiZWVmfQ==fQ== | base64 -d
picoCTF{dns_3xf1l_ftw_deadbeef}}     
```

## Notas Adicionales



## Referencias