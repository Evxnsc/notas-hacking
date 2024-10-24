## Objetivo

Let's decrypt this: [ciphertext](https://jupiter.challenges.picoctf.org/static/ee7e2388b45f521b285334abb5a63771/ciphertext)? Something seems a bit small.

## Datos de Acceso al Nivel

 [ciphertext](https://jupiter.challenges.picoctf.org/static/ee7e2388b45f521b285334abb5a63771/ciphertext)
## Solucion

```
import gmpy2  
from gmpy2 import *  
  
gmpy2.get_context().precision=2048  
  
  
e=3  
c=2205316413931134031074603746928247799030155221252519872649649212867614751848436763801274360463406171277838056821437115883619169702963504606017565783537203207707757768473109845162808575425972525116337319108047893250549462147185741761825125  
  
root, exact = iroot(c,e)  
  
print(bytes.fromhex( hex(root)[2:] ).decode())
```

## Notas Adicionales



## Referencias