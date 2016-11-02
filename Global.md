Global API
==========

Here are some of the Utility API Members:

## Global:FindFirstItemWithId(location,id) 
Finds the first item with the exact same ID value as id in location and returns it.
### Example:
```lua
local gbl = require(game.ReplicatedStorage.Global)
local blaster = gbl:FindFirstItemWithId(game.Players.LocalPlayer.StarterGear,20344594)
print(blaster.Ammo.Value)
```
## Global:FindFirstClass(obj,ClassName)
Finds the first instance in obj with class ClassName and returns it.
Will return nil if it doesn't find anything.
### Example:
```lua
local gbl = require(game.ReplicatedStorage.Global)
local blaster = gbl:FindFirstItemWithId(game.Players.LocalPlayer.StarterGear,20344594)
print(gbl:FindFirstClass(blaster,"IntValue").Name)
```
## Global:GetSettings()
Returns all of the settings values for the entire game.
### Example:
```lua
local gbl = require(game.ReplicatedStorage.Global)
local s = gbl:GetSettings()
print(s.StartingHP)
```

## Global:FindCharacterAncestor(part)
Returns the parent of the part if it is a character (Has a humanoid).
### Example:
```lua
local gbl = require(game.ReplicatedStorage.Global)
capturePoint.Touched:connect(function(part)
if (gbl:FindCharacterAncestor(part)) then print(gbl:FindCharacterAncestor(part).Name .. " has captured the base for the Rebels!")
end)
```

## Global:orderArmorsByLvl(list)
return the ordered version of the list of armors available for Saberfront games such as Alderaanaian Assault

```lua
local gbl = require(game.ReplicatedStorage.Global)
local armors = gbl:orderArmorsByLvl(nil)
for _,v in pairs(armors) do
  print(v.Name)
end
  ```

