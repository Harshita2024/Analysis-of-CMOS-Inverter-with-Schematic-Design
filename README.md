# Analysis-of-CMOS-Inverter-with-Schematic-Design
 ## Introduction
 Complementary Metal-Oxide-Semiconductor (CMOS) technology forms the foundation of modern VLSI systems. By combining pMOS and nMOS transistors in a complementary arrangement, CMOS circuits achieve low static       power dissipation, high noise margins, and scalability to nanometer process nodes. This energy efficiency and robustness have made CMOS the dominant choice for digital logic design, processors, and memory         elements in today’s integrated circuits.<br>
The CMOS inverter, being the most fundamental logic element, plays a crucial role in digital design. Its schematic consists of a pMOS connected to the supply voltage and an nMOS connected to ground, sharing a     common output node. This simple yet powerful configuration serves as the basis for implementing all other logic functions, making it an ideal circuit for performance evaluation and characterization.<br>
From a VLSI perspective, the CMOS inverter is often treated as a benchmark cell to extract key performance parameters that influence the design of larger and more complex circuits. In this project, we have performed a detailed study involving DC analysis, transient analysis, propagation delay measurement, evaluation of output capacitance effects, and calculation of power dissipation components. These analyses provide valuable insights into circuit behavior, enabling optimization for speed, power, and area in advanced VLSI designs.

## Tools and Technologies used
- **Cadence Virtuoso 6.1.7-64b** – For Schematic design  
- **GPDK 90nm** – Process Design Kit used

## Steps to be followed:
 **Step 1:** Invoking the Tool
  - Open the terminal and run the following commands to start Cadence Virtuoso:
  - csh-> cd cds_working-> source cshrc.cadence-> virtuoso <br>
  
**Step 2:** Creating a Library
  - In the Virtuoso window, go to File → New → Library.
  - In the dialog box, enter a suitable Library Name (e.g., CMOS_Inverter).
  - Select Attach to an existing technology library option.
  - From the list, choose ts018_scl_prim as the technology library.
  - Click OK to create and attach your new library. <br>
  
**Step 3:** Creating the Schematic
  - Create a Cell View
    - Go to Cell View → select the library you just created.
    - Enter a Cell Name (e.g., inverter).
    - Click OK.
  - Draw the Schematic
    -  Add Instances
      - pMOS and nMOS: Select pmos_18 and nmos_18 from ts018_scl_prim library.
      - VDD and GND: Select from analogLib library.
    -  Add Wires
      -  Use Create → Wire to connect the components properly.
    -  Add Pins
      - For schematics, only input and output pin types are used.
      - Create input pin with direction "input".
      - Create output pin with direction "output".
      - InputOutput type is mainly required for supply changes and layout design.
   - Check and Save the Schematic
      - Go to Check and Save.
      - If there are errors, recheck the connections and correct them.
      - Once error-free, your schematic design is complete.



