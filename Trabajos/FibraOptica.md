# Trabajo Práctico Fibra Óptica Redes

## Consigna:

1-Investigar los tipos de fibra óptica (mono-modo, hay 2 tipos de multi-modo), deben buscar sus diferencias técnicas(como funciona, distancias, frecuencia máxima, velocidades).

2-¿Que es Refracción y Reflexión?¿Cómo afecta a la fibra óptica?

3-¿Que tipos de conectores existen para cada tipo fibra óptica, y cuales son los mas usados en una conexión de hogar?

4-¿Que es la Atenuación de Fibra Óptica?¿Cual es la medida utilizada para la Atenuación?





5-La atenuación de Fibra Óptica se mide de la siguiente manera:
 At=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
Nc=Numero de Conectores
Atc=Atenuación de Conectores
Ne= Numero de Empalmes
Ate=Atenuación de Empalmes
LC=Largo del Cable(KM)
AtC= Atenuación por KM
0.01= Se considera este numero como el error externo debido a dobles o errores dentro del cable.
La atenuación depende de la frecuencia esta se mide en Mhz y su generación en Decibelios 
Por ejemplo:
Para 1550Mhz
Conectores:0.5dB
Empalmes:0.1dB
Cable:0.25dB
Mientras que para 1310Mhz
Conectores:0.75dB
Empalmes:0.25dB
Cable:0.5dB
entonces usando estas dos  medidas calcular un tramo de cable instalado en 400KM con 2 conectores 8 empalmes en ambas frecuencias.

Respuestas:

1)

## Fibra Monomodo(SMF): 
Es una fibra de un diámetro del núcleo interno de solo 9 microM, esta permite propagar de un solo modo de luz, a su vez minimiza la perdida de señal y es compatible con aplicaciones de alto ancho de banda a largas distancias, logrando una mayor velocidad, esta es utilizada para telecomunicaciones de alta velocidad y larga distancia


## Fibra Multimodo(MMF):
Es una fibra de un diámetro del núcleo interno de 50 o 62,5 microM, con multiples modos de luz, lo que la convierte en la ideal a cortas distancias, esta es utilizada mas para redes LAN, centros de datos,etc.

Estas se dividen en 2 tipos:

### Indice Escalonado:
Poseen un índice de refracción uniforme en el núcleo, El índice de refracción disminuye la interfaz núcleo-revestimiento, generando que el índice de refracción del revestimiento sea menor que el del núcleo.

### Indice Gradual:
Poseen un índice de refracción del núcleo que disminuye a medida que se aleja del centro, aproximándose gradualmente al índice de refracción del revestimiento en la interfaz.


Monomodo-Multimodo

Indices

2)
## Reflexión: 
Es el cambio de dirección de los rayos de luz que ocurre en un mismo medio después de incidir sobre la superficie de un medio distinto

## Refracción: 
Es el cambio de dirección de los rayos de luz que ocurre tras pasar estos de un medio a otro en que la luz se propaga con distinta velocidad.

Debido a los materiales con los cuales esta formada la fibra óptica en esta se genera un índice mayor de refracción en el núcleo que en el revestimiento, produciendo una Reflexión Interna Total, debido a que la luz se refleja pero no es capaz de atravesar la superficie entre ambos medios

ReflexionYRefraccion

3)
Existen diversos tipos, dependiendo el tipo de pulido del terminal óptico, Los mas usados son:

## FC(Ferrule Connector):
Es un conector roscado con una fijación muy resistente a vibraciones, por ello se utiliza en aplicaciones sometidas a movimiento y en inmstrumentos de precisión

## ST(Straght Tip):
Es similar pero su ajuste es en forma de montura de Bayoneta

## LC(Lucent Connector):
Ajuste similar a un RJ45 pero mas seguro y compacto que el SC, permitiendo mayores densidades de conectores en racks, paneles y FTTH

## SC(Suscriptor Connector):
Ajuste rápido a presión, compacto permitiendo integrar densidades grandes de conectores por instrumento

Conectores

4)
Es la perdida de potencia o intensidad que sufre la señal lumínica al propagarse a travez del cable, esto debido a factores como la absorción de luz, dispersión o dobleces y limita la distancia de transmisión

Su medida estándar es dB/km, ósea el Decibelio por Kilometro


5)
AT=1550Mhz
Atc=0.5
Ate=0.1
AtC=025
LC=400
Ne=8
Nc=2

1550Mhz = Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
1550Mhz = 2*0.5+8*0.1+400*0.25+400*0.01

#### 1550MHz = 105.8 dB

AT=1310MhZ
Atc=0.75
Ate=0.25
AtC=0.5
LC=400
Ne=8
Nc=2
1310= 2*0.75+8*0.25+400*0.5+400*0.01

#### 1310 MHz = 207.5 dB 
