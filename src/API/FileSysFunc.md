# Filesystem Functions

## Read File:
```lua
<string> readfile(<string> path)
```
- Returns the contents of the file located at `path`.

## Write File:
```lua
<void> writefile(<string> path, <string> content)
```
- Writes `content` to the supplied `path`.

## Append File:
```lua
<void> appendfile(<string> path, <string> content)
```
Appends `content` to the file contents at `path`.

## Load File:
```lua
<function> loadfile(<string> path)
```
- Loads the contents of the file located at `path` as a Lua function and returns it.

## List Files:
```lua
<table> listfiles(<string> folder)
```
- Returns a table of all files in `folder`.

## Is File:
```lua
<bool> isfile(<string> path)
```
- Returns `true` if `path` is a file.

## Is Folder:
```lua
<bool> isfolder(<string> path)
```
- Returns `true` if `path` is a folder.

## Make Folder:
```lua
<void> makefolder(<string> path)
```
- Creates a new folder at `path`.

## Delete Folder:
```lua
<void> delfolder(<string> path)
```
- Deletes the folder located at `path`.

## Delete File:
```lua
<void> delfile(<string> path)
```
- Deletes the file located at `path`.