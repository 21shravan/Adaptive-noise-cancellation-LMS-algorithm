# Adaptive-noise-cancellation-LMS-algorithm
A MATLAB project demonstrating Least Mean Squares adaptive filtering to suppress correlated noise in audio signals.

## Overview

This project explores adaptive noise cancellation using a primary audio signal containing both the desired audio and unwanted noise, alongside a reference noise signal correlated with the interference.

The LMS algorithm adaptively estimates the noise component and subtracts it from the primary input to produce a noise-reduced output.

## Objectives

- Implement an LMS adaptive FIR filter in MATLAB.
- Study the effect of the adaptation step size on filter performance.
- Analyze clean, noisy, and filtered audio in the time and frequency domains.

## System Architecture

1. Import the desired audio and reference noise.
2. Generate a noise-corrupted primary signal.
3. Feed the primary signal and reference noise into the adaptive filter.
4. Update filter coefficients iteratively using the LMS algorithm.
5. Analyze and listen to the noise-reduced output.

## Algorithm

The LMS algorithm updates the filter coefficients iteratively:

$$[
y(n)=\mathbf{w}^{T}(n)\mathbf{x}(n)
]$$

$$\[
e(n)=d(n)-y(n)
\]$$

$$\[
\mathbf{w}(n+1)=\mathbf{w}(n)+\mu e(n)\mathbf{x}(n)
\]$$

where $\(d(n)\)$ is the primary input, $\(\mathbf{x}(n)\$) is the reference input vector, $\(\mathbf{w}(n)\$) is the adaptive coefficient vector, $\(\mu\$) is the step size, and $\(e(n)\$) is the residual error.

## Tools and Technologies

- MATLAB
- Digital Signal Processing
- Adaptive FIR Filtering
- LMS Algorithm
- Audio Signal Analysis<img width="442" height="204" alt="Block_Diagram" src="https://github.com/user-attachments/assets/c91f694b-03d5-4499-a278-14e28c6173f0" />


## Running the Project

1. Clone or download this repository.
2. Open the MATLAB project files.
3. Add the MATLAB source directory to the MATLAB path.
4. Load the audio and reference noise files.
5. Run the main script or launch the GUI.
6. Adjust the step size and compare the input and filtered outputs.

Update the script and GUI filenames in these instructions to match the files included in the repository.

## Current Scope and Future Work

The current implementation focuses on MATLAB simulation and offline audio processing. Future work includes real-time noise cancellation using two microphones and deployment on a microcontroller, DSP platform, or laptop audio interface.

## Author

Add your name, team members, and project affiliation here.
