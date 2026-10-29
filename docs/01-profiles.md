# 01 Board profiles

[← Back to README](../README.md)

| Profile | Boards (generic) | Bluetooth | Scanner | MQTT |
|---|---|---|---|---|
| **A. Active-connection proxy** | One per floor | `bluetooth_proxy: active: true` | Yes | Scanner only, `discovery: false` |
| **B. Passive proxy + logger** | Other rooms | `active: false` | Yes | Scanner only, `discovery: false` |
| **C. Lean monitoring** | Understairs plant, utility (water) | Passive proxy, passive scan | No | **None** |
| **D. Plant, no Bluetooth** | Control room (boiler) | None (I/O fully allocated) | No | **None** |
| **E. Special** | Camera, VPin, OpenTherm node | Per need | No | None |

Standard blocks: [config/standard-blocks.yaml](../config/standard-blocks.yaml)
