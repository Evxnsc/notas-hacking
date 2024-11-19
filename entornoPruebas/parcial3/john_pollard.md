
## Objetivo

Sometimes RSA [certificates](https://jupiter.challenges.picoctf.org/static/c882787a19ed5d627eea50f318d87ac5/cert) are breakable

## Datos de Acceso al Nivel

 [certificates](https://jupiter.challenges.picoctf.org/static/c882787a19ed5d627eea50f318d87ac5/cert)
## Solucion

```
┌──(kali㉿kali)-[~/picoCTF/parcial3/johnpollard]
└─$ openssl x509 -pubkey -in cert -out cert.pub
                                                                                                                
┌──(kali㉿kali)-[~/picoCTF/parcial3/johnpollard]
└─$ openssl rsa -pubin -in cert.pub -text      
Public-Key: (53 bit)
Modulus: 4966306967 (0x11a417f)
Exponent: 65537 (0x01)
writing RSA key
-----BEGIN PUBLIC KEY-----
MCIwDQYJKoZIhvcNAQEBBQfwIDAQAB
-----END PUBLIC KEY-----

```

## Notas Adicionales



## Referencias

[factor numbers](https://www.alpertron.com.ar/ECM.HTM)
