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
