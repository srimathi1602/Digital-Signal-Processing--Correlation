# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 

clc; % clear screen
 clear all; % clear screen
 close all; % close all figure windows
% INPUT SIGNAL-1
x=input('Enter the x(n) sequence')
n=0:1:length(x)-1
figure(1)
stem(x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')
% INPUT SIGNAL 2
y=input('Enter the y(n) sequence')
n1=0: 1:length(y)-1
figure(2)
stem(y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')
% DISCRETE AUTO CORRELATED SIGNAL
out1=xcorr(x,x)
figure(3)
stem(out1)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete auto correlated waveform')
% DISCRETE CROSS CORRELATED SIGNAL
Out2=xcorr(x,y)
figure(4)
stem(out2)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete cross correlated waveform')
```

## OUTPUT:

<img width="1280" height="681" alt="image" src="https://github.com/user-attachments/assets/086034b0-af4c-4fb0-a15f-44506765570a" />


## RESULT:

<img width="1280" height="792" alt="image" src="https://github.com/user-attachments/assets/0b7b2392-175b-4939-ace1-09bdb97288d4" />


