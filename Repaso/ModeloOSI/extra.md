# 📘 Archivo 2 – Redes

---

# 🌐 Modelo TCP/IP

## 🧠 Definición
El **modelo TCP/IP** es un conjunto de protocolos que permite la comunicación entre dispositivos en una red, como Internet.  
Define cómo los datos se **formatean, envían, enrutan y reciben** entre sistemas. 0

---

## 📚 Capas del Modelo TCP/IP

### 1. Acceso a la Red
- Se encarga de la transmisión física de los datos.
- Incluye:
  - Hardware
  - Medios de transmisión
  - Direcciones MAC

---

### 2. Internet
- Se encarga del **direccionamiento lógico**.
- Determina la ruta de los datos (enrutamiento).
- Protocolo principal:
  - **IP**

---

### 3. Transporte
- Comunicación extremo a extremo.
- Control de errores y flujo de datos.

**Protocolos:**
- **TCP** → confiable (garantiza entrega)
- **UDP** → rápido (sin garantías)

---

### 4. Aplicación
- Interacción con el usuario.
- Incluye funciones de aplicación, presentación y sesión.

**Protocolos:**
- HTTP
- FTP
- DNS
- SMTP

---

# 📘 Conceptos Extra

## 🌐 Tipos de Redes

- **LAN (Local Area Network)** → red local  
- **MAN (Metropolitan Area Network)** → red de ciudad  
- **WAN (Wide Area Network)** → red global  

---

## 🔌 Medios de Transmisión

### Guiados (cableados)
- Par trenzado (UTP)
- Cable coaxial
- Fibra óptica

### No guiados (inalámbricos)
- Wi-Fi
- Bluetooth

---

## 📡 Dispositivos de Red

- **Hub** → envía datos a todos los dispositivos  
- **Switch** → envía datos al destino correcto usando MAC  
- **Router** → conecta redes diferentes usando IP  
- **Access Point** → permite conexión inalámbrica  

---

## 🧾 Direccionamiento

### Dirección IP
- Identifica un dispositivo dentro de una red. 1  
- Tipos:
  - IPv4
  - IPv6  

---

### Dirección MAC
- Identificación física única del dispositivo.
- No cambia.

---

## 📦 Protocolos

- **HTTP / HTTPS** → navegación web  
- **FTP** → transferencia de archivos  
- **DNS** → traduce nombres a direcciones IP  
- **DHCP** → asigna IP automáticamente  

---

## 🔌 Puertos

- Identifican servicios dentro de un dispositivo.
- Rango: **0 – 65535**

### Tipos:
- **0 – 1023** → bien conocidos  
- **1024 – 49151** → registrados  
- **49152 – 65535** → dinámicos