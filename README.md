# Function

* [sendPacket](#sendPacket)
* [sendVariant](#sendVariant) 
* [sendPacketRaw](#sendPacketRaw) 


## sendPacket
```js
sendPacket(int, stringPacket)

- to Send a Packet To The Server With a Specific Packet Type.

```

Example :
```lua
text = "KONTOL"
sendPacket(2, "action|input\n|text|".. text)

Output To Console : KONTOL
```

## sendVariant
```js
sendVariant(var_t, int, int)

- ?
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
