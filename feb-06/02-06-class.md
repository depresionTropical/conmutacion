## Network
>1. Todos los bits de **host_id** están en 0. Es la **DIR RED**
>2. Todos los bits en **host_id** están en 1. Es **BROADCAST RED**
>3. El espacio de direcciones entre  **DIR RED** y **BROADCAST RED** se cnomo como **AMBITO** 

## Subnetting

Divir la red en pequeñas subredes

10.0.0.0/8

10._ _ _ _ _ _ _ _ _ .0.0

Si le agrego un bit a la máscara puedo crear dos subredes
n²

No se puede aumentar la red de clase, solo disminuirla 

### Ejemplo 

subnetting para crear dos subredes


| | |Máscara|
|--|--|--|
|RED|192.168.100.0|255.255.255.128|
|1ra RED | 192.168.100.0|255.255.255.128|
|BROADCAST|192.168.100.27|255.255.255.128|
|2da RED|192.168.100.128|/25
|BROADCAST|192.168..100.255|\25

### Ejemplo

**PRIMERA RED**


|# |RED|Dir. RED|Dir Broadcast|
|--|--|--|--|
|1|10.0.0.0/30| 10.0.0.0|10.0.0.3
|2|10.0.0.4/30|10.0.0.4|10.0.0.7|
