
## Objetivo

Connect to this PostgreSQL server and find the flag! 

## Datos de Acceso al Nivel

`psql -h saturn.picoctf.net -p 64561 -U postgres pico` Password is `postgres`
## Solucion

```
\dt
select * from flags;
```

## Notas Adicionales



## Referencias