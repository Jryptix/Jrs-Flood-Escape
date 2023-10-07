# JFE Map Making - MapScript/Camera
The camera module can utilize the player's camera in many different ways. It can be used via `local camera = utils:GetModule("Camera")`.

-----------------------------------------------------

## Functions
### camera:ShakeOnce(intensity: [`NumberRange?`](https://create.roblox.com/docs/reference/engine/datatypes/NumberRange), duration: [`NumberRange?`](https://create.roblox.com/docs/reference/engine/datatypes/NumberRange), sound: [`Sound?`](https://create.roblox.com/docs/reference/engine/classes/Sound)): nil

Demonstration:
```lua
camera:ShakeOnce(NumberRange.new(5,10), NumberRange.new(10,20)) --The number range allows you to have a randomized numbers.

--Using custom sounds:
local sound = Instance.new("Sound")
sound.SoundId = "rbxassetid://2674547670"
sound.Parent = script

camera:ShakeOnce(NumberRange.new(5,10), NumberRange.new(10,20), sound)
```
This function allows to shake the player's camera only once. Optionally you can add a custom sound.

-----------------------------------------------------

### camera:ShakeRepeat(intensity: [`NumberRange?`](https://create.roblox.com/docs/reference/engine/datatypes/NumberRange), duration: [`NumberRange?`](https://create.roblox.com/docs/reference/engine/datatypes/NumberRange), sound: [`Sound?`](https://create.roblox.com/docs/reference/engine/classes/Sound), delay: `number`): nil

Demonstration:
```lua
camera:ShakeRepeat(NumberRange.new(5,10), NumberRange.new(10,20)) --The number range allows you to have a randomized numbers.

--Using custom sounds:
local sound = Instance.new("Sound")
sound.SoundId = "rbxassetid://2674547670"
sound.Parent = script

camera:ShakeRepeat(NumberRange.new(5,10), NumberRange.new(10,20), sound)
```
This function allows to shake the player's repeatedly during the round. Optionally you can add a custom sound.

-----------------------------------------------------

### camera:TiltCamera(tilt: `number`): nil

Demonstration:
```lua
camera:TiltCamera(180) --This makes the player's camera turn 180 degrees, making the camera upside down.
```
This function allows to tilt the player's camera during the round.
