# Features / Funcionalidades

## Español

### Widget (Pantalla de inicio)
- Muestra el precio de Bitcoin (BTC) en tu pantalla de inicio.
- Indicadores de estado (conexión/actualizando/error).
- Información opcional:
  - Próxima actualización.
  - Última actualización.
  - Estado de expiración (TRIAL/PRO) con badge de color por urgencia.

### Personalización
- Moneda de referencia (ej. USD) y formato del precio.
- Mostrar/ocultar decimales (cents).
- Tamaño del precio y color del precio.
- Tamaño del título del widget.
- Visibilidad de información (“Next update”, “Expiration”, etc.).
- Tema: claro / oscuro / sistema.

### Actualizaciones
- Intervalo de actualización configurable.
- Actualización manual (cuando aplica).
- Manejo de conectividad y estados de carga.

### Alertas y notificaciones
- Alertas por cambio de precio:
  - Umbral configurable (%).
  - Ventana de tiempo (horas) para evaluar el cambio.
- Notificaciones configurables:
  - Activar/desactivar.
  - Sonido.
  - Vibración.
  - (Opcional interno) debug del worker — deshabilitado en builds release.

### Licenciamiento (TRIAL/PRO)
- Activación por código (TRIAL o PRO).
- TRIAL con expiración real (minutos o días) y “hard-stop” de servidor.
- PRO con binding por dispositivo y liberación controlada (self-unbind solo para PRO).

---

## English

### Home Screen Widget
- Shows Bitcoin (BTC) price on your home screen.
- Status indicators (updating / offline / error).
- Optional info:
  - Next update time.
  - Last updated time.
  - License expiration badge (TRIAL/PRO) with urgency colors.

### Customization
- Currency and price format.
- Optional decimals (cents).
- Price text size and color.
- Widget title size.
- Information visibility toggles.
- Theme: light / dark / system.

### Updates
- Configurable refresh interval.
- Manual refresh where applicable.
- Connectivity-aware states.

### Alerts & notifications
- Price change alerts:
  - Configurable threshold (%).
  - Time window (hours).
- Notifications:
  - Enable/disable.
  - Sound.
  - Vibration.

### Licensing (TRIAL/PRO)
- Code-based activation.
- TRIAL with real expiry (minutes/days) enforced by backend.
- PRO device binding + controlled unbind (PRO only).
