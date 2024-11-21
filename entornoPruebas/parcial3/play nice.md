
## Objetivo

Not all ancient ciphers were so bad... The flag is not in standard format. `nc mercury.picoctf.net 6057` [playfair.py](https://mercury.picoctf.net/static/a48f79c95043804d1f43d5bfbffd324a/playfair.py)

## Datos de Acceso al Nivel

[playfair.py](https://mercury.picoctf.net/static/a48f79c95043804d1f43d5bfbffd324a/playfair.py)
## Solucion

```

┌──(kali㉿kali)-[~/picoCTF/parcial3/playnice]
└─$ python -c "print('WD9BUKBSPDTJ7SKD3KL8D6OA3F03G0'.lower())"
wd9bukbspdtj7skd3kl8d6oa3f03g0
                                                                                                                
┌──(kali㉿kali)-[~/picoCTF/parcial3/playnice]
└─$ nc mercury.picoctf.net 6057                                
Here is the alphabet: meiktp6yh4wxruavj9no13fb8d027c5glzsq
Here is the encrypted message: y7bcvefqecwfste224508y1ufb21ld
What is the plaintext message? wd9bukbspdtj7skd3kl8d6oa3f03g0
Congratulations! Here's the flag: 2e71b99fd3d07af3808f8dff2652ae0e

```

## Notas Adicionales



## Referencias

[decoder](https://www.dcode.fr/playfair-cipher)
