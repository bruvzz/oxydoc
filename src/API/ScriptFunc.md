# Script Functions

## Get Script Environment:
```lua
<table> getsenv(<LocalScript, ModuleScript> Script)
```
- Returns the global environment of the given script.

## Get Calling Script:
```lua
<Instance> getcallingscript(<void>)
```
- Gets the script that is calling this function.

## Get Script Closure:
```lua
<function> getscriptclosure(<Instance> Script)
```
- Returns the closure from the given script, can be used to gather `upvalues` or `constants`.

## Get Script Hash:
```lua
<string> getscripthash(<Instance> Script)
```
- Returns a SHA384 hash of the scripts bytecode. You can use this to detect changes of a script.

## Get Script Bytecode:
```lua
<string> getscriptbytecode(<Instance> Script)
```
- Returns the bytecode of the given script. This can be used in a dissassembler.