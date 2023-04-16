# JFE Map Making - MapScript
MapUtils is the main utilties used to function in JFE maps. For short, it is called 'utils'. 

## Methods
### utils:Move(part: `PVInstance`, risevector: `Vector3`, interval: `number`): nil

Demonstration:
```lua
utils:Move(map.MovingParts.Liquids._Liquid1, Vector3.new(0, 40, 0), 5)
```
This function allows to move a part by a number of studs based on the Vector3 values provided (X, Y, Z).

-----------------------------------------------------

### utils:MoveLocal(part: `PVInstance`, risevector: `Vector3`, interval: `number`): nil

Demonstration:
```lua
utils:Move(map.MovingParts.Liquids._Liquid1, Vector3.new(0, 40, 0), 5)
```
This function allows to move a part by a number of studs based on the Vector3 values provided (X, Y, Z), similar to utils:Move but it moves based on the part's orientation.

-----------------------------------------------------

### utils:ButtonEvent(buttonNumber: `number`): RBXScriptSignal?

Demonstration:
```lua
utils:ButtonEvent(2):Connect(function()
  --Line of code when button #2 is pressed
end)
```
This function is called when a specific button is pressed which depends on the button number.

-----------------------------------------------------

### utils:ChangeState(part: `BasePart`, liquidState: `string`): nil

Demonstration:
```lua
utils:ChangeState(map.MovingParts.Liquids._Liquid2, "acid")
```
This functions allows to change the state of the liquid, these being `water`, `acid`, `lava` and `custom`.

-----------------------------------------------------
