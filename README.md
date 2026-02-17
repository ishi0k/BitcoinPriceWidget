# Bitcoin Price Widget

Widget de Bitcoin para Android con actualizaciones programadas, alertas por cambio de precio y licenciamiento (TRIAL/PRO) controlado por servidor.

> Instalación por APK (GitHub/website). En algunos dispositivos verás un aviso de Google Play Protect (“App scan recommended”). Es normal cuando una app no viene desde Google Play.

## Descarga

- **APK (Release):** Ver la sección **Releases** del repositorio.
- **Checksums:** cada release incluye `SHA256SUMS` (SHA-256).

## Instalación rápida

1. Descarga el APK desde **Releases**.
2. (Opcional recomendado) Verifica el `SHA-256` del APK.
3. Abre el APK y acepta la instalación.
4. Si aparece **Google Play Protect**:
   - toca **Scan app** (recomendado), o
   - **Install without scanning** si confías en el checksum y el origen.

Guía completa: **docs/INSTALL.md**

## Verificar integridad (SHA-256)

Cada release incluye un archivo `SHA256SUMS`.

### Windows (PowerShell)

```powershell
$expected = (Get-Content .\SHA256SUMS).Split(' ')[0].ToLower()
$actual   = (Get-FileHash .\BitcoinPriceWidget-v1.0.0.apk -Algorithm SHA256).Hash.ToLower()
$expected -eq $actual
```

### Linux/macOS

```bash
sha256sum -c SHA256SUMS
```

Si el comando imprime `OK`, el APK coincide con el checksum publicado.

## Qué incluye

- Precio BTC en pantalla de inicio (widget).
- Moneda y formato personalizable (incluye decimales opcionales).
- Intervalo de actualización configurable.
- Alertas por cambios de precio (umbral + ventana de tiempo).
- Notificaciones con sonido/vibración opcionales.
- Personalización de texto: tamaño del título, tamaño/color del precio, visibilidad de info.
- Estado de licencia (TRIAL/PRO) con expiración visible opcional.
- Modo claro/oscuro/sistema.

Lista completa: **docs/FEATURES.md**

## Licencia (TRIAL/PRO)

- **TRIAL**: tiempo limitado (minutos o días) con expiración forzada por backend.
- **PRO**: licencia asociada a código + binding por dispositivo.

Detalles: **docs/SECURITY.md**

## Privacidad

No se solicita email. Para licenciamiento se usa un identificador de dispositivo y metadatos básicos del dispositivo (modelo/OS) y firma del APK para proteger el uso indebido.

Detalles: **docs/PRIVACY.md**

## Soporte

- Preguntas frecuentes: **docs/FAQ.md**
- Problemas comunes: **docs/TROUBLESHOOTING.md**
- Reporte de bugs: abre un **Issue**.

---

## English

See **docs/INSTALL.md** and **docs/FEATURES.md** (English sections included).
