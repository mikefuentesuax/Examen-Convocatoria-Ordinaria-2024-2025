# Examen-Convocatoria-Ordinaria-2024-2025


### Pregunta 1. Modelos OSI y TCP/IP
- a) El modelo OSI esta formado por siete capas: la Física, la de Enalce, la Red de Transporte, la de Sesión, Presentación y Aplicación. Este es un módelo teoríco usado para estandarizar las comunicaciones. Este modelo usa tres capas, la de Sesión, Aplicación y Presentación. La capa de Sesión gestiona las comunicaciones, la de Presentación se encarga de los formatos y la representación de los datos y la de Aplicación proporciona los servicios de red al usuario.
 
     El modelo TCP/IP consta de cuatro o cinco capas: Acceso de Red, Internet, Transporte y Aplicación. Este modelo a diferencia del OSI está diseñado a protocolos que se usan.
A diferencia del modelo OSI, el TCP/IP agrupa todas las funciones en una sola, la capa de Aplicación.

- b) Las ventajas del modelo OSI son: la separación de los datos en diferentes capas.

     Las desventajas del modelo OSI son: es más complejo a la hora de usar, no se puede adaptar completamente y la separaciñon en capas hace que se gasten más recurso.
  
     Las ventajas del modelo TCP/IP son: es más flexible a la hora de implementarse, consume menos recurso al tener menos separación entre capas.
  
     Las desventajas del modelo TCP/IP son: al comprimir todos los datos en menos capas la información puede ser mas díficil de comprender.

### Pregunta 2. Función de la Capa de Transporte y Diferencias entre TCP y UDP
- a) En ambos modelos la capa de transporte se encarga de proporcionar una comunciación de extremo a extremo.

   Para garantizar la entrega de datos  se hace uso de la segementación y reensamblaje, la cual divide los datos en segementos pequeños para poder ser enviados y reensamblados al llegar. También se dispone de la multiplexación que permite a varias aplicaciones compartir la conexión de red.

   Entre los protocolos que garantizan el correcto funcionamiento están los ACKs que envía el receptor al emisor para confirmar la llegada de los segementos.

   Para el modelo OSI, el uso está destinado hacia aplicaciones que requieran un alata fiabilidad como el correo electrónico.

   Para el modelo TCTP/IP está destinado hacia aplicaiones con menos fiabildad y que se pueden permitir la pérdida de datos como el streaming en video.

- b)


### Pregunta 3. Protocolos de Aplicación y Resolución de Nombres
- a) Se usa el FTP. Como alternativa se puede usar el STFP por su cifrado o el HTTPS que añade una capa de seguridad  exxtra a través de SSL/TLS.

- b) Primero el usuario ingresa una URL, el navegador verifica el caché DNS local en caso de que todavía no haya caducado, en caso de que lo este en local se consulta con el servidor para obtener la informaciñon DNS del dominio, se envía al cliente y se establece conexión.

### Pregunta 4. Comunicación entre Dispositivos Usando TCP/IP

- Capa de Aplicación:

Proporciona los servicios directamente a las aplicaciones y gestiona la interacción entre las aplicaciones y la red.

- Capa de Transporte:

Establece la comunicación de extremo a extremo entre aplicaiones. Segmenta los datos, controla el flujo de datos, el control de errores y la multiplexación.

- Capa de Internet:

Establece el direccionamiento lógico, el enrutamiento dr paquetes entre redes y la fragmentación de garndes paquetes-

- Capa de Acceso a Red:

Combina las funcionalidades de las capas de Enlace de Datos y Física del modelo. Es responsable de la transmisión de bits a través del medio físico y del acceso al medio. También maneja el direccionamiento físico.

### Pregunta 5. Cálculo de la Tasa de Transmisión Máxima (Fórmula de Shannon)

La tasa máxima de transmisión = 3.32 Gbps

### Pregunta 6. Ubicación de Portadoras para Eficiencia Espectral

- a) Frecuencia de la portadora anterior = 1.2 GHz - 0.3 GHz = 0.9 GHz

- b) La frecuencia de la portadora posterior = 1.2 GHz + 0.3 GHz = 1.5GHz

Evita interferencia, se maximiza la capacidad del Sistema, 

### Pregunta 7. Identificación de Modulación a partir del BER

1- BPSK

2- QPSK

3- 16-QAM

4- 64-QAM

5- 256-QAM

A mayor cantidad de símbolos por baudio, menor separación entre ellos en el plano y más susceptible en el ruido.

### Pregunta 8. Eficiencia del Sistema de Encapsulamiento
a) Datos capa 5 = 2048 bytes

3 cabeceras (48 bytes × 3) = 144 bytes
Total = 2048 + 144 = 2192 bytes

b) Cada trama de capa 2 = 512 bytes
Número de tramas = 2192 / 512 ≈ 5 tramas (redondeando hacia arriba)

c) Capa 1 añade por cada 4 bytes:

2 bytes (inicio) + 1 byte (parada) + 2 bytes (CRC) = 5 bytes adicionales
Por cada 4 bytes → 5 bytes sobrecarga
Sobre la carga útil: 5 / 9 ≈ 55.6% de sobrecarga

d) Eficiencia = Datos útiles / Total transmitido
Eficiencia ≈ 44.4%

