Learned:

I learned a lot making this project as I did not have much expirience in javascript at all. I learned how important it is for your global variables to actually have 'let' instead of 'const' on them. I also learned a lot about listeners and how they interact with the rest of my code


Challenges:

My biggest struggle was allowing certain tokens to be played on other tokens in special circumstances. Since my div's have virtually no content in them (because the content would show up on the screen in the cells) I could not include the names of the elements in the text content of the divs for cells. Instead I mangage through ChatGPT to discover the existence of the .getAttribute() method. Using this I was able to pull the name of the jpg I was using out of the div for the cell (since they all changed dynamically) and put it into a variable to check against the current clicked element. All of this code is inside the canPlaceToken method in my script.js file. It was by far the most difficult part of the assignment because the text content is used to check who's turn it is, display of the player, the border, and the winning screen so being able to pull the name of the src of a div was a life changing moment. 


Complexity:

This game is quite complex due to the rules of the game. Not only does this game prevent tokens being placed on top of certain other tokens, this game prevents the tokens being placed on top of one another directly after another oppenent has placed or changed a token. The game requires a large amount of strategy to trick one's opponent into making a mistake. 

Final:

This final version is very similar to the original idea except instead of the original 3x3 grid, the game is now a 5x5 grid in order to prevent a forced tie. 

Although ChatGPT was helpful for explaining the syntax of certain elements in javascript, I found it completely useless for actually coding in the game mostly because of the completity of the tokens.