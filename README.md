
local args = {
    [1] = game:GetService("Players").name,
    [2] = "50000"
}

wait(5)
game:GetService("ReplicatedStorage"):FindFirstChild("_CS.Events").GiveMoneyToPlr:FireServer(unpack(args))
  for i,v in pairs(workspace.PlayerVehicles:GetChildren()) do
        game:GetService("ReplicatedStorage")["_CS.Events"].FillUpCar:FireServer(v, 9e9)
    end
    wait(.2)
    game:GetService("TeleportService"):Teleport(game.PlaceId)
    
