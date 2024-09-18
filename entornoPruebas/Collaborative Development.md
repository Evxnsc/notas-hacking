
## Objetivo

My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?

## Datos de Acceso al Nivel

[challenge.zip](https://artifacts.picoctf.net/c_titan/179/challenge.zip)
## Solucion

```
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ ls         
flag.py
                                                                             
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ cat flag.py 
print("Printing the flag...")
print("picoCTF{t3@mw0rk_", end='')                                                                             
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ git checkout               
                                                                             
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ git checkout featuere/part-2
error: pathspec 'featuere/part-2' did not match any file(s) known to git
                                                                             
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ git checkout feature/part-2 
Switched to branch 'feature/part-2'
                                                                             
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ cat flag.py
print("Printing the flag...")

print("m@k3s_th3_dr3@m_", end='')                                                                             
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ git checkout feature/part-3
Switched to branch 'feature/part-3'
                          
┌──(kali㉿kali)-[~/Downloads/drop-in]
└─$ cat flag.py                
print("Printing the flag...")

print("w0rk_798f9981}")

```

## Notas Adicionales

git-checkout - Cambiar ramas o restaurar archivos de árbol de trabajo

## Referencias
[git ramas](https://git-scm.com/book/es/v2/Ramificaciones-en-Git-Gesti%C3%B3n-de-Ramas)
[git checkout](https://git-scm.com/docs/git-checkout)
