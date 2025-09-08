# New Thing Flags 
* Add `Ear1h27 Bits = X` in the Thing definition.
* The format is the same as the existing Bits field.
* Example: `Ear1h27 Bits = NODAMAGE+ANTITELEFRAG`.
* The value can also be given as a number (sum of the individual flag values below).

| Flag | Description           | Value
|-------|-----------------------|------
|MF2_NORESPAWN | Enemies do not respawn on `Nightmare` difficulty or with the `-respawn` parameter (from ID24). | 1
|MF2_FULLVOLSOUNDS | Full volume see / death sound & splash immunity (from MBF21). | 2
|MF2_NORADIUSDMG | Doesn't take splash damage (cyberdemon, mastermind) (from MBF21). | 4
|MF2_ACTIVATOR | Thing can activate most player-activated linedefs as though it were a voodoo doll. (from MBF2y). | 8
|MF2_NODAMAGE | Thing does not lose health when taking damage.	 (from MBF2y). | 16
|MF2_NOCRUSH | If Thing is a `CORPSE`, it does not turn into gibs when crushed. If Thing is `DROPPED`, it does not disappear when crushed. (Thing will still take damage from crushers.) (from MBF2y). | 32
|MF2_MONSTERPASS | Thing passes through monster-blocking lines, without being a friend, projectile or a player. (from Eternity). | 64
|MF2_SPAWNONLYNIGHTMARE | Enemies spawn only on Nightmare difficulty. | 128
|MF2_ANTITELEFRAG | Things that would telefrag this thing are telefragged instead. (from MBF2y). | 256

## Map Object Flags

`NIGHTMARE` should be exposed to the map editor like the `AMBUSH` flags.

| Bit | Value  | Description |
|-----|--------|-------------|
| 6   | 0x0040 | `NIGHTMARE`  |
