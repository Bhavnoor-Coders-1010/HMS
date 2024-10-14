# HMS
The repo contains an ipynb file with the code for Harmful Brain Acivity Classification

The dataset has been taken from the kaggle competition: hms-harmful-brain-activity-classification

The preprocessing techniques involved are:

1) Passing through a low pass filter with cutoff frequency = 30Hz becuase the data is recorded using EEG electrodes which can at max record frequencies upto 30Hz, therefore, anything above that frequency is assumed to be noise.
2) Taking Continuous Wavelet Transform of the signal of interest ,which is a way to recreate the signal in both the frequency and time domain, using that in image format to feed to a CNN as input for classifier training.
