# Graph-Plotter


A Graph is a visual representation of the values taken by a function for a varying input(s).
Graphs help us determine how the output changes with the input, finding patterns in the output and various other properties of the function.

A 2D graph plotter creates a 2-Dimensional graph of a function with one varying input. The input is usually plotted along the x-axis, and the output of the function along the y-axis.

This graph plotter first accepts the function to be plotted from the user. The function can be a combination of the input, and other most commonly used functions of the input.
When the function is ready, it is plotter on the next screen, denoted by the blue line on the screen. The values of the function at various points can be determined.

The graph can also be zoomed into, or zoomed out of to view more detailed values or to see a greater area of the graph.

Demo video : https://www.youtube.com/watch?v=YN2x8QCyRuU

### How to Run

1. Connect pins to microcontroller according to the table below.
2. Open 'project.uvproj' with Keil UVision IDE.
3. Compile and load the program into the microcontroller by connecting the 'Launch Pad' to the computer via USB.
4. Disconnect the USB cable and attach it to a power supply(eg. back to the USB port itself), which starts the program on the microcontroller.


### Required Hardware I/O connections-

#### Touch Screen connections

Touch operated through the SSI interface. Requires total 5 pins.

| Connection	| uC pins |
|-------------|---------|
| t_cs | PA2 |
| t_clk | PA3 |
| t_out (MISO) | PA4 |
| t_in (MOSI) | PA5 |
| t_pen | PA6 |

#### LCD Display Connections

The display is operated through parallel 16 bit bus. Requires 16 pins for data bus, 5 pins for control signals.

| Connection	| uC pins |
|-------------|---------|
| lcd_cs | PD0 |
| lcd_rd | PD1 |
| lcd_wr | PD2 |
| lcd_rs | PD3 |
| lcd_rst | PD6 |

Databus:

| DB0	| DB1	| DB2	| DB3	| DB4	| DB5	| DB6	| DB7	| DB8	| DB9	| DB10	| DB11	| DB12	| DB13	| DB14	| DB15	|
|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|
| PB0 | PB1 | PB2 | PB3 | PB4 | PB5 | PE0 | PE1 | PE2 | PE3 | PE4 | PE5 | PC4 | PC5 | PC6 | PC7 |


### Built With
Built on the ARM Cortex M4 microcontroller, TM4C123GH6PM, with the Texas Instruments Tiva C series TM4C123G Launch Pad. 

Keil uVision4 used as the IDE.
