# PaperZD 2.5D Template free for use!!!

Developed with Unreal Engine 5! I used PaperZD Plugin, mixed it with platformer aspects like what you would see in mario games, and an attack system similar to any hack n' slash games.

## Base Systems:
- Stats Component (able to change each enemy health, defense, damage, etc)
   - Calculate damage:
      - Now it will depend on player attack, and enemy defense (vice versa) on how much damage is dealt! HUGE WIN for me personally!!!

## Attack System:
### Linetrace instead of collision shapes
   - Mainly its due to I dont like have to mess with collision shapes all that much, and I dont think the performance is necessary for a 2D project whereas a project using a third person view (similar to FF7 Remake) would be better for collision shapes.
### Combo system that is expandable with comments
   - Able to use spritesheets
   - all dealt with in the AnimBP
   - system built around a tutorial, but expanded
       - combo built around a tree system, lets say you mash a light attack (L - shortened) then it would play L, L, L, L
       - similar to some hack and slash/button mashing games

## Objects:

You'll notice a folder called objects, I started a paperzd base mainly because I wanted the ease of use for 2D objects, granted it would be easier just to use an actor BP class, I wanted to add functionality like flipbooks, etc. To also point out there is a interface since I started expanding a bit more than I thought, so there is a Damage interface to handle taking/giving damage.

- there is two base classes (one for 3D and 2D)

- 3D: (WIP)
    - can choose between skeletal mesh or static mesh (both have its uses mainly see it good for animation)
    - this is newer than the 2D concept so while same functions apply to both, I want to expand for more animation like said before
 
- 2D:
   - instead of a mesh, you have a paper flipbook to show
   - baseline work like handling damage
   - simple destroys the actor if overlapping

## Enemies:

Has 3 types but going to fix, expand, and add more later on. 
 
- Turret
   - Uses pawn sensing, and spawns an bullet bp object when detected
   - only rotate up/down but the pawn sensing and my code makes it rotate left/right as well, going to fix when I get time xD
 
- Skeleton
   - Typical health/damage enemy
   - no ai behavior to attack the player, but can take damage and die using a sprite flicker
   - FUTURE:
        - simple AI, edge detection
        - See/hurt player

## UI

There is 3 Widget BP that I made, and put some temporary code. 

- Death/Respawn Screen
- Main Menu
- Main player HUD 

## Instructions:

click the blue box where it says code, and download as zip, and extract to unreal projects folder or wherever you keep your projects at

*side note: this was my first time using revision control with github so I dont know how it fully works*

## Images:

![abf860cd49e0a69bb6c294c65a359216](https://github.com/user-attachments/assets/4aee32ab-6400-403e-b8c7-ea4c424974fe)
![4ec5f2fcda94d65d821975539b4086b1](https://github.com/user-attachments/assets/a0eed4ed-6e23-41cb-9a3d-9870bef12766)


##### End/Credits:

I am not a professional, like others out there I use youtube, itch.io, and my own knowledge from school to make games, more recently ive been liking making templates for people to use, completely rework, or change. Hopefully some things I used/made is helpful for everyone out there, and I hope to make more and more updates, and changes in the future.
