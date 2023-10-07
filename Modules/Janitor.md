# JFE Map Making - MapScript/Janitor
The janitor module controls the deletion of any game instances. It can be used via `local janitor = utils:GetModule("Janitor")`.

-----------------------------------------------------

## Functions
### janitor.new(...: `any`): {objs = {any}}

Demonstration:
```lua
local newJanitor = janitor.new(unpack(utils.Map.ExampleFolder:GetChildren())) --Creates a new janitor in control of the children inside the example map folder
```
This function allows you to create a new janitor.

-----------------------------------------------------

### janitor:Cleanup(): nil

Demonstration:
```lua
local newJanitor = janitor.new(unpack(utils.Map.ExampleFolder:GetChildren()))

task.wait(30) --Waits 30 seconds
newJanitor:Cleanup() --Destroys the children in the example folder
```
This function will allow the janitor to cleanup the children by destroying them. Useful when you no longer need it for a period of time.
