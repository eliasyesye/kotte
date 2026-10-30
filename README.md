# Bomberman World — [your game title]

**Student:** Elias Alenius Norgren


## How to play

- **Controls:** WASD To move, Place a bomb: SPACE, Restart with "R", Exit game with "Q" or "ESC"
- **Objective and rules:** Defeat 5 enemies to win. Touching an enemy results in a loss. If you kill the final enemy and die at the same time, it results in a loss.
- **Configurations / demo setup:** Default gameplay setup

## Features and validation

| Feature | Check, observed result, and expected behaviour |
| --- | --- |
| 1. Player damage and death | I tested walking into an enemy, letting an enemy walk into the player and being in the blast zone of a bomb. In every case the game transitioned into Game Over screen and worked as expected

| 2. Round states and objective | After completing the objective of defeating 5 enemies the game transitioned into the Win screen. The gameplay stopped as intendend when the lose and win screen was shown. When you lose and win at the same time the code prioritised losing as expected as well

| 3. Safe restart | I tried restarting the game multiple times. The enemies and map got randomized each time, and the number of enemies that had been defeated got reset as well, and explosions and such was not brought into the new map. Everything worked as expected.

| 4. Solid bombs with owner escape | I tested placing a bomb and tried to move the player out of it and back into the bomb. I used print() to check if i managed to place multiple bombs in 1 tile. After placing a bomb i could move away from it and the movement was afterwards blocked by it and i was unable to place multiple bombs in 1 tile, so everything worked as expected |

| 5. Blast-range pickup | I tested placing a bomb before picking up the power up and after picking it up. The blast range was smaller before picking it up and increased after picking up the power up. As expected, the blast range was 3 tiles before the power up and increased to 5 after picking it up 

| [6 Entities and ownership] | I tried placing bombs up to capacity and tried placing more as they exploded. I was always able to place up to 3 bombs which was expected because that was the limit i set

| [7 State and timing] | I tried placing multiple bombs next to each other at different times. The first bomb always triggered the other bomb to explode instantly as well which matched the expected behaviour

| [8 State and timing] | After activating the shield i tried to walk into enemies and after the shield had expired. When walking into an enemy with a shield the player did not take damage, but took damage if i walked into an enemy after the shield had expired. It worked as expected because it successfully avoided damage only when the shield was active 


**Known issues:** After testing all the features multiple times i could not find any issues.

## Sources and assistance

This project builds on the shared Kotte foundations.

I used Copilot when I needed help to get guided in the right direction. I also used it to see if I could improve parts of my code and made it explain how that those changes could be positive for my code. I also used the Algorithms Library to find which functions I could use.



<!-- Submission: commit and push this README with your source to GitHub or the internal Gitea server. Submit the final commit link and a runnable Release ZIP from that version in Studium. Ensure the teacher can access the repository throughout assessment. -->
