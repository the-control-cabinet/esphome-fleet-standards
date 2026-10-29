# 02 Conventions

[← Back to README](../README.md)

| Topic | Standard |
|---|---|
| **Hostname** | `esp32-<room>` (lower case, hyphens); friendly name `ESP32 <Room>` |
| **API key secret** | `<hostname with underscores>_key`; the value is kept when renaming |
| **Fallback hotspot** | SSID per board (never published); **one shared password secret** |
| **Logging** | `level: INFO` (DEBUG only while diagnosing) |
| **Diagnostics** | Uptime, Wi-Fi signal, heap free, heap max block, loop time on every board |
| **Lambdas** | No `//` comments inside lambdas (ESPHome 2026.10 compile issue); keep per-event work minimal |
| **Published YAML** | Sanitised: secrets only, no SSIDs, IPs, MACs or location names |
