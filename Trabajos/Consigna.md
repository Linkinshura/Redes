# Packet Tracer - Investigue los modelos TCP/IP y OSI en acción

## Objetivos
Parte 1: Examine el tráfico web HTTP

Parte 2: Muestre elementos de la suite de protocolos TCP/IP

Aspectos básicos
Esta actividad de simulación está destinada a proporcionar una base para comprender el conjunto de protocolos TCP / IP y la relación con el modelo OSI. El modo de simulación le permite ver el contenido de datos que se envía a través de la red en cada capa.

A medida que los datos se mueven a través de la red, se desglosan en piezas más pequeñas y se identifican para que las piezas se puedan volver a juntar cuando lleguen al destino. A cada pieza se le asigna un nombre específico (unidad de datos de protocolo [PDU]) y se asocia con una capa específica de los modelos TCP / IP y OSI. El modo de simulación de Packet Tracer le permite ver cada una de las capas y la PDU asociada. Los siguientes pasos conducen al usuario a través del proceso de solicitud de una página web de un servidor web mediante utilizando la aplicaciónde navegador webdisponible en un PCcliente.

Aunque gran parte de la información mostrada se discutirá con más detalle más adelante, esta es una oportunidad para explorar la funcionalidad de Packet Tracer y poder visualizar el procesode encapsulación.

Instrucciones
Part 1: Examine el tráfico Web HTTP
En la Parte 1 de esta actividad, utilizará el modo de simulación de Packet Tracer (PT) para generar tráfico web y examinar HTTP.

Paso 1: Cambie del modo de simulación en tiempo real.
En la esquina inferior derecha de la interfaz de Packet Tracer hay botones que alternan entre el modo deTiempo Real y Simulación. PT siempre comienza en el modo de Tiempo Real, en el que los protocolos de red funcionan con tiempos realistas. Sin embargo, una característica poderosa de Packet Tracer le permite al usuario "detener el tiempo" al cambiar al modo de simulación. En el modo de simulación, los paquetes se muestran como sobres animados, el tiempo depende de los eventos y el usuario pasa por los eventos de red.

a.     Haga clic en el icono del modo de Simulación para cambiar del modo de Tiempo Real al modo de Simulación.

b.     Seleccione HTTP deEvent List Filters.

1)    Es posible que HTTP ya sea el único evento visible. Si es necesario, haga clic en el botón Edit Filters en la parte inferior del panel de simulación para mostrar los eventos visibles disponibles. Cambie la casilla de verificación Show All/None y observe cómo las casillas de verificación cambian de desmarcada a marcada o marcada a desmarcada, según el estado actual.

2)    Haga clic en la casilla de verificación Show All/None hasta que se borren todos los cuadros y luego seleccione HTTP en la pestaña Misc de la ventana Edit Filters. Haga clic en la X situada en la esquina superior derecha de la ventana para cerrar laventana Edit Filters Los eventos visibles ahora deben mostrar solo HTTP.

Step 2:Paso 2: generar tráfico web (HTTP).
Actualmente, el panel de simulación está vacío. Hay cinco columnas en la parte superior de la Event List dentro del Panel de simulación. A medida que se genera y avanza el tráfico los eventos aparecen en la lista.

Nota: El Servidor Web y el Cliente Web se muestran en el panel izquierdo. Los paneles se pueden ajustar en tamaño al pasar el cursor al lado de la barra de desplazamiento y arrastrar hacia la izquierda o hacia la derecha cuando aparece la flecha de dos puntas.

a.     Haga clic en el Cliente Web en el panel del extremo izquierdo.

b.     Haga clic en la pestaña Desktop y haga clic en el icono Web Browser para abrirlo.

c.     En el campo URL, ingrese www.osi.local y haga clic enGo.

Debido a que el tiempo en el modo de simulación es controlado por eventos, debe usar el botón Capture/Forward para mostrar eventos de red. El botón de captura hacia adelante se encuentra en el lado izquierdo de la banda azul que está debajo de la ventana de topología. De los tres botones, es el de la derecha.

d.     Haga clic en Capture/Forward cuatro veces. Debe haber cuatro eventos en el Event List.

## Pregunta:
Mire la página del navegador web del Cliente Web. ¿Cambió algo?

e.     Haga clic sobre la primer caja de color en Event List > bajo la columna Type . Puede ser necesario expandir el Panel de simulación o usar la barra de desplazamiento directamente debajo deEvent List.

Se muestra la ventana PDU Information at Device: Cliente Web. En esta ventana, solo hay dos pestañas (OSI Model y Outbound PDU Details) porque este es el comienzo de la transmisión. A medida que se examinen más eventos, se mostrarán tres pestañas, agregando una pestaña para Inbound PDU Details. Cuando un evento es el último evento en la secuencia de tráfico, solo se muestran las pestañas del OSI Model y Inbound PDU Details .

f.      Asegúrese de que la pestaña del OSI Model esté seleccionada.

Debajo de la columna Out Layers, haga clic en Layer 7.

Preguntas:
¿Qué información se enumera en los pasos numerados directamente debajo de los cuadros In Layers y Out Layers para Layer 7?

¿Cuál es el valor del Dst Port para Layer 4 en la columna Out Layers ?

¿Cual es el Dest? ¿IP para Layer 3 en la columna Out Layers?

¿Qué información se muestra en Layer 2 en la columna Out Layers ?

g.     Haga clic en la pestaña Outbound PDU Details

La información que figura en PDU Formatses reflejo de las capas del modelo TCP/IP.

