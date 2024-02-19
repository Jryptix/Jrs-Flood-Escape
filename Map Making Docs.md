> ### Contents:
> 1. Settings
> 2. Buttons
> 3. Functionality
> 4. Map Script

# [Settings](https://create.roblox.com/docs/reference/engine/classes/Configuration)
Settings is a configuration folder that is provided in your map kit. It is one of the key components when making a map and is essential to be setup.

## [BGM](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value for any BGM to be played within your map with the given music ID that is in the number value.

## [Creator](https://create.roblox.com/docs/reference/engine/classes/StringValue)
This is a placeholder value to put the name of who created the map and/or possibly contributors.

## [Difficulty](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value to put the difficulty of the map in which they are ranked in order by valid numbers.

Here is a list of difficulties:

- `[1]` - Easy
- `[2]` - Normal
- `[3]` - Hard
- `[4]` - Difficult
- `[5]` - Insane
- `[6]` - Intense
- `[7]` - Divine
- `[8]` - Perpetual
- `[Others]` - Invalid difficulty

If a number is put that isn't in the list, it will be ranked as Invalid difficulty \[x].

## [Map Image](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value for any decal to symbolize your map within the given *texture* ID that is the number value.
To get a texture ID, it is formatted in `rbxassetid://[texture-id]`. It is always a value for inserting images into decals, textures, beams and GUIs.

## [Map Name](https://create.roblox.com/docs/reference/engine/classes/StringValue)
This is a placeholder value to put the name of your map. This is the most necessary and important component to your map. The name has to fit the map's design and gameplay.

## [Max Time](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value for the max time you can put in your map. The max time is how long you can be in the map for.

## [Privacy](https://create.roblox.com/docs/reference/engine/classes/StringValue)
This is a placeholder value to set the playability either to `Public`, `Friends Only` or `Owner Only` depending if you want to prevent other players from loading your map.

## [Button](https://create.roblox.com/docs/reference/engine/classes/Configuration)
This is a configuration folder that is provided to customize how buttons are managed within the map.

### [Activated Color](https://create.roblox.com/docs/reference/engine/classes/Color3Value)
This is a placeholder value to set the color of the button light after it is pressed.

### [Active Color](https://create.roblox.com/docs/reference/engine/classes/Color3Value)
This is a placeholder value to set the color of the button light when it is ready to be pressed.

### [Group Color](https://create.roblox.com/docs/reference/engine/classes/Color3Value)
This is a placeholder value to set the color of the button light when it requires multiple people to press it when it is active.

### [Inactive Color](https://create.roblox.com/docs/reference/engine/classes/Color3Value)
This is a placeholder value to set the color of the button light when it isn't ready to be pressed yet.

### [Locator Image](https://create.roblox.com/docs/reference/engine/classes/StringValue)
This is a placeholder value to set the image of the button locator given from the *texture* ID or setting it to the `default` locator used from the game.
To get a texture ID, it is formatted in `rbxassetid://[texture-id]`. It is always a value for inserting images into decals, textures, beams and GUIs.

## [Custom Liquids](https://create.roblox.com/docs/reference/engine/classes/Configuration)
This is a configuration folder that is provided to customize your own liquid state (`custom`) that resides from `water`, `acid` and `lava`.

### [Color](https://create.roblox.com/docs/reference/engine/classes/Color3Value)
This is a placeholder value to set the color of your `custom` liquid state.

### [Oxygen Depletion](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value to set the oxygen depletion rate of your `custom` liquid state. When a player character enters this liquid with this state, the oxgyen rate will drop by how much the oxgyen depletion rate is in this value.

### [Splash Sound](https://create.roblox.com/docs/reference/engine/classes/StringValue)
This is a placeholder value for any splash sound effect to be played when entering the liquid state with the given audio ID that is in the string value.
Alternatively, you can use the default liquid splash sounds: `water`, `acid` or `lava`.

