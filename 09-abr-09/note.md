# Configuración y seguridad del Switch

## Configuración de SSH

```
conf terminal
ip domain-name cisco.com
cryto key generate rsa
username <user_name>  secret ccna
username <user_name> [privilegie 15] secret <password>
line vty 0 15 %conectar 16 maquinas 
transport input ssh 
login local % tomar los usuraios dee para login 
exit
ip ssh version 2


```
**Para configurar SSH**

1. nombre del equipo
2. ip
3. crear usario
4. crear un dominio
5. configurar el shh


## aseguridad puertos del equipo

- Todos los puerto no activos deben ser apagados
- Configurar el puerto sólo para el equipo. Especificiar direcciones MAC o grupo de direcciones MAC permitada en un puerto especifico.  Especificar que un puerto se desactive automáticamente si se detecta direcciones Mas no autorizadas

```
interface fastthernet 0/19
switchport mode access
switchport port-security %antes de configurar la seguridad del puerto
switchport port-security maximum 10 $ cantidad máxima de drecciones seguras
switchport port-security mac-address 
switchport port-security protect|restrict|shutdown
```

