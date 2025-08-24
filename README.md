# Audio-Amplifier
This project implements real-time audio processing using a Basys-3 FPGA board and a Pmod I2S2 digital audio interface. The audio processing is performed using low-pass, high-pass, band-pass, and moving average FIR filters.

Hardware Requirements:
1.Basys-3 FPGA board
2.Pmod I2S2 digital audio interface

Software Requirements:
1.GNU Octave or MATLAB for generating filter coefficients using the filter_gen.m script.
2.Vivado Design Suite for synthesizing and implementing the FPGA design.

Files:
1.Baysys-3-Master.xdc: Constraints file for the Basys-3 FPGA board.
2.fir_backend.sv: Implementation of a single/dual channel FIR filter backend.
3.fir.sv: Handles and connects the AXI stream to FIR filter backend
4.filter_gen.m: MATLAB/Octave script to generate hexadecimal coefficients for a desired FIR filter
5.single_channel_fir_engine_tb.sv and dual_channel_fir_engine_tb.sv: Testbenches for testing the FIR filter backend implementations.

Conclusion:
This project demonstrates the ability to implement real-time audio processing using FIR filters on a Basys-3 FPGA board and a Pmod I2S2 digital audio interface. The provided files and instructions should provide a starting point for further experimentation and customization of the audio processing capabilities.
