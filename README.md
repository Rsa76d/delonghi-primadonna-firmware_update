# DeLonghi PrimaDonna MITM — firmware binaries

Публічний репозиторій лише з прошивками (`.bin`) для ESP32-C6 моста
[delonghi-primadonna-ble-mitm](https://github.com/Rsa76d) (код — у приватному репозиторії).

- `index.json` — список усіх версій (новіші першими): версія, файл, розмір, SHA-256, `latest`.
- `bin/` — усі збірки v4.16 → поточна.

Пристрій читає `index.json` за адресою
`https://raw.githubusercontent.com/Rsa76d/delonghi-primadonna-firmware_update/main/index.json`.

Збірки до v4.58 зібрані на arduino-esp32 3.2.x (IDF 5.4.2), v4.59 і новіші на 3.3.5 (IDF 5.5.1).
Параметри збірки: ESP32-C6, `PartitionScheme=min_spiffs`, `CDCOnBoot=default`.
Це збірки для OTA (app-образ), а не повний образ флешу.
