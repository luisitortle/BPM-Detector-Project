# BPM Detector

A simple Jupyter Notebook that estimates the tempo (Beats Per Minute).
---

# Overview

This notebook reads an audio file (`.wav`), processes the signal by partitioning it and computing the norms of differences, then uses a frequency analysis approach (via FFT) to estimate the BPM.

---

# What It Does

- ✅ Loads a WAV audio file using `scipy.io.wavfile`
- ✅ Ensures the signal is mono by selecting one channel if needed
- ✅ Computes the frequency resolution based on the sample rate and signal length
- ✅ Partitions the signal into equal-sized chunks
- ✅ Calculates the norm of the difference in each partition.
- ✅ Applies FFT to analyze periodicity in the norms
- ✅ Prepares a BPM axis and plots the signal spectrum versus BPM
