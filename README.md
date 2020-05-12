model = game.Workspace.Tubes
script.Parent.ClickDetector.MouseClick:connect(function()
script.Parent.ClickDetector:Destroy()
for i=1,646 do
for number, part in pairs (model:GetChildren()) do
if part.Name == "Part" then
part.CFrame = part.CFrame + Vector3.new(0,.2,0)
end
end
wait(0.05)
end
end)
