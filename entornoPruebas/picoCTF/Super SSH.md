## Objetivo

Using a Secure Shell (SSH) is going to be pretty important. Can you `ssh` as `ctf-player` to `titan.picoctf.net` at port `58393` to get the flag?
## Datos de Acceso al Nivel

`ssh` as `ctf-player` to `titan.picoctf.net` at port `58393` 
## Solucion

```
$ ssh ctf-player@titan.picoctf.net -p 58393
The authenticity of host '[titan.picoctf.net]:58393 ([3.139.174.234]:58393)' can't be established.
ED25519 key fingerprint is SHA256:4S9EbTSSRZm32I+cdM5TyzthpQryv5kudRP9PIKT7XQ.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[titan.picoctf.net]:58393' (ED25519) to the list of known hosts.
ctf-player@titan.picoctf.net's password: 
Welcome ctf-player, here's your flag: picoCTF{s3cur3_c0nn3ct10n_3e293eea}
Connection to titan.picoctf.net closed.
```

## Notas Adicionales



## Referencias