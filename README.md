# EnerIQ SmartRelay – Firmware

Dieses Repo enthält nur die fertigen Firmware-Dateien für das EnerIQ SmartRelay (ESP32), keinen Quellcode.

- `version.json` – aktuelle Version, Dateiname, MD5, Datum und Änderungen. Das Gerät liest diese Datei für das Online-Update.
- `EnerIQ_V<version>.bin` – Firmware zum Online-Update oder zum Hochladen über die Update-Seite des Geräts.

Einstellungen und Kalibrierwerte bleiben bei einem Update erhalten.

## Apps (Ordner `apps/`)

- `apps.json` – neueste Version der Handy-App (`phone`) und der Uhr-App (`watch`) mit Link zur APK. Die Apps lesen diese Datei für ihr Selbst-Update (Handy: Einstellungen › Nach Update suchen, Uhr: Einstellungen › App-Update).
- `EnerIQ-Handy-<version>.apk` – Android-App fürs Handy (Steuerung und Logbuch-PDF).
- `EnerIQ-Uhr-<version>.apk` – Wear-OS-App für die Pixel Watch.

Die APKs sind mit demselben Schlüssel signiert wie die bisher installierten Versionen, deshalb lassen sie sich einfach darüber installieren.
