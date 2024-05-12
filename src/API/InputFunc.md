# Input Functions

## Is Active:
```lua
<bool> iswindowactive(<void>)  
```
- Returns if the window is focused.

## Keyboard:
```lua
<void> keypress(<uint> keycode)  
```
- Simulates a key press for the specified keycode. You can find a list of codes [here](https://docs.microsoft.com/en-us/windows/desktop/inputdev/virtual-key-codes).
```lua
<void> keyrelease(<uint> key)  
```
- Releases `key` on the keyboard.

## Left Click:
```lua
<void> mouse1click(<void>)  
```
- Simulates a full left mouse button press.
```lua
<void> mouse1press(<void>)  
```
- Simulates a left mouse button press without releasing it.
```lua
<void> mouse1release(<void>)  
```
- Simulates a left mouse button release.

## Right Click:
```lua
<void> mouse2click(<void>)
```
- Simulates a full right mouse button press.
```lua
<void> mouse2press(<void>)  
```
- Clicks down on the right mouse button.
```lua
<void> mouse2release(<void>)  
```
- Simulates a right mouse button release.

## Mouse Movement:
```lua
<void> mousescroll(<number> number)  
```
- Scrolls the mouse wheel virtually by `number` pixels.
```lua
<void> mousemoverel(<number> a1, <number> a2)  
```
- Moves the mouse cursor relatively to the current mouse position by coordinates `a1` and `a2`.
```lua
<void> mousemoveabs(<number> a1, <number> a2)  
```
- Move's your mouse to the `a1` and `a2` coordinates in pixels from top left of the window.