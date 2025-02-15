# Secret-UI-Library

```lua
local sex = loadstring(game:HttpGet('https://raw.githubusercontent.com/3345-c-a-t-s-u-s/Garry-UI/main/source'))()
```
#create the window
```lua
local Window = sex:Create('BEDOL HUB','BLADE BALL','TESTER')
```
#Create the tab
```lua
local ExampleTab = Window:CreateTab('Example','earth')
```
#create the button
```lua
ExampleTab:CreateButton("Button",function()
	print('press button')
end)
```
#create the label
```lua
ExampleTab:CreateLabel("Label")
```
#create the toggle
```lua
ExampleTab:CreateToggle("Toggle",false,function(val)
	print('toggle',val)
end)
```
#create the keybind
```lua
ExampleTab:CreateKeybind("Keybind",Enum.KeyCode.E,function(val)
	print('keybind',val)
end)
```
#create the slider
```lua
ExampleTab:CreateSlider("Slider",1,100,10,function(val)
	print('slider',val)
end)
```
#create window button
```lua
Window:CreateButton('earth',false,function(val)
	print('set time')
	if val then
		Window:Notify('Time Change','Night',1.5)
		game:GetService('TweenService'):Create(game:GetService('Lighting'),TweenInfo.new(0.5),{ClockTime = 0}):Play()
	else
		Window:Notify('Time Change','Day',1.5)
		game:GetService('TweenService'):Create(game:GetService('Lighting'),TweenInfo.new(0.5),{ClockTime = 14}):Play()
	end
end)
```
#create window ads button
```lua
Window:CreateButton('ads',false,function(val)
	print('fov change')
	if val then
		Window:Notify('FOV Change','120',1)
		game:GetService('TweenService'):Create(workspace.CurrentCamera,TweenInfo.new(0.5),{FieldOfView = 120}):Play()
	else
		Window:Notify('FOV Change','70',1)
		game:GetService('TweenService'):Create(workspace.CurrentCamera,TweenInfo.new(0.5),{FieldOfView = 70}):Play()
	end
end)
```
