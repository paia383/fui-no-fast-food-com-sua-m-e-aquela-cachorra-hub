

```
-- Script configuration
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/vozoid/ui-lib/main/ui.lua"))()

-- Create window
local Window = Library:CreateWindow("Blox Fruits Hub")

-- Auto Farm section
local FarmTab = Window:CreateTab("Auto Farm")
FarmTab:CreateButton("Activate Auto Farm", function()
    while true do
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Bury")
        wait(0.1)
    end
end)

-- Teleport section
local TeleportTab = Window:CreateTab("Teleport")
TeleportTab:CreateButton("Go to Starting Island", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1047, 17, 1427)
end)

-- Miscellaneous section
local MiscTab = Window:CreateTab("Miscellaneous")
MiscTab:CreateButton("Activate Godmode", function()
    game.Players.LocalPlayer.Character.Humanoid.MaxHealth = math.huge
    game.Players.LocalPlayer.Character.Humanoid.Health = math.huge
end)
```

