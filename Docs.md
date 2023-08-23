**Functions**
```lua
- Sleep(int ms)
- AddBot(string username, string password [, string proxy])
- RemoveBot(string name)
- GetBot([string name])
- GetBots()
```

**Bot Structure**
```lua
[!] Fields
- name
- captcha
- status
- state
- enet_state
- level
- gems
- netid
- userid

[!] Functions
- GetTile().x
- GetTile().y
- GetPing()
- Collect(int collect_range)
- CollectSet(bool state, int collect_range)
- Connect()
- Disconnect()
- SendRaw(int type, GamePacket packet)
- SendPacket(int type, string packet)
- SendGeneric(string packet)
- FindPath(int tile_x, int tile_y)
- Say(string text)
- Warp(string world_name [, string world_door])
- Enter()
- Punch(int tile_x, int tile_y)
- Place(int tile_x, int tile_y)
- Wrench(int tile_x, int tile_y)
- PunchTile(int tile_x, int tile_y)
- PlaceTile(int tile_x, int tile_y)
- WrenchTile(int tile_x, int tile_y)
- Wear(int item_id)
- Move(int direction_x, int direction_y)
- InWorld()

- SetAction(string action)
- GetAction(string action)
- GetWorld()
- GetTile(int tile_x, int tile_y)
- GetTiles()
- GetPlayer(string name)
- GetPlayers()
- GetObjects()
- GetInventory()
- FindItem(int item_id)
```

**World Structure**
```lua
[!] Fields
- name
- x
- y

[!] Functions
- IsJammed()
- IsLocked()
- GetOwnerID()
- GetAdmins()
```

**Tile Structure**
```lua
[!] Fields
- fg
- bg
- pos.x
- pos.y

[!] Functions
- IsSolid()
- IsFire()
- IsWater()
- IsReady()
- GetFlags()
- GetTile().x
- GetTile().y
```

**Object Structure**
```lua
[!] Fields
- id
- oid
- amount

[!] Functions
- GetTile().x
- GetTile().y
- GetObjectFlags()
```
**Player Structure**
```lua
[!] Fields
- name
- netid
- userid

[!] Function
- tile().x
- tile().y
- GetClothes()
- IsAdmin()
- IsOwner()
```

**Inventory Structure**
```lua
[!] Functions
- GetSize()
- GetUsed()
- GetAvailable()
- GetItems()
```

**InventoryItem Structure**
```lua
[!] Fields
- id
- amount

[!] Functions
- IsActive()
- IsClothes()
```