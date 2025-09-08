

## Generalized Sector Types
| Value | Description          
|-------|--------------
| 32 | Damage Player (5 hp) (from Boom).
| 64 | Damage Player (10 hp) (from Boom).
| 96 | Damage Player (20 hp) (from Boom).
| 128  | Secret (Boom)
| 256  | Silent Monsters (Silences any sound emitted by an actor inside the sector) (Boom-Eternity)
| 512  | Silences doors, ceilings, and other level geometry movements (Boom (Reserve))
| 4096 | Kill Player (from MBF21).
| 4128 | Kill Player and go to Exit (from MBF21).
| 4160 | Kill Player and go to Secret Exit (from MBF21).

## Linedef flags

| Flag | Description           | Value
|-------|-----------------------|------
|ML_BLOCKPLAYERS | Block players (MBF21 flag). | 512
|ML_BLOCKLANDMONSTERS | Block Land Monsters (without MT_FLOAT, like cacos, pain elemental). (from MBF21). | 0x400
|ML_BLOCKSCAN | Block hitscan and BFG9000 tracers (from ZDoom). | 0x800
|ML_BLOCKPROJECTILE | Block projectiles (from ZDoom). | 0x1000
|ML_BLOCKSIGHT | Block thing sight	 (from ZDoom). | 0x2000

## Linedef flags2
| Flag2 | Description           | Value
|-------|-----------------------|------
|ML2_DISABLECONTRAST | Disables **Fake Contrast** on the linedef.   | 1
|ML2_WRAP_MIDTEX | The middle texture on a two-sided linedef will now render the same way as on a one-sided linedef. | 2
|ML2_FLIPPED | Textures are now flipped upside down.   | 4

## Linedef Special Action
* 257-262 Scrollers Variation
* 263: WR Clear Sector Special(line);
* 264: WR Clear Line Special(line);
* 265: S1 Clear Sector Special(line);
* 266: SR Clear Line Special(line);
* 267: S1 Clear Sector Special(line);
* 268: SR Clear Line Special(line);
* 300: Macros Event (Macros ID)

## New things
The following things have been added.

| Index          | DoomEdNum | Name                               | Description                                                                                                                                                                                                                                                                                             |
|----------------|-----------|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 137 | 4000     | `MT_MEDIPACK` - "Medipack" | `Width = 20`<br>`Height = 16`<br>`Mass = 100`<br><br>An enhanced version of the medkit that restores **50 HP** by default. |
| 138 | 4001     | `MT_HEAVYARMOR` - "Heavy Armor" | `Width = 20`<br>`Height = 16`<br>`Mass = 100`<br><br>An enhanced version of the blue armor. Provides **80%** damage protection. |
| 139 | 4002     | `MT_VITALLYSERUM` - "Vitality Serum" | `Width = 20`<br>`Height = 16`<br>`Mass = 100`<br><br>Increases the player’s maximum health, allowing medkits to restore up to that value. Default: 150. |
| 140 | 4003     | `MT_ARMORSHARD` - "Armor Shard" | `Width = 20`<br>`Height = 16`<br>`Mass = 100`<br><br>Grants 10% armor. Functionally identical to the vanilla Armor Bonus. |
| 141 | 4004     | `MT_REGENERATION` - "Regeneration" | `Width = 20`<br>`Height = 16`<br>`Mass = 100`<br><br>Upon pickup, the player gains 5 HP per second for the duration of the effect. The effect lasts exactly 20 seconds. |
| 142 | -     | `MT_NIGHTMAREBALL` - "Nightmare Ball" | `Width = 6`<br>`Height = 8`<br>`Speed = 20`<br>`Damage = 3`<br><br>A component of the Nightmare Imp. The projectile is very fast.  |
| 143 | 4006     | `MT_NIGHTIMP` - "Nightmare Imp" | `Width = 20`<br>`Height = 56`<br>`Mass = 100`<br>`Speed = 10`<br>`Health = 75`<br>`Ear1h27 Bits = MF2_SPAWNONLYNIGHTMARE`<br><br>Nightmare version of the Imp. This enemy always respawns in **Nightmare skill** and only appears on Nightmare difficulty. |
| 144 | 4007     | `MT_NIGHTMAREDEMON` - "Nightmare Demon" | `Width = 30`<br>`Height = 56`<br>`Mass = 400`<br>`Speed = 10`<br>`Health = 150`<br>`Ear1h27 Bits = MF2_SPAWNONLYNIGHTMARE`<br><br>Nightmare version of the Demon. This enemy always respawns in **Nightmare skill** and only appears on Nightmare difficulty.|
| 145 | 4008     | `MT_KAMIKAZE` - "Kamikaze" | `Width = 24`<br>`Height = 56`<br>`Mass = 150`<br>`Speed = 10`<br>`Health = 60`<br>`Ear1h27 Bits = MF2_NORESPAWN`<br><br>Its sole purpose is to get close to the player and explode.|
| 146 | -     | `MT_DARKBALL` - "Dark Ball" | `Width = 6`<br>`Height = 8`<br>`Speed = 8`<br>`Damage = 3`<br><br>Dark Imp projectile. |
| 146 | 4009     | `MT_DARKIMP` - "Dark Imp" | `Width = 30`<br>`Height = 56`<br>`Mass = 400`<br>`Speed = 10`<br>`Health = 150`<br>`Ear1h27 Bits = MF2_SPAWNONLYNIGHTMARE`<br><br>An enhanced version of the Doom Imp. Throws a slow projectile, but with a chance to home in on the player. The projectile accelerates in Nightmare skill.|
| 146 | -     | `MT_DARKSMOKE` - "Dark Smoke" | `Width = 20`<br>`Height = 16`<br>`Mass = 100`<br><br>Dark Smoke is transparent.|
