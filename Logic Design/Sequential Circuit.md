- **Combinational** circuits rely exclusively on the inputs / fucntion of inputs 
- **Sequential** circuits are function of inputs and internal memory
	1. **Synchronous** : controlled by a clock
	2. **Asynchronous** : changes can happen at any instance of time  

## Clock
![](Images/clock.png)
**High Level / Positive Pulse** : when the level of the clock is 1
**Low Level / Negative Pulse**: when the level of the clock is 0
**Rising Edge**: when the clock goes from 0 to 1
**Falling Edge**: when the clock goes from 1 down to 0

## Latches
A latch is **level-sensitive**
Final value of output 𝑄 is uncertain > not used in synchronous circuits
![](Images/latches.png)
### Graphic Symbols
![](Images/latches-graphic.png)
## Flip-Flops
![](Images/Flip-Flops.png)
![](Images/ff-excitation.png)
### Graphic Symbols
The circle on the clock input indicates a **falling edge-triggered** FF
![](Images/ff-graphics.png)

## State Table
![](Images/state-table.png)
## State Diagram
State is in the bubble and 0/0 stands for INPUT/OUTPUT  
![](Images/state-diagram1.png)    
00/0 in the bubble stands for STATE/OUTPUT and the arrows contain the input  
![](Images/state-diagram2.png)  