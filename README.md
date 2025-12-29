# x4 is a bss x4 maintainer you can use it with atlas (tested only with it) you can use it manually also if you need it for some reason
```lua
_G.field = "Pepper Patch" -- change to your field
_G.slots = {LoadedDice = 5, Glitter = 6, FieldDice = 7} -- change if items in different slots
loadstring(game:HttpGet("https://raw.githubusercontent.com/1toop/x4/refs/heads/main/x4.lua"))()
```lua

Auto maintains x4 field boost by using One Loaded Dice, Field Dice, and Glitter.

**Note**: If you have many features enabled in your script ur using for autofarm, boost may expire often because script is busy with other tasks

## Setup

1. Place items in hotbar:
   - Loaded Dice -> slot 5
   - Glitter -> slot 6
   - Field Dice -> slot 7

2. Configure field (edit line 1):
```
_G.field = "Pepper Patch"
```

3. Run script while on your field

## Fields

Sunflower Field, Dandelion Field, Mushroom Field, Blue Flower Field, Clover Field, Spider Field, Strawberry Field, Bamboo Field, Pineapple Patch, Stump Field, Cactus Field, Pumpkin Patch, Pine Tree Forest, Rose Field, Mountain Top Field, Pepper Patch, Coconut Field

## Custom Slots

Change line 2 if using different slots:
```
_G.slots = {LoadedDice = 5, Glitter = 6, FieldDice = 7}
```

## How It Works

1. Waits for existing boost to expire
2. Uses Glitter → wait 60s → rolls Loaded Dice until field you choose → uses Glitter again
3. Maintains x4 by alternating Field Dice and Glitter when timer drops below 2 minutes
4. Auto restarts if boost expires
