# Reflection Functions

## Loadstring:
```lua
<function> loadstring(<string> chunk, <string?> chunkName)
```
- Loads `chunk` as a Lua function with optional `chunkName` and returns it.

## Check Caller:
```lua
<bool> checkcaller(<void>)  
```
- Returns `true` if the current thread was created by Oxygen-U.

## Is Lua Closure:
```lua
<bool> islclosure(<function> a1)  
```
- Returns `true` if `a1` is an LClosure.

## Dump String:
```lua
<string> dumpstring(<string> script)  
```
- Returns the Oxygen-U formatted bytecode for source string `script`.

## Decompile:
```lua
<string> decompile(<Instance> script)
```
- Decompiles `script` and returns the decompiled output.