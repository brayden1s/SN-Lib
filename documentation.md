# Documenation

## Creating a window
```lua
local Library = loadstring(game:HttpGet('https://raw.githubusercontent.com/vFishyTurtle/SN-Lib/main/src'))()
local lib = Library:CreateWindow({Title = "SN Lib"})
```

## Creating a tab
```lua
local t1 = lib:NewTab({Name = "Catching"})
```
## Adding a Section
```lua
local s1 = t1:NewSection({Name = "Section"})
```

## Adding a toggle
```lua
s1:NewToggle({
	Name = "Magnets",
	default = false,
	callback = function(v)
		print(v)
	end,
})
```

## Adding a slider
```lua
t1:NewSlider({
	Name = "Magnets Range",
	default = 50,
	min = 0,
	max = 100,
	callback = function(v)
		print(v)
	end,
})
```

## Adding a button
```lua
t1:NewButton({
	Name = "Button Yay",
	callback = function(v)
		print("Yay")
	end,
})
```

## Adding a dropdown
```lua
s1:NewDropdown({
	Name = "Dropdown lol",
	options = {"Apple", "Banana", "Grape"},
	default = "Grape",
	callback = function(v)
		print(v)
	end,
})
```
