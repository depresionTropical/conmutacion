# Enrutamiento dínamico

Comando

```html:
ip route <red> <mask> <salto>
```

## Configuración de rutas de respaldo

cuando o cuales es el camino. El primer camino a tomar y cuando tomar el segundo camino 

Costo administrativo. Mientras más alto sea, es la ruta más dificil a tomar, por default es 0

```html:
ip route <red> <mask> <salto> [costo administrativo]
```
Ejemplo
```cisco:
ip route 0.0.0.0 0.0.0.0 <salto1> 
ip route 0.0.0.0 0.0.0.0 <salto2> 2
ip route 0.0.0.0 0.0.0.0 <salto3> 5
```

# Ipv6

## Estrustura de IPv6

- 128bit hexadecimal de formtato (0-9,A-F)
- Usa 16bits hexadecimal separadas por dos puntos (:)
- Cada dígito 4-hexadecimal es equivalente a 16-bits
- Consiste en 8 hex/cuarteto las cuales equivalen en 16-bits por hexteto

Global Routing Prefix|Subnet ID|Interface Id|MASK
-|-|-|-
2001:0DB8:0001|5270|0127:00AB:CAFE:0E1F|/64

Los primer 3 bits van del 001 o2 200 :: 12 (IANA GLOBAL ROUTING)

