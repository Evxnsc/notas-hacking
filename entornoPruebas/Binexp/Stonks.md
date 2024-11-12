
## Objetivo

I decided to try something noone else has before. I made a bot to automatically trade stonks for me using AI and machine learning. I wouldn't believe you if you told me it's unsecure! [vuln.c](https://mercury.picoctf.net/static/a4ce675e8f85190152d66014c9eebd7e/vuln.c) `nc mercury.picoctf.net 59616`
## Datos de Acceso al Nivel

[vuln.c](https://mercury.picoctf.net/static/a4ce675e8f85190152d66014c9eebd7e/vuln.c) `nc mercury.picoctf.net 59616`
## Solucion

```
Python 3.12.6 (main, Sep  7 2024, 14:20:15) [GCC 14.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> s = 'ocip{FTC0l_I4_t5m_ll0m_y_y3n841645ebÿ£}'
>>> for x in range(0,len(s),4):
...     print(s[x+3]+s[x+2]+s[x+1]+s[x],end='')
... 
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
IndexError: string index out of range
picoCTF{I_l05t_4ll_my_m0n3y_6148be54>>> 
```

## Notas Adicionales



## Referencias

