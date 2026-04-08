HTTPS: 443
QKG.LLC: 2523 
MACOS: 456
DHCPV6: 546 Client - 547 Server

# Red
Es la capa que maneja el orden de las direcciones y sus rutas

## Funciones principales:

### Direccionamiento:
Utilizar el DHCP para asignar IP de manera automatica

Direcciones IP: Direccion hogar
Direcciones MAC(6400::/4700::3A:49B): Direccion personales

#### Dirreccionamiento Estatico:
Es aquel realizado por el usuario que utiliza el DHCP para asignar nosotros mismos el IP de manera estatica

### Enrutamiento:
Realiza una Ruta por donde pasa la informacion, enlistando los nodos por su direccion

#### Enrutamiento Automatico:
Utiliza el protocolo RIP

#### Enrutamiento Estatico:
Utiliza el protocolo ARP

######## Protocolos que vamos a utilizar nosotros:
IP,RIP,ARP,ICMP

#### IP:
Es el estándar fundamental que define las reglas para direccionar y enrutar paquetes de datos a través de redes, permitiendo que dispositivos en internet se comuniquen. 

Divide las direcciones en dos partes, red y host, separadas mediante una máscara de subred para facilitar el enrutamiento.

#### RIP:
Es un protocolo de vector de distancia utilizado en redes pequeñas para encontrar la mejor ruta (menor número de saltos) entre origen y destino

#### ARP:
Se encarga de la traduccion de las direcciones IP(logicas) de 32 bits a direcciones MAC(fisicas) de 48 bits en una red local(LAN)

#### ICMP:
Es un protocolo de la capa de red utilizado por dispositivos (como enrutadores) para diagnosticar problemas y comunicar errores en la transmisión de datos IP

