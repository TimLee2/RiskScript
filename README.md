# RiskScript
Generates random territories for each player before the game begins for the 
Risk (Game of Thrones) board game.
- Script for use can be found [here](https://timlee2.github.io/RiskGenerator/RiskScript.html).

## Description
Based on the popular board game Risk, a spin-off 
[Game of Thrones](https://www.usaopoly.com/games/risk-game-of-thrones) version was 
created which is what this script is used for. Instead of having to manually 
draw cards to decide the starting territories for each player, players can use 
this script to quickly randomize all the territories so the game can begin 
sooner. The script generates an equal amount of random territories based on the 
amount of players entered. Three different map options are available to choose 
from.

# Features
- Allows for range of 2-7 Players
- Capability to create custom names for each Player (optional)
- Selection between 3 Map types: 
    - Westeros Only
    - Westeros + Essos
    - Essos Only
- Ability to Reset Page 

# Getting Started
## Prerequisites
- It is assumed the players already have an understanding of how to play the 
game. This script provides no instructions on how to play the board game.
- Most browsers support JavaScript, but the latest version of 
[Chrome](https://www.google.com/chrome/browser/desktop/index.html) is highly
recommended.

# Usage
The layout of the web page is fairly simple, with steps guiding the 
user along the way. The reset button will reload the entire web page, 
undoing everything that has been done.

# Fisher-Yates Shuffle Algorithm
Randomization is a subtle and tough subject. I tried to find a way to randomize 
the territories so that it is **"truly randomized"**: Each player will have 
territories that are minimally clustered on the map. In other words, a player 
beginning with a whole continent will leave other players at a disadvantage. 
I stumbled upon the 
[Fisher-Yates Shuffle Algorithm](https://en.wikipedia.org/wiki/Fisher%E2%80%93Yates_shuffle) 
and the results have been promising with some testing done. Although it is not 
perfect, it does help to perform the shuffling in O(n) time.

# IF TIME PERMITS
- Add die-rolling feature
- Make design more visually appealing
- Map (or visual) to help locate territories on board

# Known Issues (or Improvements)
- Modify the reset button so the whole page doesn't have to reload 
- Notify the players that get a card advantage at start of game due to uneven 
territory distribution based on # of Players

