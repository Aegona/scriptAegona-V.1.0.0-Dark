local Material = loadstring(game:HttpGet("https://raw.githubusercontent.com/NiceBBMBThai12/NBTScript/main/Gui%20Th%20Edit%20free%2001"))()

local XX =
    Material.Load(
    {
        Title = "AEGONA HUB",
        Style = 1,
        SizeX = 400,
        SizeY = 185,
        Theme = "Light"
    }
)


local Main =
    XX.New(
    {
        Title = "Auto Farm"
    }
)

local Main2 =
    XX.New(
    {
        Title = "-- Teams --"
    }
)

local shop =
    XX.New(
    {
        Title = "-- SHOP --"
    }
)


local D =
    Main.Toggle(
    {
        Text = "-- Auto Farm Box --",
        Callback = function(Value)
            _G.AutoFarm = Value
            while _G.AutoFarm do
                wait(0.1)
    for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
    if v.Name == "TouchInterest" then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = v.Parent.CFrame
        game.Players.LocalPlayer.Character.Humanoid.Health = 0
        wait(.1)
    end
        Enabled = false
end
end
end
    }
)

local blah =
    Main2.Button(
    {
        Text = "Joim Maren",
        Callback = function(Value)

local args = {
    [1] = "SetTeam",
    [2] = "Marines"
}

game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))

        end,
        Enabled = false
    }
)

local blah =
    Main2.Button(
    {
        Text = "Joim Pirates",
        Callback = function(Value)

local args = {
    [1] = "SetTeam",
    [2] = "Pirates"
}

game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))

        end,
        Enabled = false
    }
)

local blah =
    shop.Button(
    {
        Text = "RandomFruit",
        Callback = function(Value)
local args = {
    [1] = "Cousin",
    [2] = "Buy"
}

game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
 print("Random_fruit")
        Enabled = false
        end
        }
        )
        
        
        local blah =
    Main.Button(
    {
        Text = "Rejoin",
        Callback = function(Value)
local ts = game:GetService("TeleportService")
      local p = game:GetService("Players").LocalPlayer
ts:Teleport(game.PlaceId, p)
        end,
        Enabled = false
        }
        )
        
        
        
