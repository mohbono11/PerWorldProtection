Donation Link: https://mc-host24.de/donate/craftingmanager

# PerWorldProtection

**PerWorldProtection** is a comprehensive world protection system for Minecraft servers using Skript. It allows server admins to control a wide range of actions in specific worlds or globally, ensuring gameplay balance and preventing griefing or unwanted interactions.

---
## Known issues
- Whitelisted blocks/entities don't work.

---
## Features

- **World Protection**: Protect specific worlds or all worlds by default.
- **Block & Item Control**:
  - Block breaking and placing
  - Block interaction
  - Item dropping and picking up
  - Inventory access
- **Entity Control**:
  - Damage and interaction prevention
  - Mob spawning control
- **PvP Control**: Enable or disable player-versus-player combat per world.
- **Environmental Protection**:
  - Bucket usage (fill/empty)
  - Explosions
  - Liquid flow (water/lava)
- **Advanced Options**:
  - Logging violations to console
  - Admin notifications
  - Kick players on repeated violations
  - Whitelist specific blocks or entities


Future updates may include fire spread protection and more advanced features.
---

## Configuration

All options are configurable via the `options:` section:

```
protected-worlds: "example", "another_example" # Worlds to protect (case sensitive)
block-break: true
block-place: true
block-interact: true
entity-interact: true
entity-damage: true
item-drop: true
item-pickup: true
inventory-access: true
bucket-usage: true
pvp: true
mob-spawning: false
explosions: true
liquid-flow: false

enable-logging: false
notify-admins: false
kick-on-violation: false
kick-violations-limit: 50

whitelisted-blocks: "example", "another_example"
whitelisted-entities: "example", "another_example"

no-permission-message: "&cYou don't have permission to do that in this world!"
admin-notification: "&7[PWP] &e{player} &7tried to &c{action} &7in world &b{world}"
```
---

## Commands

- `/perworldprotection` or `/pwp`: Display plugin information, including version, author, and description.
- `/pwp reload`: Reload the script configuration (requires `perworldprotection.admin` permission).

---

## Permissions

- `perworldprotection.admin`: Allows access to admin commands like reload.
- `perworldprotection.notify`: Receive notifications of violations.
- `perworldprotection.bypass`: Bypass all world protections.
- `perworldprotection.bypass.<world>`: Bypass protections for a specific world.

---

## Installation

1. Place `PerWorldProtection.sk` in your `plugins/Skript/scripts/` folder.
2. Reload Skript or the individual script using `/sk reload PerWorldProtection`.
3. Configure `options:` according to your server needs.

---

## Notes

- This script is in **Beta v1**. Always backup your server before using.
- Modifying anything below the options section is **not recommended** unless you know what you are doing.
- Future updates may include fire spread protection and more advanced features.

---

**Author:** ihatemustard  
**Version:** Beta v1

