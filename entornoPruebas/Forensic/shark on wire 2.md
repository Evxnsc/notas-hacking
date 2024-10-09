## Objetivo

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/b506393b6f9d53b94011df000c534759/capture.pcap). Recover the flag that was pilfered from the network.

## Datos de Acceso al Nivel

We found this [packet capture](https://jupiter.challenges.picoctf.org/static/b506393b6f9d53b94011df000c534759/capture.pcap). 
## Solucion

```
from scapy.all import *  
  
packets = rdpcap('capture.pcap')  
flag = ''  
for p in packets:  
    if UDP in p and p[UDP].dport == 22:  
        if p[UDP].sport > 5000:  
            flag += chr(p[UDP].sport - 5000)  
print(flag)
```

## Notas Adicionales



## Referencias