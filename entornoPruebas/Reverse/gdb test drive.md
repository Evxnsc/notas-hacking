
## Objetivo

Can you get the flag? Download this [binary](https://artifacts.picoctf.net/c/87/gdbme). Here's the test drive instructions
## Datos de Acceso al Nivel

[binary](https://artifacts.picoctf.net/c/87/gdbme)
## Solucion

```
- `$ chmod +x gdbme`
- `$ gdb gdbme`
- `(gdb) layout asm`
- `(gdb) break *(main+99)`
- `(gdb) run`
- `(gdb) jump *(main+104)`
```

## Notas Adicionales



## Referencias

