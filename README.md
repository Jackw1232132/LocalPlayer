-- Gui to Lua
-- Version: 3.2

-- Instances:

local LocalPlayer = Instance.new("ScreenGui")
local LocalPlayerF = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local Heading = Instance.new("TextLabel")
local UICorner_2 = Instance.new("UICorner")
local Avatar = Instance.new("ImageLabel")
local Title = Instance.new("TextLabel")
local Title_2 = Instance.new("TextLabel")
local Title_3 = Instance.new("TextLabel")
local UserId = Instance.new("TextLabel")
local UserName = Instance.new("TextLabel")
local Title_4 = Instance.new("TextLabel")
local Title_5 = Instance.new("TextLabel")
local Weight = Instance.new("TextLabel")
local Gender = Instance.new("TextLabel")
local Age = Instance.new("TextLabel")
local Title_6 = Instance.new("TextLabel")
local Height = Instance.new("TextLabel")
local Gui1 = Instance.new("Frame")
local UICorner_3 = Instance.new("UICorner")
local Backpack = Instance.new("ScrollingFrame")
local BackpackTemplate = Instance.new("Frame")
local BackpackAvatar = Instance.new("ImageLabel")
local BackpackTitle = Instance.new("TextLabel")
local UIGridLayout = Instance.new("UIGridLayout")
local Friendsin = Instance.new("ScrollingFrame")
local UIGridLayout_2 = Instance.new("UIGridLayout")
local FriendsTemplate = Instance.new("Frame")
local FriendsAvatar = Instance.new("ImageLabel")
local FriendsTitle = Instance.new("TextLabel")
local TextLabel = Instance.new("TextLabel")
local TextLabel_2 = Instance.new("TextLabel")
local Player = game.Players.LocalPlayer
local GenderType = {"Boy", "Girl"}
local ToolAmount = 0
local FriendsAmoutn = 0
local Mouse = Player:GetMouse()
local Can = false

--Properties:

LocalPlayer.Name = "LocalPlayer"
LocalPlayer.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
LocalPlayer.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

LocalPlayerF.Name = "LocalPlayerF"
LocalPlayerF.Parent = LocalPlayer
LocalPlayerF.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
LocalPlayerF.Position = UDim2.new(0.0123253902, 0, 0.625668466, 0)
LocalPlayerF.Size = UDim2.new(0, 631, 0, 335)

UICorner.CornerRadius = UDim.new(0, 15)
UICorner.Parent = LocalPlayerF

Heading.Name = "Heading"
Heading.Parent = LocalPlayerF
Heading.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Heading.Size = UDim2.new(0, 631, 0, 50)
Heading.Font = Enum.Font.FredokaOne
Heading.Text = "LocalPlayer Info"
Heading.TextColor3 = Color3.fromRGB(255, 255, 255)
Heading.TextScaled = true
Heading.TextSize = 14.000
Heading.TextWrapped = true

UICorner_2.CornerRadius = UDim.new(0, 15)
UICorner_2.Parent = Heading

Avatar.Name = "Avatar"
Avatar.Parent = LocalPlayerF
Avatar.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Avatar.Position = UDim2.new(0, 0, 0.149253726, 0)
Avatar.Size = UDim2.new(0, 139, 0, 126)
Avatar.Image = "rbxasset://textures/ui/GuiImagePlaceholder.png"

Title.Name = "Title"
Title.Parent = LocalPlayerF
Title.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Title.Position = UDim2.new(0.220285267, 0, 0.149253726, 0)
Title.Size = UDim2.new(0, 123, 0, 42)
Title.Font = Enum.Font.FredokaOne
Title.Text = "Name:"
Title.TextColor3 = Color3.fromRGB(255, 255, 255)
Title.TextScaled = true
Title.TextSize = 14.000
Title.TextWrapped = true

Title_2.Name = "Title"
Title_2.Parent = LocalPlayerF
Title_2.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Title_2.Position = UDim2.new(0.220285267, 0, 0.274626851, 0)
Title_2.Size = UDim2.new(0, 123, 0, 42)
Title_2.Font = Enum.Font.FredokaOne
Title_2.Text = "UserId:"
Title_2.TextColor3 = Color3.fromRGB(255, 255, 255)
Title_2.TextScaled = true
Title_2.TextSize = 14.000
Title_2.TextWrapped = true

Title_3.Name = "Title"
Title_3.Parent = LocalPlayerF
Title_3.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Title_3.Position = UDim2.new(0.220285267, 0, 0.399999976, 0)
Title_3.Size = UDim2.new(0, 123, 0, 42)
Title_3.Font = Enum.Font.FredokaOne
Title_3.Text = "Age:"
Title_3.TextColor3 = Color3.fromRGB(255, 255, 255)
Title_3.TextScaled = true
Title_3.TextSize = 14.000
Title_3.TextWrapped = true

