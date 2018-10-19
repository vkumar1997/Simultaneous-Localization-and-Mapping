# Simultaneous Localization and Mapping

SLAM has multiple application in robotics. One of the main applications of SLAM is self-driving cars. The problem with self-driving cars is we cannot figure out the exact location of the car at a given time. GPS measumrements are only accurate upto 100 meters and Speedometers are inaccurate in upward and downward hill motions. However, we can reduce the errors using a sense-move cycle rather than just using sensors to determine accurate location. Sense leads to gaining of informations and accounts for low uncertainity and Move action leads to loss of information and increases uncertaininty. However, localiztion of car becomes accurate when these two are coupled.

Here, I show a small implementation of SLAM in the 2D world. Since the main objective is to show the convergence of localization, we use random sensor values (the sensor values represent distance from hypothetical landmarks) with induced uncertainity. Furthermore, we use random move action of the car per unit time along with induced motion uncertainity. The task is to reduce the error between observed and true localization (position of car after each time step and position of landmarks). 


#Result
The results are present in 'Landmark Detection and Tracking.html'. As we see, despite high initial uncertainity, the model converges well to find the position of car after each time step.