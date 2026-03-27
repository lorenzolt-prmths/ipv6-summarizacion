# 🌐 Sumarización de rutas IPv6

## 📌 Descripción
En este proyecto se ha diseñado y configurado una red con varios routers utilizando direcciones IPv6 en Cisco Packet Tracer.

Se ha implementado la **sumarización de rutas IPv6** para agrupar varias redes en prefijos resumidos, reduciendo el tamaño de la tabla de rutas y optimizando el enrutamiento entre routers.

Se ha verificado el funcionamiento mediante:
- Tabla de rutas IPv6
- Ping entre redes
- Traceroute

---

## 🗺️ Topología de red
La red está formada por varios routers conectados mediante enlaces serial y diferentes redes IPv6.

![Topología](img/topologia.png)

---

## 📦 Sumarización IPv6
En este proyecto se han agrupado varias redes IPv6 en prefijos resumidos para reducir el número de rutas.

Ejemplos de rutas resumidas:
- `2003:FFFF:1234:FFF0::/60`
- `2017:1234:5FFF:AA80::/57`

La sumarización permite:
- Reducir el número de rutas
- Simplificar la tabla de routing
- Mejorar la eficiencia del enrutamiento

---

## 📊 Tabla de routing IPv6
Se ha comprobado la tabla de rutas con el comando:

show ipv6 route
![ipv6-routing](img/ipv6-route.png)

En la tabla se observan:
C → Connected
L → Local
S → Static (incluyendo rutas resumidas)

## 🧪Pruebas de conectividad
Se ha verificado la conectividad entre redes mediante:
- ping 2001:A:A:A::2
Resultado:
- Conectividad correcta entre redes IPv6
- 0% de pérdida de paquetes

![ping](img/ping.png)

También se puede comprobar el camino de los paquetes con:
traceroute 2001:A:A:A::2

![trace-route](img/traceroute.png)

## 🛠️ Comandos utilizados
- ipv6 unicast-routing
- ipv6 route
- show ipv6 route
- show ipv6 interface brief
- show ipv6 neighbors

## ⚙️ Tecnologías utilizadas
- Cisco Packet Tracer
- IPv6
- Routing
- Sumarización de rutas
- Redes LAN/WAN
## 🎯 Objetivos del proyecto
- Configurar direcciones IPv6
- Habilitar enrutamiento IPv6
- Aplicar sumarización de rutas
- Reducir el tamaño de la tabla de routing
- Verificar conectividad entre redes