### Pregunta 9. Cálculo de Ruta Más Corta
a) Algoritmo de Dijkstra: Encuentra la ruta más corta desde un nodo origen a todos los demás en un grafo ponderado.

b)

Dijkstra: Preciso y eficiente, pero requiere conocimiento global de la red.

Flooding: Simple, pero genera mucho tráfico redundante.

Pregunta 10. Broadcast y Rango de Hosts

a)

IP: 172.29.152.0

Máscara: 255.255.248.0 → /21

Broadcast: 172.29.159.255

b)

IP: 172.22.53.199

Máscara: 255.255.252.0 → /22

Rango válido: 172.22.52.1 a 172.22.55.254

### Pregunta 11. Última Dirección Válida y Número de Hosts

a)

Subred: 172.30.67.192/26

Broadcast: 172.30.67.255

Última válida: 172.30.67.254

b)

Máscara /26 → 2⁶ = 64 direcciones

Hosts útiles: 62

### Pregunta 12. Segmentación en Subredes

a)

Dirección: 172.18.171.190

Máscara /23 → Bloque = 172.18.170.0/23

b)

Fórmula: Número de subredes = 2^s

Para 4 subredes → s = 2 bits

Se pueden crear 4 subredes si se prestan 2 bits a la máscara.

### Pregunta 13. Conexión TCP

a) Three-Way Handshake:

SYN

SYN-ACK

ACK

b) Four-Way Handshake:

FIN

ACK

FIN

ACK

### Pregunta 14. Multiplexación en TCP

a) Multiplexación descendente: Muchos procesos usan un mismo canal TCP. Ej: Navegador con varias pestañas HTTP.

b) Multiplexación ascendente: TCP usa puertos distintos para identificar procesos destino. Esencial para entregar datos correctamente.

### Pregunta 15. Tamaño de Ventana y Congestión

a) RTT = 50 ms = 0.05 s

b) Ventana óptima = 100 Mbps × 0.05 s = 5 Mb = 625 KB

c) Número de MSS = 625 KB / 1500 B ≈ 417 segmentos

d) Este valor define cuántos datos se pueden enviar sin recibir ACKs. TCP ajusta la ventana para evitar congestión.

### Pregunta 16. Control de Congestión TCP

Slow Start: Incrementa ventana exponencialmente al inicio. Evita saturar la red.

Nagle: Agrupa pequeños paquetes. Reduce overhead.

Clark: Evita enviar si no hay espacio en buffer. Previene congestión.

### Pregunta 17. Correo y HTTP/FTP

a) Protocolos de correo:

POP3: Descarga, elimina del servidor

IMAP: Acceso remoto, sincronizado

SMTP: Envía correos

b) HTTP: Métodos como GET, POST. Conexión única.
FTP: Usa 2 conexiones (control + datos). Más complejo.

### Pregunta 18. Streaming y VoIP

a) Tipos de streaming:

UDP Streaming: En tiempo real, sin reenvío (ej: IPTV)

HTTP Streaming: Videos desde servidores web (ej: YouTube)

DASH: Calidad adaptativa (ej: Netflix)

b) VoIP: Voz convertida a paquetes IP. Problemas:

Retardo: Se mitiga con jitter buffers

Pérdida de paquetes: Se compensa con FEC o reenvío selectivo

### Pregunta 19. Congestión y Calidad de Servicio

a) Técnicas:

Buffering: Suaviza variaciones de red

DiffServ: Marca prioridad de paquetes

b) Modelos:

Best-Effort: No garantiza QoS (ej: web, email)

Servicios Multiclase: Priorización (ej: videollamadas)

Pregunta 20. Problemas de Seguridad
Confidencialidad: Evitar espionaje → Cifrado

Autenticación: Verificar identidad → Contraseñas, certificados

No repudio: Garantizar autoría → Firmas digitales

Integridad: Detectar cambios → Hash (ej: SHA)

### Pregunta 21. Cifrado Simétrico vs. Asimétrico

Característica	Simétrico	Asimétrico

Claves	1 compartida	2 (pública/privada)

Velocidad	Rápido	Más lento

Ejemplos	AES, DES	RSA, ECC

Aplicaciones	Datos locales	Intercambio de claves

### Pregunta 22. Funcionamiento RSA

a) Generación de claves:

primos: p = 3, q = 11

n = 3×11 = 33, φ(n) = (3−1)(11−1) = 20

Elegir e = 7 

d ≡ 1 mod 20 → d = 3

b) Ejemplo:

Cifrar M = 4 → C = M^e mod n = 4^7 mod 33 = 16

Descifrar C = 16 → M = C^d mod n = 16^3 mod 33 = 4

#### Pregunta 23. Firewalls, VPN, IPSec y SSL/TLS

a) Firewalls:

Filtrado de paquetes: Revisa cabeceras

Firewall de estado: Revisa conexiones completas

b)

VPN: Crea túnel seguro

IPSec: Cifra tráfico IP directamente

Ejemplo: Acceso remoto seguro

c) SSL/TLS:

Cifra conexiones web

Usa certificados y claves para garantizar seguridad

### Pregunta 24. DNS Spoofing y DNSSEC

a) DNS Spoofing:

Ataque que falsifica respuestas DNS

Puede redirigir a sitios maliciosos

b) DNSSEC:

Firma digital en respuestas DNS

Verifica autenticidad y evita manipulaciones
