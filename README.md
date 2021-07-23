#This is Roblox Code!

script.Parent.MouseButton1Click:Connect(function()
local button = script.Parent
local player = game.Players.LocalPlayer
local clicks = player:WaitForChild("leaderstats"):WaitForChild("Clicks")
local rebirths = player:WaitForChild("leaderstats"):WaitForChild("Rebirths")
	clicks.Value = clicks.Value +2000000000
	if rebirths.Value > 1 then 
		clicks.Value = clicks.Value + rebirths.Value
	end
end)
