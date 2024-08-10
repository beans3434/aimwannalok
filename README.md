local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "Beany's_Scripts", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})


   --aimlock tap

   local AIMTab = Window:MakeTab({
    Name = "AIM",
    Icon = "rbxassetid://4483345998",
    PremiumOnly = false
   })

   local Section = AIMTab:AddSection({
    Name = "Other"
   })


   AIMTab:AddButton({
    Name = "aimlock",
    Callback = function()
        local Aimbot = loadstring(game:HttpGet("https://raw.githubusercontent.com/Exunys/Aimbot-V3/main/src/Aimbot.lua"))()
        Aimbot.Load()
      end    
   })

   OrionLib:Init()
