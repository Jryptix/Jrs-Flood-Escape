# JFE Map Making - MapScript
MapUtils is the main utilties used to function in JFE maps. For short, it is called 'utils'. 

## Properties
### utils.Map: [`Model`](https://create.roblox.com/docs/reference/engine/classes/Model)
```
local map = utils.Map
```
This property references your map model.

-----------------------------------------------------

## Functions
### utils:Move(part: [`PVInstance`](https://create.roblox.com/docs/reference/engine/classes/PVInstance), risevector: [`Vector3`](https://create.roblox.com/docs/reference/engine/datatypes/Vector3), interval: `number`): nil

Demonstration:
```lua
utils:Move(map.MovingParts.Liquids._Liquid1, Vector3.new(0, 40, 0), 5)
```
This function allows to move a part by a number of studs based on the Vector3 values provided (X, Y, Z).

-----------------------------------------------------

### utils:MoveLocal(part: [`PVInstance`](https://create.roblox.com/docs/reference/engine/classes/PVInstance), risevector: [`Vector3`](https://create.roblox.com/docs/reference/engine/datatypes/Vector3), interval: `number`): nil

Demonstration:
```lua
utils:Move(map.MovingParts.Liquids._Liquid1, Vector3.new(0, 40, 0), 5)
```
This function allows to move a part by a number of studs based on the Vector3 values provided (X, Y, Z), similar to utils:Move but it moves based on the part's orientation.

-----------------------------------------------------

### utils:ButtonEvent(buttonIndex: `number` | `string`): [RBXScriptSignal](https://create.roblox.com/docs/reference/engine/datatypes/RBXScriptSignal)?

Demonstration:
```lua
--Example #1
utils:ButtonEvent(2):Connect(function(player)
  --Line of code when button #2 is pressed
end)

--Example #2
utils:ButtonEvent("3A"):Wait() --This would yield the MapScript until button #3A is pressed
```
This function is called when a specific button is pressed which depends on the button index. The index being a number if it is a normal button or a string if it is a pathbutton.
There is a parameter of the player pressing the button.

-----------------------------------------------------

### utils:ChangeState(part: [`BasePart`](https://create.roblox.com/docs/reference/engine/classes/BasePart), liquidState: `string`): nil

Demonstration:
```lua
utils:ChangeState(map.MovingParts.Liquids._Liquid2, "acid")
```
This function allows to change the state of the liquid, these being `water`, `acid`, `lava` and `custom`.

-----------------------------------------------------

### utils:Alert(message: `string`, messageColor: [`Color3`](https://create.roblox.com/docs/reference/engine/datatypes/Color3)): nil

Demonstration:
```lua
utils:Alert("Hello World!", Color3.fromRGB(255,255,255))
```
This function allows you to send alerts to all the clients during the map playthrough.

-----------------------------------------------------

### utils:ToggleCinematic(active: boolean): nil

Demonstration:
```lua
utils:ToggleCinematic(true)
```
This function allows you to toggle cinematic bars throughout the map for every player during the round. If called from LocalMapScript, it only do this for the player running the LocalScript.

-----------------------------------------------------


### utils:GetPlayersInGame(): {[`Player`](https://create.roblox.com/docs/reference/engine/classes/Player)}

Demonstration:
```lua
for i, player in pairs(utils:GetPlayersInGame()) do
  print(player.Name)
end
```
This function allows you to get a table of players during the round in the map.

-----------------------------------------------------

### utils:Teleport(touchedPart: [`BasePart`](https://create.roblox.com/docs/reference/engine/classes/BasePart), destination, [`BasePart`](https://create.roblox.com/docs/reference/engine/classes/BasePart) | [`Attachment`](https://create.roblox.com/docs/reference/engine/classes/Attachment)): nil

Demonstration:
```lua
utils:Teleport(map.Teleporters.ExampleTeleporter, map.Teleporters.ExampleDestination)
```
This function allows you to teleport players throughout the map if they are in the zone of a specific part.

-----------------------------------------------------
