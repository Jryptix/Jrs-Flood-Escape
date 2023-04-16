# JFE Map Making - MapScript
MapUtils is the main utilties used to function in JFE maps. For short, it is called 'utils'. 

## Methods
### utils:Move(part: PVInstance, risevector: Vector3, interval: number)

Demonstration:
```lua
utils:Move(map.MovingParts.Liquids._Liquid1, Vector3.new(0, 40, 0), 5)
```
This function allows to move a part by a number of studs based on the Vector3 values provided (X, Y, Z).
