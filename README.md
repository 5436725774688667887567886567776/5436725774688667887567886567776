local Debris = game:GetService("Debris")
local Player = game.Players.TargetName

function forcefield(Target)
   local FF = Instance.new("ForceField")

   FF.Parent = Target.Character
   Debris:AddItem(FF, 9999999999)

   return FF -- in case you want to do something with it
end

forcefield(Player)
