# ID27 Specdefs Definition v0.1.0

Considering the current trend of adding new flags for linedefs, it’s worth noting the limited size of the `short` variable.  
This lump not only allows introducing new `flags` while staying within the `Doom format`, but also lets you define `macros` that can perform multiple special actions simultaneously.  

| Property    | Data type                     | Description                                                                                                 |
|-------------|-------------------------------|-------------------------------------------------------------------------------------------------------------|
| `linedef index` | `short` between 0 and 32767    | Specifies the linedef number on which the flag should be set.|
| `flags2`      | `int` representing a linedef flag2 | Sets a linedef flag that goes beyond the short integer range. See (.\spec.md)| 

# Macros
| Property    | Data type                     | Description                                                                                                 |
|-------------|-------------------------------|-------------------------------------------------------------------------------------------------------------|
| `macroid[MAXMACRO]` | `short` between 0 and 1024    | Specifies the **macroid** number via tags, as defined in the linedef tag Special Action 300. See (.\spec.md)  |
| `id[MAXIDS]`      | `short` between 0 and 16| The number of actions specified in the macro.  | 
| `action` | `short` between 0 and 32767    | The number of the special action existing in the game.  |
| `variable`      | `short`, `char[8]`|A variable involved in the Special Action.   | 

Macros allow executing multiple actions simultaneously without relying on ACS or voodoo scripting.  

```
Macro `macroid[MAXMACRO]`
{
  `id[0]`: `action`, `variable`;        //0: Floor_LowerToLowest, 27;
  `id[1]`: `action`, `variable`;        //1: PrintMessage, "GOTTRAIN";
}
```
