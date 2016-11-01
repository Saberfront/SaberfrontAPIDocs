Global API
==========

Here are some of the Utility API Members:

## Global:FindFirstItemWithId(location,id) 
Finds the first item with the exact same ID value as id in location
### Example:
```lua
local gbl = require(game.ReplicatedStorage.Global)
local blaster = gbl:FindFirstItemWithId(game.Players.LocalPlayer.StarterGear,20344594)
print(blaster.Ammo.Value)
```
## Global:FindFirstClass(obj,ClassName)
Finds the first instance in obj with class ClassName.
Will return nil if it doesn't find anything.
### Example:
```lua
local gbl = require(game.ReplicatedStorage.Global)
local blaster = gbl:FindFirstItemWithId(game.Players.LocalPlayer.StarterGear,20344594)
print(gbl:FindFirstClass(blaster,"IntValue").Name)
```
