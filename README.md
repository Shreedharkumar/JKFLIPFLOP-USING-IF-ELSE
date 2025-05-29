**Name: SHREEDHAR KUMAR K.J**

**REGISTER NO: 212224230265**

# EX NO: 4 - IMPLEMENTATION OF JKFLIPFLOP 

**AIM:** 

To implement  JK flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**JK Flip-Flop**

JK flip-flop is the modified version of SR flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of JK flip-flop is shown in the following figure.

![image](https://github.com/naavaneetha/JKFLIPFLOP-USING-IF-ELSE/assets/154305477/a649c30b-232b-4558-b188-fd6c09845180)


This circuit has two inputs J & K and two outputs Qtt & Qtt’. The operation of JK flip-flop is similar to SR flip-flop. Here, we considered the inputs of SR flip-flop as S = J Qtt’ and R = KQtt in order to utilize the modified SR flip-flop for 4 combinations of inputs. The following table shows the state table of JK flip-flop.

![image](https://github.com/naavaneetha/JKFLIPFLOP-USING-IF-ELSE/assets/154305477/c4360742-e8a8-4937-b089-c46c0433f9a3)

 
Here, Qtt & Qt+1t+1 are present state & next state respectively. So, JK flip-flop can be used for one of these four functions such as Hold, Reset, Set & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of JK flip-flop. Present Inputs Present State Next State
 
![image](https://github.com/naavaneetha/JKFLIPFLOP-USING-IF-ELSE/assets/154305477/6c275261-a6d5-4c37-a3a7-1e88ca11c4cd)

By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. Three variable K-Map for next state, Qt+1t+1 is shown in the following figure.
 
![image](https://github.com/naavaneetha/JKFLIPFLOP-USING-IF-ELSE/assets/154305477/5174f41b-0ce0-4329-a372-6d1943ea6673)

The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=JQ(t)′+K′Q(t)Q(t+1)=JQ(t)′+K′Q(t)

**PROCEDURE**

### 1. Open Quartus Software
Launch **Quartus Prime** on your system.

### 2. Create a New Project
- Navigate to **File > New Project Wizard**.
- Set your **project directory**, **project name**, and **top-level entity name**.
- Add your **Verilog (.v)** or **VHDL (.vhd)** source file.
- Select the correct **FPGA device** based on your target board.

### 3. Add Design Code
- Open your top-level module (e.g., `main.v`).
- Paste or write your Verilog/VHDL design.

### 4. Compile the Design
- Go to **Processing > Start Compilation**.
- Wait until the compilation process is complete.
- Resolve any errors or warnings if present.

### 5. Generate RTL Schematic
- Navigate to **Tools > Netlist Viewers > RTL Viewer**.
- View the generated RTL schematic.
- Save the schematic using **File > Export** (as image or PDF).

### 6. Assign I/O Pins
- Open **Assignments > Pin Planner**.
- Assign FPGA pins to your module’s inputs and outputs.
- Click **Save** once done.

### 7. Create Waveform for Simulation
- Go to **File > New > Other Files > Vector Waveform File (.vwf)**.
- Click **Edit > Insert > Insert Node or Bus**.
- Select all input and output signals to monitor.

### 8. Set Simulation Parameters
- Define end time using **Edit > End Time** (e.g., `1 us`).
- Apply different **input combinations** on the waveform.

### 9. Run Functional Simulation
- Go to **Processing > Start Simulation**.
- The **timing diagram** (simulation output) will be displayed.

### 10. Save the Timing Diagram
- Save the waveform for future reference.
- Export the timing diagram image via **File > Export Image**.
   

**PROGRAM**

![Screenshot 2025-04-21 102549](https://github.com/user-attachments/assets/a12f441d-d886-4cf9-8743-52f40290cb3b)


**RTL LOGIC FOR FLIPFLOPS**

![Screenshot 2025-04-21 102702](https://github.com/user-attachments/assets/f60b1ed7-b31d-498d-9b1e-67c7a940edd7)


**TIMING DIGRAMS FOR FLIP FLOPS**

![Screenshot 2025-04-21 103217](https://github.com/user-attachments/assets/1c8d53d9-8065-4d8e-8c8f-76e7873a89b2)


**RESULTS**

JK flipflop is implemented using verilog and their functionality using their functional tables is validated.
