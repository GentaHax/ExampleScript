# Function

* [sendPacket](#sendPacket)
* [sendVariant](#sendVariant) 
* [sendPacketRaw](#sendPacketRaw) 


## sendPacket
```xml
sendPacket(int, string)
to Send a Packet To The Server With a Specific Packet Type.

```

Example :
```lua
text = "KONTOL"
sendPacket(2, "action|input\n|text|".. text)
```