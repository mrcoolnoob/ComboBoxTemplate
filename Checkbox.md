# How Tick is drawn in the checkbox?

Certainly! The Data attribute in the Path element contains a string that represents a series of commands and coordinates that define the geometry of the tick mark. This string uses the Path Markup Syntax of WPF to describe the shape of the tick mark. Let's break down the commands and coordinates in the Data attribute:

M 4.5,7.6: The "M" command stands for "MoveTo" and is followed by the X and Y coordinates. This command sets the starting point of the path to the point with the coordinates (4.5, 7.6).
L 7,10: The "L" command stands for "LineTo" and is followed by the X and Y coordinates. This command creates a straight line from the current point (4.5, 7.6) to the point with the coordinates (7, 10).
12,5: Since the "L" command was used previously, it is implied that any following pairs of coordinates are also part of the LineTo command. This creates a straight line from the previous point (7, 10) to the point with the coordinates (12, 5).
These three commands create a checkmark-like shape that represents the tick mark. When the CheckBox is checked, the tick mark becomes visible, and the Path element displays the checkmark shape based on the commands in the Data attribute.

You can modify the coordinates in the Data attribute to adjust the size, position, and shape of the tick mark.
