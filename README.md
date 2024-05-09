# NASCAT
### Theme:
Do you want to embrace your inner Dale Earnhardt? Jimmie Johnson? But don’t want to compromise your love for cats and all things cat-like? NASCAT combines the best of both worlds with a cat racing game. But beware, some dogs have got on the track and try to avoid them as you cross the finish line.
The game will record your best score (survival time).

### Keys Function:
[U]Start Game/Restart <br/>
[I]To accelerate <br/>
[K]To decelerate <br/>
[J]To go left <br/>
[L]To go right <br/>

### Course Topics Used:  
Transform Matrices <br/>
	We will need to use our knowledge of transformation matrices in order to move the player through track. We also need to perform transformations on camera matrices to show the starting page and the main stage.

Eye Space <br/>
	We will have a camera which will track our player as they traverse the track and dodge     
obstacles [dogs].

Textures <br/>
	Textures will be used extensively on our 2D polygons in order to distinguish the player from the 
track and obstacles. As well as texture scrolling from project 3.


### Advanced Features:  
Collision Detection <br/>
	Collision Detection will play a major role determining whether the player is in a crash state.
	We will check if the player has collided with any obstacles ending their current run.

Interactivity <br/>
The user will start the game with the U key. Once the game starts,the user will be constantly moving forward. Using the J and L keys, the user can go left and right to dodge the obstacles on the race track and achieve the longest survival time possible. The user can also use I and K keys to accelerate and decelerate, which helps with dodging the obstacles coming their way.


### Implementation:  
Collision Detection <br/>
Collision detection was implemented by using the player’s coordinates in relation to the dog enemy’s position. This is done by comparing the left and right most positions of the dog enemy and comparing that to the cat’s position. By checking the z-values of both objects, we can determine whether or not the player is in a death position.

Randomization <br/>
The dog is a single instance of an object, it gets placed along the highway at a random x_pos and respawns all the way in the back once it has left the screen.

Dog Randomization <br/>
The way the dog textures were randomized was by storing 3 dog textures and on spawning the enemy, selecting a random texture to use.

Texture Scrolling<br/>
To give the illusion of movement, we used the texture scrolling from assignment 3 and implemented it into our own project.

### Obstacles Faced:
Time Crunch <br/>
A big limiting factor was the amount of effective time we had to implement the features we promised in the initial proposal. It may have been more effective to stick to one initial idea to allow for greater amount of time.

Sourcing/Creating Assets <br/>
Due to our limited time, creating assets was also a significant time sink which limited how much we could do with our project. Perhaps with more time more assets could have been implemented to make the project more interesting.
Text
Dynamic text was tricky trying to implement into webgl as many bugs would occur especially regarding important animations for the player and dog enemies not moving correctly.

### Next Steps:
Health Implementation <br/>
A definite way to improve on this project would be to implement a life system to increase more interesting situations with the player while also allowing for a greater degree of difficulty. <br/>

Increasing Obstacle Variability <br/>
One of the limitations due to time was the enemy implementation. Currently the enemy has a single instance which respawns at a different x_position. However, perhaps by implementing multiple enemies with different behaviors, the game could be greatly improved. Some ideas may be a side-to-side dog which moves across the road or a dog which tracks the player. <br/>

Reactive Texture Scrolling <br/>
A feature that would be very interesting to implement would be to get the texture scrolling to react to the player’s position. This would’ve been done by fetching the z_pos of the cat and using that to perhaps speed up the texture scrolling rate using a uniform variable.

