# Miscellaneous Functions

## Set Clipboard:
```lua
<void> setclipboard(<string> content)
```
- Sets `content` to the clipboard.

## Set Fast Flag:
```lua
<void> setfflag(<string> flag, <string> value)
```
- Sets `flag`'s value to `value`.

You can find a list of all Fast Flags here: [FFlag Watcher](https://fflag.eryn.io/) | [FFlag Tracker](https://raw.githubusercontent.com/MaximumADHD/Roblox-FFlag-Tracker/main/PCDesktopClient.json)

## Get Namecall Method:
```lua
<string> getnamecallmethod(<void>)
```
- Returns the namecall method if the function is called in an `__namecall` metatable hook.

## Set Namecall Method:
```lua
<void> setnamecallmethod(<string> method)
```
- Sets the current namecall method to the new namecall method. Must be called in a `__namecall` metatable hook.

## Identify Executor:
```lua
<string> identifyexecutor(<void>)
```
- Returns `Oxygen-U` if the current executor is Oxygen-U.

## Set FPS Cap:
```lua
<void> setfpscap(<uint> cap)
```
- Sets the fps cap to `cap`.

## Save Instance:
```lua
<void> saveinstance(<table> a1)  
```
- Saves the current game into your workspace folder. You can use table `a1` to customize options for this.

| Option | Value |
| :----: | :----: |
| mode | optikmized / full / scripts |
| noscripts | true / false |
| scriptcache | true / false |
| timeout | any number |

## Message Box:
```lua
<uint> messagebox(<string> text, <string> title, <uint> flag)
```
- Creates a message box.

### Flags:
| Flag | Value |
| :----: | :----: |
| OK | 0 |
| OK / Cancel | 1 |
| Abort / Retry / Ignore | 2 |
| Yes / No / Cancel | 3 |
| Yes / No | 4 |
| Retry / Cancel | 5 |
| Cancel / Try Again / Continue | 6 |

### Return Values:
| Value | Description |
| :----: | :----: |
| 1 | OK was clicked. |
| 2 | Cancel was clicked. |
| 3 | Abort was clicked. |
| 4  | Retry was clicked. |
| 5 | Ignore was clicked |
| 6 | Yes was clicked. |
| 7 | No was clicked. |
| 10 | Try Again was clicked.  |
| 11 | Continue was clicked. |