# Function

* [sendPacket](#sendPacket)
* [sendVariant](#sendVariant) 
* [sendPacketRaw](#sendPacketRaw)
* [setGid](#setGid) 
* [setMac](#setMac) 


## ・sendPacket
```js
sendPacket(int, stringPacket)
- int // Type
- string // String Packet
```

`Example Methode:`
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

`Example Methode:`
```lua
sendVariant({
[0] = "OnConsoleMessage", 
[1] = "GentaHax!",
})

-- Sending To Console. 
```

## ・sendPacketRaw
```js
sendPacketRaw(boolean send_to_client, tankStructPacket) 
- bool send_to_client // true, false
- tankStructPacket // struct Packet
```

`Example Methode:`
```lua
sendPacketRaw(false, 
    {
      type = 10,
      value = 98
    }
) 

-- Weared Pickaxe. 

```

## ・setGid
```js
setGid(std::string) 
- it Has Max 37 Char.
```

`Example Methode:`
```lua
googleID = "hObx7tOj-6KzgT-Gx9k-t7gq-gIsingkontol"
setGid(GoogleID) 
```

## ・setMac
```js
setMac(std::sring) 
- it Has Max 18 Char.
```

`Example Methode:`
```lua
macAddress = "02:00:00:00:00:00"
setMac(macAddress)
```