# Política de Privacidad de Static Ether Free

**Última actualización:** 22 de Julio de 2026

En **Static Ether**, respetamos profundamente tu privacidad y estamos totalmente comprometidos a proteger tus datos personales y la seguridad de tu dispositivo. Esta Política de Privacidad explica de forma transparente cómo opera la aplicación **Static Ether Free** y confirma nuestro compromiso de cero recopilación de datos.

---

## 1. Operación 100% Local y Cero Recopilación de Datos (No-Logs Policy)

- **Sin Registro de Actividad:** Static Ether Free **NO recopila, NO almacena y NO transmite** ningún tipo de información personal, historial de navegación, nombres de dominio consultados, consultas DNS, direcciones IP o identificadores de dispositivo.
- **Procesamiento en Dispositivo:** Todo el procesamiento y filtrado de paquetes DNS se realiza íntegramente en la memoria RAM local de tu dispositivo a través de un motor nativo C++ optimizado.
- **Sin Seguimiento de Terceros:** La aplicación no incluye SDKs de publicidad, ni herramientas de analítica o rastreo (como Google Analytics, Firebase, AdMob o Facebook SDK).

---

## 2. Declaración del Permiso `VpnService` de Android

Static Ether Free requiere y utiliza el permiso `VpnService` de Android bajo las siguientes condiciones estrictas:

1. **Uso Exclusivo como Bucle Invertido Local (Local Loopback TUN):** El servicio crea una interfaz de red local en tu dispositivo para interceptar únicamente solicitudes de resolución DNS en el puerto 53 local.
2. **Sin Redirección Externa:** La aplicación **NO redirige tu tráfico de internet a ningún servidor VPN remoto, proxy o servidor de terceros**.
3. **Privacidad de IP:** La aplicación no altera, no oculta ni enmascara tu dirección IP pública ante servidores de internet externos.
4. **Propósito:** El único objetivo del uso de `VpnService` es permitir la inspección local de consultas DNS para bloquear dominios publicitarios y rastreadores de telemetría sin requerir permisos de superusuario (root).

---

## 3. Seguridad y Cifrado de Datos en Tránsito

- **Actualización de Reglas:** La aplicación realiza solicitudes HTTPS seguras cifradas con protocolo TLS 1.3 hacia repositorios públicos de GitHub únicamente para verificar y descargar actualizaciones periódicas de la base de datos de filtrado (`version.json` y `ads.json`).
- **Sin Información Identificable:** Estas solicitudes de actualización no contienen token de usuario, identificador de dispositivo ni información personal.

---

## 4. Almacenamiento y Protección de Datos en el Dispositivo

- **Temporizador de Cuota Diaria (Anti-Manipulación):** Para administrar el límite gratuito de 1 hora al día, la aplicación guarda un archivo binario ofuscado protegido por suma de comprobación criptográfica (`.sec_timer_v2.dat`) en el almacenamiento privado de la aplicación (`/data/data/com.tkzenith.staticether/files/`). Este archivo solo contiene contadores monotónicos del procesador del dispositivo y no guarda información de uso personal.

---

## 5. Eliminación de Datos

Dado que **Static Ether Free no recopila ni almacena ningún dato de usuario en servidores remotos**, no existen datos de usuario guardados en la nube para eliminar. Al desinstalar la aplicación de tu dispositivo, se eliminarán automáticamente todos los archivos de configuración local.

---

## 6. Cambios en esta Política de Privacidad

Nos reservamos el derecho de actualizar esta Política de Privacidad periódicamente. Cualquier cambio significativo será publicado en esta misma página con la fecha de actualización correspondiente.
