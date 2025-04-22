# HeliCrateTeleport

**Author:** Codex  
**Version:** 1.2.0  
**Plugin Type:** Oxide/uMod (Rust)  
**Dependency:** HeliSignals (must be installed)

---

## Description

Safely teleports crates spawned by HeliSignals helicopters directly to the position of the player who called them in.

Includes:
- Radial crate offsetting to prevent stacking
- Collision checks to avoid wall or terrain clipping
- Optional file-based logging for crate drop activity

---

## Features

- Teleports only crates spawned from HeliSignals helicopters (ignores vanilla patrol helicopters)
- Drops crates in a circular offset around the player
- Raycasts ground placement to avoid invalid crate positions
- Falls back to center-drop if no valid ground is found
- Logs crate drop details to a file (optional via config)

---

## Configuration

Located at `/oxide/config/HeliCrateTeleport.json`

```json
{
  "LogCrateTeleportEvents": false
}
