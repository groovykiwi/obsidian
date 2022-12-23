Combinational circuit rely exclusively on the inputs / fucntion of inputs 
Sequential circuits a function of inputs and internal memory

Synchronous is controlled by a clock
Clock signal is an input to the memory elements

present state: output value of memory (stored)
next state: input value to memory (to be stored)

## Clock
![](Images/Clock%20Cycle.png)
- **Positive Pulse**: when the level of the clock is 1
- **Negative Pulse**: when the level of the clock is 0
- **Rising Edge**: when the clock goes from 0 to 1
- **Falling Edge**: when the clock goes from 1 down to 0
## Latches
### SR latch
| S   | R   | Q   | $\bar{Q}$ | State                            |
| --- | --- | --- | --------- | -------------------------------- |
| 0   | 0   | X   | X         | No change                        |
| 0   | 1   | 0   | 1         | Reset                            |
| 1   | 0   | 1   | 0         | Set                              |
| 1   | 1   | -   | -         | Undefined (Oscillation 1&rarr;0) | 

### $\bar{S}\bar{R}$ Latch with NAND
| $\bar{S}$ | $\bar{R}$ | $Q$ | $\bar{Q}$ | State                            |
| --------- | --------- | --- | --------- | -------------------------------- |
| 1         | 1         | X   | X         | No change                        |
| 1         | 0         | 0   | 1         | Reset                            |
| 0         | 1         | 1   | 0         | Set                              |
| 0         | 0         | -   | -         | Undefined (Oscillation 0&rarr;1) |

### SR Latch with a Clock Input
Same as a normal SR Latch but only has an effect when C=1  
Uses a $\bar{S}\bar{R}$ Latch with 2 NAND gates
![](Images/SR%20Latch%20with%20clock.png)
### D Latch
![](Images/D%20Latch.png)
### Graphic Representation
![](Images/Graphic%20Latches.png)