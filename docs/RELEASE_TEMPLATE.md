# GitHub Release template

Copia/pega este texto en **GitHub Releases** y solo ajusta la versión.

---

## Bitcoin Price Widget v1.0.0

First public release.

### Download
- `BitcoinPriceWidget-v1.0.0.apk`
- `SHA256SUMS`

### Install
1. Download the APK.
2. Open it and allow installation if Android asks.
3. If Play Protect appears, tap **Scan app** (normal for non‑Play apps).

### Verify SHA‑256 (optional, recommended)

**Linux/macOS**

```bash
sha256sum -c SHA256SUMS
```

**Windows (PowerShell)**

```powershell
$expected = (Get-Content .\SHA256SUMS).Split(' ')[0].ToLower()
$actual   = (Get-FileHash .\BitcoinPriceWidget-v1.0.0.apk -Algorithm SHA256).Hash.ToLower()
$expected -eq $actual
```

If the result is `True` (Windows) or `OK` (Linux/macOS), your APK matches the published checksum.
