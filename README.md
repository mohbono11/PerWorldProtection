# PerWorldProtection (Beta v1)

**PerWorldProtection** is a comprehensive world protection system for Minecraft servers using Skript. It allows server admins to control a wide range of actions in specific worlds or globally, ensuring gameplay balance and preventing griefing or unwanted interactions.

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
