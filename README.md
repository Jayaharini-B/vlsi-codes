## 🛠 How to Run These Verilog Codes in Quartus

Follow the steps below to compile, simulate, and test the Verilog modules:

### 1. Create a New Project
1. Open **Intel Quartus Prime**.
2. Go to **File → New Project Wizard**.
3. Select a project directory and name (any name is fine).
4. Choose **Empty Project**.
5. Do *not* add files yet → Click **Next** and finish the setup.

### 2. Add Verilog Files
1. Go to **Project → Add/Remove Files in Project**.
2. Click **Add…** and select the `.v` or `.qpf` files from this repository.
3. Make sure all files appear in the project file list.
4. Click **OK**.

### 3. Set the Top-Level Entity
1. Identify your top module (Example: `full_adder`, `and_gate`, etc.)
2. Go to **Assignments → Settings**.
3. Click **Top-Level Entity** and set the correct module name.

### 4. Compile the Design
1. Click the **Start Compilation** button (purple triangle),
   or go to **Processing → Start Compilation**.
2. Wait for the analysis & synthesis to finish.
3. Check **Messages window** for errors/warnings.

### 5. Run Simulation (ModelSim / Quartus Simulator)
**Option A: Using ModelSim**
1. Open ModelSim from Quartus:  
   **Tools → Run Simulation Tool → RTL Simulation**
2. Add your testbench (`*_tb.v`) in the simulation files.
3. Compile and run the simulation.
4. View waveform using **Wave → Add → All Signals in Region**.

**Option B: Quartus Native Simulator (only for simple designs)**
1. Go to **Assignments → Settings → Simulation**.
2. Add testbench file under *Simulation Files*.
3. Run simulation from **Tools → Run Simulation Tool → RTL Simulation**.

### 6. View Output Waveforms
- Use **Format → Radix** to switch between Binary/Unsigned/Signed.
- Use Zoom In/Out to inspect timing behavior.
- Compare expected vs. actual outputs.

---

## 📎 Notes
- `.qpf` files in this repo are Quartus project files.  
- For simulation, always use the **testbench** files.  
- Ensure module names in `.v` files match the **top-level entity**.  
