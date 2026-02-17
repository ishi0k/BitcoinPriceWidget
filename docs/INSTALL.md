# Installation / Instalación (APK)

## Español

### Por qué aparece el aviso de Google Play Protect
Si instalas un APK fuera de Google Play, Play Protect puede mostrar un aviso del tipo **“App scan recommended”** indicando que no ha visto la app antes. Esto no significa necesariamente que sea maliciosa: es una verificación adicional.

Recomendación: toca **Scan app**. Si verificaste el checksum y el APK viene de este repositorio/website oficial, también puedes elegir **Install without scanning**.

Captura (ejemplo): `docs/images/alerta_google_play.jpg`

### Pasos de instalación
1. Descarga el APK desde **GitHub Releases** (o la web oficial).
2. (Opcional recomendado) Verifica el **SHA-256**:
   - En Android: usa una app de checksums, o
   - En PC (Linux/macOS): `sha256sum -c SHA256SUMS`
   - En PC (Windows PowerShell):
     ```powershell
     $expected = (Get-Content .\SHA256SUMS).Split(' ')[0].ToLower()
     $actual   = (Get-FileHash .\BitcoinPriceWidget-v1.0.0.apk -Algorithm SHA256).Hash.ToLower()
     $expected -eq $actual
     ```
3. Abre el APK descargado.
4. Si Android bloquea “instalación de fuentes desconocidas”:
   - Ajustes → Seguridad → Instalar apps desconocidas → habilita para tu navegador/archivos.
5. Instala y abre la app.
6. Concede permisos si aplica:
   - **Notificaciones** (para alertas).
   - **Alarma exacta** (si tu Android lo solicita; mejora puntualidad de actualizaciones).

### Recomendaciones para evitar problemas
- Desactiva optimización de batería para la app si tu fabricante mata procesos en segundo plano.
- Mantén conexión a internet para validación/renovación de licencia.

---

## English

### Why Google Play Protect shows a warning
When installing an APK outside Google Play, Play Protect may show **“App scan recommended”** because the app has not been widely seen before. It’s an additional security check.

Recommended: tap **Scan app**. If you verified the checksum and downloaded from the official repository/website, you may also choose **Install without scanning**.

Screenshot: `docs/images/alerta_google_play.jpg`

### Steps
1. Download the APK from **GitHub Releases** (or the official website).
2. (Recommended) Verify **SHA-256**.
   - Linux/macOS: `sha256sum -c SHA256SUMS`
   - Windows (PowerShell): see Spanish section above.
3. Open the APK.
4. If Android blocks unknown sources, allow installs for your browser/file manager.
5. Install and open.
6. Grant permissions when requested (Notifications, Exact alarms if needed).
