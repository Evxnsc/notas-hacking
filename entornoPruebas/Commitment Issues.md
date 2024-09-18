
## Objetivo

I accidentally wrote the flag down. Good thing I deleted it!

## Datos de Acceso al Nivel

[challenge.zip](https://artifacts.picoctf.net/c_titan/138/challenge.zip)
## Solucion

```
(kali㉿kali)-[~/Downloads]
└─$ ls
challenge.zip  drop-in
                                                              
┌──(kali㉿kali)-[~/Downloads]
└─$ cd drop-in 
                                                              
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ ls
message.txt
                                                              
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ cat message.txt
TOP SECRET
                                                              
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ git log                    
commit 42942c9c605b30100f5d859ef6e172027447c0db (HEAD -> master)
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:06:23 2024 +0000

    remove sensitive info

commit b562f0b425907789d11d2fe2793e67592dc6be93
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:06:23 2024 +0000

    create flag
                                                              
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ git checkout b562f0b425907789d11d2fe2793e67592dc6be93
Note: switching to 'b562f0b425907789d11d2fe2793e67592dc6be93'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at b562f0b create flag
                                                              
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ ls
message.txt
                                                              
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ cat message.txt 
picoCTF{s@n1t1z3_c785c319}

```

## Notas Adicionales



## Referencias