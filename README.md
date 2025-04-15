# fui-no-fast-food-com-sua-m-e-aquela-cachorra
-- Basic Script Hub for Blox Fruits
-- Use with compatible executors like KRNL, Synapse X, etc.

-- Load GUI
local Library = loadstring(game:HttpGet("https://pastebin.com/raw/edJT9EGX"))()
local Window = Library:CreateWindow("Blox Fruits Script Hub")

-- Farming Tab
local FarmTab = Window:CreateTab("Auto Farm")
FarmTab:CreateButton("Activate Auto Farm", function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/xQuartyx/DonateMe/main/LoadBF"))()
end)

-- Teleport Tab
local TeleportTab = Window:CreateTab("Teleport")
TeleportTab:CreateButton("Go to Starting Island", function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1047, 17, 1427)
end)

-- Miscellaneous Tab
local MiscTab = Window:CreateTab("Miscellaneous")
MiscTab:CreateButton("Activate Infinite Swords", function()
    -- Add your code here
end)
