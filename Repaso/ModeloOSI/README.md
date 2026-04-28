# 📘 Modelo OSI

## 🧠 Definición
El **Modelo OSI (Open Systems Interconnection)** es un modelo conceptual que divide la comunicación en redes en **7 capas**, permitiendo estandarizar cómo los dispositivos se comunican entre sí. 

También sirve para **identificar problemas en redes** separando cada función en niveles. 

---

## 🧱 Capas del Modelo OSI

### 1. Capa Física (Physical)
- Transmisión de **bits (0 y 1)**.
- Medio físico: cables, señales eléctricas, ópticas o inalámbricas.
- Ejemplo: cable UTP, fibra óptica.

---

### 2. Capa de Enlace de Datos (Data Link)
- Comunicación entre dispositivos conectados directamente.
- Maneja **tramas (frames)**.
- Usa direcciones **MAC**.
- Detecta errores.

---

### 3. Capa de Red (Network)
- Maneja **paquetes (packets)**.
- Se encarga del **direccionamiento lógico (IP)**.
- Determina rutas (routing).

---

### 4. Capa de Transporte (Transport)
- Maneja **segmentos**.
- Comunicación extremo a extremo.
- Control de errores y flujo.
- Protocolos:
  - TCP → confiable
  - UDP → rápido

---

### 5. Capa de Sesión (Session)
- Establece, mantiene y finaliza sesiones.
- Controla la comunicación entre dispositivos.

---

### 6. Capa de Presentación (Presentation)
- Traduce los datos.
- Funciones:
  - Codificación
  - Compresión
  - Cifrado

---

### 7. Capa de Aplicación (Application)
- Interacción directa con el usuario.
- Servicios de red.
- Protocolos: HTTP, FTP, SMTP, DNS.

---

## 🔄 Funcionamiento

### Encapsulación
- Los datos bajan desde la capa 7 a la 1.
- Cada capa agrega información (headers).
### Desencapsulación
- Los datos suben desde la capa 1 a la 7.
- Cada capa elimina su información correspondiente.

---

## 📊 Unidades de Datos (PDU)

| Capa | Unidad |
|------|--------|
| Aplicación / Presentación / Sesión | Datos |
| Transporte | Segmentos |
| Red | Paquetes |
| Enlace de Datos | Tramas |
| Física | Bits |

---

## 🎯 Importancia
- Estandariza la comunicación en redes.
- Facilita la resolución de problemas.
- Permite interoperabilidad entre sistemas distintos.