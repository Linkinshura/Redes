# Trafico TCP/IP

## Inicio
La informacion es almacenada en diferentes paquetes con diversos tamaños gracias a la IP, cada paquete requiere una identificacion, una vez terminado son enviados a la LAN.

## Camino en LAN
Dentro de esta los paquetes pueden colisionar por falta de control del trafico de ellos. El router extrae los paquetes de esta red identificandolos por sus direcciones y puede moverlos a otra red.

## Camino por Proxy

Una vez que el router suelta los paquetes estos terminan navegando por la Intranet corporativa hacia el switch donde este los guía a su camino correspondiente, una vez llegan a su destino la interfaz de red es la encargada de enviarlos al proxy, quien cumple su función de  compartir y establecer entre varios usuarios una conexión a internet.
El proxy extrae de el paquete la URL y si esta es admitida el paquete se envia al internet, en caso de no ser admitida esa dirección es destruida, finalmente el paquete vuelve al LAN para llegar al Firewall(previene introvisiones de internet y evita que información privada sea publica en internet) para luego ser recogido devuelta por el Router donde algunos paquetes al superar el ancho de banda pueden terminar destruidos, los que logran pasar llegan al internet finalmente.

## Acceso a la PC
Luego de aca transita libremente por el internet, para llegar a el PC que solicita esa URL, en este hay otro firewall donde solo permite la entrada de URL que cumplen con el criterio de selección, manteniendo únicamente los puertos 80 y 25 abiertos. El puerto 80 es la entrada de paquetes de internet a la web mientras que el 25 esta destinado a los correos. Dentro del firewall los paquetes son filtrados nuevamente  donde los rechazados terminan destruidos dentro de estos. Los paquetes que logran superar este filtro llegan a la interfaz para ir al servidor web.

## Reciclamiento
Estos paquetes terminan entregando su información a la aplicación web y luego es utilizado para reciclarse y luego llenarse de la información solicitada para volver a realizar su viaje devuelta hasta el administrador de internet donde es entregada la información solicitada
