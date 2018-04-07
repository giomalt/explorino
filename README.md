# Explorino
Arduino based robot to autonomously explore and map indoor rooms.

## What is Explorino?
  Explorino (**Explor**e + Ardu**ino**) is an open-source autonomous robot for the exploration, mapping and cleaning of indoor rooms. 
  ![First Prototype Explorino](1.0/img/explorino_1.png "First Prototype Explorino")
  
  Inspired by commercial robots on the market (eg. Roomba), we want to make a cheap and versatile robot for mapping and cleaning indoor spaces. We welcome all Arduino and robotics enthusiasts willing to help and partecipate!

### What does Explorino do?
  1. Exploration: Explorino sees its surrounding in-plane area, detect obstacles and free paths. 
  2. Mapping: Explorino memorises the taken path while acquiring the room map, inspired by [Trémaux's](https://en.wikipedia.org/wiki/Maze_solving_algorithm#Tr%C3%A9maux's_algorithm) maze solving algorithm.
  3. Cleaning: Explorino cleans all of the available units on the map.
  
 ### What is Explorino made of?
It is currenlty based on Arduino Uno. To achieve the aforementioned tasks, it uses:
  1. Four sonars to detect obstacles, two servo-motors to move while counting the type and number of taken steps 
  2. One Arduino Uno to control servos and save map into a matrix
  3. A microfiber cloth for cleaning

[Detailed list of Explorino 1.0 components.](1.0/components)

Here some gif of Explorino avoiding obstacles and cleaning:  
![Explorino avoiding obstacles](1.0/img/avoid_obstacle.gif "Explorino exploring")  ![Explorino cleaning](1.0/img/cleaning.gif "Explorino cleaning")

 The current setup has some intrinsic limitations:
 1. Servos rotations and steps get shorter over time as battery runs out
 2. Arduino internal memory is quite small, there is a compromise between the size and accuracy of the acquired map  
 3. The microfiber cloth is not reausable 

 To address these limitations and add new features, we have some ideas for the future.
 
### Some cool ideas for a future Explorino?
  [ ] 3D printed modular case: compatible with interchangable and additional components, such as:
      - microfiber / fan / wet cleaning systems
      - camera module
      - wireless charger
  [ ] 3D printed cleaning system 
  [ ] Wireless charger
  [ ] Wireless (Wifi or Bluetooth) comunication system / larger internal memory
  [ ] Website to check the progression of cleaning / keep the room under suerveillance

[Current limitations and future feature details.](milestones.md)

### Would you like to partecipate?
We are looking for other open-source enthusiasts to contribute to this project! 
In particular, we need to
* design the 3D-printed modular case and cleaning system 
* improve our deterministic algorithm to keep into account servo counter limitation

We welcome anyone who want to contribute with ideas, algorithm/coding, hardware prototypes, moral support or advertising
:smile:

### Where does Explorino come from?
We made the first prototype back in 2016, as a small side-project of an university course. 
As we were curious about autonomous mapping robotics and lazy about cleaning our room floor every day, we decided to create Explorino. We then realised that a robot for mapping and cleaning is lacking in the open-source community, so we made this project open-source. 
We hope to further improve it, by making it modular, thanks to the help of 3D-printing, other than [adding new features](milestones.md).

Thanks for reading,  
Andrea T. and Giorgio M. 


