# Proyecto Integral de Seguridad y Alta Disponibilidad
## Seguridad en entornos empresariales
### Sprint 4 - Hardening SSH

---

## Documentación Sprint 4 - Hardening SSH

**Objetivo:** Implementar medidas de seguridad en el servicio SSH del servidor, siguiendo las recomendaciones del Incibe y habilitando el doble factor de autenticación (2FA).

**Instalación de SSH:**
```bash
sudo apt update
sudo apt install openssh-server

Configuración de Hardening según Incibe:
Editar el archivo de configuración de SSH:

sudo nano /etc/ssh/sshd_config


Habilitar el Doble Factor de Autenticación (2FA):
Instalar el paquete libpam-google-authenticator:

sudo apt install libpam-google-authenticator


Editar el archivo de configuración de SSH para habilitar el uso del autenticador:


sudo nano /etc/pam.d/sshd



Agregar la línea auth required pam_google_authenticator.so, guardar y editar nuevamente el archivo de configuración de SSH:



sudo nano /etc/ssh/sshd_config



Asegurarse de tener la línea ChallengeResponseAuthentication yes. Guardar y reiniciar SSH:


sudo service ssh restart



Verificación del Doble Factor de Autenticación:

Acceder al servidor SSH normalmente con usuario y contraseña.
Cuando se solicite la contraseña, también se pedirá un código de autenticación generado por la aplicación de autenticación (como Google Authenticator).
Ingresar el código actual de la aplicación de autenticación después de la contraseña y completar el proceso de inicio de sesión.
¡Listo! El servidor SSH está instalado, asegurado con las configuraciones de hardening recomendadas por Incibe y con el doble factor de autenticación habilitado. Ajustar las configuraciones según las necesidades y requisitos específicos del entorno.






















