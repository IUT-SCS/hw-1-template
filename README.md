# Homework #1
### TurtleSim Digit Drawing
**Description:** A single Python ROS node that launches four turtles in a `turtlesim_node` window and commands each turtle to draw one digit. The four digits correspond to the last four digits of a student ID, and all four turtles draw their respective digits simultaneously (*in parallel*).
#### Steps:
1. **Launch of Simulator.** `turtlesim_node` is started in a separate terminal before running your script. Your node connects to the already-running simulator.
2. **Additional turtles get spawned.** The simulator starts with one turtle (`turtle1`). `/spawn` service creates three more, giving a total of four turtles.
3. **Positioning of the turtles.** Each turtle teleports to a starting location so the four digits will appear side by side without overlapping. Canvas is divided into four vertical zones.
4. **Designing digit shapes.** Each digit is drawn using straight lines and turns. No need for pixel-perfect rendering — the digits need to be clearly recognizable.
5. **Drawing digits in parallel.** All four turtles actively draw at the same time. A sequential approach will not receive full marks.

\
**Result:** Last four digits of a student ID.
```
Example: ID = U2010164
- turtles draw 0, 1, 6, and 4 from left to right.
```
