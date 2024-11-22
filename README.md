# microproject
This project was developed by me Andrew Ugweches and Joshua Stanley as a project for our Microprocessors module.
The project involved using a microprocessor, the STM32F031, on a breadboard and some given code to create our own game with varying inputs and outputs.
The project was good fun and I believe we managed to make a huge transformation from the original code, a simple template that allowed the character to move on the screen, to our final version HEAVILY inspired by Dance Dance Revolution.

Using the breadboard we were able to attach additional outputs, such as the LEDs and the speaker to provide more feedback to the user to improve 'gamefeel' and more closely emulate the classic title.

The game supports both singleplayer and multiplayer, selected from the main menu.
Once players select the gamemode, they are brought into the main game logic where arrows are spawned at random. Players must correctly time their inputs with the arrow lining up with the top of the screen, receiving feedback on success and failure, score and damage respectively.

Whenever a player successfully hits an arrow, the animated stickman strikes a pose and your score is increased. The speed of following arrows is increased, within limits, again to enhance gamefeel and make the game more engaging.

When an arrow is missed or an input is mistimed, your stickman blunders and loses a heart. Once you have lost all 3 hearts the game prompts the player to swap over to Player 2, if the mode has been selected, or brings the user to the Game Over screen.

On game over, your final score is displayed, and you can choose to return the menu.

As for the code, honestly it's a little messy. The code we were initially provided had it's main gameplay implemented through use of while loops within the main function. As I was coding, I continued to implement my changes within the main function by use of flags and while loops. This worked fine for testing purposes as I would run through the entire game at once to ensure proper functionality. Towards the end however, we realised the functionality could be improved by relegating main gameplay logic to functions which can be called when needed.

Unfortunately, this realization only came towards the end of the deadline, causing the horrible mess of code with many global variables, unnecessary variable overriding, and the remains of the flag and while loop logic. It's not all bad though as I believe that this has strengthened my understanding on the importance of scope, polymorphism, components and code reusability.

Below is a temporary video of the game's functionality, I will hopefully remember to change this video with an improved one, better highlighting the features and fucntionality:
https://youtu.be/i5xD1u-D6Gs?si=W-gAFQ3rtShHjG-O
