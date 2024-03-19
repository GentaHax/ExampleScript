# Function

* [sendPacket](#sendPacket)
* [sendVariant](#sendVariant) 
* [sendPacketRaw](#sendPacketRaw) 


## sendPacket
```xml
<
sendPacket(int, string)

to send a packet to the server with a specific packet type.
>
```

Example :
```lua
text = "KONTOL"
sendPacket(2, "action|input\n|text|".. text)
```