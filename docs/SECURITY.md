# Security model / Modelo de seguridad

## Español

Objetivo: limitar abuso básico (uso indefinido de TRIAL, reuso masivo de códigos) sin sacrificar UX.

### TRIAL
- Duración por minutos o días.
- Expiración local (workers) **y** verificación de servidor.
- Si el worker fallara, al intentar renovar (`refresh-license`) el backend rechaza si el trial ya venció.

### PRO
- Código PRO + binding por dispositivo.
- Límite de dispositivos por código controlado por servidor.
- `self-unbind` permitido solo para PRO (TRIAL no puede liberar cupo).

### Qué no se pretende evitar al 100%
- Dispositivos rooteados / hooking avanzado.
- APK reempaquetado con bypass de UI.

Mitigación: el valor real vive en el backend (validación y emisión de JWT).

## English
Goal: prevent basic abuse (infinite trial, mass reuse) with reasonable UX.

- TRIAL: server-enforced expiry + local workers.
- PRO: device binding + server-side device cap + PRO-only unbind.
