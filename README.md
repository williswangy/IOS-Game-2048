# IOS-Game-2048
This is a derivative ios version of the game 2048.
What is 2048 game ??
2048 is played on a gray 4×4 grid, with numbered tiles that slide smoothly when a player moves them using the four arrow keys. Every turn, a new tile will randomly appear in an empty spot on the board with a value of either 2 or 4.Tiles slide as far as possible in the chosen direction until they are stopped by either another tile or the edge of the grid. If two tiles of the same number collide while moving, they will merge into a tile with the total value of the two tiles that collided.The resulting tile cannot merge with another tile again in the same move. Higher-scoring tiles emit a soft glow.
A scoreboard on the upper-right keeps track of the user's score. The user's score starts at zero, and is incremented whenever two tiles combine, by the value of the new tile.As with many arcade games, the user's best score is shown alongside the current score.
The game is won when a tile with a value of 2048 appears on the board, hence the name of the game. After reaching the 2048 tile, players can continue to play (beyond the 2048 tile) to reach higher scores.When the player has no legal moves (there are no empty spaces and no adjacent tiles with the same value), the game ends.
## GAME
Since it is a *derivative* of the original 2048, it is not the *same*. More explicitly, it has the following additions:

* **Three board sizes**: 3x3, 4x4 and 5x5. The smaller the board is, the fewer cells you have, and the harder the game is.* 
* **Three game modes**: The original Power of 2, i.e. combining two tiles of the same value to produce their sum. The Power of 3, i.e. combining *three* consecutive tiles of the same value to produce their sum. Not surprisingly, this is pretty hard with the 3x3 board, although I found it pretty easy to get 81. 243 is a different story... And the Fibonacci sequence, i.e. combining two adjacent numbers in the sequence 2, 3, 5, 8, 13... (I omitted the two 1's in the beginning) to produce the one next to the larger value. This is pretty tricky. Try it out and you will know what I mean.
* **Three themes**: I made a bright theme and a 'joyful' theme in addition to the original one. In case you wonder how to do themes in iOS. (There may be a better way, but themes are verbose in nature, because you *have to* specify all the colors, fonts, etc.)

## The Technology

This version of 2048 is built using SpriteKit, the new 2-D game engine Apple introduced to iOS 7. As a result, it requires iOS 7 to run. On the other hand, this app has the following two great properties:

* It does not rely on *any* third-party library. Not that Cocos-2D is not great, but the fact it's using SpriteKit means that it does not have any dependencies.
* It does not have any images. That's right. The entire UI is done either via UIKit, or by Core Graphics. Check out the related files to see how that is done, if you are curious.


