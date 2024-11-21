
## Objetivo

#### Description

[keygenme-trial.py](https://mercury.picoctf.net/static/a6d9cac3bfa4935ceb50c145d3ff5586/keygenme-trial.py)

## Datos de Acceso al Nivel

[keygenme-trial.py](https://mercury.picoctf.net/static/a6d9cac3bfa4935ceb50c145d3ff5586/keygenme-trial.py)

## Solucion


```
import hashlib
import base64

# Partes de la clave
key_part_static1_trial = "picoCTF{1n_7h3_|<3y_of_"
key_part_dynamic1_trial = "xxxxxxxx"
key_part_static2_trial = "}"
key_full_template_trial = key_part_static1_trial + key_part_dynamic1_trial + key_part_static2_trial

# Nombre de usuario
username_trial = b"FREEMAN"

# Clave dinámica potencial
potential_dynamic_key = ""

# Punto de inicio del desplazamiento
offset = 23

# Posiciones en el hash SHA-256
positions = [4, 5, 3, 6, 2, 7, 1, 8]

# Generar la parte dinámica de la clave usando las posiciones
for p in positions:
    potential_dynamic_key += hashlib.sha256(username_trial).hexdigest()[p]

# Construir la clave completa
key = key_part_static1_trial + potential_dynamic_key + key_part_static2_trial

# Imprimir la clave generada y su longitud
print(key)
print(len(key))

```

## Notas Adicionales



## Referencias
