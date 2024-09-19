## Objetivo

How to automate tasks to run at intervals on linux servers? Use ssh to connect to this server:

## Datos de Acceso al Nivel

```
Server: saturn.picoctf.net
Port: 64203
Username: picoplayer 
Password: emrdK96SGH
```
## Solucion

```
──(kali㉿kali)-[~]
└─$ ssh picoplayer@saturn.picoctf.net -p 64203
The authenticity of host '[saturn.picoctf.net]:64203 ([13.59.203.175]:64203)' can't be established.
ED25519 key fingerprint is SHA256:dMTscRrUiURy7uMu5eGWwEKdd2FzqLzx6LfWhssWnNQ.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[saturn.picoctf.net]:64203' (ED25519) to the list of known hosts.
picoplayer@saturn.picoctf.net's password: 
Welcome to Ubuntu 20.04.5 LTS (GNU/Linux 6.5.0-1023-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

This system has been minimized by removing packages and content that are
not required on a system that users do not log into.

To restore this content, you can run the 'unminimize' command.

The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

picoplayer@challenge:~$ cat /etc/crontab
# picoCTF{Sch3DUL7NG_T45K3_L1NUX_0bb95b71}

```

## Notas Adicionales



## Referencias