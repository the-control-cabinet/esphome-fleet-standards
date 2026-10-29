# 03 Change control

[← Back to README](../README.md)

## Updates
1. Read the release notes; check open issues for your board type.
2. Update **one** board; watch uptime and the debug sensors for 24 h.
3. Roll out in groups; **hold** during a known regression (e.g. the 2026.10.0 task-watchdog resets, see the [BLE repo](https://github.com/the-control-cabinet/esp32-ble-presence-network/blob/main/docs/03-incident-esphome-2026-10-watchdog.md)).

## Renames
Follow the [rename runbook](https://github.com/the-control-cabinet/esp32-ble-presence-network/blob/main/docs/04-rename-and-cleanup-runbook.md): reconfigure HA, ignore the stale discovery, delete old MQTT devices, set areas, clear orphaned entities.

## Records
A fleet register: [data/fleet-register.csv](../data/fleet-register.csv) (board, profile, role, firmware, last change).
