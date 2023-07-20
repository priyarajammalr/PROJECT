# RESULTS

The SignalTap Logic Analyzer Editor allows us to debug the design in real-time and at high-speed while performing an analysis in the Quartus software.Using Signal Tap logic Analyzer, the outputs from the respective data output blocks can be captured and analysed. The output as viewed from the signal tap analyser is given below
![image](https://github.com/priyarajammalr/PROJECT/assets/115354310/3a0536b4-0228-40b6-af5c-da04bbc2dda6)

The diagrams below indicate the enabled sink_sop. This activation of sink_sop signifies the incoming data packets(i.e)the input signal.

![image](https://github.com/priyarajammalr/PROJECT/assets/115354310/944d6120-9231-4f70-baa5-4cea5deb0611)

The activation of the source_sop is shown below. This indicates the start of FFT points being displayed (both real and imaginary values).

![image](https://github.com/priyarajammalr/PROJECT/assets/115354310/7b820775-ab9d-4237-bcf5-6f04e3cc8e47)

The FFT points from the signal tap output (the real and imaginary values) are exported and using MATLAB, the IFFT of the output points are found and the result is plotted. The Matlab code used for reconstruction is as follows:

![image](https://github.com/priyarajammalr/PROJECT/assets/115354310/7e038280-938c-4c34-8843-92520b7af481)

The input sine wave whose Fast Fourier Transform was realized using Quartus is approximately reconstructed at the output side using the Inverse Fast Fourier Transform.To verify the results,we need to find the resolution(bin size of FFT)from the reconstructed sine wave's frequency domain plot.

![image](https://github.com/priyarajammalr/PROJECT/assets/115354310/12f85f49-86b3-466b-88a7-f8f3ce7558db)

Frequency Resolution(Theoretical) = Sampling rate/FFT Size = 200MHz/1024 = 195312.5Hz 
Frequency Resolution(Practical) From the Frequency plot = 195312 Hz

