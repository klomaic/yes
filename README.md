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
local NoVoid = Instance.new("TextButton")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
ScreenGui.ResetOnSpawn = false

OpenClose.Name = "Open/Close"
OpenClose.Parent = ScreenGui
OpenClose.BackgroundColor3 = Color3.fromRGB(25, 255, 0)
OpenClose.Position = UDim2.new(0.253125012, 0, 0.00245399773, 0)
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
Spawn.Position = UDim2.new(0.154000029, 0, 1.28016293, 0)
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
MiddleIsland.Position = UDim2.new(0.154000029, 0, 4.42527914, 0)
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
Speed.Position = UDim2.new(0.154000029, 0, 3.38574457, 0)
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
MegaVip.Position = UDim2.new(0.153958306, 0, 2.34663725, 0)
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
ui.Position = UDim2.new(0.153456375, 0, 6.42345285, 0)
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

NoVoid.Name = "NoVoid"
NoVoid.Parent = OpenClose
NoVoid.BackgroundColor3 = Color3.fromRGB(132, 198, 174)
NoVoid.Position = UDim2.new(0.154000029, 0, 5.35551167, 0)
NoVoid.Size = UDim2.new(0, 138, 0, 45)
NoVoid.Visible = false
NoVoid.Font = Enum.Font.SourceSans
NoVoid.Text = "NoVoid"
NoVoid.TextColor3 = Color3.fromRGB(0, 0, 0)
NoVoid.TextScaled = true
NoVoid.TextSize = 14.000
NoVoid.TextWrapped = true

-- Scripts:

local function RHXBNZD_fake_script() -- Spawn.LocalScript 
	local script = Instance.new('LocalScript', Spawn)

	script.Parent.MouseButton1Click:Connect(function()
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-0.641228, 268, 2.08173)
	end)
end
coroutine.wrap(RHXBNZD_fake_script)()
local function DUZRKZO_fake_script() -- MiddleIsland.LocalScript 
	local script = Instance.new('LocalScript', MiddleIsland)

	script.Parent.MouseButton1Click:Connect(function()
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(4,194,-6)
	end)
end
coroutine.wrap(DUZRKZO_fake_script)()
local function FRQVGX_fake_script() -- Speed.Script 
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
coroutine.wrap(FRQVGX_fake_script)()
local function VHTCV_fake_script() -- MegaVip.Script 
	local script = Instance.new('Script', MegaVip)

	local plr = game.Players.LocalPlayer
	
	script.Parent.MouseButton1Click:Connect(function()
		plr.Character.HumanoidRootPart.CFrame = CFrame.new(0, 262.5, 57)
	end)
end
coroutine.wrap(VHTCV_fake_script)()
local function UCZGKL_fake_script() -- TextButton.LocalScript 
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
coroutine.wrap(UCZGKL_fake_script)()
local function EMRDHWM_fake_script() -- OpenClose.LocalScript 
	local script = Instance.new('LocalScript', OpenClose)

	local db = true
	local par = script.Parent
	local spaw = par.Spawn
	local mid = par.MiddleIsland
	local speed = par.Speed
	local Mega = par["Mega Vip"]
	local ui = par.ui	
	local novoid = par.NoVoid
	script.Parent.MouseButton1Click:Connect(function()
		if script.Parent.Spawn.Visible == false and db == true then
			db = false
			par.Text = "Close"
			spaw.Visible = true
			mid.Visible = true
			speed.Visible = true
			Mega.Visible = true
			ui.Visible = true
			novoid.Visible = true
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
			novoid.Visible = false
			wait(.0001)
			db = true
		end
	end)
end
coroutine.wrap(EMRDHWM_fake_script)()
local function JBWK_fake_script() -- NoVoid.LocalScript 
	local script = Instance.new('LocalScript', NoVoid)

	script.Parent.MouseButton1Click:Connect(function()
		local p = Instance.new("Part")
		p.Parent = game.Workspace
		p.Anchored = true
		p.Size = Vector3.new(250,1,250)
		p.Position = Vector3.new(-3.96463, 149.5, 11.5604)
		p.Material = "Wood"
		p.Transparency = 0.4
	end)
end
coroutine.wrap(JBWK_fake_script)()