## [Lighting](https://create.roblox.com/docs/reference/engine/classes/Configuration)
This is a configuration folder that is provided to change the map lighting using [`game:GetService("Lighting")`](https://create.roblox.com/docs/reference/engine/classes/Lighting).

### [Ambient](https://create.roblox.com/docs/reference/engine/classes/Color3Value)
This is a placeholder value to set the color of `game.Lighting.Ambient`.

### [Brightness](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value to set the number of the brightness via `game.Lighting.Brightness`.

### [Color Shift Bottom](https://create.roblox.com/docs/reference/engine/classes/Color3Value)
This is a placeholder value to set the color of `game.Lighting.ColorShift_Bottom`.

### [Color Shift Top](https://create.roblox.com/docs/reference/engine/classes/Color3Value)
This is a placeholder value to set the color of `game.Lighting.ColorShift_Top`.

### [Environment Diffuse Scale](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value to set a number of `game.Lighting.EnvironmentDiffuseScale`.

### [Environment Specular Scale](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value to set a number of `game.Lighting.EnvironmentSpecularScale`.

### [Fog Color](https://create.roblox.com/docs/reference/engine/classes/Color3Value)
This is a placeholder value to set the color of `game.Lighting.FogColor`.

### [Fog End](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value to set the number of `game.Lighting.FogEnd`. This is the radius of the fog surrounding you player character. The smaller the number, the more fog covers your surroundings.

### [Fog Start](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value to set the number of `game.Lighting.FogEnd`. This is the radius of the fog surrounding you player character. The smaller the number, the less fog covers your surroundings.

### [Global Shadows](https://create.roblox.com/docs/reference/engine/classes/BoolValue)
This is a value whether you can enable global shadows via `game.Lighting.GlobalShadows`.

### [Outdoor Ambient](https://create.roblox.com/docs/reference/engine/classes/Color3Value)
This is a placeholder value to set the color of `game.Lighting.OutdoorAmbient`.

### [Shadow Softness](https://create.roblox.com/docs/reference/engine/classes/NumberValue)
This is a placeholder value to set a number of the softness of shadows via  `game.Lighting.ShadowSoftness`.

### [Time Of Day](https://create.roblox.com/docs/reference/engine/classes/StringValue)
This is a placeholder value to set a 24-hour time string representation of `game.Lighting.TimeOfDay`.

# Buttons
Buttons are a necessary component to each and every map. They must be parented inside interactives in your map model via `map.Interactives`. (`map` being your model)
An action can be applied to any part that must also be parented inside `map.Interactives`. This is yet adding a object value inside the part you want to apply action to.

This is a list of named object values:
(Key: `btn#` can be any button number)

> ## Appear
> If a part has an object value called `_Appear[btn#]`, then that part will become visible by turning `CanCollide` to true and setting the `Transparency` to 0.

> ## Fade
> If a part has an object value called `_Fade[btn#]`, then that part will become invisible by turning `CanCollide` to false and setting the `Transparency` to 1.

> ## Fall
> If a part has an object value called `_Fall[btn#]`, then that part will become unanchored and can fall if it is possible with collisions.

> ## Explode
> If a part has an object value called `_Explode[btn#]`, then that part will explode on disappearance. It does not do any damage however.

## Delay
Any action can be delayed before being fired. In order to do this, you can add a number value inside the object value called `_Delay`. The value inside the 'number value' will be the amount of seconds of delay before the action is fired.

## Models
If a model has an object value named one of the values above, then the parts inside the model will be affected by it.

# Functionality
The functionality for your map is crucial and imperative if you want to play it.
There must be a set of instances parented directly into your map model. This is so the server can detect what components are there in your map model and be able to load it correctly.

- Exit folder (`map.Exit`): [`Folder`](https://create.roblox.com/docs/reference/engine/classes/Folder)
- Interactives folder (`map.Interactives`): [`Folder`](https://create.roblox.com/docs/reference/engine/classes/Folder)
- MapScript (`map.MapScript`): [`Script`](https://create.roblox.com/docs/reference/engine/classes/Script)
- LocalMapScript (`map.LocalMapScript`): [`LocalScript`](https://create.roblox.com/docs/reference/engine/classes/LocalScript)
- Spawn (`map.Spawn`): [`Part`](https://create.roblox.com/docs/reference/engine/classes/Part)
- Settings (`map.Settings`): [`Configuration`](https://create.roblox.com/docs/reference/engine/classes/Configuration)

The exit and the settings folder must have the exact same and only those descendants in that folder when you have the model setup. If none of these aren't followed, then your map will not work.
This is most likely because the server will require them and look for them inside your map model. This can also cause the entire game to break, as it is still in unfinished state.

# Map Script
For more information on how to script your map, see **[MapUtils](https://github.com/Jryptix/Jrs-Flood-Escape/blob/main/MapUtils.md)**.
