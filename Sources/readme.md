# FFT IP CORE

![image](https://github.com/priyarajammalr/PROJECT/assets/115354310/af994a55-aa82-4d73-9591-c0bd1ce44883)


# FFT CONTROL BLOCK

The streaming FFT allows continuous processing of input data and outputs a continuous complex data stream without the need to halt the data flow in or out of the FFT IP core.The data source asserts sink_valid to indicate to the FFT function that valid data is available for input.To generate sink_valid,sink_sop and sink_eop, we create a control_for_fft block.After some clock cycles,the IP core outputs source_sop and source_eop,source_valid to denote about the result availability to downstream module.

![image](https://github.com/priyarajammalr/PROJECT/assets/115354310/d989793f-c125-43bd-8a85-650692b0ad0c)




# FFT WRAPPER

We instantiate the FFT IP Core and control_for_fft blocks in a single block ‘fft_wrapper’

# ROM

A 2kb-ROM is available in the DE0 Nano Board.To store and access values in this ROM we used ROM IP available in the IP Catalog.This ROM has 10 address lines, 12 bits for output and 1024 words. The 1024 words are entered in a .mif (Memory Initialization File). These values which are sine values are generated in MATLAB.(The matlab code is also provided).Here the values are shifted up by 1 and scaled by 1000 to avoid negative values and floating point numbers. In the .mif file we have the 1024 values stored as hexadecimal.

![image](https://github.com/priyarajammalr/PROJECT/assets/115354310/568b3547-a4f6-41d3-93a5-04badd6b672b)


# COUNTER

The 10 address lines input to ROM is given using a 10-bit counter.
