# proyecto-seguridad-en-redes-corporativas-maestre-bermudez-alejandro-garcia
proyecto-seguridad-en-redes-corporativas-maestre-bermudez-alejandro-garcia created by GitHub Classroom


# Proyecto Integral de Seguridad y Alta Disponibilidad

## Sprint 3 - Hardening Apache

### Descripción del Proyecto

Este proyecto se enfoca en fortalecer la seguridad del servidor web Apache en un entorno empresarial. Aunque el servidor ya está instalado y en funcionamiento, la seguridad no debe ser subestimada. En este sprint, nos centraremos en implementar las prácticas de hardening básicas recomendadas por el Incibe (Instituto Nacional de Ciberseguridad).

### Objetivos

El objetivo principal del sprint es configurar el servidor Apache para mejorar su seguridad. Para lograr esto, se realizarán las siguientes configuraciones, en su mayoría basadas en la guía de hardening básica de Apache proporcionada por el Incibe:

1. **Instalación de Apache**: Asegurarse de tener la instalación correcta del servidor web Apache.

2. **Configuraciones Globales**: Ajustar las configuraciones globales del servidor para mejorar la seguridad.

3. **Ficheros de Configuración**: Modificar los archivos de configuración según las recomendaciones de seguridad.

4. **Configuración de Usuarios y Grupos**: Establecer configuraciones seguras para usuarios y grupos relacionados con Apache.

5. **Ocultación de Versiones**: Ocultar la versión de Apache para reducir la superficie de ataque.

6. **Exposición Mínima de Módulos**: Configurar el servidor para exponer solo los módulos esenciales.

7. **Creación de VirtualHost Personalizado**: Configurar un VirtualHost con nombre y apellido personal.

8. **Configuración Múltiple y de Contexto (Directiva Options)**: Establecer opciones de configuración múltiples y de contexto.

9. **Restricción de Acceso al Contenido (Directiva Auth y Require)**: Configurar la autenticación mediante digest en uno de los directorios del VirtualHost.

10. **Ficheros .htaccess**: Entender y configurar adecuadamente los ficheros .htaccess para mejorar la seguridad.

11. **Evitar el Hotlinking**: Implementar medidas para prevenir el hotlinking y verificar su eficacia.

12. **Configuración HTTPS mediante OpenSSL**: Crear certificados para garantizar que el VirtualHost sea accesible solo a través de HTTPS.

13. **Modulo mod_security**: Investigar y habilitar el módulo mod_security para mejorar la detección y prevención de ataques.

14. **Ataque DoS mediante Metasploit (Slowloris)**: Realizar un ataque DoS para evaluar la resistencia del servidor.

15. **Reglas OWASP para mod_security**: Clonar e instalar las reglas recomendadas por OWASP y habilitar mod_security.

16. **Reglas para Detectar SQL Injection**: Configurar reglas específicas para detectar ataques de inyección SQL.

17. **Verificación del Servidor tras Ataque DoS**: Realizar nuevamente el ataque DoS y confirmar la accesibilidad del servidor.




