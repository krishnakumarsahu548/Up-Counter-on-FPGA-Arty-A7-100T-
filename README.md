# Up-Counter-on-FPGA-Arty-A7-100T-
This project implements a 3-bit up counter on the Digilent Arty A7-100T FPGA board using Verilog HDL. The counter increments on every clock pulse and is displayed on on-board LEDs. A clock divider is used to slow down the counting speed so that the LED transitions are clearly visible to the human eye.
# ⚙️ Features

3-bit binary up counter (000 → 111 → 000)

Visible LED blinking using a clock divider

Active-low reset (press BTN0 to reset count to zero)

Implemented and verified on Xilinx Vivado 2023.x

Target board: Arty A7-100T (xc7a100t-csg324-1)

# How it work clock divider
The clk_div register divides the 100 MHz clock.
When it overflows (≈ 1.34 s), the counter increments by 1.

LEDs show binary counting pattern 000 → 001 → 010 → … → 111 → 000.

Press BTN0 to reset the count to 000.

 # 🧰 Vivado Implementation Steps

Open Xilinx Vivado → Create New Project

Add the above Verilog file as the top module

Add the XDC file under Add or Create Constraints

Run Synthesis → Implementation → Generate Bitstream

Program the Arty A7-100T FPGA

Observe slow LED blinking in binary order

Press BTN0 to reset the counter

# Video
https://youtube.com/shorts/XJq5FsRQXXk?feature=share

# Schematic
<img width="1632" height="906" alt="image" src="https://github.com/user-attachments/assets/997f3d1e-1b76-4444-80fd-0c9fa28efae7" />

# 
<img width="1037" height="247" alt="image" src="https://github.com/user-attachments/assets/7bc9401e-ce79-49b1-a72d-52b6e3224adc" />
<img width="812" height="418" alt="image" src="https://github.com/user-attachments/assets/065e1072-b398-4fd7-bae2-82c7201d9cad" />
<img width="498" height="267" alt="image" src="https://github.com/user-attachments/assets/8c96b410-b908-439b-8aee-feedb1b455c6" /> 
<img width="501" height="258" alt="image" src="https://github.com/user-attachments/assets/8d858a4a-d5f2-4945-ac46-e295d0e83597" />




# 🧾 Author / Credits

Project: 3-bit Up Counter on FPGA

Developer: krishna Kumar
