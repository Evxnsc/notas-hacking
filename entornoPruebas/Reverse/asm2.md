
## Objetivo

What does asm2(0x4,0x2d) return? Submit the flag as a hexadecimal value (starting with '0x'). NOTE: Your submission for this question will NOT be in the normal flag format. [Source](https://jupiter.challenges.picoctf.org/static/ceac75672637589213b952abe32c84b3/test.S)

## Datos de Acceso al Nivel

 [Source](https://jupiter.challenges.picoctf.org/static/ceac75672637589213b952abe32c84b3/test.S)
## Solucion

```
stack
[     ] < esp
[     ] < ebp - oxc
[  0x4 ] < ebp -ox8
[ 0x2d ] < ebp - 0x4
[ ebp ] < ebp
[ ret ] < ebp + 0x4
[ 0x4 ] < ebp < ox8
[ 0x2d ] < ebp + 0xc

registers   
[ 0x4  ] eax

asm20x4: (0x4,0x2d)
        <+0>:   push   ebp
        <+1>:   mov    ebp,esp

        <+3>:   sub    esp,0x10
        <+6>:   mov    eax,DWORD PTR [ebp+0xc]
        <+9>:   mov    DWORD PTR [ebp-0x4],eax
        <+12>:  mov    eax,DWORD PTR [ebp+0x8]
        <+15>:  mov    DWORD PTR [ebp-0x8],eax
        <+18>:  jmp    0x50c <asm2+31>
        <+20>:  add    DWORD PTR [ebp-0x4],0x1
        <+24>:  add    DWORD PTR [ebp-0x8],0xd1
        <+31>:  cmp    DWORD PTR [ebp-0x8],0x5fa1
        <+38>:  jle    0x501 <asm2+20>
        <+40>:  mov    eax,DWORD PTR [ebp-0x4]

        <+43>:  leave  
        <+44>:  ret 

>>> 0x5fa1 / 0xd1
117.13397129186603
>>> 
>>> int(0x2d)
45
>>> hex(45 + 118)
'0xa3'
>>> 

```

## Notas Adicionales



## Referencias