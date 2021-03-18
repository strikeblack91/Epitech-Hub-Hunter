# Unreal Engine 4

Today we will create a simple hunter game, by using Unreal Engine 4.

# Quick overview of the Engine

## Step. 1 - Create a project

Create a project (game, blank, no starter content)

## Step. 2 - UI

Before creating the game, go have a look at the UI, how it works.

## Step. 3 - Current level

Have a quick look about the objects in the current level.\
The objects are on the top-right corner.

## Step. 4 - Play with the engine

Try to add some objects in the current level, run the game ...

## Step. 5 - Save

Here a small challenge:
- Create a folder named "Level"
- Save your current level in this new folder. Your level should be named "L_Main"

# Introduction to Visual Scripting

## Blueprint ?

[Here](https://docs.unrealengine.com/en-US/ProgrammingAndScripting/Blueprints/GettingStarted/index.html#:~:text=The%20Blueprints%20Visual%20Scripting%20system,or%20objects%20in%20the%20engine.)

## Step. 1 - Level Blueprint

- Find the level blueprint and open it

## Step. 2 - Events

- Print "Wow, this is so cool" when the game play
- Print "I like spam" at every frame

# View

## Step. 1 - Folder

- Create a folder named "Blueprint"

## Step. 2 - Pawn

- Create a blueprint class of type "Pawn", named "BP_Player" and place it in the blueprint folder

## Step. 3 - Camera

- Open the blueprint class
- Add a new component -> Camera

## Step. 4 - GameMode

- Create a GameMode blueprint class called "BP_HunterGameMode",
- Set the BP_Player Pawn class as default in your GameMode
- Set the current GameMode level with your new GameMode
- Save and test it

Good job, you just created the view for the player !

# Gameplay

## Step. 1 - Bird

- Create an Actor blueprint class named "BP_Bird"
- Add a sphere mesh in the class, and set it as the new root (replace the default root scene)
- Make it move on the Y axis ! (First real challenge)

## Step. 2 - PlayerController

- Create a PlayerController blueprint class named "BP_HunterPlayerController"
- Set the variables "Show Mouse Cursor" and "Enable Clicks Events" to true
- In your GameMode, set the PlayerController variable with your new PlayerController class

## Step. 3 - Mechanic

 Now that can see and use the mouse cursor, here another challenge
- When you click on a Bird, the Bird should be killed (destroyed).

# Some improvements

## Step. 1 - Function

- Open your level blueprint
- Create a function named "SpawnBird"
- The function should print "Hello"

## Step. 2 - Timer

- In the level blueprint, create a timer which is going to call the SpawnBird function every  2 seconds

## Step. 3 - Spawn

here, your final challenge
- Spawn birds with a random positions (Z axis)
