# Política de Privacidad de PouchVerse

**Fecha de vigencia: 29 de mayo de 2026**
**Producto aplicable: PouchVerse (Android)**
**Publicado por: Beijing EJIANDAN Network Technology Co., Ltd.**

---

## 1. Descripción general

Estamos comprometidos con una filosofía de producto **local primero / disponible sin conexión**. PouchVerse es una herramienta de gestión y agregación de archivos locales que no requiere registro de cuenta, no recopila datos personales y nunca sube ninguno de sus archivos ni metadatos a ningún servidor. Esta política explica de forma transparente qué hace y qué no hace la aplicación en su dispositivo Android y cómo usted mantiene el control.

---

## 2. Información que **no** recopilamos

**Nunca** recopilamos, almacenamos, subimos ni compartimos ninguno de los siguientes datos:

- Su nombre, número de teléfono, dirección de correo electrónico, número de identificación u otra información personal identificable
- Su ubicación, identificadores únicos de dispositivo (IMEI / Android ID / ID de publicidad AAID) o cualquier identificador de seguimiento
- Contenido de archivos o nombres de archivos que importe, visualice, organice o transfiera
- Sus consultas de búsqueda, historial de navegación o comportamiento de uso en la aplicación
- Sus contactos, calendario, metadatos de la biblioteca de fotos o datos de salud
- Cualquier dato utilizado para seguimiento, elaboración de perfiles, marketing o publicidad

PouchVerse **no incluye ningún SDK de terceros, servicio de análisis, red publicitaria ni servicio de notificaciones push**.

---

## 3. Datos procesados en el dispositivo

Para proporcionar las funciones principales, los siguientes datos se almacenan **exclusivamente en el directorio privado de la aplicación** (inaccesible para otras aplicaciones) y nunca salen de su dispositivo:

| Dato | Ubicación | Propósito |
|---|---|---|
| Contenido de archivos importados | `files/store/` | Gestión y vista previa de archivos |
| Metadatos de archivos (nombre, tamaño, tipo, fecha, etiqueta de color, etc.) | `databases/pouchverse.db` | Visualización, filtrado y ordenación de listas |
| Índice de búsqueda de texto completo (FTS5) | `databases/pouchverse.db` | Búsqueda por palabras clave |
| Miniaturas | `files/thumbs/` | Vista previa en listas |
| Hash de contenido (SHA-256) | `databases/pouchverse.db` | Detección de duplicados |
| Preferencias | `SharedPreferences` | Paso de búsqueda de vídeo, configuración de idioma, etc. |

Desinstalar PouchVerse **elimina permanentemente** todos los datos anteriores.

---

## 4. Permisos del sistema

- **Almacenamiento / Selector de documentos**: Importar archivos mediante el selector de documentos del sistema.
- **Medios** (si se usa): Importar fotos o vídeos desde la galería / biblioteca multimedia.
- **Dispositivos cercanos / Red local**: Descubrir dispositivos y transferir archivos por LAN.
- **Micrófono**: La aplicación no solicita activamente permiso de grabación; la extracción de texto de audio utiliza reconocimiento sin conexión en el dispositivo y el audio nunca sale del mismo.
- **Biometría / Credenciales del dispositivo**: Desbloquear la sección "Archivos privados" dentro de la aplicación.

PouchVerse **no solicita** acceso a internet (incluidos datos móviles), notificaciones push, cámara, ubicación, contactos, calendario ni permisos de movimiento. (Nota: el permiso `INTERNET` de Android se utiliza únicamente para la comunicación de socket Wi-Fi local de la función LAN y nunca se comunica con ningún servidor remoto.)

---

## 5. Actividad en la red

- **Sin conectividad a internet**: PouchVerse no envía ni recibe datos hacia ni desde ningún servidor remoto.
- **Transferencia LAN**: Solo cuando utiliza activamente la función "Transferencia LAN", la aplicación usa mDNS / NSD para descubrir dispositivos pares en la misma red local y transfiere los archivos seleccionados mediante un protocolo TCP personalizado (puerto 52013), directamente entre dispositivos.
  - Las transferencias LAN **no pasan por ningún servidor de retransmisión**; el emisor y el receptor se conectan directamente de punto a punto.
  - Las transferencias no están cifradas; evite transferir archivos confidenciales en redes Wi-Fi públicas que no sean de confianza.

---

## 6. Archivos privados

La función "Archivos privados" usa el BiometricPrompt del sistema Android (huella dactilar / reconocimiento facial / PIN / patrón / contraseña del dispositivo) para proporcionar una **capa de control de acceso secundaria dentro de la aplicación** para las carpetas privadas ocultas. Tenga en cuenta lo siguiente:

- Los archivos privados **no están cifrados en el disco**; su límite de privacidad depende de indicadores de pertenencia, el estado de desbloqueo en memoria y la ocultación en la interfaz de usuario.
- La aplicación **vuelve a bloquearse inmediatamente** al pasar a segundo plano o cerrarse; se requiere reautenticación en el próximo acceso.
- En dispositivos con root, o si alguien con acceso físico al dispositivo conoce las credenciales del mismo, los archivos podrían ser accesibles.

---

## 7. Privacidad de los menores

PouchVerse es una aplicación de uso general y no está dirigida a menores de edad. Si un menor de 14 años utiliza esta aplicación, debe hacerlo bajo la supervisión de un padre o tutor que gestione los permisos del dispositivo y el contenido importado.

---

## 8. Componentes de código abierto de terceros

PouchVerse enlaza estáticamente las siguientes bibliotecas de código abierto. **No se transmite ningún dato a través de ninguna de ellas.**

- **FFmpeg** (LGPL 2.1+): Decodificación local de vídeo / audio
- **unrar** (Licencia UnRAR, solo extracción): Extracción de archivos RAR
- **zlib** (Licencia zlib): Descompresión DEFLATE
- **SQLite3** (Dominio público): Base de datos local
- **AndroidX / Jetpack Compose** (Apache 2.0): Marco de interfaz de usuario

Los textos completos de las licencias están disponibles en la aplicación en **Barra lateral → Licencias**.

---

## 9. Exportación y eliminación de datos

- **Exportar**: Mantenga presionada una fila de archivo → Compartir, o comparta el archivo directamente con el gestor de archivos del sistema / otra aplicación.
- **Eliminar**: Deslice una fila de archivo hacia la izquierda para eliminarla, o desinstale la aplicación desde la configuración del sistema para eliminar permanentemente todos los datos locales.
- Dado que todos los datos residen íntegramente en su dispositivo, **no podemos ni intentaremos recuperar de forma remota los datos que haya eliminado**.

---

## 10. Cambios en esta política

Si esta política se actualiza de forma significativa, la nueva versión se anunciará a través de la página **Acerca de PouchVerse → Política de privacidad** dentro de la aplicación. El uso continuado de la aplicación después de cualquier cambio constituye la aceptación de la política actualizada.

---

## 11. Contáctenos

Si tiene alguna pregunta, comentario o queja sobre esta Política de privacidad, póngase en contacto con nosotros en:

- Empresa: Beijing EJIANDAN Network Technology Co., Ltd.
- Correo electrónico: [support@ejiandan.com](mailto:support@ejiandan.com)
