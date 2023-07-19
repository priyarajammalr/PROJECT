# PROJECT - FPGA REALIZATION OF FFT COMPUTATION

The Fast Fourier Transform (FFT) is a fundamental building block used in DSP
systems, with applications ranging from OFDM based Digital MODEMs, to
Ultrasound, RADAR and CT Image reconstruction algorithms. It is a fast
algorithm to compute DFT as it reduces the calculation complexity from the
order of N2 in DFT to Nlog2N, where N is the number of sample points. The
Verilog implementation of FFT includes complex numbers addition and
multiplication due to twiddle factor. In this paper, FPGA implementation of
maximum 1024-point DIT radix-2 FFT using fixed-point arithmetic has been
presented. The frequency resolution is also computed. The designed FFT can be
used in scientific computations since it requires less power and operates in high
speed. The DE0-Nano board is used as a hardware to implement the complex
FFT values.

# Tools and Software Used

Intel Quartus Prime Lite(for implementing the design in the board)
DE0-Nano – Altera Cyclone IV FPGA Board 
MATLAB(for verifying the results of FFT)

# FFT IP CORE

The Quartus has an inbuilt FFT Core in IP Catalog. The FFT IP core is a high
performance, highly-parameterizable FFT processor. The FFT IP core
implements a complex FFT or inverse FFT (IFFT) for high-performance
applications. The length or size of FFT is chosen as 1024, data flow is chosen as
variable streaming that uses fixed point representation. The input data width is 12
bits. The output width of the FFT is 23 bits. The twiddle factor occupies 18 bits.

# Block Diagram

![image](https://github.com/priyarajammalr/PROJECT/assets/115354310/b003f618-7cff-4648-928d-a8b253ca9560)




