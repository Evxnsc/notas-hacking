
## Objetivo

We have recovered a [binary](https://jupiter.challenges.picoctf.org/static/31c9b832d036a10daeef52d8b4290ef0/rev) and a [text file](https://jupiter.challenges.picoctf.org/static/31c9b832d036a10daeef52d8b4290ef0/rev_this). Can you reverse the flag.

## Datos de Acceso al Nivel

 [text file](https://jupiter.challenges.picoctf.org/static/31c9b832d036a10daeef52d8b4290ef0/rev_this). [binary](https://jupiter.challenges.picoctf.org/static/31c9b832d036a10daeef52d8b4290ef0/rev)
## Solucion

```
cifrado = open('rev_this', 'r').read()
print(cifrado)

for i in range(8, len(cifrado)-1):
	if i & 1 == 0:
		flag += chr( ord(cifrado[i])-5)
	else:
		flag += chr( ord(cifrado[i])+2)
print(flag)
```

## Notas Adicionales



## Referencias

