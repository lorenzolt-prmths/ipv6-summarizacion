# Sumarización de rutas IPv6

## Descripción
En este proyecto se ha diseñado y configurado una red con varios routers utilizando direcciones IPv6 en Cisco Packet Tracer.

Se ha implementado la sumarización de rutas IPv6 para agrupar varias redes en prefijos resumidos, reduciendo el tamaño de la tabla de rutas y optimizando el enrutamiento entre routers.

Se ha verificado el funcionamiento mediante la tabla de rutas IPv6, ping entre redes y traceroute.

## Topología de red
La red está formada por varios routers conectados mediante enlaces serial y diferentes redes IPv6 conectadas a cada router.

![Topología](img/topologia.png)

## Sumarización IPv6
En este proyecto se han agrupado varias redes IPv6 en prefijos resumidos para reducir el número de rutas en la tabla de routing.

Ejemplo de rutas resumidas en la tabla de routing:
- 2003:FFFF:1234:FFF0::/60
- 2017:1234:5FFF:AA80::/57

La sumarización permite:
- Reducir el número de rutas
- Simplificar la tabla de routing
- Mejorar la organización del enrutamiento
- Optimizar el tráfico de routing

## Tabla de routing IPv6
Se ha comprobado la tabla de rutas IPv6 con el comando:

show ipv6 route
![ipv6-route](img/ipv6-route.png)

En la tabla de rutas se pueden observar:
Rutas conectadas (C)
Rutas locales (L)
Rutas estáticas (S)
Rutas resumidas

Pruebas de conectividad
Se ha comprobado la conectividad entre redes IPv6 mediante el comando:
ping 2001:A:A:A::2
Esto verifica que existe conectividad entre diferentes redes IPv6 a través de los routers.
También se pueden comprobar los saltos entre routers mediante:
traceroute 2001:A:A:A::2

Comandos utilizados
Algunos comandos utilizados en los routers:
ipv6 unicast-routing
ipv6 route
show ipv6 route
show ipv6 interface brief
show ipv6 neighbors
Tecnologías utilizadas
Cisco Packet Tracer
IPv6
Routing
Sumarización de rutas
Redes LAN/WAN
Objetivos del proyecto
Configurar direcciones IPv6
Habilitar enrutamiento IPv6
Configurar sumarización de rutas IPv6
Reducir el tamaño de la tabla de rutas
Verificar conectividad mediante ping y traceroute
