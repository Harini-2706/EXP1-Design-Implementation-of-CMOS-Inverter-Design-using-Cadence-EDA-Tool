Ex No: 01     **Design & Implementation of CMOS Inverter Design Using Cadence EDA Tools**

**Aim:**

To design and implement a CMOS inverter circuit using Cadence EDA tools, analyse its electrical characteristics, and understand the fundamental principles of CMOS technology, including the design process, layout, and simulation techniques.

**Tools Required:**

•	Personal Computer

•	Cadence Virtuoso Software

**SCHEMATIC SIMULATION** - 

   PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION -Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.

        •	csh
        •	source /cadence/install/cshrc
        •	virtuoso 
*Procedure for Schematic simulation using Cadence*

1.	Now two windows must open 
     i) virtuoso/command interpreter window
  	  ii)”Whats New…”
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
                                  
  Gpdk45 ------------------------nmos1v, pmos1v

	Create Input and Output pins

	Make the connections by using fixed narrow wire key

	Click Check and Save button

![WhatsApp Image 2024-10-05 at 09 41 42_9579137b](https://github.com/user-attachments/assets/f363ed8d-f186-4cc8-b735-256c71d9bd90)




 
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

 ![image](https://github.com/user-attachments/assets/3ea1dd7c-ff23-43e8-b5b4-dfa53a1547aa)



iv)	Creating the new test cell view

•	Go to CIW window, Execute File-New-Cell view

	Setup the new file form

	Library: Select the one you created.

	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test

	View: Schematic

	Type: Schematic press OK

•	Follow the step 3(ii) d to make the required connections

![WhatsApp Image 2024-10-05 at 09 32 42_83e7e39c](https://github.com/user-attachments/assets/14f40d32-a261-4974-a07d-386517946feb)




 
**Analog simulation by SPECTRE.**

•	In test cell view window

•	Launch – ADE L(Analog Design Environment)

	Execute Setup—Simulation/directory/Host A new window opens

	Set the simulation window to spectre and click ok

	Execute Analysis – Choose. A window opens.

	Select the type and set the specifications and press OK

	Execute Output s—to be plotted – Select on Schematic

	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse

•	Execute Simulation -- Net list and Run


![image](https://github.com/user-attachments/assets/49c06a21-9e69-48d5-b322-e6b8b27291c8)


_For Transient Analysis Settings and Output_
 
 
![image](https://github.com/user-attachments/assets/79a4f197-75e3-465a-aa8c-c51471fcdd5d)


 ![WhatsApp Image 2024-10-05 at 09 42 26_07aabde3](https://github.com/user-attachments/assets/1cd8503c-fe44-42ac-b202-57ff8a13dea0)



_For DC Analysis Settings and Output_
![image](https://github.com/user-attachments/assets/e82ef6f5-d495-4d2d-b524-46406c94b438)


![WhatsApp Image 2024-10-05 at 09 43 17_a04c348a](https://github.com/user-attachments/assets/94999838-b1f0-4d19-a1c5-d57e87723744)



 




 

**Results:**
1.	Successfully designed the CMOS inverter schematic using Cadence EDA tools.
2.	The simulation results demonstrated the correct logic operation of the inverter, where the output voltage switches between high (Vdd) and low (0V) levels, corresponding to the input voltage transitions.
3.	The Voltage Transfer Characteristic (VTC) curve was plotted, showing the relationship between input and output voltages.