UserId.Name = "UserId"
UserId.Parent = LocalPlayerF
UserId.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
UserId.Position = UDim2.new(0.415213943, 0, 0.274626851, 0)
UserId.Size = UDim2.new(0, 123, 0, 42)
UserId.Font = Enum.Font.FredokaOne
UserId.Text = "284834234"
UserId.TextColor3 = Color3.fromRGB(85, 255, 0)
UserId.TextScaled = true
UserId.TextSize = 14.000
UserId.TextWrapped = true
UserId.Text = Player.UserId

UserName.Name = "UserName"
UserName.Parent = LocalPlayerF
UserName.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
UserName.Position = UDim2.new(0.415213943, 0, 0.149253726, 0)
UserName.Size = UDim2.new(0, 123, 0, 42)
UserName.Font = Enum.Font.FredokaOne
UserName.Text = "Roblox_Wmh"
UserName.TextColor3 = Color3.fromRGB(85, 255, 0)
UserName.TextScaled = true
UserName.TextSize = 14.000
UserName.TextWrapped = true
UserName.Text = Player.Name

Title_4.Name = "Title"
Title_4.Parent = LocalPlayerF
Title_4.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Title_4.Position = UDim2.new(0.610142648, 0, 0.274626851, 0)
Title_4.Size = UDim2.new(0, 123, 0, 42)
Title_4.Font = Enum.Font.FredokaOne
Title_4.Text = "Weight:"
Title_4.TextColor3 = Color3.fromRGB(255, 255, 255)
Title_4.TextScaled = true
Title_4.TextSize = 14.000
Title_4.TextWrapped = true

Title_5.Name = "Title"
Title_5.Parent = LocalPlayerF
Title_5.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Title_5.Position = UDim2.new(0.610142648, 0, 0.149253726, 0)
Title_5.Size = UDim2.new(0, 123, 0, 42)
Title_5.Font = Enum.Font.FredokaOne
Title_5.Text = "Gender:"
Title_5.TextColor3 = Color3.fromRGB(255, 255, 255)
Title_5.TextScaled = true
Title_5.TextSize = 14.000
Title_5.TextWrapped = true

Weight.Name = "Weight"
Weight.Parent = LocalPlayerF
Weight.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Weight.Position = UDim2.new(0.805071354, 0, 0.274626851, 0)
Weight.Size = UDim2.new(0, 123, 0, 42)
Weight.Font = Enum.Font.FredokaOne
Weight.TextColor3 = Color3.fromRGB(85, 255, 0)
Weight.TextScaled = true
Weight.TextSize = 14.000
Weight.TextWrapped = true
Weight.Text = math.random(30, 90).. "kg"

