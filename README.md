local Context = game:GetService("ScriptContext")
for _, Connection in next, getconnections(Context.Error) do
	Connection:Disable()
end


local ESP = loadstring(game:HttpGet("https://raw.githubusercontent.com/DOXSASHW/esp2/main/esp2"))()
ESP:Toggle(true)

ESP.Tracers = false
ESP.Names = false
ESP.Boxes = false

local Config = {
	WindowName = "CuteWare V1",
	Color = Color3.fromRGB(255,128,64),
	Keybind = Enum.KeyCode.LeftAlt
}

local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/AlexR32/Roblox/main/BracketV3.lua"))()
local Window = Library:CreateWindow(Config, game:GetService("CoreGui"))

local Tab1 = Window:CreateTab("Player")
local Tab2 = Window:CreateTab("Combat")
local Tab3 = Window:CreateTab("Visuals")
local Tab4 = Window:CreateTab("Anti")
local Tab5 = Window:CreateTab("Misc")
local Tab6 = Window:CreateTab("Lighting")
local Tab7 = Window:CreateTab("Teleports")
local Tab8 = Window:CreateTab("UI")

local Section1 = Tab1:CreateSection("Character 1")
local Section2 = Tab1:CreateSection("Support me!")
local Section3 = Tab8:CreateSection("Menu")
local Section4 = Tab8:CreateSection("Background")
local Section5 = Tab2:CreateSection("Combat")
local Section6 = Tab2:CreateSection("Combat Misc")
local Section7 = Tab3:CreateSection("Esp")
local Section8 = Tab3:CreateSection("World")
local Section9 = Tab4:CreateSection("Gun Mods")
local Section10 = Tab4:CreateSection("Game Anti")
local Section11 = Tab6:CreateSection("Full Bright")
local Section12 = Tab6:CreateSection("Fun")
local Section13 = Tab5:CreateSection("Random")
local Section14 = Tab7:CreateSection("Areas")
local Section15 = Tab7:CreateSection("Update Log")
local Section16 = Tab7:CreateSection("Team")
local Section17 = Tab7:CreateSection("Premium")

local function a(b, ...)
	local c = {
		...
	}
	for d, e in ipairs(c) do
		if not rawget(b, e) then
			return false
		end
	end;
	return true
end;
local f;
for d, e in ipairs(getgc(true)) do
	if typeof(e) == "table" and a(e, "A", "B", "GP", "EN") then
		f = e;
		break
	end
end;
hookfunction(f.A, function()
end)
hookfunction(f.B, function()
end)
local Toggle3 = Section13:CreateToggle("Auto Pickup", nil, function(State)
	getgenv().Instant = State

	while Instant do wait(0.5)
		for _,v in pairs(game:GetService("Workspace"):GetDescendants()) do
			if v:IsA("ProximityPrompt") and game:GetService("Players").LocalPlayer:DistanceFromCharacter(v.Parent.Position) <= 30 then
				fireproximityprompt(v,0)
				wait(0.1)
				fireproximityprompt(v,1)
			end
		end
	end
end)



loadstring(game:HttpGet("https://raw.githubusercontent.com/NougatBitz/BitzUtils/main/CriminalityFeatures.lua"))()


Section15:CreateLabel("Hyu Ego Znaet...")






local Toggle1 = Section13:CreateToggle("No fall damage", nil, function(State)
	_G.NoFallDamage = State
	local OldNameCall = nil
	OldNameCall = hookmetamethod(game, "__namecall", function(Self, ...)
		if not checkcaller() and getnamecallmethod() == "FireServer" and Self.Name == "__DFfDD" and _G.NoFallDamage then
			return
		end
		return OldNameCall(Self, ...)
	end)
end)

local Button1 = Section14:CreateButton("Vibe Check", function()
	_G.teleport = true

	while _G.teleport do wait()
		spawn(function()
			wait(10)
			_G.teleport = false
		end)
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4754.68848, -200.966553, -972.997437)
		local args = {
			[1] = "__--r",
			[2] = game.Players.LocalPlayer.Character.HumanoidRootPart.Position,
			[3] = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.Angles(0, 0, 0)} -- -4778.11719, -37.8545227, -800.468994, 0, 0, -1, 0, 1, 0, 1, 0, 0
		game:GetService("ReplicatedStorage").Events.__DFfDD:FireServer(unpack(args))
	end
end)

