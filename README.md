# Function

* [sendPacket](#sendPacket)
* [sendVariant](#sendVariant) 
* [sendPacketRaw](#sendPacketRaw) 


## ・sendPacket
```js
sendPacket(int, stringPacket)
- int // Type
- string // String Packet
```

Example :
```lua
text = "KONTOL"
sendPacket(2, "action|input\n|text|".. text)

Output To Console : KONTOL
```

## ・sendVariant
```js
sendVariant(var_t, int, int)
- var_t // Variant List
- int // Netid
- int // Delay
```

Example :
```lua
-- Log To Console.
sendVariant({
[0] = "OnConsoleMessage", 
[1] = "GentaHax!", 
})

-- Text Overlay
sendVariant({
[0] = "OnTextOverlay", 
[1] = "GentaHax!", 
}) 
```

## ・sendPacketRaw
```js
ssndPacketRaw(boolean send_to_client, tankPacketStruct) 
