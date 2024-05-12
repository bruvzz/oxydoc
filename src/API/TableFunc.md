# Table Functions

## Get Raw Metatable:
```lua
<table> getrawmetatable(<table> a1)  
```
- Returns the `__metatable` of `a1`.

## Set Raw Metatable:
```lua
<bool> setrawmetatable(<table> a1, <table> a2)
```
- Sets the `__metatable` of `a1` to `a2`.

## Set Read Only:
```lua
<void> setreadonly(<table> a1, <bool> a2)  
```
- Sets the read-only value of `a1` to `a2`.

## Is Read Only:
```lua
<bool> isreadonly(<table> a1)  
```
- Returns if `a1` is read-only.