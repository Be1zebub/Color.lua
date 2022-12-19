# Color.lua
Convert and manipulate color values.

### Example:
```lua
local alpha = 175

Color(255, 255, 0):Print("from incredible-gmod.ru with <3")

print(
	"\nfrom rgb\t\t".. Color(255, 0, 0, alpha)
	.."\nfrom hex\t\t".. Color.hex("#FF0000", alpha)
	.."\nfrom hexdeciminal\t".. Color.hexdeciminal(16711680, alpha)
	.."\nfrom hsv\t\t".. Color.hsv(0, 100, 100, alpha)
	.."\nfrom hsl\t\t".. Color.hsl(0, 100, 50, alpha)
	.."\nfrom cmyk\t\t".. Color.cmyk(0, 100, 100, 0, alpha)

	.."\n\nto hex\t\t\t".. Color(255, 0, 0, alpha):ToHex()
	.."\nto hexdeciminal\t\t".. Color(255, 0, 0, alpha):ToHexDeciminal()
	.."\nto hsv\t\t\t".. table.concat({Color(255, 0, 0, alpha):ToHSV()}, ", ")
	.."\nto hsl\t\t\t".. table.concat({Color(255, 0, 0, alpha):ToHSL()}, ", ")
	.."\nto cmyk\t\t\t".. table.concat({Color(255, 0, 0, alpha):ToCMYK()}, ", ")
)
```
![image](https://user-images.githubusercontent.com/34854689/208403051-1be77a57-567e-4f1a-90a4-9f78f9aa30e1.png)
