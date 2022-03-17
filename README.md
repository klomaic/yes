-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local TextButton = Instance.new("TextButton")
local UICorner = Instance.new("UICorner")
local TextButton_2 = Instance.new("TextButton")
local UICorner_2 = Instance.new("UICorner")
local TextButton_3 = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")
local ui = Instance.new("TextBox")
local UICorner_4 = Instance.new("UICorner")
local TextButton_4 = Instance.new("TextButton")
local TextButton_5 = Instance.new("TextButton")
local UICorner_5 = Instance.new("UICorner")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
ScreenGui.ResetOnSpawn = false

TextButton.Parent = ScreenGui
TextButton.BackgroundColor3 = Color3.fromRGB(132, 198, 174)
TextButton.Position = UDim2.new(0.00181818183, 0, 0.540029109, 0)
TextButton.Size = UDim2.new(0, 138, 0, 50)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = "Spawn"
TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton.TextScaled = true
TextButton.TextSize = 14.000
TextButton.TextWrapped = true

UICorner.Parent = TextButton

TextButton_2.Parent = ScreenGui
TextButton_2.BackgroundColor3 = Color3.fromRGB(132, 198, 174)
TextButton_2.Position = UDim2.new(0, 0, 0.621542931, 0)
TextButton_2.Size = UDim2.new(0, 138, 0, 50)
TextButton_2.Font = Enum.Font.SourceSans
TextButton_2.Text = "Middle Island"
TextButton_2.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton_2.TextScaled = true
TextButton_2.TextSize = 14.000
TextButton_2.TextWrapped = true

UICorner_2.Parent = TextButton_2

TextButton_3.Parent = ScreenGui
TextButton_3.BackgroundColor3 = Color3.fromRGB(132, 198, 174)
TextButton_3.Position = UDim2.new(0, 0, 0.704512358, 0)
TextButton_3.Size = UDim2.new(0, 138, 0, 50)
TextButton_3.Font = Enum.Font.SourceSans
TextButton_3.Text = "Speed"
TextButton_3.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton_3.TextScaled = true
TextButton_3.TextSize = 14.000
TextButton_3.TextWrapped = true

UICorner_3.Parent = TextButton_3

ui.Name = "ui"
ui.Parent = ScreenGui
ui.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ui.Position = UDim2.new(0.0927272737, 0, 0.551673949, 0)
ui.Size = UDim2.new(0, 138, 0, 33)
ui.Font = Enum.Font.SourceSans
ui.Text = ""
ui.TextColor3 = Color3.fromRGB(0, 0, 0)
ui.TextSize = 14.000

UICorner_4.Parent = ui

TextButton_4.Parent = ui
TextButton_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton_4.Position = UDim2.new(0, 0, 1, 0)
TextButton_4.Size = UDim2.new(0, 138, 0, 40)
TextButton_4.Font = Enum.Font.SourceSans
TextButton_4.Text = "GO"
TextButton_4.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton_4.TextScaled = true
TextButton_4.TextSize = 14.000
TextButton_4.TextWrapped = true

TextButton_5.Parent = ScreenGui
TextButton_5.BackgroundColor3 = Color3.fromRGB(132, 198, 174)
TextButton_5.Position = UDim2.new(0, 0, 0.78893739, 0)
TextButton_5.Size = UDim2.new(0, 138, 0, 50)
TextButton_5.Font = Enum.Font.SourceSans
TextButton_5.Text = "Mega Vip"
TextButton_5.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton_5.TextScaled = true
TextButton_5.TextSize = 14.000
TextButton_5.TextWrapped = true

UICorner_5.Parent = TextButton_5

-- Scripts:

local function INVULL_fake_script() -- TextButton.LocalScript 
	local script = Instance.new('LocalScript', TextButton)

	script.Parent.MouseButton1Click:Connect(function()
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-0.641228, 268, 2.08173)
	end)
end
coroutine.wrap(INVULL_fake_script)()
local function PMZI_fake_script() -- TextButton_2.LocalScript 
	local script = Instance.new('LocalScript', TextButton_2)

	script.Parent.MouseButton1Click:Connect(function()
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(4,194,-6)
	end)
end
coroutine.wrap(PMZI_fake_script)()
local function ZJECICO_fake_script() -- TextButton_3.Script 
	local script = Instance.new('Script', TextButton_3)

	local plr = game.Players.LocalPlayer
	
	script.Parent.MouseButton1Click:Connect(function()
		if plr.Character.Humanoid.WalkSpeed == 16 then
			game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 40
		else
			plr.Character.Humanoid.WalkSpeed = 16
		end
	end)
end
coroutine.wrap(ZJECICO_fake_script)()
local function DNSZAL_fake_script() -- TextButton_4.LocalScript 
	local script = Instance.new('LocalScript', TextButton_4)

	local text = script.Parent.Parent
	
	script.Parent.MouseButton1Click:Connect(function()
		local me = game.Players.LocalPlayer
		local char = me.Character
		local person = text.Text
		getgenv().farmer = true
	
		while wait(.001) do 
			if getgenv().farmer == true then
				char.HumanoidRootPart.CFrame = game.Workspace[person].HumanoidRootPart.CFrame*CFrame.new(-2,-4.552,1)
				if game.Workspace[person].Humanoid.Health == 0 or char.Humanoid.Health < 5 then
					char.HumanoidRootPart.CFrame = CFrame.new(4,194,-6)
					getgenv().farmer = false
				end
			end
		end
	end)
end
coroutine.wrap(DNSZAL_fake_script)()
local function ZAEW_fake_script() -- TextButton_5.Script 
	local script = Instance.new('Script', TextButton_5)

	local plr = game.Players.LocalPlayer
	
	script.Parent.MouseButton1Click:Connect(function()
		plr.Character.HumanoidRootPart.CFrame = CFrame.new(0, 262.5, 57)
	end)
end
coroutine.wrap(ZAEW_fake_script)()
