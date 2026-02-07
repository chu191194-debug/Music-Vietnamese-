# Music-Vietnamese-local sound = script.Parent:WaitForChild("Sound")

script.Parent.Touched:Connect(function(hit)
    local humanoid = hit.Parent:FindFirstChild("Humanoid")
    if humanoid then
        if not sound.IsPlaying then
            sound:Play()
        end
    end
end)
