# Noise Reduction Using Fourier Transform

## Project Overview

This project was developed in **2022** as part of my **TIPE** (Épreuve d'Évaluation des Travaux d'Initiative Personnelle Encadrés). The objective of the project is to reduce noise in urban environments using signal processing techniques, particularly the **Fourier Transform**. The main idea is to generate a **secondary sound signal** that opposes the primary noise signal, causing **destructive interference** and effectively reducing the perceived noise.

### Problem Statement

Noise pollution is a significant issue in modern cities. Various methods have been developed to mitigate its effects, one of which is **Active Noise Control** (ANC). This technique involves generating sound waves that interfere destructively with the unwanted noise, thereby reducing its overall amplitude. In this project, we explore the use of the **Fourier Transform** to analyze and decompose the primary noise signal into its frequency components and create an inverse signal to cancel out the noise.

### Key Concepts

1. **Fourier Transform**:
   - The Fourier Transform is a mathematical tool that decomposes a time-domain signal into its frequency components. This allows us to analyze the frequency spectrum of the noise and design a counteracting signal.
   
2. **Destructive Interference**:
   - In wave physics, destructive interference occurs when two waves of equal amplitude and opposite phase meet. The result is that the waves cancel each other out, which leads to a reduction in the total amplitude.

3. **Active Noise Control (ANC)**:
   - ANC is a technique used to reduce unwanted sound by generating a sound wave with the same amplitude but opposite phase to the original noise. The two waves interfere destructively, reducing the overall sound level.

### Project Implementation

The project is implemented in **Python** using the following key libraries:
- **NumPy**: For performing the **Fast Fourier Transform (FFT)** and handling numerical computations.
- **Matplotlib**: For visualizing the results, including frequency spectra and signal waveforms.
- **SoundDevice**: For recording and playing sound signals in real-time.

### Process

1. **Capturing the Noise Signal**: 
   - The noise signal is captured using a microphone and processed in real-time.
   
2. **Applying Fourier Transform**:
   - The **Fourier Transform** is applied to decompose the signal into its constituent frequencies.
   
3. **Generating the Inverse Signal**:
   - The inverse of the primary signal is generated, which should cancel out the noise via **destructive interference**.
   
4. **Combining the Signals**:
   - The primary and inverse signals are combined, and their sum should show a significant reduction in noise amplitude.

### Results

Through the application of the Fourier Transform, we can visualize the frequency spectrum of the original signal, the inverse signal, and the sum of both. The goal is to demonstrate that the summed signals interfere destructively, reducing the overall noise level.

Below is an example of the frequency spectrum before and after applying the noise cancellation technique:

- **Captured Signal Spectrum**: Shows the frequency components of the captured noise.
- **Inverse Signal Spectrum**: The frequency spectrum of the generated signal that interferes destructively with the original noise.
- **Combined Signal Spectrum**: The result of adding the captured signal and the inverse signal, which shows the reduced amplitude due to destructive interference.

## Author
ALOUI Ghaieth, POLYTECH Nice Sophia - Université Côte d'Azur 

This project was part of my **TIPE**, a personal research project aimed at deepening my understanding of signal processing, noise reduction, and the Fourier Transform. It reflects my passion for applying theoretical knowledge to real-world problems, specifically in the domain of urban noise pollution.

Feel free to reach out for questions or collaboration opportunities:

- GitHub: (https://github.com/ghaieth11)
- Email: ghaieth.aloui@etu.univ-cotedazur.fr
