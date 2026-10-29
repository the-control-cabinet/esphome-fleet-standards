# ESPHome Fleet Standards: Running 13 Controllers Like a Managed Estate

**The standards that keep 13 ESPHome controllers consistent and supportable, the way a BMS integrator standardises its outstations: board profiles by role, naming, secrets, logging and diagnostics, MQTT policy, fallback access, change control (one board first) and the rename runbook. Written from real fleet work, including a fleet-wide rework and a firmware-regression investigation.**

[![YouTube](https://img.shields.io/badge/YouTube-The%20Control%20Cabinet-red?logo=youtube)](https://www.youtube.com/channel/UC5Cupmz7vlfcodpCX7k8iuQ)
[![Portfolio](https://img.shields.io/badge/Portfolio-the--control--cabinet-24292f?logo=github)](https://github.com/the-control-cabinet/the-control-cabinet)
![Domain](https://img.shields.io/badge/BMS-fleet%20standards-blue)
![Status](https://img.shields.io/badge/Status-Live%20(documenting)-yellow)

> **The short version:**
> - **Four profiles:** active-connection BLE proxy · passive proxy + discovery logger · lean monitoring board · no-Bluetooth plant board.
> - **Every board:** encrypted API, `!secret` credentials, one shared fallback-hotspot secret, `captive_portal`, INFO logging, heap and loop-time debug sensors.
> - **MQTT only where used,** with discovery off; removed entirely elsewhere.
> - **Change control:** one board first, check uptime, then roll out; hold upgrades during a known regression.

**Portfolio position:** Automation level · controller standards. Related: [BLE network](https://github.com/the-control-cabinet/esp32-ble-presence-network) (profiles in practice, watchdog incident) · [plant monitoring](https://github.com/the-control-cabinet/heating-plant-monitoring-esphome) · [water metering](https://github.com/the-control-cabinet/mains-water-metering-modbus-rtu) · [security baseline](https://github.com/the-control-cabinet/smart-home-security-baseline)

---

## Documents

| Doc | Contents |
|---|---|
| [01 Board profiles](docs/01-profiles.md) | Profiles by role, with the standard blocks |
| [02 Conventions](docs/02-conventions.md) | Naming, secrets, logging, diagnostics, fallback access |
| [03 Change control](docs/03-change-control.md) | Updates, renames, regressions |

## Roadmap
- [ ] Fleet register populated (13 boards)
- [ ] VPin board moved onto the standards
- [ ] Fleet-wide update after the ESPHome fix, one board first
- [ ] Shared packages (ESPHome `packages:`) for the standard blocks

## Skills demonstrated (as built)
| Skill | Evidence |
|---|---|
| Standardisation | Profiles by role across 13 controllers |
| Configuration management | Naming, secrets, sanitised publishing |
| Change control | One-board-first updates; regression holds |
| Diagnostics | Uniform health sensors on every board |

📺 [The Control Cabinet on YouTube](https://www.youtube.com/channel/UC5Cupmz7vlfcodpCX7k8iuQ)

*Built and documented by James · part of [The Control Cabinet BMS portfolio](https://github.com/the-control-cabinet/the-control-cabinet). MIT Licence.*
