# VLSI-LAB-EXP-6
# AIM:
To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

# APPARATUS REQUIRED:
1.Laptop with MobaXterm

2.Cadence tool PROCEDURE SCHEMATIC ENTRY: Creating a new library:

3.In the library manager, execute File - New library. The new library form appears.

4.In the new library form, type ‘my design lib’ in the name section.

5.In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.

6.In the next ‘technology file for new library form select option attach to an existing tech file and click ok.

7.In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.

8.After creating a new library you can verify it from the library manager.

9.If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.

# Creating a schematic cell view:
1.In the CIW or library manager, execute file – new – cell viw.

2.Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.

3.Click ok when done the above setting. A black schematic window for the inverter design appears.

# Adding components to schematic:
1.In the inverter schematic window, click the instance fixed menu icon to display the add instance form.

2.Click on the browse button. This opens up a library browser from which you can select components and the symbol view.

3.After you complete the add instance form move your cursor to the schematic window and click left to place a component. LIBRARY NAME CELL NAME gpdk045 PMOS gpdk045 NMOS

4.This is a table of components for building the inverter schematic.

5.After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.
![WhatsApp Image 2024-05-15 at 09 28 09_a3a21eb3](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163832108/d23c306a-8735-4f78-bb34-b44e7cae4063)
# Adding pins to schematic:
1.Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.

2.Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin. PIN NAMES DIRECTION Vin,Vdd,Vss Input Vout Output

3.Select cancel and then the schematic window enter window file or press the f bind key. Adding wires to schematic:

4.Click the wire (narrow) icon in the schematic window.

5.In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.

6.Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.

7.Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.

# Saving the design:
Click the check and save icon in the schematic editor window observe CIW output for any errors.

# BUILDING THE INVERTER TEST DESIGN: Creating the inverter test cell view:
1.In the CIW or library manager, execute file – new – cell view.

2.Setup the newfile as shown below.

3.Click ok when done. A blank schematic window for the inverter test design appears.

4.Using the components list and properties/ comments in this table build the inverter test schematic. LIBRARY NAME CELL VIEW NAME PROPERTIES/COMMENTS My design lib Inverter Symbol Analog lib Vpulse Voltage1 = 0, Voltage2 = 1.8, delay Time = 0, Rise time=Fall time=1ns Period=20ns Analog lib Vdc, gnd Vdc = 1.8v

5.Add the above components using create – instance or by pressing I.

6.Click the wire (narrow) icon and wire your schematic.

7.Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.

8.Click on the check and save icon to save the design.
![WhatsApp Image 2024-05-15 at 09 28 47_6aa5481c](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163832108/57ea38f6-34c1-4354-ace0-5e7cfeaab4d3)
# ANALOG SIMULATION WITH SPECTRA: Starting the simulation environment:
1.In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears. Choosing a simulator:

2.In the simulation window (ADE) execute setup – simulator / directory / host.

3.In the choosing simulator form, set the simulator field to specra and click ok.

4.In the simulation window (ADE) execute the setup model libraries. To complete, move the cursor and click ok. Choosing Analysis:

5.Click the choose- Analysis icon in the simulation window (ADE).

6.The choosing analysis form appears.

7.To Setup the transient analysis. a. In the analysis section select tron. b. Set the stop time as 100ns c. Click at the moderate or enabled button and the bottom and then click apply.

8.To set for DC analysis a. In the analysis section select DC. b. Turn on save DC operating point. c. Turn on the component parameters. d. Double click the select Vpulse source or Type V0 (capital V zero). e. Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8. f. Select the enable button and click apply and then click ok.

# Selecting output for plotting:

1.Execute the o/p’s to be plotted -select on sschematic in the simulation window.

2.Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.

# Running the simulation:
1.Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.

2.When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.
![WhatsApp Image 2024-05-15 at 09 29 10_a4fbba75](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163832108/4ffb16e0-2019-4a95-9ad9-7a119772fb16)
![WhatsApp Image 2024-05-15 at 09 29 20_3503ef00](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163832108/c8c3baed-6021-44ee-b248-9fa93e4c2a85)
# CMOS NAND GATE
# NAND SCHEMATIC
![WhatsApp Image 2024-05-15 at 12 09 00_54010864](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163832108/152e3e14-8b4b-4738-8665-5adbe71d5b18)
# NAND TEST CELL VIEW
![WhatsApp Image 2024-05-15 at 12 09 25_d9228be2](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163832108/6d5c1262-ccca-4e73-a34f-fb846dc62d8f)
# NAND SIMULATION WITH SPECTRA
![WhatsApp Image 2024-05-15 at 12 09 50_681e29d8](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163832108/c07930b8-d7fe-4cbf-9c9e-8ff961842294)
# CMOS NOR GATE
# NOR SCHEMATIC
![WhatsApp Image 2024-05-15 at 12 10 15_4d1749f8](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163832108/9f863e56-cd57-44c1-886c-8255abd27f28)
# NOR TEST CELL VIEW
![WhatsApp Image 2024-05-15 at 12 10 36_41cf9830](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163832108/f7fd995a-3192-408d-8e67-653922a5584f)
# NOR SIMULATION WITH SPECTRA
![WhatsApp Image 2024-05-15 at 12 11 00_5eac5faa](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163832108/2e4f6fdb-6a14-44d4-bbe7-c99f7b02c73a)
# RESULT:
THe design and simulation of the CMOS inverter and the DC and transient responses using cadence tool is successfully observed and verified.
