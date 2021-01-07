# Circus Maximus 2020


<div align="center">
<img src="assets/Artwork/Arena.png" alt="Arena" width="100%"/>
</div>

Game by  **Niklaus Houska**, **Alain Hostettler**, **Christian Scherer** and **Maximilian Wolfertz** 

## Table of Contents
* [About](#about)
* [Game Description](#game-description)
* [Installation](#installation-windows)
* [Content](#content)
  * [Fighters](#fighters)
  * [Animals](#animals)
  * [Cheering System](#cheering-system)
  * [Reputation and Upgrades](#reputation-and-upgrades)
  * [Music](sound-effects-and-music)
* [Technical Achievements](#technical-achievements)

## About
This page contains information and executables for the Circus Maximus game released for the [Game Programming Laboratory 2020](https://gtc.inf.ethz.ch/education/game-programming-laboratory/previous-years/2020.html) at ETH Zurich. The game won the Audience Choice Award.

| Information |  |
| ---:         |          :----- |
| Developers | **Niklaus Houska**: Game mechanics, Code, 3D Artwork  <br> **Alain Hostettler**: Code Lead, UI <br> **Christian Scherer**: Code, Sound effects, Controls <br> **Maximilian Wolfertz**: Graphics, 2D Artwork |
| Platforms | Xbox, Windows |
| Release Date | May 26, 2020 |
| Genre | Real-time strategy |
| Player Count | 2 |
| Playtime per Match | 10-30 minutes |
| Development time  | ~3 months    |
| Input | Xbox Controller, (Keyboard for Player 1) |
| Framework | [Monogame](https://www.monogame.net/) |

## Game Description
Circus Maximus is a competitive multiplayer real-time strategy game for 2 players in pseudo-3D. Each player starts by assembling an army consisting of up to 5 groups with fighters of various categories. The goal is to crush the opponent’s army in the following battle. During combat, new fighters, upgrades and animals can be bought with a currency called cheering points, earned by the audience’s approval.

#### Trailer
[![Trailer](https://img.youtube.com/vi/SOApJrn-orY/0.jpg)](https://www.youtube.com/watch?v=SOApJrn-orY)

## Installation (Windows)
  1. Download Release.zip and unpack
  2. Right-click on CMGame_1.0.37.0_x64.cer -> install
  3. Select Local Machine (Requires Admin rights, Current User does not work)
  4. Select "Place all certificates in the following store" and browse to "Trusted Root Certification Authorities"
  5. Finish
  6. Install the game by double-clicking CMGame_1.0.37.0_x64.appxbundle

## Content

### Fighters
<div align="center">
<img src="assets/gifs/units_cheering.gif" alt="Units" width="100%"/>
</div>

The game features 8 unique fighters inspired by historic gladiator classes. Other fighters differ in attack, defense, HP, range, cost, movement and attack speed, as well as in unique capabilities and upgrades. 

#### Formations
<div align="center">
<img src="assets/gifs/murmillo_formation.gif" alt="Murmillo Formation" width="49%"/>
 <img src="assets/gifs/hoplomachus_formation.gif" alt="Hoplomachus Formation" width="49%"/>
</div>
Fighters are organised in groups of which a player can control up to 5 at the same time. Each group can be put in offensive, defensive or retreat stance which influences the fighters default behaviour. Depending on class, the defensive stance buffs defense stats on cost of movement speed. 

#### Let's Introduce our Fighters

<div align="center">
<img src="assets/Artwork/Murmillo.png" alt="Murmillo" width="24%"/>
 <img src="assets/Artwork/Hoplomachus.png" alt="Hoplomachus" width="24%"/>
 <img src="assets/Artwork/Sagittarius.png" alt="Sagittarius" width="24%"/>
 <img src="assets/Artwork/Eques.png" alt="Eques" width="24%"/>
</div>

**Murmillo**: An elite gladiator, that froms a slow but tanky Testudo formation in defensive stance. 

**Hoplomachus**: A spearman with attack bonus against mounted fighters. Forms a tight Phalanx formation in defensive stance that can counter the charge of *Equites*. 

**Sagittarius**: An archer with high attack from distance, but low defense. 

**Eques**: Strong and expensive cavalry that can charge into enemy formations. 


<div align="center">
<img src="assets/Artwork/Veles.png" alt="Veles" width="24%"/>
 <img src="assets/Artwork/Retiarius.png" alt="Retiarius" width="24%"/>
 <img src="assets/Artwork/Provocator.png" alt="Provocator" width="24%"/>
 <img src="assets/Artwork/Bestiarus.png" alt="Bestiarius" width="24%"/>
</div>

**Veles**: A cheap skirmisher that throws spears. Effectively counters the *Sagittarius*. 

**Retiarius**: *Retiarii* have the ability to momentarily incapacitate opponents with their net and ignore armour of entrapped enemies. They excel against elite fighters such as the  *Murmillo*, *Eques* and *Provocator*.  

**Provocator**: Trades attack for suvivability and knows how to get the crowd going. Highest defensive values and gains extra cheering points.

**Bestiarius**: Bestiarii specialize in fighting the animals of the arena, but are weak against other fighters.

### Animals
<div align="center">
<img src="assets/gifs/lion_demo.gif" alt="Lion Demo" width="49%"/>
 <img src="assets/gifs/rhino_demo.gif" alt="Rhno Demo" width="49%"/>
</div>

Lions and Rhinoceros spawn regularly in front of the spectators and unexpectetly through trap doors in the middle of the arena. Animals are strong and should only be engaged with *Bestiarii* and never from range, as such cowardice upsets the crowd. Defeating animals yields high cheering points. 

### Cheering System
<div align="center">
<img src="assets/gifs/cheering.gif" alt="Cheering" width="80%"/>
</div>

Cheering points are the game's currency. They are earned by fighting and killing opponents or animals and by entertaining the crowd by posing at regularly appearing "Cheering Hotspots" in the middle of the arena. Cheering points are exchanged for new fighters.  
Beware, cheering points can be deducted when upsetting the crowd. This happens when your fighters retreat for too long or cowardly attack animals from save distance. 

The crowd loves an underdog! A losing player will benefit from increased cheering gain as a way back into the game should his opponent not capitalize on his advantage. 

### Reputation and Upgrades
Groups can earn up to 3 stars by killing opponents and animals, signifying their reputation in the arena. Each star allows them to get an upgrade at the location at the bottom of the arena. Upgrades are unique to each fighter class and boosts their strength. More details can be found in the ingame encyclopedia. 
<div align="center">
 <img src="assets/gifs/charge.gif" alt="Sprites" width="100%"/>
</div>

### Music
Special thanks to Caesar Otterli for the *Circus Maximus Main Theme*.

## Technical Achievements
<div align="center">
 <img src="assets/Artwork/Sprites.png" alt="Sprites" width="100%"/>
</div>

The game was created using the simple [Monogame](https://www.monogame.net/) framework. Some technical achievements are listed below:
- **Render pipeline**: All models and animations were created in 3D using [Blender](https://www.blender.org/) and transformed into 2D spritesheets used within the game. For example each fighter and animal has at least a unique stand, walk, attack, die and pose animation recorded at 16 orientations and 2 team colors which accounts for several thousand individual sprites. 

- **Depth rendering**: The order of overlapping sprites is calculated pixel-wise. Each sprite thus has an additional depth channel.

- **UI system**: A full-fledged UI system has been implemented to allow the creation of complex menus and controls.

- **Movement and Collision**: Fighters move smoothly and responsive in formation. Collision avoidance and resolving prevents units from stacking. Units do not get stuck because of collision avoidance. Units effectively spread out when engaging opponents. 

- **Pathing**: Units can autonomously navigate around obstacles.
