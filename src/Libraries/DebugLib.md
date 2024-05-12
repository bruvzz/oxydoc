# Debug Library

## Get Constants:
```lua
<table> debug.getconstants(<function> f)
```
- Returns the constants in function `f` or at level `f`.

## Get Constant:
```lua
<variant> debug.getconstant(<function> f, <int> idx)
```
- Returns the constant at index `idx` in function `f` or level `f`. 

## Set Constant:
```lua
<void> debug.setconstant(<function> f, <int> idx, union<number, bool, string> value)
```
- Set constant `idx` to tuple `value` at level or function `f`.

## Get Upvalues:
```lua
<table> debug.getupvalues(<function> f)
```
- Retrieve the upvalues in function `f` or at level `f`.

## Get Upvalue:
```lua
<variant> debug.getupvalue(union<function, number> f, <number> idx)
```
- Returns the upvalue with name `idx` in function or level `f`.

## Set Upvalue:
```lua
<void> debug.setupvalue(<function> f, <int> idx, <table> value)
```
- Set upvalue `idx` to `value` at level or function `f`.

## Get Proto:
```lua
<table, function> debug.getproto(<function> f, <int> idx, <bool?> activated)
```
- Gets the inner `function` of `f` at `index`.

## Set Proto:
```lua
<void> debug.setproto(<function> fi, <number> index, <function> replacement)
```
- Replaces `fi` at `index` with function `replacement` at level or function `fi`.

## Get Stack:
```lua
<table> debug.getstack(<function> f, <int> idx)
```
- Gets the method stack at level or function `f`.

## Set Stack:
```lua
<void> debug.setstack(<function> f, <int> idx, <table> value)
```
- Sets the stack indice at `indice` to `value` at level or function `f`.

## Set Metatable:
```lua
<table> debug.setmetatable(<table> o, <table> mt)  
```
- Set the metatable of `o` to `mt`.

## Get Registry:
```lua
<table> debug.getregistry(<void>)
```
- Returns the Lua registry.

## Get Info:
```lua
<table> debug.getinfo(<function> f)
```
- Returns a table of information about function `f`.

### Info:
| Name | Type | Description |
| :----: | :----: | :----: |
| name | String | The name of the function. |
| short_src | String | A shorter version of source. |
| what | String | What the function is: Lua = Lua function - C = C function
| currentline | Integer | The line that is currently active. |
| nups | Integer | The number of upvalues that the function has. |
| func | Function | The function that is active. |
| source | String | Where the function was defined. |