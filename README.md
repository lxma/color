# color
Go package containing color constants for ANSI terminals.

# Intention
The idea is to provide constants that can be used for simple color commands. Colors are simple
string constants that can be included in printf commands, such as:
```go
    fmt.Printf("Normal text – %sthis is green%s this is bold and green%s and this is regular again.\n",
               color.Green, color.Bold, color.Reset)
```
You can also combine instructions such as:
```go
const ErrorColor = color.Red + color.Bold
fmt.Printf("%sThis is wrong\n%s", ErrorColor, color.Reset)
```
There is intentionally no code such as functions to print something in a specific color. If you are looking for
something like that, look into [fatih/color](https://github.com/fatih/color).