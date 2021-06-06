# UE4_MarsMarine
Content from course - https://www.udemy.com/share/101Xs6AEoacllQRnQ=/

![image_1](images/image_1.gif)

## Change Log

* Added `Content\Blueprints\Pawns\BP_Marine.uasset` BP Class (Character Pawn)

* Added `Content\Blueprints\GameMode\BP_MarsMarine_GameMode.uasset` Game Mode

* Added `Content\Characters\Marine\Materials\M_Marine_Inst.uasset` material instance

* Added SpringArm and Camera components to `Content\Characters\Marine\Marine.uasset`

* Added WASD movement

* Added `Content\Characters\Marine\Animations\AnimBP_Marine.uasset` AnimationBlueprint

* Added locomotion state machine to switch between IDLE and RUNNING based on character velocity

* Added `Content\Characters\Marine\Animations\Movement_BlendSpace.uasset` Blend Space

![image_2](images/image_2.png)

* Updated `Content\Characters\Marine\Animations\AnimBP_Marine.uasset` Event Graph

![image_3](images/image_3.png)

* Updated `Content\Characters\Marine\Animations\AnimBP_Marine.uasset` AnimationBlueprint and replaced the Idle and Running States with the BlendSpace

![image_4](images/image_4.png)

* Now the marine movement direction input from WASD drives the animation states

* Added mouse aiming

* Added gamepad aiming

* Added gamepad movement

* Added aim smoothing

* Added input switching

* Organized `Content\Blueprints\Pawns\BP_Marine.uasset` character event graph, functions, and vars.

![image_5](images/image_5.png)

* Added a skeletal mesh component as a child of the `Content\Blueprints\Pawns\BP_Marine.uasset` mesh component and attached to the `WeasponPoint` socket.

![image_6](images/image_6.png)

* Added a Particle System component as a child of Rifle and attached to the `MuzzleFlashSocket` socket for the barrel flash.

![image_7](images/image_7.png)

* Added weapon fire functions to the event graph to handle activating the muzzle flash and weapon sounds when the mouse is clicked or game pad trigger is used.

* The `Start Firing Weapon` function activates the particle system and plays a 2d sound.

![image_8](images/image_8.png)

* The `Stop Firing Weapon` function deactivates the muzzle flash and stops the sound. An end shot sound cue plays to hide the abrupt stopping of the sound.

![image_9](images/image_9.png)

* Added a BP_Marine Player HUD

![image_10](images/image_10.png)

* Added bindings for player kills and player health

![image_11](images/image_11.png)

* Added alien damage and death animation

* Added enemy waves

* Added player respawn

* Added particle impact effects

* Added tracer fire with a Niagra Particle System [video tutorial](https://www.youtube.com/watch?v=KDTVLMEcLjE)
