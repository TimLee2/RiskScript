# RiskScript
Generates random territories for Risk (Game of Thrones).

## Description
Based on the popular board game Risk, a spin-off Game of Thrones version was created which is what this script is used for. Instead of having to manually draw cards to decide the starting territories for each player, players can use this script to quickly randomize all the territories so the game can begin sooner. The script generates an equal amount of random territories based on the amount of players inputted. Two options are available if the players decide to play with Essos or without Essos. 

# Getting Started
## Prerequisites
Most browsers support JavaScript, but the latest version of [Chrome](https://www.google.com/chrome/browser/desktop/index.html) is highly
recommended.

# Usage
The layout of the web page is fairly simple, with instructions guiding the players along the way. The reset button will reload the entire web page, undoing everything that has been done.

# Features
- Allows for range of 2-7 Players
- Custom names for each Player (optional)
- Choose to include or not include Essos in the randomization
- Ability to Reset quickly to modify input errors

# Fisher-Yates Shuffle Algorithm
Randomization is a subtle and tough subject. I tried to find a way to randomize the territories so that it is "truly randomized": Each player will have territories that are minimally clustered on the map. In other words, a player beginning with a whole continent when other players don't will leave them at a disadvantage. I stumbled upon the [Fisher-Yates Shuffle Algorithm](https://en.wikipedia.org/wiki/Fisher%E2%80%93Yates_shuffle) and the results have been promising with some testing done. Although it is not perfect, it does help to perform the shuffling in O(n) time.

# MORE TO COME
- Add die-rolling feature
- Maybe make it look more pretty
- Map (or visual) to help locate territories on board
- An Essos only feature for 2 players

# Known Issues (or Improvements)
- Dynamically display the Players boxes instead of all 7 at once
- Modify some of the resets so the whole page doesn't have to reload 