local Button2 = Section14:CreateButton("Tower", function()
	_G.teleport2 = true

	while _G.teleport2 do wait()
		spawn(function()
			wait(10)
			_G.teleport2 = false
		end)
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4458.69434, 120.390343, -890.67627, 0, 0, 1, 0, 1, -0, -1, 0, 0)
		local args = {
			[1] = "__--r",
			[2] = game.Players.LocalPlayer.Character.HumanoidRootPart.Position,
			[3] = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.Angles(0, 0, 0)}
		game:GetService("ReplicatedStorage").Events.__DFfDD:FireServer(unpack(args))
	end
end)

local Button3 = Section14:CreateButton("Dealer", function()
	_G.teleport3 = true

	while _G.teleport3 do wait()
		spawn(function()
			wait(10)
			_G.teleport3 = false
		end)
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4815.71484, 9.84649944, -711.355225, 0.707134247, -0.707079291, 0, -0.707079291, -0.707134247, -0, 0, 0, -1)
		local args = {
			[1] = "__--r",
			[2] = game.Players.LocalPlayer.Character.HumanoidRootPart.Position,
			[3] = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.Angles(0, 0, 0)}
		game:GetService("ReplicatedStorage").Events.__DFfDD:FireServer(unpack(args))
	end
end)


local Button3 = Section14:CreateButton("Atm", function()
	_G.teleport3 = true

	while _G.teleport3 do wait()
		spawn(function()
			wait(10)
			_G.teleport3 = false
		end)
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4463.01514, 0.90637207, -453.874664, -1.1920929e-07, 0, 1.00000012, 0, 1, 0, -1.00000012, 0, -1.1920929e-07)
		local args = {
			[1] = "__--r",
			[2] = game.Players.LocalPlayer.Character.HumanoidRootPart.Position,
			[3] = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.Angles(0, 0, 0)}
		game:GetService("ReplicatedStorage").Events.__DFfDD:FireServer(unpack(args))
	end
end)

local Button4 = Section14:CreateButton("Vibe Button", function()
	_G.teleport3 = true

	while _G.teleport3 do wait()
		spawn(function()
			wait(10)
			_G.teleport3 = false
		end)
		game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-4776.8501, -36.7657585, -808.682007, 0, 0, 1, 0, 1, -0, -1, 0, 0)
		local args = {
			[1] = "__--r",
			[2] = game.Players.LocalPlayer.Character.HumanoidRootPart.Position,
			[3] = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.Angles(0, 0, 0)}
		game:GetService("ReplicatedStorage").Events.__DFfDD:FireServer(unpack(args))
	end
end)

