# Static Website Dice Roller - Pigs Lite Game
## Author: Alanna San Luis
### Class: Software Engineering

### Credits
ChatGPT, W3Schools was used for the HTML, CSS, and JSS coding
Eric Pogue for the MERNA static website template repository.


## Descriptions:
This project is a web-based version of the dice game called Pigs Lite, hosted as an Azure Static Web App.
The Pig Lite application communicates with a separate Node.js server hosted in Microsoft Azure. The static web application asynchronously calls the remote Node.js RESTful APIs to wake up the server and request random dice numbers. All random numbers are generated on the Node.js server rather than in the static web application.

##Server Communication
The static web application uses HTML, CSS, and JavaScript for the game interface and game logic, while the Node.js server provides the RESTful APIs used to generate the dice rolls. This is done by the player pressing the roll dice button which then sends a request to the Node JS server. The server then generates or rolls a random number with the 6-sided dice and that roller dice number the server generates, or rolls is then displayed in the pig lite dice roller static website. 
The static pigs lite website no longer automatically rolls the dice when the user refreshes the page, instead it is via server.
Roll the die to play Pig Lite. If you roll a 1, your turn is over and its player 2 turn. 
If you roll a 2-6, you can keep going! The first player to get to 100 points wins!

## CORS
Application uses CORS to allow communication between the static web application and the Node js server due to different origin. The code demonstration both working communication of request and response between the static website and the node js server. That line of code is not commented. Also, the code demonstrates a CORS failure by implementing a different origin that does not match, resulting the CORS policy blocking the static web application request. This is shown by the user pressing the roll the dice button, however it will not be working because there is no dice number being displayed. Also, the line of code for this CORS failure is commmented out.

## Instructions: 
The players points will continue to total up everytime a player rolls a number from 2-6.
Players can press the Hold button to save the points they have accumulated during their current turn. 
Once the player presse Hold, those points are added to their total or preserved points, andd it becomes the other players turn. 

If the player rolls a 1, their current turn is over and it becomes the other players 2 turn. 
Rolling a 1 does not reset the player preserved or total points. However, any points accumulated during the players
current turn before rolling 1 will be reset to 0.

