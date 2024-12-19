# TECH-190-Journal
//Journal on my coding in Tech 190, journey to creating "Trials of The Unik Elements"



/* Week 1: (hours spent: ~5-7)

Had introduction to Tech 190 in class.

Over the weekends, I watched the tutorial on unity provided and thoroughly learned how to use the Unity Engine.
I first took my time to get used to the UI and windows of unity, from the Hierarchy, Inspector, Project, Console, and Scene/Game

- GameObject: is the term used to describe aspects of a game. From the camera used to show what the player could see, props and objects in the game itself, and hidden controllers that does specific things like emit particles.

- Prefab: is basically a "blueprint" of a GameObject or a group of them. This allows you to duplicate the GameObject(s) for ease of use (either to spawn duplicates of them, or use them again without having to worry about repetitive actions/coding)

- Hierarchy: is where you see all of the GameObjects that are present in the game, OR specifically in the frame where you're looking at right now if you have the game running and paused it.

- Inspector: is the window that shows the "properties" of the GameObject selected in the Hierarchy. It shows all the components of the GameObject, that be it the animation, sounds, graphics, properties, or custom scripts.

- Project: is where you could see all your assets, prefabs, and custom scripts.

I coded the flappy bird game side by side with the tutorial and learned how the game is being built.

I finished coding the base game and made some additions not in the tutorial

I submitted the base game together with a short video to show what I did in the process of coding the game

*/



/* Week 2: (hours spent: ~4-5)

thougth of concepts on what my final game will be.

In the time of writing this, I thought of the game being a top down rogue-lite.

Read a couple chapters in Level Up! The Guide to Great Video Game Design

*/



/* Week 3: (hours spent: ~6)

I continued to think of concepts as I started with the "paperwork" of the game.

for now, I wrote down the gameplay and goal pitch, mechanics, levels, and the characters that will be in the game.

Continued reading the Level Up! book.

*/



/* Week 4: (hours spent: ~4)

Prepared a powerpoint to give an idea on what my game is about

the game's genres are rogue-like, action, and top-down.

powerpoint link: https://docs.google.com/presentation/d/1dMOnIY62Waz047nMhHWFrJl-nLOFq2Us2SgAPybdZNY/edit#slide=id.g30743c032b6_0_1

*/



/* week 5: (hours spent: ~8)

started brainstorming the game's content to prepare for the storyboarding phase of the designing the game.
started watching tutorials for specific scripts like procedual generation.

tutorials used:
https://youtu.be/XtQMytORBmM?si=v4SFxjG8Ly-b3F3N

https://youtube.com/playlist?list=PLcRSafycjWFenI87z7uZHFv6cUG2Tzu9v&si=wH5p2_u2ckqO0egk

*/



/* week 6: (hours spent: ~10)

continued on working on procedual generation in creating randomly generated floors in each level

finished doing the corridor random walk generation method

finished doing the Rooms first generation method

created some concept art and wrote 4/10 of the 10-pager for mid terms

*/



/* week 7: (hours spent ~8-10)

continued and finished my 10-pager for the mid terms

continued coding to try and finish the level generation of the game

*/



/* week 8: (hours spent ~15)

continued and finished coding the procedual level generation that produces a simple level with a single room, a level that creates corridors first and then random rooms, and a level that creates rooms first and connects them with corridors.

I started watching a tutorial and coding in creating:
- started polishing assets (coloring and animating)
  
- entities like the playable character and friendly/hostile NPCs.
  - prefabs for them to be able to be spawned.
  - dynamic animations that would change depending on the action done (walking or attacking)
  - coded stats for the player and the enemies to have (HP, Def, Atk, Spd, CD).

- simple skills that deals damage and be a template and base for more complex skills.
- skill collision checker to check if it hit players/enemies/props or walls. Ignoring if it goes through the caster or
  other multiple projectiles casted by the same caster.
- Added variants for Def, Atk, and CD for the respected elements (i.e Flame Attack, Aqua Defense, Earth Cooldown, etc.)

*/



/* week 9+10: (hours spent ~20)

continued working a bit on the assets and animations of enemies and attacks

coded loot drops and chances on the drops (made for trinkets/cards and currency)

Made and coded a fully functional UI that shows your health, GP, and KP (planning to also show full stats somehow around the ui)

coded enemy behavior so that they could only attack when the player is at a certain distance
  - added hidden stats to enemyStats to have Attack Range and Attack Interval

figured how to mark and label rooms made in a level using the dictionary function
  - recorded the position of where the RanWalk started before it created the room

was able to label the boss room (being the farthest room in the level from the player spawn) to be the boss
  - boss is randomly picked from the Game manager, in instantiated and transformed together with the portal to the center of the boss room
  - started planning how to add chest rooms and merchant rooms

FINALY got the gameplay loop premis working (generate level, find boss, kill boss, enter portal, repeat)

created an small algorythim from Co-Pilot that would have the gameObject (enemy) move towards the player

coded a working but some what inefficient mapping for the movement pathing using a rule that has the floor and walls play a role (floors are walkable and walls are unwalkable)

made the algorythim create nodes and anti-nodes based on the tilemaps
  - used Gizmo to visualize the nodes

made the movement be based on the enemyStats EnemySpd

*/ Week 11: (hours spent ~22)
Fixed the issues in PathFindingGrids not generating
now they generate everytime the a new map is generated

did some more work for assets

created a system that checks all rooms that are NOT BossRooms or Safe and populates those with
a fixed number of enemies randomly picked from a list

started creating the inventory system
tutorial used: https://youtube.com/playlist?list=PLcRSafycjWFegXSGBBf4fqIKWkHDw_G8D&si=uW7bUesH9t0MUsHj

/*
Week 12-15: (hours spent ~2 weeks worth)
Finished creating  the inventory system
- fixed and found a solution for equipping, dropping, and consuming items

Added a fully functional HUD that shows the controls, equipped skills, and cooldown timer

Implemented the rest of the enemies, aspects, and level types

made skills more modular for more customizations (same with enemy attacks)

implemeneted the rest of the items, skill cards, and consumables

added a HUD pop up that indicates the item and the GP/KP cost or if it was dropped

added various item drops and their chances to each veteran (level 2), elite (level 3) and aspect (levle 4) enemies.

added a working background music and music swapping feature that changes the music depending on the situation. (still needs to be fixed a bit as it doesn't continue playing another track after the current track finishes)

implemented a simple level generation algorithm that creates a random order of level types (1 element for each 3 levels that changes after every 3rd level)
- made it so that every 6th levels would be a saferoom level where you'd have above average amount of merchants and chests.
/*





