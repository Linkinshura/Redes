# Ejercicios de Atenuacion 1
Teniendo en cuenta el siguiente cuadro realizar los ejercicios:
1550Mhz
Conectores:0.5dB
Empalmes:0.1dB
Cable:0.25dB
1310Mhz
Conectores:0.75dB
Empalmes:0.25dB
Cable:0.5dB
La atenuación debe medir entre 7-25dB si supera la red es invalida
## 1-Tenemos una red con 2 conectores y 4 empalmes que recorren 10km se puede realizar y con que transferencia?
## 2-Tenemos una red con 2 conectores y 6 empalmes que recorren 40km se puede realizar y con que transferencia?
## 3-Tenemos una red con 2 conectores y 2 empalmes que recorren 3km se puede realizar y con que transfrecencia?
## 4-Tenemos una red con 4 conectores dividido de la siguiente manera:
### Tramo A: 2 conectores(A-B) con 4 empalmes que recorren 10Km 
### Tramo B: 2 conectores(A-C) con 6 empalmes y 14Km
### Tramo C: 2 conectores (B-C) con 8 empalmes y 9Km.
### ¿Cuánto es la atenuación de cada tramo y cual es la total?


## 1)
LC=10
Ne=4
Nc=2

### 1550Mhz:

AT= Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT= 2*0.5+4*0.1+10*0.25+10*0.01
AT = 4.0 Mhz

No funciona correctamente la atenuacion

### 1310Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=2*0.75+4*0.25+10*0.5+10*0.01
AT= 7.6Mhz

Funciona correctamente la atenuacion

## 2)
LC=40
Ne=6
Nc=2

### 1550Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=2*0.5+6*0.1+40*0.25+40*0.01
AT= 12.0Mhz

Funciona correctamente la atenuacion

### 1310:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=2*0.75+6*0.25+40*0.5+40*0.1
AT=27.0Mhz

No funciona correctamente la atenuacion

## 3)
LC=3
Ne=2
Nc=2

### 1550Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=2*0.5+2*0.1+3*0.25+3*0.01
AT= 1.98Mhz

No funciona correctamente la atenuacion

### 1310:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=2*0.75+2*0.25+3*0.5+3*0.1
AT=3.8Mhz

No funciona correctamente la atenuacion

## 4)
### Tramo A:
LC=10
Ne=4
Nc=2

#### 1550Mhz:

AT= Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT= 2*0.5+4*0.1+10*0.25+10*0.01
AT = 4.0 Mhz

No funciona correctamente la atenuacion

#### 1310Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=2*0.75+4*0.25+10*0.5+10*0.01
AT= 7.6Mhz

Funciona correctamente la atenuacion

### Tramo B:

LC=14
Ne=6
Nc=2

#### 1550Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=2*0.5+6*0.1+14*0.25+14*0.01
AT= 5.24Mhz

No funciona correctamente la atenuacion

#### 1310:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=2*0.75+6*0.25+14*0.5+14*0.1
AT=11.4Mhz

Funciona correctamente la atenuacion

### Tramo C:
LC=9
Ne=8
Nc=2

####1550Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=2*0.5+8*0.1+9*0.25+3*9.01
AT= 31.08Mhz

No funciona correctamente la atenuacion

#### 1310:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=2*0.75+8*0.25+9*0.5+9*0.1
AT=8.9Mhz

Funciona correctamente la atenuacion

### Total:
LC=33
Ne=18
Nc=4

#### 1550Mhz:

AT= Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT= 4*0.5+18*0.1+33*0.25+33*0.01
AT = 12.38Mhz

Funciona correctamente la atenuacion

#### 1310Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01
AT=4*0.75+18*0.25+33*0.5+33*0.01
AT= 24.33Mhz

Funciona correctamente la atenuacion