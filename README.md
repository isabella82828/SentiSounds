# SentiSounds
## Project Overview 
This project aims to develop a machine learning model capable of detecting emotions from speech, enhancing personalization in various applications. By analyzing vocal expressions, the model can infer emotional states. 

## Datasets
Two primary datasets were used: 
1. RAVDESS: Comprising approximately 1,500 audio files from 24 actors
2. SAVEE: Containing around 500 audio files from four male actors

## Audio Analysis
To understand the audio data, waveforms and spectrograms were plotted for sample files, providing visual insights into the characteristics of different emotions.

## Feature Extraction 
Utilizing Python's LibROSA library, features were extracted from the audio files to facilitate model training. Key considerations included:

- Uniform Duration: All audio clips were standardized to 3 seconds to ensure consistent feature extraction.
- Increased Sampling Rate: Doubling the sampling rate, while maintaining a constant sampling frequency, provided more detailed features, beneficial for smaller datasets.

The resulting feature arrays, each labeled with the corresponding emotion, served as input for model training.

## Model Development 
A Convolutional Neural Network (CNN) was employed, while zlternative models, such as Multilayer Perceptrons (MLPs) and Long Short-Term Memory (LSTM) networks, were also tested but yielded lower accuracies.

The model effectively distinguishes between male and female voices with 100% accuracy and identifies emotions with over 70% accuracy. 
