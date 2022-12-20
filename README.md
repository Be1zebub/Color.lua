# Color.lua
Convert and manipulate color values.

### Example:
![image](https://user-images.githubusercontent.com/34854689/208636169-3f91271c-a40a-4265-983c-38dd4fc61dd2.png)
```lua
local alpha = 175

Color(255, 255, 0):Print("from incredible-gmod.ru with <3")

print("\nconverters:")

print("\trgb > color\t", Color(0, 255, 0, alpha):ToString())
print("\thex > color\t", Color.hex("#de621f", alpha):ToString())
print("\thexdec > color\t", Color.hex(0xDED81F, alpha):ToString())
print("\thexa > color\t", Color.hexa(0x82DE1FAF):ToString())
print("\thsv > color\t", Color.hsv(120, 86, 87, alpha):ToString())
print("\thsl > color\t", Color.hsl(150, 75, 50, alpha):ToString())
print("\thwb > color\t", Color.hwb(0, 0, 0, alpha):ToString())
print("\tcmyk > color\t", Color.cmyk(86, 37, 0, 13, alpha):ToString())

print("")

print("\tcolor > hex\t", Color(0, 255, 0, alpha):ToHex())
print("\tcolor > hexa\t", Color(222, 98, 31, alpha):ToHexa())
print("\tcolor > hexdecimal", Color(222, 216, 31, alpha):ToHexDecimal())
print("\tcolor > hexadecimal", Color(130, 222, 31, alpha):ToHexaDecimal())
print("\tcolor > hsv\t", table.concat({Color(27, 193, 27, alpha):ToHSV()}, ", "))
print("\tcolor > hsl\t", table.concat({Color(31, 223, 127, alpha):ToHSL()}, ", "))
print("\tcolor > hwb\t", table.concat({Color(255, 0, 0, alpha):ToHWB()}, ", "))
print("\tcolor > cmyk\t", table.concat({Color(31, 139, 221, alpha):ToCMYK()}, ", "))

print("meta events:")

print("\t__tostring\t", tostring(Color(123)))
print("\t__concat\t", "test ".. Color(100) .. " :)")
print("\t__unm\t\t", -Color(1, 2, 3))
print("\t__add\t\t", Color(25, 25, 25) + Color(150, 75, 0, 0))
print("\t__sub\t\t", Color(255, 255, 255) - Color(0, 255, 255, 0))
print("\t__mul\t\t", Color(100, 50, 0, 100) * 2)
print("\t__div\t\t", Color(200, 50, 0) / 2)
print("\t__eq\t\t", Color(255, 0, 0) == Color(255, 0, 0), Color(255, 0, 0) == Color(0, 0, 0))
print("\t__lt\t\t", Color(255, 0, 0) < Color(0, 0, 0))
print("\t__le\t\t", Color(255, 0, 0) <= Color(255, 1, 0))

print("methods:")

print("\tUnpack\t\t", table.concat({Color(255, 0, 0):Unpack()}, ", "))
print("\tSetUnpacked\t", Color(255, 0, 0):SetUnpacked(0, 255, 0))
print("\tNormalize\t", Color(255, 50, 100):Normalize())
print("\tGetNormalized\t", Color(255, 50, 100):GetNormalized())
print("\tString\t\t", Color.hex("#16a085"):String("hello"))
print("\tGrey\t\t", Color(255, 255):Grey())
print("\tInvert\t\t", Color(255, 100):Invert())
print("\tCopy\t\t", Color(100):Copy())
print("\tToTable\t\t", Color(123):ToTable())
print("\tToVector\t", Vector and Color(0, 255):ToVector() or "Cant convert to Vector, because Vector class is not defind")
print("\tContrast\t", Color(180, 150):Contrast(true))
```
