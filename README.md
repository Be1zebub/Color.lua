# Color.lua
Convert and manipulate color values.

### Example:
```lua
local alpha = 175

Color(255, 255, 0):Print("from incredible-gmod.ru with <3")

print("\trgb > color\t", Color(255, 0, 0))
print("\thex > color\t", Color.hex("#FF0000", alpha))
print("\thexdeciminal > color", Color.hexdeciminal(16711680, alpha))
print("\thsv > color\t", Color.hsv(0, 100, 100, alpha))
print("\thsl > color\t", Color.hsl(0, 100, 50, alpha))
print("\tcmyk > color\t", Color.cmyk(0, 100, 100, 0, alpha))

print("")

print("\tcolor > hex\t", Color(255, 0, 0, alpha):ToHex())
print("\tcolor > hexdeciminal", Color(255, 0, 0, alpha):ToHexDeciminal())
print("\tcolor > hsv\t", table.concat({Color(255, 0, 0, alpha):ToHSV()}, ", "))
print("\tcolor > hsl\t", table.concat({Color(255, 0, 0, alpha):ToHSL()}, ", "))
print("\tcolor > cmyk\t", table.concat({Color(255, 0, 0, alpha):ToCMYK()}, ", "))
```
![image](https://user-images.githubusercontent.com/34854689/208408355-a2eeac06-f272-4dfd-a487-7561dd662fc2.png)
