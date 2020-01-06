# Devastator
Classic TI Game.  Needs to be modernized and remixed

David R. Arnold 
Translated for the H by Patrick Parrish 

'"Devastator'" is an arcade-style game which exphits the sprite features of the TL The screen is given a 3-D effect by careful use of the foreground and background colors. TI Extended BASIC required. 

"Devastator" is written in Extended BASIC and requires a joystick. Your mission in this fast and exciting game is to prevent the Devastator's craft from destroying Earth. 

As the game begins, you find yourself cruising above the ominous Devastator A guardian ship from the Devastator appears. You must eliminate this alien ship and at least nine others that follow in a given period. If you fail the Devastator blasts Earth with a lethal laser 

Two levels of difficulty are offered. On either level you can eliminate the guardian ship by simply positioning your cross hairs over them using the joystick. The main difference between skill levels lies in the size of these guardian ships (which are actually sprites). 

The CALL MAGNIFY statement in line 420 produces ships of two sizes. Consequently, on level one, guardian ships are large and can be easily destroyed, while level two features smaller ships which require greater dexterity to eliminate. 

The Program 

The primary game loop is from lines 450 to 510- The counter W inline 500 is increased each time through the loop. When W reaches 200, the game is over and Earth is either blasted or saved depending on whether you've destroyed the required number of guardian ships. 

If the game, as written, is just too easy or too difficult for you on the skill levels offered, vary the time limit (200) to achieve a level of play suited to your ability. 

The programming techniques used here will be of aid to you in writing your own programs on the TI. You may notice that program execution appears to pause between the title screen and the appearance of the playfield (background). Actually the playfield is being set up, but since the foreground and background 

colors of all characters are defined as black, nothing appears at this point because the screen color is also black. When all characters on the playfield have been printed, color codes are assigned simultaneously using the CALL COLOR statement so that the entire game field appears at once. 

Another trick, also achieved with color coding of characters, gives the game a 3-D effect. The Devastator is first printed in lines 220 to 320 using redefined characters from three character sets. By constantly shifting the foreground and background colors of these character sets in line 450, an illusion of movement is produced. 

Thus, as you watch the screen, you feel as though you were actually circling this colossal ship. 
