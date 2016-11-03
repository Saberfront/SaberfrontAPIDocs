LootService API
===============

Here are some members of the LootService module.

## LootService:GetChance()
returns a decimal between 0 and one using the numbers 0 and 100.

### Example:
```lua
local LootService = require(game.ReplicatedStorage.LootService)
local Chance = LootService:GetChance()
print(Chance * 100,"%")
```
## LootService:GetLootBag(MobConf)
returns a table of loot objects that a player could have
### Example:
```lua
local LootService = require(game.ReplicatedStorage.LootService)
local LootBag = LootService:GetLootBag("Inquisitor")
for _,v  in pairs(LootBag) do
    print(v.Name)
end 
```
