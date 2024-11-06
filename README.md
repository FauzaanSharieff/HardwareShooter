Welcome to Hardware Shooter, a shooting game played and observed solely through hardware (although the score is displayed on a screen). 
Aim your gun and shoot the targets before the time runs out - using only Arduino components!

PS: The project code sucks because this was my first actual project, and looking back a year later, I am flabbergasted by the incohorent
mess that I once called a masterpiece. But I still loved making the project. 






How to play the game:
There are five LED lights that act as potential targets. An LED light will randomly light up one at a 
me. The LED light which is lit up is the target that the player has to bring down. Once an LED light is 
brought down, another random LED light replaces it by lighting up. This goes on until the time runs 
out. 
The servo motor acts as the “Gun”. It is aimed, or controlled, using a potentiometer. To “Shoot” the 
gun, a push-button switch is used. Once the Servo motor is aimed at the lit-up LED light, and the 
button is pressed, it “Shoots” down the target. Once the time limit is reached, the game is over and a 
buzzer starts buzzing. The player can start a new game by pressing the switch.


How the game was designed:
The servo motor is controlled by the Potentiometer. For each LED that lights up, there are angles 
corresponding to which the “aim” is considered successful. The angles are accordingly mapped, and 
when the angle of the servo motor aligns with the angles towards the LEDs, then the value 1 is 
stored in a boolean. When the button is pressed, this value is passed and a shot is considered 
successful. Then a random LED lights up and the process is repeated. Every time a target is taken 
down successfully, the score of the player gets incremented and is displayed on the Serial Monitor. 
This goes on until a time limit of 30 seconds, after which the buzzer starts making a sound and the 
player is asked if they wish to continue.  

Components used:
x5 LED lights, a Servo Motor, a Potentiometer, a push-button switch, a Buzzer, x5 resistors of 220 
Ohms, several jumper wires, Arduino Nano Microcontroller Board and a breadboard.  
The code used for the project was written on Arduino IDE.   
