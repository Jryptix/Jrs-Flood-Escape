# JFE Map Making - MapScript/Content
The content module can utilize the content in the player's PlayerGui in many different ways. It can be used via `local content = utils:GetModule("Content")`.

-----------------------------------------------------

## Functions
### content:LoadGui(gui: [`ScreenGui`](https://create.roblox.com/docs/reference/engine/classes/ScreenGui)): nil

Demonstration:
```lua
content:LoadGui(script.ExampleGui) --The Gui is a direct child inside the script and will be loaded.
```
This function allows to load the GUI inside of the player, this is strictly used for the LocalMapScript. This effect will apply to other spectators.

-----------------------------------------------------

## Functions
### content:ToggleCinematic(active: `boolean`): nil

Demonstration:
```lua
content:ToggleCinematic(true) --This will toggle the cinematic bars of the player's PlayerGui.
```
This function allows to control the cinematic bars of the player's PlayerGui. It can be used to give intensity to the player when climbing a tower section.
