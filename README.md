Nightmare Vs. Nightmare
-------------------------------------
[Asset Store Link](http://u3d.as/KvG)  
© 2017 Justin Garza

PLEASE LEAVE A REVIEW OR RATE THE PACKAGE IF YOU FIND IT USEFUL!
Enjoy! :)

## Table of Contents

* [Contact](#Contact)
* [Description/Features](#Description-Features)
* [Terms of Use](#Terms-of-Use)
* [Required Imports](#Required-Imports)
* [Inputs](#Inputs)
* [Collision SetUp](#Collision-SetUp)
	* [Add Layers](#Add-Layers)
	* [Assign Layers](#Assign-Layers)
	* [Edit the Collisions](#Edit-the-Collisions)
* [Scenes](#Scenes)
	* [StartScene](#StartScene)
	* [TitleScene](#TitleScene)
	* [Game](#Game)
	* [Info](#Info)
* [Systems/Effects](#Systems/Effects)
	* [Audio (Music/Sound)](#Audio-(Music/Sound))
	* [SceneSwitchAnimator](#SceneSwitchAnimator)
	* [Native Sharing](#Native-Sharing)
* [Scripts](#Scripts)
* [Gifs](#Gifs)


## Contact  

Questions, suggestions, help needed?  
Contact me at:  
Email: jgarza9788@gmail.com  
Cell: 1-818-251-0647  
Contact Info: [justingarza.info/contact](http://justingarza.info/contact/)

## Description Features

This game is ment to be played by two players on the same device. For best results use Tablet.

* Unique Mobile Game
* Muliplayer OnScreenControls
* Over 1500 Icons
* ShockWave Screen Effect
* Unity Ads
* Share Button
* Share Video of GamePlay

...Reach out to me to request new features! 


## Terms of Use

You are free to add this asset to any game you’d like
However:  
please put my name in the credits, or in the special thanks section. :)  
please do not re-distribute.  

## Required Imports

Before this game can work you must import a few Standard Assets.

**CrossPlatformInput**   
this will allow the OnScreenControls to work.

![Imgur](http://i.imgur.com/XECsANnm.png)

**Post Processing Stack**
this allows you to add camera effects

![Imgur](http://i.imgur.com/IEcywl1m.png)

**Unity Ads 2.0**  
Also download Unity Ads 2.0 from the asset store 
(if needed, pending on the unity version this can be imported via the services window)

![Imgur](http://i.imgur.com/iBCCrppm.png)

**EveryPlay**  
Also download EveryPlay from the asset store 

![Imgur](http://i.imgur.com/mFGFqxom.png)

>
After importing these your asset folder should look like this   
![Imgur](http://i.imgur.com/Y2hgLMf.png)

## Inputs
pending on how you downloaded/imported the project files you might need to set up the inputs.

the inputs should look like this.

![Imgur](http://i.imgur.com/FtZOmNg.png)

## Collision SetUp
Depending on how you got this asset you might need to set up the collision rules. below are the instructions on how to do it.

### Add Layers
go to Edit->Project Settings->Tags and Layers  

![Imgur](https://i.imgur.com/wqthINt.png)

create these 4 layers  
![Imgur](https://i.imgur.com/EInzHmE.png)

### Assign Layers
go to the prefab folder and assign the layers to the objects  
![Imgur](https://i.imgur.com/WmuKftj.png)  
![Imgur](https://i.imgur.com/LWaeNk5.png)  
![Imgur](https://i.imgur.com/4Npi3tk.png)  
![Imgur](https://i.imgur.com/nCCkl3V.png)  

### Edit the Collisions
go to Edit->Project Settings->Physics  
![Imgur](https://i.imgur.com/KSptXBQ.png)

Edit the Layer Collision Matrix to match the image (below)  
![Imgur](https://i.imgur.com/zVME6FH.png)

## Scenes 

### StartScene
This scene will provide the players information about how the game works.  

![Imgur](http://i.imgur.com/1APGbuCm.png)

### TitleScene
This scene allows the players to start the game, toggle music/sounds, share the game, or go to the Info scene.  

![Imgur](http://i.imgur.com/mkdUTeem.png)

### Game
This is the actual game.
Note: it has 4 different status (Intro, Play, P1Win, P2Win)  

![Imgur](http://i.imgur.com/o5KdCd0m.png)

### Info
This scene can provide legal info about the game.




## Systems/Effects

### Audio (Music/Sound)
MusicManager and SoundManager are two Objects that are never destroyed.
They are used to play Music or a Sound without the need for each object to have it's own AudioSource Component, and this allows us to play sounds while the scene is switching. 
Read MusicManager.cs** and SoundManager.cs** for more info.

### SceneSwitchAnimator
This GameObject will allow us to have a nice scene animation while changing scenes.

### Native Sharing
This is an OpenSourced asset that can be found at...  
https://github.com/ChrisMaire/unity-native-sharing



## Scripts 

Below is a list of the scripts that make this game work, along with a breif description of what they do.

**~Assets/NightmareVsNightmare/Scripts/**

**AmmoUIManager.cs**  
This script manages the ammo (number of UIBullets) that are seen on the screen

**BothPlayersReady.cs**  
This Script will transition to the Game scene when both players are ready.

**CameraBounds.cs**  
sets bounds to determine what is in the camera's view

**CameraControl.cs**  
Moves the camera to show the winner when the game is over

**DontDestroy.cs**  
This script will allow an object to live on after scene transition.

**EveryPlayButton.cs**
takes the users to everyplay community

**explosionDamage.cs**  
causes damage to the player if it is hit by an explosion particle.

**GameManager.cs**  
This Script controls the state of the game.
Intro, Play, P1Win, P2Win.

**GameUI.cs**  
this script allows the UI to execute methods

**GoToScene.cs**  
This Script can be assigned to buttons to Switch Scenes.

**LightFlash.cs**  
controls the light in the explosion

**loopMe.cs**  
Loops objects to the other side of the screen, requires the camera to have CameraBounds.cs** attached

**MusicManager.cs**  
This script is used to manage the music.

**ObjectPool.cs**  
A pool of objects that can be reused.

**OpenMenu.cs**
used to open and close the menu

**playerHP.cs**  
this script controls the player's HP.

**playerMovement.cs**  
this script controls player movement

**PlayerPrefsBool.cs**  
Contains methods for storing bools in the PlayerPrefs.
Note: stores 0 and 1 as int, but converts it to a bool on return

**playerShoot.cs**  
this script allows the player to shoot!

**PlayRecIcon.cs**
used to set the icon for playing the recorded match.

**PlaySound.cs**  
This script is used to play a sound

**PoolManager.cs**  
This script manages pools of objects
Spawning and Recycling.

**projectile.cs**  
this script is used to detect projectile collision

**RecToggle.cs**  
used to set the RecToggle in the menu if the device is supported, or not.

**RecycleAfter.cs**  
This script Recycles a projectile (needed so the projectile fades out)

**RecycleAfter.cs**  
This script Recycles an Object after t seconds

**RecycleAfter_Projectile.cs**
This script Recycles a projectile (needed so the projectile fades out)

**Rematch.cs**  
used on the Rematch button when the game is over

**SetUp.cs**  
Creates GameObjects on Awake...but don't create them if they exists.

**ShareButton.cs**  
Used to Share this app

**SoundManager.cs**  
This script is used to manage the Sounds.

**StartScene.cs**  
used to go to the TitleScene on tap

**ToggleAnimControl.cs**  
used to control toggles

**ToggleIconSwitch.cs**  
This Script can be assigned to a toggle to control Music or Sound

**TurnOnParticles.cs**  
turns on the lights and Particles on the TitleScene


## Gifs

![Imgur](http://i.imgur.com/JBWw3zUm.gifv)  
[Imgur](http://i.imgur.com/JBWw3zU.gifv)

![Imgur](http://i.imgur.com/YjKoGDqm.gifv)  
[Imgur](http://i.imgur.com/YjKoGDq.gifv)

![Imgur](http://i.imgur.com/Y37mrVnm.gifv)  
[Imgur](http://i.imgur.com/Y37mrVn.gifv)

![Imgur](http://i.imgur.com/CvNAecym.gifv)  
[Imgur](http://i.imgur.com/CvNAecy.gifv)


