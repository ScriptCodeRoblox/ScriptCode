# ScriptCode
I made a fly script for Roblox lol (Only for ur games, dont cheat)

local player = game.Players.LocalPlayer

local flySpeed = 50

local function toggleFlight()

    if player.Character:FindFirstChild("Humanoid") then

        local humanoid = player.Character.Humanoid

        humanoid.PlatformStand = not humanoid.PlatformStand

        humanoid.Sit = not humanoid.Sit

        if humanoid.PlatformStand then

            humanoid.WalkSpeed = flySpeed

            humanoid.JumpPower = flySpeed

        else

            humanoid.WalkSpeed = 16

            humanoid.JumpPower = 50

        end

    end

end

game:GetService("UserInputService").InputBegan:Connect(function(input)

    if input.KeyCode == Enum.KeyCode.F then

        toggleFlight()

    end

end)


To activate flight in your Roblox game using the script, follow these steps:

Open Roblox Studio and open the place or game where you want to enable flight.In the "Explorer" panel, right-click on the "Workspace" folder (or the folder where you want to add the script) and select "Insert Object."Select the object type "Script" and click "OK." A new script will appear in the "Explorer" panel.Double-click the newly created script to open it in the script editor.Copy the script code without the grayed-out text that I provided earlier and paste it into the script editor.Customize the flight speed by adjusting the value of the flySpeed variable according to your preferences. You can experiment with different values to find the one that best suits your game.Click the "Save" button or press Ctrl + S to save the script.Publish your game on Roblox and run it.In the game, when the player presses the designated key (in this case, the "F" key), flight will be toggled on or off, and the player will be able to fly.

Make sure that the player has permissions to execute the script in their local environment.


please dont copy all just script you dum
