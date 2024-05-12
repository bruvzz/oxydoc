# Bit32 Library

## Bit Divide:
```lua
<int> bit.bdiv(<uint> dividend, <uint> divisor)  
```
- Divides `dividend` by `divisor`, remainder is not returned.

## Bit Add:
```lua
<int> bit.badd(<uint> a, <uint> b)  
```
- Adds `a` with `b`, allows overflows.

## Bit Subtract:
```lua
<int> bit.bsub(<uint> a, <uint> b)  
```
- Subtracts `a` with `b`, allows overflows.

## Bit Multiply:
```lua
<int> bit.bmul(<uint> a, <uint> b)  
```
- Multiplies `a` using `b`, allows overflows.

## Bit And:
```lua
<int> bit.band(<uint> x, <uint> disp)
```
- Returns the bitwise *and* of its operands.

## Bit Or:
```lua
<int> bit.bor(<uint> x, <uint> disp)
```
- Returns the bitwise *or* of its operands.

## Bit Xor:
```lua
<int> bit.bxor(<uint> x, <uint> disp)
```
- Returns the bitwise *exclusive* or of its operands.

## Bit Not:
```lua
<int> bit.bnot(<uint> x)
```
- Returns the bitwise negation of `x`.

## To Hex:
```lua
<string> bit.tohex(<uint> val)  
```
- Returns `val` to a hex string.

## To Bit:
```lua
<int> bit.tobit(<uint> val)  
```
- Returns `val` into proper form for bitwise operations.

## Left Shift:
```lua
<int> bit.lshift(<uint> x, <uint> disp)
```
- Returns the number `x` shifted `disp` bits to the left.

## Right Shift:
```lua
<int> bit.rshift(<uint> x, <uint> disp)
```
- Returns the number `x` shifted `disp` bits to the left.

## Arithmetic Shift:
```lua
<int> bit.arshift(<int> x, <int> disp)
```
- Returns the number `x` shifted `disp` bits to the right. The number `disp` may be any representable integer. Negative displacements shift to the left.

    - This shift operation is what is called an arithmetic shift. Vacant bits on the left are filled with copies of the higher bit of `x`; vacant bits on the right are filled with zeros. In particular, displacements with absolute values higher than 31 result in zero or `0xFFFFFFFF` (all original bits are shifted out).