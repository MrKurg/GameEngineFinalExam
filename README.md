# Practical Exam Part 2

# Have made use of the Object Pooling code from the GED Base project that is the Unity Project used for the Lab.

# Questions

#Object Pooling Question (T to spawn more enemies, up to 6 can be spawned)
Object pooling was implemented by first spawning the specific amount of ghosts based on the size number that is entered in the
object pooler script. When the game is started, they are spawned and deactivated. By pressing the T key, it'll activate one of the ghosts
and spawn it at the specific spawn point I have set in the scene. Up to 6 ghosts can be spawned before it stops. I have put two images in
the folder named ObjectPoolingQuestion that showcase the Unity Profiler before spawning the ghosts and after spawning the ghosts using the
Object Pooling method. As seen in the image of before, there are little spikes in the memory, but they're relatively equally spaced out. 
Whereas in the image of after, the little spikes are more frequent to indicate when an enemy has been spawned before the amount of little
spikes goes back to what it is before spawn.
This implementation optimizes the scene by already having the ghosts loaded and ready to be activated. It saves the computer 
some memory and RAM as it dosen't need to instantiate each object when they need to be spawned, they are already instantiated at the 
beginning and stored in the object pool to be activated for use later. It benefits the game by loading the extra ghosts at the beginning of 
the game, sparing more memory and RAM for other systems and not impacting game performance.

#Command Design Pattern Question (Didn't have time to implement into the Unity Project)
The pattern would have been implemented by having a list where the pellets are stored. Once a pellet has been eaten, the counter for the 
number of pellets in the list will go down by one and the eaten pellet will be removed from the list. By pressing Z for the undo command, 
the eaten pellet will be placed back to its position along with the counter going up by one instead of down. A way it could benefit the 
Pac-Man game is by letting the player undo the pellet hey've eaten if they took the wrong path and have a better one in mind to takae in 
order to more efficiently finish the level.