## Objetivo

This vault uses for-loops and byte arrays. The source code for this vault is here:

## Datos de Acceso al Nivel

 [VaultDoor3.java](https://jupiter.challenges.picoctf.org/static/943ea40e3f54fca6d2145fa7aadc5e09/VaultDoor3.java)
## Solucion

```
var password = "jU5t_a_sna_3lpm18g947_u_4_m9r54f"
undefined
var password = "jU5t_a_sna_3lpm18g947_u_4_m9r54f";
undefined
var buffer = Array(32)
undefined
var buffer = Array(32);
undefined

for (i=0; i<8; i++) {
            buffer[i] = password.charAt(i);
        }
        for (; i<16; i++) {
            buffer[i] = password.charAt(23-i);…
"g"
buffer.join("")
"jU5t_a_s1mpl3_an4gr4m_4_u_79958f"

```

## Notas Adicionales



## Referencias