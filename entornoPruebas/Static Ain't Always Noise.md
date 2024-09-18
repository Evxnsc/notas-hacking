## Objetivo

Can you look at the data in this binary: ? This [BASH script](https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/ltdis.sh) might help!

## Datos de Acceso al Nivel

[static](https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/static)
[BASH script](https://mercury.picoctf.net/static/66932732825076cad4ba43e463dae82f/ltdis.sh) 
## Solucion

```
  
┌──(kali㉿kali)-[~/Downloads]
└─$ ./ltdis.sh
Attempting disassembly of  ...
objdump: 'a.out': No such file
objdump: section '.text' mentioned in a -j option, but not found in any input file
Disassembly failed!
Usage: ltdis.sh <program-file>
Bye!
                                                     
┌──(kali㉿kali)-[~/Downloads]
└─$ ./ltdis.sh static 
Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset

┌──(kali㉿kali)-[~/Downloads]
└─$ ls
drop-in  file  flag  ltdis.sh  static  static.ltdis.strings.txt  static.ltdis.x86_64.txt
                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ cat static.ltdis.strings.txt 
    238 /lib64/ld-linux-x86-64.so.2
    361 libc.so.6
    36b puts
    370 __cxa_finalize
    37f __libc_start_main
    391 GLIBC_2.2.5
    39d _ITM_deregisterTMCloneTable
    3b9 __gmon_start__
    3c8 _ITM_registerTMCloneTable
    660 AWAVI
    667 AUATL
    6ba []A\A]A^A_
    6e8 Oh hai! Wait what? A flag? Yes, it's around here somewhere!
    7c7 ;*3$"
   1020 picoCTF{d15a5m_t34s3r_f5aeda17}

```

## Notas Adicionales



## Referencias