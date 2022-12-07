# Practical Exam Part 2

# Questions

#Object Pooling Question
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