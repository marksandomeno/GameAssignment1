                                                    Liam Gallagher, Mark Sandomeno, CPSC 4160


                                                              FLIGHT SIMULATOR


Version: Python Interpreter 3.11
IDE: PyCharm
OS: MacOS






                                                               The Game Document 

Motivation 

We chose to make this game due to our love of flappy bird and desire to learn the simple mechanics of sending obstacles down screen while also having a main character be able to move around the window to avoid them. We thought this would be a simple first project to get our feet wet in pygame and learn basic movement, time, and collision detection mechanics. Reasoning 
We chose to contain most of our code within main since it was simple enough while having a separate class for our plane object (Main character). Our functions follow the MVC architecture and are organized in a diagram listed under the image section: 

Within ‘main.py’  we have multiple major functions:
Start_screen() to set up opening screen before game beings
drawGround() to build our ground border and display it 
create_obstacles() to build red square obstacles to send down screen
move_char() - allow for plane movements
game_over() restart airtime and display game over text when collision is detected

Our game loop handles collision detection and updating the plane frame by frame in accordance to the user input on keyboard. We also check for the [esc] key to be pressed in order to close the game at any time since it plays continuously upon death.


Image 


![image_2d](https://user-images.githubusercontent.com/19656371/222315541-6277a0da-c184-4236-9cec-10bc36e90f6c.png)



Model

Class Plane: The character which the user plays the game with 
initPlane(): function which initializes the character 
drawGround(): function creating the game background
create_obstacle(): function creating an obstacle 


View 

draw(): function which draws the plane once it has been initialized 
start_screen(): creates and displays the start screen initially displayed to the user 


Controller

movePlane(): function which moves the plane upon user command 
game_over(): starts the game score (and thus the game) over once the user collides with an obstacle 
Game Loop



Future Work 

We can enhance our game in many ways, we did not have enough time to add power-up mechanics which is something we wanted to do. In future work we would make certain obstacles appear as power-ups that could slow down incoming obstacles or shrink the size of the plane. We could enhance our engine by abstracting more of our code into classes in order to make the design more robust and versatile for future game design, this would simplify our game loop and make it more readable. This game could be generalized for other games that use down-screen obstacle components and time-mechanisms to track a score. Our functions that create obstacles, setting, and start screen are all things we could use in our next game. 

