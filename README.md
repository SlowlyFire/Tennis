# Tennis   
In this project we implement **Tennis (paper game) in Bash**.  
Tennis is an (abstract) strategic pencil and paper game for two players. The game field consists of 4 fields and a centre line. These are called (-2,-1,0,1,2), with negative numbers belonging to player 1, positive to player 2. At start, the ball is at the centre line (0).  
![image](https://user-images.githubusercontent.com/83518959/192695451-507641ed-d628-4578-bbc4-7afbd2cd93ba.png)  
  
Both players start with the same initial number (e.g. 50 points). In each draw, both players choose a number, and **the ball is moved towards the player with the smallest number**. That integer number is reduced from the total points of the player. **The aim of the game is to move the ball beyond the second field of the opponent.**    

## The ball is moved as follows:    
For a simple description, we include the numbers -3 and 3 to denote the ball being beyond the second field. This results in a playfield as (-3,-2,-1,0,1,2,3).  
If player 1 chooses a bigger number, then:  
- If the ball was on a field of player 1, it will be moved over the centre line to field 1 (player 2 owns the positive fields).   
- Otherwise, the ball will be moved one field towards player 2 (for exaple from filed 1 to field 2, or from field 2 to field 3).  
**Symmetrically, the ball will be moved towards player 1 if player 1 chooses a smaller number**.  

## For the result of the game, the following rules apply, in that specific order:    
- The game ends if the ball is moved beyond the field of any player (3 or -3).  
- else if, one of the players do not have any points left, but the other player does, then the first one loses.  
- otherwise, both players do not have any points left, the game is lost for that player on whose side the ball is.  
* there could be a tie, if the ball is on the centre line (0) and both players do not have any points left.  
  
for more information, click on:  
https://en.wikipedia.org/wiki/Tennis_(paper_game)  

## Examples of the game and different wins:  
![image](https://user-images.githubusercontent.com/83518959/192701091-b767573f-f43e-40bc-bef6-323ae5c71c65.png)
![image](https://user-images.githubusercontent.com/83518959/192701109-54a86697-1ef0-4c05-b405-2ef748b0a372.png)
![image](https://user-images.githubusercontent.com/83518959/192701131-1fa48ffd-f542-47cb-91ad-222ae387c404.png)



