Sprint 2 - Copias de Seguridad
Introducción
En este sprint, abordaremos el proceso de copias de seguridad utilizando Duplicati. El objetivo es asegurar la integridad y disponibilidad de nuestros datos críticos, así como familiarizarnos con el funcionamiento de esta herramienta de copia de seguridad.

Elección de Software
Duplicati es la herramienta seleccionada para este proyecto debido a su facilidad de uso y compatibilidad con diversos servicios de almacenamiento en la nube. A diferencia de Veeam Backup Community Edition, Duplicati es más ligero y adecuado para nuestras necesidades.

Características de Duplicati
Funciona con protocolos estándar como FTP, SSH, WebDAV y servicios populares como Google Drive, Amazon S3, etc.
Ofrece cifrado AES-256 para archivos y carpetas.
Realiza copias de seguridad incrementales y deduplicación de datos.
Proporciona una interfaz web y una interfaz de línea de comandos.
Incluye un planificador y un actualizador automático.
Es software libre y de código abierto, con licencia LGPL.
Compatible con Windows, Linux y MacOS.
Diseñado para copias de seguridad en línea con capacidad de recuperación.
Copias de Seguridad
Copia 1 - "Copia Documentos"
Cifrado: Sí
Origen: Carpeta "Documentos" del servidor
Destino: Tu cuenta de Google Drive
RPO (Recovery Point Objective): Máximo 1 hora (lunes a viernes)
Pruebas de recuperación: Se requiere una batería de pruebas para verificar el funcionamiento correcto.
Copia 2 - "Copia Imágenes"
Cifrado: No
Origen: Carpeta "Imágenes" del servidor
Destino: Tu cuenta de Google Drive
RPO (Recovery Point Objective): Máximo 1 día (lunes a domingo)
Pruebas de recuperación: Se solicita una serie de pruebas para garantizar un correcto funcionamiento.
Pasos a Seguir
Instala Duplicati en tu servidor siguiendo las instrucciones correspondientes a tu sistema operativo.

Configura las copias de seguridad "Copia Documentos" y "Copia Imágenes" según los requisitos mencionados anteriormente.

Realiza pruebas exhaustivas de recuperación para garantizar la confiabilidad de las copias.

Documenta cualquier problema encontrado y las soluciones aplicadas.
