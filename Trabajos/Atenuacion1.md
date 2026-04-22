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

## 1)
LC=10
Ne=4
Nc=2

### 1550Mhz:

AT= Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT= 2x0.5 (1.0) + 4x0.1 (0.4) + 10x0.25 (2.5) + 10x0.01 (0.1)  
AT = 4.0 Mhz  

No funciona correctamente la atenuacion

### 1310Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=2x0.75 (1.5) + 4x0.25 (1.0) + 10x0.5 (5.0) + 10x0.01 (0.1)  
AT= 7.6Mhz  

Funciona correctamente la atenuacion

## 2)
LC=40
Ne=6
Nc=2

### 1550Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=2x0.5 (1.0) + 6x0.1 (0.6) + 40x0.25 (10.0) + 40x0.01 (0.4)  
AT= 12.0Mhz  

Funciona correctamente la atenuacion

### 1310:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=2x0.75 (1.5) + 6x0.25 (1.5) + 40x0.5 (20.0) + 40x0.1 (4.0)  
AT=27.0Mhz  

No funciona correctamente la atenuacion

## 3)
LC=3
Ne=2
Nc=2

### 1550Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=2x0.5 (1.0) + 2x0.1 (0.2) + 3x0.25 (0.75) + 3x0.01 (0.03)  
AT= 1.98Mhz  

No funciona correctamente la atenuacion

### 1310:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=2x0.75 (1.5) + 2x0.25 (0.5) + 3x0.5 (1.5) + 3x0.1 (0.3)  
AT=3.8Mhz  

No funciona correctamente la atenuacion

## 4)
### Tramo A:
LC=10
Ne=4
Nc=2

#### 1550Mhz:

AT= Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT= 2x0.5 (1.0) + 4x0.1 (0.4) + 10x0.25 (2.5) + 10x0.01 (0.1)  
AT = 4.0 Mhz  

No funciona correctamente la atenuacion

#### 1310Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=2x0.75 (1.5) + 4x0.25 (1.0) + 10x0.5 (5.0) + 10x0.01 (0.1)  
AT= 7.6Mhz  

Funciona correctamente la atenuacion

### Tramo B:

LC=14
Ne=6
Nc=2

#### 1550Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=2x0.5 (1.0) + 6x0.1 (0.6) + 14x0.25 (3.5) + 14x0.01 (0.14)  
AT= 5.24Mhz  

No funciona correctamente la atenuacion

#### 1310:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=2x0.75 (1.5) + 6x0.25 (1.5) + 14x0.5 (7.0) + 14x0.1 (1.4)  
AT=11.4Mhz  

Funciona correctamente la atenuacion

### Tramo C:
LC=9
Ne=8
Nc=2

####1550Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=2x0.5 (1.0) + 8x0.1 (0.8) + 9x0.25 (2.25) + 9x0.01 (0.09)  
AT= 4.14Mhz  

No funciona correctamente la atenuacion

#### 1310:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=2x0.75 (1.5) + 8x0.25 (2.0) + 9x0.5 (4.5) + 9x0.1 (0.9)  
AT=8.9Mhz  

Funciona correctamente la atenuacion

### Total:
LC=33
Ne=18
Nc=4

#### 1550Mhz:

AT= Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT= 4x0.5 (2.0) + 18x0.1 (1.8) + 33x0.25 (8.25) + 33x0.01 (0.33)  
AT = 12.38Mhz  

Funciona correctamente la atenuacion

#### 1310Mhz:

AT=Nc*Atc+Ne*Ate+LC*AtC+LC*0.01  
AT=4x0.75 (3.0) + 18x0.25 (4.5) + 33x0.5 (16.5) + 33x0.01 (0.33)  
AT= 24.33Mhz  

Funciona correctamente la atenuacion