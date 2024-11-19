
## Objetivo

We found a brand new type of encryption, can you break the secret code? (Wrap with picoCTF{}) `mlnklfnknljflfjljnjijjmmjkmljnjhmhjgjnjjjmmkjjmijhmkjhjpmkmkmljkjijnjpmhmjjgjj` [new_caesar.py](https://mercury.picoctf.net/static/43182e6d4527ef0916b2ce43883227b7/new_caesar.py)

## Datos de Acceso al Nivel

[new_caesar.py](https://mercury.picoctf.net/static/43182e6d4527ef0916b2ce43883227b7/new_caesar.py)
## Solucion

```
┌──(kali㉿kali)-[~/picoCTF/parcial3/newcaesar]
└─$ python3 exp.py       
ÜëÆëì¦Æ¬®©ªÝ«Ü®¨Ø§®ª­ÛªÙ¨Û¨ ÛÛÜ«©® ØÚ§ª
---------------------
ËÚµÚÛµÌËÇÊÈÊÊÊËÇÉ
---------------------
ºÉ¤ÉÊ¤»º¶¹·¹¹¹º¶¸
---------------------
©¸¸¹sy{vwªx©{u¥t{wz¨w¦u¨u}¨¨©xv{}¥§tw
---------------------
§§¨bhjefgjdcjfifddlgejlcf
---------------------
qQqWYTUVYSRYUXUSS[VTY[RU
---------------------
v`@`FHCDwEvHBrAHDGuDsBuBJuuvECHJrtAD
---------------------
et_tu?_5723f4e71a0736d3b1d19dde4279ac03
---------------------
TcNcd.N$&!"U#T& P/&"%S"Q S (SST#!&(PR/"
---------------------
CR=RS=DCOB@BBBCOA
---------------------
2A,AB
1?1112>0>
---------------------
!01ûóþÿ"ð!óý-üóÿò ÿ.ý ýõ  !ðþóõ-/üÿ
---------------------
/
/ ê
àâíîïâìëâîáîììäïíâäëî
---------------------
ùÙùßÑÜÝÞÑÛ
          ÚÑÝÐÝ
               ÛÛÓÞÜÑÓ
ÚÝ
---------------------
ÈèÎÀËÌÿÍþÀÊúÉÀÌÏýÌûÊýÊÂýýþÍËÀÂúüÉÌ
---------------------
íü×üý·×½¿º»î¼í¿¹é¸¿»¾ì»ê¹ì¹±ììí¼º¿±éë¸»
---------------------
None
                                                                                                                
┌──(kali㉿kali)-[~/picoCTF/parcial3/newcaesar]
└─$ cat exp.py  
import string

combined = ""
result = ""
enc = ''
ALPHABET = string.ascii_lowercase[:16]

def decryptFlag(enc1):
    global combined, result, enc
    # shift
    a = 0
    while a <= 15:
        # shifting
        y = 0
        x = 0
        while y < len(enc1):
            t1 = ord(enc1[y])
            t2 = a
            enc += ALPHABET[(t1 - t2) % len(ALPHABET)]
            y += 1
        # decryption
        while x < (len(enc) - 1):
            firstChar = ord(enc[x]) - 97
            fBit1 = "{:04b}".format(firstChar)

            secondChar = ord(enc[x + 1]) - 97
            fBit2 = "{:04b}".format(secondChar)

            tempCombine = fBit1 + fBit2
            combined += str(chr(int(tempCombine, 2)))
            x += 2
        print(combined)
        print('---------------------')
        combined = ""
        enc = ""
        a += 1

flag = 'mlnklfnknljflfjljnjijjmmjkmljnjhmhjgjnjjjmmkjjmijhmkjhjpmkmkmljkjijnjpmhmjjgjj'
print(decryptFlag(flag))
                          
```

## Notas Adicionales



## Referencias

