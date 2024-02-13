# Seguridad Perimetral con pfSense - README

## Proyecto Integral de Seguridad y Alta Disponibilidad
### Seguridad en entornos empresariales
#### Sprint 6 - Seguridad Perimetral con pfSense
##### US9: Seguridad perimetral con pfSense (fecha tope 19 de enero)

---

### Objetivo del Sprint
El objetivo de este sprint es poner en práctica los conocimientos adquiridos sobre seguridad perimetral, aplicando una arquitectura Screened Subnet (DMZ) que asegure perimetralmente el sistema mediante una estructura de tres zonas: Zona de confianza (LAN), Zona intermedia (DMZ), y Zona no confiable (WAN).

### Procedimiento

#### Instalación de pfSense
- Instalar pfSense con tres tarjetas de red:
  1. Wan (adaptador puente)
  2. Lan DMZ (Red interna 10.0.3.0/24)
  3. Lan Empleados (Red interna 10.0.2.0/24)

#### Configuración de Equipos

##### Configuración del Servidor Web (DMZ)
- Acceder a la interfaz web de configuración del servidor web.
- Seleccionar la interfaz de red del servidor web y configurar la dirección IP de la DMZ.
- Activar los puertos TCP 80 y 443.

##### Configuración del Equipo del Empleado (LAN Empleados)
- Abrir la aplicación "Configuración de red".
- Seleccionar la red de los empleados.
- En "Opciones avanzadas", añadir una regla de firewall para bloquear todo el tráfico.

### Comprobaciones Iniciales

1. **Acceso al configurador web de pfSense:**
   - El equipo de la LAN debe tener acceso al configurador web de pfSense.

2. **Acceso a Internet desde la LAN:**
   - Los equipos de la LAN deben tener acceso a Internet.

3. **Acceso entre las redes LAN y DMZ:**
   - No debe haber acceso entre las redes LAN y DMZ.

4. **Acceso a Internet desde la DMZ:**
   - La DMZ debe tener acceso a Internet.

5. **Acceso al servidor web desde la LAN:**
   - La LAN no debe tener acceso al servidor web.

### Configuración de Reglas de Firewall

1. **Regla 1: Permitir el acceso a Internet desde la DMZ:**
   - Permite que los equipos de la DMZ accedan a Internet para actualizar el software del servidor web.

2. **Regla 2: Permitir el acceso al servidor web desde la WAN:**
   - Permite que las peticiones al servidor web desde la WAN se redirijan a la dirección IP de la DMZ.

3. **Regla 3: Bloquear el tráfico HTTP desde la WAN:**
   - Bloquea el tráfico HTTP desde la WAN para permitir solo conexiones HTTPS al servidor web.

4. **Regla 4: Permitir el acceso al servicio SSH desde la WAN:**
   - Permite que las peticiones al puerto SSH desde la WAN se redirijan a la dirección IP de la DMZ.

5. **Regla 5: Bloquear el tráfico desde la LAN a la DMZ:**
   - Bloquea el tráfico desde la LAN a la DMZ para prevenir ciberataques que podrían propagarse a la DMZ.

### Pruebas de Funcionamiento
- Probar el correcto funcionamiento de las reglas de firewall configuradas.

### Pensar en Nuevas Reglas
- Considerar nuevas reglas que puedan añadirse a la configuración actual para mejorar la seguridad de la infraestructura.
