# PaperZD 2.5D Template free for use!!!

Developed with Unreal Engine 5! I used PaperZD Plugin, mixed it with platformer aspects like what you would see in mario games, and an attack system similar to any hack n' slash games.

# Attack System:
- Linetrace instead of collision shapes
   - Mainly its due to I dont like have to mess with collision shapes all that much, and I dont think the performance is necessary for a 2D project whereas a project using a third person view (similar to FF7 Remake) would be better for collision shapes.
- Combo system that is expandable with comments
   - Able to use spritesheets
   - all dealt with in the AnimBP
 
# Objects:

You'll notice a folder called objects, I started a paperzd base mainly because I wanted the ease of use for 2D objects, granted it would be easier just to use an actor BP class, I wanted to add functionality like flipbooks, etc. 

- base class
  - paper flipbook
- coins/coin stack similar to mario games
- spike trap like every platformer using multiple paper flipbook's

# Enemies:

Has 3 types but going to fix, expand, and add more later on. 

- Goomba
   - typical should move left/right and detect collisions
   - semi works, but for some reason the collision does not work 100% of the time
 
- Turret
   - Uses pawn sensing, and spawns an bullet bp object when detected
   - supposed to only rotate up/down but the pawn sensing and my code makes it rotate left/right as well, going to fix when I get time xD
 
- Skeleton
   - Typical health/damage enemy
   - no ai behavior to attack the player, but can take damage and die using a sprite flicker


# UI

There is 3 Widget BP that I made, and put some temporary code. 

- Death/Respawn Screen
- Main Menu
- Main player HUD 

# End/Credits:

I am not a professional, like others out there I use youtube, itch.io, and my own knowledge from school to make games, more recently ive been liking making templates for people to use, completely rework, or change. Hopefully some things I used/made is helpful for everyone out there, and I hope to make more and more updates, and changes in the future.
