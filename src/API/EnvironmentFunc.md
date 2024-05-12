# Environment Functions

## Get Global Environment:
```lua
<table> getgenv(<void>)
```
- Returns the `environment` that will be applied to each script ran by Oxygen-U.

## Get Roblox Environment:
```lua
<table> getrenv(<void>)
```
- Returns the Roblox `environment`.

## Get Registry:
```lua
<table> getreg(<void>)
```
- Returns the `Lua` registry.

## Get Garbage Collection:
```lua
<table> getgc(<bool?>)
```
- Returns a `table` with all `gc` objects. Use `getgc(true)` to include tables.

## Get Instances:
```lua
<table> getinstances(<void>)
```
- Returns a `table` with instances.

## Get Nil Instances:
```lua
<table> getnilinstances(<void>)
```
- Returns a `table` with instances parented to `nil`.

## Get Loaded Modules:
```lua
<table> getloadedmodules(<void>)
```
- Returns a `table` with all loaded `modules` currently in game.

## Get Connections:
```lua
<table> getconnections(<RBXScriptSignal> Signal)
```
- Returns a `table` with all connections to the given `signal`.

### Connections:
| Connection | Description |
| :----: | :---: |
| .Function | The function connected to the connection. |
| :Enable | Enables the connection. |
| :Disable  | Disables the connection.  |
| :Fire | Fires the connection. |

## Fire Signal:
```lua
<void> firesignal(<RBXScriptSignal> Signal, <variant?> Args...)
```
- Fires all signals connected to the `signal`. If given, the arguments will be used to call the function.

## Fire Click Detector:
```lua
<void> fireclickdetector(<Instance> ClickDetector, <number?> Distance = 0, <string?>)
```
- Fires the `clickdetector`. If no distance supplied, it will default to `0`.

## Fire Proximity Prompt:
```lua
<void> fireproximityprompt(<ProximityPrompt> Prompt)
```
- Fires the `proximityprompt` trigger.

## Fire Touch Interest:
```lua
<void> firetouchinterest(<BasePart> totouch, <BasePart> Part, <uint?> toggle)
```
- Touches part with `totouch`.

### Actions:
| Action | Toggle |
| :----: | :---: |
| Begins the touch. | 0 |
| Ends the touch. | 1 |

## Set Scriptable:
```lua
<void> setscriptable(<Instance> Object, <string> Property, <bool> toggle)
```
- Sets the property's scriptable state to `toggle`.

## Get Hidden Property:
```lua
<variant> gethiddenproperty(<Instance> Object, <string> Property)
```
- Returns the `value` of the property that cannot be accessed through Lua.

## Set Hidden Property:
```lua
<void> sethiddenproperty(<Instance> Object, <string> Property, <variant> Value)
```
- Sets the given property to new `value`.

## Set Simulation Radius:
```lua
<void> setsimulationradius(<int> Radius)
```
- Sets the `LocalPlayer`'s simulation radius to given `arg`.