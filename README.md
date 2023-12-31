# STARS 2023 Design Final Project

## Guitar Villains
* Jakob Dieffenbach
* Shresth Mathur
* Claire Qiao
* Mike Carranza
* TA: Fahad Aloufi

## Project Description
Based on the popular game Guitar Hero, this game offers a dynamic experience where players can put their rythm and precision to the test. Features such as song editting and difficulty selection enable new players to find their bearings while also allowing more confident players to push their reflexes to their limits. These features challenge players' skills, but also their creativity. Players can also keep track of their progress by comparing their score to the high score stored in their session. 

Two rows of LED's each display their own sequence of beats that scroll from right to left across the rows. Once a beat reaches the left most LED of either row, the player must press the button assigned to that row to score a hit. Naturally, there a total of two buttons: one for each row. Depending of how close to the beat the player presses the buttons, they will be rewarded either 1, 3, or 5 points. If the player hits a button when there are no beats on that row, they will score a miss and their total score will be decremented by 1. 

In addition to the main game, the design includes other features. The player can use a button to change between modes that allow them to select the speed of the beats, freely change the sequence of beats for each row, pause the gmae, or view the the current high score.

## Github Directory Structure 
- [Source Code](https://github.com/STARS-Design-Track-2023/GuitarVillains/tree/main/source)
- [Documents: Includes RTL Diagrams and User Manual](https://github.com/STARS-Design-Track-2023/GuitarVillains/tree/main/docs)


## Pin Layout
- GPIO[3:0] = button[3:0] - Input
- GPIO[10:4] = top_row[6:0] - Output
- GPIO[17:11] = bottom_row[6:0] - Output
- GPIO[24:18] = ss0[6:0] - Output
- GPIO[31:25] = ss1[6:0] - Output
- GPIO[32] = red_disp - Output
- GPIO[33] = green_disp - Output



## Supporting Equipment
![Breadboard Layout](docs/Breadboard.png)
<h3 align="center">Breadboard Setup</h3>

- 1 red LED
- 1 green LED
- 14 x color LED
- 2 seven segment displays

- 16 150 ohm resistors
- 8 1k ohm resistors

- 4 push buttons

- 4 Schmitt-trigger inverters
- 4 0.1 microfarad capacitors


## RTL Diagrams
![Top RTL](docs/Component%20RTL-Top%20RTL.png)
<h3 align="center">Top level RTL</h3>
