# CMPEN270-Lab15a-PongPart1
Modify a behavioral description of a finite state machine

Functional Specification
In this lab you will make a basic pong game. The LEDs are used to show the position of the ball and the 
left and right buttons act as the paddles.
1. I/O
a. Map switches to SWITCH, type STD_LOGIC_VECTOR(15 downto 0)
b. Map the left, right, up and down buttons to BTNL, BTNR, BTNU and BTND, type STD_LOGIC
c. Map the board clock to CLK, type STD_LOGIC
d. Map LEDs 15:0 to LED, type STD_LOGIC_VECTOR(15 downto 0)
e. Map 7-segment display segments to SEGMENT, type STD_LOGIC_VECTOR(0 to 6)
f. Map 7-segment display anodes to ANODE, type STD_LOGIC_VECTOR(3 downto 0)
2. Operation
a. Player 1 is on the left side and player 2 is on the right side.
b. The left button is the paddle for player 1 and the right button is the paddle for player 2.
c. The up button serves the ball.
d. When player 1 serves the ball, the LEDs move to the right. Player 2 must press the right button 
when LED 3, 2, or 1 is lit, or they lose the point and player 1 serves again. If player 2 presses the 
right button when LED 3, 2 or 1 is lit, the ball moves to the left and player 1 must press the left 
button when LED 14, 13 or 12 is lit or they lose the point and player 2 serves again. If player 1 
presses the left button when LED 14, 13 or 12 is lit, the ball moves to the right and play 
continues.
e. The down button resets the game, with player 1 ready to serve.

Discussion
This lab introduces you to an easier way to describe finite state machines in VHDL. Two FSMs are used, 
a display FSM that drives the LEDs to show the pong game, based on inputs from a control FSM that 
controls the game. This is the first of a two-part lab for this module

[Lab15a_TopLevel.pdf](https://github.com/cjdrangel209/CMPEN270-Lab15a-PongPart1/files/11512640/Lab15a_TopLevel.pdf)
[Lab15a_ControlFSM.pdf](https://github.com/cjdrangel209/CMPEN270-Lab15a-PongPart1/files/11512641/Lab15a_ControlFSM.pdf)
[Lab15a_DisplayFSM.pdf](https://github.com/cjdrangel209/CMPEN270-Lab15a-PongPart1/files/11512642/Lab15a_DisplayFSM.pdf)
