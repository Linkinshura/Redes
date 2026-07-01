# Subneteo Ejercicios modelo prueba 2

## 1) Completar el cuadro con lo que pide(realizar todos los cálculos)

| Direccion | N° Bits Subred | N° Bits Host | Subredes | Host | Mascara Subred | Broadcasting 2° Subred |
| :-------: | :------------: | :----------: | :------: | :--: | :------------: | :--------------------: |
| 192.168.0.14/29 | 5       |    3         |  32        |   6  | 255.255.255.248|  192.168.0.16          |
| 172.16.0.36 |      4        |         12     |    16    |      |                |                        |
| 10.150.14.28/12 |   4       |       20       |          |      |                |                        |
| 192.168.0.33   |    3      |       5       |          |      |                |                        |
| 128.138.4.55/19   |  3      |    13          |          |      |                |                        |
| 4.35.0.78      |      16     |  8            |          |      | 255.255.255.0  |                        |

## 1)
### 192.168.0.14 /29

2ⁿ - 2 = host
2ⁿ = 32
n = 5

2ⁿ = 32 subredes

192.168.000.014
255.255.255.000
_______________
/.  ./  ./  (00000) ---> Subred (000) ---> host

Mascara: 255.255.255.248

| Origen | Direcciones Asignables | Broadcasting |
| :-:    | :-:                    | :-:          |
| 192.168.0.0 | 192.168.0.1 - 192.168.0.6 | 192.168.0.7 |
|192.168.0.8 | 192.168.0.9 - 192.168.0.15 | 192.168.0.16|


## 2) Cual de las Siguientes es Correcta si tenemos la dirección 199.160.0.100 con una mascara de subred 255.255.255.224?

### A- pertenece a la subred 4 que esta entre la dirección raiz 199.160.0.98 y la dirección broadcasting 199.160.0.129.

### B- pertenece a la subred 5 que esta entre la dirección raíz 199.160.0.96 y la dirección broadcasting 199.160.0.127.

### C- pertenece a la subred 4 que esta entre la dirección raíz 199.160.0.96 y la dirección broadcasting 199.160.0.127.

### D- pertenece a la subred 4 que esta entre la dirección raíz 199.160.0.97 y la dirección broadcasting 199.160.0.128.

## 3) cuantas subredes se puede sacar si tenemos una máscara 255.255.255.192 para:

A-Clase C

B-Clase B

C-Clase A

## 4) Cual de los siguientes no pertenece a la misma subred si tenemos una mascara 255.255.255.240

A-172.16.4.99

B-172.16.4.111

C-172.16.4.113

D-172.168.4.104

E-Ninguna de las Anteriores.

## 5) Cual es el broadcasting, raíz y mascara de  subred para la direccion 10.27.33.14/19
