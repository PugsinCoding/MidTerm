# MidTerm
/* The Great Battleship Challenge

To the right is an image taken from a Battleship game that I a have been working on. It has a few issues and it has many missing components needed to make the game work. 

The first part of the assignment will be to improve the organization of the code through the use of inheritance. The second task (if you choose to accept it) is to make a simple game that is playable. 

Here is a link to the zipped game Download Here is a link to the zipped game. It has all of the images included. You should be able to unzip it and load it with Netbeans. 

Battleship Game

 

Step 1 Understanding The Project
The first thing you should do is unzip the project and make sure you can get it to run. The project should randomly place ships around the ocean. This is simply a 2D array of labels that has pieces of the images placed in them. Of course creating the ships and placing them on the board properly is slightly complicated but fortunately for you that work has been done.

What you will notice is that there are four different ship types with varying pieces. The following table shows this information

Ships
Ship Type	Pieces
Minesweep	2
Frigate	3
Cruiser	4
Battleship	5
The ShipInfo class is used to keep information about each ship. It holds things like the number of pieces, the name of the ship, and the direction the ship should be placed on the ocean.

Step 2 Orgnaization
While the code given works for placing the ships on the board it could really stand to be organized a little better. This is what your task is on the first part of the assignment.

the ShipInfo class has information about all ships but it does nothing for handling the images. It makes sense that there would be a Ship class that holds the general information and specialized ships like minesweep, frigate, battleship, and cruiser are derived from it.

Modify the ShipInfo class so that it is named Ship. Then derive each of the four ship types from Ship. At the very least the derived Ship will hold the images for the ship but you may want to have it hold the images in both directions. You are also going to need a mechanism to return all of the images back. I think it is best to have the class return Labels that hold each of the pieces. This way you are encapsulating the way the ship pieces are created. I will leave it up to you as to how to return a ship but you could return an array of Labels, an ArrayList of Labels just to name a couple.

When you are finished with this step your the program should run the same as it did when it was given to you with the exception that it is now more organized by using inheritance. This means you are going to have to modify the main code for the game to get your new classes to work.

Step 3 A Simple Game
The game is a simple one. To start with you want the ships to be placed around the ocean but you want them hidden. When a player clicks on a Label you should simply replace the image with the image of a hit ship or the image that represents the miss. Your program should keep track of how many misses. When a ship has been sunk you should replace all of the images with the ones that show a sunken ship.

Ship Pieces
Hit	Hit Image
Miss	Miss Image
Sunk	Sunk ImageSunk ImageSunk Image End
Please Note that Sunk is going to be several images based on the size of the ship. 

You should also provide a button to reset the game and one to show all ships on the ocean if the user decides to give up. */
