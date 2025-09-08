## New Power-ups  
The specification introduces only two new power-ups:  

| Power-up        | Description | Duration |
|-----------------|-------------|----------|
| **pw_regeneration** | Restores *n* health points every second. The value can be adjusted via DeHackEd. Default: 4 HP per second. | `25 * TICRATE` |
| **vitality** | Similar to the backpack, the **vitality serum** increases the player’s maximum health, allowing medkits to restore up to that value. Default: 150. | Lasts until the player dies, starts a new game, restarts the level, or uses `idclev##`. |

## New hardcoded strings

The following strings can be overridden by `DEHACKED` or `LANGUAGE` lumps, but are provided as defaults:

| Mnemonic           | Default text   |
|--------------------|----------------|
| `GOTREGEN`  | Regeneration! |
| `GOTVITA`    | Your health has increased!   |
