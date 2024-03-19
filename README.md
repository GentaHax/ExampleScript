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

### Example Methode:
```lua
text = "KONTOL"
sendPacket(2, "action|input\n|text|".. text)

-- Talk. 
```

## ・sendVariant
```js
sendVariant(var_t, int, int)
- var_t // Variant List
- int // Netid
- int // Delay
```

```lua
Variant List:
・"OnTextOverlay"
・"OnConsoleMessage"
・"OnDialogRequest"
・"OnReconnect"
・"OnSetClothing"
・"OnPlayPositioned"
・"OnSendToServer"
・"OnSendRoleSkinsAndTitles"
・"SetHasGrowID"
・"OnSetBux"
```

Example Methode:
```lua
sendVariant({
[0] = "OnConsoleMessage", 
[1] = "GentaHax!",
})

-- Sending To Console. 
```

## ・sendPacketRaw
```js
ssndPacketRaw(boolean send_to_client, tankStructPacket) 
- bool send_to_client // true, false
- tankStructPacket // struct Packet
```

Example Methode:
```lua
sendPacketRaw(false, 
    {
      type = 10,
      value = 98
    }
) 

-- Weared Pickaxe. 

```