Nota: La información que aparece en la sección Ethernet II de la pestaña Outbound PDU Details proporciona información aún más detallada que la que se muestra en Layer 2 en la pestañaOSI Model. Los Outbound PDU Details proporcionan información más descriptiva y detallada. Los valores bajo DEST MAC y SRC MAC dentro de la sección Ethernet II de PDU Detailsaparecen en la pestaña OSI Model bajo Layer 2, pero no se identifican como tales. Preguntas:

¿Cuál es la información común que figura en la sección IP de los PDU Details en comparación con la información que figura en la pestaña del OSI Model ? ¿Con qué capa está asociado?

¿Cuál es la información común que aparece en la sección TCP de PDU Details, en comparación con la información que aparece en la pestaña delOSI Model , y con qué capa está asociada?

¿Cuál es el host que aparece en la sección HTTP de los PDU Details? ¿Con qué capa se asociaría esta información en la pestaña del MOdelo OSI?

h.     Haga clic sobre la primer caja de color en Event List > bajo la columna Type . Solo Layer 1 está activa (sin atenuar). El dispositivo mueve la trama del búfer y lo coloca en la red.

i.      Avance al siguiente cuadro HTTP Type dentro de Event List y haga clic en la caja de color. Esta ventana contiene tanto en In Layers como Out Layers. Observe la dirección de la flecha directamente debajo de la columnaIn Layers ; apunta hacia arriba, indicando la dirección en la que viajan los datos. Desplácese por estas capas y tome nota de los elementos vistos anteriormente. En la parte superior de la columna, la flecha apunta a la derecha. Esto indica que el servidor ahora está enviando la información al cliente.

## Pregunta:
Comparando la información que se muestra en la columnaIn Layers con la de la columna Out Layers, ¿cuáles son las principales diferencias?

j.      Haga clic en la pestaña Inbound and Outbound PDU Details. Revise los detalles PDU.

k.     Haga clic sobre la última caja de color bajo la columna Info.

## Pregunta:
¿Cuántas pestañas se muestran con este evento? Explique.

### Parte 2: Muestre elementos del conjunto de Protocolos TCP/IP
En la Parte 2 de esta actividad, utilizará el modo Simulación de Packet Tracer para ver y examinar algunos de los otros protocolos que comprenden el conjunto TCP/IP.

### Step 1: View Additional Events
a.     Cierre cualquier ventana de información de PDU abierta.

b.     En elEvent List Filters > seccion Visible Events, haga clic en Show All/None.

## Pregunta:
¿Qué tipos de eventos adicionales se muestran?

Estas entradas adicionales desempeñan varios roles dentro del conjunto TCP/IP . El Protocolo de resolución de direcciones (ARP) solicita direcciones MAC para hosts de destino. DNS es responsable de convertir un nombre (por ejemplo, www.osi.local) a una dirección IP. Los eventos TCP adicionales son responsables de conectarse, acordar los parámetros de comunicación y desconectar las sesiones de comunicación entre los dispositivos. These protocols have been mentioned previously and will be further discussed as the course progresses. Currently there are over 35 possible protocols (event types) available for capture within Packet Tracer.

c.     Haga clic en el primer evento de DNS en la columna Type. Explore las pestañas OSI Model y PDU Detail y observe el proceso de encapsulación. Al mirar la pestaña OSI Model con Layer 7 resaltada, una descripción de lo que está ocurriendo se encuentra justo debajo de In Layers y Out Layers (“1. El cliente DNS envía una consulta DNS al servidor DNS."). Esta es información muy útil para ayudar a comprender lo que ocurre durante el proceso de comunicación.

d.     Haga clic en la pestaña Outbound PDU Details .

## Pregunta:
¿Qué información se indica en el campo NAME :en la sección de DNS QUERY?

e.     Haga clic en la ultima caja de color de Info de DNS en el event list.

## Preguntas:
¿En qué dispositivo se capturó la PDU?

¿Cuál es el valor que aparece junto a ADDRESS: en la sección DNS ANSWER de Inbound PDU Details?

f.      Busque el primer evento HTTP en la lista y haga clic en la caja de color del TCP event inmediatamente después de este evento. Resalte Layer 4 en la pestaña OSI Model.

## Pregunta:
En la lista numerada directamente debajo de In Layers y Out Layers, ¿cuál es la información que se muestra en los elementos 4 y 5?

TCP gestiona la conexión y desconexión del canal de comunicaciones junto con otras responsabilidades. Este evento en particular muestra que el canal de comunicación ha sido ESTABLECIDO.

g.     Haga clic en el último evento TCP. Resalte Layer 4 en la pestaña OSI Model. Examine los pasos enumerados directamente debajo de In Layers y Out Layers.

## Pregunta:
¿Cuál es el propósito de este evento, basado en la información proporcionada en el último elemento de la lista (debe ser el elemento 4)?

Preguntas de desafío
Esta simulación proporcionó un ejemplo de una sesión web entre un cliente y un servidor en una red de área local (LAN). El cliente realiza solicitudes a servicios específicos que se ejecutan en el servidor. El servidor debe estar configurado para escuchar en puertos específicos una solicitud del cliente. (Sugerencia: mire Layer 4 en la pestaña OSI Model para obtener información sobre el puerto).

Según la información que se inspeccionó durante la captura de Packet Tracer,¿qué número de puerto está escuchando el Servidor Webpara la solicitud web?

En cuál puerto esta el Servidor Web escuchando para una solicitud DNS ?
