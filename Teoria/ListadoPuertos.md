bit * 1000 = kbit

byte * 1024 = kByte

## Semiplexacion:
Permite la transmision pero obliga a elegir una sola señal al mismo tiempo, sin poder ver multiples señales a la vez(Ejemplo Canales de TV, Radio)
Deja ver una sola comunicacion a la vez para poder hacer otra o usar otra se debe cambiar de señal o frecuencia

### Metodos de envio:

#### TCP(Protocolo de Control de Transmision/Transporte):
Es el protocolo de control y chequeo de los datagramas enviando señales para avisarsi el archivo esta correcto o no.

##### Etiquetas de TCP:

| Source Port Number 2Byte | Destination port number 2Byte |        
| :--- | ---: |
| Sequence Number 4Byte(centro tabla) |
| Acknowledgement Number 4Byte (centro tabla) |
|Data Offset 4 bits| Reserved 3 bits | Control flags 9 bits | Windows size 2Byte |
| Checksum 2Byte| Urgent pointer 2Byte|  
| 20 | Byte |
| Optional Data 0-40Byte (centro tabla)|

#### UDP(Protocolo de Datagrama de Usuario):
Es el protocolo de envio en tiempo real pero sin orden ni chequeos.

| Source Port Number 2Byte | Destination Port Number 2Byte |
| :----------- | -------------: |
| Lenght 2Byte | Checksum 2Byte |
| 8 | Byte |

#### IANA
Puertos:
0-1024 Muy conocidos o conocidos
1025-49151 Registrados
49152-65535 Utiles 


[IANA](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml)

0:  Reservado para programacion 
20 Y 21(FTP): Transferencia de archivos/datos
22(SSH): Protocolo del Shell, acesso remoto seguro
23(TELNET): Acesso remoto no seguro

##### **25(SMTP): Es el que permite hacer las transferencia de Mails**

37(Tiempo): Indica el tiempo y hora global del dispositivo.
38(RAP): Protocolo que permite el acceso a la ruta
39(RIP): Protocolo que indica cual ruta es

42(Nombre)/43(Nombre Usuario): Son los que te indican los nombres

53(DNS): Es el encargado de transmitir y transformar las paginas
69(TFTP): Genera el historial de nuestras acciones en el servidor
80(HTTP): En Desuso(Sin utilizar)

110(POP3): Es el que retira el Mail desde el 25

123(NTP): Es el protocolo que se maneja dentro de la red en tiempo real, controla todo lo que sucede dentro de la red




Frecuencia: Ciclo de reloj
