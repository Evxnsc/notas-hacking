## Objetivo

Download this disk image and find the flag. Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.



## Datos de Acceso al Nivel

- [Download compressed disk image](https://artifacts.picoctf.net/c/213/disk.flag.img.gz)
## Solucion

```
└─$ fls -o 0000411648 disk.flag.img 472
r/r 1875:       .ash_history
r/r * 1876(realloc):    flag.txt
r/r 1782:       flag.txt.enc

┌──(kali㉿kali)-[~/picoCTF/forensic/operationorchid]
└─$ icat -o 0000411648 disk.flag.img 472                                             
�
 .
  ..S$
      .ash_historyflag.txt��
                            flag.txt.enc
                                        �,洞                                                                                        
┌──(kali㉿kali)-[~/picoCTF/forensic/operationorchid]
└─$ icat -o 0000411648 disk.flag.img 1782
Salted__�ށ��e��B�J▒�c�$QE&$��4jM�KGeE�1�^Ȥ7� ���؎$�'%                                                                                        
┌──(kali㉿kali)-[~/picoCTF/forensic/operationorchid]
└─$ icat -o 0000411648 disk.flag.img 1782 > flag.txt.enc
 
┌──(kali㉿kali)-[~/picoCTF/forensic/operationorchid]
└─$ openssl aes256 -salt -d -in flag.txt.enc -out flag.txt -k unbreakablepassword1234567
*** WARNING : deprecated key derivation used.
Using -iter or -pbkdf2 would be better.
bad decrypt
40A7BE26267F0000:error:1C800064:Provider routines:ossl_cipher_unpadblock:bad decrypt:../providers/implementations/ciphers/ciphercommon_block.c:107:
 
┌──(kali㉿kali)-[~/picoCTF/forensic/operationorchid]
└─$ cat flag.txt
picoCTF{h4un71ng_p457_5113beab}  
```

## Notas Adicionales



## Referencias
