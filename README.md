Project Three: Luck Game | Chris + Yeji
----------------------

![alt text](https://github.com/yk1932/LuckGame/blob/main/documentationImages/3.png)


## Description + Inspiration

Test-Your-Luck is a 4 player connected application game where users can play three rounds of chance games to compete which each other to see who is the luckiest out of the group 🍀. The main structure of the game was inspired by Jackbox Games where players enter a room code to access a game from their smartphones or tablets and play a set of mini games. Project three was a continuation of project 2. Please refer to project two's documentation for description,inspiration, process, and design. This will largerly document the changes we made to project 2.

* Link to gitch: [https://fire-shining-magnesium.glitch.me/](https://fire-shining-magnesium.glitch.me/)
* Link to github repository: https://github.com/yk1932/LuckGame

## Improvements

In the previous project, we identified a few aspects that we wanted to work on. Additionally, after some user testing and feedback , we realized that the main aspect that needed work was the UI/UX. There were many components that were unclear and at some times users would lose track of their character. We also decided to introduce avatars for the users to make the game feel a bit more alive. In general, we touched up on how the game looked like and introduced elements such as music and animations to flesh out the game.

![alt text](https://github.com/yk1932/FinalLuckGame/blob/main/documentationImages/Screen%20Shot%202022-05-14%20at%2010.43.01%20PM.png)


1. **Incorporation of Sound / Music**
After playing the game for some time, we felt that the game was extremely flat. The gameplay would get repetitive and there was no real response from the game other than the outcome of your click. We decided that adding sound effects to each click would make each interaction more meaningful and we added a background music for the game.

2.  **Animation**
Similar to the music, we felt that that the response from the game was extremely static and "dead". Thus, we decided to utilize anime.js to create some animations when a user clicked on a door. Currently, we implemented an animation when the user clicks on the chalice. Not only does this make the game look more complete, it also adds a sense of suspense since we have to wait for the animation to finish before we see the result of our choices.

3. **Improved UI/UX**
This was the main focus for project three. Through user testing and feedback, we definitely felt that the game was at some times unclear. Thus, we decided to properly indicate the turns. This was done with introducing a character for each player in the form of a mokoko. Each player is a different colored mokoko. This was indicated in the lobby (where we completely changed the layout) and users would have a star on top of their character. When the game starts, the user's mokoko will be shown on their browser tab. In the game itself, we added two new components: players alive tab and player turn tab. As the name suggests, the players alive tab indicates who is still alive in the game. This is updated whenever a player dies. For the player turn tab, the current player's mokoko will be displayed. Additionally, the background color of the tab will change to red if it is your turn. Depending on whether the player lives or dies after their choice, the player's mokoko will either smile or cry. Lastly, we added a small recap after the game ends to indicate which player has died. We believe that these changes made it easier for players to follow. The mokokos were also quite popular with the users due to their overwhelming cuteness.

![alt text](https://github.com/yk1932/FinalLuckGame/blob/main/documentationImages/Screen%20Shot%202022-05-14%20at%2010.45.02%20PM.png)

![alt text](https://github.com/yk1932/FinalLuckGame/blob/main/documentationImages/Screen%20Shot%202022-05-14%20at%2010.45.37%20PM.png)

![alt text](https://github.com/yk1932/FinalLuckGame/blob/main/documentationImages/Screen%20Shot%202022-05-14%20at%2010.45.55%20PM.png)

4. **New Game**
We also added a new game that had users guessing a number. The last person to correctly guess the number loses. In this game, the user who loses does not die. The reasoning behind is that in the previous iteration, a player could play one game and then do nothing else for the rest of the time. For that particular player, it would not be a pleasant experience as there is not much he/she can do. We thought that adding at least one game would allow for players to at least spend some more time actually engaging with the game itself.

![alt text](https://github.com/yk1932/FinalLuckGame/blob/main/documentationImages/Screen%20Shot%202022-05-14%20at%2010.46.05%20PM.png)


## Coding

Since we were working on our pre-existing code, most of the changes utilized the structure that we had before. To keep track of each character's mokoko, we did have to alter the data sent by the sockets to ensure that the correct images were displayed. Most of the new code was adding the new components in the game, changing the lobby, the new game.

## Learnings

Chris:

The main takeways for project 3 compared to project 2 is the additional need to pay attention to details. I felt that I really needed to care more about the user experience and take care of each interaction to ensure that users go through the intended process when they play our game. I had a lot of fun adding the characters along with integrating it into the game itself. The usage of sockets became much more familiar and I struggled much less here than I did in project 2.

Yeji:

The game logic for the new level was a bit different than the previous levels. Coding the most efficient winning condition was quite challenging and took some time to think through. We ended up using the the sidebar to determine the winning condition. When 3 of the Mokokos were filled in the sidebar, the losing screen was called. The name of the last mokoko, the non-filled slot of the sidebar, was called and the level ended. 

## Next Steps

There are a few things that we would want to add in the future. The first is a clearer indication for the user. Based off the presentation during class, it seemed like players still had some difficulty remembering which character they were or who's turn it was. Perhaps adding the player's mokoko on the side of the screen would help users. We really like the tab idea (mokoko on the tab) but it seems a bit too subtle for users to identify which mokoko they are.

Another aspect we would like to fully flesh out would be the animations. Currently, we only have the chalice animation and we definitely feel like more animations would make the game more fun and interactive.

One thing to consider is what can players who have died do. A way to approach this would be to allow users to display some emoticons after they die or have a cheering button. We think this could be a great addition so that users are not too bored after they die.

Lastly, we believe that this game would flourish with a greater variety of games that are randomly generated each time a user plays. This creates greater unpredictiability and would make the gameplay more interesting, preventing it from getting too stale.
