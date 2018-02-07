# Udacity VR: 4th project – Puzzler
This is 4th project for Udacity’s VR Nanodegree. This project is to learn and demonstrate how a VR developer to design a mobile game and focusing on the user experience by Puzzler Starter Project. To achieve such goal, having applied user's feedback for UI design frequently based on Lean development methodology.
![screenshut](https://github.com/himax25/Puzzler_VR_project/blob/master/VR_PIC1.png)

## Puzzler: Catching up the sequence pattern of Dungeon Orbs
This is a Puzzler that is a sort of the children’s game Simon Says. The player should figure out the sequence pattern of Dungeon Orbs’ blinking in order to escape from the dungeon.
![youtubelink](https://github.com/himax25/Puzzler_VR_project/blob/master/VR_PIC8.JPG) **(https://youtu.be/PBp2jI9z7b4)** Click the URL to see the recording video.
The player could play the Puzzle game again after exiting the dungeon by pressing Restart button.
 
# Design and Development
## Persona: a typical user
I assume the target audience of this puzzler VR user, as the followings:
* **Hilary Lee**, 11, a Girl, Elementary school student.
* Hilary is very excited to play a mobile game nowadays. 
  Especially she loves to play VR game. However, she sometimes loses focusing on a given topic in her school life. 
  I hope she could enhance her focusing by this Puzzler game training.
   
## Game scenario with UI sketches
I designed the Puzzler game scenario with UI in the following image as a prototype. This Puzzler consists of 3 parts; Starting Zone, Main Playing Dungon Zone, and Exit & Replaying Zone.
![screenshut](https://github.com/himax25/Puzzler_VR_project/blob/master/VR_PIC2.jpg)
I initially had designed the following 2 conceptual UIs for both Starting and Exit Zones. 
![screenshut](https://github.com/himax25/Puzzler_VR_project/blob/master/VR_PIC3.JPG)

## Story of this process  
In order to win this Puzzler, the player needs to figure out the pattern of the sequence with Dungeon Orbs. There are 5 Orbs in Dungeon with building up random order sequence at every time. The player should memorize the sequence when the puzzler shows the sequence initially. Otherwise, the player is unable to escape from the Dungeon. 

# User testing, feedback and changes
## User testing for UI 
I had built up the draft version of UI for both starting module and restarting module according to Conceptual UI 2. And I asked the tester to try on it and got some feedback from her.
* **Feedback:** the font & windows’ color of the following 2 UIs were initially black and white. She told me that it was too dark to read the message and ugly UI for the game. 
* **Enhancing:** I updated the font & windows’ color of these UI as a yellow colored font with a transparent dark light based window instead of.
![screenshut](https://github.com/himax25/Puzzler_VR_project/blob/master/VR_PIC4.JPG)

## User testing for Playing puzzler 
I asked her to look around the inside of the dungeon, play Puzzler, and got some feedback on this puzzler from her.
* **Feedback:** she told me that it is better to have additional instruction message window to follow up, and these 5 Orbs are too small to click on.
* **Enhancing:** I added an instruction message window in the bottom of dungeon and made bigger Orbs to point on easy.
![screenshut](https://github.com/himax25/Puzzler_VR_project/blob/master/VR_PIC5.JPG)

# Breakdown of final piece
## Starting zone
The player gets starting Puzzler by clicking the start button at Starting UI window.
![screenshut](https://github.com/himax25/Puzzler_VR_project/blob/master/VR_PIC6.JPG)
* **Movement:** the player will move into Dungeon by OnRail method movement after clicking Start button.    
* **Lighting:** there are 2 ground touches, built by Particle effect in Unity, in Starting zone.
* **Audio:** there is natural outdoor sound to come out during staying in the zone as background effective sound.

## Dungeon zone
There are 5 Orbs in Dungeon with building up random order sequence at every time. The player finds out the pattern of random Orbs’ sequence to escape from the Dungeon.
![screenshut](https://github.com/himax25/Puzzler_VR_project/blob/master/VR_PIC1.png)
* **Movement:** there is hybrid waypoint movement and OnRail method movement to play in dungeon zone. The player uses Raycasting waypoint method to choose Orbs for the game. And, the player will move into Exit zone after solving the sequence of Orbs in Dungeon by OnRail method movement.    
* **Lighting:** there are 4 touches on each side wall, built by Particle effect in Unity, and 1 directional light on the ceiling in Dungeon.
* **Audio:** there is mystical chanting sound to come out during staying in the Dungeon zone as background effective sound.

## Exit & Replaying zone
There is a Restarting UI window to pop up in order to reload the game with a new play after solving the puzzle from the Dungeon.
![screenshut](https://github.com/himax25/Puzzler_VR_project/blob/master/VR_PIC7.JPG)
* **Movement:** the player will move back into Starting zone by OnRail method movement after clicking Restart button.
* **Audio:** there is natural outdoor sound to come out during staying in the zone as background effective sound.

# Conclusion
My Puzzler VR game is oriented Android Cardboard as VR design perspective. Please be aware of that there is some dependence of Android SDK with a particular version of Unity such as a requirement of supporting **GvrPointerPhysicsRaycaster** with **GvrPointerInputModule** in Unity. 
According to the final user testing, the tester enjoyed the VR puzzler game. However, she told me that it will be more excited Puzzler game if there is a time bomb to add on such Puzzle game.

## **Author of this coding**
* Hyo Lee, linkedin [here](https://www.linkedin.com/in/hyo-max-lee-61241b13/)
* February 7, 2018.
