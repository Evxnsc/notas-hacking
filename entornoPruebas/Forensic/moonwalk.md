## Objetivo

Decode this [message](https://jupiter.challenges.picoctf.org/static/fc1edf07742e98a480c6aff7d2546107/message.wav) from the moon.

## Datos de Acceso al Nivel

Decode this [message](https://jupiter.challenges.picoctf.org/static/fc1edf07742e98a480c6aff7d2546107/message.wav) 
## Solucion

```
└─$ sstv -d message.wav   
[sstv] Searching for calibration header... Found!    
[sstv] Detected SSTV mode Scottie 1
[sstv] Decoding image...   [####################################################] 100%
[sstv] Drawing image data...
[sstv] ...Done!

┌──(kali㉿kali)-[~/picoCTF/forensic/moonwalk]
└─$ sstv -d message.wav -o result.png
[sstv] Searching for calibration header... Found!    
[sstv] Detected SSTV mode Scottie 1
[sstv] Decoding image...   [####################################################] 100%
[sstv] Drawing image data...
[sstv] ...Done!

┌──(kali㉿kali)-[~/picoCTF/forensic/moonwalk]
└─$ ls
message.wav  result.png

┌──(kali㉿kali)-[~/picoCTF/forensic/moonwalk]
└─$ open result.png 

┌──(kali㉿kali)-[~/picoCTF/forensic/moonwalk]
└─$ 

```

## Notas Adicionales

picoCTF{beep_boop_im_in_space}

## Referencias