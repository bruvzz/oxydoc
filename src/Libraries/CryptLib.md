# Crypt Library

## Encrypt:
```lua
<string> crypt.encrypt(<string> data, <string> key)  
```
- Encrypts `data` with `key`.

## Decrypt:
```lua
<string> crypt.decrypt(<string> data, <string> key)  
```
- Decrypts `data` with `key`.

## Base64 Encode:
```lua
<string> crypt.base64.encode(<string> data)  
```
- Encodes `data` with base64.

## Base64 Decode:
```lua
<string> crypt.base64.decode(<string> data)  
```
- Decodes `data` with base64.

## Hash:
```lua
<string> crypt.hash(<string> data)
```
- Hashes `data` with SHA-384.

## Derive:
```lua
<string> crypt.derive(<string> value, <uint> length)
```
- Derives a secret key from `value` with the length of `length`.

## Random:
```lua
<string> crypt.random(<uint> size)
```
- Generates a random string with `size` (cannot be negative or exceed 1024).