# Sprint 8 - Alta Disponibilidad

El objetivo de este sprint es implementar conocimientos sobre balanceo de carga con Apache, que realizará la tarea de proxy inverso y balanceador de carga.

## US12: Proxy Inverso con Apache

**Fecha Tope: 4 de marzo**

1. Configuración de Apache como Proxy Inverso.
   - Redirige las peticiones al servidor final utilizando Apache como proxy inverso.
   - Utiliza la aplicación `http.server` (servidor simple de Python) en el servidor final.
   - La página HTML final debe contener el texto: "Proxy inverso + tu nombre y apellido".
   
2. Configuración de Apache.
   - Habilita los módulos necesarios con los comandos:
     ```bash
     sudo a2enmod proxy
     sudo a2enmod proxy_http
     ```
   - Sigue la guía proporcionada para lanzar `http.server` y redirigir las peticiones.
   - Verifica el funcionamiento desde un equipo de la WAN.

## US13: Balanceador de Carga con Apache

**Fecha Tope: 4 de marzo**

1. Configuración de Apache como Balanceador de Carga.
   - Redirige las peticiones entre tres miembros del balanceador utilizando Apache.
   - Utiliza la aplicación `http.server` en los miembros del balanceador.
   - Crea tres carpetas con páginas HTML que contengan el texto: "Miembro balanceador nº __ + tu nombre y apellido".

2. Definición del Balanceador.
   - Define el balanceador en Apache con tu apellido como nombre.
   - Utiliza el método de balanceo `byrequests`, con el "primer" nodo teniendo el triple de carga que el "segundo".
   - El tercer nodo actuará como "hot-standby".
   
3. Activación del Balancer-Manager.
   - Habilita los módulos necesarios con los comandos:
     ```bash
     sudo a2enmod proxy
     sudo a2enmod proxy_http
     sudo a2enmod proxy_balancer
     sudo a2enmod lbmethod_byrequests
     sudo a2enmod slotmem_shm
     sudo a2enmod proxy_connect
     ```
   - Comenta la información que aparece en el balancer-manager.

4. Verificación del Funcionamiento.
   - Comprueba el correcto funcionamiento del balanceador.
   - Asegúrate de que el tercer nodo "hot-standby" se inicia correctamente.

## US14: Proxy Caché con pfSense (Opcional)

**Fecha Tope: 4 de marzo**

1. Configuración del Proxy Caché en pfSense.
   - Realiza una configuración básica para que los equipos de la LAN pasen por el proxy caché.
   - Comprueba la configuración para confirmar que los equipos de la LAN utilizan el proxy caché.

2. Investigación de Utilidades.
   - Investiga las utilidades de las configuraciones principales del proxy caché en pfSense.
