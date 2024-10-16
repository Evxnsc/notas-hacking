## Objetivo

Download this disk image, find the key and log into the remote machine. Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.



## Datos de Acceso al Nivel

- [Download disk image](https://artifacts.picoctf.net/c/71/disk.img.gz)
- Remote machine: `ssh -i key_file -p 49889 ctf-player@saturn.picoctf.net`
## Solucion

```
─$ fls -o 206848 disk.img 470
r/r 2344:       .ash_history
d/d 3916:       .ssh
    
┌──(kali㉿kali)-[~/picoCTF/forensic/operation]
└─$ fls -o 206848 disk.img 3916
r/r 2345:       id_ed25519
r/r 2346:       id_ed25519.pub
      
┌──(kali㉿kali)-[~/picoCTF/forensic/operation]
└─$ icat -o 206848 disk.img 2345
-----BEGIN OPENSSH PRIVATE KEY-----
b3BlbnNzaC1rZXktdjEAAAAABG5vbmUAAAAEbm9uZQAAAAAAAAABAAAAMwAAAAtzc2gtZW
QyNTUxOQAAACBgrXe4bKNhOzkCLWOmk4zDMimW9RVZngX51Y8h3BmKLAAAAJgxpYKDMaWC
gwAAAAtzc2gtZWQyNTUxOQAAACBgrXe4bKNhOzkCLWOmk4zDMimW9RVZngX51Y8h3BmKLA
AAAECItu0F8DIjWxTp+KeMDvX1lQwYtUvP2SfSVOfMOChxYGCtd7hso2E7OQItY6aTjMMy
KZb1FVmeBfnVjyHcGYosAAAADnJvb3RAbG9jYWxob3N0AQIDBAUGBw==
-----END OPENSSH PRIVATE KEY-----
    
┌──(kali㉿kali)-[~/picoCTF/forensic/operation]
└─$ icat -o 206848 disk.img 2345  > key_file
    
┌──(kali㉿kali)-[~/picoCTF/forensic/operation]
└─$ chmod 400 key_file 




Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

ctf-player@challenge:~$ ls
flag.txt
ctf-player@challenge:~$ cat flag.txt 

```

## Notas Adicionales



## Referencias