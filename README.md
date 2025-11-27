# AUTO-CORRELATION-AND-PSD

# Aim
Write a program for Autocorrelation and Power Spectral Density (PSD) of signals in Scilab and verify the Wiener–Khinchin relation.

# Equipments Needed:

i.Computer with Intel i3 processor (or higher)
ii.Scilab software


# Theory:

The Wiener–Khinchin theorem states that:
The Power Spectral Density (PSD) of a wide-sense stationary random process is the Fourier Transform of its autocorrelation function.

<img width="466" height="74" alt="507396276-f7c7673b-e086-4231-b8b4-4a677a3f7d0c" src="https://github.com/user-attachments/assets/684b85a3-6849-45c5-b0b2-f4147a68b7d8" />

This relationship bridges the time-domain correlation and frequency-domain power representations of a signal.


# Algorithm

Load or Define the Signal: Input your time-domain signal.

Compute Autocorrelation: Calculate the autocorrelation function of the signal.

Compute Power Spectral Density (PSD):

Estimate the PSD using either:

Fourier Transform of the autocorrelation function, or

Methods like Welch’s periodogram.

Plot Results: Visualize both the autocorrelation function and PSD.

# Procedure

Refer to the algorithm and write the code for the experiment.

Open Scilab on your system.

Type your code in a new editor.

Save the file.

Execute the code.

If any errors occur, debug and re-run the program.

Verify the generated waveform using tabulation and model waveform comparison.

# Program (Scilab Code)

```asm
t=0:0.01:2*3.14;
x=cos(2.5*t);
subplot(3,2,1);
plot(x); 
au=xcorr(x,x); 
subplot(3,2,2);
plot(au);
v=fft(au); 
subplot(3,2,3);
plot(abs(v));
fw=fft(x);
subplot(3,2,4);
plot(fw);
fw2=(abs(fw)).^2;
subplot(3,2,5);
plot(fw2);
```

# Output:

<img width="774" height="730" alt="Screenshot 2025-11-27 103722" src="https://github.com/user-attachments/assets/fb9b086e-4b9a-450b-b279-9a47be67fdad" />

# Result:

Thus the Autocorrelation and PSD are executed in Scilab and output is verified.
