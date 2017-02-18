Nightmare Vs. Nightmare
-------------------------------------
[Asset Store Link](http://u3d.as/KvG)  
© 2017 Justin Garza

PLEASE LEAVE A REVIEW OR RATE THE PACKAGE IF YOU FIND IT USEFUL!
Enjoy! :)

Contact  
-------------------------------------
Questions, suggestions, help needed?  
Contact me at:  
Email: jgarza9788@gmail.com  
Cell: 1-818-251-0647  
Contact Info: [justingarza.net/contact](http://justingarza.net/contact/)
  
Description/Features
-------------------------------------
This game is ment to be played by two players on the same device. For best results use Tablet.* Unique Mobile Game
* Muliplayer OnScreenControls
* Over 1500 Icons
* ShockWave Screen Effect
* Unity Ads
* Share Button

...Reach out to me to request new features!  
Terms of Use
-------------------------------------
You are free to add this asset to any game you’d like
However:  
please put my name in the credits, or in the special thanks section. :)  
please do not re-distribute.  

Table of Contents 
-------------------------------------
1. Required Imports
2. Scenes
	* StartScene
	* TitleScene
	* Game
	* Info
3. Systems/Effects
	* Audio (Music/Sound)
	* SceneSwitchAnimator
	* Native Sharing
4. Scripts
5. Gifs

  
Required Imports
-------------------------------------
Before this game can work you must import a few Standard Assets.

**CrossPlatformInput**   
this will allow the OnScreenControls to work.

**Effect**  
this will allow the Camera Effects to work.

![Imgur](http://i.imgur.com/lgjMAA7m.png)


Scenes 
-------------------------------------

**StartScene**  
This scene will provide the players information about how the game works.

![Imgur](http://i.imgur.com/1APGbuCm.png)

**TitleScene**  
This scene allows the players to start the game, toggle music/sounds, share the game, or go to the Info scene.

![Imgur](http://i.imgur.com/mkdUTeem.png)

**Game**
This is the actual game.
Note: it has 4 different status (Intro, Play, P1Win, P2Win)

![Imgur](http://i.imgur.com/o5KdCd0m.png)

**Info**
This scene can provide legal info about the game.


Systems/Effects 
-------------------------------------
**Audio (Music/Sound)**  
MusicManager and SoundManager are two Objects that are never destroyed.
They are used to play Music or a Sound without the need for each object to have it's own AudioSource Component, and this allows us to play sounds while the scene is switching. 
Read MusicManager.cs** and SoundManager.cs** for more info.

**SceneSwitchAnimator**  
This GameObject will allow us to have a nice scene animation while changing scenes.

**Native Sharing**  
This is an OpenSourced asset that can be found at...  
https://github.com/ChrisMaire/unity-native-sharing

Scripts 
-------------------------------------
Below is a list of the scripts that make this game work, along with a breif description of what they do.

###~Assets/NightmareVsNightmare/Scripts/###

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

**playerHP.cs**  
this script controls the player's HP.

**playerMovement.cs**  
this script controls player movement

**PlayerPrefsBool.cs**  
Contains methods for storing bools in the PlayerPrefs.
Note: stores 0 and 1 as int, but converts it to a bool on return

**playerShoot.cs**  
this script allows the player to shoot!

**PlaySound.cs**  
This script is used to play a sound

**PoolManager.cs**  
This script manages pools of objects
Spawning and Recycling.

**projectile.cs**  
this script is used to detect projectile collision

**RecycleAfter.cs**  
This script Recycles a projectile (needed so the projectile fades out)

**RecycleAfter.cs**  
This script Recycles an Object after t seconds

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

**TurnOnParticles.cs**  
turns on the lights and Particles on the TitleScene

**VolumeSwitch.cs**  
This Script can be assigned to a toggle to control Music or Sound


Gifs 
-------------------------------------

![Imgur](http://i.imgur.com/CvNAecym.gifv)

![Imgur](http://i.imgur.com/JBWw3zUm.gifv)

![Imgur](http://i.imgur.com/YjKoGDqm.gifv)

![Imgur](http://i.imgur.com/Y37mrVnm.gifv)



























