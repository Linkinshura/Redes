# Subneteo — Explicación Completa

## ¿Qué es el subneteo?

El subneteo consiste en dividir una red IP grande en varias redes más pequeñas llamadas **subredes**.

Sirve para:

- Organizar mejor una red
- Reducir tráfico
- Mejorar seguridad
- Aprovechar direcciones IP

---

# Conceptos importantes

| Concepto | Explicación |
|---|---|
| Dirección de red | Primera IP de la subred |
| Broadcast | Última IP de la subred |
| Hosts válidos | IPs utilizables entre red y broadcast |
| Máscara de subred | Define qué parte es red y qué parte es host |
| Gateway | IP del router dentro de la subred |

---

# Fórmulas importantes

## Hosts válidos

```txt
2^h - 2
```

Donde:

- `h` = cantidad de bits para hosts
- Se resta 2 porque:
  - 1 IP es la dirección de red
  - 1 IP es broadcast

---

## Cantidad de subredes

```txt
2^s
```

Donde:

- `s` = bits prestados para subneteo

---

## Tamaño del salto

```txt
256 - máscara
```

Se usa el último octeto de la máscara.

---

# Tabla rápida de máscaras

| CIDR | Máscara decimal | Hosts |
|---|---|---|
| /24 | 255.255.255.0 | 254 |
| /25 | 255.255.255.128 | 126 |
| /26 | 255.255.255.192 | 62 |
| /27 | 255.255.255.224 | 30 |
| /28 | 255.255.255.240 | 14 |
| /29 | 255.255.255.248 | 6 |

---

# ¿Cómo sale el 192?

La máscara `/26` significa:

```txt
26 bits en 1
```

En binario:

```txt
11111111.11111111.11111111.11000000
```

El último octeto:

```txt
11000000
```

Se convierte sumando:

```txt
128 + 64 = 192
```

Entonces:

```txt
255.255.255.192
```

---

# Ejercicio Completo

## Datos

Red:

```txt
192.168.1.0/24
```

Necesitamos:

```txt
50 hosts por subred
```

---

# PASO 1 — Calcular hosts

Usamos:

```txt
2^h - 2
```

Buscamos el primer número que alcance para 50.

| Bits host | Resultado | ¿Alcanza? |
|---|---|---|
| 5 | 30 | ❌ |
| 6 | 62 | ✅ |

Entonces:

```txt
Necesitamos 6 bits para hosts
```

---

# PASO 2 — Calcular máscara

IPv4 tiene:

```txt
32 bits
```

Si usamos 6 para hosts:

```txt
32 - 6 = 26
```

Entonces:

```txt
/26
```

Máscara decimal:

```txt
255.255.255.192
```

---

# PASO 3 — Calcular cantidad de subredes

La red original era:

```txt
/24
```

Ahora es:

```txt
/26
```

Bits prestados:

```txt
26 - 24 = 2
```

Entonces:

```txt
2^2 = 4 subredes
```

---

# PASO 4 — Calcular salto

Usamos:

```txt
256 - 192 = 64
```

El salto será:

```txt
64
```

---

# PASO 5 — Crear subredes

Las redes avanzan de 64 en 64:

```txt
0
64
128
192
```

---

# Subred 1

## Dirección de red

```txt
192.168.1.0
```

## Primer host

```txt
192.168.1.1
```

## Último host

```txt
192.168.1.62
```

## Broadcast

```txt
192.168.1.63
```

---

# Subred 2

## Dirección de red

```txt
192.168.1.64
```

## Hosts válidos

```txt
192.168.1.65 - 192.168.1.126
```

## Broadcast

```txt
192.168.1.127
```

---

# Subred 3

## Dirección de red

```txt
192.168.1.128
```

## Hosts válidos

```txt
192.168.1.129 - 192.168.1.190
```

## Broadcast

```txt
192.168.1.191
```

---

# Subred 4

## Dirección de red

```txt
192.168.1.192
```

## Hosts válidos

```txt
192.168.1.193 - 192.168.1.254
```

## Broadcast

```txt
192.168.1.255
```

---

# Tabla Final

| Subred | Hosts válidos | Broadcast |
|---|---|---|
| 192.168.1.0 | 192.168.1.1 - 192.168.1.62 | 192.168.1.63 |
| 192.168.1.64 | 192.168.1.65 - 192.168.1.126 | 192.168.1.127 |
| 192.168.1.128 | 192.168.1.129 - 192.168.1.190 | 192.168.1.191 |
| 192.168.1.192 | 192.168.1.193 - 192.168.1.254 | 192.168.1.255 |

---

# Método rápido mental

## 1. Calcular hosts

```txt
2^h - 2
```

---

## 2. Sacar máscara

```txt
32 - h
```

---

## 3. Calcular salto

```txt
256 - máscara
```

---

## 4. Enumerar redes

Ir sumando el salto.

---

# Potencias de 2 importantes

| Potencia | Resultado |
|---|---|
| 2³ | 8 |
| 2⁴ | 16 |
| 2⁵ | 32 |
| 2⁶ | 64 |
| 2⁷ | 128 |
| 2⁸ | 256 |

---

# Resumen Final

| Hosts necesarios | Máscara | Hosts disponibles |
|---|---|---|
| 14 | /28 | 14 |
| 30 | /27 | 30 |
| 62 | /26 | 62 |
| 126 | /25 | 126 |
