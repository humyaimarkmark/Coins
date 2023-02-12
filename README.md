-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local UICorner = Instance.new("UICorner")
local TextLabel = Instance.new("TextLabel")
local Frame_2 = Instance.new("Frame")
local UICorner_2 = Instance.new("UICorner")
local Frame_3 = Instance.new("Frame")
local UICorner_3 = Instance.new("UICorner")
local Frame_4 = Instance.new("Frame")
local UICorner_4 = Instance.new("UICorner")
local Frame_5 = Instance.new("Frame")
local UICorner_5 = Instance.new("UICorner")
local TextButton = Instance.new("TextButton")
local UICorner_6 = Instance.new("UICorner")
local TextButton_2 = Instance.new("TextButton")
local UICorner_7 = Instance.new("UICorner")
local TextButton_3 = Instance.new("TextButton")
local UICorner_8 = Instance.new("UICorner")
local TextButton_4 = Instance.new("TextButton")
local UICorner_9 = Instance.new("UICorner")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(125, 125, 125)
Frame.BorderSizePixel = 0
Frame.Position = UDim2.new(0.0180180185, 0, 0.281481475, 0)
Frame.Size = UDim2.new(0, 178, 0, 405)

UICorner.CornerRadius = UDim.new(0, 9)
UICorner.Parent = Frame

TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.BackgroundTransparency = 0.500
TextLabel.Position = UDim2.new(0.061797753, 0, 0.0235294122, 0)
TextLabel.Size = UDim2.new(0, 152, 0, 30)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "   UI     by    ! ohio boy#8691   "
TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true

Frame_2.Parent = ScreenGui
Frame_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame_2.Position = UDim2.new(0.0264264271, 0, 0.345679015, 0)
Frame_2.Size = UDim2.new(0, 149, 0, 51)

UICorner_2.Parent = Frame_2

Frame_3.Parent = ScreenGui
Frame_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame_3.Position = UDim2.new(0.0264264271, 0, 0.437037021, 0)
Frame_3.Size = UDim2.new(0, 149, 0, 51)

UICorner_3.Parent = Frame_3

Frame_4.Parent = ScreenGui
Frame_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame_4.Position = UDim2.new(0.0270270277, 0, 0.528395057, 0)
Frame_4.Size = UDim2.new(0, 149, 0, 51)

UICorner_4.Parent = Frame_4

Frame_5.Parent = ScreenGui
Frame_5.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Frame_5.Position = UDim2.new(0.0270270277, 0, 0.613580227, 0)
Frame_5.Size = UDim2.new(0, 149, 0, 51)

UICorner_5.Parent = Frame_5

TextButton.Parent = ScreenGui
TextButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton.BorderSizePixel = 0
TextButton.Position = UDim2.new(0.0246246252, 0, 0.345679015, 0)
TextButton.Size = UDim2.new(0, 152, 0, 51)
TextButton.Font = Enum.Font.SourceSans
TextButton.Text = "Auto Coins"
TextButton.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton.TextSize = 24.000
TextButton.MouseButton1Down:Connect(function()
	_G.farm1 = true
end)

UICorner_6.Parent = TextButton

TextButton_2.Parent = ScreenGui
TextButton_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton_2.BorderSizePixel = 0
TextButton_2.Position = UDim2.new(0.0246246252, 0, 0.43580249, 0)
TextButton_2.Size = UDim2.new(0, 152, 0, 51)
TextButton_2.Font = Enum.Font.SourceSans
TextButton_2.Text = "Sell"
TextButton_2.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton_2.TextSize = 24.000
TextButton_2.MouseButton1Down:Connect(function()
	_G.Sell = true
end)

UICorner_7.Parent = TextButton_2

TextButton_3.Parent = ScreenGui
TextButton_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton_3.BorderSizePixel = 0
TextButton_3.Position = UDim2.new(0.0258258265, 0, 0.528395057, 0)
TextButton_3.Size = UDim2.new(0, 152, 0, 51)
TextButton_3.Font = Enum.Font.SourceSans
TextButton_3.Text = "TP Rank"
TextButton_3.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton_3.TextSize = 24.000
TextButton_3.MouseButton1Down:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(202.936279296875, 2.958909273147583, -25.764314651489258)
end)

UICorner_8.Parent = TextButton_3

TextButton_4.Parent = ScreenGui
TextButton_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextButton_4.BorderSizePixel = 0
TextButton_4.Position = UDim2.new(0.0258258265, 0, 0.613580227, 0)
TextButton_4.Size = UDim2.new(0, 152, 0, 51)
TextButton_4.Font = Enum.Font.SourceSans
TextButton_4.Text = "TP BPs"
TextButton_4.TextColor3 = Color3.fromRGB(0, 0, 0)
TextButton_4.TextSize = 24.000
TextButton_4.MouseButton1Down:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(181.31968688964844, 2.95926833152771, -30.148021697998047)
end)

UICorner_9.Parent = TextButton_4



spawn(function()
	pcall(function()
		while wait() do
			if _G.farm1 then
				for i,v in pairs(game:GetService("Workspace").Coins["1"]:GetChildren()) do
					v.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
				end
			end
		end
	end)
end)

spawn(function()
	pcall(function()
		while wait() do
			if _G.Sell then
				game:GetService("ReplicatedStorage").Remotes.Sell:FireServer()
			end
		end
	end)
end)