local Toggle2 = Section13:CreateToggle("Chat Spy", nil, function(State)
	--This script reveals ALL hidden messages in the default chat
	--chat "/spy" to toggle!
	enabled = State
	--if true will check your messages too
	spyOnMyself = true
	--if true will chat the logs publicly (fun, risky)
	public = false
	--if true will use /me to stand out
	publicItalics = true
	--customize private logs
	privateProperties = {
		Color = Color3.fromRGB(0,255,255); 
		Font = Enum.Font.SourceSansBold;
		TextSize = 18;
	}
	--////////////////////////////////////////////////////////////////
	local StarterGui = game:GetService("StarterGui")
	local Players = game:GetService("Players")
	local player = Players.LocalPlayer
	local saymsg = game:GetService("ReplicatedStorage"):WaitForChild("DefaultChatSystemChatEvents"):WaitForChild("SayMessageRequest")
	local getmsg = game:GetService("ReplicatedStorage"):WaitForChild("DefaultChatSystemChatEvents"):WaitForChild("OnMessageDoneFiltering")
	local instance = (_G.chatSpyInstance or 0) + 1
	_G.chatSpyInstance = instance

	local function onChatted(p,msg)
		if _G.chatSpyInstance == instance then
			if p==player and msg:lower():sub(1,4)=="/spy" then
				enabled = not enabled
				wait(0.3)
				privateProperties.Text = "{SPY "..(enabled and "EN" or "DIS").."ABLED}"
				StarterGui:SetCore("ChatMakeSystemMessage",privateProperties)
			elseif enabled and (spyOnMyself==true or p~=player) then
				msg = msg:gsub("[\n\r]",''):gsub("\t",' '):gsub("[ ]+",' ')
				local hidden = true
				local conn = getmsg.OnClientEvent:Connect(function(packet,channel)
					if packet.SpeakerUserId==p.UserId and packet.Message==msg:sub(#msg-#packet.Message+1) and (channel=="All" or (channel=="Team" and public==false and Players[packet.FromSpeaker].Team==player.Team)) then
						hidden = false
					end
				end)
				wait(1)
				conn:Disconnect()
				if hidden and enabled then
					if public then
						saymsg:FireServer((publicItalics and "/me " or '').."{SPY} [".. p.Name .."]: "..msg,"All")
					else
						privateProperties.Text = "{SPY} [".. p.Name .."]: "..msg
						StarterGui:SetCore("ChatMakeSystemMessage",privateProperties)
					end
				end
			end
		end
	end

	for _,p in ipairs(Players:GetPlayers()) do
		p.Chatted:Connect(function(msg) onChatted(p,msg) end)
	end
	Players.PlayerAdded:Connect(function(p)
		p.Chatted:Connect(function(msg) onChatted(p,msg) end)
	end)
	privateProperties.Text = "{SPY "..(enabled and "EN" or "DIS").."ABLED}"
	StarterGui:SetCore("ChatMakeSystemMessage",privateProperties)
	local chatFrame = player.PlayerGui.Chat.Frame
	chatFrame.ChatChannelParentFrame.Visible = true
	chatFrame.ChatBarParentFrame.Position = chatFrame.ChatChannelParentFrame.Position+UDim2.new(UDim.new(),chatFrame.ChatChannelParentFrame.Size.Y)
end)

local Label1 = Section5:CreateLabel("Label 1")
Label1:UpdateText("Aiming")
local Dropdown2 = Section5:CreateDropdown("Aimbot Hit Part", {"HumanoidRootPart","Torso","Head"}, function(State)
	_G.HitPart = State
end)

local Toggle1 = Section5:CreateToggle("Aimbot (V)", nil, function(State)
	getgenv().AimPart = tostring(_G.HitPart)-- For R15 Games: {UpperTorso, LowerTorso, HumanoidRootPart, Head} | For R6 Games: {Head, Torso, HumanoidRootPart}
	getgenv().AimlockToggleKey = "V" -- Toggles Aimbot On/Off 
	getgenv().AimRadius = 50 -- How far away from someones character you want to lock on at
	getgenv().ThirdPerson = false -- Locking onto someone in your Third Person POV
	getgenv().FirstPerson = true -- Locking onto someone in your First Person POV
	getgenv().TeamCheck = false -- Check if Target is on your Team (True means it wont lock onto your teamates, false is vice versa) (Set it to false if there are no teams)
	getgenv().PredictMovement = true -- Predicts if they are moving in fast velocity (like jumping) so the aimbot will go a bit faster to match their speed 
	getgenv().PredictionVelocity = 10 -- The speed of the PredictMovement feature 

	loadstring(game:HttpGet("https://raw.githubusercontent.com/DOXSASHW/aimlock/main/aimlock", true))()
end)

local Button2 = Section5:CreateButton("Silent Aim Gui", function()

	repeat task.wait() until game.GameId ~= 0
	if Parvus and Parvus.Loaded then
		Parvus.Utilities.UI:Notification({
			Title = "Parvus Hub",
			Description = "Script already executed!",
			Duration = 5
		})
		return
	end

	getgenv().Parvus = {
		Loaded = false,
		Debug = false,
		Current = "Loader",
		Utilities = {},
		Config = {}
	}

	Parvus.Utilities.UI = Parvus.Debug and loadfile("Parvus/Utilities/UI.lua")() or loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Utilities/UI.lua"))()
	Parvus.Utilities.Config = Parvus.Debug and loadfile("Parvus/Utilities/Config.lua")() or loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Utilities/Config.lua"))()
	Parvus.Utilities.Drawing = Parvus.Debug and loadfile("Parvus/Utilities/Drawing.lua")() or loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Utilities/Drawing.lua"))()

	Parvus.Utilities.SetupFPS = function()
		local LastIteration
		local FrameUpdate = {}
		local Start = os.clock()
		return function()
			LastIteration = os.clock()
			for Index = #FrameUpdate, 1, -1 do
				FrameUpdate[Index + 1] = FrameUpdate[Index] >= LastIteration - 1 and FrameUpdate[Index] or nil
			end
			FrameUpdate[1] = LastIteration
			return os.clock() - Start >= 1 and #FrameUpdate or #FrameUpdate / (os.clock() - Start)
		end
	end

	Parvus.Utilities.NewThreadLoop = function(Wait,Function)
		coroutine.wrap(function()
			while task.wait(Wait) do
				local success, error = pcall(function()
					Function()
				end)
				if not success then
					warn("thread error happend: " .. error)
				end
			end
		end)()
	end

	Parvus.Games = {
		["1054526971"] = {
			Name = "Blackhawk Rescue Mission 5",
			Script = Parvus.Debug and readfile("Parvus/Games/BRM5.lua") or game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Games/BRM5.lua")
		},
		["580765040"] = {
			Name = "RAGDOLL UNIVERSE",
			Script = Parvus.Debug and readfile("Parvus/Games/RU.lua") or game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Games/RU.lua")
		},
		["1168263273"] = {
			Name = "Bad Business",
			Script = Parvus.Debug and readfile("Parvus/Games/BB.lua") or game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Games/BB.lua")
		},
    --[[
    ["807930589"] = {
        Name = "The Wild West",
        Script = readfile("Parvus/Games/TWW.lua")--Parvus.Debug and readfile("Parvus/Games/TWW.lua") or game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Games/TWW.lua")
    },
    ["2194874153"] = {
        Name = "Those Who Remain",
        Script = readfile("Parvus/Games/TWR.lua")--Parvus.Debug and readfile("Parvus/Games/TWR.lua") or game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Games/TWR.lua")
    }]]
	}

	local PlayerService = game:GetService("Players")
	local LocalPlayer = PlayerService.LocalPlayer
	local function IfGameSupported()
		for Id, Info in pairs(Parvus.Games) do
			if tostring(game.GameId) == Id then
				return Info
			end
		end
	end

	LocalPlayer.OnTeleport:Connect(function(State)
		if State == Enum.TeleportState.Started then
			local QueueOnTeleport = (syn and syn.queue_on_teleport) or queue_on_teleport
			QueueOnTeleport(Parvus.Debug and readfile("Parvus/Loader.lua") or game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Loader.lua"))
		end
	end)

	local SupportedGame = IfGameSupported()
	if SupportedGame then
		Parvus.Current = SupportedGame.Name
		loadstring(SupportedGame.Script)()
		Parvus.Utilities.UI:Notification({
			Title = "Parvus Hub",
			Description = Parvus.Current .. " loaded!",
			Duration = 5
		})
		Parvus.Loaded = true
	else
		Parvus.Current = "Universal"
		loadstring(Parvus.Debug and readfile("Parvus/Universal.lua") or game:HttpGetAsync("https://raw.githubusercontent.com/AlexR32/Parvus/main/Universal.lua"))()
		Parvus.Utilities.UI:Notification({
			Title = "Parvus Hub",
			Description = Parvus.Current .. " loaded!",
			Duration = 5
		})
		Parvus.Loaded = true
	end

end)

local Label2 = Section6:CreateLabel("Label 1")
Label2:UpdateText("Misc")
local Toggle2 = Section6:CreateToggle("Wallbang", nil, function(State)
	game:service[[Workspace]]:FindFirstChild('Map'):FindFirstChild('Parts'):FindFirstChild('M_Parts').Parent = game:service[[Workspace]]:FindFirstChild('Characters')
end)

local Label1 = Section7:CreateLabel("Label 1")
Label1:UpdateText("Players")
local Toggle1 = Section7:CreateToggle("Name", nil, function(State)
	ESP.Names = State
end)
local Toggle2 = Section7:CreateToggle("Box", nil, function(State)
	ESP.Boxes = State
end)
local Toggle3 = Section7:CreateToggle("Tracer", nil, function(State)
	ESP.Tracers = State
end)

local Label1 = Section8:CreateLabel("Label 1")
Label1:UpdateText("Items")
local Toggle1 = Section8:CreateToggle("Dealers", nil, function(State)
	if State then
		DEALERESP()
	else
		UNDEALERESP()
	end
end)

function DEALERESP()
	for i,v in pairs(game.Workspace:GetDescendants()) do
		if v.ClassName == 'Model' and v.Parent.Name == 'Dealer' then
			local BillboardGui = Instance.new('BillboardGui') 
			local TextLabel = Instance.new('TextLabel')
			BillboardGui.Name = "DEALERESP"
			BillboardGui.Parent = v.Parent
			BillboardGui.AlwaysOnTop = true 
			BillboardGui.Size = UDim2.new(0, 50, 0, 50)
			BillboardGui.StudsOffset = Vector3.new(0,2,0)

			TextLabel.Parent = BillboardGui
			TextLabel.BackgroundColor3 = Color3.new(1,1,1)
			TextLabel.BackgroundTransparency = 1
			TextLabel.Size = UDim2.new(1, 0, 1, 0)
			TextLabel.Text = v.Parent.Parent.Name
			TextLabel.TextColor3 = Color3.new(1, 0, 0)
			TextLabel.TextScaled = true
		end
	end
end

function UNDEALERESP()
	for i,v in pairs(game.Workspace:GetDescendants()) do
		if v.Name == "DEALERESP" then
			v:Destroy()
		end
	end
end

local Toggle2 = Section8:CreateToggle("Scraps", nil, function(State)
	if State then
		SCRAPESP()
		_G.SCRAPESPACTIVE = true
	else
		UNSCRAPESP()
		_G.SCRAPESPACTIVE = false
	end
end)

function ADDESP(thing)

	local BillboardGui = Instance.new('BillboardGui') 
	local TextLabel = Instance.new('TextLabel')
	BillboardGui.Name = "SCRAPESP"
	BillboardGui.Parent = thing
	BillboardGui.AlwaysOnTop = true 
	BillboardGui.Size = UDim2.new(0, 50, 0, 50)
	BillboardGui.StudsOffset = Vector3.new(0,2,0)

	TextLabel.Parent = BillboardGui
	TextLabel.BackgroundColor3 = Color3.new(1,1,1)
	TextLabel.BackgroundTransparency = 1
	TextLabel.Size = UDim2.new(1, 0, 1, 0)
	TextLabel.Text = "SCRAP"
	TextLabel.TextColor3 = Color3.new(0.341176, 0.450980, 1)
	TextLabel.TextScaled = true
end

function SCRAPESP()
	for i,v in pairs(game:GetService("Workspace").Filter.SpawnedPiles:GetChildren()) do
		ADDESP(v.MeshPart)
	end
end
game:GetService("Workspace").Filter.SpawnedPiles.ChildAdded:Connect(function(c)
	if _G.SCRAPESPACTIVE then
		ADDESP(c.MeshPart)
	end
end)

function UNSCRAPESP()
	for i,v in pairs(game.Workspace:GetDescendants()) do
		if v.Name == "SCRAPESP" then
			v:Destroy()
		end
	end
end

local Toggle1 = Section9:CreateToggle("Anti Recoil", nil, function(State)
	if State == true then
		ToggleBitzFeature("NoRecoil", true)
	end
	if State == false then
		ToggleBitzFeature("NoRecoil", false)
	end
end)

local Toggle2 = Section9:CreateToggle("Anti Spread", nil, function(State)
	if State == true then
		ToggleBitzFeature("NoSpread", true)
	end
	if State == false then
		ToggleBitzFeature("NoSpread", false)
	end
end)

local Toggle3 = Section10:CreateToggle("Anti Kick", nil, function(State)
	--// Remote Hook \\--
	local OldNameCall = nil
	OldNameCall = hookmetamethod(game, "__namecall", function(Self, ...)
		if not checkcaller() and getnamecallmethod() == "FireServer" and Self.Name == "ZFKLF_H" then
			return print("No kick men!")
		end
		if not checkcaller() and getnamecallmethod() == "InvokeServer" and Self.Name == "RCTNMEUN" then
			return print("No kick men!")
		end
		return OldNameCall(Self, ...)
	end)
end)

local Toggle5 = Section10:CreateToggle("Anti Stomp", nil, function(State)
	_G.AntiStomp = State
	local Downed = game:GetService("ReplicatedStorage").CharStats[game:GetService("Players").LocalPlayer.Name].Downed
	Downed.Changed:Connect(function()
		if Downed.Value == true and _G.AntiStomp == true then
			for i, v in pairs(game:GetService("Players").LocalPlayer.Character:GetChildren()) do
				if v:IsA("BasePart") then
					v:Destroy()
				end
			end
		end
	end)
end)

local Toggle = Section10:CreateToggle("Anti Fail Lock", nil, function(State)
	if State then
		_G.LOCKPICKHBE = true
		LOCKHBE()
	else
		_G.LOCKPICKHBE = false
	end
end)

function LOCKHBE()
	task.spawn(function()

		for i,v in next, game.Players.LocalPlayer.PlayerGui:GetChildren() do
			if v.Name == "LockpickGUI" then
				for k,z in next, v:GetDescendants() do
					if z.Name == "Bar" then
						z.Size = UDim2.new(0, 35, 0, 500)
					end
				end
			end
		end

		repeat
			game.Players.LocalPlayer.PlayerGui.ChildAdded:Connect(function(v)
				if _G.LOCKPICKHBE and v.Name == "LockpickGUI" then
					for i,z in next, v:GetDescendants() do
						if z.Name == "Bar" then
							z.Size = UDim2.new(0, 35, 0, 500)
						end
					end
				end
			end)
			game:GetService("RunService").RenderStepped:Wait()
		until not _G.LOCKPICKHBE
		wait(0.04)
		for i,v in next, game.Players.LocalPlayer.PlayerGui:GetChildren() do
			if v.Name == "LockpickGUI" then
				for k,z in next, v:GetDescendants() do
					if z.Name == "Bar" then
						z.Size = UDim2.new(0, 35, 0, 30)
					end
				end
			end
		end
	end)
end

local Toggle1 = Section11:CreateToggle("Full Bright", nil, function(State)
	if State == true then
		game:GetService("Lighting").ExposureCompensation = 1
	end
	if State == false then 
		game:GetService("Lighting").ExposureCompensation = 0
	end
end)

local Colorpicker1 = Section12:CreateColorpicker("OutdoorAmbient Color", function(color)
	_G.Color = color
end)

local Toggle2 = Section12:CreateToggle("Change OutdoorAmbient", nil, function(State)
	if State == true then
		game:GetService("Lighting").OutdoorAmbient = Color3.fromRGB(_G.Color)
	end
	if State == false then 
		game:GetService("Lighting").OutdoorAmbient = Color3.fromRGB(120, 137, 157)
	end
end)

local Label1 = Section1:CreateLabel("Label 1")
Label1:UpdateText("Local Player")
-------------
Section2:CreateLabel("V4 is still in developement.")
Section2:CreateLabel("Suppport my ass")
local Button1 = Section2:CreateButton("Copy Discord", function()
	setclipboard("discord.gg/elitee")
end)
Button1:AddToolTip("Discord Link")

local Button2 = Section2:CreateButton("Copy Website", function()
	setclipboard("elitehub.rocks")
end)
Button2:AddToolTip("Website Link")
-------------

local Slider1 = Section1:CreateSlider("WalkSpeed", 0,33,16,true, function(v)
	_G.WalkSpeed = v
end)

local Slider1 = Section1:CreateSlider("JumpPower", 0,73,50,true, function(v)
	_G.JumpPower = v
end)

local Slider1 = Section1:CreateSlider("FOV", 0,120,120,true, function(v)

	_G.FieldofView = v
	
end)


local Toggle1 = Section1:CreateToggle("Walk speed", nil, function(State)
	if State == true then
		getgenv().WalkSpeedValue = _G.WalkSpeed; --set your desired walkspeed here
		local Player = game:service'Players'.LocalPlayer;
		Player.Character.Humanoid:GetPropertyChangedSignal'WalkSpeed':Connect(function()
			Player.Character.Humanoid.WalkSpeed = getgenv().WalkSpeedValue;
		end)
		Player.Character.Humanoid.WalkSpeed = getgenv().WalkSpeedValue;
	end 
	if State == false then
		getgenv().WalkSpeedValue = 16; --set your desired walkspeed here
		local Player = game:service'Players'.LocalPlayer;
		Player.Character.Humanoid:GetPropertyChangedSignal'WalkSpeed':Connect(function()
			Player.Character.Humanoid.WalkSpeed = getgenv().WalkSpeedValue;
		end)
		Player.Character.Humanoid.WalkSpeed = getgenv().WalkSpeedValue;
	end
end)

Toggle1:AddToolTip("Walk speed")
Toggle1:CreateKeybind("Y", function(Key)
	print(Key)
end)

local Toggle2 = Section1:CreateToggle("Jump Power", nil, function(State)
	if State == true then
		getgenv().JumpPowerValue = _G.JumpPower; --set your desired walkspeed here
		local Player = game:service'Players'.LocalPlayer;
		Player.Character.Humanoid:GetPropertyChangedSignal'WalkSpeed':Connect(function()
			Player.Character.Humanoid.JumpPower = getgenv().JumpPowerValue;
		end)
		Player.Character.Humanoid.JumpPower = getgenv().JumpPowerValue;
	end 
	if State == false then
		getgenv().JumpPowerValue = 50; --set your desired walkspeed here
		local Player = game:service'Players'.LocalPlayer;
		Player.Character.Humanoid:GetPropertyChangedSignal'JumpPower':Connect(function()
			Player.Character.Humanoid.JumpPower = getgenv().JumpPowerValue;
		end)
		Player.Character.Humanoid.JumpPower = getgenv().JumpPowerValue;
	end
end)

Toggle2:AddToolTip("Jump Power")
Toggle2:CreateKeybind("Y", function(Key)
	print(Key)
end)

local Toggle5 = Section1:CreateToggle("Change FOV", nil, function(State)
	
	while game:GetService("RunService").RenderStepped:wait() do

		game.Workspace.Camera.FieldOfView = _G.FieldofView

	end

	
end)

local Toggle3 = Section1:CreateToggle("Inf Jump [F]", nil, function(State)
	_G.infinjump = State

	local Player = game:GetService("Players").LocalPlayer
	local Mouse = Player:GetMouse()
	if _G.infinjump then
		Mouse.KeyDown:connect(function(k)
			if k == "f" then
				Humanoid = game:GetService("Players").LocalPlayer.Character:FindFirstChildOfClass("Humanoid")
				Humanoid:ChangeState("Jumping")
				wait(0.1)
				Humanoid:ChangeState("Seated")
			end
		end)
	end

	local Player = game:GetService("Players").LocalPlayer
	local Mouse = Player:GetMouse()
	Mouse.KeyDown:connect(function(k)
		if k == "f" then
			if _G.infinjump == true then
				_G.infinjump = false
			else
				_G.infinjump = true
			end
		end
	end)      
end)

Toggle3:AddToolTip("Inf Jump")
Toggle3:CreateKeybind("Y", function(Key)
	print(Key)
end)

local Toggle4 = Section1:CreateToggle("Inf Stamina", nil, function(State)
	_G.InfStamina = State
	local StaminaTake = getrenv()._G.S_Take
	local StaminaFunc = getupvalue(StaminaTake, 2)

	for i,v in pairs(getupvalues(StaminaFunc)) do
		if type(v) == "function" and getinfo(v).name == "Upt_S" and _G.InfStamina then
			local oldFunc; 
			oldFunc = hookfunction(v, function(...)
				getupvalue(StaminaFunc, 6).S = 100
				return oldFunc(...)
			end)
		end
	end
end)

Toggle4:AddToolTip("Inf Stamina")
Toggle4:CreateKeybind("Y", function(Key)
	print(Key)
end)

local Toggle1 = Section13:CreateToggle("Noclip bypasser", nil, function(State)
	_G.noclipBypass = State
	local statetype = Enum.HumanoidStateType
	local rnd = Random.new():NextInteger(150, 100000)
	local mt = getrawmetatable(statetype)
	local mt_index = mt.__index
	setreadonly(mt, false)

	mt.__index = newcclosure(function(t, k)
		if not checkcaller() and t == statetype and k == "StrafingNoPhysics" and _G.noclipBypass then
			return rnd
		end

		return mt_index(t, k)
	end)

	setreadonly(mt, true)
end)

local Button4 = Section13:CreateButton("FPS Boost", function()

	workspace:FindFirstChildOfClass('Terrain').WaterWaveSize = 0
	workspace:FindFirstChildOfClass('Terrain').WaterWaveSpeed = 0
	workspace:FindFirstChildOfClass('Terrain').WaterReflectance = 0
	workspace:FindFirstChildOfClass('Terrain').WaterTransparency = 0
	game:GetService("Lighting").GlobalShadows = false
	settings().Rendering.QualityLevel = 1
	for i,v in pairs(game:GetDescendants()) do
		if v:IsA("Part") or v:IsA("UnionOperation") or v:IsA("MeshPart") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then
			v.Material = "Plastic"
			v.Reflectance = 0
		elseif v:IsA("Decal") then
			v.Transparency = 1
		elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
			v.Lifetime = NumberRange.new(0)
		elseif v:IsA("Explosion") then
			v.BlastPressure = 1
			v.BlastRadius = 1
		end
	end
	for i,v in pairs(game:GetService("Lighting"):GetDescendants()) do
		if v:IsA("BlurEffect") or v:IsA("SunRaysEffect") or v:IsA("ColorCorrectionEffect") or v:IsA("BloomEffect") or v:IsA("DepthOfFieldEffect") then
			v.Enabled = false
		end
	end
	workspace.DescendantAdded:Connect(function(child)
		coroutine.wrap(function()
			if child:IsA('ForceField') then
				game:GetService('RunService').Heartbeat:Wait()
				child:Destroy()
			elseif child:IsA('Sparkles') then
				game:GetService('RunService').Heartbeat:Wait()
				child:Destroy()
			elseif child:IsA('Smoke') or child:IsA('Fire') then
				game:GetService('RunService').Heartbeat:Wait()
				child:Destroy()
			end
		end)()
	end)

end)

local Toggle5 = Section1:CreateToggle("Noclip Fly [T]", nil, function(State)
	game.Players.LocalPlayer.DevCameraOcclusionMode = 'Invisicam' --INVISCAM!!!
	local mouse = game.Players.LocalPlayer:GetMouse()
	local torso = game.Players.LocalPlayer.Character.Torso
	local dir = {w = 0, s = 0, a = 0, d = 0}
	local spd = 2 mouse.KeyDown:connect(function(key)
		if key:lower() == "w" then dir.w = 1
		elseif key:lower() == "s" then dir.s = 1
		elseif key:lower() == "a" then dir.a = 1
		elseif key:lower() == "d" then dir.d = 1
		elseif key:lower() == "q" then spd = spd + 1
		elseif key:lower() == "e" then spd = spd - 1
		end end)
	mouse.KeyUp:connect(function(key)
		if key:lower() == "w" then
			dir.w = 0
		elseif key:lower() == "s" then dir.s = 0
		elseif key:lower() == "a" then dir.a = 0
		elseif key:lower() == "d" then dir.d = 0
		end end)


	enabled = false
	mouse.keyDown:connect(function(key)
		if (key) == "t" and enabled == false then
			enabled = true
			repeat wait(1/44)
				game.Players.LocalPlayer.Character.Torso.Anchored = true
				game.Players.LocalPlayer.Character.Humanoid.PlatformStand = true
				torso.CFrame = CFrame.new(torso.Position, game.Workspace.CurrentCamera.CoordinateFrame.p) * CFrame.Angles(0,math.rad(180),0) * CFrame.new((dir.d-dir.a)*spd,0,(dir.s-dir.w)*spd)
			until enabled == false
		elseif enabled == false then
			game.Players.LocalPlayer.Character.Humanoid.PlatformStand = false
			game.Players.LocalPlayer.Character.Torso.Anchored = false
		end
		if (key) == "t" and enabled == true then
			enabled = false
			game.Players.LocalPlayer.Character.Humanoid.PlatformStand = false
			game.Players.LocalPlayer.Character.Torso.Anchored = false
		end
	end)
end)

Toggle5:AddToolTip("[T to toggle]")
Toggle5:CreateKeybind("Y", function(Key)
	print(Key)
end)

local Toggle6 = Section1:CreateToggle("Noclip", nil, function(v) -- thx kayy
	_G.Noclip = v

	local function Noclip()
		if game.Players.LocalPlayer.Character ~= nil and _G.Noclip == true then
			for _, selfChar in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
				if selfChar:IsA("BasePart") and selfChar.CanCollide == true and selfChar.Name then
					selfChar.CanCollide = false
				end
			end
		end
	end

	game:GetService('RunService').Stepped:Connect(Noclip)
end)

Toggle6:AddToolTip("Noclip ez")
Toggle6:CreateKeybind("Y", function(Key)
	print(Key)
end)

local Toggle3 = Section3:CreateToggle("UI Toggle", nil, function(State)
	Window:Toggle(State)
end)

Toggle3:CreateKeybind(tostring(Config.Keybind):gsub("Enum.KeyCode.", ""), function(Key)
	Config.Keybind = Enum.KeyCode[Key]
end)
Toggle3:SetState(true)

local Colorpicker3 = Section3:CreateColorpicker("UI Color", function(Color)
	Window:ChangeColor(Color)
end)
Colorpicker3:UpdateColor(Config.Color)

-- credits to jan for patterns
local Dropdown3 = Section4:CreateDropdown("Image", {"Default","Hearts","Abstract","Hexagon","Circles","Lace With Flowers","Floral","PoliceTyan"}, function(Name)
	if Name == "Default" then
		Window:SetBackground("2151741365")
	elseif Name == "Hearts" then
		Window:SetBackground("6073763717")
	elseif Name == "Abstract" then
		Window:SetBackground("6073743871")
	elseif Name == "Hexagon" then
		Window:SetBackground("6073628839")
	elseif Name == "Circles" then
		Window:SetBackground("6071579801")
	elseif Name == "Lace With Flowers" then
		Window:SetBackground("6071575925")
	elseif Name == "Floral" then
		Window:SetBackground("5553946656")
	elseif Name == "PoliceTyan" then
		Window:SetBackground("6256504923")
	end
end)
Dropdown3:SetOption("Default")

local Colorpicker4 = Section4:CreateColorpicker("Color", function(Color)
	Window:SetBackgroundColor(Color)
end)
Colorpicker4:UpdateColor(Color3.new(1,1,1))

local Slider3 = Section4:CreateSlider("Transparency",0,1,nil,false, function(Value)
	Window:SetBackgroundTransparency(Value)
end)
Slider3:SetValue(0)

local Slider4 = Section4:CreateSlider("Tile Scale",0,1,nil,false, function(Value)
	Window:SetTileScale(Value)
end)
	Slider4:SetValue(0.5)
