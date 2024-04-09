# Routeo 

Es comunicar, conectar redes

Regla Ruteo

1. Debe haber un equipo de union
2. Todos los equipos esten en la misma red
3. Todos los equipos tengan un DG (No sé que sea)

Qué pasá si tengo que pasar por dos puntos de union? (Conectar dos routers)

Los dos equipos deben concer que equipos hay en la otra red. 
La conexión entre dos los routers es una red adicional 

#|Dir red|Equipos|Reglas
-|-|-|-
1|  182.168.100.0/24 <br>10.0.0.0/24|   Router 0|Para llegar 192.168.100.0 dehe preguntar a 10.0.0.2
2|  192.168.100.0/24 <br>10.0.0.0/24|   Router 1| Para llegar al 200.34.128.0  debe preguntar a 10.0.0.1

>Relga para routeo <br>
> ip route 192.168.100.0 255.255.255.0 10.0.0.2 <br>
ip route 200.34.128.0  255.255.255.0 10.0.0.1
