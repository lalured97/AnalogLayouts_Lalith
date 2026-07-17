# AnalogLayouts_Lalith
This a repo consisting of all the masks of certain schematics made by me which are LVS (layout versus schematic) and DRC (design run check verified) according to the TSMC 28 nm Technology, using the industry-grade layout tool of Cadence-Virtuoso.

In the Industry Level , Analog Layouts are the creation of Masks. Masks Determine how a chip is fabricated. The schematic Engineer designs the schematic with the knowledge of Analog Devices and Digital Devices (as i myself have learned through my course of Digital Design at International Institute of Information Technology, Banglore), but to see how it goes on a chip into the real world is a whole new ball game.

In the real world, the foundries( Ex: TSMC ) cannot design with the scehmatic alone. It is not their job. Their job is to manufacture the chip using masks. The middle man who generates the masks for the foundries to use is called a Layout Engineer.

The task of a Layout Engineer may seem simple. But in order to make a single layout, a layout engineer depanding upon the specifications needed for the product/chip which is being manufactured has to try to maximise or minimise some certain parameters, like he has to minimise Area usage but at the same time has to try to increase the performance. The schematic engineer only shows the connections and the devices and the i/o ports. The Layout engineer has to take that and create different masks. The masks show Layer by layer from bottom to up what layers need to be implanted, what is the area and what devices etc. The layout engineer needs to talk about the placement of the substrate, wells, taps, oxide layers, polysilicon layers, the different metal layers, VTH layers etc. And he cannot place or optimise them however he wants, he has to understand the product and also understand the limitations the foundry has, by going through the DESIGN RULE MANUAL.

The Design Rule Manual (DRM) is given by the foundry for a certain Technology. Each chip technology has a different DRM. The chip i have worked on is 28nm chip technology. And within this there are hundreds of rules. Rules for spacing, minimum area, interaction of two layers, enclosures, Antenna effects, Latch-ups etc.

The Analog engineer has to take care of all this and maximise performance by minimising power and area used. To verify everything he also has to run a number of checks like LVS, DRC, ERC, EMIR etc. I have mainly checked the primary LVS, ERC and DRC. LVS, through the creation of a netlist ensures that the nets and inputs and outputs and the VDD and VSS connections for each device and total circuit are right. The DRC takes all the rules of DRM given for your technology and starts comparing and saying if u have any mistake within say metal spacing, poly spacing, poly enclosure, p-plus enclosure, metal area, latch up errors, antenna effect errors.

I have made the following layouts under 2 weeks after learning the required process and theory:
1)INVERTER GATE
2)NAND GATE
3)AND GATE
4)NOR GATE
5)XNOR GATE

I have made the Inverter and NAND and NOR from transitor level and then combined and routed on them to make AND and XNOR. Both of them Had a different set problems and different use of layers to some extent. To account for the problems into XNOR, one has to ensure there are no DRC and LVS problems in all the basic agtes and if there is a problem, say in inverter, u have to come adjusting in all of them again,in some cases , completely changing the spacings, areas and layer sizes in all of the gates used.

The needed knowledge to ensure you have a successful layout is:
Basics: Wafer Process, Resistors, Capacitors, Power Dissipations, MOSFETS, Logic Gates, Transistors.

Core: The Overall Design Flow, Reading the DRM, Learning about the Lyout tool being used, Netlists and Stick Diagrams, All Mandatory verification checks, Device Formation with Layers, Multipliers, Fingers, Deep Sub-Micron Effects, Floor Plan, InterConnects and Parasitics, Crosstalk and Shielding, Antenna, Latch-Up, Density, EMIR, Deep Wells, Electro-Migration Effects, Electro Static Dissipation, FinFets, Double Patterning, Matching, Memory Architecture and Constraints, DeltaV DRC's, High Speed Layout Design, High Voltage Layout Design.