Gender.Name = "Gender"
Gender.Parent = LocalPlayerF
Gender.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Gender.Position = UDim2.new(0.805071354, 0, 0.149253726, 0)
Gender.Size = UDim2.new(0, 123, 0, 42)
Gender.Font = Enum.Font.FredokaOne
Gender.TextColor3 = Color3.fromRGB(85, 255, 0)
Gender.TextScaled = true
Gender.TextSize = 14.000
Gender.TextWrapped = true
Gender.Text = GenderType[math.random(1, #GenderType)]


Age.Name = "Age"
Age.Parent = LocalPlayerF
Age.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Age.Position = UDim2.new(0.415213943, 0, 0.399999976, 0)
Age.Size = UDim2.new(0, 123, 0, 42)
Age.Font = Enum.Font.FredokaOne
Age.Text = "231"
Age.TextColor3 = Color3.fromRGB(85, 255, 0)
Age.TextScaled = true
Age.TextSize = 14.000
Age.TextWrapped = true
Age.Text = Player.AccountAge

Title_6.Name = "Title"
Title_6.Parent = LocalPlayerF
Title_6.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Title_6.Position = UDim2.new(0.610142648, 0, 0.399999976, 0)
Title_6.Size = UDim2.new(0, 123, 0, 42)
Title_6.Font = Enum.Font.FredokaOne
Title_6.Text = "Height:"
Title_6.TextColor3 = Color3.fromRGB(255, 255, 255)
Title_6.TextScaled = true
Title_6.TextSize = 14.000
Title_6.TextWrapped = true

Height.Name = "Height"
Height.Parent = LocalPlayerF
Height.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
Height.Position = UDim2.new(0.805071354, 0, 0.399999976, 0)
Height.Size = UDim2.new(0, 123, 0, 42)
Height.Font = Enum.Font.FredokaOne
Height.TextColor3 = Color3.fromRGB(85, 255, 0)
Height.TextScaled = true
Height.TextSize = 14.000
Height.TextWrapped = true
Height.Text = math.random(100, 180).. "cm"

Gui1.Name = "Gui1"
Gui1.Parent = LocalPlayerF
Gui1.BackgroundColor3 = Color3.fromRGB(68, 68, 68)
Gui1.BackgroundTransparency = 0.300
Gui1.Position = UDim2.new(0, 0, 0.525373161, 0)
Gui1.Size = UDim2.new(0, 631, 0, 159)

UICorner_3.CornerRadius = UDim.new(0, 15)
UICorner_3.Parent = Gui1

Backpack.Name = "Backpack"
Backpack.Parent = Gui1
Backpack.Active = true
Backpack.BackgroundColor3 = Color3.fromRGB(129, 129, 129)
Backpack.BorderColor3 = Color3.fromRGB(85, 255, 255)
Backpack.BorderSizePixel = 3
Backpack.Position = UDim2.new(0, 0, 0.207547173, 0)
Backpack.Size = UDim2.new(0, 315, 0, 126)

BackpackTemplate.Name = "BackpackTemplate"
BackpackTemplate.Parent = Backpack
BackpackTemplate.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
BackpackTemplate.BorderSizePixel = 2
BackpackTemplate.Position = UDim2.new(0.00480680913, 0, -0.0018533374, 0)
BackpackTemplate.Size = UDim2.new(0, 75, 0, 60)
BackpackTemplate.Visible = false

BackpackAvatar.Name = "BackpackAvatar"
BackpackAvatar.Parent = BackpackTemplate
BackpackAvatar.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
BackpackAvatar.BorderSizePixel = 2
BackpackAvatar.Position = UDim2.new(-0.0133333337, 0, -0.0333333351, 0)
BackpackAvatar.Size = UDim2.new(0, 74, 0, 41)
BackpackAvatar.Image = "rbxasset://textures/ui/GuiImagePlaceholder.png"

BackpackTitle.Name = "BackpackTitle"
BackpackTitle.Parent = BackpackTemplate
BackpackTitle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
BackpackTitle.BackgroundTransparency = 1.000
BackpackTitle.Position = UDim2.new(0.0392706804, 0, 0.668219984, 0)
BackpackTitle.Size = UDim2.new(0, 71, 0, 20)
BackpackTitle.Font = Enum.Font.SourceSansBold
BackpackTitle.Text = "Roblox_Wmh"
BackpackTitle.TextColor3 = Color3.fromRGB(255, 170, 127)
BackpackTitle.TextScaled = true
BackpackTitle.TextSize = 14.000
BackpackTitle.TextWrapped = true

UIGridLayout.Parent = Backpack
UIGridLayout.SortOrder = Enum.SortOrder.LayoutOrder
UIGridLayout.CellPadding = UDim2.new(0, 0, 0, 0)
UIGridLayout.CellSize = UDim2.new(0, 75, 0, 60)

Friendsin.Name = "Friendsin"
Friendsin.Parent = Gui1
Friendsin.Active = true
Friendsin.BackgroundColor3 = Color3.fromRGB(129, 129, 129)
Friendsin.BorderColor3 = Color3.fromRGB(85, 255, 255)
Friendsin.BorderSizePixel = 3
Friendsin.Position = UDim2.new(0.500792384, 0, 0.207547173, 0)
Friendsin.Size = UDim2.new(0, 315, 0, 126)

UIGridLayout_2.Parent = Friendsin
UIGridLayout_2.SortOrder = Enum.SortOrder.LayoutOrder
UIGridLayout_2.CellPadding = UDim2.new(0, 0, 0, 0)
UIGridLayout_2.CellSize = UDim2.new(0, 75, 0, 60)

FriendsTemplate.Name = "FriendsTemplate"
FriendsTemplate.Parent = Friendsin
FriendsTemplate.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
FriendsTemplate.BorderSizePixel = 2
FriendsTemplate.Position = UDim2.new(0.00480680913, 0, -0.0018533374, 0)
FriendsTemplate.Size = UDim2.new(0, 75, 0, 60)
FriendsTemplate.Visible = false

FriendsAvatar.Name = "FriendsAvatar"
FriendsAvatar.Parent = FriendsTemplate
FriendsAvatar.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
FriendsAvatar.BorderSizePixel = 2
FriendsAvatar.Position = UDim2.new(-0.0133333337, 0, -0.0333333351, 0)
FriendsAvatar.Size = UDim2.new(0, 74, 0, 41)
FriendsAvatar.Image = "rbxasset://textures/ui/GuiImagePlaceholder.png"

FriendsTitle.Name = "Friends Title"
FriendsTitle.Parent = FriendsTemplate
FriendsTitle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
FriendsTitle.BackgroundTransparency = 1.000
FriendsTitle.Position = UDim2.new(0.0392706804, 0, 0.668219984, 0)
FriendsTitle.Size = UDim2.new(0, 71, 0, 20)
FriendsTitle.Font = Enum.Font.SourceSansBold
FriendsTitle.Text = "Roblox_Wmh"
FriendsTitle.TextColor3 = Color3.fromRGB(255, 170, 127)
FriendsTitle.TextScaled = true
FriendsTitle.TextSize = 14.000
FriendsTitle.TextWrapped = true

TextLabel.Parent = Gui1
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.Size = UDim2.new(0, 315, 0, 33)
TextLabel.Font = Enum.Font.FredokaOne
TextLabel.Text = "Backpack"
TextLabel.TextColor3 = Color3.fromRGB(170, 255, 255)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true

TextLabel_2.Parent = Gui1
TextLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_2.BackgroundTransparency = 1.000
TextLabel_2.Position = UDim2.new(0.500792384, 0, 0, 0)
TextLabel_2.Size = UDim2.new(0, 315, 0, 33)
TextLabel_2.Font = Enum.Font.FredokaOne
TextLabel_2.Text = "Friends in this server"
TextLabel_2.TextColor3 = Color3.fromRGB(170, 255, 255)
TextLabel_2.TextScaled = true
TextLabel_2.TextSize = 14.000
TextLabel_2.TextWrapped = true
Avatar.BackgroundTransparency = 1.000
BackpackAvatar.BackgroundTransparency = 1.000
FriendsAvatar.BackgroundTransparency = 1.000
BackpackTemplate.BackgroundTransparency = 0.5
FriendsTemplate.BackgroundTransparency = 0.5

function  Clear ()
	for i,Backpack in pairs(Backpack:GetChildren()) do
		if Backpack:IsA("Frame") then
			Backpack:Destroy()
		end
	end
end

function  Fill()
	Clear()
	for i,Tool in pairs(Player.Backpack:GetChildren()) do
		local BackpackT = BackpackTemplate:Clone()
		local BackpckA = BackpackAvatar:Clone()
		local BackTitle = BackpackTitle:Clone()
		BackpackT.Parent = Backpack
		BackpackT.Visible = true
		BackpackT.Active = true
		BackpckA.Parent = BackpackT
		BackpckA.Image = Tool.TextureId
		BackTitle.Parent = BackpackT
		BackTitle.Text = Tool.Name
		ToolAmount +=1
	end
end

Fill()

while wait(0.2) do
	Fill()
	TextLabel.Text = "Backpack (" .. ToolAmount .. ")"
	ToolAmount = 0
end

function  FriendClear()
	for i,Players1 in pairs(Friendsin:GetChildren()) do
		if Players1:IsA("Frame") then
			Players1:Destroy()
		end
	end
end

function  FriendFill ()
	FriendClear()
	for i,Plr in pairs(game.Players:GetChildren()) do
		if Plr:IsFriendsWith(Player.UserId) then
			local PlayerFrame = FriendsTemplate:Clone()
			local PlayerAvatar = FriendsAvatar:Clone()
			local FriendsTitle = FriendsTitle:Clone()
			PlayerFrame.Parent = Friendsin
			PlayerFrame.Visible = true
			PlayerFrame.Active = true
			PlayerAvatar.Parent = PlayerFrame
			PlayerAvatar.Image = game.Players:GetUserThumbnailAsync(Plr.UserId, Enum.ThumbnailType.AvatarThumbnail, Enum.ThumbnailSize.Size420x420)
			FriendsTitle.Parent = PlayerFrame
			FriendsTitle.Name = Plr.Name
			FriendsAmoutn +=1
		end
	end
end

FriendFill()

while wait(0.2) do
	FriendFill()
	TextLabel_2.Text = "Friends in this server (" .. FriendsAmoutn .. ")"
	FriendsAmoutn = 0
end

Mouse.KeyDown:Connect(function(key)
	if key.KeyCode == Enum.KeyCode.G then
		if Can == false then
			Can = true
			LocalPlayer.Enabled = false
		else
			if Can == true then
				Can = false
				LocalPlayer.Enabled = true
			end
		end
	end
end)
