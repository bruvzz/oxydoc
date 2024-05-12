# Hooking Functions

## Hook Function:
```lua
<function> hookfunction(<function> old, <function> new)  
```
- Hooks function `old`, replacing it with the function `new`. The `old` function is returned, you *must* use this function in order to call the original function.

## Hook Metamethod:
```lua
<function> hookmetamethod(<Object> object, <string> metamethod, <function> a1)  
```
- Hooks the `metamethod` passed in `object`'s metatable with `a1`.

## New C Closure:
```lua
<function> newcclosure(<function> a1)  
```
- Pushes a new CClosure that invokes the function `a1` upon call.