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
