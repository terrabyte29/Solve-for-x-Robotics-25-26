Spreadsheet for controls:
https://docs.google.com/spreadsheets/d/15B_y9Lt4vU23R9hhuVtT6RbHhSsFFPGtf5XDaz9-9wo/edit?gid=0#gid=0

Functionality:
There are two match autonomous routes, one for left and one for right. At this moment, both routes pick up the three balls from the middle, score them onto the respective sides high goal, and then drive forward into a match loader, picking up three balls of the correct color, and then score those into the same high goal. Then the auton route ends. 
The skills auton is currently unfinished and is in a prototype stage

Driver controls:
In Arcade control:
Left stick controls forwards/backwards movement
Right stick controls turning

In Tank control:
The left stick controls left side drivetrain throttle
The right stick controls right side drivetrain throttle

Exponential factors:
In Arcade mode, the throttle and turn have seperate exponential factors, allowing for different exponential curves

The drive mode is determined by the active user. See include/users_class.h and func setActiveUser() in src/main.cpp for code

Intake and Scoring:
The controls vary by user preference, but the common scheme is:
R1: Spins intake up and upper transit motor down, scoring for the middle goal
R2: Spins intake up and upper transit motor up, scoring for the high goal
L1: Toggles the stopper pneumatic on the high goal ball out
L2: Spins intake down and upper transit motor down, scoring for the low goal
B: Toggles the tounge mech, meant for funneling balls out of the match loader
