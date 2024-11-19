
## Objetivo

Oracles can be your best friend, they will decrypt anything, except the flag's ciphertext. How will you break it? Connect with `nc mercury.picoctf.net 33780`.

## Datos de Acceso al Nivel

`nc mercury.picoctf.net 33780`.
## Solucion

```
from pwn import *  
import binascii  
r=remote("mercury.picoctf.net",33780)  
print(r.recvuntil("n:"))  
n=int(r.recvline())  
print(n)  
print(r.recvuntil("e:"))  
e=int(r.recvline())  
print(e)  
print(r.recvuntil("ciphertext:"))  
c=int(r.recvline())  
print(c)  
print(r.recvuntil("to decrypt:"))  
# We will send c*2^e. It decrypts to c^d*2^(ed) = 2*c^d  
# It is different, and will decrypt to plaintext*2  
r.sendline(str(pow(2,e,n)*c))  
print(r.recvuntil("you go:"))  
p2=int(r.recvline())  
print(p2)  
print(p2//2)  
st="{:x}".format(p2//2)  
print(binascii.unhexlify(st))


b' Here you go:'
580550060391700078946913236734911770139931497702556153513487440893406629034802718534645538074938502890768709712035489670906
290275030195850039473456618367455885069965748851278076756743720446703314517401359267322769037469251445384354856017744835453
b'picoCTF{m4yb3_Th0se_m3s54g3s_4r3_difurrent_0801973}'
[*] Closed connection to mercury.picoctf.net port 33780
```

## Notas Adicionales



## Referencias

