# Workshop-1.5-Snake

--Folders--
Snake Game = Finished Game
Resources = Starter Sprites
Scripts = Starter Scripts (with comments)

--Steps--
Create a new Unity Project
	Set the name and make sure you select 2D game

Select camera and change background to black
Change the size of the camera to 20

Drag the Resources and Scripts folder into the project's Assets folder

Select all sprites in the Resources folder 
In the Inspector panel change their Pixels Per Unit to 1

Drag two copies of border_horizontal and border_vertical from Resources into the scene panel

Change the coordinates of the borders to create a box
(0,25,0) (0,-25,0) (-35,0,0) (35,0,0)

Select all the walls and click Add Component
Search for Box Collider 2D and select it to add a collider too all the walls
Check Is Trigger

Drag the food sprite from Resources to the scene
Add a Box Collider 2D to food and set it as a trigger
Go to Tag at the top of the Inspector and select Add Tag
Click the plus button and create a new tag called "Food" (Case sensitive make sure the 'F' is capitalized or the script will not work)
Select the food object again and change the tag to Food

Create a folder called Prefabs and drag the food object from the hierarchy into that folder
Delete the food object from the scene

Select the Main Camera and click Add Component
Search for the "Spawn Food" script and add it to the Camera
Initialize the fields on the script by dragging the proper objects from Assets to the empty boxes on the script property 

CHECKPOINT - If you press play you should see we are randomly spawning food

Drag the snake sprite from Resources to the scene
Rename the snake object in the Hierarchy to "head"
Add a Box Collider 2D to the snake object and change the size to (0.7, 0.7)
Add a Rigidbody 2D to the snake object, set the Body Type to Kinematic and make sure Simulated is checked

Drag the head object from the hierarchy to the Prefabs folder and select the new Prefab
Change the name of the prefab to "tail"
Set the Box Collider as a Trigger

Select the head object again
Add the Snake Script
Drag the tail prefab to the empty field on the script



