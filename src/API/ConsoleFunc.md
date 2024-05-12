# Console Functions

## Console Print:
```lua
<void> rconsoleprint(<string> text)
```
- Prints `text` into the console.

## Console Info:
```lua
<void> rconsoleinfo(<string> text)
```
- Prints `text` into the console, with `[INFO]` written before it.

## Console Error:
```lua
<void> rconsoleerr(<string> text)
```
- Prints `text` into the console, with `[ERROR]` written before it.

## Console Clear:
```lua
<void> rconsoleclear(<void>)
```
- Clears all text from the console.

## Console Name:
```lua
<void> rconsolename(<string> title)
```
- Sets the console's title to `title`.

## Console Input:
```lua
<string> rconsoleinput(<void>)
```
- Yields the current thread until the user inputs text and presses `Enter`. Returns the input they put in.

## Console Close:
```lua
<void> rconsoleclose(<void>)
```
- Closes the console.

## Print Console:
```lua
<void> printconsole(<string> message, <byte> red, <byte> green, <byte> blue)
```
- Prints `message` into the internal and integrated console with RGB value.

## Console Colors:
| Name | Type |
| :----: | :----: |
| Black | @@BLACK@@ |
| Blue | @@BLUE@@ |
| Green | @@GREEN@@ |
| Cyan | @@CYAN@@ |
| Red | @@RED@@ |
| Magenta | @@MAGENTA@@ |
| Light Gray | @@LIGHT_GRAY@@ |
| Dark Gray | @@DARK_GRAY@@ |
| Light Blue | @@LIGHT_BLUE@@ |
| Light Green | @@LIGHT_GREEN@@ |
| Light Cyan | @@LIGHT_CYAN@@ |
| Light Red | @@LIGHT_RED@@ |
| Light Magenta | @@LIGHT_MAGENTA@@ |
| Yellow | @@YELLOW@@ |
| White | @@WHITE@@ |
<p align="center">
    <img src="https://cdn.discordapp.com/attachments/775967135746621463/922084051194634240/image_1.png">
</p>

### Example:
```lua
rconsolename("console") -- Sets the name of the console to 'console'
rconsoleprint("gamer\n")
rconsoleprint("@@YELLOW@@") -- Changes the text color to Yellow
rconsoleprint("gamer but yellow\n")
rconsoleerr("omg error!")
rconsolewarn("omg warning!")
wait(3)
rconsoleclear() -- Clears all text
wait(1)
rconsoleclose() -- Closes the console
```
You must use `\n` at the end of `rconsoleprint` to make a new line.

`rconsoleinfo`, `rconsolewarn`, and `rconsoleerr` do this automatically.