# Design-Implementation-of-2-Bit-Multiplier-using-Cadence-Tools
Ex No: 05     Design & Implementation of 2 bit multiplier Using Cadence EDA Tools   

Aim:
To design and implement a 2-bit multiplier circuit using Cadence EDA tools, simulate its functionality, and to understand its application in digital arithmetic operations.

Tools Required:
•	Personal Computer
•	Cadence Virtuoso Software

S C H E M A T I C S I M U L A T I O N - PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION -Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
•	csh
•	source /cadence/install/cshrc
•	virtuoso 
Procedure for Schematic simulation using Cadence

1.	Now two windows must open i) virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.
i.	Create a New Library
ii.	Create Schematic Cell view.
iii.	Create the Symbol for schematic Cell view.
iv.	Create the test Cell view.
v.	Analog simulation by spectre


i)	Procedure for Creating New Library.
•	File –New – Library
•	Name: Give name for ur library Ex: VLSILAB_EXP_1
•	Enable Attach to an existing technology library, Click OK
•	Attach the library to the technology library gpdk045.Click OK
ii)	Create Schematic Cell view.
•	Go to 1st window i.e virtuoso (CIW)
•	File-New-Cell view
•	Setup the new file form
	Library: Select the one you created.
	Cell: Give the experiment name Ex: Inverter ViewSchematic
	Type: Schematic press OK
•	Add the required components from the libraries and make the connections.
	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	Click on browse. This opens the library browser
	Now select the appropriate library for components like 
	Gpdk45 ------------------------nmos1v, pmos1v
	Create Input and Output pins
	Make the connections by using fixed narrow wire key
	Click Check and Save button

![sche](https://github.com/user-attachments/assets/1769d742-f791-48a6-9220-7be32fc49462)


 
iii)	Creating the Symbol for schematic Cell view

•	In the schematic window, execute 
	Create – Cell view – From Cell view
	The cell view from cell view window appears
	Check Lib Name, Cell Name, From View name must be schematic Press ok
•	Now Symbol generation form appears. Click Ok If No changes required
•	A new window with with default symbol is created.
•	Edit the symbol if you want to give actual symbol shape else continue.
•	Execute Create-Cell view-from cell view
•	Library Name and Cell Name must be same which you have used for schematic. Press OK
•	Check for the position of pin side.Prss OK
•	Edit for the shape by Create-Shape-Choose required options to edit.

![sym](https://github.com/user-attachments/assets/c772ea3c-d6fb-4c35-8a46-4369caaf62d1)




iv)	Creating the new test cell view

•	Go to CIW window, Execute File-New-Cell view
	Setup the new file form
	Library: Select the one you created.
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	View: Schematic
	Type: Schematic press OK
•	Follow the step 3(ii) d to make the required connections


![stim](https://github.com/user-attachments/assets/9f2e8fb7-1a26-42a4-ac88-da089713c7a2)


 

Analog simulation by SPECTRE.
•	In test cell view window
•	Launch – ADE L(Analog Design Environment)
	Execute Setup—Simulation/directory/Host A new window opens
	Set the simulation window to spectre and click ok
	Execute Analysis – Choose. A window opens.
	Select the type and set the specifications and press OK
	Execute Output s—to be plotted – Select on Schematic
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
•	Execute Simulation -- Net list and Run

![Screenshot 2024-11-16 205108](https://github.com/user-attachments/assets/7b6b5f84-63df-4a62-96c4-b6b029f3bd05)


For Transient Analysis Settings and Output
![Screenshot 2024-11-16 205123](https://github.com/user-attachments/assets/363b4dac-75bd-4cee-bd62-84bcc3a30a89)


 ![Screenshot 2024-11-16 205142](https://github.com/user-attachments/assets/d6ad7ca5-2b80-4793-a044-80ce621cbaba)

  

Results:
The design and implementation of the 2-bit multiplier using Cadence EDA tools were successfully carried out. The simulation results confirmed the correct operation of the multiplier for all input combinations. 
