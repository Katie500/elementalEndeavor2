Compexity 1: 

Preventing tokens from replacing tokens that they shouldn't:

Since the div's have virtually no content in them (because the content would show up on the screen in the cells) I could not include the names of the elements in the text content of the divs for cells. Instead I mangage through ChatGPT to discover the existence of the .getAttribute() method. Using this I was able to pull the name of the jpg I was using out of the div for the cell (since they all changed dynamically) and put it into a variable to check against the current clicked element. All of this code is inside the canPlaceToken method in my script.js file.

Complexity 2:

Changing the player, making the cells dynamic:

The player is actually determed by changing the text content of the div of the cell. The font is 1pt so the 1 or 2 (used for tracking the players 1 or 2) is impossible to see. Since the text content is used to check who's turn it is, display of the player, the border, and the winning screen, it was really important to make sure that the player was tracked within the div. Since it was simple (thanks to ChatGPT explaining to me how textcontent worked) to pull the text content elements out and change them. This was a solution that worked.


Complexity 3:

Preventing a cell that has just been played from playing again immediately after:

I noticed during trialing this game that some users were glitching the game to an infinite loop by clicking the same cell over and over. By preventing this, users are forced to strategies and are less likely to fall into a loop. This was slightly difficult because I had to start tracking the last played cell and then prevent it from being played again. Although initially I was unsure where to check for this, the actual implimentation for it was not as difficult as the first two complexities. The code for this is actually in the canPlaceToken () function and it checks against a global variable to see if the cell was just played. If it wasnt, it returns true and if it was, it returns false. The previously played global is updated after the canPlaceToken is returned as true to prevent false variables. 
