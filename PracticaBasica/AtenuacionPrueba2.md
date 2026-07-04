# Datos del ejercicio

Frecuencia: **2100 MHz**

- Conectores (Nc): **4**
- ATC (Conectores): **0,02 dB**
- ATE (Empalmes): **0,1 dB**
- ATc (Cable): **0,05 dB/km**

## Fórmula

```text
At = Nc × ATC + Ne × ATE + LC × ATc + LC × 0,01
```

Donde:

- At = Atenuación Total
- Nc = Número de conectores
- ATC = Atenuación de conectores
- Ne = Número de empalmes
- ATE = Atenuación de empalmes
- LC = Longitud del cable (km)
- ATc = Atenuación del cable
- 0,01 = Error externo del cable

---

# Tramo A

Datos:

- Empalmes = 14
- Cable = 150 km

## Cálculo

```text
At = (4 × 0,02) + (14 × 0,1) + (150 × 0,05) + (150 × 0,01)

At = 0,08 + 1,4 + 7,5 + 1,5

At = 10,48 dB
```

**Resultado Tramo A: 10,48 dB**

---

# Tramo B

Datos:

- Empalmes = 4
- Cable = 90 km

## Cálculo

```text
At = (4 × 0,02) + (4 × 0,1) + (90 × 0,05) + (90 × 0,01)

At = 0,08 + 0,4 + 4,5 + 0,9

At = 5,88 dB
```

**Resultado Tramo B: 5,88 dB**

---

# Tramo C

Datos:

- Empalmes = 14
- Cable = 300 km

## Cálculo

```text
At = (4 × 0,02) + (14 × 0,1) + (300 × 0,05) + (300 × 0,01)

At = 0,08 + 1,4 + 15 + 3

At = 19,48 dB
```

**Resultado Tramo C: 19,48 dB**

---

# Atenuación Total

```text
At Total = 10,48 + 5,88 + 19,48

At Total = 35,84 dB
```

# Resultado Final

| Tramo | Atenuación |
|--------|-----------:|
| A | **10,48 dB** |
| B | **5,88 dB** |
| C | **19,48 dB** |
| **Total** | **35,84 dB** |
