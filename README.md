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


# 🧾 Author / Credits

Project: 3-bit Up Counter on FPGA

Developer: krishna
