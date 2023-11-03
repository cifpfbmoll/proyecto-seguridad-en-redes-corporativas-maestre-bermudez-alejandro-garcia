

# Sprint 2 - Copias de Seguridad

## Introducción
En este segundo sprint nos enfocaremos en implementar copias de seguridad utilizando Duplicati, con el objetivo de garantizar la integridad de nuestros datos críticos.

## Elección de Software
Hemos seleccionado Duplicati debido a su facilidad de uso y compatibilidad con múltiples servicios en la nube.

## Características de Duplicati
- Compatible con protocolos estándar y servicios populares.
- Ofrece cifrado AES-256 y copias de seguridad incrementales.
- Proporciona una interfaz web y de línea de comandos.
- Es software libre y compatible con Windows, Linux y MacOS.

## Copias de Seguridad
### Copia 1 - "Copia Documentos"
- Cifrado: Sí
- Origen: Carpeta "Documentos" del servidor
- Destino: Google Drive
- Frecuencia de respaldo: Máximo cada 1 hora de lunes a viernes.
- Pruebas de recuperación requeridas.

### Copia 2 - "Copia Imágenes"
- Cifrado: No
- Origen: Carpeta "Imágenes" del servidor
- Destino: Google Drive
- Frecuencia de respaldo: Máximo una vez al día, de lunes a domingo.
- Pruebas de recuperación solicitadas.

## Pasos a Seguir
1. Instala Duplicati en tu servidor siguiendo las instrucciones específicas para tu sistema.

2. Configura las copias de seguridad "Copia Documentos" y "Copia Imágenes" de acuerdo a los requisitos mencionados.

3. Realiza pruebas de recuperación exhaustivas para asegurar la confiabilidad de las copias.

4. Documenta cualquier problema y las soluciones aplicadas.
