-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local OpenClose = Instance.new("TextButton")
local Spawn = Instance.new("TextButton")
local MiddleIsland = Instance.new("TextButton")
local Speed = Instance.new("TextButton")
local MegaVip = Instance.new("TextButton")
local ui = Instance.new("TextBox")
local UICorner = Instance.new("UICorner")
local TextButton = Instance.new("TextButton")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
ScreenGui.ResetOnSpawn = false

OpenClose.Name = "Open/Close"
OpenClose.Parent = ScreenGui
OpenClose.BackgroundColor3 = Color3.fromRGB(25, 255, 0)
OpenClose.Position = UDim2.new(0.0463541672, 0, 0.208588973, 0)
OpenClose.Size = UDim2.new(0, 200, 0, 43)
OpenClose.Font = Enum.Font.Gotham
OpenClose.Text = "Open"
OpenClose.TextColor3 = Color3.fromRGB(0, 0, 0)
OpenClose.TextScaled = true
OpenClose.TextSize = 14.000
OpenClose.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
OpenClose.TextStrokeTransparency = 0.000
OpenClose.TextWrapped = true

Spawn.Name = "Spawn"
Spawn.Parent = OpenClose
Spawn.BackgroundColor3 = Color3.fromRGB(132, 198, 174)
Spawn.Position = UDim2.new(0.999000013, 0, 6.44295359, 0)
Spawn.Size = UDim2.new(0, 138, 0, 45)
Spawn.Visible = false
Spawn.Font = Enum.Font.SourceSans
Spawn.Text = "Spawn"
Spawn.TextColor3 = Color3.fromRGB(0, 0, 0)
Spawn.TextScaled = true
Spawn.TextSize = 14.000
Spawn.TextWrapped = true

MiddleIsland.Name = "MiddleIsland"
MiddleIsland.Parent = OpenClose
MiddleIsland.BackgroundColor3 = Color3.fromRGB(132, 198, 174)
MiddleIsland.Position = UDim2.new(0.999000013, 0, 9.58806992, 0)
MiddleIsland.Size = UDim2.new(0, 138, 0, 45)
MiddleIsland.Visible = false
MiddleIsland.Font = Enum.Font.SourceSans
MiddleIsland.Text = "Middle Island"
MiddleIsland.TextColor3 = Color3.fromRGB(0, 0, 0)
MiddleIsland.TextScaled = true
MiddleIsland.TextSize = 14.000
MiddleIsland.TextWrapped = true

Speed.Name = "Speed"
Speed.Parent = OpenClose
Speed.BackgroundColor3 = Color3.fromRGB(132, 198, 174)
Speed.Position = UDim2.new(0.999000013, 0, 8.54853535, 0)
Speed.Size = UDim2.new(0, 138, 0, 45)
Speed.Visible = false
Speed.Font = Enum.Font.SourceSans
Speed.Text = "Speed"
Speed.TextColor3 = Color3.fromRGB(0, 0, 0)
Speed.TextScaled = true
Speed.TextSize = 14.000
Speed.TextWrapped = true

MegaVip.Name = "Mega Vip"
MegaVip.Parent = OpenClose
MegaVip.BackgroundColor3 = Color3.fromRGB(132, 198, 174)
MegaVip.Position = UDim2.new(0.99895829, 0, 7.50942802, 0)
MegaVip.Size = UDim2.new(0, 138, 0, 45)
MegaVip.Visible = false
MegaVip.Font = Enum.Font.SourceSans
MegaVip.Text = "Mega Vip"
MegaVip.TextColor3 = Color3.fromRGB(0, 0, 0)
MegaVip.TextScaled = true
MegaVip.TextSize = 14.000
MegaVip.TextWrapped = true

ui.Name = "ui"
ui.Parent = OpenClose
ui.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ui.Position = UDim2.new(0.998456359, 0, 10.6327553, 0)
ui.Size = UDim2.new(0, 138, 0, 33)
ui.Visible = false
ui.Font = Enum.Font.SourceSans
ui.Text = ""
ui.TextColor3 = Color3.fromRGB(0, 0, 0)
ui.TextScaled = true
ui.TextSize = 14.000
ui.TextWrapped = true

UICorner.Parent = ui

TextButton.Parent = ui
TextButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton.Position = UDim2.new(0, 0, 1, 0)
TextButton.Size = UDim2.new(0, 138, 0, 40)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = "GO"
TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton.TextScaled = true
TextButton.TextSize = 14.000
TextButton.TextWrapped = true

-- Scripts:

local function FYJEL_fake_script() -- Spawn.LocalScript 
	local script = Instance.new('LocalScript', Spawn)

	script.Parent.MouseButton1Click:Connect(function()
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-0.641228, 268, 2.08173)
	end)
end
coroutine.wrap(FYJEL_fake_script)()
local function XYSAUUR_fake_script() -- MiddleIsland.LocalScript 
	local script = Instance.new('LocalScript', MiddleIsland)

	script.Parent.MouseButton1Click:Connect(function()
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(4,194,-6)
	end)
end
coroutine.wrap(XYSAUUR_fake_script)()
local function YSCLF_fake_script() -- Speed.Script 
	local script = Instance.new('Script', Speed)

	local plr = game.Players.LocalPlayer
	
	script.Parent.MouseButton1Click:Connect(function()
		if plr.Character.Humanoid.WalkSpeed == 16 then
			game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 40
		else
			plr.Character.Humanoid.WalkSpeed = 16
		end
	end)
end
coroutine.wrap(YSCLF_fake_script)()
local function BLTGNL_fake_script() -- MegaVip.Script 
	local script = Instance.new('Script', MegaVip)

	local plr = game.Players.LocalPlayer
	
	script.Parent.MouseButton1Click:Connect(function()
		plr.Character.HumanoidRootPart.CFrame = CFrame.new(0, 262.5, 57)
	end)
end
coroutine.wrap(BLTGNL_fake_script)()
local function EJZRHM_fake_script() -- TextButton.LocalScript 
	local script = Instance.new('LocalScript', TextButton)

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
coroutine.wrap(EJZRHM_fake_script)()
local function DWGZV_fake_script() -- OpenClose.LocalScript 
	local script = Instance.new('LocalScript', OpenClose)

	local db = true
	local par = script.Parent
	local spaw = par.Spawn
	local mid = par.MiddleIsland
	local speed = par.Speed
	local Mega = par["Mega Vip"]
	local ui = par.ui	
	script.Parent.MouseButton1Click:Connect(function()
		if script.Parent.Spawn.Visible == false and db == true then
			db = false
			par.Text = "Close"
			spaw.Visible = true
			mid.Visible = true
			speed.Visible = true
			Mega.Visible = true
			ui.Visible = true
			wait(.0001)
			db = true 
		else 
			db = false
			par.Text = "Open"
			spaw.Visible = false
			mid.Visible = false
			speed.Visible = false
			Mega.Visible = false
			ui.Visible = false
			wait(.0001)
			db = true
			print("leave a bloody scene")
		end
	end)
end
coroutine.wrap(DWGZV_fake_script)()
