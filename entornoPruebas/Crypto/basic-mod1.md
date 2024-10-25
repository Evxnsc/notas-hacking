## Objetivo

We found this weird message being passed around on the servers, we think we have a working decryption scheme. Download the message  Take each number mod 37 and map it to the following character set: 0-25 is the alphabet (uppercase), 26-35 are the decimal digits, and 36 is an underscore. Wrap your decrypted message in the picoCTF flag format (i.e. `picoCTF{decrypted_message}`)

## Datos de Acceso al Nivel

[here](https://artifacts.picoctf.net/c/127/message.txt).
## Solucion

```
 GNU nano 8.1                   exp.py                            
datos = open('message.txt').read().split()
print(datos)
flag = ''
for n in datos:
        c = int(n) % 37 
        if c>=0 and c<=25:
                s = chr(c+65)
        elif c>=26 and c<=35:
                s = chr(c+22)
        else:
                s = '_'
        flag += s
print(f"picoCTF{{{flag}}}")

```

## Notas Adicionales



## Referencias