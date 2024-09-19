## Objetivo

Don't power users get tired of making spelling mistakes in the shell? Not anymore! Enter Special, the Spell Checked Interface for Affecting Linux. Now, every word is properly spelled and capitalized... automatically and behind-the-scenes! Be the first to test Special in beta, and feel free to tell us all about how Special streamlines every development process that you face. When your co-workers see your amazing shell interface, just tell them: That's Special (TM) Start your instance to see connection details.

## Datos de Acceso al Nivel

`ssh -p 57853 ctf-player@saturn.picoctf.net`
## Solucion

```

Special$ ls
Is 
sh: 1: Is: not found
Special$ $(IFS=];b=cat]blargh/flag.txt;$b)
$(IFS=];b=cat]blargh/flag.txt;$b) 
sh: 1: picoCTF{5p311ch3ck_15_7h3_w0r57_b741d1b1}: not found
Special$ 

```

## Notas Adicionales



## Referencias

https://book.hacktricks.xyz/