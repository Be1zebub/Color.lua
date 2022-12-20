# Color.lua
Convert and manipulate color values.

### Example:
```lua
local alpha = 175

Color(255, 255, 0):Print("from incredible-gmod.ru with <3")

print("\trgb > color\t", Color(255, 0, 0, alpha))
print("\thex > color\t", Color.hex("#FF0000", alpha))
print("\thexdec > color\t", Color.hex(0xFF0000, alpha))
print("\thexa > color\t", Color.hexa(0xFF0000AF))
print("\thsv > color\t", Color.hsv(0, 100, 100, alpha))
print("\thsl > color\t", Color.hsl(0, 100, 50, alpha))
print("\tcmyk > color\t", Color.cmyk(0, 100, 100, 0, alpha))

print("")

print("\tcolor > hex\t", Color(255, 0, 0, alpha):ToHex())
print("\tcolor > hexa\t", Color(255, 0, 0, alpha):ToHexa())
print("\tcolor > hexdecimal", Color(255, 0, 0, alpha):ToHexDecimal())
print("\tcolor > hexadecimal", Color(255, 0, 0, alpha):ToHexaDecimal())
print("\tcolor > hsv\t", table.concat({Color(255, 0, 0, alpha):ToHSV()}, ", "))
print("\tcolor > hsl\t", table.concat({Color(255, 0, 0, alpha):ToHSL()}, ", "))
print("\tcolor > cmyk\t", table.concat({Color(255, 0, 0, alpha):ToCMYK()}, ", "))
```
![image](https://user-images.githubusercontent.com/34854689/208588735-72e163b5-d2a6-4dd9-8925-c27a92cc0a1e.png)
