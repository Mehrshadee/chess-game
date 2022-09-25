#CHESS GAME (simple edition)









####Description : chess game with c++


First you have to select the horizontal and vertical location of the chessman respectively,


Then you have to select the horizontal and vertical location of the destination respectivel afte a "to".


Example : A3toF7


Then if the chessman of the A3 were not allowed to move to the F7, It would respond an Error.


You have to make sure that it is whites/blackes turn, otherwise you will face to "It is blacks/whites turn!" Error.


simple rules : No Checks! The only condition of wining is to eliminate the King!


+How I wrote it :


First I used the ASCII codes of the charectors to print the bordgame. void print(int board[]) is complitely showing the process.

Then I used to save the name of the chestmen in arrays using only two letters, Which the first one is standing for the first letter of the chestmen's name.



And the second one is standing for the color of the chestman. black or white. Here it is:


string c[64]={


"RB", "AB", "FB", "VB", "KB", "FB", "AB", "RB",


"SB", "SB", "SB", "SB", "SB", "SB", "SB", "SB",


"  ", "  ", "  ", "  ", "  ", "  ", "  ", "  ",


"  ", "  ", "  ", "  ", "  ", "  ", "  ", "  ",


"  ", "  ", "  ", "  ", "  ", "  ", "  ", "  ",


"  ", "  ", "  ", "  ", "  ", "  ", "  ", "  ",


"SW", "SW", "SW", "SW", "SW", "SW", "SW", "SW",


"RW", "AW", "FW", "VW", "KW", "FW", "AW", "RW" };


Then I writed on the correct movement of the chestmen:


S is allowed to walk forward step by step. Soliders are allowed to move two steps in their first move and if they are going to aliminate opponents man, the should move 

ubliquity.


R is able to move horizontaly/verticaly 


A takes the L


F is moving ubliquity


V is a combination of F's and R's movement


K is able to mave a single step ( horizontaly/verticaly)


As they are able to eliminate each other I used to delet the eliminated chestman and replace it with the attacker.


For making this game a bit easier for the players i avoided to write the CHECK rule and decided to make it simple by ending the game shile each teams King be 

eliminated.


I used to delet the privious printings and when ever a movement accures , all of the privious prinitings would be deleted.


As it is considerable the table is updating after any movements and the privious one would be replaced by the new one.


I created a function for all of the movements and rules using BOOLIAN so I just called them in the main whenever it needed.


+How to move the chestmen :


This program first will ask for a 6-letter word and then the first 2 letters of the string is standing for the origin. The last two words are showing the location of 


the destination.


two-middle letters are not important so it is better to type "to" so it would make sense!


the programm will replace to arrays if the destination be space and if not, The destination should be replaced by space and then the chestman would replace it's 


location with the space.


Chestmen are not allowed to friendly-fire! and after each mistake the programm will give you another chance to fix it.
