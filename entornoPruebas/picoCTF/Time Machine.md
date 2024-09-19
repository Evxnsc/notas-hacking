## Objetivo

What was I last working on? I remember writing a note to help me remember...

## Datos de Acceso al Nivel

[challenge.zip](https://artifacts.picoctf.net/c_titan/163/challenge.zip)
## Solucion

```
┌──(kali㉿kali)-[~/Downloads]
└─$ cd drop-in 
                                                                                      
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ ls
message.txt
                                                                                      
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ cat message.txt 
This is what I was working on, but I'd need to look at my commit history to know why...                                                                                      
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ ls -all
total 16
drwxr-xr-x 3 kali kali 4096 Sep 17 22:32 .
drwxr-xr-x 3 kali kali 4096 Sep 17 22:32 ..
drwxr-xr-x 8 kali kali 4096 Sep 17 22:32 .git
-rw-r--r-- 1 kali kali   87 Mar 11  2024 message.txt
                                                                                      
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ git log                                              
commit e65fedb3a72a16c577f4b17023b63997134b307d (HEAD -> master)
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:07:29 2024 +0000

    picoCTF{t1m3m@ch1n3_88c35e3b}
```

## Notas Adicionales



## Referencias