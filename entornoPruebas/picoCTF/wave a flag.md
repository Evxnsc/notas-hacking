## Objetivo

Can you invoke help flags for a tool or binary? [This program](https://mercury.picoctf.net/static/beec4f433e5ee5bfcd71bba8d5863faf/warm) has extraordinarily helpful information...

## Datos de Acceso al Nivel

[This program](https://mercury.picoctf.net/static/beec4f433e5ee5bfcd71bba8d5863faf/warm) 
## Solucion

```
─(kali㉿kali)-[~/Downloads]
└─$ ls
drop-in  warm
                                                                                                                                                                                                                                           
┌──(kali㉿kali)-[~/Downloads]
└─$ ./ warm
zsh: permission denied: ./
                                                                                                                                                                                                                                           
┌──(kali㉿kali)-[~/Downloads]
└─$ ./ warm
zsh: permission denied: ./

┌──(kali㉿kali)-[~/Downloads]
└─$ ls
drop-in  warm
                               
┌──(kali㉿kali)-[~/Downloads]
└─$ chmod +x warm    

┌──(kali㉿kali)-[~/Downloads]
└─$ ./ warm      
zsh: permission denied: ./

┌──(kali㉿kali)-[~/Downloads]
└─$ ./warm 
Hello user! Pass me a -h to learn what I can do!

┌──(kali㉿kali)-[~/Downloads]
└─$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_616f7182}

```

## Notas Adicionales



## Referencias