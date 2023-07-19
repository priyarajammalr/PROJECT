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

