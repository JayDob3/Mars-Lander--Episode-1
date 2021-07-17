# Mars-Lander--Episode-1

# Game Input
The program must first read the initialization data from standard input. Then, within an infinite loop, the program must read the data from the standard input related to Mars Lander's current state and provide to the standard output the instructions to move Mars Lander.

# Initialization input
Line 1: the number surfaceN of points used to draw the surface of Mars.
Next surfaceN lines: a couple of integers landX landY providing the coordinates of a ground point. By linking all the points together in a sequential fashion, you form the surface of Mars which is composed of several segments. For the first point, landX = 0 and for the last point, landX = 6999

#Input for one game turn
A single line with 7 integers: X Y hSpeed vSpeed fuel rotate power
X,Y are the coordinates of Mars Lander (in meters).
hSpeed and vSpeed are the horizontal and vertical speed of Mars Lander (in m/s). These can be negative depending on the direction of Mars Lander.
fuel is the remaining quantity of fuel in liters. When there is no more fuel, the power of thrusters falls to zero.
rotate is the angle of rotation of Mars Lander expressed in degrees.
power is the thrust power of the landing ship.

# Output for one game turn
A single line with 2 integers: rotate power :
rotate is the desired rotation angle for Mars Lander. Please note that for each turn the actual value of the angle is limited to the value of the previous turn +/- 15°.
power is the desired thrust power. 0 = off. 4 = maximum power. Please note that for each turn the value of the actual power is limited to the value of the previous turn +/- 1.

# Constraints
2 ≤ surfaceN < 30
0 ≤ X < 7000
0 ≤ Y < 3000
-500 < hSpeed, vSpeed < 500
0 ≤ fuel ≤ 2000
-90 ≤ rotate ≤ 90
0 ≤ power ≤ 4
Response time per turn ≤ 100ms
