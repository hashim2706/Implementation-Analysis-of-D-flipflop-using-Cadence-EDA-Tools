## Ex No: 02--Design-Implementation-of-Full-Custom-2-1-MUX-using-Cadence-EDA-Tools

### Aim:
To design and implement a D-flip-flop using Cadence EDA tools, simulate its behavior, and analyze key performance parameters such as timing, power consumption, and resource utilization for a comprehensive understanding of sequential logic circuits.

### Tools Required:

- Personal Computer
- Cadence Virtuoso Software

### Circuit Diagram:

![image](https://github.com/user-attachments/assets/4466dbeb-ff80-41c1-a19e-12994b98eb4d)

### S C H E M A T I C S I M U L A T I O N:

PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
	- csh
	- source /cadence/install/cshrc
	- virtuoso

Procedure for Schematic simulation using Cadence

1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”

2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
	
  - Create a New Library
  - Create Schematic Cell view.
  - Create the Symbol for schematic Cell view.
  - Create the test Cell view.
  - Analog simulation by spectre



i)	Procedure for Creating New Library.

- File –New – Library
- Name : Give name for ur library Ex: VLSILAB_EXP_2
- Enable Attach to an existing technology library, Click OK
- Attach the library to the technology library gpdk045.Click OK

ii)	Create Schematic Cell view.

- Go to 1st window i.e virtuoso(CIW)
- File-New-Cell view
- Setup the new file form
	 + Library: Select the one you a created.
	 + Cell : Give the experiment name Ex: Inverter View_Schematic
	 + Type: Schematic press OK
    
- Add the required components from the libraries and make the connections.
	 + Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	+ Click on browse. This opens the library browser
	+ Now select the appropriate library for components like 
	+ Gpdk45 ------------------------nmos1v,  pmos1v
	+ Create Input and Output pins
	+ Make the connections by using fixed narrow wire key
	+ Click Check and Save button


![WhatsApp Image 2024-11-17 at 14 40 07_1076bb98](https://github.com/user-attachments/assets/e7570cf6-cd0b-4c98-b0ac-d52bb8d29830)




iii)	Creating the Symbol for schematic Cell view

- In the schematic window, execute 
	+	Create – Cell view – From Cell view
	+	The cell view from cell view window appears
	+	Check Lib Name, Cell Name, From View name must be schematic Press ok
- Now Symbol generation form appears. Click Ok If No changes required
- A new window with with default symbol is created.
- Edit the symbol if you want to give actual symbol shape else continue.
- Execute Create-Cell view-from cell view
- Library Name and Cell Name must be same which you have used for schematic. Press OK
- Check for the position of pin side.Prss OK
- Edit for the shape by Create-Shape-Choose required options to edit.

![WhatsApp Image 2024-11-17 at 14 40 07_c9cba221](https://github.com/user-attachments/assets/6e26f23a-cadf-4224-8a4b-a12565f4dc5a)


 
iv)	Creating the new test cell view

- Go to CIW window, Execute File-New-Cell view
	+ Setup the new file form
	+ Library: Select the one you created.
	+ Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	+ View: Schematic
	+ Type: Schematic press OK
- Follow the step 3(ii) d to make the required connections

![WhatsApp Image 2024-11-17 at 14 40 05_fbc1f15b](https://github.com/user-attachments/assets/4bb62e04-fc7b-4ccb-aa82-67c7908fc7f2)




### Analog simulation by SPECTRE.

- In test cell view window
- Launch – ADE L(Analog Design Environment)
	+ Execute Setup—Simulation/directory/Host A new window opens
	+ Set the simulation window to spectre and click ok
	+ Execute Analysis – Choose. A window opens.
	+ Select the type and set the specifications and press OK
	+ Execute Output s—to be plotted – Select on Schematic
	+ Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
- Execute Simulation -- Net list and Run

![WhatsApp Image 2024-11-17 at 14 40 07_935aea16](https://github.com/user-attachments/assets/d5124120-a92f-4b11-aed0-3e518d8483b0)



### For Transient Analysis Settings and Output


![WhatsApp Image 2024-11-17 at 14 40 06_4379d571](https://github.com/user-attachments/assets/da4f427e-b781-4683-9d85-2f1e284730d7)



![WhatsApp Image 2024-11-17 at 14 40 06_212c53eb](https://github.com/user-attachments/assets/79b249e5-024a-4786-a20b-dc3cb6da2684)




### Results:

1. The experiment successfully demonstrated the design and implementation of a 2:1 MUX using Cadence EDA tools. 
2. The successful verification through schematic, layout, and simulation underscores the effectiveness of using Cadence EDA tools for digital circuit design.











