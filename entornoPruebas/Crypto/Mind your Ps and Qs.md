## Objetivo

In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this?

## Datos de Acceso al Nivel

 [values](https://mercury.picoctf.net/static/3cfeb09681369c26e3f19d886bc1e5d9/values)
## Solucion

```
import gmpy2  
from Cryptodome.Util.number import long_to_bytes, inverse  
from gmpy2 import *  
  
c = 8533139361076999596208540806559574687666062896040360148742851107661304651861689  
n = 769457290801263793712740792519696786147248001937382943813345728685422050738403253  
p = 1617549722683965197900599011412144490161  
e = 65537  
q = 475693130177488446807040098678772442581573  
  
n = p * q  
tn = (p-1)*(q-1)  
d = inverse(e,tn)  
m = pow(c, d, n)  
print(long_to_bytes(m))
```
## Notas Adicionales

factorizamos p y q con ayuda de una pagina

## Referencias
[factordb](https://factordb.com/)
