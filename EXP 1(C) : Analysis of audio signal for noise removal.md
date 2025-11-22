# EXP 1(C) : Analysis of audio signal for noise removal

# AIM: 

# To analyse an audio signal and remove noise

# APPARATUS REQUIRED:  
PC installed with SCILAB. 

# PROGRAM: 
// DISCRETE FOURIER TRANSFORM 
```c
[x, fs] = wavread("D:\\SEM-3\\DTSP\\Exps\\1C\\input.wav");

// Remove first 2 seconds
cut_samples = round(2 * fs);
y = x(cut_samples+1:$);

// Play original
disp("Playing Original...");
playsnd(x, fs);

// Play trimmed audio
disp("Playing Audio without first 2s...");
playsnd(y, fs);

// Save the trimmed audio
wavwrite(y, fs, "D:\\SEM-3\\DTSP\\Exps\\1C\\filtered
.wav");

```

# RESULT: 

Analysis of audio signal for noise removal was removed successfully.
