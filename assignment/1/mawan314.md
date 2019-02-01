Hockey Time Keeper’s Database Design
This document outlines the design for the hockey time keeper’s database program which would allow us to keep track of the players data and allow the time keeper to record, shots, goals and power-play goals for each player on a team. The time keeper will be able to load a list of players, add a new player, list the players' roster information and list the players' stats. The timer keeper will also be able to record a player's shot, a goal with one or two assists, and a power play goal, with one or two assists.
Public Interface
There are three important classes for the program. The first is the Main Public Interface class which encapsulates the Player and provides the functionality of allowing a user to view all the information of the roster, list all the statistical information of the players, add a new player, record a shot, record a goal with up to 2 assists, and record a power play goal with up to 2 assists. The second is the Player List class which encapsulates the Players List which will be designed to keep track of the players List in an Array List. This class will be able to save a list of players to a file, read a file consisting players, have the method to add a player, record a shot, goal, and a power goal with up to 2 assists. The final class is the Player class which is responsible for managing the roster information which includes the name, date of birth, hometown etc., and play information which includes goals, assists, shot etc. 
Each of the three classes are expanded upon in the following sections, beginning with the Player and Player List classes and ending with the Main class which takes advantage of them both.
Player
The player class is will be responsible for storing the roster information and the play information. This class will store information about the roster which will include their name, date of birth, hometown, weight, height, number, and their position. We will assume that the roster information will be stored as a string.  This will also include information about their play including the points they have scored through scoring a goal or assisting one, their power play points including power play goals and assists, shots, and their shooting percentage.  The shooting percentage will be calculated. 

Your Player class will need three constructors:
•	A "roster" constructor, which will take the information needed to provide all of the player's roster information.
•	A "recreation" constructor, which will take all of the player information including roster and play information.
•	A "copy" constructor, which will take another player object and set all of the values in the new player to be the same as the original.
This class will need the following method:
•	playerPoints will keep track of the scores each players scores and assists. It aggregates the scores and assists players have scored. 
•	shootingPercantage calculates the percentage of total scores and assists a player has scored.  
•	powerplayPoints calculates the percentage of powerplay shots and assists, a player has scored.  
•	toString returns player information in a formatted way.

The item class also needs accessors for several values including:
•	getPoints which returns the players points, as an integer.
•	getAssists which returns the players assists, as an integer.
•	getPowerplayShots which returns the players powerplay shots, as an integer.
•	getPowerplayAssists which returns the players powerplay assists, as an integer.
Player Lists
The players lists class encapsulates the list of the players which are wrapped in an ArrayList. This class will keep track of the players and will allow information to be aggregated. The ArrayList would include information about each players name, position, jersey number, date of birth, hometown, height, goals, assists, powerplay goals, powerplay assists, shots. 
