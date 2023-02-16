# LOH XIN HERNG 20308801
 - Download javafx from https://gluonhq.com/products/javafx/
 - In Intellij, go to File/Project Structure/Project Settings and click on '+'
 - Locate "lib" from the downloaded javafx file 
 - Open the project and run "Main"
   
JavaDoc path: "COMP2042LohXinHerng\JavaDoc\index.html"

Start menu
   - a text box for user to enter name, if the text box is empty, a warning window will prompt
   - a start button
   - a quit button, a confirmation window will prompt
   - a dropdown list for user to choose color

 In game
   - Display the username in game 
   - Fix the score system by only adding the value of addition of number blocks nearby
     e.g. if two number blocks of "4" are nearby, it should add up and become a "8" block. Therefore, 8 is added into            the total score
   - The number blocks will only spawn when the user presses any arrow keys and if there is any movement or addition of          number blocks
      
End game
   - Add a confirmation window after the quit button is clicked 
   - Retry button to play the game again

- Leaderboard screen that save and display the high score of each user
- Returning back to game scene in the same window when user wants to retry
- Changing of background color somehow affects some color of number blocks

Changes made on 
- Controller
- Cell
- EndGame
- GameScene

Unexpected problems:
The number blocks will spawn when any key was pressed although there wasn't any addition or movement of blocks.
This was solved by adding two boolean variables addition and movement. Addition will return "true" when adder is called whereas movement will return "true" when there is any movement of number blocks by comparing the previous board stored in array with the current board 

The score system would just increase when any key was pressed although there wasn't any addition of blocks.
This was solved by replacing des+sign to the y-coordinate in moveHorizontally and x-coordinate in moveVertically

